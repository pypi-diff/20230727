# Comparing `tmp/mypy-boto3-appfabric-1.28.0.tar.gz` & `tmp/mypy-boto3-appfabric-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appfabric-1.28.0.tar", last modified: Thu Jul  6 20:58:55 2023, max compression
+gzip compressed data, was "mypy-boto3-appfabric-1.28.12.tar", last modified: Thu Jul 27 05:34:16 2023, max compression
```

## Comparing `mypy-boto3-appfabric-1.28.0.tar` & `mypy-boto3-appfabric-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.406214 mypy-boto3-appfabric-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-06 20:58:55.398214 mypy-boto3-appfabric-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.394214 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21298 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-06 20:33:12.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25097 2023-07-06 20:33:13.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25064 2023-07-06 20:33:13.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.398214 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-06 20:58:55.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 20:58:55.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:55.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 20:58:55.000000 mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:55.406214 mypy-boto3-appfabric-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:33:11.000000 mypy-boto3-appfabric-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.260584 mypy-boto3-appfabric-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-07-27 05:34:16.252584 mypy-boto3-appfabric-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.248584 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21298 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.252584 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-07-27 05:34:16.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:16.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:16.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:16.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:16.260584 mypy-boto3-appfabric-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:17:17.000000 mypy-boto3-appfabric-1.28.12/setup.py
```

### Comparing `mypy-boto3-appfabric-1.28.0/LICENSE` & `mypy-boto3-appfabric-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.0/PKG-INFO` & `mypy-boto3-appfabric-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appfabric
-Version: 1.28.0
-Summary: Type annotations for boto3.AppFabric 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AppFabric 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-appfabric"></a>
 
 # mypy-boto3-appfabric
 
 [![PyPI - mypy-boto3-appfabric](https://img.shields.io/pypi/v/mypy-boto3-appfabric.svg?color=blue)](https://pypi.org/project/mypy-boto3-appfabric)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appfabric.svg?color=blue)](https://pypi.org/project/mypy-boto3-appfabric)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appfabric?color=blue)](https://pypistats.org/packages/mypy-boto3-appfabric)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appfabric)](https://pepy.tech/project/mypy-boto3-appfabric)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppFabric 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
+[boto3.AppFabric 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
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
 [mypy-boto3-appfabric docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,27 +342,31 @@
 
 `mypy_boto3_appfabric.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appfabric.type_defs import (
     ApiKeyCredentialTypeDef,
-    TenantTypeDef,
+    TenantOutputTypeDef,
     AppBundleSummaryTypeDef,
     AppBundleTypeDef,
+    AuditLogProcessingConfigurationOutputTypeDef,
     AuditLogProcessingConfigurationTypeDef,
     AuthRequestTypeDef,
     BatchGetUserAccessTasksRequestRequestTypeDef,
     TagTypeDef,
+    TenantTypeDef,
     IngestionTypeDef,
     Oauth2CredentialTypeDef,
     DeleteAppAuthorizationRequestRequestTypeDef,
     DeleteAppBundleRequestRequestTypeDef,
     DeleteIngestionDestinationRequestRequestTypeDef,
     DeleteIngestionRequestRequestTypeDef,
+    FirehoseStreamOutputTypeDef,
+    S3BucketOutputTypeDef,
     FirehoseStreamTypeDef,
     S3BucketTypeDef,
     GetAppAuthorizationRequestRequestTypeDef,
     GetAppBundleRequestRequestTypeDef,
     GetIngestionDestinationRequestRequestTypeDef,
     GetIngestionRequestRequestTypeDef,
     IngestionDestinationSummaryTypeDef,
@@ -372,53 +376,58 @@
     ListAppBundlesRequestListAppBundlesPaginateTypeDef,
     ListAppBundlesRequestRequestTypeDef,
     ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
     ListIngestionDestinationsRequestRequestTypeDef,
     ListIngestionsRequestListIngestionsPaginateTypeDef,
     ListIngestionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     StartIngestionRequestRequestTypeDef,
     StartUserAccessTasksRequestRequestTypeDef,
     StopIngestionRequestRequestTypeDef,
     TaskErrorTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppAuthorizationSummaryTypeDef,
     AppAuthorizationTypeDef,
     ListAppBundlesResponseTypeDef,
     CreateAppBundleResponseTypeDef,
     GetAppBundleResponseTypeDef,
+    ProcessingConfigurationOutputTypeDef,
     ProcessingConfigurationTypeDef,
     ConnectAppAuthorizationRequestRequestTypeDef,
     CreateAppBundleRequestRequestTypeDef,
     CreateIngestionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIngestionResponseTypeDef,
     GetIngestionResponseTypeDef,
     CredentialTypeDef,
+    DestinationOutputTypeDef,
     DestinationTypeDef,
     ListIngestionDestinationsResponseTypeDef,
     ListIngestionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UserAccessResultItemTypeDef,
     UserAccessTaskItemTypeDef,
     ConnectAppAuthorizationResponseTypeDef,
     ListAppAuthorizationsResponseTypeDef,
     CreateAppAuthorizationResponseTypeDef,
     GetAppAuthorizationResponseTypeDef,
     UpdateAppAuthorizationResponseTypeDef,
     CreateAppAuthorizationRequestRequestTypeDef,
     UpdateAppAuthorizationRequestRequestTypeDef,
+    AuditLogDestinationConfigurationOutputTypeDef,
     AuditLogDestinationConfigurationTypeDef,
     BatchGetUserAccessTasksResponseTypeDef,
     StartUserAccessTasksResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
-    CreateIngestionDestinationRequestRequestTypeDef,
     IngestionDestinationTypeDef,
+    CreateIngestionDestinationRequestRequestTypeDef,
     UpdateIngestionDestinationRequestRequestTypeDef,
     CreateIngestionDestinationResponseTypeDef,
     GetIngestionDestinationResponseTypeDef,
     UpdateIngestionDestinationResponseTypeDef,
 )
```

### Comparing `mypy-boto3-appfabric-1.28.0/README.md` & `mypy-boto3-appfabric-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-appfabric"></a>
 
 # mypy-boto3-appfabric
 
 [![PyPI - mypy-boto3-appfabric](https://img.shields.io/pypi/v/mypy-boto3-appfabric.svg?color=blue)](https://pypi.org/project/mypy-boto3-appfabric)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appfabric.svg?color=blue)](https://pypi.org/project/mypy-boto3-appfabric)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appfabric?color=blue)](https://pypistats.org/packages/mypy-boto3-appfabric)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appfabric)](https://pepy.tech/project/mypy-boto3-appfabric)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppFabric 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
+[boto3.AppFabric 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
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
 [mypy-boto3-appfabric docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,27 +310,31 @@
 
 `mypy_boto3_appfabric.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appfabric.type_defs import (
     ApiKeyCredentialTypeDef,
-    TenantTypeDef,
+    TenantOutputTypeDef,
     AppBundleSummaryTypeDef,
     AppBundleTypeDef,
+    AuditLogProcessingConfigurationOutputTypeDef,
     AuditLogProcessingConfigurationTypeDef,
     AuthRequestTypeDef,
     BatchGetUserAccessTasksRequestRequestTypeDef,
     TagTypeDef,
+    TenantTypeDef,
     IngestionTypeDef,
     Oauth2CredentialTypeDef,
     DeleteAppAuthorizationRequestRequestTypeDef,
     DeleteAppBundleRequestRequestTypeDef,
     DeleteIngestionDestinationRequestRequestTypeDef,
     DeleteIngestionRequestRequestTypeDef,
+    FirehoseStreamOutputTypeDef,
+    S3BucketOutputTypeDef,
     FirehoseStreamTypeDef,
     S3BucketTypeDef,
     GetAppAuthorizationRequestRequestTypeDef,
     GetAppBundleRequestRequestTypeDef,
     GetIngestionDestinationRequestRequestTypeDef,
     GetIngestionRequestRequestTypeDef,
     IngestionDestinationSummaryTypeDef,
@@ -340,53 +344,58 @@
     ListAppBundlesRequestListAppBundlesPaginateTypeDef,
     ListAppBundlesRequestRequestTypeDef,
     ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
     ListIngestionDestinationsRequestRequestTypeDef,
     ListIngestionsRequestListIngestionsPaginateTypeDef,
     ListIngestionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     StartIngestionRequestRequestTypeDef,
     StartUserAccessTasksRequestRequestTypeDef,
     StopIngestionRequestRequestTypeDef,
     TaskErrorTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppAuthorizationSummaryTypeDef,
     AppAuthorizationTypeDef,
     ListAppBundlesResponseTypeDef,
     CreateAppBundleResponseTypeDef,
     GetAppBundleResponseTypeDef,
+    ProcessingConfigurationOutputTypeDef,
     ProcessingConfigurationTypeDef,
     ConnectAppAuthorizationRequestRequestTypeDef,
     CreateAppBundleRequestRequestTypeDef,
     CreateIngestionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIngestionResponseTypeDef,
     GetIngestionResponseTypeDef,
     CredentialTypeDef,
+    DestinationOutputTypeDef,
     DestinationTypeDef,
     ListIngestionDestinationsResponseTypeDef,
     ListIngestionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UserAccessResultItemTypeDef,
     UserAccessTaskItemTypeDef,
     ConnectAppAuthorizationResponseTypeDef,
     ListAppAuthorizationsResponseTypeDef,
     CreateAppAuthorizationResponseTypeDef,
     GetAppAuthorizationResponseTypeDef,
     UpdateAppAuthorizationResponseTypeDef,
     CreateAppAuthorizationRequestRequestTypeDef,
     UpdateAppAuthorizationRequestRequestTypeDef,
+    AuditLogDestinationConfigurationOutputTypeDef,
     AuditLogDestinationConfigurationTypeDef,
     BatchGetUserAccessTasksResponseTypeDef,
     StartUserAccessTasksResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
-    CreateIngestionDestinationRequestRequestTypeDef,
     IngestionDestinationTypeDef,
+    CreateIngestionDestinationRequestRequestTypeDef,
     UpdateIngestionDestinationRequestRequestTypeDef,
     CreateIngestionDestinationResponseTypeDef,
     GetIngestionDestinationResponseTypeDef,
     UpdateIngestionDestinationResponseTypeDef,
 )
```

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/__init__.py` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/__init__.pyi` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/__main__.py` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppFabric 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.AppFabric 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric\nOther"
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

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/client.py` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/client.pyi` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/literals.py` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,15 @@
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
@@ -257,26 +258,28 @@
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

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/literals.pyi` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,15 @@
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
@@ -255,26 +256,28 @@
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

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/paginator.py` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/paginator.pyi` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/type_defs.py` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,27 +34,31 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApiKeyCredentialTypeDef",
-    "TenantTypeDef",
+    "TenantOutputTypeDef",
     "AppBundleSummaryTypeDef",
     "AppBundleTypeDef",
+    "AuditLogProcessingConfigurationOutputTypeDef",
     "AuditLogProcessingConfigurationTypeDef",
     "AuthRequestTypeDef",
     "BatchGetUserAccessTasksRequestRequestTypeDef",
     "TagTypeDef",
+    "TenantTypeDef",
     "IngestionTypeDef",
     "Oauth2CredentialTypeDef",
     "DeleteAppAuthorizationRequestRequestTypeDef",
     "DeleteAppBundleRequestRequestTypeDef",
     "DeleteIngestionDestinationRequestRequestTypeDef",
     "DeleteIngestionRequestRequestTypeDef",
+    "FirehoseStreamOutputTypeDef",
+    "S3BucketOutputTypeDef",
     "FirehoseStreamTypeDef",
     "S3BucketTypeDef",
     "GetAppAuthorizationRequestRequestTypeDef",
     "GetAppBundleRequestRequestTypeDef",
     "GetIngestionDestinationRequestRequestTypeDef",
     "GetIngestionRequestRequestTypeDef",
     "IngestionDestinationSummaryTypeDef",
@@ -64,68 +68,73 @@
     "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
     "ListAppBundlesRequestRequestTypeDef",
     "ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
     "ListIngestionDestinationsRequestRequestTypeDef",
     "ListIngestionsRequestListIngestionsPaginateTypeDef",
     "ListIngestionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "StartIngestionRequestRequestTypeDef",
     "StartUserAccessTasksRequestRequestTypeDef",
     "StopIngestionRequestRequestTypeDef",
     "TaskErrorTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AppAuthorizationSummaryTypeDef",
     "AppAuthorizationTypeDef",
     "ListAppBundlesResponseTypeDef",
     "CreateAppBundleResponseTypeDef",
     "GetAppBundleResponseTypeDef",
+    "ProcessingConfigurationOutputTypeDef",
     "ProcessingConfigurationTypeDef",
     "ConnectAppAuthorizationRequestRequestTypeDef",
     "CreateAppBundleRequestRequestTypeDef",
     "CreateIngestionRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIngestionResponseTypeDef",
     "GetIngestionResponseTypeDef",
     "CredentialTypeDef",
+    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "ListIngestionDestinationsResponseTypeDef",
     "ListIngestionsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "UserAccessResultItemTypeDef",
     "UserAccessTaskItemTypeDef",
     "ConnectAppAuthorizationResponseTypeDef",
     "ListAppAuthorizationsResponseTypeDef",
     "CreateAppAuthorizationResponseTypeDef",
     "GetAppAuthorizationResponseTypeDef",
     "UpdateAppAuthorizationResponseTypeDef",
     "CreateAppAuthorizationRequestRequestTypeDef",
     "UpdateAppAuthorizationRequestRequestTypeDef",
+    "AuditLogDestinationConfigurationOutputTypeDef",
     "AuditLogDestinationConfigurationTypeDef",
     "BatchGetUserAccessTasksResponseTypeDef",
     "StartUserAccessTasksResponseTypeDef",
+    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
-    "CreateIngestionDestinationRequestRequestTypeDef",
     "IngestionDestinationTypeDef",
+    "CreateIngestionDestinationRequestRequestTypeDef",
     "UpdateIngestionDestinationRequestRequestTypeDef",
     "CreateIngestionDestinationResponseTypeDef",
     "GetIngestionDestinationResponseTypeDef",
     "UpdateIngestionDestinationResponseTypeDef",
 )
 
 ApiKeyCredentialTypeDef = TypedDict(
     "ApiKeyCredentialTypeDef",
     {
         "apiKey": str,
     },
 )
 
-TenantTypeDef = TypedDict(
-    "TenantTypeDef",
+TenantOutputTypeDef = TypedDict(
+    "TenantOutputTypeDef",
     {
         "tenantIdentifier": str,
         "tenantDisplayName": str,
     },
 )
 
 AppBundleSummaryTypeDef = TypedDict(
@@ -150,14 +159,22 @@
 )
 
 
 class AppBundleTypeDef(_RequiredAppBundleTypeDef, _OptionalAppBundleTypeDef):
     pass
 
 
+AuditLogProcessingConfigurationOutputTypeDef = TypedDict(
+    "AuditLogProcessingConfigurationOutputTypeDef",
+    {
+        "schema": SchemaType,
+        "format": FormatType,
+    },
+)
+
 AuditLogProcessingConfigurationTypeDef = TypedDict(
     "AuditLogProcessingConfigurationTypeDef",
     {
         "schema": SchemaType,
         "format": FormatType,
     },
 )
@@ -182,14 +199,22 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+TenantTypeDef = TypedDict(
+    "TenantTypeDef",
+    {
+        "tenantIdentifier": str,
+        "tenantDisplayName": str,
+    },
+)
+
 IngestionTypeDef = TypedDict(
     "IngestionTypeDef",
     {
         "arn": str,
         "appBundleArn": str,
         "app": str,
         "tenantId": str,
@@ -236,14 +261,40 @@
     "DeleteIngestionRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "ingestionIdentifier": str,
     },
 )
 
+FirehoseStreamOutputTypeDef = TypedDict(
+    "FirehoseStreamOutputTypeDef",
+    {
+        "streamName": str,
+    },
+)
+
+_RequiredS3BucketOutputTypeDef = TypedDict(
+    "_RequiredS3BucketOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+_OptionalS3BucketOutputTypeDef = TypedDict(
+    "_OptionalS3BucketOutputTypeDef",
+    {
+        "prefix": str,
+    },
+    total=False,
+)
+
+
+class S3BucketOutputTypeDef(_RequiredS3BucketOutputTypeDef, _OptionalS3BucketOutputTypeDef):
+    pass
+
+
 FirehoseStreamTypeDef = TypedDict(
     "FirehoseStreamTypeDef",
     {
         "streamName": str,
     },
 )
 
@@ -471,14 +522,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
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
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -539,27 +598,27 @@
 
 AppAuthorizationSummaryTypeDef = TypedDict(
     "AppAuthorizationSummaryTypeDef",
     {
         "appAuthorizationArn": str,
         "appBundleArn": str,
         "app": str,
-        "tenant": TenantTypeDef,
+        "tenant": TenantOutputTypeDef,
         "status": AppAuthorizationStatusType,
         "updatedAt": datetime,
     },
 )
 
 _RequiredAppAuthorizationTypeDef = TypedDict(
     "_RequiredAppAuthorizationTypeDef",
     {
         "appAuthorizationArn": str,
         "appBundleArn": str,
         "app": str,
-        "tenant": TenantTypeDef,
+        "tenant": TenantOutputTypeDef,
         "authType": AuthTypeType,
         "status": AppAuthorizationStatusType,
         "createdAt": datetime,
         "updatedAt": datetime,
     },
 )
 _OptionalAppAuthorizationTypeDef = TypedDict(
@@ -597,14 +656,22 @@
     "GetAppBundleResponseTypeDef",
     {
         "appBundle": AppBundleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ProcessingConfigurationOutputTypeDef = TypedDict(
+    "ProcessingConfigurationOutputTypeDef",
+    {
+        "auditLog": AuditLogProcessingConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ProcessingConfigurationTypeDef = TypedDict(
     "ProcessingConfigurationTypeDef",
     {
         "auditLog": AuditLogProcessingConfigurationTypeDef,
     },
     total=False,
 )
@@ -663,22 +730,14 @@
 
 class CreateIngestionRequestRequestTypeDef(
     _RequiredCreateIngestionRequestRequestTypeDef, _OptionalCreateIngestionRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
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
@@ -704,14 +763,23 @@
     {
         "oauth2Credential": Oauth2CredentialTypeDef,
         "apiKeyCredential": ApiKeyCredentialTypeDef,
     },
     total=False,
 )
 
+DestinationOutputTypeDef = TypedDict(
+    "DestinationOutputTypeDef",
+    {
+        "s3Bucket": S3BucketOutputTypeDef,
+        "firehoseStream": FirehoseStreamOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Bucket": S3BucketTypeDef,
         "firehoseStream": FirehoseStreamTypeDef,
     },
     total=False,
@@ -731,14 +799,22 @@
     {
         "ingestions": List[IngestionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UserAccessResultItemTypeDef = TypedDict(
     "UserAccessResultItemTypeDef",
     {
         "app": str,
         "tenantId": str,
         "tenantDisplayName": str,
         "taskId": str,
@@ -865,14 +941,21 @@
 class UpdateAppAuthorizationRequestRequestTypeDef(
     _RequiredUpdateAppAuthorizationRequestRequestTypeDef,
     _OptionalUpdateAppAuthorizationRequestRequestTypeDef,
 ):
     pass
 
 
+AuditLogDestinationConfigurationOutputTypeDef = TypedDict(
+    "AuditLogDestinationConfigurationOutputTypeDef",
+    {
+        "destination": DestinationOutputTypeDef,
+    },
+)
+
 AuditLogDestinationConfigurationTypeDef = TypedDict(
     "AuditLogDestinationConfigurationTypeDef",
     {
         "destination": DestinationTypeDef,
     },
 )
 
@@ -888,71 +971,79 @@
     "StartUserAccessTasksResponseTypeDef",
     {
         "userAccessTasksList": List[UserAccessTaskItemTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DestinationConfigurationOutputTypeDef = TypedDict(
+    "DestinationConfigurationOutputTypeDef",
+    {
+        "auditLog": AuditLogDestinationConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "auditLog": AuditLogDestinationConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIngestionDestinationRequestRequestTypeDef",
+_RequiredIngestionDestinationTypeDef = TypedDict(
+    "_RequiredIngestionDestinationTypeDef",
     {
-        "appBundleIdentifier": str,
-        "ingestionIdentifier": str,
-        "processingConfiguration": ProcessingConfigurationTypeDef,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
+        "arn": str,
+        "ingestionArn": str,
+        "processingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
     },
 )
-_OptionalCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIngestionDestinationRequestRequestTypeDef",
+_OptionalIngestionDestinationTypeDef = TypedDict(
+    "_OptionalIngestionDestinationTypeDef",
     {
-        "clientToken": str,
-        "tags": Sequence[TagTypeDef],
+        "status": IngestionDestinationStatusType,
+        "statusReason": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
     },
     total=False,
 )
 
 
-class CreateIngestionDestinationRequestRequestTypeDef(
-    _RequiredCreateIngestionDestinationRequestRequestTypeDef,
-    _OptionalCreateIngestionDestinationRequestRequestTypeDef,
+class IngestionDestinationTypeDef(
+    _RequiredIngestionDestinationTypeDef, _OptionalIngestionDestinationTypeDef
 ):
     pass
 
 
-_RequiredIngestionDestinationTypeDef = TypedDict(
-    "_RequiredIngestionDestinationTypeDef",
+_RequiredCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIngestionDestinationRequestRequestTypeDef",
     {
-        "arn": str,
-        "ingestionArn": str,
+        "appBundleIdentifier": str,
+        "ingestionIdentifier": str,
         "processingConfiguration": ProcessingConfigurationTypeDef,
         "destinationConfiguration": DestinationConfigurationTypeDef,
     },
 )
-_OptionalIngestionDestinationTypeDef = TypedDict(
-    "_OptionalIngestionDestinationTypeDef",
+_OptionalCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIngestionDestinationRequestRequestTypeDef",
     {
-        "status": IngestionDestinationStatusType,
-        "statusReason": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
+        "clientToken": str,
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class IngestionDestinationTypeDef(
-    _RequiredIngestionDestinationTypeDef, _OptionalIngestionDestinationTypeDef
+class CreateIngestionDestinationRequestRequestTypeDef(
+    _RequiredCreateIngestionDestinationRequestRequestTypeDef,
+    _OptionalCreateIngestionDestinationRequestRequestTypeDef,
 ):
     pass
 
 
 UpdateIngestionDestinationRequestRequestTypeDef = TypedDict(
     "UpdateIngestionDestinationRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric/type_defs.pyi` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -33,27 +33,31 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApiKeyCredentialTypeDef",
-    "TenantTypeDef",
+    "TenantOutputTypeDef",
     "AppBundleSummaryTypeDef",
     "AppBundleTypeDef",
+    "AuditLogProcessingConfigurationOutputTypeDef",
     "AuditLogProcessingConfigurationTypeDef",
     "AuthRequestTypeDef",
     "BatchGetUserAccessTasksRequestRequestTypeDef",
     "TagTypeDef",
+    "TenantTypeDef",
     "IngestionTypeDef",
     "Oauth2CredentialTypeDef",
     "DeleteAppAuthorizationRequestRequestTypeDef",
     "DeleteAppBundleRequestRequestTypeDef",
     "DeleteIngestionDestinationRequestRequestTypeDef",
     "DeleteIngestionRequestRequestTypeDef",
+    "FirehoseStreamOutputTypeDef",
+    "S3BucketOutputTypeDef",
     "FirehoseStreamTypeDef",
     "S3BucketTypeDef",
     "GetAppAuthorizationRequestRequestTypeDef",
     "GetAppBundleRequestRequestTypeDef",
     "GetIngestionDestinationRequestRequestTypeDef",
     "GetIngestionRequestRequestTypeDef",
     "IngestionDestinationSummaryTypeDef",
@@ -63,68 +67,73 @@
     "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
     "ListAppBundlesRequestRequestTypeDef",
     "ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
     "ListIngestionDestinationsRequestRequestTypeDef",
     "ListIngestionsRequestListIngestionsPaginateTypeDef",
     "ListIngestionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "StartIngestionRequestRequestTypeDef",
     "StartUserAccessTasksRequestRequestTypeDef",
     "StopIngestionRequestRequestTypeDef",
     "TaskErrorTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AppAuthorizationSummaryTypeDef",
     "AppAuthorizationTypeDef",
     "ListAppBundlesResponseTypeDef",
     "CreateAppBundleResponseTypeDef",
     "GetAppBundleResponseTypeDef",
+    "ProcessingConfigurationOutputTypeDef",
     "ProcessingConfigurationTypeDef",
     "ConnectAppAuthorizationRequestRequestTypeDef",
     "CreateAppBundleRequestRequestTypeDef",
     "CreateIngestionRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIngestionResponseTypeDef",
     "GetIngestionResponseTypeDef",
     "CredentialTypeDef",
+    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "ListIngestionDestinationsResponseTypeDef",
     "ListIngestionsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "UserAccessResultItemTypeDef",
     "UserAccessTaskItemTypeDef",
     "ConnectAppAuthorizationResponseTypeDef",
     "ListAppAuthorizationsResponseTypeDef",
     "CreateAppAuthorizationResponseTypeDef",
     "GetAppAuthorizationResponseTypeDef",
     "UpdateAppAuthorizationResponseTypeDef",
     "CreateAppAuthorizationRequestRequestTypeDef",
     "UpdateAppAuthorizationRequestRequestTypeDef",
+    "AuditLogDestinationConfigurationOutputTypeDef",
     "AuditLogDestinationConfigurationTypeDef",
     "BatchGetUserAccessTasksResponseTypeDef",
     "StartUserAccessTasksResponseTypeDef",
+    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
-    "CreateIngestionDestinationRequestRequestTypeDef",
     "IngestionDestinationTypeDef",
+    "CreateIngestionDestinationRequestRequestTypeDef",
     "UpdateIngestionDestinationRequestRequestTypeDef",
     "CreateIngestionDestinationResponseTypeDef",
     "GetIngestionDestinationResponseTypeDef",
     "UpdateIngestionDestinationResponseTypeDef",
 )
 
 ApiKeyCredentialTypeDef = TypedDict(
     "ApiKeyCredentialTypeDef",
     {
         "apiKey": str,
     },
 )
 
-TenantTypeDef = TypedDict(
-    "TenantTypeDef",
+TenantOutputTypeDef = TypedDict(
+    "TenantOutputTypeDef",
     {
         "tenantIdentifier": str,
         "tenantDisplayName": str,
     },
 )
 
 AppBundleSummaryTypeDef = TypedDict(
@@ -147,14 +156,22 @@
     },
     total=False,
 )
 
 class AppBundleTypeDef(_RequiredAppBundleTypeDef, _OptionalAppBundleTypeDef):
     pass
 
+AuditLogProcessingConfigurationOutputTypeDef = TypedDict(
+    "AuditLogProcessingConfigurationOutputTypeDef",
+    {
+        "schema": SchemaType,
+        "format": FormatType,
+    },
+)
+
 AuditLogProcessingConfigurationTypeDef = TypedDict(
     "AuditLogProcessingConfigurationTypeDef",
     {
         "schema": SchemaType,
         "format": FormatType,
     },
 )
@@ -179,14 +196,22 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+TenantTypeDef = TypedDict(
+    "TenantTypeDef",
+    {
+        "tenantIdentifier": str,
+        "tenantDisplayName": str,
+    },
+)
+
 IngestionTypeDef = TypedDict(
     "IngestionTypeDef",
     {
         "arn": str,
         "appBundleArn": str,
         "app": str,
         "tenantId": str,
@@ -233,14 +258,38 @@
     "DeleteIngestionRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "ingestionIdentifier": str,
     },
 )
 
+FirehoseStreamOutputTypeDef = TypedDict(
+    "FirehoseStreamOutputTypeDef",
+    {
+        "streamName": str,
+    },
+)
+
+_RequiredS3BucketOutputTypeDef = TypedDict(
+    "_RequiredS3BucketOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+_OptionalS3BucketOutputTypeDef = TypedDict(
+    "_OptionalS3BucketOutputTypeDef",
+    {
+        "prefix": str,
+    },
+    total=False,
+)
+
+class S3BucketOutputTypeDef(_RequiredS3BucketOutputTypeDef, _OptionalS3BucketOutputTypeDef):
+    pass
+
 FirehoseStreamTypeDef = TypedDict(
     "FirehoseStreamTypeDef",
     {
         "streamName": str,
     },
 )
 
@@ -454,14 +503,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
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
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -522,27 +579,27 @@
 
 AppAuthorizationSummaryTypeDef = TypedDict(
     "AppAuthorizationSummaryTypeDef",
     {
         "appAuthorizationArn": str,
         "appBundleArn": str,
         "app": str,
-        "tenant": TenantTypeDef,
+        "tenant": TenantOutputTypeDef,
         "status": AppAuthorizationStatusType,
         "updatedAt": datetime,
     },
 )
 
 _RequiredAppAuthorizationTypeDef = TypedDict(
     "_RequiredAppAuthorizationTypeDef",
     {
         "appAuthorizationArn": str,
         "appBundleArn": str,
         "app": str,
-        "tenant": TenantTypeDef,
+        "tenant": TenantOutputTypeDef,
         "authType": AuthTypeType,
         "status": AppAuthorizationStatusType,
         "createdAt": datetime,
         "updatedAt": datetime,
     },
 )
 _OptionalAppAuthorizationTypeDef = TypedDict(
@@ -578,14 +635,22 @@
     "GetAppBundleResponseTypeDef",
     {
         "appBundle": AppBundleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ProcessingConfigurationOutputTypeDef = TypedDict(
+    "ProcessingConfigurationOutputTypeDef",
+    {
+        "auditLog": AuditLogProcessingConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ProcessingConfigurationTypeDef = TypedDict(
     "ProcessingConfigurationTypeDef",
     {
         "auditLog": AuditLogProcessingConfigurationTypeDef,
     },
     total=False,
 )
@@ -640,22 +705,14 @@
 )
 
 class CreateIngestionRequestRequestTypeDef(
     _RequiredCreateIngestionRequestRequestTypeDef, _OptionalCreateIngestionRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
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
@@ -681,14 +738,23 @@
     {
         "oauth2Credential": Oauth2CredentialTypeDef,
         "apiKeyCredential": ApiKeyCredentialTypeDef,
     },
     total=False,
 )
 
+DestinationOutputTypeDef = TypedDict(
+    "DestinationOutputTypeDef",
+    {
+        "s3Bucket": S3BucketOutputTypeDef,
+        "firehoseStream": FirehoseStreamOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Bucket": S3BucketTypeDef,
         "firehoseStream": FirehoseStreamTypeDef,
     },
     total=False,
@@ -708,14 +774,22 @@
     {
         "ingestions": List[IngestionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UserAccessResultItemTypeDef = TypedDict(
     "UserAccessResultItemTypeDef",
     {
         "app": str,
         "tenantId": str,
         "tenantDisplayName": str,
         "taskId": str,
@@ -836,14 +910,21 @@
 
 class UpdateAppAuthorizationRequestRequestTypeDef(
     _RequiredUpdateAppAuthorizationRequestRequestTypeDef,
     _OptionalUpdateAppAuthorizationRequestRequestTypeDef,
 ):
     pass
 
+AuditLogDestinationConfigurationOutputTypeDef = TypedDict(
+    "AuditLogDestinationConfigurationOutputTypeDef",
+    {
+        "destination": DestinationOutputTypeDef,
+    },
+)
+
 AuditLogDestinationConfigurationTypeDef = TypedDict(
     "AuditLogDestinationConfigurationTypeDef",
     {
         "destination": DestinationTypeDef,
     },
 )
 
@@ -859,53 +940,37 @@
     "StartUserAccessTasksResponseTypeDef",
     {
         "userAccessTasksList": List[UserAccessTaskItemTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DestinationConfigurationTypeDef = TypedDict(
-    "DestinationConfigurationTypeDef",
+DestinationConfigurationOutputTypeDef = TypedDict(
+    "DestinationConfigurationOutputTypeDef",
     {
-        "auditLog": AuditLogDestinationConfigurationTypeDef,
+        "auditLog": AuditLogDestinationConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIngestionDestinationRequestRequestTypeDef",
-    {
-        "appBundleIdentifier": str,
-        "ingestionIdentifier": str,
-        "processingConfiguration": ProcessingConfigurationTypeDef,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-    },
-)
-_OptionalCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIngestionDestinationRequestRequestTypeDef",
+DestinationConfigurationTypeDef = TypedDict(
+    "DestinationConfigurationTypeDef",
     {
-        "clientToken": str,
-        "tags": Sequence[TagTypeDef],
+        "auditLog": AuditLogDestinationConfigurationTypeDef,
     },
     total=False,
 )
 
-class CreateIngestionDestinationRequestRequestTypeDef(
-    _RequiredCreateIngestionDestinationRequestRequestTypeDef,
-    _OptionalCreateIngestionDestinationRequestRequestTypeDef,
-):
-    pass
-
 _RequiredIngestionDestinationTypeDef = TypedDict(
     "_RequiredIngestionDestinationTypeDef",
     {
         "arn": str,
         "ingestionArn": str,
-        "processingConfiguration": ProcessingConfigurationTypeDef,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
+        "processingConfiguration": ProcessingConfigurationOutputTypeDef,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
     },
 )
 _OptionalIngestionDestinationTypeDef = TypedDict(
     "_OptionalIngestionDestinationTypeDef",
     {
         "status": IngestionDestinationStatusType,
         "statusReason": str,
@@ -916,14 +981,38 @@
 )
 
 class IngestionDestinationTypeDef(
     _RequiredIngestionDestinationTypeDef, _OptionalIngestionDestinationTypeDef
 ):
     pass
 
+_RequiredCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIngestionDestinationRequestRequestTypeDef",
+    {
+        "appBundleIdentifier": str,
+        "ingestionIdentifier": str,
+        "processingConfiguration": ProcessingConfigurationTypeDef,
+        "destinationConfiguration": DestinationConfigurationTypeDef,
+    },
+)
+_OptionalCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIngestionDestinationRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateIngestionDestinationRequestRequestTypeDef(
+    _RequiredCreateIngestionDestinationRequestRequestTypeDef,
+    _OptionalCreateIngestionDestinationRequestRequestTypeDef,
+):
+    pass
+
 UpdateIngestionDestinationRequestRequestTypeDef = TypedDict(
     "UpdateIngestionDestinationRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "ingestionIdentifier": str,
         "ingestionDestinationIdentifier": str,
         "destinationConfiguration": DestinationConfigurationTypeDef,
```

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric.egg-info/PKG-INFO` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appfabric
-Version: 1.28.0
-Summary: Type annotations for boto3.AppFabric 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AppFabric 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-appfabric"></a>
 
 # mypy-boto3-appfabric
 
 [![PyPI - mypy-boto3-appfabric](https://img.shields.io/pypi/v/mypy-boto3-appfabric.svg?color=blue)](https://pypi.org/project/mypy-boto3-appfabric)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appfabric.svg?color=blue)](https://pypi.org/project/mypy-boto3-appfabric)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appfabric?color=blue)](https://pypistats.org/packages/mypy-boto3-appfabric)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appfabric)](https://pepy.tech/project/mypy-boto3-appfabric)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppFabric 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
+[boto3.AppFabric 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
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
 [mypy-boto3-appfabric docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,27 +342,31 @@
 
 `mypy_boto3_appfabric.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appfabric.type_defs import (
     ApiKeyCredentialTypeDef,
-    TenantTypeDef,
+    TenantOutputTypeDef,
     AppBundleSummaryTypeDef,
     AppBundleTypeDef,
+    AuditLogProcessingConfigurationOutputTypeDef,
     AuditLogProcessingConfigurationTypeDef,
     AuthRequestTypeDef,
     BatchGetUserAccessTasksRequestRequestTypeDef,
     TagTypeDef,
+    TenantTypeDef,
     IngestionTypeDef,
     Oauth2CredentialTypeDef,
     DeleteAppAuthorizationRequestRequestTypeDef,
     DeleteAppBundleRequestRequestTypeDef,
     DeleteIngestionDestinationRequestRequestTypeDef,
     DeleteIngestionRequestRequestTypeDef,
+    FirehoseStreamOutputTypeDef,
+    S3BucketOutputTypeDef,
     FirehoseStreamTypeDef,
     S3BucketTypeDef,
     GetAppAuthorizationRequestRequestTypeDef,
     GetAppBundleRequestRequestTypeDef,
     GetIngestionDestinationRequestRequestTypeDef,
     GetIngestionRequestRequestTypeDef,
     IngestionDestinationSummaryTypeDef,
@@ -372,53 +376,58 @@
     ListAppBundlesRequestListAppBundlesPaginateTypeDef,
     ListAppBundlesRequestRequestTypeDef,
     ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
     ListIngestionDestinationsRequestRequestTypeDef,
     ListIngestionsRequestListIngestionsPaginateTypeDef,
     ListIngestionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     StartIngestionRequestRequestTypeDef,
     StartUserAccessTasksRequestRequestTypeDef,
     StopIngestionRequestRequestTypeDef,
     TaskErrorTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppAuthorizationSummaryTypeDef,
     AppAuthorizationTypeDef,
     ListAppBundlesResponseTypeDef,
     CreateAppBundleResponseTypeDef,
     GetAppBundleResponseTypeDef,
+    ProcessingConfigurationOutputTypeDef,
     ProcessingConfigurationTypeDef,
     ConnectAppAuthorizationRequestRequestTypeDef,
     CreateAppBundleRequestRequestTypeDef,
     CreateIngestionRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIngestionResponseTypeDef,
     GetIngestionResponseTypeDef,
     CredentialTypeDef,
+    DestinationOutputTypeDef,
     DestinationTypeDef,
     ListIngestionDestinationsResponseTypeDef,
     ListIngestionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     UserAccessResultItemTypeDef,
     UserAccessTaskItemTypeDef,
     ConnectAppAuthorizationResponseTypeDef,
     ListAppAuthorizationsResponseTypeDef,
     CreateAppAuthorizationResponseTypeDef,
     GetAppAuthorizationResponseTypeDef,
     UpdateAppAuthorizationResponseTypeDef,
     CreateAppAuthorizationRequestRequestTypeDef,
     UpdateAppAuthorizationRequestRequestTypeDef,
+    AuditLogDestinationConfigurationOutputTypeDef,
     AuditLogDestinationConfigurationTypeDef,
     BatchGetUserAccessTasksResponseTypeDef,
     StartUserAccessTasksResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
-    CreateIngestionDestinationRequestRequestTypeDef,
     IngestionDestinationTypeDef,
+    CreateIngestionDestinationRequestRequestTypeDef,
     UpdateIngestionDestinationRequestRequestTypeDef,
     CreateIngestionDestinationResponseTypeDef,
     GetIngestionDestinationResponseTypeDef,
     UpdateIngestionDestinationResponseTypeDef,
 )
```

### Comparing `mypy-boto3-appfabric-1.28.0/mypy_boto3_appfabric.egg-info/SOURCES.txt` & `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.0/setup.py` & `mypy-boto3-appfabric-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appfabric",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_appfabric"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppFabric 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.AppFabric 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

