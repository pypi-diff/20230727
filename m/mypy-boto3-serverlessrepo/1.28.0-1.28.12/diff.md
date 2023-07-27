# Comparing `tmp/mypy-boto3-serverlessrepo-1.28.0.tar.gz` & `tmp/mypy-boto3-serverlessrepo-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-serverlessrepo-1.28.0.tar", last modified: Thu Jul  6 21:00:36 2023, max compression
+gzip compressed data, was "mypy-boto3-serverlessrepo-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
```

## Comparing `mypy-boto3-serverlessrepo-1.28.0.tar` & `mypy-boto3-serverlessrepo-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:36.210428 mypy-boto3-serverlessrepo-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-07-06 21:00:36.210428 mypy-boto3-serverlessrepo-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:36.202428 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-06 20:55:31.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-07-06 20:55:31.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-07-06 20:55:31.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:36.210428 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-07-06 21:00:35.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 21:00:36.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:35.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:35.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:35.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 21:00:35.000000 mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:36.210428 mypy-boto3-serverlessrepo-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-06 20:55:30.000000 mypy-boto3-serverlessrepo-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.409289 mypy-boto3-serverlessrepo-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-27 11:49:38.405289 mypy-boto3-serverlessrepo-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.401289 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19929 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19897 2023-07-27 11:46:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.405289 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-27 11:49:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 11:49:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:38.000000 mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.409289 mypy-boto3-serverlessrepo-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-27 11:46:37.000000 mypy-boto3-serverlessrepo-1.28.12/setup.py
```

### Comparing `mypy-boto3-serverlessrepo-1.28.0/LICENSE` & `mypy-boto3-serverlessrepo-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.0/PKG-INFO` & `mypy-boto3-serverlessrepo-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-serverlessrepo
-Version: 1.28.0
-Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-serverlessrepo"></a>
 
 # mypy-boto3-serverlessrepo
 
 [![PyPI - mypy-boto3-serverlessrepo](https://img.shields.io/pypi/v/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-serverlessrepo?color=blue)](https://pypistats.org/packages/mypy-boto3-serverlessrepo)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-serverlessrepo)](https://pepy.tech/project/mypy-boto3-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServerlessApplicationRepository 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[boto3.ServerlessApplicationRepository 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,49 +335,50 @@
 
 `mypy_boto3_serverlessrepo.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_serverlessrepo.type_defs import (
     ApplicationDependencySummaryTypeDef,
+    ApplicationPolicyStatementOutputTypeDef,
     ApplicationPolicyStatementTypeDef,
     ApplicationSummaryTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateApplicationVersionRequestRequestTypeDef,
     ParameterDefinitionTypeDef,
     ParameterValueTypeDef,
     TagTypeDef,
-    CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateRequestRequestTypeDef,
-    CreateCloudFormationTemplateResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationPolicyRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetCloudFormationTemplateRequestRequestTypeDef,
-    GetCloudFormationTemplateResponseTypeDef,
-    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationDependenciesRequestRequestTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     VersionSummaryTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RollbackTriggerTypeDef,
     UnshareApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    ListApplicationDependenciesResponseTypeDef,
-    GetApplicationPolicyResponseTypeDef,
     PutApplicationPolicyRequestRequestTypeDef,
-    PutApplicationPolicyResponseTypeDef,
+    CreateCloudFormationChangeSetResponseTypeDef,
+    CreateCloudFormationTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetApplicationPolicyResponseTypeDef,
+    GetCloudFormationTemplateResponseTypeDef,
+    ListApplicationDependenciesResponseTypeDef,
     ListApplicationsResponseTypeDef,
+    PutApplicationPolicyResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     VersionTypeDef,
+    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationVersionsResponseTypeDef,
     RollbackConfigurationTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     CreateCloudFormationChangeSetRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-serverlessrepo-1.28.0/README.md` & `mypy-boto3-serverlessrepo-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-serverlessrepo"></a>
 
 # mypy-boto3-serverlessrepo
 
 [![PyPI - mypy-boto3-serverlessrepo](https://img.shields.io/pypi/v/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-serverlessrepo?color=blue)](https://pypistats.org/packages/mypy-boto3-serverlessrepo)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-serverlessrepo)](https://pepy.tech/project/mypy-boto3-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServerlessApplicationRepository 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[boto3.ServerlessApplicationRepository 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,49 +303,50 @@
 
 `mypy_boto3_serverlessrepo.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_serverlessrepo.type_defs import (
     ApplicationDependencySummaryTypeDef,
+    ApplicationPolicyStatementOutputTypeDef,
     ApplicationPolicyStatementTypeDef,
     ApplicationSummaryTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateApplicationVersionRequestRequestTypeDef,
     ParameterDefinitionTypeDef,
     ParameterValueTypeDef,
     TagTypeDef,
-    CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateRequestRequestTypeDef,
-    CreateCloudFormationTemplateResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationPolicyRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetCloudFormationTemplateRequestRequestTypeDef,
-    GetCloudFormationTemplateResponseTypeDef,
-    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationDependenciesRequestRequestTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     VersionSummaryTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RollbackTriggerTypeDef,
     UnshareApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    ListApplicationDependenciesResponseTypeDef,
-    GetApplicationPolicyResponseTypeDef,
     PutApplicationPolicyRequestRequestTypeDef,
-    PutApplicationPolicyResponseTypeDef,
+    CreateCloudFormationChangeSetResponseTypeDef,
+    CreateCloudFormationTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetApplicationPolicyResponseTypeDef,
+    GetCloudFormationTemplateResponseTypeDef,
+    ListApplicationDependenciesResponseTypeDef,
     ListApplicationsResponseTypeDef,
+    PutApplicationPolicyResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     VersionTypeDef,
+    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationVersionsResponseTypeDef,
     RollbackConfigurationTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     CreateCloudFormationChangeSetRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/__init__.py` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/__init__.pyi` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/__main__.py` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServerlessApplicationRepository 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ServerlessApplicationRepository 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository\nOther"
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

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/client.py` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/client.pyi` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/literals.py` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,15 @@
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
@@ -242,26 +243,28 @@
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

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/literals.pyi` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/literals.pyi`

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

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/paginator.py` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,43 +58,43 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         SemanticVersion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationDependenciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationDependencies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationdependenciespaginator)
         """
 
 
 class ListApplicationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationversionspaginator)
     """
 
     def paginate(
-        self, *, ApplicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApplicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationversionspaginator)
         """
 
 
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationspaginator)
         """
```

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/paginator.pyi` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,41 +55,41 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationId: str,
         SemanticVersion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationDependenciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationDependencies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationdependenciespaginator)
         """
 
 class ListApplicationVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationversionspaginator)
     """
 
     def paginate(
-        self, *, ApplicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApplicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationversionspaginator)
         """
 
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/paginators/#listapplicationspaginator)
         """
```

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/type_defs.py` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -17,52 +17,52 @@
 from .literals import CapabilityType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationDependencySummaryTypeDef",
+    "ApplicationPolicyStatementOutputTypeDef",
     "ApplicationPolicyStatementTypeDef",
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateApplicationVersionRequestRequestTypeDef",
     "ParameterDefinitionTypeDef",
     "ParameterValueTypeDef",
     "TagTypeDef",
-    "CreateCloudFormationChangeSetResponseTypeDef",
     "CreateCloudFormationTemplateRequestRequestTypeDef",
-    "CreateCloudFormationTemplateResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetApplicationPolicyRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetCloudFormationTemplateRequestRequestTypeDef",
-    "GetCloudFormationTemplateResponseTypeDef",
-    "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationDependenciesRequestRequestTypeDef",
-    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "VersionSummaryTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RollbackTriggerTypeDef",
     "UnshareApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "ListApplicationDependenciesResponseTypeDef",
-    "GetApplicationPolicyResponseTypeDef",
     "PutApplicationPolicyRequestRequestTypeDef",
-    "PutApplicationPolicyResponseTypeDef",
+    "CreateCloudFormationChangeSetResponseTypeDef",
+    "CreateCloudFormationTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetApplicationPolicyResponseTypeDef",
+    "GetCloudFormationTemplateResponseTypeDef",
+    "ListApplicationDependenciesResponseTypeDef",
     "ListApplicationsResponseTypeDef",
+    "PutApplicationPolicyResponseTypeDef",
     "CreateApplicationVersionResponseTypeDef",
     "VersionTypeDef",
+    "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "RollbackConfigurationTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "CreateCloudFormationChangeSetRequestRequestTypeDef",
 )
@@ -71,37 +71,57 @@
     "ApplicationDependencySummaryTypeDef",
     {
         "ApplicationId": str,
         "SemanticVersion": str,
     },
 )
 
-_RequiredApplicationPolicyStatementTypeDef = TypedDict(
-    "_RequiredApplicationPolicyStatementTypeDef",
+_RequiredApplicationPolicyStatementOutputTypeDef = TypedDict(
+    "_RequiredApplicationPolicyStatementOutputTypeDef",
     {
         "Actions": List[str],
         "Principals": List[str],
     },
 )
-_OptionalApplicationPolicyStatementTypeDef = TypedDict(
-    "_OptionalApplicationPolicyStatementTypeDef",
+_OptionalApplicationPolicyStatementOutputTypeDef = TypedDict(
+    "_OptionalApplicationPolicyStatementOutputTypeDef",
     {
         "PrincipalOrgIDs": List[str],
         "StatementId": str,
     },
     total=False,
 )
 
+class ApplicationPolicyStatementOutputTypeDef(
+    _RequiredApplicationPolicyStatementOutputTypeDef,
+    _OptionalApplicationPolicyStatementOutputTypeDef,
+):
+    pass
+
+_RequiredApplicationPolicyStatementTypeDef = TypedDict(
+    "_RequiredApplicationPolicyStatementTypeDef",
+    {
+        "Actions": Sequence[str],
+        "Principals": Sequence[str],
+    },
+)
+_OptionalApplicationPolicyStatementTypeDef = TypedDict(
+    "_OptionalApplicationPolicyStatementTypeDef",
+    {
+        "PrincipalOrgIDs": Sequence[str],
+        "StatementId": str,
+    },
+    total=False,
+)
 
 class ApplicationPolicyStatementTypeDef(
     _RequiredApplicationPolicyStatementTypeDef, _OptionalApplicationPolicyStatementTypeDef
 ):
     pass
 
-
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
         "ApplicationId": str,
         "Author": str,
         "Description": str,
         "Name": str,
@@ -114,21 +134,19 @@
         "HomePageUrl": str,
         "Labels": List[str],
         "SpdxLicenseId": str,
     },
     total=False,
 )
 
-
 class ApplicationSummaryTypeDef(
     _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
 ):
     pass
 
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "Author": str,
         "Description": str,
         "Name": str,
     },
@@ -148,20 +166,29 @@
         "SpdxLicenseId": str,
         "TemplateBody": str,
         "TemplateUrl": str,
     },
     total=False,
 )
 
-
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
 
 _RequiredCreateApplicationVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationVersionRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SemanticVersion": str,
     },
@@ -173,22 +200,20 @@
         "SourceCodeUrl": str,
         "TemplateBody": str,
         "TemplateUrl": str,
     },
     total=False,
 )
 
-
 class CreateApplicationVersionRequestRequestTypeDef(
     _RequiredCreateApplicationVersionRequestRequestTypeDef,
     _OptionalCreateApplicationVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredParameterDefinitionTypeDef = TypedDict(
     "_RequiredParameterDefinitionTypeDef",
     {
         "Name": str,
         "ReferencedByResources": List[str],
     },
 )
@@ -206,21 +231,19 @@
         "MinValue": int,
         "NoEcho": bool,
         "Type": str,
     },
     total=False,
 )
 
-
 class ParameterDefinitionTypeDef(
     _RequiredParameterDefinitionTypeDef, _OptionalParameterDefinitionTypeDef
 ):
     pass
 
-
 ParameterValueTypeDef = TypedDict(
     "ParameterValueTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -229,75 +252,41 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
-    "CreateCloudFormationChangeSetResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "ChangeSetId": str,
-        "SemanticVersion": str,
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCloudFormationTemplateRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalCreateCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCloudFormationTemplateRequestRequestTypeDef",
     {
         "SemanticVersion": str,
     },
     total=False,
 )
 
-
 class CreateCloudFormationTemplateRequestRequestTypeDef(
     _RequiredCreateCloudFormationTemplateRequestRequestTypeDef,
     _OptionalCreateCloudFormationTemplateRequestRequestTypeDef,
 ):
     pass
 
-
-CreateCloudFormationTemplateResponseTypeDef = TypedDict(
-    "CreateCloudFormationTemplateResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "CreationTime": str,
-        "ExpirationTime": str,
-        "SemanticVersion": str,
-        "Status": StatusType,
-        "TemplateId": str,
-        "TemplateUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApplicationPolicyRequestRequestTypeDef = TypedDict(
     "GetApplicationPolicyRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -311,66 +300,37 @@
     "_OptionalGetApplicationRequestRequestTypeDef",
     {
         "SemanticVersion": str,
     },
     total=False,
 )
 
-
 class GetApplicationRequestRequestTypeDef(
     _RequiredGetApplicationRequestRequestTypeDef, _OptionalGetApplicationRequestRequestTypeDef
 ):
     pass
 
-
 GetCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "GetCloudFormationTemplateRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "TemplateId": str,
     },
 )
 
-GetCloudFormationTemplateResponseTypeDef = TypedDict(
-    "GetCloudFormationTemplateResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "CreationTime": str,
-        "ExpirationTime": str,
-        "SemanticVersion": str,
-        "Status": StatusType,
-        "TemplateId": str,
-        "TemplateUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "SemanticVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(
-    _RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-    _OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListApplicationDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationDependenciesRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalListApplicationDependenciesRequestRequestTypeDef = TypedDict(
@@ -379,44 +339,20 @@
         "MaxItems": int,
         "NextToken": str,
         "SemanticVersion": str,
     },
     total=False,
 )
 
-
 class ListApplicationDependenciesRequestRequestTypeDef(
     _RequiredListApplicationDependenciesRequestRequestTypeDef,
     _OptionalListApplicationDependenciesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
-    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -424,22 +360,20 @@
     {
         "MaxItems": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredVersionSummaryTypeDef = TypedDict(
     "_RequiredVersionSummaryTypeDef",
     {
         "ApplicationId": str,
         "CreationTime": str,
         "SemanticVersion": str,
     },
@@ -448,57 +382,26 @@
     "_OptionalVersionSummaryTypeDef",
     {
         "SourceCodeUrl": str,
     },
     total=False,
 )
 
-
 class VersionSummaryTypeDef(_RequiredVersionSummaryTypeDef, _OptionalVersionSummaryTypeDef):
     pass
 
-
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxItems": int,
         "NextToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
         "Type": str,
     },
 )
@@ -526,60 +429,104 @@
         "Labels": Sequence[str],
         "ReadmeBody": str,
         "ReadmeUrl": str,
     },
     total=False,
 )
 
-
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+PutApplicationPolicyRequestRequestTypeDef = TypedDict(
+    "PutApplicationPolicyRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
+    },
+)
 
-ListApplicationDependenciesResponseTypeDef = TypedDict(
-    "ListApplicationDependenciesResponseTypeDef",
+CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
+    "CreateCloudFormationChangeSetResponseTypeDef",
     {
-        "Dependencies": List[ApplicationDependencySummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationId": str,
+        "ChangeSetId": str,
+        "SemanticVersion": str,
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCloudFormationTemplateResponseTypeDef = TypedDict(
+    "CreateCloudFormationTemplateResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "CreationTime": str,
+        "ExpirationTime": str,
+        "SemanticVersion": str,
+        "Status": StatusType,
+        "TemplateId": str,
+        "TemplateUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationPolicyResponseTypeDef = TypedDict(
     "GetApplicationPolicyResponseTypeDef",
     {
-        "Statements": List[ApplicationPolicyStatementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Statements": List[ApplicationPolicyStatementOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutApplicationPolicyRequestRequestTypeDef = TypedDict(
-    "PutApplicationPolicyRequestRequestTypeDef",
+GetCloudFormationTemplateResponseTypeDef = TypedDict(
+    "GetCloudFormationTemplateResponseTypeDef",
     {
         "ApplicationId": str,
-        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
+        "CreationTime": str,
+        "ExpirationTime": str,
+        "SemanticVersion": str,
+        "Status": StatusType,
+        "TemplateId": str,
+        "TemplateUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutApplicationPolicyResponseTypeDef = TypedDict(
-    "PutApplicationPolicyResponseTypeDef",
+ListApplicationDependenciesResponseTypeDef = TypedDict(
+    "ListApplicationDependenciesResponseTypeDef",
     {
-        "Statements": List[ApplicationPolicyStatementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Dependencies": List[ApplicationDependencySummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "Applications": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutApplicationPolicyResponseTypeDef = TypedDict(
+    "PutApplicationPolicyResponseTypeDef",
+    {
+        "Statements": List[ApplicationPolicyStatementOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApplicationVersionResponseTypeDef = TypedDict(
     "CreateApplicationVersionResponseTypeDef",
     {
         "ApplicationId": str,
@@ -587,15 +534,15 @@
         "ParameterDefinitions": List[ParameterDefinitionTypeDef],
         "RequiredCapabilities": List[CapabilityType],
         "ResourcesSupported": bool,
         "SemanticVersion": str,
         "SourceCodeArchiveUrl": str,
         "SourceCodeUrl": str,
         "TemplateUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredVersionTypeDef = TypedDict(
     "_RequiredVersionTypeDef",
     {
         "ApplicationId": str,
@@ -612,25 +559,72 @@
     {
         "SourceCodeArchiveUrl": str,
         "SourceCodeUrl": str,
     },
     total=False,
 )
 
-
 class VersionTypeDef(_RequiredVersionTypeDef, _OptionalVersionTypeDef):
     pass
 
+_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    {
+        "SemanticVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(
+    _RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    _OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
+    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+):
+    pass
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 ListApplicationVersionsResponseTypeDef = TypedDict(
     "ListApplicationVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
         "MonitoringTimeInMinutes": int,
@@ -651,15 +645,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "ApplicationId": str,
@@ -671,15 +665,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "ApplicationId": str,
@@ -691,15 +685,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCloudFormationChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCloudFormationChangeSetRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -720,13 +714,12 @@
         "SemanticVersion": str,
         "Tags": Sequence[TagTypeDef],
         "TemplateId": str,
     },
     total=False,
 )
 
-
 class CreateCloudFormationChangeSetRequestRequestTypeDef(
     _RequiredCreateCloudFormationChangeSetRequestRequestTypeDef,
     _OptionalCreateCloudFormationChangeSetRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo/type_defs.pyi` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,51 +17,53 @@
 from .literals import CapabilityType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ApplicationDependencySummaryTypeDef",
+    "ApplicationPolicyStatementOutputTypeDef",
     "ApplicationPolicyStatementTypeDef",
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateApplicationVersionRequestRequestTypeDef",
     "ParameterDefinitionTypeDef",
     "ParameterValueTypeDef",
     "TagTypeDef",
-    "CreateCloudFormationChangeSetResponseTypeDef",
     "CreateCloudFormationTemplateRequestRequestTypeDef",
-    "CreateCloudFormationTemplateResponseTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetApplicationPolicyRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetCloudFormationTemplateRequestRequestTypeDef",
-    "GetCloudFormationTemplateResponseTypeDef",
-    "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationDependenciesRequestRequestTypeDef",
-    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "VersionSummaryTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RollbackTriggerTypeDef",
     "UnshareApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "ListApplicationDependenciesResponseTypeDef",
-    "GetApplicationPolicyResponseTypeDef",
     "PutApplicationPolicyRequestRequestTypeDef",
-    "PutApplicationPolicyResponseTypeDef",
+    "CreateCloudFormationChangeSetResponseTypeDef",
+    "CreateCloudFormationTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetApplicationPolicyResponseTypeDef",
+    "GetCloudFormationTemplateResponseTypeDef",
+    "ListApplicationDependenciesResponseTypeDef",
     "ListApplicationsResponseTypeDef",
+    "PutApplicationPolicyResponseTypeDef",
     "CreateApplicationVersionResponseTypeDef",
     "VersionTypeDef",
+    "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "RollbackConfigurationTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "CreateCloudFormationChangeSetRequestRequestTypeDef",
 )
@@ -70,35 +72,61 @@
     "ApplicationDependencySummaryTypeDef",
     {
         "ApplicationId": str,
         "SemanticVersion": str,
     },
 )
 
-_RequiredApplicationPolicyStatementTypeDef = TypedDict(
-    "_RequiredApplicationPolicyStatementTypeDef",
+_RequiredApplicationPolicyStatementOutputTypeDef = TypedDict(
+    "_RequiredApplicationPolicyStatementOutputTypeDef",
     {
         "Actions": List[str],
         "Principals": List[str],
     },
 )
+_OptionalApplicationPolicyStatementOutputTypeDef = TypedDict(
+    "_OptionalApplicationPolicyStatementOutputTypeDef",
+    {
+        "PrincipalOrgIDs": List[str],
+        "StatementId": str,
+    },
+    total=False,
+)
+
+
+class ApplicationPolicyStatementOutputTypeDef(
+    _RequiredApplicationPolicyStatementOutputTypeDef,
+    _OptionalApplicationPolicyStatementOutputTypeDef,
+):
+    pass
+
+
+_RequiredApplicationPolicyStatementTypeDef = TypedDict(
+    "_RequiredApplicationPolicyStatementTypeDef",
+    {
+        "Actions": Sequence[str],
+        "Principals": Sequence[str],
+    },
+)
 _OptionalApplicationPolicyStatementTypeDef = TypedDict(
     "_OptionalApplicationPolicyStatementTypeDef",
     {
-        "PrincipalOrgIDs": List[str],
+        "PrincipalOrgIDs": Sequence[str],
         "StatementId": str,
     },
     total=False,
 )
 
+
 class ApplicationPolicyStatementTypeDef(
     _RequiredApplicationPolicyStatementTypeDef, _OptionalApplicationPolicyStatementTypeDef
 ):
     pass
 
+
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
         "ApplicationId": str,
         "Author": str,
         "Description": str,
         "Name": str,
@@ -111,19 +139,21 @@
         "HomePageUrl": str,
         "Labels": List[str],
         "SpdxLicenseId": str,
     },
     total=False,
 )
 
+
 class ApplicationSummaryTypeDef(
     _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
 ):
     pass
 
+
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "Author": str,
         "Description": str,
         "Name": str,
     },
@@ -143,19 +173,32 @@
         "SpdxLicenseId": str,
         "TemplateBody": str,
         "TemplateUrl": str,
     },
     total=False,
 )
 
+
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredCreateApplicationVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationVersionRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "SemanticVersion": str,
     },
 )
@@ -166,20 +209,22 @@
         "SourceCodeUrl": str,
         "TemplateBody": str,
         "TemplateUrl": str,
     },
     total=False,
 )
 
+
 class CreateApplicationVersionRequestRequestTypeDef(
     _RequiredCreateApplicationVersionRequestRequestTypeDef,
     _OptionalCreateApplicationVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredParameterDefinitionTypeDef = TypedDict(
     "_RequiredParameterDefinitionTypeDef",
     {
         "Name": str,
         "ReferencedByResources": List[str],
     },
 )
@@ -197,19 +242,21 @@
         "MinValue": int,
         "NoEcho": bool,
         "Type": str,
     },
     total=False,
 )
 
+
 class ParameterDefinitionTypeDef(
     _RequiredParameterDefinitionTypeDef, _OptionalParameterDefinitionTypeDef
 ):
     pass
 
+
 ParameterValueTypeDef = TypedDict(
     "ParameterValueTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -218,73 +265,43 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
-    "CreateCloudFormationChangeSetResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "ChangeSetId": str,
-        "SemanticVersion": str,
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCloudFormationTemplateRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalCreateCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCloudFormationTemplateRequestRequestTypeDef",
     {
         "SemanticVersion": str,
     },
     total=False,
 )
 
+
 class CreateCloudFormationTemplateRequestRequestTypeDef(
     _RequiredCreateCloudFormationTemplateRequestRequestTypeDef,
     _OptionalCreateCloudFormationTemplateRequestRequestTypeDef,
 ):
     pass
 
-CreateCloudFormationTemplateResponseTypeDef = TypedDict(
-    "CreateCloudFormationTemplateResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "CreationTime": str,
-        "ExpirationTime": str,
-        "SemanticVersion": str,
-        "Status": StatusType,
-        "TemplateId": str,
-        "TemplateUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApplicationPolicyRequestRequestTypeDef = TypedDict(
     "GetApplicationPolicyRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -298,62 +315,39 @@
     "_OptionalGetApplicationRequestRequestTypeDef",
     {
         "SemanticVersion": str,
     },
     total=False,
 )
 
+
 class GetApplicationRequestRequestTypeDef(
     _RequiredGetApplicationRequestRequestTypeDef, _OptionalGetApplicationRequestRequestTypeDef
 ):
     pass
 
+
 GetCloudFormationTemplateRequestRequestTypeDef = TypedDict(
     "GetCloudFormationTemplateRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "TemplateId": str,
     },
 )
 
-GetCloudFormationTemplateResponseTypeDef = TypedDict(
-    "GetCloudFormationTemplateResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "CreationTime": str,
-        "ExpirationTime": str,
-        "SemanticVersion": str,
-        "Status": StatusType,
-        "TemplateId": str,
-        "TemplateUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "SemanticVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(
-    _RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-    _OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListApplicationDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationDependenciesRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 _OptionalListApplicationDependenciesRequestRequestTypeDef = TypedDict(
@@ -362,39 +356,21 @@
         "MaxItems": int,
         "NextToken": str,
         "SemanticVersion": str,
     },
     total=False,
 )
 
+
 class ListApplicationDependenciesRequestRequestTypeDef(
     _RequiredListApplicationDependenciesRequestRequestTypeDef,
     _OptionalListApplicationDependenciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "ApplicationId": str,
-    },
-)
-_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
-    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-):
-    pass
 
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
@@ -403,20 +379,22 @@
     {
         "MaxItems": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredVersionSummaryTypeDef = TypedDict(
     "_RequiredVersionSummaryTypeDef",
     {
         "ApplicationId": str,
         "CreationTime": str,
         "SemanticVersion": str,
     },
@@ -425,55 +403,28 @@
     "_OptionalVersionSummaryTypeDef",
     {
         "SourceCodeUrl": str,
     },
     total=False,
 )
 
+
 class VersionSummaryTypeDef(_RequiredVersionSummaryTypeDef, _OptionalVersionSummaryTypeDef):
     pass
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "MaxItems": int,
         "NextToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
         "Type": str,
     },
 )
@@ -501,58 +452,106 @@
         "Labels": Sequence[str],
         "ReadmeBody": str,
         "ReadmeUrl": str,
     },
     total=False,
 )
 
+
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-ListApplicationDependenciesResponseTypeDef = TypedDict(
-    "ListApplicationDependenciesResponseTypeDef",
+
+PutApplicationPolicyRequestRequestTypeDef = TypedDict(
+    "PutApplicationPolicyRequestRequestTypeDef",
     {
-        "Dependencies": List[ApplicationDependencySummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationId": str,
+        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
+    },
+)
+
+CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
+    "CreateCloudFormationChangeSetResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "ChangeSetId": str,
+        "SemanticVersion": str,
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCloudFormationTemplateResponseTypeDef = TypedDict(
+    "CreateCloudFormationTemplateResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "CreationTime": str,
+        "ExpirationTime": str,
+        "SemanticVersion": str,
+        "Status": StatusType,
+        "TemplateId": str,
+        "TemplateUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationPolicyResponseTypeDef = TypedDict(
     "GetApplicationPolicyResponseTypeDef",
     {
-        "Statements": List[ApplicationPolicyStatementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Statements": List[ApplicationPolicyStatementOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutApplicationPolicyRequestRequestTypeDef = TypedDict(
-    "PutApplicationPolicyRequestRequestTypeDef",
+GetCloudFormationTemplateResponseTypeDef = TypedDict(
+    "GetCloudFormationTemplateResponseTypeDef",
     {
         "ApplicationId": str,
-        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
+        "CreationTime": str,
+        "ExpirationTime": str,
+        "SemanticVersion": str,
+        "Status": StatusType,
+        "TemplateId": str,
+        "TemplateUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutApplicationPolicyResponseTypeDef = TypedDict(
-    "PutApplicationPolicyResponseTypeDef",
+ListApplicationDependenciesResponseTypeDef = TypedDict(
+    "ListApplicationDependenciesResponseTypeDef",
     {
-        "Statements": List[ApplicationPolicyStatementTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Dependencies": List[ApplicationDependencySummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "Applications": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutApplicationPolicyResponseTypeDef = TypedDict(
+    "PutApplicationPolicyResponseTypeDef",
+    {
+        "Statements": List[ApplicationPolicyStatementOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApplicationVersionResponseTypeDef = TypedDict(
     "CreateApplicationVersionResponseTypeDef",
     {
         "ApplicationId": str,
@@ -560,15 +559,15 @@
         "ParameterDefinitions": List[ParameterDefinitionTypeDef],
         "RequiredCapabilities": List[CapabilityType],
         "ResourcesSupported": bool,
         "SemanticVersion": str,
         "SourceCodeArchiveUrl": str,
         "SourceCodeUrl": str,
         "TemplateUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredVersionTypeDef = TypedDict(
     "_RequiredVersionTypeDef",
     {
         "ApplicationId": str,
@@ -585,23 +584,78 @@
     {
         "SourceCodeArchiveUrl": str,
         "SourceCodeUrl": str,
     },
     total=False,
 )
 
+
 class VersionTypeDef(_RequiredVersionTypeDef, _OptionalVersionTypeDef):
     pass
 
+
+_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
+    {
+        "SemanticVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef(
+    _RequiredListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    _OptionalListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "ApplicationId": str,
+    },
+)
+_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
+    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListApplicationVersionsResponseTypeDef = TypedDict(
     "ListApplicationVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Versions": List[VersionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
         "MonitoringTimeInMinutes": int,
@@ -622,15 +676,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "ApplicationId": str,
@@ -642,15 +696,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "ApplicationId": str,
@@ -662,15 +716,15 @@
         "Labels": List[str],
         "LicenseUrl": str,
         "Name": str,
         "ReadmeUrl": str,
         "SpdxLicenseId": str,
         "VerifiedAuthorUrl": str,
         "Version": VersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCloudFormationChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCloudFormationChangeSetRequestRequestTypeDef",
     {
         "ApplicationId": str,
@@ -691,12 +745,13 @@
         "SemanticVersion": str,
         "Tags": Sequence[TagTypeDef],
         "TemplateId": str,
     },
     total=False,
 )
 
+
 class CreateCloudFormationChangeSetRequestRequestTypeDef(
     _RequiredCreateCloudFormationChangeSetRequestRequestTypeDef,
     _OptionalCreateCloudFormationChangeSetRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo.egg-info/PKG-INFO` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-serverlessrepo
-Version: 1.28.0
-Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ServerlessApplicationRepository 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-serverlessrepo"></a>
 
 # mypy-boto3-serverlessrepo
 
 [![PyPI - mypy-boto3-serverlessrepo](https://img.shields.io/pypi/v/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-serverlessrepo.svg?color=blue)](https://pypi.org/project/mypy-boto3-serverlessrepo)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-serverlessrepo?color=blue)](https://pypistats.org/packages/mypy-boto3-serverlessrepo)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-serverlessrepo)](https://pepy.tech/project/mypy-boto3-serverlessrepo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServerlessApplicationRepository 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
+[boto3.ServerlessApplicationRepository 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
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
 [mypy-boto3-serverlessrepo docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,49 +335,50 @@
 
 `mypy_boto3_serverlessrepo.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_serverlessrepo.type_defs import (
     ApplicationDependencySummaryTypeDef,
+    ApplicationPolicyStatementOutputTypeDef,
     ApplicationPolicyStatementTypeDef,
     ApplicationSummaryTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateApplicationVersionRequestRequestTypeDef,
     ParameterDefinitionTypeDef,
     ParameterValueTypeDef,
     TagTypeDef,
-    CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateRequestRequestTypeDef,
-    CreateCloudFormationTemplateResponseTypeDef,
     DeleteApplicationRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationPolicyRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetCloudFormationTemplateRequestRequestTypeDef,
-    GetCloudFormationTemplateResponseTypeDef,
-    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationDependenciesRequestRequestTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
     VersionSummaryTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RollbackTriggerTypeDef,
     UnshareApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    ListApplicationDependenciesResponseTypeDef,
-    GetApplicationPolicyResponseTypeDef,
     PutApplicationPolicyRequestRequestTypeDef,
-    PutApplicationPolicyResponseTypeDef,
+    CreateCloudFormationChangeSetResponseTypeDef,
+    CreateCloudFormationTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetApplicationPolicyResponseTypeDef,
+    GetCloudFormationTemplateResponseTypeDef,
+    ListApplicationDependenciesResponseTypeDef,
     ListApplicationsResponseTypeDef,
+    PutApplicationPolicyResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     VersionTypeDef,
+    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationVersionsResponseTypeDef,
     RollbackConfigurationTypeDef,
     CreateApplicationResponseTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     CreateCloudFormationChangeSetRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-serverlessrepo-1.28.0/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt` & `mypy-boto3-serverlessrepo-1.28.12/mypy_boto3_serverlessrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-serverlessrepo-1.28.0/setup.py` & `mypy-boto3-serverlessrepo-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-serverlessrepo",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_serverlessrepo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServerlessApplicationRepository 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ServerlessApplicationRepository 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

