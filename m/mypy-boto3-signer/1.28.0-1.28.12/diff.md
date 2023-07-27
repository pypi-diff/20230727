# Comparing `tmp/mypy-boto3-signer-1.28.0.tar.gz` & `tmp/mypy-boto3-signer-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-signer-1.28.0.tar", last modified: Thu Jul  6 21:00:39 2023, max compression
+gzip compressed data, was "mypy-boto3-signer-1.28.12.tar", last modified: Thu Jul 27 11:49:40 2023, max compression
```

## Comparing `mypy-boto3-signer-1.28.0.tar` & `mypy-boto3-signer-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:39.198434 mypy-boto3-signer-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:59.000000 mypy-boto3-signer-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-07-06 21:00:39.194434 mypy-boto3-signer-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-07-06 20:55:59.000000 mypy-boto3-signer-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:39.190434 mypy-boto3-signer-1.28.0/mypy_boto3_signer/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-06 20:55:59.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-06 20:55:59.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-06 20:55:59.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-07-06 20:56:00.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-07-06 20:55:59.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-07-06 20:56:00.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-06 20:56:00.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-06 20:56:00.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-06 20:56:00.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:59.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-07-06 20:56:00.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21543 2023-07-06 20:56:00.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:59.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-06 20:56:00.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-06 20:56:00.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:39.194434 mypy-boto3-signer-1.28.0/mypy_boto3_signer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-07-06 21:00:38.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 21:00:38.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:38.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:38.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:38.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 21:00:38.000000 mypy-boto3-signer-1.28.0/mypy_boto3_signer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:39.198434 mypy-boto3-signer-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:55:59.000000 mypy-boto3-signer-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:40.029305 mypy-boto3-signer-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16210 2023-07-27 11:49:40.029305 mypy-boto3-signer-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:40.013305 mypy-boto3-signer-1.28.12/mypy_boto3_signer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22895 2023-07-27 11:47:01.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22878 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:40.029305 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16210 2023-07-27 11:49:39.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 11:49:39.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:39.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:39.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:39.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 11:49:39.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:40.029305 mypy-boto3-signer-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/setup.py
```

### Comparing `mypy-boto3-signer-1.28.0/LICENSE` & `mypy-boto3-signer-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.0/PKG-INFO` & `mypy-boto3-signer-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-signer
-Version: 1.28.0
-Summary: Type annotations for boto3.signer 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.signer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-signer"></a>
 
 # mypy-boto3-signer
 
 [![PyPI - mypy-boto3-signer](https://img.shields.io/pypi/v/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-signer?color=blue)](https://pypistats.org/packages/mypy-boto3-signer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-signer)](https://pepy.tech/project/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.signer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,63 +362,69 @@
 
 `mypy_boto3_signer.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
-    AddProfilePermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
-    SigningMaterialTypeDef,
+    SigningMaterialOutputTypeDef,
     S3DestinationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
     GetRevocationStatusRequestRequestTypeDef,
-    GetRevocationStatusResponseTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
-    SignatureValidityPeriodTypeDef,
+    SignatureValidityPeriodOutputTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSigningJobsRequestRequestTypeDef,
-    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
-    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    PutSigningProfileResponseTypeDef,
+    SignatureValidityPeriodTypeDef,
+    SigningMaterialTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
-    RemoveProfilePermissionResponseTypeDef,
-    ResponseMetadataTypeDef,
     RevokeSignatureRequestRequestTypeDef,
     RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
+    S3SourceOutputTypeDef,
     S3SourceTypeDef,
     SignPayloadRequestRequestTypeDef,
-    SignPayloadResponseTypeDef,
+    SigningConfigurationOverridesOutputTypeDef,
     SigningConfigurationOverridesTypeDef,
-    StartSigningJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AddProfilePermissionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetRevocationStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutSigningProfileResponseTypeDef,
+    RemoveProfilePermissionResponseTypeDef,
+    SignPayloadResponseTypeDef,
+    StartSigningJobResponseTypeDef,
     DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     DestinationTypeDef,
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
+    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
+    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
+    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
+    SourceOutputTypeDef,
     SourceTypeDef,
+    SigningPlatformOverridesOutputTypeDef,
     SigningPlatformOverridesTypeDef,
     ListSigningProfilesResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     SigningPlatformTypeDef,
     SigningJobTypeDef,
     StartSigningJobRequestRequestTypeDef,
     DescribeSigningJobResponseTypeDef,
```

### Comparing `mypy-boto3-signer-1.28.0/README.md` & `mypy-boto3-signer-1.28.12/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-signer"></a>
 
 # mypy-boto3-signer
 
 [![PyPI - mypy-boto3-signer](https://img.shields.io/pypi/v/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-signer?color=blue)](https://pypistats.org/packages/mypy-boto3-signer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-signer)](https://pepy.tech/project/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.signer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,63 +330,69 @@
 
 `mypy_boto3_signer.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
-    AddProfilePermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
-    SigningMaterialTypeDef,
+    SigningMaterialOutputTypeDef,
     S3DestinationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
     GetRevocationStatusRequestRequestTypeDef,
-    GetRevocationStatusResponseTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
-    SignatureValidityPeriodTypeDef,
+    SignatureValidityPeriodOutputTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSigningJobsRequestRequestTypeDef,
-    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
-    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    PutSigningProfileResponseTypeDef,
+    SignatureValidityPeriodTypeDef,
+    SigningMaterialTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
-    RemoveProfilePermissionResponseTypeDef,
-    ResponseMetadataTypeDef,
     RevokeSignatureRequestRequestTypeDef,
     RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
+    S3SourceOutputTypeDef,
     S3SourceTypeDef,
     SignPayloadRequestRequestTypeDef,
-    SignPayloadResponseTypeDef,
+    SigningConfigurationOverridesOutputTypeDef,
     SigningConfigurationOverridesTypeDef,
-    StartSigningJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AddProfilePermissionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetRevocationStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutSigningProfileResponseTypeDef,
+    RemoveProfilePermissionResponseTypeDef,
+    SignPayloadResponseTypeDef,
+    StartSigningJobResponseTypeDef,
     DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     DestinationTypeDef,
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
+    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
+    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
+    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
+    SourceOutputTypeDef,
     SourceTypeDef,
+    SigningPlatformOverridesOutputTypeDef,
     SigningPlatformOverridesTypeDef,
     ListSigningProfilesResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     SigningPlatformTypeDef,
     SigningJobTypeDef,
     StartSigningJobRequestRequestTypeDef,
     DescribeSigningJobResponseTypeDef,
```

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/__init__.py` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/__init__.pyi` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/__main__.py` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.signer 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.signer 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer\nOther"
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

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/client.py` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/client.pyi` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/literals.py` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
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
@@ -253,26 +254,28 @@
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

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/literals.pyi` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,15 @@
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
@@ -251,26 +252,28 @@
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

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/paginator.py` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         isRevoked: bool = ...,
         signatureExpiresBefore: Union[datetime, str] = ...,
         signatureExpiresAfter: Union[datetime, str] = ...,
         jobInvoker: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSigningJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningjobspaginator)
         """
 
 
@@ -85,15 +85,15 @@
 
     def paginate(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSigningPlatformsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningplatformspaginator)
         """
 
 
@@ -105,13 +105,13 @@
 
     def paginate(
         self,
         *,
         includeCanceled: bool = ...,
         platformId: str = ...,
         statuses: Sequence[SigningProfileStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSigningProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningprofilespaginator)
         """
```

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/paginator.pyi` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         isRevoked: bool = ...,
         signatureExpiresBefore: Union[datetime, str] = ...,
         signatureExpiresAfter: Union[datetime, str] = ...,
         jobInvoker: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSigningJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningjobspaginator)
         """
 
 class ListSigningPlatformsPaginator(Paginator):
@@ -81,15 +81,15 @@
 
     def paginate(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSigningPlatformsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningplatformspaginator)
         """
 
 class ListSigningProfilesPaginator(Paginator):
@@ -100,13 +100,13 @@
 
     def paginate(
         self,
         *,
         includeCanceled: bool = ...,
         platformId: str = ...,
         statuses: Sequence[SigningProfileStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSigningProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningprofilespaginator)
         """
```

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/type_defs.py` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -31,66 +31,71 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddProfilePermissionRequestRequestTypeDef",
-    "AddProfilePermissionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelSigningProfileRequestRequestTypeDef",
     "DescribeSigningJobRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "SigningJobRevocationRecordTypeDef",
-    "SigningMaterialTypeDef",
+    "SigningMaterialOutputTypeDef",
     "S3DestinationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncryptionAlgorithmOptionsTypeDef",
     "GetRevocationStatusRequestRequestTypeDef",
-    "GetRevocationStatusResponseTypeDef",
     "GetSigningPlatformRequestRequestTypeDef",
     "SigningImageFormatTypeDef",
     "GetSigningProfileRequestRequestTypeDef",
-    "SignatureValidityPeriodTypeDef",
+    "SignatureValidityPeriodOutputTypeDef",
     "SigningProfileRevocationRecordTypeDef",
     "HashAlgorithmOptionsTypeDef",
     "ListProfilePermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
-    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListSigningJobsRequestRequestTypeDef",
-    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
     "ListSigningPlatformsRequestRequestTypeDef",
-    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "ListSigningProfilesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "PutSigningProfileResponseTypeDef",
+    "SignatureValidityPeriodTypeDef",
+    "SigningMaterialTypeDef",
     "RemoveProfilePermissionRequestRequestTypeDef",
-    "RemoveProfilePermissionResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeSignatureRequestRequestTypeDef",
     "RevokeSigningProfileRequestRequestTypeDef",
     "S3SignedObjectTypeDef",
+    "S3SourceOutputTypeDef",
     "S3SourceTypeDef",
     "SignPayloadRequestRequestTypeDef",
-    "SignPayloadResponseTypeDef",
+    "SigningConfigurationOverridesOutputTypeDef",
     "SigningConfigurationOverridesTypeDef",
-    "StartSigningJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AddProfilePermissionResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetRevocationStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutSigningProfileResponseTypeDef",
+    "RemoveProfilePermissionResponseTypeDef",
+    "SignPayloadResponseTypeDef",
+    "StartSigningJobResponseTypeDef",
     "DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     "DestinationTypeDef",
     "SigningProfileTypeDef",
     "SigningConfigurationTypeDef",
     "ListProfilePermissionsResponseTypeDef",
+    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
+    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "SignedObjectTypeDef",
+    "SourceOutputTypeDef",
     "SourceTypeDef",
+    "SigningPlatformOverridesOutputTypeDef",
     "SigningPlatformOverridesTypeDef",
     "ListSigningProfilesResponseTypeDef",
     "GetSigningPlatformResponseTypeDef",
     "SigningPlatformTypeDef",
     "SigningJobTypeDef",
     "StartSigningJobRequestRequestTypeDef",
     "DescribeSigningJobResponseTypeDef",
@@ -114,27 +119,28 @@
     {
         "profileVersion": str,
         "revisionId": str,
     },
     total=False,
 )
 
-
 class AddProfilePermissionRequestRequestTypeDef(
     _RequiredAddProfilePermissionRequestRequestTypeDef,
     _OptionalAddProfilePermissionRequestRequestTypeDef,
 ):
     pass
 
-
-AddProfilePermissionResponseTypeDef = TypedDict(
-    "AddProfilePermissionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CancelSigningProfileRequestRequestTypeDef = TypedDict(
     "CancelSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
@@ -163,37 +169,30 @@
         "reason": str,
         "revokedAt": datetime,
         "revokedBy": str,
     },
     total=False,
 )
 
-SigningMaterialTypeDef = TypedDict(
-    "SigningMaterialTypeDef",
+SigningMaterialOutputTypeDef = TypedDict(
+    "SigningMaterialOutputTypeDef",
     {
         "certificateArn": str,
     },
 )
 
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "bucketName": str,
         "prefix": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EncryptionAlgorithmOptionsTypeDef = TypedDict(
     "EncryptionAlgorithmOptionsTypeDef",
     {
         "allowedValues": List[EncryptionAlgorithmType],
         "defaultValue": EncryptionAlgorithmType,
     },
 )
@@ -205,22 +204,14 @@
         "platformId": str,
         "profileVersionArn": str,
         "jobArn": str,
         "certificateHashes": Sequence[str],
     },
 )
 
-GetRevocationStatusResponseTypeDef = TypedDict(
-    "GetRevocationStatusResponseTypeDef",
-    {
-        "revokedEntities": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSigningPlatformRequestRequestTypeDef = TypedDict(
     "GetSigningPlatformRequestRequestTypeDef",
     {
         "platformId": str,
     },
 )
 
@@ -242,23 +233,21 @@
     "_OptionalGetSigningProfileRequestRequestTypeDef",
     {
         "profileOwner": str,
     },
     total=False,
 )
 
-
 class GetSigningProfileRequestRequestTypeDef(
     _RequiredGetSigningProfileRequestRequestTypeDef, _OptionalGetSigningProfileRequestRequestTypeDef
 ):
     pass
 
-
-SignatureValidityPeriodTypeDef = TypedDict(
-    "SignatureValidityPeriodTypeDef",
+SignatureValidityPeriodOutputTypeDef = TypedDict(
+    "SignatureValidityPeriodOutputTypeDef",
     {
         "value": int,
         "type": ValidityTypeType,
     },
     total=False,
 )
 
@@ -290,44 +279,37 @@
     "_OptionalListProfilePermissionsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListProfilePermissionsRequestRequestTypeDef(
     _RequiredListProfilePermissionsRequestRequestTypeDef,
     _OptionalListProfilePermissionsRequestRequestTypeDef,
 ):
     pass
 
-
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "action": str,
         "principal": str,
         "statementId": str,
         "profileVersion": str,
     },
     total=False,
 )
 
-ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
-    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": SigningStatusType,
-        "platformId": str,
-        "requestedBy": str,
-        "isRevoked": bool,
-        "signatureExpiresBefore": Union[datetime, str],
-        "signatureExpiresAfter": Union[datetime, str],
-        "jobInvoker": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListSigningJobsRequestRequestTypeDef = TypedDict(
     "ListSigningJobsRequestRequestTypeDef",
     {
@@ -340,48 +322,26 @@
         "signatureExpiresBefore": Union[datetime, str],
         "signatureExpiresAfter": Union[datetime, str],
         "jobInvoker": str,
     },
     total=False,
 )
 
-ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
-    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
-    {
-        "category": str,
-        "partner": str,
-        "target": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSigningPlatformsRequestRequestTypeDef = TypedDict(
     "ListSigningPlatformsRequestRequestTypeDef",
     {
         "category": str,
         "partner": str,
         "target": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = TypedDict(
-    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
-    {
-        "includeCanceled": bool,
-        "platformId": str,
-        "statuses": Sequence[SigningProfileStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSigningProfilesRequestRequestTypeDef = TypedDict(
     "ListSigningProfilesRequestRequestTypeDef",
     {
         "includeCanceled": bool,
         "maxResults": int,
         "nextToken": str,
         "platformId": str,
@@ -393,70 +353,39 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+SignatureValidityPeriodTypeDef = TypedDict(
+    "SignatureValidityPeriodTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "value": int,
+        "type": ValidityTypeType,
     },
     total=False,
 )
 
-PutSigningProfileResponseTypeDef = TypedDict(
-    "PutSigningProfileResponseTypeDef",
+SigningMaterialTypeDef = TypedDict(
+    "SigningMaterialTypeDef",
     {
-        "arn": str,
-        "profileVersion": str,
-        "profileVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "certificateArn": str,
     },
 )
 
 RemoveProfilePermissionRequestRequestTypeDef = TypedDict(
     "RemoveProfilePermissionRequestRequestTypeDef",
     {
         "profileName": str,
         "revisionId": str,
         "statementId": str,
     },
 )
 
-RemoveProfilePermissionResponseTypeDef = TypedDict(
-    "RemoveProfilePermissionResponseTypeDef",
-    {
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 _RequiredRevokeSignatureRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeSignatureRequestRequestTypeDef",
     {
         "jobId": str,
         "reason": str,
     },
 )
@@ -464,21 +393,19 @@
     "_OptionalRevokeSignatureRequestRequestTypeDef",
     {
         "jobOwner": str,
     },
     total=False,
 )
 
-
 class RevokeSignatureRequestRequestTypeDef(
     _RequiredRevokeSignatureRequestRequestTypeDef, _OptionalRevokeSignatureRequestRequestTypeDef
 ):
     pass
 
-
 RevokeSigningProfileRequestRequestTypeDef = TypedDict(
     "RevokeSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "reason": str,
         "effectiveTime": Union[datetime, str],
@@ -490,14 +417,23 @@
     {
         "bucketName": str,
         "key": str,
     },
     total=False,
 )
 
+S3SourceOutputTypeDef = TypedDict(
+    "S3SourceOutputTypeDef",
+    {
+        "bucketName": str,
+        "key": str,
+        "version": str,
+    },
+)
+
 S3SourceTypeDef = TypedDict(
     "S3SourceTypeDef",
     {
         "bucketName": str,
         "key": str,
         "version": str,
     },
@@ -515,50 +451,37 @@
     "_OptionalSignPayloadRequestRequestTypeDef",
     {
         "profileOwner": str,
     },
     total=False,
 )
 
-
 class SignPayloadRequestRequestTypeDef(
     _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
 ):
     pass
 
-
-SignPayloadResponseTypeDef = TypedDict(
-    "SignPayloadResponseTypeDef",
+SigningConfigurationOverridesOutputTypeDef = TypedDict(
+    "SigningConfigurationOverridesOutputTypeDef",
     {
-        "jobId": str,
-        "jobOwner": str,
-        "metadata": Dict[str, str],
-        "signature": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "encryptionAlgorithm": EncryptionAlgorithmType,
+        "hashAlgorithm": HashAlgorithmType,
     },
+    total=False,
 )
 
 SigningConfigurationOverridesTypeDef = TypedDict(
     "SigningConfigurationOverridesTypeDef",
     {
         "encryptionAlgorithm": EncryptionAlgorithmType,
         "hashAlgorithm": HashAlgorithmType,
     },
     total=False,
 )
 
-StartSigningJobResponseTypeDef = TypedDict(
-    "StartSigningJobResponseTypeDef",
-    {
-        "jobId": str,
-        "jobOwner": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -567,52 +490,119 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+AddProfilePermissionResponseTypeDef = TypedDict(
+    "AddProfilePermissionResponseTypeDef",
+    {
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRevocationStatusResponseTypeDef = TypedDict(
+    "GetRevocationStatusResponseTypeDef",
+    {
+        "revokedEntities": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSigningProfileResponseTypeDef = TypedDict(
+    "PutSigningProfileResponseTypeDef",
+    {
+        "arn": str,
+        "profileVersion": str,
+        "profileVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveProfilePermissionResponseTypeDef = TypedDict(
+    "RemoveProfilePermissionResponseTypeDef",
+    {
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SignPayloadResponseTypeDef = TypedDict(
+    "SignPayloadResponseTypeDef",
+    {
+        "jobId": str,
+        "jobOwner": str,
+        "metadata": Dict[str, str],
+        "signature": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSigningJobResponseTypeDef = TypedDict(
+    "StartSigningJobResponseTypeDef",
+    {
+        "jobId": str,
+        "jobOwner": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
     "_RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
     "_OptionalDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef(
     _RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     _OptionalDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
 ):
     pass
 
-
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3": S3DestinationTypeDef,
     },
     total=False,
 )
 
 SigningProfileTypeDef = TypedDict(
     "SigningProfileTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "profileVersionArn": str,
-        "signingMaterial": SigningMaterialTypeDef,
-        "signatureValidityPeriod": SignatureValidityPeriodTypeDef,
+        "signingMaterial": SigningMaterialOutputTypeDef,
+        "signatureValidityPeriod": SignatureValidityPeriodOutputTypeDef,
         "platformId": str,
         "platformDisplayName": str,
         "signingParameters": Dict[str, str],
         "status": SigningProfileStatusType,
         "arn": str,
         "tags": Dict[str, str],
     },
@@ -630,49 +620,103 @@
 ListProfilePermissionsResponseTypeDef = TypedDict(
     "ListProfilePermissionsResponseTypeDef",
     {
         "revisionId": str,
         "policySizeBytes": int,
         "permissions": List[PermissionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
+    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
+    {
+        "status": SigningStatusType,
+        "platformId": str,
+        "requestedBy": str,
+        "isRevoked": bool,
+        "signatureExpiresBefore": Union[datetime, str],
+        "signatureExpiresAfter": Union[datetime, str],
+        "jobInvoker": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
+    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+    {
+        "category": str,
+        "partner": str,
+        "target": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = TypedDict(
+    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
+    {
+        "includeCanceled": bool,
+        "platformId": str,
+        "statuses": Sequence[SigningProfileStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 SignedObjectTypeDef = TypedDict(
     "SignedObjectTypeDef",
     {
         "s3": S3SignedObjectTypeDef,
     },
     total=False,
 )
 
+SourceOutputTypeDef = TypedDict(
+    "SourceOutputTypeDef",
+    {
+        "s3": S3SourceOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "s3": S3SourceTypeDef,
     },
     total=False,
 )
 
+SigningPlatformOverridesOutputTypeDef = TypedDict(
+    "SigningPlatformOverridesOutputTypeDef",
+    {
+        "signingConfiguration": SigningConfigurationOverridesOutputTypeDef,
+        "signingImageFormat": ImageFormatType,
+    },
+    total=False,
+)
+
 SigningPlatformOverridesTypeDef = TypedDict(
     "SigningPlatformOverridesTypeDef",
     {
         "signingConfiguration": SigningConfigurationOverridesTypeDef,
         "signingImageFormat": ImageFormatType,
     },
     total=False,
 )
 
 ListSigningProfilesResponseTypeDef = TypedDict(
     "ListSigningProfilesResponseTypeDef",
     {
         "profiles": List[SigningProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSigningPlatformResponseTypeDef = TypedDict(
     "GetSigningPlatformResponseTypeDef",
     {
         "platformId": str,
@@ -680,15 +724,15 @@
         "partner": str,
         "target": str,
         "category": Literal["AWSIoT"],
         "signingConfiguration": SigningConfigurationTypeDef,
         "signingImageFormat": SigningImageFormatTypeDef,
         "maxSizeInMB": int,
         "revocationSupported": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SigningPlatformTypeDef = TypedDict(
     "SigningPlatformTypeDef",
     {
         "platformId": str,
@@ -704,17 +748,17 @@
     total=False,
 )
 
 SigningJobTypeDef = TypedDict(
     "SigningJobTypeDef",
     {
         "jobId": str,
-        "source": SourceTypeDef,
+        "source": SourceOutputTypeDef,
         "signedObject": SignedObjectTypeDef,
-        "signingMaterial": SigningMaterialTypeDef,
+        "signingMaterial": SigningMaterialOutputTypeDef,
         "createdAt": datetime,
         "status": SigningStatusType,
         "isRevoked": bool,
         "profileName": str,
         "profileVersion": str,
         "platformId": str,
         "platformDisplayName": str,
@@ -738,65 +782,63 @@
     "_OptionalStartSigningJobRequestRequestTypeDef",
     {
         "profileOwner": str,
     },
     total=False,
 )
 
-
 class StartSigningJobRequestRequestTypeDef(
     _RequiredStartSigningJobRequestRequestTypeDef, _OptionalStartSigningJobRequestRequestTypeDef
 ):
     pass
 
-
 DescribeSigningJobResponseTypeDef = TypedDict(
     "DescribeSigningJobResponseTypeDef",
     {
         "jobId": str,
-        "source": SourceTypeDef,
-        "signingMaterial": SigningMaterialTypeDef,
+        "source": SourceOutputTypeDef,
+        "signingMaterial": SigningMaterialOutputTypeDef,
         "platformId": str,
         "platformDisplayName": str,
         "profileName": str,
         "profileVersion": str,
-        "overrides": SigningPlatformOverridesTypeDef,
+        "overrides": SigningPlatformOverridesOutputTypeDef,
         "signingParameters": Dict[str, str],
         "createdAt": datetime,
         "completedAt": datetime,
         "signatureExpiresAt": datetime,
         "requestedBy": str,
         "status": SigningStatusType,
         "statusReason": str,
         "revocationRecord": SigningJobRevocationRecordTypeDef,
         "signedObject": SignedObjectTypeDef,
         "jobOwner": str,
         "jobInvoker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSigningProfileResponseTypeDef = TypedDict(
     "GetSigningProfileResponseTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "profileVersionArn": str,
         "revocationRecord": SigningProfileRevocationRecordTypeDef,
-        "signingMaterial": SigningMaterialTypeDef,
+        "signingMaterial": SigningMaterialOutputTypeDef,
         "platformId": str,
         "platformDisplayName": str,
-        "signatureValidityPeriod": SignatureValidityPeriodTypeDef,
-        "overrides": SigningPlatformOverridesTypeDef,
+        "signatureValidityPeriod": SignatureValidityPeriodOutputTypeDef,
+        "overrides": SigningPlatformOverridesOutputTypeDef,
         "signingParameters": Dict[str, str],
         "status": SigningProfileStatusType,
         "statusReason": str,
         "arn": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutSigningProfileRequestRequestTypeDef = TypedDict(
     "_RequiredPutSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
@@ -811,31 +853,29 @@
         "overrides": SigningPlatformOverridesTypeDef,
         "signingParameters": Mapping[str, str],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class PutSigningProfileRequestRequestTypeDef(
     _RequiredPutSigningProfileRequestRequestTypeDef, _OptionalPutSigningProfileRequestRequestTypeDef
 ):
     pass
 
-
 ListSigningPlatformsResponseTypeDef = TypedDict(
     "ListSigningPlatformsResponseTypeDef",
     {
         "platforms": List[SigningPlatformTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSigningJobsResponseTypeDef = TypedDict(
     "ListSigningJobsResponseTypeDef",
     {
         "jobs": List[SigningJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/type_defs.pyi` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,65 +31,72 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddProfilePermissionRequestRequestTypeDef",
-    "AddProfilePermissionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelSigningProfileRequestRequestTypeDef",
     "DescribeSigningJobRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "SigningJobRevocationRecordTypeDef",
-    "SigningMaterialTypeDef",
+    "SigningMaterialOutputTypeDef",
     "S3DestinationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncryptionAlgorithmOptionsTypeDef",
     "GetRevocationStatusRequestRequestTypeDef",
-    "GetRevocationStatusResponseTypeDef",
     "GetSigningPlatformRequestRequestTypeDef",
     "SigningImageFormatTypeDef",
     "GetSigningProfileRequestRequestTypeDef",
-    "SignatureValidityPeriodTypeDef",
+    "SignatureValidityPeriodOutputTypeDef",
     "SigningProfileRevocationRecordTypeDef",
     "HashAlgorithmOptionsTypeDef",
     "ListProfilePermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
-    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListSigningJobsRequestRequestTypeDef",
-    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
     "ListSigningPlatformsRequestRequestTypeDef",
-    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "ListSigningProfilesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "PutSigningProfileResponseTypeDef",
+    "SignatureValidityPeriodTypeDef",
+    "SigningMaterialTypeDef",
     "RemoveProfilePermissionRequestRequestTypeDef",
-    "RemoveProfilePermissionResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeSignatureRequestRequestTypeDef",
     "RevokeSigningProfileRequestRequestTypeDef",
     "S3SignedObjectTypeDef",
+    "S3SourceOutputTypeDef",
     "S3SourceTypeDef",
     "SignPayloadRequestRequestTypeDef",
-    "SignPayloadResponseTypeDef",
+    "SigningConfigurationOverridesOutputTypeDef",
     "SigningConfigurationOverridesTypeDef",
-    "StartSigningJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AddProfilePermissionResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetRevocationStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutSigningProfileResponseTypeDef",
+    "RemoveProfilePermissionResponseTypeDef",
+    "SignPayloadResponseTypeDef",
+    "StartSigningJobResponseTypeDef",
     "DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     "DestinationTypeDef",
     "SigningProfileTypeDef",
     "SigningConfigurationTypeDef",
     "ListProfilePermissionsResponseTypeDef",
+    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
+    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "SignedObjectTypeDef",
+    "SourceOutputTypeDef",
     "SourceTypeDef",
+    "SigningPlatformOverridesOutputTypeDef",
     "SigningPlatformOverridesTypeDef",
     "ListSigningProfilesResponseTypeDef",
     "GetSigningPlatformResponseTypeDef",
     "SigningPlatformTypeDef",
     "SigningJobTypeDef",
     "StartSigningJobRequestRequestTypeDef",
     "DescribeSigningJobResponseTypeDef",
@@ -113,25 +120,30 @@
     {
         "profileVersion": str,
         "revisionId": str,
     },
     total=False,
 )
 
+
 class AddProfilePermissionRequestRequestTypeDef(
     _RequiredAddProfilePermissionRequestRequestTypeDef,
     _OptionalAddProfilePermissionRequestRequestTypeDef,
 ):
     pass
 
-AddProfilePermissionResponseTypeDef = TypedDict(
-    "AddProfilePermissionResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CancelSigningProfileRequestRequestTypeDef = TypedDict(
     "CancelSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
@@ -160,37 +172,30 @@
         "reason": str,
         "revokedAt": datetime,
         "revokedBy": str,
     },
     total=False,
 )
 
-SigningMaterialTypeDef = TypedDict(
-    "SigningMaterialTypeDef",
+SigningMaterialOutputTypeDef = TypedDict(
+    "SigningMaterialOutputTypeDef",
     {
         "certificateArn": str,
     },
 )
 
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "bucketName": str,
         "prefix": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EncryptionAlgorithmOptionsTypeDef = TypedDict(
     "EncryptionAlgorithmOptionsTypeDef",
     {
         "allowedValues": List[EncryptionAlgorithmType],
         "defaultValue": EncryptionAlgorithmType,
     },
 )
@@ -202,22 +207,14 @@
         "platformId": str,
         "profileVersionArn": str,
         "jobArn": str,
         "certificateHashes": Sequence[str],
     },
 )
 
-GetRevocationStatusResponseTypeDef = TypedDict(
-    "GetRevocationStatusResponseTypeDef",
-    {
-        "revokedEntities": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSigningPlatformRequestRequestTypeDef = TypedDict(
     "GetSigningPlatformRequestRequestTypeDef",
     {
         "platformId": str,
     },
 )
 
@@ -239,21 +236,23 @@
     "_OptionalGetSigningProfileRequestRequestTypeDef",
     {
         "profileOwner": str,
     },
     total=False,
 )
 
+
 class GetSigningProfileRequestRequestTypeDef(
     _RequiredGetSigningProfileRequestRequestTypeDef, _OptionalGetSigningProfileRequestRequestTypeDef
 ):
     pass
 
-SignatureValidityPeriodTypeDef = TypedDict(
-    "SignatureValidityPeriodTypeDef",
+
+SignatureValidityPeriodOutputTypeDef = TypedDict(
+    "SignatureValidityPeriodOutputTypeDef",
     {
         "value": int,
         "type": ValidityTypeType,
     },
     total=False,
 )
 
@@ -285,42 +284,39 @@
     "_OptionalListProfilePermissionsRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListProfilePermissionsRequestRequestTypeDef(
     _RequiredListProfilePermissionsRequestRequestTypeDef,
     _OptionalListProfilePermissionsRequestRequestTypeDef,
 ):
     pass
 
+
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "action": str,
         "principal": str,
         "statementId": str,
         "profileVersion": str,
     },
     total=False,
 )
 
-ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
-    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": SigningStatusType,
-        "platformId": str,
-        "requestedBy": str,
-        "isRevoked": bool,
-        "signatureExpiresBefore": Union[datetime, str],
-        "signatureExpiresAfter": Union[datetime, str],
-        "jobInvoker": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListSigningJobsRequestRequestTypeDef = TypedDict(
     "ListSigningJobsRequestRequestTypeDef",
     {
@@ -333,48 +329,26 @@
         "signatureExpiresBefore": Union[datetime, str],
         "signatureExpiresAfter": Union[datetime, str],
         "jobInvoker": str,
     },
     total=False,
 )
 
-ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
-    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
-    {
-        "category": str,
-        "partner": str,
-        "target": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSigningPlatformsRequestRequestTypeDef = TypedDict(
     "ListSigningPlatformsRequestRequestTypeDef",
     {
         "category": str,
         "partner": str,
         "target": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = TypedDict(
-    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
-    {
-        "includeCanceled": bool,
-        "platformId": str,
-        "statuses": Sequence[SigningProfileStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSigningProfilesRequestRequestTypeDef = TypedDict(
     "ListSigningProfilesRequestRequestTypeDef",
     {
         "includeCanceled": bool,
         "maxResults": int,
         "nextToken": str,
         "platformId": str,
@@ -386,70 +360,39 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+SignatureValidityPeriodTypeDef = TypedDict(
+    "SignatureValidityPeriodTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "value": int,
+        "type": ValidityTypeType,
     },
     total=False,
 )
 
-PutSigningProfileResponseTypeDef = TypedDict(
-    "PutSigningProfileResponseTypeDef",
+SigningMaterialTypeDef = TypedDict(
+    "SigningMaterialTypeDef",
     {
-        "arn": str,
-        "profileVersion": str,
-        "profileVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "certificateArn": str,
     },
 )
 
 RemoveProfilePermissionRequestRequestTypeDef = TypedDict(
     "RemoveProfilePermissionRequestRequestTypeDef",
     {
         "profileName": str,
         "revisionId": str,
         "statementId": str,
     },
 )
 
-RemoveProfilePermissionResponseTypeDef = TypedDict(
-    "RemoveProfilePermissionResponseTypeDef",
-    {
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 _RequiredRevokeSignatureRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeSignatureRequestRequestTypeDef",
     {
         "jobId": str,
         "reason": str,
     },
 )
@@ -457,19 +400,21 @@
     "_OptionalRevokeSignatureRequestRequestTypeDef",
     {
         "jobOwner": str,
     },
     total=False,
 )
 
+
 class RevokeSignatureRequestRequestTypeDef(
     _RequiredRevokeSignatureRequestRequestTypeDef, _OptionalRevokeSignatureRequestRequestTypeDef
 ):
     pass
 
+
 RevokeSigningProfileRequestRequestTypeDef = TypedDict(
     "RevokeSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "reason": str,
         "effectiveTime": Union[datetime, str],
@@ -481,14 +426,23 @@
     {
         "bucketName": str,
         "key": str,
     },
     total=False,
 )
 
+S3SourceOutputTypeDef = TypedDict(
+    "S3SourceOutputTypeDef",
+    {
+        "bucketName": str,
+        "key": str,
+        "version": str,
+    },
+)
+
 S3SourceTypeDef = TypedDict(
     "S3SourceTypeDef",
     {
         "bucketName": str,
         "key": str,
         "version": str,
     },
@@ -506,48 +460,39 @@
     "_OptionalSignPayloadRequestRequestTypeDef",
     {
         "profileOwner": str,
     },
     total=False,
 )
 
+
 class SignPayloadRequestRequestTypeDef(
     _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
 ):
     pass
 
-SignPayloadResponseTypeDef = TypedDict(
-    "SignPayloadResponseTypeDef",
+
+SigningConfigurationOverridesOutputTypeDef = TypedDict(
+    "SigningConfigurationOverridesOutputTypeDef",
     {
-        "jobId": str,
-        "jobOwner": str,
-        "metadata": Dict[str, str],
-        "signature": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "encryptionAlgorithm": EncryptionAlgorithmType,
+        "hashAlgorithm": HashAlgorithmType,
     },
+    total=False,
 )
 
 SigningConfigurationOverridesTypeDef = TypedDict(
     "SigningConfigurationOverridesTypeDef",
     {
         "encryptionAlgorithm": EncryptionAlgorithmType,
         "hashAlgorithm": HashAlgorithmType,
     },
     total=False,
 )
 
-StartSigningJobResponseTypeDef = TypedDict(
-    "StartSigningJobResponseTypeDef",
-    {
-        "jobId": str,
-        "jobOwner": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -556,50 +501,121 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+AddProfilePermissionResponseTypeDef = TypedDict(
+    "AddProfilePermissionResponseTypeDef",
+    {
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRevocationStatusResponseTypeDef = TypedDict(
+    "GetRevocationStatusResponseTypeDef",
+    {
+        "revokedEntities": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSigningProfileResponseTypeDef = TypedDict(
+    "PutSigningProfileResponseTypeDef",
+    {
+        "arn": str,
+        "profileVersion": str,
+        "profileVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveProfilePermissionResponseTypeDef = TypedDict(
+    "RemoveProfilePermissionResponseTypeDef",
+    {
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SignPayloadResponseTypeDef = TypedDict(
+    "SignPayloadResponseTypeDef",
+    {
+        "jobId": str,
+        "jobOwner": str,
+        "metadata": Dict[str, str],
+        "signature": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSigningJobResponseTypeDef = TypedDict(
+    "StartSigningJobResponseTypeDef",
+    {
+        "jobId": str,
+        "jobOwner": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
     "_RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
     "_OptionalDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef(
     _RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     _OptionalDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
 ):
     pass
 
+
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3": S3DestinationTypeDef,
     },
     total=False,
 )
 
 SigningProfileTypeDef = TypedDict(
     "SigningProfileTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "profileVersionArn": str,
-        "signingMaterial": SigningMaterialTypeDef,
-        "signatureValidityPeriod": SignatureValidityPeriodTypeDef,
+        "signingMaterial": SigningMaterialOutputTypeDef,
+        "signatureValidityPeriod": SignatureValidityPeriodOutputTypeDef,
         "platformId": str,
         "platformDisplayName": str,
         "signingParameters": Dict[str, str],
         "status": SigningProfileStatusType,
         "arn": str,
         "tags": Dict[str, str],
     },
@@ -617,49 +633,103 @@
 ListProfilePermissionsResponseTypeDef = TypedDict(
     "ListProfilePermissionsResponseTypeDef",
     {
         "revisionId": str,
         "policySizeBytes": int,
         "permissions": List[PermissionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
+    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
+    {
+        "status": SigningStatusType,
+        "platformId": str,
+        "requestedBy": str,
+        "isRevoked": bool,
+        "signatureExpiresBefore": Union[datetime, str],
+        "signatureExpiresAfter": Union[datetime, str],
+        "jobInvoker": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
+    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+    {
+        "category": str,
+        "partner": str,
+        "target": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = TypedDict(
+    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
+    {
+        "includeCanceled": bool,
+        "platformId": str,
+        "statuses": Sequence[SigningProfileStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 SignedObjectTypeDef = TypedDict(
     "SignedObjectTypeDef",
     {
         "s3": S3SignedObjectTypeDef,
     },
     total=False,
 )
 
+SourceOutputTypeDef = TypedDict(
+    "SourceOutputTypeDef",
+    {
+        "s3": S3SourceOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "s3": S3SourceTypeDef,
     },
     total=False,
 )
 
+SigningPlatformOverridesOutputTypeDef = TypedDict(
+    "SigningPlatformOverridesOutputTypeDef",
+    {
+        "signingConfiguration": SigningConfigurationOverridesOutputTypeDef,
+        "signingImageFormat": ImageFormatType,
+    },
+    total=False,
+)
+
 SigningPlatformOverridesTypeDef = TypedDict(
     "SigningPlatformOverridesTypeDef",
     {
         "signingConfiguration": SigningConfigurationOverridesTypeDef,
         "signingImageFormat": ImageFormatType,
     },
     total=False,
 )
 
 ListSigningProfilesResponseTypeDef = TypedDict(
     "ListSigningProfilesResponseTypeDef",
     {
         "profiles": List[SigningProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSigningPlatformResponseTypeDef = TypedDict(
     "GetSigningPlatformResponseTypeDef",
     {
         "platformId": str,
@@ -667,15 +737,15 @@
         "partner": str,
         "target": str,
         "category": Literal["AWSIoT"],
         "signingConfiguration": SigningConfigurationTypeDef,
         "signingImageFormat": SigningImageFormatTypeDef,
         "maxSizeInMB": int,
         "revocationSupported": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SigningPlatformTypeDef = TypedDict(
     "SigningPlatformTypeDef",
     {
         "platformId": str,
@@ -691,17 +761,17 @@
     total=False,
 )
 
 SigningJobTypeDef = TypedDict(
     "SigningJobTypeDef",
     {
         "jobId": str,
-        "source": SourceTypeDef,
+        "source": SourceOutputTypeDef,
         "signedObject": SignedObjectTypeDef,
-        "signingMaterial": SigningMaterialTypeDef,
+        "signingMaterial": SigningMaterialOutputTypeDef,
         "createdAt": datetime,
         "status": SigningStatusType,
         "isRevoked": bool,
         "profileName": str,
         "profileVersion": str,
         "platformId": str,
         "platformDisplayName": str,
@@ -725,63 +795,65 @@
     "_OptionalStartSigningJobRequestRequestTypeDef",
     {
         "profileOwner": str,
     },
     total=False,
 )
 
+
 class StartSigningJobRequestRequestTypeDef(
     _RequiredStartSigningJobRequestRequestTypeDef, _OptionalStartSigningJobRequestRequestTypeDef
 ):
     pass
 
+
 DescribeSigningJobResponseTypeDef = TypedDict(
     "DescribeSigningJobResponseTypeDef",
     {
         "jobId": str,
-        "source": SourceTypeDef,
-        "signingMaterial": SigningMaterialTypeDef,
+        "source": SourceOutputTypeDef,
+        "signingMaterial": SigningMaterialOutputTypeDef,
         "platformId": str,
         "platformDisplayName": str,
         "profileName": str,
         "profileVersion": str,
-        "overrides": SigningPlatformOverridesTypeDef,
+        "overrides": SigningPlatformOverridesOutputTypeDef,
         "signingParameters": Dict[str, str],
         "createdAt": datetime,
         "completedAt": datetime,
         "signatureExpiresAt": datetime,
         "requestedBy": str,
         "status": SigningStatusType,
         "statusReason": str,
         "revocationRecord": SigningJobRevocationRecordTypeDef,
         "signedObject": SignedObjectTypeDef,
         "jobOwner": str,
         "jobInvoker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSigningProfileResponseTypeDef = TypedDict(
     "GetSigningProfileResponseTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "profileVersionArn": str,
         "revocationRecord": SigningProfileRevocationRecordTypeDef,
-        "signingMaterial": SigningMaterialTypeDef,
+        "signingMaterial": SigningMaterialOutputTypeDef,
         "platformId": str,
         "platformDisplayName": str,
-        "signatureValidityPeriod": SignatureValidityPeriodTypeDef,
-        "overrides": SigningPlatformOverridesTypeDef,
+        "signatureValidityPeriod": SignatureValidityPeriodOutputTypeDef,
+        "overrides": SigningPlatformOverridesOutputTypeDef,
         "signingParameters": Dict[str, str],
         "status": SigningProfileStatusType,
         "statusReason": str,
         "arn": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutSigningProfileRequestRequestTypeDef = TypedDict(
     "_RequiredPutSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
@@ -796,29 +868,31 @@
         "overrides": SigningPlatformOverridesTypeDef,
         "signingParameters": Mapping[str, str],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class PutSigningProfileRequestRequestTypeDef(
     _RequiredPutSigningProfileRequestRequestTypeDef, _OptionalPutSigningProfileRequestRequestTypeDef
 ):
     pass
 
+
 ListSigningPlatformsResponseTypeDef = TypedDict(
     "ListSigningPlatformsResponseTypeDef",
     {
         "platforms": List[SigningPlatformTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSigningJobsResponseTypeDef = TypedDict(
     "ListSigningJobsResponseTypeDef",
     {
         "jobs": List[SigningJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/waiter.py` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer/waiter.pyi` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer.egg-info/PKG-INFO` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-signer
-Version: 1.28.0
-Summary: Type annotations for boto3.signer 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.signer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-signer"></a>
 
 # mypy-boto3-signer
 
 [![PyPI - mypy-boto3-signer](https://img.shields.io/pypi/v/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-signer?color=blue)](https://pypistats.org/packages/mypy-boto3-signer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-signer)](https://pepy.tech/project/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.signer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,63 +362,69 @@
 
 `mypy_boto3_signer.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
-    AddProfilePermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
-    SigningMaterialTypeDef,
+    SigningMaterialOutputTypeDef,
     S3DestinationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
     GetRevocationStatusRequestRequestTypeDef,
-    GetRevocationStatusResponseTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
-    SignatureValidityPeriodTypeDef,
+    SignatureValidityPeriodOutputTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListSigningJobsRequestRequestTypeDef,
-    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
-    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    PutSigningProfileResponseTypeDef,
+    SignatureValidityPeriodTypeDef,
+    SigningMaterialTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
-    RemoveProfilePermissionResponseTypeDef,
-    ResponseMetadataTypeDef,
     RevokeSignatureRequestRequestTypeDef,
     RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
+    S3SourceOutputTypeDef,
     S3SourceTypeDef,
     SignPayloadRequestRequestTypeDef,
-    SignPayloadResponseTypeDef,
+    SigningConfigurationOverridesOutputTypeDef,
     SigningConfigurationOverridesTypeDef,
-    StartSigningJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AddProfilePermissionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetRevocationStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutSigningProfileResponseTypeDef,
+    RemoveProfilePermissionResponseTypeDef,
+    SignPayloadResponseTypeDef,
+    StartSigningJobResponseTypeDef,
     DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     DestinationTypeDef,
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
+    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
+    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
+    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
+    SourceOutputTypeDef,
     SourceTypeDef,
+    SigningPlatformOverridesOutputTypeDef,
     SigningPlatformOverridesTypeDef,
     ListSigningProfilesResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     SigningPlatformTypeDef,
     SigningJobTypeDef,
     StartSigningJobRequestRequestTypeDef,
     DescribeSigningJobResponseTypeDef,
```

### Comparing `mypy-boto3-signer-1.28.0/mypy_boto3_signer.egg-info/SOURCES.txt` & `mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.0/setup.py` & `mypy-boto3-signer-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-signer",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_signer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.signer 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.signer 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

