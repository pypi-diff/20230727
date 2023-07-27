# Comparing `tmp/mypy-boto3-resource-groups-1.28.0.tar.gz` & `tmp/mypy-boto3-resource-groups-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resource-groups-1.28.0.tar", last modified: Thu Jul  6 21:00:26 2023, max compression
+gzip compressed data, was "mypy-boto3-resource-groups-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
```

## Comparing `mypy-boto3-resource-groups-1.28.0.tar` & `mypy-boto3-resource-groups-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.686409 mypy-boto3-resource-groups-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:15.000000 mypy-boto3-resource-groups-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-07-06 21:00:26.682409 mypy-boto3-resource-groups-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-06 20:53:15.000000 mypy-boto3-resource-groups-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.674409 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-06 20:53:15.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-06 20:53:15.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 20:53:15.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-06 20:53:16.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-06 20:53:15.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-06 20:53:16.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-07-06 20:53:16.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-06 20:53:16.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-06 20:53:16.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:15.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15900 2023-07-06 20:53:16.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-06 20:53:16.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:15.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.682409 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-07-06 21:00:26.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 21:00:26.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:26.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:26.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:26.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 21:00:26.000000 mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:26.686409 mypy-boto3-resource-groups-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-06 20:53:15.000000 mypy-boto3-resource-groups-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.365214 mypy-boto3-resource-groups-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15451 2023-07-27 11:49:30.357214 mypy-boto3-resource-groups-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.357214 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-27 11:44:40.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-07-27 11:44:40.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.357214 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15451 2023-07-27 11:49:30.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 11:49:30.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 11:49:30.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.365214 mypy-boto3-resource-groups-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/setup.py
```

### Comparing `mypy-boto3-resource-groups-1.28.0/LICENSE` & `mypy-boto3-resource-groups-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.0/PKG-INFO` & `mypy-boto3-resource-groups-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-groups
-Version: 1.28.0
-Summary: Type annotations for boto3.ResourceGroups 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ResourceGroups 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-resource-groups"></a>
 
 # mypy-boto3-resource-groups
 
 [![PyPI - mypy-boto3-resource-groups](https://img.shields.io/pypi/v/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resource-groups?color=blue)](https://pypistats.org/packages/mypy-boto3-resource-groups)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-groups)](https://pepy.tech/project/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,62 +341,65 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
+    ResourceQueryOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteGroupInputRequestTypeDef,
     FailedResourceTypeDef,
     GetGroupConfigurationInputRequestTypeDef,
     GetGroupInputRequestTypeDef,
     GetGroupQueryInputRequestTypeDef,
     GetTagsInputRequestTypeDef,
-    GetTagsOutputTypeDef,
+    GroupConfigurationParameterOutputTypeDef,
     GroupConfigurationParameterTypeDef,
     GroupFilterTypeDef,
     GroupIdentifierTypeDef,
     GroupResourcesInputRequestTypeDef,
     PendingResourceTypeDef,
+    PaginatorConfigTypeDef,
     ResourceFilterTypeDef,
     ResourceIdentifierTypeDef,
     ResourceStatusTypeDef,
     QueryErrorTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagInputRequestTypeDef,
-    TagOutputTypeDef,
     UngroupResourcesInputRequestTypeDef,
     UntagInputRequestTypeDef,
-    UntagOutputTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateGroupInputRequestTypeDef,
-    GetAccountSettingsOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
-    GroupQueryTypeDef,
     SearchResourcesInputRequestTypeDef,
-    SearchResourcesInputSearchResourcesPaginateTypeDef,
     UpdateGroupQueryInputRequestTypeDef,
+    GroupQueryTypeDef,
     DeleteGroupOutputTypeDef,
+    GetAccountSettingsOutputTypeDef,
     GetGroupOutputTypeDef,
+    GetTagsOutputTypeDef,
+    TagOutputTypeDef,
+    UntagOutputTypeDef,
+    UpdateAccountSettingsOutputTypeDef,
     UpdateGroupOutputTypeDef,
+    GroupConfigurationItemOutputTypeDef,
     GroupConfigurationItemTypeDef,
-    ListGroupsInputListGroupsPaginateTypeDef,
     ListGroupsInputRequestTypeDef,
     ListGroupsOutputTypeDef,
     GroupResourcesOutputTypeDef,
     UngroupResourcesOutputTypeDef,
+    ListGroupsInputListGroupsPaginateTypeDef,
+    SearchResourcesInputSearchResourcesPaginateTypeDef,
     ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
     ListGroupResourcesInputRequestTypeDef,
     ListGroupResourcesItemTypeDef,
     SearchResourcesOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     UpdateGroupQueryOutputTypeDef,
-    CreateGroupInputRequestTypeDef,
     GroupConfigurationTypeDef,
+    CreateGroupInputRequestTypeDef,
     PutGroupConfigurationInputRequestTypeDef,
     ListGroupResourcesOutputTypeDef,
     CreateGroupOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
 )
```

### Comparing `mypy-boto3-resource-groups-1.28.0/README.md` & `mypy-boto3-resource-groups-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-resource-groups"></a>
 
 # mypy-boto3-resource-groups
 
 [![PyPI - mypy-boto3-resource-groups](https://img.shields.io/pypi/v/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resource-groups?color=blue)](https://pypistats.org/packages/mypy-boto3-resource-groups)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-groups)](https://pepy.tech/project/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,62 +309,65 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
+    ResourceQueryOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteGroupInputRequestTypeDef,
     FailedResourceTypeDef,
     GetGroupConfigurationInputRequestTypeDef,
     GetGroupInputRequestTypeDef,
     GetGroupQueryInputRequestTypeDef,
     GetTagsInputRequestTypeDef,
-    GetTagsOutputTypeDef,
+    GroupConfigurationParameterOutputTypeDef,
     GroupConfigurationParameterTypeDef,
     GroupFilterTypeDef,
     GroupIdentifierTypeDef,
     GroupResourcesInputRequestTypeDef,
     PendingResourceTypeDef,
+    PaginatorConfigTypeDef,
     ResourceFilterTypeDef,
     ResourceIdentifierTypeDef,
     ResourceStatusTypeDef,
     QueryErrorTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagInputRequestTypeDef,
-    TagOutputTypeDef,
     UngroupResourcesInputRequestTypeDef,
     UntagInputRequestTypeDef,
-    UntagOutputTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateGroupInputRequestTypeDef,
-    GetAccountSettingsOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
-    GroupQueryTypeDef,
     SearchResourcesInputRequestTypeDef,
-    SearchResourcesInputSearchResourcesPaginateTypeDef,
     UpdateGroupQueryInputRequestTypeDef,
+    GroupQueryTypeDef,
     DeleteGroupOutputTypeDef,
+    GetAccountSettingsOutputTypeDef,
     GetGroupOutputTypeDef,
+    GetTagsOutputTypeDef,
+    TagOutputTypeDef,
+    UntagOutputTypeDef,
+    UpdateAccountSettingsOutputTypeDef,
     UpdateGroupOutputTypeDef,
+    GroupConfigurationItemOutputTypeDef,
     GroupConfigurationItemTypeDef,
-    ListGroupsInputListGroupsPaginateTypeDef,
     ListGroupsInputRequestTypeDef,
     ListGroupsOutputTypeDef,
     GroupResourcesOutputTypeDef,
     UngroupResourcesOutputTypeDef,
+    ListGroupsInputListGroupsPaginateTypeDef,
+    SearchResourcesInputSearchResourcesPaginateTypeDef,
     ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
     ListGroupResourcesInputRequestTypeDef,
     ListGroupResourcesItemTypeDef,
     SearchResourcesOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     UpdateGroupQueryOutputTypeDef,
-    CreateGroupInputRequestTypeDef,
     GroupConfigurationTypeDef,
+    CreateGroupInputRequestTypeDef,
     PutGroupConfigurationInputRequestTypeDef,
     ListGroupResourcesOutputTypeDef,
     CreateGroupOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
 )
```

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/__init__.py` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/__init__.pyi` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/__main__.py` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResourceGroups 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ResourceGroups 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups\nOther"
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

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/client.py` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/client.pyi` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/literals.py` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,15 @@
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
@@ -256,26 +257,28 @@
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

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/literals.pyi` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
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
@@ -254,26 +255,28 @@
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

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/paginator.py` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroupResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupresourcespaginator)
         """
 
 
@@ -76,31 +76,28 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupspaginator)
         """
 
 
 class SearchResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#searchresourcespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ResourceQuery: ResourceQueryTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceQuery: ResourceQueryTypeDef, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#searchresourcespaginator)
         """
```

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/paginator.pyi` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroupResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupresourcespaginator)
         """
 
 class ListGroupsPaginator(Paginator):
@@ -72,30 +72,27 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#listgroupspaginator)
         """
 
 class SearchResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#searchresourcespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ResourceQuery: ResourceQueryTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceQuery: ResourceQueryTypeDef, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/paginators/#searchresourcespaginator)
         """
```

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/type_defs.py` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,62 +33,65 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountSettingsTypeDef",
     "ResourceQueryTypeDef",
     "GroupTypeDef",
+    "ResourceQueryOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
     "GetGroupConfigurationInputRequestTypeDef",
     "GetGroupInputRequestTypeDef",
     "GetGroupQueryInputRequestTypeDef",
     "GetTagsInputRequestTypeDef",
-    "GetTagsOutputTypeDef",
+    "GroupConfigurationParameterOutputTypeDef",
     "GroupConfigurationParameterTypeDef",
     "GroupFilterTypeDef",
     "GroupIdentifierTypeDef",
     "GroupResourcesInputRequestTypeDef",
     "PendingResourceTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceFilterTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceStatusTypeDef",
     "QueryErrorTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagInputRequestTypeDef",
-    "TagOutputTypeDef",
     "UngroupResourcesInputRequestTypeDef",
     "UntagInputRequestTypeDef",
-    "UntagOutputTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateGroupInputRequestTypeDef",
-    "GetAccountSettingsOutputTypeDef",
-    "UpdateAccountSettingsOutputTypeDef",
-    "GroupQueryTypeDef",
     "SearchResourcesInputRequestTypeDef",
-    "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "UpdateGroupQueryInputRequestTypeDef",
+    "GroupQueryTypeDef",
     "DeleteGroupOutputTypeDef",
+    "GetAccountSettingsOutputTypeDef",
     "GetGroupOutputTypeDef",
+    "GetTagsOutputTypeDef",
+    "TagOutputTypeDef",
+    "UntagOutputTypeDef",
+    "UpdateAccountSettingsOutputTypeDef",
     "UpdateGroupOutputTypeDef",
+    "GroupConfigurationItemOutputTypeDef",
     "GroupConfigurationItemTypeDef",
-    "ListGroupsInputListGroupsPaginateTypeDef",
     "ListGroupsInputRequestTypeDef",
     "ListGroupsOutputTypeDef",
     "GroupResourcesOutputTypeDef",
     "UngroupResourcesOutputTypeDef",
+    "ListGroupsInputListGroupsPaginateTypeDef",
+    "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     "ListGroupResourcesInputRequestTypeDef",
     "ListGroupResourcesItemTypeDef",
     "SearchResourcesOutputTypeDef",
     "GetGroupQueryOutputTypeDef",
     "UpdateGroupQueryOutputTypeDef",
-    "CreateGroupInputRequestTypeDef",
     "GroupConfigurationTypeDef",
+    "CreateGroupInputRequestTypeDef",
     "PutGroupConfigurationInputRequestTypeDef",
     "ListGroupResourcesOutputTypeDef",
     "CreateGroupOutputTypeDef",
     "GetGroupConfigurationOutputTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
@@ -125,14 +128,33 @@
 )
 
 
 class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
     pass
 
 
+ResourceQueryOutputTypeDef = TypedDict(
+    "ResourceQueryOutputTypeDef",
+    {
+        "Type": QueryTypeType,
+        "Query": str,
+    },
+)
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
 DeleteGroupInputRequestTypeDef = TypedDict(
     "DeleteGroupInputRequestTypeDef",
     {
         "GroupName": str,
         "Group": str,
     },
     total=False,
@@ -177,23 +199,36 @@
 GetTagsInputRequestTypeDef = TypedDict(
     "GetTagsInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetTagsOutputTypeDef = TypedDict(
-    "GetTagsOutputTypeDef",
+_RequiredGroupConfigurationParameterOutputTypeDef = TypedDict(
+    "_RequiredGroupConfigurationParameterOutputTypeDef",
     {
-        "Arn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+    },
+)
+_OptionalGroupConfigurationParameterOutputTypeDef = TypedDict(
+    "_OptionalGroupConfigurationParameterOutputTypeDef",
+    {
+        "Values": List[str],
     },
+    total=False,
 )
 
+
+class GroupConfigurationParameterOutputTypeDef(
+    _RequiredGroupConfigurationParameterOutputTypeDef,
+    _OptionalGroupConfigurationParameterOutputTypeDef,
+):
+    pass
+
+
 _RequiredGroupConfigurationParameterTypeDef = TypedDict(
     "_RequiredGroupConfigurationParameterTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGroupConfigurationParameterTypeDef = TypedDict(
@@ -240,14 +275,24 @@
     "PendingResourceTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ResourceFilterTypeDef = TypedDict(
     "ResourceFilterTypeDef",
     {
         "Name": Literal["resource-type"],
         "Values": Sequence[str],
     },
 )
@@ -274,52 +319,22 @@
     {
         "ErrorCode": QueryErrorCodeType,
         "Message": str,
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
 TagInputRequestTypeDef = TypedDict(
     "TagInputRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Arn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UngroupResourcesInputRequestTypeDef = TypedDict(
     "UngroupResourcesInputRequestTypeDef",
     {
         "Group": str,
         "ResourceArns": Sequence[str],
     },
 )
@@ -328,23 +343,14 @@
     "UntagInputRequestTypeDef",
     {
         "Arn": str,
         "Keys": Sequence[str],
     },
 )
 
-UntagOutputTypeDef = TypedDict(
-    "UntagOutputTypeDef",
-    {
-        "Arn": str,
-        "Keys": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountSettingsInputRequestTypeDef = TypedDict(
     "UpdateAccountSettingsInputRequestTypeDef",
     {
         "GroupLifecycleEventsDesiredStatus": GroupLifecycleEventsDesiredStatusType,
     },
     total=False,
 )
@@ -355,38 +361,14 @@
         "GroupName": str,
         "Group": str,
         "Description": str,
     },
     total=False,
 )
 
-GetAccountSettingsOutputTypeDef = TypedDict(
-    "GetAccountSettingsOutputTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAccountSettingsOutputTypeDef = TypedDict(
-    "UpdateAccountSettingsOutputTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GroupQueryTypeDef = TypedDict(
-    "GroupQueryTypeDef",
-    {
-        "GroupName": str,
-        "ResourceQuery": ResourceQueryTypeDef,
-    },
-)
-
 _RequiredSearchResourcesInputRequestTypeDef = TypedDict(
     "_RequiredSearchResourcesInputRequestTypeDef",
     {
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
 _OptionalSearchResourcesInputRequestTypeDef = TypedDict(
@@ -401,36 +383,14 @@
 
 class SearchResourcesInputRequestTypeDef(
     _RequiredSearchResourcesInputRequestTypeDef, _OptionalSearchResourcesInputRequestTypeDef
 ):
     pass
 
 
-_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
-    "_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef",
-    {
-        "ResourceQuery": ResourceQueryTypeDef,
-    },
-)
-_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
-    "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SearchResourcesInputSearchResourcesPaginateTypeDef(
-    _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
-    _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredUpdateGroupQueryInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupQueryInputRequestTypeDef",
     {
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
 _OptionalUpdateGroupQueryInputRequestTypeDef = TypedDict(
@@ -445,38 +405,110 @@
 
 class UpdateGroupQueryInputRequestTypeDef(
     _RequiredUpdateGroupQueryInputRequestTypeDef, _OptionalUpdateGroupQueryInputRequestTypeDef
 ):
     pass
 
 
+GroupQueryTypeDef = TypedDict(
+    "GroupQueryTypeDef",
+    {
+        "GroupName": str,
+        "ResourceQuery": ResourceQueryOutputTypeDef,
+    },
+)
+
 DeleteGroupOutputTypeDef = TypedDict(
     "DeleteGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountSettingsOutputTypeDef = TypedDict(
+    "GetAccountSettingsOutputTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupOutputTypeDef = TypedDict(
     "GetGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsOutputTypeDef = TypedDict(
+    "GetTagsOutputTypeDef",
+    {
+        "Arn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Arn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UntagOutputTypeDef = TypedDict(
+    "UntagOutputTypeDef",
+    {
+        "Arn": str,
+        "Keys": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAccountSettingsOutputTypeDef = TypedDict(
+    "UpdateAccountSettingsOutputTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupOutputTypeDef = TypedDict(
     "UpdateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGroupConfigurationItemOutputTypeDef = TypedDict(
+    "_RequiredGroupConfigurationItemOutputTypeDef",
+    {
+        "Type": str,
+    },
+)
+_OptionalGroupConfigurationItemOutputTypeDef = TypedDict(
+    "_OptionalGroupConfigurationItemOutputTypeDef",
+    {
+        "Parameters": List[GroupConfigurationParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class GroupConfigurationItemOutputTypeDef(
+    _RequiredGroupConfigurationItemOutputTypeDef, _OptionalGroupConfigurationItemOutputTypeDef
+):
+    pass
+
+
 _RequiredGroupConfigurationItemTypeDef = TypedDict(
     "_RequiredGroupConfigurationItemTypeDef",
     {
         "Type": str,
     },
 )
 _OptionalGroupConfigurationItemTypeDef = TypedDict(
@@ -490,23 +522,14 @@
 
 class GroupConfigurationItemTypeDef(
     _RequiredGroupConfigurationItemTypeDef, _OptionalGroupConfigurationItemTypeDef
 ):
     pass
 
 
-ListGroupsInputListGroupsPaginateTypeDef = TypedDict(
-    "ListGroupsInputListGroupsPaginateTypeDef",
-    {
-        "Filters": Sequence[GroupFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGroupsInputRequestTypeDef = TypedDict(
     "ListGroupsInputRequestTypeDef",
     {
         "Filters": Sequence[GroupFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -515,45 +538,76 @@
 
 ListGroupsOutputTypeDef = TypedDict(
     "ListGroupsOutputTypeDef",
     {
         "GroupIdentifiers": List[GroupIdentifierTypeDef],
         "Groups": List[GroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GroupResourcesOutputTypeDef = TypedDict(
     "GroupResourcesOutputTypeDef",
     {
         "Succeeded": List[str],
         "Failed": List[FailedResourceTypeDef],
         "Pending": List[PendingResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UngroupResourcesOutputTypeDef = TypedDict(
     "UngroupResourcesOutputTypeDef",
     {
         "Succeeded": List[str],
         "Failed": List[FailedResourceTypeDef],
         "Pending": List[PendingResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGroupsInputListGroupsPaginateTypeDef = TypedDict(
+    "ListGroupsInputListGroupsPaginateTypeDef",
+    {
+        "Filters": Sequence[GroupFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
+    "_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef",
+    {
+        "ResourceQuery": ResourceQueryTypeDef,
+    },
+)
+_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
+    "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class SearchResourcesInputSearchResourcesPaginateTypeDef(
+    _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
+    _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
+):
+    pass
+
+
 ListGroupResourcesInputListGroupResourcesPaginateTypeDef = TypedDict(
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     {
         "GroupName": str,
         "Group": str,
         "Filters": Sequence[ResourceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListGroupResourcesInputRequestTypeDef = TypedDict(
     "ListGroupResourcesInputRequestTypeDef",
     {
@@ -577,32 +631,43 @@
 
 SearchResourcesOutputTypeDef = TypedDict(
     "SearchResourcesOutputTypeDef",
     {
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupQueryOutputTypeDef = TypedDict(
     "GetGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupQueryOutputTypeDef = TypedDict(
     "UpdateGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GroupConfigurationTypeDef = TypedDict(
+    "GroupConfigurationTypeDef",
+    {
+        "Configuration": List[GroupConfigurationItemOutputTypeDef],
+        "ProposedConfiguration": List[GroupConfigurationItemOutputTypeDef],
+        "Status": GroupConfigurationStatusType,
+        "FailureReason": str,
     },
+    total=False,
 )
 
 _RequiredCreateGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateGroupInputRequestTypeDef",
     {
         "Name": str,
     },
@@ -621,25 +686,14 @@
 
 class CreateGroupInputRequestTypeDef(
     _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
 ):
     pass
 
 
-GroupConfigurationTypeDef = TypedDict(
-    "GroupConfigurationTypeDef",
-    {
-        "Configuration": List[GroupConfigurationItemTypeDef],
-        "ProposedConfiguration": List[GroupConfigurationItemTypeDef],
-        "Status": GroupConfigurationStatusType,
-        "FailureReason": str,
-    },
-    total=False,
-)
-
 PutGroupConfigurationInputRequestTypeDef = TypedDict(
     "PutGroupConfigurationInputRequestTypeDef",
     {
         "Group": str,
         "Configuration": Sequence[GroupConfigurationItemTypeDef],
     },
     total=False,
@@ -648,29 +702,29 @@
 ListGroupResourcesOutputTypeDef = TypedDict(
     "ListGroupResourcesOutputTypeDef",
     {
         "Resources": List[ListGroupResourcesItemTypeDef],
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGroupOutputTypeDef = TypedDict(
     "CreateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResourceQuery": ResourceQueryTypeDef,
+        "ResourceQuery": ResourceQueryOutputTypeDef,
         "Tags": Dict[str, str],
         "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupConfigurationOutputTypeDef = TypedDict(
     "GetGroupConfigurationOutputTypeDef",
     {
         "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups/type_defs.pyi` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -32,62 +32,65 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountSettingsTypeDef",
     "ResourceQueryTypeDef",
     "GroupTypeDef",
+    "ResourceQueryOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
     "GetGroupConfigurationInputRequestTypeDef",
     "GetGroupInputRequestTypeDef",
     "GetGroupQueryInputRequestTypeDef",
     "GetTagsInputRequestTypeDef",
-    "GetTagsOutputTypeDef",
+    "GroupConfigurationParameterOutputTypeDef",
     "GroupConfigurationParameterTypeDef",
     "GroupFilterTypeDef",
     "GroupIdentifierTypeDef",
     "GroupResourcesInputRequestTypeDef",
     "PendingResourceTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceFilterTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceStatusTypeDef",
     "QueryErrorTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagInputRequestTypeDef",
-    "TagOutputTypeDef",
     "UngroupResourcesInputRequestTypeDef",
     "UntagInputRequestTypeDef",
-    "UntagOutputTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateGroupInputRequestTypeDef",
-    "GetAccountSettingsOutputTypeDef",
-    "UpdateAccountSettingsOutputTypeDef",
-    "GroupQueryTypeDef",
     "SearchResourcesInputRequestTypeDef",
-    "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "UpdateGroupQueryInputRequestTypeDef",
+    "GroupQueryTypeDef",
     "DeleteGroupOutputTypeDef",
+    "GetAccountSettingsOutputTypeDef",
     "GetGroupOutputTypeDef",
+    "GetTagsOutputTypeDef",
+    "TagOutputTypeDef",
+    "UntagOutputTypeDef",
+    "UpdateAccountSettingsOutputTypeDef",
     "UpdateGroupOutputTypeDef",
+    "GroupConfigurationItemOutputTypeDef",
     "GroupConfigurationItemTypeDef",
-    "ListGroupsInputListGroupsPaginateTypeDef",
     "ListGroupsInputRequestTypeDef",
     "ListGroupsOutputTypeDef",
     "GroupResourcesOutputTypeDef",
     "UngroupResourcesOutputTypeDef",
+    "ListGroupsInputListGroupsPaginateTypeDef",
+    "SearchResourcesInputSearchResourcesPaginateTypeDef",
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     "ListGroupResourcesInputRequestTypeDef",
     "ListGroupResourcesItemTypeDef",
     "SearchResourcesOutputTypeDef",
     "GetGroupQueryOutputTypeDef",
     "UpdateGroupQueryOutputTypeDef",
-    "CreateGroupInputRequestTypeDef",
     "GroupConfigurationTypeDef",
+    "CreateGroupInputRequestTypeDef",
     "PutGroupConfigurationInputRequestTypeDef",
     "ListGroupResourcesOutputTypeDef",
     "CreateGroupOutputTypeDef",
     "GetGroupConfigurationOutputTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
@@ -122,14 +125,33 @@
     },
     total=False,
 )
 
 class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
     pass
 
+ResourceQueryOutputTypeDef = TypedDict(
+    "ResourceQueryOutputTypeDef",
+    {
+        "Type": QueryTypeType,
+        "Query": str,
+    },
+)
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
 DeleteGroupInputRequestTypeDef = TypedDict(
     "DeleteGroupInputRequestTypeDef",
     {
         "GroupName": str,
         "Group": str,
     },
     total=False,
@@ -174,22 +196,33 @@
 GetTagsInputRequestTypeDef = TypedDict(
     "GetTagsInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetTagsOutputTypeDef = TypedDict(
-    "GetTagsOutputTypeDef",
+_RequiredGroupConfigurationParameterOutputTypeDef = TypedDict(
+    "_RequiredGroupConfigurationParameterOutputTypeDef",
     {
-        "Arn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
     },
 )
+_OptionalGroupConfigurationParameterOutputTypeDef = TypedDict(
+    "_OptionalGroupConfigurationParameterOutputTypeDef",
+    {
+        "Values": List[str],
+    },
+    total=False,
+)
+
+class GroupConfigurationParameterOutputTypeDef(
+    _RequiredGroupConfigurationParameterOutputTypeDef,
+    _OptionalGroupConfigurationParameterOutputTypeDef,
+):
+    pass
 
 _RequiredGroupConfigurationParameterTypeDef = TypedDict(
     "_RequiredGroupConfigurationParameterTypeDef",
     {
         "Name": str,
     },
 )
@@ -235,14 +268,24 @@
     "PendingResourceTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ResourceFilterTypeDef = TypedDict(
     "ResourceFilterTypeDef",
     {
         "Name": Literal["resource-type"],
         "Values": Sequence[str],
     },
 )
@@ -269,52 +312,22 @@
     {
         "ErrorCode": QueryErrorCodeType,
         "Message": str,
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
 TagInputRequestTypeDef = TypedDict(
     "TagInputRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Arn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UngroupResourcesInputRequestTypeDef = TypedDict(
     "UngroupResourcesInputRequestTypeDef",
     {
         "Group": str,
         "ResourceArns": Sequence[str],
     },
 )
@@ -323,23 +336,14 @@
     "UntagInputRequestTypeDef",
     {
         "Arn": str,
         "Keys": Sequence[str],
     },
 )
 
-UntagOutputTypeDef = TypedDict(
-    "UntagOutputTypeDef",
-    {
-        "Arn": str,
-        "Keys": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountSettingsInputRequestTypeDef = TypedDict(
     "UpdateAccountSettingsInputRequestTypeDef",
     {
         "GroupLifecycleEventsDesiredStatus": GroupLifecycleEventsDesiredStatusType,
     },
     total=False,
 )
@@ -350,38 +354,14 @@
         "GroupName": str,
         "Group": str,
         "Description": str,
     },
     total=False,
 )
 
-GetAccountSettingsOutputTypeDef = TypedDict(
-    "GetAccountSettingsOutputTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAccountSettingsOutputTypeDef = TypedDict(
-    "UpdateAccountSettingsOutputTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GroupQueryTypeDef = TypedDict(
-    "GroupQueryTypeDef",
-    {
-        "GroupName": str,
-        "ResourceQuery": ResourceQueryTypeDef,
-    },
-)
-
 _RequiredSearchResourcesInputRequestTypeDef = TypedDict(
     "_RequiredSearchResourcesInputRequestTypeDef",
     {
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
 _OptionalSearchResourcesInputRequestTypeDef = TypedDict(
@@ -394,34 +374,14 @@
 )
 
 class SearchResourcesInputRequestTypeDef(
     _RequiredSearchResourcesInputRequestTypeDef, _OptionalSearchResourcesInputRequestTypeDef
 ):
     pass
 
-_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
-    "_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef",
-    {
-        "ResourceQuery": ResourceQueryTypeDef,
-    },
-)
-_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
-    "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SearchResourcesInputSearchResourcesPaginateTypeDef(
-    _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
-    _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredUpdateGroupQueryInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGroupQueryInputRequestTypeDef",
     {
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
 _OptionalUpdateGroupQueryInputRequestTypeDef = TypedDict(
@@ -434,38 +394,108 @@
 )
 
 class UpdateGroupQueryInputRequestTypeDef(
     _RequiredUpdateGroupQueryInputRequestTypeDef, _OptionalUpdateGroupQueryInputRequestTypeDef
 ):
     pass
 
+GroupQueryTypeDef = TypedDict(
+    "GroupQueryTypeDef",
+    {
+        "GroupName": str,
+        "ResourceQuery": ResourceQueryOutputTypeDef,
+    },
+)
+
 DeleteGroupOutputTypeDef = TypedDict(
     "DeleteGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountSettingsOutputTypeDef = TypedDict(
+    "GetAccountSettingsOutputTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupOutputTypeDef = TypedDict(
     "GetGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsOutputTypeDef = TypedDict(
+    "GetTagsOutputTypeDef",
+    {
+        "Arn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Arn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UntagOutputTypeDef = TypedDict(
+    "UntagOutputTypeDef",
+    {
+        "Arn": str,
+        "Keys": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAccountSettingsOutputTypeDef = TypedDict(
+    "UpdateAccountSettingsOutputTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupOutputTypeDef = TypedDict(
     "UpdateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGroupConfigurationItemOutputTypeDef = TypedDict(
+    "_RequiredGroupConfigurationItemOutputTypeDef",
+    {
+        "Type": str,
+    },
+)
+_OptionalGroupConfigurationItemOutputTypeDef = TypedDict(
+    "_OptionalGroupConfigurationItemOutputTypeDef",
+    {
+        "Parameters": List[GroupConfigurationParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+class GroupConfigurationItemOutputTypeDef(
+    _RequiredGroupConfigurationItemOutputTypeDef, _OptionalGroupConfigurationItemOutputTypeDef
+):
+    pass
+
 _RequiredGroupConfigurationItemTypeDef = TypedDict(
     "_RequiredGroupConfigurationItemTypeDef",
     {
         "Type": str,
     },
 )
 _OptionalGroupConfigurationItemTypeDef = TypedDict(
@@ -477,23 +507,14 @@
 )
 
 class GroupConfigurationItemTypeDef(
     _RequiredGroupConfigurationItemTypeDef, _OptionalGroupConfigurationItemTypeDef
 ):
     pass
 
-ListGroupsInputListGroupsPaginateTypeDef = TypedDict(
-    "ListGroupsInputListGroupsPaginateTypeDef",
-    {
-        "Filters": Sequence[GroupFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGroupsInputRequestTypeDef = TypedDict(
     "ListGroupsInputRequestTypeDef",
     {
         "Filters": Sequence[GroupFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -502,45 +523,74 @@
 
 ListGroupsOutputTypeDef = TypedDict(
     "ListGroupsOutputTypeDef",
     {
         "GroupIdentifiers": List[GroupIdentifierTypeDef],
         "Groups": List[GroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GroupResourcesOutputTypeDef = TypedDict(
     "GroupResourcesOutputTypeDef",
     {
         "Succeeded": List[str],
         "Failed": List[FailedResourceTypeDef],
         "Pending": List[PendingResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UngroupResourcesOutputTypeDef = TypedDict(
     "UngroupResourcesOutputTypeDef",
     {
         "Succeeded": List[str],
         "Failed": List[FailedResourceTypeDef],
         "Pending": List[PendingResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGroupsInputListGroupsPaginateTypeDef = TypedDict(
+    "ListGroupsInputListGroupsPaginateTypeDef",
+    {
+        "Filters": Sequence[GroupFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
+    "_RequiredSearchResourcesInputSearchResourcesPaginateTypeDef",
+    {
+        "ResourceQuery": ResourceQueryTypeDef,
     },
 )
+_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef = TypedDict(
+    "_OptionalSearchResourcesInputSearchResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SearchResourcesInputSearchResourcesPaginateTypeDef(
+    _RequiredSearchResourcesInputSearchResourcesPaginateTypeDef,
+    _OptionalSearchResourcesInputSearchResourcesPaginateTypeDef,
+):
+    pass
 
 ListGroupResourcesInputListGroupResourcesPaginateTypeDef = TypedDict(
     "ListGroupResourcesInputListGroupResourcesPaginateTypeDef",
     {
         "GroupName": str,
         "Group": str,
         "Filters": Sequence[ResourceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListGroupResourcesInputRequestTypeDef = TypedDict(
     "ListGroupResourcesInputRequestTypeDef",
     {
@@ -564,34 +614,45 @@
 
 SearchResourcesOutputTypeDef = TypedDict(
     "SearchResourcesOutputTypeDef",
     {
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupQueryOutputTypeDef = TypedDict(
     "GetGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupQueryOutputTypeDef = TypedDict(
     "UpdateGroupQueryOutputTypeDef",
     {
         "GroupQuery": GroupQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GroupConfigurationTypeDef = TypedDict(
+    "GroupConfigurationTypeDef",
+    {
+        "Configuration": List[GroupConfigurationItemOutputTypeDef],
+        "ProposedConfiguration": List[GroupConfigurationItemOutputTypeDef],
+        "Status": GroupConfigurationStatusType,
+        "FailureReason": str,
+    },
+    total=False,
+)
+
 _RequiredCreateGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateGroupInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateGroupInputRequestTypeDef = TypedDict(
@@ -606,25 +667,14 @@
 )
 
 class CreateGroupInputRequestTypeDef(
     _RequiredCreateGroupInputRequestTypeDef, _OptionalCreateGroupInputRequestTypeDef
 ):
     pass
 
-GroupConfigurationTypeDef = TypedDict(
-    "GroupConfigurationTypeDef",
-    {
-        "Configuration": List[GroupConfigurationItemTypeDef],
-        "ProposedConfiguration": List[GroupConfigurationItemTypeDef],
-        "Status": GroupConfigurationStatusType,
-        "FailureReason": str,
-    },
-    total=False,
-)
-
 PutGroupConfigurationInputRequestTypeDef = TypedDict(
     "PutGroupConfigurationInputRequestTypeDef",
     {
         "Group": str,
         "Configuration": Sequence[GroupConfigurationItemTypeDef],
     },
     total=False,
@@ -633,29 +683,29 @@
 ListGroupResourcesOutputTypeDef = TypedDict(
     "ListGroupResourcesOutputTypeDef",
     {
         "Resources": List[ListGroupResourcesItemTypeDef],
         "ResourceIdentifiers": List[ResourceIdentifierTypeDef],
         "NextToken": str,
         "QueryErrors": List[QueryErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGroupOutputTypeDef = TypedDict(
     "CreateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResourceQuery": ResourceQueryTypeDef,
+        "ResourceQuery": ResourceQueryOutputTypeDef,
         "Tags": Dict[str, str],
         "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupConfigurationOutputTypeDef = TypedDict(
     "GetGroupConfigurationOutputTypeDef",
     {
         "GroupConfiguration": GroupConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups.egg-info/PKG-INFO` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-groups
-Version: 1.28.0
-Summary: Type annotations for boto3.ResourceGroups 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ResourceGroups 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-resource-groups"></a>
 
 # mypy-boto3-resource-groups
 
 [![PyPI - mypy-boto3-resource-groups](https://img.shields.io/pypi/v/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resource-groups?color=blue)](https://pypistats.org/packages/mypy-boto3-resource-groups)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-groups)](https://pepy.tech/project/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,62 +341,65 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
+    ResourceQueryOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteGroupInputRequestTypeDef,
     FailedResourceTypeDef,
     GetGroupConfigurationInputRequestTypeDef,
     GetGroupInputRequestTypeDef,
     GetGroupQueryInputRequestTypeDef,
     GetTagsInputRequestTypeDef,
-    GetTagsOutputTypeDef,
+    GroupConfigurationParameterOutputTypeDef,
     GroupConfigurationParameterTypeDef,
     GroupFilterTypeDef,
     GroupIdentifierTypeDef,
     GroupResourcesInputRequestTypeDef,
     PendingResourceTypeDef,
+    PaginatorConfigTypeDef,
     ResourceFilterTypeDef,
     ResourceIdentifierTypeDef,
     ResourceStatusTypeDef,
     QueryErrorTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagInputRequestTypeDef,
-    TagOutputTypeDef,
     UngroupResourcesInputRequestTypeDef,
     UntagInputRequestTypeDef,
-    UntagOutputTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateGroupInputRequestTypeDef,
-    GetAccountSettingsOutputTypeDef,
-    UpdateAccountSettingsOutputTypeDef,
-    GroupQueryTypeDef,
     SearchResourcesInputRequestTypeDef,
-    SearchResourcesInputSearchResourcesPaginateTypeDef,
     UpdateGroupQueryInputRequestTypeDef,
+    GroupQueryTypeDef,
     DeleteGroupOutputTypeDef,
+    GetAccountSettingsOutputTypeDef,
     GetGroupOutputTypeDef,
+    GetTagsOutputTypeDef,
+    TagOutputTypeDef,
+    UntagOutputTypeDef,
+    UpdateAccountSettingsOutputTypeDef,
     UpdateGroupOutputTypeDef,
+    GroupConfigurationItemOutputTypeDef,
     GroupConfigurationItemTypeDef,
-    ListGroupsInputListGroupsPaginateTypeDef,
     ListGroupsInputRequestTypeDef,
     ListGroupsOutputTypeDef,
     GroupResourcesOutputTypeDef,
     UngroupResourcesOutputTypeDef,
+    ListGroupsInputListGroupsPaginateTypeDef,
+    SearchResourcesInputSearchResourcesPaginateTypeDef,
     ListGroupResourcesInputListGroupResourcesPaginateTypeDef,
     ListGroupResourcesInputRequestTypeDef,
     ListGroupResourcesItemTypeDef,
     SearchResourcesOutputTypeDef,
     GetGroupQueryOutputTypeDef,
     UpdateGroupQueryOutputTypeDef,
-    CreateGroupInputRequestTypeDef,
     GroupConfigurationTypeDef,
+    CreateGroupInputRequestTypeDef,
     PutGroupConfigurationInputRequestTypeDef,
     ListGroupResourcesOutputTypeDef,
     CreateGroupOutputTypeDef,
     GetGroupConfigurationOutputTypeDef,
 )
```

### Comparing `mypy-boto3-resource-groups-1.28.0/mypy_boto3_resource_groups.egg-info/SOURCES.txt` & `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.0/setup.py` & `mypy-boto3-resource-groups-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resource-groups",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_resource_groups"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResourceGroups 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ResourceGroups 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

