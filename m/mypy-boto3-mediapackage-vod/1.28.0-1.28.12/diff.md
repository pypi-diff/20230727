# Comparing `tmp/mypy-boto3-mediapackage-vod-1.28.0.tar.gz` & `tmp/mypy-boto3-mediapackage-vod-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackage-vod-1.28.0.tar", last modified: Thu Jul  6 21:00:06 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackage-vod-1.28.12.tar", last modified: Thu Jul 27 05:35:01 2023, max compression
```

## Comparing `mypy-boto3-mediapackage-vod-1.28.0.tar` & `mypy-boto3-mediapackage-vod-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:06.138367 mypy-boto3-mediapackage-vod-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15702 2023-07-06 21:00:06.134367 mypy-boto3-mediapackage-vod-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:06.122367 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-07-06 20:47:20.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20122 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:19.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:06.134367 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15702 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:06.138367 mypy-boto3-mediapackage-vod-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-06 20:47:18.000000 mypy-boto3-mediapackage-vod-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.104441 mypy-boto3-mediapackage-vod-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-07-27 05:35:01.100441 mypy-boto3-mediapackage-vod-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14692 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.096441 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26582 2023-07-27 05:26:23.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.100441 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:35:00.000000 mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:01.104441 mypy-boto3-mediapackage-vod-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-27 05:26:21.000000 mypy-boto3-mediapackage-vod-1.28.12/setup.py
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/LICENSE` & `mypy-boto3-mediapackage-vod-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/PKG-INFO` & `mypy-boto3-mediapackage-vod-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage-vod
-Version: 1.28.0
-Summary: Type annotations for boto3.MediaPackageVod 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MediaPackageVod 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediapackage-vod"></a>
 
 # mypy-boto3-mediapackage-vod
 
 [![PyPI - mypy-boto3-mediapackage-vod](https://img.shields.io/pypi/v/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage-vod?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage-vod)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage-vod)](https://pepy.tech/project/mypy-boto3-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackageVod 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[boto3.MediaPackageVod 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,26 +343,30 @@
 
 `mypy_boto3_mediapackage_vod.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage_vod.type_defs import (
     AssetShallowTypeDef,
+    AuthorizationOutputTypeDef,
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
+    EgressAccessLogsOutputTypeDef,
     CreateAssetRequestRequestTypeDef,
     EgressEndpointTypeDef,
+    StreamSelectionOutputTypeDef,
     StreamSelectionTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeletePackagingConfigurationRequestRequestTypeDef,
     DeletePackagingGroupRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribePackagingConfigurationRequestRequestTypeDef,
     DescribePackagingGroupRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
     ListAssetsRequestListAssetsPaginateTypeDef,
     ListAssetsRequestRequestTypeDef,
     ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
     ListPackagingConfigurationsRequestRequestTypeDef,
     ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsRequestRequestTypeDef,
@@ -371,39 +375,51 @@
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ListAssetsResponseTypeDef,
     UpdatePackagingGroupRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
-    ConfigureLogsResponseTypeDef,
     CreatePackagingGroupRequestRequestTypeDef,
+    ConfigureLogsResponseTypeDef,
     CreatePackagingGroupResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
     PackagingGroupTypeDef,
     UpdatePackagingGroupResponseTypeDef,
     CreateAssetResponseTypeDef,
     DescribeAssetResponseTypeDef,
+    DashManifestOutputTypeDef,
+    HlsManifestOutputTypeDef,
+    MssManifestOutputTypeDef,
     DashManifestTypeDef,
     HlsManifestTypeDef,
     MssManifestTypeDef,
+    SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     ListPackagingGroupsResponseTypeDef,
+    CmafEncryptionOutputTypeDef,
+    DashEncryptionOutputTypeDef,
+    HlsEncryptionOutputTypeDef,
+    MssEncryptionOutputTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
     HlsEncryptionTypeDef,
     MssEncryptionTypeDef,
+    CmafPackageOutputTypeDef,
+    DashPackageOutputTypeDef,
+    HlsPackageOutputTypeDef,
+    MssPackageOutputTypeDef,
     CmafPackageTypeDef,
     DashPackageTypeDef,
     HlsPackageTypeDef,
     MssPackageTypeDef,
-    CreatePackagingConfigurationRequestRequestTypeDef,
     CreatePackagingConfigurationResponseTypeDef,
     DescribePackagingConfigurationResponseTypeDef,
     PackagingConfigurationTypeDef,
+    CreatePackagingConfigurationRequestRequestTypeDef,
     ListPackagingConfigurationsResponseTypeDef,
 )
 
 
 def get_structure() -> AssetShallowTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/README.md` & `mypy-boto3-mediapackage-vod-1.28.12/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mediapackage-vod"></a>
 
 # mypy-boto3-mediapackage-vod
 
 [![PyPI - mypy-boto3-mediapackage-vod](https://img.shields.io/pypi/v/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage-vod?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage-vod)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage-vod)](https://pepy.tech/project/mypy-boto3-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackageVod 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[boto3.MediaPackageVod 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,26 +311,30 @@
 
 `mypy_boto3_mediapackage_vod.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage_vod.type_defs import (
     AssetShallowTypeDef,
+    AuthorizationOutputTypeDef,
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
+    EgressAccessLogsOutputTypeDef,
     CreateAssetRequestRequestTypeDef,
     EgressEndpointTypeDef,
+    StreamSelectionOutputTypeDef,
     StreamSelectionTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeletePackagingConfigurationRequestRequestTypeDef,
     DeletePackagingGroupRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribePackagingConfigurationRequestRequestTypeDef,
     DescribePackagingGroupRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
     ListAssetsRequestListAssetsPaginateTypeDef,
     ListAssetsRequestRequestTypeDef,
     ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
     ListPackagingConfigurationsRequestRequestTypeDef,
     ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsRequestRequestTypeDef,
@@ -339,39 +343,51 @@
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ListAssetsResponseTypeDef,
     UpdatePackagingGroupRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
-    ConfigureLogsResponseTypeDef,
     CreatePackagingGroupRequestRequestTypeDef,
+    ConfigureLogsResponseTypeDef,
     CreatePackagingGroupResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
     PackagingGroupTypeDef,
     UpdatePackagingGroupResponseTypeDef,
     CreateAssetResponseTypeDef,
     DescribeAssetResponseTypeDef,
+    DashManifestOutputTypeDef,
+    HlsManifestOutputTypeDef,
+    MssManifestOutputTypeDef,
     DashManifestTypeDef,
     HlsManifestTypeDef,
     MssManifestTypeDef,
+    SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     ListPackagingGroupsResponseTypeDef,
+    CmafEncryptionOutputTypeDef,
+    DashEncryptionOutputTypeDef,
+    HlsEncryptionOutputTypeDef,
+    MssEncryptionOutputTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
     HlsEncryptionTypeDef,
     MssEncryptionTypeDef,
+    CmafPackageOutputTypeDef,
+    DashPackageOutputTypeDef,
+    HlsPackageOutputTypeDef,
+    MssPackageOutputTypeDef,
     CmafPackageTypeDef,
     DashPackageTypeDef,
     HlsPackageTypeDef,
     MssPackageTypeDef,
-    CreatePackagingConfigurationRequestRequestTypeDef,
     CreatePackagingConfigurationResponseTypeDef,
     DescribePackagingConfigurationResponseTypeDef,
     PackagingConfigurationTypeDef,
+    CreatePackagingConfigurationRequestRequestTypeDef,
     ListPackagingConfigurationsResponseTypeDef,
 )
 
 
 def get_structure() -> AssetShallowTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/__init__.py` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/__init__.pyi` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/__main__.py` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaPackageVod 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.MediaPackageVod 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod\nOther"
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

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/client.py` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/client.pyi` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/literals.py` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
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
@@ -271,26 +272,28 @@
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
@@ -437,14 +440,15 @@
 PaginatorName = Literal["list_assets", "list_packaging_configurations", "list_packaging_groups"]
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

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/literals.pyi` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,15 @@
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
@@ -269,26 +270,28 @@
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
@@ -435,14 +438,15 @@
 PaginatorName = Literal["list_assets", "list_packaging_configurations", "list_packaging_groups"]
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

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/paginator.py` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/paginator.pyi` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/type_defs.py` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/type_defs.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,26 +34,30 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssetShallowTypeDef",
+    "AuthorizationOutputTypeDef",
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
+    "EgressAccessLogsOutputTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "EgressEndpointTypeDef",
+    "StreamSelectionOutputTypeDef",
     "StreamSelectionTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeletePackagingConfigurationRequestRequestTypeDef",
     "DeletePackagingGroupRequestRequestTypeDef",
     "DescribeAssetRequestRequestTypeDef",
     "DescribePackagingConfigurationRequestRequestTypeDef",
     "DescribePackagingGroupRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionContractConfigurationOutputTypeDef",
     "EncryptionContractConfigurationTypeDef",
     "ListAssetsRequestListAssetsPaginateTypeDef",
     "ListAssetsRequestRequestTypeDef",
     "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
     "ListPackagingConfigurationsRequestRequestTypeDef",
     "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
     "ListPackagingGroupsRequestRequestTypeDef",
@@ -62,39 +66,51 @@
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ListAssetsResponseTypeDef",
     "UpdatePackagingGroupRequestRequestTypeDef",
     "ConfigureLogsRequestRequestTypeDef",
-    "ConfigureLogsResponseTypeDef",
     "CreatePackagingGroupRequestRequestTypeDef",
+    "ConfigureLogsResponseTypeDef",
     "CreatePackagingGroupResponseTypeDef",
     "DescribePackagingGroupResponseTypeDef",
     "PackagingGroupTypeDef",
     "UpdatePackagingGroupResponseTypeDef",
     "CreateAssetResponseTypeDef",
     "DescribeAssetResponseTypeDef",
+    "DashManifestOutputTypeDef",
+    "HlsManifestOutputTypeDef",
+    "MssManifestOutputTypeDef",
     "DashManifestTypeDef",
     "HlsManifestTypeDef",
     "MssManifestTypeDef",
+    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "ListPackagingGroupsResponseTypeDef",
+    "CmafEncryptionOutputTypeDef",
+    "DashEncryptionOutputTypeDef",
+    "HlsEncryptionOutputTypeDef",
+    "MssEncryptionOutputTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
     "HlsEncryptionTypeDef",
     "MssEncryptionTypeDef",
+    "CmafPackageOutputTypeDef",
+    "DashPackageOutputTypeDef",
+    "HlsPackageOutputTypeDef",
+    "MssPackageOutputTypeDef",
     "CmafPackageTypeDef",
     "DashPackageTypeDef",
     "HlsPackageTypeDef",
     "MssPackageTypeDef",
-    "CreatePackagingConfigurationRequestRequestTypeDef",
     "CreatePackagingConfigurationResponseTypeDef",
     "DescribePackagingConfigurationResponseTypeDef",
     "PackagingConfigurationTypeDef",
+    "CreatePackagingConfigurationRequestRequestTypeDef",
     "ListPackagingConfigurationsResponseTypeDef",
 )
 
 AssetShallowTypeDef = TypedDict(
     "AssetShallowTypeDef",
     {
         "Arn": str,
@@ -105,14 +121,22 @@
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
     },
     total=False,
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
@@ -121,14 +145,22 @@
     "EgressAccessLogsTypeDef",
     {
         "LogGroupName": str,
     },
     total=False,
 )
 
+EgressAccessLogsOutputTypeDef = TypedDict(
+    "EgressAccessLogsOutputTypeDef",
+    {
+        "LogGroupName": str,
+    },
+    total=False,
+)
+
 _RequiredCreateAssetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetRequestRequestTypeDef",
     {
         "Id": str,
         "PackagingGroupId": str,
         "SourceArn": str,
         "SourceRoleArn": str,
@@ -156,14 +188,24 @@
         "PackagingConfigurationId": str,
         "Status": str,
         "Url": str,
     },
     total=False,
 )
 
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
 StreamSelectionTypeDef = TypedDict(
     "StreamSelectionTypeDef",
     {
         "MaxVideoBitsPerSecond": int,
         "MinVideoBitsPerSecond": int,
         "StreamOrder": StreamOrderType,
     },
@@ -215,14 +257,22 @@
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
@@ -382,28 +432,14 @@
 
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
 
-ConfigureLogsResponseTypeDef = TypedDict(
-    "ConfigureLogsResponseTypeDef",
-    {
-        "Arn": str,
-        "Authorization": AuthorizationTypeDef,
-        "CreatedAt": str,
-        "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
-        "Id": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackagingGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalCreatePackagingGroupRequestRequestTypeDef = TypedDict(
@@ -420,67 +456,81 @@
 class CreatePackagingGroupRequestRequestTypeDef(
     _RequiredCreatePackagingGroupRequestRequestTypeDef,
     _OptionalCreatePackagingGroupRequestRequestTypeDef,
 ):
     pass
 
 
+ConfigureLogsResponseTypeDef = TypedDict(
+    "ConfigureLogsResponseTypeDef",
+    {
+        "Arn": str,
+        "Authorization": AuthorizationOutputTypeDef,
+        "CreatedAt": str,
+        "DomainName": str,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "Id": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreatePackagingGroupResponseTypeDef = TypedDict(
     "CreatePackagingGroupResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackagingGroupResponseTypeDef = TypedDict(
     "DescribePackagingGroupResponseTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PackagingGroupTypeDef = TypedDict(
     "PackagingGroupTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
 UpdatePackagingGroupResponseTypeDef = TypedDict(
     "UpdatePackagingGroupResponseTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAssetResponseTypeDef = TypedDict(
@@ -511,14 +561,49 @@
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DashManifestOutputTypeDef = TypedDict(
+    "DashManifestOutputTypeDef",
+    {
+        "ManifestLayout": ManifestLayoutType,
+        "ManifestName": str,
+        "MinBufferTimeSeconds": int,
+        "Profile": ProfileType,
+        "ScteMarkersSource": ScteMarkersSourceType,
+        "StreamSelection": StreamSelectionOutputTypeDef,
+    },
+    total=False,
+)
+
+HlsManifestOutputTypeDef = TypedDict(
+    "HlsManifestOutputTypeDef",
+    {
+        "AdMarkers": AdMarkersType,
+        "IncludeIframeOnlyStream": bool,
+        "ManifestName": str,
+        "ProgramDateTimeIntervalSeconds": int,
+        "RepeatExtXKey": bool,
+        "StreamSelection": StreamSelectionOutputTypeDef,
+    },
+    total=False,
+)
+
+MssManifestOutputTypeDef = TypedDict(
+    "MssManifestOutputTypeDef",
+    {
+        "ManifestName": str,
+        "StreamSelection": StreamSelectionOutputTypeDef,
+    },
+    total=False,
+)
+
 DashManifestTypeDef = TypedDict(
     "DashManifestTypeDef",
     {
         "ManifestLayout": ManifestLayoutType,
         "ManifestName": str,
         "MinBufferTimeSeconds": int,
         "Profile": ProfileType,
@@ -546,14 +631,37 @@
     {
         "ManifestName": str,
         "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
+_RequiredSpekeKeyProviderOutputTypeDef = TypedDict(
+    "_RequiredSpekeKeyProviderOutputTypeDef",
+    {
+        "RoleArn": str,
+        "SystemIds": List[str],
+        "Url": str,
+    },
+)
+_OptionalSpekeKeyProviderOutputTypeDef = TypedDict(
+    "_OptionalSpekeKeyProviderOutputTypeDef",
+    {
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
         "RoleArn": str,
         "SystemIds": Sequence[str],
         "Url": str,
     },
@@ -576,14 +684,71 @@
     {
         "NextToken": str,
         "PackagingGroups": List[PackagingGroupTypeDef],
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
+DashEncryptionOutputTypeDef = TypedDict(
+    "DashEncryptionOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
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
@@ -629,14 +794,105 @@
 MssEncryptionTypeDef = TypedDict(
     "MssEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 
+_RequiredCmafPackageOutputTypeDef = TypedDict(
+    "_RequiredCmafPackageOutputTypeDef",
+    {
+        "HlsManifests": List[HlsManifestOutputTypeDef],
+    },
+)
+_OptionalCmafPackageOutputTypeDef = TypedDict(
+    "_OptionalCmafPackageOutputTypeDef",
+    {
+        "Encryption": CmafEncryptionOutputTypeDef,
+        "IncludeEncoderConfigurationInSegments": bool,
+        "SegmentDurationSeconds": int,
+    },
+    total=False,
+)
+
+
+class CmafPackageOutputTypeDef(
+    _RequiredCmafPackageOutputTypeDef, _OptionalCmafPackageOutputTypeDef
+):
+    pass
+
+
+_RequiredDashPackageOutputTypeDef = TypedDict(
+    "_RequiredDashPackageOutputTypeDef",
+    {
+        "DashManifests": List[DashManifestOutputTypeDef],
+    },
+)
+_OptionalDashPackageOutputTypeDef = TypedDict(
+    "_OptionalDashPackageOutputTypeDef",
+    {
+        "Encryption": DashEncryptionOutputTypeDef,
+        "IncludeEncoderConfigurationInSegments": bool,
+        "IncludeIframeOnlyStream": bool,
+        "PeriodTriggers": List[Literal["ADS"]],
+        "SegmentDurationSeconds": int,
+        "SegmentTemplateFormat": SegmentTemplateFormatType,
+    },
+    total=False,
+)
+
+
+class DashPackageOutputTypeDef(
+    _RequiredDashPackageOutputTypeDef, _OptionalDashPackageOutputTypeDef
+):
+    pass
+
+
+_RequiredHlsPackageOutputTypeDef = TypedDict(
+    "_RequiredHlsPackageOutputTypeDef",
+    {
+        "HlsManifests": List[HlsManifestOutputTypeDef],
+    },
+)
+_OptionalHlsPackageOutputTypeDef = TypedDict(
+    "_OptionalHlsPackageOutputTypeDef",
+    {
+        "Encryption": HlsEncryptionOutputTypeDef,
+        "IncludeDvbSubtitles": bool,
+        "SegmentDurationSeconds": int,
+        "UseAudioRenditionGroup": bool,
+    },
+    total=False,
+)
+
+
+class HlsPackageOutputTypeDef(_RequiredHlsPackageOutputTypeDef, _OptionalHlsPackageOutputTypeDef):
+    pass
+
+
+_RequiredMssPackageOutputTypeDef = TypedDict(
+    "_RequiredMssPackageOutputTypeDef",
+    {
+        "MssManifests": List[MssManifestOutputTypeDef],
+    },
+)
+_OptionalMssPackageOutputTypeDef = TypedDict(
+    "_OptionalMssPackageOutputTypeDef",
+    {
+        "Encryption": MssEncryptionOutputTypeDef,
+        "SegmentDurationSeconds": int,
+    },
+    total=False,
+)
+
+
+class MssPackageOutputTypeDef(_RequiredMssPackageOutputTypeDef, _OptionalMssPackageOutputTypeDef):
+    pass
+
+
 _RequiredCmafPackageTypeDef = TypedDict(
     "_RequiredCmafPackageTypeDef",
     {
         "HlsManifests": Sequence[HlsManifestTypeDef],
     },
 )
 _OptionalCmafPackageTypeDef = TypedDict(
@@ -716,89 +972,89 @@
 )
 
 
 class MssPackageTypeDef(_RequiredMssPackageTypeDef, _OptionalMssPackageTypeDef):
     pass
 
 
-_RequiredCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePackagingConfigurationRequestRequestTypeDef",
-    {
-        "Id": str,
-        "PackagingGroupId": str,
-    },
-)
-_OptionalCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePackagingConfigurationRequestRequestTypeDef",
-    {
-        "CmafPackage": CmafPackageTypeDef,
-        "DashPackage": DashPackageTypeDef,
-        "HlsPackage": HlsPackageTypeDef,
-        "MssPackage": MssPackageTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreatePackagingConfigurationRequestRequestTypeDef(
-    _RequiredCreatePackagingConfigurationRequestRequestTypeDef,
-    _OptionalCreatePackagingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 CreatePackagingConfigurationResponseTypeDef = TypedDict(
     "CreatePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
-        "CmafPackage": CmafPackageTypeDef,
+        "CmafPackage": CmafPackageOutputTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageTypeDef,
-        "HlsPackage": HlsPackageTypeDef,
+        "DashPackage": DashPackageOutputTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackagingConfigurationResponseTypeDef = TypedDict(
     "DescribePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
-        "CmafPackage": CmafPackageTypeDef,
+        "CmafPackage": CmafPackageOutputTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageTypeDef,
-        "HlsPackage": HlsPackageTypeDef,
+        "DashPackage": DashPackageOutputTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PackagingConfigurationTypeDef = TypedDict(
     "PackagingConfigurationTypeDef",
     {
         "Arn": str,
-        "CmafPackage": CmafPackageTypeDef,
+        "CmafPackage": CmafPackageOutputTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageTypeDef,
-        "HlsPackage": HlsPackageTypeDef,
+        "DashPackage": DashPackageOutputTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePackagingConfigurationRequestRequestTypeDef",
+    {
+        "Id": str,
+        "PackagingGroupId": str,
+    },
+)
+_OptionalCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePackagingConfigurationRequestRequestTypeDef",
+    {
+        "CmafPackage": CmafPackageTypeDef,
+        "DashPackage": DashPackageTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
+        "MssPackage": MssPackageTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreatePackagingConfigurationRequestRequestTypeDef(
+    _RequiredCreatePackagingConfigurationRequestRequestTypeDef,
+    _OptionalCreatePackagingConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 ListPackagingConfigurationsResponseTypeDef = TypedDict(
     "ListPackagingConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingConfigurations": List[PackagingConfigurationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod/type_defs.pyi` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -33,26 +33,30 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssetShallowTypeDef",
+    "AuthorizationOutputTypeDef",
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
+    "EgressAccessLogsOutputTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "EgressEndpointTypeDef",
+    "StreamSelectionOutputTypeDef",
     "StreamSelectionTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeletePackagingConfigurationRequestRequestTypeDef",
     "DeletePackagingGroupRequestRequestTypeDef",
     "DescribeAssetRequestRequestTypeDef",
     "DescribePackagingConfigurationRequestRequestTypeDef",
     "DescribePackagingGroupRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionContractConfigurationOutputTypeDef",
     "EncryptionContractConfigurationTypeDef",
     "ListAssetsRequestListAssetsPaginateTypeDef",
     "ListAssetsRequestRequestTypeDef",
     "ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef",
     "ListPackagingConfigurationsRequestRequestTypeDef",
     "ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef",
     "ListPackagingGroupsRequestRequestTypeDef",
@@ -61,39 +65,51 @@
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ListAssetsResponseTypeDef",
     "UpdatePackagingGroupRequestRequestTypeDef",
     "ConfigureLogsRequestRequestTypeDef",
-    "ConfigureLogsResponseTypeDef",
     "CreatePackagingGroupRequestRequestTypeDef",
+    "ConfigureLogsResponseTypeDef",
     "CreatePackagingGroupResponseTypeDef",
     "DescribePackagingGroupResponseTypeDef",
     "PackagingGroupTypeDef",
     "UpdatePackagingGroupResponseTypeDef",
     "CreateAssetResponseTypeDef",
     "DescribeAssetResponseTypeDef",
+    "DashManifestOutputTypeDef",
+    "HlsManifestOutputTypeDef",
+    "MssManifestOutputTypeDef",
     "DashManifestTypeDef",
     "HlsManifestTypeDef",
     "MssManifestTypeDef",
+    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "ListPackagingGroupsResponseTypeDef",
+    "CmafEncryptionOutputTypeDef",
+    "DashEncryptionOutputTypeDef",
+    "HlsEncryptionOutputTypeDef",
+    "MssEncryptionOutputTypeDef",
     "CmafEncryptionTypeDef",
     "DashEncryptionTypeDef",
     "HlsEncryptionTypeDef",
     "MssEncryptionTypeDef",
+    "CmafPackageOutputTypeDef",
+    "DashPackageOutputTypeDef",
+    "HlsPackageOutputTypeDef",
+    "MssPackageOutputTypeDef",
     "CmafPackageTypeDef",
     "DashPackageTypeDef",
     "HlsPackageTypeDef",
     "MssPackageTypeDef",
-    "CreatePackagingConfigurationRequestRequestTypeDef",
     "CreatePackagingConfigurationResponseTypeDef",
     "DescribePackagingConfigurationResponseTypeDef",
     "PackagingConfigurationTypeDef",
+    "CreatePackagingConfigurationRequestRequestTypeDef",
     "ListPackagingConfigurationsResponseTypeDef",
 )
 
 AssetShallowTypeDef = TypedDict(
     "AssetShallowTypeDef",
     {
         "Arn": str,
@@ -104,14 +120,22 @@
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
     },
     total=False,
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
@@ -120,14 +144,22 @@
     "EgressAccessLogsTypeDef",
     {
         "LogGroupName": str,
     },
     total=False,
 )
 
+EgressAccessLogsOutputTypeDef = TypedDict(
+    "EgressAccessLogsOutputTypeDef",
+    {
+        "LogGroupName": str,
+    },
+    total=False,
+)
+
 _RequiredCreateAssetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssetRequestRequestTypeDef",
     {
         "Id": str,
         "PackagingGroupId": str,
         "SourceArn": str,
         "SourceRoleArn": str,
@@ -153,14 +185,24 @@
         "PackagingConfigurationId": str,
         "Status": str,
         "Url": str,
     },
     total=False,
 )
 
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
 StreamSelectionTypeDef = TypedDict(
     "StreamSelectionTypeDef",
     {
         "MaxVideoBitsPerSecond": int,
         "MinVideoBitsPerSecond": int,
         "StreamOrder": StreamOrderType,
     },
@@ -212,14 +254,22 @@
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
@@ -375,28 +425,14 @@
 )
 
 class ConfigureLogsRequestRequestTypeDef(
     _RequiredConfigureLogsRequestRequestTypeDef, _OptionalConfigureLogsRequestRequestTypeDef
 ):
     pass
 
-ConfigureLogsResponseTypeDef = TypedDict(
-    "ConfigureLogsResponseTypeDef",
-    {
-        "Arn": str,
-        "Authorization": AuthorizationTypeDef,
-        "CreatedAt": str,
-        "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
-        "Id": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackagingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackagingGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalCreatePackagingGroupRequestRequestTypeDef = TypedDict(
@@ -411,67 +447,81 @@
 
 class CreatePackagingGroupRequestRequestTypeDef(
     _RequiredCreatePackagingGroupRequestRequestTypeDef,
     _OptionalCreatePackagingGroupRequestRequestTypeDef,
 ):
     pass
 
+ConfigureLogsResponseTypeDef = TypedDict(
+    "ConfigureLogsResponseTypeDef",
+    {
+        "Arn": str,
+        "Authorization": AuthorizationOutputTypeDef,
+        "CreatedAt": str,
+        "DomainName": str,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
+        "Id": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreatePackagingGroupResponseTypeDef = TypedDict(
     "CreatePackagingGroupResponseTypeDef",
     {
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackagingGroupResponseTypeDef = TypedDict(
     "DescribePackagingGroupResponseTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PackagingGroupTypeDef = TypedDict(
     "PackagingGroupTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
 UpdatePackagingGroupResponseTypeDef = TypedDict(
     "UpdatePackagingGroupResponseTypeDef",
     {
         "ApproximateAssetCount": int,
         "Arn": str,
-        "Authorization": AuthorizationTypeDef,
+        "Authorization": AuthorizationOutputTypeDef,
         "CreatedAt": str,
         "DomainName": str,
-        "EgressAccessLogs": EgressAccessLogsTypeDef,
+        "EgressAccessLogs": EgressAccessLogsOutputTypeDef,
         "Id": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateAssetResponseTypeDef = TypedDict(
@@ -502,14 +552,49 @@
         "SourceArn": str,
         "SourceRoleArn": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DashManifestOutputTypeDef = TypedDict(
+    "DashManifestOutputTypeDef",
+    {
+        "ManifestLayout": ManifestLayoutType,
+        "ManifestName": str,
+        "MinBufferTimeSeconds": int,
+        "Profile": ProfileType,
+        "ScteMarkersSource": ScteMarkersSourceType,
+        "StreamSelection": StreamSelectionOutputTypeDef,
+    },
+    total=False,
+)
+
+HlsManifestOutputTypeDef = TypedDict(
+    "HlsManifestOutputTypeDef",
+    {
+        "AdMarkers": AdMarkersType,
+        "IncludeIframeOnlyStream": bool,
+        "ManifestName": str,
+        "ProgramDateTimeIntervalSeconds": int,
+        "RepeatExtXKey": bool,
+        "StreamSelection": StreamSelectionOutputTypeDef,
+    },
+    total=False,
+)
+
+MssManifestOutputTypeDef = TypedDict(
+    "MssManifestOutputTypeDef",
+    {
+        "ManifestName": str,
+        "StreamSelection": StreamSelectionOutputTypeDef,
+    },
+    total=False,
+)
+
 DashManifestTypeDef = TypedDict(
     "DashManifestTypeDef",
     {
         "ManifestLayout": ManifestLayoutType,
         "ManifestName": str,
         "MinBufferTimeSeconds": int,
         "Profile": ProfileType,
@@ -537,14 +622,35 @@
     {
         "ManifestName": str,
         "StreamSelection": StreamSelectionTypeDef,
     },
     total=False,
 )
 
+_RequiredSpekeKeyProviderOutputTypeDef = TypedDict(
+    "_RequiredSpekeKeyProviderOutputTypeDef",
+    {
+        "RoleArn": str,
+        "SystemIds": List[str],
+        "Url": str,
+    },
+)
+_OptionalSpekeKeyProviderOutputTypeDef = TypedDict(
+    "_OptionalSpekeKeyProviderOutputTypeDef",
+    {
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
         "RoleArn": str,
         "SystemIds": Sequence[str],
         "Url": str,
     },
@@ -565,14 +671,67 @@
     {
         "NextToken": str,
         "PackagingGroups": List[PackagingGroupTypeDef],
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
+    },
+    total=False,
+)
+
+class CmafEncryptionOutputTypeDef(
+    _RequiredCmafEncryptionOutputTypeDef, _OptionalCmafEncryptionOutputTypeDef
+):
+    pass
+
+DashEncryptionOutputTypeDef = TypedDict(
+    "DashEncryptionOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
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
@@ -614,14 +773,97 @@
 MssEncryptionTypeDef = TypedDict(
     "MssEncryptionTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
 
+_RequiredCmafPackageOutputTypeDef = TypedDict(
+    "_RequiredCmafPackageOutputTypeDef",
+    {
+        "HlsManifests": List[HlsManifestOutputTypeDef],
+    },
+)
+_OptionalCmafPackageOutputTypeDef = TypedDict(
+    "_OptionalCmafPackageOutputTypeDef",
+    {
+        "Encryption": CmafEncryptionOutputTypeDef,
+        "IncludeEncoderConfigurationInSegments": bool,
+        "SegmentDurationSeconds": int,
+    },
+    total=False,
+)
+
+class CmafPackageOutputTypeDef(
+    _RequiredCmafPackageOutputTypeDef, _OptionalCmafPackageOutputTypeDef
+):
+    pass
+
+_RequiredDashPackageOutputTypeDef = TypedDict(
+    "_RequiredDashPackageOutputTypeDef",
+    {
+        "DashManifests": List[DashManifestOutputTypeDef],
+    },
+)
+_OptionalDashPackageOutputTypeDef = TypedDict(
+    "_OptionalDashPackageOutputTypeDef",
+    {
+        "Encryption": DashEncryptionOutputTypeDef,
+        "IncludeEncoderConfigurationInSegments": bool,
+        "IncludeIframeOnlyStream": bool,
+        "PeriodTriggers": List[Literal["ADS"]],
+        "SegmentDurationSeconds": int,
+        "SegmentTemplateFormat": SegmentTemplateFormatType,
+    },
+    total=False,
+)
+
+class DashPackageOutputTypeDef(
+    _RequiredDashPackageOutputTypeDef, _OptionalDashPackageOutputTypeDef
+):
+    pass
+
+_RequiredHlsPackageOutputTypeDef = TypedDict(
+    "_RequiredHlsPackageOutputTypeDef",
+    {
+        "HlsManifests": List[HlsManifestOutputTypeDef],
+    },
+)
+_OptionalHlsPackageOutputTypeDef = TypedDict(
+    "_OptionalHlsPackageOutputTypeDef",
+    {
+        "Encryption": HlsEncryptionOutputTypeDef,
+        "IncludeDvbSubtitles": bool,
+        "SegmentDurationSeconds": int,
+        "UseAudioRenditionGroup": bool,
+    },
+    total=False,
+)
+
+class HlsPackageOutputTypeDef(_RequiredHlsPackageOutputTypeDef, _OptionalHlsPackageOutputTypeDef):
+    pass
+
+_RequiredMssPackageOutputTypeDef = TypedDict(
+    "_RequiredMssPackageOutputTypeDef",
+    {
+        "MssManifests": List[MssManifestOutputTypeDef],
+    },
+)
+_OptionalMssPackageOutputTypeDef = TypedDict(
+    "_OptionalMssPackageOutputTypeDef",
+    {
+        "Encryption": MssEncryptionOutputTypeDef,
+        "SegmentDurationSeconds": int,
+    },
+    total=False,
+)
+
+class MssPackageOutputTypeDef(_RequiredMssPackageOutputTypeDef, _OptionalMssPackageOutputTypeDef):
+    pass
+
 _RequiredCmafPackageTypeDef = TypedDict(
     "_RequiredCmafPackageTypeDef",
     {
         "HlsManifests": Sequence[HlsManifestTypeDef],
     },
 )
 _OptionalCmafPackageTypeDef = TypedDict(
@@ -693,87 +935,87 @@
     },
     total=False,
 )
 
 class MssPackageTypeDef(_RequiredMssPackageTypeDef, _OptionalMssPackageTypeDef):
     pass
 
-_RequiredCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePackagingConfigurationRequestRequestTypeDef",
-    {
-        "Id": str,
-        "PackagingGroupId": str,
-    },
-)
-_OptionalCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePackagingConfigurationRequestRequestTypeDef",
-    {
-        "CmafPackage": CmafPackageTypeDef,
-        "DashPackage": DashPackageTypeDef,
-        "HlsPackage": HlsPackageTypeDef,
-        "MssPackage": MssPackageTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreatePackagingConfigurationRequestRequestTypeDef(
-    _RequiredCreatePackagingConfigurationRequestRequestTypeDef,
-    _OptionalCreatePackagingConfigurationRequestRequestTypeDef,
-):
-    pass
-
 CreatePackagingConfigurationResponseTypeDef = TypedDict(
     "CreatePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
-        "CmafPackage": CmafPackageTypeDef,
+        "CmafPackage": CmafPackageOutputTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageTypeDef,
-        "HlsPackage": HlsPackageTypeDef,
+        "DashPackage": DashPackageOutputTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePackagingConfigurationResponseTypeDef = TypedDict(
     "DescribePackagingConfigurationResponseTypeDef",
     {
         "Arn": str,
-        "CmafPackage": CmafPackageTypeDef,
+        "CmafPackage": CmafPackageOutputTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageTypeDef,
-        "HlsPackage": HlsPackageTypeDef,
+        "DashPackage": DashPackageOutputTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PackagingConfigurationTypeDef = TypedDict(
     "PackagingConfigurationTypeDef",
     {
         "Arn": str,
-        "CmafPackage": CmafPackageTypeDef,
+        "CmafPackage": CmafPackageOutputTypeDef,
         "CreatedAt": str,
-        "DashPackage": DashPackageTypeDef,
-        "HlsPackage": HlsPackageTypeDef,
+        "DashPackage": DashPackageOutputTypeDef,
+        "HlsPackage": HlsPackageOutputTypeDef,
         "Id": str,
-        "MssPackage": MssPackageTypeDef,
+        "MssPackage": MssPackageOutputTypeDef,
         "PackagingGroupId": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+_RequiredCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePackagingConfigurationRequestRequestTypeDef",
+    {
+        "Id": str,
+        "PackagingGroupId": str,
+    },
+)
+_OptionalCreatePackagingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePackagingConfigurationRequestRequestTypeDef",
+    {
+        "CmafPackage": CmafPackageTypeDef,
+        "DashPackage": DashPackageTypeDef,
+        "HlsPackage": HlsPackageTypeDef,
+        "MssPackage": MssPackageTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreatePackagingConfigurationRequestRequestTypeDef(
+    _RequiredCreatePackagingConfigurationRequestRequestTypeDef,
+    _OptionalCreatePackagingConfigurationRequestRequestTypeDef,
+):
+    pass
+
 ListPackagingConfigurationsResponseTypeDef = TypedDict(
     "ListPackagingConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "PackagingConfigurations": List[PackagingConfigurationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage-vod
-Version: 1.28.0
-Summary: Type annotations for boto3.MediaPackageVod 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MediaPackageVod 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediapackage-vod"></a>
 
 # mypy-boto3-mediapackage-vod
 
 [![PyPI - mypy-boto3-mediapackage-vod](https://img.shields.io/pypi/v/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage-vod.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage-vod?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage-vod)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackage-vod)](https://pepy.tech/project/mypy-boto3-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackageVod 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[boto3.MediaPackageVod 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [mypy-boto3-mediapackage-vod docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,26 +343,30 @@
 
 `mypy_boto3_mediapackage_vod.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediapackage_vod.type_defs import (
     AssetShallowTypeDef,
+    AuthorizationOutputTypeDef,
     AuthorizationTypeDef,
     EgressAccessLogsTypeDef,
+    EgressAccessLogsOutputTypeDef,
     CreateAssetRequestRequestTypeDef,
     EgressEndpointTypeDef,
+    StreamSelectionOutputTypeDef,
     StreamSelectionTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeletePackagingConfigurationRequestRequestTypeDef,
     DeletePackagingGroupRequestRequestTypeDef,
     DescribeAssetRequestRequestTypeDef,
     DescribePackagingConfigurationRequestRequestTypeDef,
     DescribePackagingGroupRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
     ListAssetsRequestListAssetsPaginateTypeDef,
     ListAssetsRequestRequestTypeDef,
     ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef,
     ListPackagingConfigurationsRequestRequestTypeDef,
     ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef,
     ListPackagingGroupsRequestRequestTypeDef,
@@ -371,39 +375,51 @@
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ListAssetsResponseTypeDef,
     UpdatePackagingGroupRequestRequestTypeDef,
     ConfigureLogsRequestRequestTypeDef,
-    ConfigureLogsResponseTypeDef,
     CreatePackagingGroupRequestRequestTypeDef,
+    ConfigureLogsResponseTypeDef,
     CreatePackagingGroupResponseTypeDef,
     DescribePackagingGroupResponseTypeDef,
     PackagingGroupTypeDef,
     UpdatePackagingGroupResponseTypeDef,
     CreateAssetResponseTypeDef,
     DescribeAssetResponseTypeDef,
+    DashManifestOutputTypeDef,
+    HlsManifestOutputTypeDef,
+    MssManifestOutputTypeDef,
     DashManifestTypeDef,
     HlsManifestTypeDef,
     MssManifestTypeDef,
+    SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
     ListPackagingGroupsResponseTypeDef,
+    CmafEncryptionOutputTypeDef,
+    DashEncryptionOutputTypeDef,
+    HlsEncryptionOutputTypeDef,
+    MssEncryptionOutputTypeDef,
     CmafEncryptionTypeDef,
     DashEncryptionTypeDef,
     HlsEncryptionTypeDef,
     MssEncryptionTypeDef,
+    CmafPackageOutputTypeDef,
+    DashPackageOutputTypeDef,
+    HlsPackageOutputTypeDef,
+    MssPackageOutputTypeDef,
     CmafPackageTypeDef,
     DashPackageTypeDef,
     HlsPackageTypeDef,
     MssPackageTypeDef,
-    CreatePackagingConfigurationRequestRequestTypeDef,
     CreatePackagingConfigurationResponseTypeDef,
     DescribePackagingConfigurationResponseTypeDef,
     PackagingConfigurationTypeDef,
+    CreatePackagingConfigurationRequestRequestTypeDef,
     ListPackagingConfigurationsResponseTypeDef,
 )
 
 
 def get_structure() -> AssetShallowTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt` & `mypy-boto3-mediapackage-vod-1.28.12/mypy_boto3_mediapackage_vod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-vod-1.28.0/setup.py` & `mypy-boto3-mediapackage-vod-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackage-vod",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_mediapackage_vod"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaPackageVod 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MediaPackageVod 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

