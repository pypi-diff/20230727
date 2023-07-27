# Comparing `tmp/mypy-boto3-rolesanywhere-1.28.0.tar.gz` & `tmp/mypy-boto3-rolesanywhere-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rolesanywhere-1.28.0.tar", last modified: Thu Jul  6 21:00:28 2023, max compression
+gzip compressed data, was "mypy-boto3-rolesanywhere-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
```

## Comparing `mypy-boto3-rolesanywhere-1.28.0.tar` & `mypy-boto3-rolesanywhere-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:28.454412 mypy-boto3-rolesanywhere-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14985 2023-07-06 21:00:28.446412 mypy-boto3-rolesanywhere-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:28.446412 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20567 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-06 20:53:27.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15319 2023-07-06 20:53:27.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:28.446412 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14985 2023-07-06 21:00:28.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 21:00:28.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:28.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:28.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:28.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 21:00:28.000000 mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:28.454412 mypy-boto3-rolesanywhere-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-06 20:53:26.000000 mypy-boto3-rolesanywhere-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.689217 mypy-boto3-rolesanywhere-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-07-27 11:49:30.681217 mypy-boto3-rolesanywhere-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.681217 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20567 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.681217 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-07-27 11:49:30.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 11:49:30.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:49:30.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.689217 mypy-boto3-rolesanywhere-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/setup.py
```

### Comparing `mypy-boto3-rolesanywhere-1.28.0/LICENSE` & `mypy-boto3-rolesanywhere-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.0/PKG-INFO` & `mypy-boto3-rolesanywhere-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.28.0
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-rolesanywhere"></a>
 
 # mypy-boto3-rolesanywhere
 
 [![PyPI - mypy-boto3-rolesanywhere](https://img.shields.io/pypi/v/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rolesanywhere?color=blue)](https://pypistats.org/packages/mypy-boto3-rolesanywhere)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [mypy-boto3-rolesanywhere docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,51 +338,54 @@
 
 ```python
 from mypy_boto3_rolesanywhere.type_defs import (
     TagTypeDef,
     NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
+    ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
-    ListRequestListCrlsPaginateTypeDef,
-    ListRequestListProfilesPaginateTypeDef,
-    ListRequestListSubjectsPaginateTypeDef,
-    ListRequestListTrustAnchorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     NotificationSettingDetailTypeDef,
     NotificationSettingKeyTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
+    SourceDataOutputTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
+    ListRequestListCrlsPaginateTypeDef,
+    ListRequestListProfilesPaginateTypeDef,
+    ListRequestListSubjectsPaginateTypeDef,
+    ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ResetNotificationSettingsRequestRequestTypeDef,
+    SourceOutputTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
-    CreateTrustAnchorRequestRequestTypeDef,
     TrustAnchorDetailTypeDef,
+    CreateTrustAnchorRequestRequestTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
     ListTrustAnchorsResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
```

### Comparing `mypy-boto3-rolesanywhere-1.28.0/README.md` & `mypy-boto3-rolesanywhere-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-rolesanywhere"></a>
 
 # mypy-boto3-rolesanywhere
 
 [![PyPI - mypy-boto3-rolesanywhere](https://img.shields.io/pypi/v/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rolesanywhere?color=blue)](https://pypistats.org/packages/mypy-boto3-rolesanywhere)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [mypy-boto3-rolesanywhere docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,51 +306,54 @@
 
 ```python
 from mypy_boto3_rolesanywhere.type_defs import (
     TagTypeDef,
     NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
+    ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
-    ListRequestListCrlsPaginateTypeDef,
-    ListRequestListProfilesPaginateTypeDef,
-    ListRequestListSubjectsPaginateTypeDef,
-    ListRequestListTrustAnchorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     NotificationSettingDetailTypeDef,
     NotificationSettingKeyTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
+    SourceDataOutputTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
+    ListRequestListCrlsPaginateTypeDef,
+    ListRequestListProfilesPaginateTypeDef,
+    ListRequestListSubjectsPaginateTypeDef,
+    ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ResetNotificationSettingsRequestRequestTypeDef,
+    SourceOutputTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
-    CreateTrustAnchorRequestRequestTypeDef,
     TrustAnchorDetailTypeDef,
+    CreateTrustAnchorRequestRequestTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
     ListTrustAnchorsResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
```

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/__init__.py` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/__init__.pyi` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/__main__.py` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IAMRolesAnywhere 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.IAMRolesAnywhere 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere\nOther"
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

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/client.py` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/client.pyi` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/literals.py` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,15 @@
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
@@ -244,26 +245,28 @@
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

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/literals.pyi` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/literals.pyi`

 * *Files 1% similar despite different names*

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

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/paginator.py` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,58 +58,58 @@
 class ListCrlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listcrlspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCrlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listcrlspaginator)
         """
 
 
 class ListProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listprofilespaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listprofilespaginator)
         """
 
 
 class ListSubjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listsubjectspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listsubjectspaginator)
         """
 
 
 class ListTrustAnchorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listtrustanchorspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTrustAnchorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listtrustanchorspaginator)
         """
```

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/paginator.pyi` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,55 +55,55 @@
 class ListCrlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listcrlspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCrlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listcrlspaginator)
         """
 
 class ListProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listprofilespaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listprofilespaginator)
         """
 
 class ListSubjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listsubjectspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listsubjectspaginator)
         """
 
 class ListTrustAnchorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listtrustanchorspaginator)
     """
 
     def paginate(
-        self, *, pageSize: int = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pageSize: int = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTrustAnchorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/paginators/#listtrustanchorspaginator)
         """
```

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/type_defs.py` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,57 +24,59 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
+    "ResponseMetadataTypeDef",
     "InstancePropertyTypeDef",
     "ProfileDetailTypeDef",
-    "ListRequestListCrlsPaginateTypeDef",
-    "ListRequestListProfilesPaginateTypeDef",
-    "ListRequestListSubjectsPaginateTypeDef",
-    "ListRequestListTrustAnchorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRequestRequestTypeDef",
     "SubjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "NotificationSettingDetailTypeDef",
     "NotificationSettingKeyTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
+    "SourceDataOutputTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCrlRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
     "SubjectDetailTypeDef",
     "ListProfilesResponseTypeDef",
     "ProfileDetailResponseTypeDef",
+    "ListRequestListCrlsPaginateTypeDef",
+    "ListRequestListProfilesPaginateTypeDef",
+    "ListRequestListSubjectsPaginateTypeDef",
+    "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListSubjectsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ResetNotificationSettingsRequestRequestTypeDef",
+    "SourceOutputTypeDef",
     "SourceTypeDef",
     "SubjectDetailResponseTypeDef",
-    "CreateTrustAnchorRequestRequestTypeDef",
     "TrustAnchorDetailTypeDef",
+    "CreateTrustAnchorRequestRequestTypeDef",
     "UpdateTrustAnchorRequestRequestTypeDef",
     "ListTrustAnchorsResponseTypeDef",
     "PutNotificationSettingsResponseTypeDef",
     "ResetNotificationSettingsResponseTypeDef",
     "TrustAnchorDetailResponseTypeDef",
 )
 
@@ -98,21 +100,19 @@
     {
         "channel": Literal["ALL"],
         "threshold": int,
     },
     total=False,
 )
 
-
 class NotificationSettingTypeDef(
     _RequiredNotificationSettingTypeDef, _OptionalNotificationSettingTypeDef
 ):
     pass
 
-
 CredentialSummaryTypeDef = TypedDict(
     "CredentialSummaryTypeDef",
     {
         "enabled": bool,
         "failed": bool,
         "issuer": str,
         "seenAt": datetime,
@@ -133,14 +133,25 @@
         "name": str,
         "trustAnchorArn": str,
         "updatedAt": datetime,
     },
     total=False,
 )
 
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
 InstancePropertyTypeDef = TypedDict(
     "InstancePropertyTypeDef",
     {
         "failed": bool,
         "properties": Dict[str, str],
         "seenAt": datetime,
     },
@@ -162,46 +173,20 @@
         "roleArns": List[str],
         "sessionPolicy": str,
         "updatedAt": datetime,
     },
     total=False,
 )
 
-ListRequestListCrlsPaginateTypeDef = TypedDict(
-    "ListRequestListCrlsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRequestListProfilesPaginateTypeDef = TypedDict(
-    "ListRequestListProfilesPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRequestListSubjectsPaginateTypeDef = TypedDict(
-    "ListRequestListSubjectsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRequestListTrustAnchorsPaginateTypeDef = TypedDict(
-    "ListRequestListTrustAnchorsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListRequestRequestTypeDef = TypedDict(
     "ListRequestRequestTypeDef",
     {
@@ -228,14 +213,22 @@
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
 _RequiredNotificationSettingDetailTypeDef = TypedDict(
     "_RequiredNotificationSettingDetailTypeDef",
     {
         "enabled": bool,
         "event": NotificationEventType,
     },
 )
@@ -245,63 +238,38 @@
         "channel": Literal["ALL"],
         "configuredBy": str,
         "threshold": int,
     },
     total=False,
 )
 
-
 class NotificationSettingDetailTypeDef(
     _RequiredNotificationSettingDetailTypeDef, _OptionalNotificationSettingDetailTypeDef
 ):
     pass
 
-
 _RequiredNotificationSettingKeyTypeDef = TypedDict(
     "_RequiredNotificationSettingKeyTypeDef",
     {
         "event": NotificationEventType,
     },
 )
 _OptionalNotificationSettingKeyTypeDef = TypedDict(
     "_OptionalNotificationSettingKeyTypeDef",
     {
         "channel": Literal["ALL"],
     },
     total=False,
 )
 
-
 class NotificationSettingKeyTypeDef(
     _RequiredNotificationSettingKeyTypeDef, _OptionalNotificationSettingKeyTypeDef
 ):
     pass
 
-
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
 ScalarCrlRequestRequestTypeDef = TypedDict(
     "ScalarCrlRequestRequestTypeDef",
     {
         "crlId": str,
     },
 )
 
@@ -322,14 +290,23 @@
 ScalarTrustAnchorRequestRequestTypeDef = TypedDict(
     "ScalarTrustAnchorRequestRequestTypeDef",
     {
         "trustAnchorId": str,
     },
 )
 
+SourceDataOutputTypeDef = TypedDict(
+    "SourceDataOutputTypeDef",
+    {
+        "acmPcaArn": str,
+        "x509CertificateData": str,
+    },
+    total=False,
+)
+
 SourceDataTypeDef = TypedDict(
     "SourceDataTypeDef",
     {
         "acmPcaArn": str,
         "x509CertificateData": str,
     },
     total=False,
@@ -354,21 +331,19 @@
     {
         "crlData": Union[str, bytes, IO[Any], StreamingBody],
         "name": str,
     },
     total=False,
 )
 
-
 class UpdateCrlRequestRequestTypeDef(
     _RequiredUpdateCrlRequestRequestTypeDef, _OptionalUpdateCrlRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileRequestRequestTypeDef",
     {
         "profileId": str,
     },
 )
 _OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
@@ -379,21 +354,19 @@
         "name": str,
         "roleArns": Sequence[str],
         "sessionPolicy": str,
     },
     total=False,
 )
 
-
 class UpdateProfileRequestRequestTypeDef(
     _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfileRequestRequestTypeDef",
     {
         "name": str,
         "roleArns": Sequence[str],
     },
 )
@@ -406,21 +379,19 @@
         "requireInstanceProperties": bool,
         "sessionPolicy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateProfileRequestRequestTypeDef(
     _RequiredCreateProfileRequestRequestTypeDef, _OptionalCreateProfileRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredImportCrlRequestRequestTypeDef = TypedDict(
     "_RequiredImportCrlRequestRequestTypeDef",
     {
         "crlData": Union[str, bytes, IO[Any], StreamingBody],
         "name": str,
         "trustAnchorArn": str,
     },
@@ -430,29 +401,19 @@
     {
         "enabled": bool,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ImportCrlRequestRequestTypeDef(
     _RequiredImportCrlRequestRequestTypeDef, _OptionalImportCrlRequestRequestTypeDef
 ):
     pass
 
-
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
@@ -465,24 +426,24 @@
     },
 )
 
 CrlDetailResponseTypeDef = TypedDict(
     "CrlDetailResponseTypeDef",
     {
         "crl": CrlDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCrlsResponseTypeDef = TypedDict(
     "ListCrlsResponseTypeDef",
     {
         "crls": List[CrlDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubjectDetailTypeDef = TypedDict(
     "SubjectDetailTypeDef",
     {
         "createdAt": datetime,
@@ -499,60 +460,128 @@
 )
 
 ListProfilesResponseTypeDef = TypedDict(
     "ListProfilesResponseTypeDef",
     {
         "nextToken": str,
         "profiles": List[ProfileDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProfileDetailResponseTypeDef = TypedDict(
     "ProfileDetailResponseTypeDef",
     {
         "profile": ProfileDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRequestListCrlsPaginateTypeDef = TypedDict(
+    "ListRequestListCrlsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRequestListProfilesPaginateTypeDef = TypedDict(
+    "ListRequestListProfilesPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRequestListSubjectsPaginateTypeDef = TypedDict(
+    "ListRequestListSubjectsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListRequestListTrustAnchorsPaginateTypeDef = TypedDict(
+    "ListRequestListTrustAnchorsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListSubjectsResponseTypeDef = TypedDict(
     "ListSubjectsResponseTypeDef",
     {
         "nextToken": str,
         "subjects": List[SubjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetNotificationSettingsRequestRequestTypeDef = TypedDict(
     "ResetNotificationSettingsRequestRequestTypeDef",
     {
         "notificationSettingKeys": Sequence[NotificationSettingKeyTypeDef],
         "trustAnchorId": str,
     },
 )
 
+SourceOutputTypeDef = TypedDict(
+    "SourceOutputTypeDef",
+    {
+        "sourceData": SourceDataOutputTypeDef,
+        "sourceType": TrustAnchorTypeType,
+    },
+    total=False,
+)
+
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "sourceData": SourceDataTypeDef,
         "sourceType": TrustAnchorTypeType,
     },
     total=False,
 )
 
 SubjectDetailResponseTypeDef = TypedDict(
     "SubjectDetailResponseTypeDef",
     {
         "subject": SubjectDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TrustAnchorDetailTypeDef = TypedDict(
+    "TrustAnchorDetailTypeDef",
+    {
+        "createdAt": datetime,
+        "enabled": bool,
+        "name": str,
+        "notificationSettings": List[NotificationSettingDetailTypeDef],
+        "source": SourceOutputTypeDef,
+        "trustAnchorArn": str,
+        "trustAnchorId": str,
+        "updatedAt": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustAnchorRequestRequestTypeDef",
     {
         "name": str,
         "source": SourceTypeDef,
     },
 )
@@ -562,36 +591,19 @@
         "enabled": bool,
         "notificationSettings": Sequence[NotificationSettingTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateTrustAnchorRequestRequestTypeDef(
     _RequiredCreateTrustAnchorRequestRequestTypeDef, _OptionalCreateTrustAnchorRequestRequestTypeDef
 ):
     pass
 
-
-TrustAnchorDetailTypeDef = TypedDict(
-    "TrustAnchorDetailTypeDef",
-    {
-        "createdAt": datetime,
-        "enabled": bool,
-        "name": str,
-        "notificationSettings": List[NotificationSettingDetailTypeDef],
-        "source": SourceTypeDef,
-        "trustAnchorArn": str,
-        "trustAnchorId": str,
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrustAnchorRequestRequestTypeDef",
     {
         "trustAnchorId": str,
     },
 )
 _OptionalUpdateTrustAnchorRequestRequestTypeDef = TypedDict(
@@ -599,46 +611,44 @@
     {
         "name": str,
         "source": SourceTypeDef,
     },
     total=False,
 )
 
-
 class UpdateTrustAnchorRequestRequestTypeDef(
     _RequiredUpdateTrustAnchorRequestRequestTypeDef, _OptionalUpdateTrustAnchorRequestRequestTypeDef
 ):
     pass
 
-
 ListTrustAnchorsResponseTypeDef = TypedDict(
     "ListTrustAnchorsResponseTypeDef",
     {
         "nextToken": str,
         "trustAnchors": List[TrustAnchorDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutNotificationSettingsResponseTypeDef = TypedDict(
     "PutNotificationSettingsResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetNotificationSettingsResponseTypeDef = TypedDict(
     "ResetNotificationSettingsResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrustAnchorDetailResponseTypeDef = TypedDict(
     "TrustAnchorDetailResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere/type_defs.pyi` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,56 +24,60 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
     "NotificationSettingTypeDef",
     "CredentialSummaryTypeDef",
     "CrlDetailTypeDef",
+    "ResponseMetadataTypeDef",
     "InstancePropertyTypeDef",
     "ProfileDetailTypeDef",
-    "ListRequestListCrlsPaginateTypeDef",
-    "ListRequestListProfilesPaginateTypeDef",
-    "ListRequestListSubjectsPaginateTypeDef",
-    "ListRequestListTrustAnchorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRequestRequestTypeDef",
     "SubjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "NotificationSettingDetailTypeDef",
     "NotificationSettingKeyTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
+    "SourceDataOutputTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCrlRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
     "SubjectDetailTypeDef",
     "ListProfilesResponseTypeDef",
     "ProfileDetailResponseTypeDef",
+    "ListRequestListCrlsPaginateTypeDef",
+    "ListRequestListProfilesPaginateTypeDef",
+    "ListRequestListSubjectsPaginateTypeDef",
+    "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListSubjectsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ResetNotificationSettingsRequestRequestTypeDef",
+    "SourceOutputTypeDef",
     "SourceTypeDef",
     "SubjectDetailResponseTypeDef",
-    "CreateTrustAnchorRequestRequestTypeDef",
     "TrustAnchorDetailTypeDef",
+    "CreateTrustAnchorRequestRequestTypeDef",
     "UpdateTrustAnchorRequestRequestTypeDef",
     "ListTrustAnchorsResponseTypeDef",
     "PutNotificationSettingsResponseTypeDef",
     "ResetNotificationSettingsResponseTypeDef",
     "TrustAnchorDetailResponseTypeDef",
 )
 
@@ -97,19 +101,21 @@
     {
         "channel": Literal["ALL"],
         "threshold": int,
     },
     total=False,
 )
 
+
 class NotificationSettingTypeDef(
     _RequiredNotificationSettingTypeDef, _OptionalNotificationSettingTypeDef
 ):
     pass
 
+
 CredentialSummaryTypeDef = TypedDict(
     "CredentialSummaryTypeDef",
     {
         "enabled": bool,
         "failed": bool,
         "issuer": str,
         "seenAt": datetime,
@@ -130,14 +136,25 @@
         "name": str,
         "trustAnchorArn": str,
         "updatedAt": datetime,
     },
     total=False,
 )
 
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
 InstancePropertyTypeDef = TypedDict(
     "InstancePropertyTypeDef",
     {
         "failed": bool,
         "properties": Dict[str, str],
         "seenAt": datetime,
     },
@@ -159,46 +176,20 @@
         "roleArns": List[str],
         "sessionPolicy": str,
         "updatedAt": datetime,
     },
     total=False,
 )
 
-ListRequestListCrlsPaginateTypeDef = TypedDict(
-    "ListRequestListCrlsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRequestListProfilesPaginateTypeDef = TypedDict(
-    "ListRequestListProfilesPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRequestListSubjectsPaginateTypeDef = TypedDict(
-    "ListRequestListSubjectsPaginateTypeDef",
-    {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListRequestListTrustAnchorsPaginateTypeDef = TypedDict(
-    "ListRequestListTrustAnchorsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "pageSize": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListRequestRequestTypeDef = TypedDict(
     "ListRequestRequestTypeDef",
     {
@@ -225,14 +216,22 @@
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
 _RequiredNotificationSettingDetailTypeDef = TypedDict(
     "_RequiredNotificationSettingDetailTypeDef",
     {
         "enabled": bool,
         "event": NotificationEventType,
     },
 )
@@ -242,58 +241,41 @@
         "channel": Literal["ALL"],
         "configuredBy": str,
         "threshold": int,
     },
     total=False,
 )
 
+
 class NotificationSettingDetailTypeDef(
     _RequiredNotificationSettingDetailTypeDef, _OptionalNotificationSettingDetailTypeDef
 ):
     pass
 
+
 _RequiredNotificationSettingKeyTypeDef = TypedDict(
     "_RequiredNotificationSettingKeyTypeDef",
     {
         "event": NotificationEventType,
     },
 )
 _OptionalNotificationSettingKeyTypeDef = TypedDict(
     "_OptionalNotificationSettingKeyTypeDef",
     {
         "channel": Literal["ALL"],
     },
     total=False,
 )
 
+
 class NotificationSettingKeyTypeDef(
     _RequiredNotificationSettingKeyTypeDef, _OptionalNotificationSettingKeyTypeDef
 ):
     pass
 
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
 
 ScalarCrlRequestRequestTypeDef = TypedDict(
     "ScalarCrlRequestRequestTypeDef",
     {
         "crlId": str,
     },
 )
@@ -315,14 +297,23 @@
 ScalarTrustAnchorRequestRequestTypeDef = TypedDict(
     "ScalarTrustAnchorRequestRequestTypeDef",
     {
         "trustAnchorId": str,
     },
 )
 
+SourceDataOutputTypeDef = TypedDict(
+    "SourceDataOutputTypeDef",
+    {
+        "acmPcaArn": str,
+        "x509CertificateData": str,
+    },
+    total=False,
+)
+
 SourceDataTypeDef = TypedDict(
     "SourceDataTypeDef",
     {
         "acmPcaArn": str,
         "x509CertificateData": str,
     },
     total=False,
@@ -347,19 +338,21 @@
     {
         "crlData": Union[str, bytes, IO[Any], StreamingBody],
         "name": str,
     },
     total=False,
 )
 
+
 class UpdateCrlRequestRequestTypeDef(
     _RequiredUpdateCrlRequestRequestTypeDef, _OptionalUpdateCrlRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProfileRequestRequestTypeDef",
     {
         "profileId": str,
     },
 )
 _OptionalUpdateProfileRequestRequestTypeDef = TypedDict(
@@ -370,19 +363,21 @@
         "name": str,
         "roleArns": Sequence[str],
         "sessionPolicy": str,
     },
     total=False,
 )
 
+
 class UpdateProfileRequestRequestTypeDef(
     _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfileRequestRequestTypeDef",
     {
         "name": str,
         "roleArns": Sequence[str],
     },
 )
@@ -395,19 +390,21 @@
         "requireInstanceProperties": bool,
         "sessionPolicy": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateProfileRequestRequestTypeDef(
     _RequiredCreateProfileRequestRequestTypeDef, _OptionalCreateProfileRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredImportCrlRequestRequestTypeDef = TypedDict(
     "_RequiredImportCrlRequestRequestTypeDef",
     {
         "crlData": Union[str, bytes, IO[Any], StreamingBody],
         "name": str,
         "trustAnchorArn": str,
     },
@@ -417,26 +414,20 @@
     {
         "enabled": bool,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ImportCrlRequestRequestTypeDef(
     _RequiredImportCrlRequestRequestTypeDef, _OptionalImportCrlRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
@@ -450,24 +441,24 @@
     },
 )
 
 CrlDetailResponseTypeDef = TypedDict(
     "CrlDetailResponseTypeDef",
     {
         "crl": CrlDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCrlsResponseTypeDef = TypedDict(
     "ListCrlsResponseTypeDef",
     {
         "crls": List[CrlDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubjectDetailTypeDef = TypedDict(
     "SubjectDetailTypeDef",
     {
         "createdAt": datetime,
@@ -484,58 +475,126 @@
 )
 
 ListProfilesResponseTypeDef = TypedDict(
     "ListProfilesResponseTypeDef",
     {
         "nextToken": str,
         "profiles": List[ProfileDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProfileDetailResponseTypeDef = TypedDict(
     "ProfileDetailResponseTypeDef",
     {
         "profile": ProfileDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRequestListCrlsPaginateTypeDef = TypedDict(
+    "ListRequestListCrlsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRequestListProfilesPaginateTypeDef = TypedDict(
+    "ListRequestListProfilesPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRequestListSubjectsPaginateTypeDef = TypedDict(
+    "ListRequestListSubjectsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRequestListTrustAnchorsPaginateTypeDef = TypedDict(
+    "ListRequestListTrustAnchorsPaginateTypeDef",
+    {
+        "pageSize": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListSubjectsResponseTypeDef = TypedDict(
     "ListSubjectsResponseTypeDef",
     {
         "nextToken": str,
         "subjects": List[SubjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetNotificationSettingsRequestRequestTypeDef = TypedDict(
     "ResetNotificationSettingsRequestRequestTypeDef",
     {
         "notificationSettingKeys": Sequence[NotificationSettingKeyTypeDef],
         "trustAnchorId": str,
     },
 )
 
+SourceOutputTypeDef = TypedDict(
+    "SourceOutputTypeDef",
+    {
+        "sourceData": SourceDataOutputTypeDef,
+        "sourceType": TrustAnchorTypeType,
+    },
+    total=False,
+)
+
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "sourceData": SourceDataTypeDef,
         "sourceType": TrustAnchorTypeType,
     },
     total=False,
 )
 
 SubjectDetailResponseTypeDef = TypedDict(
     "SubjectDetailResponseTypeDef",
     {
         "subject": SubjectDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TrustAnchorDetailTypeDef = TypedDict(
+    "TrustAnchorDetailTypeDef",
+    {
+        "createdAt": datetime,
+        "enabled": bool,
+        "name": str,
+        "notificationSettings": List[NotificationSettingDetailTypeDef],
+        "source": SourceOutputTypeDef,
+        "trustAnchorArn": str,
+        "trustAnchorId": str,
+        "updatedAt": datetime,
     },
+    total=False,
 )
 
 _RequiredCreateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustAnchorRequestRequestTypeDef",
     {
         "name": str,
         "source": SourceTypeDef,
@@ -547,33 +606,20 @@
         "enabled": bool,
         "notificationSettings": Sequence[NotificationSettingTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateTrustAnchorRequestRequestTypeDef(
     _RequiredCreateTrustAnchorRequestRequestTypeDef, _OptionalCreateTrustAnchorRequestRequestTypeDef
 ):
     pass
 
-TrustAnchorDetailTypeDef = TypedDict(
-    "TrustAnchorDetailTypeDef",
-    {
-        "createdAt": datetime,
-        "enabled": bool,
-        "name": str,
-        "notificationSettings": List[NotificationSettingDetailTypeDef],
-        "source": SourceTypeDef,
-        "trustAnchorArn": str,
-        "trustAnchorId": str,
-        "updatedAt": datetime,
-    },
-    total=False,
-)
 
 _RequiredUpdateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrustAnchorRequestRequestTypeDef",
     {
         "trustAnchorId": str,
     },
 )
@@ -582,44 +628,46 @@
     {
         "name": str,
         "source": SourceTypeDef,
     },
     total=False,
 )
 
+
 class UpdateTrustAnchorRequestRequestTypeDef(
     _RequiredUpdateTrustAnchorRequestRequestTypeDef, _OptionalUpdateTrustAnchorRequestRequestTypeDef
 ):
     pass
 
+
 ListTrustAnchorsResponseTypeDef = TypedDict(
     "ListTrustAnchorsResponseTypeDef",
     {
         "nextToken": str,
         "trustAnchors": List[TrustAnchorDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutNotificationSettingsResponseTypeDef = TypedDict(
     "PutNotificationSettingsResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetNotificationSettingsResponseTypeDef = TypedDict(
     "ResetNotificationSettingsResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrustAnchorDetailResponseTypeDef = TypedDict(
     "TrustAnchorDetailResponseTypeDef",
     {
         "trustAnchor": TrustAnchorDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere.egg-info/PKG-INFO` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.28.0
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-rolesanywhere"></a>
 
 # mypy-boto3-rolesanywhere
 
 [![PyPI - mypy-boto3-rolesanywhere](https://img.shields.io/pypi/v/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-rolesanywhere?color=blue)](https://pypistats.org/packages/mypy-boto3-rolesanywhere)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [mypy-boto3-rolesanywhere docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,51 +338,54 @@
 
 ```python
 from mypy_boto3_rolesanywhere.type_defs import (
     TagTypeDef,
     NotificationSettingTypeDef,
     CredentialSummaryTypeDef,
     CrlDetailTypeDef,
+    ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
-    ListRequestListCrlsPaginateTypeDef,
-    ListRequestListProfilesPaginateTypeDef,
-    ListRequestListSubjectsPaginateTypeDef,
-    ListRequestListTrustAnchorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     NotificationSettingDetailTypeDef,
     NotificationSettingKeyTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
+    SourceDataOutputTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
+    ListRequestListCrlsPaginateTypeDef,
+    ListRequestListProfilesPaginateTypeDef,
+    ListRequestListSubjectsPaginateTypeDef,
+    ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ResetNotificationSettingsRequestRequestTypeDef,
+    SourceOutputTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
-    CreateTrustAnchorRequestRequestTypeDef,
     TrustAnchorDetailTypeDef,
+    CreateTrustAnchorRequestRequestTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
     ListTrustAnchorsResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
```

### Comparing `mypy-boto3-rolesanywhere-1.28.0/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt` & `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.0/setup.py` & `mypy-boto3-rolesanywhere-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rolesanywhere",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_rolesanywhere"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IAMRolesAnywhere 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.IAMRolesAnywhere 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

