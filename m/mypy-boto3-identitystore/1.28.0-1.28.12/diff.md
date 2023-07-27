# Comparing `tmp/mypy-boto3-identitystore-1.28.0.tar.gz` & `tmp/mypy-boto3-identitystore-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-identitystore-1.28.0.tar", last modified: Thu Jul  6 20:59:43 2023, max compression
+gzip compressed data, was "mypy-boto3-identitystore-1.28.12.tar", last modified: Thu Jul 27 05:34:46 2023, max compression
```

## Comparing `mypy-boto3-identitystore-1.28.0.tar` & `mypy-boto3-identitystore-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:43.770321 mypy-boto3-identitystore-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-07-06 20:59:43.770321 mypy-boto3-identitystore-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:43.766321 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-07-06 20:42:52.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-07-06 20:42:52.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19245 2023-07-06 20:42:52.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:43.770321 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-07-06 20:59:43.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 20:59:43.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:43.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:43.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:43.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 20:59:43.000000 mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:43.770321 mypy-boto3-identitystore-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-06 20:42:51.000000 mypy-boto3-identitystore-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.736492 mypy-boto3-identitystore-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15467 2023-07-27 05:34:46.736492 mypy-boto3-identitystore-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.736492 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-27 05:23:28.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-27 05:23:28.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-27 05:23:28.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20678 2023-07-27 05:23:28.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-07-27 05:23:28.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.736492 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15467 2023-07-27 05:34:46.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 05:34:46.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:46.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:46.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:46.736492 mypy-boto3-identitystore-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/setup.py
```

### Comparing `mypy-boto3-identitystore-1.28.0/LICENSE` & `mypy-boto3-identitystore-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.0/PKG-INFO` & `mypy-boto3-identitystore-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-identitystore
-Version: 1.28.0
-Summary: Type annotations for boto3.IdentityStore 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IdentityStore 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-identitystore"></a>
 
 # mypy-boto3-identitystore
 
 [![PyPI - mypy-boto3-identitystore](https://img.shields.io/pypi/v/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-identitystore?color=blue)](https://pypistats.org/packages/mypy-boto3-identitystore)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-identitystore)](https://pepy.tech/project/mypy-boto3-identitystore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IdentityStore 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
+[boto3.IdentityStore 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
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
 [mypy-boto3-identitystore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,14 +334,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_identitystore.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_identitystore.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     ExternalIdTypeDef,
     UniqueAttributeTypeDef,
     AttributeOperationTypeDef,
     MemberIdTypeDef,
     CreateGroupMembershipResponseTypeDef,
     CreateGroupRequestRequestTypeDef,
@@ -350,55 +351,60 @@
     NameTypeDef,
     PhoneNumberTypeDef,
     CreateUserResponseTypeDef,
     DeleteGroupMembershipRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeGroupMembershipRequestRequestTypeDef,
+    MemberIdOutputTypeDef,
     DescribeGroupRequestRequestTypeDef,
+    ExternalIdOutputTypeDef,
     DescribeUserRequestRequestTypeDef,
+    EmailOutputTypeDef,
+    NameOutputTypeDef,
+    PhoneNumberOutputTypeDef,
     FilterTypeDef,
     GetGroupIdResponseTypeDef,
     GetGroupMembershipIdResponseTypeDef,
     GetUserIdResponseTypeDef,
     ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
     ListGroupMembershipsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
-    DescribeGroupResponseTypeDef,
-    GroupTypeDef,
     AlternateIdentifierTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
-    DescribeGroupMembershipResponseTypeDef,
     GetGroupMembershipIdRequestRequestTypeDef,
-    GroupMembershipExistenceResultTypeDef,
-    GroupMembershipTypeDef,
     IsMemberInGroupsRequestRequestTypeDef,
     ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     ListGroupMembershipsForMemberRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
+    DescribeGroupMembershipResponseTypeDef,
+    GroupMembershipExistenceResultTypeDef,
+    GroupMembershipTypeDef,
+    DescribeGroupResponseTypeDef,
+    GroupTypeDef,
     DescribeUserResponseTypeDef,
     UserTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
-    ListGroupsResponseTypeDef,
     GetGroupIdRequestRequestTypeDef,
     GetUserIdRequestRequestTypeDef,
     IsMemberInGroupsResponseTypeDef,
     ListGroupMembershipsForMemberResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
+    ListGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-identitystore-1.28.0/README.md` & `mypy-boto3-identitystore-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-identitystore"></a>
 
 # mypy-boto3-identitystore
 
 [![PyPI - mypy-boto3-identitystore](https://img.shields.io/pypi/v/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-identitystore?color=blue)](https://pypistats.org/packages/mypy-boto3-identitystore)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-identitystore)](https://pepy.tech/project/mypy-boto3-identitystore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IdentityStore 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
+[boto3.IdentityStore 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
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
 [mypy-boto3-identitystore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,14 +302,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_identitystore.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_identitystore.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     ExternalIdTypeDef,
     UniqueAttributeTypeDef,
     AttributeOperationTypeDef,
     MemberIdTypeDef,
     CreateGroupMembershipResponseTypeDef,
     CreateGroupRequestRequestTypeDef,
@@ -318,55 +319,60 @@
     NameTypeDef,
     PhoneNumberTypeDef,
     CreateUserResponseTypeDef,
     DeleteGroupMembershipRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeGroupMembershipRequestRequestTypeDef,
+    MemberIdOutputTypeDef,
     DescribeGroupRequestRequestTypeDef,
+    ExternalIdOutputTypeDef,
     DescribeUserRequestRequestTypeDef,
+    EmailOutputTypeDef,
+    NameOutputTypeDef,
+    PhoneNumberOutputTypeDef,
     FilterTypeDef,
     GetGroupIdResponseTypeDef,
     GetGroupMembershipIdResponseTypeDef,
     GetUserIdResponseTypeDef,
     ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
     ListGroupMembershipsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
-    DescribeGroupResponseTypeDef,
-    GroupTypeDef,
     AlternateIdentifierTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
-    DescribeGroupMembershipResponseTypeDef,
     GetGroupMembershipIdRequestRequestTypeDef,
-    GroupMembershipExistenceResultTypeDef,
-    GroupMembershipTypeDef,
     IsMemberInGroupsRequestRequestTypeDef,
     ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     ListGroupMembershipsForMemberRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
+    DescribeGroupMembershipResponseTypeDef,
+    GroupMembershipExistenceResultTypeDef,
+    GroupMembershipTypeDef,
+    DescribeGroupResponseTypeDef,
+    GroupTypeDef,
     DescribeUserResponseTypeDef,
     UserTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
-    ListGroupsResponseTypeDef,
     GetGroupIdRequestRequestTypeDef,
     GetUserIdRequestRequestTypeDef,
     IsMemberInGroupsResponseTypeDef,
     ListGroupMembershipsForMemberResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
+    ListGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/__init__.py` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/__init__.pyi` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/__main__.py` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IdentityStore 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.IdentityStore 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore\nOther"
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

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/client.py` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/client.pyi` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/literals.py` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
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
@@ -238,26 +239,28 @@
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

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/literals.pyi` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
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
@@ -236,26 +237,28 @@
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

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/paginator.py` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/paginator.pyi` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/type_defs.py` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 Type annotations for identitystore service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_identitystore.type_defs import AddressTypeDef
+    from mypy_boto3_identitystore.type_defs import AddressOutputTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Any, Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AddressOutputTypeDef",
     "AddressTypeDef",
     "ExternalIdTypeDef",
     "UniqueAttributeTypeDef",
     "AttributeOperationTypeDef",
     "MemberIdTypeDef",
     "CreateGroupMembershipResponseTypeDef",
     "CreateGroupRequestRequestTypeDef",
@@ -33,53 +33,73 @@
     "NameTypeDef",
     "PhoneNumberTypeDef",
     "CreateUserResponseTypeDef",
     "DeleteGroupMembershipRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeGroupMembershipRequestRequestTypeDef",
+    "MemberIdOutputTypeDef",
     "DescribeGroupRequestRequestTypeDef",
+    "ExternalIdOutputTypeDef",
     "DescribeUserRequestRequestTypeDef",
+    "EmailOutputTypeDef",
+    "NameOutputTypeDef",
+    "PhoneNumberOutputTypeDef",
     "FilterTypeDef",
     "GetGroupIdResponseTypeDef",
     "GetGroupMembershipIdResponseTypeDef",
     "GetUserIdResponseTypeDef",
     "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
     "ListGroupMembershipsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
-    "DescribeGroupResponseTypeDef",
-    "GroupTypeDef",
     "AlternateIdentifierTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
-    "DescribeGroupMembershipResponseTypeDef",
     "GetGroupMembershipIdRequestRequestTypeDef",
-    "GroupMembershipExistenceResultTypeDef",
-    "GroupMembershipTypeDef",
     "IsMemberInGroupsRequestRequestTypeDef",
     "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
     "ListGroupMembershipsForMemberRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
+    "DescribeGroupMembershipResponseTypeDef",
+    "GroupMembershipExistenceResultTypeDef",
+    "GroupMembershipTypeDef",
+    "DescribeGroupResponseTypeDef",
+    "GroupTypeDef",
     "DescribeUserResponseTypeDef",
     "UserTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
-    "ListGroupsResponseTypeDef",
     "GetGroupIdRequestRequestTypeDef",
     "GetUserIdRequestRequestTypeDef",
     "IsMemberInGroupsResponseTypeDef",
     "ListGroupMembershipsForMemberResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
+    "ListGroupsResponseTypeDef",
     "ListUsersResponseTypeDef",
 )
 
+AddressOutputTypeDef = TypedDict(
+    "AddressOutputTypeDef",
+    {
+        "StreetAddress": str,
+        "Locality": str,
+        "Region": str,
+        "PostalCode": str,
+        "Country": str,
+        "Formatted": str,
+        "Type": str,
+        "Primary": bool,
+    },
+    total=False,
+)
+
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "StreetAddress": str,
         "Locality": str,
         "Region": str,
         "PostalCode": str,
@@ -117,21 +137,19 @@
     "_OptionalAttributeOperationTypeDef",
     {
         "AttributeValue": Mapping[str, Any],
     },
     total=False,
 )
 
-
 class AttributeOperationTypeDef(
     _RequiredAttributeOperationTypeDef, _OptionalAttributeOperationTypeDef
 ):
     pass
 
-
 MemberIdTypeDef = TypedDict(
     "MemberIdTypeDef",
     {
         "UserId": str,
     },
     total=False,
 )
@@ -156,21 +174,19 @@
     {
         "DisplayName": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
-
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "GroupId": str,
         "IdentityStoreId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -246,30 +262,79 @@
     "DescribeGroupMembershipRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MembershipId": str,
     },
 )
 
+MemberIdOutputTypeDef = TypedDict(
+    "MemberIdOutputTypeDef",
+    {
+        "UserId": str,
+    },
+    total=False,
+)
+
 DescribeGroupRequestRequestTypeDef = TypedDict(
     "DescribeGroupRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
     },
 )
 
+ExternalIdOutputTypeDef = TypedDict(
+    "ExternalIdOutputTypeDef",
+    {
+        "Issuer": str,
+        "Id": str,
+    },
+)
+
 DescribeUserRequestRequestTypeDef = TypedDict(
     "DescribeUserRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "UserId": str,
     },
 )
 
+EmailOutputTypeDef = TypedDict(
+    "EmailOutputTypeDef",
+    {
+        "Value": str,
+        "Type": str,
+        "Primary": bool,
+    },
+    total=False,
+)
+
+NameOutputTypeDef = TypedDict(
+    "NameOutputTypeDef",
+    {
+        "Formatted": str,
+        "FamilyName": str,
+        "GivenName": str,
+        "MiddleName": str,
+        "HonorificPrefix": str,
+        "HonorificSuffix": str,
+    },
+    total=False,
+)
+
+PhoneNumberOutputTypeDef = TypedDict(
+    "PhoneNumberOutputTypeDef",
+    {
+        "Value": str,
+        "Type": str,
+        "Primary": bool,
+    },
+    total=False,
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "AttributePath": str,
         "AttributeValue": str,
     },
 )
@@ -312,22 +377,20 @@
     "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
     _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
     _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListGroupMembershipsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
     },
 )
@@ -336,22 +399,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListGroupMembershipsRequestRequestTypeDef(
     _RequiredListGroupMembershipsRequestRequestTypeDef,
     _OptionalListGroupMembershipsRequestRequestTypeDef,
 ):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -365,48 +426,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-DescribeGroupResponseTypeDef = TypedDict(
-    "DescribeGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "DisplayName": str,
-        "ExternalIds": List[ExternalIdTypeDef],
-        "Description": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGroupTypeDef = TypedDict(
-    "_RequiredGroupTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-    },
-)
-_OptionalGroupTypeDef = TypedDict(
-    "_OptionalGroupTypeDef",
-    {
-        "DisplayName": str,
-        "ExternalIds": List[ExternalIdTypeDef],
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
-    pass
-
-
 AlternateIdentifierTypeDef = TypedDict(
     "AlternateIdentifierTypeDef",
     {
         "ExternalId": ExternalIdTypeDef,
         "UniqueAttribute": UniqueAttributeTypeDef,
     },
     total=False,
@@ -435,65 +462,23 @@
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
 
-DescribeGroupMembershipResponseTypeDef = TypedDict(
-    "DescribeGroupMembershipResponseTypeDef",
-    {
-        "IdentityStoreId": str,
-        "MembershipId": str,
-        "GroupId": str,
-        "MemberId": MemberIdTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGroupMembershipIdRequestRequestTypeDef = TypedDict(
     "GetGroupMembershipIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
 
-GroupMembershipExistenceResultTypeDef = TypedDict(
-    "GroupMembershipExistenceResultTypeDef",
-    {
-        "GroupId": str,
-        "MemberId": MemberIdTypeDef,
-        "MembershipExists": bool,
-    },
-    total=False,
-)
-
-_RequiredGroupMembershipTypeDef = TypedDict(
-    "_RequiredGroupMembershipTypeDef",
-    {
-        "IdentityStoreId": str,
-    },
-)
-_OptionalGroupMembershipTypeDef = TypedDict(
-    "_OptionalGroupMembershipTypeDef",
-    {
-        "MembershipId": str,
-        "GroupId": str,
-        "MemberId": MemberIdTypeDef,
-    },
-    total=False,
-)
-
-
-class GroupMembershipTypeDef(_RequiredGroupMembershipTypeDef, _OptionalGroupMembershipTypeDef):
-    pass
-
-
 IsMemberInGroupsRequestRequestTypeDef = TypedDict(
     "IsMemberInGroupsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
         "GroupIds": Sequence[str],
     },
@@ -514,22 +499,20 @@
         {
             "PaginationConfig": "PaginatorConfigTypeDef",
         },
         total=False,
     )
 )
 
-
 class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
     _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListGroupMembershipsForMemberRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsForMemberRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
@@ -538,22 +521,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListGroupMembershipsForMemberRequestRequestTypeDef(
     _RequiredListGroupMembershipsForMemberRequestRequestTypeDef,
     _OptionalListGroupMembershipsForMemberRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalCreateUserRequestRequestTypeDef = TypedDict(
@@ -572,34 +553,104 @@
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
     },
     total=False,
 )
 
-
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+DescribeGroupMembershipResponseTypeDef = TypedDict(
+    "DescribeGroupMembershipResponseTypeDef",
+    {
+        "IdentityStoreId": str,
+        "MembershipId": str,
+        "GroupId": str,
+        "MemberId": MemberIdOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GroupMembershipExistenceResultTypeDef = TypedDict(
+    "GroupMembershipExistenceResultTypeDef",
+    {
+        "GroupId": str,
+        "MemberId": MemberIdOutputTypeDef,
+        "MembershipExists": bool,
+    },
+    total=False,
+)
+
+_RequiredGroupMembershipTypeDef = TypedDict(
+    "_RequiredGroupMembershipTypeDef",
+    {
+        "IdentityStoreId": str,
+    },
+)
+_OptionalGroupMembershipTypeDef = TypedDict(
+    "_OptionalGroupMembershipTypeDef",
+    {
+        "MembershipId": str,
+        "GroupId": str,
+        "MemberId": MemberIdOutputTypeDef,
+    },
+    total=False,
+)
+
+class GroupMembershipTypeDef(_RequiredGroupMembershipTypeDef, _OptionalGroupMembershipTypeDef):
+    pass
+
+DescribeGroupResponseTypeDef = TypedDict(
+    "DescribeGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "DisplayName": str,
+        "ExternalIds": List[ExternalIdOutputTypeDef],
+        "Description": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGroupTypeDef = TypedDict(
+    "_RequiredGroupTypeDef",
+    {
+        "GroupId": str,
+        "IdentityStoreId": str,
+    },
+)
+_OptionalGroupTypeDef = TypedDict(
+    "_OptionalGroupTypeDef",
+    {
+        "DisplayName": str,
+        "ExternalIds": List[ExternalIdOutputTypeDef],
+        "Description": str,
+    },
+    total=False,
+)
+
+class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
+    pass
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "UserName": str,
         "UserId": str,
-        "ExternalIds": List[ExternalIdTypeDef],
-        "Name": NameTypeDef,
+        "ExternalIds": List[ExternalIdOutputTypeDef],
+        "Name": NameOutputTypeDef,
         "DisplayName": str,
         "NickName": str,
         "ProfileUrl": str,
-        "Emails": List[EmailTypeDef],
-        "Addresses": List[AddressTypeDef],
-        "PhoneNumbers": List[PhoneNumberTypeDef],
+        "Emails": List[EmailOutputTypeDef],
+        "Addresses": List[AddressOutputTypeDef],
+        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
         "UserType": str,
         "Title": str,
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
         "IdentityStoreId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -613,36 +664,34 @@
         "IdentityStoreId": str,
     },
 )
 _OptionalUserTypeDef = TypedDict(
     "_OptionalUserTypeDef",
     {
         "UserName": str,
-        "ExternalIds": List[ExternalIdTypeDef],
-        "Name": NameTypeDef,
+        "ExternalIds": List[ExternalIdOutputTypeDef],
+        "Name": NameOutputTypeDef,
         "DisplayName": str,
         "NickName": str,
         "ProfileUrl": str,
-        "Emails": List[EmailTypeDef],
-        "Addresses": List[AddressTypeDef],
-        "PhoneNumbers": List[PhoneNumberTypeDef],
+        "Emails": List[EmailOutputTypeDef],
+        "Addresses": List[AddressOutputTypeDef],
+        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
         "UserType": str,
         "Title": str,
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
     },
     total=False,
 )
 
-
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
-
 _RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
     "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
@@ -650,22 +699,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListGroupsRequestListGroupsPaginateTypeDef(
     _RequiredListGroupsRequestListGroupsPaginateTypeDef,
     _OptionalListGroupsRequestListGroupsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalListGroupsRequestRequestTypeDef = TypedDict(
@@ -674,21 +721,19 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
 class ListGroupsRequestRequestTypeDef(
     _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
@@ -696,22 +741,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -720,30 +763,19 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-
-ListGroupsResponseTypeDef = TypedDict(
-    "ListGroupsResponseTypeDef",
-    {
-        "Groups": List[GroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGroupIdRequestRequestTypeDef = TypedDict(
     "GetGroupIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "AlternateIdentifier": AlternateIdentifierTypeDef,
     },
 )
@@ -778,14 +810,23 @@
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListGroupsResponseTypeDef = TypedDict(
+    "ListGroupsResponseTypeDef",
+    {
+        "Groups": List[GroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore/type_defs.pyi` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 Type annotations for identitystore service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_identitystore.type_defs import AddressTypeDef
+    from mypy_boto3_identitystore.type_defs import AddressOutputTypeDef
 
-    data: AddressTypeDef = {...}
+    data: AddressOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Any, Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AddressOutputTypeDef",
     "AddressTypeDef",
     "ExternalIdTypeDef",
     "UniqueAttributeTypeDef",
     "AttributeOperationTypeDef",
     "MemberIdTypeDef",
     "CreateGroupMembershipResponseTypeDef",
     "CreateGroupRequestRequestTypeDef",
@@ -32,53 +34,73 @@
     "NameTypeDef",
     "PhoneNumberTypeDef",
     "CreateUserResponseTypeDef",
     "DeleteGroupMembershipRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeGroupMembershipRequestRequestTypeDef",
+    "MemberIdOutputTypeDef",
     "DescribeGroupRequestRequestTypeDef",
+    "ExternalIdOutputTypeDef",
     "DescribeUserRequestRequestTypeDef",
+    "EmailOutputTypeDef",
+    "NameOutputTypeDef",
+    "PhoneNumberOutputTypeDef",
     "FilterTypeDef",
     "GetGroupIdResponseTypeDef",
     "GetGroupMembershipIdResponseTypeDef",
     "GetUserIdResponseTypeDef",
     "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
     "ListGroupMembershipsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
-    "DescribeGroupResponseTypeDef",
-    "GroupTypeDef",
     "AlternateIdentifierTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
-    "DescribeGroupMembershipResponseTypeDef",
     "GetGroupMembershipIdRequestRequestTypeDef",
-    "GroupMembershipExistenceResultTypeDef",
-    "GroupMembershipTypeDef",
     "IsMemberInGroupsRequestRequestTypeDef",
     "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
     "ListGroupMembershipsForMemberRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
+    "DescribeGroupMembershipResponseTypeDef",
+    "GroupMembershipExistenceResultTypeDef",
+    "GroupMembershipTypeDef",
+    "DescribeGroupResponseTypeDef",
+    "GroupTypeDef",
     "DescribeUserResponseTypeDef",
     "UserTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
-    "ListGroupsResponseTypeDef",
     "GetGroupIdRequestRequestTypeDef",
     "GetUserIdRequestRequestTypeDef",
     "IsMemberInGroupsResponseTypeDef",
     "ListGroupMembershipsForMemberResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
+    "ListGroupsResponseTypeDef",
     "ListUsersResponseTypeDef",
 )
 
+AddressOutputTypeDef = TypedDict(
+    "AddressOutputTypeDef",
+    {
+        "StreetAddress": str,
+        "Locality": str,
+        "Region": str,
+        "PostalCode": str,
+        "Country": str,
+        "Formatted": str,
+        "Type": str,
+        "Primary": bool,
+    },
+    total=False,
+)
+
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "StreetAddress": str,
         "Locality": str,
         "Region": str,
         "PostalCode": str,
@@ -116,19 +138,21 @@
     "_OptionalAttributeOperationTypeDef",
     {
         "AttributeValue": Mapping[str, Any],
     },
     total=False,
 )
 
+
 class AttributeOperationTypeDef(
     _RequiredAttributeOperationTypeDef, _OptionalAttributeOperationTypeDef
 ):
     pass
 
+
 MemberIdTypeDef = TypedDict(
     "MemberIdTypeDef",
     {
         "UserId": str,
     },
     total=False,
 )
@@ -153,19 +177,21 @@
     {
         "DisplayName": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
+
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "GroupId": str,
         "IdentityStoreId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -241,30 +267,79 @@
     "DescribeGroupMembershipRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MembershipId": str,
     },
 )
 
+MemberIdOutputTypeDef = TypedDict(
+    "MemberIdOutputTypeDef",
+    {
+        "UserId": str,
+    },
+    total=False,
+)
+
 DescribeGroupRequestRequestTypeDef = TypedDict(
     "DescribeGroupRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
     },
 )
 
+ExternalIdOutputTypeDef = TypedDict(
+    "ExternalIdOutputTypeDef",
+    {
+        "Issuer": str,
+        "Id": str,
+    },
+)
+
 DescribeUserRequestRequestTypeDef = TypedDict(
     "DescribeUserRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "UserId": str,
     },
 )
 
+EmailOutputTypeDef = TypedDict(
+    "EmailOutputTypeDef",
+    {
+        "Value": str,
+        "Type": str,
+        "Primary": bool,
+    },
+    total=False,
+)
+
+NameOutputTypeDef = TypedDict(
+    "NameOutputTypeDef",
+    {
+        "Formatted": str,
+        "FamilyName": str,
+        "GivenName": str,
+        "MiddleName": str,
+        "HonorificPrefix": str,
+        "HonorificSuffix": str,
+    },
+    total=False,
+)
+
+PhoneNumberOutputTypeDef = TypedDict(
+    "PhoneNumberOutputTypeDef",
+    {
+        "Value": str,
+        "Type": str,
+        "Primary": bool,
+    },
+    total=False,
+)
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "AttributePath": str,
         "AttributeValue": str,
     },
 )
@@ -307,20 +382,22 @@
     "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
     _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
     _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListGroupMembershipsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
     },
 )
@@ -329,20 +406,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListGroupMembershipsRequestRequestTypeDef(
     _RequiredListGroupMembershipsRequestRequestTypeDef,
     _OptionalListGroupMembershipsRequestRequestTypeDef,
 ):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -356,46 +435,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-DescribeGroupResponseTypeDef = TypedDict(
-    "DescribeGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "DisplayName": str,
-        "ExternalIds": List[ExternalIdTypeDef],
-        "Description": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGroupTypeDef = TypedDict(
-    "_RequiredGroupTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-    },
-)
-_OptionalGroupTypeDef = TypedDict(
-    "_OptionalGroupTypeDef",
-    {
-        "DisplayName": str,
-        "ExternalIds": List[ExternalIdTypeDef],
-        "Description": str,
-    },
-    total=False,
-)
-
-class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
-    pass
-
 AlternateIdentifierTypeDef = TypedDict(
     "AlternateIdentifierTypeDef",
     {
         "ExternalId": ExternalIdTypeDef,
         "UniqueAttribute": UniqueAttributeTypeDef,
     },
     total=False,
@@ -424,63 +471,23 @@
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
 
-DescribeGroupMembershipResponseTypeDef = TypedDict(
-    "DescribeGroupMembershipResponseTypeDef",
-    {
-        "IdentityStoreId": str,
-        "MembershipId": str,
-        "GroupId": str,
-        "MemberId": MemberIdTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetGroupMembershipIdRequestRequestTypeDef = TypedDict(
     "GetGroupMembershipIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
 
-GroupMembershipExistenceResultTypeDef = TypedDict(
-    "GroupMembershipExistenceResultTypeDef",
-    {
-        "GroupId": str,
-        "MemberId": MemberIdTypeDef,
-        "MembershipExists": bool,
-    },
-    total=False,
-)
-
-_RequiredGroupMembershipTypeDef = TypedDict(
-    "_RequiredGroupMembershipTypeDef",
-    {
-        "IdentityStoreId": str,
-    },
-)
-_OptionalGroupMembershipTypeDef = TypedDict(
-    "_OptionalGroupMembershipTypeDef",
-    {
-        "MembershipId": str,
-        "GroupId": str,
-        "MemberId": MemberIdTypeDef,
-    },
-    total=False,
-)
-
-class GroupMembershipTypeDef(_RequiredGroupMembershipTypeDef, _OptionalGroupMembershipTypeDef):
-    pass
-
 IsMemberInGroupsRequestRequestTypeDef = TypedDict(
     "IsMemberInGroupsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
         "GroupIds": Sequence[str],
     },
@@ -501,20 +508,22 @@
         {
             "PaginationConfig": "PaginatorConfigTypeDef",
         },
         total=False,
     )
 )
 
+
 class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
     _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListGroupMembershipsForMemberRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsForMemberRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
@@ -523,20 +532,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListGroupMembershipsForMemberRequestRequestTypeDef(
     _RequiredListGroupMembershipsForMemberRequestRequestTypeDef,
     _OptionalListGroupMembershipsForMemberRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalCreateUserRequestRequestTypeDef = TypedDict(
@@ -555,32 +566,110 @@
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
     },
     total=False,
 )
 
+
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+
+DescribeGroupMembershipResponseTypeDef = TypedDict(
+    "DescribeGroupMembershipResponseTypeDef",
+    {
+        "IdentityStoreId": str,
+        "MembershipId": str,
+        "GroupId": str,
+        "MemberId": MemberIdOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GroupMembershipExistenceResultTypeDef = TypedDict(
+    "GroupMembershipExistenceResultTypeDef",
+    {
+        "GroupId": str,
+        "MemberId": MemberIdOutputTypeDef,
+        "MembershipExists": bool,
+    },
+    total=False,
+)
+
+_RequiredGroupMembershipTypeDef = TypedDict(
+    "_RequiredGroupMembershipTypeDef",
+    {
+        "IdentityStoreId": str,
+    },
+)
+_OptionalGroupMembershipTypeDef = TypedDict(
+    "_OptionalGroupMembershipTypeDef",
+    {
+        "MembershipId": str,
+        "GroupId": str,
+        "MemberId": MemberIdOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class GroupMembershipTypeDef(_RequiredGroupMembershipTypeDef, _OptionalGroupMembershipTypeDef):
+    pass
+
+
+DescribeGroupResponseTypeDef = TypedDict(
+    "DescribeGroupResponseTypeDef",
+    {
+        "GroupId": str,
+        "DisplayName": str,
+        "ExternalIds": List[ExternalIdOutputTypeDef],
+        "Description": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGroupTypeDef = TypedDict(
+    "_RequiredGroupTypeDef",
+    {
+        "GroupId": str,
+        "IdentityStoreId": str,
+    },
+)
+_OptionalGroupTypeDef = TypedDict(
+    "_OptionalGroupTypeDef",
+    {
+        "DisplayName": str,
+        "ExternalIds": List[ExternalIdOutputTypeDef],
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
+    pass
+
+
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "UserName": str,
         "UserId": str,
-        "ExternalIds": List[ExternalIdTypeDef],
-        "Name": NameTypeDef,
+        "ExternalIds": List[ExternalIdOutputTypeDef],
+        "Name": NameOutputTypeDef,
         "DisplayName": str,
         "NickName": str,
         "ProfileUrl": str,
-        "Emails": List[EmailTypeDef],
-        "Addresses": List[AddressTypeDef],
-        "PhoneNumbers": List[PhoneNumberTypeDef],
+        "Emails": List[EmailOutputTypeDef],
+        "Addresses": List[AddressOutputTypeDef],
+        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
         "UserType": str,
         "Title": str,
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
         "IdentityStoreId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -594,34 +683,36 @@
         "IdentityStoreId": str,
     },
 )
 _OptionalUserTypeDef = TypedDict(
     "_OptionalUserTypeDef",
     {
         "UserName": str,
-        "ExternalIds": List[ExternalIdTypeDef],
-        "Name": NameTypeDef,
+        "ExternalIds": List[ExternalIdOutputTypeDef],
+        "Name": NameOutputTypeDef,
         "DisplayName": str,
         "NickName": str,
         "ProfileUrl": str,
-        "Emails": List[EmailTypeDef],
-        "Addresses": List[AddressTypeDef],
-        "PhoneNumbers": List[PhoneNumberTypeDef],
+        "Emails": List[EmailOutputTypeDef],
+        "Addresses": List[AddressOutputTypeDef],
+        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
         "UserType": str,
         "Title": str,
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
     },
     total=False,
 )
 
+
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
+
 _RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
     "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
@@ -629,20 +720,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListGroupsRequestListGroupsPaginateTypeDef(
     _RequiredListGroupsRequestListGroupsPaginateTypeDef,
     _OptionalListGroupsRequestListGroupsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalListGroupsRequestRequestTypeDef = TypedDict(
@@ -651,19 +744,21 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+
 class ListGroupsRequestRequestTypeDef(
     _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
@@ -671,20 +766,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -693,27 +790,20 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-ListGroupsResponseTypeDef = TypedDict(
-    "ListGroupsResponseTypeDef",
-    {
-        "Groups": List[GroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetGroupIdRequestRequestTypeDef = TypedDict(
     "GetGroupIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "AlternateIdentifier": AlternateIdentifierTypeDef,
     },
@@ -749,14 +839,23 @@
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListGroupsResponseTypeDef = TypedDict(
+    "ListGroupsResponseTypeDef",
+    {
+        "Groups": List[GroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore.egg-info/PKG-INFO` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-identitystore
-Version: 1.28.0
-Summary: Type annotations for boto3.IdentityStore 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IdentityStore 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-identitystore"></a>
 
 # mypy-boto3-identitystore
 
 [![PyPI - mypy-boto3-identitystore](https://img.shields.io/pypi/v/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-identitystore?color=blue)](https://pypistats.org/packages/mypy-boto3-identitystore)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-identitystore)](https://pepy.tech/project/mypy-boto3-identitystore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IdentityStore 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
+[boto3.IdentityStore 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
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
 [mypy-boto3-identitystore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,14 +334,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_identitystore.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_identitystore.type_defs import (
+    AddressOutputTypeDef,
     AddressTypeDef,
     ExternalIdTypeDef,
     UniqueAttributeTypeDef,
     AttributeOperationTypeDef,
     MemberIdTypeDef,
     CreateGroupMembershipResponseTypeDef,
     CreateGroupRequestRequestTypeDef,
@@ -350,55 +351,60 @@
     NameTypeDef,
     PhoneNumberTypeDef,
     CreateUserResponseTypeDef,
     DeleteGroupMembershipRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeGroupMembershipRequestRequestTypeDef,
+    MemberIdOutputTypeDef,
     DescribeGroupRequestRequestTypeDef,
+    ExternalIdOutputTypeDef,
     DescribeUserRequestRequestTypeDef,
+    EmailOutputTypeDef,
+    NameOutputTypeDef,
+    PhoneNumberOutputTypeDef,
     FilterTypeDef,
     GetGroupIdResponseTypeDef,
     GetGroupMembershipIdResponseTypeDef,
     GetUserIdResponseTypeDef,
     ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
     ListGroupMembershipsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
-    DescribeGroupResponseTypeDef,
-    GroupTypeDef,
     AlternateIdentifierTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
-    DescribeGroupMembershipResponseTypeDef,
     GetGroupMembershipIdRequestRequestTypeDef,
-    GroupMembershipExistenceResultTypeDef,
-    GroupMembershipTypeDef,
     IsMemberInGroupsRequestRequestTypeDef,
     ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     ListGroupMembershipsForMemberRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
+    DescribeGroupMembershipResponseTypeDef,
+    GroupMembershipExistenceResultTypeDef,
+    GroupMembershipTypeDef,
+    DescribeGroupResponseTypeDef,
+    GroupTypeDef,
     DescribeUserResponseTypeDef,
     UserTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
-    ListGroupsResponseTypeDef,
     GetGroupIdRequestRequestTypeDef,
     GetUserIdRequestRequestTypeDef,
     IsMemberInGroupsResponseTypeDef,
     ListGroupMembershipsForMemberResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
+    ListGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
 )
 
 
-def get_structure() -> AddressTypeDef:
+def get_structure() -> AddressOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-identitystore-1.28.0/mypy_boto3_identitystore.egg-info/SOURCES.txt` & `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.0/setup.py` & `mypy-boto3-identitystore-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-identitystore",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_identitystore"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IdentityStore 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.IdentityStore 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

