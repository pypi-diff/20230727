# Comparing `tmp/mypy-boto3-amplify-1.28.0.tar.gz` & `tmp/mypy-boto3-amplify-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplify-1.28.0.tar", last modified: Thu Jul  6 20:58:51 2023, max compression
+gzip compressed data, was "mypy-boto3-amplify-1.28.12.tar", last modified: Thu Jul 27 05:34:13 2023, max compression
```

## Comparing `mypy-boto3-amplify-1.28.0.tar` & `mypy-boto3-amplify-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.650206 mypy-boto3-amplify-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:32:42.000000 mypy-boto3-amplify-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-06 20:58:51.650206 mypy-boto3-amplify-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14837 2023-07-06 20:32:42.000000 mypy-boto3-amplify-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.630206 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-06 20:32:42.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-06 20:32:42.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:32:42.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27948 2023-07-06 20:32:42.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27900 2023-07-06 20:32:42.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-07-06 20:32:43.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-07-06 20:32:43.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-06 20:32:42.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-06 20:32:42.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:42.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35266 2023-07-06 20:32:44.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35207 2023-07-06 20:32:43.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:32:42.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.630206 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-06 20:58:51.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 20:58:51.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:51.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:51.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:51.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:58:51.000000 mypy-boto3-amplify-1.28.0/mypy_boto3_amplify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:51.650206 mypy-boto3-amplify-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:32:42.000000 mypy-boto3-amplify-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.844594 mypy-boto3-amplify-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16422 2023-07-27 05:34:13.844594 mypy-boto3-amplify-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.840594 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27948 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27900 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36465 2023-07-27 05:17:01.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36404 2023-07-27 05:17:01.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.844594 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16422 2023-07-27 05:34:13.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 05:34:13.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:13.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:13.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:13.844594 mypy-boto3-amplify-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/setup.py
```

### Comparing `mypy-boto3-amplify-1.28.0/LICENSE` & `mypy-boto3-amplify-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.0/PKG-INFO` & `mypy-boto3-amplify-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplify
-Version: 1.28.0
-Summary: Type annotations for boto3.Amplify 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Amplify 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-amplify"></a>
 
 # mypy-boto3-amplify
 
 [![PyPI - mypy-boto3-amplify](https://img.shields.io/pypi/v/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplify?color=blue)](https://pypistats.org/packages/mypy-boto3-amplify)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplify)](https://pepy.tech/project/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,20 +337,22 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplify.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplify.type_defs import (
-    AutoBranchCreationConfigTypeDef,
-    CustomRuleTypeDef,
+    AutoBranchCreationConfigOutputTypeDef,
+    CustomRuleOutputTypeDef,
     ProductionBranchTypeDef,
     ArtifactTypeDef,
+    AutoBranchCreationConfigTypeDef,
     BackendEnvironmentTypeDef,
     BranchTypeDef,
+    CustomRuleTypeDef,
     ResponseMetadataTypeDef,
     CreateBackendEnvironmentRequestRequestTypeDef,
     CreateBranchRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     SubDomainSettingTypeDef,
     CreateWebhookRequestRequestTypeDef,
     WebhookTypeDef,
@@ -378,21 +380,22 @@
     ListDomainAssociationsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebhooksRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StartJobRequestRequestTypeDef,
     StopJobRequestRequestTypeDef,
+    SubDomainSettingOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBranchRequestRequestTypeDef,
     UpdateWebhookRequestRequestTypeDef,
+    AppTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
-    AppTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     DeleteBackendEnvironmentResultTypeDef,
     DeleteBranchResultTypeDef,
     GenerateAccessLogsResultTypeDef,
     GetArtifactUrlResultTypeDef,
@@ -400,15 +403,14 @@
     GetBranchResultTypeDef,
     ListArtifactsResultTypeDef,
     ListBackendEnvironmentsResultTypeDef,
     ListBranchesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateBranchResultTypeDef,
     CreateDomainAssociationRequestRequestTypeDef,
-    SubDomainTypeDef,
     UpdateDomainAssociationRequestRequestTypeDef,
     CreateWebhookResultTypeDef,
     DeleteWebhookResultTypeDef,
     GetWebhookResultTypeDef,
     ListWebhooksResultTypeDef,
     UpdateWebhookResultTypeDef,
     DeleteJobResultTypeDef,
@@ -417,30 +419,31 @@
     StartJobResultTypeDef,
     StopJobResultTypeDef,
     JobTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     ListBranchesRequestListBranchesPaginateTypeDef,
     ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
+    SubDomainTypeDef,
     CreateAppResultTypeDef,
     DeleteAppResultTypeDef,
     GetAppResultTypeDef,
     ListAppsResultTypeDef,
     UpdateAppResultTypeDef,
-    DomainAssociationTypeDef,
     GetJobResultTypeDef,
+    DomainAssociationTypeDef,
     CreateDomainAssociationResultTypeDef,
     DeleteDomainAssociationResultTypeDef,
     GetDomainAssociationResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
 )
 
 
-def get_structure() -> AutoBranchCreationConfigTypeDef:
+def get_structure() -> AutoBranchCreationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplify-1.28.0/README.md` & `mypy-boto3-amplify-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-amplify"></a>
 
 # mypy-boto3-amplify
 
 [![PyPI - mypy-boto3-amplify](https://img.shields.io/pypi/v/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplify?color=blue)](https://pypistats.org/packages/mypy-boto3-amplify)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplify)](https://pepy.tech/project/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,20 +305,22 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplify.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplify.type_defs import (
-    AutoBranchCreationConfigTypeDef,
-    CustomRuleTypeDef,
+    AutoBranchCreationConfigOutputTypeDef,
+    CustomRuleOutputTypeDef,
     ProductionBranchTypeDef,
     ArtifactTypeDef,
+    AutoBranchCreationConfigTypeDef,
     BackendEnvironmentTypeDef,
     BranchTypeDef,
+    CustomRuleTypeDef,
     ResponseMetadataTypeDef,
     CreateBackendEnvironmentRequestRequestTypeDef,
     CreateBranchRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     SubDomainSettingTypeDef,
     CreateWebhookRequestRequestTypeDef,
     WebhookTypeDef,
@@ -346,21 +348,22 @@
     ListDomainAssociationsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebhooksRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StartJobRequestRequestTypeDef,
     StopJobRequestRequestTypeDef,
+    SubDomainSettingOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBranchRequestRequestTypeDef,
     UpdateWebhookRequestRequestTypeDef,
+    AppTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
-    AppTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     DeleteBackendEnvironmentResultTypeDef,
     DeleteBranchResultTypeDef,
     GenerateAccessLogsResultTypeDef,
     GetArtifactUrlResultTypeDef,
@@ -368,15 +371,14 @@
     GetBranchResultTypeDef,
     ListArtifactsResultTypeDef,
     ListBackendEnvironmentsResultTypeDef,
     ListBranchesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateBranchResultTypeDef,
     CreateDomainAssociationRequestRequestTypeDef,
-    SubDomainTypeDef,
     UpdateDomainAssociationRequestRequestTypeDef,
     CreateWebhookResultTypeDef,
     DeleteWebhookResultTypeDef,
     GetWebhookResultTypeDef,
     ListWebhooksResultTypeDef,
     UpdateWebhookResultTypeDef,
     DeleteJobResultTypeDef,
@@ -385,30 +387,31 @@
     StartJobResultTypeDef,
     StopJobResultTypeDef,
     JobTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     ListBranchesRequestListBranchesPaginateTypeDef,
     ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
+    SubDomainTypeDef,
     CreateAppResultTypeDef,
     DeleteAppResultTypeDef,
     GetAppResultTypeDef,
     ListAppsResultTypeDef,
     UpdateAppResultTypeDef,
-    DomainAssociationTypeDef,
     GetJobResultTypeDef,
+    DomainAssociationTypeDef,
     CreateDomainAssociationResultTypeDef,
     DeleteDomainAssociationResultTypeDef,
     GetDomainAssociationResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
 )
 
 
-def get_structure() -> AutoBranchCreationConfigTypeDef:
+def get_structure() -> AutoBranchCreationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/__init__.py` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/__init__.pyi` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/__main__.py` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Amplify 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Amplify 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify\nOther"
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

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/client.py` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/client.pyi` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/literals.py` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DomainStatusType",
     "JobStatusType",
     "JobTypeType",
     "ListAppsPaginatorName",
     "ListBranchesPaginatorName",
     "ListDomainAssociationsPaginatorName",
@@ -33,15 +32,14 @@
     "AmplifyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DomainStatusType = Literal[
     "AVAILABLE",
     "CREATING",
     "FAILED",
     "IN_PROGRESS",
     "PENDING_DEPLOYMENT",
     "PENDING_VERIFICATION",
@@ -175,14 +173,15 @@
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
@@ -261,26 +260,28 @@
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

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/literals.pyi` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/literals.py`

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
     "DomainStatusType",
     "JobStatusType",
     "JobTypeType",
     "ListAppsPaginatorName",
     "ListBranchesPaginatorName",
     "ListDomainAssociationsPaginatorName",
@@ -32,14 +33,15 @@
     "AmplifyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DomainStatusType = Literal[
     "AVAILABLE",
     "CREATING",
     "FAILED",
     "IN_PROGRESS",
     "PENDING_DEPLOYMENT",
     "PENDING_VERIFICATION",
@@ -173,14 +175,15 @@
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
@@ -259,26 +262,28 @@
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

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/paginator.py` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/paginator.pyi` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/type_defs.py` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplify service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigTypeDef
+    from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
 
-    data: AutoBranchCreationConfigTypeDef = {...}
+    data: AutoBranchCreationConfigOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -27,20 +27,22 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AutoBranchCreationConfigTypeDef",
-    "CustomRuleTypeDef",
+    "AutoBranchCreationConfigOutputTypeDef",
+    "CustomRuleOutputTypeDef",
     "ProductionBranchTypeDef",
     "ArtifactTypeDef",
+    "AutoBranchCreationConfigTypeDef",
     "BackendEnvironmentTypeDef",
     "BranchTypeDef",
+    "CustomRuleTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackendEnvironmentRequestRequestTypeDef",
     "CreateBranchRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "SubDomainSettingTypeDef",
     "CreateWebhookRequestRequestTypeDef",
     "WebhookTypeDef",
@@ -68,21 +70,22 @@
     "ListDomainAssociationsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebhooksRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StartJobRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
+    "SubDomainSettingOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBranchRequestRequestTypeDef",
     "UpdateWebhookRequestRequestTypeDef",
+    "AppTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
-    "AppTypeDef",
     "CreateBackendEnvironmentResultTypeDef",
     "CreateBranchResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "DeleteBackendEnvironmentResultTypeDef",
     "DeleteBranchResultTypeDef",
     "GenerateAccessLogsResultTypeDef",
     "GetArtifactUrlResultTypeDef",
@@ -90,15 +93,14 @@
     "GetBranchResultTypeDef",
     "ListArtifactsResultTypeDef",
     "ListBackendEnvironmentsResultTypeDef",
     "ListBranchesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateBranchResultTypeDef",
     "CreateDomainAssociationRequestRequestTypeDef",
-    "SubDomainTypeDef",
     "UpdateDomainAssociationRequestRequestTypeDef",
     "CreateWebhookResultTypeDef",
     "DeleteWebhookResultTypeDef",
     "GetWebhookResultTypeDef",
     "ListWebhooksResultTypeDef",
     "UpdateWebhookResultTypeDef",
     "DeleteJobResultTypeDef",
@@ -107,63 +109,64 @@
     "StartJobResultTypeDef",
     "StopJobResultTypeDef",
     "JobTypeDef",
     "ListAppsRequestListAppsPaginateTypeDef",
     "ListBranchesRequestListBranchesPaginateTypeDef",
     "ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
+    "SubDomainTypeDef",
     "CreateAppResultTypeDef",
     "DeleteAppResultTypeDef",
     "GetAppResultTypeDef",
     "ListAppsResultTypeDef",
     "UpdateAppResultTypeDef",
-    "DomainAssociationTypeDef",
     "GetJobResultTypeDef",
+    "DomainAssociationTypeDef",
     "CreateDomainAssociationResultTypeDef",
     "DeleteDomainAssociationResultTypeDef",
     "GetDomainAssociationResultTypeDef",
     "ListDomainAssociationsResultTypeDef",
     "UpdateDomainAssociationResultTypeDef",
 )
 
-AutoBranchCreationConfigTypeDef = TypedDict(
-    "AutoBranchCreationConfigTypeDef",
+AutoBranchCreationConfigOutputTypeDef = TypedDict(
+    "AutoBranchCreationConfigOutputTypeDef",
     {
         "stage": StageType,
         "framework": str,
         "enableAutoBuild": bool,
-        "environmentVariables": Mapping[str, str],
+        "environmentVariables": Dict[str, str],
         "basicAuthCredentials": str,
         "enableBasicAuth": bool,
         "enablePerformanceMode": bool,
         "buildSpec": str,
         "enablePullRequestPreview": bool,
         "pullRequestEnvironmentName": str,
     },
     total=False,
 )
 
-_RequiredCustomRuleTypeDef = TypedDict(
-    "_RequiredCustomRuleTypeDef",
+_RequiredCustomRuleOutputTypeDef = TypedDict(
+    "_RequiredCustomRuleOutputTypeDef",
     {
         "source": str,
         "target": str,
     },
 )
-_OptionalCustomRuleTypeDef = TypedDict(
-    "_OptionalCustomRuleTypeDef",
+_OptionalCustomRuleOutputTypeDef = TypedDict(
+    "_OptionalCustomRuleOutputTypeDef",
     {
         "status": str,
         "condition": str,
     },
     total=False,
 )
 
 
-class CustomRuleTypeDef(_RequiredCustomRuleTypeDef, _OptionalCustomRuleTypeDef):
+class CustomRuleOutputTypeDef(_RequiredCustomRuleOutputTypeDef, _OptionalCustomRuleOutputTypeDef):
     pass
 
 
 ProductionBranchTypeDef = TypedDict(
     "ProductionBranchTypeDef",
     {
         "lastDeployTime": datetime,
@@ -178,14 +181,31 @@
     "ArtifactTypeDef",
     {
         "artifactFileName": str,
         "artifactId": str,
     },
 )
 
+AutoBranchCreationConfigTypeDef = TypedDict(
+    "AutoBranchCreationConfigTypeDef",
+    {
+        "stage": StageType,
+        "framework": str,
+        "enableAutoBuild": bool,
+        "environmentVariables": Mapping[str, str],
+        "basicAuthCredentials": str,
+        "enableBasicAuth": bool,
+        "enablePerformanceMode": bool,
+        "buildSpec": str,
+        "enablePullRequestPreview": bool,
+        "pullRequestEnvironmentName": str,
+    },
+    total=False,
+)
+
 _RequiredBackendEnvironmentTypeDef = TypedDict(
     "_RequiredBackendEnvironmentTypeDef",
     {
         "backendEnvironmentArn": str,
         "environmentName": str,
         "createTime": datetime,
         "updateTime": datetime,
@@ -247,14 +267,35 @@
 )
 
 
 class BranchTypeDef(_RequiredBranchTypeDef, _OptionalBranchTypeDef):
     pass
 
 
+_RequiredCustomRuleTypeDef = TypedDict(
+    "_RequiredCustomRuleTypeDef",
+    {
+        "source": str,
+        "target": str,
+    },
+)
+_OptionalCustomRuleTypeDef = TypedDict(
+    "_OptionalCustomRuleTypeDef",
+    {
+        "status": str,
+        "condition": str,
+    },
+    total=False,
+)
+
+
+class CustomRuleTypeDef(_RequiredCustomRuleTypeDef, _OptionalCustomRuleTypeDef):
+    pass
+
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -786,14 +827,22 @@
     {
         "appId": str,
         "branchName": str,
         "jobId": str,
     },
 )
 
+SubDomainSettingOutputTypeDef = TypedDict(
+    "SubDomainSettingOutputTypeDef",
+    {
+        "prefix": str,
+        "branchName": str,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -860,14 +909,55 @@
 
 class UpdateWebhookRequestRequestTypeDef(
     _RequiredUpdateWebhookRequestRequestTypeDef, _OptionalUpdateWebhookRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredAppTypeDef = TypedDict(
+    "_RequiredAppTypeDef",
+    {
+        "appId": str,
+        "appArn": str,
+        "name": str,
+        "description": str,
+        "repository": str,
+        "platform": PlatformType,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "environmentVariables": Dict[str, str],
+        "defaultDomain": str,
+        "enableBranchAutoBuild": bool,
+        "enableBasicAuth": bool,
+    },
+)
+_OptionalAppTypeDef = TypedDict(
+    "_OptionalAppTypeDef",
+    {
+        "tags": Dict[str, str],
+        "iamServiceRoleArn": str,
+        "enableBranchAutoDeletion": bool,
+        "basicAuthCredentials": str,
+        "customRules": List[CustomRuleOutputTypeDef],
+        "productionBranch": ProductionBranchTypeDef,
+        "buildSpec": str,
+        "customHeaders": str,
+        "enableAutoBranchCreation": bool,
+        "autoBranchCreationPatterns": List[str],
+        "autoBranchCreationConfig": AutoBranchCreationConfigOutputTypeDef,
+        "repositoryCloneMethod": RepositoryCloneMethodType,
+    },
+    total=False,
+)
+
+
+class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+    pass
+
+
 _RequiredCreateAppRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAppRequestRequestTypeDef = TypedDict(
@@ -936,55 +1026,14 @@
 
 class UpdateAppRequestRequestTypeDef(
     _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredAppTypeDef = TypedDict(
-    "_RequiredAppTypeDef",
-    {
-        "appId": str,
-        "appArn": str,
-        "name": str,
-        "description": str,
-        "repository": str,
-        "platform": PlatformType,
-        "createTime": datetime,
-        "updateTime": datetime,
-        "environmentVariables": Dict[str, str],
-        "defaultDomain": str,
-        "enableBranchAutoBuild": bool,
-        "enableBasicAuth": bool,
-    },
-)
-_OptionalAppTypeDef = TypedDict(
-    "_OptionalAppTypeDef",
-    {
-        "tags": Dict[str, str],
-        "iamServiceRoleArn": str,
-        "enableBranchAutoDeletion": bool,
-        "basicAuthCredentials": str,
-        "customRules": List[CustomRuleTypeDef],
-        "productionBranch": ProductionBranchTypeDef,
-        "buildSpec": str,
-        "customHeaders": str,
-        "enableAutoBranchCreation": bool,
-        "autoBranchCreationPatterns": List[str],
-        "autoBranchCreationConfig": AutoBranchCreationConfigTypeDef,
-        "repositoryCloneMethod": RepositoryCloneMethodType,
-    },
-    total=False,
-)
-
-
-class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
-    pass
-
-
 CreateBackendEnvironmentResultTypeDef = TypedDict(
     "CreateBackendEnvironmentResultTypeDef",
     {
         "backendEnvironment": BackendEnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1121,23 +1170,14 @@
 class CreateDomainAssociationRequestRequestTypeDef(
     _RequiredCreateDomainAssociationRequestRequestTypeDef,
     _OptionalCreateDomainAssociationRequestRequestTypeDef,
 ):
     pass
 
 
-SubDomainTypeDef = TypedDict(
-    "SubDomainTypeDef",
-    {
-        "subDomainSetting": SubDomainSettingTypeDef,
-        "verified": bool,
-        "dnsRecord": str,
-    },
-)
-
 _RequiredUpdateDomainAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainAssociationRequestRequestTypeDef",
     {
         "appId": str,
         "domainName": str,
     },
 )
@@ -1320,14 +1360,23 @@
 
 class ListJobsRequestListJobsPaginateTypeDef(
     _RequiredListJobsRequestListJobsPaginateTypeDef, _OptionalListJobsRequestListJobsPaginateTypeDef
 ):
     pass
 
 
+SubDomainTypeDef = TypedDict(
+    "SubDomainTypeDef",
+    {
+        "subDomainSetting": SubDomainSettingOutputTypeDef,
+        "verified": bool,
+        "dnsRecord": str,
+    },
+)
+
 CreateAppResultTypeDef = TypedDict(
     "CreateAppResultTypeDef",
     {
         "app": AppTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1361,14 +1410,22 @@
     "UpdateAppResultTypeDef",
     {
         "app": AppTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetJobResultTypeDef = TypedDict(
+    "GetJobResultTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDomainAssociationTypeDef = TypedDict(
     "_RequiredDomainAssociationTypeDef",
     {
         "domainAssociationArn": str,
         "domainName": str,
         "enableAutoSubDomain": bool,
         "domainStatus": DomainStatusType,
@@ -1389,22 +1446,14 @@
 
 class DomainAssociationTypeDef(
     _RequiredDomainAssociationTypeDef, _OptionalDomainAssociationTypeDef
 ):
     pass
 
 
-GetJobResultTypeDef = TypedDict(
-    "GetJobResultTypeDef",
-    {
-        "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateDomainAssociationResultTypeDef = TypedDict(
     "CreateDomainAssociationResultTypeDef",
     {
         "domainAssociation": DomainAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify/type_defs.pyi` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplify service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigTypeDef
+    from mypy_boto3_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
 
-    data: AutoBranchCreationConfigTypeDef = {...}
+    data: AutoBranchCreationConfigOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -26,20 +26,22 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AutoBranchCreationConfigTypeDef",
-    "CustomRuleTypeDef",
+    "AutoBranchCreationConfigOutputTypeDef",
+    "CustomRuleOutputTypeDef",
     "ProductionBranchTypeDef",
     "ArtifactTypeDef",
+    "AutoBranchCreationConfigTypeDef",
     "BackendEnvironmentTypeDef",
     "BranchTypeDef",
+    "CustomRuleTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackendEnvironmentRequestRequestTypeDef",
     "CreateBranchRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "SubDomainSettingTypeDef",
     "CreateWebhookRequestRequestTypeDef",
     "WebhookTypeDef",
@@ -67,21 +69,22 @@
     "ListDomainAssociationsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebhooksRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StartJobRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
+    "SubDomainSettingOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBranchRequestRequestTypeDef",
     "UpdateWebhookRequestRequestTypeDef",
+    "AppTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
-    "AppTypeDef",
     "CreateBackendEnvironmentResultTypeDef",
     "CreateBranchResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "DeleteBackendEnvironmentResultTypeDef",
     "DeleteBranchResultTypeDef",
     "GenerateAccessLogsResultTypeDef",
     "GetArtifactUrlResultTypeDef",
@@ -89,15 +92,14 @@
     "GetBranchResultTypeDef",
     "ListArtifactsResultTypeDef",
     "ListBackendEnvironmentsResultTypeDef",
     "ListBranchesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateBranchResultTypeDef",
     "CreateDomainAssociationRequestRequestTypeDef",
-    "SubDomainTypeDef",
     "UpdateDomainAssociationRequestRequestTypeDef",
     "CreateWebhookResultTypeDef",
     "DeleteWebhookResultTypeDef",
     "GetWebhookResultTypeDef",
     "ListWebhooksResultTypeDef",
     "UpdateWebhookResultTypeDef",
     "DeleteJobResultTypeDef",
@@ -106,62 +108,63 @@
     "StartJobResultTypeDef",
     "StopJobResultTypeDef",
     "JobTypeDef",
     "ListAppsRequestListAppsPaginateTypeDef",
     "ListBranchesRequestListBranchesPaginateTypeDef",
     "ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
+    "SubDomainTypeDef",
     "CreateAppResultTypeDef",
     "DeleteAppResultTypeDef",
     "GetAppResultTypeDef",
     "ListAppsResultTypeDef",
     "UpdateAppResultTypeDef",
-    "DomainAssociationTypeDef",
     "GetJobResultTypeDef",
+    "DomainAssociationTypeDef",
     "CreateDomainAssociationResultTypeDef",
     "DeleteDomainAssociationResultTypeDef",
     "GetDomainAssociationResultTypeDef",
     "ListDomainAssociationsResultTypeDef",
     "UpdateDomainAssociationResultTypeDef",
 )
 
-AutoBranchCreationConfigTypeDef = TypedDict(
-    "AutoBranchCreationConfigTypeDef",
+AutoBranchCreationConfigOutputTypeDef = TypedDict(
+    "AutoBranchCreationConfigOutputTypeDef",
     {
         "stage": StageType,
         "framework": str,
         "enableAutoBuild": bool,
-        "environmentVariables": Mapping[str, str],
+        "environmentVariables": Dict[str, str],
         "basicAuthCredentials": str,
         "enableBasicAuth": bool,
         "enablePerformanceMode": bool,
         "buildSpec": str,
         "enablePullRequestPreview": bool,
         "pullRequestEnvironmentName": str,
     },
     total=False,
 )
 
-_RequiredCustomRuleTypeDef = TypedDict(
-    "_RequiredCustomRuleTypeDef",
+_RequiredCustomRuleOutputTypeDef = TypedDict(
+    "_RequiredCustomRuleOutputTypeDef",
     {
         "source": str,
         "target": str,
     },
 )
-_OptionalCustomRuleTypeDef = TypedDict(
-    "_OptionalCustomRuleTypeDef",
+_OptionalCustomRuleOutputTypeDef = TypedDict(
+    "_OptionalCustomRuleOutputTypeDef",
     {
         "status": str,
         "condition": str,
     },
     total=False,
 )
 
-class CustomRuleTypeDef(_RequiredCustomRuleTypeDef, _OptionalCustomRuleTypeDef):
+class CustomRuleOutputTypeDef(_RequiredCustomRuleOutputTypeDef, _OptionalCustomRuleOutputTypeDef):
     pass
 
 ProductionBranchTypeDef = TypedDict(
     "ProductionBranchTypeDef",
     {
         "lastDeployTime": datetime,
         "status": str,
@@ -175,14 +178,31 @@
     "ArtifactTypeDef",
     {
         "artifactFileName": str,
         "artifactId": str,
     },
 )
 
+AutoBranchCreationConfigTypeDef = TypedDict(
+    "AutoBranchCreationConfigTypeDef",
+    {
+        "stage": StageType,
+        "framework": str,
+        "enableAutoBuild": bool,
+        "environmentVariables": Mapping[str, str],
+        "basicAuthCredentials": str,
+        "enableBasicAuth": bool,
+        "enablePerformanceMode": bool,
+        "buildSpec": str,
+        "enablePullRequestPreview": bool,
+        "pullRequestEnvironmentName": str,
+    },
+    total=False,
+)
+
 _RequiredBackendEnvironmentTypeDef = TypedDict(
     "_RequiredBackendEnvironmentTypeDef",
     {
         "backendEnvironmentArn": str,
         "environmentName": str,
         "createTime": datetime,
         "updateTime": datetime,
@@ -240,14 +260,33 @@
     },
     total=False,
 )
 
 class BranchTypeDef(_RequiredBranchTypeDef, _OptionalBranchTypeDef):
     pass
 
+_RequiredCustomRuleTypeDef = TypedDict(
+    "_RequiredCustomRuleTypeDef",
+    {
+        "source": str,
+        "target": str,
+    },
+)
+_OptionalCustomRuleTypeDef = TypedDict(
+    "_OptionalCustomRuleTypeDef",
+    {
+        "status": str,
+        "condition": str,
+    },
+    total=False,
+)
+
+class CustomRuleTypeDef(_RequiredCustomRuleTypeDef, _OptionalCustomRuleTypeDef):
+    pass
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -749,14 +788,22 @@
     {
         "appId": str,
         "branchName": str,
         "jobId": str,
     },
 )
 
+SubDomainSettingOutputTypeDef = TypedDict(
+    "SubDomainSettingOutputTypeDef",
+    {
+        "prefix": str,
+        "branchName": str,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -819,14 +866,53 @@
 )
 
 class UpdateWebhookRequestRequestTypeDef(
     _RequiredUpdateWebhookRequestRequestTypeDef, _OptionalUpdateWebhookRequestRequestTypeDef
 ):
     pass
 
+_RequiredAppTypeDef = TypedDict(
+    "_RequiredAppTypeDef",
+    {
+        "appId": str,
+        "appArn": str,
+        "name": str,
+        "description": str,
+        "repository": str,
+        "platform": PlatformType,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "environmentVariables": Dict[str, str],
+        "defaultDomain": str,
+        "enableBranchAutoBuild": bool,
+        "enableBasicAuth": bool,
+    },
+)
+_OptionalAppTypeDef = TypedDict(
+    "_OptionalAppTypeDef",
+    {
+        "tags": Dict[str, str],
+        "iamServiceRoleArn": str,
+        "enableBranchAutoDeletion": bool,
+        "basicAuthCredentials": str,
+        "customRules": List[CustomRuleOutputTypeDef],
+        "productionBranch": ProductionBranchTypeDef,
+        "buildSpec": str,
+        "customHeaders": str,
+        "enableAutoBranchCreation": bool,
+        "autoBranchCreationPatterns": List[str],
+        "autoBranchCreationConfig": AutoBranchCreationConfigOutputTypeDef,
+        "repositoryCloneMethod": RepositoryCloneMethodType,
+    },
+    total=False,
+)
+
+class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+    pass
+
 _RequiredCreateAppRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAppRequestRequestTypeDef = TypedDict(
@@ -891,53 +977,14 @@
 )
 
 class UpdateAppRequestRequestTypeDef(
     _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
 ):
     pass
 
-_RequiredAppTypeDef = TypedDict(
-    "_RequiredAppTypeDef",
-    {
-        "appId": str,
-        "appArn": str,
-        "name": str,
-        "description": str,
-        "repository": str,
-        "platform": PlatformType,
-        "createTime": datetime,
-        "updateTime": datetime,
-        "environmentVariables": Dict[str, str],
-        "defaultDomain": str,
-        "enableBranchAutoBuild": bool,
-        "enableBasicAuth": bool,
-    },
-)
-_OptionalAppTypeDef = TypedDict(
-    "_OptionalAppTypeDef",
-    {
-        "tags": Dict[str, str],
-        "iamServiceRoleArn": str,
-        "enableBranchAutoDeletion": bool,
-        "basicAuthCredentials": str,
-        "customRules": List[CustomRuleTypeDef],
-        "productionBranch": ProductionBranchTypeDef,
-        "buildSpec": str,
-        "customHeaders": str,
-        "enableAutoBranchCreation": bool,
-        "autoBranchCreationPatterns": List[str],
-        "autoBranchCreationConfig": AutoBranchCreationConfigTypeDef,
-        "repositoryCloneMethod": RepositoryCloneMethodType,
-    },
-    total=False,
-)
-
-class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
-    pass
-
 CreateBackendEnvironmentResultTypeDef = TypedDict(
     "CreateBackendEnvironmentResultTypeDef",
     {
         "backendEnvironment": BackendEnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1072,23 +1119,14 @@
 
 class CreateDomainAssociationRequestRequestTypeDef(
     _RequiredCreateDomainAssociationRequestRequestTypeDef,
     _OptionalCreateDomainAssociationRequestRequestTypeDef,
 ):
     pass
 
-SubDomainTypeDef = TypedDict(
-    "SubDomainTypeDef",
-    {
-        "subDomainSetting": SubDomainSettingTypeDef,
-        "verified": bool,
-        "dnsRecord": str,
-    },
-)
-
 _RequiredUpdateDomainAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainAssociationRequestRequestTypeDef",
     {
         "appId": str,
         "domainName": str,
     },
 )
@@ -1263,14 +1301,23 @@
 )
 
 class ListJobsRequestListJobsPaginateTypeDef(
     _RequiredListJobsRequestListJobsPaginateTypeDef, _OptionalListJobsRequestListJobsPaginateTypeDef
 ):
     pass
 
+SubDomainTypeDef = TypedDict(
+    "SubDomainTypeDef",
+    {
+        "subDomainSetting": SubDomainSettingOutputTypeDef,
+        "verified": bool,
+        "dnsRecord": str,
+    },
+)
+
 CreateAppResultTypeDef = TypedDict(
     "CreateAppResultTypeDef",
     {
         "app": AppTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1304,14 +1351,22 @@
     "UpdateAppResultTypeDef",
     {
         "app": AppTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetJobResultTypeDef = TypedDict(
+    "GetJobResultTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDomainAssociationTypeDef = TypedDict(
     "_RequiredDomainAssociationTypeDef",
     {
         "domainAssociationArn": str,
         "domainName": str,
         "enableAutoSubDomain": bool,
         "domainStatus": DomainStatusType,
@@ -1330,22 +1385,14 @@
 )
 
 class DomainAssociationTypeDef(
     _RequiredDomainAssociationTypeDef, _OptionalDomainAssociationTypeDef
 ):
     pass
 
-GetJobResultTypeDef = TypedDict(
-    "GetJobResultTypeDef",
-    {
-        "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateDomainAssociationResultTypeDef = TypedDict(
     "CreateDomainAssociationResultTypeDef",
     {
         "domainAssociation": DomainAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify.egg-info/PKG-INFO` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplify
-Version: 1.28.0
-Summary: Type annotations for boto3.Amplify 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Amplify 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-amplify"></a>
 
 # mypy-boto3-amplify
 
 [![PyPI - mypy-boto3-amplify](https://img.shields.io/pypi/v/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplify?color=blue)](https://pypistats.org/packages/mypy-boto3-amplify)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplify)](https://pepy.tech/project/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,20 +337,22 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplify.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplify.type_defs import (
-    AutoBranchCreationConfigTypeDef,
-    CustomRuleTypeDef,
+    AutoBranchCreationConfigOutputTypeDef,
+    CustomRuleOutputTypeDef,
     ProductionBranchTypeDef,
     ArtifactTypeDef,
+    AutoBranchCreationConfigTypeDef,
     BackendEnvironmentTypeDef,
     BranchTypeDef,
+    CustomRuleTypeDef,
     ResponseMetadataTypeDef,
     CreateBackendEnvironmentRequestRequestTypeDef,
     CreateBranchRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     SubDomainSettingTypeDef,
     CreateWebhookRequestRequestTypeDef,
     WebhookTypeDef,
@@ -378,21 +380,22 @@
     ListDomainAssociationsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebhooksRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StartJobRequestRequestTypeDef,
     StopJobRequestRequestTypeDef,
+    SubDomainSettingOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBranchRequestRequestTypeDef,
     UpdateWebhookRequestRequestTypeDef,
+    AppTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
-    AppTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     DeleteBackendEnvironmentResultTypeDef,
     DeleteBranchResultTypeDef,
     GenerateAccessLogsResultTypeDef,
     GetArtifactUrlResultTypeDef,
@@ -400,15 +403,14 @@
     GetBranchResultTypeDef,
     ListArtifactsResultTypeDef,
     ListBackendEnvironmentsResultTypeDef,
     ListBranchesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateBranchResultTypeDef,
     CreateDomainAssociationRequestRequestTypeDef,
-    SubDomainTypeDef,
     UpdateDomainAssociationRequestRequestTypeDef,
     CreateWebhookResultTypeDef,
     DeleteWebhookResultTypeDef,
     GetWebhookResultTypeDef,
     ListWebhooksResultTypeDef,
     UpdateWebhookResultTypeDef,
     DeleteJobResultTypeDef,
@@ -417,30 +419,31 @@
     StartJobResultTypeDef,
     StopJobResultTypeDef,
     JobTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     ListBranchesRequestListBranchesPaginateTypeDef,
     ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
+    SubDomainTypeDef,
     CreateAppResultTypeDef,
     DeleteAppResultTypeDef,
     GetAppResultTypeDef,
     ListAppsResultTypeDef,
     UpdateAppResultTypeDef,
-    DomainAssociationTypeDef,
     GetJobResultTypeDef,
+    DomainAssociationTypeDef,
     CreateDomainAssociationResultTypeDef,
     DeleteDomainAssociationResultTypeDef,
     GetDomainAssociationResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
 )
 
 
-def get_structure() -> AutoBranchCreationConfigTypeDef:
+def get_structure() -> AutoBranchCreationConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplify-1.28.0/mypy_boto3_amplify.egg-info/SOURCES.txt` & `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.0/setup.py` & `mypy-boto3-amplify-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplify",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_amplify"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Amplify 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Amplify 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

