# Comparing `tmp/mypy-boto3-codebuild-1.28.0.tar.gz` & `tmp/mypy-boto3-codebuild-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codebuild-1.28.0.tar", last modified: Thu Jul  6 20:59:12 2023, max compression
+gzip compressed data, was "mypy-boto3-codebuild-1.28.12.tar", last modified: Thu Jul 27 05:34:27 2023, max compression
```

## Comparing `mypy-boto3-codebuild-1.28.0.tar` & `mypy-boto3-codebuild-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.674251 mypy-boto3-codebuild-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:45.000000 mypy-boto3-codebuild-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-07-06 20:59:12.674251 mypy-boto3-codebuild-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-06 20:35:45.000000 mypy-boto3-codebuild-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.666251 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-06 20:35:45.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-06 20:35:45.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:35:45.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41431 2023-07-06 20:35:45.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41367 2023-07-06 20:35:45.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-06 20:35:46.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-07-06 20:35:46.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-06 20:35:45.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15324 2023-07-06 20:35:45.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:45.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57281 2023-07-06 20:35:49.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57222 2023-07-06 20:35:48.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:45.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.674251 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-07-06 20:59:12.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 20:59:12.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:12.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 20:59:12.000000 mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:12.674251 mypy-boto3-codebuild-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:35:45.000000 mypy-boto3-codebuild-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.240556 mypy-boto3-codebuild-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21786 2023-07-27 05:34:27.240556 mypy-boto3-codebuild-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20291 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.236556 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41431 2023-07-27 05:18:56.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41367 2023-07-27 05:18:56.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-07-27 05:18:57.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-07-27 05:18:56.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-27 05:18:56.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15324 2023-07-27 05:18:56.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65803 2023-07-27 05:18:58.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65726 2023-07-27 05:18:57.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.240556 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21786 2023-07-27 05:34:27.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:27.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:27.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:27.000000 mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:27.240556 mypy-boto3-codebuild-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:18:55.000000 mypy-boto3-codebuild-1.28.12/setup.py
```

### Comparing `mypy-boto3-codebuild-1.28.0/LICENSE` & `mypy-boto3-codebuild-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.0/PKG-INFO` & `mypy-boto3-codebuild-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codebuild
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeBuild 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodeBuild 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codebuild"></a>
 
 # mypy-boto3-codebuild
 
 [![PyPI - mypy-boto3-codebuild](https://img.shields.io/pypi/v/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codebuild?color=blue)](https://pypistats.org/packages/mypy-boto3-codebuild)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codebuild)](https://pepy.tech/project/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [mypy-boto3-codebuild docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/).
 
 See how it helps to find and fix potential bugs:
 
@@ -412,52 +412,61 @@
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
     BatchGetBuildsInputRequestTypeDef,
     BatchGetProjectsInputRequestTypeDef,
     BatchGetReportGroupsInputRequestTypeDef,
     BatchGetReportsInputRequestTypeDef,
+    BatchRestrictionsOutputTypeDef,
     BatchRestrictionsTypeDef,
     BuildArtifactsTypeDef,
     BuildBatchFilterTypeDef,
     PhaseContextTypeDef,
-    ProjectCacheTypeDef,
-    ProjectFileSystemLocationTypeDef,
-    ProjectSourceVersionTypeDef,
-    VpcConfigTypeDef,
+    ProjectCacheOutputTypeDef,
+    ProjectFileSystemLocationOutputTypeDef,
+    ProjectSourceVersionOutputTypeDef,
+    VpcConfigOutputTypeDef,
+    BuildStatusConfigOutputTypeDef,
     BuildStatusConfigTypeDef,
     ResolvedArtifactTypeDef,
     DebugSessionTypeDef,
     ExportedEnvironmentVariableTypeDef,
     NetworkInterfaceTypeDef,
+    CloudWatchLogsConfigOutputTypeDef,
     CloudWatchLogsConfigTypeDef,
     CodeCoverageReportSummaryTypeDef,
     CodeCoverageTypeDef,
     ProjectArtifactsTypeDef,
+    ProjectCacheTypeDef,
+    ProjectFileSystemLocationTypeDef,
+    ProjectSourceVersionTypeDef,
     TagTypeDef,
+    VpcConfigTypeDef,
     WebhookFilterTypeDef,
     DeleteBuildBatchInputRequestTypeDef,
     DeleteProjectInputRequestTypeDef,
     DeleteReportGroupInputRequestTypeDef,
     DeleteReportInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteSourceCredentialsInputRequestTypeDef,
     DeleteSourceCredentialsOutputTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
     DescribeCodeCoveragesInputRequestTypeDef,
     TestCaseFilterTypeDef,
     TestCaseTypeDef,
     EnvironmentImageTypeDef,
+    EnvironmentVariableOutputTypeDef,
     EnvironmentVariableTypeDef,
     GetReportGroupTrendInputRequestTypeDef,
     ReportGroupTrendStatsTypeDef,
     ReportWithRawDataTypeDef,
     GetResourcePolicyInputRequestTypeDef,
     GetResourcePolicyOutputTypeDef,
+    GitSubmodulesConfigOutputTypeDef,
     GitSubmodulesConfigTypeDef,
     ImportSourceCredentialsInputRequestTypeDef,
     ImportSourceCredentialsOutputTypeDef,
     InvalidateProjectCacheInputRequestTypeDef,
     ListBuildBatchesForProjectOutputTypeDef,
     ListBuildBatchesOutputTypeDef,
     ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
@@ -478,86 +487,98 @@
     ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
     ListSharedProjectsInputRequestTypeDef,
     ListSharedProjectsOutputTypeDef,
     ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     ListSharedReportGroupsInputRequestTypeDef,
     ListSharedReportGroupsOutputTypeDef,
     SourceCredentialsInfoTypeDef,
+    S3LogsConfigOutputTypeDef,
     S3LogsConfigTypeDef,
     PaginatorConfigTypeDef,
+    ProjectArtifactsOutputTypeDef,
     ProjectBadgeTypeDef,
+    RegistryCredentialOutputTypeDef,
     RegistryCredentialTypeDef,
+    SourceAuthOutputTypeDef,
     SourceAuthTypeDef,
+    TagOutputTypeDef,
     PutResourcePolicyInputRequestTypeDef,
     PutResourcePolicyOutputTypeDef,
+    S3ReportExportConfigOutputTypeDef,
     S3ReportExportConfigTypeDef,
     TestReportSummaryTypeDef,
     ResponseMetadataTypeDef,
     RetryBuildBatchInputRequestTypeDef,
     RetryBuildInputRequestTypeDef,
     StopBuildBatchInputRequestTypeDef,
     StopBuildInputRequestTypeDef,
     UpdateProjectVisibilityInputRequestTypeDef,
     UpdateProjectVisibilityOutputTypeDef,
+    WebhookFilterOutputTypeDef,
     BatchDeleteBuildsOutputTypeDef,
     DeleteBuildBatchOutputTypeDef,
+    ProjectBuildBatchConfigOutputTypeDef,
     ProjectBuildBatchConfigTypeDef,
     ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
     ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
-    WebhookTypeDef,
     DescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     DescribeTestCasesInputRequestTypeDef,
     DescribeTestCasesOutputTypeDef,
     EnvironmentLanguageTypeDef,
     GetReportGroupTrendOutputTypeDef,
     ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     ListReportsForReportGroupInputRequestTypeDef,
     ListReportsInputListReportsPaginateTypeDef,
     ListReportsInputRequestTypeDef,
     ListSourceCredentialsOutputTypeDef,
-    LogsConfigTypeDef,
+    LogsConfigOutputTypeDef,
     LogsLocationTypeDef,
+    LogsConfigTypeDef,
+    ProjectEnvironmentOutputTypeDef,
     ProjectEnvironmentTypeDef,
+    ProjectSourceOutputTypeDef,
     ProjectSourceTypeDef,
+    ReportExportConfigOutputTypeDef,
     ReportExportConfigTypeDef,
+    WebhookTypeDef,
     BuildGroupTypeDef,
-    CreateWebhookOutputTypeDef,
-    UpdateWebhookOutputTypeDef,
     EnvironmentPlatformTypeDef,
     BuildTypeDef,
     CreateProjectInputRequestTypeDef,
-    ProjectTypeDef,
     StartBuildBatchInputRequestTypeDef,
     StartBuildInputRequestTypeDef,
     UpdateProjectInputRequestTypeDef,
-    CreateReportGroupInputRequestTypeDef,
     ReportGroupTypeDef,
     ReportTypeDef,
+    CreateReportGroupInputRequestTypeDef,
     UpdateReportGroupInputRequestTypeDef,
+    CreateWebhookOutputTypeDef,
+    ProjectTypeDef,
+    UpdateWebhookOutputTypeDef,
     BuildBatchTypeDef,
     ListCuratedEnvironmentImagesOutputTypeDef,
     BatchGetBuildsOutputTypeDef,
     RetryBuildOutputTypeDef,
     StartBuildOutputTypeDef,
     StopBuildOutputTypeDef,
-    BatchGetProjectsOutputTypeDef,
-    CreateProjectOutputTypeDef,
-    UpdateProjectOutputTypeDef,
     BatchGetReportGroupsOutputTypeDef,
     CreateReportGroupOutputTypeDef,
     UpdateReportGroupOutputTypeDef,
     BatchGetReportsOutputTypeDef,
+    BatchGetProjectsOutputTypeDef,
+    CreateProjectOutputTypeDef,
+    UpdateProjectOutputTypeDef,
     BatchGetBuildBatchesOutputTypeDef,
     RetryBuildBatchOutputTypeDef,
     StartBuildBatchOutputTypeDef,
     StopBuildBatchOutputTypeDef,
 )
```

### Comparing `mypy-boto3-codebuild-1.28.0/README.md` & `mypy-boto3-codebuild-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codebuild"></a>
 
 # mypy-boto3-codebuild
 
 [![PyPI - mypy-boto3-codebuild](https://img.shields.io/pypi/v/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codebuild?color=blue)](https://pypistats.org/packages/mypy-boto3-codebuild)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codebuild)](https://pepy.tech/project/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [mypy-boto3-codebuild docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/).
 
 See how it helps to find and fix potential bugs:
 
@@ -380,52 +380,61 @@
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
     BatchGetBuildsInputRequestTypeDef,
     BatchGetProjectsInputRequestTypeDef,
     BatchGetReportGroupsInputRequestTypeDef,
     BatchGetReportsInputRequestTypeDef,
+    BatchRestrictionsOutputTypeDef,
     BatchRestrictionsTypeDef,
     BuildArtifactsTypeDef,
     BuildBatchFilterTypeDef,
     PhaseContextTypeDef,
-    ProjectCacheTypeDef,
-    ProjectFileSystemLocationTypeDef,
-    ProjectSourceVersionTypeDef,
-    VpcConfigTypeDef,
+    ProjectCacheOutputTypeDef,
+    ProjectFileSystemLocationOutputTypeDef,
+    ProjectSourceVersionOutputTypeDef,
+    VpcConfigOutputTypeDef,
+    BuildStatusConfigOutputTypeDef,
     BuildStatusConfigTypeDef,
     ResolvedArtifactTypeDef,
     DebugSessionTypeDef,
     ExportedEnvironmentVariableTypeDef,
     NetworkInterfaceTypeDef,
+    CloudWatchLogsConfigOutputTypeDef,
     CloudWatchLogsConfigTypeDef,
     CodeCoverageReportSummaryTypeDef,
     CodeCoverageTypeDef,
     ProjectArtifactsTypeDef,
+    ProjectCacheTypeDef,
+    ProjectFileSystemLocationTypeDef,
+    ProjectSourceVersionTypeDef,
     TagTypeDef,
+    VpcConfigTypeDef,
     WebhookFilterTypeDef,
     DeleteBuildBatchInputRequestTypeDef,
     DeleteProjectInputRequestTypeDef,
     DeleteReportGroupInputRequestTypeDef,
     DeleteReportInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteSourceCredentialsInputRequestTypeDef,
     DeleteSourceCredentialsOutputTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
     DescribeCodeCoveragesInputRequestTypeDef,
     TestCaseFilterTypeDef,
     TestCaseTypeDef,
     EnvironmentImageTypeDef,
+    EnvironmentVariableOutputTypeDef,
     EnvironmentVariableTypeDef,
     GetReportGroupTrendInputRequestTypeDef,
     ReportGroupTrendStatsTypeDef,
     ReportWithRawDataTypeDef,
     GetResourcePolicyInputRequestTypeDef,
     GetResourcePolicyOutputTypeDef,
+    GitSubmodulesConfigOutputTypeDef,
     GitSubmodulesConfigTypeDef,
     ImportSourceCredentialsInputRequestTypeDef,
     ImportSourceCredentialsOutputTypeDef,
     InvalidateProjectCacheInputRequestTypeDef,
     ListBuildBatchesForProjectOutputTypeDef,
     ListBuildBatchesOutputTypeDef,
     ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
@@ -446,86 +455,98 @@
     ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
     ListSharedProjectsInputRequestTypeDef,
     ListSharedProjectsOutputTypeDef,
     ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     ListSharedReportGroupsInputRequestTypeDef,
     ListSharedReportGroupsOutputTypeDef,
     SourceCredentialsInfoTypeDef,
+    S3LogsConfigOutputTypeDef,
     S3LogsConfigTypeDef,
     PaginatorConfigTypeDef,
+    ProjectArtifactsOutputTypeDef,
     ProjectBadgeTypeDef,
+    RegistryCredentialOutputTypeDef,
     RegistryCredentialTypeDef,
+    SourceAuthOutputTypeDef,
     SourceAuthTypeDef,
+    TagOutputTypeDef,
     PutResourcePolicyInputRequestTypeDef,
     PutResourcePolicyOutputTypeDef,
+    S3ReportExportConfigOutputTypeDef,
     S3ReportExportConfigTypeDef,
     TestReportSummaryTypeDef,
     ResponseMetadataTypeDef,
     RetryBuildBatchInputRequestTypeDef,
     RetryBuildInputRequestTypeDef,
     StopBuildBatchInputRequestTypeDef,
     StopBuildInputRequestTypeDef,
     UpdateProjectVisibilityInputRequestTypeDef,
     UpdateProjectVisibilityOutputTypeDef,
+    WebhookFilterOutputTypeDef,
     BatchDeleteBuildsOutputTypeDef,
     DeleteBuildBatchOutputTypeDef,
+    ProjectBuildBatchConfigOutputTypeDef,
     ProjectBuildBatchConfigTypeDef,
     ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
     ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
-    WebhookTypeDef,
     DescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     DescribeTestCasesInputRequestTypeDef,
     DescribeTestCasesOutputTypeDef,
     EnvironmentLanguageTypeDef,
     GetReportGroupTrendOutputTypeDef,
     ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     ListReportsForReportGroupInputRequestTypeDef,
     ListReportsInputListReportsPaginateTypeDef,
     ListReportsInputRequestTypeDef,
     ListSourceCredentialsOutputTypeDef,
-    LogsConfigTypeDef,
+    LogsConfigOutputTypeDef,
     LogsLocationTypeDef,
+    LogsConfigTypeDef,
+    ProjectEnvironmentOutputTypeDef,
     ProjectEnvironmentTypeDef,
+    ProjectSourceOutputTypeDef,
     ProjectSourceTypeDef,
+    ReportExportConfigOutputTypeDef,
     ReportExportConfigTypeDef,
+    WebhookTypeDef,
     BuildGroupTypeDef,
-    CreateWebhookOutputTypeDef,
-    UpdateWebhookOutputTypeDef,
     EnvironmentPlatformTypeDef,
     BuildTypeDef,
     CreateProjectInputRequestTypeDef,
-    ProjectTypeDef,
     StartBuildBatchInputRequestTypeDef,
     StartBuildInputRequestTypeDef,
     UpdateProjectInputRequestTypeDef,
-    CreateReportGroupInputRequestTypeDef,
     ReportGroupTypeDef,
     ReportTypeDef,
+    CreateReportGroupInputRequestTypeDef,
     UpdateReportGroupInputRequestTypeDef,
+    CreateWebhookOutputTypeDef,
+    ProjectTypeDef,
+    UpdateWebhookOutputTypeDef,
     BuildBatchTypeDef,
     ListCuratedEnvironmentImagesOutputTypeDef,
     BatchGetBuildsOutputTypeDef,
     RetryBuildOutputTypeDef,
     StartBuildOutputTypeDef,
     StopBuildOutputTypeDef,
-    BatchGetProjectsOutputTypeDef,
-    CreateProjectOutputTypeDef,
-    UpdateProjectOutputTypeDef,
     BatchGetReportGroupsOutputTypeDef,
     CreateReportGroupOutputTypeDef,
     UpdateReportGroupOutputTypeDef,
     BatchGetReportsOutputTypeDef,
+    BatchGetProjectsOutputTypeDef,
+    CreateProjectOutputTypeDef,
+    UpdateProjectOutputTypeDef,
     BatchGetBuildBatchesOutputTypeDef,
     RetryBuildBatchOutputTypeDef,
     StartBuildBatchOutputTypeDef,
     StopBuildBatchOutputTypeDef,
 )
```

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/__init__.py` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/__init__.pyi` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/__main__.py` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeBuild 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CodeBuild 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild\nOther"
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

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/client.py` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/client.pyi` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/literals.py` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/literals.pyi`

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
     "ArtifactNamespaceType",
     "ArtifactPackagingType",
     "ArtifactsTypeType",
     "AuthTypeType",
     "BatchReportModeTypeType",
     "BucketOwnerAccessType",
@@ -73,15 +72,14 @@
     "CodeBuildServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ArtifactNamespaceType = Literal["BUILD_ID", "NONE"]
 ArtifactPackagingType = Literal["NONE", "ZIP"]
 ArtifactsTypeType = Literal["CODEPIPELINE", "NO_ARTIFACTS", "S3"]
 AuthTypeType = Literal["BASIC_AUTH", "OAUTH", "PERSONAL_ACCESS_TOKEN"]
 BatchReportModeTypeType = Literal["REPORT_AGGREGATED_BATCH", "REPORT_INDIVIDUAL_BUILDS"]
 BucketOwnerAccessType = Literal["FULL", "NONE", "READ_ONLY"]
 BuildBatchPhaseTypeType = Literal[
@@ -291,14 +289,15 @@
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
@@ -377,26 +376,28 @@
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

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/literals.pyi` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ArtifactNamespaceType",
     "ArtifactPackagingType",
     "ArtifactsTypeType",
     "AuthTypeType",
     "BatchReportModeTypeType",
     "BucketOwnerAccessType",
@@ -72,14 +73,15 @@
     "CodeBuildServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ArtifactNamespaceType = Literal["BUILD_ID", "NONE"]
 ArtifactPackagingType = Literal["NONE", "ZIP"]
 ArtifactsTypeType = Literal["CODEPIPELINE", "NO_ARTIFACTS", "S3"]
 AuthTypeType = Literal["BASIC_AUTH", "OAUTH", "PERSONAL_ACCESS_TOKEN"]
 BatchReportModeTypeType = Literal["REPORT_AGGREGATED_BATCH", "REPORT_INDIVIDUAL_BUILDS"]
 BucketOwnerAccessType = Literal["FULL", "NONE", "READ_ONLY"]
 BuildBatchPhaseTypeType = Literal[
@@ -289,14 +291,15 @@
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
@@ -375,26 +378,28 @@
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

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/paginator.py` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/paginator.pyi` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/type_defs.py` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,52 +67,61 @@
     "BatchDeleteBuildsInputRequestTypeDef",
     "BuildNotDeletedTypeDef",
     "BatchGetBuildBatchesInputRequestTypeDef",
     "BatchGetBuildsInputRequestTypeDef",
     "BatchGetProjectsInputRequestTypeDef",
     "BatchGetReportGroupsInputRequestTypeDef",
     "BatchGetReportsInputRequestTypeDef",
+    "BatchRestrictionsOutputTypeDef",
     "BatchRestrictionsTypeDef",
     "BuildArtifactsTypeDef",
     "BuildBatchFilterTypeDef",
     "PhaseContextTypeDef",
-    "ProjectCacheTypeDef",
-    "ProjectFileSystemLocationTypeDef",
-    "ProjectSourceVersionTypeDef",
-    "VpcConfigTypeDef",
+    "ProjectCacheOutputTypeDef",
+    "ProjectFileSystemLocationOutputTypeDef",
+    "ProjectSourceVersionOutputTypeDef",
+    "VpcConfigOutputTypeDef",
+    "BuildStatusConfigOutputTypeDef",
     "BuildStatusConfigTypeDef",
     "ResolvedArtifactTypeDef",
     "DebugSessionTypeDef",
     "ExportedEnvironmentVariableTypeDef",
     "NetworkInterfaceTypeDef",
+    "CloudWatchLogsConfigOutputTypeDef",
     "CloudWatchLogsConfigTypeDef",
     "CodeCoverageReportSummaryTypeDef",
     "CodeCoverageTypeDef",
     "ProjectArtifactsTypeDef",
+    "ProjectCacheTypeDef",
+    "ProjectFileSystemLocationTypeDef",
+    "ProjectSourceVersionTypeDef",
     "TagTypeDef",
+    "VpcConfigTypeDef",
     "WebhookFilterTypeDef",
     "DeleteBuildBatchInputRequestTypeDef",
     "DeleteProjectInputRequestTypeDef",
     "DeleteReportGroupInputRequestTypeDef",
     "DeleteReportInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteSourceCredentialsInputRequestTypeDef",
     "DeleteSourceCredentialsOutputTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
     "DescribeCodeCoveragesInputRequestTypeDef",
     "TestCaseFilterTypeDef",
     "TestCaseTypeDef",
     "EnvironmentImageTypeDef",
+    "EnvironmentVariableOutputTypeDef",
     "EnvironmentVariableTypeDef",
     "GetReportGroupTrendInputRequestTypeDef",
     "ReportGroupTrendStatsTypeDef",
     "ReportWithRawDataTypeDef",
     "GetResourcePolicyInputRequestTypeDef",
     "GetResourcePolicyOutputTypeDef",
+    "GitSubmodulesConfigOutputTypeDef",
     "GitSubmodulesConfigTypeDef",
     "ImportSourceCredentialsInputRequestTypeDef",
     "ImportSourceCredentialsOutputTypeDef",
     "InvalidateProjectCacheInputRequestTypeDef",
     "ListBuildBatchesForProjectOutputTypeDef",
     "ListBuildBatchesOutputTypeDef",
     "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
@@ -133,86 +142,98 @@
     "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
     "ListSharedProjectsInputRequestTypeDef",
     "ListSharedProjectsOutputTypeDef",
     "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "ListSharedReportGroupsInputRequestTypeDef",
     "ListSharedReportGroupsOutputTypeDef",
     "SourceCredentialsInfoTypeDef",
+    "S3LogsConfigOutputTypeDef",
     "S3LogsConfigTypeDef",
     "PaginatorConfigTypeDef",
+    "ProjectArtifactsOutputTypeDef",
     "ProjectBadgeTypeDef",
+    "RegistryCredentialOutputTypeDef",
     "RegistryCredentialTypeDef",
+    "SourceAuthOutputTypeDef",
     "SourceAuthTypeDef",
+    "TagOutputTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
     "PutResourcePolicyOutputTypeDef",
+    "S3ReportExportConfigOutputTypeDef",
     "S3ReportExportConfigTypeDef",
     "TestReportSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "RetryBuildBatchInputRequestTypeDef",
     "RetryBuildInputRequestTypeDef",
     "StopBuildBatchInputRequestTypeDef",
     "StopBuildInputRequestTypeDef",
     "UpdateProjectVisibilityInputRequestTypeDef",
     "UpdateProjectVisibilityOutputTypeDef",
+    "WebhookFilterOutputTypeDef",
     "BatchDeleteBuildsOutputTypeDef",
     "DeleteBuildBatchOutputTypeDef",
+    "ProjectBuildBatchConfigOutputTypeDef",
     "ProjectBuildBatchConfigTypeDef",
     "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     "ListBuildBatchesForProjectInputRequestTypeDef",
     "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
     "ListBuildBatchesInputRequestTypeDef",
     "BuildBatchPhaseTypeDef",
     "BuildPhaseTypeDef",
     "BuildSummaryTypeDef",
     "DescribeCodeCoveragesOutputTypeDef",
     "CreateWebhookInputRequestTypeDef",
     "UpdateWebhookInputRequestTypeDef",
-    "WebhookTypeDef",
     "DescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     "DescribeTestCasesInputRequestTypeDef",
     "DescribeTestCasesOutputTypeDef",
     "EnvironmentLanguageTypeDef",
     "GetReportGroupTrendOutputTypeDef",
     "ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     "ListReportsForReportGroupInputRequestTypeDef",
     "ListReportsInputListReportsPaginateTypeDef",
     "ListReportsInputRequestTypeDef",
     "ListSourceCredentialsOutputTypeDef",
-    "LogsConfigTypeDef",
+    "LogsConfigOutputTypeDef",
     "LogsLocationTypeDef",
+    "LogsConfigTypeDef",
+    "ProjectEnvironmentOutputTypeDef",
     "ProjectEnvironmentTypeDef",
+    "ProjectSourceOutputTypeDef",
     "ProjectSourceTypeDef",
+    "ReportExportConfigOutputTypeDef",
     "ReportExportConfigTypeDef",
+    "WebhookTypeDef",
     "BuildGroupTypeDef",
-    "CreateWebhookOutputTypeDef",
-    "UpdateWebhookOutputTypeDef",
     "EnvironmentPlatformTypeDef",
     "BuildTypeDef",
     "CreateProjectInputRequestTypeDef",
-    "ProjectTypeDef",
     "StartBuildBatchInputRequestTypeDef",
     "StartBuildInputRequestTypeDef",
     "UpdateProjectInputRequestTypeDef",
-    "CreateReportGroupInputRequestTypeDef",
     "ReportGroupTypeDef",
     "ReportTypeDef",
+    "CreateReportGroupInputRequestTypeDef",
     "UpdateReportGroupInputRequestTypeDef",
+    "CreateWebhookOutputTypeDef",
+    "ProjectTypeDef",
+    "UpdateWebhookOutputTypeDef",
     "BuildBatchTypeDef",
     "ListCuratedEnvironmentImagesOutputTypeDef",
     "BatchGetBuildsOutputTypeDef",
     "RetryBuildOutputTypeDef",
     "StartBuildOutputTypeDef",
     "StopBuildOutputTypeDef",
-    "BatchGetProjectsOutputTypeDef",
-    "CreateProjectOutputTypeDef",
-    "UpdateProjectOutputTypeDef",
     "BatchGetReportGroupsOutputTypeDef",
     "CreateReportGroupOutputTypeDef",
     "UpdateReportGroupOutputTypeDef",
     "BatchGetReportsOutputTypeDef",
+    "BatchGetProjectsOutputTypeDef",
+    "CreateProjectOutputTypeDef",
+    "UpdateProjectOutputTypeDef",
     "BatchGetBuildBatchesOutputTypeDef",
     "RetryBuildBatchOutputTypeDef",
     "StartBuildBatchOutputTypeDef",
     "StopBuildBatchOutputTypeDef",
 )
 
 BatchDeleteBuildsInputRequestTypeDef = TypedDict(
@@ -262,19 +283,28 @@
 BatchGetReportsInputRequestTypeDef = TypedDict(
     "BatchGetReportsInputRequestTypeDef",
     {
         "reportArns": Sequence[str],
     },
 )
 
+BatchRestrictionsOutputTypeDef = TypedDict(
+    "BatchRestrictionsOutputTypeDef",
+    {
+        "maximumBuildsAllowed": int,
+        "computeTypesAllowed": List[str],
+    },
+    total=False,
+)
+
 BatchRestrictionsTypeDef = TypedDict(
     "BatchRestrictionsTypeDef",
     {
         "maximumBuildsAllowed": int,
-        "computeTypesAllowed": List[str],
+        "computeTypesAllowed": Sequence[str],
     },
     total=False,
 )
 
 BuildArtifactsTypeDef = TypedDict(
     "BuildArtifactsTypeDef",
     {
@@ -302,64 +332,75 @@
     {
         "statusCode": str,
         "message": str,
     },
     total=False,
 )
 
-_RequiredProjectCacheTypeDef = TypedDict(
-    "_RequiredProjectCacheTypeDef",
+_RequiredProjectCacheOutputTypeDef = TypedDict(
+    "_RequiredProjectCacheOutputTypeDef",
     {
         "type": CacheTypeType,
     },
 )
-_OptionalProjectCacheTypeDef = TypedDict(
-    "_OptionalProjectCacheTypeDef",
+_OptionalProjectCacheOutputTypeDef = TypedDict(
+    "_OptionalProjectCacheOutputTypeDef",
     {
         "location": str,
         "modes": List[CacheModeType],
     },
     total=False,
 )
 
 
-class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
+class ProjectCacheOutputTypeDef(
+    _RequiredProjectCacheOutputTypeDef, _OptionalProjectCacheOutputTypeDef
+):
     pass
 
 
-ProjectFileSystemLocationTypeDef = TypedDict(
-    "ProjectFileSystemLocationTypeDef",
+ProjectFileSystemLocationOutputTypeDef = TypedDict(
+    "ProjectFileSystemLocationOutputTypeDef",
     {
         "type": Literal["EFS"],
         "location": str,
         "mountPoint": str,
         "identifier": str,
         "mountOptions": str,
     },
     total=False,
 )
 
-ProjectSourceVersionTypeDef = TypedDict(
-    "ProjectSourceVersionTypeDef",
+ProjectSourceVersionOutputTypeDef = TypedDict(
+    "ProjectSourceVersionOutputTypeDef",
     {
         "sourceIdentifier": str,
         "sourceVersion": str,
     },
 )
 
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
     {
         "vpcId": str,
         "subnets": List[str],
         "securityGroupIds": List[str],
     },
     total=False,
 )
 
+BuildStatusConfigOutputTypeDef = TypedDict(
+    "BuildStatusConfigOutputTypeDef",
+    {
+        "context": str,
+        "targetUrl": str,
+    },
+    total=False,
+)
+
 BuildStatusConfigTypeDef = TypedDict(
     "BuildStatusConfigTypeDef",
     {
         "context": str,
         "targetUrl": str,
     },
     total=False,
@@ -398,14 +439,36 @@
     {
         "subnetId": str,
         "networkInterfaceId": str,
     },
     total=False,
 )
 
+_RequiredCloudWatchLogsConfigOutputTypeDef = TypedDict(
+    "_RequiredCloudWatchLogsConfigOutputTypeDef",
+    {
+        "status": LogsConfigStatusTypeType,
+    },
+)
+_OptionalCloudWatchLogsConfigOutputTypeDef = TypedDict(
+    "_OptionalCloudWatchLogsConfigOutputTypeDef",
+    {
+        "groupName": str,
+        "streamName": str,
+    },
+    total=False,
+)
+
+
+class CloudWatchLogsConfigOutputTypeDef(
+    _RequiredCloudWatchLogsConfigOutputTypeDef, _OptionalCloudWatchLogsConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredCloudWatchLogsConfigTypeDef = TypedDict(
     "_RequiredCloudWatchLogsConfigTypeDef",
     {
         "status": LogsConfigStatusTypeType,
     },
 )
 _OptionalCloudWatchLogsConfigTypeDef = TypedDict(
@@ -477,23 +540,73 @@
 )
 
 
 class ProjectArtifactsTypeDef(_RequiredProjectArtifactsTypeDef, _OptionalProjectArtifactsTypeDef):
     pass
 
 
+_RequiredProjectCacheTypeDef = TypedDict(
+    "_RequiredProjectCacheTypeDef",
+    {
+        "type": CacheTypeType,
+    },
+)
+_OptionalProjectCacheTypeDef = TypedDict(
+    "_OptionalProjectCacheTypeDef",
+    {
+        "location": str,
+        "modes": Sequence[CacheModeType],
+    },
+    total=False,
+)
+
+
+class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
+    pass
+
+
+ProjectFileSystemLocationTypeDef = TypedDict(
+    "ProjectFileSystemLocationTypeDef",
+    {
+        "type": Literal["EFS"],
+        "location": str,
+        "mountPoint": str,
+        "identifier": str,
+        "mountOptions": str,
+    },
+    total=False,
+)
+
+ProjectSourceVersionTypeDef = TypedDict(
+    "ProjectSourceVersionTypeDef",
+    {
+        "sourceIdentifier": str,
+        "sourceVersion": str,
+    },
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "vpcId": str,
+        "subnets": Sequence[str],
+        "securityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredWebhookFilterTypeDef = TypedDict(
     "_RequiredWebhookFilterTypeDef",
     {
         "type": WebhookFilterTypeType,
         "pattern": str,
     },
 )
@@ -664,14 +777,36 @@
         "name": str,
         "description": str,
         "versions": List[str],
     },
     total=False,
 )
 
+_RequiredEnvironmentVariableOutputTypeDef = TypedDict(
+    "_RequiredEnvironmentVariableOutputTypeDef",
+    {
+        "name": str,
+        "value": str,
+    },
+)
+_OptionalEnvironmentVariableOutputTypeDef = TypedDict(
+    "_OptionalEnvironmentVariableOutputTypeDef",
+    {
+        "type": EnvironmentVariableTypeType,
+    },
+    total=False,
+)
+
+
+class EnvironmentVariableOutputTypeDef(
+    _RequiredEnvironmentVariableOutputTypeDef, _OptionalEnvironmentVariableOutputTypeDef
+):
+    pass
+
+
 _RequiredEnvironmentVariableTypeDef = TypedDict(
     "_RequiredEnvironmentVariableTypeDef",
     {
         "name": str,
         "value": str,
     },
 )
@@ -742,14 +877,21 @@
     "GetResourcePolicyOutputTypeDef",
     {
         "policy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GitSubmodulesConfigOutputTypeDef = TypedDict(
+    "GitSubmodulesConfigOutputTypeDef",
+    {
+        "fetchSubmodules": bool,
+    },
+)
+
 GitSubmodulesConfigTypeDef = TypedDict(
     "GitSubmodulesConfigTypeDef",
     {
         "fetchSubmodules": bool,
     },
 )
 
@@ -1044,14 +1186,37 @@
         "arn": str,
         "serverType": ServerTypeType,
         "authType": AuthTypeType,
     },
     total=False,
 )
 
+_RequiredS3LogsConfigOutputTypeDef = TypedDict(
+    "_RequiredS3LogsConfigOutputTypeDef",
+    {
+        "status": LogsConfigStatusTypeType,
+    },
+)
+_OptionalS3LogsConfigOutputTypeDef = TypedDict(
+    "_OptionalS3LogsConfigOutputTypeDef",
+    {
+        "location": str,
+        "encryptionDisabled": bool,
+        "bucketOwnerAccess": BucketOwnerAccessType,
+    },
+    total=False,
+)
+
+
+class S3LogsConfigOutputTypeDef(
+    _RequiredS3LogsConfigOutputTypeDef, _OptionalS3LogsConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredS3LogsConfigTypeDef = TypedDict(
     "_RequiredS3LogsConfigTypeDef",
     {
         "status": LogsConfigStatusTypeType,
     },
 )
 _OptionalS3LogsConfigTypeDef = TypedDict(
@@ -1075,31 +1240,87 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredProjectArtifactsOutputTypeDef = TypedDict(
+    "_RequiredProjectArtifactsOutputTypeDef",
+    {
+        "type": ArtifactsTypeType,
+    },
+)
+_OptionalProjectArtifactsOutputTypeDef = TypedDict(
+    "_OptionalProjectArtifactsOutputTypeDef",
+    {
+        "location": str,
+        "path": str,
+        "namespaceType": ArtifactNamespaceType,
+        "name": str,
+        "packaging": ArtifactPackagingType,
+        "overrideArtifactName": bool,
+        "encryptionDisabled": bool,
+        "artifactIdentifier": str,
+        "bucketOwnerAccess": BucketOwnerAccessType,
+    },
+    total=False,
+)
+
+
+class ProjectArtifactsOutputTypeDef(
+    _RequiredProjectArtifactsOutputTypeDef, _OptionalProjectArtifactsOutputTypeDef
+):
+    pass
+
+
 ProjectBadgeTypeDef = TypedDict(
     "ProjectBadgeTypeDef",
     {
         "badgeEnabled": bool,
         "badgeRequestUrl": str,
     },
     total=False,
 )
 
+RegistryCredentialOutputTypeDef = TypedDict(
+    "RegistryCredentialOutputTypeDef",
+    {
+        "credential": str,
+        "credentialProvider": Literal["SECRETS_MANAGER"],
+    },
+)
+
 RegistryCredentialTypeDef = TypedDict(
     "RegistryCredentialTypeDef",
     {
         "credential": str,
         "credentialProvider": Literal["SECRETS_MANAGER"],
     },
 )
 
+_RequiredSourceAuthOutputTypeDef = TypedDict(
+    "_RequiredSourceAuthOutputTypeDef",
+    {
+        "type": Literal["OAUTH"],
+    },
+)
+_OptionalSourceAuthOutputTypeDef = TypedDict(
+    "_OptionalSourceAuthOutputTypeDef",
+    {
+        "resource": str,
+    },
+    total=False,
+)
+
+
+class SourceAuthOutputTypeDef(_RequiredSourceAuthOutputTypeDef, _OptionalSourceAuthOutputTypeDef):
+    pass
+
+
 _RequiredSourceAuthTypeDef = TypedDict(
     "_RequiredSourceAuthTypeDef",
     {
         "type": Literal["OAUTH"],
     },
 )
 _OptionalSourceAuthTypeDef = TypedDict(
@@ -1111,14 +1332,23 @@
 )
 
 
 class SourceAuthTypeDef(_RequiredSourceAuthTypeDef, _OptionalSourceAuthTypeDef):
     pass
 
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 PutResourcePolicyInputRequestTypeDef = TypedDict(
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
@@ -1127,14 +1357,27 @@
     "PutResourcePolicyOutputTypeDef",
     {
         "resourceArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+S3ReportExportConfigOutputTypeDef = TypedDict(
+    "S3ReportExportConfigOutputTypeDef",
+    {
+        "bucket": str,
+        "bucketOwner": str,
+        "path": str,
+        "packaging": ReportPackagingTypeType,
+        "encryptionKey": str,
+        "encryptionDisabled": bool,
+    },
+    total=False,
+)
+
 S3ReportExportConfigTypeDef = TypedDict(
     "S3ReportExportConfigTypeDef",
     {
         "bucket": str,
         "bucketOwner": str,
         "path": str,
         "packaging": ReportPackagingTypeType,
@@ -1226,14 +1469,36 @@
         "projectArn": str,
         "publicProjectAlias": str,
         "projectVisibility": ProjectVisibilityTypeType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredWebhookFilterOutputTypeDef = TypedDict(
+    "_RequiredWebhookFilterOutputTypeDef",
+    {
+        "type": WebhookFilterTypeType,
+        "pattern": str,
+    },
+)
+_OptionalWebhookFilterOutputTypeDef = TypedDict(
+    "_OptionalWebhookFilterOutputTypeDef",
+    {
+        "excludeMatchedPattern": bool,
+    },
+    total=False,
+)
+
+
+class WebhookFilterOutputTypeDef(
+    _RequiredWebhookFilterOutputTypeDef, _OptionalWebhookFilterOutputTypeDef
+):
+    pass
+
+
 BatchDeleteBuildsOutputTypeDef = TypedDict(
     "BatchDeleteBuildsOutputTypeDef",
     {
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1245,14 +1510,26 @@
         "statusCode": str,
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ProjectBuildBatchConfigOutputTypeDef = TypedDict(
+    "ProjectBuildBatchConfigOutputTypeDef",
+    {
+        "serviceRole": str,
+        "combineArtifacts": bool,
+        "restrictions": BatchRestrictionsOutputTypeDef,
+        "timeoutInMins": int,
+        "batchReportMode": BatchReportModeTypeType,
+    },
+    total=False,
+)
+
 ProjectBuildBatchConfigTypeDef = TypedDict(
     "ProjectBuildBatchConfigTypeDef",
     {
         "serviceRole": str,
         "combineArtifacts": bool,
         "restrictions": BatchRestrictionsTypeDef,
         "timeoutInMins": int,
@@ -1395,28 +1672,14 @@
 
 class UpdateWebhookInputRequestTypeDef(
     _RequiredUpdateWebhookInputRequestTypeDef, _OptionalUpdateWebhookInputRequestTypeDef
 ):
     pass
 
 
-WebhookTypeDef = TypedDict(
-    "WebhookTypeDef",
-    {
-        "url": str,
-        "payloadUrl": str,
-        "secret": str,
-        "branchFilter": str,
-        "filterGroups": List[List[WebhookFilterTypeDef]],
-        "buildType": WebhookBuildTypeType,
-        "lastModifiedSecret": datetime,
-    },
-    total=False,
-)
-
 _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
@@ -1560,50 +1823,86 @@
     "ListSourceCredentialsOutputTypeDef",
     {
         "sourceCredentialsInfos": List[SourceCredentialsInfoTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-LogsConfigTypeDef = TypedDict(
-    "LogsConfigTypeDef",
+LogsConfigOutputTypeDef = TypedDict(
+    "LogsConfigOutputTypeDef",
     {
-        "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
-        "s3Logs": S3LogsConfigTypeDef,
+        "cloudWatchLogs": CloudWatchLogsConfigOutputTypeDef,
+        "s3Logs": S3LogsConfigOutputTypeDef,
     },
     total=False,
 )
 
 LogsLocationTypeDef = TypedDict(
     "LogsLocationTypeDef",
     {
         "groupName": str,
         "streamName": str,
         "deepLink": str,
         "s3DeepLink": str,
         "cloudWatchLogsArn": str,
         "s3LogsArn": str,
+        "cloudWatchLogs": CloudWatchLogsConfigOutputTypeDef,
+        "s3Logs": S3LogsConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+LogsConfigTypeDef = TypedDict(
+    "LogsConfigTypeDef",
+    {
         "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
         "s3Logs": S3LogsConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredProjectEnvironmentOutputTypeDef = TypedDict(
+    "_RequiredProjectEnvironmentOutputTypeDef",
+    {
+        "type": EnvironmentTypeType,
+        "image": str,
+        "computeType": ComputeTypeType,
+    },
+)
+_OptionalProjectEnvironmentOutputTypeDef = TypedDict(
+    "_OptionalProjectEnvironmentOutputTypeDef",
+    {
+        "environmentVariables": List[EnvironmentVariableOutputTypeDef],
+        "privilegedMode": bool,
+        "certificate": str,
+        "registryCredential": RegistryCredentialOutputTypeDef,
+        "imagePullCredentialsType": ImagePullCredentialsTypeType,
+    },
+    total=False,
+)
+
+
+class ProjectEnvironmentOutputTypeDef(
+    _RequiredProjectEnvironmentOutputTypeDef, _OptionalProjectEnvironmentOutputTypeDef
+):
+    pass
+
+
 _RequiredProjectEnvironmentTypeDef = TypedDict(
     "_RequiredProjectEnvironmentTypeDef",
     {
         "type": EnvironmentTypeType,
         "image": str,
         "computeType": ComputeTypeType,
     },
 )
 _OptionalProjectEnvironmentTypeDef = TypedDict(
     "_OptionalProjectEnvironmentTypeDef",
     {
-        "environmentVariables": List[EnvironmentVariableTypeDef],
+        "environmentVariables": Sequence[EnvironmentVariableTypeDef],
         "privilegedMode": bool,
         "certificate": str,
         "registryCredential": RegistryCredentialTypeDef,
         "imagePullCredentialsType": ImagePullCredentialsTypeType,
     },
     total=False,
 )
@@ -1611,14 +1910,43 @@
 
 class ProjectEnvironmentTypeDef(
     _RequiredProjectEnvironmentTypeDef, _OptionalProjectEnvironmentTypeDef
 ):
     pass
 
 
+_RequiredProjectSourceOutputTypeDef = TypedDict(
+    "_RequiredProjectSourceOutputTypeDef",
+    {
+        "type": SourceTypeType,
+    },
+)
+_OptionalProjectSourceOutputTypeDef = TypedDict(
+    "_OptionalProjectSourceOutputTypeDef",
+    {
+        "location": str,
+        "gitCloneDepth": int,
+        "gitSubmodulesConfig": GitSubmodulesConfigOutputTypeDef,
+        "buildspec": str,
+        "auth": SourceAuthOutputTypeDef,
+        "reportBuildStatus": bool,
+        "buildStatusConfig": BuildStatusConfigOutputTypeDef,
+        "insecureSsl": bool,
+        "sourceIdentifier": str,
+    },
+    total=False,
+)
+
+
+class ProjectSourceOutputTypeDef(
+    _RequiredProjectSourceOutputTypeDef, _OptionalProjectSourceOutputTypeDef
+):
+    pass
+
+
 _RequiredProjectSourceTypeDef = TypedDict(
     "_RequiredProjectSourceTypeDef",
     {
         "type": SourceTypeType,
     },
 )
 _OptionalProjectSourceTypeDef = TypedDict(
@@ -1638,51 +1966,58 @@
 )
 
 
 class ProjectSourceTypeDef(_RequiredProjectSourceTypeDef, _OptionalProjectSourceTypeDef):
     pass
 
 
+ReportExportConfigOutputTypeDef = TypedDict(
+    "ReportExportConfigOutputTypeDef",
+    {
+        "exportConfigType": ReportExportConfigTypeType,
+        "s3Destination": S3ReportExportConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ReportExportConfigTypeDef = TypedDict(
     "ReportExportConfigTypeDef",
     {
         "exportConfigType": ReportExportConfigTypeType,
         "s3Destination": S3ReportExportConfigTypeDef,
     },
     total=False,
 )
 
+WebhookTypeDef = TypedDict(
+    "WebhookTypeDef",
+    {
+        "url": str,
+        "payloadUrl": str,
+        "secret": str,
+        "branchFilter": str,
+        "filterGroups": List[List[WebhookFilterOutputTypeDef]],
+        "buildType": WebhookBuildTypeType,
+        "lastModifiedSecret": datetime,
+    },
+    total=False,
+)
+
 BuildGroupTypeDef = TypedDict(
     "BuildGroupTypeDef",
     {
         "identifier": str,
         "dependsOn": List[str],
         "ignoreFailure": bool,
         "currentBuildSummary": BuildSummaryTypeDef,
         "priorBuildSummaryList": List[BuildSummaryTypeDef],
     },
     total=False,
 )
 
-CreateWebhookOutputTypeDef = TypedDict(
-    "CreateWebhookOutputTypeDef",
-    {
-        "webhook": WebhookTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateWebhookOutputTypeDef = TypedDict(
-    "UpdateWebhookOutputTypeDef",
-    {
-        "webhook": WebhookTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentPlatformTypeDef = TypedDict(
     "EnvironmentPlatformTypeDef",
     {
         "platform": PlatformTypeType,
         "languages": List[EnvironmentLanguageTypeDef],
     },
     total=False,
@@ -1698,33 +2033,33 @@
         "endTime": datetime,
         "currentPhase": str,
         "buildStatus": StatusTypeType,
         "sourceVersion": str,
         "resolvedSourceVersion": str,
         "projectName": str,
         "phases": List[BuildPhaseTypeDef],
-        "source": ProjectSourceTypeDef,
-        "secondarySources": List[ProjectSourceTypeDef],
-        "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
+        "source": ProjectSourceOutputTypeDef,
+        "secondarySources": List[ProjectSourceOutputTypeDef],
+        "secondarySourceVersions": List[ProjectSourceVersionOutputTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
-        "cache": ProjectCacheTypeDef,
-        "environment": ProjectEnvironmentTypeDef,
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
         "logs": LogsLocationTypeDef,
         "timeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "buildComplete": bool,
         "initiator": str,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "encryptionKey": str,
         "exportedEnvironmentVariables": List[ExportedEnvironmentVariableTypeDef],
         "reportArns": List[str],
-        "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
+        "fileSystemLocations": List[ProjectFileSystemLocationOutputTypeDef],
         "debugSession": DebugSessionTypeDef,
         "buildBatchArn": str,
     },
     total=False,
 )
 
 _RequiredCreateProjectInputRequestTypeDef = TypedDict(
@@ -1763,49 +2098,14 @@
 
 class CreateProjectInputRequestTypeDef(
     _RequiredCreateProjectInputRequestTypeDef, _OptionalCreateProjectInputRequestTypeDef
 ):
     pass
 
 
-ProjectTypeDef = TypedDict(
-    "ProjectTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "source": ProjectSourceTypeDef,
-        "secondarySources": List[ProjectSourceTypeDef],
-        "sourceVersion": str,
-        "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
-        "artifacts": ProjectArtifactsTypeDef,
-        "secondaryArtifacts": List[ProjectArtifactsTypeDef],
-        "cache": ProjectCacheTypeDef,
-        "environment": ProjectEnvironmentTypeDef,
-        "serviceRole": str,
-        "timeoutInMinutes": int,
-        "queuedTimeoutInMinutes": int,
-        "encryptionKey": str,
-        "tags": List[TagTypeDef],
-        "created": datetime,
-        "lastModified": datetime,
-        "webhook": WebhookTypeDef,
-        "vpcConfig": VpcConfigTypeDef,
-        "badge": ProjectBadgeTypeDef,
-        "logsConfig": LogsConfigTypeDef,
-        "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
-        "concurrentBuildLimit": int,
-        "projectVisibility": ProjectVisibilityTypeType,
-        "publicProjectAlias": str,
-        "resourceAccessRole": str,
-    },
-    total=False,
-)
-
 _RequiredStartBuildBatchInputRequestTypeDef = TypedDict(
     "_RequiredStartBuildBatchInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalStartBuildBatchInputRequestTypeDef = TypedDict(
@@ -1938,47 +2238,24 @@
 
 class UpdateProjectInputRequestTypeDef(
     _RequiredUpdateProjectInputRequestTypeDef, _OptionalUpdateProjectInputRequestTypeDef
 ):
     pass
 
 
-_RequiredCreateReportGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateReportGroupInputRequestTypeDef",
-    {
-        "name": str,
-        "type": ReportTypeType,
-        "exportConfig": ReportExportConfigTypeDef,
-    },
-)
-_OptionalCreateReportGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateReportGroupInputRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateReportGroupInputRequestTypeDef(
-    _RequiredCreateReportGroupInputRequestTypeDef, _OptionalCreateReportGroupInputRequestTypeDef
-):
-    pass
-
-
 ReportGroupTypeDef = TypedDict(
     "ReportGroupTypeDef",
     {
         "arn": str,
         "name": str,
         "type": ReportTypeType,
-        "exportConfig": ReportExportConfigTypeDef,
+        "exportConfig": ReportExportConfigOutputTypeDef,
         "created": datetime,
         "lastModified": datetime,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "status": ReportGroupStatusTypeType,
     },
     total=False,
 )
 
 ReportTypeDef = TypedDict(
     "ReportTypeDef",
@@ -1987,22 +2264,45 @@
         "type": ReportTypeType,
         "name": str,
         "reportGroupArn": str,
         "executionId": str,
         "status": ReportStatusTypeType,
         "created": datetime,
         "expired": datetime,
-        "exportConfig": ReportExportConfigTypeDef,
+        "exportConfig": ReportExportConfigOutputTypeDef,
         "truncated": bool,
         "testSummary": TestReportSummaryTypeDef,
         "codeCoverageSummary": CodeCoverageReportSummaryTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateReportGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateReportGroupInputRequestTypeDef",
+    {
+        "name": str,
+        "type": ReportTypeType,
+        "exportConfig": ReportExportConfigTypeDef,
+    },
+)
+_OptionalCreateReportGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateReportGroupInputRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateReportGroupInputRequestTypeDef(
+    _RequiredCreateReportGroupInputRequestTypeDef, _OptionalCreateReportGroupInputRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateReportGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReportGroupInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateReportGroupInputRequestTypeDef = TypedDict(
@@ -2017,45 +2317,96 @@
 
 class UpdateReportGroupInputRequestTypeDef(
     _RequiredUpdateReportGroupInputRequestTypeDef, _OptionalUpdateReportGroupInputRequestTypeDef
 ):
     pass
 
 
+CreateWebhookOutputTypeDef = TypedDict(
+    "CreateWebhookOutputTypeDef",
+    {
+        "webhook": WebhookTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ProjectTypeDef = TypedDict(
+    "ProjectTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "source": ProjectSourceOutputTypeDef,
+        "secondarySources": List[ProjectSourceOutputTypeDef],
+        "sourceVersion": str,
+        "secondarySourceVersions": List[ProjectSourceVersionOutputTypeDef],
+        "artifacts": ProjectArtifactsOutputTypeDef,
+        "secondaryArtifacts": List[ProjectArtifactsOutputTypeDef],
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
+        "serviceRole": str,
+        "timeoutInMinutes": int,
+        "queuedTimeoutInMinutes": int,
+        "encryptionKey": str,
+        "tags": List[TagOutputTypeDef],
+        "created": datetime,
+        "lastModified": datetime,
+        "webhook": WebhookTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
+        "badge": ProjectBadgeTypeDef,
+        "logsConfig": LogsConfigOutputTypeDef,
+        "fileSystemLocations": List[ProjectFileSystemLocationOutputTypeDef],
+        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
+        "concurrentBuildLimit": int,
+        "projectVisibility": ProjectVisibilityTypeType,
+        "publicProjectAlias": str,
+        "resourceAccessRole": str,
+    },
+    total=False,
+)
+
+UpdateWebhookOutputTypeDef = TypedDict(
+    "UpdateWebhookOutputTypeDef",
+    {
+        "webhook": WebhookTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BuildBatchTypeDef = TypedDict(
     "BuildBatchTypeDef",
     {
         "id": str,
         "arn": str,
         "startTime": datetime,
         "endTime": datetime,
         "currentPhase": str,
         "buildBatchStatus": StatusTypeType,
         "sourceVersion": str,
         "resolvedSourceVersion": str,
         "projectName": str,
         "phases": List[BuildBatchPhaseTypeDef],
-        "source": ProjectSourceTypeDef,
-        "secondarySources": List[ProjectSourceTypeDef],
-        "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
+        "source": ProjectSourceOutputTypeDef,
+        "secondarySources": List[ProjectSourceOutputTypeDef],
+        "secondarySourceVersions": List[ProjectSourceVersionOutputTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
-        "cache": ProjectCacheTypeDef,
-        "environment": ProjectEnvironmentTypeDef,
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
-        "logConfig": LogsConfigTypeDef,
+        "logConfig": LogsConfigOutputTypeDef,
         "buildTimeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "complete": bool,
         "initiator": str,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
         "encryptionKey": str,
         "buildBatchNumber": int,
-        "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
+        "fileSystemLocations": List[ProjectFileSystemLocationOutputTypeDef],
+        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
         "buildGroups": List[BuildGroupTypeDef],
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
 ListCuratedEnvironmentImagesOutputTypeDef = TypedDict(
@@ -2095,69 +2446,69 @@
     "StopBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BatchGetProjectsOutputTypeDef = TypedDict(
-    "BatchGetProjectsOutputTypeDef",
+BatchGetReportGroupsOutputTypeDef = TypedDict(
+    "BatchGetReportGroupsOutputTypeDef",
     {
-        "projects": List[ProjectTypeDef],
-        "projectsNotFound": List[str],
+        "reportGroups": List[ReportGroupTypeDef],
+        "reportGroupsNotFound": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateProjectOutputTypeDef = TypedDict(
-    "CreateProjectOutputTypeDef",
+CreateReportGroupOutputTypeDef = TypedDict(
+    "CreateReportGroupOutputTypeDef",
     {
-        "project": ProjectTypeDef,
+        "reportGroup": ReportGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateProjectOutputTypeDef = TypedDict(
-    "UpdateProjectOutputTypeDef",
+UpdateReportGroupOutputTypeDef = TypedDict(
+    "UpdateReportGroupOutputTypeDef",
     {
-        "project": ProjectTypeDef,
+        "reportGroup": ReportGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BatchGetReportGroupsOutputTypeDef = TypedDict(
-    "BatchGetReportGroupsOutputTypeDef",
+BatchGetReportsOutputTypeDef = TypedDict(
+    "BatchGetReportsOutputTypeDef",
     {
-        "reportGroups": List[ReportGroupTypeDef],
-        "reportGroupsNotFound": List[str],
+        "reports": List[ReportTypeDef],
+        "reportsNotFound": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReportGroupOutputTypeDef = TypedDict(
-    "CreateReportGroupOutputTypeDef",
+BatchGetProjectsOutputTypeDef = TypedDict(
+    "BatchGetProjectsOutputTypeDef",
     {
-        "reportGroup": ReportGroupTypeDef,
+        "projects": List[ProjectTypeDef],
+        "projectsNotFound": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateReportGroupOutputTypeDef = TypedDict(
-    "UpdateReportGroupOutputTypeDef",
+CreateProjectOutputTypeDef = TypedDict(
+    "CreateProjectOutputTypeDef",
     {
-        "reportGroup": ReportGroupTypeDef,
+        "project": ProjectTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BatchGetReportsOutputTypeDef = TypedDict(
-    "BatchGetReportsOutputTypeDef",
+UpdateProjectOutputTypeDef = TypedDict(
+    "UpdateProjectOutputTypeDef",
     {
-        "reports": List[ReportTypeDef],
-        "reportsNotFound": List[str],
+        "project": ProjectTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetBuildBatchesOutputTypeDef = TypedDict(
     "BatchGetBuildBatchesOutputTypeDef",
     {
```

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild/type_defs.pyi` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -66,52 +66,61 @@
     "BatchDeleteBuildsInputRequestTypeDef",
     "BuildNotDeletedTypeDef",
     "BatchGetBuildBatchesInputRequestTypeDef",
     "BatchGetBuildsInputRequestTypeDef",
     "BatchGetProjectsInputRequestTypeDef",
     "BatchGetReportGroupsInputRequestTypeDef",
     "BatchGetReportsInputRequestTypeDef",
+    "BatchRestrictionsOutputTypeDef",
     "BatchRestrictionsTypeDef",
     "BuildArtifactsTypeDef",
     "BuildBatchFilterTypeDef",
     "PhaseContextTypeDef",
-    "ProjectCacheTypeDef",
-    "ProjectFileSystemLocationTypeDef",
-    "ProjectSourceVersionTypeDef",
-    "VpcConfigTypeDef",
+    "ProjectCacheOutputTypeDef",
+    "ProjectFileSystemLocationOutputTypeDef",
+    "ProjectSourceVersionOutputTypeDef",
+    "VpcConfigOutputTypeDef",
+    "BuildStatusConfigOutputTypeDef",
     "BuildStatusConfigTypeDef",
     "ResolvedArtifactTypeDef",
     "DebugSessionTypeDef",
     "ExportedEnvironmentVariableTypeDef",
     "NetworkInterfaceTypeDef",
+    "CloudWatchLogsConfigOutputTypeDef",
     "CloudWatchLogsConfigTypeDef",
     "CodeCoverageReportSummaryTypeDef",
     "CodeCoverageTypeDef",
     "ProjectArtifactsTypeDef",
+    "ProjectCacheTypeDef",
+    "ProjectFileSystemLocationTypeDef",
+    "ProjectSourceVersionTypeDef",
     "TagTypeDef",
+    "VpcConfigTypeDef",
     "WebhookFilterTypeDef",
     "DeleteBuildBatchInputRequestTypeDef",
     "DeleteProjectInputRequestTypeDef",
     "DeleteReportGroupInputRequestTypeDef",
     "DeleteReportInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteSourceCredentialsInputRequestTypeDef",
     "DeleteSourceCredentialsOutputTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
     "DescribeCodeCoveragesInputRequestTypeDef",
     "TestCaseFilterTypeDef",
     "TestCaseTypeDef",
     "EnvironmentImageTypeDef",
+    "EnvironmentVariableOutputTypeDef",
     "EnvironmentVariableTypeDef",
     "GetReportGroupTrendInputRequestTypeDef",
     "ReportGroupTrendStatsTypeDef",
     "ReportWithRawDataTypeDef",
     "GetResourcePolicyInputRequestTypeDef",
     "GetResourcePolicyOutputTypeDef",
+    "GitSubmodulesConfigOutputTypeDef",
     "GitSubmodulesConfigTypeDef",
     "ImportSourceCredentialsInputRequestTypeDef",
     "ImportSourceCredentialsOutputTypeDef",
     "InvalidateProjectCacheInputRequestTypeDef",
     "ListBuildBatchesForProjectOutputTypeDef",
     "ListBuildBatchesOutputTypeDef",
     "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
@@ -132,86 +141,98 @@
     "ListSharedProjectsInputListSharedProjectsPaginateTypeDef",
     "ListSharedProjectsInputRequestTypeDef",
     "ListSharedProjectsOutputTypeDef",
     "ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef",
     "ListSharedReportGroupsInputRequestTypeDef",
     "ListSharedReportGroupsOutputTypeDef",
     "SourceCredentialsInfoTypeDef",
+    "S3LogsConfigOutputTypeDef",
     "S3LogsConfigTypeDef",
     "PaginatorConfigTypeDef",
+    "ProjectArtifactsOutputTypeDef",
     "ProjectBadgeTypeDef",
+    "RegistryCredentialOutputTypeDef",
     "RegistryCredentialTypeDef",
+    "SourceAuthOutputTypeDef",
     "SourceAuthTypeDef",
+    "TagOutputTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
     "PutResourcePolicyOutputTypeDef",
+    "S3ReportExportConfigOutputTypeDef",
     "S3ReportExportConfigTypeDef",
     "TestReportSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "RetryBuildBatchInputRequestTypeDef",
     "RetryBuildInputRequestTypeDef",
     "StopBuildBatchInputRequestTypeDef",
     "StopBuildInputRequestTypeDef",
     "UpdateProjectVisibilityInputRequestTypeDef",
     "UpdateProjectVisibilityOutputTypeDef",
+    "WebhookFilterOutputTypeDef",
     "BatchDeleteBuildsOutputTypeDef",
     "DeleteBuildBatchOutputTypeDef",
+    "ProjectBuildBatchConfigOutputTypeDef",
     "ProjectBuildBatchConfigTypeDef",
     "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     "ListBuildBatchesForProjectInputRequestTypeDef",
     "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
     "ListBuildBatchesInputRequestTypeDef",
     "BuildBatchPhaseTypeDef",
     "BuildPhaseTypeDef",
     "BuildSummaryTypeDef",
     "DescribeCodeCoveragesOutputTypeDef",
     "CreateWebhookInputRequestTypeDef",
     "UpdateWebhookInputRequestTypeDef",
-    "WebhookTypeDef",
     "DescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     "DescribeTestCasesInputRequestTypeDef",
     "DescribeTestCasesOutputTypeDef",
     "EnvironmentLanguageTypeDef",
     "GetReportGroupTrendOutputTypeDef",
     "ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     "ListReportsForReportGroupInputRequestTypeDef",
     "ListReportsInputListReportsPaginateTypeDef",
     "ListReportsInputRequestTypeDef",
     "ListSourceCredentialsOutputTypeDef",
-    "LogsConfigTypeDef",
+    "LogsConfigOutputTypeDef",
     "LogsLocationTypeDef",
+    "LogsConfigTypeDef",
+    "ProjectEnvironmentOutputTypeDef",
     "ProjectEnvironmentTypeDef",
+    "ProjectSourceOutputTypeDef",
     "ProjectSourceTypeDef",
+    "ReportExportConfigOutputTypeDef",
     "ReportExportConfigTypeDef",
+    "WebhookTypeDef",
     "BuildGroupTypeDef",
-    "CreateWebhookOutputTypeDef",
-    "UpdateWebhookOutputTypeDef",
     "EnvironmentPlatformTypeDef",
     "BuildTypeDef",
     "CreateProjectInputRequestTypeDef",
-    "ProjectTypeDef",
     "StartBuildBatchInputRequestTypeDef",
     "StartBuildInputRequestTypeDef",
     "UpdateProjectInputRequestTypeDef",
-    "CreateReportGroupInputRequestTypeDef",
     "ReportGroupTypeDef",
     "ReportTypeDef",
+    "CreateReportGroupInputRequestTypeDef",
     "UpdateReportGroupInputRequestTypeDef",
+    "CreateWebhookOutputTypeDef",
+    "ProjectTypeDef",
+    "UpdateWebhookOutputTypeDef",
     "BuildBatchTypeDef",
     "ListCuratedEnvironmentImagesOutputTypeDef",
     "BatchGetBuildsOutputTypeDef",
     "RetryBuildOutputTypeDef",
     "StartBuildOutputTypeDef",
     "StopBuildOutputTypeDef",
-    "BatchGetProjectsOutputTypeDef",
-    "CreateProjectOutputTypeDef",
-    "UpdateProjectOutputTypeDef",
     "BatchGetReportGroupsOutputTypeDef",
     "CreateReportGroupOutputTypeDef",
     "UpdateReportGroupOutputTypeDef",
     "BatchGetReportsOutputTypeDef",
+    "BatchGetProjectsOutputTypeDef",
+    "CreateProjectOutputTypeDef",
+    "UpdateProjectOutputTypeDef",
     "BatchGetBuildBatchesOutputTypeDef",
     "RetryBuildBatchOutputTypeDef",
     "StartBuildBatchOutputTypeDef",
     "StopBuildBatchOutputTypeDef",
 )
 
 BatchDeleteBuildsInputRequestTypeDef = TypedDict(
@@ -261,19 +282,28 @@
 BatchGetReportsInputRequestTypeDef = TypedDict(
     "BatchGetReportsInputRequestTypeDef",
     {
         "reportArns": Sequence[str],
     },
 )
 
+BatchRestrictionsOutputTypeDef = TypedDict(
+    "BatchRestrictionsOutputTypeDef",
+    {
+        "maximumBuildsAllowed": int,
+        "computeTypesAllowed": List[str],
+    },
+    total=False,
+)
+
 BatchRestrictionsTypeDef = TypedDict(
     "BatchRestrictionsTypeDef",
     {
         "maximumBuildsAllowed": int,
-        "computeTypesAllowed": List[str],
+        "computeTypesAllowed": Sequence[str],
     },
     total=False,
 )
 
 BuildArtifactsTypeDef = TypedDict(
     "BuildArtifactsTypeDef",
     {
@@ -301,62 +331,73 @@
     {
         "statusCode": str,
         "message": str,
     },
     total=False,
 )
 
-_RequiredProjectCacheTypeDef = TypedDict(
-    "_RequiredProjectCacheTypeDef",
+_RequiredProjectCacheOutputTypeDef = TypedDict(
+    "_RequiredProjectCacheOutputTypeDef",
     {
         "type": CacheTypeType,
     },
 )
-_OptionalProjectCacheTypeDef = TypedDict(
-    "_OptionalProjectCacheTypeDef",
+_OptionalProjectCacheOutputTypeDef = TypedDict(
+    "_OptionalProjectCacheOutputTypeDef",
     {
         "location": str,
         "modes": List[CacheModeType],
     },
     total=False,
 )
 
-class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
+class ProjectCacheOutputTypeDef(
+    _RequiredProjectCacheOutputTypeDef, _OptionalProjectCacheOutputTypeDef
+):
     pass
 
-ProjectFileSystemLocationTypeDef = TypedDict(
-    "ProjectFileSystemLocationTypeDef",
+ProjectFileSystemLocationOutputTypeDef = TypedDict(
+    "ProjectFileSystemLocationOutputTypeDef",
     {
         "type": Literal["EFS"],
         "location": str,
         "mountPoint": str,
         "identifier": str,
         "mountOptions": str,
     },
     total=False,
 )
 
-ProjectSourceVersionTypeDef = TypedDict(
-    "ProjectSourceVersionTypeDef",
+ProjectSourceVersionOutputTypeDef = TypedDict(
+    "ProjectSourceVersionOutputTypeDef",
     {
         "sourceIdentifier": str,
         "sourceVersion": str,
     },
 )
 
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
     {
         "vpcId": str,
         "subnets": List[str],
         "securityGroupIds": List[str],
     },
     total=False,
 )
 
+BuildStatusConfigOutputTypeDef = TypedDict(
+    "BuildStatusConfigOutputTypeDef",
+    {
+        "context": str,
+        "targetUrl": str,
+    },
+    total=False,
+)
+
 BuildStatusConfigTypeDef = TypedDict(
     "BuildStatusConfigTypeDef",
     {
         "context": str,
         "targetUrl": str,
     },
     total=False,
@@ -395,14 +436,34 @@
     {
         "subnetId": str,
         "networkInterfaceId": str,
     },
     total=False,
 )
 
+_RequiredCloudWatchLogsConfigOutputTypeDef = TypedDict(
+    "_RequiredCloudWatchLogsConfigOutputTypeDef",
+    {
+        "status": LogsConfigStatusTypeType,
+    },
+)
+_OptionalCloudWatchLogsConfigOutputTypeDef = TypedDict(
+    "_OptionalCloudWatchLogsConfigOutputTypeDef",
+    {
+        "groupName": str,
+        "streamName": str,
+    },
+    total=False,
+)
+
+class CloudWatchLogsConfigOutputTypeDef(
+    _RequiredCloudWatchLogsConfigOutputTypeDef, _OptionalCloudWatchLogsConfigOutputTypeDef
+):
+    pass
+
 _RequiredCloudWatchLogsConfigTypeDef = TypedDict(
     "_RequiredCloudWatchLogsConfigTypeDef",
     {
         "status": LogsConfigStatusTypeType,
     },
 )
 _OptionalCloudWatchLogsConfigTypeDef = TypedDict(
@@ -470,23 +531,71 @@
     },
     total=False,
 )
 
 class ProjectArtifactsTypeDef(_RequiredProjectArtifactsTypeDef, _OptionalProjectArtifactsTypeDef):
     pass
 
+_RequiredProjectCacheTypeDef = TypedDict(
+    "_RequiredProjectCacheTypeDef",
+    {
+        "type": CacheTypeType,
+    },
+)
+_OptionalProjectCacheTypeDef = TypedDict(
+    "_OptionalProjectCacheTypeDef",
+    {
+        "location": str,
+        "modes": Sequence[CacheModeType],
+    },
+    total=False,
+)
+
+class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
+    pass
+
+ProjectFileSystemLocationTypeDef = TypedDict(
+    "ProjectFileSystemLocationTypeDef",
+    {
+        "type": Literal["EFS"],
+        "location": str,
+        "mountPoint": str,
+        "identifier": str,
+        "mountOptions": str,
+    },
+    total=False,
+)
+
+ProjectSourceVersionTypeDef = TypedDict(
+    "ProjectSourceVersionTypeDef",
+    {
+        "sourceIdentifier": str,
+        "sourceVersion": str,
+    },
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
+    {
+        "vpcId": str,
+        "subnets": Sequence[str],
+        "securityGroupIds": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredWebhookFilterTypeDef = TypedDict(
     "_RequiredWebhookFilterTypeDef",
     {
         "type": WebhookFilterTypeType,
         "pattern": str,
     },
 )
@@ -649,14 +758,34 @@
         "name": str,
         "description": str,
         "versions": List[str],
     },
     total=False,
 )
 
+_RequiredEnvironmentVariableOutputTypeDef = TypedDict(
+    "_RequiredEnvironmentVariableOutputTypeDef",
+    {
+        "name": str,
+        "value": str,
+    },
+)
+_OptionalEnvironmentVariableOutputTypeDef = TypedDict(
+    "_OptionalEnvironmentVariableOutputTypeDef",
+    {
+        "type": EnvironmentVariableTypeType,
+    },
+    total=False,
+)
+
+class EnvironmentVariableOutputTypeDef(
+    _RequiredEnvironmentVariableOutputTypeDef, _OptionalEnvironmentVariableOutputTypeDef
+):
+    pass
+
 _RequiredEnvironmentVariableTypeDef = TypedDict(
     "_RequiredEnvironmentVariableTypeDef",
     {
         "name": str,
         "value": str,
     },
 )
@@ -723,14 +852,21 @@
     "GetResourcePolicyOutputTypeDef",
     {
         "policy": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GitSubmodulesConfigOutputTypeDef = TypedDict(
+    "GitSubmodulesConfigOutputTypeDef",
+    {
+        "fetchSubmodules": bool,
+    },
+)
+
 GitSubmodulesConfigTypeDef = TypedDict(
     "GitSubmodulesConfigTypeDef",
     {
         "fetchSubmodules": bool,
     },
 )
 
@@ -1019,14 +1155,35 @@
         "arn": str,
         "serverType": ServerTypeType,
         "authType": AuthTypeType,
     },
     total=False,
 )
 
+_RequiredS3LogsConfigOutputTypeDef = TypedDict(
+    "_RequiredS3LogsConfigOutputTypeDef",
+    {
+        "status": LogsConfigStatusTypeType,
+    },
+)
+_OptionalS3LogsConfigOutputTypeDef = TypedDict(
+    "_OptionalS3LogsConfigOutputTypeDef",
+    {
+        "location": str,
+        "encryptionDisabled": bool,
+        "bucketOwnerAccess": BucketOwnerAccessType,
+    },
+    total=False,
+)
+
+class S3LogsConfigOutputTypeDef(
+    _RequiredS3LogsConfigOutputTypeDef, _OptionalS3LogsConfigOutputTypeDef
+):
+    pass
+
 _RequiredS3LogsConfigTypeDef = TypedDict(
     "_RequiredS3LogsConfigTypeDef",
     {
         "status": LogsConfigStatusTypeType,
     },
 )
 _OptionalS3LogsConfigTypeDef = TypedDict(
@@ -1048,31 +1205,83 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredProjectArtifactsOutputTypeDef = TypedDict(
+    "_RequiredProjectArtifactsOutputTypeDef",
+    {
+        "type": ArtifactsTypeType,
+    },
+)
+_OptionalProjectArtifactsOutputTypeDef = TypedDict(
+    "_OptionalProjectArtifactsOutputTypeDef",
+    {
+        "location": str,
+        "path": str,
+        "namespaceType": ArtifactNamespaceType,
+        "name": str,
+        "packaging": ArtifactPackagingType,
+        "overrideArtifactName": bool,
+        "encryptionDisabled": bool,
+        "artifactIdentifier": str,
+        "bucketOwnerAccess": BucketOwnerAccessType,
+    },
+    total=False,
+)
+
+class ProjectArtifactsOutputTypeDef(
+    _RequiredProjectArtifactsOutputTypeDef, _OptionalProjectArtifactsOutputTypeDef
+):
+    pass
+
 ProjectBadgeTypeDef = TypedDict(
     "ProjectBadgeTypeDef",
     {
         "badgeEnabled": bool,
         "badgeRequestUrl": str,
     },
     total=False,
 )
 
+RegistryCredentialOutputTypeDef = TypedDict(
+    "RegistryCredentialOutputTypeDef",
+    {
+        "credential": str,
+        "credentialProvider": Literal["SECRETS_MANAGER"],
+    },
+)
+
 RegistryCredentialTypeDef = TypedDict(
     "RegistryCredentialTypeDef",
     {
         "credential": str,
         "credentialProvider": Literal["SECRETS_MANAGER"],
     },
 )
 
+_RequiredSourceAuthOutputTypeDef = TypedDict(
+    "_RequiredSourceAuthOutputTypeDef",
+    {
+        "type": Literal["OAUTH"],
+    },
+)
+_OptionalSourceAuthOutputTypeDef = TypedDict(
+    "_OptionalSourceAuthOutputTypeDef",
+    {
+        "resource": str,
+    },
+    total=False,
+)
+
+class SourceAuthOutputTypeDef(_RequiredSourceAuthOutputTypeDef, _OptionalSourceAuthOutputTypeDef):
+    pass
+
 _RequiredSourceAuthTypeDef = TypedDict(
     "_RequiredSourceAuthTypeDef",
     {
         "type": Literal["OAUTH"],
     },
 )
 _OptionalSourceAuthTypeDef = TypedDict(
@@ -1082,14 +1291,23 @@
     },
     total=False,
 )
 
 class SourceAuthTypeDef(_RequiredSourceAuthTypeDef, _OptionalSourceAuthTypeDef):
     pass
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 PutResourcePolicyInputRequestTypeDef = TypedDict(
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
@@ -1098,14 +1316,27 @@
     "PutResourcePolicyOutputTypeDef",
     {
         "resourceArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+S3ReportExportConfigOutputTypeDef = TypedDict(
+    "S3ReportExportConfigOutputTypeDef",
+    {
+        "bucket": str,
+        "bucketOwner": str,
+        "path": str,
+        "packaging": ReportPackagingTypeType,
+        "encryptionKey": str,
+        "encryptionDisabled": bool,
+    },
+    total=False,
+)
+
 S3ReportExportConfigTypeDef = TypedDict(
     "S3ReportExportConfigTypeDef",
     {
         "bucket": str,
         "bucketOwner": str,
         "path": str,
         "packaging": ReportPackagingTypeType,
@@ -1195,14 +1426,34 @@
         "projectArn": str,
         "publicProjectAlias": str,
         "projectVisibility": ProjectVisibilityTypeType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredWebhookFilterOutputTypeDef = TypedDict(
+    "_RequiredWebhookFilterOutputTypeDef",
+    {
+        "type": WebhookFilterTypeType,
+        "pattern": str,
+    },
+)
+_OptionalWebhookFilterOutputTypeDef = TypedDict(
+    "_OptionalWebhookFilterOutputTypeDef",
+    {
+        "excludeMatchedPattern": bool,
+    },
+    total=False,
+)
+
+class WebhookFilterOutputTypeDef(
+    _RequiredWebhookFilterOutputTypeDef, _OptionalWebhookFilterOutputTypeDef
+):
+    pass
+
 BatchDeleteBuildsOutputTypeDef = TypedDict(
     "BatchDeleteBuildsOutputTypeDef",
     {
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1214,14 +1465,26 @@
         "statusCode": str,
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ProjectBuildBatchConfigOutputTypeDef = TypedDict(
+    "ProjectBuildBatchConfigOutputTypeDef",
+    {
+        "serviceRole": str,
+        "combineArtifacts": bool,
+        "restrictions": BatchRestrictionsOutputTypeDef,
+        "timeoutInMins": int,
+        "batchReportMode": BatchReportModeTypeType,
+    },
+    total=False,
+)
+
 ProjectBuildBatchConfigTypeDef = TypedDict(
     "ProjectBuildBatchConfigTypeDef",
     {
         "serviceRole": str,
         "combineArtifacts": bool,
         "restrictions": BatchRestrictionsTypeDef,
         "timeoutInMins": int,
@@ -1360,28 +1623,14 @@
 )
 
 class UpdateWebhookInputRequestTypeDef(
     _RequiredUpdateWebhookInputRequestTypeDef, _OptionalUpdateWebhookInputRequestTypeDef
 ):
     pass
 
-WebhookTypeDef = TypedDict(
-    "WebhookTypeDef",
-    {
-        "url": str,
-        "payloadUrl": str,
-        "secret": str,
-        "branchFilter": str,
-        "filterGroups": List[List[WebhookFilterTypeDef]],
-        "buildType": WebhookBuildTypeType,
-        "lastModifiedSecret": datetime,
-    },
-    total=False,
-)
-
 _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
     "_RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef = TypedDict(
@@ -1517,63 +1766,124 @@
     "ListSourceCredentialsOutputTypeDef",
     {
         "sourceCredentialsInfos": List[SourceCredentialsInfoTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-LogsConfigTypeDef = TypedDict(
-    "LogsConfigTypeDef",
+LogsConfigOutputTypeDef = TypedDict(
+    "LogsConfigOutputTypeDef",
     {
-        "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
-        "s3Logs": S3LogsConfigTypeDef,
+        "cloudWatchLogs": CloudWatchLogsConfigOutputTypeDef,
+        "s3Logs": S3LogsConfigOutputTypeDef,
     },
     total=False,
 )
 
 LogsLocationTypeDef = TypedDict(
     "LogsLocationTypeDef",
     {
         "groupName": str,
         "streamName": str,
         "deepLink": str,
         "s3DeepLink": str,
         "cloudWatchLogsArn": str,
         "s3LogsArn": str,
+        "cloudWatchLogs": CloudWatchLogsConfigOutputTypeDef,
+        "s3Logs": S3LogsConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+LogsConfigTypeDef = TypedDict(
+    "LogsConfigTypeDef",
+    {
         "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
         "s3Logs": S3LogsConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredProjectEnvironmentOutputTypeDef = TypedDict(
+    "_RequiredProjectEnvironmentOutputTypeDef",
+    {
+        "type": EnvironmentTypeType,
+        "image": str,
+        "computeType": ComputeTypeType,
+    },
+)
+_OptionalProjectEnvironmentOutputTypeDef = TypedDict(
+    "_OptionalProjectEnvironmentOutputTypeDef",
+    {
+        "environmentVariables": List[EnvironmentVariableOutputTypeDef],
+        "privilegedMode": bool,
+        "certificate": str,
+        "registryCredential": RegistryCredentialOutputTypeDef,
+        "imagePullCredentialsType": ImagePullCredentialsTypeType,
+    },
+    total=False,
+)
+
+class ProjectEnvironmentOutputTypeDef(
+    _RequiredProjectEnvironmentOutputTypeDef, _OptionalProjectEnvironmentOutputTypeDef
+):
+    pass
+
 _RequiredProjectEnvironmentTypeDef = TypedDict(
     "_RequiredProjectEnvironmentTypeDef",
     {
         "type": EnvironmentTypeType,
         "image": str,
         "computeType": ComputeTypeType,
     },
 )
 _OptionalProjectEnvironmentTypeDef = TypedDict(
     "_OptionalProjectEnvironmentTypeDef",
     {
-        "environmentVariables": List[EnvironmentVariableTypeDef],
+        "environmentVariables": Sequence[EnvironmentVariableTypeDef],
         "privilegedMode": bool,
         "certificate": str,
         "registryCredential": RegistryCredentialTypeDef,
         "imagePullCredentialsType": ImagePullCredentialsTypeType,
     },
     total=False,
 )
 
 class ProjectEnvironmentTypeDef(
     _RequiredProjectEnvironmentTypeDef, _OptionalProjectEnvironmentTypeDef
 ):
     pass
 
+_RequiredProjectSourceOutputTypeDef = TypedDict(
+    "_RequiredProjectSourceOutputTypeDef",
+    {
+        "type": SourceTypeType,
+    },
+)
+_OptionalProjectSourceOutputTypeDef = TypedDict(
+    "_OptionalProjectSourceOutputTypeDef",
+    {
+        "location": str,
+        "gitCloneDepth": int,
+        "gitSubmodulesConfig": GitSubmodulesConfigOutputTypeDef,
+        "buildspec": str,
+        "auth": SourceAuthOutputTypeDef,
+        "reportBuildStatus": bool,
+        "buildStatusConfig": BuildStatusConfigOutputTypeDef,
+        "insecureSsl": bool,
+        "sourceIdentifier": str,
+    },
+    total=False,
+)
+
+class ProjectSourceOutputTypeDef(
+    _RequiredProjectSourceOutputTypeDef, _OptionalProjectSourceOutputTypeDef
+):
+    pass
+
 _RequiredProjectSourceTypeDef = TypedDict(
     "_RequiredProjectSourceTypeDef",
     {
         "type": SourceTypeType,
     },
 )
 _OptionalProjectSourceTypeDef = TypedDict(
@@ -1591,51 +1901,58 @@
     },
     total=False,
 )
 
 class ProjectSourceTypeDef(_RequiredProjectSourceTypeDef, _OptionalProjectSourceTypeDef):
     pass
 
+ReportExportConfigOutputTypeDef = TypedDict(
+    "ReportExportConfigOutputTypeDef",
+    {
+        "exportConfigType": ReportExportConfigTypeType,
+        "s3Destination": S3ReportExportConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ReportExportConfigTypeDef = TypedDict(
     "ReportExportConfigTypeDef",
     {
         "exportConfigType": ReportExportConfigTypeType,
         "s3Destination": S3ReportExportConfigTypeDef,
     },
     total=False,
 )
 
+WebhookTypeDef = TypedDict(
+    "WebhookTypeDef",
+    {
+        "url": str,
+        "payloadUrl": str,
+        "secret": str,
+        "branchFilter": str,
+        "filterGroups": List[List[WebhookFilterOutputTypeDef]],
+        "buildType": WebhookBuildTypeType,
+        "lastModifiedSecret": datetime,
+    },
+    total=False,
+)
+
 BuildGroupTypeDef = TypedDict(
     "BuildGroupTypeDef",
     {
         "identifier": str,
         "dependsOn": List[str],
         "ignoreFailure": bool,
         "currentBuildSummary": BuildSummaryTypeDef,
         "priorBuildSummaryList": List[BuildSummaryTypeDef],
     },
     total=False,
 )
 
-CreateWebhookOutputTypeDef = TypedDict(
-    "CreateWebhookOutputTypeDef",
-    {
-        "webhook": WebhookTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateWebhookOutputTypeDef = TypedDict(
-    "UpdateWebhookOutputTypeDef",
-    {
-        "webhook": WebhookTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentPlatformTypeDef = TypedDict(
     "EnvironmentPlatformTypeDef",
     {
         "platform": PlatformTypeType,
         "languages": List[EnvironmentLanguageTypeDef],
     },
     total=False,
@@ -1651,33 +1968,33 @@
         "endTime": datetime,
         "currentPhase": str,
         "buildStatus": StatusTypeType,
         "sourceVersion": str,
         "resolvedSourceVersion": str,
         "projectName": str,
         "phases": List[BuildPhaseTypeDef],
-        "source": ProjectSourceTypeDef,
-        "secondarySources": List[ProjectSourceTypeDef],
-        "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
+        "source": ProjectSourceOutputTypeDef,
+        "secondarySources": List[ProjectSourceOutputTypeDef],
+        "secondarySourceVersions": List[ProjectSourceVersionOutputTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
-        "cache": ProjectCacheTypeDef,
-        "environment": ProjectEnvironmentTypeDef,
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
         "logs": LogsLocationTypeDef,
         "timeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "buildComplete": bool,
         "initiator": str,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "encryptionKey": str,
         "exportedEnvironmentVariables": List[ExportedEnvironmentVariableTypeDef],
         "reportArns": List[str],
-        "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
+        "fileSystemLocations": List[ProjectFileSystemLocationOutputTypeDef],
         "debugSession": DebugSessionTypeDef,
         "buildBatchArn": str,
     },
     total=False,
 )
 
 _RequiredCreateProjectInputRequestTypeDef = TypedDict(
@@ -1714,49 +2031,14 @@
 )
 
 class CreateProjectInputRequestTypeDef(
     _RequiredCreateProjectInputRequestTypeDef, _OptionalCreateProjectInputRequestTypeDef
 ):
     pass
 
-ProjectTypeDef = TypedDict(
-    "ProjectTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "source": ProjectSourceTypeDef,
-        "secondarySources": List[ProjectSourceTypeDef],
-        "sourceVersion": str,
-        "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
-        "artifacts": ProjectArtifactsTypeDef,
-        "secondaryArtifacts": List[ProjectArtifactsTypeDef],
-        "cache": ProjectCacheTypeDef,
-        "environment": ProjectEnvironmentTypeDef,
-        "serviceRole": str,
-        "timeoutInMinutes": int,
-        "queuedTimeoutInMinutes": int,
-        "encryptionKey": str,
-        "tags": List[TagTypeDef],
-        "created": datetime,
-        "lastModified": datetime,
-        "webhook": WebhookTypeDef,
-        "vpcConfig": VpcConfigTypeDef,
-        "badge": ProjectBadgeTypeDef,
-        "logsConfig": LogsConfigTypeDef,
-        "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
-        "concurrentBuildLimit": int,
-        "projectVisibility": ProjectVisibilityTypeType,
-        "publicProjectAlias": str,
-        "resourceAccessRole": str,
-    },
-    total=False,
-)
-
 _RequiredStartBuildBatchInputRequestTypeDef = TypedDict(
     "_RequiredStartBuildBatchInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalStartBuildBatchInputRequestTypeDef = TypedDict(
@@ -1883,45 +2165,24 @@
 )
 
 class UpdateProjectInputRequestTypeDef(
     _RequiredUpdateProjectInputRequestTypeDef, _OptionalUpdateProjectInputRequestTypeDef
 ):
     pass
 
-_RequiredCreateReportGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateReportGroupInputRequestTypeDef",
-    {
-        "name": str,
-        "type": ReportTypeType,
-        "exportConfig": ReportExportConfigTypeDef,
-    },
-)
-_OptionalCreateReportGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateReportGroupInputRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateReportGroupInputRequestTypeDef(
-    _RequiredCreateReportGroupInputRequestTypeDef, _OptionalCreateReportGroupInputRequestTypeDef
-):
-    pass
-
 ReportGroupTypeDef = TypedDict(
     "ReportGroupTypeDef",
     {
         "arn": str,
         "name": str,
         "type": ReportTypeType,
-        "exportConfig": ReportExportConfigTypeDef,
+        "exportConfig": ReportExportConfigOutputTypeDef,
         "created": datetime,
         "lastModified": datetime,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "status": ReportGroupStatusTypeType,
     },
     total=False,
 )
 
 ReportTypeDef = TypedDict(
     "ReportTypeDef",
@@ -1930,22 +2191,43 @@
         "type": ReportTypeType,
         "name": str,
         "reportGroupArn": str,
         "executionId": str,
         "status": ReportStatusTypeType,
         "created": datetime,
         "expired": datetime,
-        "exportConfig": ReportExportConfigTypeDef,
+        "exportConfig": ReportExportConfigOutputTypeDef,
         "truncated": bool,
         "testSummary": TestReportSummaryTypeDef,
         "codeCoverageSummary": CodeCoverageReportSummaryTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateReportGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateReportGroupInputRequestTypeDef",
+    {
+        "name": str,
+        "type": ReportTypeType,
+        "exportConfig": ReportExportConfigTypeDef,
+    },
+)
+_OptionalCreateReportGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateReportGroupInputRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateReportGroupInputRequestTypeDef(
+    _RequiredCreateReportGroupInputRequestTypeDef, _OptionalCreateReportGroupInputRequestTypeDef
+):
+    pass
+
 _RequiredUpdateReportGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReportGroupInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateReportGroupInputRequestTypeDef = TypedDict(
@@ -1958,45 +2240,96 @@
 )
 
 class UpdateReportGroupInputRequestTypeDef(
     _RequiredUpdateReportGroupInputRequestTypeDef, _OptionalUpdateReportGroupInputRequestTypeDef
 ):
     pass
 
+CreateWebhookOutputTypeDef = TypedDict(
+    "CreateWebhookOutputTypeDef",
+    {
+        "webhook": WebhookTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ProjectTypeDef = TypedDict(
+    "ProjectTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "source": ProjectSourceOutputTypeDef,
+        "secondarySources": List[ProjectSourceOutputTypeDef],
+        "sourceVersion": str,
+        "secondarySourceVersions": List[ProjectSourceVersionOutputTypeDef],
+        "artifacts": ProjectArtifactsOutputTypeDef,
+        "secondaryArtifacts": List[ProjectArtifactsOutputTypeDef],
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
+        "serviceRole": str,
+        "timeoutInMinutes": int,
+        "queuedTimeoutInMinutes": int,
+        "encryptionKey": str,
+        "tags": List[TagOutputTypeDef],
+        "created": datetime,
+        "lastModified": datetime,
+        "webhook": WebhookTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
+        "badge": ProjectBadgeTypeDef,
+        "logsConfig": LogsConfigOutputTypeDef,
+        "fileSystemLocations": List[ProjectFileSystemLocationOutputTypeDef],
+        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
+        "concurrentBuildLimit": int,
+        "projectVisibility": ProjectVisibilityTypeType,
+        "publicProjectAlias": str,
+        "resourceAccessRole": str,
+    },
+    total=False,
+)
+
+UpdateWebhookOutputTypeDef = TypedDict(
+    "UpdateWebhookOutputTypeDef",
+    {
+        "webhook": WebhookTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BuildBatchTypeDef = TypedDict(
     "BuildBatchTypeDef",
     {
         "id": str,
         "arn": str,
         "startTime": datetime,
         "endTime": datetime,
         "currentPhase": str,
         "buildBatchStatus": StatusTypeType,
         "sourceVersion": str,
         "resolvedSourceVersion": str,
         "projectName": str,
         "phases": List[BuildBatchPhaseTypeDef],
-        "source": ProjectSourceTypeDef,
-        "secondarySources": List[ProjectSourceTypeDef],
-        "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
+        "source": ProjectSourceOutputTypeDef,
+        "secondarySources": List[ProjectSourceOutputTypeDef],
+        "secondarySourceVersions": List[ProjectSourceVersionOutputTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
-        "cache": ProjectCacheTypeDef,
-        "environment": ProjectEnvironmentTypeDef,
+        "cache": ProjectCacheOutputTypeDef,
+        "environment": ProjectEnvironmentOutputTypeDef,
         "serviceRole": str,
-        "logConfig": LogsConfigTypeDef,
+        "logConfig": LogsConfigOutputTypeDef,
         "buildTimeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "complete": bool,
         "initiator": str,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
         "encryptionKey": str,
         "buildBatchNumber": int,
-        "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
+        "fileSystemLocations": List[ProjectFileSystemLocationOutputTypeDef],
+        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
         "buildGroups": List[BuildGroupTypeDef],
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
 ListCuratedEnvironmentImagesOutputTypeDef = TypedDict(
@@ -2036,69 +2369,69 @@
     "StopBuildOutputTypeDef",
     {
         "build": BuildTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BatchGetProjectsOutputTypeDef = TypedDict(
-    "BatchGetProjectsOutputTypeDef",
+BatchGetReportGroupsOutputTypeDef = TypedDict(
+    "BatchGetReportGroupsOutputTypeDef",
     {
-        "projects": List[ProjectTypeDef],
-        "projectsNotFound": List[str],
+        "reportGroups": List[ReportGroupTypeDef],
+        "reportGroupsNotFound": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateProjectOutputTypeDef = TypedDict(
-    "CreateProjectOutputTypeDef",
+CreateReportGroupOutputTypeDef = TypedDict(
+    "CreateReportGroupOutputTypeDef",
     {
-        "project": ProjectTypeDef,
+        "reportGroup": ReportGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateProjectOutputTypeDef = TypedDict(
-    "UpdateProjectOutputTypeDef",
+UpdateReportGroupOutputTypeDef = TypedDict(
+    "UpdateReportGroupOutputTypeDef",
     {
-        "project": ProjectTypeDef,
+        "reportGroup": ReportGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BatchGetReportGroupsOutputTypeDef = TypedDict(
-    "BatchGetReportGroupsOutputTypeDef",
+BatchGetReportsOutputTypeDef = TypedDict(
+    "BatchGetReportsOutputTypeDef",
     {
-        "reportGroups": List[ReportGroupTypeDef],
-        "reportGroupsNotFound": List[str],
+        "reports": List[ReportTypeDef],
+        "reportsNotFound": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateReportGroupOutputTypeDef = TypedDict(
-    "CreateReportGroupOutputTypeDef",
+BatchGetProjectsOutputTypeDef = TypedDict(
+    "BatchGetProjectsOutputTypeDef",
     {
-        "reportGroup": ReportGroupTypeDef,
+        "projects": List[ProjectTypeDef],
+        "projectsNotFound": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateReportGroupOutputTypeDef = TypedDict(
-    "UpdateReportGroupOutputTypeDef",
+CreateProjectOutputTypeDef = TypedDict(
+    "CreateProjectOutputTypeDef",
     {
-        "reportGroup": ReportGroupTypeDef,
+        "project": ProjectTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-BatchGetReportsOutputTypeDef = TypedDict(
-    "BatchGetReportsOutputTypeDef",
+UpdateProjectOutputTypeDef = TypedDict(
+    "UpdateProjectOutputTypeDef",
     {
-        "reports": List[ReportTypeDef],
-        "reportsNotFound": List[str],
+        "project": ProjectTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetBuildBatchesOutputTypeDef = TypedDict(
     "BatchGetBuildBatchesOutputTypeDef",
     {
```

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild.egg-info/PKG-INFO` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codebuild
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeBuild 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodeBuild 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codebuild"></a>
 
 # mypy-boto3-codebuild
 
 [![PyPI - mypy-boto3-codebuild](https://img.shields.io/pypi/v/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codebuild.svg?color=blue)](https://pypi.org/project/mypy-boto3-codebuild)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codebuild?color=blue)](https://pypistats.org/packages/mypy-boto3-codebuild)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codebuild)](https://pepy.tech/project/mypy-boto3-codebuild)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeBuild 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
+[boto3.CodeBuild 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild)
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
 [mypy-boto3-codebuild docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codebuild/).
 
 See how it helps to find and fix potential bugs:
 
@@ -412,52 +412,61 @@
     BatchDeleteBuildsInputRequestTypeDef,
     BuildNotDeletedTypeDef,
     BatchGetBuildBatchesInputRequestTypeDef,
     BatchGetBuildsInputRequestTypeDef,
     BatchGetProjectsInputRequestTypeDef,
     BatchGetReportGroupsInputRequestTypeDef,
     BatchGetReportsInputRequestTypeDef,
+    BatchRestrictionsOutputTypeDef,
     BatchRestrictionsTypeDef,
     BuildArtifactsTypeDef,
     BuildBatchFilterTypeDef,
     PhaseContextTypeDef,
-    ProjectCacheTypeDef,
-    ProjectFileSystemLocationTypeDef,
-    ProjectSourceVersionTypeDef,
-    VpcConfigTypeDef,
+    ProjectCacheOutputTypeDef,
+    ProjectFileSystemLocationOutputTypeDef,
+    ProjectSourceVersionOutputTypeDef,
+    VpcConfigOutputTypeDef,
+    BuildStatusConfigOutputTypeDef,
     BuildStatusConfigTypeDef,
     ResolvedArtifactTypeDef,
     DebugSessionTypeDef,
     ExportedEnvironmentVariableTypeDef,
     NetworkInterfaceTypeDef,
+    CloudWatchLogsConfigOutputTypeDef,
     CloudWatchLogsConfigTypeDef,
     CodeCoverageReportSummaryTypeDef,
     CodeCoverageTypeDef,
     ProjectArtifactsTypeDef,
+    ProjectCacheTypeDef,
+    ProjectFileSystemLocationTypeDef,
+    ProjectSourceVersionTypeDef,
     TagTypeDef,
+    VpcConfigTypeDef,
     WebhookFilterTypeDef,
     DeleteBuildBatchInputRequestTypeDef,
     DeleteProjectInputRequestTypeDef,
     DeleteReportGroupInputRequestTypeDef,
     DeleteReportInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteSourceCredentialsInputRequestTypeDef,
     DeleteSourceCredentialsOutputTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
     DescribeCodeCoveragesInputRequestTypeDef,
     TestCaseFilterTypeDef,
     TestCaseTypeDef,
     EnvironmentImageTypeDef,
+    EnvironmentVariableOutputTypeDef,
     EnvironmentVariableTypeDef,
     GetReportGroupTrendInputRequestTypeDef,
     ReportGroupTrendStatsTypeDef,
     ReportWithRawDataTypeDef,
     GetResourcePolicyInputRequestTypeDef,
     GetResourcePolicyOutputTypeDef,
+    GitSubmodulesConfigOutputTypeDef,
     GitSubmodulesConfigTypeDef,
     ImportSourceCredentialsInputRequestTypeDef,
     ImportSourceCredentialsOutputTypeDef,
     InvalidateProjectCacheInputRequestTypeDef,
     ListBuildBatchesForProjectOutputTypeDef,
     ListBuildBatchesOutputTypeDef,
     ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
@@ -478,86 +487,98 @@
     ListSharedProjectsInputListSharedProjectsPaginateTypeDef,
     ListSharedProjectsInputRequestTypeDef,
     ListSharedProjectsOutputTypeDef,
     ListSharedReportGroupsInputListSharedReportGroupsPaginateTypeDef,
     ListSharedReportGroupsInputRequestTypeDef,
     ListSharedReportGroupsOutputTypeDef,
     SourceCredentialsInfoTypeDef,
+    S3LogsConfigOutputTypeDef,
     S3LogsConfigTypeDef,
     PaginatorConfigTypeDef,
+    ProjectArtifactsOutputTypeDef,
     ProjectBadgeTypeDef,
+    RegistryCredentialOutputTypeDef,
     RegistryCredentialTypeDef,
+    SourceAuthOutputTypeDef,
     SourceAuthTypeDef,
+    TagOutputTypeDef,
     PutResourcePolicyInputRequestTypeDef,
     PutResourcePolicyOutputTypeDef,
+    S3ReportExportConfigOutputTypeDef,
     S3ReportExportConfigTypeDef,
     TestReportSummaryTypeDef,
     ResponseMetadataTypeDef,
     RetryBuildBatchInputRequestTypeDef,
     RetryBuildInputRequestTypeDef,
     StopBuildBatchInputRequestTypeDef,
     StopBuildInputRequestTypeDef,
     UpdateProjectVisibilityInputRequestTypeDef,
     UpdateProjectVisibilityOutputTypeDef,
+    WebhookFilterOutputTypeDef,
     BatchDeleteBuildsOutputTypeDef,
     DeleteBuildBatchOutputTypeDef,
+    ProjectBuildBatchConfigOutputTypeDef,
     ProjectBuildBatchConfigTypeDef,
     ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef,
     ListBuildBatchesForProjectInputRequestTypeDef,
     ListBuildBatchesInputListBuildBatchesPaginateTypeDef,
     ListBuildBatchesInputRequestTypeDef,
     BuildBatchPhaseTypeDef,
     BuildPhaseTypeDef,
     BuildSummaryTypeDef,
     DescribeCodeCoveragesOutputTypeDef,
     CreateWebhookInputRequestTypeDef,
     UpdateWebhookInputRequestTypeDef,
-    WebhookTypeDef,
     DescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     DescribeTestCasesInputRequestTypeDef,
     DescribeTestCasesOutputTypeDef,
     EnvironmentLanguageTypeDef,
     GetReportGroupTrendOutputTypeDef,
     ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     ListReportsForReportGroupInputRequestTypeDef,
     ListReportsInputListReportsPaginateTypeDef,
     ListReportsInputRequestTypeDef,
     ListSourceCredentialsOutputTypeDef,
-    LogsConfigTypeDef,
+    LogsConfigOutputTypeDef,
     LogsLocationTypeDef,
+    LogsConfigTypeDef,
+    ProjectEnvironmentOutputTypeDef,
     ProjectEnvironmentTypeDef,
+    ProjectSourceOutputTypeDef,
     ProjectSourceTypeDef,
+    ReportExportConfigOutputTypeDef,
     ReportExportConfigTypeDef,
+    WebhookTypeDef,
     BuildGroupTypeDef,
-    CreateWebhookOutputTypeDef,
-    UpdateWebhookOutputTypeDef,
     EnvironmentPlatformTypeDef,
     BuildTypeDef,
     CreateProjectInputRequestTypeDef,
-    ProjectTypeDef,
     StartBuildBatchInputRequestTypeDef,
     StartBuildInputRequestTypeDef,
     UpdateProjectInputRequestTypeDef,
-    CreateReportGroupInputRequestTypeDef,
     ReportGroupTypeDef,
     ReportTypeDef,
+    CreateReportGroupInputRequestTypeDef,
     UpdateReportGroupInputRequestTypeDef,
+    CreateWebhookOutputTypeDef,
+    ProjectTypeDef,
+    UpdateWebhookOutputTypeDef,
     BuildBatchTypeDef,
     ListCuratedEnvironmentImagesOutputTypeDef,
     BatchGetBuildsOutputTypeDef,
     RetryBuildOutputTypeDef,
     StartBuildOutputTypeDef,
     StopBuildOutputTypeDef,
-    BatchGetProjectsOutputTypeDef,
-    CreateProjectOutputTypeDef,
-    UpdateProjectOutputTypeDef,
     BatchGetReportGroupsOutputTypeDef,
     CreateReportGroupOutputTypeDef,
     UpdateReportGroupOutputTypeDef,
     BatchGetReportsOutputTypeDef,
+    BatchGetProjectsOutputTypeDef,
+    CreateProjectOutputTypeDef,
+    UpdateProjectOutputTypeDef,
     BatchGetBuildBatchesOutputTypeDef,
     RetryBuildBatchOutputTypeDef,
     StartBuildBatchOutputTypeDef,
     StopBuildBatchOutputTypeDef,
 )
```

### Comparing `mypy-boto3-codebuild-1.28.0/mypy_boto3_codebuild.egg-info/SOURCES.txt` & `mypy-boto3-codebuild-1.28.12/mypy_boto3_codebuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codebuild-1.28.0/setup.py` & `mypy-boto3-codebuild-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codebuild",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_codebuild"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeBuild 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CodeBuild 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

