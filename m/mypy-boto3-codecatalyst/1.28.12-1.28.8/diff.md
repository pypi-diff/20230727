# Comparing `tmp/mypy-boto3-codecatalyst-1.28.12.tar.gz` & `tmp/mypy-boto3-codecatalyst-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codecatalyst-1.28.12.tar", last modified: Thu Jul 27 05:34:27 2023, max compression
+gzip compressed data, was "mypy-boto3-codecatalyst-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-codecatalyst-1.28.12.tar` & `mypy-boto3-codecatalyst-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.264556 mypy-boto3-codecatalyst-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-07-27 05:34:27.260556 mypy-boto3-codecatalyst-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16729 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.260556 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27809 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-27 05:18:59.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39480 2023-07-27 05:19:00.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39411 2023-07-27 05:19:00.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.260556 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-07-27 05:34:27.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:27.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:27.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:27.000000 mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:27.264556 mypy-boto3-codecatalyst-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:18:58.000000 mypy-boto3-codecatalyst-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.012775 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27809 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37203 2023-07-20 19:46:46.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37150 2023-07-20 19:46:46.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18249 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 19:47:55.000000 mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.016775 mypy-boto3-codecatalyst-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 19:46:45.000000 mypy-boto3-codecatalyst-1.28.8/setup.py
```

### Comparing `mypy-boto3-codecatalyst-1.28.12/LICENSE` & `mypy-boto3-codecatalyst-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.12/PKG-INFO` & `mypy-boto3-codecatalyst-1.28.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecatalyst
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeCatalyst 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.8
+Summary: Type annotations for boto3.CodeCatalyst 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codecatalyst"></a>
 
 # mypy-boto3-codecatalyst
 
 [![PyPI - mypy-boto3-codecatalyst](https://img.shields.io/pypi/v/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecatalyst)](https://pepy.tech/project/mypy-boto3-codecatalyst)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,101 +358,101 @@
 `mypy_boto3_codecatalyst.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
     CreateAccessTokenRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
     CreateSourceRepositoryRequestRequestTypeDef,
-    CreateSourceRepositoryResponseTypeDef,
     DeleteAccessTokenRequestRequestTypeDef,
     DeleteDevEnvironmentRequestRequestTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DeleteSourceRepositoryRequestRequestTypeDef,
-    DeleteSourceRepositoryResponseTypeDef,
     DeleteSpaceRequestRequestTypeDef,
-    DeleteSpaceResponseTypeDef,
     DevEnvironmentAccessDetailsTypeDef,
     DevEnvironmentRepositorySummaryTypeDef,
     ExecuteCommandSessionConfigurationTypeDef,
     DevEnvironmentSessionSummaryTypeDef,
     IdeTypeDef,
     PersistentStorageTypeDef,
     EmailAddressTypeDef,
     EventPayloadTypeDef,
     ProjectInformationTypeDef,
     UserIdentityTypeDef,
     FilterTypeDef,
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
-    GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSourceRepositoryRequestRequestTypeDef,
-    GetSourceRepositoryResponseTypeDef,
     GetSpaceRequestRequestTypeDef,
-    GetSpaceResponseTypeDef,
     GetSubscriptionRequestRequestTypeDef,
-    GetSubscriptionResponseTypeDef,
     GetUserDetailsRequestRequestTypeDef,
     IdeConfigurationOutputTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
-    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartDevEnvironmentResponseTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionRequestRequestTypeDef,
-    StopDevEnvironmentSessionResponseTypeDef,
     UpdateProjectRequestRequestTypeDef,
-    UpdateProjectResponseTypeDef,
     UpdateSpaceRequestRequestTypeDef,
+    CreateAccessTokenResponseTypeDef,
+    CreateDevEnvironmentResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryResponseTypeDef,
+    DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteSourceRepositoryResponseTypeDef,
+    DeleteSpaceResponseTypeDef,
+    GetProjectResponseTypeDef,
+    GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryResponseTypeDef,
+    GetSpaceResponseTypeDef,
+    GetSubscriptionResponseTypeDef,
+    ListAccessTokensResponseTypeDef,
+    StartDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentSessionResponseTypeDef,
+    UpdateProjectResponseTypeDef,
     UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
+    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
+    ListEventLogsRequestListEventLogsPaginateTypeDef,
+    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    ListSpacesRequestListSpacesPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.28.12/README.md` & `mypy-boto3-codecatalyst-1.28.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codecatalyst"></a>
 
 # mypy-boto3-codecatalyst
 
 [![PyPI - mypy-boto3-codecatalyst](https://img.shields.io/pypi/v/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecatalyst)](https://pepy.tech/project/mypy-boto3-codecatalyst)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,101 +326,101 @@
 `mypy_boto3_codecatalyst.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
     CreateAccessTokenRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
     CreateSourceRepositoryRequestRequestTypeDef,
-    CreateSourceRepositoryResponseTypeDef,
     DeleteAccessTokenRequestRequestTypeDef,
     DeleteDevEnvironmentRequestRequestTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DeleteSourceRepositoryRequestRequestTypeDef,
-    DeleteSourceRepositoryResponseTypeDef,
     DeleteSpaceRequestRequestTypeDef,
-    DeleteSpaceResponseTypeDef,
     DevEnvironmentAccessDetailsTypeDef,
     DevEnvironmentRepositorySummaryTypeDef,
     ExecuteCommandSessionConfigurationTypeDef,
     DevEnvironmentSessionSummaryTypeDef,
     IdeTypeDef,
     PersistentStorageTypeDef,
     EmailAddressTypeDef,
     EventPayloadTypeDef,
     ProjectInformationTypeDef,
     UserIdentityTypeDef,
     FilterTypeDef,
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
-    GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSourceRepositoryRequestRequestTypeDef,
-    GetSourceRepositoryResponseTypeDef,
     GetSpaceRequestRequestTypeDef,
-    GetSpaceResponseTypeDef,
     GetSubscriptionRequestRequestTypeDef,
-    GetSubscriptionResponseTypeDef,
     GetUserDetailsRequestRequestTypeDef,
     IdeConfigurationOutputTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
-    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartDevEnvironmentResponseTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionRequestRequestTypeDef,
-    StopDevEnvironmentSessionResponseTypeDef,
     UpdateProjectRequestRequestTypeDef,
-    UpdateProjectResponseTypeDef,
     UpdateSpaceRequestRequestTypeDef,
+    CreateAccessTokenResponseTypeDef,
+    CreateDevEnvironmentResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryResponseTypeDef,
+    DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteSourceRepositoryResponseTypeDef,
+    DeleteSpaceResponseTypeDef,
+    GetProjectResponseTypeDef,
+    GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryResponseTypeDef,
+    GetSpaceResponseTypeDef,
+    GetSubscriptionResponseTypeDef,
+    ListAccessTokensResponseTypeDef,
+    StartDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentSessionResponseTypeDef,
+    UpdateProjectResponseTypeDef,
     UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
+    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
+    ListEventLogsRequestListEventLogsPaginateTypeDef,
+    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    ListSpacesRequestListSpacesPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/__init__.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/__init__.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/__main__.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeCatalyst 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CodeCatalyst 1.28.8\nVersion:         1.28.8\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/client.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/client.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/literals.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -264,15 +263,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/literals.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -262,15 +261,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/paginator.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 class ListAccessTokensPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listaccesstokenspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessTokensResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listaccesstokenspaginator)
         """
 
 
@@ -97,15 +97,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         devEnvironmentId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevEnvironmentSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentsessionspaginator)
         """
 
 
@@ -117,15 +117,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentspaginator)
         """
 
 
@@ -138,15 +138,15 @@
     def paginate(
         self,
         *,
         spaceName: str,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         eventName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventLogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listeventlogspaginator)
         """
 
 
@@ -157,30 +157,30 @@
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         filters: Sequence[ProjectListFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listprojectspaginator)
         """
 
 
 class ListSourceRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositoriespaginator)
     """
 
     def paginate(
-        self, *, spaceName: str, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, spaceName: str, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSourceRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositoriespaginator)
         """
 
 
@@ -192,28 +192,28 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSourceRepositoryBranchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositorybranchespaginator)
         """
 
 
 class ListSpacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSpacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listspacespaginator)
         """
```

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/paginator.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 class ListAccessTokensPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listaccesstokenspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessTokensResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListAccessTokens.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listaccesstokenspaginator)
         """
 
 class ListDevEnvironmentSessionsPaginator(Paginator):
@@ -93,15 +93,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         devEnvironmentId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevEnvironmentSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironmentSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentsessionspaginator)
         """
 
 class ListDevEnvironmentsPaginator(Paginator):
@@ -112,15 +112,15 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListDevEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listdevenvironmentspaginator)
         """
 
 class ListEventLogsPaginator(Paginator):
@@ -132,15 +132,15 @@
     def paginate(
         self,
         *,
         spaceName: str,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         eventName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventLogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListEventLogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listeventlogspaginator)
         """
 
 class ListProjectsPaginator(Paginator):
@@ -150,29 +150,29 @@
     """
 
     def paginate(
         self,
         *,
         spaceName: str,
         filters: Sequence[ProjectListFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listprojectspaginator)
         """
 
 class ListSourceRepositoriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositoriespaginator)
     """
 
     def paginate(
-        self, *, spaceName: str, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, spaceName: str, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSourceRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositories.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositoriespaginator)
         """
 
 class ListSourceRepositoryBranchesPaginator(Paginator):
@@ -183,27 +183,27 @@
 
     def paginate(
         self,
         *,
         spaceName: str,
         projectName: str,
         sourceRepositoryName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSourceRepositoryBranchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSourceRepositoryBranches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listsourcerepositorybranchespaginator)
         """
 
 class ListSpacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSpacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst.Paginator.ListSpaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/paginators/#listspacespaginator)
         """
```

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/type_defs.py` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,134 +33,121 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessTokenSummaryTypeDef",
     "CreateAccessTokenRequestRequestTypeDef",
-    "CreateAccessTokenResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
-    "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchRequestRequestTypeDef",
-    "CreateSourceRepositoryBranchResponseTypeDef",
     "CreateSourceRepositoryRequestRequestTypeDef",
-    "CreateSourceRepositoryResponseTypeDef",
     "DeleteAccessTokenRequestRequestTypeDef",
     "DeleteDevEnvironmentRequestRequestTypeDef",
-    "DeleteDevEnvironmentResponseTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResponseTypeDef",
     "DeleteSourceRepositoryRequestRequestTypeDef",
-    "DeleteSourceRepositoryResponseTypeDef",
     "DeleteSpaceRequestRequestTypeDef",
-    "DeleteSpaceResponseTypeDef",
     "DevEnvironmentAccessDetailsTypeDef",
     "DevEnvironmentRepositorySummaryTypeDef",
     "ExecuteCommandSessionConfigurationTypeDef",
     "DevEnvironmentSessionSummaryTypeDef",
     "IdeTypeDef",
     "PersistentStorageTypeDef",
     "EmailAddressTypeDef",
     "EventPayloadTypeDef",
     "ProjectInformationTypeDef",
     "UserIdentityTypeDef",
     "FilterTypeDef",
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
-    "GetProjectResponseTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
     "GetSourceRepositoryRequestRequestTypeDef",
-    "GetSourceRepositoryResponseTypeDef",
     "GetSpaceRequestRequestTypeDef",
-    "GetSpaceResponseTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
-    "GetSubscriptionResponseTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
     "IdeConfigurationOutputTypeDef",
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
-    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
     "ListDevEnvironmentSessionsRequestRequestTypeDef",
-    "ListEventLogsRequestListEventLogsPaginateTypeDef",
     "ListEventLogsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
     "ProjectSummaryTypeDef",
     "ListSourceRepositoriesItemTypeDef",
-    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
-    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
-    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentRequestRequestTypeDef",
-    "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionRequestRequestTypeDef",
-    "StopDevEnvironmentSessionResponseTypeDef",
     "UpdateProjectRequestRequestTypeDef",
-    "UpdateProjectResponseTypeDef",
     "UpdateSpaceRequestRequestTypeDef",
+    "CreateAccessTokenResponseTypeDef",
+    "CreateDevEnvironmentResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateSourceRepositoryBranchResponseTypeDef",
+    "CreateSourceRepositoryResponseTypeDef",
+    "DeleteDevEnvironmentResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "DeleteSourceRepositoryResponseTypeDef",
+    "DeleteSpaceResponseTypeDef",
+    "GetProjectResponseTypeDef",
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    "GetSourceRepositoryResponseTypeDef",
+    "GetSpaceResponseTypeDef",
+    "GetSubscriptionResponseTypeDef",
+    "ListAccessTokensResponseTypeDef",
+    "StartDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentSessionResponseTypeDef",
+    "UpdateProjectResponseTypeDef",
     "UpdateSpaceResponseTypeDef",
     "VerifySessionResponseTypeDef",
-    "ListAccessTokensResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
     "ListDevEnvironmentSessionsResponseTypeDef",
     "DevEnvironmentSummaryTypeDef",
     "GetDevEnvironmentResponseTypeDef",
     "GetUserDetailsResponseTypeDef",
     "EventLogEntryTypeDef",
-    "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     "ListDevEnvironmentsRequestRequestTypeDef",
     "UpdateDevEnvironmentResponseTypeDef",
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
+    "ListEventLogsRequestListEventLogsPaginateTypeDef",
+    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
+    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSourceRepositoriesResponseTypeDef",
     "ListSourceRepositoryBranchesResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     "ListDevEnvironmentsResponseTypeDef",
     "ListEventLogsResponseTypeDef",
 )
 
-_RequiredAccessTokenSummaryTypeDef = TypedDict(
-    "_RequiredAccessTokenSummaryTypeDef",
+AccessTokenSummaryTypeDef = TypedDict(
+    "AccessTokenSummaryTypeDef",
     {
         "id": str,
         "name": str,
-    },
-)
-_OptionalAccessTokenSummaryTypeDef = TypedDict(
-    "_OptionalAccessTokenSummaryTypeDef",
-    {
         "expiresTime": datetime,
     },
-    total=False,
 )
 
-
-class AccessTokenSummaryTypeDef(
-    _RequiredAccessTokenSummaryTypeDef, _OptionalAccessTokenSummaryTypeDef
-):
-    pass
-
-
 _RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessTokenRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
@@ -174,22 +161,22 @@
 
 class CreateAccessTokenRequestRequestTypeDef(
     _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
 ):
     pass
 
 
-CreateAccessTokenResponseTypeDef = TypedDict(
-    "CreateAccessTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "secret": str,
-        "name": str,
-        "expiresTime": datetime,
-        "accessTokenId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 IdeConfigurationTypeDef = TypedDict(
     "IdeConfigurationTypeDef",
     {
         "runtime": str,
@@ -220,24 +207,14 @@
 )
 
 
 class RepositoryInputTypeDef(_RequiredRepositoryInputTypeDef, _OptionalRepositoryInputTypeDef):
     pass
 
 
-CreateDevEnvironmentResponseTypeDef = TypedDict(
-    "CreateDevEnvironmentResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "displayName": str,
     },
 )
@@ -252,25 +229,14 @@
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSourceRepositoryBranchRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
         "name": str,
@@ -288,25 +254,14 @@
 class CreateSourceRepositoryBranchRequestRequestTypeDef(
     _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef,
     _OptionalCreateSourceRepositoryBranchRequestRequestTypeDef,
 ):
     pass
 
 
-CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
-    "CreateSourceRepositoryBranchResponseTypeDef",
-    {
-        "ref": str,
-        "name": str,
-        "lastUpdatedTime": datetime,
-        "headCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSourceRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSourceRepositoryRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "name": str,
     },
@@ -323,25 +278,14 @@
 class CreateSourceRepositoryRequestRequestTypeDef(
     _RequiredCreateSourceRepositoryRequestRequestTypeDef,
     _OptionalCreateSourceRepositoryRequestRequestTypeDef,
 ):
     pass
 
 
-CreateSourceRepositoryResponseTypeDef = TypedDict(
-    "CreateSourceRepositoryResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "name": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccessTokenRequestRequestTypeDef = TypedDict(
     "DeleteAccessTokenRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -350,106 +294,54 @@
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
 )
 
-DeleteDevEnvironmentResponseTypeDef = TypedDict(
-    "DeleteDevEnvironmentResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "name": str,
     },
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSourceRepositoryRequestRequestTypeDef = TypedDict(
     "DeleteSourceRepositoryRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "name": str,
     },
 )
 
-DeleteSourceRepositoryResponseTypeDef = TypedDict(
-    "DeleteSourceRepositoryResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSpaceRequestRequestTypeDef = TypedDict(
     "DeleteSpaceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteSpaceResponseTypeDef = TypedDict(
-    "DeleteSpaceResponseTypeDef",
-    {
-        "name": str,
-        "displayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DevEnvironmentAccessDetailsTypeDef = TypedDict(
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
 
-_RequiredDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentRepositorySummaryTypeDef",
+DevEnvironmentRepositorySummaryTypeDef = TypedDict(
+    "DevEnvironmentRepositorySummaryTypeDef",
     {
         "repositoryName": str,
-    },
-)
-_OptionalDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentRepositorySummaryTypeDef",
-    {
         "branchName": str,
     },
-    total=False,
 )
 
-
-class DevEnvironmentRepositorySummaryTypeDef(
-    _RequiredDevEnvironmentRepositorySummaryTypeDef, _OptionalDevEnvironmentRepositorySummaryTypeDef
-):
-    pass
-
-
 _RequiredExecuteCommandSessionConfigurationTypeDef = TypedDict(
     "_RequiredExecuteCommandSessionConfigurationTypeDef",
     {
         "command": str,
     },
 )
 _OptionalExecuteCommandSessionConfigurationTypeDef = TypedDict(
@@ -481,15 +373,14 @@
 
 IdeTypeDef = TypedDict(
     "IdeTypeDef",
     {
         "runtime": str,
         "name": str,
     },
-    total=False,
 )
 
 PersistentStorageTypeDef = TypedDict(
     "PersistentStorageTypeDef",
     {
         "sizeInGiB": int,
     },
@@ -497,56 +388,42 @@
 
 EmailAddressTypeDef = TypedDict(
     "EmailAddressTypeDef",
     {
         "email": str,
         "verified": bool,
     },
-    total=False,
 )
 
 EventPayloadTypeDef = TypedDict(
     "EventPayloadTypeDef",
     {
         "contentType": str,
         "data": str,
     },
-    total=False,
 )
 
 ProjectInformationTypeDef = TypedDict(
     "ProjectInformationTypeDef",
     {
         "name": str,
         "projectId": str,
     },
-    total=False,
 )
 
-_RequiredUserIdentityTypeDef = TypedDict(
-    "_RequiredUserIdentityTypeDef",
+UserIdentityTypeDef = TypedDict(
+    "UserIdentityTypeDef",
     {
         "userType": UserTypeType,
         "principalId": str,
-    },
-)
-_OptionalUserIdentityTypeDef = TypedDict(
-    "_OptionalUserIdentityTypeDef",
-    {
         "userName": str,
         "awsAccountId": str,
     },
-    total=False,
 )
 
-
-class UserIdentityTypeDef(_RequiredUserIdentityTypeDef, _OptionalUserIdentityTypeDef):
-    pass
-
-
 _RequiredFilterTypeDef = TypedDict(
     "_RequiredFilterTypeDef",
     {
         "key": str,
         "values": Sequence[str],
     },
 )
@@ -576,98 +453,46 @@
     "GetProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "name": str,
     },
 )
 
-GetProjectResponseTypeDef = TypedDict(
-    "GetProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSourceRepositoryCloneUrlsRequestRequestTypeDef = TypedDict(
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
 )
 
-GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
-    {
-        "https": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSourceRepositoryRequestRequestTypeDef = TypedDict(
     "GetSourceRepositoryRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "name": str,
     },
 )
 
-GetSourceRepositoryResponseTypeDef = TypedDict(
-    "GetSourceRepositoryResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "name": str,
-        "description": str,
-        "lastUpdatedTime": datetime,
-        "createdTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSpaceRequestRequestTypeDef = TypedDict(
     "GetSpaceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetSpaceResponseTypeDef = TypedDict(
-    "GetSpaceResponseTypeDef",
-    {
-        "name": str,
-        "regionName": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSubscriptionRequestRequestTypeDef = TypedDict(
     "GetSubscriptionRequestRequestTypeDef",
     {
         "spaceName": str,
     },
 )
 
-GetSubscriptionResponseTypeDef = TypedDict(
-    "GetSubscriptionResponseTypeDef",
-    {
-        "subscriptionType": str,
-        "awsAccountName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetUserDetailsRequestRequestTypeDef = TypedDict(
     "GetUserDetailsRequestRequestTypeDef",
     {
         "id": str,
         "userName": str,
     },
     total=False,
@@ -675,58 +500,35 @@
 
 IdeConfigurationOutputTypeDef = TypedDict(
     "IdeConfigurationOutputTypeDef",
     {
         "runtime": str,
         "name": str,
     },
-    total=False,
 )
 
-ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccessTokensRequestRequestTypeDef = TypedDict(
     "ListAccessTokensRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "devEnvironmentId": str,
-    },
-)
-_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
-    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDevEnvironmentSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevEnvironmentSessionsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "devEnvironmentId": str,
     },
@@ -744,39 +546,14 @@
 class ListDevEnvironmentSessionsRequestRequestTypeDef(
     _RequiredListDevEnvironmentSessionsRequestRequestTypeDef,
     _OptionalListDevEnvironmentSessionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "eventName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListEventLogsRequestListEventLogsPaginateTypeDef(
-    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
-    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEventLogsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventLogsRequestRequestTypeDef",
     {
         "spaceName": str,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
@@ -816,80 +593,33 @@
 
 class ProjectListFilterTypeDef(
     _RequiredProjectListFilterTypeDef, _OptionalProjectListFilterTypeDef
 ):
     pass
 
 
-_RequiredProjectSummaryTypeDef = TypedDict(
-    "_RequiredProjectSummaryTypeDef",
+ProjectSummaryTypeDef = TypedDict(
+    "ProjectSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalProjectSummaryTypeDef = TypedDict(
-    "_OptionalProjectSummaryTypeDef",
-    {
         "displayName": str,
         "description": str,
     },
-    total=False,
 )
 
-
-class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
-    pass
-
-
-_RequiredListSourceRepositoriesItemTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesItemTypeDef",
+ListSourceRepositoriesItemTypeDef = TypedDict(
+    "ListSourceRepositoriesItemTypeDef",
     {
         "id": str,
         "name": str,
+        "description": str,
         "lastUpdatedTime": datetime,
         "createdTime": datetime,
     },
 )
-_OptionalListSourceRepositoriesItemTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesItemTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-
-class ListSourceRepositoriesItemTypeDef(
-    _RequiredListSourceRepositoriesItemTypeDef, _OptionalListSourceRepositoriesItemTypeDef
-):
-    pass
-
-
-_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-    },
-)
-_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
-    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-):
-    pass
-
 
 _RequiredListSourceRepositoriesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
@@ -915,41 +645,16 @@
     "ListSourceRepositoryBranchesItemTypeDef",
     {
         "ref": str,
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
     },
-    total=False,
 )
 
-_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "sourceRepositoryName": str,
-    },
-)
-_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
-    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSourceRepositoryBranchesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoryBranchesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
@@ -967,202 +672,307 @@
 class ListSourceRepositoryBranchesRequestRequestTypeDef(
     _RequiredListSourceRepositoryBranchesRequestRequestTypeDef,
     _OptionalListSourceRepositoryBranchesRequestRequestTypeDef,
 ):
     pass
 
 
-ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
-    "ListSpacesRequestListSpacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSpacesRequestRequestTypeDef = TypedDict(
     "ListSpacesRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredSpaceSummaryTypeDef = TypedDict(
-    "_RequiredSpaceSummaryTypeDef",
+SpaceSummaryTypeDef = TypedDict(
+    "SpaceSummaryTypeDef",
     {
         "name": str,
         "regionName": str,
+        "displayName": str,
+        "description": str,
     },
 )
-_OptionalSpaceSummaryTypeDef = TypedDict(
-    "_OptionalSpaceSummaryTypeDef",
+
+StopDevEnvironmentRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+    },
+)
+
+StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "sessionId": str,
+    },
+)
+
+_RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProjectRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+    },
+)
+_OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProjectRequestRequestTypeDef",
     {
-        "displayName": str,
         "description": str,
     },
     total=False,
 )
 
 
-class SpaceSummaryTypeDef(_RequiredSpaceSummaryTypeDef, _OptionalSpaceSummaryTypeDef):
+class UpdateProjectRequestRequestTypeDef(
+    _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
+):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredUpdateSpaceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSpaceRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "name": str,
+    },
+)
+_OptionalUpdateSpaceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSpaceRequestRequestTypeDef",
+    {
+        "description": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+class UpdateSpaceRequestRequestTypeDef(
+    _RequiredUpdateSpaceRequestRequestTypeDef, _OptionalUpdateSpaceRequestRequestTypeDef
+):
+    pass
+
+
+CreateAccessTokenResponseTypeDef = TypedDict(
+    "CreateAccessTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "secret": str,
+        "name": str,
+        "expiresTime": datetime,
+        "accessTokenId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDevEnvironmentResponseTypeDef = TypedDict(
-    "StartDevEnvironmentResponseTypeDef",
+CreateDevEnvironmentResponseTypeDef = TypedDict(
+    "CreateDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "status": DevEnvironmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentRequestRequestTypeDef",
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
     {
         "spaceName": str,
-        "projectName": str,
-        "id": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentResponseTypeDef = TypedDict(
-    "StopDevEnvironmentResponseTypeDef",
+CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryBranchResponseTypeDef",
     {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "status": DevEnvironmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ref": str,
+        "name": str,
+        "lastUpdatedTime": datetime,
+        "headCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentSessionRequestRequestTypeDef",
+CreateSourceRepositoryResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
-        "id": str,
-        "sessionId": str,
+        "name": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentSessionResponseTypeDef = TypedDict(
-    "StopDevEnvironmentSessionResponseTypeDef",
+DeleteDevEnvironmentResponseTypeDef = TypedDict(
+    "DeleteDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateProjectRequestRequestTypeDef",
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
     {
         "spaceName": str,
         "name": str,
+        "displayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateProjectRequestRequestTypeDef",
+
+DeleteSourceRepositoryResponseTypeDef = TypedDict(
+    "DeleteSourceRepositoryResponseTypeDef",
     {
-        "description": str,
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+DeleteSpaceResponseTypeDef = TypedDict(
+    "DeleteSpaceResponseTypeDef",
+    {
+        "name": str,
+        "displayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateProjectRequestRequestTypeDef(
-    _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
-):
-    pass
-
-
-UpdateProjectResponseTypeDef = TypedDict(
-    "UpdateProjectResponseTypeDef",
+GetProjectResponseTypeDef = TypedDict(
+    "GetProjectResponseTypeDef",
     {
         "spaceName": str,
         "name": str,
         "displayName": str,
         "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSpaceRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSpaceRequestRequestTypeDef",
+GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
     {
+        "https": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSourceRepositoryResponseTypeDef = TypedDict(
+    "GetSourceRepositoryResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
         "name": str,
+        "description": str,
+        "lastUpdatedTime": datetime,
+        "createdTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateSpaceRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSpaceRequestRequestTypeDef",
+
+GetSpaceResponseTypeDef = TypedDict(
+    "GetSpaceResponseTypeDef",
     {
+        "name": str,
+        "regionName": str,
+        "displayName": str,
         "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetSubscriptionResponseTypeDef = TypedDict(
+    "GetSubscriptionResponseTypeDef",
+    {
+        "subscriptionType": str,
+        "awsAccountName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateSpaceRequestRequestTypeDef(
-    _RequiredUpdateSpaceRequestRequestTypeDef, _OptionalUpdateSpaceRequestRequestTypeDef
-):
-    pass
+ListAccessTokensResponseTypeDef = TypedDict(
+    "ListAccessTokensResponseTypeDef",
+    {
+        "items": List[AccessTokenSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDevEnvironmentResponseTypeDef = TypedDict(
+    "StartDevEnvironmentResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "status": DevEnvironmentStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDevEnvironmentResponseTypeDef = TypedDict(
+    "StopDevEnvironmentResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "status": DevEnvironmentStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDevEnvironmentSessionResponseTypeDef = TypedDict(
+    "StopDevEnvironmentSessionResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "sessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateProjectResponseTypeDef = TypedDict(
+    "UpdateProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 UpdateSpaceResponseTypeDef = TypedDict(
     "UpdateSpaceResponseTypeDef",
     {
         "name": str,
         "displayName": str,
         "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VerifySessionResponseTypeDef = TypedDict(
     "VerifySessionResponseTypeDef",
     {
         "identity": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAccessTokensResponseTypeDef = TypedDict(
-    "ListAccessTokensResponseTypeDef",
-    {
-        "items": List[AccessTokenSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1249,15 +1059,15 @@
     "StartDevEnvironmentSessionResponseTypeDef",
     {
         "accessDetails": DevEnvironmentAccessDetailsTypeDef,
         "sessionId": str,
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDevEnvironmentSessionConfigurationTypeDef = TypedDict(
     "_RequiredDevEnvironmentSessionConfigurationTypeDef",
     {
         "sessionType": DevEnvironmentSessionTypeType,
@@ -1280,49 +1090,36 @@
 
 
 ListDevEnvironmentSessionsResponseTypeDef = TypedDict(
     "ListDevEnvironmentSessionsResponseTypeDef",
     {
         "items": List[DevEnvironmentSessionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDevEnvironmentSummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentSummaryTypeDef",
+DevEnvironmentSummaryTypeDef = TypedDict(
+    "DevEnvironmentSummaryTypeDef",
     {
+        "spaceName": str,
+        "projectName": str,
         "id": str,
         "lastUpdatedTime": datetime,
         "creatorId": str,
         "status": DevEnvironmentStatusType,
+        "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
+        "alias": str,
+        "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
     },
 )
-_OptionalDevEnvironmentSummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentSummaryTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "statusReason": str,
-        "alias": str,
-        "ides": List[IdeTypeDef],
-    },
-    total=False,
-)
-
-
-class DevEnvironmentSummaryTypeDef(
-    _RequiredDevEnvironmentSummaryTypeDef, _OptionalDevEnvironmentSummaryTypeDef
-):
-    pass
-
 
 GetDevEnvironmentResponseTypeDef = TypedDict(
     "GetDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
@@ -1332,137 +1129,238 @@
         "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
         "alias": str,
         "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserDetailsResponseTypeDef = TypedDict(
     "GetUserDetailsResponseTypeDef",
     {
         "userId": str,
         "userName": str,
         "displayName": str,
         "primaryEmail": EmailAddressTypeDef,
         "version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEventLogEntryTypeDef = TypedDict(
-    "_RequiredEventLogEntryTypeDef",
+EventLogEntryTypeDef = TypedDict(
+    "EventLogEntryTypeDef",
     {
         "id": str,
         "eventName": str,
         "eventType": str,
         "eventCategory": str,
         "eventSource": str,
         "eventTime": datetime,
         "operationType": OperationTypeType,
         "userIdentity": UserIdentityTypeDef,
-    },
-)
-_OptionalEventLogEntryTypeDef = TypedDict(
-    "_OptionalEventLogEntryTypeDef",
-    {
         "projectInformation": ProjectInformationTypeDef,
         "requestId": str,
         "requestPayload": EventPayloadTypeDef,
         "responsePayload": EventPayloadTypeDef,
         "errorCode": str,
         "sourceIpAddress": str,
         "userAgent": str,
     },
+)
+
+_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+    },
+)
+_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
+    {
+        "filters": Sequence[FilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListDevEnvironmentsRequestRequestTypeDef(
+    _RequiredListDevEnvironmentsRequestRequestTypeDef,
+    _OptionalListDevEnvironmentsRequestRequestTypeDef,
+):
+    pass
+
+
+UpdateDevEnvironmentResponseTypeDef = TypedDict(
+    "UpdateDevEnvironmentResponseTypeDef",
+    {
+        "id": str,
+        "spaceName": str,
+        "projectName": str,
+        "alias": str,
+        "ides": List[IdeConfigurationOutputTypeDef],
+        "instanceType": InstanceTypeType,
+        "inactivityTimeoutMinutes": int,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "devEnvironmentId": str,
+    },
+)
+_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
 
-class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
+class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
+    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+):
     pass
 
 
 _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
 _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef(
     _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
+_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "eventName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEventLogsRequestListEventLogsPaginateTypeDef(
+    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
+    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
-_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
+_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListDevEnvironmentsRequestRequestTypeDef(
-    _RequiredListDevEnvironmentsRequestRequestTypeDef,
-    _OptionalListDevEnvironmentsRequestRequestTypeDef,
+class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
+    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
 ):
     pass
 
 
-UpdateDevEnvironmentResponseTypeDef = TypedDict(
-    "UpdateDevEnvironmentResponseTypeDef",
+_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     {
-        "id": str,
         "spaceName": str,
         "projectName": str,
-        "alias": str,
-        "ides": List[IdeConfigurationOutputTypeDef],
-        "instanceType": InstanceTypeType,
-        "inactivityTimeoutMinutes": int,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sourceRepositoryName": str,
+    },
+)
+_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+
+class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
+    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+):
+    pass
+
+
+ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
+    "ListSpacesRequestListSpacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 _RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
     {
         "spaceName": str,
     },
 )
 _OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
     {
         "filters": Sequence[ProjectListFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListProjectsRequestListProjectsPaginateTypeDef(
     _RequiredListProjectsRequestListProjectsPaginateTypeDef,
@@ -1495,42 +1393,42 @@
 
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSourceRepositoriesResponseTypeDef = TypedDict(
     "ListSourceRepositoriesResponseTypeDef",
     {
         "items": List[ListSourceRepositoriesItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSourceRepositoryBranchesResponseTypeDef = TypedDict(
     "ListSourceRepositoryBranchesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ListSourceRepositoryBranchesItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpacesResponseTypeDef = TypedDict(
     "ListSpacesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[SpaceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1541,19 +1439,19 @@
 )
 
 ListDevEnvironmentsResponseTypeDef = TypedDict(
     "ListDevEnvironmentsResponseTypeDef",
     {
         "items": List[DevEnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventLogsResponseTypeDef = TypedDict(
     "ListEventLogsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[EventLogEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst/type_defs.pyi` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -32,132 +32,121 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessTokenSummaryTypeDef",
     "CreateAccessTokenRequestRequestTypeDef",
-    "CreateAccessTokenResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "IdeConfigurationTypeDef",
     "PersistentStorageConfigurationTypeDef",
     "RepositoryInputTypeDef",
-    "CreateDevEnvironmentResponseTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "CreateProjectResponseTypeDef",
     "CreateSourceRepositoryBranchRequestRequestTypeDef",
-    "CreateSourceRepositoryBranchResponseTypeDef",
     "CreateSourceRepositoryRequestRequestTypeDef",
-    "CreateSourceRepositoryResponseTypeDef",
     "DeleteAccessTokenRequestRequestTypeDef",
     "DeleteDevEnvironmentRequestRequestTypeDef",
-    "DeleteDevEnvironmentResponseTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResponseTypeDef",
     "DeleteSourceRepositoryRequestRequestTypeDef",
-    "DeleteSourceRepositoryResponseTypeDef",
     "DeleteSpaceRequestRequestTypeDef",
-    "DeleteSpaceResponseTypeDef",
     "DevEnvironmentAccessDetailsTypeDef",
     "DevEnvironmentRepositorySummaryTypeDef",
     "ExecuteCommandSessionConfigurationTypeDef",
     "DevEnvironmentSessionSummaryTypeDef",
     "IdeTypeDef",
     "PersistentStorageTypeDef",
     "EmailAddressTypeDef",
     "EventPayloadTypeDef",
     "ProjectInformationTypeDef",
     "UserIdentityTypeDef",
     "FilterTypeDef",
     "GetDevEnvironmentRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
-    "GetProjectResponseTypeDef",
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
     "GetSourceRepositoryRequestRequestTypeDef",
-    "GetSourceRepositoryResponseTypeDef",
     "GetSpaceRequestRequestTypeDef",
-    "GetSpaceResponseTypeDef",
     "GetSubscriptionRequestRequestTypeDef",
-    "GetSubscriptionResponseTypeDef",
     "GetUserDetailsRequestRequestTypeDef",
     "IdeConfigurationOutputTypeDef",
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessTokensRequestRequestTypeDef",
-    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
     "ListDevEnvironmentSessionsRequestRequestTypeDef",
-    "ListEventLogsRequestListEventLogsPaginateTypeDef",
     "ListEventLogsRequestRequestTypeDef",
     "ProjectListFilterTypeDef",
     "ProjectSummaryTypeDef",
     "ListSourceRepositoriesItemTypeDef",
-    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     "ListSourceRepositoriesRequestRequestTypeDef",
     "ListSourceRepositoryBranchesItemTypeDef",
-    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     "ListSourceRepositoryBranchesRequestRequestTypeDef",
-    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentRequestRequestTypeDef",
-    "StopDevEnvironmentResponseTypeDef",
     "StopDevEnvironmentSessionRequestRequestTypeDef",
-    "StopDevEnvironmentSessionResponseTypeDef",
     "UpdateProjectRequestRequestTypeDef",
-    "UpdateProjectResponseTypeDef",
     "UpdateSpaceRequestRequestTypeDef",
+    "CreateAccessTokenResponseTypeDef",
+    "CreateDevEnvironmentResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateSourceRepositoryBranchResponseTypeDef",
+    "CreateSourceRepositoryResponseTypeDef",
+    "DeleteDevEnvironmentResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "DeleteSourceRepositoryResponseTypeDef",
+    "DeleteSpaceResponseTypeDef",
+    "GetProjectResponseTypeDef",
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
+    "GetSourceRepositoryResponseTypeDef",
+    "GetSpaceResponseTypeDef",
+    "GetSubscriptionResponseTypeDef",
+    "ListAccessTokensResponseTypeDef",
+    "StartDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentResponseTypeDef",
+    "StopDevEnvironmentSessionResponseTypeDef",
+    "UpdateProjectResponseTypeDef",
     "UpdateSpaceResponseTypeDef",
     "VerifySessionResponseTypeDef",
-    "ListAccessTokensResponseTypeDef",
     "StartDevEnvironmentRequestRequestTypeDef",
     "UpdateDevEnvironmentRequestRequestTypeDef",
     "CreateDevEnvironmentRequestRequestTypeDef",
     "StartDevEnvironmentSessionResponseTypeDef",
     "DevEnvironmentSessionConfigurationTypeDef",
     "ListDevEnvironmentSessionsResponseTypeDef",
     "DevEnvironmentSummaryTypeDef",
     "GetDevEnvironmentResponseTypeDef",
     "GetUserDetailsResponseTypeDef",
     "EventLogEntryTypeDef",
-    "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     "ListDevEnvironmentsRequestRequestTypeDef",
     "UpdateDevEnvironmentResponseTypeDef",
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    "ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    "ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
+    "ListEventLogsRequestListEventLogsPaginateTypeDef",
+    "ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
+    "ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSourceRepositoriesResponseTypeDef",
     "ListSourceRepositoryBranchesResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     "ListDevEnvironmentsResponseTypeDef",
     "ListEventLogsResponseTypeDef",
 )
 
-_RequiredAccessTokenSummaryTypeDef = TypedDict(
-    "_RequiredAccessTokenSummaryTypeDef",
+AccessTokenSummaryTypeDef = TypedDict(
+    "AccessTokenSummaryTypeDef",
     {
         "id": str,
         "name": str,
-    },
-)
-_OptionalAccessTokenSummaryTypeDef = TypedDict(
-    "_OptionalAccessTokenSummaryTypeDef",
-    {
         "expiresTime": datetime,
     },
-    total=False,
 )
 
-class AccessTokenSummaryTypeDef(
-    _RequiredAccessTokenSummaryTypeDef, _OptionalAccessTokenSummaryTypeDef
-):
-    pass
-
 _RequiredCreateAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessTokenRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAccessTokenRequestRequestTypeDef = TypedDict(
@@ -169,22 +158,22 @@
 )
 
 class CreateAccessTokenRequestRequestTypeDef(
     _RequiredCreateAccessTokenRequestRequestTypeDef, _OptionalCreateAccessTokenRequestRequestTypeDef
 ):
     pass
 
-CreateAccessTokenResponseTypeDef = TypedDict(
-    "CreateAccessTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "secret": str,
-        "name": str,
-        "expiresTime": datetime,
-        "accessTokenId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 IdeConfigurationTypeDef = TypedDict(
     "IdeConfigurationTypeDef",
     {
         "runtime": str,
@@ -213,24 +202,14 @@
     },
     total=False,
 )
 
 class RepositoryInputTypeDef(_RequiredRepositoryInputTypeDef, _OptionalRepositoryInputTypeDef):
     pass
 
-CreateDevEnvironmentResponseTypeDef = TypedDict(
-    "CreateDevEnvironmentResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "displayName": str,
     },
 )
@@ -243,25 +222,14 @@
 )
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSourceRepositoryBranchRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
         "name": str,
@@ -277,25 +245,14 @@
 
 class CreateSourceRepositoryBranchRequestRequestTypeDef(
     _RequiredCreateSourceRepositoryBranchRequestRequestTypeDef,
     _OptionalCreateSourceRepositoryBranchRequestRequestTypeDef,
 ):
     pass
 
-CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
-    "CreateSourceRepositoryBranchResponseTypeDef",
-    {
-        "ref": str,
-        "name": str,
-        "lastUpdatedTime": datetime,
-        "headCommitId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSourceRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSourceRepositoryRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "name": str,
     },
@@ -310,25 +267,14 @@
 
 class CreateSourceRepositoryRequestRequestTypeDef(
     _RequiredCreateSourceRepositoryRequestRequestTypeDef,
     _OptionalCreateSourceRepositoryRequestRequestTypeDef,
 ):
     pass
 
-CreateSourceRepositoryResponseTypeDef = TypedDict(
-    "CreateSourceRepositoryResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "name": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccessTokenRequestRequestTypeDef = TypedDict(
     "DeleteAccessTokenRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -337,104 +283,54 @@
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
     },
 )
 
-DeleteDevEnvironmentResponseTypeDef = TypedDict(
-    "DeleteDevEnvironmentResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "name": str,
     },
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSourceRepositoryRequestRequestTypeDef = TypedDict(
     "DeleteSourceRepositoryRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "name": str,
     },
 )
 
-DeleteSourceRepositoryResponseTypeDef = TypedDict(
-    "DeleteSourceRepositoryResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSpaceRequestRequestTypeDef = TypedDict(
     "DeleteSpaceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteSpaceResponseTypeDef = TypedDict(
-    "DeleteSpaceResponseTypeDef",
-    {
-        "name": str,
-        "displayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DevEnvironmentAccessDetailsTypeDef = TypedDict(
     "DevEnvironmentAccessDetailsTypeDef",
     {
         "streamUrl": str,
         "tokenValue": str,
     },
 )
 
-_RequiredDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentRepositorySummaryTypeDef",
+DevEnvironmentRepositorySummaryTypeDef = TypedDict(
+    "DevEnvironmentRepositorySummaryTypeDef",
     {
         "repositoryName": str,
-    },
-)
-_OptionalDevEnvironmentRepositorySummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentRepositorySummaryTypeDef",
-    {
         "branchName": str,
     },
-    total=False,
 )
 
-class DevEnvironmentRepositorySummaryTypeDef(
-    _RequiredDevEnvironmentRepositorySummaryTypeDef, _OptionalDevEnvironmentRepositorySummaryTypeDef
-):
-    pass
-
 _RequiredExecuteCommandSessionConfigurationTypeDef = TypedDict(
     "_RequiredExecuteCommandSessionConfigurationTypeDef",
     {
         "command": str,
     },
 )
 _OptionalExecuteCommandSessionConfigurationTypeDef = TypedDict(
@@ -464,15 +360,14 @@
 
 IdeTypeDef = TypedDict(
     "IdeTypeDef",
     {
         "runtime": str,
         "name": str,
     },
-    total=False,
 )
 
 PersistentStorageTypeDef = TypedDict(
     "PersistentStorageTypeDef",
     {
         "sizeInGiB": int,
     },
@@ -480,54 +375,42 @@
 
 EmailAddressTypeDef = TypedDict(
     "EmailAddressTypeDef",
     {
         "email": str,
         "verified": bool,
     },
-    total=False,
 )
 
 EventPayloadTypeDef = TypedDict(
     "EventPayloadTypeDef",
     {
         "contentType": str,
         "data": str,
     },
-    total=False,
 )
 
 ProjectInformationTypeDef = TypedDict(
     "ProjectInformationTypeDef",
     {
         "name": str,
         "projectId": str,
     },
-    total=False,
 )
 
-_RequiredUserIdentityTypeDef = TypedDict(
-    "_RequiredUserIdentityTypeDef",
+UserIdentityTypeDef = TypedDict(
+    "UserIdentityTypeDef",
     {
         "userType": UserTypeType,
         "principalId": str,
-    },
-)
-_OptionalUserIdentityTypeDef = TypedDict(
-    "_OptionalUserIdentityTypeDef",
-    {
         "userName": str,
         "awsAccountId": str,
     },
-    total=False,
 )
 
-class UserIdentityTypeDef(_RequiredUserIdentityTypeDef, _OptionalUserIdentityTypeDef):
-    pass
-
 _RequiredFilterTypeDef = TypedDict(
     "_RequiredFilterTypeDef",
     {
         "key": str,
         "values": Sequence[str],
     },
 )
@@ -555,98 +438,46 @@
     "GetProjectRequestRequestTypeDef",
     {
         "spaceName": str,
         "name": str,
     },
 )
 
-GetProjectResponseTypeDef = TypedDict(
-    "GetProjectResponseTypeDef",
-    {
-        "spaceName": str,
-        "name": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSourceRepositoryCloneUrlsRequestRequestTypeDef = TypedDict(
     "GetSourceRepositoryCloneUrlsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
 )
 
-GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
-    "GetSourceRepositoryCloneUrlsResponseTypeDef",
-    {
-        "https": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSourceRepositoryRequestRequestTypeDef = TypedDict(
     "GetSourceRepositoryRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "name": str,
     },
 )
 
-GetSourceRepositoryResponseTypeDef = TypedDict(
-    "GetSourceRepositoryResponseTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "name": str,
-        "description": str,
-        "lastUpdatedTime": datetime,
-        "createdTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSpaceRequestRequestTypeDef = TypedDict(
     "GetSpaceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetSpaceResponseTypeDef = TypedDict(
-    "GetSpaceResponseTypeDef",
-    {
-        "name": str,
-        "regionName": str,
-        "displayName": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSubscriptionRequestRequestTypeDef = TypedDict(
     "GetSubscriptionRequestRequestTypeDef",
     {
         "spaceName": str,
     },
 )
 
-GetSubscriptionResponseTypeDef = TypedDict(
-    "GetSubscriptionResponseTypeDef",
-    {
-        "subscriptionType": str,
-        "awsAccountName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetUserDetailsRequestRequestTypeDef = TypedDict(
     "GetUserDetailsRequestRequestTypeDef",
     {
         "id": str,
         "userName": str,
     },
     total=False,
@@ -654,56 +485,35 @@
 
 IdeConfigurationOutputTypeDef = TypedDict(
     "IdeConfigurationOutputTypeDef",
     {
         "runtime": str,
         "name": str,
     },
-    total=False,
 )
 
-ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
-    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccessTokensRequestRequestTypeDef = TypedDict(
     "ListAccessTokensRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "devEnvironmentId": str,
-    },
-)
-_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
-    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDevEnvironmentSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevEnvironmentSessionsRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "devEnvironmentId": str,
     },
@@ -719,37 +529,14 @@
 
 class ListDevEnvironmentSessionsRequestRequestTypeDef(
     _RequiredListDevEnvironmentSessionsRequestRequestTypeDef,
     _OptionalListDevEnvironmentSessionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "spaceName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
-    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
-    {
-        "eventName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListEventLogsRequestListEventLogsPaginateTypeDef(
-    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
-    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
-):
-    pass
-
 _RequiredListEventLogsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventLogsRequestRequestTypeDef",
     {
         "spaceName": str,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
@@ -785,74 +572,33 @@
 )
 
 class ProjectListFilterTypeDef(
     _RequiredProjectListFilterTypeDef, _OptionalProjectListFilterTypeDef
 ):
     pass
 
-_RequiredProjectSummaryTypeDef = TypedDict(
-    "_RequiredProjectSummaryTypeDef",
+ProjectSummaryTypeDef = TypedDict(
+    "ProjectSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalProjectSummaryTypeDef = TypedDict(
-    "_OptionalProjectSummaryTypeDef",
-    {
         "displayName": str,
         "description": str,
     },
-    total=False,
 )
 
-class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
-    pass
-
-_RequiredListSourceRepositoriesItemTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesItemTypeDef",
+ListSourceRepositoriesItemTypeDef = TypedDict(
+    "ListSourceRepositoriesItemTypeDef",
     {
         "id": str,
         "name": str,
+        "description": str,
         "lastUpdatedTime": datetime,
         "createdTime": datetime,
     },
 )
-_OptionalListSourceRepositoriesItemTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesItemTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-class ListSourceRepositoriesItemTypeDef(
-    _RequiredListSourceRepositoriesItemTypeDef, _OptionalListSourceRepositoriesItemTypeDef
-):
-    pass
-
-_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-    },
-)
-_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
-    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
-):
-    pass
 
 _RequiredListSourceRepositoriesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoriesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
@@ -876,39 +622,16 @@
     "ListSourceRepositoryBranchesItemTypeDef",
     {
         "ref": str,
         "name": str,
         "lastUpdatedTime": datetime,
         "headCommitId": str,
     },
-    total=False,
 )
 
-_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "sourceRepositoryName": str,
-    },
-)
-_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
-    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
-    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
-):
-    pass
-
 _RequiredListSourceRepositoryBranchesRequestRequestTypeDef = TypedDict(
     "_RequiredListSourceRepositoryBranchesRequestRequestTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "sourceRepositoryName": str,
     },
@@ -924,196 +647,303 @@
 
 class ListSourceRepositoryBranchesRequestRequestTypeDef(
     _RequiredListSourceRepositoryBranchesRequestRequestTypeDef,
     _OptionalListSourceRepositoryBranchesRequestRequestTypeDef,
 ):
     pass
 
-ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
-    "ListSpacesRequestListSpacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSpacesRequestRequestTypeDef = TypedDict(
     "ListSpacesRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredSpaceSummaryTypeDef = TypedDict(
-    "_RequiredSpaceSummaryTypeDef",
+SpaceSummaryTypeDef = TypedDict(
+    "SpaceSummaryTypeDef",
     {
         "name": str,
         "regionName": str,
+        "displayName": str,
+        "description": str,
     },
 )
-_OptionalSpaceSummaryTypeDef = TypedDict(
-    "_OptionalSpaceSummaryTypeDef",
+
+StopDevEnvironmentRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+    },
+)
+
+StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
+    "StopDevEnvironmentSessionRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "sessionId": str,
+    },
+)
+
+_RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProjectRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+    },
+)
+_OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProjectRequestRequestTypeDef",
     {
-        "displayName": str,
         "description": str,
     },
     total=False,
 )
 
-class SpaceSummaryTypeDef(_RequiredSpaceSummaryTypeDef, _OptionalSpaceSummaryTypeDef):
+class UpdateProjectRequestRequestTypeDef(
+    _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
+):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredUpdateSpaceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSpaceRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "name": str,
+    },
+)
+_OptionalUpdateSpaceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSpaceRequestRequestTypeDef",
+    {
+        "description": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+class UpdateSpaceRequestRequestTypeDef(
+    _RequiredUpdateSpaceRequestRequestTypeDef, _OptionalUpdateSpaceRequestRequestTypeDef
+):
+    pass
+
+CreateAccessTokenResponseTypeDef = TypedDict(
+    "CreateAccessTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "secret": str,
+        "name": str,
+        "expiresTime": datetime,
+        "accessTokenId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDevEnvironmentResponseTypeDef = TypedDict(
-    "StartDevEnvironmentResponseTypeDef",
+CreateDevEnvironmentResponseTypeDef = TypedDict(
+    "CreateDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "status": DevEnvironmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentRequestRequestTypeDef",
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
     {
         "spaceName": str,
-        "projectName": str,
-        "id": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentResponseTypeDef = TypedDict(
-    "StopDevEnvironmentResponseTypeDef",
+CreateSourceRepositoryBranchResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryBranchResponseTypeDef",
     {
-        "spaceName": str,
-        "projectName": str,
-        "id": str,
-        "status": DevEnvironmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ref": str,
+        "name": str,
+        "lastUpdatedTime": datetime,
+        "headCommitId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
-    "StopDevEnvironmentSessionRequestRequestTypeDef",
+CreateSourceRepositoryResponseTypeDef = TypedDict(
+    "CreateSourceRepositoryResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
-        "id": str,
-        "sessionId": str,
+        "name": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopDevEnvironmentSessionResponseTypeDef = TypedDict(
-    "StopDevEnvironmentSessionResponseTypeDef",
+DeleteDevEnvironmentResponseTypeDef = TypedDict(
+    "DeleteDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateProjectRequestRequestTypeDef",
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
     {
         "spaceName": str,
         "name": str,
+        "displayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateProjectRequestRequestTypeDef",
+
+DeleteSourceRepositoryResponseTypeDef = TypedDict(
+    "DeleteSourceRepositoryResponseTypeDef",
     {
-        "description": str,
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateProjectRequestRequestTypeDef(
-    _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
-):
-    pass
+DeleteSpaceResponseTypeDef = TypedDict(
+    "DeleteSpaceResponseTypeDef",
+    {
+        "name": str,
+        "displayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateProjectResponseTypeDef = TypedDict(
-    "UpdateProjectResponseTypeDef",
+GetProjectResponseTypeDef = TypedDict(
+    "GetProjectResponseTypeDef",
     {
         "spaceName": str,
         "name": str,
         "displayName": str,
         "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSpaceRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSpaceRequestRequestTypeDef",
+GetSourceRepositoryCloneUrlsResponseTypeDef = TypedDict(
+    "GetSourceRepositoryCloneUrlsResponseTypeDef",
     {
-        "name": str,
+        "https": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateSpaceRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSpaceRequestRequestTypeDef",
+
+GetSourceRepositoryResponseTypeDef = TypedDict(
+    "GetSourceRepositoryResponseTypeDef",
     {
+        "spaceName": str,
+        "projectName": str,
+        "name": str,
         "description": str,
+        "lastUpdatedTime": datetime,
+        "createdTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateSpaceRequestRequestTypeDef(
-    _RequiredUpdateSpaceRequestRequestTypeDef, _OptionalUpdateSpaceRequestRequestTypeDef
-):
-    pass
-
-UpdateSpaceResponseTypeDef = TypedDict(
-    "UpdateSpaceResponseTypeDef",
+GetSpaceResponseTypeDef = TypedDict(
+    "GetSpaceResponseTypeDef",
     {
         "name": str,
+        "regionName": str,
         "displayName": str,
         "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VerifySessionResponseTypeDef = TypedDict(
-    "VerifySessionResponseTypeDef",
+GetSubscriptionResponseTypeDef = TypedDict(
+    "GetSubscriptionResponseTypeDef",
     {
-        "identity": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "subscriptionType": str,
+        "awsAccountName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccessTokensResponseTypeDef = TypedDict(
     "ListAccessTokensResponseTypeDef",
     {
         "items": List[AccessTokenSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDevEnvironmentResponseTypeDef = TypedDict(
+    "StartDevEnvironmentResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "status": DevEnvironmentStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDevEnvironmentResponseTypeDef = TypedDict(
+    "StopDevEnvironmentResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "status": DevEnvironmentStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDevEnvironmentSessionResponseTypeDef = TypedDict(
+    "StopDevEnvironmentSessionResponseTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "id": str,
+        "sessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProjectResponseTypeDef = TypedDict(
+    "UpdateProjectResponseTypeDef",
+    {
+        "spaceName": str,
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSpaceResponseTypeDef = TypedDict(
+    "UpdateSpaceResponseTypeDef",
+    {
+        "name": str,
+        "displayName": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifySessionResponseTypeDef = TypedDict(
+    "VerifySessionResponseTypeDef",
+    {
+        "identity": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartDevEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartDevEnvironmentRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1194,15 +1024,15 @@
     "StartDevEnvironmentSessionResponseTypeDef",
     {
         "accessDetails": DevEnvironmentAccessDetailsTypeDef,
         "sessionId": str,
         "spaceName": str,
         "projectName": str,
         "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDevEnvironmentSessionConfigurationTypeDef = TypedDict(
     "_RequiredDevEnvironmentSessionConfigurationTypeDef",
     {
         "sessionType": DevEnvironmentSessionTypeType,
@@ -1223,47 +1053,36 @@
     pass
 
 ListDevEnvironmentSessionsResponseTypeDef = TypedDict(
     "ListDevEnvironmentSessionsResponseTypeDef",
     {
         "items": List[DevEnvironmentSessionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDevEnvironmentSummaryTypeDef = TypedDict(
-    "_RequiredDevEnvironmentSummaryTypeDef",
+DevEnvironmentSummaryTypeDef = TypedDict(
+    "DevEnvironmentSummaryTypeDef",
     {
+        "spaceName": str,
+        "projectName": str,
         "id": str,
         "lastUpdatedTime": datetime,
         "creatorId": str,
         "status": DevEnvironmentStatusType,
+        "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
+        "alias": str,
+        "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
     },
 )
-_OptionalDevEnvironmentSummaryTypeDef = TypedDict(
-    "_OptionalDevEnvironmentSummaryTypeDef",
-    {
-        "spaceName": str,
-        "projectName": str,
-        "statusReason": str,
-        "alias": str,
-        "ides": List[IdeTypeDef],
-    },
-    total=False,
-)
-
-class DevEnvironmentSummaryTypeDef(
-    _RequiredDevEnvironmentSummaryTypeDef, _OptionalDevEnvironmentSummaryTypeDef
-):
-    pass
 
 GetDevEnvironmentResponseTypeDef = TypedDict(
     "GetDevEnvironmentResponseTypeDef",
     {
         "spaceName": str,
         "projectName": str,
         "id": str,
@@ -1273,131 +1092,226 @@
         "statusReason": str,
         "repositories": List[DevEnvironmentRepositorySummaryTypeDef],
         "alias": str,
         "ides": List[IdeTypeDef],
         "instanceType": InstanceTypeType,
         "inactivityTimeoutMinutes": int,
         "persistentStorage": PersistentStorageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserDetailsResponseTypeDef = TypedDict(
     "GetUserDetailsResponseTypeDef",
     {
         "userId": str,
         "userName": str,
         "displayName": str,
         "primaryEmail": EmailAddressTypeDef,
         "version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEventLogEntryTypeDef = TypedDict(
-    "_RequiredEventLogEntryTypeDef",
+EventLogEntryTypeDef = TypedDict(
+    "EventLogEntryTypeDef",
     {
         "id": str,
         "eventName": str,
         "eventType": str,
         "eventCategory": str,
         "eventSource": str,
         "eventTime": datetime,
         "operationType": OperationTypeType,
         "userIdentity": UserIdentityTypeDef,
-    },
-)
-_OptionalEventLogEntryTypeDef = TypedDict(
-    "_OptionalEventLogEntryTypeDef",
-    {
         "projectInformation": ProjectInformationTypeDef,
         "requestId": str,
         "requestPayload": EventPayloadTypeDef,
         "responsePayload": EventPayloadTypeDef,
         "errorCode": str,
         "sourceIpAddress": str,
         "userAgent": str,
     },
+)
+
+_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+    },
+)
+_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
+    {
+        "filters": Sequence[FilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListDevEnvironmentsRequestRequestTypeDef(
+    _RequiredListDevEnvironmentsRequestRequestTypeDef,
+    _OptionalListDevEnvironmentsRequestRequestTypeDef,
+):
+    pass
+
+UpdateDevEnvironmentResponseTypeDef = TypedDict(
+    "UpdateDevEnvironmentResponseTypeDef",
+    {
+        "id": str,
+        "spaceName": str,
+        "projectName": str,
+        "alias": str,
+        "ides": List[IdeConfigurationOutputTypeDef],
+        "instanceType": InstanceTypeType,
+        "inactivityTimeoutMinutes": int,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAccessTokensRequestListAccessTokensPaginateTypeDef = TypedDict(
+    "ListAccessTokensRequestListAccessTokensPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
     total=False,
 )
 
-class EventLogEntryTypeDef(_RequiredEventLogEntryTypeDef, _OptionalEventLogEntryTypeDef):
+_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "projectName": str,
+        "devEnvironmentId": str,
+    },
+)
+_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef(
+    _RequiredListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    _OptionalListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+):
     pass
 
 _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
 _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef = TypedDict(
     "_OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef(
     _RequiredListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     _OptionalListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
 ):
     pass
 
-_RequiredListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDevEnvironmentsRequestRequestTypeDef",
+_RequiredListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_RequiredListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "spaceName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListEventLogsRequestListEventLogsPaginateTypeDef = TypedDict(
+    "_OptionalListEventLogsRequestListEventLogsPaginateTypeDef",
+    {
+        "eventName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEventLogsRequestListEventLogsPaginateTypeDef(
+    _RequiredListEventLogsRequestListEventLogsPaginateTypeDef,
+    _OptionalListEventLogsRequestListEventLogsPaginateTypeDef,
+):
+    pass
+
+_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     {
         "spaceName": str,
         "projectName": str,
     },
 )
-_OptionalListDevEnvironmentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDevEnvironmentsRequestRequestTypeDef",
+_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListDevEnvironmentsRequestRequestTypeDef(
-    _RequiredListDevEnvironmentsRequestRequestTypeDef,
-    _OptionalListDevEnvironmentsRequestRequestTypeDef,
+class ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef(
+    _RequiredListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    _OptionalListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
 ):
     pass
 
-UpdateDevEnvironmentResponseTypeDef = TypedDict(
-    "UpdateDevEnvironmentResponseTypeDef",
+_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
     {
-        "id": str,
         "spaceName": str,
         "projectName": str,
-        "alias": str,
-        "ides": List[IdeConfigurationOutputTypeDef],
-        "instanceType": InstanceTypeType,
-        "inactivityTimeoutMinutes": int,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sourceRepositoryName": str,
+    },
+)
+_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef = TypedDict(
+    "_OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef(
+    _RequiredListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    _OptionalListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+):
+    pass
+
+ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
+    "ListSpacesRequestListSpacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 _RequiredListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_RequiredListProjectsRequestListProjectsPaginateTypeDef",
     {
         "spaceName": str,
     },
 )
 _OptionalListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "_OptionalListProjectsRequestListProjectsPaginateTypeDef",
     {
         "filters": Sequence[ProjectListFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListProjectsRequestListProjectsPaginateTypeDef(
     _RequiredListProjectsRequestListProjectsPaginateTypeDef,
     _OptionalListProjectsRequestListProjectsPaginateTypeDef,
@@ -1426,42 +1340,42 @@
     pass
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSourceRepositoriesResponseTypeDef = TypedDict(
     "ListSourceRepositoriesResponseTypeDef",
     {
         "items": List[ListSourceRepositoriesItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSourceRepositoryBranchesResponseTypeDef = TypedDict(
     "ListSourceRepositoryBranchesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[ListSourceRepositoryBranchesItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpacesResponseTypeDef = TypedDict(
     "ListSpacesResponseTypeDef",
     {
         "nextToken": str,
         "items": List[SpaceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDevEnvironmentSessionRequestRequestTypeDef = TypedDict(
     "StartDevEnvironmentSessionRequestRequestTypeDef",
     {
         "spaceName": str,
@@ -1472,19 +1386,19 @@
 )
 
 ListDevEnvironmentsResponseTypeDef = TypedDict(
     "ListDevEnvironmentsResponseTypeDef",
     {
         "items": List[DevEnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventLogsResponseTypeDef = TypedDict(
     "ListEventLogsResponseTypeDef",
     {
         "nextToken": str,
         "items": List[EventLogEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst.egg-info/PKG-INFO` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecatalyst
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeCatalyst 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.8
+Summary: Type annotations for boto3.CodeCatalyst 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codecatalyst"></a>
 
 # mypy-boto3-codecatalyst
 
 [![PyPI - mypy-boto3-codecatalyst](https://img.shields.io/pypi/v/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecatalyst.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecatalyst)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecatalyst)](https://pepy.tech/project/mypy-boto3-codecatalyst)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecatalyst?color=blue)](https://pypistats.org/packages/mypy-boto3-codecatalyst)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCatalyst 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
+[boto3.CodeCatalyst 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#CodeCatalyst)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codecatalyst docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecatalyst/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,101 +358,101 @@
 `mypy_boto3_codecatalyst.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codecatalyst.type_defs import (
     AccessTokenSummaryTypeDef,
     CreateAccessTokenRequestRequestTypeDef,
-    CreateAccessTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     IdeConfigurationTypeDef,
     PersistentStorageConfigurationTypeDef,
     RepositoryInputTypeDef,
-    CreateDevEnvironmentResponseTypeDef,
     CreateProjectRequestRequestTypeDef,
-    CreateProjectResponseTypeDef,
     CreateSourceRepositoryBranchRequestRequestTypeDef,
-    CreateSourceRepositoryBranchResponseTypeDef,
     CreateSourceRepositoryRequestRequestTypeDef,
-    CreateSourceRepositoryResponseTypeDef,
     DeleteAccessTokenRequestRequestTypeDef,
     DeleteDevEnvironmentRequestRequestTypeDef,
-    DeleteDevEnvironmentResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DeleteSourceRepositoryRequestRequestTypeDef,
-    DeleteSourceRepositoryResponseTypeDef,
     DeleteSpaceRequestRequestTypeDef,
-    DeleteSpaceResponseTypeDef,
     DevEnvironmentAccessDetailsTypeDef,
     DevEnvironmentRepositorySummaryTypeDef,
     ExecuteCommandSessionConfigurationTypeDef,
     DevEnvironmentSessionSummaryTypeDef,
     IdeTypeDef,
     PersistentStorageTypeDef,
     EmailAddressTypeDef,
     EventPayloadTypeDef,
     ProjectInformationTypeDef,
     UserIdentityTypeDef,
     FilterTypeDef,
     GetDevEnvironmentRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
-    GetProjectResponseTypeDef,
     GetSourceRepositoryCloneUrlsRequestRequestTypeDef,
-    GetSourceRepositoryCloneUrlsResponseTypeDef,
     GetSourceRepositoryRequestRequestTypeDef,
-    GetSourceRepositoryResponseTypeDef,
     GetSpaceRequestRequestTypeDef,
-    GetSpaceResponseTypeDef,
     GetSubscriptionRequestRequestTypeDef,
-    GetSubscriptionResponseTypeDef,
     GetUserDetailsRequestRequestTypeDef,
     IdeConfigurationOutputTypeDef,
-    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessTokensRequestRequestTypeDef,
-    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
     ListDevEnvironmentSessionsRequestRequestTypeDef,
-    ListEventLogsRequestListEventLogsPaginateTypeDef,
     ListEventLogsRequestRequestTypeDef,
     ProjectListFilterTypeDef,
     ProjectSummaryTypeDef,
     ListSourceRepositoriesItemTypeDef,
-    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
     ListSourceRepositoriesRequestRequestTypeDef,
     ListSourceRepositoryBranchesItemTypeDef,
-    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
     ListSourceRepositoryBranchesRequestRequestTypeDef,
-    ListSpacesRequestListSpacesPaginateTypeDef,
     ListSpacesRequestRequestTypeDef,
     SpaceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartDevEnvironmentResponseTypeDef,
     StopDevEnvironmentRequestRequestTypeDef,
-    StopDevEnvironmentResponseTypeDef,
     StopDevEnvironmentSessionRequestRequestTypeDef,
-    StopDevEnvironmentSessionResponseTypeDef,
     UpdateProjectRequestRequestTypeDef,
-    UpdateProjectResponseTypeDef,
     UpdateSpaceRequestRequestTypeDef,
+    CreateAccessTokenResponseTypeDef,
+    CreateDevEnvironmentResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateSourceRepositoryBranchResponseTypeDef,
+    CreateSourceRepositoryResponseTypeDef,
+    DeleteDevEnvironmentResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteSourceRepositoryResponseTypeDef,
+    DeleteSpaceResponseTypeDef,
+    GetProjectResponseTypeDef,
+    GetSourceRepositoryCloneUrlsResponseTypeDef,
+    GetSourceRepositoryResponseTypeDef,
+    GetSpaceResponseTypeDef,
+    GetSubscriptionResponseTypeDef,
+    ListAccessTokensResponseTypeDef,
+    StartDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentResponseTypeDef,
+    StopDevEnvironmentSessionResponseTypeDef,
+    UpdateProjectResponseTypeDef,
     UpdateSpaceResponseTypeDef,
     VerifySessionResponseTypeDef,
-    ListAccessTokensResponseTypeDef,
     StartDevEnvironmentRequestRequestTypeDef,
     UpdateDevEnvironmentRequestRequestTypeDef,
     CreateDevEnvironmentRequestRequestTypeDef,
     StartDevEnvironmentSessionResponseTypeDef,
     DevEnvironmentSessionConfigurationTypeDef,
     ListDevEnvironmentSessionsResponseTypeDef,
     DevEnvironmentSummaryTypeDef,
     GetDevEnvironmentResponseTypeDef,
     GetUserDetailsResponseTypeDef,
     EventLogEntryTypeDef,
-    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
     ListDevEnvironmentsRequestRequestTypeDef,
     UpdateDevEnvironmentResponseTypeDef,
+    ListAccessTokensRequestListAccessTokensPaginateTypeDef,
+    ListDevEnvironmentSessionsRequestListDevEnvironmentSessionsPaginateTypeDef,
+    ListDevEnvironmentsRequestListDevEnvironmentsPaginateTypeDef,
+    ListEventLogsRequestListEventLogsPaginateTypeDef,
+    ListSourceRepositoriesRequestListSourceRepositoriesPaginateTypeDef,
+    ListSourceRepositoryBranchesRequestListSourceRepositoryBranchesPaginateTypeDef,
+    ListSpacesRequestListSpacesPaginateTypeDef,
     ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ListProjectsResponseTypeDef,
     ListSourceRepositoriesResponseTypeDef,
     ListSourceRepositoryBranchesResponseTypeDef,
     ListSpacesResponseTypeDef,
     StartDevEnvironmentSessionRequestRequestTypeDef,
```

### Comparing `mypy-boto3-codecatalyst-1.28.12/mypy_boto3_codecatalyst.egg-info/SOURCES.txt` & `mypy-boto3-codecatalyst-1.28.8/mypy_boto3_codecatalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecatalyst-1.28.12/setup.py` & `mypy-boto3-codecatalyst-1.28.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codecatalyst",
-    version="1.28.12",
+    version="1.28.8",
     packages=["mypy_boto3_codecatalyst"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeCatalyst 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CodeCatalyst 1.28.8 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

