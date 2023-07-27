# Comparing `tmp/mypy-boto3-grafana-1.28.0.tar.gz` & `tmp/mypy-boto3-grafana-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-grafana-1.28.0.tar", last modified: Thu Jul  6 20:59:40 2023, max compression
+gzip compressed data, was "mypy-boto3-grafana-1.28.12.tar", last modified: Thu Jul 27 05:34:44 2023, max compression
```

## Comparing `mypy-boto3-grafana-1.28.0.tar` & `mypy-boto3-grafana-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.454314 mypy-boto3-grafana-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15067 2023-07-06 20:59:40.450314 mypy-boto3-grafana-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.446314 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-06 20:42:13.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-07-06 20:42:13.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19334 2023-07-06 20:42:13.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:40.450314 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15067 2023-07-06 20:59:40.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 20:59:40.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:40.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:40.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:40.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:59:40.000000 mypy-boto3-grafana-1.28.0/mypy_boto3_grafana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:40.454314 mypy-boto3-grafana-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:42:12.000000 mypy-boto3-grafana-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.632500 mypy-boto3-grafana-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-07-27 05:34:44.632500 mypy-boto3-grafana-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.632500 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-07-27 05:23:03.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-07-27 05:23:03.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-27 05:23:03.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-27 05:23:03.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22786 2023-07-27 05:23:03.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22759 2023-07-27 05:23:03.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.632500 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-07-27 05:34:44.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 05:34:44.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:44.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:44.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:44.632500 mypy-boto3-grafana-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/setup.py
```

### Comparing `mypy-boto3-grafana-1.28.0/LICENSE` & `mypy-boto3-grafana-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.0/PKG-INFO` & `mypy-boto3-grafana-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-grafana
-Version: 1.28.0
-Summary: Type annotations for boto3.ManagedGrafana 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ManagedGrafana 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-grafana"></a>
 
 # mypy-boto3-grafana
 
 [![PyPI - mypy-boto3-grafana](https://img.shields.io/pypi/v/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-grafana?color=blue)](https://pypistats.org/packages/mypy-boto3-grafana)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-grafana)](https://pepy.tech/project/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
 
@@ -278,21 +278,26 @@
 `mypy_boto3_grafana.paginator` module contains type annotations for all
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_grafana import ManagedGrafanaClient
-from mypy_boto3_grafana.paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from mypy_boto3_grafana.paginator import (
+    ListPermissionsPaginator,
+    ListVersionsPaginator,
+    ListWorkspacesPaginator,
+)
 
 client: ManagedGrafanaClient = Session().client("grafana")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
 list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
@@ -302,14 +307,15 @@
 ```python
 from mypy_boto3_grafana.literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     ListPermissionsPaginatorName,
+    ListVersionsPaginatorName,
     ListWorkspacesPaginatorName,
     NotificationDestinationTypeType,
     PermissionTypeType,
     RoleType,
     SamlConfigurationStatusType,
     UpdateActionType,
     UserTypeType,
@@ -331,14 +337,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_grafana.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_grafana.type_defs import (
+    AssertionAttributesOutputTypeDef,
     AssertionAttributesTypeDef,
     AssociateLicenseRequestRequestTypeDef,
     AwsSsoAuthenticationTypeDef,
     AuthenticationSummaryTypeDef,
     CreateWorkspaceApiKeyRequestRequestTypeDef,
     CreateWorkspaceApiKeyResponseTypeDef,
     NetworkAccessConfigurationTypeDef,
@@ -347,55 +354,65 @@
     DeleteWorkspaceApiKeyResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
     DescribeWorkspaceAuthenticationRequestRequestTypeDef,
     DescribeWorkspaceConfigurationRequestRequestTypeDef,
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceRequestRequestTypeDef,
     DisassociateLicenseRequestRequestTypeDef,
+    IdpMetadataOutputTypeDef,
     IdpMetadataTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListPermissionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListVersionsRequestListVersionsPaginateTypeDef,
+    ListVersionsRequestRequestTypeDef,
+    ListVersionsResponseTypeDef,
     ListWorkspacesRequestListWorkspacesPaginateTypeDef,
     ListWorkspacesRequestRequestTypeDef,
+    NetworkAccessConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
-    UserTypeDef,
+    UserOutputTypeDef,
     ResponseMetadataTypeDef,
+    RoleValuesOutputTypeDef,
     RoleValuesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UserTypeDef,
     UpdateWorkspaceConfigurationRequestRequestTypeDef,
+    VpcConfigurationOutputTypeDef,
     WorkspaceSummaryTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
-    WorkspaceDescriptionTypeDef,
     PermissionEntryTypeDef,
-    UpdateInstructionTypeDef,
+    UpdateInstructionOutputTypeDef,
+    SamlConfigurationOutputTypeDef,
     SamlConfigurationTypeDef,
+    UpdateInstructionTypeDef,
+    WorkspaceDescriptionTypeDef,
     ListWorkspacesResponseTypeDef,
+    ListPermissionsResponseTypeDef,
+    UpdateErrorTypeDef,
+    SamlAuthenticationTypeDef,
+    UpdateWorkspaceAuthenticationRequestRequestTypeDef,
+    UpdatePermissionsRequestRequestTypeDef,
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
-    ListPermissionsResponseTypeDef,
-    UpdateErrorTypeDef,
-    UpdatePermissionsRequestRequestTypeDef,
-    SamlAuthenticationTypeDef,
-    UpdateWorkspaceAuthenticationRequestRequestTypeDef,
     UpdatePermissionsResponseTypeDef,
     AuthenticationDescriptionTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
 )
 
 
-def get_structure() -> AssertionAttributesTypeDef:
+def get_structure() -> AssertionAttributesOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-grafana-1.28.0/README.md` & `mypy-boto3-grafana-1.28.12/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-grafana"></a>
 
 # mypy-boto3-grafana
 
 [![PyPI - mypy-boto3-grafana](https://img.shields.io/pypi/v/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-grafana?color=blue)](https://pypistats.org/packages/mypy-boto3-grafana)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-grafana)](https://pepy.tech/project/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
 
@@ -246,21 +246,26 @@
 `mypy_boto3_grafana.paginator` module contains type annotations for all
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_grafana import ManagedGrafanaClient
-from mypy_boto3_grafana.paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from mypy_boto3_grafana.paginator import (
+    ListPermissionsPaginator,
+    ListVersionsPaginator,
+    ListWorkspacesPaginator,
+)
 
 client: ManagedGrafanaClient = Session().client("grafana")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
 list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
@@ -270,14 +275,15 @@
 ```python
 from mypy_boto3_grafana.literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     ListPermissionsPaginatorName,
+    ListVersionsPaginatorName,
     ListWorkspacesPaginatorName,
     NotificationDestinationTypeType,
     PermissionTypeType,
     RoleType,
     SamlConfigurationStatusType,
     UpdateActionType,
     UserTypeType,
@@ -299,14 +305,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_grafana.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_grafana.type_defs import (
+    AssertionAttributesOutputTypeDef,
     AssertionAttributesTypeDef,
     AssociateLicenseRequestRequestTypeDef,
     AwsSsoAuthenticationTypeDef,
     AuthenticationSummaryTypeDef,
     CreateWorkspaceApiKeyRequestRequestTypeDef,
     CreateWorkspaceApiKeyResponseTypeDef,
     NetworkAccessConfigurationTypeDef,
@@ -315,55 +322,65 @@
     DeleteWorkspaceApiKeyResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
     DescribeWorkspaceAuthenticationRequestRequestTypeDef,
     DescribeWorkspaceConfigurationRequestRequestTypeDef,
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceRequestRequestTypeDef,
     DisassociateLicenseRequestRequestTypeDef,
+    IdpMetadataOutputTypeDef,
     IdpMetadataTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListPermissionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListVersionsRequestListVersionsPaginateTypeDef,
+    ListVersionsRequestRequestTypeDef,
+    ListVersionsResponseTypeDef,
     ListWorkspacesRequestListWorkspacesPaginateTypeDef,
     ListWorkspacesRequestRequestTypeDef,
+    NetworkAccessConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
-    UserTypeDef,
+    UserOutputTypeDef,
     ResponseMetadataTypeDef,
+    RoleValuesOutputTypeDef,
     RoleValuesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UserTypeDef,
     UpdateWorkspaceConfigurationRequestRequestTypeDef,
+    VpcConfigurationOutputTypeDef,
     WorkspaceSummaryTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
-    WorkspaceDescriptionTypeDef,
     PermissionEntryTypeDef,
-    UpdateInstructionTypeDef,
+    UpdateInstructionOutputTypeDef,
+    SamlConfigurationOutputTypeDef,
     SamlConfigurationTypeDef,
+    UpdateInstructionTypeDef,
+    WorkspaceDescriptionTypeDef,
     ListWorkspacesResponseTypeDef,
+    ListPermissionsResponseTypeDef,
+    UpdateErrorTypeDef,
+    SamlAuthenticationTypeDef,
+    UpdateWorkspaceAuthenticationRequestRequestTypeDef,
+    UpdatePermissionsRequestRequestTypeDef,
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
-    ListPermissionsResponseTypeDef,
-    UpdateErrorTypeDef,
-    UpdatePermissionsRequestRequestTypeDef,
-    SamlAuthenticationTypeDef,
-    UpdateWorkspaceAuthenticationRequestRequestTypeDef,
     UpdatePermissionsResponseTypeDef,
     AuthenticationDescriptionTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
 )
 
 
-def get_structure() -> AssertionAttributesTypeDef:
+def get_structure() -> AssertionAttributesOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/__init__.py` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,25 +4,33 @@
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_grafana import (
         Client,
         ListPermissionsPaginator,
+        ListVersionsPaginator,
         ListWorkspacesPaginator,
         ManagedGrafanaClient,
     )
 
     session = Session()
     client: ManagedGrafanaClient = session.client("grafana")
 
     list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+    list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
     list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
     ```
 """
 from .client import ManagedGrafanaClient
-from .paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from .paginator import ListPermissionsPaginator, ListVersionsPaginator, ListWorkspacesPaginator
 
 Client = ManagedGrafanaClient
 
 
-__all__ = ("Client", "ListPermissionsPaginator", "ListWorkspacesPaginator", "ManagedGrafanaClient")
+__all__ = (
+    "Client",
+    "ListPermissionsPaginator",
+    "ListVersionsPaginator",
+    "ListWorkspacesPaginator",
+    "ManagedGrafanaClient",
+)
```

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/__init__.pyi` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -4,24 +4,32 @@
 Usage::
 
     ```python
     from boto3.session import Session
     from mypy_boto3_grafana import (
         Client,
         ListPermissionsPaginator,
+        ListVersionsPaginator,
         ListWorkspacesPaginator,
         ManagedGrafanaClient,
     )
 
     session = Session()
     client: ManagedGrafanaClient = session.client("grafana")
 
     list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+    list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
     list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
     ```
 """
 from .client import ManagedGrafanaClient
-from .paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from .paginator import ListPermissionsPaginator, ListVersionsPaginator, ListWorkspacesPaginator
 
 Client = ManagedGrafanaClient
 
-__all__ = ("Client", "ListPermissionsPaginator", "ListWorkspacesPaginator", "ManagedGrafanaClient")
+__all__ = (
+    "Client",
+    "ListPermissionsPaginator",
+    "ListVersionsPaginator",
+    "ListWorkspacesPaginator",
+    "ManagedGrafanaClient",
+)
```

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/__main__.py` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedGrafana 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ManagedGrafana 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana\nOther"
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

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/client.py` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,28 @@
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     PermissionTypeType,
     UserTypeType,
 )
-from .paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from .paginator import ListPermissionsPaginator, ListVersionsPaginator, ListWorkspacesPaginator
 from .type_defs import (
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceApiKeyResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceApiKeyResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     NetworkAccessConfigurationTypeDef,
     SamlConfigurationTypeDef,
     UpdateInstructionTypeDef,
     UpdatePermissionsResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
@@ -252,14 +253,24 @@
         The `ListTagsForResource` operation returns the tags that are associated with
         the Amazon Managed Service for Grafana resource specified by the `resourceArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#list_tags_for_resource)
         """
 
+    def list_versions(
+        self, *, maxResults: int = ..., nextToken: str = ..., workspaceId: str = ...
+    ) -> ListVersionsResponseTypeDef:
+        """
+        Lists available versions of Grafana.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_versions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#list_versions)
+        """
+
     def list_workspaces(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListWorkspacesResponseTypeDef:
         """
         Returns a list of Amazon Managed Grafana workspaces in the account, with some
         information about each workspace.
 
@@ -333,15 +344,15 @@
         authenticates users from, using SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_workspace_authentication)
         """
 
     def update_workspace_configuration(
-        self, *, configuration: str, workspaceId: str
+        self, *, configuration: str, workspaceId: str, grafanaVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the configuration string for the given workspace See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/grafana-2020-08-18/UpdateWorkspaceConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_workspace_configuration)
@@ -353,12 +364,19 @@
     ) -> ListPermissionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(self, operation_name: Literal["list_versions"]) -> ListVersionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_workspaces"]) -> ListWorkspacesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/client.pyi` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,28 @@
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     PermissionTypeType,
     UserTypeType,
 )
-from .paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from .paginator import ListPermissionsPaginator, ListVersionsPaginator, ListWorkspacesPaginator
 from .type_defs import (
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceApiKeyResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceApiKeyResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     NetworkAccessConfigurationTypeDef,
     SamlConfigurationTypeDef,
     UpdateInstructionTypeDef,
     UpdatePermissionsResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
@@ -233,14 +234,23 @@
         """
         The `ListTagsForResource` operation returns the tags that are associated with
         the Amazon Managed Service for Grafana resource specified by the `resourceArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#list_tags_for_resource)
         """
+    def list_versions(
+        self, *, maxResults: int = ..., nextToken: str = ..., workspaceId: str = ...
+    ) -> ListVersionsResponseTypeDef:
+        """
+        Lists available versions of Grafana.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.list_versions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#list_versions)
+        """
     def list_workspaces(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListWorkspacesResponseTypeDef:
         """
         Returns a list of Amazon Managed Grafana workspaces in the account, with some
         information about each workspace.
 
@@ -308,15 +318,15 @@
         Use this operation to define the identity provider (IdP) that this workspace
         authenticates users from, using SAML.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_authentication)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_workspace_authentication)
         """
     def update_workspace_configuration(
-        self, *, configuration: str, workspaceId: str
+        self, *, configuration: str, workspaceId: str, grafanaVersion: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the configuration string for the given workspace See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/grafana-2020-08-18/UpdateWorkspaceConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.update_workspace_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#update_workspace_configuration)
@@ -326,12 +336,18 @@
         self, operation_name: Literal["list_permissions"]
     ) -> ListPermissionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
         """
     @overload
+    def get_paginator(self, operation_name: Literal["list_versions"]) -> ListVersionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
+        """
+    @overload
     def get_paginator(self, operation_name: Literal["list_workspaces"]) -> ListWorkspacesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/literals.py` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 __all__ = (
     "AccountAccessTypeType",
     "AuthenticationProviderTypesType",
     "DataSourceTypeType",
     "LicenseTypeType",
     "ListPermissionsPaginatorName",
+    "ListVersionsPaginatorName",
     "ListWorkspacesPaginatorName",
     "NotificationDestinationTypeType",
     "PermissionTypeType",
     "RoleType",
     "SamlConfigurationStatusType",
     "UpdateActionType",
     "UserTypeType",
@@ -52,14 +53,15 @@
     "SITEWISE",
     "TIMESTREAM",
     "TWINMAKER",
     "XRAY",
 ]
 LicenseTypeType = Literal["ENTERPRISE", "ENTERPRISE_FREE_TRIAL"]
 ListPermissionsPaginatorName = Literal["list_permissions"]
+ListVersionsPaginatorName = Literal["list_versions"]
 ListWorkspacesPaginatorName = Literal["list_workspaces"]
 NotificationDestinationTypeType = Literal["SNS"]
 PermissionTypeType = Literal["CUSTOMER_MANAGED", "SERVICE_MANAGED"]
 RoleType = Literal["ADMIN", "EDITOR", "VIEWER"]
 SamlConfigurationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
 UpdateActionType = Literal["ADD", "REVOKE"]
 UserTypeType = Literal["SSO_GROUP", "SSO_USER"]
@@ -71,14 +73,16 @@
     "DELETION_FAILED",
     "FAILED",
     "LICENSE_REMOVAL_FAILED",
     "UPDATE_FAILED",
     "UPDATING",
     "UPGRADE_FAILED",
     "UPGRADING",
+    "VERSION_UPDATE_FAILED",
+    "VERSION_UPDATING",
 ]
 ManagedGrafanaServiceName = Literal["grafana"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -192,14 +196,15 @@
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
@@ -278,26 +283,28 @@
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
@@ -437,15 +444,15 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-PaginatorName = Literal["list_permissions", "list_workspaces"]
+PaginatorName = Literal["list_permissions", "list_versions", "list_workspaces"]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
     "eu-west-1",
```

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/literals.pyi` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 __all__ = (
     "AccountAccessTypeType",
     "AuthenticationProviderTypesType",
     "DataSourceTypeType",
     "LicenseTypeType",
     "ListPermissionsPaginatorName",
+    "ListVersionsPaginatorName",
     "ListWorkspacesPaginatorName",
     "NotificationDestinationTypeType",
     "PermissionTypeType",
     "RoleType",
     "SamlConfigurationStatusType",
     "UpdateActionType",
     "UserTypeType",
@@ -50,14 +51,15 @@
     "SITEWISE",
     "TIMESTREAM",
     "TWINMAKER",
     "XRAY",
 ]
 LicenseTypeType = Literal["ENTERPRISE", "ENTERPRISE_FREE_TRIAL"]
 ListPermissionsPaginatorName = Literal["list_permissions"]
+ListVersionsPaginatorName = Literal["list_versions"]
 ListWorkspacesPaginatorName = Literal["list_workspaces"]
 NotificationDestinationTypeType = Literal["SNS"]
 PermissionTypeType = Literal["CUSTOMER_MANAGED", "SERVICE_MANAGED"]
 RoleType = Literal["ADMIN", "EDITOR", "VIEWER"]
 SamlConfigurationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
 UpdateActionType = Literal["ADD", "REVOKE"]
 UserTypeType = Literal["SSO_GROUP", "SSO_USER"]
@@ -69,14 +71,16 @@
     "DELETION_FAILED",
     "FAILED",
     "LICENSE_REMOVAL_FAILED",
     "UPDATE_FAILED",
     "UPDATING",
     "UPGRADE_FAILED",
     "UPGRADING",
+    "VERSION_UPDATE_FAILED",
+    "VERSION_UPDATING",
 ]
 ManagedGrafanaServiceName = Literal["grafana"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -190,14 +194,15 @@
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
@@ -276,26 +281,28 @@
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
@@ -435,15 +442,15 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-PaginatorName = Literal["list_permissions", "list_workspaces"]
+PaginatorName = Literal["list_permissions", "list_versions", "list_workspaces"]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "eu-central-1",
     "eu-west-1",
```

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/paginator.py` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/paginator.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,36 +7,39 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_grafana.client import ManagedGrafanaClient
     from mypy_boto3_grafana.paginator import (
         ListPermissionsPaginator,
+        ListVersionsPaginator,
         ListWorkspacesPaginator,
     )
 
     session = Session()
     client: ManagedGrafanaClient = session.client("grafana")
 
     list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+    list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
     list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import UserTypeType
 from .type_defs import (
     ListPermissionsResponseTypeDef,
+    ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
-__all__ = ("ListPermissionsPaginator", "ListWorkspacesPaginator")
+__all__ = ("ListPermissionsPaginator", "ListVersionsPaginator", "ListWorkspacesPaginator")
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
@@ -62,14 +65,29 @@
     ) -> _PageIterator[ListPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listpermissionspaginator)
         """
 
 
+class ListVersionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listversionspaginator)
+    """
+
+    def paginate(
+        self, *, workspaceId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListVersionsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listversionspaginator)
+        """
+
+
 class ListWorkspacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listworkspacespaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/paginator.pyi` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/paginator.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -7,36 +7,39 @@
 
     ```python
     from boto3.session import Session
 
     from mypy_boto3_grafana.client import ManagedGrafanaClient
     from mypy_boto3_grafana.paginator import (
         ListPermissionsPaginator,
+        ListVersionsPaginator,
         ListWorkspacesPaginator,
     )
 
     session = Session()
     client: ManagedGrafanaClient = session.client("grafana")
 
     list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+    list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
     list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
     ```
 """
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import UserTypeType
 from .type_defs import (
     ListPermissionsResponseTypeDef,
+    ListVersionsResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
-__all__ = ("ListPermissionsPaginator", "ListWorkspacesPaginator")
+__all__ = ("ListPermissionsPaginator", "ListVersionsPaginator", "ListWorkspacesPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -58,14 +61,28 @@
         PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listpermissionspaginator)
         """
 
+class ListVersionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listversionspaginator)
+    """
+
+    def paginate(
+        self, *, workspaceId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+    ) -> _PageIterator[ListVersionsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listversionspaginator)
+        """
+
 class ListWorkspacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listworkspacespaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/type_defs.py` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for grafana service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_grafana.type_defs import AssertionAttributesTypeDef
+    from mypy_boto3_grafana.type_defs import AssertionAttributesOutputTypeDef
 
-    data: AssertionAttributesTypeDef = {...}
+    data: AssertionAttributesOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -35,14 +35,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AssertionAttributesOutputTypeDef",
     "AssertionAttributesTypeDef",
     "AssociateLicenseRequestRequestTypeDef",
     "AwsSsoAuthenticationTypeDef",
     "AuthenticationSummaryTypeDef",
     "CreateWorkspaceApiKeyRequestRequestTypeDef",
     "CreateWorkspaceApiKeyResponseTypeDef",
     "NetworkAccessConfigurationTypeDef",
@@ -51,53 +52,76 @@
     "DeleteWorkspaceApiKeyResponseTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
     "DescribeWorkspaceAuthenticationRequestRequestTypeDef",
     "DescribeWorkspaceConfigurationRequestRequestTypeDef",
     "DescribeWorkspaceConfigurationResponseTypeDef",
     "DescribeWorkspaceRequestRequestTypeDef",
     "DisassociateLicenseRequestRequestTypeDef",
+    "IdpMetadataOutputTypeDef",
     "IdpMetadataTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ListVersionsRequestListVersionsPaginateTypeDef",
+    "ListVersionsRequestRequestTypeDef",
+    "ListVersionsResponseTypeDef",
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
+    "NetworkAccessConfigurationOutputTypeDef",
     "PaginatorConfigTypeDef",
-    "UserTypeDef",
+    "UserOutputTypeDef",
     "ResponseMetadataTypeDef",
+    "RoleValuesOutputTypeDef",
     "RoleValuesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UserTypeDef",
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "WorkspaceSummaryTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
-    "WorkspaceDescriptionTypeDef",
     "PermissionEntryTypeDef",
-    "UpdateInstructionTypeDef",
+    "UpdateInstructionOutputTypeDef",
+    "SamlConfigurationOutputTypeDef",
     "SamlConfigurationTypeDef",
+    "UpdateInstructionTypeDef",
+    "WorkspaceDescriptionTypeDef",
     "ListWorkspacesResponseTypeDef",
+    "ListPermissionsResponseTypeDef",
+    "UpdateErrorTypeDef",
+    "SamlAuthenticationTypeDef",
+    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
+    "UpdatePermissionsRequestRequestTypeDef",
     "AssociateLicenseResponseTypeDef",
     "CreateWorkspaceResponseTypeDef",
     "DeleteWorkspaceResponseTypeDef",
     "DescribeWorkspaceResponseTypeDef",
     "DisassociateLicenseResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
-    "ListPermissionsResponseTypeDef",
-    "UpdateErrorTypeDef",
-    "UpdatePermissionsRequestRequestTypeDef",
-    "SamlAuthenticationTypeDef",
-    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
     "UpdatePermissionsResponseTypeDef",
     "AuthenticationDescriptionTypeDef",
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     "UpdateWorkspaceAuthenticationResponseTypeDef",
 )
 
+AssertionAttributesOutputTypeDef = TypedDict(
+    "AssertionAttributesOutputTypeDef",
+    {
+        "email": str,
+        "groups": str,
+        "login": str,
+        "name": str,
+        "org": str,
+        "role": str,
+    },
+    total=False,
+)
+
 AssertionAttributesTypeDef = TypedDict(
     "AssertionAttributesTypeDef",
     {
         "email": str,
         "groups": str,
         "login": str,
         "name": str,
@@ -163,24 +187,24 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkAccessConfigurationTypeDef = TypedDict(
     "NetworkAccessConfigurationTypeDef",
     {
-        "prefixListIds": List[str],
-        "vpceIds": List[str],
+        "prefixListIds": Sequence[str],
+        "vpceIds": Sequence[str],
     },
 )
 
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
+        "securityGroupIds": Sequence[str],
+        "subnetIds": Sequence[str],
     },
 )
 
 DeleteWorkspaceApiKeyRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceApiKeyRequestRequestTypeDef",
     {
         "keyName": str,
@@ -218,14 +242,15 @@
     },
 )
 
 DescribeWorkspaceConfigurationResponseTypeDef = TypedDict(
     "DescribeWorkspaceConfigurationResponseTypeDef",
     {
         "configuration": str,
+        "grafanaVersion": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspaceRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceRequestRequestTypeDef",
     {
@@ -237,14 +262,23 @@
     "DisassociateLicenseRequestRequestTypeDef",
     {
         "licenseType": LicenseTypeType,
         "workspaceId": str,
     },
 )
 
+IdpMetadataOutputTypeDef = TypedDict(
+    "IdpMetadataOutputTypeDef",
+    {
+        "url": str,
+        "xml": str,
+    },
+    total=False,
+)
+
 IdpMetadataTypeDef = TypedDict(
     "IdpMetadataTypeDef",
     {
         "url": str,
         "xml": str,
     },
     total=False,
@@ -311,14 +345,42 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListVersionsRequestListVersionsPaginateTypeDef = TypedDict(
+    "ListVersionsRequestListVersionsPaginateTypeDef",
+    {
+        "workspaceId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListVersionsRequestRequestTypeDef = TypedDict(
+    "ListVersionsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "workspaceId": str,
+    },
+    total=False,
+)
+
+ListVersionsResponseTypeDef = TypedDict(
+    "ListVersionsResponseTypeDef",
+    {
+        "grafanaVersions": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListWorkspacesRequestListWorkspacesPaginateTypeDef = TypedDict(
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -328,26 +390,34 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+NetworkAccessConfigurationOutputTypeDef = TypedDict(
+    "NetworkAccessConfigurationOutputTypeDef",
+    {
+        "prefixListIds": List[str],
+        "vpceIds": List[str],
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-UserTypeDef = TypedDict(
-    "UserTypeDef",
+UserOutputTypeDef = TypedDict(
+    "UserOutputTypeDef",
     {
         "id": str,
         "type": UserTypeType,
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
@@ -357,23 +427,32 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RoleValuesTypeDef = TypedDict(
-    "RoleValuesTypeDef",
+RoleValuesOutputTypeDef = TypedDict(
+    "RoleValuesOutputTypeDef",
     {
         "admin": List[str],
         "editor": List[str],
     },
     total=False,
 )
 
+RoleValuesTypeDef = TypedDict(
+    "RoleValuesTypeDef",
+    {
+        "admin": Sequence[str],
+        "editor": Sequence[str],
+    },
+    total=False,
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -382,21 +461,52 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateWorkspaceConfigurationRequestRequestTypeDef",
+UserTypeDef = TypedDict(
+    "UserTypeDef",
+    {
+        "id": str,
+        "type": UserTypeType,
+    },
+)
+
+_RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef",
     {
         "configuration": str,
         "workspaceId": str,
     },
 )
+_OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef",
+    {
+        "grafanaVersion": str,
+    },
+    total=False,
+)
+
+
+class UpdateWorkspaceConfigurationRequestRequestTypeDef(
+    _RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef,
+    _OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
+    {
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
+    },
+)
 
 _RequiredWorkspaceSummaryTypeDef = TypedDict(
     "_RequiredWorkspaceSummaryTypeDef",
     {
         "authentication": AuthenticationSummaryTypeDef,
         "created": datetime,
         "endpoint": str,
@@ -488,151 +598,136 @@
 
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredWorkspaceDescriptionTypeDef = TypedDict(
-    "_RequiredWorkspaceDescriptionTypeDef",
+PermissionEntryTypeDef = TypedDict(
+    "PermissionEntryTypeDef",
     {
-        "authentication": AuthenticationSummaryTypeDef,
-        "created": datetime,
-        "dataSources": List[DataSourceTypeType],
-        "endpoint": str,
-        "grafanaVersion": str,
-        "id": str,
-        "modified": datetime,
-        "status": WorkspaceStatusType,
+        "role": RoleType,
+        "user": UserOutputTypeDef,
     },
 )
-_OptionalWorkspaceDescriptionTypeDef = TypedDict(
-    "_OptionalWorkspaceDescriptionTypeDef",
+
+UpdateInstructionOutputTypeDef = TypedDict(
+    "UpdateInstructionOutputTypeDef",
     {
-        "accountAccessType": AccountAccessTypeType,
-        "description": str,
-        "freeTrialConsumed": bool,
-        "freeTrialExpiration": datetime,
-        "licenseExpiration": datetime,
-        "licenseType": LicenseTypeType,
-        "name": str,
-        "networkAccessControl": NetworkAccessConfigurationTypeDef,
-        "notificationDestinations": List[Literal["SNS"]],
-        "organizationRoleName": str,
-        "organizationalUnits": List[str],
-        "permissionType": PermissionTypeType,
-        "stackSetName": str,
-        "tags": Dict[str, str],
-        "vpcConfiguration": VpcConfigurationTypeDef,
-        "workspaceRoleArn": str,
+        "action": UpdateActionType,
+        "role": RoleType,
+        "users": List[UserOutputTypeDef],
     },
-    total=False,
 )
 
-
-class WorkspaceDescriptionTypeDef(
-    _RequiredWorkspaceDescriptionTypeDef, _OptionalWorkspaceDescriptionTypeDef
-):
-    pass
-
-
-PermissionEntryTypeDef = TypedDict(
-    "PermissionEntryTypeDef",
+_RequiredSamlConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSamlConfigurationOutputTypeDef",
     {
-        "role": RoleType,
-        "user": UserTypeDef,
+        "idpMetadata": IdpMetadataOutputTypeDef,
     },
 )
-
-UpdateInstructionTypeDef = TypedDict(
-    "UpdateInstructionTypeDef",
+_OptionalSamlConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSamlConfigurationOutputTypeDef",
     {
-        "action": UpdateActionType,
-        "role": RoleType,
-        "users": Sequence[UserTypeDef],
+        "allowedOrganizations": List[str],
+        "assertionAttributes": AssertionAttributesOutputTypeDef,
+        "loginValidityDuration": int,
+        "roleValues": RoleValuesOutputTypeDef,
     },
+    total=False,
 )
 
+
+class SamlConfigurationOutputTypeDef(
+    _RequiredSamlConfigurationOutputTypeDef, _OptionalSamlConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredSamlConfigurationTypeDef = TypedDict(
     "_RequiredSamlConfigurationTypeDef",
     {
         "idpMetadata": IdpMetadataTypeDef,
     },
 )
 _OptionalSamlConfigurationTypeDef = TypedDict(
     "_OptionalSamlConfigurationTypeDef",
     {
-        "allowedOrganizations": List[str],
+        "allowedOrganizations": Sequence[str],
         "assertionAttributes": AssertionAttributesTypeDef,
         "loginValidityDuration": int,
         "roleValues": RoleValuesTypeDef,
     },
     total=False,
 )
 
 
 class SamlConfigurationTypeDef(
     _RequiredSamlConfigurationTypeDef, _OptionalSamlConfigurationTypeDef
 ):
     pass
 
 
-ListWorkspacesResponseTypeDef = TypedDict(
-    "ListWorkspacesResponseTypeDef",
+UpdateInstructionTypeDef = TypedDict(
+    "UpdateInstructionTypeDef",
     {
-        "nextToken": str,
-        "workspaces": List[WorkspaceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "action": UpdateActionType,
+        "role": RoleType,
+        "users": Sequence[UserTypeDef],
     },
 )
 
-AssociateLicenseResponseTypeDef = TypedDict(
-    "AssociateLicenseResponseTypeDef",
+_RequiredWorkspaceDescriptionTypeDef = TypedDict(
+    "_RequiredWorkspaceDescriptionTypeDef",
     {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "authentication": AuthenticationSummaryTypeDef,
+        "created": datetime,
+        "dataSources": List[DataSourceTypeType],
+        "endpoint": str,
+        "grafanaVersion": str,
+        "id": str,
+        "modified": datetime,
+        "status": WorkspaceStatusType,
     },
 )
-
-CreateWorkspaceResponseTypeDef = TypedDict(
-    "CreateWorkspaceResponseTypeDef",
+_OptionalWorkspaceDescriptionTypeDef = TypedDict(
+    "_OptionalWorkspaceDescriptionTypeDef",
     {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "accountAccessType": AccountAccessTypeType,
+        "description": str,
+        "freeTrialConsumed": bool,
+        "freeTrialExpiration": datetime,
+        "licenseExpiration": datetime,
+        "licenseType": LicenseTypeType,
+        "name": str,
+        "networkAccessControl": NetworkAccessConfigurationOutputTypeDef,
+        "notificationDestinations": List[Literal["SNS"]],
+        "organizationRoleName": str,
+        "organizationalUnits": List[str],
+        "permissionType": PermissionTypeType,
+        "stackSetName": str,
+        "tags": Dict[str, str],
+        "vpcConfiguration": VpcConfigurationOutputTypeDef,
+        "workspaceRoleArn": str,
     },
+    total=False,
 )
 
-DeleteWorkspaceResponseTypeDef = TypedDict(
-    "DeleteWorkspaceResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-DescribeWorkspaceResponseTypeDef = TypedDict(
-    "DescribeWorkspaceResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class WorkspaceDescriptionTypeDef(
+    _RequiredWorkspaceDescriptionTypeDef, _OptionalWorkspaceDescriptionTypeDef
+):
+    pass
 
-DisassociateLicenseResponseTypeDef = TypedDict(
-    "DisassociateLicenseResponseTypeDef",
-    {
-        "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-UpdateWorkspaceResponseTypeDef = TypedDict(
-    "UpdateWorkspaceResponseTypeDef",
+ListWorkspacesResponseTypeDef = TypedDict(
+    "ListWorkspacesResponseTypeDef",
     {
-        "workspace": WorkspaceDescriptionTypeDef,
+        "nextToken": str,
+        "workspaces": List[WorkspaceSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
@@ -641,38 +736,30 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateErrorTypeDef = TypedDict(
     "UpdateErrorTypeDef",
     {
-        "causedBy": UpdateInstructionTypeDef,
+        "causedBy": UpdateInstructionOutputTypeDef,
         "code": int,
         "message": str,
     },
 )
 
-UpdatePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdatePermissionsRequestRequestTypeDef",
-    {
-        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
-        "workspaceId": str,
-    },
-)
-
 _RequiredSamlAuthenticationTypeDef = TypedDict(
     "_RequiredSamlAuthenticationTypeDef",
     {
         "status": SamlConfigurationStatusType,
     },
 )
 _OptionalSamlAuthenticationTypeDef = TypedDict(
     "_OptionalSamlAuthenticationTypeDef",
     {
-        "configuration": SamlConfigurationTypeDef,
+        "configuration": SamlConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 
 class SamlAuthenticationTypeDef(
     _RequiredSamlAuthenticationTypeDef, _OptionalSamlAuthenticationTypeDef
@@ -699,14 +786,70 @@
 class UpdateWorkspaceAuthenticationRequestRequestTypeDef(
     _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef,
     _OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef,
 ):
     pass
 
 
+UpdatePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdatePermissionsRequestRequestTypeDef",
+    {
+        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
+        "workspaceId": str,
+    },
+)
+
+AssociateLicenseResponseTypeDef = TypedDict(
+    "AssociateLicenseResponseTypeDef",
+    {
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateWorkspaceResponseTypeDef = TypedDict(
+    "CreateWorkspaceResponseTypeDef",
+    {
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteWorkspaceResponseTypeDef = TypedDict(
+    "DeleteWorkspaceResponseTypeDef",
+    {
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeWorkspaceResponseTypeDef = TypedDict(
+    "DescribeWorkspaceResponseTypeDef",
+    {
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DisassociateLicenseResponseTypeDef = TypedDict(
+    "DisassociateLicenseResponseTypeDef",
+    {
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateWorkspaceResponseTypeDef = TypedDict(
+    "UpdateWorkspaceResponseTypeDef",
+    {
+        "workspace": WorkspaceDescriptionTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdatePermissionsResponseTypeDef = TypedDict(
     "UpdatePermissionsResponseTypeDef",
     {
         "errors": List[UpdateErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana/type_defs.pyi` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for grafana service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_grafana.type_defs import AssertionAttributesTypeDef
+    from mypy_boto3_grafana.type_defs import AssertionAttributesOutputTypeDef
 
-    data: AssertionAttributesTypeDef = {...}
+    data: AssertionAttributesOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -34,14 +34,15 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AssertionAttributesOutputTypeDef",
     "AssertionAttributesTypeDef",
     "AssociateLicenseRequestRequestTypeDef",
     "AwsSsoAuthenticationTypeDef",
     "AuthenticationSummaryTypeDef",
     "CreateWorkspaceApiKeyRequestRequestTypeDef",
     "CreateWorkspaceApiKeyResponseTypeDef",
     "NetworkAccessConfigurationTypeDef",
@@ -50,53 +51,76 @@
     "DeleteWorkspaceApiKeyResponseTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
     "DescribeWorkspaceAuthenticationRequestRequestTypeDef",
     "DescribeWorkspaceConfigurationRequestRequestTypeDef",
     "DescribeWorkspaceConfigurationResponseTypeDef",
     "DescribeWorkspaceRequestRequestTypeDef",
     "DisassociateLicenseRequestRequestTypeDef",
+    "IdpMetadataOutputTypeDef",
     "IdpMetadataTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ListVersionsRequestListVersionsPaginateTypeDef",
+    "ListVersionsRequestRequestTypeDef",
+    "ListVersionsResponseTypeDef",
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
+    "NetworkAccessConfigurationOutputTypeDef",
     "PaginatorConfigTypeDef",
-    "UserTypeDef",
+    "UserOutputTypeDef",
     "ResponseMetadataTypeDef",
+    "RoleValuesOutputTypeDef",
     "RoleValuesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UserTypeDef",
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "WorkspaceSummaryTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
-    "WorkspaceDescriptionTypeDef",
     "PermissionEntryTypeDef",
-    "UpdateInstructionTypeDef",
+    "UpdateInstructionOutputTypeDef",
+    "SamlConfigurationOutputTypeDef",
     "SamlConfigurationTypeDef",
+    "UpdateInstructionTypeDef",
+    "WorkspaceDescriptionTypeDef",
     "ListWorkspacesResponseTypeDef",
+    "ListPermissionsResponseTypeDef",
+    "UpdateErrorTypeDef",
+    "SamlAuthenticationTypeDef",
+    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
+    "UpdatePermissionsRequestRequestTypeDef",
     "AssociateLicenseResponseTypeDef",
     "CreateWorkspaceResponseTypeDef",
     "DeleteWorkspaceResponseTypeDef",
     "DescribeWorkspaceResponseTypeDef",
     "DisassociateLicenseResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
-    "ListPermissionsResponseTypeDef",
-    "UpdateErrorTypeDef",
-    "UpdatePermissionsRequestRequestTypeDef",
-    "SamlAuthenticationTypeDef",
-    "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
     "UpdatePermissionsResponseTypeDef",
     "AuthenticationDescriptionTypeDef",
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     "UpdateWorkspaceAuthenticationResponseTypeDef",
 )
 
+AssertionAttributesOutputTypeDef = TypedDict(
+    "AssertionAttributesOutputTypeDef",
+    {
+        "email": str,
+        "groups": str,
+        "login": str,
+        "name": str,
+        "org": str,
+        "role": str,
+    },
+    total=False,
+)
+
 AssertionAttributesTypeDef = TypedDict(
     "AssertionAttributesTypeDef",
     {
         "email": str,
         "groups": str,
         "login": str,
         "name": str,
@@ -160,24 +184,24 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NetworkAccessConfigurationTypeDef = TypedDict(
     "NetworkAccessConfigurationTypeDef",
     {
-        "prefixListIds": List[str],
-        "vpceIds": List[str],
+        "prefixListIds": Sequence[str],
+        "vpceIds": Sequence[str],
     },
 )
 
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
+        "securityGroupIds": Sequence[str],
+        "subnetIds": Sequence[str],
     },
 )
 
 DeleteWorkspaceApiKeyRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceApiKeyRequestRequestTypeDef",
     {
         "keyName": str,
@@ -215,14 +239,15 @@
     },
 )
 
 DescribeWorkspaceConfigurationResponseTypeDef = TypedDict(
     "DescribeWorkspaceConfigurationResponseTypeDef",
     {
         "configuration": str,
+        "grafanaVersion": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeWorkspaceRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceRequestRequestTypeDef",
     {
@@ -234,14 +259,23 @@
     "DisassociateLicenseRequestRequestTypeDef",
     {
         "licenseType": LicenseTypeType,
         "workspaceId": str,
     },
 )
 
+IdpMetadataOutputTypeDef = TypedDict(
+    "IdpMetadataOutputTypeDef",
+    {
+        "url": str,
+        "xml": str,
+    },
+    total=False,
+)
+
 IdpMetadataTypeDef = TypedDict(
     "IdpMetadataTypeDef",
     {
         "url": str,
         "xml": str,
     },
     total=False,
@@ -304,14 +338,42 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListVersionsRequestListVersionsPaginateTypeDef = TypedDict(
+    "ListVersionsRequestListVersionsPaginateTypeDef",
+    {
+        "workspaceId": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+ListVersionsRequestRequestTypeDef = TypedDict(
+    "ListVersionsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "workspaceId": str,
+    },
+    total=False,
+)
+
+ListVersionsResponseTypeDef = TypedDict(
+    "ListVersionsResponseTypeDef",
+    {
+        "grafanaVersions": List[str],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListWorkspacesRequestListWorkspacesPaginateTypeDef = TypedDict(
     "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -321,26 +383,34 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+NetworkAccessConfigurationOutputTypeDef = TypedDict(
+    "NetworkAccessConfigurationOutputTypeDef",
+    {
+        "prefixListIds": List[str],
+        "vpceIds": List[str],
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-UserTypeDef = TypedDict(
-    "UserTypeDef",
+UserOutputTypeDef = TypedDict(
+    "UserOutputTypeDef",
     {
         "id": str,
         "type": UserTypeType,
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
@@ -350,23 +420,32 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RoleValuesTypeDef = TypedDict(
-    "RoleValuesTypeDef",
+RoleValuesOutputTypeDef = TypedDict(
+    "RoleValuesOutputTypeDef",
     {
         "admin": List[str],
         "editor": List[str],
     },
     total=False,
 )
 
+RoleValuesTypeDef = TypedDict(
+    "RoleValuesTypeDef",
+    {
+        "admin": Sequence[str],
+        "editor": Sequence[str],
+    },
+    total=False,
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -375,21 +454,50 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdateWorkspaceConfigurationRequestRequestTypeDef",
+UserTypeDef = TypedDict(
+    "UserTypeDef",
+    {
+        "id": str,
+        "type": UserTypeType,
+    },
+)
+
+_RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef",
     {
         "configuration": str,
         "workspaceId": str,
     },
 )
+_OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef",
+    {
+        "grafanaVersion": str,
+    },
+    total=False,
+)
+
+class UpdateWorkspaceConfigurationRequestRequestTypeDef(
+    _RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef,
+    _OptionalUpdateWorkspaceConfigurationRequestRequestTypeDef,
+):
+    pass
+
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
+    {
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
+    },
+)
 
 _RequiredWorkspaceSummaryTypeDef = TypedDict(
     "_RequiredWorkspaceSummaryTypeDef",
     {
         "authentication": AuthenticationSummaryTypeDef,
         "created": datetime,
         "endpoint": str,
@@ -475,14 +583,84 @@
 )
 
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
+PermissionEntryTypeDef = TypedDict(
+    "PermissionEntryTypeDef",
+    {
+        "role": RoleType,
+        "user": UserOutputTypeDef,
+    },
+)
+
+UpdateInstructionOutputTypeDef = TypedDict(
+    "UpdateInstructionOutputTypeDef",
+    {
+        "action": UpdateActionType,
+        "role": RoleType,
+        "users": List[UserOutputTypeDef],
+    },
+)
+
+_RequiredSamlConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSamlConfigurationOutputTypeDef",
+    {
+        "idpMetadata": IdpMetadataOutputTypeDef,
+    },
+)
+_OptionalSamlConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSamlConfigurationOutputTypeDef",
+    {
+        "allowedOrganizations": List[str],
+        "assertionAttributes": AssertionAttributesOutputTypeDef,
+        "loginValidityDuration": int,
+        "roleValues": RoleValuesOutputTypeDef,
+    },
+    total=False,
+)
+
+class SamlConfigurationOutputTypeDef(
+    _RequiredSamlConfigurationOutputTypeDef, _OptionalSamlConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredSamlConfigurationTypeDef = TypedDict(
+    "_RequiredSamlConfigurationTypeDef",
+    {
+        "idpMetadata": IdpMetadataTypeDef,
+    },
+)
+_OptionalSamlConfigurationTypeDef = TypedDict(
+    "_OptionalSamlConfigurationTypeDef",
+    {
+        "allowedOrganizations": Sequence[str],
+        "assertionAttributes": AssertionAttributesTypeDef,
+        "loginValidityDuration": int,
+        "roleValues": RoleValuesTypeDef,
+    },
+    total=False,
+)
+
+class SamlConfigurationTypeDef(
+    _RequiredSamlConfigurationTypeDef, _OptionalSamlConfigurationTypeDef
+):
+    pass
+
+UpdateInstructionTypeDef = TypedDict(
+    "UpdateInstructionTypeDef",
+    {
+        "action": UpdateActionType,
+        "role": RoleType,
+        "users": Sequence[UserTypeDef],
+    },
+)
+
 _RequiredWorkspaceDescriptionTypeDef = TypedDict(
     "_RequiredWorkspaceDescriptionTypeDef",
     {
         "authentication": AuthenticationSummaryTypeDef,
         "created": datetime,
         "dataSources": List[DataSourceTypeType],
         "endpoint": str,
@@ -498,77 +676,104 @@
         "accountAccessType": AccountAccessTypeType,
         "description": str,
         "freeTrialConsumed": bool,
         "freeTrialExpiration": datetime,
         "licenseExpiration": datetime,
         "licenseType": LicenseTypeType,
         "name": str,
-        "networkAccessControl": NetworkAccessConfigurationTypeDef,
+        "networkAccessControl": NetworkAccessConfigurationOutputTypeDef,
         "notificationDestinations": List[Literal["SNS"]],
         "organizationRoleName": str,
         "organizationalUnits": List[str],
         "permissionType": PermissionTypeType,
         "stackSetName": str,
         "tags": Dict[str, str],
-        "vpcConfiguration": VpcConfigurationTypeDef,
+        "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "workspaceRoleArn": str,
     },
     total=False,
 )
 
 class WorkspaceDescriptionTypeDef(
     _RequiredWorkspaceDescriptionTypeDef, _OptionalWorkspaceDescriptionTypeDef
 ):
     pass
 
-PermissionEntryTypeDef = TypedDict(
-    "PermissionEntryTypeDef",
+ListWorkspacesResponseTypeDef = TypedDict(
+    "ListWorkspacesResponseTypeDef",
     {
-        "role": RoleType,
-        "user": UserTypeDef,
+        "nextToken": str,
+        "workspaces": List[WorkspaceSummaryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateInstructionTypeDef = TypedDict(
-    "UpdateInstructionTypeDef",
+ListPermissionsResponseTypeDef = TypedDict(
+    "ListPermissionsResponseTypeDef",
     {
-        "action": UpdateActionType,
-        "role": RoleType,
-        "users": Sequence[UserTypeDef],
+        "nextToken": str,
+        "permissions": List[PermissionEntryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredSamlConfigurationTypeDef = TypedDict(
-    "_RequiredSamlConfigurationTypeDef",
+UpdateErrorTypeDef = TypedDict(
+    "UpdateErrorTypeDef",
     {
-        "idpMetadata": IdpMetadataTypeDef,
+        "causedBy": UpdateInstructionOutputTypeDef,
+        "code": int,
+        "message": str,
     },
 )
-_OptionalSamlConfigurationTypeDef = TypedDict(
-    "_OptionalSamlConfigurationTypeDef",
+
+_RequiredSamlAuthenticationTypeDef = TypedDict(
+    "_RequiredSamlAuthenticationTypeDef",
     {
-        "allowedOrganizations": List[str],
-        "assertionAttributes": AssertionAttributesTypeDef,
-        "loginValidityDuration": int,
-        "roleValues": RoleValuesTypeDef,
+        "status": SamlConfigurationStatusType,
+    },
+)
+_OptionalSamlAuthenticationTypeDef = TypedDict(
+    "_OptionalSamlAuthenticationTypeDef",
+    {
+        "configuration": SamlConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-class SamlConfigurationTypeDef(
-    _RequiredSamlConfigurationTypeDef, _OptionalSamlConfigurationTypeDef
+class SamlAuthenticationTypeDef(
+    _RequiredSamlAuthenticationTypeDef, _OptionalSamlAuthenticationTypeDef
 ):
     pass
 
-ListWorkspacesResponseTypeDef = TypedDict(
-    "ListWorkspacesResponseTypeDef",
+_RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef",
     {
-        "nextToken": str,
-        "workspaces": List[WorkspaceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "authenticationProviders": Sequence[AuthenticationProviderTypesType],
+        "workspaceId": str,
+    },
+)
+_OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef",
+    {
+        "samlConfiguration": SamlConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateWorkspaceAuthenticationRequestRequestTypeDef(
+    _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef,
+    _OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef,
+):
+    pass
+
+UpdatePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdatePermissionsRequestRequestTypeDef",
+    {
+        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
+        "workspaceId": str,
     },
 )
 
 AssociateLicenseResponseTypeDef = TypedDict(
     "AssociateLicenseResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
@@ -612,80 +817,14 @@
     "UpdateWorkspaceResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPermissionsResponseTypeDef = TypedDict(
-    "ListPermissionsResponseTypeDef",
-    {
-        "nextToken": str,
-        "permissions": List[PermissionEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateErrorTypeDef = TypedDict(
-    "UpdateErrorTypeDef",
-    {
-        "causedBy": UpdateInstructionTypeDef,
-        "code": int,
-        "message": str,
-    },
-)
-
-UpdatePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdatePermissionsRequestRequestTypeDef",
-    {
-        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
-        "workspaceId": str,
-    },
-)
-
-_RequiredSamlAuthenticationTypeDef = TypedDict(
-    "_RequiredSamlAuthenticationTypeDef",
-    {
-        "status": SamlConfigurationStatusType,
-    },
-)
-_OptionalSamlAuthenticationTypeDef = TypedDict(
-    "_OptionalSamlAuthenticationTypeDef",
-    {
-        "configuration": SamlConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class SamlAuthenticationTypeDef(
-    _RequiredSamlAuthenticationTypeDef, _OptionalSamlAuthenticationTypeDef
-):
-    pass
-
-_RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef",
-    {
-        "authenticationProviders": Sequence[AuthenticationProviderTypesType],
-        "workspaceId": str,
-    },
-)
-_OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef",
-    {
-        "samlConfiguration": SamlConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class UpdateWorkspaceAuthenticationRequestRequestTypeDef(
-    _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef,
-    _OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef,
-):
-    pass
-
 UpdatePermissionsResponseTypeDef = TypedDict(
     "UpdatePermissionsResponseTypeDef",
     {
         "errors": List[UpdateErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana.egg-info/PKG-INFO` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-grafana
-Version: 1.28.0
-Summary: Type annotations for boto3.ManagedGrafana 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ManagedGrafana 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-grafana"></a>
 
 # mypy-boto3-grafana
 
 [![PyPI - mypy-boto3-grafana](https://img.shields.io/pypi/v/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-grafana?color=blue)](https://pypistats.org/packages/mypy-boto3-grafana)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-grafana)](https://pepy.tech/project/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
 
@@ -278,21 +278,26 @@
 `mypy_boto3_grafana.paginator` module contains type annotations for all
 paginators.
 
 ```python
 from boto3.session import Session
 
 from mypy_boto3_grafana import ManagedGrafanaClient
-from mypy_boto3_grafana.paginator import ListPermissionsPaginator, ListWorkspacesPaginator
+from mypy_boto3_grafana.paginator import (
+    ListPermissionsPaginator,
+    ListVersionsPaginator,
+    ListWorkspacesPaginator,
+)
 
 client: ManagedGrafanaClient = Session().client("grafana")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_permissions_paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
+list_versions_paginator: ListVersionsPaginator = client.get_paginator("list_versions")
 list_workspaces_paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
@@ -302,14 +307,15 @@
 ```python
 from mypy_boto3_grafana.literals import (
     AccountAccessTypeType,
     AuthenticationProviderTypesType,
     DataSourceTypeType,
     LicenseTypeType,
     ListPermissionsPaginatorName,
+    ListVersionsPaginatorName,
     ListWorkspacesPaginatorName,
     NotificationDestinationTypeType,
     PermissionTypeType,
     RoleType,
     SamlConfigurationStatusType,
     UpdateActionType,
     UserTypeType,
@@ -331,14 +337,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_grafana.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_grafana.type_defs import (
+    AssertionAttributesOutputTypeDef,
     AssertionAttributesTypeDef,
     AssociateLicenseRequestRequestTypeDef,
     AwsSsoAuthenticationTypeDef,
     AuthenticationSummaryTypeDef,
     CreateWorkspaceApiKeyRequestRequestTypeDef,
     CreateWorkspaceApiKeyResponseTypeDef,
     NetworkAccessConfigurationTypeDef,
@@ -347,55 +354,65 @@
     DeleteWorkspaceApiKeyResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
     DescribeWorkspaceAuthenticationRequestRequestTypeDef,
     DescribeWorkspaceConfigurationRequestRequestTypeDef,
     DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceRequestRequestTypeDef,
     DisassociateLicenseRequestRequestTypeDef,
+    IdpMetadataOutputTypeDef,
     IdpMetadataTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListPermissionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListVersionsRequestListVersionsPaginateTypeDef,
+    ListVersionsRequestRequestTypeDef,
+    ListVersionsResponseTypeDef,
     ListWorkspacesRequestListWorkspacesPaginateTypeDef,
     ListWorkspacesRequestRequestTypeDef,
+    NetworkAccessConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
-    UserTypeDef,
+    UserOutputTypeDef,
     ResponseMetadataTypeDef,
+    RoleValuesOutputTypeDef,
     RoleValuesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UserTypeDef,
     UpdateWorkspaceConfigurationRequestRequestTypeDef,
+    VpcConfigurationOutputTypeDef,
     WorkspaceSummaryTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
-    WorkspaceDescriptionTypeDef,
     PermissionEntryTypeDef,
-    UpdateInstructionTypeDef,
+    UpdateInstructionOutputTypeDef,
+    SamlConfigurationOutputTypeDef,
     SamlConfigurationTypeDef,
+    UpdateInstructionTypeDef,
+    WorkspaceDescriptionTypeDef,
     ListWorkspacesResponseTypeDef,
+    ListPermissionsResponseTypeDef,
+    UpdateErrorTypeDef,
+    SamlAuthenticationTypeDef,
+    UpdateWorkspaceAuthenticationRequestRequestTypeDef,
+    UpdatePermissionsRequestRequestTypeDef,
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
-    ListPermissionsResponseTypeDef,
-    UpdateErrorTypeDef,
-    UpdatePermissionsRequestRequestTypeDef,
-    SamlAuthenticationTypeDef,
-    UpdateWorkspaceAuthenticationRequestRequestTypeDef,
     UpdatePermissionsResponseTypeDef,
     AuthenticationDescriptionTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
 )
 
 
-def get_structure() -> AssertionAttributesTypeDef:
+def get_structure() -> AssertionAttributesOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-grafana-1.28.0/mypy_boto3_grafana.egg-info/SOURCES.txt` & `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.0/setup.py` & `mypy-boto3-grafana-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-grafana",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_grafana"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ManagedGrafana 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ManagedGrafana 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

