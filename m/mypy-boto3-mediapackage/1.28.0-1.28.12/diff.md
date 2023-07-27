# Comparing `tmp/mypy-boto3-mediapackage-1.28.0.tar.gz` & `tmp/mypy-boto3-mediapackage-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackage-1.28.0.tar", last modified: Thu Jul  6 21:00:05 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackage-1.28.12.tar", last modified: Thu Jul 27 05:35:00 2023, max compression
```

## Comparing `mypy-boto3-mediapackage-1.28.0.tar` & `mypy-boto3-mediapackage-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:05.742366 mypy-boto3-mediapackage-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-07-06 21:00:05.738366 mypy-boto3-mediapackage-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:05.718366 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-07-06 20:47:16.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-06 20:47:16.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-07-06 20:47:16.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-06 20:47:16.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-06 20:47:16.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25765 2023-07-06 20:47:17.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25742 2023-07-06 20:47:17.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:05.738366 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:05.742366 mypy-boto3-mediapackage-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:47:13.000000 mypy-boto3-mediapackage-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.856442 mypy-boto3-mediapackage-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-07-27 05:35:00.848442 mypy-boto3-mediapackage-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.840442 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31687 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31656 2023-07-27 05:26:20.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.848442 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:00.856442 mypy-boto3-mediapackage-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:26:19.000000 mypy-boto3-mediapackage-1.28.12/setup.py
```

### Comparing `mypy-boto3-mediapackage-1.28.0/LICENSE` & `mypy-boto3-mediapackage-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.0/PKG-INFO` & `mypy-boto3-mediapackage-1.28.12/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage
-Version: 1.28.0
-Summary: Type annotations for boto3.MediaPackage 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MediaPackage 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediapackage"></a>
 
 # mypy-boto3-mediapackage
 
 [![PyPI - mypy-boto3-mediapackage](https://img.shields.io/pypi/v/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage)](https://pepy.tech/project/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,28 +345,34 @@
 ### Typed dictionaries
 
 `mypy_boto3_mediapackage.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage.type_defs import (
+    AuthorizationOutputTypeDef,
     AuthorizationTypeDef,
-    EgressAccessLogsTypeDef,
-    IngressAccessLogsTypeDef,
+    EgressAccessLogsOutputTypeDef,
+    IngressAccessLogsOutputTypeDef,
     HlsManifestCreateOrUpdateParametersTypeDef,
     StreamSelectionTypeDef,
     HlsManifestTypeDef,
+    StreamSelectionOutputTypeDef,
+    EgressAccessLogsTypeDef,
+    IngressAccessLogsTypeDef,
     CreateChannelRequestRequestTypeDef,
     S3DestinationTypeDef,
+    S3DestinationOutputTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeHarvestJobRequestRequestTypeDef,
     DescribeOriginEndpointRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
     IngestEndpointTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
     ListHarvestJobsRequestRequestTypeDef,
     ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
@@ -381,45 +387,53 @@
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
     CreateHarvestJobRequestRequestTypeDef,
     CreateHarvestJobResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     HarvestJobTypeDef,
+    SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     HlsIngestTypeDef,
     ListHarvestJobsResponseTypeDef,
+    CmafEncryptionOutputTypeDef,
+    DashEncryptionOutputTypeDef,
+    HlsEncryptionOutputTypeDef,
+    MssEncryptionOutputTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
     HlsEncryptionTypeDef,
     MssEncryptionTypeDef,
     ChannelTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateChannelResponseTypeDef,
     DescribeChannelResponseTypeDef,
     RotateChannelCredentialsResponseTypeDef,
     RotateIngestEndpointCredentialsResponseTypeDef,
     UpdateChannelResponseTypeDef,
-    CmafPackageCreateOrUpdateParametersTypeDef,
     CmafPackageTypeDef,
+    DashPackageOutputTypeDef,
+    HlsPackageOutputTypeDef,
+    MssPackageOutputTypeDef,
+    CmafPackageCreateOrUpdateParametersTypeDef,
     DashPackageTypeDef,
     HlsPackageTypeDef,
     MssPackageTypeDef,
     ListChannelsResponseTypeDef,
-    CreateOriginEndpointRequestRequestTypeDef,
     CreateOriginEndpointResponseTypeDef,
     DescribeOriginEndpointResponseTypeDef,
     OriginEndpointTypeDef,
-    UpdateOriginEndpointRequestRequestTypeDef,
     UpdateOriginEndpointResponseTypeDef,
+    CreateOriginEndpointRequestRequestTypeDef,
+    UpdateOriginEndpointRequestRequestTypeDef,
     ListOriginEndpointsResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationTypeDef:
+def get_structure() -> AuthorizationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackage-1.28.0/README.md` & `mypy-boto3-mediapackage-1.28.12/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mediapackage"></a>
 
 # mypy-boto3-mediapackage
 
 [![PyPI - mypy-boto3-mediapackage](https://img.shields.io/pypi/v/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage)](https://pepy.tech/project/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,28 +313,34 @@
 ### Typed dictionaries
 
 `mypy_boto3_mediapackage.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage.type_defs import (
+    AuthorizationOutputTypeDef,
     AuthorizationTypeDef,
-    EgressAccessLogsTypeDef,
-    IngressAccessLogsTypeDef,
+    EgressAccessLogsOutputTypeDef,
+    IngressAccessLogsOutputTypeDef,
     HlsManifestCreateOrUpdateParametersTypeDef,
     StreamSelectionTypeDef,
     HlsManifestTypeDef,
+    StreamSelectionOutputTypeDef,
+    EgressAccessLogsTypeDef,
+    IngressAccessLogsTypeDef,
     CreateChannelRequestRequestTypeDef,
     S3DestinationTypeDef,
+    S3DestinationOutputTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeHarvestJobRequestRequestTypeDef,
     DescribeOriginEndpointRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
     IngestEndpointTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
     ListHarvestJobsRequestRequestTypeDef,
     ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
@@ -349,45 +355,53 @@
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
     CreateHarvestJobRequestRequestTypeDef,
     CreateHarvestJobResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     HarvestJobTypeDef,
+    SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     HlsIngestTypeDef,
     ListHarvestJobsResponseTypeDef,
+    CmafEncryptionOutputTypeDef,
+    DashEncryptionOutputTypeDef,
+    HlsEncryptionOutputTypeDef,
+    MssEncryptionOutputTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
     HlsEncryptionTypeDef,
     MssEncryptionTypeDef,
     ChannelTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateChannelResponseTypeDef,
     DescribeChannelResponseTypeDef,
     RotateChannelCredentialsResponseTypeDef,
     RotateIngestEndpointCredentialsResponseTypeDef,
     UpdateChannelResponseTypeDef,
-    CmafPackageCreateOrUpdateParametersTypeDef,
     CmafPackageTypeDef,
+    DashPackageOutputTypeDef,
+    HlsPackageOutputTypeDef,
+    MssPackageOutputTypeDef,
+    CmafPackageCreateOrUpdateParametersTypeDef,
     DashPackageTypeDef,
     HlsPackageTypeDef,
     MssPackageTypeDef,
     ListChannelsResponseTypeDef,
-    CreateOriginEndpointRequestRequestTypeDef,
     CreateOriginEndpointResponseTypeDef,
     DescribeOriginEndpointResponseTypeDef,
     OriginEndpointTypeDef,
-    UpdateOriginEndpointRequestRequestTypeDef,
     UpdateOriginEndpointResponseTypeDef,
+    CreateOriginEndpointRequestRequestTypeDef,
+    UpdateOriginEndpointRequestRequestTypeDef,
     ListOriginEndpointsResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationTypeDef:
+def get_structure() -> AuthorizationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/__init__.py` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/__init__.pyi` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/__main__.py` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaPackage 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.MediaPackage 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage\nOther"
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

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/client.py` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/client.pyi` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/literals.py` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,15 @@
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
@@ -292,26 +293,28 @@
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
@@ -458,14 +461,15 @@
 PaginatorName = Literal["list_channels", "list_harvest_jobs", "list_origin_endpoints"]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/literals.pyi` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
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
@@ -290,26 +291,28 @@
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
@@ -456,14 +459,15 @@
 PaginatorName = Literal["list_channels", "list_harvest_jobs", "list_origin_endpoints"]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/paginator.py` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/paginator.pyi` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/type_defs.py` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for mediapackage service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediapackage.type_defs import AuthorizationTypeDef
+    from mypy_boto3_mediapackage.type_defs import AuthorizationOutputTypeDef
 
-    data: AuthorizationTypeDef = {...}
+    data: AuthorizationOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdMarkersType,
@@ -37,30 +37,35 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AuthorizationOutputTypeDef",
     "AuthorizationTypeDef",
-    "EgressAccessLogsTypeDef",
-    "IngressAccessLogsTypeDef",
+    "EgressAccessLogsOutputTypeDef",
+    "IngressAccessLogsOutputTypeDef",
     "HlsManifestCreateOrUpdateParametersTypeDef",
     "StreamSelectionTypeDef",
     "HlsManifestTypeDef",
+    "StreamSelectionOutputTypeDef",
+    "EgressAccessLogsTypeDef",
+    "IngressAccessLogsTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "S3DestinationTypeDef",
+    "S3DestinationOutputTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeHarvestJobRequestRequestTypeDef",
     "DescribeOriginEndpointRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionContractConfigurationOutputTypeDef",
     "EncryptionContractConfigurationTypeDef",
     "IngestEndpointTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
     "ListHarvestJobsRequestRequestTypeDef",
     "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
@@ -75,61 +80,77 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "ConfigureLogsRequestRequestTypeDef",
     "CreateHarvestJobRequestRequestTypeDef",
     "CreateHarvestJobResponseTypeDef",
     "DescribeHarvestJobResponseTypeDef",
     "HarvestJobTypeDef",
+    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "HlsIngestTypeDef",
     "ListHarvestJobsResponseTypeDef",
+    "CmafEncryptionOutputTypeDef",
+    "DashEncryptionOutputTypeDef",
+    "HlsEncryptionOutputTypeDef",
+    "MssEncryptionOutputTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
     "HlsEncryptionTypeDef",
     "MssEncryptionTypeDef",
     "ChannelTypeDef",
     "ConfigureLogsResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "RotateChannelCredentialsResponseTypeDef",
     "RotateIngestEndpointCredentialsResponseTypeDef",
     "UpdateChannelResponseTypeDef",
-    "CmafPackageCreateOrUpdateParametersTypeDef",
     "CmafPackageTypeDef",
+    "DashPackageOutputTypeDef",
+    "HlsPackageOutputTypeDef",
+    "MssPackageOutputTypeDef",
+    "CmafPackageCreateOrUpdateParametersTypeDef",
     "DashPackageTypeDef",
     "HlsPackageTypeDef",
     "MssPackageTypeDef",
     "ListChannelsResponseTypeDef",
-    "CreateOriginEndpointRequestRequestTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "DescribeOriginEndpointResponseTypeDef",
     "OriginEndpointTypeDef",
-    "UpdateOriginEndpointRequestRequestTypeDef",
     "UpdateOriginEndpointResponseTypeDef",
+    "CreateOriginEndpointRequestRequestTypeDef",
+    "UpdateOriginEndpointRequestRequestTypeDef",
     "ListOriginEndpointsResponseTypeDef",
 )
 
+AuthorizationOutputTypeDef = TypedDict(
+    "AuthorizationOutputTypeDef",
+    {
+        "CdnIdentifierSecret": str,
+        "SecretsRoleArn": str,
+    },
+)
+
 AuthorizationTypeDef = TypedDict(
     "AuthorizationTypeDef",
     {
         "CdnIdentifierSecret": str,
         "SecretsRoleArn": str,
     },
 )
 
-EgressAccessLogsTypeDef = TypedDict(
-    "EgressAccessLogsTypeDef",
+EgressAccessLogsOutputTypeDef = TypedDict(
+    "EgressAccessLogsOutputTypeDef",
     {
         "LogGroupName": str,
     },
     total=False,
 )
 
-IngressAccessLogsTypeDef = TypedDict(
-    "IngressAccessLogsTypeDef",
+IngressAccessLogsOutputTypeDef = TypedDict(
+    "IngressAccessLogsOutputTypeDef",
     {
         "LogGroupName": str,
     },
     total=False,
 )
 
 _RequiredHlsManifestCreateOrUpdateParametersTypeDef = TypedDict(
@@ -149,22 +170,20 @@
         "PlaylistType": PlaylistTypeType,
         "PlaylistWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class HlsManifestCreateOrUpdateParametersTypeDef(
     _RequiredHlsManifestCreateOrUpdateParametersTypeDef,
     _OptionalHlsManifestCreateOrUpdateParametersTypeDef,
 ):
     pass
 
-
 StreamSelectionTypeDef = TypedDict(
     "StreamSelectionTypeDef",
     {
         "MaxVideoBitsPerSecond": int,
         "MinVideoBitsPerSecond": int,
         "StreamOrder": StreamOrderType,
     },
@@ -189,18 +208,42 @@
         "Url": str,
         "AdTriggers": List[AdTriggersElementType],
         "AdsOnDeliveryRestrictions": AdsOnDeliveryRestrictionsType,
     },
     total=False,
 )
 
-
 class HlsManifestTypeDef(_RequiredHlsManifestTypeDef, _OptionalHlsManifestTypeDef):
     pass
 
+StreamSelectionOutputTypeDef = TypedDict(
+    "StreamSelectionOutputTypeDef",
+    {
+        "MaxVideoBitsPerSecond": int,
+        "MinVideoBitsPerSecond": int,
+        "StreamOrder": StreamOrderType,
+    },
+    total=False,
+)
+
+EgressAccessLogsTypeDef = TypedDict(
+    "EgressAccessLogsTypeDef",
+    {
+        "LogGroupName": str,
+    },
+    total=False,
+)
+
+IngressAccessLogsTypeDef = TypedDict(
+    "IngressAccessLogsTypeDef",
+    {
+        "LogGroupName": str,
+    },
+    total=False,
+)
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
@@ -209,30 +252,37 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "BucketName": str,
         "ManifestKey": str,
         "RoleArn": str,
     },
 )
 
+S3DestinationOutputTypeDef = TypedDict(
+    "S3DestinationOutputTypeDef",
+    {
+        "BucketName": str,
+        "ManifestKey": str,
+        "RoleArn": str,
+    },
+)
+
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -267,14 +317,22 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionContractConfigurationOutputTypeDef = TypedDict(
+    "EncryptionContractConfigurationOutputTypeDef",
+    {
+        "PresetSpeke20Audio": PresetSpeke20AudioType,
+        "PresetSpeke20Video": PresetSpeke20VideoType,
+    },
+)
+
 EncryptionContractConfigurationTypeDef = TypedDict(
     "EncryptionContractConfigurationTypeDef",
     {
         "PresetSpeke20Audio": PresetSpeke20AudioType,
         "PresetSpeke20Video": PresetSpeke20VideoType,
     },
 )
@@ -424,21 +482,19 @@
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredConfigureLogsRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureLogsRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalConfigureLogsRequestRequestTypeDef = TypedDict(
@@ -446,21 +502,19 @@
     {
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
     },
     total=False,
 )
 
-
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
-
 CreateHarvestJobRequestRequestTypeDef = TypedDict(
     "CreateHarvestJobRequestRequestTypeDef",
     {
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
         "S3Destination": S3DestinationTypeDef,
@@ -473,15 +527,15 @@
     {
         "Arn": str,
         "ChannelId": str,
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
-        "S3Destination": S3DestinationTypeDef,
+        "S3Destination": S3DestinationOutputTypeDef,
         "StartTime": str,
         "Status": StatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeHarvestJobResponseTypeDef = TypedDict(
@@ -489,15 +543,15 @@
     {
         "Arn": str,
         "ChannelId": str,
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
-        "S3Destination": S3DestinationTypeDef,
+        "S3Destination": S3DestinationOutputTypeDef,
         "StartTime": str,
         "Status": StatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HarvestJobTypeDef = TypedDict(
@@ -505,21 +559,44 @@
     {
         "Arn": str,
         "ChannelId": str,
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
-        "S3Destination": S3DestinationTypeDef,
+        "S3Destination": S3DestinationOutputTypeDef,
         "StartTime": str,
         "Status": StatusType,
     },
     total=False,
 )
 
+_RequiredSpekeKeyProviderOutputTypeDef = TypedDict(
+    "_RequiredSpekeKeyProviderOutputTypeDef",
+    {
+        "ResourceId": str,
+        "RoleArn": str,
+        "SystemIds": List[str],
+        "Url": str,
+    },
+)
+_OptionalSpekeKeyProviderOutputTypeDef = TypedDict(
+    "_OptionalSpekeKeyProviderOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "EncryptionContractConfiguration": EncryptionContractConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class SpekeKeyProviderOutputTypeDef(
+    _RequiredSpekeKeyProviderOutputTypeDef, _OptionalSpekeKeyProviderOutputTypeDef
+):
+    pass
+
 _RequiredSpekeKeyProviderTypeDef = TypedDict(
     "_RequiredSpekeKeyProviderTypeDef",
     {
         "ResourceId": str,
         "RoleArn": str,
         "SystemIds": Sequence[str],
         "Url": str,
@@ -530,19 +607,17 @@
     {
         "CertificateArn": str,
         "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class SpekeKeyProviderTypeDef(_RequiredSpekeKeyProviderTypeDef, _OptionalSpekeKeyProviderTypeDef):
     pass
 
-
 HlsIngestTypeDef = TypedDict(
     "HlsIngestTypeDef",
     {
         "IngestEndpoints": List[IngestEndpointTypeDef],
     },
     total=False,
 )
@@ -552,14 +627,83 @@
     {
         "HarvestJobs": List[HarvestJobTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCmafEncryptionOutputTypeDef = TypedDict(
+    "_RequiredCmafEncryptionOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+_OptionalCmafEncryptionOutputTypeDef = TypedDict(
+    "_OptionalCmafEncryptionOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "EncryptionMethod": CmafEncryptionMethodType,
+        "KeyRotationIntervalSeconds": int,
+    },
+    total=False,
+)
+
+class CmafEncryptionOutputTypeDef(
+    _RequiredCmafEncryptionOutputTypeDef, _OptionalCmafEncryptionOutputTypeDef
+):
+    pass
+
+_RequiredDashEncryptionOutputTypeDef = TypedDict(
+    "_RequiredDashEncryptionOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+_OptionalDashEncryptionOutputTypeDef = TypedDict(
+    "_OptionalDashEncryptionOutputTypeDef",
+    {
+        "KeyRotationIntervalSeconds": int,
+    },
+    total=False,
+)
+
+class DashEncryptionOutputTypeDef(
+    _RequiredDashEncryptionOutputTypeDef, _OptionalDashEncryptionOutputTypeDef
+):
+    pass
+
+_RequiredHlsEncryptionOutputTypeDef = TypedDict(
+    "_RequiredHlsEncryptionOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+_OptionalHlsEncryptionOutputTypeDef = TypedDict(
+    "_OptionalHlsEncryptionOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "EncryptionMethod": EncryptionMethodType,
+        "KeyRotationIntervalSeconds": int,
+        "RepeatExtXKey": bool,
+    },
+    total=False,
+)
+
+class HlsEncryptionOutputTypeDef(
+    _RequiredHlsEncryptionOutputTypeDef, _OptionalHlsEncryptionOutputTypeDef
+):
+    pass
+
+MssEncryptionOutputTypeDef = TypedDict(
+    "MssEncryptionOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+
 _RequiredCmafEncryptionTypeDef = TypedDict(
     "_RequiredCmafEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 _OptionalCmafEncryptionTypeDef = TypedDict(
@@ -568,38 +712,34 @@
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionMethodType,
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class CmafEncryptionTypeDef(_RequiredCmafEncryptionTypeDef, _OptionalCmafEncryptionTypeDef):
     pass
 
-
 _RequiredDashEncryptionTypeDef = TypedDict(
     "_RequiredDashEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 _OptionalDashEncryptionTypeDef = TypedDict(
     "_OptionalDashEncryptionTypeDef",
     {
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
-
 class DashEncryptionTypeDef(_RequiredDashEncryptionTypeDef, _OptionalDashEncryptionTypeDef):
     pass
 
-
 _RequiredHlsEncryptionTypeDef = TypedDict(
     "_RequiredHlsEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 _OptionalHlsEncryptionTypeDef = TypedDict(
@@ -609,148 +749,199 @@
         "EncryptionMethod": EncryptionMethodType,
         "KeyRotationIntervalSeconds": int,
         "RepeatExtXKey": bool,
     },
     total=False,
 )
 
-
 class HlsEncryptionTypeDef(_RequiredHlsEncryptionTypeDef, _OptionalHlsEncryptionTypeDef):
     pass
 
-
 MssEncryptionTypeDef = TypedDict(
     "MssEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
 ConfigureLogsResponseTypeDef = TypedDict(
     "ConfigureLogsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RotateChannelCredentialsResponseTypeDef = TypedDict(
     "RotateChannelCredentialsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RotateIngestEndpointCredentialsResponseTypeDef = TypedDict(
     "RotateIngestEndpointCredentialsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CmafPackageCreateOrUpdateParametersTypeDef = TypedDict(
-    "CmafPackageCreateOrUpdateParametersTypeDef",
+CmafPackageTypeDef = TypedDict(
+    "CmafPackageTypeDef",
     {
-        "Encryption": CmafEncryptionTypeDef,
-        "HlsManifests": Sequence[HlsManifestCreateOrUpdateParametersTypeDef],
+        "Encryption": CmafEncryptionOutputTypeDef,
+        "HlsManifests": List[HlsManifestTypeDef],
         "SegmentDurationSeconds": int,
         "SegmentPrefix": str,
-        "StreamSelection": StreamSelectionTypeDef,
+        "StreamSelection": StreamSelectionOutputTypeDef,
     },
     total=False,
 )
 
-CmafPackageTypeDef = TypedDict(
-    "CmafPackageTypeDef",
+DashPackageOutputTypeDef = TypedDict(
+    "DashPackageOutputTypeDef",
+    {
+        "AdTriggers": List[AdTriggersElementType],
+        "AdsOnDeliveryRestrictions": AdsOnDeliveryRestrictionsType,
+        "Encryption": DashEncryptionOutputTypeDef,
+        "IncludeIframeOnlyStream": bool,
+        "ManifestLayout": ManifestLayoutType,
+        "ManifestWindowSeconds": int,
+        "MinBufferTimeSeconds": int,
+        "MinUpdatePeriodSeconds": int,
+        "PeriodTriggers": List[Literal["ADS"]],
+        "Profile": ProfileType,
+        "SegmentDurationSeconds": int,
+        "SegmentTemplateFormat": SegmentTemplateFormatType,
+        "StreamSelection": StreamSelectionOutputTypeDef,
+        "SuggestedPresentationDelaySeconds": int,
+        "UtcTiming": UtcTimingType,
+        "UtcTimingUri": str,
+    },
+    total=False,
+)
+
+HlsPackageOutputTypeDef = TypedDict(
+    "HlsPackageOutputTypeDef",
+    {
+        "AdMarkers": AdMarkersType,
+        "AdTriggers": List[AdTriggersElementType],
+        "AdsOnDeliveryRestrictions": AdsOnDeliveryRestrictionsType,
+        "Encryption": HlsEncryptionOutputTypeDef,
+        "IncludeDvbSubtitles": bool,
+        "IncludeIframeOnlyStream": bool,
+        "PlaylistType": PlaylistTypeType,
+        "PlaylistWindowSeconds": int,
+        "ProgramDateTimeIntervalSeconds": int,
+        "SegmentDurationSeconds": int,
+        "StreamSelection": StreamSelectionOutputTypeDef,
+        "UseAudioRenditionGroup": bool,
+    },
+    total=False,
+)
+
+MssPackageOutputTypeDef = TypedDict(
+    "MssPackageOutputTypeDef",
+    {
+        "Encryption": MssEncryptionOutputTypeDef,
+        "ManifestWindowSeconds": int,
+        "SegmentDurationSeconds": int,
+        "StreamSelection": StreamSelectionOutputTypeDef,
+    },
+    total=False,
+)
+
+CmafPackageCreateOrUpdateParametersTypeDef = TypedDict(
+    "CmafPackageCreateOrUpdateParametersTypeDef",
     {
         "Encryption": CmafEncryptionTypeDef,
-        "HlsManifests": List[HlsManifestTypeDef],
+        "HlsManifests": Sequence[HlsManifestCreateOrUpdateParametersTypeDef],
         "SegmentDurationSeconds": int,
         "SegmentPrefix": str,
         "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
@@ -812,176 +1003,172 @@
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
+CreateOriginEndpointResponseTypeDef = TypedDict(
+    "CreateOriginEndpointResponseTypeDef",
     {
+        "Arn": str,
+        "Authorization": AuthorizationOutputTypeDef,
         "ChannelId": str,
-        "Id": str,
-    },
-)
-_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
-    {
-        "Authorization": AuthorizationTypeDef,
-        "CmafPackage": CmafPackageCreateOrUpdateParametersTypeDef,
-        "DashPackage": DashPackageTypeDef,
+        "CmafPackage": CmafPackageTypeDef,
+        "CreatedAt": str,
+        "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
+        "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
-        "Tags": Mapping[str, str],
+        "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
-        "Whitelist": Sequence[str],
+        "Url": str,
+        "Whitelist": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class CreateOriginEndpointRequestRequestTypeDef(
-    _RequiredCreateOriginEndpointRequestRequestTypeDef,
-    _OptionalCreateOriginEndpointRequestRequestTypeDef,
-):
-    pass
-
-
-CreateOriginEndpointResponseTypeDef = TypedDict(
-    "CreateOriginEndpointResponseTypeDef",
+DescribeOriginEndpointResponseTypeDef = TypedDict(
+    "DescribeOriginEndpointResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageTypeDef,
+        "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeOriginEndpointResponseTypeDef = TypedDict(
-    "DescribeOriginEndpointResponseTypeDef",
+OriginEndpointTypeDef = TypedDict(
+    "OriginEndpointTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageTypeDef,
+        "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-OriginEndpointTypeDef = TypedDict(
-    "OriginEndpointTypeDef",
+UpdateOriginEndpointResponseTypeDef = TypedDict(
+    "UpdateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageTypeDef,
+        "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
+_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
+        "ChannelId": str,
         "Id": str,
     },
 )
-_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
+_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
     {
         "Authorization": AuthorizationTypeDef,
         "CmafPackage": CmafPackageCreateOrUpdateParametersTypeDef,
         "DashPackage": DashPackageTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageTypeDef,
         "ManifestName": str,
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
+        "Tags": Mapping[str, str],
         "TimeDelaySeconds": int,
         "Whitelist": Sequence[str],
     },
     total=False,
 )
 
-
-class UpdateOriginEndpointRequestRequestTypeDef(
-    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
-    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
+class CreateOriginEndpointRequestRequestTypeDef(
+    _RequiredCreateOriginEndpointRequestRequestTypeDef,
+    _OptionalCreateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateOriginEndpointResponseTypeDef = TypedDict(
-    "UpdateOriginEndpointResponseTypeDef",
+_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
     {
-        "Arn": str,
         "Authorization": AuthorizationTypeDef,
-        "ChannelId": str,
-        "CmafPackage": CmafPackageTypeDef,
-        "CreatedAt": str,
+        "CmafPackage": CmafPackageCreateOrUpdateParametersTypeDef,
         "DashPackage": DashPackageTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageTypeDef,
-        "Id": str,
         "ManifestName": str,
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
-        "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
-        "Url": str,
-        "Whitelist": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Whitelist": Sequence[str],
     },
+    total=False,
 )
 
+class UpdateOriginEndpointRequestRequestTypeDef(
+    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
+    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
+):
+    pass
+
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "NextToken": str,
         "OriginEndpoints": List[OriginEndpointTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/type_defs.pyi` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for mediapackage service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediapackage.type_defs import AuthorizationTypeDef
+    from mypy_boto3_mediapackage.type_defs import AuthorizationOutputTypeDef
 
-    data: AuthorizationTypeDef = {...}
+    data: AuthorizationOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdMarkersType,
@@ -37,29 +37,36 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AuthorizationOutputTypeDef",
     "AuthorizationTypeDef",
-    "EgressAccessLogsTypeDef",
-    "IngressAccessLogsTypeDef",
+    "EgressAccessLogsOutputTypeDef",
+    "IngressAccessLogsOutputTypeDef",
     "HlsManifestCreateOrUpdateParametersTypeDef",
     "StreamSelectionTypeDef",
     "HlsManifestTypeDef",
+    "StreamSelectionOutputTypeDef",
+    "EgressAccessLogsTypeDef",
+    "IngressAccessLogsTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "S3DestinationTypeDef",
+    "S3DestinationOutputTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DescribeHarvestJobRequestRequestTypeDef",
     "DescribeOriginEndpointRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionContractConfigurationOutputTypeDef",
     "EncryptionContractConfigurationTypeDef",
     "IngestEndpointTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListHarvestJobsRequestListHarvestJobsPaginateTypeDef",
     "ListHarvestJobsRequestRequestTypeDef",
     "ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef",
@@ -74,61 +81,77 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "ConfigureLogsRequestRequestTypeDef",
     "CreateHarvestJobRequestRequestTypeDef",
     "CreateHarvestJobResponseTypeDef",
     "DescribeHarvestJobResponseTypeDef",
     "HarvestJobTypeDef",
+    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "HlsIngestTypeDef",
     "ListHarvestJobsResponseTypeDef",
+    "CmafEncryptionOutputTypeDef",
+    "DashEncryptionOutputTypeDef",
+    "HlsEncryptionOutputTypeDef",
+    "MssEncryptionOutputTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
     "HlsEncryptionTypeDef",
     "MssEncryptionTypeDef",
     "ChannelTypeDef",
     "ConfigureLogsResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "RotateChannelCredentialsResponseTypeDef",
     "RotateIngestEndpointCredentialsResponseTypeDef",
     "UpdateChannelResponseTypeDef",
-    "CmafPackageCreateOrUpdateParametersTypeDef",
     "CmafPackageTypeDef",
+    "DashPackageOutputTypeDef",
+    "HlsPackageOutputTypeDef",
+    "MssPackageOutputTypeDef",
+    "CmafPackageCreateOrUpdateParametersTypeDef",
     "DashPackageTypeDef",
     "HlsPackageTypeDef",
     "MssPackageTypeDef",
     "ListChannelsResponseTypeDef",
-    "CreateOriginEndpointRequestRequestTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "DescribeOriginEndpointResponseTypeDef",
     "OriginEndpointTypeDef",
-    "UpdateOriginEndpointRequestRequestTypeDef",
     "UpdateOriginEndpointResponseTypeDef",
+    "CreateOriginEndpointRequestRequestTypeDef",
+    "UpdateOriginEndpointRequestRequestTypeDef",
     "ListOriginEndpointsResponseTypeDef",
 )
 
+AuthorizationOutputTypeDef = TypedDict(
+    "AuthorizationOutputTypeDef",
+    {
+        "CdnIdentifierSecret": str,
+        "SecretsRoleArn": str,
+    },
+)
+
 AuthorizationTypeDef = TypedDict(
     "AuthorizationTypeDef",
     {
         "CdnIdentifierSecret": str,
         "SecretsRoleArn": str,
     },
 )
 
-EgressAccessLogsTypeDef = TypedDict(
-    "EgressAccessLogsTypeDef",
+EgressAccessLogsOutputTypeDef = TypedDict(
+    "EgressAccessLogsOutputTypeDef",
     {
         "LogGroupName": str,
     },
     total=False,
 )
 
-IngressAccessLogsTypeDef = TypedDict(
-    "IngressAccessLogsTypeDef",
+IngressAccessLogsOutputTypeDef = TypedDict(
+    "IngressAccessLogsOutputTypeDef",
     {
         "LogGroupName": str,
     },
     total=False,
 )
 
 _RequiredHlsManifestCreateOrUpdateParametersTypeDef = TypedDict(
@@ -148,20 +171,22 @@
         "PlaylistType": PlaylistTypeType,
         "PlaylistWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class HlsManifestCreateOrUpdateParametersTypeDef(
     _RequiredHlsManifestCreateOrUpdateParametersTypeDef,
     _OptionalHlsManifestCreateOrUpdateParametersTypeDef,
 ):
     pass
 
+
 StreamSelectionTypeDef = TypedDict(
     "StreamSelectionTypeDef",
     {
         "MaxVideoBitsPerSecond": int,
         "MinVideoBitsPerSecond": int,
         "StreamOrder": StreamOrderType,
     },
@@ -186,17 +211,45 @@
         "Url": str,
         "AdTriggers": List[AdTriggersElementType],
         "AdsOnDeliveryRestrictions": AdsOnDeliveryRestrictionsType,
     },
     total=False,
 )
 
+
 class HlsManifestTypeDef(_RequiredHlsManifestTypeDef, _OptionalHlsManifestTypeDef):
     pass
 
+
+StreamSelectionOutputTypeDef = TypedDict(
+    "StreamSelectionOutputTypeDef",
+    {
+        "MaxVideoBitsPerSecond": int,
+        "MinVideoBitsPerSecond": int,
+        "StreamOrder": StreamOrderType,
+    },
+    total=False,
+)
+
+EgressAccessLogsTypeDef = TypedDict(
+    "EgressAccessLogsTypeDef",
+    {
+        "LogGroupName": str,
+    },
+    total=False,
+)
+
+IngressAccessLogsTypeDef = TypedDict(
+    "IngressAccessLogsTypeDef",
+    {
+        "LogGroupName": str,
+    },
+    total=False,
+)
+
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalCreateChannelRequestRequestTypeDef = TypedDict(
@@ -204,28 +257,39 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
+
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "BucketName": str,
         "ManifestKey": str,
         "RoleArn": str,
     },
 )
 
+S3DestinationOutputTypeDef = TypedDict(
+    "S3DestinationOutputTypeDef",
+    {
+        "BucketName": str,
+        "ManifestKey": str,
+        "RoleArn": str,
+    },
+)
+
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -260,14 +324,22 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionContractConfigurationOutputTypeDef = TypedDict(
+    "EncryptionContractConfigurationOutputTypeDef",
+    {
+        "PresetSpeke20Audio": PresetSpeke20AudioType,
+        "PresetSpeke20Video": PresetSpeke20VideoType,
+    },
+)
+
 EncryptionContractConfigurationTypeDef = TypedDict(
     "EncryptionContractConfigurationTypeDef",
     {
         "PresetSpeke20Audio": PresetSpeke20AudioType,
         "PresetSpeke20Video": PresetSpeke20VideoType,
     },
 )
@@ -417,19 +489,21 @@
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredConfigureLogsRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureLogsRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalConfigureLogsRequestRequestTypeDef = TypedDict(
@@ -437,19 +511,21 @@
     {
         "EgressAccessLogs": EgressAccessLogsTypeDef,
         "IngressAccessLogs": IngressAccessLogsTypeDef,
     },
     total=False,
 )
 
+
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
+
 CreateHarvestJobRequestRequestTypeDef = TypedDict(
     "CreateHarvestJobRequestRequestTypeDef",
     {
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
         "S3Destination": S3DestinationTypeDef,
@@ -462,15 +538,15 @@
     {
         "Arn": str,
         "ChannelId": str,
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
-        "S3Destination": S3DestinationTypeDef,
+        "S3Destination": S3DestinationOutputTypeDef,
         "StartTime": str,
         "Status": StatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeHarvestJobResponseTypeDef = TypedDict(
@@ -478,15 +554,15 @@
     {
         "Arn": str,
         "ChannelId": str,
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
-        "S3Destination": S3DestinationTypeDef,
+        "S3Destination": S3DestinationOutputTypeDef,
         "StartTime": str,
         "Status": StatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 HarvestJobTypeDef = TypedDict(
@@ -494,21 +570,46 @@
     {
         "Arn": str,
         "ChannelId": str,
         "CreatedAt": str,
         "EndTime": str,
         "Id": str,
         "OriginEndpointId": str,
-        "S3Destination": S3DestinationTypeDef,
+        "S3Destination": S3DestinationOutputTypeDef,
         "StartTime": str,
         "Status": StatusType,
     },
     total=False,
 )
 
+_RequiredSpekeKeyProviderOutputTypeDef = TypedDict(
+    "_RequiredSpekeKeyProviderOutputTypeDef",
+    {
+        "ResourceId": str,
+        "RoleArn": str,
+        "SystemIds": List[str],
+        "Url": str,
+    },
+)
+_OptionalSpekeKeyProviderOutputTypeDef = TypedDict(
+    "_OptionalSpekeKeyProviderOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "EncryptionContractConfiguration": EncryptionContractConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class SpekeKeyProviderOutputTypeDef(
+    _RequiredSpekeKeyProviderOutputTypeDef, _OptionalSpekeKeyProviderOutputTypeDef
+):
+    pass
+
+
 _RequiredSpekeKeyProviderTypeDef = TypedDict(
     "_RequiredSpekeKeyProviderTypeDef",
     {
         "ResourceId": str,
         "RoleArn": str,
         "SystemIds": Sequence[str],
         "Url": str,
@@ -519,17 +620,19 @@
     {
         "CertificateArn": str,
         "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class SpekeKeyProviderTypeDef(_RequiredSpekeKeyProviderTypeDef, _OptionalSpekeKeyProviderTypeDef):
     pass
 
+
 HlsIngestTypeDef = TypedDict(
     "HlsIngestTypeDef",
     {
         "IngestEndpoints": List[IngestEndpointTypeDef],
     },
     total=False,
 )
@@ -539,14 +642,89 @@
     {
         "HarvestJobs": List[HarvestJobTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCmafEncryptionOutputTypeDef = TypedDict(
+    "_RequiredCmafEncryptionOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+_OptionalCmafEncryptionOutputTypeDef = TypedDict(
+    "_OptionalCmafEncryptionOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "EncryptionMethod": CmafEncryptionMethodType,
+        "KeyRotationIntervalSeconds": int,
+    },
+    total=False,
+)
+
+
+class CmafEncryptionOutputTypeDef(
+    _RequiredCmafEncryptionOutputTypeDef, _OptionalCmafEncryptionOutputTypeDef
+):
+    pass
+
+
+_RequiredDashEncryptionOutputTypeDef = TypedDict(
+    "_RequiredDashEncryptionOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+_OptionalDashEncryptionOutputTypeDef = TypedDict(
+    "_OptionalDashEncryptionOutputTypeDef",
+    {
+        "KeyRotationIntervalSeconds": int,
+    },
+    total=False,
+)
+
+
+class DashEncryptionOutputTypeDef(
+    _RequiredDashEncryptionOutputTypeDef, _OptionalDashEncryptionOutputTypeDef
+):
+    pass
+
+
+_RequiredHlsEncryptionOutputTypeDef = TypedDict(
+    "_RequiredHlsEncryptionOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+_OptionalHlsEncryptionOutputTypeDef = TypedDict(
+    "_OptionalHlsEncryptionOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "EncryptionMethod": EncryptionMethodType,
+        "KeyRotationIntervalSeconds": int,
+        "RepeatExtXKey": bool,
+    },
+    total=False,
+)
+
+
+class HlsEncryptionOutputTypeDef(
+    _RequiredHlsEncryptionOutputTypeDef, _OptionalHlsEncryptionOutputTypeDef
+):
+    pass
+
+
+MssEncryptionOutputTypeDef = TypedDict(
+    "MssEncryptionOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+
 _RequiredCmafEncryptionTypeDef = TypedDict(
     "_RequiredCmafEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 _OptionalCmafEncryptionTypeDef = TypedDict(
@@ -555,34 +733,38 @@
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionMethodType,
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class CmafEncryptionTypeDef(_RequiredCmafEncryptionTypeDef, _OptionalCmafEncryptionTypeDef):
     pass
 
+
 _RequiredDashEncryptionTypeDef = TypedDict(
     "_RequiredDashEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 _OptionalDashEncryptionTypeDef = TypedDict(
     "_OptionalDashEncryptionTypeDef",
     {
         "KeyRotationIntervalSeconds": int,
     },
     total=False,
 )
 
+
 class DashEncryptionTypeDef(_RequiredDashEncryptionTypeDef, _OptionalDashEncryptionTypeDef):
     pass
 
+
 _RequiredHlsEncryptionTypeDef = TypedDict(
     "_RequiredHlsEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 _OptionalHlsEncryptionTypeDef = TypedDict(
@@ -592,146 +774,201 @@
         "EncryptionMethod": EncryptionMethodType,
         "KeyRotationIntervalSeconds": int,
         "RepeatExtXKey": bool,
     },
     total=False,
 )
 
+
 class HlsEncryptionTypeDef(_RequiredHlsEncryptionTypeDef, _OptionalHlsEncryptionTypeDef):
     pass
 
+
 MssEncryptionTypeDef = TypedDict(
     "MssEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
 ConfigureLogsResponseTypeDef = TypedDict(
     "ConfigureLogsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RotateChannelCredentialsResponseTypeDef = TypedDict(
     "RotateChannelCredentialsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RotateIngestEndpointCredentialsResponseTypeDef = TypedDict(
     "RotateIngestEndpointCredentialsResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": str,
         "Description": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "HlsIngest": HlsIngestTypeDef,
         "Id": str,
-        "IngressAccessLogs": IngressAccessLogsTypeDef,
+        "IngressAccessLogs": IngressAccessLogsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CmafPackageCreateOrUpdateParametersTypeDef = TypedDict(
-    "CmafPackageCreateOrUpdateParametersTypeDef",
+CmafPackageTypeDef = TypedDict(
+    "CmafPackageTypeDef",
     {
-        "Encryption": CmafEncryptionTypeDef,
-        "HlsManifests": Sequence[HlsManifestCreateOrUpdateParametersTypeDef],
+        "Encryption": CmafEncryptionOutputTypeDef,
+        "HlsManifests": List[HlsManifestTypeDef],
         "SegmentDurationSeconds": int,
         "SegmentPrefix": str,
-        "StreamSelection": StreamSelectionTypeDef,
+        "StreamSelection": StreamSelectionOutputTypeDef,
     },
     total=False,
 )
 
-CmafPackageTypeDef = TypedDict(
-    "CmafPackageTypeDef",
+DashPackageOutputTypeDef = TypedDict(
+    "DashPackageOutputTypeDef",
+    {
+        "AdTriggers": List[AdTriggersElementType],
+        "AdsOnDeliveryRestrictions": AdsOnDeliveryRestrictionsType,
+        "Encryption": DashEncryptionOutputTypeDef,
+        "IncludeIframeOnlyStream": bool,
+        "ManifestLayout": ManifestLayoutType,
+        "ManifestWindowSeconds": int,
+        "MinBufferTimeSeconds": int,
+        "MinUpdatePeriodSeconds": int,
+        "PeriodTriggers": List[Literal["ADS"]],
+        "Profile": ProfileType,
+        "SegmentDurationSeconds": int,
+        "SegmentTemplateFormat": SegmentTemplateFormatType,
+        "StreamSelection": StreamSelectionOutputTypeDef,
+        "SuggestedPresentationDelaySeconds": int,
+        "UtcTiming": UtcTimingType,
+        "UtcTimingUri": str,
+    },
+    total=False,
+)
+
+HlsPackageOutputTypeDef = TypedDict(
+    "HlsPackageOutputTypeDef",
+    {
+        "AdMarkers": AdMarkersType,
+        "AdTriggers": List[AdTriggersElementType],
+        "AdsOnDeliveryRestrictions": AdsOnDeliveryRestrictionsType,
+        "Encryption": HlsEncryptionOutputTypeDef,
+        "IncludeDvbSubtitles": bool,
+        "IncludeIframeOnlyStream": bool,
+        "PlaylistType": PlaylistTypeType,
+        "PlaylistWindowSeconds": int,
+        "ProgramDateTimeIntervalSeconds": int,
+        "SegmentDurationSeconds": int,
+        "StreamSelection": StreamSelectionOutputTypeDef,
+        "UseAudioRenditionGroup": bool,
+    },
+    total=False,
+)
+
+MssPackageOutputTypeDef = TypedDict(
+    "MssPackageOutputTypeDef",
+    {
+        "Encryption": MssEncryptionOutputTypeDef,
+        "ManifestWindowSeconds": int,
+        "SegmentDurationSeconds": int,
+        "StreamSelection": StreamSelectionOutputTypeDef,
+    },
+    total=False,
+)
+
+CmafPackageCreateOrUpdateParametersTypeDef = TypedDict(
+    "CmafPackageCreateOrUpdateParametersTypeDef",
     {
         "Encryption": CmafEncryptionTypeDef,
-        "HlsManifests": List[HlsManifestTypeDef],
+        "HlsManifests": Sequence[HlsManifestCreateOrUpdateParametersTypeDef],
         "SegmentDurationSeconds": int,
         "SegmentPrefix": str,
         "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
@@ -793,172 +1030,176 @@
     {
         "Channels": List[ChannelTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
+CreateOriginEndpointResponseTypeDef = TypedDict(
+    "CreateOriginEndpointResponseTypeDef",
     {
+        "Arn": str,
+        "Authorization": AuthorizationOutputTypeDef,
         "ChannelId": str,
-        "Id": str,
-    },
-)
-_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
-    {
-        "Authorization": AuthorizationTypeDef,
-        "CmafPackage": CmafPackageCreateOrUpdateParametersTypeDef,
-        "DashPackage": DashPackageTypeDef,
+        "CmafPackage": CmafPackageTypeDef,
+        "CreatedAt": str,
+        "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
+        "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
-        "Tags": Mapping[str, str],
+        "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
-        "Whitelist": Sequence[str],
+        "Url": str,
+        "Whitelist": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class CreateOriginEndpointRequestRequestTypeDef(
-    _RequiredCreateOriginEndpointRequestRequestTypeDef,
-    _OptionalCreateOriginEndpointRequestRequestTypeDef,
-):
-    pass
-
-CreateOriginEndpointResponseTypeDef = TypedDict(
-    "CreateOriginEndpointResponseTypeDef",
+DescribeOriginEndpointResponseTypeDef = TypedDict(
+    "DescribeOriginEndpointResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageTypeDef,
+        "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeOriginEndpointResponseTypeDef = TypedDict(
-    "DescribeOriginEndpointResponseTypeDef",
+OriginEndpointTypeDef = TypedDict(
+    "OriginEndpointTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageTypeDef,
+        "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-OriginEndpointTypeDef = TypedDict(
-    "OriginEndpointTypeDef",
+UpdateOriginEndpointResponseTypeDef = TypedDict(
+    "UpdateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "ChannelId": str,
         "CmafPackage": CmafPackageTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageTypeDef,
+        "DashPackage": DashPackageOutputTypeDef,
         "Description": str,
-        "HlsPackage": HlsPackageTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
         "ManifestName": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
         "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
         "Url": str,
         "Whitelist": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
+_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
+        "ChannelId": str,
         "Id": str,
     },
 )
-_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
+_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
     {
         "Authorization": AuthorizationTypeDef,
         "CmafPackage": CmafPackageCreateOrUpdateParametersTypeDef,
         "DashPackage": DashPackageTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageTypeDef,
         "ManifestName": str,
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
+        "Tags": Mapping[str, str],
         "TimeDelaySeconds": int,
         "Whitelist": Sequence[str],
     },
     total=False,
 )
 
-class UpdateOriginEndpointRequestRequestTypeDef(
-    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
-    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
+
+class CreateOriginEndpointRequestRequestTypeDef(
+    _RequiredCreateOriginEndpointRequestRequestTypeDef,
+    _OptionalCreateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
-UpdateOriginEndpointResponseTypeDef = TypedDict(
-    "UpdateOriginEndpointResponseTypeDef",
+
+_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
     {
-        "Arn": str,
         "Authorization": AuthorizationTypeDef,
-        "ChannelId": str,
-        "CmafPackage": CmafPackageTypeDef,
-        "CreatedAt": str,
+        "CmafPackage": CmafPackageCreateOrUpdateParametersTypeDef,
         "DashPackage": DashPackageTypeDef,
         "Description": str,
         "HlsPackage": HlsPackageTypeDef,
-        "Id": str,
         "ManifestName": str,
         "MssPackage": MssPackageTypeDef,
         "Origination": OriginationType,
         "StartoverWindowSeconds": int,
-        "Tags": Dict[str, str],
         "TimeDelaySeconds": int,
-        "Url": str,
-        "Whitelist": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Whitelist": Sequence[str],
     },
+    total=False,
 )
 
+
+class UpdateOriginEndpointRequestRequestTypeDef(
+    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
+    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
+):
+    pass
+
+
 ListOriginEndpointsResponseTypeDef = TypedDict(
     "ListOriginEndpointsResponseTypeDef",
     {
         "NextToken": str,
         "OriginEndpoints": List[OriginEndpointTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/PKG-INFO` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage
-Version: 1.28.0
-Summary: Type annotations for boto3.MediaPackage 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MediaPackage 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediapackage"></a>
 
 # mypy-boto3-mediapackage
 
 [![PyPI - mypy-boto3-mediapackage](https://img.shields.io/pypi/v/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage)](https://pepy.tech/project/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
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
 [mypy-boto3-mediapackage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,28 +345,34 @@
 ### Typed dictionaries
 
 `mypy_boto3_mediapackage.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage.type_defs import (
+    AuthorizationOutputTypeDef,
     AuthorizationTypeDef,
-    EgressAccessLogsTypeDef,
-    IngressAccessLogsTypeDef,
+    EgressAccessLogsOutputTypeDef,
+    IngressAccessLogsOutputTypeDef,
     HlsManifestCreateOrUpdateParametersTypeDef,
     StreamSelectionTypeDef,
     HlsManifestTypeDef,
+    StreamSelectionOutputTypeDef,
+    EgressAccessLogsTypeDef,
+    IngressAccessLogsTypeDef,
     CreateChannelRequestRequestTypeDef,
     S3DestinationTypeDef,
+    S3DestinationOutputTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DescribeHarvestJobRequestRequestTypeDef,
     DescribeOriginEndpointRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
     IngestEndpointTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListHarvestJobsRequestListHarvestJobsPaginateTypeDef,
     ListHarvestJobsRequestRequestTypeDef,
     ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef,
@@ -381,45 +387,53 @@
     UntagResourceRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
     CreateHarvestJobRequestRequestTypeDef,
     CreateHarvestJobResponseTypeDef,
     DescribeHarvestJobResponseTypeDef,
     HarvestJobTypeDef,
+    SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     HlsIngestTypeDef,
     ListHarvestJobsResponseTypeDef,
+    CmafEncryptionOutputTypeDef,
+    DashEncryptionOutputTypeDef,
+    HlsEncryptionOutputTypeDef,
+    MssEncryptionOutputTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
     HlsEncryptionTypeDef,
     MssEncryptionTypeDef,
     ChannelTypeDef,
     ConfigureLogsResponseTypeDef,
     CreateChannelResponseTypeDef,
     DescribeChannelResponseTypeDef,
     RotateChannelCredentialsResponseTypeDef,
     RotateIngestEndpointCredentialsResponseTypeDef,
     UpdateChannelResponseTypeDef,
-    CmafPackageCreateOrUpdateParametersTypeDef,
     CmafPackageTypeDef,
+    DashPackageOutputTypeDef,
+    HlsPackageOutputTypeDef,
+    MssPackageOutputTypeDef,
+    CmafPackageCreateOrUpdateParametersTypeDef,
     DashPackageTypeDef,
     HlsPackageTypeDef,
     MssPackageTypeDef,
     ListChannelsResponseTypeDef,
-    CreateOriginEndpointRequestRequestTypeDef,
     CreateOriginEndpointResponseTypeDef,
     DescribeOriginEndpointResponseTypeDef,
     OriginEndpointTypeDef,
-    UpdateOriginEndpointRequestRequestTypeDef,
     UpdateOriginEndpointResponseTypeDef,
+    CreateOriginEndpointRequestRequestTypeDef,
+    UpdateOriginEndpointRequestRequestTypeDef,
     ListOriginEndpointsResponseTypeDef,
 )
 
 
-def get_structure() -> AuthorizationTypeDef:
+def get_structure() -> AuthorizationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/SOURCES.txt` & `mypy-boto3-mediapackage-1.28.12/mypy_boto3_mediapackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.28.0/setup.py` & `mypy-boto3-mediapackage-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackage",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_mediapackage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaPackage 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.MediaPackage 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

