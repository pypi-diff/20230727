# Comparing `tmp/mypy-boto3-sso-admin-1.28.0.tar.gz` & `tmp/mypy-boto3-sso-admin-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sso-admin-1.28.0.tar", last modified: Thu Jul  6 21:00:43 2023, max compression
+gzip compressed data, was "mypy-boto3-sso-admin-1.28.12.tar", last modified: Thu Jul 27 11:49:43 2023, max compression
```

## Comparing `mypy-boto3-sso-admin-1.28.0.tar` & `mypy-boto3-sso-admin-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:43.054442 mypy-boto3-sso-admin-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-07-06 21:00:43.050442 mypy-boto3-sso-admin-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18871 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:43.042442 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34841 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34786 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39832 2023-07-06 20:56:44.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39783 2023-07-06 20:56:44.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:43.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:43.050442 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-07-06 21:00:42.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 21:00:42.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:42.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:42.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:42.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 21:00:42.000000 mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:43.054442 mypy-boto3-sso-admin-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-06 20:56:42.000000 mypy-boto3-sso-admin-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.753340 mypy-boto3-sso-admin-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20614 2023-07-27 11:49:43.753340 mypy-boto3-sso-admin-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19120 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.753340 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34841 2023-07-27 11:47:37.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34786 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-07-27 11:47:37.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-07-27 11:47:37.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-07-27 11:47:37.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-07-27 11:47:37.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41509 2023-07-27 11:47:38.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41458 2023-07-27 11:47:37.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.753340 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20614 2023-07-27 11:49:43.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 11:49:43.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:43.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 11:49:43.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:43.753340 mypy-boto3-sso-admin-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/setup.py
```

### Comparing `mypy-boto3-sso-admin-1.28.0/LICENSE` & `mypy-boto3-sso-admin-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.0/PKG-INFO` & `mypy-boto3-sso-admin-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-admin
-Version: 1.28.0
-Summary: Type annotations for boto3.SSOAdmin 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SSOAdmin 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sso-admin"></a>
 
 # mypy-boto3-sso-admin
 
 [![PyPI - mypy-boto3-sso-admin](https://img.shields.io/pypi/v/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso-admin?color=blue)](https://pypistats.org/packages/mypy-boto3-sso-admin)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso-admin)](https://pepy.tech/project/mypy-boto3-sso-admin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOAdmin 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
+[boto3.SSOAdmin 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
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
 [mypy-boto3-sso-admin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -376,105 +376,111 @@
 ### Typed dictionaries
 
 `mypy_boto3_sso_admin.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso_admin.type_defs import (
+    AccessControlAttributeValueOutputTypeDef,
     AccessControlAttributeValueTypeDef,
     AccountAssignmentOperationStatusMetadataTypeDef,
     AccountAssignmentOperationStatusTypeDef,
     AccountAssignmentTypeDef,
     CustomerManagedPolicyReferenceTypeDef,
     AttachManagedPolicyToPermissionSetRequestRequestTypeDef,
     AttachedManagedPolicyTypeDef,
     CreateAccountAssignmentRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     PermissionSetTypeDef,
+    CustomerManagedPolicyReferenceOutputTypeDef,
     DeleteAccountAssignmentRequestRequestTypeDef,
     DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef,
     DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DeletePermissionSetRequestRequestTypeDef,
     DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef,
     DescribeAccountAssignmentCreationStatusRequestRequestTypeDef,
     DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DescribePermissionSetProvisioningStatusRequestRequestTypeDef,
     PermissionSetProvisioningStatusTypeDef,
     DescribePermissionSetRequestRequestTypeDef,
     DetachManagedPolicyFromPermissionSetRequestRequestTypeDef,
     GetInlinePolicyForPermissionSetRequestRequestTypeDef,
-    GetInlinePolicyForPermissionSetResponseTypeDef,
     GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef,
     InstanceMetadataTypeDef,
     OperationStatusFilterTypeDef,
-    ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountAssignmentsRequestRequestTypeDef,
-    ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
     ListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
-    ListAccountsForProvisionedPermissionSetResponseTypeDef,
-    ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
-    ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
     ListManagedPoliciesInPermissionSetRequestRequestTypeDef,
     PermissionSetProvisioningStatusMetadataTypeDef,
-    ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
     ListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
-    ListPermissionSetsProvisionedToAccountResponseTypeDef,
-    ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
     ListPermissionSetsRequestRequestTypeDef,
-    ListPermissionSetsResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     ProvisionPermissionSetRequestRequestTypeDef,
     PutInlinePolicyToPermissionSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePermissionSetRequestRequestTypeDef,
+    AccessControlAttributeOutputTypeDef,
     AccessControlAttributeTypeDef,
-    ListAccountAssignmentCreationStatusResponseTypeDef,
-    ListAccountAssignmentDeletionStatusResponseTypeDef,
+    AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
+    DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef,
+    PermissionsBoundaryTypeDef,
     CreateAccountAssignmentResponseTypeDef,
     DeleteAccountAssignmentResponseTypeDef,
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
+    GetInlinePolicyForPermissionSetResponseTypeDef,
+    ListAccountAssignmentCreationStatusResponseTypeDef,
+    ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
-    AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
-    DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef,
-    ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
-    PermissionsBoundaryTypeDef,
+    ListAccountsForProvisionedPermissionSetResponseTypeDef,
     ListManagedPoliciesInPermissionSetResponseTypeDef,
+    ListPermissionSetsProvisionedToAccountResponseTypeDef,
+    ListPermissionSetsResponseTypeDef,
     CreatePermissionSetRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreatePermissionSetResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
+    ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
+    PermissionsBoundaryOutputTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     ProvisionPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
-    ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
     ListAccountAssignmentCreationStatusRequestRequestTypeDef,
-    ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
     ListAccountAssignmentDeletionStatusRequestRequestTypeDef,
-    ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
     ListPermissionSetProvisioningStatusRequestRequestTypeDef,
+    ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+    ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
+    ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+    ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
+    ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
+    ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+    ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
+    ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
+    ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListPermissionSetProvisioningStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    InstanceAccessControlAttributeConfigurationOutputTypeDef,
     InstanceAccessControlAttributeConfigurationTypeDef,
-    GetPermissionsBoundaryForPermissionSetResponseTypeDef,
     PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef,
-    CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
+    GetPermissionsBoundaryForPermissionSetResponseTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
+    CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessControlAttributeValueTypeDef:
+def get_structure() -> AccessControlAttributeValueOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sso-admin-1.28.0/README.md` & `mypy-boto3-sso-admin-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sso-admin"></a>
 
 # mypy-boto3-sso-admin
 
 [![PyPI - mypy-boto3-sso-admin](https://img.shields.io/pypi/v/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso-admin?color=blue)](https://pypistats.org/packages/mypy-boto3-sso-admin)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso-admin)](https://pepy.tech/project/mypy-boto3-sso-admin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOAdmin 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
+[boto3.SSOAdmin 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
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
 [mypy-boto3-sso-admin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,105 +344,111 @@
 ### Typed dictionaries
 
 `mypy_boto3_sso_admin.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso_admin.type_defs import (
+    AccessControlAttributeValueOutputTypeDef,
     AccessControlAttributeValueTypeDef,
     AccountAssignmentOperationStatusMetadataTypeDef,
     AccountAssignmentOperationStatusTypeDef,
     AccountAssignmentTypeDef,
     CustomerManagedPolicyReferenceTypeDef,
     AttachManagedPolicyToPermissionSetRequestRequestTypeDef,
     AttachedManagedPolicyTypeDef,
     CreateAccountAssignmentRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     PermissionSetTypeDef,
+    CustomerManagedPolicyReferenceOutputTypeDef,
     DeleteAccountAssignmentRequestRequestTypeDef,
     DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef,
     DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DeletePermissionSetRequestRequestTypeDef,
     DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef,
     DescribeAccountAssignmentCreationStatusRequestRequestTypeDef,
     DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DescribePermissionSetProvisioningStatusRequestRequestTypeDef,
     PermissionSetProvisioningStatusTypeDef,
     DescribePermissionSetRequestRequestTypeDef,
     DetachManagedPolicyFromPermissionSetRequestRequestTypeDef,
     GetInlinePolicyForPermissionSetRequestRequestTypeDef,
-    GetInlinePolicyForPermissionSetResponseTypeDef,
     GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef,
     InstanceMetadataTypeDef,
     OperationStatusFilterTypeDef,
-    ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountAssignmentsRequestRequestTypeDef,
-    ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
     ListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
-    ListAccountsForProvisionedPermissionSetResponseTypeDef,
-    ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
-    ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
     ListManagedPoliciesInPermissionSetRequestRequestTypeDef,
     PermissionSetProvisioningStatusMetadataTypeDef,
-    ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
     ListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
-    ListPermissionSetsProvisionedToAccountResponseTypeDef,
-    ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
     ListPermissionSetsRequestRequestTypeDef,
-    ListPermissionSetsResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     ProvisionPermissionSetRequestRequestTypeDef,
     PutInlinePolicyToPermissionSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePermissionSetRequestRequestTypeDef,
+    AccessControlAttributeOutputTypeDef,
     AccessControlAttributeTypeDef,
-    ListAccountAssignmentCreationStatusResponseTypeDef,
-    ListAccountAssignmentDeletionStatusResponseTypeDef,
+    AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
+    DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef,
+    PermissionsBoundaryTypeDef,
     CreateAccountAssignmentResponseTypeDef,
     DeleteAccountAssignmentResponseTypeDef,
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
+    GetInlinePolicyForPermissionSetResponseTypeDef,
+    ListAccountAssignmentCreationStatusResponseTypeDef,
+    ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
-    AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
-    DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef,
-    ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
-    PermissionsBoundaryTypeDef,
+    ListAccountsForProvisionedPermissionSetResponseTypeDef,
     ListManagedPoliciesInPermissionSetResponseTypeDef,
+    ListPermissionSetsProvisionedToAccountResponseTypeDef,
+    ListPermissionSetsResponseTypeDef,
     CreatePermissionSetRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreatePermissionSetResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
+    ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
+    PermissionsBoundaryOutputTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     ProvisionPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
-    ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
     ListAccountAssignmentCreationStatusRequestRequestTypeDef,
-    ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
     ListAccountAssignmentDeletionStatusRequestRequestTypeDef,
-    ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
     ListPermissionSetProvisioningStatusRequestRequestTypeDef,
+    ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+    ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
+    ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+    ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
+    ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
+    ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+    ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
+    ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
+    ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListPermissionSetProvisioningStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    InstanceAccessControlAttributeConfigurationOutputTypeDef,
     InstanceAccessControlAttributeConfigurationTypeDef,
-    GetPermissionsBoundaryForPermissionSetResponseTypeDef,
     PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef,
-    CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
+    GetPermissionsBoundaryForPermissionSetResponseTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
+    CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessControlAttributeValueTypeDef:
+def get_structure() -> AccessControlAttributeValueOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/__init__.py` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/__init__.pyi` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/__main__.py` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSOAdmin 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SSOAdmin 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin\nOther"
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

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/client.py` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/client.pyi` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/literals.py` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,15 @@
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
@@ -280,26 +281,28 @@
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

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/literals.pyi` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,15 @@
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
@@ -278,26 +279,28 @@
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

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/paginator.py` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountAssignmentCreationStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentCreationStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountassignmentcreationstatuspaginator)
         """
 
 
@@ -111,15 +111,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountAssignmentDeletionStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentDeletionStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountassignmentdeletionstatuspaginator)
         """
 
 
@@ -131,15 +131,15 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         AccountId: str,
         PermissionSetArn: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountAssignmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountassignmentspaginator)
         """
 
 
@@ -151,15 +151,15 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         ProvisioningStatus: ProvisioningStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountsForProvisionedPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountsForProvisionedPermissionSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountsforprovisionedpermissionsetpaginator)
         """
 
 
@@ -170,30 +170,30 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListCustomerManagedPolicyReferencesInPermissionSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listcustomermanagedpolicyreferencesinpermissionsetpaginator)
         """
 
 
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listinstancespaginator)
         """
 
 
@@ -204,15 +204,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedPoliciesInPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListManagedPoliciesInPermissionSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listmanagedpoliciesinpermissionsetpaginator)
         """
 
 
@@ -223,30 +223,30 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPermissionSetProvisioningStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetProvisioningStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetprovisioningstatuspaginator)
         """
 
 
 class ListPermissionSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetspaginator)
     """
 
     def paginate(
-        self, *, InstanceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPermissionSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetspaginator)
         """
 
 
@@ -258,32 +258,28 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         AccountId: str,
         ProvisioningStatus: ProvisioningStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPermissionSetsProvisionedToAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetsProvisionedToAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetsprovisionedtoaccountpaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self,
-        *,
-        InstanceArn: str,
-        ResourceArn: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceArn: str, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/paginator.pyi` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountAssignmentCreationStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentCreationStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountassignmentcreationstatuspaginator)
         """
 
 class ListAccountAssignmentDeletionStatusPaginator(Paginator):
@@ -107,15 +107,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountAssignmentDeletionStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentDeletionStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountassignmentdeletionstatuspaginator)
         """
 
 class ListAccountAssignmentsPaginator(Paginator):
@@ -126,15 +126,15 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         AccountId: str,
         PermissionSetArn: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountAssignmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountassignmentspaginator)
         """
 
 class ListAccountsForProvisionedPermissionSetPaginator(Paginator):
@@ -145,15 +145,15 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
         ProvisioningStatus: ProvisioningStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccountsForProvisionedPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountsForProvisionedPermissionSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listaccountsforprovisionedpermissionsetpaginator)
         """
 
 class ListCustomerManagedPolicyReferencesInPermissionSetPaginator(Paginator):
@@ -163,29 +163,29 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListCustomerManagedPolicyReferencesInPermissionSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listcustomermanagedpolicyreferencesinpermissionsetpaginator)
         """
 
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listinstancespaginator)
         """
 
 class ListManagedPoliciesInPermissionSetPaginator(Paginator):
@@ -195,15 +195,15 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         PermissionSetArn: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedPoliciesInPermissionSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListManagedPoliciesInPermissionSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listmanagedpoliciesinpermissionsetpaginator)
         """
 
 class ListPermissionSetProvisioningStatusPaginator(Paginator):
@@ -213,29 +213,29 @@
     """
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         Filter: OperationStatusFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPermissionSetProvisioningStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetProvisioningStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetprovisioningstatuspaginator)
         """
 
 class ListPermissionSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetspaginator)
     """
 
     def paginate(
-        self, *, InstanceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPermissionSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetspaginator)
         """
 
 class ListPermissionSetsProvisionedToAccountPaginator(Paginator):
@@ -246,31 +246,27 @@
 
     def paginate(
         self,
         *,
         InstanceArn: str,
         AccountId: str,
         ProvisioningStatus: ProvisioningStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPermissionSetsProvisionedToAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetsProvisionedToAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listpermissionsetsprovisionedtoaccountpaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self,
-        *,
-        InstanceArn: str,
-        ResourceArn: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceArn: str, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/type_defs.py` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/type_defs.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for sso-admin service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_sso_admin.type_defs import AccessControlAttributeValueTypeDef
+    from mypy_boto3_sso_admin.type_defs import AccessControlAttributeValueOutputTypeDef
 
-    data: AccessControlAttributeValueTypeDef = {...}
+    data: AccessControlAttributeValueOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -30,103 +30,116 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AccessControlAttributeValueOutputTypeDef",
     "AccessControlAttributeValueTypeDef",
     "AccountAssignmentOperationStatusMetadataTypeDef",
     "AccountAssignmentOperationStatusTypeDef",
     "AccountAssignmentTypeDef",
     "CustomerManagedPolicyReferenceTypeDef",
     "AttachManagedPolicyToPermissionSetRequestRequestTypeDef",
     "AttachedManagedPolicyTypeDef",
     "CreateAccountAssignmentRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "PermissionSetTypeDef",
+    "CustomerManagedPolicyReferenceOutputTypeDef",
     "DeleteAccountAssignmentRequestRequestTypeDef",
     "DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef",
     "DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "DeletePermissionSetRequestRequestTypeDef",
     "DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef",
     "DescribeAccountAssignmentCreationStatusRequestRequestTypeDef",
     "DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef",
     "DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "DescribePermissionSetProvisioningStatusRequestRequestTypeDef",
     "PermissionSetProvisioningStatusTypeDef",
     "DescribePermissionSetRequestRequestTypeDef",
     "DetachManagedPolicyFromPermissionSetRequestRequestTypeDef",
     "GetInlinePolicyForPermissionSetRequestRequestTypeDef",
-    "GetInlinePolicyForPermissionSetResponseTypeDef",
     "GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef",
     "InstanceMetadataTypeDef",
     "OperationStatusFilterTypeDef",
-    "ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountAssignmentsRequestRequestTypeDef",
-    "ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
     "ListAccountsForProvisionedPermissionSetRequestRequestTypeDef",
-    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
-    "ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
     "ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
-    "ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
     "ListManagedPoliciesInPermissionSetRequestRequestTypeDef",
     "PermissionSetProvisioningStatusMetadataTypeDef",
-    "ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
     "ListPermissionSetsProvisionedToAccountRequestRequestTypeDef",
-    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
-    "ListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
     "ListPermissionSetsRequestRequestTypeDef",
-    "ListPermissionSetsResponseTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "ProvisionPermissionSetRequestRequestTypeDef",
     "PutInlinePolicyToPermissionSetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePermissionSetRequestRequestTypeDef",
+    "AccessControlAttributeOutputTypeDef",
     "AccessControlAttributeTypeDef",
-    "ListAccountAssignmentCreationStatusResponseTypeDef",
-    "ListAccountAssignmentDeletionStatusResponseTypeDef",
+    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
+    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
+    "PermissionsBoundaryTypeDef",
     "CreateAccountAssignmentResponseTypeDef",
     "DeleteAccountAssignmentResponseTypeDef",
     "DescribeAccountAssignmentCreationStatusResponseTypeDef",
     "DescribeAccountAssignmentDeletionStatusResponseTypeDef",
+    "GetInlinePolicyForPermissionSetResponseTypeDef",
+    "ListAccountAssignmentCreationStatusResponseTypeDef",
+    "ListAccountAssignmentDeletionStatusResponseTypeDef",
     "ListAccountAssignmentsResponseTypeDef",
-    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
-    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
-    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
-    "PermissionsBoundaryTypeDef",
+    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
     "ListManagedPoliciesInPermissionSetResponseTypeDef",
+    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
+    "ListPermissionSetsResponseTypeDef",
     "CreatePermissionSetRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreatePermissionSetResponseTypeDef",
     "DescribePermissionSetResponseTypeDef",
+    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
+    "PermissionsBoundaryOutputTypeDef",
     "DescribePermissionSetProvisioningStatusResponseTypeDef",
     "ProvisionPermissionSetResponseTypeDef",
     "ListInstancesResponseTypeDef",
-    "ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
     "ListAccountAssignmentCreationStatusRequestRequestTypeDef",
-    "ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
     "ListAccountAssignmentDeletionStatusRequestRequestTypeDef",
-    "ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     "ListPermissionSetProvisioningStatusRequestRequestTypeDef",
+    "ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
+    "ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
+    "ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
+    "ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
+    "ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
+    "ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+    "ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
+    "ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
+    "ListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListPermissionSetProvisioningStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "InstanceAccessControlAttributeConfigurationOutputTypeDef",
     "InstanceAccessControlAttributeConfigurationTypeDef",
-    "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
-    "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
+    "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
+    "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
 )
 
+AccessControlAttributeValueOutputTypeDef = TypedDict(
+    "AccessControlAttributeValueOutputTypeDef",
+    {
+        "Source": List[str],
+    },
+)
+
 AccessControlAttributeValueTypeDef = TypedDict(
     "AccessControlAttributeValueTypeDef",
     {
         "Source": Sequence[str],
     },
 )
 
@@ -214,14 +227,25 @@
         "TargetType": Literal["AWS_ACCOUNT"],
         "PermissionSetArn": str,
         "PrincipalType": PrincipalTypeType,
         "PrincipalId": str,
     },
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -235,14 +259,36 @@
         "CreatedDate": datetime,
         "SessionDuration": str,
         "RelayState": str,
     },
     total=False,
 )
 
+_RequiredCustomerManagedPolicyReferenceOutputTypeDef = TypedDict(
+    "_RequiredCustomerManagedPolicyReferenceOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCustomerManagedPolicyReferenceOutputTypeDef = TypedDict(
+    "_OptionalCustomerManagedPolicyReferenceOutputTypeDef",
+    {
+        "Path": str,
+    },
+    total=False,
+)
+
+
+class CustomerManagedPolicyReferenceOutputTypeDef(
+    _RequiredCustomerManagedPolicyReferenceOutputTypeDef,
+    _OptionalCustomerManagedPolicyReferenceOutputTypeDef,
+):
+    pass
+
+
 DeleteAccountAssignmentRequestRequestTypeDef = TypedDict(
     "DeleteAccountAssignmentRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "TargetId": str,
         "TargetType": Literal["AWS_ACCOUNT"],
         "PermissionSetArn": str,
@@ -347,22 +393,14 @@
     "GetInlinePolicyForPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
 
-GetInlinePolicyForPermissionSetResponseTypeDef = TypedDict(
-    "GetInlinePolicyForPermissionSetResponseTypeDef",
-    {
-        "InlinePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef = TypedDict(
     "GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -380,38 +418,24 @@
     "OperationStatusFilterTypeDef",
     {
         "Status": StatusValuesType,
     },
     total=False,
 )
 
-_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "AccountId": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef(
-    _RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
-    _OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAccountAssignmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountAssignmentsRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "AccountId": str,
         "PermissionSetArn": str,
     },
@@ -429,38 +453,14 @@
 class ListAccountAssignmentsRequestRequestTypeDef(
     _RequiredListAccountAssignmentsRequestRequestTypeDef,
     _OptionalListAccountAssignmentsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
-    "_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
-    "_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
-    {
-        "ProvisioningStatus": ProvisioningStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef(
-    _RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
-    _OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAccountsForProvisionedPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountsForProvisionedPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -478,46 +478,14 @@
 class ListAccountsForProvisionedPermissionSetRequestRequestTypeDef(
     _RequiredListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
     _OptionalListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
 ):
     pass
 
 
-ListAccountsForProvisionedPermissionSetResponseTypeDef = TypedDict(
-    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
-    {
-        "AccountIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
-    "_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
-    "_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef(
-    _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
-    _OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -534,54 +502,23 @@
 class ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef(
     _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
     _OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
 ):
     pass
 
 
-ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "ListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInstancesRequestRequestTypeDef = TypedDict(
     "ListInstancesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
-    "_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
-    "_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef(
-    _RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
-    _OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListManagedPoliciesInPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedPoliciesInPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -608,38 +545,14 @@
         "Status": StatusValuesType,
         "RequestId": str,
         "CreatedDate": datetime,
     },
     total=False,
 )
 
-_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
-    "_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "AccountId": str,
-    },
-)
-_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
-    "_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
-    {
-        "ProvisioningStatus": ProvisioningStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef(
-    _RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
-    _OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPermissionSetsProvisionedToAccountRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionSetsProvisionedToAccountRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "AccountId": str,
     },
 )
@@ -657,45 +570,14 @@
 class ListPermissionSetsProvisionedToAccountRequestRequestTypeDef(
     _RequiredListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
     _OptionalListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
 ):
     pass
 
 
-ListPermissionSetsProvisionedToAccountResponseTypeDef = TypedDict(
-    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
-    {
-        "NextToken": str,
-        "PermissionSets": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
-    "_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
-    {
-        "InstanceArn": str,
-    },
-)
-_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
-    "_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPermissionSetsRequestListPermissionSetsPaginateTypeDef(
-    _RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
-    _OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPermissionSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionSetsRequestRequestTypeDef",
     {
         "InstanceArn": str,
     },
 )
 _OptionalListPermissionSetsRequestRequestTypeDef = TypedDict(
@@ -711,46 +593,14 @@
 class ListPermissionSetsRequestRequestTypeDef(
     _RequiredListPermissionSetsRequestRequestTypeDef,
     _OptionalListPermissionSetsRequestRequestTypeDef,
 ):
     pass
 
 
-ListPermissionSetsResponseTypeDef = TypedDict(
-    "ListPermissionSetsResponseTypeDef",
-    {
-        "PermissionSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "ResourceArn": str,
     },
 )
@@ -766,22 +616,20 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 _RequiredProvisionPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
@@ -809,25 +657,14 @@
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
         "InlinePolicy": str,
     },
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
@@ -854,123 +691,157 @@
 class UpdatePermissionSetRequestRequestTypeDef(
     _RequiredUpdatePermissionSetRequestRequestTypeDef,
     _OptionalUpdatePermissionSetRequestRequestTypeDef,
 ):
     pass
 
 
+AccessControlAttributeOutputTypeDef = TypedDict(
+    "AccessControlAttributeOutputTypeDef",
+    {
+        "Key": str,
+        "Value": AccessControlAttributeValueOutputTypeDef,
+    },
+)
+
 AccessControlAttributeTypeDef = TypedDict(
     "AccessControlAttributeTypeDef",
     {
         "Key": str,
         "Value": AccessControlAttributeValueTypeDef,
     },
 )
 
-ListAccountAssignmentCreationStatusResponseTypeDef = TypedDict(
-    "ListAccountAssignmentCreationStatusResponseTypeDef",
+AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef = TypedDict(
+    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
     {
-        "AccountAssignmentsCreationStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
     },
 )
 
-ListAccountAssignmentDeletionStatusResponseTypeDef = TypedDict(
-    "ListAccountAssignmentDeletionStatusResponseTypeDef",
+DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef = TypedDict(
+    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
     {
-        "AccountAssignmentsDeletionStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
+    },
+)
+
+PermissionsBoundaryTypeDef = TypedDict(
+    "PermissionsBoundaryTypeDef",
+    {
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
+        "ManagedPolicyArn": str,
     },
+    total=False,
 )
 
 CreateAccountAssignmentResponseTypeDef = TypedDict(
     "CreateAccountAssignmentResponseTypeDef",
     {
         "AccountAssignmentCreationStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAccountAssignmentResponseTypeDef = TypedDict(
     "DeleteAccountAssignmentResponseTypeDef",
     {
         "AccountAssignmentDeletionStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountAssignmentCreationStatusResponseTypeDef = TypedDict(
     "DescribeAccountAssignmentCreationStatusResponseTypeDef",
     {
         "AccountAssignmentCreationStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountAssignmentDeletionStatusResponseTypeDef = TypedDict(
     "DescribeAccountAssignmentDeletionStatusResponseTypeDef",
     {
         "AccountAssignmentDeletionStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAccountAssignmentsResponseTypeDef = TypedDict(
-    "ListAccountAssignmentsResponseTypeDef",
+GetInlinePolicyForPermissionSetResponseTypeDef = TypedDict(
+    "GetInlinePolicyForPermissionSetResponseTypeDef",
     {
-        "AccountAssignments": List[AccountAssignmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "InlinePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef = TypedDict(
-    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
+ListAccountAssignmentCreationStatusResponseTypeDef = TypedDict(
+    "ListAccountAssignmentCreationStatusResponseTypeDef",
     {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
+        "AccountAssignmentsCreationStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef = TypedDict(
-    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
+ListAccountAssignmentDeletionStatusResponseTypeDef = TypedDict(
+    "ListAccountAssignmentDeletionStatusResponseTypeDef",
     {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
+        "AccountAssignmentsDeletionStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef = TypedDict(
-    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
+ListAccountAssignmentsResponseTypeDef = TypedDict(
+    "ListAccountAssignmentsResponseTypeDef",
     {
-        "CustomerManagedPolicyReferences": List[CustomerManagedPolicyReferenceTypeDef],
+        "AccountAssignments": List[AccountAssignmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PermissionsBoundaryTypeDef = TypedDict(
-    "PermissionsBoundaryTypeDef",
+ListAccountsForProvisionedPermissionSetResponseTypeDef = TypedDict(
+    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
     {
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
-        "ManagedPolicyArn": str,
+        "AccountIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListManagedPoliciesInPermissionSetResponseTypeDef = TypedDict(
     "ListManagedPoliciesInPermissionSetResponseTypeDef",
     {
         "AttachedManagedPolicies": List[AttachedManagedPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPermissionSetsProvisionedToAccountResponseTypeDef = TypedDict(
+    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
+    {
+        "NextToken": str,
+        "PermissionSets": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPermissionSetsResponseTypeDef = TypedDict(
+    "ListPermissionSetsResponseTypeDef",
+    {
+        "PermissionSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePermissionSetRequestRequestTypeDef",
     {
         "Name": str,
@@ -992,266 +863,462 @@
 class CreatePermissionSetRequestRequestTypeDef(
     _RequiredCreatePermissionSetRequestRequestTypeDef,
     _OptionalCreatePermissionSetRequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreatePermissionSetResponseTypeDef = TypedDict(
     "CreatePermissionSetResponseTypeDef",
     {
         "PermissionSet": PermissionSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePermissionSetResponseTypeDef = TypedDict(
     "DescribePermissionSetResponseTypeDef",
     {
         "PermissionSet": PermissionSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef = TypedDict(
+    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
+    {
+        "CustomerManagedPolicyReferences": List[CustomerManagedPolicyReferenceOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PermissionsBoundaryOutputTypeDef = TypedDict(
+    "PermissionsBoundaryOutputTypeDef",
+    {
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceOutputTypeDef,
+        "ManagedPolicyArn": str,
+    },
+    total=False,
+)
+
 DescribePermissionSetProvisioningStatusResponseTypeDef = TypedDict(
     "DescribePermissionSetProvisioningStatusResponseTypeDef",
     {
         "PermissionSetProvisioningStatus": PermissionSetProvisioningStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProvisionPermissionSetResponseTypeDef = TypedDict(
     "ProvisionPermissionSetResponseTypeDef",
     {
         "PermissionSetProvisioningStatus": PermissionSetProvisioningStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "Instances": List[InstanceMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
+_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef",
     {
         "InstanceArn": str,
     },
 )
-_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
+_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef",
     {
+        "MaxResults": int,
+        "NextToken": str,
         "Filter": OperationStatusFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef(
-    _RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
-    _OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+class ListAccountAssignmentCreationStatusRequestRequestTypeDef(
+    _RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef,
+    _OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef",
+_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef",
     {
         "InstanceArn": str,
     },
 )
-_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef",
+_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filter": OperationStatusFilterTypeDef,
     },
     total=False,
 )
 
 
-class ListAccountAssignmentCreationStatusRequestRequestTypeDef(
-    _RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef,
-    _OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef,
+class ListAccountAssignmentDeletionStatusRequestRequestTypeDef(
+    _RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef,
+    _OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef",
+    {
+        "InstanceArn": str,
+    },
+)
+_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "Filter": OperationStatusFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPermissionSetProvisioningStatusRequestRequestTypeDef(
+    _RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef,
+    _OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
+    {
+        "InstanceArn": str,
+    },
+)
+_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
+    {
+        "Filter": OperationStatusFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef(
+    _RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+    _OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
 ):
     pass
 
 
 _RequiredListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef = TypedDict(
     "_RequiredListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
     {
         "InstanceArn": str,
     },
 )
 _OptionalListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef = TypedDict(
     "_OptionalListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
     {
         "Filter": OperationStatusFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef(
     _RequiredListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
     _OptionalListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef",
+_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
     {
         "InstanceArn": str,
+        "AccountId": str,
+        "PermissionSetArn": str,
     },
 )
-_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef",
+_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
-        "Filter": OperationStatusFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListAccountAssignmentDeletionStatusRequestRequestTypeDef(
-    _RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef,
-    _OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef,
+class ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef(
+    _RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+    _OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
+    "_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
+    "_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
+    {
+        "ProvisioningStatus": ProvisioningStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef(
+    _RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
+    _OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
+    "_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
+    "_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef(
+    _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
+    _OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
+):
+    pass
+
+
+ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "ListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
+    "_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
+    "_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef(
+    _RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+    _OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
 ):
     pass
 
 
 _RequiredListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef = TypedDict(
     "_RequiredListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     {
         "InstanceArn": str,
     },
 )
 _OptionalListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef = TypedDict(
     "_OptionalListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     {
         "Filter": OperationStatusFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef(
     _RequiredListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
     _OptionalListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef",
+_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
+    "_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
     {
         "InstanceArn": str,
+        "AccountId": str,
     },
 )
-_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef",
+_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
+    "_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
-        "Filter": OperationStatusFilterTypeDef,
+        "ProvisioningStatus": ProvisioningStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListPermissionSetProvisioningStatusRequestRequestTypeDef(
-    _RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef,
-    _OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef,
+class ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef(
+    _RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
+    _OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
+    "_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
+    {
+        "InstanceArn": str,
+    },
+)
+_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
+    "_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPermissionSetsRequestListPermissionSetsPaginateTypeDef(
+    _RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
+    _OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
 
 ListPermissionSetProvisioningStatusResponseTypeDef = TypedDict(
     "ListPermissionSetProvisioningStatusResponseTypeDef",
     {
         "PermissionSetsProvisioningStatus": List[PermissionSetProvisioningStatusMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InstanceAccessControlAttributeConfigurationTypeDef = TypedDict(
-    "InstanceAccessControlAttributeConfigurationTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "AccessControlAttributes": Sequence[AccessControlAttributeTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetPermissionsBoundaryForPermissionSetResponseTypeDef = TypedDict(
-    "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
+InstanceAccessControlAttributeConfigurationOutputTypeDef = TypedDict(
+    "InstanceAccessControlAttributeConfigurationOutputTypeDef",
     {
-        "PermissionsBoundary": PermissionsBoundaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccessControlAttributes": List[AccessControlAttributeOutputTypeDef],
+    },
+)
+
+InstanceAccessControlAttributeConfigurationTypeDef = TypedDict(
+    "InstanceAccessControlAttributeConfigurationTypeDef",
+    {
+        "AccessControlAttributes": Sequence[AccessControlAttributeTypeDef],
     },
 )
 
 PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef = TypedDict(
     "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
         "PermissionsBoundary": PermissionsBoundaryTypeDef,
     },
 )
 
-CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
+GetPermissionsBoundaryForPermissionSetResponseTypeDef = TypedDict(
+    "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     {
-        "InstanceArn": str,
-        "InstanceAccessControlAttributeConfiguration": (
-            InstanceAccessControlAttributeConfigurationTypeDef
-        ),
+        "PermissionsBoundary": PermissionsBoundaryOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef = TypedDict(
     "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     {
         "Status": InstanceAccessControlAttributeConfigurationStatusType,
         "StatusReason": str,
         "InstanceAccessControlAttributeConfiguration": (
+            InstanceAccessControlAttributeConfigurationOutputTypeDef
+        ),
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
+    {
+        "InstanceArn": str,
+        "InstanceAccessControlAttributeConfiguration": (
             InstanceAccessControlAttributeConfigurationTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     {
         "InstanceArn": str,
```

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin/type_defs.pyi` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/type_defs.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for sso-admin service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_sso_admin.type_defs import AccessControlAttributeValueTypeDef
+    from mypy_boto3_sso_admin.type_defs import AccessControlAttributeValueOutputTypeDef
 
-    data: AccessControlAttributeValueTypeDef = {...}
+    data: AccessControlAttributeValueOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -29,103 +29,116 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AccessControlAttributeValueOutputTypeDef",
     "AccessControlAttributeValueTypeDef",
     "AccountAssignmentOperationStatusMetadataTypeDef",
     "AccountAssignmentOperationStatusTypeDef",
     "AccountAssignmentTypeDef",
     "CustomerManagedPolicyReferenceTypeDef",
     "AttachManagedPolicyToPermissionSetRequestRequestTypeDef",
     "AttachedManagedPolicyTypeDef",
     "CreateAccountAssignmentRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "PermissionSetTypeDef",
+    "CustomerManagedPolicyReferenceOutputTypeDef",
     "DeleteAccountAssignmentRequestRequestTypeDef",
     "DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef",
     "DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "DeletePermissionSetRequestRequestTypeDef",
     "DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef",
     "DescribeAccountAssignmentCreationStatusRequestRequestTypeDef",
     "DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef",
     "DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "DescribePermissionSetProvisioningStatusRequestRequestTypeDef",
     "PermissionSetProvisioningStatusTypeDef",
     "DescribePermissionSetRequestRequestTypeDef",
     "DetachManagedPolicyFromPermissionSetRequestRequestTypeDef",
     "GetInlinePolicyForPermissionSetRequestRequestTypeDef",
-    "GetInlinePolicyForPermissionSetResponseTypeDef",
     "GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef",
     "InstanceMetadataTypeDef",
     "OperationStatusFilterTypeDef",
-    "ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountAssignmentsRequestRequestTypeDef",
-    "ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
     "ListAccountsForProvisionedPermissionSetRequestRequestTypeDef",
-    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
-    "ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
     "ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
-    "ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
     "ListManagedPoliciesInPermissionSetRequestRequestTypeDef",
     "PermissionSetProvisioningStatusMetadataTypeDef",
-    "ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
     "ListPermissionSetsProvisionedToAccountRequestRequestTypeDef",
-    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
-    "ListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
     "ListPermissionSetsRequestRequestTypeDef",
-    "ListPermissionSetsResponseTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "ProvisionPermissionSetRequestRequestTypeDef",
     "PutInlinePolicyToPermissionSetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePermissionSetRequestRequestTypeDef",
+    "AccessControlAttributeOutputTypeDef",
     "AccessControlAttributeTypeDef",
-    "ListAccountAssignmentCreationStatusResponseTypeDef",
-    "ListAccountAssignmentDeletionStatusResponseTypeDef",
+    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
+    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
+    "PermissionsBoundaryTypeDef",
     "CreateAccountAssignmentResponseTypeDef",
     "DeleteAccountAssignmentResponseTypeDef",
     "DescribeAccountAssignmentCreationStatusResponseTypeDef",
     "DescribeAccountAssignmentDeletionStatusResponseTypeDef",
+    "GetInlinePolicyForPermissionSetResponseTypeDef",
+    "ListAccountAssignmentCreationStatusResponseTypeDef",
+    "ListAccountAssignmentDeletionStatusResponseTypeDef",
     "ListAccountAssignmentsResponseTypeDef",
-    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
-    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
-    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
-    "PermissionsBoundaryTypeDef",
+    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
     "ListManagedPoliciesInPermissionSetResponseTypeDef",
+    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
+    "ListPermissionSetsResponseTypeDef",
     "CreatePermissionSetRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreatePermissionSetResponseTypeDef",
     "DescribePermissionSetResponseTypeDef",
+    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
+    "PermissionsBoundaryOutputTypeDef",
     "DescribePermissionSetProvisioningStatusResponseTypeDef",
     "ProvisionPermissionSetResponseTypeDef",
     "ListInstancesResponseTypeDef",
-    "ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
     "ListAccountAssignmentCreationStatusRequestRequestTypeDef",
-    "ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
     "ListAccountAssignmentDeletionStatusRequestRequestTypeDef",
-    "ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     "ListPermissionSetProvisioningStatusRequestRequestTypeDef",
+    "ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
+    "ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
+    "ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
+    "ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
+    "ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
+    "ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+    "ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
+    "ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
+    "ListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListPermissionSetProvisioningStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "InstanceAccessControlAttributeConfigurationOutputTypeDef",
     "InstanceAccessControlAttributeConfigurationTypeDef",
-    "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
-    "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
+    "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
+    "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
 )
 
+AccessControlAttributeValueOutputTypeDef = TypedDict(
+    "AccessControlAttributeValueOutputTypeDef",
+    {
+        "Source": List[str],
+    },
+)
+
 AccessControlAttributeValueTypeDef = TypedDict(
     "AccessControlAttributeValueTypeDef",
     {
         "Source": Sequence[str],
     },
 )
 
@@ -211,14 +224,25 @@
         "TargetType": Literal["AWS_ACCOUNT"],
         "PermissionSetArn": str,
         "PrincipalType": PrincipalTypeType,
         "PrincipalId": str,
     },
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -232,14 +256,34 @@
         "CreatedDate": datetime,
         "SessionDuration": str,
         "RelayState": str,
     },
     total=False,
 )
 
+_RequiredCustomerManagedPolicyReferenceOutputTypeDef = TypedDict(
+    "_RequiredCustomerManagedPolicyReferenceOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCustomerManagedPolicyReferenceOutputTypeDef = TypedDict(
+    "_OptionalCustomerManagedPolicyReferenceOutputTypeDef",
+    {
+        "Path": str,
+    },
+    total=False,
+)
+
+class CustomerManagedPolicyReferenceOutputTypeDef(
+    _RequiredCustomerManagedPolicyReferenceOutputTypeDef,
+    _OptionalCustomerManagedPolicyReferenceOutputTypeDef,
+):
+    pass
+
 DeleteAccountAssignmentRequestRequestTypeDef = TypedDict(
     "DeleteAccountAssignmentRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "TargetId": str,
         "TargetType": Literal["AWS_ACCOUNT"],
         "PermissionSetArn": str,
@@ -344,22 +388,14 @@
     "GetInlinePolicyForPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
 
-GetInlinePolicyForPermissionSetResponseTypeDef = TypedDict(
-    "GetInlinePolicyForPermissionSetResponseTypeDef",
-    {
-        "InlinePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef = TypedDict(
     "GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -377,36 +413,24 @@
     "OperationStatusFilterTypeDef",
     {
         "Status": StatusValuesType,
     },
     total=False,
 )
 
-_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "AccountId": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef(
-    _RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
-    _OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAccountAssignmentsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountAssignmentsRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "AccountId": str,
         "PermissionSetArn": str,
     },
@@ -422,36 +446,14 @@
 
 class ListAccountAssignmentsRequestRequestTypeDef(
     _RequiredListAccountAssignmentsRequestRequestTypeDef,
     _OptionalListAccountAssignmentsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
-    "_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
-    "_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
-    {
-        "ProvisioningStatus": ProvisioningStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef(
-    _RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
-    _OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
-):
-    pass
-
 _RequiredListAccountsForProvisionedPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountsForProvisionedPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -467,44 +469,14 @@
 
 class ListAccountsForProvisionedPermissionSetRequestRequestTypeDef(
     _RequiredListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
     _OptionalListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
 ):
     pass
 
-ListAccountsForProvisionedPermissionSetResponseTypeDef = TypedDict(
-    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
-    {
-        "AccountIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
-    "_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
-    "_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef(
-    _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
-    _OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
-):
-    pass
-
 _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -519,52 +491,23 @@
 
 class ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef(
     _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
     _OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
 ):
     pass
 
-ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "ListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInstancesRequestRequestTypeDef = TypedDict(
     "ListInstancesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
-    "_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-    },
-)
-_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
-    "_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef(
-    _RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
-    _OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
-):
-    pass
-
 _RequiredListManagedPoliciesInPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredListManagedPoliciesInPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
     },
 )
@@ -589,36 +532,14 @@
         "Status": StatusValuesType,
         "RequestId": str,
         "CreatedDate": datetime,
     },
     total=False,
 )
 
-_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
-    "_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "AccountId": str,
-    },
-)
-_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
-    "_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
-    {
-        "ProvisioningStatus": ProvisioningStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef(
-    _RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
-    _OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
-):
-    pass
-
 _RequiredListPermissionSetsProvisionedToAccountRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionSetsProvisionedToAccountRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "AccountId": str,
     },
 )
@@ -634,43 +555,14 @@
 
 class ListPermissionSetsProvisionedToAccountRequestRequestTypeDef(
     _RequiredListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
     _OptionalListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
 ):
     pass
 
-ListPermissionSetsProvisionedToAccountResponseTypeDef = TypedDict(
-    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
-    {
-        "NextToken": str,
-        "PermissionSets": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
-    "_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
-    {
-        "InstanceArn": str,
-    },
-)
-_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
-    "_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPermissionSetsRequestListPermissionSetsPaginateTypeDef(
-    _RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
-    _OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPermissionSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionSetsRequestRequestTypeDef",
     {
         "InstanceArn": str,
     },
 )
 _OptionalListPermissionSetsRequestRequestTypeDef = TypedDict(
@@ -684,44 +576,14 @@
 
 class ListPermissionSetsRequestRequestTypeDef(
     _RequiredListPermissionSetsRequestRequestTypeDef,
     _OptionalListPermissionSetsRequestRequestTypeDef,
 ):
     pass
 
-ListPermissionSetsResponseTypeDef = TypedDict(
-    "ListPermissionSetsResponseTypeDef",
-    {
-        "PermissionSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "InstanceArn": str,
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "ResourceArn": str,
     },
 )
@@ -735,22 +597,20 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 _RequiredProvisionPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
@@ -776,25 +636,14 @@
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
         "InlinePolicy": str,
     },
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
@@ -819,123 +668,157 @@
 
 class UpdatePermissionSetRequestRequestTypeDef(
     _RequiredUpdatePermissionSetRequestRequestTypeDef,
     _OptionalUpdatePermissionSetRequestRequestTypeDef,
 ):
     pass
 
+AccessControlAttributeOutputTypeDef = TypedDict(
+    "AccessControlAttributeOutputTypeDef",
+    {
+        "Key": str,
+        "Value": AccessControlAttributeValueOutputTypeDef,
+    },
+)
+
 AccessControlAttributeTypeDef = TypedDict(
     "AccessControlAttributeTypeDef",
     {
         "Key": str,
         "Value": AccessControlAttributeValueTypeDef,
     },
 )
 
-ListAccountAssignmentCreationStatusResponseTypeDef = TypedDict(
-    "ListAccountAssignmentCreationStatusResponseTypeDef",
+AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef = TypedDict(
+    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
     {
-        "AccountAssignmentsCreationStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
     },
 )
 
-ListAccountAssignmentDeletionStatusResponseTypeDef = TypedDict(
-    "ListAccountAssignmentDeletionStatusResponseTypeDef",
+DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef = TypedDict(
+    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
     {
-        "AccountAssignmentsDeletionStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
     },
 )
 
+PermissionsBoundaryTypeDef = TypedDict(
+    "PermissionsBoundaryTypeDef",
+    {
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
+        "ManagedPolicyArn": str,
+    },
+    total=False,
+)
+
 CreateAccountAssignmentResponseTypeDef = TypedDict(
     "CreateAccountAssignmentResponseTypeDef",
     {
         "AccountAssignmentCreationStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAccountAssignmentResponseTypeDef = TypedDict(
     "DeleteAccountAssignmentResponseTypeDef",
     {
         "AccountAssignmentDeletionStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountAssignmentCreationStatusResponseTypeDef = TypedDict(
     "DescribeAccountAssignmentCreationStatusResponseTypeDef",
     {
         "AccountAssignmentCreationStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountAssignmentDeletionStatusResponseTypeDef = TypedDict(
     "DescribeAccountAssignmentDeletionStatusResponseTypeDef",
     {
         "AccountAssignmentDeletionStatus": AccountAssignmentOperationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAccountAssignmentsResponseTypeDef = TypedDict(
-    "ListAccountAssignmentsResponseTypeDef",
+GetInlinePolicyForPermissionSetResponseTypeDef = TypedDict(
+    "GetInlinePolicyForPermissionSetResponseTypeDef",
     {
-        "AccountAssignments": List[AccountAssignmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "InlinePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef = TypedDict(
-    "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
+ListAccountAssignmentCreationStatusResponseTypeDef = TypedDict(
+    "ListAccountAssignmentCreationStatusResponseTypeDef",
     {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
+        "AccountAssignmentsCreationStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef = TypedDict(
-    "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
+ListAccountAssignmentDeletionStatusResponseTypeDef = TypedDict(
+    "ListAccountAssignmentDeletionStatusResponseTypeDef",
     {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
+        "AccountAssignmentsDeletionStatus": List[AccountAssignmentOperationStatusMetadataTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef = TypedDict(
-    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
+ListAccountAssignmentsResponseTypeDef = TypedDict(
+    "ListAccountAssignmentsResponseTypeDef",
     {
-        "CustomerManagedPolicyReferences": List[CustomerManagedPolicyReferenceTypeDef],
+        "AccountAssignments": List[AccountAssignmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PermissionsBoundaryTypeDef = TypedDict(
-    "PermissionsBoundaryTypeDef",
+ListAccountsForProvisionedPermissionSetResponseTypeDef = TypedDict(
+    "ListAccountsForProvisionedPermissionSetResponseTypeDef",
     {
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceTypeDef,
-        "ManagedPolicyArn": str,
+        "AccountIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListManagedPoliciesInPermissionSetResponseTypeDef = TypedDict(
     "ListManagedPoliciesInPermissionSetResponseTypeDef",
     {
         "AttachedManagedPolicies": List[AttachedManagedPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPermissionSetsProvisionedToAccountResponseTypeDef = TypedDict(
+    "ListPermissionSetsProvisionedToAccountResponseTypeDef",
+    {
+        "NextToken": str,
+        "PermissionSets": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPermissionSetsResponseTypeDef = TypedDict(
+    "ListPermissionSetsResponseTypeDef",
+    {
+        "PermissionSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePermissionSetRequestRequestTypeDef",
     {
         "Name": str,
@@ -955,254 +838,436 @@
 
 class CreatePermissionSetRequestRequestTypeDef(
     _RequiredCreatePermissionSetRequestRequestTypeDef,
     _OptionalCreatePermissionSetRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreatePermissionSetResponseTypeDef = TypedDict(
     "CreatePermissionSetResponseTypeDef",
     {
         "PermissionSet": PermissionSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePermissionSetResponseTypeDef = TypedDict(
     "DescribePermissionSetResponseTypeDef",
     {
         "PermissionSet": PermissionSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef = TypedDict(
+    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
+    {
+        "CustomerManagedPolicyReferences": List[CustomerManagedPolicyReferenceOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PermissionsBoundaryOutputTypeDef = TypedDict(
+    "PermissionsBoundaryOutputTypeDef",
+    {
+        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceOutputTypeDef,
+        "ManagedPolicyArn": str,
     },
+    total=False,
 )
 
 DescribePermissionSetProvisioningStatusResponseTypeDef = TypedDict(
     "DescribePermissionSetProvisioningStatusResponseTypeDef",
     {
         "PermissionSetProvisioningStatus": PermissionSetProvisioningStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProvisionPermissionSetResponseTypeDef = TypedDict(
     "ProvisionPermissionSetResponseTypeDef",
     {
         "PermissionSetProvisioningStatus": PermissionSetProvisioningStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "Instances": List[InstanceMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
+_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef",
     {
         "InstanceArn": str,
     },
 )
-_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
+_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef",
     {
+        "MaxResults": int,
+        "NextToken": str,
         "Filter": OperationStatusFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef(
-    _RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
-    _OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+class ListAccountAssignmentCreationStatusRequestRequestTypeDef(
+    _RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef,
+    _OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef",
+_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef",
     {
         "InstanceArn": str,
     },
 )
-_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef",
+_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filter": OperationStatusFilterTypeDef,
     },
     total=False,
 )
 
-class ListAccountAssignmentCreationStatusRequestRequestTypeDef(
-    _RequiredListAccountAssignmentCreationStatusRequestRequestTypeDef,
-    _OptionalListAccountAssignmentCreationStatusRequestRequestTypeDef,
+class ListAccountAssignmentDeletionStatusRequestRequestTypeDef(
+    _RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef,
+    _OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef",
+    {
+        "InstanceArn": str,
+    },
+)
+_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "Filter": OperationStatusFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListPermissionSetProvisioningStatusRequestRequestTypeDef(
+    _RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef,
+    _OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
+    {
+        "InstanceArn": str,
+    },
+)
+_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
+    {
+        "Filter": OperationStatusFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef(
+    _RequiredListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+    _OptionalListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
 ):
     pass
 
 _RequiredListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef = TypedDict(
     "_RequiredListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
     {
         "InstanceArn": str,
     },
 )
 _OptionalListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef = TypedDict(
     "_OptionalListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef",
     {
         "Filter": OperationStatusFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef(
     _RequiredListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
     _OptionalListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
 ):
     pass
 
-_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef",
+_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
+    "_RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
     {
         "InstanceArn": str,
+        "AccountId": str,
+        "PermissionSetArn": str,
     },
 )
-_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef",
+_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = TypedDict(
+    "_OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
-        "Filter": OperationStatusFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListAccountAssignmentDeletionStatusRequestRequestTypeDef(
-    _RequiredListAccountAssignmentDeletionStatusRequestRequestTypeDef,
-    _OptionalListAccountAssignmentDeletionStatusRequestRequestTypeDef,
+class ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef(
+    _RequiredListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+    _OptionalListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+):
+    pass
+
+_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
+    "_RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = TypedDict(
+    "_OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef",
+    {
+        "ProvisioningStatus": ProvisioningStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef(
+    _RequiredListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
+    _OptionalListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
+):
+    pass
+
+_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
+    "_RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef = TypedDict(
+    "_OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef(
+    _RequiredListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
+    _OptionalListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
+):
+    pass
+
+ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "ListInstancesRequestListInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
+    "_RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+    },
+)
+_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = TypedDict(
+    "_OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef(
+    _RequiredListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+    _OptionalListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
 ):
     pass
 
 _RequiredListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef = TypedDict(
     "_RequiredListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     {
         "InstanceArn": str,
     },
 )
 _OptionalListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef = TypedDict(
     "_OptionalListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     {
         "Filter": OperationStatusFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef(
     _RequiredListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
     _OptionalListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
 ):
     pass
 
-_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef",
+_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
+    "_RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
     {
         "InstanceArn": str,
+        "AccountId": str,
     },
 )
-_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef",
+_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = TypedDict(
+    "_OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
-        "Filter": OperationStatusFilterTypeDef,
+        "ProvisioningStatus": ProvisioningStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListPermissionSetProvisioningStatusRequestRequestTypeDef(
-    _RequiredListPermissionSetProvisioningStatusRequestRequestTypeDef,
-    _OptionalListPermissionSetProvisioningStatusRequestRequestTypeDef,
+class ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef(
+    _RequiredListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
+    _OptionalListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
+):
+    pass
+
+_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
+    "_RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
+    {
+        "InstanceArn": str,
+    },
+)
+_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef = TypedDict(
+    "_OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPermissionSetsRequestListPermissionSetsPaginateTypeDef(
+    _RequiredListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
+    _OptionalListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "InstanceArn": str,
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
 ListPermissionSetProvisioningStatusResponseTypeDef = TypedDict(
     "ListPermissionSetProvisioningStatusResponseTypeDef",
     {
         "PermissionSetsProvisioningStatus": List[PermissionSetProvisioningStatusMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InstanceAccessControlAttributeConfigurationTypeDef = TypedDict(
-    "InstanceAccessControlAttributeConfigurationTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "AccessControlAttributes": Sequence[AccessControlAttributeTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetPermissionsBoundaryForPermissionSetResponseTypeDef = TypedDict(
-    "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
+InstanceAccessControlAttributeConfigurationOutputTypeDef = TypedDict(
+    "InstanceAccessControlAttributeConfigurationOutputTypeDef",
     {
-        "PermissionsBoundary": PermissionsBoundaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccessControlAttributes": List[AccessControlAttributeOutputTypeDef],
+    },
+)
+
+InstanceAccessControlAttributeConfigurationTypeDef = TypedDict(
+    "InstanceAccessControlAttributeConfigurationTypeDef",
+    {
+        "AccessControlAttributes": Sequence[AccessControlAttributeTypeDef],
     },
 )
 
 PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef = TypedDict(
     "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
         "PermissionsBoundary": PermissionsBoundaryTypeDef,
     },
 )
 
-CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
+GetPermissionsBoundaryForPermissionSetResponseTypeDef = TypedDict(
+    "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     {
-        "InstanceArn": str,
-        "InstanceAccessControlAttributeConfiguration": (
-            InstanceAccessControlAttributeConfigurationTypeDef
-        ),
+        "PermissionsBoundary": PermissionsBoundaryOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef = TypedDict(
     "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     {
         "Status": InstanceAccessControlAttributeConfigurationStatusType,
         "StatusReason": str,
         "InstanceAccessControlAttributeConfiguration": (
+            InstanceAccessControlAttributeConfigurationOutputTypeDef
+        ),
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
+    {
+        "InstanceArn": str,
+        "InstanceAccessControlAttributeConfiguration": (
             InstanceAccessControlAttributeConfigurationTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     {
         "InstanceArn": str,
```

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin.egg-info/PKG-INFO` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-admin
-Version: 1.28.0
-Summary: Type annotations for boto3.SSOAdmin 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SSOAdmin 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sso-admin"></a>
 
 # mypy-boto3-sso-admin
 
 [![PyPI - mypy-boto3-sso-admin](https://img.shields.io/pypi/v/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sso-admin?color=blue)](https://pypistats.org/packages/mypy-boto3-sso-admin)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso-admin)](https://pepy.tech/project/mypy-boto3-sso-admin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOAdmin 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
+[boto3.SSOAdmin 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
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
 [mypy-boto3-sso-admin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -376,105 +376,111 @@
 ### Typed dictionaries
 
 `mypy_boto3_sso_admin.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sso_admin.type_defs import (
+    AccessControlAttributeValueOutputTypeDef,
     AccessControlAttributeValueTypeDef,
     AccountAssignmentOperationStatusMetadataTypeDef,
     AccountAssignmentOperationStatusTypeDef,
     AccountAssignmentTypeDef,
     CustomerManagedPolicyReferenceTypeDef,
     AttachManagedPolicyToPermissionSetRequestRequestTypeDef,
     AttachedManagedPolicyTypeDef,
     CreateAccountAssignmentRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     PermissionSetTypeDef,
+    CustomerManagedPolicyReferenceOutputTypeDef,
     DeleteAccountAssignmentRequestRequestTypeDef,
     DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef,
     DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DeletePermissionSetRequestRequestTypeDef,
     DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef,
     DescribeAccountAssignmentCreationStatusRequestRequestTypeDef,
     DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DescribePermissionSetProvisioningStatusRequestRequestTypeDef,
     PermissionSetProvisioningStatusTypeDef,
     DescribePermissionSetRequestRequestTypeDef,
     DetachManagedPolicyFromPermissionSetRequestRequestTypeDef,
     GetInlinePolicyForPermissionSetRequestRequestTypeDef,
-    GetInlinePolicyForPermissionSetResponseTypeDef,
     GetPermissionsBoundaryForPermissionSetRequestRequestTypeDef,
     InstanceMetadataTypeDef,
     OperationStatusFilterTypeDef,
-    ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountAssignmentsRequestRequestTypeDef,
-    ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
     ListAccountsForProvisionedPermissionSetRequestRequestTypeDef,
-    ListAccountsForProvisionedPermissionSetResponseTypeDef,
-    ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
-    ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
     ListManagedPoliciesInPermissionSetRequestRequestTypeDef,
     PermissionSetProvisioningStatusMetadataTypeDef,
-    ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
     ListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
-    ListPermissionSetsProvisionedToAccountResponseTypeDef,
-    ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
     ListPermissionSetsRequestRequestTypeDef,
-    ListPermissionSetsResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     ProvisionPermissionSetRequestRequestTypeDef,
     PutInlinePolicyToPermissionSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePermissionSetRequestRequestTypeDef,
+    AccessControlAttributeOutputTypeDef,
     AccessControlAttributeTypeDef,
-    ListAccountAssignmentCreationStatusResponseTypeDef,
-    ListAccountAssignmentDeletionStatusResponseTypeDef,
+    AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
+    DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef,
+    PermissionsBoundaryTypeDef,
     CreateAccountAssignmentResponseTypeDef,
     DeleteAccountAssignmentResponseTypeDef,
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
+    GetInlinePolicyForPermissionSetResponseTypeDef,
+    ListAccountAssignmentCreationStatusResponseTypeDef,
+    ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
-    AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
-    DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef,
-    ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
-    PermissionsBoundaryTypeDef,
+    ListAccountsForProvisionedPermissionSetResponseTypeDef,
     ListManagedPoliciesInPermissionSetResponseTypeDef,
+    ListPermissionSetsProvisionedToAccountResponseTypeDef,
+    ListPermissionSetsResponseTypeDef,
     CreatePermissionSetRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreatePermissionSetResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
+    ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
+    PermissionsBoundaryOutputTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     ProvisionPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
-    ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
     ListAccountAssignmentCreationStatusRequestRequestTypeDef,
-    ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
     ListAccountAssignmentDeletionStatusRequestRequestTypeDef,
-    ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
     ListPermissionSetProvisioningStatusRequestRequestTypeDef,
+    ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
+    ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef,
+    ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef,
+    ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef,
+    ListCustomerManagedPolicyReferencesInPermissionSetRequestListCustomerManagedPolicyReferencesInPermissionSetPaginateTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
+    ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
+    ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
+    ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
+    ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListPermissionSetProvisioningStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    InstanceAccessControlAttributeConfigurationOutputTypeDef,
     InstanceAccessControlAttributeConfigurationTypeDef,
-    GetPermissionsBoundaryForPermissionSetResponseTypeDef,
     PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef,
-    CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
+    GetPermissionsBoundaryForPermissionSetResponseTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
+    CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessControlAttributeValueTypeDef:
+def get_structure() -> AccessControlAttributeValueOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sso-admin-1.28.0/mypy_boto3_sso_admin.egg-info/SOURCES.txt` & `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.0/setup.py` & `mypy-boto3-sso-admin-1.28.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sso-admin",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sso_admin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSOAdmin 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.SSOAdmin 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

