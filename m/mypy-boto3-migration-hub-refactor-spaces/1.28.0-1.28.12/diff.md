# Comparing `tmp/mypy-boto3-migration-hub-refactor-spaces-1.28.0.tar.gz` & `tmp/mypy-boto3-migration-hub-refactor-spaces-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migration-hub-refactor-spaces-1.28.0.tar", last modified: Thu Jul  6 21:00:09 2023, max compression
+gzip compressed data, was "mypy-boto3-migration-hub-refactor-spaces-1.28.12.tar", last modified: Thu Jul 27 05:35:03 2023, max compression
```

## Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0.tar` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:09.118373 mypy-boto3-migration-hub-refactor-spaces-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-07-06 21:00:09.118373 mypy-boto3-migration-hub-refactor-spaces-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:09.118373 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28408 2023-07-06 20:47:46.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-07-06 20:47:46.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:45.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:09.118373 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-07-06 21:00:08.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-06 21:00:08.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:08.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:08.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:08.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 21:00:08.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:09.118373 mypy-boto3-migration-hub-refactor-spaces-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-06 20:47:44.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.180433 mypy-boto3-migration-hub-refactor-spaces-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-07-27 05:35:03.172433 mypy-boto3-migration-hub-refactor-spaces-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.168433 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29910 2023-07-27 05:26:40.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-07-27 05:26:40.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.172433 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-07-27 05:35:03.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-27 05:35:03.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:03.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 05:35:03.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:03.180433 mypy-boto3-migration-hub-refactor-spaces-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/setup.py
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/LICENSE` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/PKG-INFO` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migration-hub-refactor-spaces
-Version: 1.28.0
-Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-migration-hub-refactor-spaces"></a>
 
 # mypy-boto3-migration-hub-refactor-spaces
 
 [![PyPI - mypy-boto3-migration-hub-refactor-spaces](https://img.shields.io/pypi/v/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migration-hub-refactor-spaces?color=blue)](https://pypistats.org/packages/mypy-boto3-migration-hub-refactor-spaces)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migration-hub-refactor-spaces)](https://pepy.tech/project/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,23 +349,27 @@
 
 `mypy_boto3_migration_hub_refactor_spaces.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migration_hub_refactor_spaces.type_defs import (
     ApiGatewayProxyConfigTypeDef,
+    ApiGatewayProxyInputOutputTypeDef,
     ApiGatewayProxyInputTypeDef,
     ApiGatewayProxySummaryTypeDef,
     ErrorResponseTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentResponseTypeDef,
     DefaultRouteInputTypeDef,
     UriPathRouteInputTypeDef,
+    UriPathRouteInputOutputTypeDef,
     LambdaEndpointInputTypeDef,
     UrlEndpointInputTypeDef,
+    LambdaEndpointInputOutputTypeDef,
+    UrlEndpointInputOutputTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteApplicationResponseTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteEnvironmentResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseTypeDef,
@@ -397,16 +401,16 @@
     PutResourcePolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UrlEndpointSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRouteRequestRequestTypeDef,
     UpdateRouteResponseTypeDef,
-    CreateApplicationRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
+    CreateApplicationRequestRequestTypeDef,
     ApplicationSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     GetApplicationResponseTypeDef,
     GetEnvironmentResponseTypeDef,
     GetRouteResponseTypeDef,
     RouteSummaryTypeDef,
     CreateRouteRequestRequestTypeDef,
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/README.md` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-migration-hub-refactor-spaces"></a>
 
 # mypy-boto3-migration-hub-refactor-spaces
 
 [![PyPI - mypy-boto3-migration-hub-refactor-spaces](https://img.shields.io/pypi/v/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migration-hub-refactor-spaces?color=blue)](https://pypistats.org/packages/mypy-boto3-migration-hub-refactor-spaces)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migration-hub-refactor-spaces)](https://pepy.tech/project/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,23 +317,27 @@
 
 `mypy_boto3_migration_hub_refactor_spaces.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migration_hub_refactor_spaces.type_defs import (
     ApiGatewayProxyConfigTypeDef,
+    ApiGatewayProxyInputOutputTypeDef,
     ApiGatewayProxyInputTypeDef,
     ApiGatewayProxySummaryTypeDef,
     ErrorResponseTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentResponseTypeDef,
     DefaultRouteInputTypeDef,
     UriPathRouteInputTypeDef,
+    UriPathRouteInputOutputTypeDef,
     LambdaEndpointInputTypeDef,
     UrlEndpointInputTypeDef,
+    LambdaEndpointInputOutputTypeDef,
+    UrlEndpointInputOutputTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteApplicationResponseTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteEnvironmentResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseTypeDef,
@@ -365,16 +369,16 @@
     PutResourcePolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UrlEndpointSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRouteRequestRequestTypeDef,
     UpdateRouteResponseTypeDef,
-    CreateApplicationRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
+    CreateApplicationRequestRequestTypeDef,
     ApplicationSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     GetApplicationResponseTypeDef,
     GetEnvironmentResponseTypeDef,
     GetRouteResponseTypeDef,
     RouteSummaryTypeDef,
     CreateRouteRequestRequestTypeDef,
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/__init__.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/__main__.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces\nOther"
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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/client.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/client.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/literals.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,15 @@
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
@@ -298,26 +299,28 @@
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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/literals.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,15 @@
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
@@ -296,26 +297,28 @@
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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/paginator.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/type_defs.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,27 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApiGatewayProxyConfigTypeDef",
+    "ApiGatewayProxyInputOutputTypeDef",
     "ApiGatewayProxyInputTypeDef",
     "ApiGatewayProxySummaryTypeDef",
     "ErrorResponseTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentResponseTypeDef",
     "DefaultRouteInputTypeDef",
     "UriPathRouteInputTypeDef",
+    "UriPathRouteInputOutputTypeDef",
     "LambdaEndpointInputTypeDef",
     "UrlEndpointInputTypeDef",
+    "LambdaEndpointInputOutputTypeDef",
+    "UrlEndpointInputOutputTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteApplicationResponseTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteEnvironmentResponseTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
     "DeleteRouteResponseTypeDef",
@@ -86,16 +90,16 @@
     "PutResourcePolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UrlEndpointSummaryTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRouteRequestRequestTypeDef",
     "UpdateRouteResponseTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
     "ApplicationSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "GetApplicationResponseTypeDef",
     "GetEnvironmentResponseTypeDef",
     "GetRouteResponseTypeDef",
     "RouteSummaryTypeDef",
     "CreateRouteRequestRequestTypeDef",
@@ -121,14 +125,23 @@
         "ProxyUrl": str,
         "StageName": str,
         "VpcLinkId": str,
     },
     total=False,
 )
 
+ApiGatewayProxyInputOutputTypeDef = TypedDict(
+    "ApiGatewayProxyInputOutputTypeDef",
+    {
+        "EndpointType": ApiGatewayEndpointTypeType,
+        "StageName": str,
+    },
+    total=False,
+)
+
 ApiGatewayProxyInputTypeDef = TypedDict(
     "ApiGatewayProxyInputTypeDef",
     {
         "EndpointType": ApiGatewayEndpointTypeType,
         "StageName": str,
     },
     total=False,
@@ -230,14 +243,38 @@
 
 class UriPathRouteInputTypeDef(
     _RequiredUriPathRouteInputTypeDef, _OptionalUriPathRouteInputTypeDef
 ):
     pass
 
 
+_RequiredUriPathRouteInputOutputTypeDef = TypedDict(
+    "_RequiredUriPathRouteInputOutputTypeDef",
+    {
+        "ActivationState": RouteActivationStateType,
+        "SourcePath": str,
+    },
+)
+_OptionalUriPathRouteInputOutputTypeDef = TypedDict(
+    "_OptionalUriPathRouteInputOutputTypeDef",
+    {
+        "AppendSourcePath": bool,
+        "IncludeChildPaths": bool,
+        "Methods": List[HttpMethodType],
+    },
+    total=False,
+)
+
+
+class UriPathRouteInputOutputTypeDef(
+    _RequiredUriPathRouteInputOutputTypeDef, _OptionalUriPathRouteInputOutputTypeDef
+):
+    pass
+
+
 LambdaEndpointInputTypeDef = TypedDict(
     "LambdaEndpointInputTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -256,14 +293,42 @@
 )
 
 
 class UrlEndpointInputTypeDef(_RequiredUrlEndpointInputTypeDef, _OptionalUrlEndpointInputTypeDef):
     pass
 
 
+LambdaEndpointInputOutputTypeDef = TypedDict(
+    "LambdaEndpointInputOutputTypeDef",
+    {
+        "Arn": str,
+    },
+)
+
+_RequiredUrlEndpointInputOutputTypeDef = TypedDict(
+    "_RequiredUrlEndpointInputOutputTypeDef",
+    {
+        "Url": str,
+    },
+)
+_OptionalUrlEndpointInputOutputTypeDef = TypedDict(
+    "_OptionalUrlEndpointInputOutputTypeDef",
+    {
+        "HealthUrl": str,
+    },
+    total=False,
+)
+
+
+class UrlEndpointInputOutputTypeDef(
+    _RequiredUrlEndpointInputOutputTypeDef, _OptionalUrlEndpointInputOutputTypeDef
+):
+    pass
+
+
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
@@ -725,14 +790,34 @@
         "RouteId": str,
         "ServiceId": str,
         "State": RouteStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "ApiGatewayProxy": ApiGatewayProxyInputOutputTypeDef,
+        "ApplicationId": str,
+        "Arn": str,
+        "CreatedByAccountId": str,
+        "CreatedTime": datetime,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "OwnerAccountId": str,
+        "ProxyType": Literal["API_GATEWAY"],
+        "State": ApplicationStateType,
+        "Tags": Dict[str, str],
+        "VpcId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
         "Name": str,
         "ProxyType": Literal["API_GATEWAY"],
         "VpcId": str,
@@ -751,34 +836,14 @@
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "ApiGatewayProxy": ApiGatewayProxyInputTypeDef,
-        "ApplicationId": str,
-        "Arn": str,
-        "CreatedByAccountId": str,
-        "CreatedTime": datetime,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "OwnerAccountId": str,
-        "ProxyType": Literal["API_GATEWAY"],
-        "State": ApplicationStateType,
-        "Tags": Dict[str, str],
-        "VpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ApplicationSummaryTypeDef = TypedDict(
     "ApplicationSummaryTypeDef",
     {
         "ApiGatewayProxy": ApiGatewayProxySummaryTypeDef,
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
@@ -942,15 +1007,15 @@
         "LastUpdatedTime": datetime,
         "OwnerAccountId": str,
         "RouteId": str,
         "RouteType": RouteTypeType,
         "ServiceId": str,
         "State": RouteStateType,
         "Tags": Dict[str, str],
-        "UriPathRoute": UriPathRouteInputTypeDef,
+        "UriPathRoute": UriPathRouteInputOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
@@ -986,22 +1051,22 @@
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
         "Description": str,
         "EndpointType": ServiceEndpointTypeType,
         "EnvironmentId": str,
-        "LambdaEndpoint": LambdaEndpointInputTypeDef,
+        "LambdaEndpoint": LambdaEndpointInputOutputTypeDef,
         "LastUpdatedTime": datetime,
         "Name": str,
         "OwnerAccountId": str,
         "ServiceId": str,
         "State": ServiceStateType,
         "Tags": Dict[str, str],
-        "UrlEndpoint": UrlEndpointInputTypeDef,
+        "UrlEndpoint": UrlEndpointInputOutputTypeDef,
         "VpcId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentVpcsResponseTypeDef = TypedDict(
     "ListEnvironmentVpcsResponseTypeDef",
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,23 +37,27 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApiGatewayProxyConfigTypeDef",
+    "ApiGatewayProxyInputOutputTypeDef",
     "ApiGatewayProxyInputTypeDef",
     "ApiGatewayProxySummaryTypeDef",
     "ErrorResponseTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentResponseTypeDef",
     "DefaultRouteInputTypeDef",
     "UriPathRouteInputTypeDef",
+    "UriPathRouteInputOutputTypeDef",
     "LambdaEndpointInputTypeDef",
     "UrlEndpointInputTypeDef",
+    "LambdaEndpointInputOutputTypeDef",
+    "UrlEndpointInputOutputTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteApplicationResponseTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteEnvironmentResponseTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
     "DeleteRouteResponseTypeDef",
@@ -85,16 +89,16 @@
     "PutResourcePolicyRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UrlEndpointSummaryTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRouteRequestRequestTypeDef",
     "UpdateRouteResponseTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
     "ApplicationSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "GetApplicationResponseTypeDef",
     "GetEnvironmentResponseTypeDef",
     "GetRouteResponseTypeDef",
     "RouteSummaryTypeDef",
     "CreateRouteRequestRequestTypeDef",
@@ -120,14 +124,23 @@
         "ProxyUrl": str,
         "StageName": str,
         "VpcLinkId": str,
     },
     total=False,
 )
 
+ApiGatewayProxyInputOutputTypeDef = TypedDict(
+    "ApiGatewayProxyInputOutputTypeDef",
+    {
+        "EndpointType": ApiGatewayEndpointTypeType,
+        "StageName": str,
+    },
+    total=False,
+)
+
 ApiGatewayProxyInputTypeDef = TypedDict(
     "ApiGatewayProxyInputTypeDef",
     {
         "EndpointType": ApiGatewayEndpointTypeType,
         "StageName": str,
     },
     total=False,
@@ -225,14 +238,36 @@
 )
 
 class UriPathRouteInputTypeDef(
     _RequiredUriPathRouteInputTypeDef, _OptionalUriPathRouteInputTypeDef
 ):
     pass
 
+_RequiredUriPathRouteInputOutputTypeDef = TypedDict(
+    "_RequiredUriPathRouteInputOutputTypeDef",
+    {
+        "ActivationState": RouteActivationStateType,
+        "SourcePath": str,
+    },
+)
+_OptionalUriPathRouteInputOutputTypeDef = TypedDict(
+    "_OptionalUriPathRouteInputOutputTypeDef",
+    {
+        "AppendSourcePath": bool,
+        "IncludeChildPaths": bool,
+        "Methods": List[HttpMethodType],
+    },
+    total=False,
+)
+
+class UriPathRouteInputOutputTypeDef(
+    _RequiredUriPathRouteInputOutputTypeDef, _OptionalUriPathRouteInputOutputTypeDef
+):
+    pass
+
 LambdaEndpointInputTypeDef = TypedDict(
     "LambdaEndpointInputTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -249,14 +284,40 @@
     },
     total=False,
 )
 
 class UrlEndpointInputTypeDef(_RequiredUrlEndpointInputTypeDef, _OptionalUrlEndpointInputTypeDef):
     pass
 
+LambdaEndpointInputOutputTypeDef = TypedDict(
+    "LambdaEndpointInputOutputTypeDef",
+    {
+        "Arn": str,
+    },
+)
+
+_RequiredUrlEndpointInputOutputTypeDef = TypedDict(
+    "_RequiredUrlEndpointInputOutputTypeDef",
+    {
+        "Url": str,
+    },
+)
+_OptionalUrlEndpointInputOutputTypeDef = TypedDict(
+    "_OptionalUrlEndpointInputOutputTypeDef",
+    {
+        "HealthUrl": str,
+    },
+    total=False,
+)
+
+class UrlEndpointInputOutputTypeDef(
+    _RequiredUrlEndpointInputOutputTypeDef, _OptionalUrlEndpointInputOutputTypeDef
+):
+    pass
+
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
@@ -702,14 +763,34 @@
         "RouteId": str,
         "ServiceId": str,
         "State": RouteStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "ApiGatewayProxy": ApiGatewayProxyInputOutputTypeDef,
+        "ApplicationId": str,
+        "Arn": str,
+        "CreatedByAccountId": str,
+        "CreatedTime": datetime,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "OwnerAccountId": str,
+        "ProxyType": Literal["API_GATEWAY"],
+        "State": ApplicationStateType,
+        "Tags": Dict[str, str],
+        "VpcId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
         "Name": str,
         "ProxyType": Literal["API_GATEWAY"],
         "VpcId": str,
@@ -726,34 +807,14 @@
 )
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "ApiGatewayProxy": ApiGatewayProxyInputTypeDef,
-        "ApplicationId": str,
-        "Arn": str,
-        "CreatedByAccountId": str,
-        "CreatedTime": datetime,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "OwnerAccountId": str,
-        "ProxyType": Literal["API_GATEWAY"],
-        "State": ApplicationStateType,
-        "Tags": Dict[str, str],
-        "VpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ApplicationSummaryTypeDef = TypedDict(
     "ApplicationSummaryTypeDef",
     {
         "ApiGatewayProxy": ApiGatewayProxySummaryTypeDef,
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
@@ -915,15 +976,15 @@
         "LastUpdatedTime": datetime,
         "OwnerAccountId": str,
         "RouteId": str,
         "RouteType": RouteTypeType,
         "ServiceId": str,
         "State": RouteStateType,
         "Tags": Dict[str, str],
-        "UriPathRoute": UriPathRouteInputTypeDef,
+        "UriPathRoute": UriPathRouteInputOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
@@ -957,22 +1018,22 @@
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
         "Description": str,
         "EndpointType": ServiceEndpointTypeType,
         "EnvironmentId": str,
-        "LambdaEndpoint": LambdaEndpointInputTypeDef,
+        "LambdaEndpoint": LambdaEndpointInputOutputTypeDef,
         "LastUpdatedTime": datetime,
         "Name": str,
         "OwnerAccountId": str,
         "ServiceId": str,
         "State": ServiceStateType,
         "Tags": Dict[str, str],
-        "UrlEndpoint": UrlEndpointInputTypeDef,
+        "UrlEndpoint": UrlEndpointInputOutputTypeDef,
         "VpcId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEnvironmentVpcsResponseTypeDef = TypedDict(
     "ListEnvironmentVpcsResponseTypeDef",
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migration-hub-refactor-spaces
-Version: 1.28.0
-Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-migration-hub-refactor-spaces"></a>
 
 # mypy-boto3-migration-hub-refactor-spaces
 
 [![PyPI - mypy-boto3-migration-hub-refactor-spaces](https://img.shields.io/pypi/v/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migration-hub-refactor-spaces?color=blue)](https://pypistats.org/packages/mypy-boto3-migration-hub-refactor-spaces)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migration-hub-refactor-spaces)](https://pepy.tech/project/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,23 +349,27 @@
 
 `mypy_boto3_migration_hub_refactor_spaces.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migration_hub_refactor_spaces.type_defs import (
     ApiGatewayProxyConfigTypeDef,
+    ApiGatewayProxyInputOutputTypeDef,
     ApiGatewayProxyInputTypeDef,
     ApiGatewayProxySummaryTypeDef,
     ErrorResponseTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentResponseTypeDef,
     DefaultRouteInputTypeDef,
     UriPathRouteInputTypeDef,
+    UriPathRouteInputOutputTypeDef,
     LambdaEndpointInputTypeDef,
     UrlEndpointInputTypeDef,
+    LambdaEndpointInputOutputTypeDef,
+    UrlEndpointInputOutputTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteApplicationResponseTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteEnvironmentResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseTypeDef,
@@ -397,16 +401,16 @@
     PutResourcePolicyRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UrlEndpointSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRouteRequestRequestTypeDef,
     UpdateRouteResponseTypeDef,
-    CreateApplicationRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
+    CreateApplicationRequestRequestTypeDef,
     ApplicationSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     GetApplicationResponseTypeDef,
     GetEnvironmentResponseTypeDef,
     GetRouteResponseTypeDef,
     RouteSummaryTypeDef,
     CreateRouteRequestRequestTypeDef,
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.0/setup.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.12/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migration-hub-refactor-spaces",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_migration_hub_refactor_spaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

