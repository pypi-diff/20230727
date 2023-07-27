# Comparing `tmp/mypy-boto3-cognito-identity-1.28.0.tar.gz` & `tmp/mypy-boto3-cognito-identity-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-identity-1.28.0.tar", last modified: Thu Jul  6 20:59:16 2023, max compression
+gzip compressed data, was "mypy-boto3-cognito-identity-1.28.12.tar", last modified: Thu Jul 27 05:34:29 2023, max compression
```

## Comparing `mypy-boto3-cognito-identity-1.28.0.tar` & `mypy-boto3-cognito-identity-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:16.306259 mypy-boto3-cognito-identity-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15130 2023-07-06 20:59:16.306259 mypy-boto3-cognito-identity-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:16.298259 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-07-06 20:36:20.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18275 2023-07-06 20:36:20.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:16.306259 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15130 2023-07-06 20:59:16.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 20:59:16.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:16.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:16.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:16.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 20:59:16.000000 mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:16.306259 mypy-boto3-cognito-identity-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-06 20:36:19.000000 mypy-boto3-cognito-identity-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.460549 mypy-boto3-cognito-identity-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-07-27 05:34:29.460549 mypy-boto3-cognito-identity-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.456549 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19571 2023-07-27 05:19:17.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19545 2023-07-27 05:19:17.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.456549 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-07-27 05:34:29.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:34:29.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:29.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:29.000000 mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:29.460549 mypy-boto3-cognito-identity-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-27 05:19:16.000000 mypy-boto3-cognito-identity-1.28.12/setup.py
```

### Comparing `mypy-boto3-cognito-identity-1.28.0/LICENSE` & `mypy-boto3-cognito-identity-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.0/PKG-INFO` & `mypy-boto3-cognito-identity-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-identity
-Version: 1.28.0
-Summary: Type annotations for boto3.CognitoIdentity 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CognitoIdentity 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cognito-identity"></a>
 
 # mypy-boto3-cognito-identity
 
 [![PyPI - mypy-boto3-cognito-identity](https://img.shields.io/pypi/v/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-identity?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-identity)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-identity)](https://pepy.tech/project/mypy-boto3-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentity 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[boto3.CognitoIdentity 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [mypy-boto3-cognito-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,14 +326,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_cognito_identity.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_identity.type_defs import (
+    CognitoIdentityProviderOutputTypeDef,
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
     UnprocessedIdentityIdTypeDef,
     DeleteIdentityPoolInputRequestTypeDef,
     DescribeIdentityInputRequestTypeDef,
     DescribeIdentityPoolInputRequestTypeDef,
@@ -354,40 +355,43 @@
     ListIdentitiesInputRequestTypeDef,
     ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     ListIdentityPoolsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityInputRequestTypeDef,
     LookupDeveloperIdentityResponseTypeDef,
+    MappingRuleOutputTypeDef,
     MappingRuleTypeDef,
     MergeDeveloperIdentitiesInputRequestTypeDef,
     MergeDeveloperIdentitiesResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     SetPrincipalTagAttributeMapInputRequestTypeDef,
     SetPrincipalTagAttributeMapResponseTypeDef,
     TagResourceInputRequestTypeDef,
     UnlinkDeveloperIdentityInputRequestTypeDef,
     UnlinkIdentityInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    IdentityPoolTypeDef,
     CreateIdentityPoolInputRequestTypeDef,
     IdentityPoolRequestTypeDef,
-    IdentityPoolTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
     DeleteIdentitiesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
+    RulesConfigurationTypeOutputTypeDef,
     RulesConfigurationTypeTypeDef,
+    RoleMappingOutputTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
-def get_structure() -> CognitoIdentityProviderTypeDef:
+def get_structure() -> CognitoIdentityProviderOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-identity-1.28.0/README.md` & `mypy-boto3-cognito-identity-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cognito-identity"></a>
 
 # mypy-boto3-cognito-identity
 
 [![PyPI - mypy-boto3-cognito-identity](https://img.shields.io/pypi/v/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-identity?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-identity)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-identity)](https://pepy.tech/project/mypy-boto3-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentity 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[boto3.CognitoIdentity 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [mypy-boto3-cognito-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -294,14 +294,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_cognito_identity.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_identity.type_defs import (
+    CognitoIdentityProviderOutputTypeDef,
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
     UnprocessedIdentityIdTypeDef,
     DeleteIdentityPoolInputRequestTypeDef,
     DescribeIdentityInputRequestTypeDef,
     DescribeIdentityPoolInputRequestTypeDef,
@@ -322,40 +323,43 @@
     ListIdentitiesInputRequestTypeDef,
     ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     ListIdentityPoolsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityInputRequestTypeDef,
     LookupDeveloperIdentityResponseTypeDef,
+    MappingRuleOutputTypeDef,
     MappingRuleTypeDef,
     MergeDeveloperIdentitiesInputRequestTypeDef,
     MergeDeveloperIdentitiesResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     SetPrincipalTagAttributeMapInputRequestTypeDef,
     SetPrincipalTagAttributeMapResponseTypeDef,
     TagResourceInputRequestTypeDef,
     UnlinkDeveloperIdentityInputRequestTypeDef,
     UnlinkIdentityInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    IdentityPoolTypeDef,
     CreateIdentityPoolInputRequestTypeDef,
     IdentityPoolRequestTypeDef,
-    IdentityPoolTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
     DeleteIdentitiesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
+    RulesConfigurationTypeOutputTypeDef,
     RulesConfigurationTypeTypeDef,
+    RoleMappingOutputTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
-def get_structure() -> CognitoIdentityProviderTypeDef:
+def get_structure() -> CognitoIdentityProviderOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/__init__.py` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/__init__.pyi` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/__main__.py` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoIdentity 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CognitoIdentity 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity\nOther"
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

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/client.py` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/client.pyi` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/literals.py` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,15 @@
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
@@ -240,26 +241,28 @@
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

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/literals.pyi` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/literals.pyi`

 * *Files 2% similar despite different names*

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

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/paginator.py` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/paginator.pyi` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/type_defs.py` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cognito-identity service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cognito_identity.type_defs import CognitoIdentityProviderTypeDef
+    from mypy_boto3_cognito_identity.type_defs import CognitoIdentityProviderOutputTypeDef
 
-    data: CognitoIdentityProviderTypeDef = {...}
+    data: CognitoIdentityProviderOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -23,16 +23,16 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "CognitoIdentityProviderOutputTypeDef",
     "CognitoIdentityProviderTypeDef",
     "CredentialsTypeDef",
     "DeleteIdentitiesInputRequestTypeDef",
     "UnprocessedIdentityIdTypeDef",
     "DeleteIdentityPoolInputRequestTypeDef",
     "DescribeIdentityInputRequestTypeDef",
     "DescribeIdentityPoolInputRequestTypeDef",
@@ -53,38 +53,51 @@
     "ListIdentitiesInputRequestTypeDef",
     "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     "ListIdentityPoolsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "LookupDeveloperIdentityInputRequestTypeDef",
     "LookupDeveloperIdentityResponseTypeDef",
+    "MappingRuleOutputTypeDef",
     "MappingRuleTypeDef",
     "MergeDeveloperIdentitiesInputRequestTypeDef",
     "MergeDeveloperIdentitiesResponseTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "SetPrincipalTagAttributeMapInputRequestTypeDef",
     "SetPrincipalTagAttributeMapResponseTypeDef",
     "TagResourceInputRequestTypeDef",
     "UnlinkDeveloperIdentityInputRequestTypeDef",
     "UnlinkIdentityInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "IdentityPoolTypeDef",
     "CreateIdentityPoolInputRequestTypeDef",
     "IdentityPoolRequestTypeDef",
-    "IdentityPoolTypeDef",
     "GetCredentialsForIdentityResponseTypeDef",
     "DeleteIdentitiesResponseTypeDef",
     "ListIdentitiesResponseTypeDef",
     "ListIdentityPoolsResponseTypeDef",
+    "RulesConfigurationTypeOutputTypeDef",
     "RulesConfigurationTypeTypeDef",
+    "RoleMappingOutputTypeDef",
     "RoleMappingTypeDef",
     "GetIdentityPoolRolesResponseTypeDef",
     "SetIdentityPoolRolesInputRequestTypeDef",
 )
 
+CognitoIdentityProviderOutputTypeDef = TypedDict(
+    "CognitoIdentityProviderOutputTypeDef",
+    {
+        "ProviderName": str,
+        "ClientId": str,
+        "ServerSideTokenCheck": bool,
+    },
+    total=False,
+)
+
 CognitoIdentityProviderTypeDef = TypedDict(
     "CognitoIdentityProviderTypeDef",
     {
         "ProviderName": str,
         "ClientId": str,
         "ServerSideTokenCheck": bool,
     },
@@ -157,22 +170,20 @@
     {
         "Logins": Mapping[str, str],
         "CustomRoleArn": str,
     },
     total=False,
 )
 
-
 class GetCredentialsForIdentityInputRequestTypeDef(
     _RequiredGetCredentialsForIdentityInputRequestTypeDef,
     _OptionalGetCredentialsForIdentityInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetIdInputRequestTypeDef = TypedDict(
     "_RequiredGetIdInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalGetIdInputRequestTypeDef = TypedDict(
@@ -180,21 +191,19 @@
     {
         "AccountId": str,
         "Logins": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetIdInputRequestTypeDef(
     _RequiredGetIdInputRequestTypeDef, _OptionalGetIdInputRequestTypeDef
 ):
     pass
 
-
 GetIdResponseTypeDef = TypedDict(
     "GetIdResponseTypeDef",
     {
         "IdentityId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -219,22 +228,20 @@
         "IdentityId": str,
         "PrincipalTags": Mapping[str, str],
         "TokenDuration": int,
     },
     total=False,
 )
 
-
 class GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef(
     _RequiredGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
     _OptionalGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
-
 GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
     "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
     {
         "IdentityId": str,
         "Token": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -250,21 +257,19 @@
     "_OptionalGetOpenIdTokenInputRequestTypeDef",
     {
         "Logins": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetOpenIdTokenInputRequestTypeDef(
     _RequiredGetOpenIdTokenInputRequestTypeDef, _OptionalGetOpenIdTokenInputRequestTypeDef
 ):
     pass
 
-
 GetOpenIdTokenResponseTypeDef = TypedDict(
     "GetOpenIdTokenResponseTypeDef",
     {
         "IdentityId": str,
         "Token": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -332,21 +337,19 @@
     {
         "NextToken": str,
         "HideDisabled": bool,
     },
     total=False,
 )
 
-
 class ListIdentitiesInputRequestTypeDef(
     _RequiredListIdentitiesInputRequestTypeDef, _OptionalListIdentitiesInputRequestTypeDef
 ):
     pass
 
-
 ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
     "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -361,21 +364,19 @@
     "_OptionalListIdentityPoolsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListIdentityPoolsInputRequestTypeDef(
     _RequiredListIdentityPoolsInputRequestTypeDef, _OptionalListIdentityPoolsInputRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -400,32 +401,40 @@
         "DeveloperUserIdentifier": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class LookupDeveloperIdentityInputRequestTypeDef(
     _RequiredLookupDeveloperIdentityInputRequestTypeDef,
     _OptionalLookupDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
-
 LookupDeveloperIdentityResponseTypeDef = TypedDict(
     "LookupDeveloperIdentityResponseTypeDef",
     {
         "IdentityId": str,
         "DeveloperUserIdentifierList": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MappingRuleOutputTypeDef = TypedDict(
+    "MappingRuleOutputTypeDef",
+    {
+        "Claim": str,
+        "MatchType": MappingRuleMatchTypeType,
+        "Value": str,
+        "RoleARN": str,
+    },
+)
+
 MappingRuleTypeDef = TypedDict(
     "MappingRuleTypeDef",
     {
         "Claim": str,
         "MatchType": MappingRuleMatchTypeType,
         "Value": str,
         "RoleARN": str,
@@ -483,22 +492,20 @@
     {
         "UseDefaults": bool,
         "PrincipalTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class SetPrincipalTagAttributeMapInputRequestTypeDef(
     _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef,
     _OptionalSetPrincipalTagAttributeMapInputRequestTypeDef,
 ):
     pass
 
-
 SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
     "SetPrincipalTagAttributeMapResponseTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
         "UseDefaults": bool,
         "PrincipalTags": Dict[str, str],
@@ -537,14 +544,31 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+IdentityPoolTypeDef = TypedDict(
+    "IdentityPoolTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityPoolName": str,
+        "AllowUnauthenticatedIdentities": bool,
+        "AllowClassicFlow": bool,
+        "SupportedLoginProviders": Dict[str, str],
+        "DeveloperProviderName": str,
+        "OpenIdConnectProviderARNs": List[str],
+        "CognitoIdentityProviders": List[CognitoIdentityProviderOutputTypeDef],
+        "SamlProviderARNs": List[str],
+        "IdentityPoolTags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateIdentityPoolInputRequestTypeDef = TypedDict(
     "_RequiredCreateIdentityPoolInputRequestTypeDef",
     {
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
     },
 )
@@ -558,21 +582,19 @@
         "CognitoIdentityProviders": Sequence[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": Sequence[str],
         "IdentityPoolTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateIdentityPoolInputRequestTypeDef(
     _RequiredCreateIdentityPoolInputRequestTypeDef, _OptionalCreateIdentityPoolInputRequestTypeDef
 ):
     pass
 
-
 _RequiredIdentityPoolRequestTypeDef = TypedDict(
     "_RequiredIdentityPoolRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
     },
@@ -587,38 +609,19 @@
         "CognitoIdentityProviders": Sequence[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": Sequence[str],
         "IdentityPoolTags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class IdentityPoolRequestTypeDef(
     _RequiredIdentityPoolRequestTypeDef, _OptionalIdentityPoolRequestTypeDef
 ):
     pass
 
-
-IdentityPoolTypeDef = TypedDict(
-    "IdentityPoolTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityPoolName": str,
-        "AllowUnauthenticatedIdentities": bool,
-        "AllowClassicFlow": bool,
-        "SupportedLoginProviders": Dict[str, str],
-        "DeveloperProviderName": str,
-        "OpenIdConnectProviderARNs": List[str],
-        "CognitoIdentityProviders": List[CognitoIdentityProviderTypeDef],
-        "SamlProviderARNs": List[str],
-        "IdentityPoolTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCredentialsForIdentityResponseTypeDef = TypedDict(
     "GetCredentialsForIdentityResponseTypeDef",
     {
         "IdentityId": str,
         "Credentials": CredentialsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -647,21 +650,48 @@
     {
         "IdentityPools": List[IdentityPoolShortDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RulesConfigurationTypeOutputTypeDef = TypedDict(
+    "RulesConfigurationTypeOutputTypeDef",
+    {
+        "Rules": List[MappingRuleOutputTypeDef],
+    },
+)
+
 RulesConfigurationTypeTypeDef = TypedDict(
     "RulesConfigurationTypeTypeDef",
     {
-        "Rules": List[MappingRuleTypeDef],
+        "Rules": Sequence[MappingRuleTypeDef],
+    },
+)
+
+_RequiredRoleMappingOutputTypeDef = TypedDict(
+    "_RequiredRoleMappingOutputTypeDef",
+    {
+        "Type": RoleMappingTypeType,
+    },
+)
+_OptionalRoleMappingOutputTypeDef = TypedDict(
+    "_OptionalRoleMappingOutputTypeDef",
+    {
+        "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
+        "RulesConfiguration": RulesConfigurationTypeOutputTypeDef,
     },
+    total=False,
 )
 
+class RoleMappingOutputTypeDef(
+    _RequiredRoleMappingOutputTypeDef, _OptionalRoleMappingOutputTypeDef
+):
+    pass
+
 _RequiredRoleMappingTypeDef = TypedDict(
     "_RequiredRoleMappingTypeDef",
     {
         "Type": RoleMappingTypeType,
     },
 )
 _OptionalRoleMappingTypeDef = TypedDict(
@@ -669,25 +699,23 @@
     {
         "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
         "RulesConfiguration": RulesConfigurationTypeTypeDef,
     },
     total=False,
 )
 
-
 class RoleMappingTypeDef(_RequiredRoleMappingTypeDef, _OptionalRoleMappingTypeDef):
     pass
 
-
 GetIdentityPoolRolesResponseTypeDef = TypedDict(
     "GetIdentityPoolRolesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Dict[str, str],
-        "RoleMappings": Dict[str, RoleMappingTypeDef],
+        "RoleMappings": Dict[str, RoleMappingOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolRolesInputRequestTypeDef",
     {
@@ -699,13 +727,12 @@
     "_OptionalSetIdentityPoolRolesInputRequestTypeDef",
     {
         "RoleMappings": Mapping[str, RoleMappingTypeDef],
     },
     total=False,
 )
 
-
 class SetIdentityPoolRolesInputRequestTypeDef(
     _RequiredSetIdentityPoolRolesInputRequestTypeDef,
     _OptionalSetIdentityPoolRolesInputRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity/type_defs.pyi` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cognito-identity service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cognito_identity.type_defs import CognitoIdentityProviderTypeDef
+    from mypy_boto3_cognito_identity.type_defs import CognitoIdentityProviderOutputTypeDef
 
-    data: CognitoIdentityProviderTypeDef = {...}
+    data: CognitoIdentityProviderOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -23,15 +23,17 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "CognitoIdentityProviderOutputTypeDef",
     "CognitoIdentityProviderTypeDef",
     "CredentialsTypeDef",
     "DeleteIdentitiesInputRequestTypeDef",
     "UnprocessedIdentityIdTypeDef",
     "DeleteIdentityPoolInputRequestTypeDef",
     "DescribeIdentityInputRequestTypeDef",
     "DescribeIdentityPoolInputRequestTypeDef",
@@ -52,38 +54,51 @@
     "ListIdentitiesInputRequestTypeDef",
     "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     "ListIdentityPoolsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "LookupDeveloperIdentityInputRequestTypeDef",
     "LookupDeveloperIdentityResponseTypeDef",
+    "MappingRuleOutputTypeDef",
     "MappingRuleTypeDef",
     "MergeDeveloperIdentitiesInputRequestTypeDef",
     "MergeDeveloperIdentitiesResponseTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "SetPrincipalTagAttributeMapInputRequestTypeDef",
     "SetPrincipalTagAttributeMapResponseTypeDef",
     "TagResourceInputRequestTypeDef",
     "UnlinkDeveloperIdentityInputRequestTypeDef",
     "UnlinkIdentityInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "IdentityPoolTypeDef",
     "CreateIdentityPoolInputRequestTypeDef",
     "IdentityPoolRequestTypeDef",
-    "IdentityPoolTypeDef",
     "GetCredentialsForIdentityResponseTypeDef",
     "DeleteIdentitiesResponseTypeDef",
     "ListIdentitiesResponseTypeDef",
     "ListIdentityPoolsResponseTypeDef",
+    "RulesConfigurationTypeOutputTypeDef",
     "RulesConfigurationTypeTypeDef",
+    "RoleMappingOutputTypeDef",
     "RoleMappingTypeDef",
     "GetIdentityPoolRolesResponseTypeDef",
     "SetIdentityPoolRolesInputRequestTypeDef",
 )
 
+CognitoIdentityProviderOutputTypeDef = TypedDict(
+    "CognitoIdentityProviderOutputTypeDef",
+    {
+        "ProviderName": str,
+        "ClientId": str,
+        "ServerSideTokenCheck": bool,
+    },
+    total=False,
+)
+
 CognitoIdentityProviderTypeDef = TypedDict(
     "CognitoIdentityProviderTypeDef",
     {
         "ProviderName": str,
         "ClientId": str,
         "ServerSideTokenCheck": bool,
     },
@@ -156,20 +171,22 @@
     {
         "Logins": Mapping[str, str],
         "CustomRoleArn": str,
     },
     total=False,
 )
 
+
 class GetCredentialsForIdentityInputRequestTypeDef(
     _RequiredGetCredentialsForIdentityInputRequestTypeDef,
     _OptionalGetCredentialsForIdentityInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetIdInputRequestTypeDef = TypedDict(
     "_RequiredGetIdInputRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 _OptionalGetIdInputRequestTypeDef = TypedDict(
@@ -177,19 +194,21 @@
     {
         "AccountId": str,
         "Logins": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetIdInputRequestTypeDef(
     _RequiredGetIdInputRequestTypeDef, _OptionalGetIdInputRequestTypeDef
 ):
     pass
 
+
 GetIdResponseTypeDef = TypedDict(
     "GetIdResponseTypeDef",
     {
         "IdentityId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -214,20 +233,22 @@
         "IdentityId": str,
         "PrincipalTags": Mapping[str, str],
         "TokenDuration": int,
     },
     total=False,
 )
 
+
 class GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef(
     _RequiredGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
     _OptionalGetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
+
 GetOpenIdTokenForDeveloperIdentityResponseTypeDef = TypedDict(
     "GetOpenIdTokenForDeveloperIdentityResponseTypeDef",
     {
         "IdentityId": str,
         "Token": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -243,19 +264,21 @@
     "_OptionalGetOpenIdTokenInputRequestTypeDef",
     {
         "Logins": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetOpenIdTokenInputRequestTypeDef(
     _RequiredGetOpenIdTokenInputRequestTypeDef, _OptionalGetOpenIdTokenInputRequestTypeDef
 ):
     pass
 
+
 GetOpenIdTokenResponseTypeDef = TypedDict(
     "GetOpenIdTokenResponseTypeDef",
     {
         "IdentityId": str,
         "Token": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -323,19 +346,21 @@
     {
         "NextToken": str,
         "HideDisabled": bool,
     },
     total=False,
 )
 
+
 class ListIdentitiesInputRequestTypeDef(
     _RequiredListIdentitiesInputRequestTypeDef, _OptionalListIdentitiesInputRequestTypeDef
 ):
     pass
 
+
 ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = TypedDict(
     "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -350,19 +375,21 @@
     "_OptionalListIdentityPoolsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListIdentityPoolsInputRequestTypeDef(
     _RequiredListIdentityPoolsInputRequestTypeDef, _OptionalListIdentityPoolsInputRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -387,30 +414,42 @@
         "DeveloperUserIdentifier": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class LookupDeveloperIdentityInputRequestTypeDef(
     _RequiredLookupDeveloperIdentityInputRequestTypeDef,
     _OptionalLookupDeveloperIdentityInputRequestTypeDef,
 ):
     pass
 
+
 LookupDeveloperIdentityResponseTypeDef = TypedDict(
     "LookupDeveloperIdentityResponseTypeDef",
     {
         "IdentityId": str,
         "DeveloperUserIdentifierList": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MappingRuleOutputTypeDef = TypedDict(
+    "MappingRuleOutputTypeDef",
+    {
+        "Claim": str,
+        "MatchType": MappingRuleMatchTypeType,
+        "Value": str,
+        "RoleARN": str,
+    },
+)
+
 MappingRuleTypeDef = TypedDict(
     "MappingRuleTypeDef",
     {
         "Claim": str,
         "MatchType": MappingRuleMatchTypeType,
         "Value": str,
         "RoleARN": str,
@@ -468,20 +507,22 @@
     {
         "UseDefaults": bool,
         "PrincipalTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class SetPrincipalTagAttributeMapInputRequestTypeDef(
     _RequiredSetPrincipalTagAttributeMapInputRequestTypeDef,
     _OptionalSetPrincipalTagAttributeMapInputRequestTypeDef,
 ):
     pass
 
+
 SetPrincipalTagAttributeMapResponseTypeDef = TypedDict(
     "SetPrincipalTagAttributeMapResponseTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityProviderName": str,
         "UseDefaults": bool,
         "PrincipalTags": Dict[str, str],
@@ -520,14 +561,31 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+IdentityPoolTypeDef = TypedDict(
+    "IdentityPoolTypeDef",
+    {
+        "IdentityPoolId": str,
+        "IdentityPoolName": str,
+        "AllowUnauthenticatedIdentities": bool,
+        "AllowClassicFlow": bool,
+        "SupportedLoginProviders": Dict[str, str],
+        "DeveloperProviderName": str,
+        "OpenIdConnectProviderARNs": List[str],
+        "CognitoIdentityProviders": List[CognitoIdentityProviderOutputTypeDef],
+        "SamlProviderARNs": List[str],
+        "IdentityPoolTags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateIdentityPoolInputRequestTypeDef = TypedDict(
     "_RequiredCreateIdentityPoolInputRequestTypeDef",
     {
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
     },
 )
@@ -541,19 +599,21 @@
         "CognitoIdentityProviders": Sequence[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": Sequence[str],
         "IdentityPoolTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateIdentityPoolInputRequestTypeDef(
     _RequiredCreateIdentityPoolInputRequestTypeDef, _OptionalCreateIdentityPoolInputRequestTypeDef
 ):
     pass
 
+
 _RequiredIdentityPoolRequestTypeDef = TypedDict(
     "_RequiredIdentityPoolRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityPoolName": str,
         "AllowUnauthenticatedIdentities": bool,
     },
@@ -568,35 +628,20 @@
         "CognitoIdentityProviders": Sequence[CognitoIdentityProviderTypeDef],
         "SamlProviderARNs": Sequence[str],
         "IdentityPoolTags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class IdentityPoolRequestTypeDef(
     _RequiredIdentityPoolRequestTypeDef, _OptionalIdentityPoolRequestTypeDef
 ):
     pass
 
-IdentityPoolTypeDef = TypedDict(
-    "IdentityPoolTypeDef",
-    {
-        "IdentityPoolId": str,
-        "IdentityPoolName": str,
-        "AllowUnauthenticatedIdentities": bool,
-        "AllowClassicFlow": bool,
-        "SupportedLoginProviders": Dict[str, str],
-        "DeveloperProviderName": str,
-        "OpenIdConnectProviderARNs": List[str],
-        "CognitoIdentityProviders": List[CognitoIdentityProviderTypeDef],
-        "SamlProviderARNs": List[str],
-        "IdentityPoolTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetCredentialsForIdentityResponseTypeDef = TypedDict(
     "GetCredentialsForIdentityResponseTypeDef",
     {
         "IdentityId": str,
         "Credentials": CredentialsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -626,21 +671,50 @@
     {
         "IdentityPools": List[IdentityPoolShortDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RulesConfigurationTypeOutputTypeDef = TypedDict(
+    "RulesConfigurationTypeOutputTypeDef",
+    {
+        "Rules": List[MappingRuleOutputTypeDef],
+    },
+)
+
 RulesConfigurationTypeTypeDef = TypedDict(
     "RulesConfigurationTypeTypeDef",
     {
-        "Rules": List[MappingRuleTypeDef],
+        "Rules": Sequence[MappingRuleTypeDef],
+    },
+)
+
+_RequiredRoleMappingOutputTypeDef = TypedDict(
+    "_RequiredRoleMappingOutputTypeDef",
+    {
+        "Type": RoleMappingTypeType,
+    },
+)
+_OptionalRoleMappingOutputTypeDef = TypedDict(
+    "_OptionalRoleMappingOutputTypeDef",
+    {
+        "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
+        "RulesConfiguration": RulesConfigurationTypeOutputTypeDef,
     },
+    total=False,
 )
 
+
+class RoleMappingOutputTypeDef(
+    _RequiredRoleMappingOutputTypeDef, _OptionalRoleMappingOutputTypeDef
+):
+    pass
+
+
 _RequiredRoleMappingTypeDef = TypedDict(
     "_RequiredRoleMappingTypeDef",
     {
         "Type": RoleMappingTypeType,
     },
 )
 _OptionalRoleMappingTypeDef = TypedDict(
@@ -648,23 +722,25 @@
     {
         "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
         "RulesConfiguration": RulesConfigurationTypeTypeDef,
     },
     total=False,
 )
 
+
 class RoleMappingTypeDef(_RequiredRoleMappingTypeDef, _OptionalRoleMappingTypeDef):
     pass
 
+
 GetIdentityPoolRolesResponseTypeDef = TypedDict(
     "GetIdentityPoolRolesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Dict[str, str],
-        "RoleMappings": Dict[str, RoleMappingTypeDef],
+        "RoleMappings": Dict[str, RoleMappingOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolRolesInputRequestTypeDef",
     {
@@ -676,12 +752,13 @@
     "_OptionalSetIdentityPoolRolesInputRequestTypeDef",
     {
         "RoleMappings": Mapping[str, RoleMappingTypeDef],
     },
     total=False,
 )
 
+
 class SetIdentityPoolRolesInputRequestTypeDef(
     _RequiredSetIdentityPoolRolesInputRequestTypeDef,
     _OptionalSetIdentityPoolRolesInputRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity.egg-info/PKG-INFO` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-identity
-Version: 1.28.0
-Summary: Type annotations for boto3.CognitoIdentity 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CognitoIdentity 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cognito-identity"></a>
 
 # mypy-boto3-cognito-identity
 
 [![PyPI - mypy-boto3-cognito-identity](https://img.shields.io/pypi/v/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-identity?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-identity)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-identity)](https://pepy.tech/project/mypy-boto3-cognito-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentity 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
+[boto3.CognitoIdentity 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
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
 [mypy-boto3-cognito-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,14 +326,15 @@
 ### Typed dictionaries
 
 `mypy_boto3_cognito_identity.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_identity.type_defs import (
+    CognitoIdentityProviderOutputTypeDef,
     CognitoIdentityProviderTypeDef,
     CredentialsTypeDef,
     DeleteIdentitiesInputRequestTypeDef,
     UnprocessedIdentityIdTypeDef,
     DeleteIdentityPoolInputRequestTypeDef,
     DescribeIdentityInputRequestTypeDef,
     DescribeIdentityPoolInputRequestTypeDef,
@@ -354,40 +355,43 @@
     ListIdentitiesInputRequestTypeDef,
     ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
     ListIdentityPoolsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityInputRequestTypeDef,
     LookupDeveloperIdentityResponseTypeDef,
+    MappingRuleOutputTypeDef,
     MappingRuleTypeDef,
     MergeDeveloperIdentitiesInputRequestTypeDef,
     MergeDeveloperIdentitiesResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     SetPrincipalTagAttributeMapInputRequestTypeDef,
     SetPrincipalTagAttributeMapResponseTypeDef,
     TagResourceInputRequestTypeDef,
     UnlinkDeveloperIdentityInputRequestTypeDef,
     UnlinkIdentityInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    IdentityPoolTypeDef,
     CreateIdentityPoolInputRequestTypeDef,
     IdentityPoolRequestTypeDef,
-    IdentityPoolTypeDef,
     GetCredentialsForIdentityResponseTypeDef,
     DeleteIdentitiesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
+    RulesConfigurationTypeOutputTypeDef,
     RulesConfigurationTypeTypeDef,
+    RoleMappingOutputTypeDef,
     RoleMappingTypeDef,
     GetIdentityPoolRolesResponseTypeDef,
     SetIdentityPoolRolesInputRequestTypeDef,
 )
 
 
-def get_structure() -> CognitoIdentityProviderTypeDef:
+def get_structure() -> CognitoIdentityProviderOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cognito-identity-1.28.0/mypy_boto3_cognito_identity.egg-info/SOURCES.txt` & `mypy-boto3-cognito-identity-1.28.12/mypy_boto3_cognito_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-identity-1.28.0/setup.py` & `mypy-boto3-cognito-identity-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-identity",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cognito_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CognitoIdentity 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CognitoIdentity 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

