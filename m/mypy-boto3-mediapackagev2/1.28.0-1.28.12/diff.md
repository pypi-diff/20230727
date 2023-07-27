# Comparing `tmp/mypy-boto3-mediapackagev2-1.28.0.tar.gz` & `tmp/mypy-boto3-mediapackagev2-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackagev2-1.28.0.tar", last modified: Thu Jul  6 21:00:06 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackagev2-1.28.12.tar", last modified: Thu Jul 27 05:35:01 2023, max compression
```

## Comparing `mypy-boto3-mediapackagev2-1.28.0.tar` & `mypy-boto3-mediapackagev2-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:06.134367 mypy-boto3-mediapackagev2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:20.000000 mypy-boto3-mediapackagev2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-06 21:00:06.126367 mypy-boto3-mediapackagev2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-07-06 20:47:20.000000 mypy-boto3-mediapackagev2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:06.122367 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-06 20:47:20.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-06 20:47:20.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:47:20.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-07-06 20:47:20.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20244 2023-07-06 20:47:20.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-06 20:47:21.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-06 20:47:21.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-06 20:47:20.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-06 20:47:20.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:20.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26978 2023-07-06 20:47:21.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26937 2023-07-06 20:47:21.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:20.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:06.126367 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-06 21:00:05.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 21:00:05.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:05.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:05.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:05.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 21:00:05.000000 mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:06.134367 mypy-boto3-mediapackagev2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-06 20:47:20.000000 mypy-boto3-mediapackagev2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.756438 mypy-boto3-mediapackagev2-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-07-27 05:35:01.756438 mypy-boto3-mediapackagev2-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.748438 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20278 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20244 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29180 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29138 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:24.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.756438 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-07-27 05:35:01.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:35:01.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:01.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:35:01.000000 mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:01.756438 mypy-boto3-mediapackagev2-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:26:23.000000 mypy-boto3-mediapackagev2-1.28.12/setup.py
```

### Comparing `mypy-boto3-mediapackagev2-1.28.0/LICENSE` & `mypy-boto3-mediapackagev2-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.0/PKG-INFO` & `mypy-boto3-mediapackagev2-1.28.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackagev2
-Version: 1.28.0
-Summary: Type annotations for boto3.mediapackagev2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.mediapackagev2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediapackagev2"></a>
 
 # mypy-boto3-mediapackagev2
 
 [![PyPI - mypy-boto3-mediapackagev2](https://img.shields.io/pypi/v/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackagev2?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackagev2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackagev2)](https://pepy.tech/project/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
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
 [mypy-boto3-mediapackagev2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,21 +353,24 @@
     ScteHlsTypeDef,
     DeleteChannelGroupRequestRequestTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointPolicyRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
+    EncryptionMethodOutputTypeDef,
     EncryptionMethodTypeDef,
     GetChannelGroupRequestRequestTypeDef,
     GetChannelGroupResponseTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
     GetChannelPolicyResponseTypeDef,
     GetChannelRequestRequestTypeDef,
+    ScteHlsOutputTypeDef,
     GetOriginEndpointPolicyRequestRequestTypeDef,
     GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointRequestRequestTypeDef,
     ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
     ListChannelGroupsRequestRequestTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
@@ -377,39 +380,43 @@
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     PutOriginEndpointPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    ScteOutputTypeDef,
     ScteTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelGroupRequestRequestTypeDef,
     UpdateChannelGroupResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelResponseTypeDef,
     GetChannelResponseTypeDef,
     UpdateChannelResponseTypeDef,
     CreateHlsManifestConfigurationTypeDef,
     CreateLowLatencyHlsManifestConfigurationTypeDef,
+    SpekeKeyProviderOutputTypeDef,
+    SpekeKeyProviderTypeDef,
     GetHlsManifestConfigurationTypeDef,
     GetLowLatencyHlsManifestConfigurationTypeDef,
-    SpekeKeyProviderTypeDef,
     OriginEndpointListConfigurationTypeDef,
+    EncryptionOutputTypeDef,
     EncryptionTypeDef,
     ListOriginEndpointsResponseTypeDef,
+    SegmentOutputTypeDef,
     SegmentTypeDef,
-    CreateOriginEndpointRequestRequestTypeDef,
     CreateOriginEndpointResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
-    UpdateOriginEndpointRequestRequestTypeDef,
     UpdateOriginEndpointResponseTypeDef,
+    CreateOriginEndpointRequestRequestTypeDef,
+    UpdateOriginEndpointRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ChannelGroupListConfigurationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mediapackagev2-1.28.0/README.md` & `mypy-boto3-mediapackagev2-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mediapackagev2"></a>
 
 # mypy-boto3-mediapackagev2
 
 [![PyPI - mypy-boto3-mediapackagev2](https://img.shields.io/pypi/v/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackagev2?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackagev2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackagev2)](https://pepy.tech/project/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
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
 [mypy-boto3-mediapackagev2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,21 +321,24 @@
     ScteHlsTypeDef,
     DeleteChannelGroupRequestRequestTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointPolicyRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
+    EncryptionMethodOutputTypeDef,
     EncryptionMethodTypeDef,
     GetChannelGroupRequestRequestTypeDef,
     GetChannelGroupResponseTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
     GetChannelPolicyResponseTypeDef,
     GetChannelRequestRequestTypeDef,
+    ScteHlsOutputTypeDef,
     GetOriginEndpointPolicyRequestRequestTypeDef,
     GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointRequestRequestTypeDef,
     ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
     ListChannelGroupsRequestRequestTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
@@ -345,39 +348,43 @@
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     PutOriginEndpointPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    ScteOutputTypeDef,
     ScteTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelGroupRequestRequestTypeDef,
     UpdateChannelGroupResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelResponseTypeDef,
     GetChannelResponseTypeDef,
     UpdateChannelResponseTypeDef,
     CreateHlsManifestConfigurationTypeDef,
     CreateLowLatencyHlsManifestConfigurationTypeDef,
+    SpekeKeyProviderOutputTypeDef,
+    SpekeKeyProviderTypeDef,
     GetHlsManifestConfigurationTypeDef,
     GetLowLatencyHlsManifestConfigurationTypeDef,
-    SpekeKeyProviderTypeDef,
     OriginEndpointListConfigurationTypeDef,
+    EncryptionOutputTypeDef,
     EncryptionTypeDef,
     ListOriginEndpointsResponseTypeDef,
+    SegmentOutputTypeDef,
     SegmentTypeDef,
-    CreateOriginEndpointRequestRequestTypeDef,
     CreateOriginEndpointResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
-    UpdateOriginEndpointRequestRequestTypeDef,
     UpdateOriginEndpointResponseTypeDef,
+    CreateOriginEndpointRequestRequestTypeDef,
+    UpdateOriginEndpointRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ChannelGroupListConfigurationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/__init__.py` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/__init__.pyi` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/__main__.py` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.mediapackagev2 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.mediapackagev2 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2\nOther"
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

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/client.py` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/client.pyi` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/literals.py` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
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
@@ -275,26 +276,28 @@
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
@@ -441,14 +444,15 @@
 PaginatorName = Literal["list_channel_groups", "list_channels", "list_origin_endpoints"]
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

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/literals.pyi` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
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
@@ -273,26 +274,28 @@
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
@@ -439,14 +442,15 @@
 PaginatorName = Literal["list_channel_groups", "list_channels", "list_origin_endpoints"]
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

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/paginator.py` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/paginator.pyi` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/type_defs.py` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,21 +45,24 @@
     "ScteHlsTypeDef",
     "DeleteChannelGroupRequestRequestTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointPolicyRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionContractConfigurationOutputTypeDef",
     "EncryptionContractConfigurationTypeDef",
+    "EncryptionMethodOutputTypeDef",
     "EncryptionMethodTypeDef",
     "GetChannelGroupRequestRequestTypeDef",
     "GetChannelGroupResponseTypeDef",
     "GetChannelPolicyRequestRequestTypeDef",
     "GetChannelPolicyResponseTypeDef",
     "GetChannelRequestRequestTypeDef",
+    "ScteHlsOutputTypeDef",
     "GetOriginEndpointPolicyRequestRequestTypeDef",
     "GetOriginEndpointPolicyResponseTypeDef",
     "GetOriginEndpointRequestRequestTypeDef",
     "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
     "ListChannelGroupsRequestRequestTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
@@ -69,39 +72,43 @@
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "PutOriginEndpointPolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "ScteOutputTypeDef",
     "ScteTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelGroupRequestRequestTypeDef",
     "UpdateChannelGroupResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "ListChannelGroupsResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "GetChannelResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "CreateHlsManifestConfigurationTypeDef",
     "CreateLowLatencyHlsManifestConfigurationTypeDef",
+    "SpekeKeyProviderOutputTypeDef",
+    "SpekeKeyProviderTypeDef",
     "GetHlsManifestConfigurationTypeDef",
     "GetLowLatencyHlsManifestConfigurationTypeDef",
-    "SpekeKeyProviderTypeDef",
     "OriginEndpointListConfigurationTypeDef",
+    "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
     "ListOriginEndpointsResponseTypeDef",
+    "SegmentOutputTypeDef",
     "SegmentTypeDef",
-    "CreateOriginEndpointRequestRequestTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "GetOriginEndpointResponseTypeDef",
-    "UpdateOriginEndpointRequestRequestTypeDef",
     "UpdateOriginEndpointResponseTypeDef",
+    "CreateOriginEndpointRequestRequestTypeDef",
+    "UpdateOriginEndpointRequestRequestTypeDef",
 )
 
 _RequiredChannelGroupListConfigurationTypeDef = TypedDict(
     "_RequiredChannelGroupListConfigurationTypeDef",
     {
         "ChannelGroupName": str,
         "Arn": str,
@@ -272,22 +279,39 @@
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
 
+EncryptionMethodOutputTypeDef = TypedDict(
+    "EncryptionMethodOutputTypeDef",
+    {
+        "TsEncryptionMethod": TsEncryptionMethodType,
+        "CmafEncryptionMethod": CmafEncryptionMethodType,
+    },
+    total=False,
+)
+
 EncryptionMethodTypeDef = TypedDict(
     "EncryptionMethodTypeDef",
     {
         "TsEncryptionMethod": TsEncryptionMethodType,
         "CmafEncryptionMethod": CmafEncryptionMethodType,
     },
     total=False,
@@ -336,14 +360,22 @@
     "GetChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
 
+ScteHlsOutputTypeDef = TypedDict(
+    "ScteHlsOutputTypeDef",
+    {
+        "AdMarkerHls": Literal["DATERANGE"],
+    },
+    total=False,
+)
+
 GetOriginEndpointPolicyRequestRequestTypeDef = TypedDict(
     "GetOriginEndpointPolicyRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
@@ -573,14 +605,22 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+ScteOutputTypeDef = TypedDict(
+    "ScteOutputTypeDef",
+    {
+        "ScteFilter": List[ScteFilterType],
+    },
+    total=False,
+)
+
 ScteTypeDef = TypedDict(
     "ScteTypeDef",
     {
         "ScteFilter": Sequence[ScteFilterType],
     },
     total=False,
 )
@@ -767,28 +807,50 @@
 class CreateLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredCreateLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalCreateLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
 
+SpekeKeyProviderOutputTypeDef = TypedDict(
+    "SpekeKeyProviderOutputTypeDef",
+    {
+        "EncryptionContractConfiguration": EncryptionContractConfigurationOutputTypeDef,
+        "ResourceId": str,
+        "DrmSystems": List[DrmSystemType],
+        "RoleArn": str,
+        "Url": str,
+    },
+)
+
+SpekeKeyProviderTypeDef = TypedDict(
+    "SpekeKeyProviderTypeDef",
+    {
+        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
+        "ResourceId": str,
+        "DrmSystems": Sequence[DrmSystemType],
+        "RoleArn": str,
+        "Url": str,
+    },
+)
+
 _RequiredGetHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredGetHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "Url": str,
     },
 )
 _OptionalGetHlsManifestConfigurationTypeDef = TypedDict(
     "_OptionalGetHlsManifestConfigurationTypeDef",
     {
         "ChildManifestName": str,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
-        "ScteHls": ScteHlsTypeDef,
+        "ScteHls": ScteHlsOutputTypeDef,
     },
     total=False,
 )
 
 
 class GetHlsManifestConfigurationTypeDef(
     _RequiredGetHlsManifestConfigurationTypeDef, _OptionalGetHlsManifestConfigurationTypeDef
@@ -805,38 +867,27 @@
 )
 _OptionalGetLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_OptionalGetLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ChildManifestName": str,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
-        "ScteHls": ScteHlsTypeDef,
+        "ScteHls": ScteHlsOutputTypeDef,
     },
     total=False,
 )
 
 
 class GetLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredGetLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalGetLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
 
-SpekeKeyProviderTypeDef = TypedDict(
-    "SpekeKeyProviderTypeDef",
-    {
-        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
-        "ResourceId": str,
-        "DrmSystems": Sequence[DrmSystemType],
-        "RoleArn": str,
-        "Url": str,
-    },
-)
-
 _RequiredOriginEndpointListConfigurationTypeDef = TypedDict(
     "_RequiredOriginEndpointListConfigurationTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
@@ -858,14 +909,35 @@
 
 class OriginEndpointListConfigurationTypeDef(
     _RequiredOriginEndpointListConfigurationTypeDef, _OptionalOriginEndpointListConfigurationTypeDef
 ):
     pass
 
 
+_RequiredEncryptionOutputTypeDef = TypedDict(
+    "_RequiredEncryptionOutputTypeDef",
+    {
+        "EncryptionMethod": EncryptionMethodOutputTypeDef,
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+_OptionalEncryptionOutputTypeDef = TypedDict(
+    "_OptionalEncryptionOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "KeyRotationIntervalSeconds": int,
+    },
+    total=False,
+)
+
+
+class EncryptionOutputTypeDef(_RequiredEncryptionOutputTypeDef, _OptionalEncryptionOutputTypeDef):
+    pass
+
+
 _RequiredEncryptionTypeDef = TypedDict(
     "_RequiredEncryptionTypeDef",
     {
         "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
@@ -888,140 +960,153 @@
     {
         "Items": List[OriginEndpointListConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SegmentOutputTypeDef = TypedDict(
+    "SegmentOutputTypeDef",
+    {
+        "SegmentDurationSeconds": int,
+        "SegmentName": str,
+        "TsUseAudioRenditionGroup": bool,
+        "IncludeIframeOnlyStreams": bool,
+        "TsIncludeDvbSubtitles": bool,
+        "Scte": ScteOutputTypeDef,
+        "Encryption": EncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
 SegmentTypeDef = TypedDict(
     "SegmentTypeDef",
     {
         "SegmentDurationSeconds": int,
         "SegmentName": str,
         "TsUseAudioRenditionGroup": bool,
         "IncludeIframeOnlyStreams": bool,
         "TsIncludeDvbSubtitles": bool,
         "Scte": ScteTypeDef,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
+CreateOriginEndpointResponseTypeDef = TypedDict(
+    "CreateOriginEndpointResponseTypeDef",
     {
+        "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-    },
-)
-_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
-    {
-        "Segment": SegmentTypeDef,
-        "ClientToken": str,
+        "Segment": SegmentOutputTypeDef,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
-        "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
-        "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
-        "Tags": Mapping[str, str],
+        "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
+        "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
+        "Tags": Dict[str, str],
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
+GetOriginEndpointResponseTypeDef = TypedDict(
+    "GetOriginEndpointResponseTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-        "Segment": SegmentTypeDef,
+        "Segment": SegmentOutputTypeDef,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetOriginEndpointResponseTypeDef = TypedDict(
-    "GetOriginEndpointResponseTypeDef",
+UpdateOriginEndpointResponseTypeDef = TypedDict(
+    "UpdateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-        "Segment": SegmentTypeDef,
+        "Segment": SegmentOutputTypeDef,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
+_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
     },
 )
-_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
+_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
     {
         "Segment": SegmentTypeDef,
+        "ClientToken": str,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class UpdateOriginEndpointRequestRequestTypeDef(
-    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
-    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
+class CreateOriginEndpointRequestRequestTypeDef(
+    _RequiredCreateOriginEndpointRequestRequestTypeDef,
+    _OptionalCreateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateOriginEndpointResponseTypeDef = TypedDict(
-    "UpdateOriginEndpointResponseTypeDef",
+_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
-        "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
+    },
+)
+_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
+    {
         "Segment": SegmentTypeDef,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
-        "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
-        "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
+        "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
     },
+    total=False,
 )
+
+
+class UpdateOriginEndpointRequestRequestTypeDef(
+    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
+    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2/type_defs.pyi` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,21 +44,24 @@
     "ScteHlsTypeDef",
     "DeleteChannelGroupRequestRequestTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteOriginEndpointPolicyRequestRequestTypeDef",
     "DeleteOriginEndpointRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionContractConfigurationOutputTypeDef",
     "EncryptionContractConfigurationTypeDef",
+    "EncryptionMethodOutputTypeDef",
     "EncryptionMethodTypeDef",
     "GetChannelGroupRequestRequestTypeDef",
     "GetChannelGroupResponseTypeDef",
     "GetChannelPolicyRequestRequestTypeDef",
     "GetChannelPolicyResponseTypeDef",
     "GetChannelRequestRequestTypeDef",
+    "ScteHlsOutputTypeDef",
     "GetOriginEndpointPolicyRequestRequestTypeDef",
     "GetOriginEndpointPolicyResponseTypeDef",
     "GetOriginEndpointRequestRequestTypeDef",
     "ListChannelGroupsRequestListChannelGroupsPaginateTypeDef",
     "ListChannelGroupsRequestRequestTypeDef",
     "ListChannelsRequestListChannelsPaginateTypeDef",
     "ListChannelsRequestRequestTypeDef",
@@ -68,39 +71,43 @@
     "ListOriginEndpointsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "PutChannelPolicyRequestRequestTypeDef",
     "PutOriginEndpointPolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "ScteOutputTypeDef",
     "ScteTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelGroupRequestRequestTypeDef",
     "UpdateChannelGroupResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "ListChannelGroupsResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateChannelResponseTypeDef",
     "GetChannelResponseTypeDef",
     "UpdateChannelResponseTypeDef",
     "CreateHlsManifestConfigurationTypeDef",
     "CreateLowLatencyHlsManifestConfigurationTypeDef",
+    "SpekeKeyProviderOutputTypeDef",
+    "SpekeKeyProviderTypeDef",
     "GetHlsManifestConfigurationTypeDef",
     "GetLowLatencyHlsManifestConfigurationTypeDef",
-    "SpekeKeyProviderTypeDef",
     "OriginEndpointListConfigurationTypeDef",
+    "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
     "ListOriginEndpointsResponseTypeDef",
+    "SegmentOutputTypeDef",
     "SegmentTypeDef",
-    "CreateOriginEndpointRequestRequestTypeDef",
     "CreateOriginEndpointResponseTypeDef",
     "GetOriginEndpointResponseTypeDef",
-    "UpdateOriginEndpointRequestRequestTypeDef",
     "UpdateOriginEndpointResponseTypeDef",
+    "CreateOriginEndpointRequestRequestTypeDef",
+    "UpdateOriginEndpointRequestRequestTypeDef",
 )
 
 _RequiredChannelGroupListConfigurationTypeDef = TypedDict(
     "_RequiredChannelGroupListConfigurationTypeDef",
     {
         "ChannelGroupName": str,
         "Arn": str,
@@ -263,22 +270,39 @@
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
 
+EncryptionMethodOutputTypeDef = TypedDict(
+    "EncryptionMethodOutputTypeDef",
+    {
+        "TsEncryptionMethod": TsEncryptionMethodType,
+        "CmafEncryptionMethod": CmafEncryptionMethodType,
+    },
+    total=False,
+)
+
 EncryptionMethodTypeDef = TypedDict(
     "EncryptionMethodTypeDef",
     {
         "TsEncryptionMethod": TsEncryptionMethodType,
         "CmafEncryptionMethod": CmafEncryptionMethodType,
     },
     total=False,
@@ -327,14 +351,22 @@
     "GetChannelRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
     },
 )
 
+ScteHlsOutputTypeDef = TypedDict(
+    "ScteHlsOutputTypeDef",
+    {
+        "AdMarkerHls": Literal["DATERANGE"],
+    },
+    total=False,
+)
+
 GetOriginEndpointPolicyRequestRequestTypeDef = TypedDict(
     "GetOriginEndpointPolicyRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
     },
@@ -552,14 +584,22 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+ScteOutputTypeDef = TypedDict(
+    "ScteOutputTypeDef",
+    {
+        "ScteFilter": List[ScteFilterType],
+    },
+    total=False,
+)
+
 ScteTypeDef = TypedDict(
     "ScteTypeDef",
     {
         "ScteFilter": Sequence[ScteFilterType],
     },
     total=False,
 )
@@ -738,28 +778,50 @@
 
 class CreateLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredCreateLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalCreateLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
+SpekeKeyProviderOutputTypeDef = TypedDict(
+    "SpekeKeyProviderOutputTypeDef",
+    {
+        "EncryptionContractConfiguration": EncryptionContractConfigurationOutputTypeDef,
+        "ResourceId": str,
+        "DrmSystems": List[DrmSystemType],
+        "RoleArn": str,
+        "Url": str,
+    },
+)
+
+SpekeKeyProviderTypeDef = TypedDict(
+    "SpekeKeyProviderTypeDef",
+    {
+        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
+        "ResourceId": str,
+        "DrmSystems": Sequence[DrmSystemType],
+        "RoleArn": str,
+        "Url": str,
+    },
+)
+
 _RequiredGetHlsManifestConfigurationTypeDef = TypedDict(
     "_RequiredGetHlsManifestConfigurationTypeDef",
     {
         "ManifestName": str,
         "Url": str,
     },
 )
 _OptionalGetHlsManifestConfigurationTypeDef = TypedDict(
     "_OptionalGetHlsManifestConfigurationTypeDef",
     {
         "ChildManifestName": str,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
-        "ScteHls": ScteHlsTypeDef,
+        "ScteHls": ScteHlsOutputTypeDef,
     },
     total=False,
 )
 
 class GetHlsManifestConfigurationTypeDef(
     _RequiredGetHlsManifestConfigurationTypeDef, _OptionalGetHlsManifestConfigurationTypeDef
 ):
@@ -774,36 +836,25 @@
 )
 _OptionalGetLowLatencyHlsManifestConfigurationTypeDef = TypedDict(
     "_OptionalGetLowLatencyHlsManifestConfigurationTypeDef",
     {
         "ChildManifestName": str,
         "ManifestWindowSeconds": int,
         "ProgramDateTimeIntervalSeconds": int,
-        "ScteHls": ScteHlsTypeDef,
+        "ScteHls": ScteHlsOutputTypeDef,
     },
     total=False,
 )
 
 class GetLowLatencyHlsManifestConfigurationTypeDef(
     _RequiredGetLowLatencyHlsManifestConfigurationTypeDef,
     _OptionalGetLowLatencyHlsManifestConfigurationTypeDef,
 ):
     pass
 
-SpekeKeyProviderTypeDef = TypedDict(
-    "SpekeKeyProviderTypeDef",
-    {
-        "EncryptionContractConfiguration": EncryptionContractConfigurationTypeDef,
-        "ResourceId": str,
-        "DrmSystems": Sequence[DrmSystemType],
-        "RoleArn": str,
-        "Url": str,
-    },
-)
-
 _RequiredOriginEndpointListConfigurationTypeDef = TypedDict(
     "_RequiredOriginEndpointListConfigurationTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
@@ -823,14 +874,33 @@
 )
 
 class OriginEndpointListConfigurationTypeDef(
     _RequiredOriginEndpointListConfigurationTypeDef, _OptionalOriginEndpointListConfigurationTypeDef
 ):
     pass
 
+_RequiredEncryptionOutputTypeDef = TypedDict(
+    "_RequiredEncryptionOutputTypeDef",
+    {
+        "EncryptionMethod": EncryptionMethodOutputTypeDef,
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+_OptionalEncryptionOutputTypeDef = TypedDict(
+    "_OptionalEncryptionOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "KeyRotationIntervalSeconds": int,
+    },
+    total=False,
+)
+
+class EncryptionOutputTypeDef(_RequiredEncryptionOutputTypeDef, _OptionalEncryptionOutputTypeDef):
+    pass
+
 _RequiredEncryptionTypeDef = TypedDict(
     "_RequiredEncryptionTypeDef",
     {
         "EncryptionMethod": EncryptionMethodTypeDef,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
 )
@@ -851,136 +921,150 @@
     {
         "Items": List[OriginEndpointListConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SegmentOutputTypeDef = TypedDict(
+    "SegmentOutputTypeDef",
+    {
+        "SegmentDurationSeconds": int,
+        "SegmentName": str,
+        "TsUseAudioRenditionGroup": bool,
+        "IncludeIframeOnlyStreams": bool,
+        "TsIncludeDvbSubtitles": bool,
+        "Scte": ScteOutputTypeDef,
+        "Encryption": EncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
 SegmentTypeDef = TypedDict(
     "SegmentTypeDef",
     {
         "SegmentDurationSeconds": int,
         "SegmentName": str,
         "TsUseAudioRenditionGroup": bool,
         "IncludeIframeOnlyStreams": bool,
         "TsIncludeDvbSubtitles": bool,
         "Scte": ScteTypeDef,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
+CreateOriginEndpointResponseTypeDef = TypedDict(
+    "CreateOriginEndpointResponseTypeDef",
     {
+        "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-    },
-)
-_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
-    {
-        "Segment": SegmentTypeDef,
-        "ClientToken": str,
+        "Segment": SegmentOutputTypeDef,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
-        "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
-        "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
-        "Tags": Mapping[str, str],
+        "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
+        "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
+        "Tags": Dict[str, str],
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
+GetOriginEndpointResponseTypeDef = TypedDict(
+    "GetOriginEndpointResponseTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-        "Segment": SegmentTypeDef,
+        "Segment": SegmentOutputTypeDef,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetOriginEndpointResponseTypeDef = TypedDict(
-    "GetOriginEndpointResponseTypeDef",
+UpdateOriginEndpointResponseTypeDef = TypedDict(
+    "UpdateOriginEndpointResponseTypeDef",
     {
         "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
-        "Segment": SegmentTypeDef,
+        "Segment": SegmentOutputTypeDef,
         "CreatedAt": datetime,
         "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
+_RequiredCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOriginEndpointRequestRequestTypeDef",
     {
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
     },
 )
-_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
+_OptionalCreateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOriginEndpointRequestRequestTypeDef",
     {
         "Segment": SegmentTypeDef,
+        "ClientToken": str,
         "Description": str,
         "StartoverWindowSeconds": int,
         "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
         "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-class UpdateOriginEndpointRequestRequestTypeDef(
-    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
-    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
+class CreateOriginEndpointRequestRequestTypeDef(
+    _RequiredCreateOriginEndpointRequestRequestTypeDef,
+    _OptionalCreateOriginEndpointRequestRequestTypeDef,
 ):
     pass
 
-UpdateOriginEndpointResponseTypeDef = TypedDict(
-    "UpdateOriginEndpointResponseTypeDef",
+_RequiredUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateOriginEndpointRequestRequestTypeDef",
     {
-        "Arn": str,
         "ChannelGroupName": str,
         "ChannelName": str,
         "OriginEndpointName": str,
         "ContainerType": ContainerTypeType,
+    },
+)
+_OptionalUpdateOriginEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateOriginEndpointRequestRequestTypeDef",
+    {
         "Segment": SegmentTypeDef,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
         "Description": str,
         "StartoverWindowSeconds": int,
-        "HlsManifests": List[GetHlsManifestConfigurationTypeDef],
-        "LowLatencyHlsManifests": List[GetLowLatencyHlsManifestConfigurationTypeDef],
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "HlsManifests": Sequence[CreateHlsManifestConfigurationTypeDef],
+        "LowLatencyHlsManifests": Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef],
     },
+    total=False,
 )
+
+class UpdateOriginEndpointRequestRequestTypeDef(
+    _RequiredUpdateOriginEndpointRequestRequestTypeDef,
+    _OptionalUpdateOriginEndpointRequestRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2.egg-info/PKG-INFO` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackagev2
-Version: 1.28.0
-Summary: Type annotations for boto3.mediapackagev2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.mediapackagev2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mediapackagev2"></a>
 
 # mypy-boto3-mediapackagev2
 
 [![PyPI - mypy-boto3-mediapackagev2](https://img.shields.io/pypi/v/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackagev2.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackagev2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackagev2?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackagev2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediapackagev2)](https://pepy.tech/project/mypy-boto3-mediapackagev2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.mediapackagev2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
+[boto3.mediapackagev2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
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
 [mypy-boto3-mediapackagev2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackagev2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,21 +353,24 @@
     ScteHlsTypeDef,
     DeleteChannelGroupRequestRequestTypeDef,
     DeleteChannelPolicyRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteOriginEndpointPolicyRequestRequestTypeDef,
     DeleteOriginEndpointRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionContractConfigurationOutputTypeDef,
     EncryptionContractConfigurationTypeDef,
+    EncryptionMethodOutputTypeDef,
     EncryptionMethodTypeDef,
     GetChannelGroupRequestRequestTypeDef,
     GetChannelGroupResponseTypeDef,
     GetChannelPolicyRequestRequestTypeDef,
     GetChannelPolicyResponseTypeDef,
     GetChannelRequestRequestTypeDef,
+    ScteHlsOutputTypeDef,
     GetOriginEndpointPolicyRequestRequestTypeDef,
     GetOriginEndpointPolicyResponseTypeDef,
     GetOriginEndpointRequestRequestTypeDef,
     ListChannelGroupsRequestListChannelGroupsPaginateTypeDef,
     ListChannelGroupsRequestRequestTypeDef,
     ListChannelsRequestListChannelsPaginateTypeDef,
     ListChannelsRequestRequestTypeDef,
@@ -377,39 +380,43 @@
     ListOriginEndpointsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     PutChannelPolicyRequestRequestTypeDef,
     PutOriginEndpointPolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    ScteOutputTypeDef,
     ScteTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateChannelGroupRequestRequestTypeDef,
     UpdateChannelGroupResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     ListChannelGroupsResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelResponseTypeDef,
     GetChannelResponseTypeDef,
     UpdateChannelResponseTypeDef,
     CreateHlsManifestConfigurationTypeDef,
     CreateLowLatencyHlsManifestConfigurationTypeDef,
+    SpekeKeyProviderOutputTypeDef,
+    SpekeKeyProviderTypeDef,
     GetHlsManifestConfigurationTypeDef,
     GetLowLatencyHlsManifestConfigurationTypeDef,
-    SpekeKeyProviderTypeDef,
     OriginEndpointListConfigurationTypeDef,
+    EncryptionOutputTypeDef,
     EncryptionTypeDef,
     ListOriginEndpointsResponseTypeDef,
+    SegmentOutputTypeDef,
     SegmentTypeDef,
-    CreateOriginEndpointRequestRequestTypeDef,
     CreateOriginEndpointResponseTypeDef,
     GetOriginEndpointResponseTypeDef,
-    UpdateOriginEndpointRequestRequestTypeDef,
     UpdateOriginEndpointResponseTypeDef,
+    CreateOriginEndpointRequestRequestTypeDef,
+    UpdateOriginEndpointRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ChannelGroupListConfigurationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mediapackagev2-1.28.0/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt` & `mypy-boto3-mediapackagev2-1.28.12/mypy_boto3_mediapackagev2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackagev2-1.28.0/setup.py` & `mypy-boto3-mediapackagev2-1.28.12/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackagev2",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_mediapackagev2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.mediapackagev2 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.mediapackagev2 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

