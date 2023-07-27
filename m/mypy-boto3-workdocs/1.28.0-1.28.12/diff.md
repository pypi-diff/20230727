# Comparing `tmp/mypy-boto3-workdocs-1.28.0.tar.gz` & `tmp/mypy-boto3-workdocs-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workdocs-1.28.0.tar", last modified: Thu Jul  6 21:00:52 2023, max compression
+gzip compressed data, was "mypy-boto3-workdocs-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
```

## Comparing `mypy-boto3-workdocs-1.28.0.tar` & `mypy-boto3-workdocs-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.222461 mypy-boto3-workdocs-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:58:09.000000 mypy-boto3-workdocs-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-06 21:00:52.222461 mypy-boto3-workdocs-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-07-06 20:58:09.000000 mypy-boto3-workdocs-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.214461 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-06 20:58:09.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-06 20:58:09.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:58:09.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38652 2023-07-06 20:58:09.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38591 2023-07-06 20:58:09.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-07-06 20:58:10.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13800 2023-07-06 20:58:09.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-07-06 20:58:09.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-07-06 20:58:09.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:09.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50612 2023-07-06 20:58:11.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50521 2023-07-06 20:58:10.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:58:09.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:52.222461 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-06 21:00:51.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 21:00:52.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:51.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:51.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:51.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:51.000000 mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:52.222461 mypy-boto3-workdocs-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:58:08.000000 mypy-boto3-workdocs-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.849495 mypy-boto3-workdocs-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-07-27 11:49:49.849495 mypy-boto3-workdocs-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.849495 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38652 2023-07-27 11:48:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38591 2023-07-27 11:48:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-07-27 11:48:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-07-27 11:48:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13859 2023-07-27 11:48:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-07-27 11:48:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50773 2023-07-27 11:48:50.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50682 2023-07-27 11:48:50.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.849495 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-07-27 11:49:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 11:49:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.849495 mypy-boto3-workdocs-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/setup.py
```

### Comparing `mypy-boto3-workdocs-1.28.0/LICENSE` & `mypy-boto3-workdocs-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.0/PKG-INFO` & `mypy-boto3-workdocs-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workdocs
-Version: 1.28.0
-Summary: Type annotations for boto3.WorkDocs 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WorkDocs 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workdocs"></a>
 
 # mypy-boto3-workdocs
 
 [![PyPI - mypy-boto3-workdocs](https://img.shields.io/pypi/v/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workdocs?color=blue)](https://pypistats.org/packages/mypy-boto3-workdocs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workdocs)](https://pepy.tech/project/mypy-boto3-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkDocs 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[boto3.WorkDocs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [mypy-boto3-workdocs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -397,14 +397,15 @@
 `mypy_boto3_workdocs.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workdocs.type_defs import (
     AbortDocumentVersionUploadRequestRequestTypeDef,
     ActivateUserRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UserMetadataTypeDef,
     NotificationOptionsTypeDef,
     SharePrincipalTypeDef,
     ShareResultTypeDef,
     CreateCommentRequestRequestTypeDef,
     CreateCustomMetadataRequestRequestTypeDef,
     CreateFolderRequestRequestTypeDef,
@@ -420,86 +421,86 @@
     DeleteDocumentRequestRequestTypeDef,
     DeleteDocumentVersionRequestRequestTypeDef,
     DeleteFolderContentsRequestRequestTypeDef,
     DeleteFolderRequestRequestTypeDef,
     DeleteLabelsRequestRequestTypeDef,
     DeleteNotificationSubscriptionRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeActivitiesRequestRequestTypeDef,
-    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
     DescribeCommentsRequestRequestTypeDef,
-    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeDocumentVersionsRequestRequestTypeDef,
     DocumentVersionMetadataTypeDef,
-    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeFolderContentsRequestRequestTypeDef,
-    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeGroupsRequestRequestTypeDef,
     GroupMetadataTypeDef,
-    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestRequestTypeDef,
-    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
     DescribeResourcePermissionsRequestRequestTypeDef,
-    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
     DescribeRootFoldersRequestRequestTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     LongRangeTypeTypeDef,
     SearchPrincipalTypeTypeDef,
     GetCurrentUserRequestRequestTypeDef,
     GetDocumentPathRequestRequestTypeDef,
     GetDocumentRequestRequestTypeDef,
     GetDocumentVersionRequestRequestTypeDef,
     GetFolderPathRequestRequestTypeDef,
     GetFolderRequestRequestTypeDef,
     GetResourcesRequestRequestTypeDef,
     InitiateDocumentVersionUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
-    PaginatorConfigTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
-    ResponseMetadataTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
+    StorageRuleTypeOutputTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     UpdateDocumentVersionRequestRequestTypeDef,
     UpdateFolderRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ResourceMetadataTypeDef,
     AddResourcePermissionsRequestRequestTypeDef,
     AddResourcePermissionsResponseTypeDef,
     CreateFolderResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
-    UserStorageMetadataTypeDef,
+    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
+    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeDocumentVersionsResponseTypeDef,
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
     FiltersTypeDef,
     PrincipalTypeDef,
     ResourcePathTypeDef,
-    UserTypeDef,
+    UserStorageMetadataTypeDef,
     DescribeFolderContentsResponseTypeDef,
     GetDocumentResponseTypeDef,
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
     SearchResourcesRequestRequestTypeDef,
     SearchResourcesRequestSearchResourcesPaginateTypeDef,
     DescribeResourcePermissionsResponseTypeDef,
     GetDocumentPathResponseTypeDef,
     GetFolderPathResponseTypeDef,
+    UserTypeDef,
     ActivateUserResponseTypeDef,
     CommentMetadataTypeDef,
     CommentTypeDef,
     CreateUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     GetCurrentUserResponseTypeDef,
     UpdateUserResponseTypeDef,
```

### Comparing `mypy-boto3-workdocs-1.28.0/README.md` & `mypy-boto3-workdocs-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-workdocs"></a>
 
 # mypy-boto3-workdocs
 
 [![PyPI - mypy-boto3-workdocs](https://img.shields.io/pypi/v/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workdocs?color=blue)](https://pypistats.org/packages/mypy-boto3-workdocs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workdocs)](https://pepy.tech/project/mypy-boto3-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkDocs 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[boto3.WorkDocs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [mypy-boto3-workdocs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,14 +365,15 @@
 `mypy_boto3_workdocs.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workdocs.type_defs import (
     AbortDocumentVersionUploadRequestRequestTypeDef,
     ActivateUserRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UserMetadataTypeDef,
     NotificationOptionsTypeDef,
     SharePrincipalTypeDef,
     ShareResultTypeDef,
     CreateCommentRequestRequestTypeDef,
     CreateCustomMetadataRequestRequestTypeDef,
     CreateFolderRequestRequestTypeDef,
@@ -388,86 +389,86 @@
     DeleteDocumentRequestRequestTypeDef,
     DeleteDocumentVersionRequestRequestTypeDef,
     DeleteFolderContentsRequestRequestTypeDef,
     DeleteFolderRequestRequestTypeDef,
     DeleteLabelsRequestRequestTypeDef,
     DeleteNotificationSubscriptionRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeActivitiesRequestRequestTypeDef,
-    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
     DescribeCommentsRequestRequestTypeDef,
-    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeDocumentVersionsRequestRequestTypeDef,
     DocumentVersionMetadataTypeDef,
-    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeFolderContentsRequestRequestTypeDef,
-    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeGroupsRequestRequestTypeDef,
     GroupMetadataTypeDef,
-    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestRequestTypeDef,
-    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
     DescribeResourcePermissionsRequestRequestTypeDef,
-    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
     DescribeRootFoldersRequestRequestTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     LongRangeTypeTypeDef,
     SearchPrincipalTypeTypeDef,
     GetCurrentUserRequestRequestTypeDef,
     GetDocumentPathRequestRequestTypeDef,
     GetDocumentRequestRequestTypeDef,
     GetDocumentVersionRequestRequestTypeDef,
     GetFolderPathRequestRequestTypeDef,
     GetFolderRequestRequestTypeDef,
     GetResourcesRequestRequestTypeDef,
     InitiateDocumentVersionUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
-    PaginatorConfigTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
-    ResponseMetadataTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
+    StorageRuleTypeOutputTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     UpdateDocumentVersionRequestRequestTypeDef,
     UpdateFolderRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ResourceMetadataTypeDef,
     AddResourcePermissionsRequestRequestTypeDef,
     AddResourcePermissionsResponseTypeDef,
     CreateFolderResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
-    UserStorageMetadataTypeDef,
+    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
+    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeDocumentVersionsResponseTypeDef,
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
     FiltersTypeDef,
     PrincipalTypeDef,
     ResourcePathTypeDef,
-    UserTypeDef,
+    UserStorageMetadataTypeDef,
     DescribeFolderContentsResponseTypeDef,
     GetDocumentResponseTypeDef,
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
     SearchResourcesRequestRequestTypeDef,
     SearchResourcesRequestSearchResourcesPaginateTypeDef,
     DescribeResourcePermissionsResponseTypeDef,
     GetDocumentPathResponseTypeDef,
     GetFolderPathResponseTypeDef,
+    UserTypeDef,
     ActivateUserResponseTypeDef,
     CommentMetadataTypeDef,
     CommentTypeDef,
     CreateUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     GetCurrentUserResponseTypeDef,
     UpdateUserResponseTypeDef,
```

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/__init__.py` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/__init__.pyi` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/__main__.py` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkDocs 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.WorkDocs 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs\nOther"
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

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/client.py` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/client.pyi` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/literals.py` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,15 @@
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
@@ -402,26 +403,28 @@
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

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/literals.pyi` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,15 @@
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
@@ -400,26 +401,28 @@
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

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/paginator.py` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeactivitiespaginator)
         """
 
 
@@ -130,15 +130,15 @@
 
     def paginate(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeCommentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeComments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describecommentspaginator)
         """
 
 
@@ -151,15 +151,15 @@
     def paginate(
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Include: str = ...,
         Fields: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDocumentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeDocumentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describedocumentversionspaginator)
         """
 
 
@@ -174,15 +174,15 @@
         *,
         FolderId: str,
         AuthenticationToken: str = ...,
         Sort: ResourceSortTypeType = ...,
         Order: OrderTypeType = ...,
         Type: FolderContentTypeType = ...,
         Include: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeFolderContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeFolderContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describefoldercontentspaginator)
         """
 
 
@@ -194,30 +194,30 @@
 
     def paginate(
         self,
         *,
         SearchQuery: str,
         AuthenticationToken: str = ...,
         OrganizationId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describegroupspaginator)
         """
 
 
 class DescribeNotificationSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describenotificationsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeNotificationSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describenotificationsubscriptionspaginator)
         """
 
 
@@ -229,30 +229,30 @@
 
     def paginate(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         PrincipalId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeResourcePermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeResourcePermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeresourcepermissionspaginator)
         """
 
 
 class DescribeRootFoldersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describerootfolderspaginator)
     """
 
     def paginate(
-        self, *, AuthenticationToken: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AuthenticationToken: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRootFoldersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describerootfolderspaginator)
         """
 
 
@@ -269,15 +269,15 @@
         OrganizationId: str = ...,
         UserIds: str = ...,
         Query: str = ...,
         Include: UserFilterTypeType = ...,
         Order: OrderTypeType = ...,
         Sort: UserSortTypeType = ...,
         Fields: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeuserspaginator)
         """
 
 
@@ -293,13 +293,13 @@
         AuthenticationToken: str = ...,
         QueryText: str = ...,
         QueryScopes: Sequence[SearchQueryScopeTypeType] = ...,
         OrganizationId: str = ...,
         AdditionalResponseFields: Sequence[Literal["WEBURL"]] = ...,
         Filters: FiltersTypeDef = ...,
         OrderBy: Sequence[SearchSortResultTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.SearchResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#searchresourcespaginator)
         """
```

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/paginator.pyi` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/paginator.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         OrganizationId: str = ...,
         ActivityTypes: str = ...,
         ResourceId: str = ...,
         UserId: str = ...,
         IncludeIndirectActivities: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeActivities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeactivitiespaginator)
         """
 
 class DescribeCommentsPaginator(Paginator):
@@ -125,15 +125,15 @@
 
     def paginate(
         self,
         *,
         DocumentId: str,
         VersionId: str,
         AuthenticationToken: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeCommentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeComments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describecommentspaginator)
         """
 
 class DescribeDocumentVersionsPaginator(Paginator):
@@ -145,15 +145,15 @@
     def paginate(
         self,
         *,
         DocumentId: str,
         AuthenticationToken: str = ...,
         Include: str = ...,
         Fields: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDocumentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeDocumentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describedocumentversionspaginator)
         """
 
 class DescribeFolderContentsPaginator(Paginator):
@@ -167,15 +167,15 @@
         *,
         FolderId: str,
         AuthenticationToken: str = ...,
         Sort: ResourceSortTypeType = ...,
         Order: OrderTypeType = ...,
         Type: FolderContentTypeType = ...,
         Include: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeFolderContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeFolderContents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describefoldercontentspaginator)
         """
 
 class DescribeGroupsPaginator(Paginator):
@@ -186,29 +186,29 @@
 
     def paginate(
         self,
         *,
         SearchQuery: str,
         AuthenticationToken: str = ...,
         OrganizationId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describegroupspaginator)
         """
 
 class DescribeNotificationSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describenotificationsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, OrganizationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, OrganizationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeNotificationSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeNotificationSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describenotificationsubscriptionspaginator)
         """
 
 class DescribeResourcePermissionsPaginator(Paginator):
@@ -219,29 +219,29 @@
 
     def paginate(
         self,
         *,
         ResourceId: str,
         AuthenticationToken: str = ...,
         PrincipalId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeResourcePermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeResourcePermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeresourcepermissionspaginator)
         """
 
 class DescribeRootFoldersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describerootfolderspaginator)
     """
 
     def paginate(
-        self, *, AuthenticationToken: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AuthenticationToken: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeRootFoldersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeRootFolders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describerootfolderspaginator)
         """
 
 class DescribeUsersPaginator(Paginator):
@@ -257,15 +257,15 @@
         OrganizationId: str = ...,
         UserIds: str = ...,
         Query: str = ...,
         Include: UserFilterTypeType = ...,
         Order: OrderTypeType = ...,
         Sort: UserSortTypeType = ...,
         Fields: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.DescribeUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#describeuserspaginator)
         """
 
 class SearchResourcesPaginator(Paginator):
@@ -280,13 +280,13 @@
         AuthenticationToken: str = ...,
         QueryText: str = ...,
         QueryScopes: Sequence[SearchQueryScopeTypeType] = ...,
         OrganizationId: str = ...,
         AdditionalResponseFields: Sequence[Literal["WEBURL"]] = ...,
         Filters: FiltersTypeDef = ...,
         OrderBy: Sequence[SearchSortResultTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs.Paginator.SearchResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/paginators/#searchresourcespaginator)
         """
```

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/type_defs.py` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AbortDocumentVersionUploadRequestRequestTypeDef",
     "ActivateUserRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UserMetadataTypeDef",
     "NotificationOptionsTypeDef",
     "SharePrincipalTypeDef",
     "ShareResultTypeDef",
     "CreateCommentRequestRequestTypeDef",
     "CreateCustomMetadataRequestRequestTypeDef",
     "CreateFolderRequestRequestTypeDef",
@@ -82,86 +83,86 @@
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteDocumentVersionRequestRequestTypeDef",
     "DeleteFolderContentsRequestRequestTypeDef",
     "DeleteFolderRequestRequestTypeDef",
     "DeleteLabelsRequestRequestTypeDef",
     "DeleteNotificationSubscriptionRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
-    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeActivitiesRequestRequestTypeDef",
-    "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
     "DescribeCommentsRequestRequestTypeDef",
-    "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
     "DescribeDocumentVersionsRequestRequestTypeDef",
     "DocumentVersionMetadataTypeDef",
-    "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
     "DescribeFolderContentsRequestRequestTypeDef",
-    "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
     "DescribeGroupsRequestRequestTypeDef",
     "GroupMetadataTypeDef",
-    "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
     "DescribeNotificationSubscriptionsRequestRequestTypeDef",
-    "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
     "DescribeResourcePermissionsRequestRequestTypeDef",
-    "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
     "DescribeRootFoldersRequestRequestTypeDef",
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "LongRangeTypeTypeDef",
     "SearchPrincipalTypeTypeDef",
     "GetCurrentUserRequestRequestTypeDef",
     "GetDocumentPathRequestRequestTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "GetDocumentVersionRequestRequestTypeDef",
     "GetFolderPathRequestRequestTypeDef",
     "GetFolderRequestRequestTypeDef",
     "GetResourcesRequestRequestTypeDef",
     "InitiateDocumentVersionUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
-    "PaginatorConfigTypeDef",
     "PermissionInfoTypeDef",
     "RemoveAllResourcePermissionsRequestRequestTypeDef",
     "RemoveResourcePermissionRequestRequestTypeDef",
     "ResourcePathComponentTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreDocumentVersionsRequestRequestTypeDef",
     "SearchSortResultTypeDef",
+    "StorageRuleTypeOutputTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
     "UpdateDocumentVersionRequestRequestTypeDef",
     "UpdateFolderRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ResourceMetadataTypeDef",
     "AddResourcePermissionsRequestRequestTypeDef",
     "AddResourcePermissionsResponseTypeDef",
     "CreateFolderResponseTypeDef",
     "DescribeRootFoldersResponseTypeDef",
     "GetFolderResponseTypeDef",
     "CreateNotificationSubscriptionResponseTypeDef",
     "DescribeNotificationSubscriptionsResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
-    "UserStorageMetadataTypeDef",
+    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
+    "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeDocumentVersionsResponseTypeDef",
     "DocumentMetadataTypeDef",
     "GetDocumentVersionResponseTypeDef",
     "DescribeGroupsResponseTypeDef",
     "ParticipantsTypeDef",
     "FiltersTypeDef",
     "PrincipalTypeDef",
     "ResourcePathTypeDef",
-    "UserTypeDef",
+    "UserStorageMetadataTypeDef",
     "DescribeFolderContentsResponseTypeDef",
     "GetDocumentResponseTypeDef",
     "GetResourcesResponseTypeDef",
     "InitiateDocumentVersionUploadResponseTypeDef",
     "SearchResourcesRequestRequestTypeDef",
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "DescribeResourcePermissionsResponseTypeDef",
     "GetDocumentPathResponseTypeDef",
     "GetFolderPathResponseTypeDef",
+    "UserTypeDef",
     "ActivateUserResponseTypeDef",
     "CommentMetadataTypeDef",
     "CommentTypeDef",
     "CreateUserResponseTypeDef",
     "DescribeUsersResponseTypeDef",
     "GetCurrentUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
@@ -213,14 +214,25 @@
 
 class ActivateUserRequestRequestTypeDef(
     _RequiredActivateUserRequestRequestTypeDef, _OptionalActivateUserRequestRequestTypeDef
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
+
 UserMetadataTypeDef = TypedDict(
     "UserMetadataTypeDef",
     {
         "Id": str,
         "Username": str,
         "GivenName": str,
         "Surname": str,
@@ -616,26 +628,20 @@
 
 class DeleteUserRequestRequestTypeDef(
     _RequiredDeleteUserRequestRequestTypeDef, _OptionalDeleteUserRequestRequestTypeDef
 ):
     pass
 
 
-DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
-    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AuthenticationToken": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "OrganizationId": str,
-        "ActivityTypes": str,
-        "ResourceId": str,
-        "UserId": str,
-        "IncludeIndirectActivities": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeActivitiesRequestRequestTypeDef = TypedDict(
     "DescribeActivitiesRequestRequestTypeDef",
     {
@@ -649,38 +655,14 @@
         "IncludeIndirectActivities": bool,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
-    {
-        "DocumentId": str,
-        "VersionId": str,
-    },
-)
-_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeCommentsRequestDescribeCommentsPaginateTypeDef(
-    _RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-    _OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeCommentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommentsRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
     },
 )
@@ -697,39 +679,14 @@
 
 class DescribeCommentsRequestRequestTypeDef(
     _RequiredDescribeCommentsRequestRequestTypeDef, _OptionalDescribeCommentsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    {
-        "DocumentId": str,
-    },
-)
-_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Include": str,
-        "Fields": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef(
-    _RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-    _OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentVersionsRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalDescribeDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -768,41 +725,14 @@
         "CreatorId": str,
         "Thumbnail": Dict[DocumentThumbnailTypeType, str],
         "Source": Dict[DocumentSourceTypeType, str],
     },
     total=False,
 )
 
-_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    {
-        "FolderId": str,
-    },
-)
-_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Sort": ResourceSortTypeType,
-        "Order": OrderTypeType,
-        "Type": FolderContentTypeType,
-        "Include": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef(
-    _RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-    _OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeFolderContentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFolderContentsRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalDescribeFolderContentsRequestRequestTypeDef = TypedDict(
@@ -823,38 +753,14 @@
 class DescribeFolderContentsRequestRequestTypeDef(
     _RequiredDescribeFolderContentsRequestRequestTypeDef,
     _OptionalDescribeFolderContentsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    {
-        "SearchQuery": str,
-    },
-)
-_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "OrganizationId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeGroupsRequestDescribeGroupsPaginateTypeDef(
-    _RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-    _OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeGroupsRequestRequestTypeDef",
     {
         "SearchQuery": str,
     },
 )
 _OptionalDescribeGroupsRequestRequestTypeDef = TypedDict(
@@ -880,36 +786,14 @@
     {
         "Id": str,
         "Name": str,
     },
     total=False,
 )
 
-_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef(
-    _RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-    _OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalDescribeNotificationSubscriptionsRequestRequestTypeDef = TypedDict(
@@ -925,38 +809,14 @@
 class DescribeNotificationSubscriptionsRequestRequestTypeDef(
     _RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef,
     _OptionalDescribeNotificationSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "PrincipalId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef(
-    _RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-    _OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeResourcePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourcePermissionsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalDescribeResourcePermissionsRequestRequestTypeDef = TypedDict(
@@ -974,36 +834,14 @@
 class DescribeResourcePermissionsRequestRequestTypeDef(
     _RequiredDescribeResourcePermissionsRequestRequestTypeDef,
     _OptionalDescribeResourcePermissionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-    },
-)
-_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef(
-    _RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-    _OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeRootFoldersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRootFoldersRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
 )
 _OptionalDescribeRootFoldersRequestRequestTypeDef = TypedDict(
@@ -1019,30 +857,14 @@
 class DescribeRootFoldersRequestRequestTypeDef(
     _RequiredDescribeRootFoldersRequestRequestTypeDef,
     _OptionalDescribeRootFoldersRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "OrganizationId": str,
-        "UserIds": str,
-        "Query": str,
-        "Include": UserFilterTypeType,
-        "Order": OrderTypeType,
-        "Sort": UserSortTypeType,
-        "Fields": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUsersRequestRequestTypeDef = TypedDict(
     "DescribeUsersRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
         "OrganizationId": str,
         "UserIds": str,
         "Query": str,
@@ -1052,21 +874,14 @@
         "Marker": str,
         "Limit": int,
         "Fields": str,
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
 LongRangeTypeTypeDef = TypedDict(
     "LongRangeTypeTypeDef",
     {
         "StartValue": int,
         "EndValue": int,
     },
     total=False,
@@ -1249,24 +1064,14 @@
     {
         "UploadUrl": str,
         "SignedHeaders": Dict[str, str],
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
 PermissionInfoTypeDef = TypedDict(
     "PermissionInfoTypeDef",
     {
         "Role": RoleTypeType,
         "Type": RolePermissionTypeType,
     },
     total=False,
@@ -1323,25 +1128,14 @@
     {
         "Id": str,
         "Name": str,
     },
     total=False,
 )
 
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
 _RequiredRestoreDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreDocumentVersionsRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalRestoreDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -1365,14 +1159,23 @@
     {
         "Field": OrderByFieldTypeType,
         "Order": SortOrderType,
     },
     total=False,
 )
 
+StorageRuleTypeOutputTypeDef = TypedDict(
+    "StorageRuleTypeOutputTypeDef",
+    {
+        "StorageAllocatedInBytes": int,
+        "StorageType": StorageTypeType,
+    },
+    total=False,
+)
+
 _RequiredUpdateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalUpdateDocumentRequestRequestTypeDef = TypedDict(
@@ -1437,14 +1240,21 @@
 
 class UpdateFolderRequestRequestTypeDef(
     _RequiredUpdateFolderRequestRequestTypeDef, _OptionalUpdateFolderRequestRequestTypeDef
 ):
     pass
 
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ResourceMetadataTypeDef = TypedDict(
     "ResourceMetadataTypeDef",
     {
         "Type": ResourceTypeType,
         "Name": str,
         "OriginalName": str,
         "Id": str,
@@ -1479,58 +1289,58 @@
     pass
 
 
 AddResourcePermissionsResponseTypeDef = TypedDict(
     "AddResourcePermissionsResponseTypeDef",
     {
         "ShareResults": List[ShareResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFolderResponseTypeDef = TypedDict(
     "CreateFolderResponseTypeDef",
     {
         "Metadata": FolderMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRootFoldersResponseTypeDef = TypedDict(
     "DescribeRootFoldersResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFolderResponseTypeDef = TypedDict(
     "GetFolderResponseTypeDef",
     {
         "Metadata": FolderMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNotificationSubscriptionResponseTypeDef = TypedDict(
     "CreateNotificationSubscriptionResponseTypeDef",
     {
         "Subscription": SubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotificationSubscriptionsResponseTypeDef = TypedDict(
     "DescribeNotificationSubscriptionsResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "Username": str,
@@ -1582,29 +1392,220 @@
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
 
-UserStorageMetadataTypeDef = TypedDict(
-    "UserStorageMetadataTypeDef",
+DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
+    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     {
-        "StorageUtilizedInBytes": int,
-        "StorageRule": StorageRuleTypeTypeDef,
+        "AuthenticationToken": str,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "OrganizationId": str,
+        "ActivityTypes": str,
+        "ResourceId": str,
+        "UserId": str,
+        "IncludeIndirectActivities": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    {
+        "DocumentId": str,
+        "VersionId": str,
+    },
+)
+_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeCommentsRequestDescribeCommentsPaginateTypeDef(
+    _RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    _OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    {
+        "DocumentId": str,
+    },
+)
+_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Include": str,
+        "Fields": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef(
+    _RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+    _OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    {
+        "FolderId": str,
+    },
+)
+_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Sort": ResourceSortTypeType,
+        "Order": OrderTypeType,
+        "Type": FolderContentTypeType,
+        "Include": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef(
+    _RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+    _OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    {
+        "SearchQuery": str,
+    },
+)
+_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "OrganizationId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeGroupsRequestDescribeGroupsPaginateTypeDef(
+    _RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+    _OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef(
+    _RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+    _OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "PrincipalId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef(
+    _RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+    _OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+    },
+)
+_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef(
+    _RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+    _OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+):
+    pass
+
+
+DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "OrganizationId": str,
+        "UserIds": str,
+        "Query": str,
+        "Include": UserFilterTypeType,
+        "Order": OrderTypeType,
+        "Sort": UserSortTypeType,
+        "Fields": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDocumentVersionsResponseTypeDef = TypedDict(
     "DescribeDocumentVersionsResponseTypeDef",
     {
         "DocumentVersions": List[DocumentVersionMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentMetadataTypeDef = TypedDict(
     "DocumentMetadataTypeDef",
     {
         "Id": str,
@@ -1620,24 +1621,24 @@
 )
 
 GetDocumentVersionResponseTypeDef = TypedDict(
     "GetDocumentVersionResponseTypeDef",
     {
         "Metadata": DocumentVersionMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGroupsResponseTypeDef = TypedDict(
     "DescribeGroupsResponseTypeDef",
     {
         "Groups": List[GroupMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ParticipantsTypeDef = TypedDict(
     "ParticipantsTypeDef",
     {
         "Users": List[UserMetadataTypeDef],
@@ -1677,71 +1678,58 @@
     "ResourcePathTypeDef",
     {
         "Components": List[ResourcePathComponentTypeDef],
     },
     total=False,
 )
 
-UserTypeDef = TypedDict(
-    "UserTypeDef",
+UserStorageMetadataTypeDef = TypedDict(
+    "UserStorageMetadataTypeDef",
     {
-        "Id": str,
-        "Username": str,
-        "EmailAddress": str,
-        "GivenName": str,
-        "Surname": str,
-        "OrganizationId": str,
-        "RootFolderId": str,
-        "RecycleBinFolderId": str,
-        "Status": UserStatusTypeType,
-        "Type": UserTypeType,
-        "CreatedTimestamp": datetime,
-        "ModifiedTimestamp": datetime,
-        "TimeZoneId": str,
-        "Locale": LocaleTypeType,
-        "Storage": UserStorageMetadataTypeDef,
+        "StorageUtilizedInBytes": int,
+        "StorageRule": StorageRuleTypeOutputTypeDef,
     },
     total=False,
 )
 
 DescribeFolderContentsResponseTypeDef = TypedDict(
     "DescribeFolderContentsResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentResponseTypeDef = TypedDict(
     "GetDocumentResponseTypeDef",
     {
         "Metadata": DocumentMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcesResponseTypeDef = TypedDict(
     "GetResourcesResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InitiateDocumentVersionUploadResponseTypeDef = TypedDict(
     "InitiateDocumentVersionUploadResponseTypeDef",
     {
         "Metadata": DocumentMetadataTypeDef,
         "UploadMetadata": UploadMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchResourcesRequestRequestTypeDef = TypedDict(
     "SearchResourcesRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
@@ -1763,49 +1751,71 @@
         "AuthenticationToken": str,
         "QueryText": str,
         "QueryScopes": Sequence[SearchQueryScopeTypeType],
         "OrganizationId": str,
         "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
         "Filters": FiltersTypeDef,
         "OrderBy": Sequence[SearchSortResultTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeResourcePermissionsResponseTypeDef = TypedDict(
     "DescribeResourcePermissionsResponseTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentPathResponseTypeDef = TypedDict(
     "GetDocumentPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFolderPathResponseTypeDef = TypedDict(
     "GetFolderPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UserTypeDef = TypedDict(
+    "UserTypeDef",
+    {
+        "Id": str,
+        "Username": str,
+        "EmailAddress": str,
+        "GivenName": str,
+        "Surname": str,
+        "OrganizationId": str,
+        "RootFolderId": str,
+        "RecycleBinFolderId": str,
+        "Status": UserStatusTypeType,
+        "Type": UserTypeType,
+        "CreatedTimestamp": datetime,
+        "ModifiedTimestamp": datetime,
+        "TimeZoneId": str,
+        "Locale": LocaleTypeType,
+        "Storage": UserStorageMetadataTypeDef,
+    },
+    total=False,
+)
+
 ActivateUserResponseTypeDef = TypedDict(
     "ActivateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommentMetadataTypeDef = TypedDict(
     "CommentMetadataTypeDef",
     {
         "CommentId": str,
@@ -1844,41 +1854,41 @@
     pass
 
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUsersResponseTypeDef = TypedDict(
     "DescribeUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "TotalNumberOfUsers": int,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCurrentUserResponseTypeDef = TypedDict(
     "GetCurrentUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActivityTypeDef = TypedDict(
     "ActivityTypeDef",
     {
         "Type": ActivityTypeType,
@@ -1907,37 +1917,37 @@
     total=False,
 )
 
 CreateCommentResponseTypeDef = TypedDict(
     "CreateCommentResponseTypeDef",
     {
         "Comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCommentsResponseTypeDef = TypedDict(
     "DescribeCommentsResponseTypeDef",
     {
         "Comments": List[CommentTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeActivitiesResponseTypeDef = TypedDict(
     "DescribeActivitiesResponseTypeDef",
     {
         "UserActivities": List[ActivityTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchResourcesResponseTypeDef = TypedDict(
     "SearchResourcesResponseTypeDef",
     {
         "Items": List[ResponseItemTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs/type_defs.pyi` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AbortDocumentVersionUploadRequestRequestTypeDef",
     "ActivateUserRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UserMetadataTypeDef",
     "NotificationOptionsTypeDef",
     "SharePrincipalTypeDef",
     "ShareResultTypeDef",
     "CreateCommentRequestRequestTypeDef",
     "CreateCustomMetadataRequestRequestTypeDef",
     "CreateFolderRequestRequestTypeDef",
@@ -81,86 +82,86 @@
     "DeleteDocumentRequestRequestTypeDef",
     "DeleteDocumentVersionRequestRequestTypeDef",
     "DeleteFolderContentsRequestRequestTypeDef",
     "DeleteFolderRequestRequestTypeDef",
     "DeleteLabelsRequestRequestTypeDef",
     "DeleteNotificationSubscriptionRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
-    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeActivitiesRequestRequestTypeDef",
-    "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
     "DescribeCommentsRequestRequestTypeDef",
-    "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
     "DescribeDocumentVersionsRequestRequestTypeDef",
     "DocumentVersionMetadataTypeDef",
-    "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
     "DescribeFolderContentsRequestRequestTypeDef",
-    "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
     "DescribeGroupsRequestRequestTypeDef",
     "GroupMetadataTypeDef",
-    "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
     "DescribeNotificationSubscriptionsRequestRequestTypeDef",
-    "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
     "DescribeResourcePermissionsRequestRequestTypeDef",
-    "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
     "DescribeRootFoldersRequestRequestTypeDef",
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "LongRangeTypeTypeDef",
     "SearchPrincipalTypeTypeDef",
     "GetCurrentUserRequestRequestTypeDef",
     "GetDocumentPathRequestRequestTypeDef",
     "GetDocumentRequestRequestTypeDef",
     "GetDocumentVersionRequestRequestTypeDef",
     "GetFolderPathRequestRequestTypeDef",
     "GetFolderRequestRequestTypeDef",
     "GetResourcesRequestRequestTypeDef",
     "InitiateDocumentVersionUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
-    "PaginatorConfigTypeDef",
     "PermissionInfoTypeDef",
     "RemoveAllResourcePermissionsRequestRequestTypeDef",
     "RemoveResourcePermissionRequestRequestTypeDef",
     "ResourcePathComponentTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreDocumentVersionsRequestRequestTypeDef",
     "SearchSortResultTypeDef",
+    "StorageRuleTypeOutputTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
     "UpdateDocumentVersionRequestRequestTypeDef",
     "UpdateFolderRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ResourceMetadataTypeDef",
     "AddResourcePermissionsRequestRequestTypeDef",
     "AddResourcePermissionsResponseTypeDef",
     "CreateFolderResponseTypeDef",
     "DescribeRootFoldersResponseTypeDef",
     "GetFolderResponseTypeDef",
     "CreateNotificationSubscriptionResponseTypeDef",
     "DescribeNotificationSubscriptionsResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
-    "UserStorageMetadataTypeDef",
+    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
+    "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    "DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeDocumentVersionsResponseTypeDef",
     "DocumentMetadataTypeDef",
     "GetDocumentVersionResponseTypeDef",
     "DescribeGroupsResponseTypeDef",
     "ParticipantsTypeDef",
     "FiltersTypeDef",
     "PrincipalTypeDef",
     "ResourcePathTypeDef",
-    "UserTypeDef",
+    "UserStorageMetadataTypeDef",
     "DescribeFolderContentsResponseTypeDef",
     "GetDocumentResponseTypeDef",
     "GetResourcesResponseTypeDef",
     "InitiateDocumentVersionUploadResponseTypeDef",
     "SearchResourcesRequestRequestTypeDef",
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "DescribeResourcePermissionsResponseTypeDef",
     "GetDocumentPathResponseTypeDef",
     "GetFolderPathResponseTypeDef",
+    "UserTypeDef",
     "ActivateUserResponseTypeDef",
     "CommentMetadataTypeDef",
     "CommentTypeDef",
     "CreateUserResponseTypeDef",
     "DescribeUsersResponseTypeDef",
     "GetCurrentUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
@@ -208,14 +209,25 @@
 )
 
 class ActivateUserRequestRequestTypeDef(
     _RequiredActivateUserRequestRequestTypeDef, _OptionalActivateUserRequestRequestTypeDef
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
+
 UserMetadataTypeDef = TypedDict(
     "UserMetadataTypeDef",
     {
         "Id": str,
         "Username": str,
         "GivenName": str,
         "Surname": str,
@@ -585,26 +597,20 @@
 )
 
 class DeleteUserRequestRequestTypeDef(
     _RequiredDeleteUserRequestRequestTypeDef, _OptionalDeleteUserRequestRequestTypeDef
 ):
     pass
 
-DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
-    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AuthenticationToken": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "OrganizationId": str,
-        "ActivityTypes": str,
-        "ResourceId": str,
-        "UserId": str,
-        "IncludeIndirectActivities": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeActivitiesRequestRequestTypeDef = TypedDict(
     "DescribeActivitiesRequestRequestTypeDef",
     {
@@ -618,36 +624,14 @@
         "IncludeIndirectActivities": bool,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
-    {
-        "DocumentId": str,
-        "VersionId": str,
-    },
-)
-_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeCommentsRequestDescribeCommentsPaginateTypeDef(
-    _RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-    _OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeCommentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommentsRequestRequestTypeDef",
     {
         "DocumentId": str,
         "VersionId": str,
     },
 )
@@ -662,37 +646,14 @@
 )
 
 class DescribeCommentsRequestRequestTypeDef(
     _RequiredDescribeCommentsRequestRequestTypeDef, _OptionalDescribeCommentsRequestRequestTypeDef
 ):
     pass
 
-_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    {
-        "DocumentId": str,
-    },
-)
-_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Include": str,
-        "Fields": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef(
-    _RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-    _OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDocumentVersionsRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalDescribeDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -729,39 +690,14 @@
         "CreatorId": str,
         "Thumbnail": Dict[DocumentThumbnailTypeType, str],
         "Source": Dict[DocumentSourceTypeType, str],
     },
     total=False,
 )
 
-_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    {
-        "FolderId": str,
-    },
-)
-_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "Sort": ResourceSortTypeType,
-        "Order": OrderTypeType,
-        "Type": FolderContentTypeType,
-        "Include": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef(
-    _RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-    _OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeFolderContentsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeFolderContentsRequestRequestTypeDef",
     {
         "FolderId": str,
     },
 )
 _OptionalDescribeFolderContentsRequestRequestTypeDef = TypedDict(
@@ -780,36 +716,14 @@
 
 class DescribeFolderContentsRequestRequestTypeDef(
     _RequiredDescribeFolderContentsRequestRequestTypeDef,
     _OptionalDescribeFolderContentsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    {
-        "SearchQuery": str,
-    },
-)
-_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "OrganizationId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeGroupsRequestDescribeGroupsPaginateTypeDef(
-    _RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-    _OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeGroupsRequestRequestTypeDef",
     {
         "SearchQuery": str,
     },
 )
 _OptionalDescribeGroupsRequestRequestTypeDef = TypedDict(
@@ -833,34 +747,14 @@
     {
         "Id": str,
         "Name": str,
     },
     total=False,
 )
 
-_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    {
-        "OrganizationId": str,
-    },
-)
-_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef(
-    _RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-    _OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalDescribeNotificationSubscriptionsRequestRequestTypeDef = TypedDict(
@@ -874,36 +768,14 @@
 
 class DescribeNotificationSubscriptionsRequestRequestTypeDef(
     _RequiredDescribeNotificationSubscriptionsRequestRequestTypeDef,
     _OptionalDescribeNotificationSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "PrincipalId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef(
-    _RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-    _OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeResourcePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourcePermissionsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalDescribeResourcePermissionsRequestRequestTypeDef = TypedDict(
@@ -919,34 +791,14 @@
 
 class DescribeResourcePermissionsRequestRequestTypeDef(
     _RequiredDescribeResourcePermissionsRequestRequestTypeDef,
     _OptionalDescribeResourcePermissionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-    },
-)
-_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef(
-    _RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-    _OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeRootFoldersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRootFoldersRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
     },
 )
 _OptionalDescribeRootFoldersRequestRequestTypeDef = TypedDict(
@@ -960,30 +812,14 @@
 
 class DescribeRootFoldersRequestRequestTypeDef(
     _RequiredDescribeRootFoldersRequestRequestTypeDef,
     _OptionalDescribeRootFoldersRequestRequestTypeDef,
 ):
     pass
 
-DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
-    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
-    {
-        "AuthenticationToken": str,
-        "OrganizationId": str,
-        "UserIds": str,
-        "Query": str,
-        "Include": UserFilterTypeType,
-        "Order": OrderTypeType,
-        "Sort": UserSortTypeType,
-        "Fields": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUsersRequestRequestTypeDef = TypedDict(
     "DescribeUsersRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
         "OrganizationId": str,
         "UserIds": str,
         "Query": str,
@@ -993,21 +829,14 @@
         "Marker": str,
         "Limit": int,
         "Fields": str,
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
 LongRangeTypeTypeDef = TypedDict(
     "LongRangeTypeTypeDef",
     {
         "StartValue": int,
         "EndValue": int,
     },
     total=False,
@@ -1178,24 +1007,14 @@
     {
         "UploadUrl": str,
         "SignedHeaders": Dict[str, str],
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
 PermissionInfoTypeDef = TypedDict(
     "PermissionInfoTypeDef",
     {
         "Role": RoleTypeType,
         "Type": RolePermissionTypeType,
     },
     total=False,
@@ -1248,25 +1067,14 @@
     {
         "Id": str,
         "Name": str,
     },
     total=False,
 )
 
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
 _RequiredRestoreDocumentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreDocumentVersionsRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalRestoreDocumentVersionsRequestRequestTypeDef = TypedDict(
@@ -1288,14 +1096,23 @@
     {
         "Field": OrderByFieldTypeType,
         "Order": SortOrderType,
     },
     total=False,
 )
 
+StorageRuleTypeOutputTypeDef = TypedDict(
+    "StorageRuleTypeOutputTypeDef",
+    {
+        "StorageAllocatedInBytes": int,
+        "StorageType": StorageTypeType,
+    },
+    total=False,
+)
+
 _RequiredUpdateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalUpdateDocumentRequestRequestTypeDef = TypedDict(
@@ -1354,14 +1171,21 @@
 )
 
 class UpdateFolderRequestRequestTypeDef(
     _RequiredUpdateFolderRequestRequestTypeDef, _OptionalUpdateFolderRequestRequestTypeDef
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ResourceMetadataTypeDef = TypedDict(
     "ResourceMetadataTypeDef",
     {
         "Type": ResourceTypeType,
         "Name": str,
         "OriginalName": str,
         "Id": str,
@@ -1394,58 +1218,58 @@
 ):
     pass
 
 AddResourcePermissionsResponseTypeDef = TypedDict(
     "AddResourcePermissionsResponseTypeDef",
     {
         "ShareResults": List[ShareResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFolderResponseTypeDef = TypedDict(
     "CreateFolderResponseTypeDef",
     {
         "Metadata": FolderMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRootFoldersResponseTypeDef = TypedDict(
     "DescribeRootFoldersResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFolderResponseTypeDef = TypedDict(
     "GetFolderResponseTypeDef",
     {
         "Metadata": FolderMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNotificationSubscriptionResponseTypeDef = TypedDict(
     "CreateNotificationSubscriptionResponseTypeDef",
     {
         "Subscription": SubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotificationSubscriptionsResponseTypeDef = TypedDict(
     "DescribeNotificationSubscriptionsResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "Username": str,
@@ -1493,29 +1317,206 @@
 )
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
-UserStorageMetadataTypeDef = TypedDict(
-    "UserStorageMetadataTypeDef",
+DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
+    "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     {
-        "StorageUtilizedInBytes": int,
-        "StorageRule": StorageRuleTypeTypeDef,
+        "AuthenticationToken": str,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "OrganizationId": str,
+        "ActivityTypes": str,
+        "ResourceId": str,
+        "UserId": str,
+        "IncludeIndirectActivities": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    {
+        "DocumentId": str,
+        "VersionId": str,
+    },
+)
+_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeCommentsRequestDescribeCommentsPaginateTypeDef(
+    _RequiredDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    _OptionalDescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    {
+        "DocumentId": str,
+    },
+)
+_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Include": str,
+        "Fields": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef(
+    _RequiredDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+    _OptionalDescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    {
+        "FolderId": str,
+    },
+)
+_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "Sort": ResourceSortTypeType,
+        "Order": OrderTypeType,
+        "Type": FolderContentTypeType,
+        "Include": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef(
+    _RequiredDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+    _OptionalDescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    {
+        "SearchQuery": str,
+    },
+)
+_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "OrganizationId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeGroupsRequestDescribeGroupsPaginateTypeDef(
+    _RequiredDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+    _OptionalDescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    {
+        "OrganizationId": str,
+    },
+)
+_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef(
+    _RequiredDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+    _OptionalDescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "PrincipalId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef(
+    _RequiredDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+    _OptionalDescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+    },
+)
+_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef(
+    _RequiredDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+    _OptionalDescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+):
+    pass
+
+DescribeUsersRequestDescribeUsersPaginateTypeDef = TypedDict(
+    "DescribeUsersRequestDescribeUsersPaginateTypeDef",
+    {
+        "AuthenticationToken": str,
+        "OrganizationId": str,
+        "UserIds": str,
+        "Query": str,
+        "Include": UserFilterTypeType,
+        "Order": OrderTypeType,
+        "Sort": UserSortTypeType,
+        "Fields": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeDocumentVersionsResponseTypeDef = TypedDict(
     "DescribeDocumentVersionsResponseTypeDef",
     {
         "DocumentVersions": List[DocumentVersionMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DocumentMetadataTypeDef = TypedDict(
     "DocumentMetadataTypeDef",
     {
         "Id": str,
@@ -1531,24 +1532,24 @@
 )
 
 GetDocumentVersionResponseTypeDef = TypedDict(
     "GetDocumentVersionResponseTypeDef",
     {
         "Metadata": DocumentVersionMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGroupsResponseTypeDef = TypedDict(
     "DescribeGroupsResponseTypeDef",
     {
         "Groups": List[GroupMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ParticipantsTypeDef = TypedDict(
     "ParticipantsTypeDef",
     {
         "Users": List[UserMetadataTypeDef],
@@ -1588,71 +1589,58 @@
     "ResourcePathTypeDef",
     {
         "Components": List[ResourcePathComponentTypeDef],
     },
     total=False,
 )
 
-UserTypeDef = TypedDict(
-    "UserTypeDef",
+UserStorageMetadataTypeDef = TypedDict(
+    "UserStorageMetadataTypeDef",
     {
-        "Id": str,
-        "Username": str,
-        "EmailAddress": str,
-        "GivenName": str,
-        "Surname": str,
-        "OrganizationId": str,
-        "RootFolderId": str,
-        "RecycleBinFolderId": str,
-        "Status": UserStatusTypeType,
-        "Type": UserTypeType,
-        "CreatedTimestamp": datetime,
-        "ModifiedTimestamp": datetime,
-        "TimeZoneId": str,
-        "Locale": LocaleTypeType,
-        "Storage": UserStorageMetadataTypeDef,
+        "StorageUtilizedInBytes": int,
+        "StorageRule": StorageRuleTypeOutputTypeDef,
     },
     total=False,
 )
 
 DescribeFolderContentsResponseTypeDef = TypedDict(
     "DescribeFolderContentsResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentResponseTypeDef = TypedDict(
     "GetDocumentResponseTypeDef",
     {
         "Metadata": DocumentMetadataTypeDef,
         "CustomMetadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcesResponseTypeDef = TypedDict(
     "GetResourcesResponseTypeDef",
     {
         "Folders": List[FolderMetadataTypeDef],
         "Documents": List[DocumentMetadataTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InitiateDocumentVersionUploadResponseTypeDef = TypedDict(
     "InitiateDocumentVersionUploadResponseTypeDef",
     {
         "Metadata": DocumentMetadataTypeDef,
         "UploadMetadata": UploadMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchResourcesRequestRequestTypeDef = TypedDict(
     "SearchResourcesRequestRequestTypeDef",
     {
         "AuthenticationToken": str,
@@ -1674,49 +1662,71 @@
         "AuthenticationToken": str,
         "QueryText": str,
         "QueryScopes": Sequence[SearchQueryScopeTypeType],
         "OrganizationId": str,
         "AdditionalResponseFields": Sequence[Literal["WEBURL"]],
         "Filters": FiltersTypeDef,
         "OrderBy": Sequence[SearchSortResultTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeResourcePermissionsResponseTypeDef = TypedDict(
     "DescribeResourcePermissionsResponseTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentPathResponseTypeDef = TypedDict(
     "GetDocumentPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFolderPathResponseTypeDef = TypedDict(
     "GetFolderPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UserTypeDef = TypedDict(
+    "UserTypeDef",
+    {
+        "Id": str,
+        "Username": str,
+        "EmailAddress": str,
+        "GivenName": str,
+        "Surname": str,
+        "OrganizationId": str,
+        "RootFolderId": str,
+        "RecycleBinFolderId": str,
+        "Status": UserStatusTypeType,
+        "Type": UserTypeType,
+        "CreatedTimestamp": datetime,
+        "ModifiedTimestamp": datetime,
+        "TimeZoneId": str,
+        "Locale": LocaleTypeType,
+        "Storage": UserStorageMetadataTypeDef,
+    },
+    total=False,
+)
+
 ActivateUserResponseTypeDef = TypedDict(
     "ActivateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommentMetadataTypeDef = TypedDict(
     "CommentMetadataTypeDef",
     {
         "CommentId": str,
@@ -1753,41 +1763,41 @@
 class CommentTypeDef(_RequiredCommentTypeDef, _OptionalCommentTypeDef):
     pass
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUsersResponseTypeDef = TypedDict(
     "DescribeUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "TotalNumberOfUsers": int,
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCurrentUserResponseTypeDef = TypedDict(
     "GetCurrentUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActivityTypeDef = TypedDict(
     "ActivityTypeDef",
     {
         "Type": ActivityTypeType,
@@ -1816,37 +1826,37 @@
     total=False,
 )
 
 CreateCommentResponseTypeDef = TypedDict(
     "CreateCommentResponseTypeDef",
     {
         "Comment": CommentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCommentsResponseTypeDef = TypedDict(
     "DescribeCommentsResponseTypeDef",
     {
         "Comments": List[CommentTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeActivitiesResponseTypeDef = TypedDict(
     "DescribeActivitiesResponseTypeDef",
     {
         "UserActivities": List[ActivityTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchResourcesResponseTypeDef = TypedDict(
     "SearchResourcesResponseTypeDef",
     {
         "Items": List[ResponseItemTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs.egg-info/PKG-INFO` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workdocs
-Version: 1.28.0
-Summary: Type annotations for boto3.WorkDocs 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WorkDocs 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-workdocs"></a>
 
 # mypy-boto3-workdocs
 
 [![PyPI - mypy-boto3-workdocs](https://img.shields.io/pypi/v/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-workdocs?color=blue)](https://pypistats.org/packages/mypy-boto3-workdocs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workdocs)](https://pepy.tech/project/mypy-boto3-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkDocs 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[boto3.WorkDocs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [mypy-boto3-workdocs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -397,14 +397,15 @@
 `mypy_boto3_workdocs.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_workdocs.type_defs import (
     AbortDocumentVersionUploadRequestRequestTypeDef,
     ActivateUserRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UserMetadataTypeDef,
     NotificationOptionsTypeDef,
     SharePrincipalTypeDef,
     ShareResultTypeDef,
     CreateCommentRequestRequestTypeDef,
     CreateCustomMetadataRequestRequestTypeDef,
     CreateFolderRequestRequestTypeDef,
@@ -420,86 +421,86 @@
     DeleteDocumentRequestRequestTypeDef,
     DeleteDocumentVersionRequestRequestTypeDef,
     DeleteFolderContentsRequestRequestTypeDef,
     DeleteFolderRequestRequestTypeDef,
     DeleteLabelsRequestRequestTypeDef,
     DeleteNotificationSubscriptionRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
-    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeActivitiesRequestRequestTypeDef,
-    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
     DescribeCommentsRequestRequestTypeDef,
-    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeDocumentVersionsRequestRequestTypeDef,
     DocumentVersionMetadataTypeDef,
-    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeFolderContentsRequestRequestTypeDef,
-    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeGroupsRequestRequestTypeDef,
     GroupMetadataTypeDef,
-    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestRequestTypeDef,
-    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
     DescribeResourcePermissionsRequestRequestTypeDef,
-    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
     DescribeRootFoldersRequestRequestTypeDef,
-    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     LongRangeTypeTypeDef,
     SearchPrincipalTypeTypeDef,
     GetCurrentUserRequestRequestTypeDef,
     GetDocumentPathRequestRequestTypeDef,
     GetDocumentRequestRequestTypeDef,
     GetDocumentVersionRequestRequestTypeDef,
     GetFolderPathRequestRequestTypeDef,
     GetFolderRequestRequestTypeDef,
     GetResourcesRequestRequestTypeDef,
     InitiateDocumentVersionUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
-    PaginatorConfigTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
-    ResponseMetadataTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
+    StorageRuleTypeOutputTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     UpdateDocumentVersionRequestRequestTypeDef,
     UpdateFolderRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     ResourceMetadataTypeDef,
     AddResourcePermissionsRequestRequestTypeDef,
     AddResourcePermissionsResponseTypeDef,
     CreateFolderResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
-    UserStorageMetadataTypeDef,
+    DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
+    DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
+    DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
+    DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
+    DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
+    DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
+    DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
+    DescribeRootFoldersRequestDescribeRootFoldersPaginateTypeDef,
+    DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeDocumentVersionsResponseTypeDef,
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
     FiltersTypeDef,
     PrincipalTypeDef,
     ResourcePathTypeDef,
-    UserTypeDef,
+    UserStorageMetadataTypeDef,
     DescribeFolderContentsResponseTypeDef,
     GetDocumentResponseTypeDef,
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
     SearchResourcesRequestRequestTypeDef,
     SearchResourcesRequestSearchResourcesPaginateTypeDef,
     DescribeResourcePermissionsResponseTypeDef,
     GetDocumentPathResponseTypeDef,
     GetFolderPathResponseTypeDef,
+    UserTypeDef,
     ActivateUserResponseTypeDef,
     CommentMetadataTypeDef,
     CommentTypeDef,
     CreateUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     GetCurrentUserResponseTypeDef,
     UpdateUserResponseTypeDef,
```

### Comparing `mypy-boto3-workdocs-1.28.0/mypy_boto3_workdocs.egg-info/SOURCES.txt` & `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.0/setup.py` & `mypy-boto3-workdocs-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workdocs",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_workdocs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkDocs 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.WorkDocs 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

