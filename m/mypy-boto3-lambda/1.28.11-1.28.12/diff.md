# Comparing `tmp/mypy-boto3-lambda-1.28.11.tar.gz` & `tmp/mypy-boto3-lambda-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lambda-1.28.11.tar", last modified: Tue Jul 25 19:49:13 2023, max compression
+gzip compressed data, was "mypy-boto3-lambda-1.28.12.tar", last modified: Thu Jul 27 05:34:55 2023, max compression
```

## Comparing `mypy-boto3-lambda-1.28.11.tar` & `mypy-boto3-lambda-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.817034 mypy-boto3-lambda-1.28.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:47:57.000000 mypy-boto3-lambda-1.28.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25545 2023-07-25 19:49:13.817034 mypy-boto3-lambda-1.28.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24062 2023-07-25 19:47:57.000000 mypy-boto3-lambda-1.28.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.809034 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-25 19:47:57.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-25 19:47:57.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-25 19:47:57.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59888 2023-07-25 19:47:59.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59798 2023-07-25 19:47:57.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-07-25 19:47:59.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-07-25 19:47:59.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-07-25 19:47:59.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-07-25 19:47:59.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:47:57.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    81604 2023-07-25 19:48:00.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    81501 2023-07-25 19:48:00.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:47:57.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-25 19:47:59.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-25 19:47:59.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.817034 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25545 2023-07-25 19:49:13.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-25 19:49:13.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:13.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 19:49:13.000000 mypy-boto3-lambda-1.28.11/mypy_boto3_lambda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:13.817034 mypy-boto3-lambda-1.28.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-25 19:47:57.000000 mypy-boto3-lambda-1.28.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.556461 mypy-boto3-lambda-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25529 2023-07-27 05:34:55.556461 mypy-boto3-lambda-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.556461 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59888 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59798 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    82923 2023-07-27 05:24:58.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82816 2023-07-27 05:24:56.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.556461 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25529 2023-07-27 05:34:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:55.556461 mypy-boto3-lambda-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/setup.py
```

### Comparing `mypy-boto3-lambda-1.28.11/LICENSE` & `mypy-boto3-lambda-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.11/PKG-INFO` & `mypy-boto3-lambda-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lambda
-Version: 1.28.11
-Summary: Type annotations for boto3.Lambda 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.Lambda 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lambda"></a>
 
 # mypy-boto3-lambda
 
 [![PyPI - mypy-boto3-lambda](https://img.shields.io/pypi/v/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lambda?color=blue)](https://pypistats.org/packages/mypy-boto3-lambda)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lambda)](https://pepy.tech/project/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
 
@@ -461,24 +461,26 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lambda.type_defs import (
     AccountLimitTypeDef,
     AccountUsageTypeDef,
     AddLayerVersionPermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddLayerVersionPermissionResponseTypeDef,
     AddPermissionRequestRequestTypeDef,
+    AddPermissionResponseTypeDef,
     AliasRoutingConfigurationOutputTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersOutputTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigOutputTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
     CodeSigningPoliciesOutputTypeDef,
     CodeSigningPoliciesTypeDef,
+    ConcurrencyResponseMetadataTypeDef,
     ConcurrencyTypeDef,
     CorsOutputTypeDef,
     CorsTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     ScalingConfigTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
@@ -504,14 +506,15 @@
     DeleteLayerVersionRequestRequestTypeDef,
     DeleteProvisionedConcurrencyConfigRequestRequestTypeDef,
     OnFailureOutputTypeDef,
     OnSuccessOutputTypeDef,
     OnFailureTypeDef,
     OnSuccessTypeDef,
     DocumentDBEventSourceConfigOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnvironmentErrorTypeDef,
     EphemeralStorageOutputTypeDef,
     ScalingConfigOutputTypeDef,
     SelfManagedEventSourceOutputTypeDef,
     SelfManagedKafkaEventSourceConfigOutputTypeDef,
     SourceAccessConfigurationOutputTypeDef,
     FileSystemConfigOutputTypeDef,
@@ -522,79 +525,87 @@
     SnapStartResponseTypeDef,
     TracingConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
     GetAliasRequestRequestTypeDef,
     GetCodeSigningConfigRequestRequestTypeDef,
     GetEventSourceMappingRequestRequestTypeDef,
     GetFunctionCodeSigningConfigRequestRequestTypeDef,
+    GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyRequestRequestTypeDef,
+    GetFunctionConcurrencyResponseTypeDef,
     WaiterConfigTypeDef,
     GetFunctionConfigurationRequestRequestTypeDef,
     GetFunctionEventInvokeConfigRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetFunctionUrlConfigRequestRequestTypeDef,
     GetLayerVersionByArnRequestRequestTypeDef,
     GetLayerVersionPolicyRequestRequestTypeDef,
+    GetLayerVersionPolicyResponseTypeDef,
     GetLayerVersionRequestRequestTypeDef,
     LayerVersionContentOutputTypeDef,
     GetPolicyRequestRequestTypeDef,
+    GetPolicyResponseTypeDef,
     GetProvisionedConcurrencyConfigRequestRequestTypeDef,
+    GetProvisionedConcurrencyConfigResponseTypeDef,
     GetRuntimeManagementConfigRequestRequestTypeDef,
+    GetRuntimeManagementConfigResponseTypeDef,
     ImageConfigErrorTypeDef,
     ImageConfigOutputTypeDef,
     InvocationRequestRequestTypeDef,
+    InvocationResponseTypeDef,
     InvokeAsyncRequestRequestTypeDef,
+    InvokeAsyncResponseTypeDef,
     InvokeResponseStreamUpdateTypeDef,
     InvokeWithResponseStreamCompleteEventTypeDef,
     InvokeWithResponseStreamRequestRequestTypeDef,
     LayerVersionContentInputTypeDef,
     LayerVersionsListItemTypeDef,
-    PaginatorConfigTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
     ListAliasesRequestRequestTypeDef,
+    ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
     ListCodeSigningConfigsRequestRequestTypeDef,
+    ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
     ListEventSourceMappingsRequestRequestTypeDef,
+    ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
     ListFunctionEventInvokeConfigsRequestRequestTypeDef,
+    ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
     ListFunctionUrlConfigsRequestRequestTypeDef,
+    ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
     ListFunctionsByCodeSigningConfigRequestRequestTypeDef,
+    ListFunctionsByCodeSigningConfigResponseTypeDef,
+    ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListFunctionsRequestRequestTypeDef,
+    ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
     ListLayerVersionsRequestRequestTypeDef,
+    ListLayersRequestListLayersPaginateTypeDef,
     ListLayersRequestRequestTypeDef,
+    ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
     ListProvisionedConcurrencyConfigsRequestRequestTypeDef,
     ProvisionedConcurrencyConfigListItemTypeDef,
     ListTagsRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
+    ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListVersionsByFunctionRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PublishVersionRequestRequestTypeDef,
     PutFunctionCodeSigningConfigRequestRequestTypeDef,
+    PutFunctionCodeSigningConfigResponseTypeDef,
     PutFunctionConcurrencyRequestRequestTypeDef,
     PutProvisionedConcurrencyConfigRequestRequestTypeDef,
+    PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigRequestRequestTypeDef,
+    PutRuntimeManagementConfigResponseTypeDef,
     RemoveLayerVersionPermissionRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RuntimeVersionErrorTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFunctionCodeRequestRequestTypeDef,
-    AddLayerVersionPermissionResponseTypeDef,
-    AddPermissionResponseTypeDef,
-    ConcurrencyResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetAccountSettingsResponseTypeDef,
-    GetFunctionCodeSigningConfigResponseTypeDef,
-    GetFunctionConcurrencyResponseTypeDef,
-    GetLayerVersionPolicyResponseTypeDef,
-    GetPolicyResponseTypeDef,
-    GetProvisionedConcurrencyConfigResponseTypeDef,
-    GetRuntimeManagementConfigResponseTypeDef,
-    InvocationResponseTypeDef,
-    InvokeAsyncResponseTypeDef,
-    ListFunctionsByCodeSigningConfigResponseTypeDef,
-    ListTagsResponseTypeDef,
-    PutFunctionCodeSigningConfigResponseTypeDef,
-    PutProvisionedConcurrencyConfigResponseTypeDef,
-    PutRuntimeManagementConfigResponseTypeDef,
     AliasConfigurationResponseMetadataTypeDef,
     AliasConfigurationTypeDef,
     CreateAliasRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     CodeSigningConfigTypeDef,
     CreateCodeSigningConfigRequestRequestTypeDef,
     UpdateCodeSigningConfigRequestRequestTypeDef,
@@ -620,25 +631,14 @@
     GetLayerVersionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     ImageConfigResponseTypeDef,
     InvokeWithResponseStreamResponseEventTypeDef,
     PublishLayerVersionRequestRequestTypeDef,
     LayersListItemTypeDef,
     ListLayerVersionsResponseTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
-    ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
-    ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
-    ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
-    ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
-    ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
-    ListFunctionsRequestListFunctionsPaginateTypeDef,
-    ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
-    ListLayersRequestListLayersPaginateTypeDef,
-    ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
-    ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListProvisionedConcurrencyConfigsResponseTypeDef,
     RuntimeVersionConfigTypeDef,
     ListAliasesResponseTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
```

### Comparing `mypy-boto3-lambda-1.28.11/README.md` & `mypy-boto3-lambda-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lambda"></a>
 
 # mypy-boto3-lambda
 
 [![PyPI - mypy-boto3-lambda](https://img.shields.io/pypi/v/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lambda?color=blue)](https://pypistats.org/packages/mypy-boto3-lambda)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lambda)](https://pepy.tech/project/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
 
@@ -429,24 +429,26 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lambda.type_defs import (
     AccountLimitTypeDef,
     AccountUsageTypeDef,
     AddLayerVersionPermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddLayerVersionPermissionResponseTypeDef,
     AddPermissionRequestRequestTypeDef,
+    AddPermissionResponseTypeDef,
     AliasRoutingConfigurationOutputTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersOutputTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigOutputTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
     CodeSigningPoliciesOutputTypeDef,
     CodeSigningPoliciesTypeDef,
+    ConcurrencyResponseMetadataTypeDef,
     ConcurrencyTypeDef,
     CorsOutputTypeDef,
     CorsTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     ScalingConfigTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
@@ -472,14 +474,15 @@
     DeleteLayerVersionRequestRequestTypeDef,
     DeleteProvisionedConcurrencyConfigRequestRequestTypeDef,
     OnFailureOutputTypeDef,
     OnSuccessOutputTypeDef,
     OnFailureTypeDef,
     OnSuccessTypeDef,
     DocumentDBEventSourceConfigOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnvironmentErrorTypeDef,
     EphemeralStorageOutputTypeDef,
     ScalingConfigOutputTypeDef,
     SelfManagedEventSourceOutputTypeDef,
     SelfManagedKafkaEventSourceConfigOutputTypeDef,
     SourceAccessConfigurationOutputTypeDef,
     FileSystemConfigOutputTypeDef,
@@ -490,79 +493,87 @@
     SnapStartResponseTypeDef,
     TracingConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
     GetAliasRequestRequestTypeDef,
     GetCodeSigningConfigRequestRequestTypeDef,
     GetEventSourceMappingRequestRequestTypeDef,
     GetFunctionCodeSigningConfigRequestRequestTypeDef,
+    GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyRequestRequestTypeDef,
+    GetFunctionConcurrencyResponseTypeDef,
     WaiterConfigTypeDef,
     GetFunctionConfigurationRequestRequestTypeDef,
     GetFunctionEventInvokeConfigRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetFunctionUrlConfigRequestRequestTypeDef,
     GetLayerVersionByArnRequestRequestTypeDef,
     GetLayerVersionPolicyRequestRequestTypeDef,
+    GetLayerVersionPolicyResponseTypeDef,
     GetLayerVersionRequestRequestTypeDef,
     LayerVersionContentOutputTypeDef,
     GetPolicyRequestRequestTypeDef,
+    GetPolicyResponseTypeDef,
     GetProvisionedConcurrencyConfigRequestRequestTypeDef,
+    GetProvisionedConcurrencyConfigResponseTypeDef,
     GetRuntimeManagementConfigRequestRequestTypeDef,
+    GetRuntimeManagementConfigResponseTypeDef,
     ImageConfigErrorTypeDef,
     ImageConfigOutputTypeDef,
     InvocationRequestRequestTypeDef,
+    InvocationResponseTypeDef,
     InvokeAsyncRequestRequestTypeDef,
+    InvokeAsyncResponseTypeDef,
     InvokeResponseStreamUpdateTypeDef,
     InvokeWithResponseStreamCompleteEventTypeDef,
     InvokeWithResponseStreamRequestRequestTypeDef,
     LayerVersionContentInputTypeDef,
     LayerVersionsListItemTypeDef,
-    PaginatorConfigTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
     ListAliasesRequestRequestTypeDef,
+    ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
     ListCodeSigningConfigsRequestRequestTypeDef,
+    ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
     ListEventSourceMappingsRequestRequestTypeDef,
+    ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
     ListFunctionEventInvokeConfigsRequestRequestTypeDef,
+    ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
     ListFunctionUrlConfigsRequestRequestTypeDef,
+    ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
     ListFunctionsByCodeSigningConfigRequestRequestTypeDef,
+    ListFunctionsByCodeSigningConfigResponseTypeDef,
+    ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListFunctionsRequestRequestTypeDef,
+    ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
     ListLayerVersionsRequestRequestTypeDef,
+    ListLayersRequestListLayersPaginateTypeDef,
     ListLayersRequestRequestTypeDef,
+    ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
     ListProvisionedConcurrencyConfigsRequestRequestTypeDef,
     ProvisionedConcurrencyConfigListItemTypeDef,
     ListTagsRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
+    ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListVersionsByFunctionRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PublishVersionRequestRequestTypeDef,
     PutFunctionCodeSigningConfigRequestRequestTypeDef,
+    PutFunctionCodeSigningConfigResponseTypeDef,
     PutFunctionConcurrencyRequestRequestTypeDef,
     PutProvisionedConcurrencyConfigRequestRequestTypeDef,
+    PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigRequestRequestTypeDef,
+    PutRuntimeManagementConfigResponseTypeDef,
     RemoveLayerVersionPermissionRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RuntimeVersionErrorTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFunctionCodeRequestRequestTypeDef,
-    AddLayerVersionPermissionResponseTypeDef,
-    AddPermissionResponseTypeDef,
-    ConcurrencyResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetAccountSettingsResponseTypeDef,
-    GetFunctionCodeSigningConfigResponseTypeDef,
-    GetFunctionConcurrencyResponseTypeDef,
-    GetLayerVersionPolicyResponseTypeDef,
-    GetPolicyResponseTypeDef,
-    GetProvisionedConcurrencyConfigResponseTypeDef,
-    GetRuntimeManagementConfigResponseTypeDef,
-    InvocationResponseTypeDef,
-    InvokeAsyncResponseTypeDef,
-    ListFunctionsByCodeSigningConfigResponseTypeDef,
-    ListTagsResponseTypeDef,
-    PutFunctionCodeSigningConfigResponseTypeDef,
-    PutProvisionedConcurrencyConfigResponseTypeDef,
-    PutRuntimeManagementConfigResponseTypeDef,
     AliasConfigurationResponseMetadataTypeDef,
     AliasConfigurationTypeDef,
     CreateAliasRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     CodeSigningConfigTypeDef,
     CreateCodeSigningConfigRequestRequestTypeDef,
     UpdateCodeSigningConfigRequestRequestTypeDef,
@@ -588,25 +599,14 @@
     GetLayerVersionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     ImageConfigResponseTypeDef,
     InvokeWithResponseStreamResponseEventTypeDef,
     PublishLayerVersionRequestRequestTypeDef,
     LayersListItemTypeDef,
     ListLayerVersionsResponseTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
-    ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
-    ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
-    ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
-    ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
-    ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
-    ListFunctionsRequestListFunctionsPaginateTypeDef,
-    ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
-    ListLayersRequestListLayersPaginateTypeDef,
-    ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
-    ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListProvisionedConcurrencyConfigsResponseTypeDef,
     RuntimeVersionConfigTypeDef,
     ListAliasesResponseTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
```

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/__init__.py` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/__init__.pyi` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/__main__.py` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lambda 1.28.11\nVersion:         1.28.11\nBuilder version:"
-        " 7.15.1\nDocs:           "
+        "Type annotations for boto3.Lambda 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.11")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/client.py` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/client.pyi` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/literals.py` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ArchitectureType",
     "CodeSigningPolicyType",
     "EndPointTypeType",
     "EventSourcePositionType",
     "FullDocumentType",
     "FunctionActiveV2WaiterName",
@@ -65,15 +64,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ArchitectureType = Literal["arm64", "x86_64"]
 CodeSigningPolicyType = Literal["Enforce", "Warn"]
 EndPointTypeType = Literal["KAFKA_BOOTSTRAP_SERVERS"]
 EventSourcePositionType = Literal["AT_TIMESTAMP", "LATEST", "TRIM_HORIZON"]
 FullDocumentType = Literal["Default", "UpdateLookup"]
 FunctionActiveV2WaiterName = Literal["function_active_v2"]
 FunctionActiveWaiterName = Literal["function_active"]
@@ -316,14 +314,15 @@
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
@@ -402,14 +401,15 @@
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
```

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/literals.pyi` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ArchitectureType",
     "CodeSigningPolicyType",
     "EndPointTypeType",
     "EventSourcePositionType",
     "FullDocumentType",
     "FunctionActiveV2WaiterName",
@@ -64,14 +65,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 ArchitectureType = Literal["arm64", "x86_64"]
 CodeSigningPolicyType = Literal["Enforce", "Warn"]
 EndPointTypeType = Literal["KAFKA_BOOTSTRAP_SERVERS"]
 EventSourcePositionType = Literal["AT_TIMESTAMP", "LATEST", "TRIM_HORIZON"]
 FullDocumentType = Literal["Default", "UpdateLookup"]
 FunctionActiveV2WaiterName = Literal["function_active_v2"]
 FunctionActiveWaiterName = Literal["function_active"]
@@ -314,14 +316,15 @@
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
@@ -400,14 +403,15 @@
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
```

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/paginator.py` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -61,217 +61,203 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListAliasesPaginator",
     "ListCodeSigningConfigsPaginator",
     "ListEventSourceMappingsPaginator",
     "ListFunctionEventInvokeConfigsPaginator",
     "ListFunctionUrlConfigsPaginator",
     "ListFunctionsPaginator",
     "ListFunctionsByCodeSigningConfigPaginator",
     "ListLayerVersionsPaginator",
     "ListLayersPaginator",
     "ListProvisionedConcurrencyConfigsPaginator",
     "ListVersionsByFunctionPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listaliasespaginator)
     """
 
     def paginate(
         self,
         *,
         FunctionName: str,
         FunctionVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listaliasespaginator)
         """
 
-
 class ListCodeSigningConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListCodeSigningConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listcodesigningconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCodeSigningConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListCodeSigningConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listcodesigningconfigspaginator)
         """
 
-
 class ListEventSourceMappingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListEventSourceMappings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listeventsourcemappingspaginator)
     """
 
     def paginate(
         self,
         *,
         EventSourceArn: str = ...,
         FunctionName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventSourceMappingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListEventSourceMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listeventsourcemappingspaginator)
         """
 
-
 class ListFunctionEventInvokeConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionEventInvokeConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctioneventinvokeconfigspaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionEventInvokeConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionEventInvokeConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctioneventinvokeconfigspaginator)
         """
 
-
 class ListFunctionUrlConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionUrlConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionurlconfigspaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionUrlConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionUrlConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionurlconfigspaginator)
         """
 
-
 class ListFunctionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionspaginator)
     """
 
     def paginate(
         self,
         *,
         MasterRegion: str = ...,
         FunctionVersion: Literal["ALL"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionspaginator)
         """
 
-
 class ListFunctionsByCodeSigningConfigPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionsByCodeSigningConfig)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionsbycodesigningconfigpaginator)
     """
 
     def paginate(
-        self, *, CodeSigningConfigArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CodeSigningConfigArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionsByCodeSigningConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionsByCodeSigningConfig.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionsbycodesigningconfigpaginator)
         """
 
-
 class ListLayerVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayerVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listlayerversionspaginator)
     """
 
     def paginate(
         self,
         *,
         LayerName: str,
         CompatibleRuntime: RuntimeType = ...,
         CompatibleArchitecture: ArchitectureType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLayerVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayerVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listlayerversionspaginator)
         """
 
-
 class ListLayersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listlayerspaginator)
     """
 
     def paginate(
         self,
         *,
         CompatibleRuntime: RuntimeType = ...,
         CompatibleArchitecture: ArchitectureType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLayersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listlayerspaginator)
         """
 
-
 class ListProvisionedConcurrencyConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListProvisionedConcurrencyConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listprovisionedconcurrencyconfigspaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProvisionedConcurrencyConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListProvisionedConcurrencyConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listprovisionedconcurrencyconfigspaginator)
         """
 
-
 class ListVersionsByFunctionPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListVersionsByFunction)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listversionsbyfunctionpaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVersionsByFunctionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListVersionsByFunction.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listversionsbyfunctionpaginator)
         """
```

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/paginator.pyi` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,203 +61,217 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListAliasesPaginator",
     "ListCodeSigningConfigsPaginator",
     "ListEventSourceMappingsPaginator",
     "ListFunctionEventInvokeConfigsPaginator",
     "ListFunctionUrlConfigsPaginator",
     "ListFunctionsPaginator",
     "ListFunctionsByCodeSigningConfigPaginator",
     "ListLayerVersionsPaginator",
     "ListLayersPaginator",
     "ListProvisionedConcurrencyConfigsPaginator",
     "ListVersionsByFunctionPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listaliasespaginator)
     """
 
     def paginate(
         self,
         *,
         FunctionName: str,
         FunctionVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listaliasespaginator)
         """
 
+
 class ListCodeSigningConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListCodeSigningConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listcodesigningconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCodeSigningConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListCodeSigningConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listcodesigningconfigspaginator)
         """
 
+
 class ListEventSourceMappingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListEventSourceMappings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listeventsourcemappingspaginator)
     """
 
     def paginate(
         self,
         *,
         EventSourceArn: str = ...,
         FunctionName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventSourceMappingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListEventSourceMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listeventsourcemappingspaginator)
         """
 
+
 class ListFunctionEventInvokeConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionEventInvokeConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctioneventinvokeconfigspaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionEventInvokeConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionEventInvokeConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctioneventinvokeconfigspaginator)
         """
 
+
 class ListFunctionUrlConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionUrlConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionurlconfigspaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionUrlConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionUrlConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionurlconfigspaginator)
         """
 
+
 class ListFunctionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionspaginator)
     """
 
     def paginate(
         self,
         *,
         MasterRegion: str = ...,
         FunctionVersion: Literal["ALL"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionspaginator)
         """
 
+
 class ListFunctionsByCodeSigningConfigPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionsByCodeSigningConfig)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionsbycodesigningconfigpaginator)
     """
 
     def paginate(
-        self, *, CodeSigningConfigArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, CodeSigningConfigArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListFunctionsByCodeSigningConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionsByCodeSigningConfig.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionsbycodesigningconfigpaginator)
         """
 
+
 class ListLayerVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayerVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listlayerversionspaginator)
     """
 
     def paginate(
         self,
         *,
         LayerName: str,
         CompatibleRuntime: RuntimeType = ...,
         CompatibleArchitecture: ArchitectureType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLayerVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayerVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listlayerversionspaginator)
         """
 
+
 class ListLayersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listlayerspaginator)
     """
 
     def paginate(
         self,
         *,
         CompatibleRuntime: RuntimeType = ...,
         CompatibleArchitecture: ArchitectureType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListLayersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listlayerspaginator)
         """
 
+
 class ListProvisionedConcurrencyConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListProvisionedConcurrencyConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listprovisionedconcurrencyconfigspaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListProvisionedConcurrencyConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListProvisionedConcurrencyConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listprovisionedconcurrencyconfigspaginator)
         """
 
+
 class ListVersionsByFunctionPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListVersionsByFunction)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listversionsbyfunctionpaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListVersionsByFunctionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListVersionsByFunction.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listversionsbyfunctionpaginator)
         """
```

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/type_defs.py` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,24 +52,26 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountLimitTypeDef",
     "AccountUsageTypeDef",
     "AddLayerVersionPermissionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddLayerVersionPermissionResponseTypeDef",
     "AddPermissionRequestRequestTypeDef",
+    "AddPermissionResponseTypeDef",
     "AliasRoutingConfigurationOutputTypeDef",
     "AliasRoutingConfigurationTypeDef",
     "AllowedPublishersOutputTypeDef",
     "AllowedPublishersTypeDef",
     "AmazonManagedKafkaEventSourceConfigOutputTypeDef",
     "AmazonManagedKafkaEventSourceConfigTypeDef",
     "CodeSigningPoliciesOutputTypeDef",
     "CodeSigningPoliciesTypeDef",
+    "ConcurrencyResponseMetadataTypeDef",
     "ConcurrencyTypeDef",
     "CorsOutputTypeDef",
     "CorsTypeDef",
     "DocumentDBEventSourceConfigTypeDef",
     "ScalingConfigTypeDef",
     "SelfManagedEventSourceTypeDef",
     "SelfManagedKafkaEventSourceConfigTypeDef",
@@ -95,14 +97,15 @@
     "DeleteLayerVersionRequestRequestTypeDef",
     "DeleteProvisionedConcurrencyConfigRequestRequestTypeDef",
     "OnFailureOutputTypeDef",
     "OnSuccessOutputTypeDef",
     "OnFailureTypeDef",
     "OnSuccessTypeDef",
     "DocumentDBEventSourceConfigOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnvironmentErrorTypeDef",
     "EphemeralStorageOutputTypeDef",
     "ScalingConfigOutputTypeDef",
     "SelfManagedEventSourceOutputTypeDef",
     "SelfManagedKafkaEventSourceConfigOutputTypeDef",
     "SourceAccessConfigurationOutputTypeDef",
     "FileSystemConfigOutputTypeDef",
@@ -113,79 +116,87 @@
     "SnapStartResponseTypeDef",
     "TracingConfigResponseTypeDef",
     "VpcConfigResponseTypeDef",
     "GetAliasRequestRequestTypeDef",
     "GetCodeSigningConfigRequestRequestTypeDef",
     "GetEventSourceMappingRequestRequestTypeDef",
     "GetFunctionCodeSigningConfigRequestRequestTypeDef",
+    "GetFunctionCodeSigningConfigResponseTypeDef",
     "GetFunctionConcurrencyRequestRequestTypeDef",
+    "GetFunctionConcurrencyResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetFunctionConfigurationRequestRequestTypeDef",
     "GetFunctionEventInvokeConfigRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetFunctionUrlConfigRequestRequestTypeDef",
     "GetLayerVersionByArnRequestRequestTypeDef",
     "GetLayerVersionPolicyRequestRequestTypeDef",
+    "GetLayerVersionPolicyResponseTypeDef",
     "GetLayerVersionRequestRequestTypeDef",
     "LayerVersionContentOutputTypeDef",
     "GetPolicyRequestRequestTypeDef",
+    "GetPolicyResponseTypeDef",
     "GetProvisionedConcurrencyConfigRequestRequestTypeDef",
+    "GetProvisionedConcurrencyConfigResponseTypeDef",
     "GetRuntimeManagementConfigRequestRequestTypeDef",
+    "GetRuntimeManagementConfigResponseTypeDef",
     "ImageConfigErrorTypeDef",
     "ImageConfigOutputTypeDef",
     "InvocationRequestRequestTypeDef",
+    "InvocationResponseTypeDef",
     "InvokeAsyncRequestRequestTypeDef",
+    "InvokeAsyncResponseTypeDef",
     "InvokeResponseStreamUpdateTypeDef",
     "InvokeWithResponseStreamCompleteEventTypeDef",
     "InvokeWithResponseStreamRequestRequestTypeDef",
     "LayerVersionContentInputTypeDef",
     "LayerVersionsListItemTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAliasesRequestRequestTypeDef",
+    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
     "ListCodeSigningConfigsRequestRequestTypeDef",
+    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
     "ListEventSourceMappingsRequestRequestTypeDef",
+    "ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
     "ListFunctionEventInvokeConfigsRequestRequestTypeDef",
+    "ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
     "ListFunctionUrlConfigsRequestRequestTypeDef",
+    "ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
     "ListFunctionsByCodeSigningConfigRequestRequestTypeDef",
+    "ListFunctionsByCodeSigningConfigResponseTypeDef",
+    "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListFunctionsRequestRequestTypeDef",
+    "ListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
     "ListLayerVersionsRequestRequestTypeDef",
+    "ListLayersRequestListLayersPaginateTypeDef",
     "ListLayersRequestRequestTypeDef",
+    "ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
     "ListProvisionedConcurrencyConfigsRequestRequestTypeDef",
     "ProvisionedConcurrencyConfigListItemTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
+    "ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
     "ListVersionsByFunctionRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PublishVersionRequestRequestTypeDef",
     "PutFunctionCodeSigningConfigRequestRequestTypeDef",
+    "PutFunctionCodeSigningConfigResponseTypeDef",
     "PutFunctionConcurrencyRequestRequestTypeDef",
     "PutProvisionedConcurrencyConfigRequestRequestTypeDef",
+    "PutProvisionedConcurrencyConfigResponseTypeDef",
     "PutRuntimeManagementConfigRequestRequestTypeDef",
+    "PutRuntimeManagementConfigResponseTypeDef",
     "RemoveLayerVersionPermissionRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RuntimeVersionErrorTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFunctionCodeRequestRequestTypeDef",
-    "AddLayerVersionPermissionResponseTypeDef",
-    "AddPermissionResponseTypeDef",
-    "ConcurrencyResponseMetadataTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetAccountSettingsResponseTypeDef",
-    "GetFunctionCodeSigningConfigResponseTypeDef",
-    "GetFunctionConcurrencyResponseTypeDef",
-    "GetLayerVersionPolicyResponseTypeDef",
-    "GetPolicyResponseTypeDef",
-    "GetProvisionedConcurrencyConfigResponseTypeDef",
-    "GetRuntimeManagementConfigResponseTypeDef",
-    "InvocationResponseTypeDef",
-    "InvokeAsyncResponseTypeDef",
-    "ListFunctionsByCodeSigningConfigResponseTypeDef",
-    "ListTagsResponseTypeDef",
-    "PutFunctionCodeSigningConfigResponseTypeDef",
-    "PutProvisionedConcurrencyConfigResponseTypeDef",
-    "PutRuntimeManagementConfigResponseTypeDef",
     "AliasConfigurationResponseMetadataTypeDef",
     "AliasConfigurationTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
     "CodeSigningConfigTypeDef",
     "CreateCodeSigningConfigRequestRequestTypeDef",
     "UpdateCodeSigningConfigRequestRequestTypeDef",
@@ -211,25 +222,14 @@
     "GetLayerVersionResponseTypeDef",
     "PublishLayerVersionResponseTypeDef",
     "ImageConfigResponseTypeDef",
     "InvokeWithResponseStreamResponseEventTypeDef",
     "PublishLayerVersionRequestRequestTypeDef",
     "LayersListItemTypeDef",
     "ListLayerVersionsResponseTypeDef",
-    "ListAliasesRequestListAliasesPaginateTypeDef",
-    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
-    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
-    "ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
-    "ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
-    "ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
-    "ListFunctionsRequestListFunctionsPaginateTypeDef",
-    "ListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
-    "ListLayersRequestListLayersPaginateTypeDef",
-    "ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
-    "ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
     "ListProvisionedConcurrencyConfigsResponseTypeDef",
     "RuntimeVersionConfigTypeDef",
     "ListAliasesResponseTypeDef",
     "CreateCodeSigningConfigResponseTypeDef",
     "GetCodeSigningConfigResponseTypeDef",
     "ListCodeSigningConfigsResponseTypeDef",
     "UpdateCodeSigningConfigResponseTypeDef",
@@ -258,22 +258,24 @@
     {
         "TotalCodeSize": int,
         "CodeSizeUnzipped": int,
         "CodeSizeZipped": int,
         "ConcurrentExecutions": int,
         "UnreservedConcurrentExecutions": int,
     },
+    total=False,
 )
 
 AccountUsageTypeDef = TypedDict(
     "AccountUsageTypeDef",
     {
         "TotalCodeSize": int,
         "FunctionCount": int,
     },
+    total=False,
 )
 
 _RequiredAddLayerVersionPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredAddLayerVersionPermissionRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
@@ -295,22 +297,20 @@
 class AddLayerVersionPermissionRequestRequestTypeDef(
     _RequiredAddLayerVersionPermissionRequestRequestTypeDef,
     _OptionalAddLayerVersionPermissionRequestRequestTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddLayerVersionPermissionResponseTypeDef = TypedDict(
+    "AddLayerVersionPermissionResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Statement": str,
+        "RevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAddPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredAddPermissionRequestRequestTypeDef",
     {
         "FunctionName": str,
@@ -336,19 +336,28 @@
 
 class AddPermissionRequestRequestTypeDef(
     _RequiredAddPermissionRequestRequestTypeDef, _OptionalAddPermissionRequestRequestTypeDef
 ):
     pass
 
 
+AddPermissionResponseTypeDef = TypedDict(
+    "AddPermissionResponseTypeDef",
+    {
+        "Statement": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AliasRoutingConfigurationOutputTypeDef = TypedDict(
     "AliasRoutingConfigurationOutputTypeDef",
     {
         "AdditionalVersionWeights": Dict[str, float],
     },
+    total=False,
 )
 
 AliasRoutingConfigurationTypeDef = TypedDict(
     "AliasRoutingConfigurationTypeDef",
     {
         "AdditionalVersionWeights": Mapping[str, float],
     },
@@ -370,14 +379,15 @@
 )
 
 AmazonManagedKafkaEventSourceConfigOutputTypeDef = TypedDict(
     "AmazonManagedKafkaEventSourceConfigOutputTypeDef",
     {
         "ConsumerGroupId": str,
     },
+    total=False,
 )
 
 AmazonManagedKafkaEventSourceConfigTypeDef = TypedDict(
     "AmazonManagedKafkaEventSourceConfigTypeDef",
     {
         "ConsumerGroupId": str,
     },
@@ -385,41 +395,52 @@
 )
 
 CodeSigningPoliciesOutputTypeDef = TypedDict(
     "CodeSigningPoliciesOutputTypeDef",
     {
         "UntrustedArtifactOnDeployment": CodeSigningPolicyType,
     },
+    total=False,
 )
 
 CodeSigningPoliciesTypeDef = TypedDict(
     "CodeSigningPoliciesTypeDef",
     {
         "UntrustedArtifactOnDeployment": CodeSigningPolicyType,
     },
     total=False,
 )
 
+ConcurrencyResponseMetadataTypeDef = TypedDict(
+    "ConcurrencyResponseMetadataTypeDef",
+    {
+        "ReservedConcurrentExecutions": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConcurrencyTypeDef = TypedDict(
     "ConcurrencyTypeDef",
     {
         "ReservedConcurrentExecutions": int,
     },
+    total=False,
 )
 
 CorsOutputTypeDef = TypedDict(
     "CorsOutputTypeDef",
     {
         "AllowCredentials": bool,
         "AllowHeaders": List[str],
         "AllowMethods": List[str],
         "AllowOrigins": List[str],
         "ExposeHeaders": List[str],
         "MaxAge": int,
     },
+    total=False,
 )
 
 CorsTypeDef = TypedDict(
     "CorsTypeDef",
     {
         "AllowCredentials": bool,
         "AllowHeaders": Sequence[str],
@@ -553,14 +574,15 @@
 )
 
 DeadLetterConfigOutputTypeDef = TypedDict(
     "DeadLetterConfigOutputTypeDef",
     {
         "TargetArn": str,
     },
+    total=False,
 )
 
 DeleteAliasRequestRequestTypeDef = TypedDict(
     "DeleteAliasRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Name": str,
@@ -677,21 +699,23 @@
 )
 
 OnFailureOutputTypeDef = TypedDict(
     "OnFailureOutputTypeDef",
     {
         "Destination": str,
     },
+    total=False,
 )
 
 OnSuccessOutputTypeDef = TypedDict(
     "OnSuccessOutputTypeDef",
     {
         "Destination": str,
     },
+    total=False,
 )
 
 OnFailureTypeDef = TypedDict(
     "OnFailureTypeDef",
     {
         "Destination": str,
     },
@@ -709,58 +733,71 @@
 DocumentDBEventSourceConfigOutputTypeDef = TypedDict(
     "DocumentDBEventSourceConfigOutputTypeDef",
     {
         "DatabaseName": str,
         "CollectionName": str,
         "FullDocument": FullDocumentType,
     },
+    total=False,
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 EnvironmentErrorTypeDef = TypedDict(
     "EnvironmentErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
+    total=False,
 )
 
 EphemeralStorageOutputTypeDef = TypedDict(
     "EphemeralStorageOutputTypeDef",
     {
         "Size": int,
     },
 )
 
 ScalingConfigOutputTypeDef = TypedDict(
     "ScalingConfigOutputTypeDef",
     {
         "MaximumConcurrency": int,
     },
+    total=False,
 )
 
 SelfManagedEventSourceOutputTypeDef = TypedDict(
     "SelfManagedEventSourceOutputTypeDef",
     {
         "Endpoints": Dict[Literal["KAFKA_BOOTSTRAP_SERVERS"], List[str]],
     },
+    total=False,
 )
 
 SelfManagedKafkaEventSourceConfigOutputTypeDef = TypedDict(
     "SelfManagedKafkaEventSourceConfigOutputTypeDef",
     {
         "ConsumerGroupId": str,
     },
+    total=False,
 )
 
 SourceAccessConfigurationOutputTypeDef = TypedDict(
     "SourceAccessConfigurationOutputTypeDef",
     {
         "Type": SourceAccessTypeType,
         "URI": str,
     },
+    total=False,
 )
 
 FileSystemConfigOutputTypeDef = TypedDict(
     "FileSystemConfigOutputTypeDef",
     {
         "Arn": str,
         "LocalMountPath": str,
@@ -768,14 +805,15 @@
 )
 
 FilterOutputTypeDef = TypedDict(
     "FilterOutputTypeDef",
     {
         "Pattern": str,
     },
+    total=False,
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Pattern": str,
     },
@@ -786,48 +824,53 @@
     "FunctionCodeLocationTypeDef",
     {
         "RepositoryType": str,
         "Location": str,
         "ImageUri": str,
         "ResolvedImageUri": str,
     },
+    total=False,
 )
 
 LayerTypeDef = TypedDict(
     "LayerTypeDef",
     {
         "Arn": str,
         "CodeSize": int,
         "SigningProfileVersionArn": str,
         "SigningJobArn": str,
     },
+    total=False,
 )
 
 SnapStartResponseTypeDef = TypedDict(
     "SnapStartResponseTypeDef",
     {
         "ApplyOn": SnapStartApplyOnType,
         "OptimizationStatus": SnapStartOptimizationStatusType,
     },
+    total=False,
 )
 
 TracingConfigResponseTypeDef = TypedDict(
     "TracingConfigResponseTypeDef",
     {
         "Mode": TracingModeType,
     },
+    total=False,
 )
 
 VpcConfigResponseTypeDef = TypedDict(
     "VpcConfigResponseTypeDef",
     {
         "SubnetIds": List[str],
         "SecurityGroupIds": List[str],
         "VpcId": str,
     },
+    total=False,
 )
 
 GetAliasRequestRequestTypeDef = TypedDict(
     "GetAliasRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Name": str,
@@ -851,21 +894,38 @@
 GetFunctionCodeSigningConfigRequestRequestTypeDef = TypedDict(
     "GetFunctionCodeSigningConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 
+GetFunctionCodeSigningConfigResponseTypeDef = TypedDict(
+    "GetFunctionCodeSigningConfigResponseTypeDef",
+    {
+        "CodeSigningConfigArn": str,
+        "FunctionName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetFunctionConcurrencyRequestRequestTypeDef = TypedDict(
     "GetFunctionConcurrencyRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 
+GetFunctionConcurrencyResponseTypeDef = TypedDict(
+    "GetFunctionConcurrencyResponseTypeDef",
+    {
+        "ReservedConcurrentExecutions": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -969,14 +1029,23 @@
     "GetLayerVersionPolicyRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
     },
 )
 
+GetLayerVersionPolicyResponseTypeDef = TypedDict(
+    "GetLayerVersionPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetLayerVersionRequestRequestTypeDef = TypedDict(
     "GetLayerVersionRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
     },
 )
@@ -986,14 +1055,15 @@
     {
         "Location": str,
         "CodeSha256": str,
         "CodeSize": int,
         "SigningProfileVersionArn": str,
         "SigningJobArn": str,
     },
+    total=False,
 )
 
 _RequiredGetPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetPolicyRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
@@ -1009,22 +1079,44 @@
 
 class GetPolicyRequestRequestTypeDef(
     _RequiredGetPolicyRequestRequestTypeDef, _OptionalGetPolicyRequestRequestTypeDef
 ):
     pass
 
 
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetProvisionedConcurrencyConfigRequestRequestTypeDef = TypedDict(
     "GetProvisionedConcurrencyConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Qualifier": str,
     },
 )
 
+GetProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
+    "GetProvisionedConcurrencyConfigResponseTypeDef",
+    {
+        "RequestedProvisionedConcurrentExecutions": int,
+        "AvailableProvisionedConcurrentExecutions": int,
+        "AllocatedProvisionedConcurrentExecutions": int,
+        "Status": ProvisionedConcurrencyStatusEnumType,
+        "StatusReason": str,
+        "LastModified": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRuntimeManagementConfigRequestRequestTypeDef = TypedDict(
     "_RequiredGetRuntimeManagementConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalGetRuntimeManagementConfigRequestRequestTypeDef = TypedDict(
@@ -1039,29 +1131,41 @@
 class GetRuntimeManagementConfigRequestRequestTypeDef(
     _RequiredGetRuntimeManagementConfigRequestRequestTypeDef,
     _OptionalGetRuntimeManagementConfigRequestRequestTypeDef,
 ):
     pass
 
 
+GetRuntimeManagementConfigResponseTypeDef = TypedDict(
+    "GetRuntimeManagementConfigResponseTypeDef",
+    {
+        "UpdateRuntimeOn": UpdateRuntimeOnType,
+        "RuntimeVersionArn": str,
+        "FunctionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImageConfigErrorTypeDef = TypedDict(
     "ImageConfigErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
+    total=False,
 )
 
 ImageConfigOutputTypeDef = TypedDict(
     "ImageConfigOutputTypeDef",
     {
         "EntryPoint": List[str],
         "Command": List[str],
         "WorkingDirectory": str,
     },
+    total=False,
 )
 
 _RequiredInvocationRequestRequestTypeDef = TypedDict(
     "_RequiredInvocationRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
@@ -1081,36 +1185,58 @@
 
 class InvocationRequestRequestTypeDef(
     _RequiredInvocationRequestRequestTypeDef, _OptionalInvocationRequestRequestTypeDef
 ):
     pass
 
 
+InvocationResponseTypeDef = TypedDict(
+    "InvocationResponseTypeDef",
+    {
+        "StatusCode": int,
+        "FunctionError": str,
+        "LogResult": str,
+        "Payload": StreamingBody,
+        "ExecutedVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InvokeAsyncRequestRequestTypeDef = TypedDict(
     "InvokeAsyncRequestRequestTypeDef",
     {
         "FunctionName": str,
         "InvokeArgs": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
+InvokeAsyncResponseTypeDef = TypedDict(
+    "InvokeAsyncResponseTypeDef",
+    {
+        "Status": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InvokeResponseStreamUpdateTypeDef = TypedDict(
     "InvokeResponseStreamUpdateTypeDef",
     {
         "Payload": bytes,
     },
+    total=False,
 )
 
 InvokeWithResponseStreamCompleteEventTypeDef = TypedDict(
     "InvokeWithResponseStreamCompleteEventTypeDef",
     {
         "ErrorCode": str,
         "ErrorDetails": str,
         "LogResult": str,
     },
+    total=False,
 )
 
 _RequiredInvokeWithResponseStreamRequestRequestTypeDef = TypedDict(
     "_RequiredInvokeWithResponseStreamRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
@@ -1153,26 +1279,40 @@
         "Version": int,
         "Description": str,
         "CreatedDate": str,
         "CompatibleRuntimes": List[RuntimeType],
         "LicenseInfo": str,
         "CompatibleArchitectures": List[ArchitectureType],
     },
+    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "FunctionName": str,
+    },
+)
+_OptionalListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "FunctionVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListAliasesRequestListAliasesPaginateTypeDef(
+    _RequiredListAliasesRequestListAliasesPaginateTypeDef,
+    _OptionalListAliasesRequestListAliasesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredListAliasesRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListAliasesRequestRequestTypeDef = TypedDict(
@@ -1188,34 +1328,74 @@
 
 class ListAliasesRequestRequestTypeDef(
     _RequiredListAliasesRequestRequestTypeDef, _OptionalListAliasesRequestRequestTypeDef
 ):
     pass
 
 
+ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef = TypedDict(
+    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCodeSigningConfigsRequestRequestTypeDef = TypedDict(
     "ListCodeSigningConfigsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef = TypedDict(
+    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
+    {
+        "EventSourceArn": str,
+        "FunctionName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEventSourceMappingsRequestRequestTypeDef = TypedDict(
     "ListEventSourceMappingsRequestRequestTypeDef",
     {
         "EventSourceArn": str,
         "FunctionName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef(
+    _RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
+    _OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFunctionEventInvokeConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionEventInvokeConfigsRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListFunctionEventInvokeConfigsRequestRequestTypeDef = TypedDict(
@@ -1231,14 +1411,36 @@
 class ListFunctionEventInvokeConfigsRequestRequestTypeDef(
     _RequiredListFunctionEventInvokeConfigsRequestRequestTypeDef,
     _OptionalListFunctionEventInvokeConfigsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef(
+    _RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
+    _OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFunctionUrlConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionUrlConfigsRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListFunctionUrlConfigsRequestRequestTypeDef = TypedDict(
@@ -1254,14 +1456,36 @@
 class ListFunctionUrlConfigsRequestRequestTypeDef(
     _RequiredListFunctionUrlConfigsRequestRequestTypeDef,
     _OptionalListFunctionUrlConfigsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
+    {
+        "CodeSigningConfigArn": str,
+    },
+)
+_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef(
+    _RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
+    _OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListFunctionsByCodeSigningConfigRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionsByCodeSigningConfigRequestRequestTypeDef",
     {
         "CodeSigningConfigArn": str,
     },
 )
 _OptionalListFunctionsByCodeSigningConfigRequestRequestTypeDef = TypedDict(
@@ -1277,25 +1501,68 @@
 class ListFunctionsByCodeSigningConfigRequestRequestTypeDef(
     _RequiredListFunctionsByCodeSigningConfigRequestRequestTypeDef,
     _OptionalListFunctionsByCodeSigningConfigRequestRequestTypeDef,
 ):
     pass
 
 
+ListFunctionsByCodeSigningConfigResponseTypeDef = TypedDict(
+    "ListFunctionsByCodeSigningConfigResponseTypeDef",
+    {
+        "NextMarker": str,
+        "FunctionArns": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
+    "ListFunctionsRequestListFunctionsPaginateTypeDef",
+    {
+        "MasterRegion": str,
+        "FunctionVersion": Literal["ALL"],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFunctionsRequestRequestTypeDef = TypedDict(
     "ListFunctionsRequestRequestTypeDef",
     {
         "MasterRegion": str,
         "FunctionVersion": Literal["ALL"],
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
+    {
+        "LayerName": str,
+    },
+)
+_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
+    {
+        "CompatibleRuntime": RuntimeType,
+        "CompatibleArchitecture": ArchitectureType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListLayerVersionsRequestListLayerVersionsPaginateTypeDef(
+    _RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
+    _OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListLayerVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLayerVersionsRequestRequestTypeDef",
     {
         "LayerName": str,
     },
 )
 _OptionalListLayerVersionsRequestRequestTypeDef = TypedDict(
@@ -1312,25 +1579,57 @@
 
 class ListLayerVersionsRequestRequestTypeDef(
     _RequiredListLayerVersionsRequestRequestTypeDef, _OptionalListLayerVersionsRequestRequestTypeDef
 ):
     pass
 
 
+ListLayersRequestListLayersPaginateTypeDef = TypedDict(
+    "ListLayersRequestListLayersPaginateTypeDef",
+    {
+        "CompatibleRuntime": RuntimeType,
+        "CompatibleArchitecture": ArchitectureType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLayersRequestRequestTypeDef = TypedDict(
     "ListLayersRequestRequestTypeDef",
     {
         "CompatibleRuntime": RuntimeType,
         "Marker": str,
         "MaxItems": int,
         "CompatibleArchitecture": ArchitectureType,
     },
     total=False,
 )
 
+_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef(
+    _RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
+    _OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListProvisionedConcurrencyConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListProvisionedConcurrencyConfigsRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListProvisionedConcurrencyConfigsRequestRequestTypeDef = TypedDict(
@@ -1357,23 +1656,54 @@
         "RequestedProvisionedConcurrentExecutions": int,
         "AvailableProvisionedConcurrentExecutions": int,
         "AllocatedProvisionedConcurrentExecutions": int,
         "Status": ProvisionedConcurrencyStatusEnumType,
         "StatusReason": str,
         "LastModified": str,
     },
+    total=False,
 )
 
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "Resource": str,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
+    "_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
+    "_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef(
+    _RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
+    _OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListVersionsByFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredListVersionsByFunctionRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListVersionsByFunctionRequestRequestTypeDef = TypedDict(
@@ -1389,14 +1719,24 @@
 class ListVersionsByFunctionRequestRequestTypeDef(
     _RequiredListVersionsByFunctionRequestRequestTypeDef,
     _OptionalListVersionsByFunctionRequestRequestTypeDef,
 ):
     pass
 
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 _RequiredPublishVersionRequestRequestTypeDef = TypedDict(
     "_RequiredPublishVersionRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalPublishVersionRequestRequestTypeDef = TypedDict(
@@ -1420,14 +1760,23 @@
     "PutFunctionCodeSigningConfigRequestRequestTypeDef",
     {
         "CodeSigningConfigArn": str,
         "FunctionName": str,
     },
 )
 
+PutFunctionCodeSigningConfigResponseTypeDef = TypedDict(
+    "PutFunctionCodeSigningConfigResponseTypeDef",
+    {
+        "CodeSigningConfigArn": str,
+        "FunctionName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutFunctionConcurrencyRequestRequestTypeDef = TypedDict(
     "PutFunctionConcurrencyRequestRequestTypeDef",
     {
         "FunctionName": str,
         "ReservedConcurrentExecutions": int,
     },
 )
@@ -1437,14 +1786,27 @@
     {
         "FunctionName": str,
         "Qualifier": str,
         "ProvisionedConcurrentExecutions": int,
     },
 )
 
+PutProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
+    "PutProvisionedConcurrencyConfigResponseTypeDef",
+    {
+        "RequestedProvisionedConcurrentExecutions": int,
+        "AvailableProvisionedConcurrentExecutions": int,
+        "AllocatedProvisionedConcurrentExecutions": int,
+        "Status": ProvisionedConcurrencyStatusEnumType,
+        "StatusReason": str,
+        "LastModified": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutRuntimeManagementConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuntimeManagementConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
         "UpdateRuntimeOn": UpdateRuntimeOnType,
     },
 )
@@ -1461,14 +1823,24 @@
 class PutRuntimeManagementConfigRequestRequestTypeDef(
     _RequiredPutRuntimeManagementConfigRequestRequestTypeDef,
     _OptionalPutRuntimeManagementConfigRequestRequestTypeDef,
 ):
     pass
 
 
+PutRuntimeManagementConfigResponseTypeDef = TypedDict(
+    "PutRuntimeManagementConfigResponseTypeDef",
+    {
+        "UpdateRuntimeOn": UpdateRuntimeOnType,
+        "FunctionArn": str,
+        "RuntimeVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRemoveLayerVersionPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLayerVersionPermissionRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
         "StatementId": str,
     },
@@ -1508,20 +1880,32 @@
 
 class RemovePermissionRequestRequestTypeDef(
     _RequiredRemovePermissionRequestRequestTypeDef, _OptionalRemovePermissionRequestRequestTypeDef
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
 RuntimeVersionErrorTypeDef = TypedDict(
     "RuntimeVersionErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
+    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "Tags": Mapping[str, str],
@@ -1562,205 +1946,47 @@
 class UpdateFunctionCodeRequestRequestTypeDef(
     _RequiredUpdateFunctionCodeRequestRequestTypeDef,
     _OptionalUpdateFunctionCodeRequestRequestTypeDef,
 ):
     pass
 
 
-AddLayerVersionPermissionResponseTypeDef = TypedDict(
-    "AddLayerVersionPermissionResponseTypeDef",
-    {
-        "Statement": str,
-        "RevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddPermissionResponseTypeDef = TypedDict(
-    "AddPermissionResponseTypeDef",
-    {
-        "Statement": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConcurrencyResponseMetadataTypeDef = TypedDict(
-    "ConcurrencyResponseMetadataTypeDef",
-    {
-        "ReservedConcurrentExecutions": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetAccountSettingsResponseTypeDef = TypedDict(
     "GetAccountSettingsResponseTypeDef",
     {
         "AccountLimit": AccountLimitTypeDef,
         "AccountUsage": AccountUsageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetFunctionCodeSigningConfigResponseTypeDef = TypedDict(
-    "GetFunctionCodeSigningConfigResponseTypeDef",
-    {
-        "CodeSigningConfigArn": str,
-        "FunctionName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetFunctionConcurrencyResponseTypeDef = TypedDict(
-    "GetFunctionConcurrencyResponseTypeDef",
-    {
-        "ReservedConcurrentExecutions": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLayerVersionPolicyResponseTypeDef = TypedDict(
-    "GetLayerVersionPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
-    "GetProvisionedConcurrencyConfigResponseTypeDef",
-    {
-        "RequestedProvisionedConcurrentExecutions": int,
-        "AvailableProvisionedConcurrentExecutions": int,
-        "AllocatedProvisionedConcurrentExecutions": int,
-        "Status": ProvisionedConcurrencyStatusEnumType,
-        "StatusReason": str,
-        "LastModified": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRuntimeManagementConfigResponseTypeDef = TypedDict(
-    "GetRuntimeManagementConfigResponseTypeDef",
-    {
-        "UpdateRuntimeOn": UpdateRuntimeOnType,
-        "RuntimeVersionArn": str,
-        "FunctionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InvocationResponseTypeDef = TypedDict(
-    "InvocationResponseTypeDef",
-    {
-        "StatusCode": int,
-        "FunctionError": str,
-        "LogResult": str,
-        "Payload": StreamingBody,
-        "ExecutedVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InvokeAsyncResponseTypeDef = TypedDict(
-    "InvokeAsyncResponseTypeDef",
-    {
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListFunctionsByCodeSigningConfigResponseTypeDef = TypedDict(
-    "ListFunctionsByCodeSigningConfigResponseTypeDef",
-    {
-        "NextMarker": str,
-        "FunctionArns": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutFunctionCodeSigningConfigResponseTypeDef = TypedDict(
-    "PutFunctionCodeSigningConfigResponseTypeDef",
-    {
-        "CodeSigningConfigArn": str,
-        "FunctionName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
-    "PutProvisionedConcurrencyConfigResponseTypeDef",
-    {
-        "RequestedProvisionedConcurrentExecutions": int,
-        "AvailableProvisionedConcurrentExecutions": int,
-        "AllocatedProvisionedConcurrentExecutions": int,
-        "Status": ProvisionedConcurrencyStatusEnumType,
-        "StatusReason": str,
-        "LastModified": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutRuntimeManagementConfigResponseTypeDef = TypedDict(
-    "PutRuntimeManagementConfigResponseTypeDef",
-    {
-        "UpdateRuntimeOn": UpdateRuntimeOnType,
-        "FunctionArn": str,
-        "RuntimeVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AliasConfigurationResponseMetadataTypeDef = TypedDict(
     "AliasConfigurationResponseMetadataTypeDef",
     {
         "AliasArn": str,
         "Name": str,
         "FunctionVersion": str,
         "Description": str,
         "RoutingConfig": AliasRoutingConfigurationOutputTypeDef,
         "RevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AliasConfigurationTypeDef = TypedDict(
     "AliasConfigurationTypeDef",
     {
         "AliasArn": str,
         "Name": str,
         "FunctionVersion": str,
         "Description": str,
         "RoutingConfig": AliasRoutingConfigurationOutputTypeDef,
         "RevisionId": str,
     },
+    total=False,
 )
 
 _RequiredCreateAliasRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAliasRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Name": str,
@@ -1804,25 +2030,38 @@
 
 class UpdateAliasRequestRequestTypeDef(
     _RequiredUpdateAliasRequestRequestTypeDef, _OptionalUpdateAliasRequestRequestTypeDef
 ):
     pass
 
 
-CodeSigningConfigTypeDef = TypedDict(
-    "CodeSigningConfigTypeDef",
+_RequiredCodeSigningConfigTypeDef = TypedDict(
+    "_RequiredCodeSigningConfigTypeDef",
     {
         "CodeSigningConfigId": str,
         "CodeSigningConfigArn": str,
-        "Description": str,
         "AllowedPublishers": AllowedPublishersOutputTypeDef,
         "CodeSigningPolicies": CodeSigningPoliciesOutputTypeDef,
         "LastModified": str,
     },
 )
+_OptionalCodeSigningConfigTypeDef = TypedDict(
+    "_OptionalCodeSigningConfigTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class CodeSigningConfigTypeDef(
+    _RequiredCodeSigningConfigTypeDef, _OptionalCodeSigningConfigTypeDef
+):
+    pass
+
 
 _RequiredCreateCodeSigningConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCodeSigningConfigRequestRequestTypeDef",
     {
         "AllowedPublishers": AllowedPublishersTypeDef,
     },
 )
@@ -1872,56 +2111,69 @@
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
         "Cors": CorsOutputTypeDef,
         "CreationTime": str,
         "InvokeMode": InvokeModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-FunctionUrlConfigTypeDef = TypedDict(
-    "FunctionUrlConfigTypeDef",
+_RequiredFunctionUrlConfigTypeDef = TypedDict(
+    "_RequiredFunctionUrlConfigTypeDef",
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "CreationTime": str,
         "LastModifiedTime": str,
-        "Cors": CorsOutputTypeDef,
         "AuthType": FunctionUrlAuthTypeType,
+    },
+)
+_OptionalFunctionUrlConfigTypeDef = TypedDict(
+    "_OptionalFunctionUrlConfigTypeDef",
+    {
+        "Cors": CorsOutputTypeDef,
         "InvokeMode": InvokeModeType,
     },
+    total=False,
 )
 
+
+class FunctionUrlConfigTypeDef(
+    _RequiredFunctionUrlConfigTypeDef, _OptionalFunctionUrlConfigTypeDef
+):
+    pass
+
+
 GetFunctionUrlConfigResponseTypeDef = TypedDict(
     "GetFunctionUrlConfigResponseTypeDef",
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
         "Cors": CorsOutputTypeDef,
         "CreationTime": str,
         "LastModifiedTime": str,
         "InvokeMode": InvokeModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFunctionUrlConfigResponseTypeDef = TypedDict(
     "UpdateFunctionUrlConfigResponseTypeDef",
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
         "Cors": CorsOutputTypeDef,
         "CreationTime": str,
         "LastModifiedTime": str,
         "InvokeMode": InvokeModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFunctionUrlConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
@@ -2053,14 +2305,15 @@
 
 DestinationConfigOutputTypeDef = TypedDict(
     "DestinationConfigOutputTypeDef",
     {
         "OnSuccess": OnSuccessOutputTypeDef,
         "OnFailure": OnFailureOutputTypeDef,
     },
+    total=False,
 )
 
 DestinationConfigTypeDef = TypedDict(
     "DestinationConfigTypeDef",
     {
         "OnSuccess": OnSuccessTypeDef,
         "OnFailure": OnFailureTypeDef,
@@ -2070,21 +2323,23 @@
 
 EnvironmentResponseTypeDef = TypedDict(
     "EnvironmentResponseTypeDef",
     {
         "Variables": Dict[str, str],
         "Error": EnvironmentErrorTypeDef,
     },
+    total=False,
 )
 
 FilterCriteriaOutputTypeDef = TypedDict(
     "FilterCriteriaOutputTypeDef",
     {
         "Filters": List[FilterOutputTypeDef],
     },
+    total=False,
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
     },
@@ -2237,15 +2492,15 @@
         "LayerVersionArn": str,
         "Description": str,
         "CreatedDate": str,
         "Version": int,
         "CompatibleRuntimes": List[RuntimeType],
         "LicenseInfo": str,
         "CompatibleArchitectures": List[ArchitectureType],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PublishLayerVersionResponseTypeDef = TypedDict(
     "PublishLayerVersionResponseTypeDef",
     {
         "Content": LayerVersionContentOutputTypeDef,
@@ -2253,32 +2508,34 @@
         "LayerVersionArn": str,
         "Description": str,
         "CreatedDate": str,
         "Version": int,
         "CompatibleRuntimes": List[RuntimeType],
         "LicenseInfo": str,
         "CompatibleArchitectures": List[ArchitectureType],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImageConfigResponseTypeDef = TypedDict(
     "ImageConfigResponseTypeDef",
     {
         "ImageConfig": ImageConfigOutputTypeDef,
         "Error": ImageConfigErrorTypeDef,
     },
+    total=False,
 )
 
 InvokeWithResponseStreamResponseEventTypeDef = TypedDict(
     "InvokeWithResponseStreamResponseEventTypeDef",
     {
         "PayloadChunk": InvokeResponseStreamUpdateTypeDef,
         "InvokeComplete": InvokeWithResponseStreamCompleteEventTypeDef,
     },
+    total=False,
 )
 
 _RequiredPublishLayerVersionRequestRequestTypeDef = TypedDict(
     "_RequiredPublishLayerVersionRequestRequestTypeDef",
     {
         "LayerName": str,
         "Content": LayerVersionContentInputTypeDef,
@@ -2306,309 +2563,117 @@
 LayersListItemTypeDef = TypedDict(
     "LayersListItemTypeDef",
     {
         "LayerName": str,
         "LayerArn": str,
         "LatestMatchingVersion": LayerVersionsListItemTypeDef,
     },
+    total=False,
 )
 
 ListLayerVersionsResponseTypeDef = TypedDict(
     "ListLayerVersionsResponseTypeDef",
     {
         "NextMarker": str,
         "LayerVersions": List[LayerVersionsListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
-    {
-        "FunctionVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListAliasesRequestListAliasesPaginateTypeDef(
-    _RequiredListAliasesRequestListAliasesPaginateTypeDef,
-    _OptionalListAliasesRequestListAliasesPaginateTypeDef,
-):
-    pass
-
-
-ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef = TypedDict(
-    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef = TypedDict(
-    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
-    {
-        "EventSourceArn": str,
-        "FunctionName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef(
-    _RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
-    _OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef(
-    _RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
-    _OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
-    {
-        "CodeSigningConfigArn": str,
-    },
-)
-_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef(
-    _RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
-    _OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
-):
-    pass
-
-
-ListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
-    "ListFunctionsRequestListFunctionsPaginateTypeDef",
-    {
-        "MasterRegion": str,
-        "FunctionVersion": Literal["ALL"],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
-    {
-        "LayerName": str,
-    },
-)
-_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
-    {
-        "CompatibleRuntime": RuntimeType,
-        "CompatibleArchitecture": ArchitectureType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListLayerVersionsRequestListLayerVersionsPaginateTypeDef(
-    _RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
-    _OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
-):
-    pass
-
-
-ListLayersRequestListLayersPaginateTypeDef = TypedDict(
-    "ListLayersRequestListLayersPaginateTypeDef",
-    {
-        "CompatibleRuntime": RuntimeType,
-        "CompatibleArchitecture": ArchitectureType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef(
-    _RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
-    _OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
-    "_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
-    {
-        "FunctionName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
-    "_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef(
-    _RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
-    _OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
-):
-    pass
-
 
 ListProvisionedConcurrencyConfigsResponseTypeDef = TypedDict(
     "ListProvisionedConcurrencyConfigsResponseTypeDef",
     {
         "ProvisionedConcurrencyConfigs": List[ProvisionedConcurrencyConfigListItemTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuntimeVersionConfigTypeDef = TypedDict(
     "RuntimeVersionConfigTypeDef",
     {
         "RuntimeVersionArn": str,
         "Error": RuntimeVersionErrorTypeDef,
     },
+    total=False,
 )
 
 ListAliasesResponseTypeDef = TypedDict(
     "ListAliasesResponseTypeDef",
     {
         "NextMarker": str,
         "Aliases": List[AliasConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCodeSigningConfigResponseTypeDef = TypedDict(
     "CreateCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCodeSigningConfigResponseTypeDef = TypedDict(
     "GetCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCodeSigningConfigsResponseTypeDef = TypedDict(
     "ListCodeSigningConfigsResponseTypeDef",
     {
         "NextMarker": str,
         "CodeSigningConfigs": List[CodeSigningConfigTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCodeSigningConfigResponseTypeDef = TypedDict(
     "UpdateCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFunctionUrlConfigsResponseTypeDef = TypedDict(
     "ListFunctionUrlConfigsResponseTypeDef",
     {
         "FunctionUrlConfigs": List[FunctionUrlConfigTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionEventInvokeConfigResponseMetadataTypeDef = TypedDict(
     "FunctionEventInvokeConfigResponseMetadataTypeDef",
     {
         "LastModified": datetime,
         "FunctionArn": str,
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
         "DestinationConfig": DestinationConfigOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionEventInvokeConfigTypeDef = TypedDict(
     "FunctionEventInvokeConfigTypeDef",
     {
         "LastModified": datetime,
         "FunctionArn": str,
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
         "DestinationConfig": DestinationConfigOutputTypeDef,
     },
+    total=False,
 )
 
 _RequiredPutFunctionEventInvokeConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutFunctionEventInvokeConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
@@ -2683,15 +2748,15 @@
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigOutputTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigOutputTypeDef,
         "ScalingConfig": ScalingConfigOutputTypeDef,
         "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventSourceMappingConfigurationTypeDef = TypedDict(
     "EventSourceMappingConfigurationTypeDef",
     {
         "UUID": str,
@@ -2718,14 +2783,15 @@
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigOutputTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigOutputTypeDef,
         "ScalingConfig": ScalingConfigOutputTypeDef,
         "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigOutputTypeDef,
     },
+    total=False,
 )
 
 _RequiredCreateEventSourceMappingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventSourceMappingRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
@@ -2806,24 +2872,24 @@
 InvokeWithResponseStreamResponseTypeDef = TypedDict(
     "InvokeWithResponseStreamResponseTypeDef",
     {
         "StatusCode": int,
         "ExecutedVersion": str,
         "EventStream": "EventStream[InvokeWithResponseStreamResponseEventTypeDef]",
         "ResponseStreamContentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLayersResponseTypeDef = TypedDict(
     "ListLayersResponseTypeDef",
     {
         "NextMarker": str,
         "Layers": List[LayersListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionConfigurationResponseMetadataTypeDef = TypedDict(
     "FunctionConfigurationResponseMetadataTypeDef",
     {
         "FunctionName": str,
@@ -2857,15 +2923,15 @@
         "ImageConfigResponse": ImageConfigResponseTypeDef,
         "SigningProfileVersionArn": str,
         "SigningJobArn": str,
         "Architectures": List[ArchitectureType],
         "EphemeralStorage": EphemeralStorageOutputTypeDef,
         "SnapStart": SnapStartResponseTypeDef,
         "RuntimeVersionConfig": RuntimeVersionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionConfigurationTypeDef = TypedDict(
     "FunctionConfigurationTypeDef",
     {
         "FunctionName": str,
@@ -2900,55 +2966,56 @@
         "SigningProfileVersionArn": str,
         "SigningJobArn": str,
         "Architectures": List[ArchitectureType],
         "EphemeralStorage": EphemeralStorageOutputTypeDef,
         "SnapStart": SnapStartResponseTypeDef,
         "RuntimeVersionConfig": RuntimeVersionConfigTypeDef,
     },
+    total=False,
 )
 
 ListFunctionEventInvokeConfigsResponseTypeDef = TypedDict(
     "ListFunctionEventInvokeConfigsResponseTypeDef",
     {
         "FunctionEventInvokeConfigs": List[FunctionEventInvokeConfigTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventSourceMappingsResponseTypeDef = TypedDict(
     "ListEventSourceMappingsResponseTypeDef",
     {
         "NextMarker": str,
         "EventSourceMappings": List[EventSourceMappingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFunctionResponseTypeDef = TypedDict(
     "GetFunctionResponseTypeDef",
     {
         "Configuration": FunctionConfigurationTypeDef,
         "Code": FunctionCodeLocationTypeDef,
         "Tags": Dict[str, str],
         "Concurrency": ConcurrencyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFunctionsResponseTypeDef = TypedDict(
     "ListFunctionsResponseTypeDef",
     {
         "NextMarker": str,
         "Functions": List[FunctionConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVersionsByFunctionResponseTypeDef = TypedDict(
     "ListVersionsByFunctionResponseTypeDef",
     {
         "NextMarker": str,
         "Versions": List[FunctionConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/type_defs.pyi` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -51,24 +51,26 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountLimitTypeDef",
     "AccountUsageTypeDef",
     "AddLayerVersionPermissionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddLayerVersionPermissionResponseTypeDef",
     "AddPermissionRequestRequestTypeDef",
+    "AddPermissionResponseTypeDef",
     "AliasRoutingConfigurationOutputTypeDef",
     "AliasRoutingConfigurationTypeDef",
     "AllowedPublishersOutputTypeDef",
     "AllowedPublishersTypeDef",
     "AmazonManagedKafkaEventSourceConfigOutputTypeDef",
     "AmazonManagedKafkaEventSourceConfigTypeDef",
     "CodeSigningPoliciesOutputTypeDef",
     "CodeSigningPoliciesTypeDef",
+    "ConcurrencyResponseMetadataTypeDef",
     "ConcurrencyTypeDef",
     "CorsOutputTypeDef",
     "CorsTypeDef",
     "DocumentDBEventSourceConfigTypeDef",
     "ScalingConfigTypeDef",
     "SelfManagedEventSourceTypeDef",
     "SelfManagedKafkaEventSourceConfigTypeDef",
@@ -94,14 +96,15 @@
     "DeleteLayerVersionRequestRequestTypeDef",
     "DeleteProvisionedConcurrencyConfigRequestRequestTypeDef",
     "OnFailureOutputTypeDef",
     "OnSuccessOutputTypeDef",
     "OnFailureTypeDef",
     "OnSuccessTypeDef",
     "DocumentDBEventSourceConfigOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnvironmentErrorTypeDef",
     "EphemeralStorageOutputTypeDef",
     "ScalingConfigOutputTypeDef",
     "SelfManagedEventSourceOutputTypeDef",
     "SelfManagedKafkaEventSourceConfigOutputTypeDef",
     "SourceAccessConfigurationOutputTypeDef",
     "FileSystemConfigOutputTypeDef",
@@ -112,79 +115,87 @@
     "SnapStartResponseTypeDef",
     "TracingConfigResponseTypeDef",
     "VpcConfigResponseTypeDef",
     "GetAliasRequestRequestTypeDef",
     "GetCodeSigningConfigRequestRequestTypeDef",
     "GetEventSourceMappingRequestRequestTypeDef",
     "GetFunctionCodeSigningConfigRequestRequestTypeDef",
+    "GetFunctionCodeSigningConfigResponseTypeDef",
     "GetFunctionConcurrencyRequestRequestTypeDef",
+    "GetFunctionConcurrencyResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetFunctionConfigurationRequestRequestTypeDef",
     "GetFunctionEventInvokeConfigRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetFunctionUrlConfigRequestRequestTypeDef",
     "GetLayerVersionByArnRequestRequestTypeDef",
     "GetLayerVersionPolicyRequestRequestTypeDef",
+    "GetLayerVersionPolicyResponseTypeDef",
     "GetLayerVersionRequestRequestTypeDef",
     "LayerVersionContentOutputTypeDef",
     "GetPolicyRequestRequestTypeDef",
+    "GetPolicyResponseTypeDef",
     "GetProvisionedConcurrencyConfigRequestRequestTypeDef",
+    "GetProvisionedConcurrencyConfigResponseTypeDef",
     "GetRuntimeManagementConfigRequestRequestTypeDef",
+    "GetRuntimeManagementConfigResponseTypeDef",
     "ImageConfigErrorTypeDef",
     "ImageConfigOutputTypeDef",
     "InvocationRequestRequestTypeDef",
+    "InvocationResponseTypeDef",
     "InvokeAsyncRequestRequestTypeDef",
+    "InvokeAsyncResponseTypeDef",
     "InvokeResponseStreamUpdateTypeDef",
     "InvokeWithResponseStreamCompleteEventTypeDef",
     "InvokeWithResponseStreamRequestRequestTypeDef",
     "LayerVersionContentInputTypeDef",
     "LayerVersionsListItemTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAliasesRequestRequestTypeDef",
+    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
     "ListCodeSigningConfigsRequestRequestTypeDef",
+    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
     "ListEventSourceMappingsRequestRequestTypeDef",
+    "ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
     "ListFunctionEventInvokeConfigsRequestRequestTypeDef",
+    "ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
     "ListFunctionUrlConfigsRequestRequestTypeDef",
+    "ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
     "ListFunctionsByCodeSigningConfigRequestRequestTypeDef",
+    "ListFunctionsByCodeSigningConfigResponseTypeDef",
+    "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListFunctionsRequestRequestTypeDef",
+    "ListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
     "ListLayerVersionsRequestRequestTypeDef",
+    "ListLayersRequestListLayersPaginateTypeDef",
     "ListLayersRequestRequestTypeDef",
+    "ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
     "ListProvisionedConcurrencyConfigsRequestRequestTypeDef",
     "ProvisionedConcurrencyConfigListItemTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
+    "ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
     "ListVersionsByFunctionRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "PublishVersionRequestRequestTypeDef",
     "PutFunctionCodeSigningConfigRequestRequestTypeDef",
+    "PutFunctionCodeSigningConfigResponseTypeDef",
     "PutFunctionConcurrencyRequestRequestTypeDef",
     "PutProvisionedConcurrencyConfigRequestRequestTypeDef",
+    "PutProvisionedConcurrencyConfigResponseTypeDef",
     "PutRuntimeManagementConfigRequestRequestTypeDef",
+    "PutRuntimeManagementConfigResponseTypeDef",
     "RemoveLayerVersionPermissionRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "RuntimeVersionErrorTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFunctionCodeRequestRequestTypeDef",
-    "AddLayerVersionPermissionResponseTypeDef",
-    "AddPermissionResponseTypeDef",
-    "ConcurrencyResponseMetadataTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetAccountSettingsResponseTypeDef",
-    "GetFunctionCodeSigningConfigResponseTypeDef",
-    "GetFunctionConcurrencyResponseTypeDef",
-    "GetLayerVersionPolicyResponseTypeDef",
-    "GetPolicyResponseTypeDef",
-    "GetProvisionedConcurrencyConfigResponseTypeDef",
-    "GetRuntimeManagementConfigResponseTypeDef",
-    "InvocationResponseTypeDef",
-    "InvokeAsyncResponseTypeDef",
-    "ListFunctionsByCodeSigningConfigResponseTypeDef",
-    "ListTagsResponseTypeDef",
-    "PutFunctionCodeSigningConfigResponseTypeDef",
-    "PutProvisionedConcurrencyConfigResponseTypeDef",
-    "PutRuntimeManagementConfigResponseTypeDef",
     "AliasConfigurationResponseMetadataTypeDef",
     "AliasConfigurationTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
     "CodeSigningConfigTypeDef",
     "CreateCodeSigningConfigRequestRequestTypeDef",
     "UpdateCodeSigningConfigRequestRequestTypeDef",
@@ -210,25 +221,14 @@
     "GetLayerVersionResponseTypeDef",
     "PublishLayerVersionResponseTypeDef",
     "ImageConfigResponseTypeDef",
     "InvokeWithResponseStreamResponseEventTypeDef",
     "PublishLayerVersionRequestRequestTypeDef",
     "LayersListItemTypeDef",
     "ListLayerVersionsResponseTypeDef",
-    "ListAliasesRequestListAliasesPaginateTypeDef",
-    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
-    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
-    "ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
-    "ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
-    "ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
-    "ListFunctionsRequestListFunctionsPaginateTypeDef",
-    "ListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
-    "ListLayersRequestListLayersPaginateTypeDef",
-    "ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
-    "ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
     "ListProvisionedConcurrencyConfigsResponseTypeDef",
     "RuntimeVersionConfigTypeDef",
     "ListAliasesResponseTypeDef",
     "CreateCodeSigningConfigResponseTypeDef",
     "GetCodeSigningConfigResponseTypeDef",
     "ListCodeSigningConfigsResponseTypeDef",
     "UpdateCodeSigningConfigResponseTypeDef",
@@ -257,22 +257,24 @@
     {
         "TotalCodeSize": int,
         "CodeSizeUnzipped": int,
         "CodeSizeZipped": int,
         "ConcurrentExecutions": int,
         "UnreservedConcurrentExecutions": int,
     },
+    total=False,
 )
 
 AccountUsageTypeDef = TypedDict(
     "AccountUsageTypeDef",
     {
         "TotalCodeSize": int,
         "FunctionCount": int,
     },
+    total=False,
 )
 
 _RequiredAddLayerVersionPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredAddLayerVersionPermissionRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
@@ -292,22 +294,20 @@
 
 class AddLayerVersionPermissionRequestRequestTypeDef(
     _RequiredAddLayerVersionPermissionRequestRequestTypeDef,
     _OptionalAddLayerVersionPermissionRequestRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddLayerVersionPermissionResponseTypeDef = TypedDict(
+    "AddLayerVersionPermissionResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Statement": str,
+        "RevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredAddPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredAddPermissionRequestRequestTypeDef",
     {
         "FunctionName": str,
@@ -331,19 +331,28 @@
 )
 
 class AddPermissionRequestRequestTypeDef(
     _RequiredAddPermissionRequestRequestTypeDef, _OptionalAddPermissionRequestRequestTypeDef
 ):
     pass
 
+AddPermissionResponseTypeDef = TypedDict(
+    "AddPermissionResponseTypeDef",
+    {
+        "Statement": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AliasRoutingConfigurationOutputTypeDef = TypedDict(
     "AliasRoutingConfigurationOutputTypeDef",
     {
         "AdditionalVersionWeights": Dict[str, float],
     },
+    total=False,
 )
 
 AliasRoutingConfigurationTypeDef = TypedDict(
     "AliasRoutingConfigurationTypeDef",
     {
         "AdditionalVersionWeights": Mapping[str, float],
     },
@@ -365,14 +374,15 @@
 )
 
 AmazonManagedKafkaEventSourceConfigOutputTypeDef = TypedDict(
     "AmazonManagedKafkaEventSourceConfigOutputTypeDef",
     {
         "ConsumerGroupId": str,
     },
+    total=False,
 )
 
 AmazonManagedKafkaEventSourceConfigTypeDef = TypedDict(
     "AmazonManagedKafkaEventSourceConfigTypeDef",
     {
         "ConsumerGroupId": str,
     },
@@ -380,41 +390,52 @@
 )
 
 CodeSigningPoliciesOutputTypeDef = TypedDict(
     "CodeSigningPoliciesOutputTypeDef",
     {
         "UntrustedArtifactOnDeployment": CodeSigningPolicyType,
     },
+    total=False,
 )
 
 CodeSigningPoliciesTypeDef = TypedDict(
     "CodeSigningPoliciesTypeDef",
     {
         "UntrustedArtifactOnDeployment": CodeSigningPolicyType,
     },
     total=False,
 )
 
+ConcurrencyResponseMetadataTypeDef = TypedDict(
+    "ConcurrencyResponseMetadataTypeDef",
+    {
+        "ReservedConcurrentExecutions": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ConcurrencyTypeDef = TypedDict(
     "ConcurrencyTypeDef",
     {
         "ReservedConcurrentExecutions": int,
     },
+    total=False,
 )
 
 CorsOutputTypeDef = TypedDict(
     "CorsOutputTypeDef",
     {
         "AllowCredentials": bool,
         "AllowHeaders": List[str],
         "AllowMethods": List[str],
         "AllowOrigins": List[str],
         "ExposeHeaders": List[str],
         "MaxAge": int,
     },
+    total=False,
 )
 
 CorsTypeDef = TypedDict(
     "CorsTypeDef",
     {
         "AllowCredentials": bool,
         "AllowHeaders": Sequence[str],
@@ -548,14 +569,15 @@
 )
 
 DeadLetterConfigOutputTypeDef = TypedDict(
     "DeadLetterConfigOutputTypeDef",
     {
         "TargetArn": str,
     },
+    total=False,
 )
 
 DeleteAliasRequestRequestTypeDef = TypedDict(
     "DeleteAliasRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Name": str,
@@ -666,21 +688,23 @@
 )
 
 OnFailureOutputTypeDef = TypedDict(
     "OnFailureOutputTypeDef",
     {
         "Destination": str,
     },
+    total=False,
 )
 
 OnSuccessOutputTypeDef = TypedDict(
     "OnSuccessOutputTypeDef",
     {
         "Destination": str,
     },
+    total=False,
 )
 
 OnFailureTypeDef = TypedDict(
     "OnFailureTypeDef",
     {
         "Destination": str,
     },
@@ -698,58 +722,71 @@
 DocumentDBEventSourceConfigOutputTypeDef = TypedDict(
     "DocumentDBEventSourceConfigOutputTypeDef",
     {
         "DatabaseName": str,
         "CollectionName": str,
         "FullDocument": FullDocumentType,
     },
+    total=False,
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 EnvironmentErrorTypeDef = TypedDict(
     "EnvironmentErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
+    total=False,
 )
 
 EphemeralStorageOutputTypeDef = TypedDict(
     "EphemeralStorageOutputTypeDef",
     {
         "Size": int,
     },
 )
 
 ScalingConfigOutputTypeDef = TypedDict(
     "ScalingConfigOutputTypeDef",
     {
         "MaximumConcurrency": int,
     },
+    total=False,
 )
 
 SelfManagedEventSourceOutputTypeDef = TypedDict(
     "SelfManagedEventSourceOutputTypeDef",
     {
         "Endpoints": Dict[Literal["KAFKA_BOOTSTRAP_SERVERS"], List[str]],
     },
+    total=False,
 )
 
 SelfManagedKafkaEventSourceConfigOutputTypeDef = TypedDict(
     "SelfManagedKafkaEventSourceConfigOutputTypeDef",
     {
         "ConsumerGroupId": str,
     },
+    total=False,
 )
 
 SourceAccessConfigurationOutputTypeDef = TypedDict(
     "SourceAccessConfigurationOutputTypeDef",
     {
         "Type": SourceAccessTypeType,
         "URI": str,
     },
+    total=False,
 )
 
 FileSystemConfigOutputTypeDef = TypedDict(
     "FileSystemConfigOutputTypeDef",
     {
         "Arn": str,
         "LocalMountPath": str,
@@ -757,14 +794,15 @@
 )
 
 FilterOutputTypeDef = TypedDict(
     "FilterOutputTypeDef",
     {
         "Pattern": str,
     },
+    total=False,
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Pattern": str,
     },
@@ -775,48 +813,53 @@
     "FunctionCodeLocationTypeDef",
     {
         "RepositoryType": str,
         "Location": str,
         "ImageUri": str,
         "ResolvedImageUri": str,
     },
+    total=False,
 )
 
 LayerTypeDef = TypedDict(
     "LayerTypeDef",
     {
         "Arn": str,
         "CodeSize": int,
         "SigningProfileVersionArn": str,
         "SigningJobArn": str,
     },
+    total=False,
 )
 
 SnapStartResponseTypeDef = TypedDict(
     "SnapStartResponseTypeDef",
     {
         "ApplyOn": SnapStartApplyOnType,
         "OptimizationStatus": SnapStartOptimizationStatusType,
     },
+    total=False,
 )
 
 TracingConfigResponseTypeDef = TypedDict(
     "TracingConfigResponseTypeDef",
     {
         "Mode": TracingModeType,
     },
+    total=False,
 )
 
 VpcConfigResponseTypeDef = TypedDict(
     "VpcConfigResponseTypeDef",
     {
         "SubnetIds": List[str],
         "SecurityGroupIds": List[str],
         "VpcId": str,
     },
+    total=False,
 )
 
 GetAliasRequestRequestTypeDef = TypedDict(
     "GetAliasRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Name": str,
@@ -840,21 +883,38 @@
 GetFunctionCodeSigningConfigRequestRequestTypeDef = TypedDict(
     "GetFunctionCodeSigningConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 
+GetFunctionCodeSigningConfigResponseTypeDef = TypedDict(
+    "GetFunctionCodeSigningConfigResponseTypeDef",
+    {
+        "CodeSigningConfigArn": str,
+        "FunctionName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetFunctionConcurrencyRequestRequestTypeDef = TypedDict(
     "GetFunctionConcurrencyRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 
+GetFunctionConcurrencyResponseTypeDef = TypedDict(
+    "GetFunctionConcurrencyResponseTypeDef",
+    {
+        "ReservedConcurrentExecutions": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -950,14 +1010,23 @@
     "GetLayerVersionPolicyRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
     },
 )
 
+GetLayerVersionPolicyResponseTypeDef = TypedDict(
+    "GetLayerVersionPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetLayerVersionRequestRequestTypeDef = TypedDict(
     "GetLayerVersionRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
     },
 )
@@ -967,14 +1036,15 @@
     {
         "Location": str,
         "CodeSha256": str,
         "CodeSize": int,
         "SigningProfileVersionArn": str,
         "SigningJobArn": str,
     },
+    total=False,
 )
 
 _RequiredGetPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetPolicyRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
@@ -988,22 +1058,44 @@
 )
 
 class GetPolicyRequestRequestTypeDef(
     _RequiredGetPolicyRequestRequestTypeDef, _OptionalGetPolicyRequestRequestTypeDef
 ):
     pass
 
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetProvisionedConcurrencyConfigRequestRequestTypeDef = TypedDict(
     "GetProvisionedConcurrencyConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Qualifier": str,
     },
 )
 
+GetProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
+    "GetProvisionedConcurrencyConfigResponseTypeDef",
+    {
+        "RequestedProvisionedConcurrentExecutions": int,
+        "AvailableProvisionedConcurrentExecutions": int,
+        "AllocatedProvisionedConcurrentExecutions": int,
+        "Status": ProvisionedConcurrencyStatusEnumType,
+        "StatusReason": str,
+        "LastModified": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetRuntimeManagementConfigRequestRequestTypeDef = TypedDict(
     "_RequiredGetRuntimeManagementConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalGetRuntimeManagementConfigRequestRequestTypeDef = TypedDict(
@@ -1016,29 +1108,41 @@
 
 class GetRuntimeManagementConfigRequestRequestTypeDef(
     _RequiredGetRuntimeManagementConfigRequestRequestTypeDef,
     _OptionalGetRuntimeManagementConfigRequestRequestTypeDef,
 ):
     pass
 
+GetRuntimeManagementConfigResponseTypeDef = TypedDict(
+    "GetRuntimeManagementConfigResponseTypeDef",
+    {
+        "UpdateRuntimeOn": UpdateRuntimeOnType,
+        "RuntimeVersionArn": str,
+        "FunctionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ImageConfigErrorTypeDef = TypedDict(
     "ImageConfigErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
+    total=False,
 )
 
 ImageConfigOutputTypeDef = TypedDict(
     "ImageConfigOutputTypeDef",
     {
         "EntryPoint": List[str],
         "Command": List[str],
         "WorkingDirectory": str,
     },
+    total=False,
 )
 
 _RequiredInvocationRequestRequestTypeDef = TypedDict(
     "_RequiredInvocationRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
@@ -1056,36 +1160,58 @@
 )
 
 class InvocationRequestRequestTypeDef(
     _RequiredInvocationRequestRequestTypeDef, _OptionalInvocationRequestRequestTypeDef
 ):
     pass
 
+InvocationResponseTypeDef = TypedDict(
+    "InvocationResponseTypeDef",
+    {
+        "StatusCode": int,
+        "FunctionError": str,
+        "LogResult": str,
+        "Payload": StreamingBody,
+        "ExecutedVersion": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InvokeAsyncRequestRequestTypeDef = TypedDict(
     "InvokeAsyncRequestRequestTypeDef",
     {
         "FunctionName": str,
         "InvokeArgs": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
+InvokeAsyncResponseTypeDef = TypedDict(
+    "InvokeAsyncResponseTypeDef",
+    {
+        "Status": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 InvokeResponseStreamUpdateTypeDef = TypedDict(
     "InvokeResponseStreamUpdateTypeDef",
     {
         "Payload": bytes,
     },
+    total=False,
 )
 
 InvokeWithResponseStreamCompleteEventTypeDef = TypedDict(
     "InvokeWithResponseStreamCompleteEventTypeDef",
     {
         "ErrorCode": str,
         "ErrorDetails": str,
         "LogResult": str,
     },
+    total=False,
 )
 
 _RequiredInvokeWithResponseStreamRequestRequestTypeDef = TypedDict(
     "_RequiredInvokeWithResponseStreamRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
@@ -1126,26 +1252,38 @@
         "Version": int,
         "Description": str,
         "CreatedDate": str,
         "CompatibleRuntimes": List[RuntimeType],
         "LicenseInfo": str,
         "CompatibleArchitectures": List[ArchitectureType],
     },
+    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "FunctionName": str,
+    },
+)
+_OptionalListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "FunctionVersion": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListAliasesRequestListAliasesPaginateTypeDef(
+    _RequiredListAliasesRequestListAliasesPaginateTypeDef,
+    _OptionalListAliasesRequestListAliasesPaginateTypeDef,
+):
+    pass
+
 _RequiredListAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredListAliasesRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListAliasesRequestRequestTypeDef = TypedDict(
@@ -1159,34 +1297,72 @@
 )
 
 class ListAliasesRequestRequestTypeDef(
     _RequiredListAliasesRequestRequestTypeDef, _OptionalListAliasesRequestRequestTypeDef
 ):
     pass
 
+ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef = TypedDict(
+    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListCodeSigningConfigsRequestRequestTypeDef = TypedDict(
     "ListCodeSigningConfigsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef = TypedDict(
+    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
+    {
+        "EventSourceArn": str,
+        "FunctionName": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListEventSourceMappingsRequestRequestTypeDef = TypedDict(
     "ListEventSourceMappingsRequestRequestTypeDef",
     {
         "EventSourceArn": str,
         "FunctionName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef(
+    _RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
+    _OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
+):
+    pass
+
 _RequiredListFunctionEventInvokeConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionEventInvokeConfigsRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListFunctionEventInvokeConfigsRequestRequestTypeDef = TypedDict(
@@ -1200,14 +1376,34 @@
 
 class ListFunctionEventInvokeConfigsRequestRequestTypeDef(
     _RequiredListFunctionEventInvokeConfigsRequestRequestTypeDef,
     _OptionalListFunctionEventInvokeConfigsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef(
+    _RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
+    _OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
+):
+    pass
+
 _RequiredListFunctionUrlConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionUrlConfigsRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListFunctionUrlConfigsRequestRequestTypeDef = TypedDict(
@@ -1221,14 +1417,34 @@
 
 class ListFunctionUrlConfigsRequestRequestTypeDef(
     _RequiredListFunctionUrlConfigsRequestRequestTypeDef,
     _OptionalListFunctionUrlConfigsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
+    {
+        "CodeSigningConfigArn": str,
+    },
+)
+_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef(
+    _RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
+    _OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
+):
+    pass
+
 _RequiredListFunctionsByCodeSigningConfigRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionsByCodeSigningConfigRequestRequestTypeDef",
     {
         "CodeSigningConfigArn": str,
     },
 )
 _OptionalListFunctionsByCodeSigningConfigRequestRequestTypeDef = TypedDict(
@@ -1242,25 +1458,66 @@
 
 class ListFunctionsByCodeSigningConfigRequestRequestTypeDef(
     _RequiredListFunctionsByCodeSigningConfigRequestRequestTypeDef,
     _OptionalListFunctionsByCodeSigningConfigRequestRequestTypeDef,
 ):
     pass
 
+ListFunctionsByCodeSigningConfigResponseTypeDef = TypedDict(
+    "ListFunctionsByCodeSigningConfigResponseTypeDef",
+    {
+        "NextMarker": str,
+        "FunctionArns": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
+    "ListFunctionsRequestListFunctionsPaginateTypeDef",
+    {
+        "MasterRegion": str,
+        "FunctionVersion": Literal["ALL"],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListFunctionsRequestRequestTypeDef = TypedDict(
     "ListFunctionsRequestRequestTypeDef",
     {
         "MasterRegion": str,
         "FunctionVersion": Literal["ALL"],
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
+_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
+    {
+        "LayerName": str,
+    },
+)
+_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
+    {
+        "CompatibleRuntime": RuntimeType,
+        "CompatibleArchitecture": ArchitectureType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListLayerVersionsRequestListLayerVersionsPaginateTypeDef(
+    _RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
+    _OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
+):
+    pass
+
 _RequiredListLayerVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLayerVersionsRequestRequestTypeDef",
     {
         "LayerName": str,
     },
 )
 _OptionalListLayerVersionsRequestRequestTypeDef = TypedDict(
@@ -1275,25 +1532,55 @@
 )
 
 class ListLayerVersionsRequestRequestTypeDef(
     _RequiredListLayerVersionsRequestRequestTypeDef, _OptionalListLayerVersionsRequestRequestTypeDef
 ):
     pass
 
+ListLayersRequestListLayersPaginateTypeDef = TypedDict(
+    "ListLayersRequestListLayersPaginateTypeDef",
+    {
+        "CompatibleRuntime": RuntimeType,
+        "CompatibleArchitecture": ArchitectureType,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListLayersRequestRequestTypeDef = TypedDict(
     "ListLayersRequestRequestTypeDef",
     {
         "CompatibleRuntime": RuntimeType,
         "Marker": str,
         "MaxItems": int,
         "CompatibleArchitecture": ArchitectureType,
     },
     total=False,
 )
 
+_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef(
+    _RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
+    _OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
+):
+    pass
+
 _RequiredListProvisionedConcurrencyConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListProvisionedConcurrencyConfigsRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListProvisionedConcurrencyConfigsRequestRequestTypeDef = TypedDict(
@@ -1318,23 +1605,52 @@
         "RequestedProvisionedConcurrentExecutions": int,
         "AvailableProvisionedConcurrentExecutions": int,
         "AllocatedProvisionedConcurrentExecutions": int,
         "Status": ProvisionedConcurrencyStatusEnumType,
         "StatusReason": str,
         "LastModified": str,
     },
+    total=False,
 )
 
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "Resource": str,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
+    "_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
+    "_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef(
+    _RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
+    _OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
+):
+    pass
+
 _RequiredListVersionsByFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredListVersionsByFunctionRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListVersionsByFunctionRequestRequestTypeDef = TypedDict(
@@ -1348,14 +1664,24 @@
 
 class ListVersionsByFunctionRequestRequestTypeDef(
     _RequiredListVersionsByFunctionRequestRequestTypeDef,
     _OptionalListVersionsByFunctionRequestRequestTypeDef,
 ):
     pass
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 _RequiredPublishVersionRequestRequestTypeDef = TypedDict(
     "_RequiredPublishVersionRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalPublishVersionRequestRequestTypeDef = TypedDict(
@@ -1377,14 +1703,23 @@
     "PutFunctionCodeSigningConfigRequestRequestTypeDef",
     {
         "CodeSigningConfigArn": str,
         "FunctionName": str,
     },
 )
 
+PutFunctionCodeSigningConfigResponseTypeDef = TypedDict(
+    "PutFunctionCodeSigningConfigResponseTypeDef",
+    {
+        "CodeSigningConfigArn": str,
+        "FunctionName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutFunctionConcurrencyRequestRequestTypeDef = TypedDict(
     "PutFunctionConcurrencyRequestRequestTypeDef",
     {
         "FunctionName": str,
         "ReservedConcurrentExecutions": int,
     },
 )
@@ -1394,14 +1729,27 @@
     {
         "FunctionName": str,
         "Qualifier": str,
         "ProvisionedConcurrentExecutions": int,
     },
 )
 
+PutProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
+    "PutProvisionedConcurrencyConfigResponseTypeDef",
+    {
+        "RequestedProvisionedConcurrentExecutions": int,
+        "AvailableProvisionedConcurrentExecutions": int,
+        "AllocatedProvisionedConcurrentExecutions": int,
+        "Status": ProvisionedConcurrencyStatusEnumType,
+        "StatusReason": str,
+        "LastModified": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutRuntimeManagementConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuntimeManagementConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
         "UpdateRuntimeOn": UpdateRuntimeOnType,
     },
 )
@@ -1416,14 +1764,24 @@
 
 class PutRuntimeManagementConfigRequestRequestTypeDef(
     _RequiredPutRuntimeManagementConfigRequestRequestTypeDef,
     _OptionalPutRuntimeManagementConfigRequestRequestTypeDef,
 ):
     pass
 
+PutRuntimeManagementConfigResponseTypeDef = TypedDict(
+    "PutRuntimeManagementConfigResponseTypeDef",
+    {
+        "UpdateRuntimeOn": UpdateRuntimeOnType,
+        "FunctionArn": str,
+        "RuntimeVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredRemoveLayerVersionPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLayerVersionPermissionRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
         "StatementId": str,
     },
@@ -1459,20 +1817,32 @@
 )
 
 class RemovePermissionRequestRequestTypeDef(
     _RequiredRemovePermissionRequestRequestTypeDef, _OptionalRemovePermissionRequestRequestTypeDef
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
 RuntimeVersionErrorTypeDef = TypedDict(
     "RuntimeVersionErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
+    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "Tags": Mapping[str, str],
@@ -1511,205 +1881,47 @@
 
 class UpdateFunctionCodeRequestRequestTypeDef(
     _RequiredUpdateFunctionCodeRequestRequestTypeDef,
     _OptionalUpdateFunctionCodeRequestRequestTypeDef,
 ):
     pass
 
-AddLayerVersionPermissionResponseTypeDef = TypedDict(
-    "AddLayerVersionPermissionResponseTypeDef",
-    {
-        "Statement": str,
-        "RevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AddPermissionResponseTypeDef = TypedDict(
-    "AddPermissionResponseTypeDef",
-    {
-        "Statement": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ConcurrencyResponseMetadataTypeDef = TypedDict(
-    "ConcurrencyResponseMetadataTypeDef",
-    {
-        "ReservedConcurrentExecutions": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetAccountSettingsResponseTypeDef = TypedDict(
     "GetAccountSettingsResponseTypeDef",
     {
         "AccountLimit": AccountLimitTypeDef,
         "AccountUsage": AccountUsageTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetFunctionCodeSigningConfigResponseTypeDef = TypedDict(
-    "GetFunctionCodeSigningConfigResponseTypeDef",
-    {
-        "CodeSigningConfigArn": str,
-        "FunctionName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetFunctionConcurrencyResponseTypeDef = TypedDict(
-    "GetFunctionConcurrencyResponseTypeDef",
-    {
-        "ReservedConcurrentExecutions": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetLayerVersionPolicyResponseTypeDef = TypedDict(
-    "GetLayerVersionPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
-    "GetProvisionedConcurrencyConfigResponseTypeDef",
-    {
-        "RequestedProvisionedConcurrentExecutions": int,
-        "AvailableProvisionedConcurrentExecutions": int,
-        "AllocatedProvisionedConcurrentExecutions": int,
-        "Status": ProvisionedConcurrencyStatusEnumType,
-        "StatusReason": str,
-        "LastModified": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetRuntimeManagementConfigResponseTypeDef = TypedDict(
-    "GetRuntimeManagementConfigResponseTypeDef",
-    {
-        "UpdateRuntimeOn": UpdateRuntimeOnType,
-        "RuntimeVersionArn": str,
-        "FunctionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InvocationResponseTypeDef = TypedDict(
-    "InvocationResponseTypeDef",
-    {
-        "StatusCode": int,
-        "FunctionError": str,
-        "LogResult": str,
-        "Payload": StreamingBody,
-        "ExecutedVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-InvokeAsyncResponseTypeDef = TypedDict(
-    "InvokeAsyncResponseTypeDef",
-    {
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListFunctionsByCodeSigningConfigResponseTypeDef = TypedDict(
-    "ListFunctionsByCodeSigningConfigResponseTypeDef",
-    {
-        "NextMarker": str,
-        "FunctionArns": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutFunctionCodeSigningConfigResponseTypeDef = TypedDict(
-    "PutFunctionCodeSigningConfigResponseTypeDef",
-    {
-        "CodeSigningConfigArn": str,
-        "FunctionName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
-    "PutProvisionedConcurrencyConfigResponseTypeDef",
-    {
-        "RequestedProvisionedConcurrentExecutions": int,
-        "AvailableProvisionedConcurrentExecutions": int,
-        "AllocatedProvisionedConcurrentExecutions": int,
-        "Status": ProvisionedConcurrencyStatusEnumType,
-        "StatusReason": str,
-        "LastModified": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutRuntimeManagementConfigResponseTypeDef = TypedDict(
-    "PutRuntimeManagementConfigResponseTypeDef",
-    {
-        "UpdateRuntimeOn": UpdateRuntimeOnType,
-        "FunctionArn": str,
-        "RuntimeVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AliasConfigurationResponseMetadataTypeDef = TypedDict(
     "AliasConfigurationResponseMetadataTypeDef",
     {
         "AliasArn": str,
         "Name": str,
         "FunctionVersion": str,
         "Description": str,
         "RoutingConfig": AliasRoutingConfigurationOutputTypeDef,
         "RevisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AliasConfigurationTypeDef = TypedDict(
     "AliasConfigurationTypeDef",
     {
         "AliasArn": str,
         "Name": str,
         "FunctionVersion": str,
         "Description": str,
         "RoutingConfig": AliasRoutingConfigurationOutputTypeDef,
         "RevisionId": str,
     },
+    total=False,
 )
 
 _RequiredCreateAliasRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAliasRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Name": str,
@@ -1749,25 +1961,36 @@
 )
 
 class UpdateAliasRequestRequestTypeDef(
     _RequiredUpdateAliasRequestRequestTypeDef, _OptionalUpdateAliasRequestRequestTypeDef
 ):
     pass
 
-CodeSigningConfigTypeDef = TypedDict(
-    "CodeSigningConfigTypeDef",
+_RequiredCodeSigningConfigTypeDef = TypedDict(
+    "_RequiredCodeSigningConfigTypeDef",
     {
         "CodeSigningConfigId": str,
         "CodeSigningConfigArn": str,
-        "Description": str,
         "AllowedPublishers": AllowedPublishersOutputTypeDef,
         "CodeSigningPolicies": CodeSigningPoliciesOutputTypeDef,
         "LastModified": str,
     },
 )
+_OptionalCodeSigningConfigTypeDef = TypedDict(
+    "_OptionalCodeSigningConfigTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class CodeSigningConfigTypeDef(
+    _RequiredCodeSigningConfigTypeDef, _OptionalCodeSigningConfigTypeDef
+):
+    pass
 
 _RequiredCreateCodeSigningConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCodeSigningConfigRequestRequestTypeDef",
     {
         "AllowedPublishers": AllowedPublishersTypeDef,
     },
 )
@@ -1813,56 +2036,67 @@
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
         "Cors": CorsOutputTypeDef,
         "CreationTime": str,
         "InvokeMode": InvokeModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-FunctionUrlConfigTypeDef = TypedDict(
-    "FunctionUrlConfigTypeDef",
+_RequiredFunctionUrlConfigTypeDef = TypedDict(
+    "_RequiredFunctionUrlConfigTypeDef",
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "CreationTime": str,
         "LastModifiedTime": str,
-        "Cors": CorsOutputTypeDef,
         "AuthType": FunctionUrlAuthTypeType,
+    },
+)
+_OptionalFunctionUrlConfigTypeDef = TypedDict(
+    "_OptionalFunctionUrlConfigTypeDef",
+    {
+        "Cors": CorsOutputTypeDef,
         "InvokeMode": InvokeModeType,
     },
+    total=False,
 )
 
+class FunctionUrlConfigTypeDef(
+    _RequiredFunctionUrlConfigTypeDef, _OptionalFunctionUrlConfigTypeDef
+):
+    pass
+
 GetFunctionUrlConfigResponseTypeDef = TypedDict(
     "GetFunctionUrlConfigResponseTypeDef",
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
         "Cors": CorsOutputTypeDef,
         "CreationTime": str,
         "LastModifiedTime": str,
         "InvokeMode": InvokeModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateFunctionUrlConfigResponseTypeDef = TypedDict(
     "UpdateFunctionUrlConfigResponseTypeDef",
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
         "Cors": CorsOutputTypeDef,
         "CreationTime": str,
         "LastModifiedTime": str,
         "InvokeMode": InvokeModeType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFunctionUrlConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
@@ -1986,14 +2220,15 @@
 
 DestinationConfigOutputTypeDef = TypedDict(
     "DestinationConfigOutputTypeDef",
     {
         "OnSuccess": OnSuccessOutputTypeDef,
         "OnFailure": OnFailureOutputTypeDef,
     },
+    total=False,
 )
 
 DestinationConfigTypeDef = TypedDict(
     "DestinationConfigTypeDef",
     {
         "OnSuccess": OnSuccessTypeDef,
         "OnFailure": OnFailureTypeDef,
@@ -2003,21 +2238,23 @@
 
 EnvironmentResponseTypeDef = TypedDict(
     "EnvironmentResponseTypeDef",
     {
         "Variables": Dict[str, str],
         "Error": EnvironmentErrorTypeDef,
     },
+    total=False,
 )
 
 FilterCriteriaOutputTypeDef = TypedDict(
     "FilterCriteriaOutputTypeDef",
     {
         "Filters": List[FilterOutputTypeDef],
     },
+    total=False,
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
     },
@@ -2158,15 +2395,15 @@
         "LayerVersionArn": str,
         "Description": str,
         "CreatedDate": str,
         "Version": int,
         "CompatibleRuntimes": List[RuntimeType],
         "LicenseInfo": str,
         "CompatibleArchitectures": List[ArchitectureType],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PublishLayerVersionResponseTypeDef = TypedDict(
     "PublishLayerVersionResponseTypeDef",
     {
         "Content": LayerVersionContentOutputTypeDef,
@@ -2174,32 +2411,34 @@
         "LayerVersionArn": str,
         "Description": str,
         "CreatedDate": str,
         "Version": int,
         "CompatibleRuntimes": List[RuntimeType],
         "LicenseInfo": str,
         "CompatibleArchitectures": List[ArchitectureType],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImageConfigResponseTypeDef = TypedDict(
     "ImageConfigResponseTypeDef",
     {
         "ImageConfig": ImageConfigOutputTypeDef,
         "Error": ImageConfigErrorTypeDef,
     },
+    total=False,
 )
 
 InvokeWithResponseStreamResponseEventTypeDef = TypedDict(
     "InvokeWithResponseStreamResponseEventTypeDef",
     {
         "PayloadChunk": InvokeResponseStreamUpdateTypeDef,
         "InvokeComplete": InvokeWithResponseStreamCompleteEventTypeDef,
     },
+    total=False,
 )
 
 _RequiredPublishLayerVersionRequestRequestTypeDef = TypedDict(
     "_RequiredPublishLayerVersionRequestRequestTypeDef",
     {
         "LayerName": str,
         "Content": LayerVersionContentInputTypeDef,
@@ -2225,295 +2464,117 @@
 LayersListItemTypeDef = TypedDict(
     "LayersListItemTypeDef",
     {
         "LayerName": str,
         "LayerArn": str,
         "LatestMatchingVersion": LayerVersionsListItemTypeDef,
     },
+    total=False,
 )
 
 ListLayerVersionsResponseTypeDef = TypedDict(
     "ListLayerVersionsResponseTypeDef",
     {
         "NextMarker": str,
         "LayerVersions": List[LayerVersionsListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
-    {
-        "FunctionVersion": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListAliasesRequestListAliasesPaginateTypeDef(
-    _RequiredListAliasesRequestListAliasesPaginateTypeDef,
-    _OptionalListAliasesRequestListAliasesPaginateTypeDef,
-):
-    pass
-
-ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef = TypedDict(
-    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef = TypedDict(
-    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
-    {
-        "EventSourceArn": str,
-        "FunctionName": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef(
-    _RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
-    _OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
-):
-    pass
-
-_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef(
-    _RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
-    _OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
-):
-    pass
-
-_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
-    {
-        "CodeSigningConfigArn": str,
-    },
-)
-_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef(
-    _RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
-    _OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
-):
-    pass
-
-ListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
-    "ListFunctionsRequestListFunctionsPaginateTypeDef",
-    {
-        "MasterRegion": str,
-        "FunctionVersion": Literal["ALL"],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
-    {
-        "LayerName": str,
-    },
-)
-_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
-    {
-        "CompatibleRuntime": RuntimeType,
-        "CompatibleArchitecture": ArchitectureType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListLayerVersionsRequestListLayerVersionsPaginateTypeDef(
-    _RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
-    _OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
-):
-    pass
-
-ListLayersRequestListLayersPaginateTypeDef = TypedDict(
-    "ListLayersRequestListLayersPaginateTypeDef",
-    {
-        "CompatibleRuntime": RuntimeType,
-        "CompatibleArchitecture": ArchitectureType,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef(
-    _RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
-    _OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
-):
-    pass
-
-_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
-    "_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
-    "_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef(
-    _RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
-    _OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
-):
-    pass
-
 ListProvisionedConcurrencyConfigsResponseTypeDef = TypedDict(
     "ListProvisionedConcurrencyConfigsResponseTypeDef",
     {
         "ProvisionedConcurrencyConfigs": List[ProvisionedConcurrencyConfigListItemTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RuntimeVersionConfigTypeDef = TypedDict(
     "RuntimeVersionConfigTypeDef",
     {
         "RuntimeVersionArn": str,
         "Error": RuntimeVersionErrorTypeDef,
     },
+    total=False,
 )
 
 ListAliasesResponseTypeDef = TypedDict(
     "ListAliasesResponseTypeDef",
     {
         "NextMarker": str,
         "Aliases": List[AliasConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCodeSigningConfigResponseTypeDef = TypedDict(
     "CreateCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCodeSigningConfigResponseTypeDef = TypedDict(
     "GetCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCodeSigningConfigsResponseTypeDef = TypedDict(
     "ListCodeSigningConfigsResponseTypeDef",
     {
         "NextMarker": str,
         "CodeSigningConfigs": List[CodeSigningConfigTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCodeSigningConfigResponseTypeDef = TypedDict(
     "UpdateCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFunctionUrlConfigsResponseTypeDef = TypedDict(
     "ListFunctionUrlConfigsResponseTypeDef",
     {
         "FunctionUrlConfigs": List[FunctionUrlConfigTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionEventInvokeConfigResponseMetadataTypeDef = TypedDict(
     "FunctionEventInvokeConfigResponseMetadataTypeDef",
     {
         "LastModified": datetime,
         "FunctionArn": str,
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
         "DestinationConfig": DestinationConfigOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionEventInvokeConfigTypeDef = TypedDict(
     "FunctionEventInvokeConfigTypeDef",
     {
         "LastModified": datetime,
         "FunctionArn": str,
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
         "DestinationConfig": DestinationConfigOutputTypeDef,
     },
+    total=False,
 )
 
 _RequiredPutFunctionEventInvokeConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutFunctionEventInvokeConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
@@ -2584,15 +2645,15 @@
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigOutputTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigOutputTypeDef,
         "ScalingConfig": ScalingConfigOutputTypeDef,
         "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventSourceMappingConfigurationTypeDef = TypedDict(
     "EventSourceMappingConfigurationTypeDef",
     {
         "UUID": str,
@@ -2619,14 +2680,15 @@
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
         "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigOutputTypeDef,
         "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigOutputTypeDef,
         "ScalingConfig": ScalingConfigOutputTypeDef,
         "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigOutputTypeDef,
     },
+    total=False,
 )
 
 _RequiredCreateEventSourceMappingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventSourceMappingRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
@@ -2703,24 +2765,24 @@
 InvokeWithResponseStreamResponseTypeDef = TypedDict(
     "InvokeWithResponseStreamResponseTypeDef",
     {
         "StatusCode": int,
         "ExecutedVersion": str,
         "EventStream": "EventStream[InvokeWithResponseStreamResponseEventTypeDef]",
         "ResponseStreamContentType": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLayersResponseTypeDef = TypedDict(
     "ListLayersResponseTypeDef",
     {
         "NextMarker": str,
         "Layers": List[LayersListItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionConfigurationResponseMetadataTypeDef = TypedDict(
     "FunctionConfigurationResponseMetadataTypeDef",
     {
         "FunctionName": str,
@@ -2754,15 +2816,15 @@
         "ImageConfigResponse": ImageConfigResponseTypeDef,
         "SigningProfileVersionArn": str,
         "SigningJobArn": str,
         "Architectures": List[ArchitectureType],
         "EphemeralStorage": EphemeralStorageOutputTypeDef,
         "SnapStart": SnapStartResponseTypeDef,
         "RuntimeVersionConfig": RuntimeVersionConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 FunctionConfigurationTypeDef = TypedDict(
     "FunctionConfigurationTypeDef",
     {
         "FunctionName": str,
@@ -2797,55 +2859,56 @@
         "SigningProfileVersionArn": str,
         "SigningJobArn": str,
         "Architectures": List[ArchitectureType],
         "EphemeralStorage": EphemeralStorageOutputTypeDef,
         "SnapStart": SnapStartResponseTypeDef,
         "RuntimeVersionConfig": RuntimeVersionConfigTypeDef,
     },
+    total=False,
 )
 
 ListFunctionEventInvokeConfigsResponseTypeDef = TypedDict(
     "ListFunctionEventInvokeConfigsResponseTypeDef",
     {
         "FunctionEventInvokeConfigs": List[FunctionEventInvokeConfigTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventSourceMappingsResponseTypeDef = TypedDict(
     "ListEventSourceMappingsResponseTypeDef",
     {
         "NextMarker": str,
         "EventSourceMappings": List[EventSourceMappingConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetFunctionResponseTypeDef = TypedDict(
     "GetFunctionResponseTypeDef",
     {
         "Configuration": FunctionConfigurationTypeDef,
         "Code": FunctionCodeLocationTypeDef,
         "Tags": Dict[str, str],
         "Concurrency": ConcurrencyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListFunctionsResponseTypeDef = TypedDict(
     "ListFunctionsResponseTypeDef",
     {
         "NextMarker": str,
         "Functions": List[FunctionConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListVersionsByFunctionResponseTypeDef = TypedDict(
     "ListVersionsByFunctionResponseTypeDef",
     {
         "NextMarker": str,
         "Versions": List[FunctionConfigurationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/waiter.py` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda/waiter.pyi` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda.egg-info/PKG-INFO` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lambda
-Version: 1.28.11
-Summary: Type annotations for boto3.Lambda 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.Lambda 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lambda"></a>
 
 # mypy-boto3-lambda
 
 [![PyPI - mypy-boto3-lambda](https://img.shields.io/pypi/v/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lambda?color=blue)](https://pypistats.org/packages/mypy-boto3-lambda)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lambda)](https://pepy.tech/project/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
 
@@ -461,24 +461,26 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lambda.type_defs import (
     AccountLimitTypeDef,
     AccountUsageTypeDef,
     AddLayerVersionPermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddLayerVersionPermissionResponseTypeDef,
     AddPermissionRequestRequestTypeDef,
+    AddPermissionResponseTypeDef,
     AliasRoutingConfigurationOutputTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersOutputTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigOutputTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
     CodeSigningPoliciesOutputTypeDef,
     CodeSigningPoliciesTypeDef,
+    ConcurrencyResponseMetadataTypeDef,
     ConcurrencyTypeDef,
     CorsOutputTypeDef,
     CorsTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     ScalingConfigTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
@@ -504,14 +506,15 @@
     DeleteLayerVersionRequestRequestTypeDef,
     DeleteProvisionedConcurrencyConfigRequestRequestTypeDef,
     OnFailureOutputTypeDef,
     OnSuccessOutputTypeDef,
     OnFailureTypeDef,
     OnSuccessTypeDef,
     DocumentDBEventSourceConfigOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnvironmentErrorTypeDef,
     EphemeralStorageOutputTypeDef,
     ScalingConfigOutputTypeDef,
     SelfManagedEventSourceOutputTypeDef,
     SelfManagedKafkaEventSourceConfigOutputTypeDef,
     SourceAccessConfigurationOutputTypeDef,
     FileSystemConfigOutputTypeDef,
@@ -522,79 +525,87 @@
     SnapStartResponseTypeDef,
     TracingConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
     GetAliasRequestRequestTypeDef,
     GetCodeSigningConfigRequestRequestTypeDef,
     GetEventSourceMappingRequestRequestTypeDef,
     GetFunctionCodeSigningConfigRequestRequestTypeDef,
+    GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyRequestRequestTypeDef,
+    GetFunctionConcurrencyResponseTypeDef,
     WaiterConfigTypeDef,
     GetFunctionConfigurationRequestRequestTypeDef,
     GetFunctionEventInvokeConfigRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetFunctionUrlConfigRequestRequestTypeDef,
     GetLayerVersionByArnRequestRequestTypeDef,
     GetLayerVersionPolicyRequestRequestTypeDef,
+    GetLayerVersionPolicyResponseTypeDef,
     GetLayerVersionRequestRequestTypeDef,
     LayerVersionContentOutputTypeDef,
     GetPolicyRequestRequestTypeDef,
+    GetPolicyResponseTypeDef,
     GetProvisionedConcurrencyConfigRequestRequestTypeDef,
+    GetProvisionedConcurrencyConfigResponseTypeDef,
     GetRuntimeManagementConfigRequestRequestTypeDef,
+    GetRuntimeManagementConfigResponseTypeDef,
     ImageConfigErrorTypeDef,
     ImageConfigOutputTypeDef,
     InvocationRequestRequestTypeDef,
+    InvocationResponseTypeDef,
     InvokeAsyncRequestRequestTypeDef,
+    InvokeAsyncResponseTypeDef,
     InvokeResponseStreamUpdateTypeDef,
     InvokeWithResponseStreamCompleteEventTypeDef,
     InvokeWithResponseStreamRequestRequestTypeDef,
     LayerVersionContentInputTypeDef,
     LayerVersionsListItemTypeDef,
-    PaginatorConfigTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
     ListAliasesRequestRequestTypeDef,
+    ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
     ListCodeSigningConfigsRequestRequestTypeDef,
+    ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
     ListEventSourceMappingsRequestRequestTypeDef,
+    ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
     ListFunctionEventInvokeConfigsRequestRequestTypeDef,
+    ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
     ListFunctionUrlConfigsRequestRequestTypeDef,
+    ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
     ListFunctionsByCodeSigningConfigRequestRequestTypeDef,
+    ListFunctionsByCodeSigningConfigResponseTypeDef,
+    ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListFunctionsRequestRequestTypeDef,
+    ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
     ListLayerVersionsRequestRequestTypeDef,
+    ListLayersRequestListLayersPaginateTypeDef,
     ListLayersRequestRequestTypeDef,
+    ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
     ListProvisionedConcurrencyConfigsRequestRequestTypeDef,
     ProvisionedConcurrencyConfigListItemTypeDef,
     ListTagsRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
+    ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListVersionsByFunctionRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     PublishVersionRequestRequestTypeDef,
     PutFunctionCodeSigningConfigRequestRequestTypeDef,
+    PutFunctionCodeSigningConfigResponseTypeDef,
     PutFunctionConcurrencyRequestRequestTypeDef,
     PutProvisionedConcurrencyConfigRequestRequestTypeDef,
+    PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigRequestRequestTypeDef,
+    PutRuntimeManagementConfigResponseTypeDef,
     RemoveLayerVersionPermissionRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     RuntimeVersionErrorTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFunctionCodeRequestRequestTypeDef,
-    AddLayerVersionPermissionResponseTypeDef,
-    AddPermissionResponseTypeDef,
-    ConcurrencyResponseMetadataTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetAccountSettingsResponseTypeDef,
-    GetFunctionCodeSigningConfigResponseTypeDef,
-    GetFunctionConcurrencyResponseTypeDef,
-    GetLayerVersionPolicyResponseTypeDef,
-    GetPolicyResponseTypeDef,
-    GetProvisionedConcurrencyConfigResponseTypeDef,
-    GetRuntimeManagementConfigResponseTypeDef,
-    InvocationResponseTypeDef,
-    InvokeAsyncResponseTypeDef,
-    ListFunctionsByCodeSigningConfigResponseTypeDef,
-    ListTagsResponseTypeDef,
-    PutFunctionCodeSigningConfigResponseTypeDef,
-    PutProvisionedConcurrencyConfigResponseTypeDef,
-    PutRuntimeManagementConfigResponseTypeDef,
     AliasConfigurationResponseMetadataTypeDef,
     AliasConfigurationTypeDef,
     CreateAliasRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     CodeSigningConfigTypeDef,
     CreateCodeSigningConfigRequestRequestTypeDef,
     UpdateCodeSigningConfigRequestRequestTypeDef,
@@ -620,25 +631,14 @@
     GetLayerVersionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     ImageConfigResponseTypeDef,
     InvokeWithResponseStreamResponseEventTypeDef,
     PublishLayerVersionRequestRequestTypeDef,
     LayersListItemTypeDef,
     ListLayerVersionsResponseTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
-    ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
-    ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
-    ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
-    ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
-    ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
-    ListFunctionsRequestListFunctionsPaginateTypeDef,
-    ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
-    ListLayersRequestListLayersPaginateTypeDef,
-    ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
-    ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListProvisionedConcurrencyConfigsResponseTypeDef,
     RuntimeVersionConfigTypeDef,
     ListAliasesResponseTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
```

### Comparing `mypy-boto3-lambda-1.28.11/mypy_boto3_lambda.egg-info/SOURCES.txt` & `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.11/setup.py` & `mypy-boto3-lambda-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lambda",
-    version="1.28.11",
+    version="1.28.12",
     packages=["mypy_boto3_lambda"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Lambda 1.28.11 service generated with mypy-boto3-builder 7.15.1"
+        "Type annotations for boto3.Lambda 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

