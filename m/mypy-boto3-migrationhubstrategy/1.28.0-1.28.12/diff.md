# Comparing `tmp/mypy-boto3-migrationhubstrategy-1.28.0.tar.gz` & `tmp/mypy-boto3-migrationhubstrategy-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhubstrategy-1.28.0.tar", last modified: Thu Jul  6 21:00:11 2023, max compression
+gzip compressed data, was "mypy-boto3-migrationhubstrategy-1.28.12.tar", last modified: Thu Jul 27 05:35:04 2023, max compression
```

## Comparing `mypy-boto3-migrationhubstrategy-1.28.0.tar` & `mypy-boto3-migrationhubstrategy-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.026377 mypy-boto3-migrationhubstrategy-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18853 2023-07-06 21:00:11.026377 mypy-boto3-migrationhubstrategy-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17301 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.018377 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20755 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31754 2023-07-06 20:47:51.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31743 2023-07-06 20:47:51.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.026377 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18853 2023-07-06 21:00:10.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-06 21:00:10.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:10.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:10.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:10.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 21:00:10.000000 mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:11.026377 mypy-boto3-migrationhubstrategy-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-06 20:47:50.000000 mypy-boto3-migrationhubstrategy-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.120430 mypy-boto3-migrationhubstrategy-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-07-27 05:35:04.120430 mypy-boto3-migrationhubstrategy-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17786 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.116430 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20755 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-07-27 05:26:43.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-07-27 05:26:43.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-07-27 05:26:45.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35110 2023-07-27 05:26:45.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.120430 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-07-27 05:35:03.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:35:03.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:03.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 05:35:03.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:04.120430 mypy-boto3-migrationhubstrategy-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/setup.py
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/LICENSE` & `mypy-boto3-migrationhubstrategy-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/PKG-INFO` & `mypy-boto3-migrationhubstrategy-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhubstrategy
-Version: 1.28.0
-Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-migrationhubstrategy"></a>
 
 # mypy-boto3-migrationhubstrategy
 
 [![PyPI - mypy-boto3-migrationhubstrategy](https://img.shields.io/pypi/v/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhubstrategy?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhubstrategy)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhubstrategy)](https://pepy.tech/project/mypy-boto3-migrationhubstrategy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubStrategyRecommendations 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
+[boto3.MigrationHubStrategyRecommendations 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -394,24 +394,30 @@
     DatabaseConfigDetailTypeDef,
     SourceCodeRepositoryTypeDef,
     ApplicationComponentStatusSummaryTypeDef,
     ApplicationComponentSummaryTypeDef,
     ServerStatusSummaryTypeDef,
     ServerSummaryTypeDef,
     StrategySummaryTypeDef,
+    AssessmentTargetOutputTypeDef,
     AssessmentTargetTypeDef,
     AssociatedApplicationTypeDef,
+    AwsManagedResourcesOutputTypeDef,
     AwsManagedResourcesTypeDef,
+    BusinessGoalsOutputTypeDef,
     BusinessGoalsTypeDef,
     IPAddressBasedRemoteInfoTypeDef,
     PipelineInfoTypeDef,
     RemoteSourceCodeAnalysisServerInfoTypeDef,
     VcenterBasedRemoteInfoTypeDef,
     VersionControlInfoTypeDef,
     DataCollectionDetailsTypeDef,
+    HeterogeneousOutputTypeDef,
+    HomogeneousOutputTypeDef,
+    NoDatabaseMigrationPreferenceOutputTypeDef,
     HeterogeneousTypeDef,
     HomogeneousTypeDef,
     NoDatabaseMigrationPreferenceTypeDef,
     GetApplicationComponentDetailsRequestRequestTypeDef,
     GetApplicationComponentStrategiesRequestRequestTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetImportFileTaskRequestRequestTypeDef,
@@ -424,14 +430,16 @@
     GetServerStrategiesRequestRequestTypeDef,
     GroupTypeDef,
     ImportFileTaskInformationTypeDef,
     ListCollectorsRequestListCollectorsPaginateTypeDef,
     ListCollectorsRequestRequestTypeDef,
     ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListImportFileTaskRequestRequestTypeDef,
+    NoManagementPreferenceOutputTypeDef,
+    SelfManageResourcesOutputTypeDef,
     NoManagementPreferenceTypeDef,
     SelfManageResourcesTypeDef,
     NetworkInfoTypeDef,
     OSInfoTypeDef,
     PaginatorConfigTypeDef,
     TransformationToolTypeDef,
     ResponseMetadataTypeDef,
@@ -441,35 +449,40 @@
     StartImportFileTaskResponseTypeDef,
     StartRecommendationReportGenerationResponseTypeDef,
     StopAssessmentRequestRequestTypeDef,
     StrategyOptionTypeDef,
     AntipatternReportResultTypeDef,
     AssessmentSummaryTypeDef,
     StartAssessmentRequestRequestTypeDef,
+    PrioritizeBusinessGoalsOutputTypeDef,
     PrioritizeBusinessGoalsTypeDef,
     ConfigurationSummaryTypeDef,
     GetAssessmentResponseTypeDef,
+    DatabaseMigrationPreferenceOutputTypeDef,
     DatabaseMigrationPreferenceTypeDef,
     GetRecommendationReportDetailsResponseTypeDef,
     ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef,
     ListApplicationComponentsRequestRequestTypeDef,
     ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     StartImportFileTaskRequestRequestTypeDef,
     StartRecommendationReportGenerationRequestRequestTypeDef,
     ListImportFileTaskResponseTypeDef,
+    ManagementPreferenceOutputTypeDef,
     ManagementPreferenceTypeDef,
     SystemInfoTypeDef,
     RecommendationSetTypeDef,
     UpdateApplicationComponentConfigRequestRequestTypeDef,
     UpdateServerConfigRequestRequestTypeDef,
     ResultTypeDef,
     GetPortfolioSummaryResponseTypeDef,
     CollectorTypeDef,
+    DatabasePreferencesOutputTypeDef,
     DatabasePreferencesTypeDef,
+    ApplicationPreferencesOutputTypeDef,
     ApplicationPreferencesTypeDef,
     ApplicationComponentStrategyTypeDef,
     ServerDetailTypeDef,
     ServerStrategyTypeDef,
     ApplicationComponentDetailTypeDef,
     ListCollectorsResponseTypeDef,
     GetPortfolioPreferencesResponseTypeDef,
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/README.md` & `mypy-boto3-migrationhubstrategy-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-migrationhubstrategy"></a>
 
 # mypy-boto3-migrationhubstrategy
 
 [![PyPI - mypy-boto3-migrationhubstrategy](https://img.shields.io/pypi/v/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhubstrategy?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhubstrategy)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhubstrategy)](https://pepy.tech/project/mypy-boto3-migrationhubstrategy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubStrategyRecommendations 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
+[boto3.MigrationHubStrategyRecommendations 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,24 +362,30 @@
     DatabaseConfigDetailTypeDef,
     SourceCodeRepositoryTypeDef,
     ApplicationComponentStatusSummaryTypeDef,
     ApplicationComponentSummaryTypeDef,
     ServerStatusSummaryTypeDef,
     ServerSummaryTypeDef,
     StrategySummaryTypeDef,
+    AssessmentTargetOutputTypeDef,
     AssessmentTargetTypeDef,
     AssociatedApplicationTypeDef,
+    AwsManagedResourcesOutputTypeDef,
     AwsManagedResourcesTypeDef,
+    BusinessGoalsOutputTypeDef,
     BusinessGoalsTypeDef,
     IPAddressBasedRemoteInfoTypeDef,
     PipelineInfoTypeDef,
     RemoteSourceCodeAnalysisServerInfoTypeDef,
     VcenterBasedRemoteInfoTypeDef,
     VersionControlInfoTypeDef,
     DataCollectionDetailsTypeDef,
+    HeterogeneousOutputTypeDef,
+    HomogeneousOutputTypeDef,
+    NoDatabaseMigrationPreferenceOutputTypeDef,
     HeterogeneousTypeDef,
     HomogeneousTypeDef,
     NoDatabaseMigrationPreferenceTypeDef,
     GetApplicationComponentDetailsRequestRequestTypeDef,
     GetApplicationComponentStrategiesRequestRequestTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetImportFileTaskRequestRequestTypeDef,
@@ -392,14 +398,16 @@
     GetServerStrategiesRequestRequestTypeDef,
     GroupTypeDef,
     ImportFileTaskInformationTypeDef,
     ListCollectorsRequestListCollectorsPaginateTypeDef,
     ListCollectorsRequestRequestTypeDef,
     ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListImportFileTaskRequestRequestTypeDef,
+    NoManagementPreferenceOutputTypeDef,
+    SelfManageResourcesOutputTypeDef,
     NoManagementPreferenceTypeDef,
     SelfManageResourcesTypeDef,
     NetworkInfoTypeDef,
     OSInfoTypeDef,
     PaginatorConfigTypeDef,
     TransformationToolTypeDef,
     ResponseMetadataTypeDef,
@@ -409,35 +417,40 @@
     StartImportFileTaskResponseTypeDef,
     StartRecommendationReportGenerationResponseTypeDef,
     StopAssessmentRequestRequestTypeDef,
     StrategyOptionTypeDef,
     AntipatternReportResultTypeDef,
     AssessmentSummaryTypeDef,
     StartAssessmentRequestRequestTypeDef,
+    PrioritizeBusinessGoalsOutputTypeDef,
     PrioritizeBusinessGoalsTypeDef,
     ConfigurationSummaryTypeDef,
     GetAssessmentResponseTypeDef,
+    DatabaseMigrationPreferenceOutputTypeDef,
     DatabaseMigrationPreferenceTypeDef,
     GetRecommendationReportDetailsResponseTypeDef,
     ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef,
     ListApplicationComponentsRequestRequestTypeDef,
     ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     StartImportFileTaskRequestRequestTypeDef,
     StartRecommendationReportGenerationRequestRequestTypeDef,
     ListImportFileTaskResponseTypeDef,
+    ManagementPreferenceOutputTypeDef,
     ManagementPreferenceTypeDef,
     SystemInfoTypeDef,
     RecommendationSetTypeDef,
     UpdateApplicationComponentConfigRequestRequestTypeDef,
     UpdateServerConfigRequestRequestTypeDef,
     ResultTypeDef,
     GetPortfolioSummaryResponseTypeDef,
     CollectorTypeDef,
+    DatabasePreferencesOutputTypeDef,
     DatabasePreferencesTypeDef,
+    ApplicationPreferencesOutputTypeDef,
     ApplicationPreferencesTypeDef,
     ApplicationComponentStrategyTypeDef,
     ServerDetailTypeDef,
     ServerStrategyTypeDef,
     ApplicationComponentDetailTypeDef,
     ListCollectorsResponseTypeDef,
     GetPortfolioPreferencesResponseTypeDef,
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/__init__.py` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/__init__.pyi` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/__main__.py` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations\nOther"
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

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/client.py` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/client.pyi` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/literals.py` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,14 +385,15 @@
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
@@ -471,26 +472,28 @@
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

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/literals.pyi` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -383,14 +383,15 @@
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
@@ -469,26 +470,28 @@
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

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/paginator.py` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/paginator.pyi` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/type_defs.py` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,24 +78,30 @@
     "DatabaseConfigDetailTypeDef",
     "SourceCodeRepositoryTypeDef",
     "ApplicationComponentStatusSummaryTypeDef",
     "ApplicationComponentSummaryTypeDef",
     "ServerStatusSummaryTypeDef",
     "ServerSummaryTypeDef",
     "StrategySummaryTypeDef",
+    "AssessmentTargetOutputTypeDef",
     "AssessmentTargetTypeDef",
     "AssociatedApplicationTypeDef",
+    "AwsManagedResourcesOutputTypeDef",
     "AwsManagedResourcesTypeDef",
+    "BusinessGoalsOutputTypeDef",
     "BusinessGoalsTypeDef",
     "IPAddressBasedRemoteInfoTypeDef",
     "PipelineInfoTypeDef",
     "RemoteSourceCodeAnalysisServerInfoTypeDef",
     "VcenterBasedRemoteInfoTypeDef",
     "VersionControlInfoTypeDef",
     "DataCollectionDetailsTypeDef",
+    "HeterogeneousOutputTypeDef",
+    "HomogeneousOutputTypeDef",
+    "NoDatabaseMigrationPreferenceOutputTypeDef",
     "HeterogeneousTypeDef",
     "HomogeneousTypeDef",
     "NoDatabaseMigrationPreferenceTypeDef",
     "GetApplicationComponentDetailsRequestRequestTypeDef",
     "GetApplicationComponentStrategiesRequestRequestTypeDef",
     "GetAssessmentRequestRequestTypeDef",
     "GetImportFileTaskRequestRequestTypeDef",
@@ -108,14 +114,16 @@
     "GetServerStrategiesRequestRequestTypeDef",
     "GroupTypeDef",
     "ImportFileTaskInformationTypeDef",
     "ListCollectorsRequestListCollectorsPaginateTypeDef",
     "ListCollectorsRequestRequestTypeDef",
     "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
     "ListImportFileTaskRequestRequestTypeDef",
+    "NoManagementPreferenceOutputTypeDef",
+    "SelfManageResourcesOutputTypeDef",
     "NoManagementPreferenceTypeDef",
     "SelfManageResourcesTypeDef",
     "NetworkInfoTypeDef",
     "OSInfoTypeDef",
     "PaginatorConfigTypeDef",
     "TransformationToolTypeDef",
     "ResponseMetadataTypeDef",
@@ -125,35 +133,40 @@
     "StartImportFileTaskResponseTypeDef",
     "StartRecommendationReportGenerationResponseTypeDef",
     "StopAssessmentRequestRequestTypeDef",
     "StrategyOptionTypeDef",
     "AntipatternReportResultTypeDef",
     "AssessmentSummaryTypeDef",
     "StartAssessmentRequestRequestTypeDef",
+    "PrioritizeBusinessGoalsOutputTypeDef",
     "PrioritizeBusinessGoalsTypeDef",
     "ConfigurationSummaryTypeDef",
     "GetAssessmentResponseTypeDef",
+    "DatabaseMigrationPreferenceOutputTypeDef",
     "DatabaseMigrationPreferenceTypeDef",
     "GetRecommendationReportDetailsResponseTypeDef",
     "ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef",
     "ListApplicationComponentsRequestRequestTypeDef",
     "ListServersRequestListServersPaginateTypeDef",
     "ListServersRequestRequestTypeDef",
     "StartImportFileTaskRequestRequestTypeDef",
     "StartRecommendationReportGenerationRequestRequestTypeDef",
     "ListImportFileTaskResponseTypeDef",
+    "ManagementPreferenceOutputTypeDef",
     "ManagementPreferenceTypeDef",
     "SystemInfoTypeDef",
     "RecommendationSetTypeDef",
     "UpdateApplicationComponentConfigRequestRequestTypeDef",
     "UpdateServerConfigRequestRequestTypeDef",
     "ResultTypeDef",
     "GetPortfolioSummaryResponseTypeDef",
     "CollectorTypeDef",
+    "DatabasePreferencesOutputTypeDef",
     "DatabasePreferencesTypeDef",
+    "ApplicationPreferencesOutputTypeDef",
     "ApplicationPreferencesTypeDef",
     "ApplicationComponentStrategyTypeDef",
     "ServerDetailTypeDef",
     "ServerStrategyTypeDef",
     "ApplicationComponentDetailTypeDef",
     "ListCollectorsResponseTypeDef",
     "GetPortfolioPreferencesResponseTypeDef",
@@ -271,37 +284,64 @@
     {
         "count": int,
         "strategy": StrategyType,
     },
     total=False,
 )
 
+AssessmentTargetOutputTypeDef = TypedDict(
+    "AssessmentTargetOutputTypeDef",
+    {
+        "condition": ConditionType,
+        "name": str,
+        "values": List[str],
+    },
+)
+
 AssessmentTargetTypeDef = TypedDict(
     "AssessmentTargetTypeDef",
     {
         "condition": ConditionType,
         "name": str,
-        "values": List[str],
+        "values": Sequence[str],
     },
 )
 
 AssociatedApplicationTypeDef = TypedDict(
     "AssociatedApplicationTypeDef",
     {
         "id": str,
         "name": str,
     },
     total=False,
 )
 
+AwsManagedResourcesOutputTypeDef = TypedDict(
+    "AwsManagedResourcesOutputTypeDef",
+    {
+        "targetDestination": List[AwsManagedTargetDestinationType],
+    },
+)
+
 AwsManagedResourcesTypeDef = TypedDict(
     "AwsManagedResourcesTypeDef",
     {
-        "targetDestination": List[AwsManagedTargetDestinationType],
+        "targetDestination": Sequence[AwsManagedTargetDestinationType],
+    },
+)
+
+BusinessGoalsOutputTypeDef = TypedDict(
+    "BusinessGoalsOutputTypeDef",
+    {
+        "licenseCostReduction": int,
+        "modernizeInfrastructureWithCloudNativeTechnologies": int,
+        "reduceOperationalOverheadWithManagedServices": int,
+        "speedOfMigration": int,
     },
+    total=False,
 )
 
 BusinessGoalsTypeDef = TypedDict(
     "BusinessGoalsTypeDef",
     {
         "licenseCostReduction": int,
         "modernizeInfrastructureWithCloudNativeTechnologies": int,
@@ -367,33 +407,55 @@
         "status": AssessmentStatusType,
         "statusMessage": str,
         "success": int,
     },
     total=False,
 )
 
+HeterogeneousOutputTypeDef = TypedDict(
+    "HeterogeneousOutputTypeDef",
+    {
+        "targetDatabaseEngine": List[HeterogeneousTargetDatabaseEngineType],
+    },
+)
+
+HomogeneousOutputTypeDef = TypedDict(
+    "HomogeneousOutputTypeDef",
+    {
+        "targetDatabaseEngine": List[Literal["None specified"]],
+    },
+    total=False,
+)
+
+NoDatabaseMigrationPreferenceOutputTypeDef = TypedDict(
+    "NoDatabaseMigrationPreferenceOutputTypeDef",
+    {
+        "targetDatabaseEngine": List[TargetDatabaseEngineType],
+    },
+)
+
 HeterogeneousTypeDef = TypedDict(
     "HeterogeneousTypeDef",
     {
-        "targetDatabaseEngine": List[HeterogeneousTargetDatabaseEngineType],
+        "targetDatabaseEngine": Sequence[HeterogeneousTargetDatabaseEngineType],
     },
 )
 
 HomogeneousTypeDef = TypedDict(
     "HomogeneousTypeDef",
     {
-        "targetDatabaseEngine": List[Literal["None specified"]],
+        "targetDatabaseEngine": Sequence[Literal["None specified"]],
     },
     total=False,
 )
 
 NoDatabaseMigrationPreferenceTypeDef = TypedDict(
     "NoDatabaseMigrationPreferenceTypeDef",
     {
-        "targetDatabaseEngine": List[TargetDatabaseEngineType],
+        "targetDatabaseEngine": Sequence[TargetDatabaseEngineType],
     },
 )
 
 GetApplicationComponentDetailsRequestRequestTypeDef = TypedDict(
     "GetApplicationComponentDetailsRequestRequestTypeDef",
     {
         "applicationComponentId": str,
@@ -575,25 +637,39 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+NoManagementPreferenceOutputTypeDef = TypedDict(
+    "NoManagementPreferenceOutputTypeDef",
+    {
+        "targetDestination": List[NoPreferenceTargetDestinationType],
+    },
+)
+
+SelfManageResourcesOutputTypeDef = TypedDict(
+    "SelfManageResourcesOutputTypeDef",
+    {
+        "targetDestination": List[SelfManageTargetDestinationType],
+    },
+)
+
 NoManagementPreferenceTypeDef = TypedDict(
     "NoManagementPreferenceTypeDef",
     {
-        "targetDestination": List[NoPreferenceTargetDestinationType],
+        "targetDestination": Sequence[NoPreferenceTargetDestinationType],
     },
 )
 
 SelfManageResourcesTypeDef = TypedDict(
     "SelfManageResourcesTypeDef",
     {
-        "targetDestination": List[SelfManageTargetDestinationType],
+        "targetDestination": Sequence[SelfManageTargetDestinationType],
     },
 )
 
 NetworkInfoTypeDef = TypedDict(
     "NetworkInfoTypeDef",
     {
         "interfaceName": str,
@@ -739,14 +815,22 @@
         "assessmentTargets": Sequence[AssessmentTargetTypeDef],
         "s3bucketForAnalysisData": str,
         "s3bucketForReportData": str,
     },
     total=False,
 )
 
+PrioritizeBusinessGoalsOutputTypeDef = TypedDict(
+    "PrioritizeBusinessGoalsOutputTypeDef",
+    {
+        "businessGoals": BusinessGoalsOutputTypeDef,
+    },
+    total=False,
+)
+
 PrioritizeBusinessGoalsTypeDef = TypedDict(
     "PrioritizeBusinessGoalsTypeDef",
     {
         "businessGoals": BusinessGoalsTypeDef,
     },
     total=False,
 )
@@ -762,21 +846,31 @@
     },
     total=False,
 )
 
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
-        "assessmentTargets": List[AssessmentTargetTypeDef],
+        "assessmentTargets": List[AssessmentTargetOutputTypeDef],
         "dataCollectionDetails": DataCollectionDetailsTypeDef,
         "id": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DatabaseMigrationPreferenceOutputTypeDef = TypedDict(
+    "DatabaseMigrationPreferenceOutputTypeDef",
+    {
+        "heterogeneous": HeterogeneousOutputTypeDef,
+        "homogeneous": HomogeneousOutputTypeDef,
+        "noPreference": NoDatabaseMigrationPreferenceOutputTypeDef,
+    },
+    total=False,
+)
+
 DatabaseMigrationPreferenceTypeDef = TypedDict(
     "DatabaseMigrationPreferenceTypeDef",
     {
         "heterogeneous": HeterogeneousTypeDef,
         "homogeneous": HomogeneousTypeDef,
         "noPreference": NoDatabaseMigrationPreferenceTypeDef,
     },
@@ -882,14 +976,24 @@
     {
         "nextToken": str,
         "taskInfos": List[ImportFileTaskInformationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ManagementPreferenceOutputTypeDef = TypedDict(
+    "ManagementPreferenceOutputTypeDef",
+    {
+        "awsManagedResources": AwsManagedResourcesOutputTypeDef,
+        "noPreference": NoManagementPreferenceOutputTypeDef,
+        "selfManageResources": SelfManageResourcesOutputTypeDef,
+    },
+    total=False,
+)
+
 ManagementPreferenceTypeDef = TypedDict(
     "ManagementPreferenceTypeDef",
     {
         "awsManagedResources": AwsManagedResourcesTypeDef,
         "noPreference": NoManagementPreferenceTypeDef,
         "selfManageResources": SelfManageResourcesTypeDef,
     },
@@ -996,23 +1100,40 @@
         "ipAddress": str,
         "lastActivityTimeStamp": str,
         "registeredTimeStamp": str,
     },
     total=False,
 )
 
+DatabasePreferencesOutputTypeDef = TypedDict(
+    "DatabasePreferencesOutputTypeDef",
+    {
+        "databaseManagementPreference": DatabaseManagementPreferenceType,
+        "databaseMigrationPreference": DatabaseMigrationPreferenceOutputTypeDef,
+    },
+    total=False,
+)
+
 DatabasePreferencesTypeDef = TypedDict(
     "DatabasePreferencesTypeDef",
     {
         "databaseManagementPreference": DatabaseManagementPreferenceType,
         "databaseMigrationPreference": DatabaseMigrationPreferenceTypeDef,
     },
     total=False,
 )
 
+ApplicationPreferencesOutputTypeDef = TypedDict(
+    "ApplicationPreferencesOutputTypeDef",
+    {
+        "managementPreference": ManagementPreferenceOutputTypeDef,
+    },
+    total=False,
+)
+
 ApplicationPreferencesTypeDef = TypedDict(
     "ApplicationPreferencesTypeDef",
     {
         "managementPreference": ManagementPreferenceTypeDef,
     },
     total=False,
 )
@@ -1098,17 +1219,17 @@
     },
 )
 
 GetPortfolioPreferencesResponseTypeDef = TypedDict(
     "GetPortfolioPreferencesResponseTypeDef",
     {
         "applicationMode": ApplicationModeType,
-        "applicationPreferences": ApplicationPreferencesTypeDef,
-        "databasePreferences": DatabasePreferencesTypeDef,
-        "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
+        "applicationPreferences": ApplicationPreferencesOutputTypeDef,
+        "databasePreferences": DatabasePreferencesOutputTypeDef,
+        "prioritizeBusinessGoals": PrioritizeBusinessGoalsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutPortfolioPreferencesRequestRequestTypeDef = TypedDict(
     "PutPortfolioPreferencesRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy/type_defs.pyi` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -77,24 +77,30 @@
     "DatabaseConfigDetailTypeDef",
     "SourceCodeRepositoryTypeDef",
     "ApplicationComponentStatusSummaryTypeDef",
     "ApplicationComponentSummaryTypeDef",
     "ServerStatusSummaryTypeDef",
     "ServerSummaryTypeDef",
     "StrategySummaryTypeDef",
+    "AssessmentTargetOutputTypeDef",
     "AssessmentTargetTypeDef",
     "AssociatedApplicationTypeDef",
+    "AwsManagedResourcesOutputTypeDef",
     "AwsManagedResourcesTypeDef",
+    "BusinessGoalsOutputTypeDef",
     "BusinessGoalsTypeDef",
     "IPAddressBasedRemoteInfoTypeDef",
     "PipelineInfoTypeDef",
     "RemoteSourceCodeAnalysisServerInfoTypeDef",
     "VcenterBasedRemoteInfoTypeDef",
     "VersionControlInfoTypeDef",
     "DataCollectionDetailsTypeDef",
+    "HeterogeneousOutputTypeDef",
+    "HomogeneousOutputTypeDef",
+    "NoDatabaseMigrationPreferenceOutputTypeDef",
     "HeterogeneousTypeDef",
     "HomogeneousTypeDef",
     "NoDatabaseMigrationPreferenceTypeDef",
     "GetApplicationComponentDetailsRequestRequestTypeDef",
     "GetApplicationComponentStrategiesRequestRequestTypeDef",
     "GetAssessmentRequestRequestTypeDef",
     "GetImportFileTaskRequestRequestTypeDef",
@@ -107,14 +113,16 @@
     "GetServerStrategiesRequestRequestTypeDef",
     "GroupTypeDef",
     "ImportFileTaskInformationTypeDef",
     "ListCollectorsRequestListCollectorsPaginateTypeDef",
     "ListCollectorsRequestRequestTypeDef",
     "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
     "ListImportFileTaskRequestRequestTypeDef",
+    "NoManagementPreferenceOutputTypeDef",
+    "SelfManageResourcesOutputTypeDef",
     "NoManagementPreferenceTypeDef",
     "SelfManageResourcesTypeDef",
     "NetworkInfoTypeDef",
     "OSInfoTypeDef",
     "PaginatorConfigTypeDef",
     "TransformationToolTypeDef",
     "ResponseMetadataTypeDef",
@@ -124,35 +132,40 @@
     "StartImportFileTaskResponseTypeDef",
     "StartRecommendationReportGenerationResponseTypeDef",
     "StopAssessmentRequestRequestTypeDef",
     "StrategyOptionTypeDef",
     "AntipatternReportResultTypeDef",
     "AssessmentSummaryTypeDef",
     "StartAssessmentRequestRequestTypeDef",
+    "PrioritizeBusinessGoalsOutputTypeDef",
     "PrioritizeBusinessGoalsTypeDef",
     "ConfigurationSummaryTypeDef",
     "GetAssessmentResponseTypeDef",
+    "DatabaseMigrationPreferenceOutputTypeDef",
     "DatabaseMigrationPreferenceTypeDef",
     "GetRecommendationReportDetailsResponseTypeDef",
     "ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef",
     "ListApplicationComponentsRequestRequestTypeDef",
     "ListServersRequestListServersPaginateTypeDef",
     "ListServersRequestRequestTypeDef",
     "StartImportFileTaskRequestRequestTypeDef",
     "StartRecommendationReportGenerationRequestRequestTypeDef",
     "ListImportFileTaskResponseTypeDef",
+    "ManagementPreferenceOutputTypeDef",
     "ManagementPreferenceTypeDef",
     "SystemInfoTypeDef",
     "RecommendationSetTypeDef",
     "UpdateApplicationComponentConfigRequestRequestTypeDef",
     "UpdateServerConfigRequestRequestTypeDef",
     "ResultTypeDef",
     "GetPortfolioSummaryResponseTypeDef",
     "CollectorTypeDef",
+    "DatabasePreferencesOutputTypeDef",
     "DatabasePreferencesTypeDef",
+    "ApplicationPreferencesOutputTypeDef",
     "ApplicationPreferencesTypeDef",
     "ApplicationComponentStrategyTypeDef",
     "ServerDetailTypeDef",
     "ServerStrategyTypeDef",
     "ApplicationComponentDetailTypeDef",
     "ListCollectorsResponseTypeDef",
     "GetPortfolioPreferencesResponseTypeDef",
@@ -270,37 +283,64 @@
     {
         "count": int,
         "strategy": StrategyType,
     },
     total=False,
 )
 
+AssessmentTargetOutputTypeDef = TypedDict(
+    "AssessmentTargetOutputTypeDef",
+    {
+        "condition": ConditionType,
+        "name": str,
+        "values": List[str],
+    },
+)
+
 AssessmentTargetTypeDef = TypedDict(
     "AssessmentTargetTypeDef",
     {
         "condition": ConditionType,
         "name": str,
-        "values": List[str],
+        "values": Sequence[str],
     },
 )
 
 AssociatedApplicationTypeDef = TypedDict(
     "AssociatedApplicationTypeDef",
     {
         "id": str,
         "name": str,
     },
     total=False,
 )
 
+AwsManagedResourcesOutputTypeDef = TypedDict(
+    "AwsManagedResourcesOutputTypeDef",
+    {
+        "targetDestination": List[AwsManagedTargetDestinationType],
+    },
+)
+
 AwsManagedResourcesTypeDef = TypedDict(
     "AwsManagedResourcesTypeDef",
     {
-        "targetDestination": List[AwsManagedTargetDestinationType],
+        "targetDestination": Sequence[AwsManagedTargetDestinationType],
+    },
+)
+
+BusinessGoalsOutputTypeDef = TypedDict(
+    "BusinessGoalsOutputTypeDef",
+    {
+        "licenseCostReduction": int,
+        "modernizeInfrastructureWithCloudNativeTechnologies": int,
+        "reduceOperationalOverheadWithManagedServices": int,
+        "speedOfMigration": int,
     },
+    total=False,
 )
 
 BusinessGoalsTypeDef = TypedDict(
     "BusinessGoalsTypeDef",
     {
         "licenseCostReduction": int,
         "modernizeInfrastructureWithCloudNativeTechnologies": int,
@@ -366,33 +406,55 @@
         "status": AssessmentStatusType,
         "statusMessage": str,
         "success": int,
     },
     total=False,
 )
 
+HeterogeneousOutputTypeDef = TypedDict(
+    "HeterogeneousOutputTypeDef",
+    {
+        "targetDatabaseEngine": List[HeterogeneousTargetDatabaseEngineType],
+    },
+)
+
+HomogeneousOutputTypeDef = TypedDict(
+    "HomogeneousOutputTypeDef",
+    {
+        "targetDatabaseEngine": List[Literal["None specified"]],
+    },
+    total=False,
+)
+
+NoDatabaseMigrationPreferenceOutputTypeDef = TypedDict(
+    "NoDatabaseMigrationPreferenceOutputTypeDef",
+    {
+        "targetDatabaseEngine": List[TargetDatabaseEngineType],
+    },
+)
+
 HeterogeneousTypeDef = TypedDict(
     "HeterogeneousTypeDef",
     {
-        "targetDatabaseEngine": List[HeterogeneousTargetDatabaseEngineType],
+        "targetDatabaseEngine": Sequence[HeterogeneousTargetDatabaseEngineType],
     },
 )
 
 HomogeneousTypeDef = TypedDict(
     "HomogeneousTypeDef",
     {
-        "targetDatabaseEngine": List[Literal["None specified"]],
+        "targetDatabaseEngine": Sequence[Literal["None specified"]],
     },
     total=False,
 )
 
 NoDatabaseMigrationPreferenceTypeDef = TypedDict(
     "NoDatabaseMigrationPreferenceTypeDef",
     {
-        "targetDatabaseEngine": List[TargetDatabaseEngineType],
+        "targetDatabaseEngine": Sequence[TargetDatabaseEngineType],
     },
 )
 
 GetApplicationComponentDetailsRequestRequestTypeDef = TypedDict(
     "GetApplicationComponentDetailsRequestRequestTypeDef",
     {
         "applicationComponentId": str,
@@ -570,25 +632,39 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+NoManagementPreferenceOutputTypeDef = TypedDict(
+    "NoManagementPreferenceOutputTypeDef",
+    {
+        "targetDestination": List[NoPreferenceTargetDestinationType],
+    },
+)
+
+SelfManageResourcesOutputTypeDef = TypedDict(
+    "SelfManageResourcesOutputTypeDef",
+    {
+        "targetDestination": List[SelfManageTargetDestinationType],
+    },
+)
+
 NoManagementPreferenceTypeDef = TypedDict(
     "NoManagementPreferenceTypeDef",
     {
-        "targetDestination": List[NoPreferenceTargetDestinationType],
+        "targetDestination": Sequence[NoPreferenceTargetDestinationType],
     },
 )
 
 SelfManageResourcesTypeDef = TypedDict(
     "SelfManageResourcesTypeDef",
     {
-        "targetDestination": List[SelfManageTargetDestinationType],
+        "targetDestination": Sequence[SelfManageTargetDestinationType],
     },
 )
 
 NetworkInfoTypeDef = TypedDict(
     "NetworkInfoTypeDef",
     {
         "interfaceName": str,
@@ -734,14 +810,22 @@
         "assessmentTargets": Sequence[AssessmentTargetTypeDef],
         "s3bucketForAnalysisData": str,
         "s3bucketForReportData": str,
     },
     total=False,
 )
 
+PrioritizeBusinessGoalsOutputTypeDef = TypedDict(
+    "PrioritizeBusinessGoalsOutputTypeDef",
+    {
+        "businessGoals": BusinessGoalsOutputTypeDef,
+    },
+    total=False,
+)
+
 PrioritizeBusinessGoalsTypeDef = TypedDict(
     "PrioritizeBusinessGoalsTypeDef",
     {
         "businessGoals": BusinessGoalsTypeDef,
     },
     total=False,
 )
@@ -757,21 +841,31 @@
     },
     total=False,
 )
 
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
-        "assessmentTargets": List[AssessmentTargetTypeDef],
+        "assessmentTargets": List[AssessmentTargetOutputTypeDef],
         "dataCollectionDetails": DataCollectionDetailsTypeDef,
         "id": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DatabaseMigrationPreferenceOutputTypeDef = TypedDict(
+    "DatabaseMigrationPreferenceOutputTypeDef",
+    {
+        "heterogeneous": HeterogeneousOutputTypeDef,
+        "homogeneous": HomogeneousOutputTypeDef,
+        "noPreference": NoDatabaseMigrationPreferenceOutputTypeDef,
+    },
+    total=False,
+)
+
 DatabaseMigrationPreferenceTypeDef = TypedDict(
     "DatabaseMigrationPreferenceTypeDef",
     {
         "heterogeneous": HeterogeneousTypeDef,
         "homogeneous": HomogeneousTypeDef,
         "noPreference": NoDatabaseMigrationPreferenceTypeDef,
     },
@@ -875,14 +969,24 @@
     {
         "nextToken": str,
         "taskInfos": List[ImportFileTaskInformationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ManagementPreferenceOutputTypeDef = TypedDict(
+    "ManagementPreferenceOutputTypeDef",
+    {
+        "awsManagedResources": AwsManagedResourcesOutputTypeDef,
+        "noPreference": NoManagementPreferenceOutputTypeDef,
+        "selfManageResources": SelfManageResourcesOutputTypeDef,
+    },
+    total=False,
+)
+
 ManagementPreferenceTypeDef = TypedDict(
     "ManagementPreferenceTypeDef",
     {
         "awsManagedResources": AwsManagedResourcesTypeDef,
         "noPreference": NoManagementPreferenceTypeDef,
         "selfManageResources": SelfManageResourcesTypeDef,
     },
@@ -985,23 +1089,40 @@
         "ipAddress": str,
         "lastActivityTimeStamp": str,
         "registeredTimeStamp": str,
     },
     total=False,
 )
 
+DatabasePreferencesOutputTypeDef = TypedDict(
+    "DatabasePreferencesOutputTypeDef",
+    {
+        "databaseManagementPreference": DatabaseManagementPreferenceType,
+        "databaseMigrationPreference": DatabaseMigrationPreferenceOutputTypeDef,
+    },
+    total=False,
+)
+
 DatabasePreferencesTypeDef = TypedDict(
     "DatabasePreferencesTypeDef",
     {
         "databaseManagementPreference": DatabaseManagementPreferenceType,
         "databaseMigrationPreference": DatabaseMigrationPreferenceTypeDef,
     },
     total=False,
 )
 
+ApplicationPreferencesOutputTypeDef = TypedDict(
+    "ApplicationPreferencesOutputTypeDef",
+    {
+        "managementPreference": ManagementPreferenceOutputTypeDef,
+    },
+    total=False,
+)
+
 ApplicationPreferencesTypeDef = TypedDict(
     "ApplicationPreferencesTypeDef",
     {
         "managementPreference": ManagementPreferenceTypeDef,
     },
     total=False,
 )
@@ -1087,17 +1208,17 @@
     },
 )
 
 GetPortfolioPreferencesResponseTypeDef = TypedDict(
     "GetPortfolioPreferencesResponseTypeDef",
     {
         "applicationMode": ApplicationModeType,
-        "applicationPreferences": ApplicationPreferencesTypeDef,
-        "databasePreferences": DatabasePreferencesTypeDef,
-        "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
+        "applicationPreferences": ApplicationPreferencesOutputTypeDef,
+        "databasePreferences": DatabasePreferencesOutputTypeDef,
+        "prioritizeBusinessGoals": PrioritizeBusinessGoalsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutPortfolioPreferencesRequestRequestTypeDef = TypedDict(
     "PutPortfolioPreferencesRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhubstrategy
-Version: 1.28.0
-Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-migrationhubstrategy"></a>
 
 # mypy-boto3-migrationhubstrategy
 
 [![PyPI - mypy-boto3-migrationhubstrategy](https://img.shields.io/pypi/v/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhubstrategy?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhubstrategy)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhubstrategy)](https://pepy.tech/project/mypy-boto3-migrationhubstrategy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubStrategyRecommendations 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
+[boto3.MigrationHubStrategyRecommendations 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -394,24 +394,30 @@
     DatabaseConfigDetailTypeDef,
     SourceCodeRepositoryTypeDef,
     ApplicationComponentStatusSummaryTypeDef,
     ApplicationComponentSummaryTypeDef,
     ServerStatusSummaryTypeDef,
     ServerSummaryTypeDef,
     StrategySummaryTypeDef,
+    AssessmentTargetOutputTypeDef,
     AssessmentTargetTypeDef,
     AssociatedApplicationTypeDef,
+    AwsManagedResourcesOutputTypeDef,
     AwsManagedResourcesTypeDef,
+    BusinessGoalsOutputTypeDef,
     BusinessGoalsTypeDef,
     IPAddressBasedRemoteInfoTypeDef,
     PipelineInfoTypeDef,
     RemoteSourceCodeAnalysisServerInfoTypeDef,
     VcenterBasedRemoteInfoTypeDef,
     VersionControlInfoTypeDef,
     DataCollectionDetailsTypeDef,
+    HeterogeneousOutputTypeDef,
+    HomogeneousOutputTypeDef,
+    NoDatabaseMigrationPreferenceOutputTypeDef,
     HeterogeneousTypeDef,
     HomogeneousTypeDef,
     NoDatabaseMigrationPreferenceTypeDef,
     GetApplicationComponentDetailsRequestRequestTypeDef,
     GetApplicationComponentStrategiesRequestRequestTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetImportFileTaskRequestRequestTypeDef,
@@ -424,14 +430,16 @@
     GetServerStrategiesRequestRequestTypeDef,
     GroupTypeDef,
     ImportFileTaskInformationTypeDef,
     ListCollectorsRequestListCollectorsPaginateTypeDef,
     ListCollectorsRequestRequestTypeDef,
     ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListImportFileTaskRequestRequestTypeDef,
+    NoManagementPreferenceOutputTypeDef,
+    SelfManageResourcesOutputTypeDef,
     NoManagementPreferenceTypeDef,
     SelfManageResourcesTypeDef,
     NetworkInfoTypeDef,
     OSInfoTypeDef,
     PaginatorConfigTypeDef,
     TransformationToolTypeDef,
     ResponseMetadataTypeDef,
@@ -441,35 +449,40 @@
     StartImportFileTaskResponseTypeDef,
     StartRecommendationReportGenerationResponseTypeDef,
     StopAssessmentRequestRequestTypeDef,
     StrategyOptionTypeDef,
     AntipatternReportResultTypeDef,
     AssessmentSummaryTypeDef,
     StartAssessmentRequestRequestTypeDef,
+    PrioritizeBusinessGoalsOutputTypeDef,
     PrioritizeBusinessGoalsTypeDef,
     ConfigurationSummaryTypeDef,
     GetAssessmentResponseTypeDef,
+    DatabaseMigrationPreferenceOutputTypeDef,
     DatabaseMigrationPreferenceTypeDef,
     GetRecommendationReportDetailsResponseTypeDef,
     ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef,
     ListApplicationComponentsRequestRequestTypeDef,
     ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     StartImportFileTaskRequestRequestTypeDef,
     StartRecommendationReportGenerationRequestRequestTypeDef,
     ListImportFileTaskResponseTypeDef,
+    ManagementPreferenceOutputTypeDef,
     ManagementPreferenceTypeDef,
     SystemInfoTypeDef,
     RecommendationSetTypeDef,
     UpdateApplicationComponentConfigRequestRequestTypeDef,
     UpdateServerConfigRequestRequestTypeDef,
     ResultTypeDef,
     GetPortfolioSummaryResponseTypeDef,
     CollectorTypeDef,
+    DatabasePreferencesOutputTypeDef,
     DatabasePreferencesTypeDef,
+    ApplicationPreferencesOutputTypeDef,
     ApplicationPreferencesTypeDef,
     ApplicationComponentStrategyTypeDef,
     ServerDetailTypeDef,
     ServerStrategyTypeDef,
     ApplicationComponentDetailTypeDef,
     ListCollectorsResponseTypeDef,
     GetPortfolioPreferencesResponseTypeDef,
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt` & `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.0/setup.py` & `mypy-boto3-migrationhubstrategy-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhubstrategy",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_migrationhubstrategy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.0 service generated"
-        " with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.12 service generated"
+        " with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

