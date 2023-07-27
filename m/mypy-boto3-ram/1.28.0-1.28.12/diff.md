# Comparing `tmp/mypy-boto3-ram-1.28.0.tar.gz` & `tmp/mypy-boto3-ram-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ram-1.28.0.tar", last modified: Thu Jul  6 21:00:22 2023, max compression
+gzip compressed data, was "mypy-boto3-ram-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
```

## Comparing `mypy-boto3-ram-1.28.0.tar` & `mypy-boto3-ram-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:22.902401 mypy-boto3-ram-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-07-06 21:00:22.898401 mypy-boto3-ram-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:22.894401 mypy-boto3-ram-1.28.0/mypy_boto3_ram/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31754 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31707 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-06 20:52:23.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41071 2023-07-06 20:52:24.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41006 2023-07-06 20:52:23.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:22.898401 mypy-boto3-ram-1.28.0/mypy_boto3_ram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-07-06 21:00:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 21:00:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:22.000000 mypy-boto3-ram-1.28.0/mypy_boto3_ram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:22.902401 mypy-boto3-ram-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:52:22.000000 mypy-boto3-ram-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.593188 mypy-boto3-ram-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17668 2023-07-27 11:49:27.581188 mypy-boto3-ram-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.577188 mypy-boto3-ram-1.28.12/mypy_boto3_ram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-07-27 11:43:55.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31821 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-07-27 11:43:56.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-27 11:43:56.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-07-27 11:43:55.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-27 11:43:55.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41268 2023-07-27 11:43:57.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41203 2023-07-27 11:43:56.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.581188 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17668 2023-07-27 11:49:27.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:27.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:27.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.593188 mypy-boto3-ram-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/setup.py
```

### Comparing `mypy-boto3-ram-1.28.0/LICENSE` & `mypy-boto3-ram-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.0/PKG-INFO` & `mypy-boto3-ram-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ram
-Version: 1.28.0
-Summary: Type annotations for boto3.RAM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.RAM 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ram"></a>
 
 # mypy-boto3-ram
 
 [![PyPI - mypy-boto3-ram](https://img.shields.io/pypi/v/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ram?color=blue)](https://pypistats.org/packages/mypy-boto3-ram)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ram)](https://pepy.tech/project/mypy-boto3-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RAM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[boto3.RAM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
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
 [mypy-boto3-ram docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,85 +357,86 @@
 
 `mypy_boto3_ram.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ram.type_defs import (
     AcceptResourceShareInvitationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AssociateResourceSharePermissionRequestRequestTypeDef,
-    AssociateResourceSharePermissionResponseTypeDef,
     AssociateResourceShareRequestRequestTypeDef,
     ResourceShareAssociationTypeDef,
     AssociatedPermissionTypeDef,
     TagTypeDef,
     CreatePermissionVersionRequestRequestTypeDef,
     DeletePermissionRequestRequestTypeDef,
-    DeletePermissionResponseTypeDef,
     DeletePermissionVersionRequestRequestTypeDef,
-    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareRequestRequestTypeDef,
-    DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionRequestRequestTypeDef,
-    DisassociateResourceSharePermissionResponseTypeDef,
     DisassociateResourceShareRequestRequestTypeDef,
-    EnableSharingWithAwsOrganizationResponseTypeDef,
     GetPermissionRequestRequestTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
-    GetResourcePoliciesResponseTypeDef,
-    GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
     GetResourceShareAssociationsRequestRequestTypeDef,
-    GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
     GetResourceShareInvitationsRequestRequestTypeDef,
     TagFilterTypeDef,
     ListPendingInvitationResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListPermissionAssociationsRequestRequestTypeDef,
     ListPermissionVersionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
-    ListPrincipalsRequestListPrincipalsPaginateTypeDef,
     ListPrincipalsRequestRequestTypeDef,
     PrincipalTypeDef,
     ListReplacePermissionAssociationsWorkRequestRequestTypeDef,
     ReplacePermissionAssociationsWorkTypeDef,
     ListResourceSharePermissionsRequestRequestTypeDef,
     ListResourceTypesRequestRequestTypeDef,
     ServiceNameAndResourceTypeTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef,
-    PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     RejectResourceShareInvitationRequestRequestTypeDef,
     ReplacePermissionAssociationsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     SetDefaultPermissionVersionRequestRequestTypeDef,
-    SetDefaultPermissionVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateResourceShareRequestRequestTypeDef,
+    AssociateResourceSharePermissionResponseTypeDef,
+    DeletePermissionResponseTypeDef,
+    DeletePermissionVersionResponseTypeDef,
+    DeleteResourceShareResponseTypeDef,
+    DisassociateResourceSharePermissionResponseTypeDef,
+    EnableSharingWithAwsOrganizationResponseTypeDef,
+    GetResourcePoliciesResponseTypeDef,
+    PromoteResourceShareCreatedFromPolicyResponseTypeDef,
+    SetDefaultPermissionVersionResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     ResourceShareInvitationTypeDef,
     ListPermissionAssociationsResponseTypeDef,
     CreatePermissionRequestRequestTypeDef,
     CreateResourceShareRequestRequestTypeDef,
-    ResourceSharePermissionDetailTypeDef,
-    ResourceSharePermissionSummaryTypeDef,
-    ResourceShareTypeDef,
     TagResourceRequestRequestTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
+    GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
+    ListPrincipalsRequestListPrincipalsPaginateTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
     GetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     GetResourceSharesRequestRequestTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListPrincipalsResponseTypeDef,
     ListReplacePermissionAssociationsWorkResponseTypeDef,
     ReplacePermissionAssociationsResponseTypeDef,
     ListResourceTypesResponseTypeDef,
+    ResourceSharePermissionDetailTypeDef,
+    ResourceSharePermissionSummaryTypeDef,
+    ResourceShareTypeDef,
     AcceptResourceShareInvitationResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
     CreatePermissionVersionResponseTypeDef,
     GetPermissionResponseTypeDef,
     CreatePermissionResponseTypeDef,
     ListPermissionVersionsResponseTypeDef,
```

### Comparing `mypy-boto3-ram-1.28.0/README.md` & `mypy-boto3-ram-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ram"></a>
 
 # mypy-boto3-ram
 
 [![PyPI - mypy-boto3-ram](https://img.shields.io/pypi/v/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ram?color=blue)](https://pypistats.org/packages/mypy-boto3-ram)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ram)](https://pepy.tech/project/mypy-boto3-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RAM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[boto3.RAM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
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
 [mypy-boto3-ram docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,85 +325,86 @@
 
 `mypy_boto3_ram.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ram.type_defs import (
     AcceptResourceShareInvitationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AssociateResourceSharePermissionRequestRequestTypeDef,
-    AssociateResourceSharePermissionResponseTypeDef,
     AssociateResourceShareRequestRequestTypeDef,
     ResourceShareAssociationTypeDef,
     AssociatedPermissionTypeDef,
     TagTypeDef,
     CreatePermissionVersionRequestRequestTypeDef,
     DeletePermissionRequestRequestTypeDef,
-    DeletePermissionResponseTypeDef,
     DeletePermissionVersionRequestRequestTypeDef,
-    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareRequestRequestTypeDef,
-    DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionRequestRequestTypeDef,
-    DisassociateResourceSharePermissionResponseTypeDef,
     DisassociateResourceShareRequestRequestTypeDef,
-    EnableSharingWithAwsOrganizationResponseTypeDef,
     GetPermissionRequestRequestTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
-    GetResourcePoliciesResponseTypeDef,
-    GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
     GetResourceShareAssociationsRequestRequestTypeDef,
-    GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
     GetResourceShareInvitationsRequestRequestTypeDef,
     TagFilterTypeDef,
     ListPendingInvitationResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListPermissionAssociationsRequestRequestTypeDef,
     ListPermissionVersionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
-    ListPrincipalsRequestListPrincipalsPaginateTypeDef,
     ListPrincipalsRequestRequestTypeDef,
     PrincipalTypeDef,
     ListReplacePermissionAssociationsWorkRequestRequestTypeDef,
     ReplacePermissionAssociationsWorkTypeDef,
     ListResourceSharePermissionsRequestRequestTypeDef,
     ListResourceTypesRequestRequestTypeDef,
     ServiceNameAndResourceTypeTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef,
-    PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     RejectResourceShareInvitationRequestRequestTypeDef,
     ReplacePermissionAssociationsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     SetDefaultPermissionVersionRequestRequestTypeDef,
-    SetDefaultPermissionVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateResourceShareRequestRequestTypeDef,
+    AssociateResourceSharePermissionResponseTypeDef,
+    DeletePermissionResponseTypeDef,
+    DeletePermissionVersionResponseTypeDef,
+    DeleteResourceShareResponseTypeDef,
+    DisassociateResourceSharePermissionResponseTypeDef,
+    EnableSharingWithAwsOrganizationResponseTypeDef,
+    GetResourcePoliciesResponseTypeDef,
+    PromoteResourceShareCreatedFromPolicyResponseTypeDef,
+    SetDefaultPermissionVersionResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     ResourceShareInvitationTypeDef,
     ListPermissionAssociationsResponseTypeDef,
     CreatePermissionRequestRequestTypeDef,
     CreateResourceShareRequestRequestTypeDef,
-    ResourceSharePermissionDetailTypeDef,
-    ResourceSharePermissionSummaryTypeDef,
-    ResourceShareTypeDef,
     TagResourceRequestRequestTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
+    GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
+    ListPrincipalsRequestListPrincipalsPaginateTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
     GetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     GetResourceSharesRequestRequestTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListPrincipalsResponseTypeDef,
     ListReplacePermissionAssociationsWorkResponseTypeDef,
     ReplacePermissionAssociationsResponseTypeDef,
     ListResourceTypesResponseTypeDef,
+    ResourceSharePermissionDetailTypeDef,
+    ResourceSharePermissionSummaryTypeDef,
+    ResourceShareTypeDef,
     AcceptResourceShareInvitationResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
     CreatePermissionVersionResponseTypeDef,
     GetPermissionResponseTypeDef,
     CreatePermissionResponseTypeDef,
     ListPermissionVersionsResponseTypeDef,
```

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram/__init__.py` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram/__init__.pyi` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram/__main__.py` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RAM 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.RAM 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM\nOther"
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

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram/client.py` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,16 @@
 
     def associate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
+        sources: Sequence[str] = ...
     ) -> AssociateResourceShareResponseTypeDef:
         """
         Adds the specified list of principals and list of resources to a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#associate_resource_share)
         """
@@ -230,15 +231,16 @@
         *,
         name: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
         allowExternalPrincipals: bool = ...,
         clientToken: str = ...,
-        permissionArns: Sequence[str] = ...
+        permissionArns: Sequence[str] = ...,
+        sources: Sequence[str] = ...
     ) -> CreateResourceShareResponseTypeDef:
         """
         Creates a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_resource_share)
         """
@@ -276,15 +278,16 @@
 
     def disassociate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
+        sources: Sequence[str] = ...
     ) -> DisassociateResourceShareResponseTypeDef:
         """
         Removes the specified principals or resources from participating in the
         specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#disassociate_resource_share)
```

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram/client.pyi` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,16 @@
         """
     def associate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
+        sources: Sequence[str] = ...
     ) -> AssociateResourceShareResponseTypeDef:
         """
         Adds the specified list of principals and list of resources to a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#associate_resource_share)
         """
@@ -218,15 +219,16 @@
         *,
         name: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
         allowExternalPrincipals: bool = ...,
         clientToken: str = ...,
-        permissionArns: Sequence[str] = ...
+        permissionArns: Sequence[str] = ...,
+        sources: Sequence[str] = ...
     ) -> CreateResourceShareResponseTypeDef:
         """
         Creates a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#create_resource_share)
         """
@@ -260,15 +262,16 @@
         """
     def disassociate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
+        sources: Sequence[str] = ...
     ) -> DisassociateResourceShareResponseTypeDef:
         """
         Removes the specified principals or resources from participating in the
         specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/client/#disassociate_resource_share)
```

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram/literals.py` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,15 @@
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
@@ -274,26 +275,28 @@
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

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram/literals.pyi` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,15 @@
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
@@ -272,26 +273,28 @@
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

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram/paginator.py` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceArns: Sequence[str],
         principal: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourcepoliciespaginator)
         """
 
 
@@ -100,15 +100,15 @@
         self,
         *,
         associationType: ResourceShareAssociationTypeType,
         resourceShareArns: Sequence[str] = ...,
         resourceArn: str = ...,
         principal: str = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceShareAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShareAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourceshareassociationspaginator)
         """
 
 
@@ -119,15 +119,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceShareInvitationArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceShareInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShareInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourceshareinvitationspaginator)
         """
 
 
@@ -143,15 +143,15 @@
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         permissionArn: str = ...,
         permissionVersion: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceSharesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourcesharespaginator)
         """
 
 
@@ -165,15 +165,15 @@
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceArn: str = ...,
         principals: Sequence[str] = ...,
         resourceType: str = ...,
         resourceShareArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.ListPrincipals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#listprincipalspaginator)
         """
 
 
@@ -188,13 +188,13 @@
         *,
         resourceOwner: ResourceOwnerType,
         principal: str = ...,
         resourceType: str = ...,
         resourceArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#listresourcespaginator)
         """
```

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram/paginator.pyi` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceArns: Sequence[str],
         principal: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourcepoliciespaginator)
         """
 
 class GetResourceShareAssociationsPaginator(Paginator):
@@ -96,15 +96,15 @@
         self,
         *,
         associationType: ResourceShareAssociationTypeType,
         resourceShareArns: Sequence[str] = ...,
         resourceArn: str = ...,
         principal: str = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceShareAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShareAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourceshareassociationspaginator)
         """
 
 class GetResourceShareInvitationsPaginator(Paginator):
@@ -114,15 +114,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceShareInvitationArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceShareInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShareInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourceshareinvitationspaginator)
         """
 
 class GetResourceSharesPaginator(Paginator):
@@ -137,15 +137,15 @@
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         permissionArn: str = ...,
         permissionVersion: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourceSharesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#getresourcesharespaginator)
         """
 
 class ListPrincipalsPaginator(Paginator):
@@ -158,15 +158,15 @@
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceArn: str = ...,
         principals: Sequence[str] = ...,
         resourceType: str = ...,
         resourceShareArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.ListPrincipals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#listprincipalspaginator)
         """
 
 class ListResourcesPaginator(Paginator):
@@ -180,13 +180,13 @@
         *,
         resourceOwner: ResourceOwnerType,
         principal: str = ...,
         resourceType: str = ...,
         resourceArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/paginators/#listresourcespaginator)
         """
```

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram/type_defs.py` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -33,88 +33,88 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptResourceShareInvitationRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateResourceSharePermissionRequestRequestTypeDef",
-    "AssociateResourceSharePermissionResponseTypeDef",
     "AssociateResourceShareRequestRequestTypeDef",
     "ResourceShareAssociationTypeDef",
     "AssociatedPermissionTypeDef",
     "TagTypeDef",
     "CreatePermissionVersionRequestRequestTypeDef",
     "DeletePermissionRequestRequestTypeDef",
-    "DeletePermissionResponseTypeDef",
     "DeletePermissionVersionRequestRequestTypeDef",
-    "DeletePermissionVersionResponseTypeDef",
     "DeleteResourceShareRequestRequestTypeDef",
-    "DeleteResourceShareResponseTypeDef",
     "DisassociateResourceSharePermissionRequestRequestTypeDef",
-    "DisassociateResourceSharePermissionResponseTypeDef",
     "DisassociateResourceShareRequestRequestTypeDef",
-    "EnableSharingWithAwsOrganizationResponseTypeDef",
     "GetPermissionRequestRequestTypeDef",
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
-    "GetResourcePoliciesResponseTypeDef",
-    "GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
     "GetResourceShareAssociationsRequestRequestTypeDef",
-    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
     "GetResourceShareInvitationsRequestRequestTypeDef",
     "TagFilterTypeDef",
     "ListPendingInvitationResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListPermissionAssociationsRequestRequestTypeDef",
     "ListPermissionVersionsRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
-    "ListPrincipalsRequestListPrincipalsPaginateTypeDef",
     "ListPrincipalsRequestRequestTypeDef",
     "PrincipalTypeDef",
     "ListReplacePermissionAssociationsWorkRequestRequestTypeDef",
     "ReplacePermissionAssociationsWorkTypeDef",
     "ListResourceSharePermissionsRequestRequestTypeDef",
     "ListResourceTypesRequestRequestTypeDef",
     "ServiceNameAndResourceTypeTypeDef",
-    "ListResourcesRequestListResourcesPaginateTypeDef",
     "ListResourcesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PromotePermissionCreatedFromPolicyRequestRequestTypeDef",
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
-    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
     "RejectResourceShareInvitationRequestRequestTypeDef",
     "ReplacePermissionAssociationsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "SetDefaultPermissionVersionRequestRequestTypeDef",
-    "SetDefaultPermissionVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateResourceShareRequestRequestTypeDef",
+    "AssociateResourceSharePermissionResponseTypeDef",
+    "DeletePermissionResponseTypeDef",
+    "DeletePermissionVersionResponseTypeDef",
+    "DeleteResourceShareResponseTypeDef",
+    "DisassociateResourceSharePermissionResponseTypeDef",
+    "EnableSharingWithAwsOrganizationResponseTypeDef",
+    "GetResourcePoliciesResponseTypeDef",
+    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
+    "SetDefaultPermissionVersionResponseTypeDef",
     "AssociateResourceShareResponseTypeDef",
     "DisassociateResourceShareResponseTypeDef",
     "GetResourceShareAssociationsResponseTypeDef",
     "ResourceShareInvitationTypeDef",
     "ListPermissionAssociationsResponseTypeDef",
     "CreatePermissionRequestRequestTypeDef",
     "CreateResourceShareRequestRequestTypeDef",
-    "ResourceSharePermissionDetailTypeDef",
-    "ResourceSharePermissionSummaryTypeDef",
-    "ResourceShareTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    "GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
+    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
+    "ListPrincipalsRequestListPrincipalsPaginateTypeDef",
+    "ListResourcesRequestListResourcesPaginateTypeDef",
     "GetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     "GetResourceSharesRequestRequestTypeDef",
     "ListPendingInvitationResourcesResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "ListPrincipalsResponseTypeDef",
     "ListReplacePermissionAssociationsWorkResponseTypeDef",
     "ReplacePermissionAssociationsResponseTypeDef",
     "ListResourceTypesResponseTypeDef",
+    "ResourceSharePermissionDetailTypeDef",
+    "ResourceSharePermissionSummaryTypeDef",
+    "ResourceShareTypeDef",
     "AcceptResourceShareInvitationResponseTypeDef",
     "GetResourceShareInvitationsResponseTypeDef",
     "RejectResourceShareInvitationResponseTypeDef",
     "CreatePermissionVersionResponseTypeDef",
     "GetPermissionResponseTypeDef",
     "CreatePermissionResponseTypeDef",
     "ListPermissionVersionsResponseTypeDef",
@@ -136,21 +136,30 @@
     "_OptionalAcceptResourceShareInvitationRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class AcceptResourceShareInvitationRequestRequestTypeDef(
     _RequiredAcceptResourceShareInvitationRequestRequestTypeDef,
     _OptionalAcceptResourceShareInvitationRequestRequestTypeDef,
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
 
 _RequiredAssociateResourceSharePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateResourceSharePermissionRequestRequestTypeDef",
     {
         "resourceShareArn": str,
         "permissionArn": str,
     },
@@ -161,55 +170,43 @@
         "replace": bool,
         "clientToken": str,
         "permissionVersion": int,
     },
     total=False,
 )
 
-
 class AssociateResourceSharePermissionRequestRequestTypeDef(
     _RequiredAssociateResourceSharePermissionRequestRequestTypeDef,
     _OptionalAssociateResourceSharePermissionRequestRequestTypeDef,
 ):
     pass
 
-
-AssociateResourceSharePermissionResponseTypeDef = TypedDict(
-    "AssociateResourceSharePermissionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssociateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalAssociateResourceShareRequestRequestTypeDef = TypedDict(
     "_OptionalAssociateResourceShareRequestRequestTypeDef",
     {
         "resourceArns": Sequence[str],
         "principals": Sequence[str],
         "clientToken": str,
+        "sources": Sequence[str],
     },
     total=False,
 )
 
-
 class AssociateResourceShareRequestRequestTypeDef(
     _RequiredAssociateResourceShareRequestRequestTypeDef,
     _OptionalAssociateResourceShareRequestRequestTypeDef,
 ):
     pass
 
-
 ResourceShareAssociationTypeDef = TypedDict(
     "ResourceShareAssociationTypeDef",
     {
         "resourceShareArn": str,
         "resourceShareName": str,
         "associatedEntity": str,
         "associationType": ResourceShareAssociationTypeType,
@@ -257,53 +254,39 @@
     "_OptionalCreatePermissionVersionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreatePermissionVersionRequestRequestTypeDef(
     _RequiredCreatePermissionVersionRequestRequestTypeDef,
     _OptionalCreatePermissionVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeletePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePermissionRequestRequestTypeDef",
     {
         "permissionArn": str,
     },
 )
 _OptionalDeletePermissionRequestRequestTypeDef = TypedDict(
     "_OptionalDeletePermissionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeletePermissionRequestRequestTypeDef(
     _RequiredDeletePermissionRequestRequestTypeDef, _OptionalDeletePermissionRequestRequestTypeDef
 ):
     pass
 
-
-DeletePermissionResponseTypeDef = TypedDict(
-    "DeletePermissionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "permissionStatus": PermissionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeletePermissionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePermissionVersionRequestRequestTypeDef",
     {
         "permissionArn": str,
         "permissionVersion": int,
     },
 )
@@ -311,63 +294,40 @@
     "_OptionalDeletePermissionVersionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeletePermissionVersionRequestRequestTypeDef(
     _RequiredDeletePermissionVersionRequestRequestTypeDef,
     _OptionalDeletePermissionVersionRequestRequestTypeDef,
 ):
     pass
 
-
-DeletePermissionVersionResponseTypeDef = TypedDict(
-    "DeletePermissionVersionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "permissionStatus": PermissionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalDeleteResourceShareRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteResourceShareRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteResourceShareRequestRequestTypeDef(
     _RequiredDeleteResourceShareRequestRequestTypeDef,
     _OptionalDeleteResourceShareRequestRequestTypeDef,
 ):
     pass
 
-
-DeleteResourceShareResponseTypeDef = TypedDict(
-    "DeleteResourceShareResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisassociateResourceSharePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateResourceSharePermissionRequestRequestTypeDef",
     {
         "resourceShareArn": str,
         "permissionArn": str,
     },
 )
@@ -375,107 +335,72 @@
     "_OptionalDisassociateResourceSharePermissionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DisassociateResourceSharePermissionRequestRequestTypeDef(
     _RequiredDisassociateResourceSharePermissionRequestRequestTypeDef,
     _OptionalDisassociateResourceSharePermissionRequestRequestTypeDef,
 ):
     pass
 
-
-DisassociateResourceSharePermissionResponseTypeDef = TypedDict(
-    "DisassociateResourceSharePermissionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisassociateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalDisassociateResourceShareRequestRequestTypeDef = TypedDict(
     "_OptionalDisassociateResourceShareRequestRequestTypeDef",
     {
         "resourceArns": Sequence[str],
         "principals": Sequence[str],
         "clientToken": str,
+        "sources": Sequence[str],
     },
     total=False,
 )
 
-
 class DisassociateResourceShareRequestRequestTypeDef(
     _RequiredDisassociateResourceShareRequestRequestTypeDef,
     _OptionalDisassociateResourceShareRequestRequestTypeDef,
 ):
     pass
 
-
-EnableSharingWithAwsOrganizationResponseTypeDef = TypedDict(
-    "EnableSharingWithAwsOrganizationResponseTypeDef",
-    {
-        "returnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredGetPermissionRequestRequestTypeDef",
     {
         "permissionArn": str,
     },
 )
 _OptionalGetPermissionRequestRequestTypeDef = TypedDict(
     "_OptionalGetPermissionRequestRequestTypeDef",
     {
         "permissionVersion": int,
     },
     total=False,
 )
 
-
 class GetPermissionRequestRequestTypeDef(
     _RequiredGetPermissionRequestRequestTypeDef, _OptionalGetPermissionRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "resourceArns": Sequence[str],
-    },
-)
-_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "principal": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "resourceArns": Sequence[str],
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -484,57 +409,20 @@
         "principal": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetResourcePoliciesRequestRequestTypeDef(
     _RequiredGetResourcePoliciesRequestRequestTypeDef,
     _OptionalGetResourcePoliciesRequestRequestTypeDef,
 ):
     pass
 
-
-GetResourcePoliciesResponseTypeDef = TypedDict(
-    "GetResourcePoliciesResponseTypeDef",
-    {
-        "policies": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
-    {
-        "associationType": ResourceShareAssociationTypeType,
-    },
-)
-_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
-    {
-        "resourceShareArns": Sequence[str],
-        "resourceArn": str,
-        "principal": str,
-        "associationStatus": ResourceShareAssociationStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef(
-    _RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
-    _OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetResourceShareAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceShareAssociationsRequestRequestTypeDef",
     {
         "associationType": ResourceShareAssociationTypeType,
     },
 )
 _OptionalGetResourceShareAssociationsRequestRequestTypeDef = TypedDict(
@@ -546,32 +434,20 @@
         "associationStatus": ResourceShareAssociationStatusType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetResourceShareAssociationsRequestRequestTypeDef(
     _RequiredGetResourceShareAssociationsRequestRequestTypeDef,
     _OptionalGetResourceShareAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
-GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef = TypedDict(
-    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
-    {
-        "resourceShareInvitationArns": Sequence[str],
-        "resourceShareArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetResourceShareInvitationsRequestRequestTypeDef = TypedDict(
     "GetResourceShareInvitationsRequestRequestTypeDef",
     {
         "resourceShareInvitationArns": Sequence[str],
         "resourceShareArns": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -600,22 +476,20 @@
         "nextToken": str,
         "maxResults": int,
         "resourceRegionScope": ResourceRegionScopeFilterType,
     },
     total=False,
 )
 
-
 class ListPendingInvitationResourcesRequestRequestTypeDef(
     _RequiredListPendingInvitationResourcesRequestRequestTypeDef,
     _OptionalListPendingInvitationResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "arn": str,
         "type": str,
         "resourceShareArn": str,
         "resourceGroupArn": str,
@@ -654,59 +528,31 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListPermissionVersionsRequestRequestTypeDef(
     _RequiredListPermissionVersionsRequestRequestTypeDef,
     _OptionalListPermissionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListPermissionsRequestRequestTypeDef = TypedDict(
     "ListPermissionsRequestRequestTypeDef",
     {
         "resourceType": str,
         "nextToken": str,
         "maxResults": int,
         "permissionType": PermissionTypeFilterType,
     },
     total=False,
 )
 
-_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef",
-    {
-        "resourceOwner": ResourceOwnerType,
-    },
-)
-_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef",
-    {
-        "resourceArn": str,
-        "principals": Sequence[str],
-        "resourceType": str,
-        "resourceShareArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPrincipalsRequestListPrincipalsPaginateTypeDef(
-    _RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef,
-    _OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalsRequestRequestTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
     },
 )
 _OptionalListPrincipalsRequestRequestTypeDef = TypedDict(
@@ -718,21 +564,19 @@
         "resourceShareArns": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListPrincipalsRequestRequestTypeDef(
     _RequiredListPrincipalsRequestRequestTypeDef, _OptionalListPrincipalsRequestRequestTypeDef
 ):
     pass
 
-
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
         "id": str,
         "resourceShareArn": str,
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
@@ -779,22 +623,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListResourceSharePermissionsRequestRequestTypeDef(
     _RequiredListResourceSharePermissionsRequestRequestTypeDef,
     _OptionalListResourceSharePermissionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListResourceTypesRequestRequestTypeDef = TypedDict(
     "ListResourceTypesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "resourceRegionScope": ResourceRegionScopeFilterType,
     },
@@ -807,41 +649,14 @@
         "resourceType": str,
         "serviceName": str,
         "resourceRegionScope": ResourceRegionScopeType,
     },
     total=False,
 )
 
-_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "resourceOwner": ResourceOwnerType,
-    },
-)
-_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "principal": str,
-        "resourceType": str,
-        "resourceArns": Sequence[str],
-        "resourceShareArns": Sequence[str],
-        "resourceRegionScope": ResourceRegionScopeFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourcesRequestListResourcesPaginateTypeDef(
-    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
-    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -854,31 +669,19 @@
         "nextToken": str,
         "maxResults": int,
         "resourceRegionScope": ResourceRegionScopeFilterType,
     },
     total=False,
 )
 
-
 class ListResourcesRequestRequestTypeDef(
     _RequiredListResourcesRequestRequestTypeDef, _OptionalListResourcesRequestRequestTypeDef
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
 _RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef",
     {
         "permissionArn": str,
         "name": str,
     },
 )
@@ -886,59 +689,47 @@
     "_OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class PromotePermissionCreatedFromPolicyRequestRequestTypeDef(
     _RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     _OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef = TypedDict(
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 
-PromoteResourceShareCreatedFromPolicyResponseTypeDef = TypedDict(
-    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
-    {
-        "returnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRejectResourceShareInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredRejectResourceShareInvitationRequestRequestTypeDef",
     {
         "resourceShareInvitationArn": str,
     },
 )
 _OptionalRejectResourceShareInvitationRequestRequestTypeDef = TypedDict(
     "_OptionalRejectResourceShareInvitationRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class RejectResourceShareInvitationRequestRequestTypeDef(
     _RequiredRejectResourceShareInvitationRequestRequestTypeDef,
     _OptionalRejectResourceShareInvitationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredReplacePermissionAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredReplacePermissionAssociationsRequestRequestTypeDef",
     {
         "fromPermissionArn": str,
         "toPermissionArn": str,
     },
 )
@@ -947,31 +738,27 @@
     {
         "fromPermissionVersion": int,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class ReplacePermissionAssociationsRequestRequestTypeDef(
     _RequiredReplacePermissionAssociationsRequestRequestTypeDef,
     _OptionalReplacePermissionAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "key": str,
+        "value": str,
     },
+    total=False,
 )
 
 _RequiredSetDefaultPermissionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredSetDefaultPermissionVersionRequestRequestTypeDef",
     {
         "permissionArn": str,
         "permissionVersion": int,
@@ -981,31 +768,20 @@
     "_OptionalSetDefaultPermissionVersionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class SetDefaultPermissionVersionRequestRequestTypeDef(
     _RequiredSetDefaultPermissionVersionRequestRequestTypeDef,
     _OptionalSetDefaultPermissionVersionRequestRequestTypeDef,
 ):
     pass
 
-
-SetDefaultPermissionVersionResponseTypeDef = TypedDict(
-    "SetDefaultPermissionVersionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUntagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUntagResourceRequestRequestTypeDef",
     {
         "tagKeys": Sequence[str],
     },
 )
 _OptionalUntagResourceRequestRequestTypeDef = TypedDict(
@@ -1013,21 +789,19 @@
     {
         "resourceShareArn": str,
         "resourceArn": str,
     },
     total=False,
 )
 
-
 class UntagResourceRequestRequestTypeDef(
     _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalUpdateResourceShareRequestRequestTypeDef = TypedDict(
@@ -1036,46 +810,125 @@
         "name": str,
         "allowExternalPrincipals": bool,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateResourceShareRequestRequestTypeDef(
     _RequiredUpdateResourceShareRequestRequestTypeDef,
     _OptionalUpdateResourceShareRequestRequestTypeDef,
 ):
     pass
 
+AssociateResourceSharePermissionResponseTypeDef = TypedDict(
+    "AssociateResourceSharePermissionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePermissionResponseTypeDef = TypedDict(
+    "DeletePermissionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "permissionStatus": PermissionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePermissionVersionResponseTypeDef = TypedDict(
+    "DeletePermissionVersionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "permissionStatus": PermissionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResourceShareResponseTypeDef = TypedDict(
+    "DeleteResourceShareResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateResourceSharePermissionResponseTypeDef = TypedDict(
+    "DisassociateResourceSharePermissionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnableSharingWithAwsOrganizationResponseTypeDef = TypedDict(
+    "EnableSharingWithAwsOrganizationResponseTypeDef",
+    {
+        "returnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePoliciesResponseTypeDef = TypedDict(
+    "GetResourcePoliciesResponseTypeDef",
+    {
+        "policies": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PromoteResourceShareCreatedFromPolicyResponseTypeDef = TypedDict(
+    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
+    {
+        "returnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetDefaultPermissionVersionResponseTypeDef = TypedDict(
+    "SetDefaultPermissionVersionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 AssociateResourceShareResponseTypeDef = TypedDict(
     "AssociateResourceShareResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResourceShareResponseTypeDef = TypedDict(
     "DisassociateResourceShareResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceShareAssociationsResponseTypeDef = TypedDict(
     "GetResourceShareAssociationsResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceShareInvitationTypeDef = TypedDict(
     "ResourceShareInvitationTypeDef",
     {
         "resourceShareInvitationArn": str,
@@ -1092,15 +945,15 @@
 )
 
 ListPermissionAssociationsResponseTypeDef = TypedDict(
     "ListPermissionAssociationsResponseTypeDef",
     {
         "permissions": List[AssociatedPermissionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePermissionRequestRequestTypeDef",
     {
         "name": str,
@@ -1113,21 +966,19 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePermissionRequestRequestTypeDef(
     _RequiredCreatePermissionRequestRequestTypeDef, _OptionalCreatePermissionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceShareRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateResourceShareRequestRequestTypeDef = TypedDict(
@@ -1135,103 +986,148 @@
     {
         "resourceArns": Sequence[str],
         "principals": Sequence[str],
         "tags": Sequence[TagTypeDef],
         "allowExternalPrincipals": bool,
         "clientToken": str,
         "permissionArns": Sequence[str],
+        "sources": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateResourceShareRequestRequestTypeDef(
     _RequiredCreateResourceShareRequestRequestTypeDef,
     _OptionalCreateResourceShareRequestRequestTypeDef,
 ):
     pass
 
+_RequiredTagResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredTagResourceRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+)
+_OptionalTagResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalTagResourceRequestRequestTypeDef",
+    {
+        "resourceShareArn": str,
+        "resourceArn": str,
+    },
+    total=False,
+)
 
-ResourceSharePermissionDetailTypeDef = TypedDict(
-    "ResourceSharePermissionDetailTypeDef",
+class TagResourceRequestRequestTypeDef(
+    _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
+):
+    pass
+
+_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "permission": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
-        "permissionType": PermissionTypeType,
-        "featureSet": PermissionFeatureSetType,
-        "status": PermissionStatusType,
-        "tags": List[TagTypeDef],
+        "resourceArns": Sequence[str],
+    },
+)
+_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "principal": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResourceSharePermissionSummaryTypeDef = TypedDict(
-    "ResourceSharePermissionSummaryTypeDef",
+class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
     {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "status": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
-        "permissionType": PermissionTypeType,
-        "featureSet": PermissionFeatureSetType,
-        "tags": List[TagTypeDef],
+        "associationType": ResourceShareAssociationTypeType,
+    },
+)
+_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
+    {
+        "resourceShareArns": Sequence[str],
+        "resourceArn": str,
+        "principal": str,
+        "associationStatus": ResourceShareAssociationStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResourceShareTypeDef = TypedDict(
-    "ResourceShareTypeDef",
+class GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef(
+    _RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
+    _OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
+):
+    pass
+
+GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef = TypedDict(
+    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
     {
-        "resourceShareArn": str,
-        "name": str,
-        "owningAccountId": str,
-        "allowExternalPrincipals": bool,
-        "status": ResourceShareStatusType,
-        "statusMessage": str,
-        "tags": List[TagTypeDef],
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "featureSet": ResourceShareFeatureSetType,
+        "resourceShareInvitationArns": Sequence[str],
+        "resourceShareArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredTagResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredTagResourceRequestRequestTypeDef",
+_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "resourceOwner": ResourceOwnerType,
     },
 )
-_OptionalTagResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalTagResourceRequestRequestTypeDef",
+_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef",
     {
-        "resourceShareArn": str,
         "resourceArn": str,
+        "principals": Sequence[str],
+        "resourceType": str,
+        "resourceShareArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class TagResourceRequestRequestTypeDef(
-    _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
+class ListPrincipalsRequestListPrincipalsPaginateTypeDef(
+    _RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef,
+    _OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef,
 ):
     pass
 
+_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "resourceOwner": ResourceOwnerType,
+    },
+)
+_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "principal": str,
+        "resourceType": str,
+        "resourceArns": Sequence[str],
+        "resourceShareArns": Sequence[str],
+        "resourceRegionScope": ResourceRegionScopeFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourcesRequestListResourcesPaginateTypeDef(
+    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
+    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
+):
+    pass
 
 _RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef = TypedDict(
     "_RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
     },
 )
@@ -1240,27 +1136,25 @@
     {
         "resourceShareArns": Sequence[str],
         "resourceShareStatus": ResourceShareStatusType,
         "name": str,
         "tagFilters": Sequence[TagFilterTypeDef],
         "permissionArn": str,
         "permissionVersion": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetResourceSharesRequestGetResourceSharesPaginateTypeDef(
     _RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     _OptionalGetResourceSharesRequestGetResourceSharesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetResourceSharesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceSharesRequestRequestTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
     },
 )
 _OptionalGetResourceSharesRequestRequestTypeDef = TypedDict(
@@ -1274,183 +1168,237 @@
         "maxResults": int,
         "permissionArn": str,
         "permissionVersion": int,
     },
     total=False,
 )
 
-
 class GetResourceSharesRequestRequestTypeDef(
     _RequiredGetResourceSharesRequestRequestTypeDef, _OptionalGetResourceSharesRequestRequestTypeDef
 ):
     pass
 
-
 ListPendingInvitationResourcesResponseTypeDef = TypedDict(
     "ListPendingInvitationResourcesResponseTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPrincipalsResponseTypeDef = TypedDict(
     "ListPrincipalsResponseTypeDef",
     {
         "principals": List[PrincipalTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReplacePermissionAssociationsWorkResponseTypeDef = TypedDict(
     "ListReplacePermissionAssociationsWorkResponseTypeDef",
     {
         "replacePermissionAssociationsWorks": List[ReplacePermissionAssociationsWorkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplacePermissionAssociationsResponseTypeDef = TypedDict(
     "ReplacePermissionAssociationsResponseTypeDef",
     {
         "replacePermissionAssociationsWork": ReplacePermissionAssociationsWorkTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceTypesResponseTypeDef = TypedDict(
     "ListResourceTypesResponseTypeDef",
     {
         "resourceTypes": List[ServiceNameAndResourceTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResourceSharePermissionDetailTypeDef = TypedDict(
+    "ResourceSharePermissionDetailTypeDef",
+    {
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "permission": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+        "permissionType": PermissionTypeType,
+        "featureSet": PermissionFeatureSetType,
+        "status": PermissionStatusType,
+        "tags": List[TagOutputTypeDef],
     },
+    total=False,
+)
+
+ResourceSharePermissionSummaryTypeDef = TypedDict(
+    "ResourceSharePermissionSummaryTypeDef",
+    {
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "status": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+        "permissionType": PermissionTypeType,
+        "featureSet": PermissionFeatureSetType,
+        "tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+ResourceShareTypeDef = TypedDict(
+    "ResourceShareTypeDef",
+    {
+        "resourceShareArn": str,
+        "name": str,
+        "owningAccountId": str,
+        "allowExternalPrincipals": bool,
+        "status": ResourceShareStatusType,
+        "statusMessage": str,
+        "tags": List[TagOutputTypeDef],
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "featureSet": ResourceShareFeatureSetType,
+    },
+    total=False,
 )
 
 AcceptResourceShareInvitationResponseTypeDef = TypedDict(
     "AcceptResourceShareInvitationResponseTypeDef",
     {
         "resourceShareInvitation": ResourceShareInvitationTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceShareInvitationsResponseTypeDef = TypedDict(
     "GetResourceShareInvitationsResponseTypeDef",
     {
         "resourceShareInvitations": List[ResourceShareInvitationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RejectResourceShareInvitationResponseTypeDef = TypedDict(
     "RejectResourceShareInvitationResponseTypeDef",
     {
         "resourceShareInvitation": ResourceShareInvitationTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePermissionVersionResponseTypeDef = TypedDict(
     "CreatePermissionVersionResponseTypeDef",
     {
         "permission": ResourceSharePermissionDetailTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPermissionResponseTypeDef = TypedDict(
     "GetPermissionResponseTypeDef",
     {
         "permission": ResourceSharePermissionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePermissionResponseTypeDef = TypedDict(
     "CreatePermissionResponseTypeDef",
     {
         "permission": ResourceSharePermissionSummaryTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionVersionsResponseTypeDef = TypedDict(
     "ListPermissionVersionsResponseTypeDef",
     {
         "permissions": List[ResourceSharePermissionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "permissions": List[ResourceSharePermissionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceSharePermissionsResponseTypeDef = TypedDict(
     "ListResourceSharePermissionsResponseTypeDef",
     {
         "permissions": List[ResourceSharePermissionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PromotePermissionCreatedFromPolicyResponseTypeDef = TypedDict(
     "PromotePermissionCreatedFromPolicyResponseTypeDef",
     {
         "permission": ResourceSharePermissionSummaryTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResourceShareResponseTypeDef = TypedDict(
     "CreateResourceShareResponseTypeDef",
     {
         "resourceShare": ResourceShareTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceSharesResponseTypeDef = TypedDict(
     "GetResourceSharesResponseTypeDef",
     {
         "resourceShares": List[ResourceShareTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceShareResponseTypeDef = TypedDict(
     "UpdateResourceShareResponseTypeDef",
     {
         "resourceShare": ResourceShareTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram/type_defs.pyi` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,87 +33,89 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptResourceShareInvitationRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateResourceSharePermissionRequestRequestTypeDef",
-    "AssociateResourceSharePermissionResponseTypeDef",
     "AssociateResourceShareRequestRequestTypeDef",
     "ResourceShareAssociationTypeDef",
     "AssociatedPermissionTypeDef",
     "TagTypeDef",
     "CreatePermissionVersionRequestRequestTypeDef",
     "DeletePermissionRequestRequestTypeDef",
-    "DeletePermissionResponseTypeDef",
     "DeletePermissionVersionRequestRequestTypeDef",
-    "DeletePermissionVersionResponseTypeDef",
     "DeleteResourceShareRequestRequestTypeDef",
-    "DeleteResourceShareResponseTypeDef",
     "DisassociateResourceSharePermissionRequestRequestTypeDef",
-    "DisassociateResourceSharePermissionResponseTypeDef",
     "DisassociateResourceShareRequestRequestTypeDef",
-    "EnableSharingWithAwsOrganizationResponseTypeDef",
     "GetPermissionRequestRequestTypeDef",
-    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
-    "GetResourcePoliciesResponseTypeDef",
-    "GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
     "GetResourceShareAssociationsRequestRequestTypeDef",
-    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
     "GetResourceShareInvitationsRequestRequestTypeDef",
     "TagFilterTypeDef",
     "ListPendingInvitationResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListPermissionAssociationsRequestRequestTypeDef",
     "ListPermissionVersionsRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
-    "ListPrincipalsRequestListPrincipalsPaginateTypeDef",
     "ListPrincipalsRequestRequestTypeDef",
     "PrincipalTypeDef",
     "ListReplacePermissionAssociationsWorkRequestRequestTypeDef",
     "ReplacePermissionAssociationsWorkTypeDef",
     "ListResourceSharePermissionsRequestRequestTypeDef",
     "ListResourceTypesRequestRequestTypeDef",
     "ServiceNameAndResourceTypeTypeDef",
-    "ListResourcesRequestListResourcesPaginateTypeDef",
     "ListResourcesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PromotePermissionCreatedFromPolicyRequestRequestTypeDef",
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
-    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
     "RejectResourceShareInvitationRequestRequestTypeDef",
     "ReplacePermissionAssociationsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "SetDefaultPermissionVersionRequestRequestTypeDef",
-    "SetDefaultPermissionVersionResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateResourceShareRequestRequestTypeDef",
+    "AssociateResourceSharePermissionResponseTypeDef",
+    "DeletePermissionResponseTypeDef",
+    "DeletePermissionVersionResponseTypeDef",
+    "DeleteResourceShareResponseTypeDef",
+    "DisassociateResourceSharePermissionResponseTypeDef",
+    "EnableSharingWithAwsOrganizationResponseTypeDef",
+    "GetResourcePoliciesResponseTypeDef",
+    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
+    "SetDefaultPermissionVersionResponseTypeDef",
     "AssociateResourceShareResponseTypeDef",
     "DisassociateResourceShareResponseTypeDef",
     "GetResourceShareAssociationsResponseTypeDef",
     "ResourceShareInvitationTypeDef",
     "ListPermissionAssociationsResponseTypeDef",
     "CreatePermissionRequestRequestTypeDef",
     "CreateResourceShareRequestRequestTypeDef",
-    "ResourceSharePermissionDetailTypeDef",
-    "ResourceSharePermissionSummaryTypeDef",
-    "ResourceShareTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    "GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
+    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
+    "ListPrincipalsRequestListPrincipalsPaginateTypeDef",
+    "ListResourcesRequestListResourcesPaginateTypeDef",
     "GetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     "GetResourceSharesRequestRequestTypeDef",
     "ListPendingInvitationResourcesResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "ListPrincipalsResponseTypeDef",
     "ListReplacePermissionAssociationsWorkResponseTypeDef",
     "ReplacePermissionAssociationsResponseTypeDef",
     "ListResourceTypesResponseTypeDef",
+    "ResourceSharePermissionDetailTypeDef",
+    "ResourceSharePermissionSummaryTypeDef",
+    "ResourceShareTypeDef",
     "AcceptResourceShareInvitationResponseTypeDef",
     "GetResourceShareInvitationsResponseTypeDef",
     "RejectResourceShareInvitationResponseTypeDef",
     "CreatePermissionVersionResponseTypeDef",
     "GetPermissionResponseTypeDef",
     "CreatePermissionResponseTypeDef",
     "ListPermissionVersionsResponseTypeDef",
@@ -135,20 +137,33 @@
     "_OptionalAcceptResourceShareInvitationRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class AcceptResourceShareInvitationRequestRequestTypeDef(
     _RequiredAcceptResourceShareInvitationRequestRequestTypeDef,
     _OptionalAcceptResourceShareInvitationRequestRequestTypeDef,
 ):
     pass
 
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
 _RequiredAssociateResourceSharePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateResourceSharePermissionRequestRequestTypeDef",
     {
         "resourceShareArn": str,
         "permissionArn": str,
     },
 )
@@ -158,51 +173,47 @@
         "replace": bool,
         "clientToken": str,
         "permissionVersion": int,
     },
     total=False,
 )
 
+
 class AssociateResourceSharePermissionRequestRequestTypeDef(
     _RequiredAssociateResourceSharePermissionRequestRequestTypeDef,
     _OptionalAssociateResourceSharePermissionRequestRequestTypeDef,
 ):
     pass
 
-AssociateResourceSharePermissionResponseTypeDef = TypedDict(
-    "AssociateResourceSharePermissionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredAssociateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalAssociateResourceShareRequestRequestTypeDef = TypedDict(
     "_OptionalAssociateResourceShareRequestRequestTypeDef",
     {
         "resourceArns": Sequence[str],
         "principals": Sequence[str],
         "clientToken": str,
+        "sources": Sequence[str],
     },
     total=False,
 )
 
+
 class AssociateResourceShareRequestRequestTypeDef(
     _RequiredAssociateResourceShareRequestRequestTypeDef,
     _OptionalAssociateResourceShareRequestRequestTypeDef,
 ):
     pass
 
+
 ResourceShareAssociationTypeDef = TypedDict(
     "ResourceShareAssociationTypeDef",
     {
         "resourceShareArn": str,
         "resourceShareName": str,
         "associatedEntity": str,
         "associationType": ResourceShareAssociationTypeType,
@@ -250,48 +261,42 @@
     "_OptionalCreatePermissionVersionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreatePermissionVersionRequestRequestTypeDef(
     _RequiredCreatePermissionVersionRequestRequestTypeDef,
     _OptionalCreatePermissionVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeletePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePermissionRequestRequestTypeDef",
     {
         "permissionArn": str,
     },
 )
 _OptionalDeletePermissionRequestRequestTypeDef = TypedDict(
     "_OptionalDeletePermissionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeletePermissionRequestRequestTypeDef(
     _RequiredDeletePermissionRequestRequestTypeDef, _OptionalDeletePermissionRequestRequestTypeDef
 ):
     pass
 
-DeletePermissionResponseTypeDef = TypedDict(
-    "DeletePermissionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "permissionStatus": PermissionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeletePermissionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePermissionVersionRequestRequestTypeDef",
     {
         "permissionArn": str,
         "permissionVersion": int,
     },
@@ -300,29 +305,21 @@
     "_OptionalDeletePermissionVersionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeletePermissionVersionRequestRequestTypeDef(
     _RequiredDeletePermissionVersionRequestRequestTypeDef,
     _OptionalDeletePermissionVersionRequestRequestTypeDef,
 ):
     pass
 
-DeletePermissionVersionResponseTypeDef = TypedDict(
-    "DeletePermissionVersionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "permissionStatus": PermissionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeleteResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
@@ -330,28 +327,21 @@
     "_OptionalDeleteResourceShareRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteResourceShareRequestRequestTypeDef(
     _RequiredDeleteResourceShareRequestRequestTypeDef,
     _OptionalDeleteResourceShareRequestRequestTypeDef,
 ):
     pass
 
-DeleteResourceShareResponseTypeDef = TypedDict(
-    "DeleteResourceShareResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDisassociateResourceSharePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateResourceSharePermissionRequestRequestTypeDef",
     {
         "resourceShareArn": str,
         "permissionArn": str,
     },
@@ -360,58 +350,46 @@
     "_OptionalDisassociateResourceSharePermissionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DisassociateResourceSharePermissionRequestRequestTypeDef(
     _RequiredDisassociateResourceSharePermissionRequestRequestTypeDef,
     _OptionalDisassociateResourceSharePermissionRequestRequestTypeDef,
 ):
     pass
 
-DisassociateResourceSharePermissionResponseTypeDef = TypedDict(
-    "DisassociateResourceSharePermissionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDisassociateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalDisassociateResourceShareRequestRequestTypeDef = TypedDict(
     "_OptionalDisassociateResourceShareRequestRequestTypeDef",
     {
         "resourceArns": Sequence[str],
         "principals": Sequence[str],
         "clientToken": str,
+        "sources": Sequence[str],
     },
     total=False,
 )
 
+
 class DisassociateResourceShareRequestRequestTypeDef(
     _RequiredDisassociateResourceShareRequestRequestTypeDef,
     _OptionalDisassociateResourceShareRequestRequestTypeDef,
 ):
     pass
 
-EnableSharingWithAwsOrganizationResponseTypeDef = TypedDict(
-    "EnableSharingWithAwsOrganizationResponseTypeDef",
-    {
-        "returnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredGetPermissionRequestRequestTypeDef",
     {
         "permissionArn": str,
     },
 )
@@ -419,40 +397,31 @@
     "_OptionalGetPermissionRequestRequestTypeDef",
     {
         "permissionVersion": int,
     },
     total=False,
 )
 
+
 class GetPermissionRequestRequestTypeDef(
     _RequiredGetPermissionRequestRequestTypeDef, _OptionalGetPermissionRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
-    {
-        "resourceArns": Sequence[str],
-    },
-)
-_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "principal": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetResourcePoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesRequestRequestTypeDef",
     {
         "resourceArns": Sequence[str],
     },
 )
 _OptionalGetResourcePoliciesRequestRequestTypeDef = TypedDict(
@@ -461,52 +430,21 @@
         "principal": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetResourcePoliciesRequestRequestTypeDef(
     _RequiredGetResourcePoliciesRequestRequestTypeDef,
     _OptionalGetResourcePoliciesRequestRequestTypeDef,
 ):
     pass
 
-GetResourcePoliciesResponseTypeDef = TypedDict(
-    "GetResourcePoliciesResponseTypeDef",
-    {
-        "policies": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
-    {
-        "associationType": ResourceShareAssociationTypeType,
-    },
-)
-_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
-    {
-        "resourceShareArns": Sequence[str],
-        "resourceArn": str,
-        "principal": str,
-        "associationStatus": ResourceShareAssociationStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef(
-    _RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
-    _OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
-):
-    pass
 
 _RequiredGetResourceShareAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceShareAssociationsRequestRequestTypeDef",
     {
         "associationType": ResourceShareAssociationTypeType,
     },
 )
@@ -519,29 +457,21 @@
         "associationStatus": ResourceShareAssociationStatusType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetResourceShareAssociationsRequestRequestTypeDef(
     _RequiredGetResourceShareAssociationsRequestRequestTypeDef,
     _OptionalGetResourceShareAssociationsRequestRequestTypeDef,
 ):
     pass
 
-GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef = TypedDict(
-    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
-    {
-        "resourceShareInvitationArns": Sequence[str],
-        "resourceShareArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 GetResourceShareInvitationsRequestRequestTypeDef = TypedDict(
     "GetResourceShareInvitationsRequestRequestTypeDef",
     {
         "resourceShareInvitationArns": Sequence[str],
         "resourceShareArns": Sequence[str],
         "nextToken": str,
@@ -571,20 +501,22 @@
         "nextToken": str,
         "maxResults": int,
         "resourceRegionScope": ResourceRegionScopeFilterType,
     },
     total=False,
 )
 
+
 class ListPendingInvitationResourcesRequestRequestTypeDef(
     _RequiredListPendingInvitationResourcesRequestRequestTypeDef,
     _OptionalListPendingInvitationResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "arn": str,
         "type": str,
         "resourceShareArn": str,
         "resourceGroupArn": str,
@@ -623,55 +555,33 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListPermissionVersionsRequestRequestTypeDef(
     _RequiredListPermissionVersionsRequestRequestTypeDef,
     _OptionalListPermissionVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListPermissionsRequestRequestTypeDef = TypedDict(
     "ListPermissionsRequestRequestTypeDef",
     {
         "resourceType": str,
         "nextToken": str,
         "maxResults": int,
         "permissionType": PermissionTypeFilterType,
     },
     total=False,
 )
 
-_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef",
-    {
-        "resourceOwner": ResourceOwnerType,
-    },
-)
-_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef",
-    {
-        "resourceArn": str,
-        "principals": Sequence[str],
-        "resourceType": str,
-        "resourceShareArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPrincipalsRequestListPrincipalsPaginateTypeDef(
-    _RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef,
-    _OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalsRequestRequestTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
     },
 )
 _OptionalListPrincipalsRequestRequestTypeDef = TypedDict(
@@ -683,19 +593,21 @@
         "resourceShareArns": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListPrincipalsRequestRequestTypeDef(
     _RequiredListPrincipalsRequestRequestTypeDef, _OptionalListPrincipalsRequestRequestTypeDef
 ):
     pass
 
+
 PrincipalTypeDef = TypedDict(
     "PrincipalTypeDef",
     {
         "id": str,
         "resourceShareArn": str,
         "creationTime": datetime,
         "lastUpdatedTime": datetime,
@@ -742,20 +654,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListResourceSharePermissionsRequestRequestTypeDef(
     _RequiredListResourceSharePermissionsRequestRequestTypeDef,
     _OptionalListResourceSharePermissionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListResourceTypesRequestRequestTypeDef = TypedDict(
     "ListResourceTypesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "resourceRegionScope": ResourceRegionScopeFilterType,
     },
@@ -768,39 +682,14 @@
         "resourceType": str,
         "serviceName": str,
         "resourceRegionScope": ResourceRegionScopeType,
     },
     total=False,
 )
 
-_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "resourceOwner": ResourceOwnerType,
-    },
-)
-_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "principal": str,
-        "resourceType": str,
-        "resourceArns": Sequence[str],
-        "resourceShareArns": Sequence[str],
-        "resourceRegionScope": ResourceRegionScopeFilterType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourcesRequestListResourcesPaginateTypeDef(
-    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
-    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -813,28 +702,20 @@
         "nextToken": str,
         "maxResults": int,
         "resourceRegionScope": ResourceRegionScopeFilterType,
     },
     total=False,
 )
 
+
 class ListResourcesRequestRequestTypeDef(
     _RequiredListResourcesRequestRequestTypeDef, _OptionalListResourcesRequestRequestTypeDef
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
 
 _RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef",
     {
         "permissionArn": str,
         "name": str,
     },
@@ -843,55 +724,51 @@
     "_OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class PromotePermissionCreatedFromPolicyRequestRequestTypeDef(
     _RequiredPromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     _OptionalPromotePermissionCreatedFromPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef = TypedDict(
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 
-PromoteResourceShareCreatedFromPolicyResponseTypeDef = TypedDict(
-    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
-    {
-        "returnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRejectResourceShareInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredRejectResourceShareInvitationRequestRequestTypeDef",
     {
         "resourceShareInvitationArn": str,
     },
 )
 _OptionalRejectResourceShareInvitationRequestRequestTypeDef = TypedDict(
     "_OptionalRejectResourceShareInvitationRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class RejectResourceShareInvitationRequestRequestTypeDef(
     _RequiredRejectResourceShareInvitationRequestRequestTypeDef,
     _OptionalRejectResourceShareInvitationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredReplacePermissionAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredReplacePermissionAssociationsRequestRequestTypeDef",
     {
         "fromPermissionArn": str,
         "toPermissionArn": str,
     },
 )
@@ -900,29 +777,29 @@
     {
         "fromPermissionVersion": int,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class ReplacePermissionAssociationsRequestRequestTypeDef(
     _RequiredReplacePermissionAssociationsRequestRequestTypeDef,
     _OptionalReplacePermissionAssociationsRequestRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "key": str,
+        "value": str,
     },
+    total=False,
 )
 
 _RequiredSetDefaultPermissionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredSetDefaultPermissionVersionRequestRequestTypeDef",
     {
         "permissionArn": str,
         "permissionVersion": int,
@@ -932,28 +809,21 @@
     "_OptionalSetDefaultPermissionVersionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class SetDefaultPermissionVersionRequestRequestTypeDef(
     _RequiredSetDefaultPermissionVersionRequestRequestTypeDef,
     _OptionalSetDefaultPermissionVersionRequestRequestTypeDef,
 ):
     pass
 
-SetDefaultPermissionVersionResponseTypeDef = TypedDict(
-    "SetDefaultPermissionVersionResponseTypeDef",
-    {
-        "returnValue": bool,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUntagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUntagResourceRequestRequestTypeDef",
     {
         "tagKeys": Sequence[str],
     },
 )
@@ -962,19 +832,21 @@
     {
         "resourceShareArn": str,
         "resourceArn": str,
     },
     total=False,
 )
 
+
 class UntagResourceRequestRequestTypeDef(
     _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceShareRequestRequestTypeDef",
     {
         "resourceShareArn": str,
     },
 )
 _OptionalUpdateResourceShareRequestRequestTypeDef = TypedDict(
@@ -983,44 +855,127 @@
         "name": str,
         "allowExternalPrincipals": bool,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateResourceShareRequestRequestTypeDef(
     _RequiredUpdateResourceShareRequestRequestTypeDef,
     _OptionalUpdateResourceShareRequestRequestTypeDef,
 ):
     pass
 
+
+AssociateResourceSharePermissionResponseTypeDef = TypedDict(
+    "AssociateResourceSharePermissionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePermissionResponseTypeDef = TypedDict(
+    "DeletePermissionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "permissionStatus": PermissionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePermissionVersionResponseTypeDef = TypedDict(
+    "DeletePermissionVersionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "permissionStatus": PermissionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResourceShareResponseTypeDef = TypedDict(
+    "DeleteResourceShareResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateResourceSharePermissionResponseTypeDef = TypedDict(
+    "DisassociateResourceSharePermissionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnableSharingWithAwsOrganizationResponseTypeDef = TypedDict(
+    "EnableSharingWithAwsOrganizationResponseTypeDef",
+    {
+        "returnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePoliciesResponseTypeDef = TypedDict(
+    "GetResourcePoliciesResponseTypeDef",
+    {
+        "policies": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PromoteResourceShareCreatedFromPolicyResponseTypeDef = TypedDict(
+    "PromoteResourceShareCreatedFromPolicyResponseTypeDef",
+    {
+        "returnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetDefaultPermissionVersionResponseTypeDef = TypedDict(
+    "SetDefaultPermissionVersionResponseTypeDef",
+    {
+        "returnValue": bool,
+        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AssociateResourceShareResponseTypeDef = TypedDict(
     "AssociateResourceShareResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResourceShareResponseTypeDef = TypedDict(
     "DisassociateResourceShareResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceShareAssociationsResponseTypeDef = TypedDict(
     "GetResourceShareAssociationsResponseTypeDef",
     {
         "resourceShareAssociations": List[ResourceShareAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceShareInvitationTypeDef = TypedDict(
     "ResourceShareInvitationTypeDef",
     {
         "resourceShareInvitationArn": str,
@@ -1037,15 +992,15 @@
 )
 
 ListPermissionAssociationsResponseTypeDef = TypedDict(
     "ListPermissionAssociationsResponseTypeDef",
     {
         "permissions": List[AssociatedPermissionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePermissionRequestRequestTypeDef",
     {
         "name": str,
@@ -1058,19 +1013,21 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePermissionRequestRequestTypeDef(
     _RequiredCreatePermissionRequestRequestTypeDef, _OptionalCreatePermissionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateResourceShareRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceShareRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateResourceShareRequestRequestTypeDef = TypedDict(
@@ -1078,100 +1035,161 @@
     {
         "resourceArns": Sequence[str],
         "principals": Sequence[str],
         "tags": Sequence[TagTypeDef],
         "allowExternalPrincipals": bool,
         "clientToken": str,
         "permissionArns": Sequence[str],
+        "sources": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateResourceShareRequestRequestTypeDef(
     _RequiredCreateResourceShareRequestRequestTypeDef,
     _OptionalCreateResourceShareRequestRequestTypeDef,
 ):
     pass
 
-ResourceSharePermissionDetailTypeDef = TypedDict(
-    "ResourceSharePermissionDetailTypeDef",
+
+_RequiredTagResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredTagResourceRequestRequestTypeDef",
     {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "permission": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
-        "permissionType": PermissionTypeType,
-        "featureSet": PermissionFeatureSetType,
-        "status": PermissionStatusType,
-        "tags": List[TagTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+)
+_OptionalTagResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalTagResourceRequestRequestTypeDef",
+    {
+        "resourceShareArn": str,
+        "resourceArn": str,
     },
     total=False,
 )
 
-ResourceSharePermissionSummaryTypeDef = TypedDict(
-    "ResourceSharePermissionSummaryTypeDef",
+
+class TagResourceRequestRequestTypeDef(
+    _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "status": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
-        "permissionType": PermissionTypeType,
-        "featureSet": PermissionFeatureSetType,
-        "tags": List[TagTypeDef],
+        "resourceArns": Sequence[str],
+    },
+)
+_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
+    {
+        "principal": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResourceShareTypeDef = TypedDict(
-    "ResourceShareTypeDef",
+
+class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
     {
-        "resourceShareArn": str,
-        "name": str,
-        "owningAccountId": str,
-        "allowExternalPrincipals": bool,
-        "status": ResourceShareStatusType,
-        "statusMessage": str,
-        "tags": List[TagTypeDef],
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "featureSet": ResourceShareFeatureSetType,
+        "associationType": ResourceShareAssociationTypeType,
+    },
+)
+_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
+    {
+        "resourceShareArns": Sequence[str],
+        "resourceArn": str,
+        "principal": str,
+        "associationStatus": ResourceShareAssociationStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredTagResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredTagResourceRequestRequestTypeDef",
+
+class GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef(
+    _RequiredGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
+    _OptionalGetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
+):
+    pass
+
+
+GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef = TypedDict(
+    "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "resourceShareInvitationArns": Sequence[str],
+        "resourceShareArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalTagResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalTagResourceRequestRequestTypeDef",
+
+_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef",
+    {
+        "resourceOwner": ResourceOwnerType,
+    },
+)
+_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef",
     {
-        "resourceShareArn": str,
         "resourceArn": str,
+        "principals": Sequence[str],
+        "resourceType": str,
+        "resourceShareArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class TagResourceRequestRequestTypeDef(
-    _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
+
+class ListPrincipalsRequestListPrincipalsPaginateTypeDef(
+    _RequiredListPrincipalsRequestListPrincipalsPaginateTypeDef,
+    _OptionalListPrincipalsRequestListPrincipalsPaginateTypeDef,
 ):
     pass
 
+
+_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "resourceOwner": ResourceOwnerType,
+    },
+)
+_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "principal": str,
+        "resourceType": str,
+        "resourceArns": Sequence[str],
+        "resourceShareArns": Sequence[str],
+        "resourceRegionScope": ResourceRegionScopeFilterType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourcesRequestListResourcesPaginateTypeDef(
+    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
+    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef = TypedDict(
     "_RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
     },
 )
 _OptionalGetResourceSharesRequestGetResourceSharesPaginateTypeDef = TypedDict(
@@ -1179,25 +1197,27 @@
     {
         "resourceShareArns": Sequence[str],
         "resourceShareStatus": ResourceShareStatusType,
         "name": str,
         "tagFilters": Sequence[TagFilterTypeDef],
         "permissionArn": str,
         "permissionVersion": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetResourceSharesRequestGetResourceSharesPaginateTypeDef(
     _RequiredGetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     _OptionalGetResourceSharesRequestGetResourceSharesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetResourceSharesRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceSharesRequestRequestTypeDef",
     {
         "resourceOwner": ResourceOwnerType,
     },
 )
 _OptionalGetResourceSharesRequestRequestTypeDef = TypedDict(
@@ -1211,181 +1231,239 @@
         "maxResults": int,
         "permissionArn": str,
         "permissionVersion": int,
     },
     total=False,
 )
 
+
 class GetResourceSharesRequestRequestTypeDef(
     _RequiredGetResourceSharesRequestRequestTypeDef, _OptionalGetResourceSharesRequestRequestTypeDef
 ):
     pass
 
+
 ListPendingInvitationResourcesResponseTypeDef = TypedDict(
     "ListPendingInvitationResourcesResponseTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPrincipalsResponseTypeDef = TypedDict(
     "ListPrincipalsResponseTypeDef",
     {
         "principals": List[PrincipalTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReplacePermissionAssociationsWorkResponseTypeDef = TypedDict(
     "ListReplacePermissionAssociationsWorkResponseTypeDef",
     {
         "replacePermissionAssociationsWorks": List[ReplacePermissionAssociationsWorkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplacePermissionAssociationsResponseTypeDef = TypedDict(
     "ReplacePermissionAssociationsResponseTypeDef",
     {
         "replacePermissionAssociationsWork": ReplacePermissionAssociationsWorkTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceTypesResponseTypeDef = TypedDict(
     "ListResourceTypesResponseTypeDef",
     {
         "resourceTypes": List[ServiceNameAndResourceTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResourceSharePermissionDetailTypeDef = TypedDict(
+    "ResourceSharePermissionDetailTypeDef",
+    {
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "permission": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+        "permissionType": PermissionTypeType,
+        "featureSet": PermissionFeatureSetType,
+        "status": PermissionStatusType,
+        "tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+ResourceSharePermissionSummaryTypeDef = TypedDict(
+    "ResourceSharePermissionSummaryTypeDef",
+    {
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "status": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+        "permissionType": PermissionTypeType,
+        "featureSet": PermissionFeatureSetType,
+        "tags": List[TagOutputTypeDef],
     },
+    total=False,
+)
+
+ResourceShareTypeDef = TypedDict(
+    "ResourceShareTypeDef",
+    {
+        "resourceShareArn": str,
+        "name": str,
+        "owningAccountId": str,
+        "allowExternalPrincipals": bool,
+        "status": ResourceShareStatusType,
+        "statusMessage": str,
+        "tags": List[TagOutputTypeDef],
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "featureSet": ResourceShareFeatureSetType,
+    },
+    total=False,
 )
 
 AcceptResourceShareInvitationResponseTypeDef = TypedDict(
     "AcceptResourceShareInvitationResponseTypeDef",
     {
         "resourceShareInvitation": ResourceShareInvitationTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceShareInvitationsResponseTypeDef = TypedDict(
     "GetResourceShareInvitationsResponseTypeDef",
     {
         "resourceShareInvitations": List[ResourceShareInvitationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RejectResourceShareInvitationResponseTypeDef = TypedDict(
     "RejectResourceShareInvitationResponseTypeDef",
     {
         "resourceShareInvitation": ResourceShareInvitationTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePermissionVersionResponseTypeDef = TypedDict(
     "CreatePermissionVersionResponseTypeDef",
     {
         "permission": ResourceSharePermissionDetailTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPermissionResponseTypeDef = TypedDict(
     "GetPermissionResponseTypeDef",
     {
         "permission": ResourceSharePermissionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePermissionResponseTypeDef = TypedDict(
     "CreatePermissionResponseTypeDef",
     {
         "permission": ResourceSharePermissionSummaryTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionVersionsResponseTypeDef = TypedDict(
     "ListPermissionVersionsResponseTypeDef",
     {
         "permissions": List[ResourceSharePermissionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "permissions": List[ResourceSharePermissionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceSharePermissionsResponseTypeDef = TypedDict(
     "ListResourceSharePermissionsResponseTypeDef",
     {
         "permissions": List[ResourceSharePermissionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PromotePermissionCreatedFromPolicyResponseTypeDef = TypedDict(
     "PromotePermissionCreatedFromPolicyResponseTypeDef",
     {
         "permission": ResourceSharePermissionSummaryTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResourceShareResponseTypeDef = TypedDict(
     "CreateResourceShareResponseTypeDef",
     {
         "resourceShare": ResourceShareTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceSharesResponseTypeDef = TypedDict(
     "GetResourceSharesResponseTypeDef",
     {
         "resourceShares": List[ResourceShareTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceShareResponseTypeDef = TypedDict(
     "UpdateResourceShareResponseTypeDef",
     {
         "resourceShare": ResourceShareTypeDef,
         "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram.egg-info/PKG-INFO` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ram
-Version: 1.28.0
-Summary: Type annotations for boto3.RAM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.RAM 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ram"></a>
 
 # mypy-boto3-ram
 
 [![PyPI - mypy-boto3-ram](https://img.shields.io/pypi/v/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ram?color=blue)](https://pypistats.org/packages/mypy-boto3-ram)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ram)](https://pepy.tech/project/mypy-boto3-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RAM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[boto3.RAM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
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
 [mypy-boto3-ram docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,85 +357,86 @@
 
 `mypy_boto3_ram.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ram.type_defs import (
     AcceptResourceShareInvitationRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AssociateResourceSharePermissionRequestRequestTypeDef,
-    AssociateResourceSharePermissionResponseTypeDef,
     AssociateResourceShareRequestRequestTypeDef,
     ResourceShareAssociationTypeDef,
     AssociatedPermissionTypeDef,
     TagTypeDef,
     CreatePermissionVersionRequestRequestTypeDef,
     DeletePermissionRequestRequestTypeDef,
-    DeletePermissionResponseTypeDef,
     DeletePermissionVersionRequestRequestTypeDef,
-    DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareRequestRequestTypeDef,
-    DeleteResourceShareResponseTypeDef,
     DisassociateResourceSharePermissionRequestRequestTypeDef,
-    DisassociateResourceSharePermissionResponseTypeDef,
     DisassociateResourceShareRequestRequestTypeDef,
-    EnableSharingWithAwsOrganizationResponseTypeDef,
     GetPermissionRequestRequestTypeDef,
-    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
-    GetResourcePoliciesResponseTypeDef,
-    GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
     GetResourceShareAssociationsRequestRequestTypeDef,
-    GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
     GetResourceShareInvitationsRequestRequestTypeDef,
     TagFilterTypeDef,
     ListPendingInvitationResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListPermissionAssociationsRequestRequestTypeDef,
     ListPermissionVersionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
-    ListPrincipalsRequestListPrincipalsPaginateTypeDef,
     ListPrincipalsRequestRequestTypeDef,
     PrincipalTypeDef,
     ListReplacePermissionAssociationsWorkRequestRequestTypeDef,
     ReplacePermissionAssociationsWorkTypeDef,
     ListResourceSharePermissionsRequestRequestTypeDef,
     ListResourceTypesRequestRequestTypeDef,
     ServiceNameAndResourceTypeTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef,
-    PromoteResourceShareCreatedFromPolicyResponseTypeDef,
     RejectResourceShareInvitationRequestRequestTypeDef,
     ReplacePermissionAssociationsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     SetDefaultPermissionVersionRequestRequestTypeDef,
-    SetDefaultPermissionVersionResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateResourceShareRequestRequestTypeDef,
+    AssociateResourceSharePermissionResponseTypeDef,
+    DeletePermissionResponseTypeDef,
+    DeletePermissionVersionResponseTypeDef,
+    DeleteResourceShareResponseTypeDef,
+    DisassociateResourceSharePermissionResponseTypeDef,
+    EnableSharingWithAwsOrganizationResponseTypeDef,
+    GetResourcePoliciesResponseTypeDef,
+    PromoteResourceShareCreatedFromPolicyResponseTypeDef,
+    SetDefaultPermissionVersionResponseTypeDef,
     AssociateResourceShareResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     ResourceShareInvitationTypeDef,
     ListPermissionAssociationsResponseTypeDef,
     CreatePermissionRequestRequestTypeDef,
     CreateResourceShareRequestRequestTypeDef,
-    ResourceSharePermissionDetailTypeDef,
-    ResourceSharePermissionSummaryTypeDef,
-    ResourceShareTypeDef,
     TagResourceRequestRequestTypeDef,
+    GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
+    GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
+    GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
+    ListPrincipalsRequestListPrincipalsPaginateTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
     GetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     GetResourceSharesRequestRequestTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListPrincipalsResponseTypeDef,
     ListReplacePermissionAssociationsWorkResponseTypeDef,
     ReplacePermissionAssociationsResponseTypeDef,
     ListResourceTypesResponseTypeDef,
+    ResourceSharePermissionDetailTypeDef,
+    ResourceSharePermissionSummaryTypeDef,
+    ResourceShareTypeDef,
     AcceptResourceShareInvitationResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
     CreatePermissionVersionResponseTypeDef,
     GetPermissionResponseTypeDef,
     CreatePermissionResponseTypeDef,
     ListPermissionVersionsResponseTypeDef,
```

### Comparing `mypy-boto3-ram-1.28.0/mypy_boto3_ram.egg-info/SOURCES.txt` & `mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.0/setup.py` & `mypy-boto3-ram-1.28.12/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ram",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ram"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RAM 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.RAM 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

