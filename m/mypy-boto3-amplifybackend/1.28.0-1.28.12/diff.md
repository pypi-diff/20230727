# Comparing `tmp/mypy-boto3-amplifybackend-1.28.0.tar.gz` & `tmp/mypy-boto3-amplifybackend-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplifybackend-1.28.0.tar", last modified: Thu Jul  6 20:58:55 2023, max compression
+gzip compressed data, was "mypy-boto3-amplifybackend-1.28.12.tar", last modified: Thu Jul 27 05:34:16 2023, max compression
```

## Comparing `mypy-boto3-amplifybackend-1.28.0.tar` & `mypy-boto3-amplifybackend-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.366214 mypy-boto3-amplifybackend-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:32:45.000000 mypy-boto3-amplifybackend-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-07-06 20:58:55.366214 mypy-boto3-amplifybackend-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-06 20:32:45.000000 mypy-boto3-amplifybackend-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.358214 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 20:32:45.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-06 20:32:45.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:32:45.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23022 2023-07-06 20:32:45.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22983 2023-07-06 20:32:45.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-06 20:32:46.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-06 20:32:46.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-06 20:32:45.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-06 20:32:45.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:45.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    38938 2023-07-06 20:32:47.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38885 2023-07-06 20:32:46.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:32:45.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.366214 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-07-06 20:58:55.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 20:58:55.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:55.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 20:58:55.000000 mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:55.366214 mypy-boto3-amplifybackend-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-06 20:32:44.000000 mypy-boto3-amplifybackend-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.332584 mypy-boto3-amplifybackend-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-07-27 05:34:16.332584 mypy-boto3-amplifybackend-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.332584 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23022 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22983 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48488 2023-07-27 05:17:03.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48419 2023-07-27 05:17:03.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.332584 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-07-27 05:34:16.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:16.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:16.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:16.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:16.332584 mypy-boto3-amplifybackend-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/setup.py
```

### Comparing `mypy-boto3-amplifybackend-1.28.0/LICENSE` & `mypy-boto3-amplifybackend-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.0/PKG-INFO` & `mypy-boto3-amplifybackend-1.28.12/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifybackend
-Version: 1.28.0
-Summary: Type annotations for boto3.AmplifyBackend 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AmplifyBackend 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-amplifybackend"></a>
 
 # mypy-boto3-amplifybackend
 
 [![PyPI - mypy-boto3-amplifybackend](https://img.shields.io/pypi/v/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplifybackend?color=blue)](https://pypistats.org/packages/mypy-boto3-amplifybackend)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifybackend)](https://pepy.tech/project/mypy-boto3-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyBackend 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[boto3.AmplifyBackend 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,26 +336,36 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplifybackend.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifybackend.type_defs import (
+    BackendAPIAppSyncAuthSettingsOutputTypeDef,
     BackendAPIAppSyncAuthSettingsTypeDef,
+    BackendAPIConflictResolutionOutputTypeDef,
     BackendAPIConflictResolutionTypeDef,
+    BackendAuthAppleProviderConfigOutputTypeDef,
     BackendAuthAppleProviderConfigTypeDef,
+    BackendAuthSocialProviderConfigOutputTypeDef,
     BackendAuthSocialProviderConfigTypeDef,
     BackendJobRespObjTypeDef,
+    BackendStoragePermissionsOutputTypeDef,
     BackendStoragePermissionsTypeDef,
     CloneBackendRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    EmailSettingsOutputTypeDef,
+    SmsSettingsOutputTypeDef,
     EmailSettingsTypeDef,
     SmsSettingsTypeDef,
+    CreateBackendAuthIdentityPoolConfigOutputTypeDef,
     CreateBackendAuthIdentityPoolConfigTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
+    CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
     CreateBackendAuthPasswordPolicyConfigTypeDef,
     CreateBackendConfigRequestRequestTypeDef,
     CreateBackendRequestRequestTypeDef,
     CreateTokenRequestRequestTypeDef,
     DeleteBackendAuthRequestRequestTypeDef,
     DeleteBackendRequestRequestTypeDef,
     DeleteBackendStorageRequestRequestTypeDef,
@@ -369,24 +379,27 @@
     GetTokenRequestRequestTypeDef,
     ImportBackendAuthRequestRequestTypeDef,
     ImportBackendStorageRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListBackendJobsRequestRequestTypeDef,
     ListS3BucketsRequestRequestTypeDef,
     S3BucketInfoTypeDef,
+    LoginAuthConfigReqObjOutputTypeDef,
     LoginAuthConfigReqObjTypeDef,
     RemoveAllBackendsRequestRequestTypeDef,
     RemoveBackendConfigRequestRequestTypeDef,
     UpdateBackendAuthIdentityPoolConfigTypeDef,
     UpdateBackendAuthPasswordPolicyConfigTypeDef,
     UpdateBackendJobRequestRequestTypeDef,
+    BackendAPIAuthTypeOutputTypeDef,
     BackendAPIAuthTypeTypeDef,
+    SocialProviderSettingsOutputTypeDef,
     SocialProviderSettingsTypeDef,
-    CreateBackendStorageResourceConfigTypeDef,
     GetBackendStorageResourceConfigTypeDef,
+    CreateBackendStorageResourceConfigTypeDef,
     UpdateBackendStorageResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResponseTypeDef,
@@ -406,46 +419,53 @@
     ListBackendJobsResponseTypeDef,
     RemoveAllBackendsResponseTypeDef,
     RemoveBackendConfigResponseTypeDef,
     UpdateBackendAPIResponseTypeDef,
     UpdateBackendAuthResponseTypeDef,
     UpdateBackendJobResponseTypeDef,
     UpdateBackendStorageResponseTypeDef,
+    CreateBackendAuthForgotPasswordConfigOutputTypeDef,
+    CreateBackendAuthVerificationMessageConfigOutputTypeDef,
     CreateBackendAuthForgotPasswordConfigTypeDef,
     CreateBackendAuthVerificationMessageConfigTypeDef,
     UpdateBackendAuthForgotPasswordConfigTypeDef,
     UpdateBackendAuthVerificationMessageConfigTypeDef,
+    CreateBackendAuthMFAConfigOutputTypeDef,
     CreateBackendAuthMFAConfigTypeDef,
     UpdateBackendAuthMFAConfigTypeDef,
     ListBackendJobsRequestListBackendJobsPaginateTypeDef,
     ListS3BucketsResponseTypeDef,
-    UpdateBackendConfigRequestRequestTypeDef,
     UpdateBackendConfigResponseTypeDef,
+    UpdateBackendConfigRequestRequestTypeDef,
+    BackendAPIResourceConfigOutputTypeDef,
     BackendAPIResourceConfigTypeDef,
+    CreateBackendAuthOAuthConfigOutputTypeDef,
     CreateBackendAuthOAuthConfigTypeDef,
     UpdateBackendAuthOAuthConfigTypeDef,
-    CreateBackendStorageRequestRequestTypeDef,
     GetBackendStorageResponseTypeDef,
+    CreateBackendStorageRequestRequestTypeDef,
     UpdateBackendStorageRequestRequestTypeDef,
+    GetBackendAPIResponseTypeDef,
     CreateBackendAPIRequestRequestTypeDef,
     DeleteBackendAPIRequestRequestTypeDef,
     GetBackendAPIRequestRequestTypeDef,
-    GetBackendAPIResponseTypeDef,
     UpdateBackendAPIRequestRequestTypeDef,
+    CreateBackendAuthUserPoolConfigOutputTypeDef,
     CreateBackendAuthUserPoolConfigTypeDef,
     UpdateBackendAuthUserPoolConfigTypeDef,
+    CreateBackendAuthResourceConfigOutputTypeDef,
     CreateBackendAuthResourceConfigTypeDef,
     UpdateBackendAuthResourceConfigTypeDef,
-    CreateBackendAuthRequestRequestTypeDef,
     GetBackendAuthResponseTypeDef,
+    CreateBackendAuthRequestRequestTypeDef,
     UpdateBackendAuthRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BackendAPIAppSyncAuthSettingsTypeDef:
+def get_structure() -> BackendAPIAppSyncAuthSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifybackend-1.28.0/README.md` & `mypy-boto3-amplifybackend-1.28.12/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-amplifybackend"></a>
 
 # mypy-boto3-amplifybackend
 
 [![PyPI - mypy-boto3-amplifybackend](https://img.shields.io/pypi/v/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplifybackend?color=blue)](https://pypistats.org/packages/mypy-boto3-amplifybackend)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifybackend)](https://pepy.tech/project/mypy-boto3-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyBackend 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[boto3.AmplifyBackend 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,26 +304,36 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplifybackend.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifybackend.type_defs import (
+    BackendAPIAppSyncAuthSettingsOutputTypeDef,
     BackendAPIAppSyncAuthSettingsTypeDef,
+    BackendAPIConflictResolutionOutputTypeDef,
     BackendAPIConflictResolutionTypeDef,
+    BackendAuthAppleProviderConfigOutputTypeDef,
     BackendAuthAppleProviderConfigTypeDef,
+    BackendAuthSocialProviderConfigOutputTypeDef,
     BackendAuthSocialProviderConfigTypeDef,
     BackendJobRespObjTypeDef,
+    BackendStoragePermissionsOutputTypeDef,
     BackendStoragePermissionsTypeDef,
     CloneBackendRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    EmailSettingsOutputTypeDef,
+    SmsSettingsOutputTypeDef,
     EmailSettingsTypeDef,
     SmsSettingsTypeDef,
+    CreateBackendAuthIdentityPoolConfigOutputTypeDef,
     CreateBackendAuthIdentityPoolConfigTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
+    CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
     CreateBackendAuthPasswordPolicyConfigTypeDef,
     CreateBackendConfigRequestRequestTypeDef,
     CreateBackendRequestRequestTypeDef,
     CreateTokenRequestRequestTypeDef,
     DeleteBackendAuthRequestRequestTypeDef,
     DeleteBackendRequestRequestTypeDef,
     DeleteBackendStorageRequestRequestTypeDef,
@@ -337,24 +347,27 @@
     GetTokenRequestRequestTypeDef,
     ImportBackendAuthRequestRequestTypeDef,
     ImportBackendStorageRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListBackendJobsRequestRequestTypeDef,
     ListS3BucketsRequestRequestTypeDef,
     S3BucketInfoTypeDef,
+    LoginAuthConfigReqObjOutputTypeDef,
     LoginAuthConfigReqObjTypeDef,
     RemoveAllBackendsRequestRequestTypeDef,
     RemoveBackendConfigRequestRequestTypeDef,
     UpdateBackendAuthIdentityPoolConfigTypeDef,
     UpdateBackendAuthPasswordPolicyConfigTypeDef,
     UpdateBackendJobRequestRequestTypeDef,
+    BackendAPIAuthTypeOutputTypeDef,
     BackendAPIAuthTypeTypeDef,
+    SocialProviderSettingsOutputTypeDef,
     SocialProviderSettingsTypeDef,
-    CreateBackendStorageResourceConfigTypeDef,
     GetBackendStorageResourceConfigTypeDef,
+    CreateBackendStorageResourceConfigTypeDef,
     UpdateBackendStorageResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResponseTypeDef,
@@ -374,46 +387,53 @@
     ListBackendJobsResponseTypeDef,
     RemoveAllBackendsResponseTypeDef,
     RemoveBackendConfigResponseTypeDef,
     UpdateBackendAPIResponseTypeDef,
     UpdateBackendAuthResponseTypeDef,
     UpdateBackendJobResponseTypeDef,
     UpdateBackendStorageResponseTypeDef,
+    CreateBackendAuthForgotPasswordConfigOutputTypeDef,
+    CreateBackendAuthVerificationMessageConfigOutputTypeDef,
     CreateBackendAuthForgotPasswordConfigTypeDef,
     CreateBackendAuthVerificationMessageConfigTypeDef,
     UpdateBackendAuthForgotPasswordConfigTypeDef,
     UpdateBackendAuthVerificationMessageConfigTypeDef,
+    CreateBackendAuthMFAConfigOutputTypeDef,
     CreateBackendAuthMFAConfigTypeDef,
     UpdateBackendAuthMFAConfigTypeDef,
     ListBackendJobsRequestListBackendJobsPaginateTypeDef,
     ListS3BucketsResponseTypeDef,
-    UpdateBackendConfigRequestRequestTypeDef,
     UpdateBackendConfigResponseTypeDef,
+    UpdateBackendConfigRequestRequestTypeDef,
+    BackendAPIResourceConfigOutputTypeDef,
     BackendAPIResourceConfigTypeDef,
+    CreateBackendAuthOAuthConfigOutputTypeDef,
     CreateBackendAuthOAuthConfigTypeDef,
     UpdateBackendAuthOAuthConfigTypeDef,
-    CreateBackendStorageRequestRequestTypeDef,
     GetBackendStorageResponseTypeDef,
+    CreateBackendStorageRequestRequestTypeDef,
     UpdateBackendStorageRequestRequestTypeDef,
+    GetBackendAPIResponseTypeDef,
     CreateBackendAPIRequestRequestTypeDef,
     DeleteBackendAPIRequestRequestTypeDef,
     GetBackendAPIRequestRequestTypeDef,
-    GetBackendAPIResponseTypeDef,
     UpdateBackendAPIRequestRequestTypeDef,
+    CreateBackendAuthUserPoolConfigOutputTypeDef,
     CreateBackendAuthUserPoolConfigTypeDef,
     UpdateBackendAuthUserPoolConfigTypeDef,
+    CreateBackendAuthResourceConfigOutputTypeDef,
     CreateBackendAuthResourceConfigTypeDef,
     UpdateBackendAuthResourceConfigTypeDef,
-    CreateBackendAuthRequestRequestTypeDef,
     GetBackendAuthResponseTypeDef,
+    CreateBackendAuthRequestRequestTypeDef,
     UpdateBackendAuthRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BackendAPIAppSyncAuthSettingsTypeDef:
+def get_structure() -> BackendAPIAppSyncAuthSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/__init__.py` & `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/__init__.pyi` & `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/client.py` & `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/client.pyi` & `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/literals.py` & `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,14 +200,15 @@
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
@@ -286,26 +287,28 @@
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

### Comparing `mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/literals.pyi` & `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,15 @@
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
@@ -284,26 +285,28 @@
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

### Comparing `mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/paginator.py` & `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/paginator.pyi` & `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/type_defs.py` & `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplifybackend service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsTypeDef
+    from mypy_boto3_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsOutputTypeDef
 
-    data: BackendAPIAppSyncAuthSettingsTypeDef = {...}
+    data: BackendAPIAppSyncAuthSettingsOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AdditionalConstraintsElementType,
@@ -38,26 +38,36 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BackendAPIAppSyncAuthSettingsOutputTypeDef",
     "BackendAPIAppSyncAuthSettingsTypeDef",
+    "BackendAPIConflictResolutionOutputTypeDef",
     "BackendAPIConflictResolutionTypeDef",
+    "BackendAuthAppleProviderConfigOutputTypeDef",
     "BackendAuthAppleProviderConfigTypeDef",
+    "BackendAuthSocialProviderConfigOutputTypeDef",
     "BackendAuthSocialProviderConfigTypeDef",
     "BackendJobRespObjTypeDef",
+    "BackendStoragePermissionsOutputTypeDef",
     "BackendStoragePermissionsTypeDef",
     "CloneBackendRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "EmailSettingsOutputTypeDef",
+    "SmsSettingsOutputTypeDef",
     "EmailSettingsTypeDef",
     "SmsSettingsTypeDef",
+    "CreateBackendAuthIdentityPoolConfigOutputTypeDef",
     "CreateBackendAuthIdentityPoolConfigTypeDef",
+    "SettingsOutputTypeDef",
     "SettingsTypeDef",
+    "CreateBackendAuthPasswordPolicyConfigOutputTypeDef",
     "CreateBackendAuthPasswordPolicyConfigTypeDef",
     "CreateBackendConfigRequestRequestTypeDef",
     "CreateBackendRequestRequestTypeDef",
     "CreateTokenRequestRequestTypeDef",
     "DeleteBackendAuthRequestRequestTypeDef",
     "DeleteBackendRequestRequestTypeDef",
     "DeleteBackendStorageRequestRequestTypeDef",
@@ -71,24 +81,27 @@
     "GetTokenRequestRequestTypeDef",
     "ImportBackendAuthRequestRequestTypeDef",
     "ImportBackendStorageRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListBackendJobsRequestRequestTypeDef",
     "ListS3BucketsRequestRequestTypeDef",
     "S3BucketInfoTypeDef",
+    "LoginAuthConfigReqObjOutputTypeDef",
     "LoginAuthConfigReqObjTypeDef",
     "RemoveAllBackendsRequestRequestTypeDef",
     "RemoveBackendConfigRequestRequestTypeDef",
     "UpdateBackendAuthIdentityPoolConfigTypeDef",
     "UpdateBackendAuthPasswordPolicyConfigTypeDef",
     "UpdateBackendJobRequestRequestTypeDef",
+    "BackendAPIAuthTypeOutputTypeDef",
     "BackendAPIAuthTypeTypeDef",
+    "SocialProviderSettingsOutputTypeDef",
     "SocialProviderSettingsTypeDef",
-    "CreateBackendStorageResourceConfigTypeDef",
     "GetBackendStorageResourceConfigTypeDef",
+    "CreateBackendStorageResourceConfigTypeDef",
     "UpdateBackendStorageResourceConfigTypeDef",
     "CloneBackendResponseTypeDef",
     "CreateBackendAPIResponseTypeDef",
     "CreateBackendAuthResponseTypeDef",
     "CreateBackendConfigResponseTypeDef",
     "CreateBackendResponseTypeDef",
     "CreateBackendStorageResponseTypeDef",
@@ -108,44 +121,66 @@
     "ListBackendJobsResponseTypeDef",
     "RemoveAllBackendsResponseTypeDef",
     "RemoveBackendConfigResponseTypeDef",
     "UpdateBackendAPIResponseTypeDef",
     "UpdateBackendAuthResponseTypeDef",
     "UpdateBackendJobResponseTypeDef",
     "UpdateBackendStorageResponseTypeDef",
+    "CreateBackendAuthForgotPasswordConfigOutputTypeDef",
+    "CreateBackendAuthVerificationMessageConfigOutputTypeDef",
     "CreateBackendAuthForgotPasswordConfigTypeDef",
     "CreateBackendAuthVerificationMessageConfigTypeDef",
     "UpdateBackendAuthForgotPasswordConfigTypeDef",
     "UpdateBackendAuthVerificationMessageConfigTypeDef",
+    "CreateBackendAuthMFAConfigOutputTypeDef",
     "CreateBackendAuthMFAConfigTypeDef",
     "UpdateBackendAuthMFAConfigTypeDef",
     "ListBackendJobsRequestListBackendJobsPaginateTypeDef",
     "ListS3BucketsResponseTypeDef",
-    "UpdateBackendConfigRequestRequestTypeDef",
     "UpdateBackendConfigResponseTypeDef",
+    "UpdateBackendConfigRequestRequestTypeDef",
+    "BackendAPIResourceConfigOutputTypeDef",
     "BackendAPIResourceConfigTypeDef",
+    "CreateBackendAuthOAuthConfigOutputTypeDef",
     "CreateBackendAuthOAuthConfigTypeDef",
     "UpdateBackendAuthOAuthConfigTypeDef",
-    "CreateBackendStorageRequestRequestTypeDef",
     "GetBackendStorageResponseTypeDef",
+    "CreateBackendStorageRequestRequestTypeDef",
     "UpdateBackendStorageRequestRequestTypeDef",
+    "GetBackendAPIResponseTypeDef",
     "CreateBackendAPIRequestRequestTypeDef",
     "DeleteBackendAPIRequestRequestTypeDef",
     "GetBackendAPIRequestRequestTypeDef",
-    "GetBackendAPIResponseTypeDef",
     "UpdateBackendAPIRequestRequestTypeDef",
+    "CreateBackendAuthUserPoolConfigOutputTypeDef",
     "CreateBackendAuthUserPoolConfigTypeDef",
     "UpdateBackendAuthUserPoolConfigTypeDef",
+    "CreateBackendAuthResourceConfigOutputTypeDef",
     "CreateBackendAuthResourceConfigTypeDef",
     "UpdateBackendAuthResourceConfigTypeDef",
-    "CreateBackendAuthRequestRequestTypeDef",
     "GetBackendAuthResponseTypeDef",
+    "CreateBackendAuthRequestRequestTypeDef",
     "UpdateBackendAuthRequestRequestTypeDef",
 )
 
+BackendAPIAppSyncAuthSettingsOutputTypeDef = TypedDict(
+    "BackendAPIAppSyncAuthSettingsOutputTypeDef",
+    {
+        "CognitoUserPoolId": str,
+        "Description": str,
+        "ExpirationTime": float,
+        "OpenIDAuthTTL": str,
+        "OpenIDClientId": str,
+        "OpenIDIatTTL": str,
+        "OpenIDIssueURL": str,
+        "OpenIDProviderName": str,
+    },
+    total=False,
+)
+
 BackendAPIAppSyncAuthSettingsTypeDef = TypedDict(
     "BackendAPIAppSyncAuthSettingsTypeDef",
     {
         "CognitoUserPoolId": str,
         "Description": str,
         "ExpirationTime": float,
         "OpenIDAuthTTL": str,
@@ -153,33 +188,61 @@
         "OpenIDIatTTL": str,
         "OpenIDIssueURL": str,
         "OpenIDProviderName": str,
     },
     total=False,
 )
 
+BackendAPIConflictResolutionOutputTypeDef = TypedDict(
+    "BackendAPIConflictResolutionOutputTypeDef",
+    {
+        "ResolutionStrategy": ResolutionStrategyType,
+    },
+    total=False,
+)
+
 BackendAPIConflictResolutionTypeDef = TypedDict(
     "BackendAPIConflictResolutionTypeDef",
     {
         "ResolutionStrategy": ResolutionStrategyType,
     },
     total=False,
 )
 
+BackendAuthAppleProviderConfigOutputTypeDef = TypedDict(
+    "BackendAuthAppleProviderConfigOutputTypeDef",
+    {
+        "ClientId": str,
+        "KeyId": str,
+        "PrivateKey": str,
+        "TeamId": str,
+    },
+    total=False,
+)
+
 BackendAuthAppleProviderConfigTypeDef = TypedDict(
     "BackendAuthAppleProviderConfigTypeDef",
     {
         "ClientId": str,
         "KeyId": str,
         "PrivateKey": str,
         "TeamId": str,
     },
     total=False,
 )
 
+BackendAuthSocialProviderConfigOutputTypeDef = TypedDict(
+    "BackendAuthSocialProviderConfigOutputTypeDef",
+    {
+        "ClientId": str,
+        "ClientSecret": str,
+    },
+    total=False,
+)
+
 BackendAuthSocialProviderConfigTypeDef = TypedDict(
     "BackendAuthSocialProviderConfigTypeDef",
     {
         "ClientId": str,
         "ClientSecret": str,
     },
     total=False,
@@ -208,14 +271,35 @@
 
 class BackendJobRespObjTypeDef(
     _RequiredBackendJobRespObjTypeDef, _OptionalBackendJobRespObjTypeDef
 ):
     pass
 
 
+_RequiredBackendStoragePermissionsOutputTypeDef = TypedDict(
+    "_RequiredBackendStoragePermissionsOutputTypeDef",
+    {
+        "Authenticated": List[AuthenticatedElementType],
+    },
+)
+_OptionalBackendStoragePermissionsOutputTypeDef = TypedDict(
+    "_OptionalBackendStoragePermissionsOutputTypeDef",
+    {
+        "UnAuthenticated": List[UnAuthenticatedElementType],
+    },
+    total=False,
+)
+
+
+class BackendStoragePermissionsOutputTypeDef(
+    _RequiredBackendStoragePermissionsOutputTypeDef, _OptionalBackendStoragePermissionsOutputTypeDef
+):
+    pass
+
+
 _RequiredBackendStoragePermissionsTypeDef = TypedDict(
     "_RequiredBackendStoragePermissionsTypeDef",
     {
         "Authenticated": Sequence[AuthenticatedElementType],
     },
 )
 _OptionalBackendStoragePermissionsTypeDef = TypedDict(
@@ -249,14 +333,31 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+EmailSettingsOutputTypeDef = TypedDict(
+    "EmailSettingsOutputTypeDef",
+    {
+        "EmailMessage": str,
+        "EmailSubject": str,
+    },
+    total=False,
+)
+
+SmsSettingsOutputTypeDef = TypedDict(
+    "SmsSettingsOutputTypeDef",
+    {
+        "SmsMessage": str,
+    },
+    total=False,
+)
+
 EmailSettingsTypeDef = TypedDict(
     "EmailSettingsTypeDef",
     {
         "EmailMessage": str,
         "EmailSubject": str,
     },
     total=False,
@@ -266,31 +367,70 @@
     "SmsSettingsTypeDef",
     {
         "SmsMessage": str,
     },
     total=False,
 )
 
+CreateBackendAuthIdentityPoolConfigOutputTypeDef = TypedDict(
+    "CreateBackendAuthIdentityPoolConfigOutputTypeDef",
+    {
+        "IdentityPoolName": str,
+        "UnauthenticatedLogin": bool,
+    },
+)
+
 CreateBackendAuthIdentityPoolConfigTypeDef = TypedDict(
     "CreateBackendAuthIdentityPoolConfigTypeDef",
     {
         "IdentityPoolName": str,
         "UnauthenticatedLogin": bool,
     },
 )
 
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
+    {
+        "MfaTypes": List[MfaTypesElementType],
+        "SmsMessage": str,
+    },
+    total=False,
+)
+
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "MfaTypes": Sequence[MfaTypesElementType],
         "SmsMessage": str,
     },
     total=False,
 )
 
+_RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef",
+    {
+        "MinimumLength": float,
+    },
+)
+_OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef",
+    {
+        "AdditionalConstraints": List[AdditionalConstraintsElementType],
+    },
+    total=False,
+)
+
+
+class CreateBackendAuthPasswordPolicyConfigOutputTypeDef(
+    _RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef,
+    _OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateBackendAuthPasswordPolicyConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthPasswordPolicyConfigTypeDef",
     {
         "MinimumLength": float,
     },
 )
 _OptionalCreateBackendAuthPasswordPolicyConfigTypeDef = TypedDict(
@@ -569,14 +709,25 @@
     {
         "CreationDate": str,
         "Name": str,
     },
     total=False,
 )
 
+LoginAuthConfigReqObjOutputTypeDef = TypedDict(
+    "LoginAuthConfigReqObjOutputTypeDef",
+    {
+        "AwsCognitoIdentityPoolId": str,
+        "AwsCognitoRegion": str,
+        "AwsUserPoolsId": str,
+        "AwsUserPoolsWebClientId": str,
+    },
+    total=False,
+)
+
 LoginAuthConfigReqObjTypeDef = TypedDict(
     "LoginAuthConfigReqObjTypeDef",
     {
         "AwsCognitoIdentityPoolId": str,
         "AwsCognitoRegion": str,
         "AwsUserPoolsId": str,
         "AwsUserPoolsWebClientId": str,
@@ -649,76 +800,96 @@
 
 class UpdateBackendJobRequestRequestTypeDef(
     _RequiredUpdateBackendJobRequestRequestTypeDef, _OptionalUpdateBackendJobRequestRequestTypeDef
 ):
     pass
 
 
+BackendAPIAuthTypeOutputTypeDef = TypedDict(
+    "BackendAPIAuthTypeOutputTypeDef",
+    {
+        "Mode": ModeType,
+        "Settings": BackendAPIAppSyncAuthSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 BackendAPIAuthTypeTypeDef = TypedDict(
     "BackendAPIAuthTypeTypeDef",
     {
         "Mode": ModeType,
         "Settings": BackendAPIAppSyncAuthSettingsTypeDef,
     },
     total=False,
 )
 
+SocialProviderSettingsOutputTypeDef = TypedDict(
+    "SocialProviderSettingsOutputTypeDef",
+    {
+        "Facebook": BackendAuthSocialProviderConfigOutputTypeDef,
+        "Google": BackendAuthSocialProviderConfigOutputTypeDef,
+        "LoginWithAmazon": BackendAuthSocialProviderConfigOutputTypeDef,
+        "SignInWithApple": BackendAuthAppleProviderConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 SocialProviderSettingsTypeDef = TypedDict(
     "SocialProviderSettingsTypeDef",
     {
         "Facebook": BackendAuthSocialProviderConfigTypeDef,
         "Google": BackendAuthSocialProviderConfigTypeDef,
         "LoginWithAmazon": BackendAuthSocialProviderConfigTypeDef,
         "SignInWithApple": BackendAuthAppleProviderConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateBackendStorageResourceConfigTypeDef = TypedDict(
-    "_RequiredCreateBackendStorageResourceConfigTypeDef",
+_RequiredGetBackendStorageResourceConfigTypeDef = TypedDict(
+    "_RequiredGetBackendStorageResourceConfigTypeDef",
     {
-        "Permissions": BackendStoragePermissionsTypeDef,
+        "Imported": bool,
         "ServiceName": Literal["S3"],
     },
 )
-_OptionalCreateBackendStorageResourceConfigTypeDef = TypedDict(
-    "_OptionalCreateBackendStorageResourceConfigTypeDef",
+_OptionalGetBackendStorageResourceConfigTypeDef = TypedDict(
+    "_OptionalGetBackendStorageResourceConfigTypeDef",
     {
         "BucketName": str,
+        "Permissions": BackendStoragePermissionsOutputTypeDef,
     },
     total=False,
 )
 
 
-class CreateBackendStorageResourceConfigTypeDef(
-    _RequiredCreateBackendStorageResourceConfigTypeDef,
-    _OptionalCreateBackendStorageResourceConfigTypeDef,
+class GetBackendStorageResourceConfigTypeDef(
+    _RequiredGetBackendStorageResourceConfigTypeDef, _OptionalGetBackendStorageResourceConfigTypeDef
 ):
     pass
 
 
-_RequiredGetBackendStorageResourceConfigTypeDef = TypedDict(
-    "_RequiredGetBackendStorageResourceConfigTypeDef",
+_RequiredCreateBackendStorageResourceConfigTypeDef = TypedDict(
+    "_RequiredCreateBackendStorageResourceConfigTypeDef",
     {
-        "Imported": bool,
+        "Permissions": BackendStoragePermissionsTypeDef,
         "ServiceName": Literal["S3"],
     },
 )
-_OptionalGetBackendStorageResourceConfigTypeDef = TypedDict(
-    "_OptionalGetBackendStorageResourceConfigTypeDef",
+_OptionalCreateBackendStorageResourceConfigTypeDef = TypedDict(
+    "_OptionalCreateBackendStorageResourceConfigTypeDef",
     {
         "BucketName": str,
-        "Permissions": BackendStoragePermissionsTypeDef,
     },
     total=False,
 )
 
 
-class GetBackendStorageResourceConfigTypeDef(
-    _RequiredGetBackendStorageResourceConfigTypeDef, _OptionalGetBackendStorageResourceConfigTypeDef
+class CreateBackendStorageResourceConfigTypeDef(
+    _RequiredCreateBackendStorageResourceConfigTypeDef,
+    _OptionalCreateBackendStorageResourceConfigTypeDef,
 ):
     pass
 
 
 UpdateBackendStorageResourceConfigTypeDef = TypedDict(
     "UpdateBackendStorageResourceConfigTypeDef",
     {
@@ -1034,14 +1205,60 @@
         "BackendEnvironmentName": str,
         "JobId": str,
         "Status": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateBackendAuthForgotPasswordConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthForgotPasswordConfigOutputTypeDef",
+    {
+        "DeliveryMethod": DeliveryMethodType,
+    },
+)
+_OptionalCreateBackendAuthForgotPasswordConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthForgotPasswordConfigOutputTypeDef",
+    {
+        "EmailSettings": EmailSettingsOutputTypeDef,
+        "SmsSettings": SmsSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateBackendAuthForgotPasswordConfigOutputTypeDef(
+    _RequiredCreateBackendAuthForgotPasswordConfigOutputTypeDef,
+    _OptionalCreateBackendAuthForgotPasswordConfigOutputTypeDef,
+):
+    pass
+
+
+_RequiredCreateBackendAuthVerificationMessageConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthVerificationMessageConfigOutputTypeDef",
+    {
+        "DeliveryMethod": DeliveryMethodType,
+    },
+)
+_OptionalCreateBackendAuthVerificationMessageConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthVerificationMessageConfigOutputTypeDef",
+    {
+        "EmailSettings": EmailSettingsOutputTypeDef,
+        "SmsSettings": SmsSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateBackendAuthVerificationMessageConfigOutputTypeDef(
+    _RequiredCreateBackendAuthVerificationMessageConfigOutputTypeDef,
+    _OptionalCreateBackendAuthVerificationMessageConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateBackendAuthForgotPasswordConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthForgotPasswordConfigTypeDef",
     {
         "DeliveryMethod": DeliveryMethodType,
     },
 )
 _OptionalCreateBackendAuthForgotPasswordConfigTypeDef = TypedDict(
@@ -1113,14 +1330,36 @@
 class UpdateBackendAuthVerificationMessageConfigTypeDef(
     _RequiredUpdateBackendAuthVerificationMessageConfigTypeDef,
     _OptionalUpdateBackendAuthVerificationMessageConfigTypeDef,
 ):
     pass
 
 
+_RequiredCreateBackendAuthMFAConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthMFAConfigOutputTypeDef",
+    {
+        "MFAMode": MFAModeType,
+    },
+)
+_OptionalCreateBackendAuthMFAConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthMFAConfigOutputTypeDef",
+    {
+        "Settings": SettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateBackendAuthMFAConfigOutputTypeDef(
+    _RequiredCreateBackendAuthMFAConfigOutputTypeDef,
+    _OptionalCreateBackendAuthMFAConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateBackendAuthMFAConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthMFAConfigTypeDef",
     {
         "MFAMode": MFAModeType,
     },
 )
 _OptionalCreateBackendAuthMFAConfigTypeDef = TypedDict(
@@ -1178,14 +1417,25 @@
     {
         "Buckets": List[S3BucketInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateBackendConfigResponseTypeDef = TypedDict(
+    "UpdateBackendConfigResponseTypeDef",
+    {
+        "AppId": str,
+        "BackendManagerAppId": str,
+        "Error": str,
+        "LoginAuthConfig": LoginAuthConfigReqObjOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateBackendConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBackendConfigRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 _OptionalUpdateBackendConfigRequestRequestTypeDef = TypedDict(
@@ -1200,23 +1450,25 @@
 class UpdateBackendConfigRequestRequestTypeDef(
     _RequiredUpdateBackendConfigRequestRequestTypeDef,
     _OptionalUpdateBackendConfigRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateBackendConfigResponseTypeDef = TypedDict(
-    "UpdateBackendConfigResponseTypeDef",
+BackendAPIResourceConfigOutputTypeDef = TypedDict(
+    "BackendAPIResourceConfigOutputTypeDef",
     {
-        "AppId": str,
-        "BackendManagerAppId": str,
-        "Error": str,
-        "LoginAuthConfig": LoginAuthConfigReqObjTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AdditionalAuthTypes": List[BackendAPIAuthTypeOutputTypeDef],
+        "ApiName": str,
+        "ConflictResolution": BackendAPIConflictResolutionOutputTypeDef,
+        "DefaultAuthType": BackendAPIAuthTypeOutputTypeDef,
+        "Service": str,
+        "TransformSchema": str,
     },
+    total=False,
 )
 
 BackendAPIResourceConfigTypeDef = TypedDict(
     "BackendAPIResourceConfigTypeDef",
     {
         "AdditionalAuthTypes": Sequence[BackendAPIAuthTypeTypeDef],
         "ApiName": str,
@@ -1224,14 +1476,40 @@
         "DefaultAuthType": BackendAPIAuthTypeTypeDef,
         "Service": str,
         "TransformSchema": str,
     },
     total=False,
 )
 
+_RequiredCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthOAuthConfigOutputTypeDef",
+    {
+        "OAuthGrantType": OAuthGrantTypeType,
+        "OAuthScopes": List[OAuthScopesElementType],
+        "RedirectSignInURIs": List[str],
+        "RedirectSignOutURIs": List[str],
+    },
+)
+_OptionalCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthOAuthConfigOutputTypeDef",
+    {
+        "DomainPrefix": str,
+        "SocialProviderSettings": SocialProviderSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateBackendAuthOAuthConfigOutputTypeDef(
+    _RequiredCreateBackendAuthOAuthConfigOutputTypeDef,
+    _OptionalCreateBackendAuthOAuthConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateBackendAuthOAuthConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthOAuthConfigTypeDef",
     {
         "OAuthGrantType": OAuthGrantTypeType,
         "OAuthScopes": Sequence[OAuthScopesElementType],
         "RedirectSignInURIs": Sequence[str],
         "RedirectSignOutURIs": Sequence[str],
@@ -1262,45 +1540,57 @@
         "RedirectSignInURIs": Sequence[str],
         "RedirectSignOutURIs": Sequence[str],
         "SocialProviderSettings": SocialProviderSettingsTypeDef,
     },
     total=False,
 )
 
-CreateBackendStorageRequestRequestTypeDef = TypedDict(
-    "CreateBackendStorageRequestRequestTypeDef",
+GetBackendStorageResponseTypeDef = TypedDict(
+    "GetBackendStorageResponseTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": CreateBackendStorageResourceConfigTypeDef,
+        "ResourceConfig": GetBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBackendStorageResponseTypeDef = TypedDict(
-    "GetBackendStorageResponseTypeDef",
+CreateBackendStorageRequestRequestTypeDef = TypedDict(
+    "CreateBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": GetBackendStorageResourceConfigTypeDef,
+        "ResourceConfig": CreateBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBackendStorageRequestRequestTypeDef = TypedDict(
     "UpdateBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": UpdateBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
     },
 )
 
+GetBackendAPIResponseTypeDef = TypedDict(
+    "GetBackendAPIResponseTypeDef",
+    {
+        "AppId": str,
+        "BackendEnvironmentName": str,
+        "Error": str,
+        "ResourceConfig": BackendAPIResourceConfigOutputTypeDef,
+        "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateBackendAPIRequestRequestTypeDef = TypedDict(
     "CreateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
         "ResourceName": str,
@@ -1349,26 +1639,14 @@
 
 class GetBackendAPIRequestRequestTypeDef(
     _RequiredGetBackendAPIRequestRequestTypeDef, _OptionalGetBackendAPIRequestRequestTypeDef
 ):
     pass
 
 
-GetBackendAPIResponseTypeDef = TypedDict(
-    "GetBackendAPIResponseTypeDef",
-    {
-        "AppId": str,
-        "BackendEnvironmentName": str,
-        "Error": str,
-        "ResourceConfig": BackendAPIResourceConfigTypeDef,
-        "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateBackendAPIRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceName": str,
     },
@@ -1384,14 +1662,42 @@
 
 class UpdateBackendAPIRequestRequestTypeDef(
     _RequiredUpdateBackendAPIRequestRequestTypeDef, _OptionalUpdateBackendAPIRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthUserPoolConfigOutputTypeDef",
+    {
+        "RequiredSignUpAttributes": List[RequiredSignUpAttributesElementType],
+        "SignInMethod": SignInMethodType,
+        "UserPoolName": str,
+    },
+)
+_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef",
+    {
+        "ForgotPassword": CreateBackendAuthForgotPasswordConfigOutputTypeDef,
+        "Mfa": CreateBackendAuthMFAConfigOutputTypeDef,
+        "OAuth": CreateBackendAuthOAuthConfigOutputTypeDef,
+        "PasswordPolicy": CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
+        "VerificationMessage": CreateBackendAuthVerificationMessageConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateBackendAuthUserPoolConfigOutputTypeDef(
+    _RequiredCreateBackendAuthUserPoolConfigOutputTypeDef,
+    _OptionalCreateBackendAuthUserPoolConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateBackendAuthUserPoolConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthUserPoolConfigTypeDef",
     {
         "RequiredSignUpAttributes": Sequence[RequiredSignUpAttributesElementType],
         "SignInMethod": SignInMethodType,
         "UserPoolName": str,
     },
@@ -1423,14 +1729,38 @@
         "OAuth": UpdateBackendAuthOAuthConfigTypeDef,
         "PasswordPolicy": UpdateBackendAuthPasswordPolicyConfigTypeDef,
         "VerificationMessage": UpdateBackendAuthVerificationMessageConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthResourceConfigOutputTypeDef",
+    {
+        "AuthResources": AuthResourcesType,
+        "Service": Literal["COGNITO"],
+        "UserPoolConfigs": CreateBackendAuthUserPoolConfigOutputTypeDef,
+    },
+)
+_OptionalCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthResourceConfigOutputTypeDef",
+    {
+        "IdentityPoolConfigs": CreateBackendAuthIdentityPoolConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateBackendAuthResourceConfigOutputTypeDef(
+    _RequiredCreateBackendAuthResourceConfigOutputTypeDef,
+    _OptionalCreateBackendAuthResourceConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateBackendAuthResourceConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthResourceConfigTypeDef",
     {
         "AuthResources": AuthResourcesType,
         "Service": Literal["COGNITO"],
         "UserPoolConfigs": CreateBackendAuthUserPoolConfigTypeDef,
     },
@@ -1469,33 +1799,33 @@
 
 class UpdateBackendAuthResourceConfigTypeDef(
     _RequiredUpdateBackendAuthResourceConfigTypeDef, _OptionalUpdateBackendAuthResourceConfigTypeDef
 ):
     pass
 
 
-CreateBackendAuthRequestRequestTypeDef = TypedDict(
-    "CreateBackendAuthRequestRequestTypeDef",
+GetBackendAuthResponseTypeDef = TypedDict(
+    "GetBackendAuthResponseTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
+        "Error": str,
+        "ResourceConfig": CreateBackendAuthResourceConfigOutputTypeDef,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBackendAuthResponseTypeDef = TypedDict(
-    "GetBackendAuthResponseTypeDef",
+CreateBackendAuthRequestRequestTypeDef = TypedDict(
+    "CreateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "Error": str,
         "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBackendAuthRequestRequestTypeDef = TypedDict(
     "UpdateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
```

### Comparing `mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend/type_defs.pyi` & `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplifybackend service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsTypeDef
+    from mypy_boto3_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsOutputTypeDef
 
-    data: BackendAPIAppSyncAuthSettingsTypeDef = {...}
+    data: BackendAPIAppSyncAuthSettingsOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AdditionalConstraintsElementType,
@@ -37,26 +37,36 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BackendAPIAppSyncAuthSettingsOutputTypeDef",
     "BackendAPIAppSyncAuthSettingsTypeDef",
+    "BackendAPIConflictResolutionOutputTypeDef",
     "BackendAPIConflictResolutionTypeDef",
+    "BackendAuthAppleProviderConfigOutputTypeDef",
     "BackendAuthAppleProviderConfigTypeDef",
+    "BackendAuthSocialProviderConfigOutputTypeDef",
     "BackendAuthSocialProviderConfigTypeDef",
     "BackendJobRespObjTypeDef",
+    "BackendStoragePermissionsOutputTypeDef",
     "BackendStoragePermissionsTypeDef",
     "CloneBackendRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "EmailSettingsOutputTypeDef",
+    "SmsSettingsOutputTypeDef",
     "EmailSettingsTypeDef",
     "SmsSettingsTypeDef",
+    "CreateBackendAuthIdentityPoolConfigOutputTypeDef",
     "CreateBackendAuthIdentityPoolConfigTypeDef",
+    "SettingsOutputTypeDef",
     "SettingsTypeDef",
+    "CreateBackendAuthPasswordPolicyConfigOutputTypeDef",
     "CreateBackendAuthPasswordPolicyConfigTypeDef",
     "CreateBackendConfigRequestRequestTypeDef",
     "CreateBackendRequestRequestTypeDef",
     "CreateTokenRequestRequestTypeDef",
     "DeleteBackendAuthRequestRequestTypeDef",
     "DeleteBackendRequestRequestTypeDef",
     "DeleteBackendStorageRequestRequestTypeDef",
@@ -70,24 +80,27 @@
     "GetTokenRequestRequestTypeDef",
     "ImportBackendAuthRequestRequestTypeDef",
     "ImportBackendStorageRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListBackendJobsRequestRequestTypeDef",
     "ListS3BucketsRequestRequestTypeDef",
     "S3BucketInfoTypeDef",
+    "LoginAuthConfigReqObjOutputTypeDef",
     "LoginAuthConfigReqObjTypeDef",
     "RemoveAllBackendsRequestRequestTypeDef",
     "RemoveBackendConfigRequestRequestTypeDef",
     "UpdateBackendAuthIdentityPoolConfigTypeDef",
     "UpdateBackendAuthPasswordPolicyConfigTypeDef",
     "UpdateBackendJobRequestRequestTypeDef",
+    "BackendAPIAuthTypeOutputTypeDef",
     "BackendAPIAuthTypeTypeDef",
+    "SocialProviderSettingsOutputTypeDef",
     "SocialProviderSettingsTypeDef",
-    "CreateBackendStorageResourceConfigTypeDef",
     "GetBackendStorageResourceConfigTypeDef",
+    "CreateBackendStorageResourceConfigTypeDef",
     "UpdateBackendStorageResourceConfigTypeDef",
     "CloneBackendResponseTypeDef",
     "CreateBackendAPIResponseTypeDef",
     "CreateBackendAuthResponseTypeDef",
     "CreateBackendConfigResponseTypeDef",
     "CreateBackendResponseTypeDef",
     "CreateBackendStorageResponseTypeDef",
@@ -107,44 +120,66 @@
     "ListBackendJobsResponseTypeDef",
     "RemoveAllBackendsResponseTypeDef",
     "RemoveBackendConfigResponseTypeDef",
     "UpdateBackendAPIResponseTypeDef",
     "UpdateBackendAuthResponseTypeDef",
     "UpdateBackendJobResponseTypeDef",
     "UpdateBackendStorageResponseTypeDef",
+    "CreateBackendAuthForgotPasswordConfigOutputTypeDef",
+    "CreateBackendAuthVerificationMessageConfigOutputTypeDef",
     "CreateBackendAuthForgotPasswordConfigTypeDef",
     "CreateBackendAuthVerificationMessageConfigTypeDef",
     "UpdateBackendAuthForgotPasswordConfigTypeDef",
     "UpdateBackendAuthVerificationMessageConfigTypeDef",
+    "CreateBackendAuthMFAConfigOutputTypeDef",
     "CreateBackendAuthMFAConfigTypeDef",
     "UpdateBackendAuthMFAConfigTypeDef",
     "ListBackendJobsRequestListBackendJobsPaginateTypeDef",
     "ListS3BucketsResponseTypeDef",
-    "UpdateBackendConfigRequestRequestTypeDef",
     "UpdateBackendConfigResponseTypeDef",
+    "UpdateBackendConfigRequestRequestTypeDef",
+    "BackendAPIResourceConfigOutputTypeDef",
     "BackendAPIResourceConfigTypeDef",
+    "CreateBackendAuthOAuthConfigOutputTypeDef",
     "CreateBackendAuthOAuthConfigTypeDef",
     "UpdateBackendAuthOAuthConfigTypeDef",
-    "CreateBackendStorageRequestRequestTypeDef",
     "GetBackendStorageResponseTypeDef",
+    "CreateBackendStorageRequestRequestTypeDef",
     "UpdateBackendStorageRequestRequestTypeDef",
+    "GetBackendAPIResponseTypeDef",
     "CreateBackendAPIRequestRequestTypeDef",
     "DeleteBackendAPIRequestRequestTypeDef",
     "GetBackendAPIRequestRequestTypeDef",
-    "GetBackendAPIResponseTypeDef",
     "UpdateBackendAPIRequestRequestTypeDef",
+    "CreateBackendAuthUserPoolConfigOutputTypeDef",
     "CreateBackendAuthUserPoolConfigTypeDef",
     "UpdateBackendAuthUserPoolConfigTypeDef",
+    "CreateBackendAuthResourceConfigOutputTypeDef",
     "CreateBackendAuthResourceConfigTypeDef",
     "UpdateBackendAuthResourceConfigTypeDef",
-    "CreateBackendAuthRequestRequestTypeDef",
     "GetBackendAuthResponseTypeDef",
+    "CreateBackendAuthRequestRequestTypeDef",
     "UpdateBackendAuthRequestRequestTypeDef",
 )
 
+BackendAPIAppSyncAuthSettingsOutputTypeDef = TypedDict(
+    "BackendAPIAppSyncAuthSettingsOutputTypeDef",
+    {
+        "CognitoUserPoolId": str,
+        "Description": str,
+        "ExpirationTime": float,
+        "OpenIDAuthTTL": str,
+        "OpenIDClientId": str,
+        "OpenIDIatTTL": str,
+        "OpenIDIssueURL": str,
+        "OpenIDProviderName": str,
+    },
+    total=False,
+)
+
 BackendAPIAppSyncAuthSettingsTypeDef = TypedDict(
     "BackendAPIAppSyncAuthSettingsTypeDef",
     {
         "CognitoUserPoolId": str,
         "Description": str,
         "ExpirationTime": float,
         "OpenIDAuthTTL": str,
@@ -152,33 +187,61 @@
         "OpenIDIatTTL": str,
         "OpenIDIssueURL": str,
         "OpenIDProviderName": str,
     },
     total=False,
 )
 
+BackendAPIConflictResolutionOutputTypeDef = TypedDict(
+    "BackendAPIConflictResolutionOutputTypeDef",
+    {
+        "ResolutionStrategy": ResolutionStrategyType,
+    },
+    total=False,
+)
+
 BackendAPIConflictResolutionTypeDef = TypedDict(
     "BackendAPIConflictResolutionTypeDef",
     {
         "ResolutionStrategy": ResolutionStrategyType,
     },
     total=False,
 )
 
+BackendAuthAppleProviderConfigOutputTypeDef = TypedDict(
+    "BackendAuthAppleProviderConfigOutputTypeDef",
+    {
+        "ClientId": str,
+        "KeyId": str,
+        "PrivateKey": str,
+        "TeamId": str,
+    },
+    total=False,
+)
+
 BackendAuthAppleProviderConfigTypeDef = TypedDict(
     "BackendAuthAppleProviderConfigTypeDef",
     {
         "ClientId": str,
         "KeyId": str,
         "PrivateKey": str,
         "TeamId": str,
     },
     total=False,
 )
 
+BackendAuthSocialProviderConfigOutputTypeDef = TypedDict(
+    "BackendAuthSocialProviderConfigOutputTypeDef",
+    {
+        "ClientId": str,
+        "ClientSecret": str,
+    },
+    total=False,
+)
+
 BackendAuthSocialProviderConfigTypeDef = TypedDict(
     "BackendAuthSocialProviderConfigTypeDef",
     {
         "ClientId": str,
         "ClientSecret": str,
     },
     total=False,
@@ -205,14 +268,33 @@
 )
 
 class BackendJobRespObjTypeDef(
     _RequiredBackendJobRespObjTypeDef, _OptionalBackendJobRespObjTypeDef
 ):
     pass
 
+_RequiredBackendStoragePermissionsOutputTypeDef = TypedDict(
+    "_RequiredBackendStoragePermissionsOutputTypeDef",
+    {
+        "Authenticated": List[AuthenticatedElementType],
+    },
+)
+_OptionalBackendStoragePermissionsOutputTypeDef = TypedDict(
+    "_OptionalBackendStoragePermissionsOutputTypeDef",
+    {
+        "UnAuthenticated": List[UnAuthenticatedElementType],
+    },
+    total=False,
+)
+
+class BackendStoragePermissionsOutputTypeDef(
+    _RequiredBackendStoragePermissionsOutputTypeDef, _OptionalBackendStoragePermissionsOutputTypeDef
+):
+    pass
+
 _RequiredBackendStoragePermissionsTypeDef = TypedDict(
     "_RequiredBackendStoragePermissionsTypeDef",
     {
         "Authenticated": Sequence[AuthenticatedElementType],
     },
 )
 _OptionalBackendStoragePermissionsTypeDef = TypedDict(
@@ -244,14 +326,31 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+EmailSettingsOutputTypeDef = TypedDict(
+    "EmailSettingsOutputTypeDef",
+    {
+        "EmailMessage": str,
+        "EmailSubject": str,
+    },
+    total=False,
+)
+
+SmsSettingsOutputTypeDef = TypedDict(
+    "SmsSettingsOutputTypeDef",
+    {
+        "SmsMessage": str,
+    },
+    total=False,
+)
+
 EmailSettingsTypeDef = TypedDict(
     "EmailSettingsTypeDef",
     {
         "EmailMessage": str,
         "EmailSubject": str,
     },
     total=False,
@@ -261,31 +360,68 @@
     "SmsSettingsTypeDef",
     {
         "SmsMessage": str,
     },
     total=False,
 )
 
+CreateBackendAuthIdentityPoolConfigOutputTypeDef = TypedDict(
+    "CreateBackendAuthIdentityPoolConfigOutputTypeDef",
+    {
+        "IdentityPoolName": str,
+        "UnauthenticatedLogin": bool,
+    },
+)
+
 CreateBackendAuthIdentityPoolConfigTypeDef = TypedDict(
     "CreateBackendAuthIdentityPoolConfigTypeDef",
     {
         "IdentityPoolName": str,
         "UnauthenticatedLogin": bool,
     },
 )
 
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
+    {
+        "MfaTypes": List[MfaTypesElementType],
+        "SmsMessage": str,
+    },
+    total=False,
+)
+
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "MfaTypes": Sequence[MfaTypesElementType],
         "SmsMessage": str,
     },
     total=False,
 )
 
+_RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef",
+    {
+        "MinimumLength": float,
+    },
+)
+_OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef",
+    {
+        "AdditionalConstraints": List[AdditionalConstraintsElementType],
+    },
+    total=False,
+)
+
+class CreateBackendAuthPasswordPolicyConfigOutputTypeDef(
+    _RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef,
+    _OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef,
+):
+    pass
+
 _RequiredCreateBackendAuthPasswordPolicyConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthPasswordPolicyConfigTypeDef",
     {
         "MinimumLength": float,
     },
 )
 _OptionalCreateBackendAuthPasswordPolicyConfigTypeDef = TypedDict(
@@ -550,14 +686,25 @@
     {
         "CreationDate": str,
         "Name": str,
     },
     total=False,
 )
 
+LoginAuthConfigReqObjOutputTypeDef = TypedDict(
+    "LoginAuthConfigReqObjOutputTypeDef",
+    {
+        "AwsCognitoIdentityPoolId": str,
+        "AwsCognitoRegion": str,
+        "AwsUserPoolsId": str,
+        "AwsUserPoolsWebClientId": str,
+    },
+    total=False,
+)
+
 LoginAuthConfigReqObjTypeDef = TypedDict(
     "LoginAuthConfigReqObjTypeDef",
     {
         "AwsCognitoIdentityPoolId": str,
         "AwsCognitoRegion": str,
         "AwsUserPoolsId": str,
         "AwsUserPoolsWebClientId": str,
@@ -626,73 +773,93 @@
 )
 
 class UpdateBackendJobRequestRequestTypeDef(
     _RequiredUpdateBackendJobRequestRequestTypeDef, _OptionalUpdateBackendJobRequestRequestTypeDef
 ):
     pass
 
+BackendAPIAuthTypeOutputTypeDef = TypedDict(
+    "BackendAPIAuthTypeOutputTypeDef",
+    {
+        "Mode": ModeType,
+        "Settings": BackendAPIAppSyncAuthSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
 BackendAPIAuthTypeTypeDef = TypedDict(
     "BackendAPIAuthTypeTypeDef",
     {
         "Mode": ModeType,
         "Settings": BackendAPIAppSyncAuthSettingsTypeDef,
     },
     total=False,
 )
 
+SocialProviderSettingsOutputTypeDef = TypedDict(
+    "SocialProviderSettingsOutputTypeDef",
+    {
+        "Facebook": BackendAuthSocialProviderConfigOutputTypeDef,
+        "Google": BackendAuthSocialProviderConfigOutputTypeDef,
+        "LoginWithAmazon": BackendAuthSocialProviderConfigOutputTypeDef,
+        "SignInWithApple": BackendAuthAppleProviderConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 SocialProviderSettingsTypeDef = TypedDict(
     "SocialProviderSettingsTypeDef",
     {
         "Facebook": BackendAuthSocialProviderConfigTypeDef,
         "Google": BackendAuthSocialProviderConfigTypeDef,
         "LoginWithAmazon": BackendAuthSocialProviderConfigTypeDef,
         "SignInWithApple": BackendAuthAppleProviderConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateBackendStorageResourceConfigTypeDef = TypedDict(
-    "_RequiredCreateBackendStorageResourceConfigTypeDef",
+_RequiredGetBackendStorageResourceConfigTypeDef = TypedDict(
+    "_RequiredGetBackendStorageResourceConfigTypeDef",
     {
-        "Permissions": BackendStoragePermissionsTypeDef,
+        "Imported": bool,
         "ServiceName": Literal["S3"],
     },
 )
-_OptionalCreateBackendStorageResourceConfigTypeDef = TypedDict(
-    "_OptionalCreateBackendStorageResourceConfigTypeDef",
+_OptionalGetBackendStorageResourceConfigTypeDef = TypedDict(
+    "_OptionalGetBackendStorageResourceConfigTypeDef",
     {
         "BucketName": str,
+        "Permissions": BackendStoragePermissionsOutputTypeDef,
     },
     total=False,
 )
 
-class CreateBackendStorageResourceConfigTypeDef(
-    _RequiredCreateBackendStorageResourceConfigTypeDef,
-    _OptionalCreateBackendStorageResourceConfigTypeDef,
+class GetBackendStorageResourceConfigTypeDef(
+    _RequiredGetBackendStorageResourceConfigTypeDef, _OptionalGetBackendStorageResourceConfigTypeDef
 ):
     pass
 
-_RequiredGetBackendStorageResourceConfigTypeDef = TypedDict(
-    "_RequiredGetBackendStorageResourceConfigTypeDef",
+_RequiredCreateBackendStorageResourceConfigTypeDef = TypedDict(
+    "_RequiredCreateBackendStorageResourceConfigTypeDef",
     {
-        "Imported": bool,
+        "Permissions": BackendStoragePermissionsTypeDef,
         "ServiceName": Literal["S3"],
     },
 )
-_OptionalGetBackendStorageResourceConfigTypeDef = TypedDict(
-    "_OptionalGetBackendStorageResourceConfigTypeDef",
+_OptionalCreateBackendStorageResourceConfigTypeDef = TypedDict(
+    "_OptionalCreateBackendStorageResourceConfigTypeDef",
     {
         "BucketName": str,
-        "Permissions": BackendStoragePermissionsTypeDef,
     },
     total=False,
 )
 
-class GetBackendStorageResourceConfigTypeDef(
-    _RequiredGetBackendStorageResourceConfigTypeDef, _OptionalGetBackendStorageResourceConfigTypeDef
+class CreateBackendStorageResourceConfigTypeDef(
+    _RequiredCreateBackendStorageResourceConfigTypeDef,
+    _OptionalCreateBackendStorageResourceConfigTypeDef,
 ):
     pass
 
 UpdateBackendStorageResourceConfigTypeDef = TypedDict(
     "UpdateBackendStorageResourceConfigTypeDef",
     {
         "Permissions": BackendStoragePermissionsTypeDef,
@@ -1007,14 +1174,56 @@
         "BackendEnvironmentName": str,
         "JobId": str,
         "Status": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateBackendAuthForgotPasswordConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthForgotPasswordConfigOutputTypeDef",
+    {
+        "DeliveryMethod": DeliveryMethodType,
+    },
+)
+_OptionalCreateBackendAuthForgotPasswordConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthForgotPasswordConfigOutputTypeDef",
+    {
+        "EmailSettings": EmailSettingsOutputTypeDef,
+        "SmsSettings": SmsSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class CreateBackendAuthForgotPasswordConfigOutputTypeDef(
+    _RequiredCreateBackendAuthForgotPasswordConfigOutputTypeDef,
+    _OptionalCreateBackendAuthForgotPasswordConfigOutputTypeDef,
+):
+    pass
+
+_RequiredCreateBackendAuthVerificationMessageConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthVerificationMessageConfigOutputTypeDef",
+    {
+        "DeliveryMethod": DeliveryMethodType,
+    },
+)
+_OptionalCreateBackendAuthVerificationMessageConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthVerificationMessageConfigOutputTypeDef",
+    {
+        "EmailSettings": EmailSettingsOutputTypeDef,
+        "SmsSettings": SmsSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class CreateBackendAuthVerificationMessageConfigOutputTypeDef(
+    _RequiredCreateBackendAuthVerificationMessageConfigOutputTypeDef,
+    _OptionalCreateBackendAuthVerificationMessageConfigOutputTypeDef,
+):
+    pass
+
 _RequiredCreateBackendAuthForgotPasswordConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthForgotPasswordConfigTypeDef",
     {
         "DeliveryMethod": DeliveryMethodType,
     },
 )
 _OptionalCreateBackendAuthForgotPasswordConfigTypeDef = TypedDict(
@@ -1080,14 +1289,34 @@
 
 class UpdateBackendAuthVerificationMessageConfigTypeDef(
     _RequiredUpdateBackendAuthVerificationMessageConfigTypeDef,
     _OptionalUpdateBackendAuthVerificationMessageConfigTypeDef,
 ):
     pass
 
+_RequiredCreateBackendAuthMFAConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthMFAConfigOutputTypeDef",
+    {
+        "MFAMode": MFAModeType,
+    },
+)
+_OptionalCreateBackendAuthMFAConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthMFAConfigOutputTypeDef",
+    {
+        "Settings": SettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class CreateBackendAuthMFAConfigOutputTypeDef(
+    _RequiredCreateBackendAuthMFAConfigOutputTypeDef,
+    _OptionalCreateBackendAuthMFAConfigOutputTypeDef,
+):
+    pass
+
 _RequiredCreateBackendAuthMFAConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthMFAConfigTypeDef",
     {
         "MFAMode": MFAModeType,
     },
 )
 _OptionalCreateBackendAuthMFAConfigTypeDef = TypedDict(
@@ -1141,14 +1370,25 @@
     {
         "Buckets": List[S3BucketInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateBackendConfigResponseTypeDef = TypedDict(
+    "UpdateBackendConfigResponseTypeDef",
+    {
+        "AppId": str,
+        "BackendManagerAppId": str,
+        "Error": str,
+        "LoginAuthConfig": LoginAuthConfigReqObjOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateBackendConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBackendConfigRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 _OptionalUpdateBackendConfigRequestRequestTypeDef = TypedDict(
@@ -1161,23 +1401,25 @@
 
 class UpdateBackendConfigRequestRequestTypeDef(
     _RequiredUpdateBackendConfigRequestRequestTypeDef,
     _OptionalUpdateBackendConfigRequestRequestTypeDef,
 ):
     pass
 
-UpdateBackendConfigResponseTypeDef = TypedDict(
-    "UpdateBackendConfigResponseTypeDef",
+BackendAPIResourceConfigOutputTypeDef = TypedDict(
+    "BackendAPIResourceConfigOutputTypeDef",
     {
-        "AppId": str,
-        "BackendManagerAppId": str,
-        "Error": str,
-        "LoginAuthConfig": LoginAuthConfigReqObjTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AdditionalAuthTypes": List[BackendAPIAuthTypeOutputTypeDef],
+        "ApiName": str,
+        "ConflictResolution": BackendAPIConflictResolutionOutputTypeDef,
+        "DefaultAuthType": BackendAPIAuthTypeOutputTypeDef,
+        "Service": str,
+        "TransformSchema": str,
     },
+    total=False,
 )
 
 BackendAPIResourceConfigTypeDef = TypedDict(
     "BackendAPIResourceConfigTypeDef",
     {
         "AdditionalAuthTypes": Sequence[BackendAPIAuthTypeTypeDef],
         "ApiName": str,
@@ -1185,14 +1427,38 @@
         "DefaultAuthType": BackendAPIAuthTypeTypeDef,
         "Service": str,
         "TransformSchema": str,
     },
     total=False,
 )
 
+_RequiredCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthOAuthConfigOutputTypeDef",
+    {
+        "OAuthGrantType": OAuthGrantTypeType,
+        "OAuthScopes": List[OAuthScopesElementType],
+        "RedirectSignInURIs": List[str],
+        "RedirectSignOutURIs": List[str],
+    },
+)
+_OptionalCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthOAuthConfigOutputTypeDef",
+    {
+        "DomainPrefix": str,
+        "SocialProviderSettings": SocialProviderSettingsOutputTypeDef,
+    },
+    total=False,
+)
+
+class CreateBackendAuthOAuthConfigOutputTypeDef(
+    _RequiredCreateBackendAuthOAuthConfigOutputTypeDef,
+    _OptionalCreateBackendAuthOAuthConfigOutputTypeDef,
+):
+    pass
+
 _RequiredCreateBackendAuthOAuthConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthOAuthConfigTypeDef",
     {
         "OAuthGrantType": OAuthGrantTypeType,
         "OAuthScopes": Sequence[OAuthScopesElementType],
         "RedirectSignInURIs": Sequence[str],
         "RedirectSignOutURIs": Sequence[str],
@@ -1221,45 +1487,57 @@
         "RedirectSignInURIs": Sequence[str],
         "RedirectSignOutURIs": Sequence[str],
         "SocialProviderSettings": SocialProviderSettingsTypeDef,
     },
     total=False,
 )
 
-CreateBackendStorageRequestRequestTypeDef = TypedDict(
-    "CreateBackendStorageRequestRequestTypeDef",
+GetBackendStorageResponseTypeDef = TypedDict(
+    "GetBackendStorageResponseTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": CreateBackendStorageResourceConfigTypeDef,
+        "ResourceConfig": GetBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBackendStorageResponseTypeDef = TypedDict(
-    "GetBackendStorageResponseTypeDef",
+CreateBackendStorageRequestRequestTypeDef = TypedDict(
+    "CreateBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": GetBackendStorageResourceConfigTypeDef,
+        "ResourceConfig": CreateBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBackendStorageRequestRequestTypeDef = TypedDict(
     "UpdateBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": UpdateBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
     },
 )
 
+GetBackendAPIResponseTypeDef = TypedDict(
+    "GetBackendAPIResponseTypeDef",
+    {
+        "AppId": str,
+        "BackendEnvironmentName": str,
+        "Error": str,
+        "ResourceConfig": BackendAPIResourceConfigOutputTypeDef,
+        "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateBackendAPIRequestRequestTypeDef = TypedDict(
     "CreateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
         "ResourceName": str,
@@ -1304,26 +1582,14 @@
 )
 
 class GetBackendAPIRequestRequestTypeDef(
     _RequiredGetBackendAPIRequestRequestTypeDef, _OptionalGetBackendAPIRequestRequestTypeDef
 ):
     pass
 
-GetBackendAPIResponseTypeDef = TypedDict(
-    "GetBackendAPIResponseTypeDef",
-    {
-        "AppId": str,
-        "BackendEnvironmentName": str,
-        "Error": str,
-        "ResourceConfig": BackendAPIResourceConfigTypeDef,
-        "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateBackendAPIRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceName": str,
     },
@@ -1337,14 +1603,40 @@
 )
 
 class UpdateBackendAPIRequestRequestTypeDef(
     _RequiredUpdateBackendAPIRequestRequestTypeDef, _OptionalUpdateBackendAPIRequestRequestTypeDef
 ):
     pass
 
+_RequiredCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthUserPoolConfigOutputTypeDef",
+    {
+        "RequiredSignUpAttributes": List[RequiredSignUpAttributesElementType],
+        "SignInMethod": SignInMethodType,
+        "UserPoolName": str,
+    },
+)
+_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef",
+    {
+        "ForgotPassword": CreateBackendAuthForgotPasswordConfigOutputTypeDef,
+        "Mfa": CreateBackendAuthMFAConfigOutputTypeDef,
+        "OAuth": CreateBackendAuthOAuthConfigOutputTypeDef,
+        "PasswordPolicy": CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
+        "VerificationMessage": CreateBackendAuthVerificationMessageConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class CreateBackendAuthUserPoolConfigOutputTypeDef(
+    _RequiredCreateBackendAuthUserPoolConfigOutputTypeDef,
+    _OptionalCreateBackendAuthUserPoolConfigOutputTypeDef,
+):
+    pass
+
 _RequiredCreateBackendAuthUserPoolConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthUserPoolConfigTypeDef",
     {
         "RequiredSignUpAttributes": Sequence[RequiredSignUpAttributesElementType],
         "SignInMethod": SignInMethodType,
         "UserPoolName": str,
     },
@@ -1374,14 +1666,36 @@
         "OAuth": UpdateBackendAuthOAuthConfigTypeDef,
         "PasswordPolicy": UpdateBackendAuthPasswordPolicyConfigTypeDef,
         "VerificationMessage": UpdateBackendAuthVerificationMessageConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
+    "_RequiredCreateBackendAuthResourceConfigOutputTypeDef",
+    {
+        "AuthResources": AuthResourcesType,
+        "Service": Literal["COGNITO"],
+        "UserPoolConfigs": CreateBackendAuthUserPoolConfigOutputTypeDef,
+    },
+)
+_OptionalCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
+    "_OptionalCreateBackendAuthResourceConfigOutputTypeDef",
+    {
+        "IdentityPoolConfigs": CreateBackendAuthIdentityPoolConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class CreateBackendAuthResourceConfigOutputTypeDef(
+    _RequiredCreateBackendAuthResourceConfigOutputTypeDef,
+    _OptionalCreateBackendAuthResourceConfigOutputTypeDef,
+):
+    pass
+
 _RequiredCreateBackendAuthResourceConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthResourceConfigTypeDef",
     {
         "AuthResources": AuthResourcesType,
         "Service": Literal["COGNITO"],
         "UserPoolConfigs": CreateBackendAuthUserPoolConfigTypeDef,
     },
@@ -1416,33 +1730,33 @@
 )
 
 class UpdateBackendAuthResourceConfigTypeDef(
     _RequiredUpdateBackendAuthResourceConfigTypeDef, _OptionalUpdateBackendAuthResourceConfigTypeDef
 ):
     pass
 
-CreateBackendAuthRequestRequestTypeDef = TypedDict(
-    "CreateBackendAuthRequestRequestTypeDef",
+GetBackendAuthResponseTypeDef = TypedDict(
+    "GetBackendAuthResponseTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
+        "Error": str,
+        "ResourceConfig": CreateBackendAuthResourceConfigOutputTypeDef,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBackendAuthResponseTypeDef = TypedDict(
-    "GetBackendAuthResponseTypeDef",
+CreateBackendAuthRequestRequestTypeDef = TypedDict(
+    "CreateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "Error": str,
         "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBackendAuthRequestRequestTypeDef = TypedDict(
     "UpdateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
```

### Comparing `mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend.egg-info/PKG-INFO` & `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifybackend
-Version: 1.28.0
-Summary: Type annotations for boto3.AmplifyBackend 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AmplifyBackend 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-amplifybackend"></a>
 
 # mypy-boto3-amplifybackend
 
 [![PyPI - mypy-boto3-amplifybackend](https://img.shields.io/pypi/v/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplifybackend?color=blue)](https://pypistats.org/packages/mypy-boto3-amplifybackend)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifybackend)](https://pepy.tech/project/mypy-boto3-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyBackend 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[boto3.AmplifyBackend 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,26 +336,36 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplifybackend.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifybackend.type_defs import (
+    BackendAPIAppSyncAuthSettingsOutputTypeDef,
     BackendAPIAppSyncAuthSettingsTypeDef,
+    BackendAPIConflictResolutionOutputTypeDef,
     BackendAPIConflictResolutionTypeDef,
+    BackendAuthAppleProviderConfigOutputTypeDef,
     BackendAuthAppleProviderConfigTypeDef,
+    BackendAuthSocialProviderConfigOutputTypeDef,
     BackendAuthSocialProviderConfigTypeDef,
     BackendJobRespObjTypeDef,
+    BackendStoragePermissionsOutputTypeDef,
     BackendStoragePermissionsTypeDef,
     CloneBackendRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    EmailSettingsOutputTypeDef,
+    SmsSettingsOutputTypeDef,
     EmailSettingsTypeDef,
     SmsSettingsTypeDef,
+    CreateBackendAuthIdentityPoolConfigOutputTypeDef,
     CreateBackendAuthIdentityPoolConfigTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
+    CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
     CreateBackendAuthPasswordPolicyConfigTypeDef,
     CreateBackendConfigRequestRequestTypeDef,
     CreateBackendRequestRequestTypeDef,
     CreateTokenRequestRequestTypeDef,
     DeleteBackendAuthRequestRequestTypeDef,
     DeleteBackendRequestRequestTypeDef,
     DeleteBackendStorageRequestRequestTypeDef,
@@ -369,24 +379,27 @@
     GetTokenRequestRequestTypeDef,
     ImportBackendAuthRequestRequestTypeDef,
     ImportBackendStorageRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListBackendJobsRequestRequestTypeDef,
     ListS3BucketsRequestRequestTypeDef,
     S3BucketInfoTypeDef,
+    LoginAuthConfigReqObjOutputTypeDef,
     LoginAuthConfigReqObjTypeDef,
     RemoveAllBackendsRequestRequestTypeDef,
     RemoveBackendConfigRequestRequestTypeDef,
     UpdateBackendAuthIdentityPoolConfigTypeDef,
     UpdateBackendAuthPasswordPolicyConfigTypeDef,
     UpdateBackendJobRequestRequestTypeDef,
+    BackendAPIAuthTypeOutputTypeDef,
     BackendAPIAuthTypeTypeDef,
+    SocialProviderSettingsOutputTypeDef,
     SocialProviderSettingsTypeDef,
-    CreateBackendStorageResourceConfigTypeDef,
     GetBackendStorageResourceConfigTypeDef,
+    CreateBackendStorageResourceConfigTypeDef,
     UpdateBackendStorageResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResponseTypeDef,
@@ -406,46 +419,53 @@
     ListBackendJobsResponseTypeDef,
     RemoveAllBackendsResponseTypeDef,
     RemoveBackendConfigResponseTypeDef,
     UpdateBackendAPIResponseTypeDef,
     UpdateBackendAuthResponseTypeDef,
     UpdateBackendJobResponseTypeDef,
     UpdateBackendStorageResponseTypeDef,
+    CreateBackendAuthForgotPasswordConfigOutputTypeDef,
+    CreateBackendAuthVerificationMessageConfigOutputTypeDef,
     CreateBackendAuthForgotPasswordConfigTypeDef,
     CreateBackendAuthVerificationMessageConfigTypeDef,
     UpdateBackendAuthForgotPasswordConfigTypeDef,
     UpdateBackendAuthVerificationMessageConfigTypeDef,
+    CreateBackendAuthMFAConfigOutputTypeDef,
     CreateBackendAuthMFAConfigTypeDef,
     UpdateBackendAuthMFAConfigTypeDef,
     ListBackendJobsRequestListBackendJobsPaginateTypeDef,
     ListS3BucketsResponseTypeDef,
-    UpdateBackendConfigRequestRequestTypeDef,
     UpdateBackendConfigResponseTypeDef,
+    UpdateBackendConfigRequestRequestTypeDef,
+    BackendAPIResourceConfigOutputTypeDef,
     BackendAPIResourceConfigTypeDef,
+    CreateBackendAuthOAuthConfigOutputTypeDef,
     CreateBackendAuthOAuthConfigTypeDef,
     UpdateBackendAuthOAuthConfigTypeDef,
-    CreateBackendStorageRequestRequestTypeDef,
     GetBackendStorageResponseTypeDef,
+    CreateBackendStorageRequestRequestTypeDef,
     UpdateBackendStorageRequestRequestTypeDef,
+    GetBackendAPIResponseTypeDef,
     CreateBackendAPIRequestRequestTypeDef,
     DeleteBackendAPIRequestRequestTypeDef,
     GetBackendAPIRequestRequestTypeDef,
-    GetBackendAPIResponseTypeDef,
     UpdateBackendAPIRequestRequestTypeDef,
+    CreateBackendAuthUserPoolConfigOutputTypeDef,
     CreateBackendAuthUserPoolConfigTypeDef,
     UpdateBackendAuthUserPoolConfigTypeDef,
+    CreateBackendAuthResourceConfigOutputTypeDef,
     CreateBackendAuthResourceConfigTypeDef,
     UpdateBackendAuthResourceConfigTypeDef,
-    CreateBackendAuthRequestRequestTypeDef,
     GetBackendAuthResponseTypeDef,
+    CreateBackendAuthRequestRequestTypeDef,
     UpdateBackendAuthRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BackendAPIAppSyncAuthSettingsTypeDef:
+def get_structure() -> BackendAPIAppSyncAuthSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifybackend-1.28.0/mypy_boto3_amplifybackend.egg-info/SOURCES.txt` & `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.0/setup.py` & `mypy-boto3-amplifybackend-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplifybackend",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_amplifybackend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AmplifyBackend 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.AmplifyBackend 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

