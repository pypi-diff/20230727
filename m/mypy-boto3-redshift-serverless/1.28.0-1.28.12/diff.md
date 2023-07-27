# Comparing `tmp/mypy-boto3-redshift-serverless-1.28.0.tar.gz` & `tmp/mypy-boto3-redshift-serverless-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-serverless-1.28.0.tar", last modified: Thu Jul  6 21:00:25 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-serverless-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
```

## Comparing `mypy-boto3-redshift-serverless-1.28.0.tar` & `mypy-boto3-redshift-serverless-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:25.454406 mypy-boto3-redshift-serverless-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:52:59.000000 mypy-boto3-redshift-serverless-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18352 2023-07-06 21:00:25.454406 mypy-boto3-redshift-serverless-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-07-06 20:52:59.000000 mypy-boto3-redshift-serverless-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:25.438406 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-06 20:52:59.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-06 20:52:59.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-06 20:52:59.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-07-06 20:53:00.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32938 2023-07-06 20:53:00.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-07-06 20:53:00.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-07-06 20:53:00.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-06 20:53:00.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-07-06 20:53:00.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:52:59.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33810 2023-07-06 20:53:01.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33779 2023-07-06 20:53:01.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:52:59.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:25.454406 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18352 2023-07-06 21:00:25.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 21:00:25.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:25.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:25.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:25.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 21:00:25.000000 mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:25.454406 mypy-boto3-redshift-serverless-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-06 20:52:59.000000 mypy-boto3-redshift-serverless-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.181212 mypy-boto3-redshift-serverless-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-07-27 11:49:30.181212 mypy-boto3-redshift-serverless-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.169212 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32938 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34089 2023-07-27 11:44:27.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34058 2023-07-27 11:44:27.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.181212 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-07-27 11:49:29.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-27 11:49:29.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:29.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:29.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:29.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 11:49:29.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.181212 mypy-boto3-redshift-serverless-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/setup.py
```

### Comparing `mypy-boto3-redshift-serverless-1.28.0/LICENSE` & `mypy-boto3-redshift-serverless-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.0/PKG-INFO` & `mypy-boto3-redshift-serverless-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-serverless
-Version: 1.28.0
-Summary: Type annotations for boto3.RedshiftServerless 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.RedshiftServerless 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-redshift-serverless"></a>
 
 # mypy-boto3-redshift-serverless
 
 [![PyPI - mypy-boto3-redshift-serverless](https://img.shields.io/pypi/v/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-serverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-serverless)](https://pepy.tech/project/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,75 +353,69 @@
 ### Typed dictionaries
 
 `mypy_boto3_redshift_serverless.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_serverless.type_defs import (
+    ConfigParameterOutputTypeDef,
     ConfigParameterTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     SnapshotTypeDef,
     CreateEndpointAccessRequestRequestTypeDef,
     NamespaceTypeDef,
     CreateUsageLimitRequestRequestTypeDef,
     UsageLimitTypeDef,
     DeleteEndpointAccessRequestRequestTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteUsageLimitRequestRequestTypeDef,
     DeleteWorkgroupRequestRequestTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     GetCredentialsRequestRequestTypeDef,
-    GetCredentialsResponseTypeDef,
     GetEndpointAccessRequestRequestTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetRecoveryPointRequestRequestTypeDef,
     RecoveryPointTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     ResourcePolicyTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetTableRestoreStatusRequestRequestTypeDef,
     TableRestoreStatusTypeDef,
     GetUsageLimitRequestRequestTypeDef,
     GetWorkgroupRequestRequestTypeDef,
-    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
-    ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
-    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
     ListRecoveryPointsRequestRequestTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
-    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
+    TagOutputTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
-    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     RestoreTableFromSnapshotRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEndpointAccessRequestRequestTypeDef,
     UpdateNamespaceRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateUsageLimitRequestRequestTypeDef,
     UpdateWorkgroupRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateWorkgroupRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    GetCredentialsResponseTypeDef,
     ConvertRecoveryPointToSnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     GetSnapshotResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateNamespaceResponseTypeDef,
@@ -439,14 +433,22 @@
     GetRecoveryPointResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     GetTableRestoreStatusResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
+    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
+    ListNamespacesRequestListNamespacesPaginateTypeDef,
+    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
+    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
+    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -456,15 +458,15 @@
     DeleteWorkgroupResponseTypeDef,
     GetWorkgroupResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
 
-def get_structure() -> ConfigParameterTypeDef:
+def get_structure() -> ConfigParameterOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-redshift-serverless-1.28.0/README.md` & `mypy-boto3-redshift-serverless-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-redshift-serverless"></a>
 
 # mypy-boto3-redshift-serverless
 
 [![PyPI - mypy-boto3-redshift-serverless](https://img.shields.io/pypi/v/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-serverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-serverless)](https://pepy.tech/project/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,75 +321,69 @@
 ### Typed dictionaries
 
 `mypy_boto3_redshift_serverless.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_serverless.type_defs import (
+    ConfigParameterOutputTypeDef,
     ConfigParameterTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     SnapshotTypeDef,
     CreateEndpointAccessRequestRequestTypeDef,
     NamespaceTypeDef,
     CreateUsageLimitRequestRequestTypeDef,
     UsageLimitTypeDef,
     DeleteEndpointAccessRequestRequestTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteUsageLimitRequestRequestTypeDef,
     DeleteWorkgroupRequestRequestTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     GetCredentialsRequestRequestTypeDef,
-    GetCredentialsResponseTypeDef,
     GetEndpointAccessRequestRequestTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetRecoveryPointRequestRequestTypeDef,
     RecoveryPointTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     ResourcePolicyTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetTableRestoreStatusRequestRequestTypeDef,
     TableRestoreStatusTypeDef,
     GetUsageLimitRequestRequestTypeDef,
     GetWorkgroupRequestRequestTypeDef,
-    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
-    ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
-    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
     ListRecoveryPointsRequestRequestTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
-    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
+    TagOutputTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
-    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     RestoreTableFromSnapshotRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEndpointAccessRequestRequestTypeDef,
     UpdateNamespaceRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateUsageLimitRequestRequestTypeDef,
     UpdateWorkgroupRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateWorkgroupRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    GetCredentialsResponseTypeDef,
     ConvertRecoveryPointToSnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     GetSnapshotResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateNamespaceResponseTypeDef,
@@ -407,14 +401,22 @@
     GetRecoveryPointResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     GetTableRestoreStatusResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
+    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
+    ListNamespacesRequestListNamespacesPaginateTypeDef,
+    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
+    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
+    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -424,15 +426,15 @@
     DeleteWorkgroupResponseTypeDef,
     GetWorkgroupResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
 
-def get_structure() -> ConfigParameterTypeDef:
+def get_structure() -> ConfigParameterOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/__init__.py` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/__init__.pyi` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/__main__.py` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RedshiftServerless 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.RedshiftServerless 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless\nOther"
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

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/client.py` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/client.pyi` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/literals.py` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,15 @@
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
@@ -258,26 +259,28 @@
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

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/literals.pyi` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/literals.pyi`

 * *Files 0% similar despite different names*

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

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/paginator.py` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,30 +76,30 @@
     """
 
     def paginate(
         self,
         *,
         vpcId: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEndpointAccessResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListEndpointAccess.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listendpointaccesspaginator)
         """
 
 
 class ListNamespacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listnamespacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listnamespacespaginator)
         """
 
 
@@ -112,15 +112,15 @@
     def paginate(
         self,
         *,
         endTime: Union[datetime, str] = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         startTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryPointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listrecoverypointspaginator)
         """
 
 
@@ -134,15 +134,15 @@
         self,
         *,
         endTime: Union[datetime, str] = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         ownerAccount: str = ...,
         startTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listsnapshotspaginator)
         """
 
 
@@ -153,15 +153,15 @@
     """
 
     def paginate(
         self,
         *,
         namespaceName: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTableRestoreStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListTableRestoreStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listtablerestorestatuspaginator)
         """
 
 
@@ -172,28 +172,28 @@
     """
 
     def paginate(
         self,
         *,
         resourceArn: str = ...,
         usageType: UsageLimitUsageTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsageLimitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListUsageLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listusagelimitspaginator)
         """
 
 
 class ListWorkgroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listworkgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkgroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listworkgroupspaginator)
         """
```

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/paginator.pyi` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -73,29 +73,29 @@
     """
 
     def paginate(
         self,
         *,
         vpcId: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEndpointAccessResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListEndpointAccess.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listendpointaccesspaginator)
         """
 
 class ListNamespacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listnamespacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNamespacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListNamespaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listnamespacespaginator)
         """
 
 class ListRecoveryPointsPaginator(Paginator):
@@ -107,15 +107,15 @@
     def paginate(
         self,
         *,
         endTime: Union[datetime, str] = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         startTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecoveryPointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListRecoveryPoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listrecoverypointspaginator)
         """
 
 class ListSnapshotsPaginator(Paginator):
@@ -128,15 +128,15 @@
         self,
         *,
         endTime: Union[datetime, str] = ...,
         namespaceArn: str = ...,
         namespaceName: str = ...,
         ownerAccount: str = ...,
         startTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listsnapshotspaginator)
         """
 
 class ListTableRestoreStatusPaginator(Paginator):
@@ -146,15 +146,15 @@
     """
 
     def paginate(
         self,
         *,
         namespaceName: str = ...,
         workgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTableRestoreStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListTableRestoreStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listtablerestorestatuspaginator)
         """
 
 class ListUsageLimitsPaginator(Paginator):
@@ -164,27 +164,27 @@
     """
 
     def paginate(
         self,
         *,
         resourceArn: str = ...,
         usageType: UsageLimitUsageTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsageLimitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListUsageLimits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listusagelimitspaginator)
         """
 
 class ListWorkgroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listworkgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkgroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless.Paginator.ListWorkgroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/paginators/#listworkgroupspaginator)
         """
```

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/type_defs.py` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for redshift-serverless service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_redshift_serverless.type_defs import ConfigParameterTypeDef
+    from mypy_boto3_redshift_serverless.type_defs import ConfigParameterOutputTypeDef
 
-    data: ConfigParameterTypeDef = {...}
+    data: ConfigParameterOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -28,75 +28,69 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ConfigParameterOutputTypeDef",
     "ConfigParameterTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "SnapshotTypeDef",
     "CreateEndpointAccessRequestRequestTypeDef",
     "NamespaceTypeDef",
     "CreateUsageLimitRequestRequestTypeDef",
     "UsageLimitTypeDef",
     "DeleteEndpointAccessRequestRequestTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
     "DeleteUsageLimitRequestRequestTypeDef",
     "DeleteWorkgroupRequestRequestTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "GetCredentialsRequestRequestTypeDef",
-    "GetCredentialsResponseTypeDef",
     "GetEndpointAccessRequestRequestTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetRecoveryPointRequestRequestTypeDef",
     "RecoveryPointTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetTableRestoreStatusRequestRequestTypeDef",
     "TableRestoreStatusTypeDef",
     "GetUsageLimitRequestRequestTypeDef",
     "GetWorkgroupRequestRequestTypeDef",
-    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEndpointAccessRequestRequestTypeDef",
-    "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
     "ListRecoveryPointsRequestRequestTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
     "ListTableRestoreStatusRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    "TagOutputTypeDef",
     "ListUsageLimitsRequestRequestTypeDef",
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
     "ListWorkgroupsRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "RestoreTableFromSnapshotRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEndpointAccessRequestRequestTypeDef",
     "UpdateNamespaceRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateUsageLimitRequestRequestTypeDef",
     "UpdateWorkgroupRequestRequestTypeDef",
     "ConvertRecoveryPointToSnapshotRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateWorkgroupRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "GetCredentialsResponseTypeDef",
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DeleteSnapshotResponseTypeDef",
     "GetSnapshotResponseTypeDef",
     "ListSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
     "CreateNamespaceResponseTypeDef",
@@ -114,14 +108,22 @@
     "GetRecoveryPointResponseTypeDef",
     "ListRecoveryPointsResponseTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
     "GetTableRestoreStatusResponseTypeDef",
     "ListTableRestoreStatusResponseTypeDef",
     "RestoreTableFromSnapshotResponseTypeDef",
+    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+    "ListNamespacesRequestListNamespacesPaginateTypeDef",
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "VpcEndpointTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "CreateEndpointAccessResponseTypeDef",
     "DeleteEndpointAccessResponseTypeDef",
     "GetEndpointAccessResponseTypeDef",
     "ListEndpointAccessResponseTypeDef",
@@ -130,14 +132,23 @@
     "CreateWorkgroupResponseTypeDef",
     "DeleteWorkgroupResponseTypeDef",
     "GetWorkgroupResponseTypeDef",
     "ListWorkgroupsResponseTypeDef",
     "UpdateWorkgroupResponseTypeDef",
 )
 
+ConfigParameterOutputTypeDef = TypedDict(
+    "ConfigParameterOutputTypeDef",
+    {
+        "parameterKey": str,
+        "parameterValue": str,
+    },
+    total=False,
+)
+
 ConfigParameterTypeDef = TypedDict(
     "ConfigParameterTypeDef",
     {
         "parameterKey": str,
         "parameterValue": str,
     },
     total=False,
@@ -147,14 +158,25 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
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
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "accountsWithProvisionedRestoreAccess": List[str],
         "accountsWithRestoreAccess": List[str],
         "actualIncrementalBackupSizeInMegaBytes": float,
         "adminUsername": str,
@@ -342,25 +364,14 @@
 
 class GetCredentialsRequestRequestTypeDef(
     _RequiredGetCredentialsRequestRequestTypeDef, _OptionalGetCredentialsRequestRequestTypeDef
 ):
     pass
 
 
-GetCredentialsResponseTypeDef = TypedDict(
-    "GetCredentialsResponseTypeDef",
-    {
-        "dbPassword": str,
-        "dbUser": str,
-        "expiration": datetime,
-        "nextRefreshTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEndpointAccessRequestRequestTypeDef = TypedDict(
     "GetEndpointAccessRequestRequestTypeDef",
     {
         "endpointName": str,
     },
 )
 
@@ -456,20 +467,20 @@
 GetWorkgroupRequestRequestTypeDef = TypedDict(
     "GetWorkgroupRequestRequestTypeDef",
     {
         "workgroupName": str,
     },
 )
 
-ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = TypedDict(
-    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "vpcId": str,
-        "workgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListEndpointAccessRequestRequestTypeDef = TypedDict(
     "ListEndpointAccessRequestRequestTypeDef",
     {
@@ -477,93 +488,50 @@
         "nextToken": str,
         "vpcId": str,
         "workgroupName": str,
     },
     total=False,
 )
 
-ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
-    "ListNamespacesRequestListNamespacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNamespacesRequestRequestTypeDef = TypedDict(
     "ListNamespacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
-        "namespaceName": str,
-        "startTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRecoveryPointsRequestRequestTypeDef = TypedDict(
     "ListRecoveryPointsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "maxResults": int,
         "namespaceArn": str,
         "namespaceName": str,
         "nextToken": str,
         "startTime": Union[datetime, str],
     },
     total=False,
 )
 
-ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
-        "namespaceName": str,
-        "ownerAccount": str,
-        "startTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSnapshotsRequestRequestTypeDef = TypedDict(
     "ListSnapshotsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "maxResults": int,
         "namespaceArn": str,
         "namespaceName": str,
         "nextToken": str,
         "ownerAccount": str,
         "startTime": Union[datetime, str],
     },
     total=False,
 )
 
-ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
-    {
-        "namespaceName": str,
-        "workgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTableRestoreStatusRequestRequestTypeDef = TypedDict(
     "ListTableRestoreStatusRequestRequestTypeDef",
     {
         "maxResults": int,
         "namespaceName": str,
         "nextToken": str,
         "workgroupName": str,
@@ -574,43 +542,33 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "resourceArn": str,
-        "usageType": UsageLimitUsageTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "key": str,
+        "value": str,
     },
-    total=False,
 )
 
 ListUsageLimitsRequestRequestTypeDef = TypedDict(
     "ListUsageLimitsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "resourceArn": str,
         "usageType": UsageLimitUsageTypeType,
     },
     total=False,
 )
 
-ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkgroupsRequestRequestTypeDef = TypedDict(
     "ListWorkgroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -623,43 +581,22 @@
         "networkInterfaceId": str,
         "privateIpAddress": str,
         "subnetId": str,
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
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
 RestoreFromRecoveryPointRequestRequestTypeDef = TypedDict(
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     {
         "namespaceName": str,
         "recoveryPointId": str,
         "workgroupName": str,
     },
@@ -946,235 +883,317 @@
 
 class CreateWorkgroupRequestRequestTypeDef(
     _RequiredCreateWorkgroupRequestRequestTypeDef, _OptionalCreateWorkgroupRequestRequestTypeDef
 ):
     pass
 
 
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
 
+GetCredentialsResponseTypeDef = TypedDict(
+    "GetCredentialsResponseTypeDef",
+    {
+        "dbPassword": str,
+        "dbUser": str,
+        "expiration": datetime,
+        "nextRefreshTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ConvertRecoveryPointToSnapshotResponseTypeDef = TypedDict(
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSnapshotResponseTypeDef = TypedDict(
     "CreateSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSnapshotResponseTypeDef = TypedDict(
     "DeleteSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotResponseTypeDef = TypedDict(
     "GetSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSnapshotsResponseTypeDef = TypedDict(
     "ListSnapshotsResponseTypeDef",
     {
         "nextToken": str,
         "snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSnapshotResponseTypeDef = TypedDict(
     "UpdateSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNamespaceResponseTypeDef = TypedDict(
     "CreateNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteNamespaceResponseTypeDef = TypedDict(
     "DeleteNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNamespaceResponseTypeDef = TypedDict(
     "GetNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "namespaces": List[NamespaceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreFromRecoveryPointResponseTypeDef = TypedDict(
     "RestoreFromRecoveryPointResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
         "recoveryPointId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreFromSnapshotResponseTypeDef = TypedDict(
     "RestoreFromSnapshotResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
         "ownerAccount": str,
         "snapshotName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNamespaceResponseTypeDef = TypedDict(
     "UpdateNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateUsageLimitResponseTypeDef = TypedDict(
     "CreateUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteUsageLimitResponseTypeDef = TypedDict(
     "DeleteUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUsageLimitResponseTypeDef = TypedDict(
     "GetUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsageLimitsResponseTypeDef = TypedDict(
     "ListUsageLimitsResponseTypeDef",
     {
         "nextToken": str,
         "usageLimits": List[UsageLimitTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUsageLimitResponseTypeDef = TypedDict(
     "UpdateUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecoveryPointResponseTypeDef = TypedDict(
     "GetRecoveryPointResponseTypeDef",
     {
         "recoveryPoint": RecoveryPointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryPointsResponseTypeDef = TypedDict(
     "ListRecoveryPointsResponseTypeDef",
     {
         "nextToken": str,
         "recoveryPoints": List[RecoveryPointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcePolicyResponseTypeDef = TypedDict(
     "GetResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourcePolicyResponseTypeDef = TypedDict(
     "PutResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTableRestoreStatusResponseTypeDef = TypedDict(
     "GetTableRestoreStatusResponseTypeDef",
     {
         "tableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTableRestoreStatusResponseTypeDef = TypedDict(
     "ListTableRestoreStatusResponseTypeDef",
     {
         "nextToken": str,
         "tableRestoreStatuses": List[TableRestoreStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableFromSnapshotResponseTypeDef = TypedDict(
     "RestoreTableFromSnapshotResponseTypeDef",
     {
         "tableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = TypedDict(
+    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+    {
+        "vpcId": str,
+        "workgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
+    "ListNamespacesRequestListNamespacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "namespaceArn": str,
+        "namespaceName": str,
+        "startTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ownerAccount": str,
+        "startTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+    {
+        "namespaceName": str,
+        "workgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "usageType": UsageLimitUsageTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "networkInterfaces": List[NetworkInterfaceTypeDef],
@@ -1211,56 +1230,56 @@
     total=False,
 )
 
 CreateEndpointAccessResponseTypeDef = TypedDict(
     "CreateEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEndpointAccessResponseTypeDef = TypedDict(
     "DeleteEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEndpointAccessResponseTypeDef = TypedDict(
     "GetEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEndpointAccessResponseTypeDef = TypedDict(
     "ListEndpointAccessResponseTypeDef",
     {
         "endpoints": List[EndpointAccessTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointAccessResponseTypeDef = TypedDict(
     "UpdateEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkgroupTypeDef = TypedDict(
     "WorkgroupTypeDef",
     {
         "baseCapacity": int,
-        "configParameters": List[ConfigParameterTypeDef],
+        "configParameters": List[ConfigParameterOutputTypeDef],
         "creationDate": datetime,
         "endpoint": EndpointTypeDef,
         "enhancedVpcRouting": bool,
         "namespaceName": str,
         "port": int,
         "publiclyAccessible": bool,
         "securityGroupIds": List[str],
@@ -1273,43 +1292,43 @@
     total=False,
 )
 
 CreateWorkgroupResponseTypeDef = TypedDict(
     "CreateWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteWorkgroupResponseTypeDef = TypedDict(
     "DeleteWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkgroupResponseTypeDef = TypedDict(
     "GetWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkgroupsResponseTypeDef = TypedDict(
     "ListWorkgroupsResponseTypeDef",
     {
         "nextToken": str,
         "workgroups": List[WorkgroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkgroupResponseTypeDef = TypedDict(
     "UpdateWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless/type_defs.pyi` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for redshift-serverless service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_redshift_serverless.type_defs import ConfigParameterTypeDef
+    from mypy_boto3_redshift_serverless.type_defs import ConfigParameterOutputTypeDef
 
-    data: ConfigParameterTypeDef = {...}
+    data: ConfigParameterOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -27,75 +27,69 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ConfigParameterOutputTypeDef",
     "ConfigParameterTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "SnapshotTypeDef",
     "CreateEndpointAccessRequestRequestTypeDef",
     "NamespaceTypeDef",
     "CreateUsageLimitRequestRequestTypeDef",
     "UsageLimitTypeDef",
     "DeleteEndpointAccessRequestRequestTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
     "DeleteUsageLimitRequestRequestTypeDef",
     "DeleteWorkgroupRequestRequestTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "GetCredentialsRequestRequestTypeDef",
-    "GetCredentialsResponseTypeDef",
     "GetEndpointAccessRequestRequestTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetRecoveryPointRequestRequestTypeDef",
     "RecoveryPointTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetTableRestoreStatusRequestRequestTypeDef",
     "TableRestoreStatusTypeDef",
     "GetUsageLimitRequestRequestTypeDef",
     "GetWorkgroupRequestRequestTypeDef",
-    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEndpointAccessRequestRequestTypeDef",
-    "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
     "ListRecoveryPointsRequestRequestTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
     "ListTableRestoreStatusRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    "TagOutputTypeDef",
     "ListUsageLimitsRequestRequestTypeDef",
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
     "ListWorkgroupsRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "RestoreTableFromSnapshotRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEndpointAccessRequestRequestTypeDef",
     "UpdateNamespaceRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateUsageLimitRequestRequestTypeDef",
     "UpdateWorkgroupRequestRequestTypeDef",
     "ConvertRecoveryPointToSnapshotRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateWorkgroupRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "GetCredentialsResponseTypeDef",
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DeleteSnapshotResponseTypeDef",
     "GetSnapshotResponseTypeDef",
     "ListSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
     "CreateNamespaceResponseTypeDef",
@@ -113,14 +107,22 @@
     "GetRecoveryPointResponseTypeDef",
     "ListRecoveryPointsResponseTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
     "GetTableRestoreStatusResponseTypeDef",
     "ListTableRestoreStatusResponseTypeDef",
     "RestoreTableFromSnapshotResponseTypeDef",
+    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+    "ListNamespacesRequestListNamespacesPaginateTypeDef",
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "VpcEndpointTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "CreateEndpointAccessResponseTypeDef",
     "DeleteEndpointAccessResponseTypeDef",
     "GetEndpointAccessResponseTypeDef",
     "ListEndpointAccessResponseTypeDef",
@@ -129,14 +131,23 @@
     "CreateWorkgroupResponseTypeDef",
     "DeleteWorkgroupResponseTypeDef",
     "GetWorkgroupResponseTypeDef",
     "ListWorkgroupsResponseTypeDef",
     "UpdateWorkgroupResponseTypeDef",
 )
 
+ConfigParameterOutputTypeDef = TypedDict(
+    "ConfigParameterOutputTypeDef",
+    {
+        "parameterKey": str,
+        "parameterValue": str,
+    },
+    total=False,
+)
+
 ConfigParameterTypeDef = TypedDict(
     "ConfigParameterTypeDef",
     {
         "parameterKey": str,
         "parameterValue": str,
     },
     total=False,
@@ -146,14 +157,25 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
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
 SnapshotTypeDef = TypedDict(
     "SnapshotTypeDef",
     {
         "accountsWithProvisionedRestoreAccess": List[str],
         "accountsWithRestoreAccess": List[str],
         "actualIncrementalBackupSizeInMegaBytes": float,
         "adminUsername": str,
@@ -333,25 +355,14 @@
 )
 
 class GetCredentialsRequestRequestTypeDef(
     _RequiredGetCredentialsRequestRequestTypeDef, _OptionalGetCredentialsRequestRequestTypeDef
 ):
     pass
 
-GetCredentialsResponseTypeDef = TypedDict(
-    "GetCredentialsResponseTypeDef",
-    {
-        "dbPassword": str,
-        "dbUser": str,
-        "expiration": datetime,
-        "nextRefreshTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEndpointAccessRequestRequestTypeDef = TypedDict(
     "GetEndpointAccessRequestRequestTypeDef",
     {
         "endpointName": str,
     },
 )
 
@@ -447,20 +458,20 @@
 GetWorkgroupRequestRequestTypeDef = TypedDict(
     "GetWorkgroupRequestRequestTypeDef",
     {
         "workgroupName": str,
     },
 )
 
-ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = TypedDict(
-    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "vpcId": str,
-        "workgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListEndpointAccessRequestRequestTypeDef = TypedDict(
     "ListEndpointAccessRequestRequestTypeDef",
     {
@@ -468,93 +479,50 @@
         "nextToken": str,
         "vpcId": str,
         "workgroupName": str,
     },
     total=False,
 )
 
-ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
-    "ListNamespacesRequestListNamespacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNamespacesRequestRequestTypeDef = TypedDict(
     "ListNamespacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
-    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
-        "namespaceName": str,
-        "startTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRecoveryPointsRequestRequestTypeDef = TypedDict(
     "ListRecoveryPointsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "maxResults": int,
         "namespaceArn": str,
         "namespaceName": str,
         "nextToken": str,
         "startTime": Union[datetime, str],
     },
     total=False,
 )
 
-ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "namespaceArn": str,
-        "namespaceName": str,
-        "ownerAccount": str,
-        "startTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSnapshotsRequestRequestTypeDef = TypedDict(
     "ListSnapshotsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "maxResults": int,
         "namespaceArn": str,
         "namespaceName": str,
         "nextToken": str,
         "ownerAccount": str,
         "startTime": Union[datetime, str],
     },
     total=False,
 )
 
-ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
-    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
-    {
-        "namespaceName": str,
-        "workgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTableRestoreStatusRequestRequestTypeDef = TypedDict(
     "ListTableRestoreStatusRequestRequestTypeDef",
     {
         "maxResults": int,
         "namespaceName": str,
         "nextToken": str,
         "workgroupName": str,
@@ -565,43 +533,33 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
-    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "resourceArn": str,
-        "usageType": UsageLimitUsageTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "key": str,
+        "value": str,
     },
-    total=False,
 )
 
 ListUsageLimitsRequestRequestTypeDef = TypedDict(
     "ListUsageLimitsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "resourceArn": str,
         "usageType": UsageLimitUsageTypeType,
     },
     total=False,
 )
 
-ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
-    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkgroupsRequestRequestTypeDef = TypedDict(
     "ListWorkgroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -614,43 +572,22 @@
         "networkInterfaceId": str,
         "privateIpAddress": str,
         "subnetId": str,
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
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
 RestoreFromRecoveryPointRequestRequestTypeDef = TypedDict(
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     {
         "namespaceName": str,
         "recoveryPointId": str,
         "workgroupName": str,
     },
@@ -915,235 +852,317 @@
 )
 
 class CreateWorkgroupRequestRequestTypeDef(
     _RequiredCreateWorkgroupRequestRequestTypeDef, _OptionalCreateWorkgroupRequestRequestTypeDef
 ):
     pass
 
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
 
+GetCredentialsResponseTypeDef = TypedDict(
+    "GetCredentialsResponseTypeDef",
+    {
+        "dbPassword": str,
+        "dbUser": str,
+        "expiration": datetime,
+        "nextRefreshTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ConvertRecoveryPointToSnapshotResponseTypeDef = TypedDict(
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSnapshotResponseTypeDef = TypedDict(
     "CreateSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSnapshotResponseTypeDef = TypedDict(
     "DeleteSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotResponseTypeDef = TypedDict(
     "GetSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSnapshotsResponseTypeDef = TypedDict(
     "ListSnapshotsResponseTypeDef",
     {
         "nextToken": str,
         "snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSnapshotResponseTypeDef = TypedDict(
     "UpdateSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateNamespaceResponseTypeDef = TypedDict(
     "CreateNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteNamespaceResponseTypeDef = TypedDict(
     "DeleteNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNamespaceResponseTypeDef = TypedDict(
     "GetNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "namespaces": List[NamespaceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreFromRecoveryPointResponseTypeDef = TypedDict(
     "RestoreFromRecoveryPointResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
         "recoveryPointId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreFromSnapshotResponseTypeDef = TypedDict(
     "RestoreFromSnapshotResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
         "ownerAccount": str,
         "snapshotName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNamespaceResponseTypeDef = TypedDict(
     "UpdateNamespaceResponseTypeDef",
     {
         "namespace": NamespaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateUsageLimitResponseTypeDef = TypedDict(
     "CreateUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteUsageLimitResponseTypeDef = TypedDict(
     "DeleteUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUsageLimitResponseTypeDef = TypedDict(
     "GetUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsageLimitsResponseTypeDef = TypedDict(
     "ListUsageLimitsResponseTypeDef",
     {
         "nextToken": str,
         "usageLimits": List[UsageLimitTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUsageLimitResponseTypeDef = TypedDict(
     "UpdateUsageLimitResponseTypeDef",
     {
         "usageLimit": UsageLimitTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecoveryPointResponseTypeDef = TypedDict(
     "GetRecoveryPointResponseTypeDef",
     {
         "recoveryPoint": RecoveryPointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecoveryPointsResponseTypeDef = TypedDict(
     "ListRecoveryPointsResponseTypeDef",
     {
         "nextToken": str,
         "recoveryPoints": List[RecoveryPointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcePolicyResponseTypeDef = TypedDict(
     "GetResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourcePolicyResponseTypeDef = TypedDict(
     "PutResourcePolicyResponseTypeDef",
     {
         "resourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTableRestoreStatusResponseTypeDef = TypedDict(
     "GetTableRestoreStatusResponseTypeDef",
     {
         "tableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTableRestoreStatusResponseTypeDef = TypedDict(
     "ListTableRestoreStatusResponseTypeDef",
     {
         "nextToken": str,
         "tableRestoreStatuses": List[TableRestoreStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreTableFromSnapshotResponseTypeDef = TypedDict(
     "RestoreTableFromSnapshotResponseTypeDef",
     {
         "tableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEndpointAccessRequestListEndpointAccessPaginateTypeDef = TypedDict(
+    "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
+    {
+        "vpcId": str,
+        "workgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListNamespacesRequestListNamespacesPaginateTypeDef = TypedDict(
+    "ListNamespacesRequestListNamespacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef = TypedDict(
+    "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "namespaceArn": str,
+        "namespaceName": str,
+        "startTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "endTime": Union[datetime, str],
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ownerAccount": str,
+        "startTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef = TypedDict(
+    "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
+    {
+        "namespaceName": str,
+        "workgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListUsageLimitsRequestListUsageLimitsPaginateTypeDef = TypedDict(
+    "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
+    {
+        "resourceArn": str,
+        "usageType": UsageLimitUsageTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkgroupsRequestListWorkgroupsPaginateTypeDef = TypedDict(
+    "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "networkInterfaces": List[NetworkInterfaceTypeDef],
@@ -1180,56 +1199,56 @@
     total=False,
 )
 
 CreateEndpointAccessResponseTypeDef = TypedDict(
     "CreateEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEndpointAccessResponseTypeDef = TypedDict(
     "DeleteEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEndpointAccessResponseTypeDef = TypedDict(
     "GetEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEndpointAccessResponseTypeDef = TypedDict(
     "ListEndpointAccessResponseTypeDef",
     {
         "endpoints": List[EndpointAccessTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointAccessResponseTypeDef = TypedDict(
     "UpdateEndpointAccessResponseTypeDef",
     {
         "endpoint": EndpointAccessTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkgroupTypeDef = TypedDict(
     "WorkgroupTypeDef",
     {
         "baseCapacity": int,
-        "configParameters": List[ConfigParameterTypeDef],
+        "configParameters": List[ConfigParameterOutputTypeDef],
         "creationDate": datetime,
         "endpoint": EndpointTypeDef,
         "enhancedVpcRouting": bool,
         "namespaceName": str,
         "port": int,
         "publiclyAccessible": bool,
         "securityGroupIds": List[str],
@@ -1242,43 +1261,43 @@
     total=False,
 )
 
 CreateWorkgroupResponseTypeDef = TypedDict(
     "CreateWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteWorkgroupResponseTypeDef = TypedDict(
     "DeleteWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkgroupResponseTypeDef = TypedDict(
     "GetWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkgroupsResponseTypeDef = TypedDict(
     "ListWorkgroupsResponseTypeDef",
     {
         "nextToken": str,
         "workgroups": List[WorkgroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkgroupResponseTypeDef = TypedDict(
     "UpdateWorkgroupResponseTypeDef",
     {
         "workgroup": WorkgroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless.egg-info/PKG-INFO` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-serverless
-Version: 1.28.0
-Summary: Type annotations for boto3.RedshiftServerless 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.RedshiftServerless 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-redshift-serverless"></a>
 
 # mypy-boto3-redshift-serverless
 
 [![PyPI - mypy-boto3-redshift-serverless](https://img.shields.io/pypi/v/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-redshift-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-redshift-serverless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-serverless)](https://pepy.tech/project/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,75 +353,69 @@
 ### Typed dictionaries
 
 `mypy_boto3_redshift_serverless.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_serverless.type_defs import (
+    ConfigParameterOutputTypeDef,
     ConfigParameterTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     SnapshotTypeDef,
     CreateEndpointAccessRequestRequestTypeDef,
     NamespaceTypeDef,
     CreateUsageLimitRequestRequestTypeDef,
     UsageLimitTypeDef,
     DeleteEndpointAccessRequestRequestTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
     DeleteUsageLimitRequestRequestTypeDef,
     DeleteWorkgroupRequestRequestTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     GetCredentialsRequestRequestTypeDef,
-    GetCredentialsResponseTypeDef,
     GetEndpointAccessRequestRequestTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetRecoveryPointRequestRequestTypeDef,
     RecoveryPointTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     ResourcePolicyTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetTableRestoreStatusRequestRequestTypeDef,
     TableRestoreStatusTypeDef,
     GetUsageLimitRequestRequestTypeDef,
     GetWorkgroupRequestRequestTypeDef,
-    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
-    ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
-    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
     ListRecoveryPointsRequestRequestTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
-    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
+    TagOutputTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
-    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     RestoreTableFromSnapshotRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEndpointAccessRequestRequestTypeDef,
     UpdateNamespaceRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateUsageLimitRequestRequestTypeDef,
     UpdateWorkgroupRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateWorkgroupRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    GetCredentialsResponseTypeDef,
     ConvertRecoveryPointToSnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     GetSnapshotResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateNamespaceResponseTypeDef,
@@ -439,14 +433,22 @@
     GetRecoveryPointResponseTypeDef,
     ListRecoveryPointsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
     PutResourcePolicyResponseTypeDef,
     GetTableRestoreStatusResponseTypeDef,
     ListTableRestoreStatusResponseTypeDef,
     RestoreTableFromSnapshotResponseTypeDef,
+    ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
+    ListNamespacesRequestListNamespacesPaginateTypeDef,
+    ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
+    ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
+    ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -456,15 +458,15 @@
     DeleteWorkgroupResponseTypeDef,
     GetWorkgroupResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
 
-def get_structure() -> ConfigParameterTypeDef:
+def get_structure() -> ConfigParameterOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-redshift-serverless-1.28.0/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt` & `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.0/setup.py` & `mypy-boto3-redshift-serverless-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift-serverless",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_redshift_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RedshiftServerless 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.RedshiftServerless 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

