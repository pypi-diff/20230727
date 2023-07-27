# Comparing `tmp/mypy-boto3-servicecatalog-appregistry-1.28.0.tar.gz` & `tmp/mypy-boto3-servicecatalog-appregistry-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicecatalog-appregistry-1.28.0.tar", last modified: Thu Jul  6 21:00:36 2023, max compression
+gzip compressed data, was "mypy-boto3-servicecatalog-appregistry-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
```

## Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0.tar` & `mypy-boto3-servicecatalog-appregistry-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:36.914430 mypy-boto3-servicecatalog-appregistry-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17155 2023-07-06 21:00:36.914430 mypy-boto3-servicecatalog-appregistry-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15609 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:36.914430 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21071 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21722 2023-07-06 20:55:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:36.914430 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17155 2023-07-06 21:00:36.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-06 21:00:36.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:36.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:36.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:36.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:36.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:36.914430 mypy-boto3-servicecatalog-appregistry-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-06 20:55:43.000000 mypy-boto3-servicecatalog-appregistry-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.617291 mypy-boto3-servicecatalog-appregistry-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-27 11:49:38.617291 mypy-boto3-servicecatalog-appregistry-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.617291 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21071 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22117 2023-07-27 11:46:47.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22096 2023-07-27 11:46:47.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.617291 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.617291 mypy-boto3-servicecatalog-appregistry-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/setup.py
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/LICENSE` & `mypy-boto3-servicecatalog-appregistry-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/PKG-INFO` & `mypy-boto3-servicecatalog-appregistry-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog-appregistry
-Version: 1.28.0
-Summary: Type annotations for boto3.AppRegistry 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AppRegistry 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-servicecatalog-appregistry"></a>
 
 # mypy-boto3-servicecatalog-appregistry
 
 [![PyPI - mypy-boto3-servicecatalog-appregistry](https://img.shields.io/pypi/v/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog-appregistry?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog-appregistry)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog-appregistry)](https://pepy.tech/project/mypy-boto3-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRegistry 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
+[boto3.AppRegistry 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [mypy-boto3-servicecatalog-appregistry docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,83 +345,85 @@
 ### Typed dictionaries
 
 `mypy_boto3_servicecatalog_appregistry.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_servicecatalog_appregistry.type_defs import (
+    TagQueryConfigurationOutputTypeDef,
     TagQueryConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociateAttributeGroupRequestRequestTypeDef,
-    AssociateAttributeGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateResourceRequestRequestTypeDef,
-    AssociateResourceResponseTypeDef,
     AttributeGroupDetailsTypeDef,
     AttributeGroupSummaryTypeDef,
     AttributeGroupTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateAttributeGroupRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteAttributeGroupRequestRequestTypeDef,
     DisassociateAttributeGroupRequestRequestTypeDef,
-    DisassociateAttributeGroupResponseTypeDef,
     DisassociateResourceRequestRequestTypeDef,
-    DisassociateResourceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetAssociatedResourceRequestRequestTypeDef,
     GetAttributeGroupRequestRequestTypeDef,
-    GetAttributeGroupResponseTypeDef,
     ResourceGroupTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
     ListAssociatedAttributeGroupsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsResponseTypeDef,
-    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
     ListAssociatedResourcesRequestRequestTypeDef,
-    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
     ListAttributeGroupsForApplicationRequestRequestTypeDef,
-    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ListAttributeGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     ResourceDetailsTypeDef,
-    ResponseMetadataTypeDef,
     SyncResourceRequestRequestTypeDef,
-    SyncResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateAttributeGroupRequestRequestTypeDef,
+    AppRegistryConfigurationOutputTypeDef,
     AppRegistryConfigurationTypeDef,
+    AssociateAttributeGroupResponseTypeDef,
+    AssociateResourceResponseTypeDef,
+    CreateApplicationResponseTypeDef,
     DeleteApplicationResponseTypeDef,
+    DisassociateAttributeGroupResponseTypeDef,
+    DisassociateResourceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAttributeGroupResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    CreateApplicationResponseTypeDef,
+    ListAssociatedAttributeGroupsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SyncResourceResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListAttributeGroupsForApplicationResponseTypeDef,
     DeleteAttributeGroupResponseTypeDef,
     ListAttributeGroupsResponseTypeDef,
     CreateAttributeGroupResponseTypeDef,
     UpdateAttributeGroupResponseTypeDef,
     IntegrationsTypeDef,
     ResourceIntegrationsTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ResourceInfoTypeDef,
     GetConfigurationResponseTypeDef,
     PutConfigurationRequestRequestTypeDef,
     GetApplicationResponseTypeDef,
     ResourceTypeDef,
     ListAssociatedResourcesResponseTypeDef,
     GetAssociatedResourceResponseTypeDef,
 )
 
 
-def get_structure() -> TagQueryConfigurationTypeDef:
+def get_structure() -> TagQueryConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/README.md` & `mypy-boto3-servicecatalog-appregistry-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-servicecatalog-appregistry"></a>
 
 # mypy-boto3-servicecatalog-appregistry
 
 [![PyPI - mypy-boto3-servicecatalog-appregistry](https://img.shields.io/pypi/v/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog-appregistry?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog-appregistry)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog-appregistry)](https://pepy.tech/project/mypy-boto3-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRegistry 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
+[boto3.AppRegistry 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [mypy-boto3-servicecatalog-appregistry docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,83 +313,85 @@
 ### Typed dictionaries
 
 `mypy_boto3_servicecatalog_appregistry.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_servicecatalog_appregistry.type_defs import (
+    TagQueryConfigurationOutputTypeDef,
     TagQueryConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociateAttributeGroupRequestRequestTypeDef,
-    AssociateAttributeGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateResourceRequestRequestTypeDef,
-    AssociateResourceResponseTypeDef,
     AttributeGroupDetailsTypeDef,
     AttributeGroupSummaryTypeDef,
     AttributeGroupTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateAttributeGroupRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteAttributeGroupRequestRequestTypeDef,
     DisassociateAttributeGroupRequestRequestTypeDef,
-    DisassociateAttributeGroupResponseTypeDef,
     DisassociateResourceRequestRequestTypeDef,
-    DisassociateResourceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetAssociatedResourceRequestRequestTypeDef,
     GetAttributeGroupRequestRequestTypeDef,
-    GetAttributeGroupResponseTypeDef,
     ResourceGroupTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
     ListAssociatedAttributeGroupsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsResponseTypeDef,
-    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
     ListAssociatedResourcesRequestRequestTypeDef,
-    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
     ListAttributeGroupsForApplicationRequestRequestTypeDef,
-    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ListAttributeGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     ResourceDetailsTypeDef,
-    ResponseMetadataTypeDef,
     SyncResourceRequestRequestTypeDef,
-    SyncResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateAttributeGroupRequestRequestTypeDef,
+    AppRegistryConfigurationOutputTypeDef,
     AppRegistryConfigurationTypeDef,
+    AssociateAttributeGroupResponseTypeDef,
+    AssociateResourceResponseTypeDef,
+    CreateApplicationResponseTypeDef,
     DeleteApplicationResponseTypeDef,
+    DisassociateAttributeGroupResponseTypeDef,
+    DisassociateResourceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAttributeGroupResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    CreateApplicationResponseTypeDef,
+    ListAssociatedAttributeGroupsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SyncResourceResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListAttributeGroupsForApplicationResponseTypeDef,
     DeleteAttributeGroupResponseTypeDef,
     ListAttributeGroupsResponseTypeDef,
     CreateAttributeGroupResponseTypeDef,
     UpdateAttributeGroupResponseTypeDef,
     IntegrationsTypeDef,
     ResourceIntegrationsTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ResourceInfoTypeDef,
     GetConfigurationResponseTypeDef,
     PutConfigurationRequestRequestTypeDef,
     GetApplicationResponseTypeDef,
     ResourceTypeDef,
     ListAssociatedResourcesResponseTypeDef,
     GetAssociatedResourceResponseTypeDef,
 )
 
 
-def get_structure() -> TagQueryConfigurationTypeDef:
+def get_structure() -> TagQueryConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/__init__.py` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/__init__.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/__main__.py` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppRegistry 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.AppRegistry 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry\nOther"
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

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/client.py` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/client.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/literals.py` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,15 @@
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
@@ -248,26 +249,28 @@
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

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/literals.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,15 @@
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
@@ -246,26 +247,28 @@
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

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/paginator.py` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,73 +62,73 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listapplicationspaginator)
         """
 
 
 class ListAssociatedAttributeGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedattributegroupspaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociatedAttributeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedattributegroupspaginator)
         """
 
 
 class ListAssociatedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedresourcespaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociatedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedresourcespaginator)
         """
 
 
 class ListAttributeGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttributeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupspaginator)
         """
 
 
 class ListAttributeGroupsForApplicationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroupsForApplication)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupsforapplicationpaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttributeGroupsForApplicationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroupsForApplication.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupsforapplicationpaginator)
         """
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/paginator.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -59,69 +59,69 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listapplicationspaginator)
         """
 
 class ListAssociatedAttributeGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedattributegroupspaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociatedAttributeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedAttributeGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedattributegroupspaginator)
         """
 
 class ListAssociatedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedresourcespaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssociatedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAssociatedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listassociatedresourcespaginator)
         """
 
 class ListAttributeGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttributeGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupspaginator)
         """
 
 class ListAttributeGroupsForApplicationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroupsForApplication)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupsforapplicationpaginator)
     """
 
     def paginate(
-        self, *, application: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, application: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttributeGroupsForApplicationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry.Paginator.ListAttributeGroupsForApplication.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/paginators/#listattributegroupsforapplicationpaginator)
         """
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/type_defs.py` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for servicecatalog-appregistry service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_servicecatalog_appregistry.type_defs import TagQueryConfigurationTypeDef
+    from mypy_boto3_servicecatalog_appregistry.type_defs import TagQueryConfigurationOutputTypeDef
 
-    data: TagQueryConfigurationTypeDef = {...}
+    data: TagQueryConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ResourceGroupStateType, ResourceTypeType, SyncActionType
@@ -20,81 +20,91 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "TagQueryConfigurationOutputTypeDef",
     "TagQueryConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "AssociateAttributeGroupRequestRequestTypeDef",
-    "AssociateAttributeGroupResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateResourceRequestRequestTypeDef",
-    "AssociateResourceResponseTypeDef",
     "AttributeGroupDetailsTypeDef",
     "AttributeGroupSummaryTypeDef",
     "AttributeGroupTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateAttributeGroupRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteAttributeGroupRequestRequestTypeDef",
     "DisassociateAttributeGroupRequestRequestTypeDef",
-    "DisassociateAttributeGroupResponseTypeDef",
     "DisassociateResourceRequestRequestTypeDef",
-    "DisassociateResourceResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetAssociatedResourceRequestRequestTypeDef",
     "GetAttributeGroupRequestRequestTypeDef",
-    "GetAttributeGroupResponseTypeDef",
     "ResourceGroupTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
     "ListAssociatedAttributeGroupsRequestRequestTypeDef",
-    "ListAssociatedAttributeGroupsResponseTypeDef",
-    "ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
     "ListAssociatedResourcesRequestRequestTypeDef",
-    "ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
     "ListAttributeGroupsForApplicationRequestRequestTypeDef",
-    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
     "ListAttributeGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "SyncResourceRequestRequestTypeDef",
-    "SyncResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateAttributeGroupRequestRequestTypeDef",
+    "AppRegistryConfigurationOutputTypeDef",
     "AppRegistryConfigurationTypeDef",
+    "AssociateAttributeGroupResponseTypeDef",
+    "AssociateResourceResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
     "DeleteApplicationResponseTypeDef",
+    "DisassociateAttributeGroupResponseTypeDef",
+    "DisassociateResourceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAttributeGroupResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "CreateApplicationResponseTypeDef",
+    "ListAssociatedAttributeGroupsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SyncResourceResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "ListAttributeGroupsForApplicationResponseTypeDef",
     "DeleteAttributeGroupResponseTypeDef",
     "ListAttributeGroupsResponseTypeDef",
     "CreateAttributeGroupResponseTypeDef",
     "UpdateAttributeGroupResponseTypeDef",
     "IntegrationsTypeDef",
     "ResourceIntegrationsTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+    "ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    "ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
     "ResourceInfoTypeDef",
     "GetConfigurationResponseTypeDef",
     "PutConfigurationRequestRequestTypeDef",
     "GetApplicationResponseTypeDef",
     "ResourceTypeDef",
     "ListAssociatedResourcesResponseTypeDef",
     "GetAssociatedResourceResponseTypeDef",
 )
 
+TagQueryConfigurationOutputTypeDef = TypedDict(
+    "TagQueryConfigurationOutputTypeDef",
+    {
+        "tagKey": str,
+    },
+    total=False,
+)
+
 TagQueryConfigurationTypeDef = TypedDict(
     "TagQueryConfigurationTypeDef",
     {
         "tagKey": str,
     },
     total=False,
 )
@@ -130,41 +140,34 @@
     "AssociateAttributeGroupRequestRequestTypeDef",
     {
         "application": str,
         "attributeGroup": str,
     },
 )
 
-AssociateAttributeGroupResponseTypeDef = TypedDict(
-    "AssociateAttributeGroupResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "applicationArn": str,
-        "attributeGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociateResourceRequestRequestTypeDef = TypedDict(
     "AssociateResourceRequestRequestTypeDef",
     {
         "application": str,
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
-AssociateResourceResponseTypeDef = TypedDict(
-    "AssociateResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttributeGroupDetailsTypeDef = TypedDict(
     "AttributeGroupDetailsTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "createdBy": str,
@@ -266,48 +269,23 @@
     "DisassociateAttributeGroupRequestRequestTypeDef",
     {
         "application": str,
         "attributeGroup": str,
     },
 )
 
-DisassociateAttributeGroupResponseTypeDef = TypedDict(
-    "DisassociateAttributeGroupResponseTypeDef",
-    {
-        "applicationArn": str,
-        "attributeGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateResourceRequestRequestTypeDef = TypedDict(
     "DisassociateResourceRequestRequestTypeDef",
     {
         "application": str,
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
-DisassociateResourceResponseTypeDef = TypedDict(
-    "DisassociateResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApplicationRequestRequestTypeDef = TypedDict(
     "GetApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 
@@ -323,83 +301,43 @@
 GetAttributeGroupRequestRequestTypeDef = TypedDict(
     "GetAttributeGroupRequestRequestTypeDef",
     {
         "attributeGroup": str,
     },
 )
 
-GetAttributeGroupResponseTypeDef = TypedDict(
-    "GetAttributeGroupResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "attributes": str,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "tags": Dict[str, str],
-        "createdBy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceGroupTypeDef = TypedDict(
     "ResourceGroupTypeDef",
     {
         "state": ResourceGroupStateType,
         "arn": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
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
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-        {
-            "application": str,
-        },
-    )
-)
-_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef(
-    _RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-    _OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssociatedAttributeGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedAttributeGroupsRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAssociatedAttributeGroupsRequestRequestTypeDef = TypedDict(
@@ -415,45 +353,14 @@
 class ListAssociatedAttributeGroupsRequestRequestTypeDef(
     _RequiredListAssociatedAttributeGroupsRequestRequestTypeDef,
     _OptionalListAssociatedAttributeGroupsRequestRequestTypeDef,
 ):
     pass
 
 
-ListAssociatedAttributeGroupsResponseTypeDef = TypedDict(
-    "ListAssociatedAttributeGroupsResponseTypeDef",
-    {
-        "attributeGroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    {
-        "application": str,
-    },
-)
-_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef(
-    _RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-    _OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssociatedResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedResourcesRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAssociatedResourcesRequestRequestTypeDef = TypedDict(
@@ -469,36 +376,14 @@
 class ListAssociatedResourcesRequestRequestTypeDef(
     _RequiredListAssociatedResourcesRequestRequestTypeDef,
     _OptionalListAssociatedResourcesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
-    "_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    {
-        "application": str,
-    },
-)
-_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
-    "_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef(
-    _RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-    _OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAttributeGroupsForApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredListAttributeGroupsForApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAttributeGroupsForApplicationRequestRequestTypeDef = TypedDict(
@@ -514,22 +399,14 @@
 class ListAttributeGroupsForApplicationRequestRequestTypeDef(
     _RequiredListAttributeGroupsForApplicationRequestRequestTypeDef,
     _OptionalListAttributeGroupsForApplicationRequestRequestTypeDef,
 ):
     pass
 
 
-ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = TypedDict(
-    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAttributeGroupsRequestRequestTypeDef = TypedDict(
     "ListAttributeGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -538,69 +415,30 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "tagValue": str,
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
 SyncResourceRequestRequestTypeDef = TypedDict(
     "SyncResourceRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
-SyncResourceResponseTypeDef = TypedDict(
-    "SyncResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "actionTaken": SyncActionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -655,94 +493,188 @@
 class UpdateAttributeGroupRequestRequestTypeDef(
     _RequiredUpdateAttributeGroupRequestRequestTypeDef,
     _OptionalUpdateAttributeGroupRequestRequestTypeDef,
 ):
     pass
 
 
+AppRegistryConfigurationOutputTypeDef = TypedDict(
+    "AppRegistryConfigurationOutputTypeDef",
+    {
+        "tagQueryConfiguration": TagQueryConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 AppRegistryConfigurationTypeDef = TypedDict(
     "AppRegistryConfigurationTypeDef",
     {
         "tagQueryConfiguration": TagQueryConfigurationTypeDef,
     },
     total=False,
 )
 
+AssociateAttributeGroupResponseTypeDef = TypedDict(
+    "AssociateAttributeGroupResponseTypeDef",
+    {
+        "applicationArn": str,
+        "attributeGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateResourceResponseTypeDef = TypedDict(
+    "AssociateResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "application": ApplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteApplicationResponseTypeDef = TypedDict(
     "DeleteApplicationResponseTypeDef",
     {
         "application": ApplicationSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateAttributeGroupResponseTypeDef = TypedDict(
+    "DisassociateAttributeGroupResponseTypeDef",
+    {
+        "applicationArn": str,
+        "attributeGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateResourceResponseTypeDef = TypedDict(
+    "DisassociateResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAttributeGroupResponseTypeDef = TypedDict(
+    "GetAttributeGroupResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "attributes": str,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "tags": Dict[str, str],
+        "createdBy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
+ListAssociatedAttributeGroupsResponseTypeDef = TypedDict(
+    "ListAssociatedAttributeGroupsResponseTypeDef",
     {
-        "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "attributeGroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SyncResourceResponseTypeDef = TypedDict(
+    "SyncResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "actionTaken": SyncActionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttributeGroupsForApplicationResponseTypeDef = TypedDict(
     "ListAttributeGroupsForApplicationResponseTypeDef",
     {
         "attributeGroupsDetails": List[AttributeGroupDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAttributeGroupResponseTypeDef = TypedDict(
     "DeleteAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttributeGroupsResponseTypeDef = TypedDict(
     "ListAttributeGroupsResponseTypeDef",
     {
         "attributeGroups": List[AttributeGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAttributeGroupResponseTypeDef = TypedDict(
     "CreateAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAttributeGroupResponseTypeDef = TypedDict(
     "UpdateAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntegrationsTypeDef = TypedDict(
     "IntegrationsTypeDef",
     {
         "resourceGroup": ResourceGroupTypeDef,
@@ -754,30 +686,116 @@
     "ResourceIntegrationsTypeDef",
     {
         "resourceGroup": ResourceGroupTypeDef,
     },
     total=False,
 )
 
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+        {
+            "application": str,
+        },
+    )
+)
+_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef(
+    _RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+    _OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    {
+        "application": str,
+    },
+)
+_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef(
+    _RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+    _OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
+    "_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    {
+        "application": str,
+    },
+)
+_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
+    "_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef(
+    _RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+    _OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+):
+    pass
+
+
+ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = TypedDict(
+    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ResourceInfoTypeDef = TypedDict(
     "ResourceInfoTypeDef",
     {
         "name": str,
         "arn": str,
         "resourceType": ResourceTypeType,
         "resourceDetails": ResourceDetailsTypeDef,
     },
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
-        "configuration": AppRegistryConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "configuration": AppRegistryConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutConfigurationRequestRequestTypeDef = TypedDict(
     "PutConfigurationRequestRequestTypeDef",
     {
         "configuration": AppRegistryConfigurationTypeDef,
@@ -792,15 +810,15 @@
         "name": str,
         "description": str,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "associatedResourceCount": int,
         "tags": Dict[str, str],
         "integrations": IntegrationsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "name": str,
@@ -812,18 +830,18 @@
 )
 
 ListAssociatedResourcesResponseTypeDef = TypedDict(
     "ListAssociatedResourcesResponseTypeDef",
     {
         "resources": List[ResourceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssociatedResourceResponseTypeDef = TypedDict(
     "GetAssociatedResourceResponseTypeDef",
     {
         "resource": ResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry/type_defs.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,98 +2,108 @@
 Type annotations for servicecatalog-appregistry service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_servicecatalog_appregistry.type_defs import TagQueryConfigurationTypeDef
+    from mypy_boto3_servicecatalog_appregistry.type_defs import TagQueryConfigurationOutputTypeDef
 
-    data: TagQueryConfigurationTypeDef = {...}
+    data: TagQueryConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ResourceGroupStateType, ResourceTypeType, SyncActionType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "TagQueryConfigurationOutputTypeDef",
     "TagQueryConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "AssociateAttributeGroupRequestRequestTypeDef",
-    "AssociateAttributeGroupResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateResourceRequestRequestTypeDef",
-    "AssociateResourceResponseTypeDef",
     "AttributeGroupDetailsTypeDef",
     "AttributeGroupSummaryTypeDef",
     "AttributeGroupTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "CreateAttributeGroupRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteAttributeGroupRequestRequestTypeDef",
     "DisassociateAttributeGroupRequestRequestTypeDef",
-    "DisassociateAttributeGroupResponseTypeDef",
     "DisassociateResourceRequestRequestTypeDef",
-    "DisassociateResourceResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetAssociatedResourceRequestRequestTypeDef",
     "GetAttributeGroupRequestRequestTypeDef",
-    "GetAttributeGroupResponseTypeDef",
     "ResourceGroupTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
     "ListAssociatedAttributeGroupsRequestRequestTypeDef",
-    "ListAssociatedAttributeGroupsResponseTypeDef",
-    "ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
     "ListAssociatedResourcesRequestRequestTypeDef",
-    "ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
     "ListAttributeGroupsForApplicationRequestRequestTypeDef",
-    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
     "ListAttributeGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "SyncResourceRequestRequestTypeDef",
-    "SyncResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateAttributeGroupRequestRequestTypeDef",
+    "AppRegistryConfigurationOutputTypeDef",
     "AppRegistryConfigurationTypeDef",
+    "AssociateAttributeGroupResponseTypeDef",
+    "AssociateResourceResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
     "DeleteApplicationResponseTypeDef",
+    "DisassociateAttributeGroupResponseTypeDef",
+    "DisassociateResourceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAttributeGroupResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "CreateApplicationResponseTypeDef",
+    "ListAssociatedAttributeGroupsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SyncResourceResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "ListAttributeGroupsForApplicationResponseTypeDef",
     "DeleteAttributeGroupResponseTypeDef",
     "ListAttributeGroupsResponseTypeDef",
     "CreateAttributeGroupResponseTypeDef",
     "UpdateAttributeGroupResponseTypeDef",
     "IntegrationsTypeDef",
     "ResourceIntegrationsTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+    "ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    "ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
     "ResourceInfoTypeDef",
     "GetConfigurationResponseTypeDef",
     "PutConfigurationRequestRequestTypeDef",
     "GetApplicationResponseTypeDef",
     "ResourceTypeDef",
     "ListAssociatedResourcesResponseTypeDef",
     "GetAssociatedResourceResponseTypeDef",
 )
 
+TagQueryConfigurationOutputTypeDef = TypedDict(
+    "TagQueryConfigurationOutputTypeDef",
+    {
+        "tagKey": str,
+    },
+    total=False,
+)
+
 TagQueryConfigurationTypeDef = TypedDict(
     "TagQueryConfigurationTypeDef",
     {
         "tagKey": str,
     },
     total=False,
 )
@@ -129,41 +139,34 @@
     "AssociateAttributeGroupRequestRequestTypeDef",
     {
         "application": str,
         "attributeGroup": str,
     },
 )
 
-AssociateAttributeGroupResponseTypeDef = TypedDict(
-    "AssociateAttributeGroupResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "applicationArn": str,
-        "attributeGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AssociateResourceRequestRequestTypeDef = TypedDict(
     "AssociateResourceRequestRequestTypeDef",
     {
         "application": str,
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
-AssociateResourceResponseTypeDef = TypedDict(
-    "AssociateResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttributeGroupDetailsTypeDef = TypedDict(
     "AttributeGroupDetailsTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "createdBy": str,
@@ -261,48 +264,23 @@
     "DisassociateAttributeGroupRequestRequestTypeDef",
     {
         "application": str,
         "attributeGroup": str,
     },
 )
 
-DisassociateAttributeGroupResponseTypeDef = TypedDict(
-    "DisassociateAttributeGroupResponseTypeDef",
-    {
-        "applicationArn": str,
-        "attributeGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateResourceRequestRequestTypeDef = TypedDict(
     "DisassociateResourceRequestRequestTypeDef",
     {
         "application": str,
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
-DisassociateResourceResponseTypeDef = TypedDict(
-    "DisassociateResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApplicationRequestRequestTypeDef = TypedDict(
     "GetApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 
@@ -318,81 +296,43 @@
 GetAttributeGroupRequestRequestTypeDef = TypedDict(
     "GetAttributeGroupRequestRequestTypeDef",
     {
         "attributeGroup": str,
     },
 )
 
-GetAttributeGroupResponseTypeDef = TypedDict(
-    "GetAttributeGroupResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "description": str,
-        "attributes": str,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "tags": Dict[str, str],
-        "createdBy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceGroupTypeDef = TypedDict(
     "ResourceGroupTypeDef",
     {
         "state": ResourceGroupStateType,
         "arn": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
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
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-        {
-            "application": str,
-        },
-    )
-)
-_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef(
-    _RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-    _OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssociatedAttributeGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedAttributeGroupsRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAssociatedAttributeGroupsRequestRequestTypeDef = TypedDict(
@@ -406,43 +346,14 @@
 
 class ListAssociatedAttributeGroupsRequestRequestTypeDef(
     _RequiredListAssociatedAttributeGroupsRequestRequestTypeDef,
     _OptionalListAssociatedAttributeGroupsRequestRequestTypeDef,
 ):
     pass
 
-ListAssociatedAttributeGroupsResponseTypeDef = TypedDict(
-    "ListAssociatedAttributeGroupsResponseTypeDef",
-    {
-        "attributeGroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    {
-        "application": str,
-    },
-)
-_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef(
-    _RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-    _OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssociatedResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListAssociatedResourcesRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAssociatedResourcesRequestRequestTypeDef = TypedDict(
@@ -456,34 +367,14 @@
 
 class ListAssociatedResourcesRequestRequestTypeDef(
     _RequiredListAssociatedResourcesRequestRequestTypeDef,
     _OptionalListAssociatedResourcesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
-    "_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    {
-        "application": str,
-    },
-)
-_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
-    "_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef(
-    _RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-    _OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
-):
-    pass
-
 _RequiredListAttributeGroupsForApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredListAttributeGroupsForApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalListAttributeGroupsForApplicationRequestRequestTypeDef = TypedDict(
@@ -497,22 +388,14 @@
 
 class ListAttributeGroupsForApplicationRequestRequestTypeDef(
     _RequiredListAttributeGroupsForApplicationRequestRequestTypeDef,
     _OptionalListAttributeGroupsForApplicationRequestRequestTypeDef,
 ):
     pass
 
-ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = TypedDict(
-    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAttributeGroupsRequestRequestTypeDef = TypedDict(
     "ListAttributeGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -521,69 +404,30 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "tagValue": str,
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
 SyncResourceRequestRequestTypeDef = TypedDict(
     "SyncResourceRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resource": str,
     },
 )
 
-SyncResourceResponseTypeDef = TypedDict(
-    "SyncResourceResponseTypeDef",
-    {
-        "applicationArn": str,
-        "resourceArn": str,
-        "actionTaken": SyncActionType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -634,94 +478,188 @@
 
 class UpdateAttributeGroupRequestRequestTypeDef(
     _RequiredUpdateAttributeGroupRequestRequestTypeDef,
     _OptionalUpdateAttributeGroupRequestRequestTypeDef,
 ):
     pass
 
+AppRegistryConfigurationOutputTypeDef = TypedDict(
+    "AppRegistryConfigurationOutputTypeDef",
+    {
+        "tagQueryConfiguration": TagQueryConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 AppRegistryConfigurationTypeDef = TypedDict(
     "AppRegistryConfigurationTypeDef",
     {
         "tagQueryConfiguration": TagQueryConfigurationTypeDef,
     },
     total=False,
 )
 
+AssociateAttributeGroupResponseTypeDef = TypedDict(
+    "AssociateAttributeGroupResponseTypeDef",
+    {
+        "applicationArn": str,
+        "attributeGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateResourceResponseTypeDef = TypedDict(
+    "AssociateResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "application": ApplicationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteApplicationResponseTypeDef = TypedDict(
     "DeleteApplicationResponseTypeDef",
     {
         "application": ApplicationSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateAttributeGroupResponseTypeDef = TypedDict(
+    "DisassociateAttributeGroupResponseTypeDef",
+    {
+        "applicationArn": str,
+        "attributeGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateResourceResponseTypeDef = TypedDict(
+    "DisassociateResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAttributeGroupResponseTypeDef = TypedDict(
+    "GetAttributeGroupResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "attributes": str,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "tags": Dict[str, str],
+        "createdBy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
+ListAssociatedAttributeGroupsResponseTypeDef = TypedDict(
+    "ListAssociatedAttributeGroupsResponseTypeDef",
     {
-        "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "attributeGroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SyncResourceResponseTypeDef = TypedDict(
+    "SyncResourceResponseTypeDef",
+    {
+        "applicationArn": str,
+        "resourceArn": str,
+        "actionTaken": SyncActionType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttributeGroupsForApplicationResponseTypeDef = TypedDict(
     "ListAttributeGroupsForApplicationResponseTypeDef",
     {
         "attributeGroupsDetails": List[AttributeGroupDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAttributeGroupResponseTypeDef = TypedDict(
     "DeleteAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttributeGroupsResponseTypeDef = TypedDict(
     "ListAttributeGroupsResponseTypeDef",
     {
         "attributeGroups": List[AttributeGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAttributeGroupResponseTypeDef = TypedDict(
     "CreateAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAttributeGroupResponseTypeDef = TypedDict(
     "UpdateAttributeGroupResponseTypeDef",
     {
         "attributeGroup": AttributeGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntegrationsTypeDef = TypedDict(
     "IntegrationsTypeDef",
     {
         "resourceGroup": ResourceGroupTypeDef,
@@ -733,30 +671,110 @@
     "ResourceIntegrationsTypeDef",
     {
         "resourceGroup": ResourceGroupTypeDef,
     },
     total=False,
 )
 
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+        {
+            "application": str,
+        },
+    )
+)
+_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef(
+    _RequiredListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+    _OptionalListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    {
+        "application": str,
+    },
+)
+_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef(
+    _RequiredListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+    _OptionalListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
+    "_RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    {
+        "application": str,
+    },
+)
+_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef = TypedDict(
+    "_OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef(
+    _RequiredListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+    _OptionalListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+):
+    pass
+
+ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef = TypedDict(
+    "ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ResourceInfoTypeDef = TypedDict(
     "ResourceInfoTypeDef",
     {
         "name": str,
         "arn": str,
         "resourceType": ResourceTypeType,
         "resourceDetails": ResourceDetailsTypeDef,
     },
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
-        "configuration": AppRegistryConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "configuration": AppRegistryConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutConfigurationRequestRequestTypeDef = TypedDict(
     "PutConfigurationRequestRequestTypeDef",
     {
         "configuration": AppRegistryConfigurationTypeDef,
@@ -771,15 +789,15 @@
         "name": str,
         "description": str,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "associatedResourceCount": int,
         "tags": Dict[str, str],
         "integrations": IntegrationsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "name": str,
@@ -791,18 +809,18 @@
 )
 
 ListAssociatedResourcesResponseTypeDef = TypedDict(
     "ListAssociatedResourcesResponseTypeDef",
     {
         "resources": List[ResourceInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssociatedResourceResponseTypeDef = TypedDict(
     "GetAssociatedResourceResponseTypeDef",
     {
         "resource": ResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog-appregistry
-Version: 1.28.0
-Summary: Type annotations for boto3.AppRegistry 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AppRegistry 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-servicecatalog-appregistry"></a>
 
 # mypy-boto3-servicecatalog-appregistry
 
 [![PyPI - mypy-boto3-servicecatalog-appregistry](https://img.shields.io/pypi/v/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog-appregistry?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog-appregistry)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog-appregistry)](https://pepy.tech/project/mypy-boto3-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRegistry 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
+[boto3.AppRegistry 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [mypy-boto3-servicecatalog-appregistry docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,83 +345,85 @@
 ### Typed dictionaries
 
 `mypy_boto3_servicecatalog_appregistry.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_servicecatalog_appregistry.type_defs import (
+    TagQueryConfigurationOutputTypeDef,
     TagQueryConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociateAttributeGroupRequestRequestTypeDef,
-    AssociateAttributeGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     AssociateResourceRequestRequestTypeDef,
-    AssociateResourceResponseTypeDef,
     AttributeGroupDetailsTypeDef,
     AttributeGroupSummaryTypeDef,
     AttributeGroupTypeDef,
     CreateApplicationRequestRequestTypeDef,
     CreateAttributeGroupRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteAttributeGroupRequestRequestTypeDef,
     DisassociateAttributeGroupRequestRequestTypeDef,
-    DisassociateAttributeGroupResponseTypeDef,
     DisassociateResourceRequestRequestTypeDef,
-    DisassociateResourceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetAssociatedResourceRequestRequestTypeDef,
     GetAttributeGroupRequestRequestTypeDef,
-    GetAttributeGroupResponseTypeDef,
     ResourceGroupTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
     ListAssociatedAttributeGroupsRequestRequestTypeDef,
-    ListAssociatedAttributeGroupsResponseTypeDef,
-    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
     ListAssociatedResourcesRequestRequestTypeDef,
-    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
     ListAttributeGroupsForApplicationRequestRequestTypeDef,
-    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ListAttributeGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     ResourceDetailsTypeDef,
-    ResponseMetadataTypeDef,
     SyncResourceRequestRequestTypeDef,
-    SyncResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateAttributeGroupRequestRequestTypeDef,
+    AppRegistryConfigurationOutputTypeDef,
     AppRegistryConfigurationTypeDef,
+    AssociateAttributeGroupResponseTypeDef,
+    AssociateResourceResponseTypeDef,
+    CreateApplicationResponseTypeDef,
     DeleteApplicationResponseTypeDef,
+    DisassociateAttributeGroupResponseTypeDef,
+    DisassociateResourceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAttributeGroupResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    CreateApplicationResponseTypeDef,
+    ListAssociatedAttributeGroupsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SyncResourceResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListAttributeGroupsForApplicationResponseTypeDef,
     DeleteAttributeGroupResponseTypeDef,
     ListAttributeGroupsResponseTypeDef,
     CreateAttributeGroupResponseTypeDef,
     UpdateAttributeGroupResponseTypeDef,
     IntegrationsTypeDef,
     ResourceIntegrationsTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListAssociatedAttributeGroupsRequestListAssociatedAttributeGroupsPaginateTypeDef,
+    ListAssociatedResourcesRequestListAssociatedResourcesPaginateTypeDef,
+    ListAttributeGroupsForApplicationRequestListAttributeGroupsForApplicationPaginateTypeDef,
+    ListAttributeGroupsRequestListAttributeGroupsPaginateTypeDef,
     ResourceInfoTypeDef,
     GetConfigurationResponseTypeDef,
     PutConfigurationRequestRequestTypeDef,
     GetApplicationResponseTypeDef,
     ResourceTypeDef,
     ListAssociatedResourcesResponseTypeDef,
     GetAssociatedResourceResponseTypeDef,
 )
 
 
-def get_structure() -> TagQueryConfigurationTypeDef:
+def get_structure() -> TagQueryConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt` & `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.0/setup.py` & `mypy-boto3-servicecatalog-appregistry-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-servicecatalog-appregistry",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_servicecatalog_appregistry"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppRegistry 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.AppRegistry 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

