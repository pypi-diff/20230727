# Comparing `tmp/mypy-boto3-verifiedpermissions-1.28.0.tar.gz` & `tmp/mypy-boto3-verifiedpermissions-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-verifiedpermissions-1.28.0.tar", last modified: Thu Jul  6 21:00:49 2023, max compression
+gzip compressed data, was "mypy-boto3-verifiedpermissions-1.28.12.tar", last modified: Thu Jul 27 11:49:47 2023, max compression
```

## Comparing `mypy-boto3-verifiedpermissions-1.28.0.tar` & `mypy-boto3-verifiedpermissions-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.266455 mypy-boto3-verifiedpermissions-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:29.000000 mypy-boto3-verifiedpermissions-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-07-06 21:00:49.262455 mypy-boto3-verifiedpermissions-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-06 20:57:29.000000 mypy-boto3-verifiedpermissions-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.250455 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-06 20:57:29.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-06 20:57:29.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-06 20:57:29.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21090 2023-07-06 20:57:30.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21055 2023-07-06 20:57:29.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-06 20:57:30.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-06 20:57:30.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-06 20:57:30.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-06 20:57:30.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:29.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31246 2023-07-06 20:57:31.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31195 2023-07-06 20:57:30.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:29.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.262455 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-07-06 21:00:49.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 21:00:49.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:49.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:49.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:49.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 21:00:49.000000 mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:49.266455 mypy-boto3-verifiedpermissions-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-06 20:57:29.000000 mypy-boto3-verifiedpermissions-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.529473 mypy-boto3-verifiedpermissions-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16930 2023-07-27 11:49:47.525473 mypy-boto3-verifiedpermissions-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.517473 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21090 2023-07-27 11:48:14.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21055 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-07-27 11:48:16.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-27 11:48:16.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-27 11:48:14.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-27 11:48:14.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31636 2023-07-27 11:48:17.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31585 2023-07-27 11:48:16.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.525473 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16930 2023-07-27 11:49:47.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-27 11:49:47.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:47.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:47.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:47.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 11:49:47.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:47.529473 mypy-boto3-verifiedpermissions-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/setup.py
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/LICENSE` & `mypy-boto3-verifiedpermissions-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/PKG-INFO` & `mypy-boto3-verifiedpermissions-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-verifiedpermissions
-Version: 1.28.0
-Summary: Type annotations for boto3.VerifiedPermissions 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.VerifiedPermissions 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-verifiedpermissions"></a>
 
 # mypy-boto3-verifiedpermissions
 
 [![PyPI - mypy-boto3-verifiedpermissions](https://img.shields.io/pypi/v/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-verifiedpermissions?color=blue)](https://pypistats.org/packages/mypy-boto3-verifiedpermissions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-verifiedpermissions)](https://pepy.tech/project/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
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
 [mypy-boto3-verifiedpermissions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,93 +343,95 @@
 
 ```python
 from mypy_boto3_verifiedpermissions.type_defs import (
     ActionIdentifierTypeDef,
     EntityIdentifierTypeDef,
     CognitoUserPoolConfigurationTypeDef,
     ContextDefinitionTypeDef,
-    CreateIdentitySourceOutputTypeDef,
+    ResponseMetadataTypeDef,
+    EntityIdentifierOutputTypeDef,
     ValidationSettingsTypeDef,
-    CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateInputRequestTypeDef,
-    CreatePolicyTemplateOutputTypeDef,
     DeleteIdentitySourceInputRequestTypeDef,
     DeletePolicyInputRequestTypeDef,
     DeletePolicyStoreInputRequestTypeDef,
     DeletePolicyTemplateInputRequestTypeDef,
     DeterminingPolicyItemTypeDef,
     EvaluationErrorItemTypeDef,
     GetIdentitySourceInputRequestTypeDef,
     IdentitySourceDetailsTypeDef,
     GetPolicyInputRequestTypeDef,
     GetPolicyStoreInputRequestTypeDef,
+    ValidationSettingsOutputTypeDef,
     GetPolicyTemplateInputRequestTypeDef,
-    GetPolicyTemplateOutputTypeDef,
     GetSchemaInputRequestTypeDef,
-    GetSchemaOutputTypeDef,
     IdentitySourceFilterTypeDef,
     IdentitySourceItemDetailsTypeDef,
-    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPolicyStoresInputRequestTypeDef,
     PolicyStoreItemTypeDef,
-    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyTemplatesInputRequestTypeDef,
     PolicyTemplateItemTypeDef,
-    PaginatorConfigTypeDef,
     StaticPolicyDefinitionDetailTypeDef,
     StaticPolicyDefinitionItemTypeDef,
     StaticPolicyDefinitionTypeDef,
     SchemaDefinitionTypeDef,
-    PutSchemaOutputTypeDef,
-    ResponseMetadataTypeDef,
     UpdateCognitoUserPoolConfigurationTypeDef,
-    UpdateIdentitySourceOutputTypeDef,
     UpdateStaticPolicyDefinitionTypeDef,
-    UpdatePolicyStoreOutputTypeDef,
     UpdatePolicyTemplateInputRequestTypeDef,
-    UpdatePolicyTemplateOutputTypeDef,
     AttributeValueTypeDef,
-    CreatePolicyOutputTypeDef,
     EntityItemTypeDef,
     EntityReferenceTypeDef,
+    TemplateLinkedPolicyDefinitionTypeDef,
+    ConfigurationTypeDef,
+    CreateIdentitySourceOutputTypeDef,
+    CreatePolicyStoreOutputTypeDef,
+    CreatePolicyTemplateOutputTypeDef,
+    GetPolicyTemplateOutputTypeDef,
+    GetSchemaOutputTypeDef,
+    PutSchemaOutputTypeDef,
+    UpdateIdentitySourceOutputTypeDef,
+    UpdatePolicyStoreOutputTypeDef,
+    UpdatePolicyTemplateOutputTypeDef,
+    CreatePolicyOutputTypeDef,
     TemplateLinkedPolicyDefinitionDetailTypeDef,
     TemplateLinkedPolicyDefinitionItemTypeDef,
-    TemplateLinkedPolicyDefinitionTypeDef,
     UpdatePolicyOutputTypeDef,
-    ConfigurationTypeDef,
     CreatePolicyStoreInputRequestTypeDef,
-    GetPolicyStoreOutputTypeDef,
     UpdatePolicyStoreInputRequestTypeDef,
     IsAuthorizedOutputTypeDef,
     IsAuthorizedWithTokenOutputTypeDef,
     GetIdentitySourceOutputTypeDef,
-    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    GetPolicyStoreOutputTypeDef,
     ListIdentitySourcesInputRequestTypeDef,
     IdentitySourceItemTypeDef,
+    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
+    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyStoresOutputTypeDef,
     ListPolicyTemplatesOutputTypeDef,
     PutSchemaInputRequestTypeDef,
     UpdateConfigurationTypeDef,
     UpdatePolicyDefinitionTypeDef,
     EntitiesDefinitionTypeDef,
     PolicyFilterTypeDef,
-    PolicyDefinitionDetailTypeDef,
-    PolicyDefinitionItemTypeDef,
     PolicyDefinitionTypeDef,
     CreateIdentitySourceInputRequestTypeDef,
+    PolicyDefinitionDetailTypeDef,
+    PolicyDefinitionItemTypeDef,
     ListIdentitySourcesOutputTypeDef,
     UpdateIdentitySourceInputRequestTypeDef,
     UpdatePolicyInputRequestTypeDef,
     IsAuthorizedInputRequestTypeDef,
     IsAuthorizedWithTokenInputRequestTypeDef,
     ListPoliciesInputListPoliciesPaginateTypeDef,
     ListPoliciesInputRequestTypeDef,
+    CreatePolicyInputRequestTypeDef,
     GetPolicyOutputTypeDef,
     PolicyItemTypeDef,
-    CreatePolicyInputRequestTypeDef,
     ListPoliciesOutputTypeDef,
 )
 
 
 def get_structure() -> ActionIdentifierTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/README.md` & `mypy-boto3-verifiedpermissions-1.28.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-verifiedpermissions"></a>
 
 # mypy-boto3-verifiedpermissions
 
 [![PyPI - mypy-boto3-verifiedpermissions](https://img.shields.io/pypi/v/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-verifiedpermissions?color=blue)](https://pypistats.org/packages/mypy-boto3-verifiedpermissions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-verifiedpermissions)](https://pepy.tech/project/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
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
 [mypy-boto3-verifiedpermissions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,93 +311,95 @@
 
 ```python
 from mypy_boto3_verifiedpermissions.type_defs import (
     ActionIdentifierTypeDef,
     EntityIdentifierTypeDef,
     CognitoUserPoolConfigurationTypeDef,
     ContextDefinitionTypeDef,
-    CreateIdentitySourceOutputTypeDef,
+    ResponseMetadataTypeDef,
+    EntityIdentifierOutputTypeDef,
     ValidationSettingsTypeDef,
-    CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateInputRequestTypeDef,
-    CreatePolicyTemplateOutputTypeDef,
     DeleteIdentitySourceInputRequestTypeDef,
     DeletePolicyInputRequestTypeDef,
     DeletePolicyStoreInputRequestTypeDef,
     DeletePolicyTemplateInputRequestTypeDef,
     DeterminingPolicyItemTypeDef,
     EvaluationErrorItemTypeDef,
     GetIdentitySourceInputRequestTypeDef,
     IdentitySourceDetailsTypeDef,
     GetPolicyInputRequestTypeDef,
     GetPolicyStoreInputRequestTypeDef,
+    ValidationSettingsOutputTypeDef,
     GetPolicyTemplateInputRequestTypeDef,
-    GetPolicyTemplateOutputTypeDef,
     GetSchemaInputRequestTypeDef,
-    GetSchemaOutputTypeDef,
     IdentitySourceFilterTypeDef,
     IdentitySourceItemDetailsTypeDef,
-    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPolicyStoresInputRequestTypeDef,
     PolicyStoreItemTypeDef,
-    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyTemplatesInputRequestTypeDef,
     PolicyTemplateItemTypeDef,
-    PaginatorConfigTypeDef,
     StaticPolicyDefinitionDetailTypeDef,
     StaticPolicyDefinitionItemTypeDef,
     StaticPolicyDefinitionTypeDef,
     SchemaDefinitionTypeDef,
-    PutSchemaOutputTypeDef,
-    ResponseMetadataTypeDef,
     UpdateCognitoUserPoolConfigurationTypeDef,
-    UpdateIdentitySourceOutputTypeDef,
     UpdateStaticPolicyDefinitionTypeDef,
-    UpdatePolicyStoreOutputTypeDef,
     UpdatePolicyTemplateInputRequestTypeDef,
-    UpdatePolicyTemplateOutputTypeDef,
     AttributeValueTypeDef,
-    CreatePolicyOutputTypeDef,
     EntityItemTypeDef,
     EntityReferenceTypeDef,
+    TemplateLinkedPolicyDefinitionTypeDef,
+    ConfigurationTypeDef,
+    CreateIdentitySourceOutputTypeDef,
+    CreatePolicyStoreOutputTypeDef,
+    CreatePolicyTemplateOutputTypeDef,
+    GetPolicyTemplateOutputTypeDef,
+    GetSchemaOutputTypeDef,
+    PutSchemaOutputTypeDef,
+    UpdateIdentitySourceOutputTypeDef,
+    UpdatePolicyStoreOutputTypeDef,
+    UpdatePolicyTemplateOutputTypeDef,
+    CreatePolicyOutputTypeDef,
     TemplateLinkedPolicyDefinitionDetailTypeDef,
     TemplateLinkedPolicyDefinitionItemTypeDef,
-    TemplateLinkedPolicyDefinitionTypeDef,
     UpdatePolicyOutputTypeDef,
-    ConfigurationTypeDef,
     CreatePolicyStoreInputRequestTypeDef,
-    GetPolicyStoreOutputTypeDef,
     UpdatePolicyStoreInputRequestTypeDef,
     IsAuthorizedOutputTypeDef,
     IsAuthorizedWithTokenOutputTypeDef,
     GetIdentitySourceOutputTypeDef,
-    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    GetPolicyStoreOutputTypeDef,
     ListIdentitySourcesInputRequestTypeDef,
     IdentitySourceItemTypeDef,
+    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
+    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyStoresOutputTypeDef,
     ListPolicyTemplatesOutputTypeDef,
     PutSchemaInputRequestTypeDef,
     UpdateConfigurationTypeDef,
     UpdatePolicyDefinitionTypeDef,
     EntitiesDefinitionTypeDef,
     PolicyFilterTypeDef,
-    PolicyDefinitionDetailTypeDef,
-    PolicyDefinitionItemTypeDef,
     PolicyDefinitionTypeDef,
     CreateIdentitySourceInputRequestTypeDef,
+    PolicyDefinitionDetailTypeDef,
+    PolicyDefinitionItemTypeDef,
     ListIdentitySourcesOutputTypeDef,
     UpdateIdentitySourceInputRequestTypeDef,
     UpdatePolicyInputRequestTypeDef,
     IsAuthorizedInputRequestTypeDef,
     IsAuthorizedWithTokenInputRequestTypeDef,
     ListPoliciesInputListPoliciesPaginateTypeDef,
     ListPoliciesInputRequestTypeDef,
+    CreatePolicyInputRequestTypeDef,
     GetPolicyOutputTypeDef,
     PolicyItemTypeDef,
-    CreatePolicyInputRequestTypeDef,
     ListPoliciesOutputTypeDef,
 )
 
 
 def get_structure() -> ActionIdentifierTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/__init__.py` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/__init__.pyi` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/__main__.py` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VerifiedPermissions 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.VerifiedPermissions 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions\nOther"
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

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/client.py` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/client.pyi` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/literals.py` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/literals.py`

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

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/literals.pyi` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/literals.pyi`

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

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/paginator.py` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filters: Sequence[IdentitySourceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdentitySourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListIdentitySources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listidentitysourcespaginator)
         """
 
 
@@ -83,43 +83,43 @@
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filter: PolicyFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpoliciespaginator)
         """
 
 
 class ListPolicyStoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicystorespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPolicyStoresOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicystorespaginator)
         """
 
 
 class ListPolicyTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicytemplatespaginator)
     """
 
     def paginate(
-        self, *, policyStoreId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, policyStoreId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPolicyTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicytemplatespaginator)
         """
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/paginator.pyi` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filters: Sequence[IdentitySourceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdentitySourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListIdentitySources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listidentitysourcespaginator)
         """
 
 class ListPoliciesPaginator(Paginator):
@@ -79,41 +79,41 @@
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filter: PolicyFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpoliciespaginator)
         """
 
 class ListPolicyStoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicystorespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPolicyStoresOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicystorespaginator)
         """
 
 class ListPolicyTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicytemplatespaginator)
     """
 
     def paginate(
-        self, *, policyStoreId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, policyStoreId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPolicyTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/paginators/#listpolicytemplatespaginator)
         """
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/type_defs.py` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,99 +22,100 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionIdentifierTypeDef",
     "EntityIdentifierTypeDef",
     "CognitoUserPoolConfigurationTypeDef",
     "ContextDefinitionTypeDef",
-    "CreateIdentitySourceOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "EntityIdentifierOutputTypeDef",
     "ValidationSettingsTypeDef",
-    "CreatePolicyStoreOutputTypeDef",
     "CreatePolicyTemplateInputRequestTypeDef",
-    "CreatePolicyTemplateOutputTypeDef",
     "DeleteIdentitySourceInputRequestTypeDef",
     "DeletePolicyInputRequestTypeDef",
     "DeletePolicyStoreInputRequestTypeDef",
     "DeletePolicyTemplateInputRequestTypeDef",
     "DeterminingPolicyItemTypeDef",
     "EvaluationErrorItemTypeDef",
     "GetIdentitySourceInputRequestTypeDef",
     "IdentitySourceDetailsTypeDef",
     "GetPolicyInputRequestTypeDef",
     "GetPolicyStoreInputRequestTypeDef",
+    "ValidationSettingsOutputTypeDef",
     "GetPolicyTemplateInputRequestTypeDef",
-    "GetPolicyTemplateOutputTypeDef",
     "GetSchemaInputRequestTypeDef",
-    "GetSchemaOutputTypeDef",
     "IdentitySourceFilterTypeDef",
     "IdentitySourceItemDetailsTypeDef",
-    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListPolicyStoresInputRequestTypeDef",
     "PolicyStoreItemTypeDef",
-    "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyTemplatesInputRequestTypeDef",
     "PolicyTemplateItemTypeDef",
-    "PaginatorConfigTypeDef",
     "StaticPolicyDefinitionDetailTypeDef",
     "StaticPolicyDefinitionItemTypeDef",
     "StaticPolicyDefinitionTypeDef",
     "SchemaDefinitionTypeDef",
-    "PutSchemaOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateCognitoUserPoolConfigurationTypeDef",
-    "UpdateIdentitySourceOutputTypeDef",
     "UpdateStaticPolicyDefinitionTypeDef",
-    "UpdatePolicyStoreOutputTypeDef",
     "UpdatePolicyTemplateInputRequestTypeDef",
-    "UpdatePolicyTemplateOutputTypeDef",
     "AttributeValueTypeDef",
-    "CreatePolicyOutputTypeDef",
     "EntityItemTypeDef",
     "EntityReferenceTypeDef",
+    "TemplateLinkedPolicyDefinitionTypeDef",
+    "ConfigurationTypeDef",
+    "CreateIdentitySourceOutputTypeDef",
+    "CreatePolicyStoreOutputTypeDef",
+    "CreatePolicyTemplateOutputTypeDef",
+    "GetPolicyTemplateOutputTypeDef",
+    "GetSchemaOutputTypeDef",
+    "PutSchemaOutputTypeDef",
+    "UpdateIdentitySourceOutputTypeDef",
+    "UpdatePolicyStoreOutputTypeDef",
+    "UpdatePolicyTemplateOutputTypeDef",
+    "CreatePolicyOutputTypeDef",
     "TemplateLinkedPolicyDefinitionDetailTypeDef",
     "TemplateLinkedPolicyDefinitionItemTypeDef",
-    "TemplateLinkedPolicyDefinitionTypeDef",
     "UpdatePolicyOutputTypeDef",
-    "ConfigurationTypeDef",
     "CreatePolicyStoreInputRequestTypeDef",
-    "GetPolicyStoreOutputTypeDef",
     "UpdatePolicyStoreInputRequestTypeDef",
     "IsAuthorizedOutputTypeDef",
     "IsAuthorizedWithTokenOutputTypeDef",
     "GetIdentitySourceOutputTypeDef",
-    "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    "GetPolicyStoreOutputTypeDef",
     "ListIdentitySourcesInputRequestTypeDef",
     "IdentitySourceItemTypeDef",
+    "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+    "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyStoresOutputTypeDef",
     "ListPolicyTemplatesOutputTypeDef",
     "PutSchemaInputRequestTypeDef",
     "UpdateConfigurationTypeDef",
     "UpdatePolicyDefinitionTypeDef",
     "EntitiesDefinitionTypeDef",
     "PolicyFilterTypeDef",
-    "PolicyDefinitionDetailTypeDef",
-    "PolicyDefinitionItemTypeDef",
     "PolicyDefinitionTypeDef",
     "CreateIdentitySourceInputRequestTypeDef",
+    "PolicyDefinitionDetailTypeDef",
+    "PolicyDefinitionItemTypeDef",
     "ListIdentitySourcesOutputTypeDef",
     "UpdateIdentitySourceInputRequestTypeDef",
     "UpdatePolicyInputRequestTypeDef",
     "IsAuthorizedInputRequestTypeDef",
     "IsAuthorizedWithTokenInputRequestTypeDef",
     "ListPoliciesInputListPoliciesPaginateTypeDef",
     "ListPoliciesInputRequestTypeDef",
+    "CreatePolicyInputRequestTypeDef",
     "GetPolicyOutputTypeDef",
     "PolicyItemTypeDef",
-    "CreatePolicyInputRequestTypeDef",
     "ListPoliciesOutputTypeDef",
 )
 
 ActionIdentifierTypeDef = TypedDict(
     "ActionIdentifierTypeDef",
     {
         "actionType": str,
@@ -140,55 +141,50 @@
     "_OptionalCognitoUserPoolConfigurationTypeDef",
     {
         "clientIds": Sequence[str],
     },
     total=False,
 )
 
-
 class CognitoUserPoolConfigurationTypeDef(
     _RequiredCognitoUserPoolConfigurationTypeDef, _OptionalCognitoUserPoolConfigurationTypeDef
 ):
     pass
 
-
 ContextDefinitionTypeDef = TypedDict(
     "ContextDefinitionTypeDef",
     {
         "contextMap": Mapping[str, "AttributeValueTypeDef"],
     },
     total=False,
 )
 
-CreateIdentitySourceOutputTypeDef = TypedDict(
-    "CreateIdentitySourceOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-ValidationSettingsTypeDef = TypedDict(
-    "ValidationSettingsTypeDef",
+EntityIdentifierOutputTypeDef = TypedDict(
+    "EntityIdentifierOutputTypeDef",
     {
-        "mode": ValidationModeType,
+        "entityType": str,
+        "entityId": str,
     },
 )
 
-CreatePolicyStoreOutputTypeDef = TypedDict(
-    "CreatePolicyStoreOutputTypeDef",
+ValidationSettingsTypeDef = TypedDict(
+    "ValidationSettingsTypeDef",
     {
-        "policyStoreId": str,
-        "arn": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "mode": ValidationModeType,
     },
 )
 
 _RequiredCreatePolicyTemplateInputRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -200,33 +196,20 @@
     {
         "clientToken": str,
         "description": str,
     },
     total=False,
 )
 
-
 class CreatePolicyTemplateInputRequestTypeDef(
     _RequiredCreatePolicyTemplateInputRequestTypeDef,
     _OptionalCreatePolicyTemplateInputRequestTypeDef,
 ):
     pass
 
-
-CreatePolicyTemplateOutputTypeDef = TypedDict(
-    "CreatePolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIdentitySourceInputRequestTypeDef = TypedDict(
     "DeleteIdentitySourceInputRequestTypeDef",
     {
         "policyStoreId": str,
         "identitySourceId": str,
     },
 )
@@ -298,53 +281,36 @@
 GetPolicyStoreInputRequestTypeDef = TypedDict(
     "GetPolicyStoreInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 
-GetPolicyTemplateInputRequestTypeDef = TypedDict(
-    "GetPolicyTemplateInputRequestTypeDef",
+ValidationSettingsOutputTypeDef = TypedDict(
+    "ValidationSettingsOutputTypeDef",
     {
-        "policyStoreId": str,
-        "policyTemplateId": str,
+        "mode": ValidationModeType,
     },
 )
 
-GetPolicyTemplateOutputTypeDef = TypedDict(
-    "GetPolicyTemplateOutputTypeDef",
+GetPolicyTemplateInputRequestTypeDef = TypedDict(
+    "GetPolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
-        "description": str,
-        "statement": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSchemaInputRequestTypeDef = TypedDict(
     "GetSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 
-GetSchemaOutputTypeDef = TypedDict(
-    "GetSchemaOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "schema": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentitySourceFilterTypeDef = TypedDict(
     "IdentitySourceFilterTypeDef",
     {
         "principalEntityType": str,
     },
     total=False,
 )
@@ -356,18 +322,20 @@
         "userPoolArn": str,
         "discoveryUrl": str,
         "openIdIssuer": Literal["COGNITO"],
     },
     total=False,
 )
 
-ListPolicyStoresInputListPolicyStoresPaginateTypeDef = TypedDict(
-    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
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
 
 ListPolicyStoresInputRequestTypeDef = TypedDict(
     "ListPolicyStoresInputRequestTypeDef",
     {
@@ -382,36 +350,14 @@
     {
         "policyStoreId": str,
         "arn": str,
         "createdDate": datetime,
     },
 )
 
-_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
-    {
-        "policyStoreId": str,
-    },
-)
-_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(
-    _RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
-    _OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPolicyTemplatesInputRequestTypeDef = TypedDict(
     "_RequiredListPolicyTemplatesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListPolicyTemplatesInputRequestTypeDef = TypedDict(
@@ -419,21 +365,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListPolicyTemplatesInputRequestTypeDef(
     _RequiredListPolicyTemplatesInputRequestTypeDef, _OptionalListPolicyTemplatesInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPolicyTemplateItemTypeDef = TypedDict(
     "_RequiredPolicyTemplateItemTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
@@ -443,52 +387,38 @@
     "_OptionalPolicyTemplateItemTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class PolicyTemplateItemTypeDef(
     _RequiredPolicyTemplateItemTypeDef, _OptionalPolicyTemplateItemTypeDef
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
 _RequiredStaticPolicyDefinitionDetailTypeDef = TypedDict(
     "_RequiredStaticPolicyDefinitionDetailTypeDef",
     {
         "statement": str,
     },
 )
 _OptionalStaticPolicyDefinitionDetailTypeDef = TypedDict(
     "_OptionalStaticPolicyDefinitionDetailTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class StaticPolicyDefinitionDetailTypeDef(
     _RequiredStaticPolicyDefinitionDetailTypeDef, _OptionalStaticPolicyDefinitionDetailTypeDef
 ):
     pass
 
-
 StaticPolicyDefinitionItemTypeDef = TypedDict(
     "StaticPolicyDefinitionItemTypeDef",
     {
         "description": str,
     },
     total=False,
 )
@@ -503,116 +433,66 @@
     "_OptionalStaticPolicyDefinitionTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class StaticPolicyDefinitionTypeDef(
     _RequiredStaticPolicyDefinitionTypeDef, _OptionalStaticPolicyDefinitionTypeDef
 ):
     pass
 
-
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "cedarJson": str,
     },
     total=False,
 )
 
-PutSchemaOutputTypeDef = TypedDict(
-    "PutSchemaOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "namespaces": List[str],
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 _RequiredUpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
     "_RequiredUpdateCognitoUserPoolConfigurationTypeDef",
     {
         "userPoolArn": str,
     },
 )
 _OptionalUpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
     "_OptionalUpdateCognitoUserPoolConfigurationTypeDef",
     {
         "clientIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateCognitoUserPoolConfigurationTypeDef(
     _RequiredUpdateCognitoUserPoolConfigurationTypeDef,
     _OptionalUpdateCognitoUserPoolConfigurationTypeDef,
 ):
     pass
 
-
-UpdateIdentitySourceOutputTypeDef = TypedDict(
-    "UpdateIdentitySourceOutputTypeDef",
-    {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateStaticPolicyDefinitionTypeDef = TypedDict(
     "_RequiredUpdateStaticPolicyDefinitionTypeDef",
     {
         "statement": str,
     },
 )
 _OptionalUpdateStaticPolicyDefinitionTypeDef = TypedDict(
     "_OptionalUpdateStaticPolicyDefinitionTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class UpdateStaticPolicyDefinitionTypeDef(
     _RequiredUpdateStaticPolicyDefinitionTypeDef, _OptionalUpdateStaticPolicyDefinitionTypeDef
 ):
     pass
 
-
-UpdatePolicyStoreOutputTypeDef = TypedDict(
-    "UpdatePolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePolicyTemplateInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
         "statement": str,
     },
@@ -621,60 +501,33 @@
     "_OptionalUpdatePolicyTemplateInputRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class UpdatePolicyTemplateInputRequestTypeDef(
     _RequiredUpdatePolicyTemplateInputRequestTypeDef,
     _OptionalUpdatePolicyTemplateInputRequestTypeDef,
 ):
     pass
 
-
-UpdatePolicyTemplateOutputTypeDef = TypedDict(
-    "UpdatePolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "boolean": bool,
         "entityIdentifier": EntityIdentifierTypeDef,
         "long": int,
         "string": str,
         "set": Sequence[Dict[str, Any]],
         "record": Mapping[str, Dict[str, Any]],
     },
     total=False,
 )
 
-CreatePolicyOutputTypeDef = TypedDict(
-    "CreatePolicyOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyId": str,
-        "policyType": PolicyTypeType,
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEntityItemTypeDef = TypedDict(
     "_RequiredEntityItemTypeDef",
     {
         "identifier": EntityIdentifierTypeDef,
     },
 )
 _OptionalEntityItemTypeDef = TypedDict(
@@ -682,214 +535,296 @@
     {
         "attributes": Mapping[str, "AttributeValueTypeDef"],
         "parents": Sequence[EntityIdentifierTypeDef],
     },
     total=False,
 )
 
-
 class EntityItemTypeDef(_RequiredEntityItemTypeDef, _OptionalEntityItemTypeDef):
     pass
 
-
 EntityReferenceTypeDef = TypedDict(
     "EntityReferenceTypeDef",
     {
         "unspecified": bool,
         "identifier": EntityIdentifierTypeDef,
     },
     total=False,
 )
 
-_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
-    "_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef",
+_RequiredTemplateLinkedPolicyDefinitionTypeDef = TypedDict(
+    "_RequiredTemplateLinkedPolicyDefinitionTypeDef",
     {
         "policyTemplateId": str,
     },
 )
-_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
-    "_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef",
+_OptionalTemplateLinkedPolicyDefinitionTypeDef = TypedDict(
+    "_OptionalTemplateLinkedPolicyDefinitionTypeDef",
     {
         "principal": EntityIdentifierTypeDef,
         "resource": EntityIdentifierTypeDef,
     },
     total=False,
 )
 
-
-class TemplateLinkedPolicyDefinitionDetailTypeDef(
-    _RequiredTemplateLinkedPolicyDefinitionDetailTypeDef,
-    _OptionalTemplateLinkedPolicyDefinitionDetailTypeDef,
+class TemplateLinkedPolicyDefinitionTypeDef(
+    _RequiredTemplateLinkedPolicyDefinitionTypeDef, _OptionalTemplateLinkedPolicyDefinitionTypeDef
 ):
     pass
 
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "cognitoUserPoolConfiguration": CognitoUserPoolConfigurationTypeDef,
+    },
+    total=False,
+)
 
-_RequiredTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
-    "_RequiredTemplateLinkedPolicyDefinitionItemTypeDef",
+CreateIdentitySourceOutputTypeDef = TypedDict(
+    "CreateIdentitySourceOutputTypeDef",
     {
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyStoreOutputTypeDef = TypedDict(
+    "CreatePolicyStoreOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "arn": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyTemplateOutputTypeDef = TypedDict(
+    "CreatePolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
         "policyTemplateId": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
-    "_OptionalTemplateLinkedPolicyDefinitionItemTypeDef",
+
+GetPolicyTemplateOutputTypeDef = TypedDict(
+    "GetPolicyTemplateOutputTypeDef",
     {
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "description": str,
+        "statement": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetSchemaOutputTypeDef = TypedDict(
+    "GetSchemaOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "schema": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class TemplateLinkedPolicyDefinitionItemTypeDef(
-    _RequiredTemplateLinkedPolicyDefinitionItemTypeDef,
-    _OptionalTemplateLinkedPolicyDefinitionItemTypeDef,
-):
-    pass
+PutSchemaOutputTypeDef = TypedDict(
+    "PutSchemaOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "namespaces": List[str],
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateIdentitySourceOutputTypeDef = TypedDict(
+    "UpdateIdentitySourceOutputTypeDef",
+    {
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredTemplateLinkedPolicyDefinitionTypeDef = TypedDict(
-    "_RequiredTemplateLinkedPolicyDefinitionTypeDef",
+UpdatePolicyStoreOutputTypeDef = TypedDict(
+    "UpdatePolicyStoreOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "arn": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePolicyTemplateOutputTypeDef = TypedDict(
+    "UpdatePolicyTemplateOutputTypeDef",
     {
+        "policyStoreId": str,
         "policyTemplateId": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalTemplateLinkedPolicyDefinitionTypeDef = TypedDict(
-    "_OptionalTemplateLinkedPolicyDefinitionTypeDef",
+
+CreatePolicyOutputTypeDef = TypedDict(
+    "CreatePolicyOutputTypeDef",
     {
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
+        "policyStoreId": str,
+        "policyId": str,
+        "policyType": PolicyTypeType,
+        "principal": EntityIdentifierOutputTypeDef,
+        "resource": EntityIdentifierOutputTypeDef,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
+    "_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef",
+    {
+        "policyTemplateId": str,
+    },
+)
+_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
+    "_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef",
+    {
+        "principal": EntityIdentifierOutputTypeDef,
+        "resource": EntityIdentifierOutputTypeDef,
+    },
+    total=False,
+)
 
-class TemplateLinkedPolicyDefinitionTypeDef(
-    _RequiredTemplateLinkedPolicyDefinitionTypeDef, _OptionalTemplateLinkedPolicyDefinitionTypeDef
+class TemplateLinkedPolicyDefinitionDetailTypeDef(
+    _RequiredTemplateLinkedPolicyDefinitionDetailTypeDef,
+    _OptionalTemplateLinkedPolicyDefinitionDetailTypeDef,
 ):
     pass
 
+_RequiredTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
+    "_RequiredTemplateLinkedPolicyDefinitionItemTypeDef",
+    {
+        "policyTemplateId": str,
+    },
+)
+_OptionalTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
+    "_OptionalTemplateLinkedPolicyDefinitionItemTypeDef",
+    {
+        "principal": EntityIdentifierOutputTypeDef,
+        "resource": EntityIdentifierOutputTypeDef,
+    },
+    total=False,
+)
+
+class TemplateLinkedPolicyDefinitionItemTypeDef(
+    _RequiredTemplateLinkedPolicyDefinitionItemTypeDef,
+    _OptionalTemplateLinkedPolicyDefinitionItemTypeDef,
+):
+    pass
 
 UpdatePolicyOutputTypeDef = TypedDict(
     "UpdatePolicyOutputTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
         "policyType": PolicyTypeType,
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
+        "principal": EntityIdentifierOutputTypeDef,
+        "resource": EntityIdentifierOutputTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "cognitoUserPoolConfiguration": CognitoUserPoolConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreatePolicyStoreInputRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyStoreInputRequestTypeDef",
     {
         "validationSettings": ValidationSettingsTypeDef,
     },
 )
 _OptionalCreatePolicyStoreInputRequestTypeDef = TypedDict(
     "_OptionalCreatePolicyStoreInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreatePolicyStoreInputRequestTypeDef(
     _RequiredCreatePolicyStoreInputRequestTypeDef, _OptionalCreatePolicyStoreInputRequestTypeDef
 ):
     pass
 
-
-GetPolicyStoreOutputTypeDef = TypedDict(
-    "GetPolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "validationSettings": ValidationSettingsTypeDef,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdatePolicyStoreInputRequestTypeDef = TypedDict(
     "UpdatePolicyStoreInputRequestTypeDef",
     {
         "policyStoreId": str,
         "validationSettings": ValidationSettingsTypeDef,
     },
 )
 
 IsAuthorizedOutputTypeDef = TypedDict(
     "IsAuthorizedOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IsAuthorizedWithTokenOutputTypeDef = TypedDict(
     "IsAuthorizedWithTokenOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentitySourceOutputTypeDef = TypedDict(
     "GetIdentitySourceOutputTypeDef",
     {
         "createdDate": datetime,
         "details": IdentitySourceDetailsTypeDef,
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "principalEntityType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
-    "_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+GetPolicyStoreOutputTypeDef = TypedDict(
+    "GetPolicyStoreOutputTypeDef",
     {
         "policyStoreId": str,
+        "arn": str,
+        "validationSettings": ValidationSettingsOutputTypeDef,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
-    "_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
-    {
-        "filters": Sequence[IdentitySourceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef(
-    _RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
-    _OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
-):
-    pass
-
 
 _RequiredListIdentitySourcesInputRequestTypeDef = TypedDict(
     "_RequiredListIdentitySourcesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
@@ -899,48 +834,95 @@
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[IdentitySourceFilterTypeDef],
     },
     total=False,
 )
 
-
 class ListIdentitySourcesInputRequestTypeDef(
     _RequiredListIdentitySourcesInputRequestTypeDef, _OptionalListIdentitySourcesInputRequestTypeDef
 ):
     pass
 
-
 IdentitySourceItemTypeDef = TypedDict(
     "IdentitySourceItemTypeDef",
     {
         "createdDate": datetime,
         "details": IdentitySourceItemDetailsTypeDef,
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "principalEntityType": str,
     },
 )
 
+_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
+    "_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    {
+        "policyStoreId": str,
+    },
+)
+_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
+    "_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    {
+        "filters": Sequence[IdentitySourceFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef(
+    _RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    _OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+):
+    pass
+
+ListPolicyStoresInputListPolicyStoresPaginateTypeDef = TypedDict(
+    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
+    {
+        "policyStoreId": str,
+    },
+)
+_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(
+    _RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
+    _OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
+):
+    pass
+
 ListPolicyStoresOutputTypeDef = TypedDict(
     "ListPolicyStoresOutputTypeDef",
     {
         "nextToken": str,
         "policyStores": List[PolicyStoreItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPolicyTemplatesOutputTypeDef = TypedDict(
     "ListPolicyTemplatesOutputTypeDef",
     {
         "nextToken": str,
         "policyTemplates": List[PolicyTemplateItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSchemaInputRequestTypeDef = TypedDict(
     "PutSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -979,32 +961,14 @@
         "resource": EntityReferenceTypeDef,
         "policyType": PolicyTypeType,
         "policyTemplateId": str,
     },
     total=False,
 )
 
-PolicyDefinitionDetailTypeDef = TypedDict(
-    "PolicyDefinitionDetailTypeDef",
-    {
-        "static": StaticPolicyDefinitionDetailTypeDef,
-        "templateLinked": TemplateLinkedPolicyDefinitionDetailTypeDef,
-    },
-    total=False,
-)
-
-PolicyDefinitionItemTypeDef = TypedDict(
-    "PolicyDefinitionItemTypeDef",
-    {
-        "static": StaticPolicyDefinitionItemTypeDef,
-        "templateLinked": TemplateLinkedPolicyDefinitionItemTypeDef,
-    },
-    total=False,
-)
-
 PolicyDefinitionTypeDef = TypedDict(
     "PolicyDefinitionTypeDef",
     {
         "static": StaticPolicyDefinitionTypeDef,
         "templateLinked": TemplateLinkedPolicyDefinitionTypeDef,
     },
     total=False,
@@ -1022,28 +986,44 @@
     {
         "clientToken": str,
         "principalEntityType": str,
     },
     total=False,
 )
 
-
 class CreateIdentitySourceInputRequestTypeDef(
     _RequiredCreateIdentitySourceInputRequestTypeDef,
     _OptionalCreateIdentitySourceInputRequestTypeDef,
 ):
     pass
 
+PolicyDefinitionDetailTypeDef = TypedDict(
+    "PolicyDefinitionDetailTypeDef",
+    {
+        "static": StaticPolicyDefinitionDetailTypeDef,
+        "templateLinked": TemplateLinkedPolicyDefinitionDetailTypeDef,
+    },
+    total=False,
+)
+
+PolicyDefinitionItemTypeDef = TypedDict(
+    "PolicyDefinitionItemTypeDef",
+    {
+        "static": StaticPolicyDefinitionItemTypeDef,
+        "templateLinked": TemplateLinkedPolicyDefinitionItemTypeDef,
+    },
+    total=False,
+)
 
 ListIdentitySourcesOutputTypeDef = TypedDict(
     "ListIdentitySourcesOutputTypeDef",
     {
         "nextToken": str,
         "identitySources": List[IdentitySourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateIdentitySourceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentitySourceInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -1055,22 +1035,20 @@
     "_OptionalUpdateIdentitySourceInputRequestTypeDef",
     {
         "principalEntityType": str,
     },
     total=False,
 )
 
-
 class UpdateIdentitySourceInputRequestTypeDef(
     _RequiredUpdateIdentitySourceInputRequestTypeDef,
     _OptionalUpdateIdentitySourceInputRequestTypeDef,
 ):
     pass
 
-
 UpdatePolicyInputRequestTypeDef = TypedDict(
     "UpdatePolicyInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
         "definition": UpdatePolicyDefinitionTypeDef,
     },
@@ -1090,21 +1068,19 @@
         "resource": EntityIdentifierTypeDef,
         "context": ContextDefinitionTypeDef,
         "entities": EntitiesDefinitionTypeDef,
     },
     total=False,
 )
 
-
 class IsAuthorizedInputRequestTypeDef(
     _RequiredIsAuthorizedInputRequestTypeDef, _OptionalIsAuthorizedInputRequestTypeDef
 ):
     pass
 
-
 _RequiredIsAuthorizedWithTokenInputRequestTypeDef = TypedDict(
     "_RequiredIsAuthorizedWithTokenInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalIsAuthorizedWithTokenInputRequestTypeDef = TypedDict(
@@ -1116,45 +1092,41 @@
         "resource": EntityIdentifierTypeDef,
         "context": ContextDefinitionTypeDef,
         "entities": EntitiesDefinitionTypeDef,
     },
     total=False,
 )
 
-
 class IsAuthorizedWithTokenInputRequestTypeDef(
     _RequiredIsAuthorizedWithTokenInputRequestTypeDef,
     _OptionalIsAuthorizedWithTokenInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredListPoliciesInputListPoliciesPaginateTypeDef = TypedDict(
     "_RequiredListPoliciesInputListPoliciesPaginateTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListPoliciesInputListPoliciesPaginateTypeDef = TypedDict(
     "_OptionalListPoliciesInputListPoliciesPaginateTypeDef",
     {
         "filter": PolicyFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListPoliciesInputListPoliciesPaginateTypeDef(
     _RequiredListPoliciesInputListPoliciesPaginateTypeDef,
     _OptionalListPoliciesInputListPoliciesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListPoliciesInputRequestTypeDef = TypedDict(
     "_RequiredListPoliciesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListPoliciesInputRequestTypeDef = TypedDict(
@@ -1163,33 +1135,51 @@
         "nextToken": str,
         "maxResults": int,
         "filter": PolicyFilterTypeDef,
     },
     total=False,
 )
 
-
 class ListPoliciesInputRequestTypeDef(
     _RequiredListPoliciesInputRequestTypeDef, _OptionalListPoliciesInputRequestTypeDef
 ):
     pass
 
+_RequiredCreatePolicyInputRequestTypeDef = TypedDict(
+    "_RequiredCreatePolicyInputRequestTypeDef",
+    {
+        "policyStoreId": str,
+        "definition": PolicyDefinitionTypeDef,
+    },
+)
+_OptionalCreatePolicyInputRequestTypeDef = TypedDict(
+    "_OptionalCreatePolicyInputRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class CreatePolicyInputRequestTypeDef(
+    _RequiredCreatePolicyInputRequestTypeDef, _OptionalCreatePolicyInputRequestTypeDef
+):
+    pass
 
 GetPolicyOutputTypeDef = TypedDict(
     "GetPolicyOutputTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
         "policyType": PolicyTypeType,
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
+        "principal": EntityIdentifierOutputTypeDef,
+        "resource": EntityIdentifierOutputTypeDef,
         "definition": PolicyDefinitionDetailTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPolicyItemTypeDef = TypedDict(
     "_RequiredPolicyItemTypeDef",
     {
         "policyStoreId": str,
@@ -1199,48 +1189,24 @@
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
     },
 )
 _OptionalPolicyItemTypeDef = TypedDict(
     "_OptionalPolicyItemTypeDef",
     {
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
+        "principal": EntityIdentifierOutputTypeDef,
+        "resource": EntityIdentifierOutputTypeDef,
     },
     total=False,
 )
 
-
 class PolicyItemTypeDef(_RequiredPolicyItemTypeDef, _OptionalPolicyItemTypeDef):
     pass
 
-
-_RequiredCreatePolicyInputRequestTypeDef = TypedDict(
-    "_RequiredCreatePolicyInputRequestTypeDef",
-    {
-        "policyStoreId": str,
-        "definition": PolicyDefinitionTypeDef,
-    },
-)
-_OptionalCreatePolicyInputRequestTypeDef = TypedDict(
-    "_OptionalCreatePolicyInputRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class CreatePolicyInputRequestTypeDef(
-    _RequiredCreatePolicyInputRequestTypeDef, _OptionalCreatePolicyInputRequestTypeDef
-):
-    pass
-
-
 ListPoliciesOutputTypeDef = TypedDict(
     "ListPoliciesOutputTypeDef",
     {
         "nextToken": str,
         "policies": List[PolicyItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions/type_defs.pyi` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,98 +22,101 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActionIdentifierTypeDef",
     "EntityIdentifierTypeDef",
     "CognitoUserPoolConfigurationTypeDef",
     "ContextDefinitionTypeDef",
-    "CreateIdentitySourceOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "EntityIdentifierOutputTypeDef",
     "ValidationSettingsTypeDef",
-    "CreatePolicyStoreOutputTypeDef",
     "CreatePolicyTemplateInputRequestTypeDef",
-    "CreatePolicyTemplateOutputTypeDef",
     "DeleteIdentitySourceInputRequestTypeDef",
     "DeletePolicyInputRequestTypeDef",
     "DeletePolicyStoreInputRequestTypeDef",
     "DeletePolicyTemplateInputRequestTypeDef",
     "DeterminingPolicyItemTypeDef",
     "EvaluationErrorItemTypeDef",
     "GetIdentitySourceInputRequestTypeDef",
     "IdentitySourceDetailsTypeDef",
     "GetPolicyInputRequestTypeDef",
     "GetPolicyStoreInputRequestTypeDef",
+    "ValidationSettingsOutputTypeDef",
     "GetPolicyTemplateInputRequestTypeDef",
-    "GetPolicyTemplateOutputTypeDef",
     "GetSchemaInputRequestTypeDef",
-    "GetSchemaOutputTypeDef",
     "IdentitySourceFilterTypeDef",
     "IdentitySourceItemDetailsTypeDef",
-    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListPolicyStoresInputRequestTypeDef",
     "PolicyStoreItemTypeDef",
-    "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyTemplatesInputRequestTypeDef",
     "PolicyTemplateItemTypeDef",
-    "PaginatorConfigTypeDef",
     "StaticPolicyDefinitionDetailTypeDef",
     "StaticPolicyDefinitionItemTypeDef",
     "StaticPolicyDefinitionTypeDef",
     "SchemaDefinitionTypeDef",
-    "PutSchemaOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateCognitoUserPoolConfigurationTypeDef",
-    "UpdateIdentitySourceOutputTypeDef",
     "UpdateStaticPolicyDefinitionTypeDef",
-    "UpdatePolicyStoreOutputTypeDef",
     "UpdatePolicyTemplateInputRequestTypeDef",
-    "UpdatePolicyTemplateOutputTypeDef",
     "AttributeValueTypeDef",
-    "CreatePolicyOutputTypeDef",
     "EntityItemTypeDef",
     "EntityReferenceTypeDef",
+    "TemplateLinkedPolicyDefinitionTypeDef",
+    "ConfigurationTypeDef",
+    "CreateIdentitySourceOutputTypeDef",
+    "CreatePolicyStoreOutputTypeDef",
+    "CreatePolicyTemplateOutputTypeDef",
+    "GetPolicyTemplateOutputTypeDef",
+    "GetSchemaOutputTypeDef",
+    "PutSchemaOutputTypeDef",
+    "UpdateIdentitySourceOutputTypeDef",
+    "UpdatePolicyStoreOutputTypeDef",
+    "UpdatePolicyTemplateOutputTypeDef",
+    "CreatePolicyOutputTypeDef",
     "TemplateLinkedPolicyDefinitionDetailTypeDef",
     "TemplateLinkedPolicyDefinitionItemTypeDef",
-    "TemplateLinkedPolicyDefinitionTypeDef",
     "UpdatePolicyOutputTypeDef",
-    "ConfigurationTypeDef",
     "CreatePolicyStoreInputRequestTypeDef",
-    "GetPolicyStoreOutputTypeDef",
     "UpdatePolicyStoreInputRequestTypeDef",
     "IsAuthorizedOutputTypeDef",
     "IsAuthorizedWithTokenOutputTypeDef",
     "GetIdentitySourceOutputTypeDef",
-    "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    "GetPolicyStoreOutputTypeDef",
     "ListIdentitySourcesInputRequestTypeDef",
     "IdentitySourceItemTypeDef",
+    "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+    "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyStoresOutputTypeDef",
     "ListPolicyTemplatesOutputTypeDef",
     "PutSchemaInputRequestTypeDef",
     "UpdateConfigurationTypeDef",
     "UpdatePolicyDefinitionTypeDef",
     "EntitiesDefinitionTypeDef",
     "PolicyFilterTypeDef",
-    "PolicyDefinitionDetailTypeDef",
-    "PolicyDefinitionItemTypeDef",
     "PolicyDefinitionTypeDef",
     "CreateIdentitySourceInputRequestTypeDef",
+    "PolicyDefinitionDetailTypeDef",
+    "PolicyDefinitionItemTypeDef",
     "ListIdentitySourcesOutputTypeDef",
     "UpdateIdentitySourceInputRequestTypeDef",
     "UpdatePolicyInputRequestTypeDef",
     "IsAuthorizedInputRequestTypeDef",
     "IsAuthorizedWithTokenInputRequestTypeDef",
     "ListPoliciesInputListPoliciesPaginateTypeDef",
     "ListPoliciesInputRequestTypeDef",
+    "CreatePolicyInputRequestTypeDef",
     "GetPolicyOutputTypeDef",
     "PolicyItemTypeDef",
-    "CreatePolicyInputRequestTypeDef",
     "ListPoliciesOutputTypeDef",
 )
 
 ActionIdentifierTypeDef = TypedDict(
     "ActionIdentifierTypeDef",
     {
         "actionType": str,
@@ -139,53 +142,52 @@
     "_OptionalCognitoUserPoolConfigurationTypeDef",
     {
         "clientIds": Sequence[str],
     },
     total=False,
 )
 
+
 class CognitoUserPoolConfigurationTypeDef(
     _RequiredCognitoUserPoolConfigurationTypeDef, _OptionalCognitoUserPoolConfigurationTypeDef
 ):
     pass
 
+
 ContextDefinitionTypeDef = TypedDict(
     "ContextDefinitionTypeDef",
     {
         "contextMap": Mapping[str, "AttributeValueTypeDef"],
     },
     total=False,
 )
 
-CreateIdentitySourceOutputTypeDef = TypedDict(
-    "CreateIdentitySourceOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-ValidationSettingsTypeDef = TypedDict(
-    "ValidationSettingsTypeDef",
+EntityIdentifierOutputTypeDef = TypedDict(
+    "EntityIdentifierOutputTypeDef",
     {
-        "mode": ValidationModeType,
+        "entityType": str,
+        "entityId": str,
     },
 )
 
-CreatePolicyStoreOutputTypeDef = TypedDict(
-    "CreatePolicyStoreOutputTypeDef",
+ValidationSettingsTypeDef = TypedDict(
+    "ValidationSettingsTypeDef",
     {
-        "policyStoreId": str,
-        "arn": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "mode": ValidationModeType,
     },
 )
 
 _RequiredCreatePolicyTemplateInputRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -197,30 +199,21 @@
     {
         "clientToken": str,
         "description": str,
     },
     total=False,
 )
 
+
 class CreatePolicyTemplateInputRequestTypeDef(
     _RequiredCreatePolicyTemplateInputRequestTypeDef,
     _OptionalCreatePolicyTemplateInputRequestTypeDef,
 ):
     pass
 
-CreatePolicyTemplateOutputTypeDef = TypedDict(
-    "CreatePolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteIdentitySourceInputRequestTypeDef = TypedDict(
     "DeleteIdentitySourceInputRequestTypeDef",
     {
         "policyStoreId": str,
         "identitySourceId": str,
     },
@@ -293,53 +286,36 @@
 GetPolicyStoreInputRequestTypeDef = TypedDict(
     "GetPolicyStoreInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 
-GetPolicyTemplateInputRequestTypeDef = TypedDict(
-    "GetPolicyTemplateInputRequestTypeDef",
+ValidationSettingsOutputTypeDef = TypedDict(
+    "ValidationSettingsOutputTypeDef",
     {
-        "policyStoreId": str,
-        "policyTemplateId": str,
+        "mode": ValidationModeType,
     },
 )
 
-GetPolicyTemplateOutputTypeDef = TypedDict(
-    "GetPolicyTemplateOutputTypeDef",
+GetPolicyTemplateInputRequestTypeDef = TypedDict(
+    "GetPolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
-        "description": str,
-        "statement": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSchemaInputRequestTypeDef = TypedDict(
     "GetSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 
-GetSchemaOutputTypeDef = TypedDict(
-    "GetSchemaOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "schema": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentitySourceFilterTypeDef = TypedDict(
     "IdentitySourceFilterTypeDef",
     {
         "principalEntityType": str,
     },
     total=False,
 )
@@ -351,18 +327,20 @@
         "userPoolArn": str,
         "discoveryUrl": str,
         "openIdIssuer": Literal["COGNITO"],
     },
     total=False,
 )
 
-ListPolicyStoresInputListPolicyStoresPaginateTypeDef = TypedDict(
-    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
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
 
 ListPolicyStoresInputRequestTypeDef = TypedDict(
     "ListPolicyStoresInputRequestTypeDef",
     {
@@ -377,34 +355,14 @@
     {
         "policyStoreId": str,
         "arn": str,
         "createdDate": datetime,
     },
 )
 
-_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
-    {
-        "policyStoreId": str,
-    },
-)
-_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(
-    _RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
-    _OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
-):
-    pass
-
 _RequiredListPolicyTemplatesInputRequestTypeDef = TypedDict(
     "_RequiredListPolicyTemplatesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListPolicyTemplatesInputRequestTypeDef = TypedDict(
@@ -412,19 +370,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListPolicyTemplatesInputRequestTypeDef(
     _RequiredListPolicyTemplatesInputRequestTypeDef, _OptionalListPolicyTemplatesInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPolicyTemplateItemTypeDef = TypedDict(
     "_RequiredPolicyTemplateItemTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
@@ -434,28 +394,20 @@
     "_OptionalPolicyTemplateItemTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class PolicyTemplateItemTypeDef(
     _RequiredPolicyTemplateItemTypeDef, _OptionalPolicyTemplateItemTypeDef
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
 
 _RequiredStaticPolicyDefinitionDetailTypeDef = TypedDict(
     "_RequiredStaticPolicyDefinitionDetailTypeDef",
     {
         "statement": str,
     },
 )
@@ -463,19 +415,21 @@
     "_OptionalStaticPolicyDefinitionDetailTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class StaticPolicyDefinitionDetailTypeDef(
     _RequiredStaticPolicyDefinitionDetailTypeDef, _OptionalStaticPolicyDefinitionDetailTypeDef
 ):
     pass
 
+
 StaticPolicyDefinitionItemTypeDef = TypedDict(
     "StaticPolicyDefinitionItemTypeDef",
     {
         "description": str,
     },
     total=False,
 )
@@ -490,79 +444,50 @@
     "_OptionalStaticPolicyDefinitionTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class StaticPolicyDefinitionTypeDef(
     _RequiredStaticPolicyDefinitionTypeDef, _OptionalStaticPolicyDefinitionTypeDef
 ):
     pass
 
+
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "cedarJson": str,
     },
     total=False,
 )
 
-PutSchemaOutputTypeDef = TypedDict(
-    "PutSchemaOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "namespaces": List[str],
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 _RequiredUpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
     "_RequiredUpdateCognitoUserPoolConfigurationTypeDef",
     {
         "userPoolArn": str,
     },
 )
 _OptionalUpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
     "_OptionalUpdateCognitoUserPoolConfigurationTypeDef",
     {
         "clientIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateCognitoUserPoolConfigurationTypeDef(
     _RequiredUpdateCognitoUserPoolConfigurationTypeDef,
     _OptionalUpdateCognitoUserPoolConfigurationTypeDef,
 ):
     pass
 
-UpdateIdentitySourceOutputTypeDef = TypedDict(
-    "UpdateIdentitySourceOutputTypeDef",
-    {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateStaticPolicyDefinitionTypeDef = TypedDict(
     "_RequiredUpdateStaticPolicyDefinitionTypeDef",
     {
         "statement": str,
     },
 )
@@ -570,29 +495,20 @@
     "_OptionalUpdateStaticPolicyDefinitionTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class UpdateStaticPolicyDefinitionTypeDef(
     _RequiredUpdateStaticPolicyDefinitionTypeDef, _OptionalUpdateStaticPolicyDefinitionTypeDef
 ):
     pass
 
-UpdatePolicyStoreOutputTypeDef = TypedDict(
-    "UpdatePolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdatePolicyTemplateInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
         "statement": str,
@@ -602,58 +518,35 @@
     "_OptionalUpdatePolicyTemplateInputRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class UpdatePolicyTemplateInputRequestTypeDef(
     _RequiredUpdatePolicyTemplateInputRequestTypeDef,
     _OptionalUpdatePolicyTemplateInputRequestTypeDef,
 ):
     pass
 
-UpdatePolicyTemplateOutputTypeDef = TypedDict(
-    "UpdatePolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "boolean": bool,
         "entityIdentifier": EntityIdentifierTypeDef,
         "long": int,
         "string": str,
         "set": Sequence[Dict[str, Any]],
         "record": Mapping[str, Dict[str, Any]],
     },
     total=False,
 )
 
-CreatePolicyOutputTypeDef = TypedDict(
-    "CreatePolicyOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyId": str,
-        "policyType": PolicyTypeType,
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEntityItemTypeDef = TypedDict(
     "_RequiredEntityItemTypeDef",
     {
         "identifier": EntityIdentifierTypeDef,
     },
 )
 _OptionalEntityItemTypeDef = TypedDict(
@@ -661,140 +554,253 @@
     {
         "attributes": Mapping[str, "AttributeValueTypeDef"],
         "parents": Sequence[EntityIdentifierTypeDef],
     },
     total=False,
 )
 
+
 class EntityItemTypeDef(_RequiredEntityItemTypeDef, _OptionalEntityItemTypeDef):
     pass
 
+
 EntityReferenceTypeDef = TypedDict(
     "EntityReferenceTypeDef",
     {
         "unspecified": bool,
         "identifier": EntityIdentifierTypeDef,
     },
     total=False,
 )
 
+_RequiredTemplateLinkedPolicyDefinitionTypeDef = TypedDict(
+    "_RequiredTemplateLinkedPolicyDefinitionTypeDef",
+    {
+        "policyTemplateId": str,
+    },
+)
+_OptionalTemplateLinkedPolicyDefinitionTypeDef = TypedDict(
+    "_OptionalTemplateLinkedPolicyDefinitionTypeDef",
+    {
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
+    },
+    total=False,
+)
+
+
+class TemplateLinkedPolicyDefinitionTypeDef(
+    _RequiredTemplateLinkedPolicyDefinitionTypeDef, _OptionalTemplateLinkedPolicyDefinitionTypeDef
+):
+    pass
+
+
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "cognitoUserPoolConfiguration": CognitoUserPoolConfigurationTypeDef,
+    },
+    total=False,
+)
+
+CreateIdentitySourceOutputTypeDef = TypedDict(
+    "CreateIdentitySourceOutputTypeDef",
+    {
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyStoreOutputTypeDef = TypedDict(
+    "CreatePolicyStoreOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "arn": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyTemplateOutputTypeDef = TypedDict(
+    "CreatePolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyTemplateOutputTypeDef = TypedDict(
+    "GetPolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "description": str,
+        "statement": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSchemaOutputTypeDef = TypedDict(
+    "GetSchemaOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "schema": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSchemaOutputTypeDef = TypedDict(
+    "PutSchemaOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "namespaces": List[str],
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateIdentitySourceOutputTypeDef = TypedDict(
+    "UpdateIdentitySourceOutputTypeDef",
+    {
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePolicyStoreOutputTypeDef = TypedDict(
+    "UpdatePolicyStoreOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "arn": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePolicyTemplateOutputTypeDef = TypedDict(
+    "UpdatePolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyOutputTypeDef = TypedDict(
+    "CreatePolicyOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyId": str,
+        "policyType": PolicyTypeType,
+        "principal": EntityIdentifierOutputTypeDef,
+        "resource": EntityIdentifierOutputTypeDef,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
     "_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef",
     {
         "policyTemplateId": str,
     },
 )
 _OptionalTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
     "_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef",
     {
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
+        "principal": EntityIdentifierOutputTypeDef,
+        "resource": EntityIdentifierOutputTypeDef,
     },
     total=False,
 )
 
+
 class TemplateLinkedPolicyDefinitionDetailTypeDef(
     _RequiredTemplateLinkedPolicyDefinitionDetailTypeDef,
     _OptionalTemplateLinkedPolicyDefinitionDetailTypeDef,
 ):
     pass
 
+
 _RequiredTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
     "_RequiredTemplateLinkedPolicyDefinitionItemTypeDef",
     {
         "policyTemplateId": str,
     },
 )
 _OptionalTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
     "_OptionalTemplateLinkedPolicyDefinitionItemTypeDef",
     {
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
+        "principal": EntityIdentifierOutputTypeDef,
+        "resource": EntityIdentifierOutputTypeDef,
     },
     total=False,
 )
 
+
 class TemplateLinkedPolicyDefinitionItemTypeDef(
     _RequiredTemplateLinkedPolicyDefinitionItemTypeDef,
     _OptionalTemplateLinkedPolicyDefinitionItemTypeDef,
 ):
     pass
 
-_RequiredTemplateLinkedPolicyDefinitionTypeDef = TypedDict(
-    "_RequiredTemplateLinkedPolicyDefinitionTypeDef",
-    {
-        "policyTemplateId": str,
-    },
-)
-_OptionalTemplateLinkedPolicyDefinitionTypeDef = TypedDict(
-    "_OptionalTemplateLinkedPolicyDefinitionTypeDef",
-    {
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
-    },
-    total=False,
-)
-
-class TemplateLinkedPolicyDefinitionTypeDef(
-    _RequiredTemplateLinkedPolicyDefinitionTypeDef, _OptionalTemplateLinkedPolicyDefinitionTypeDef
-):
-    pass
 
 UpdatePolicyOutputTypeDef = TypedDict(
     "UpdatePolicyOutputTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
         "policyType": PolicyTypeType,
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
+        "principal": EntityIdentifierOutputTypeDef,
+        "resource": EntityIdentifierOutputTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "cognitoUserPoolConfiguration": CognitoUserPoolConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreatePolicyStoreInputRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyStoreInputRequestTypeDef",
     {
         "validationSettings": ValidationSettingsTypeDef,
     },
 )
 _OptionalCreatePolicyStoreInputRequestTypeDef = TypedDict(
     "_OptionalCreatePolicyStoreInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreatePolicyStoreInputRequestTypeDef(
     _RequiredCreatePolicyStoreInputRequestTypeDef, _OptionalCreatePolicyStoreInputRequestTypeDef
 ):
     pass
 
-GetPolicyStoreOutputTypeDef = TypedDict(
-    "GetPolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "validationSettings": ValidationSettingsTypeDef,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UpdatePolicyStoreInputRequestTypeDef = TypedDict(
     "UpdatePolicyStoreInputRequestTypeDef",
     {
         "policyStoreId": str,
         "validationSettings": ValidationSettingsTypeDef,
     },
@@ -802,61 +808,52 @@
 
 IsAuthorizedOutputTypeDef = TypedDict(
     "IsAuthorizedOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IsAuthorizedWithTokenOutputTypeDef = TypedDict(
     "IsAuthorizedWithTokenOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentitySourceOutputTypeDef = TypedDict(
     "GetIdentitySourceOutputTypeDef",
     {
         "createdDate": datetime,
         "details": IdentitySourceDetailsTypeDef,
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "principalEntityType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
-    "_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+GetPolicyStoreOutputTypeDef = TypedDict(
+    "GetPolicyStoreOutputTypeDef",
     {
         "policyStoreId": str,
+        "arn": str,
+        "validationSettings": ValidationSettingsOutputTypeDef,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
-    "_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
-    {
-        "filters": Sequence[IdentitySourceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef(
-    _RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
-    _OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
-):
-    pass
 
 _RequiredListIdentitySourcesInputRequestTypeDef = TypedDict(
     "_RequiredListIdentitySourcesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
@@ -866,46 +863,101 @@
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[IdentitySourceFilterTypeDef],
     },
     total=False,
 )
 
+
 class ListIdentitySourcesInputRequestTypeDef(
     _RequiredListIdentitySourcesInputRequestTypeDef, _OptionalListIdentitySourcesInputRequestTypeDef
 ):
     pass
 
+
 IdentitySourceItemTypeDef = TypedDict(
     "IdentitySourceItemTypeDef",
     {
         "createdDate": datetime,
         "details": IdentitySourceItemDetailsTypeDef,
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "principalEntityType": str,
     },
 )
 
+_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
+    "_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    {
+        "policyStoreId": str,
+    },
+)
+_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
+    "_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    {
+        "filters": Sequence[IdentitySourceFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef(
+    _RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    _OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+):
+    pass
+
+
+ListPolicyStoresInputListPolicyStoresPaginateTypeDef = TypedDict(
+    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
+    {
+        "policyStoreId": str,
+    },
+)
+_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(
+    _RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
+    _OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
+):
+    pass
+
+
 ListPolicyStoresOutputTypeDef = TypedDict(
     "ListPolicyStoresOutputTypeDef",
     {
         "nextToken": str,
         "policyStores": List[PolicyStoreItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPolicyTemplatesOutputTypeDef = TypedDict(
     "ListPolicyTemplatesOutputTypeDef",
     {
         "nextToken": str,
         "policyTemplates": List[PolicyTemplateItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSchemaInputRequestTypeDef = TypedDict(
     "PutSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -944,32 +996,14 @@
         "resource": EntityReferenceTypeDef,
         "policyType": PolicyTypeType,
         "policyTemplateId": str,
     },
     total=False,
 )
 
-PolicyDefinitionDetailTypeDef = TypedDict(
-    "PolicyDefinitionDetailTypeDef",
-    {
-        "static": StaticPolicyDefinitionDetailTypeDef,
-        "templateLinked": TemplateLinkedPolicyDefinitionDetailTypeDef,
-    },
-    total=False,
-)
-
-PolicyDefinitionItemTypeDef = TypedDict(
-    "PolicyDefinitionItemTypeDef",
-    {
-        "static": StaticPolicyDefinitionItemTypeDef,
-        "templateLinked": TemplateLinkedPolicyDefinitionItemTypeDef,
-    },
-    total=False,
-)
-
 PolicyDefinitionTypeDef = TypedDict(
     "PolicyDefinitionTypeDef",
     {
         "static": StaticPolicyDefinitionTypeDef,
         "templateLinked": TemplateLinkedPolicyDefinitionTypeDef,
     },
     total=False,
@@ -987,26 +1021,46 @@
     {
         "clientToken": str,
         "principalEntityType": str,
     },
     total=False,
 )
 
+
 class CreateIdentitySourceInputRequestTypeDef(
     _RequiredCreateIdentitySourceInputRequestTypeDef,
     _OptionalCreateIdentitySourceInputRequestTypeDef,
 ):
     pass
 
+
+PolicyDefinitionDetailTypeDef = TypedDict(
+    "PolicyDefinitionDetailTypeDef",
+    {
+        "static": StaticPolicyDefinitionDetailTypeDef,
+        "templateLinked": TemplateLinkedPolicyDefinitionDetailTypeDef,
+    },
+    total=False,
+)
+
+PolicyDefinitionItemTypeDef = TypedDict(
+    "PolicyDefinitionItemTypeDef",
+    {
+        "static": StaticPolicyDefinitionItemTypeDef,
+        "templateLinked": TemplateLinkedPolicyDefinitionItemTypeDef,
+    },
+    total=False,
+)
+
 ListIdentitySourcesOutputTypeDef = TypedDict(
     "ListIdentitySourcesOutputTypeDef",
     {
         "nextToken": str,
         "identitySources": List[IdentitySourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateIdentitySourceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentitySourceInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -1018,20 +1072,22 @@
     "_OptionalUpdateIdentitySourceInputRequestTypeDef",
     {
         "principalEntityType": str,
     },
     total=False,
 )
 
+
 class UpdateIdentitySourceInputRequestTypeDef(
     _RequiredUpdateIdentitySourceInputRequestTypeDef,
     _OptionalUpdateIdentitySourceInputRequestTypeDef,
 ):
     pass
 
+
 UpdatePolicyInputRequestTypeDef = TypedDict(
     "UpdatePolicyInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
         "definition": UpdatePolicyDefinitionTypeDef,
     },
@@ -1051,19 +1107,21 @@
         "resource": EntityIdentifierTypeDef,
         "context": ContextDefinitionTypeDef,
         "entities": EntitiesDefinitionTypeDef,
     },
     total=False,
 )
 
+
 class IsAuthorizedInputRequestTypeDef(
     _RequiredIsAuthorizedInputRequestTypeDef, _OptionalIsAuthorizedInputRequestTypeDef
 ):
     pass
 
+
 _RequiredIsAuthorizedWithTokenInputRequestTypeDef = TypedDict(
     "_RequiredIsAuthorizedWithTokenInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalIsAuthorizedWithTokenInputRequestTypeDef = TypedDict(
@@ -1075,41 +1133,45 @@
         "resource": EntityIdentifierTypeDef,
         "context": ContextDefinitionTypeDef,
         "entities": EntitiesDefinitionTypeDef,
     },
     total=False,
 )
 
+
 class IsAuthorizedWithTokenInputRequestTypeDef(
     _RequiredIsAuthorizedWithTokenInputRequestTypeDef,
     _OptionalIsAuthorizedWithTokenInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredListPoliciesInputListPoliciesPaginateTypeDef = TypedDict(
     "_RequiredListPoliciesInputListPoliciesPaginateTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListPoliciesInputListPoliciesPaginateTypeDef = TypedDict(
     "_OptionalListPoliciesInputListPoliciesPaginateTypeDef",
     {
         "filter": PolicyFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListPoliciesInputListPoliciesPaginateTypeDef(
     _RequiredListPoliciesInputListPoliciesPaginateTypeDef,
     _OptionalListPoliciesInputListPoliciesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListPoliciesInputRequestTypeDef = TypedDict(
     "_RequiredListPoliciesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListPoliciesInputRequestTypeDef = TypedDict(
@@ -1118,31 +1180,55 @@
         "nextToken": str,
         "maxResults": int,
         "filter": PolicyFilterTypeDef,
     },
     total=False,
 )
 
+
 class ListPoliciesInputRequestTypeDef(
     _RequiredListPoliciesInputRequestTypeDef, _OptionalListPoliciesInputRequestTypeDef
 ):
     pass
 
+
+_RequiredCreatePolicyInputRequestTypeDef = TypedDict(
+    "_RequiredCreatePolicyInputRequestTypeDef",
+    {
+        "policyStoreId": str,
+        "definition": PolicyDefinitionTypeDef,
+    },
+)
+_OptionalCreatePolicyInputRequestTypeDef = TypedDict(
+    "_OptionalCreatePolicyInputRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class CreatePolicyInputRequestTypeDef(
+    _RequiredCreatePolicyInputRequestTypeDef, _OptionalCreatePolicyInputRequestTypeDef
+):
+    pass
+
+
 GetPolicyOutputTypeDef = TypedDict(
     "GetPolicyOutputTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
         "policyType": PolicyTypeType,
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
+        "principal": EntityIdentifierOutputTypeDef,
+        "resource": EntityIdentifierOutputTypeDef,
         "definition": PolicyDefinitionDetailTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPolicyItemTypeDef = TypedDict(
     "_RequiredPolicyItemTypeDef",
     {
         "policyStoreId": str,
@@ -1152,44 +1238,26 @@
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
     },
 )
 _OptionalPolicyItemTypeDef = TypedDict(
     "_OptionalPolicyItemTypeDef",
     {
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
+        "principal": EntityIdentifierOutputTypeDef,
+        "resource": EntityIdentifierOutputTypeDef,
     },
     total=False,
 )
 
+
 class PolicyItemTypeDef(_RequiredPolicyItemTypeDef, _OptionalPolicyItemTypeDef):
     pass
 
-_RequiredCreatePolicyInputRequestTypeDef = TypedDict(
-    "_RequiredCreatePolicyInputRequestTypeDef",
-    {
-        "policyStoreId": str,
-        "definition": PolicyDefinitionTypeDef,
-    },
-)
-_OptionalCreatePolicyInputRequestTypeDef = TypedDict(
-    "_OptionalCreatePolicyInputRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class CreatePolicyInputRequestTypeDef(
-    _RequiredCreatePolicyInputRequestTypeDef, _OptionalCreatePolicyInputRequestTypeDef
-):
-    pass
 
 ListPoliciesOutputTypeDef = TypedDict(
     "ListPoliciesOutputTypeDef",
     {
         "nextToken": str,
         "policies": List[PolicyItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-verifiedpermissions
-Version: 1.28.0
-Summary: Type annotations for boto3.VerifiedPermissions 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.VerifiedPermissions 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-verifiedpermissions"></a>
 
 # mypy-boto3-verifiedpermissions
 
 [![PyPI - mypy-boto3-verifiedpermissions](https://img.shields.io/pypi/v/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-verifiedpermissions?color=blue)](https://pypistats.org/packages/mypy-boto3-verifiedpermissions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-verifiedpermissions)](https://pepy.tech/project/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
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
 [mypy-boto3-verifiedpermissions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,93 +343,95 @@
 
 ```python
 from mypy_boto3_verifiedpermissions.type_defs import (
     ActionIdentifierTypeDef,
     EntityIdentifierTypeDef,
     CognitoUserPoolConfigurationTypeDef,
     ContextDefinitionTypeDef,
-    CreateIdentitySourceOutputTypeDef,
+    ResponseMetadataTypeDef,
+    EntityIdentifierOutputTypeDef,
     ValidationSettingsTypeDef,
-    CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateInputRequestTypeDef,
-    CreatePolicyTemplateOutputTypeDef,
     DeleteIdentitySourceInputRequestTypeDef,
     DeletePolicyInputRequestTypeDef,
     DeletePolicyStoreInputRequestTypeDef,
     DeletePolicyTemplateInputRequestTypeDef,
     DeterminingPolicyItemTypeDef,
     EvaluationErrorItemTypeDef,
     GetIdentitySourceInputRequestTypeDef,
     IdentitySourceDetailsTypeDef,
     GetPolicyInputRequestTypeDef,
     GetPolicyStoreInputRequestTypeDef,
+    ValidationSettingsOutputTypeDef,
     GetPolicyTemplateInputRequestTypeDef,
-    GetPolicyTemplateOutputTypeDef,
     GetSchemaInputRequestTypeDef,
-    GetSchemaOutputTypeDef,
     IdentitySourceFilterTypeDef,
     IdentitySourceItemDetailsTypeDef,
-    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPolicyStoresInputRequestTypeDef,
     PolicyStoreItemTypeDef,
-    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyTemplatesInputRequestTypeDef,
     PolicyTemplateItemTypeDef,
-    PaginatorConfigTypeDef,
     StaticPolicyDefinitionDetailTypeDef,
     StaticPolicyDefinitionItemTypeDef,
     StaticPolicyDefinitionTypeDef,
     SchemaDefinitionTypeDef,
-    PutSchemaOutputTypeDef,
-    ResponseMetadataTypeDef,
     UpdateCognitoUserPoolConfigurationTypeDef,
-    UpdateIdentitySourceOutputTypeDef,
     UpdateStaticPolicyDefinitionTypeDef,
-    UpdatePolicyStoreOutputTypeDef,
     UpdatePolicyTemplateInputRequestTypeDef,
-    UpdatePolicyTemplateOutputTypeDef,
     AttributeValueTypeDef,
-    CreatePolicyOutputTypeDef,
     EntityItemTypeDef,
     EntityReferenceTypeDef,
+    TemplateLinkedPolicyDefinitionTypeDef,
+    ConfigurationTypeDef,
+    CreateIdentitySourceOutputTypeDef,
+    CreatePolicyStoreOutputTypeDef,
+    CreatePolicyTemplateOutputTypeDef,
+    GetPolicyTemplateOutputTypeDef,
+    GetSchemaOutputTypeDef,
+    PutSchemaOutputTypeDef,
+    UpdateIdentitySourceOutputTypeDef,
+    UpdatePolicyStoreOutputTypeDef,
+    UpdatePolicyTemplateOutputTypeDef,
+    CreatePolicyOutputTypeDef,
     TemplateLinkedPolicyDefinitionDetailTypeDef,
     TemplateLinkedPolicyDefinitionItemTypeDef,
-    TemplateLinkedPolicyDefinitionTypeDef,
     UpdatePolicyOutputTypeDef,
-    ConfigurationTypeDef,
     CreatePolicyStoreInputRequestTypeDef,
-    GetPolicyStoreOutputTypeDef,
     UpdatePolicyStoreInputRequestTypeDef,
     IsAuthorizedOutputTypeDef,
     IsAuthorizedWithTokenOutputTypeDef,
     GetIdentitySourceOutputTypeDef,
-    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    GetPolicyStoreOutputTypeDef,
     ListIdentitySourcesInputRequestTypeDef,
     IdentitySourceItemTypeDef,
+    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
+    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyStoresOutputTypeDef,
     ListPolicyTemplatesOutputTypeDef,
     PutSchemaInputRequestTypeDef,
     UpdateConfigurationTypeDef,
     UpdatePolicyDefinitionTypeDef,
     EntitiesDefinitionTypeDef,
     PolicyFilterTypeDef,
-    PolicyDefinitionDetailTypeDef,
-    PolicyDefinitionItemTypeDef,
     PolicyDefinitionTypeDef,
     CreateIdentitySourceInputRequestTypeDef,
+    PolicyDefinitionDetailTypeDef,
+    PolicyDefinitionItemTypeDef,
     ListIdentitySourcesOutputTypeDef,
     UpdateIdentitySourceInputRequestTypeDef,
     UpdatePolicyInputRequestTypeDef,
     IsAuthorizedInputRequestTypeDef,
     IsAuthorizedWithTokenInputRequestTypeDef,
     ListPoliciesInputListPoliciesPaginateTypeDef,
     ListPoliciesInputRequestTypeDef,
+    CreatePolicyInputRequestTypeDef,
     GetPolicyOutputTypeDef,
     PolicyItemTypeDef,
-    CreatePolicyInputRequestTypeDef,
     ListPoliciesOutputTypeDef,
 )
 
 
 def get_structure() -> ActionIdentifierTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt` & `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.0/setup.py` & `mypy-boto3-verifiedpermissions-1.28.12/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-verifiedpermissions",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_verifiedpermissions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VerifiedPermissions 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.VerifiedPermissions 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

