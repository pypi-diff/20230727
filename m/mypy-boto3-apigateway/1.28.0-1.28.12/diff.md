# Comparing `tmp/mypy-boto3-apigateway-1.28.0.tar.gz` & `tmp/mypy-boto3-apigateway-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apigateway-1.28.0.tar", last modified: Thu Jul  6 20:58:55 2023, max compression
+gzip compressed data, was "mypy-boto3-apigateway-1.28.12.tar", last modified: Thu Jul 27 05:34:16 2023, max compression
```

## Comparing `mypy-boto3-apigateway-1.28.0.tar` & `mypy-boto3-apigateway-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.370214 mypy-boto3-apigateway-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:32:55.000000 mypy-boto3-apigateway-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24739 2023-07-06 20:58:55.366214 mypy-boto3-apigateway-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23242 2023-07-06 20:32:55.000000 mypy-boto3-apigateway-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.362214 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-06 20:32:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-06 20:32:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:32:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83079 2023-07-06 20:32:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    82934 2023-07-06 20:32:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-07-06 20:32:56.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-07-06 20:32:56.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-07-06 20:32:56.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-07-06 20:32:56.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    93118 2023-07-06 20:32:59.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    92969 2023-07-06 20:32:58.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:32:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.366214 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24739 2023-07-06 20:58:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 20:58:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:58:55.000000 mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:55.370214 mypy-boto3-apigateway-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:32:54.000000 mypy-boto3-apigateway-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.380583 mypy-boto3-apigateway-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:08.000000 mypy-boto3-apigateway-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24965 2023-07-27 05:34:16.380583 mypy-boto3-apigateway-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23466 2023-07-27 05:17:08.000000 mypy-boto3-apigateway-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.380583 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-27 05:17:08.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-27 05:17:08.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:17:08.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83079 2023-07-27 05:17:09.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82934 2023-07-27 05:17:08.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-07-27 05:17:09.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-27 05:17:09.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-07-27 05:17:09.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-07-27 05:17:09.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:08.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    95206 2023-07-27 05:17:11.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95055 2023-07-27 05:17:10.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:08.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.380583 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24965 2023-07-27 05:34:16.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:16.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:16.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:16.000000 mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:16.380583 mypy-boto3-apigateway-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:17:08.000000 mypy-boto3-apigateway-1.28.12/setup.py
```

### Comparing `mypy-boto3-apigateway-1.28.0/LICENSE` & `mypy-boto3-apigateway-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.0/PKG-INFO` & `mypy-boto3-apigateway-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigateway
-Version: 1.28.0
-Summary: Type annotations for boto3.APIGateway 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.APIGateway 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-apigateway"></a>
 
 # mypy-boto3-apigateway
 
 [![PyPI - mypy-boto3-apigateway](https://img.shields.io/pypi/v/mypy-boto3-apigateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apigateway?color=blue)](https://pypistats.org/packages/mypy-boto3-apigateway)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigateway)](https://pepy.tech/project/mypy-boto3-apigateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.APIGateway 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
+[boto3.APIGateway 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
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
 [mypy-boto3-apigateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -405,22 +405,24 @@
 
 `mypy_boto3_apigateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigateway.type_defs import (
     AccessLogSettingsTypeDef,
-    ThrottleSettingsTypeDef,
+    ThrottleSettingsOutputTypeDef,
     ApiKeyIdsTypeDef,
     ApiKeyResponseMetadataTypeDef,
     ApiKeyTypeDef,
+    ThrottleSettingsTypeDef,
     AuthorizerResponseMetadataTypeDef,
     AuthorizerTypeDef,
     BasePathMappingResponseMetadataTypeDef,
     BasePathMappingTypeDef,
+    CanarySettingsOutputTypeDef,
     CanarySettingsTypeDef,
     ClientCertificateResponseMetadataTypeDef,
     ClientCertificateTypeDef,
     StageKeyTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBasePathMappingRequestRequestTypeDef,
     DeploymentCanarySettingsTypeDef,
@@ -453,16 +455,18 @@
     DeleteRestApiRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteUsagePlanKeyRequestRequestTypeDef,
     DeleteUsagePlanRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     MethodSnapshotTypeDef,
     DocumentationPartIdsTypeDef,
+    DocumentationPartLocationOutputTypeDef,
     DocumentationVersionResponseMetadataTypeDef,
     DocumentationVersionTypeDef,
+    EndpointConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportResponseTypeDef,
     FlushStageAuthorizersCacheRequestRequestTypeDef,
     FlushStageCacheRequestRequestTypeDef,
     GatewayResponseResponseMetadataTypeDef,
     GatewayResponseTypeDef,
@@ -530,28 +534,30 @@
     GetVpcLinkRequestRequestTypeDef,
     GetVpcLinksRequestGetVpcLinksPaginateTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     ImportApiKeysRequestRequestTypeDef,
     ImportDocumentationPartsRequestRequestTypeDef,
     ImportRestApiRequestRequestTypeDef,
     IntegrationResponseTypeDef,
-    TlsConfigTypeDef,
+    TlsConfigOutputTypeDef,
     IntegrationResponseResponseMetadataTypeDef,
     MethodResponseTypeDef,
     MethodResponseResponseMetadataTypeDef,
     MethodSettingTypeDef,
     ModelResponseMetadataTypeDef,
     ModelTypeDef,
     PaginatorConfigTypeDef,
     PatchOperationTypeDef,
     PutGatewayResponseRequestRequestTypeDef,
+    TlsConfigTypeDef,
     PutIntegrationResponseRequestRequestTypeDef,
     PutMethodRequestRequestTypeDef,
     PutMethodResponseRequestRequestTypeDef,
     PutRestApiRequestRequestTypeDef,
+    QuotaSettingsOutputTypeDef,
     RequestValidatorResponseMetadataTypeDef,
     RequestValidatorTypeDef,
     ResponseMetadataTypeDef,
     SdkConfigurationPropertyTypeDef,
     SdkResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TagsTypeDef,
@@ -563,38 +569,38 @@
     UntagResourceRequestRequestTypeDef,
     UsagePlanKeyResponseMetadataTypeDef,
     UsagePlanKeyTypeDef,
     UsageTypeDef,
     VpcLinkResponseMetadataTypeDef,
     VpcLinkTypeDef,
     AccountTypeDef,
-    ApiStageTypeDef,
+    ApiStageOutputTypeDef,
     ApiKeysTypeDef,
+    ApiStageTypeDef,
     AuthorizersTypeDef,
     BasePathMappingsTypeDef,
     CreateStageRequestRequestTypeDef,
     ClientCertificatesTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     CreateDocumentationPartRequestRequestTypeDef,
-    DocumentationPartResponseMetadataTypeDef,
-    DocumentationPartTypeDef,
     CreateRestApiRequestRequestTypeDef,
-    RestApiResponseMetadataTypeDef,
-    RestApiTypeDef,
     CreateDomainNameRequestRequestTypeDef,
     DeploymentResponseMetadataTypeDef,
     DeploymentTypeDef,
+    DocumentationPartResponseMetadataTypeDef,
+    DocumentationPartTypeDef,
     DocumentationVersionsTypeDef,
+    RestApiResponseMetadataTypeDef,
+    RestApiTypeDef,
     DomainNameResponseMetadataTypeDef,
     DomainNameTypeDef,
     GatewayResponsesTypeDef,
     IntegrationResponseMetadataTypeDef,
     IntegrationTypeDef,
-    PutIntegrationRequestRequestTypeDef,
     StageResponseMetadataTypeDef,
     StageTypeDef,
     ModelsTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateApiKeyRequestRequestTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
     UpdateBasePathMappingRequestRequestTypeDef,
@@ -612,25 +618,26 @@
     UpdateRequestValidatorRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateRestApiRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
     UpdateUsagePlanRequestRequestTypeDef,
     UpdateUsageRequestRequestTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
+    PutIntegrationRequestRequestTypeDef,
     RequestValidatorsTypeDef,
     SdkTypeResponseMetadataTypeDef,
     SdkTypeTypeDef,
     UsagePlanKeysTypeDef,
     VpcLinksTypeDef,
-    CreateUsagePlanRequestRequestTypeDef,
     UsagePlanResponseMetadataTypeDef,
     UsagePlanTypeDef,
+    CreateUsagePlanRequestRequestTypeDef,
+    DeploymentsTypeDef,
     DocumentationPartsTypeDef,
     RestApisTypeDef,
-    DeploymentsTypeDef,
     DomainNamesTypeDef,
     MethodResponseMetadataTypeDef,
     MethodTypeDef,
     StagesTypeDef,
     SdkTypesTypeDef,
     UsagePlansTypeDef,
     ResourceResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-apigateway-1.28.0/README.md` & `mypy-boto3-apigateway-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-apigateway"></a>
 
 # mypy-boto3-apigateway
 
 [![PyPI - mypy-boto3-apigateway](https://img.shields.io/pypi/v/mypy-boto3-apigateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apigateway?color=blue)](https://pypistats.org/packages/mypy-boto3-apigateway)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigateway)](https://pepy.tech/project/mypy-boto3-apigateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.APIGateway 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
+[boto3.APIGateway 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
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
 [mypy-boto3-apigateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -373,22 +373,24 @@
 
 `mypy_boto3_apigateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigateway.type_defs import (
     AccessLogSettingsTypeDef,
-    ThrottleSettingsTypeDef,
+    ThrottleSettingsOutputTypeDef,
     ApiKeyIdsTypeDef,
     ApiKeyResponseMetadataTypeDef,
     ApiKeyTypeDef,
+    ThrottleSettingsTypeDef,
     AuthorizerResponseMetadataTypeDef,
     AuthorizerTypeDef,
     BasePathMappingResponseMetadataTypeDef,
     BasePathMappingTypeDef,
+    CanarySettingsOutputTypeDef,
     CanarySettingsTypeDef,
     ClientCertificateResponseMetadataTypeDef,
     ClientCertificateTypeDef,
     StageKeyTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBasePathMappingRequestRequestTypeDef,
     DeploymentCanarySettingsTypeDef,
@@ -421,16 +423,18 @@
     DeleteRestApiRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteUsagePlanKeyRequestRequestTypeDef,
     DeleteUsagePlanRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     MethodSnapshotTypeDef,
     DocumentationPartIdsTypeDef,
+    DocumentationPartLocationOutputTypeDef,
     DocumentationVersionResponseMetadataTypeDef,
     DocumentationVersionTypeDef,
+    EndpointConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportResponseTypeDef,
     FlushStageAuthorizersCacheRequestRequestTypeDef,
     FlushStageCacheRequestRequestTypeDef,
     GatewayResponseResponseMetadataTypeDef,
     GatewayResponseTypeDef,
@@ -498,28 +502,30 @@
     GetVpcLinkRequestRequestTypeDef,
     GetVpcLinksRequestGetVpcLinksPaginateTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     ImportApiKeysRequestRequestTypeDef,
     ImportDocumentationPartsRequestRequestTypeDef,
     ImportRestApiRequestRequestTypeDef,
     IntegrationResponseTypeDef,
-    TlsConfigTypeDef,
+    TlsConfigOutputTypeDef,
     IntegrationResponseResponseMetadataTypeDef,
     MethodResponseTypeDef,
     MethodResponseResponseMetadataTypeDef,
     MethodSettingTypeDef,
     ModelResponseMetadataTypeDef,
     ModelTypeDef,
     PaginatorConfigTypeDef,
     PatchOperationTypeDef,
     PutGatewayResponseRequestRequestTypeDef,
+    TlsConfigTypeDef,
     PutIntegrationResponseRequestRequestTypeDef,
     PutMethodRequestRequestTypeDef,
     PutMethodResponseRequestRequestTypeDef,
     PutRestApiRequestRequestTypeDef,
+    QuotaSettingsOutputTypeDef,
     RequestValidatorResponseMetadataTypeDef,
     RequestValidatorTypeDef,
     ResponseMetadataTypeDef,
     SdkConfigurationPropertyTypeDef,
     SdkResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TagsTypeDef,
@@ -531,38 +537,38 @@
     UntagResourceRequestRequestTypeDef,
     UsagePlanKeyResponseMetadataTypeDef,
     UsagePlanKeyTypeDef,
     UsageTypeDef,
     VpcLinkResponseMetadataTypeDef,
     VpcLinkTypeDef,
     AccountTypeDef,
-    ApiStageTypeDef,
+    ApiStageOutputTypeDef,
     ApiKeysTypeDef,
+    ApiStageTypeDef,
     AuthorizersTypeDef,
     BasePathMappingsTypeDef,
     CreateStageRequestRequestTypeDef,
     ClientCertificatesTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     CreateDocumentationPartRequestRequestTypeDef,
-    DocumentationPartResponseMetadataTypeDef,
-    DocumentationPartTypeDef,
     CreateRestApiRequestRequestTypeDef,
-    RestApiResponseMetadataTypeDef,
-    RestApiTypeDef,
     CreateDomainNameRequestRequestTypeDef,
     DeploymentResponseMetadataTypeDef,
     DeploymentTypeDef,
+    DocumentationPartResponseMetadataTypeDef,
+    DocumentationPartTypeDef,
     DocumentationVersionsTypeDef,
+    RestApiResponseMetadataTypeDef,
+    RestApiTypeDef,
     DomainNameResponseMetadataTypeDef,
     DomainNameTypeDef,
     GatewayResponsesTypeDef,
     IntegrationResponseMetadataTypeDef,
     IntegrationTypeDef,
-    PutIntegrationRequestRequestTypeDef,
     StageResponseMetadataTypeDef,
     StageTypeDef,
     ModelsTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateApiKeyRequestRequestTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
     UpdateBasePathMappingRequestRequestTypeDef,
@@ -580,25 +586,26 @@
     UpdateRequestValidatorRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateRestApiRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
     UpdateUsagePlanRequestRequestTypeDef,
     UpdateUsageRequestRequestTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
+    PutIntegrationRequestRequestTypeDef,
     RequestValidatorsTypeDef,
     SdkTypeResponseMetadataTypeDef,
     SdkTypeTypeDef,
     UsagePlanKeysTypeDef,
     VpcLinksTypeDef,
-    CreateUsagePlanRequestRequestTypeDef,
     UsagePlanResponseMetadataTypeDef,
     UsagePlanTypeDef,
+    CreateUsagePlanRequestRequestTypeDef,
+    DeploymentsTypeDef,
     DocumentationPartsTypeDef,
     RestApisTypeDef,
-    DeploymentsTypeDef,
     DomainNamesTypeDef,
     MethodResponseMetadataTypeDef,
     MethodTypeDef,
     StagesTypeDef,
     SdkTypesTypeDef,
     UsagePlansTypeDef,
     ResourceResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/__init__.py` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/__init__.pyi` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/__main__.py` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.APIGateway 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.APIGateway 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway\nOther"
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

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/client.py` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/client.pyi` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/literals.py` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,15 @@
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
@@ -349,26 +350,28 @@
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

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/literals.pyi` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,15 @@
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
@@ -347,26 +348,28 @@
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

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/paginator.py` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/paginator.pyi` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/type_defs.py` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,22 +46,24 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessLogSettingsTypeDef",
-    "ThrottleSettingsTypeDef",
+    "ThrottleSettingsOutputTypeDef",
     "ApiKeyIdsTypeDef",
     "ApiKeyResponseMetadataTypeDef",
     "ApiKeyTypeDef",
+    "ThrottleSettingsTypeDef",
     "AuthorizerResponseMetadataTypeDef",
     "AuthorizerTypeDef",
     "BasePathMappingResponseMetadataTypeDef",
     "BasePathMappingTypeDef",
+    "CanarySettingsOutputTypeDef",
     "CanarySettingsTypeDef",
     "ClientCertificateResponseMetadataTypeDef",
     "ClientCertificateTypeDef",
     "StageKeyTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "CreateBasePathMappingRequestRequestTypeDef",
     "DeploymentCanarySettingsTypeDef",
@@ -94,16 +96,18 @@
     "DeleteRestApiRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeleteUsagePlanKeyRequestRequestTypeDef",
     "DeleteUsagePlanRequestRequestTypeDef",
     "DeleteVpcLinkRequestRequestTypeDef",
     "MethodSnapshotTypeDef",
     "DocumentationPartIdsTypeDef",
+    "DocumentationPartLocationOutputTypeDef",
     "DocumentationVersionResponseMetadataTypeDef",
     "DocumentationVersionTypeDef",
+    "EndpointConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportResponseTypeDef",
     "FlushStageAuthorizersCacheRequestRequestTypeDef",
     "FlushStageCacheRequestRequestTypeDef",
     "GatewayResponseResponseMetadataTypeDef",
     "GatewayResponseTypeDef",
@@ -171,28 +175,30 @@
     "GetVpcLinkRequestRequestTypeDef",
     "GetVpcLinksRequestGetVpcLinksPaginateTypeDef",
     "GetVpcLinksRequestRequestTypeDef",
     "ImportApiKeysRequestRequestTypeDef",
     "ImportDocumentationPartsRequestRequestTypeDef",
     "ImportRestApiRequestRequestTypeDef",
     "IntegrationResponseTypeDef",
-    "TlsConfigTypeDef",
+    "TlsConfigOutputTypeDef",
     "IntegrationResponseResponseMetadataTypeDef",
     "MethodResponseTypeDef",
     "MethodResponseResponseMetadataTypeDef",
     "MethodSettingTypeDef",
     "ModelResponseMetadataTypeDef",
     "ModelTypeDef",
     "PaginatorConfigTypeDef",
     "PatchOperationTypeDef",
     "PutGatewayResponseRequestRequestTypeDef",
+    "TlsConfigTypeDef",
     "PutIntegrationResponseRequestRequestTypeDef",
     "PutMethodRequestRequestTypeDef",
     "PutMethodResponseRequestRequestTypeDef",
     "PutRestApiRequestRequestTypeDef",
+    "QuotaSettingsOutputTypeDef",
     "RequestValidatorResponseMetadataTypeDef",
     "RequestValidatorTypeDef",
     "ResponseMetadataTypeDef",
     "SdkConfigurationPropertyTypeDef",
     "SdkResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TagsTypeDef",
@@ -204,38 +210,38 @@
     "UntagResourceRequestRequestTypeDef",
     "UsagePlanKeyResponseMetadataTypeDef",
     "UsagePlanKeyTypeDef",
     "UsageTypeDef",
     "VpcLinkResponseMetadataTypeDef",
     "VpcLinkTypeDef",
     "AccountTypeDef",
-    "ApiStageTypeDef",
+    "ApiStageOutputTypeDef",
     "ApiKeysTypeDef",
+    "ApiStageTypeDef",
     "AuthorizersTypeDef",
     "BasePathMappingsTypeDef",
     "CreateStageRequestRequestTypeDef",
     "ClientCertificatesTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "CreateDocumentationPartRequestRequestTypeDef",
-    "DocumentationPartResponseMetadataTypeDef",
-    "DocumentationPartTypeDef",
     "CreateRestApiRequestRequestTypeDef",
-    "RestApiResponseMetadataTypeDef",
-    "RestApiTypeDef",
     "CreateDomainNameRequestRequestTypeDef",
     "DeploymentResponseMetadataTypeDef",
     "DeploymentTypeDef",
+    "DocumentationPartResponseMetadataTypeDef",
+    "DocumentationPartTypeDef",
     "DocumentationVersionsTypeDef",
+    "RestApiResponseMetadataTypeDef",
+    "RestApiTypeDef",
     "DomainNameResponseMetadataTypeDef",
     "DomainNameTypeDef",
     "GatewayResponsesTypeDef",
     "IntegrationResponseMetadataTypeDef",
     "IntegrationTypeDef",
-    "PutIntegrationRequestRequestTypeDef",
     "StageResponseMetadataTypeDef",
     "StageTypeDef",
     "ModelsTypeDef",
     "UpdateAccountRequestRequestTypeDef",
     "UpdateApiKeyRequestRequestTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
     "UpdateBasePathMappingRequestRequestTypeDef",
@@ -253,25 +259,26 @@
     "UpdateRequestValidatorRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateRestApiRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
     "UpdateUsagePlanRequestRequestTypeDef",
     "UpdateUsageRequestRequestTypeDef",
     "UpdateVpcLinkRequestRequestTypeDef",
+    "PutIntegrationRequestRequestTypeDef",
     "RequestValidatorsTypeDef",
     "SdkTypeResponseMetadataTypeDef",
     "SdkTypeTypeDef",
     "UsagePlanKeysTypeDef",
     "VpcLinksTypeDef",
-    "CreateUsagePlanRequestRequestTypeDef",
     "UsagePlanResponseMetadataTypeDef",
     "UsagePlanTypeDef",
+    "CreateUsagePlanRequestRequestTypeDef",
+    "DeploymentsTypeDef",
     "DocumentationPartsTypeDef",
     "RestApisTypeDef",
-    "DeploymentsTypeDef",
     "DomainNamesTypeDef",
     "MethodResponseMetadataTypeDef",
     "MethodTypeDef",
     "StagesTypeDef",
     "SdkTypesTypeDef",
     "UsagePlansTypeDef",
     "ResourceResponseMetadataTypeDef",
@@ -284,16 +291,16 @@
     {
         "format": str,
         "destinationArn": str,
     },
     total=False,
 )
 
-ThrottleSettingsTypeDef = TypedDict(
-    "ThrottleSettingsTypeDef",
+ThrottleSettingsOutputTypeDef = TypedDict(
+    "ThrottleSettingsOutputTypeDef",
     {
         "burstLimit": int,
         "rateLimit": float,
     },
     total=False,
 )
 
@@ -336,14 +343,23 @@
         "lastUpdatedDate": datetime,
         "stageKeys": List[str],
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+ThrottleSettingsTypeDef = TypedDict(
+    "ThrottleSettingsTypeDef",
+    {
+        "burstLimit": int,
+        "rateLimit": float,
+    },
+    total=False,
+)
+
 AuthorizerResponseMetadataTypeDef = TypedDict(
     "AuthorizerResponseMetadataTypeDef",
     {
         "id": str,
         "name": str,
         "type": AuthorizerTypeType,
         "providerARNs": List[str],
@@ -390,14 +406,25 @@
         "basePath": str,
         "restApiId": str,
         "stage": str,
     },
     total=False,
 )
 
+CanarySettingsOutputTypeDef = TypedDict(
+    "CanarySettingsOutputTypeDef",
+    {
+        "percentTraffic": float,
+        "deploymentId": str,
+        "stageVariableOverrides": Dict[str, str],
+        "useStageCache": bool,
+    },
+    total=False,
+)
+
 CanarySettingsTypeDef = TypedDict(
     "CanarySettingsTypeDef",
     {
         "percentTraffic": float,
         "deploymentId": str,
         "stageVariableOverrides": Mapping[str, str],
         "useStageCache": bool,
@@ -850,14 +877,38 @@
     {
         "ids": List[str],
         "warnings": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDocumentationPartLocationOutputTypeDef = TypedDict(
+    "_RequiredDocumentationPartLocationOutputTypeDef",
+    {
+        "type": DocumentationPartTypeType,
+    },
+)
+_OptionalDocumentationPartLocationOutputTypeDef = TypedDict(
+    "_OptionalDocumentationPartLocationOutputTypeDef",
+    {
+        "path": str,
+        "method": str,
+        "statusCode": str,
+        "name": str,
+    },
+    total=False,
+)
+
+
+class DocumentationPartLocationOutputTypeDef(
+    _RequiredDocumentationPartLocationOutputTypeDef, _OptionalDocumentationPartLocationOutputTypeDef
+):
+    pass
+
+
 DocumentationVersionResponseMetadataTypeDef = TypedDict(
     "DocumentationVersionResponseMetadataTypeDef",
     {
         "version": str,
         "createdDate": datetime,
         "description": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -870,14 +921,23 @@
         "version": str,
         "createdDate": datetime,
         "description": str,
     },
     total=False,
 )
 
+EndpointConfigurationOutputTypeDef = TypedDict(
+    "EndpointConfigurationOutputTypeDef",
+    {
+        "types": List[EndpointTypeType],
+        "vpcEndpointIds": List[str],
+    },
+    total=False,
+)
+
 MutualTlsAuthenticationTypeDef = TypedDict(
     "MutualTlsAuthenticationTypeDef",
     {
         "truststoreUri": str,
         "truststoreVersion": str,
         "truststoreWarnings": List[str],
     },
@@ -1988,16 +2048,16 @@
         "responseParameters": Dict[str, str],
         "responseTemplates": Dict[str, str],
         "contentHandling": ContentHandlingStrategyType,
     },
     total=False,
 )
 
-TlsConfigTypeDef = TypedDict(
-    "TlsConfigTypeDef",
+TlsConfigOutputTypeDef = TypedDict(
+    "TlsConfigOutputTypeDef",
     {
         "insecureSkipVerification": bool,
     },
     total=False,
 )
 
 IntegrationResponseResponseMetadataTypeDef = TypedDict(
@@ -2115,14 +2175,22 @@
 class PutGatewayResponseRequestRequestTypeDef(
     _RequiredPutGatewayResponseRequestRequestTypeDef,
     _OptionalPutGatewayResponseRequestRequestTypeDef,
 ):
     pass
 
 
+TlsConfigTypeDef = TypedDict(
+    "TlsConfigTypeDef",
+    {
+        "insecureSkipVerification": bool,
+    },
+    total=False,
+)
+
 _RequiredPutIntegrationResponseRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntegrationResponseRequestRequestTypeDef",
     {
         "restApiId": str,
         "resourceId": str,
         "httpMethod": str,
         "statusCode": str,
@@ -2222,14 +2290,24 @@
 
 class PutRestApiRequestRequestTypeDef(
     _RequiredPutRestApiRequestRequestTypeDef, _OptionalPutRestApiRequestRequestTypeDef
 ):
     pass
 
 
+QuotaSettingsOutputTypeDef = TypedDict(
+    "QuotaSettingsOutputTypeDef",
+    {
+        "limit": int,
+        "offset": int,
+        "period": QuotaPeriodTypeType,
+    },
+    total=False,
+)
+
 RequestValidatorResponseMetadataTypeDef = TypedDict(
     "RequestValidatorResponseMetadataTypeDef",
     {
         "id": str,
         "name": str,
         "validateRequestBody": bool,
         "validateRequestParameters": bool,
@@ -2458,41 +2536,51 @@
     total=False,
 )
 
 AccountTypeDef = TypedDict(
     "AccountTypeDef",
     {
         "cloudwatchRoleArn": str,
-        "throttleSettings": ThrottleSettingsTypeDef,
+        "throttleSettings": ThrottleSettingsOutputTypeDef,
         "features": List[str],
         "apiKeyVersion": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ApiStageTypeDef = TypedDict(
-    "ApiStageTypeDef",
+ApiStageOutputTypeDef = TypedDict(
+    "ApiStageOutputTypeDef",
     {
         "apiId": str,
         "stage": str,
-        "throttle": Mapping[str, ThrottleSettingsTypeDef],
+        "throttle": Dict[str, ThrottleSettingsOutputTypeDef],
     },
     total=False,
 )
 
 ApiKeysTypeDef = TypedDict(
     "ApiKeysTypeDef",
     {
         "warnings": List[str],
         "position": str,
         "items": List[ApiKeyTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ApiStageTypeDef = TypedDict(
+    "ApiStageTypeDef",
+    {
+        "apiId": str,
+        "stage": str,
+        "throttle": Mapping[str, ThrottleSettingsTypeDef],
+    },
+    total=False,
+)
+
 AuthorizersTypeDef = TypedDict(
     "AuthorizersTypeDef",
     {
         "position": str,
         "items": List[AuthorizerTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2594,34 +2682,14 @@
     {
         "restApiId": str,
         "location": DocumentationPartLocationTypeDef,
         "properties": str,
     },
 )
 
-DocumentationPartResponseMetadataTypeDef = TypedDict(
-    "DocumentationPartResponseMetadataTypeDef",
-    {
-        "id": str,
-        "location": DocumentationPartLocationTypeDef,
-        "properties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DocumentationPartTypeDef = TypedDict(
-    "DocumentationPartTypeDef",
-    {
-        "id": str,
-        "location": DocumentationPartLocationTypeDef,
-        "properties": str,
-    },
-    total=False,
-)
-
 _RequiredCreateRestApiRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRestApiRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateRestApiRequestRequestTypeDef = TypedDict(
@@ -2644,54 +2712,14 @@
 
 class CreateRestApiRequestRequestTypeDef(
     _RequiredCreateRestApiRequestRequestTypeDef, _OptionalCreateRestApiRequestRequestTypeDef
 ):
     pass
 
 
-RestApiResponseMetadataTypeDef = TypedDict(
-    "RestApiResponseMetadataTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "description": str,
-        "createdDate": datetime,
-        "version": str,
-        "warnings": List[str],
-        "binaryMediaTypes": List[str],
-        "minimumCompressionSize": int,
-        "apiKeySource": ApiKeySourceTypeType,
-        "endpointConfiguration": EndpointConfigurationTypeDef,
-        "policy": str,
-        "tags": Dict[str, str],
-        "disableExecuteApiEndpoint": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RestApiTypeDef = TypedDict(
-    "RestApiTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "description": str,
-        "createdDate": datetime,
-        "version": str,
-        "warnings": List[str],
-        "binaryMediaTypes": List[str],
-        "minimumCompressionSize": int,
-        "apiKeySource": ApiKeySourceTypeType,
-        "endpointConfiguration": EndpointConfigurationTypeDef,
-        "policy": str,
-        "tags": Dict[str, str],
-        "disableExecuteApiEndpoint": bool,
-    },
-    total=False,
-)
-
 _RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainNameRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 _OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
@@ -2738,37 +2766,97 @@
         "description": str,
         "createdDate": datetime,
         "apiSummary": Dict[str, Dict[str, MethodSnapshotTypeDef]],
     },
     total=False,
 )
 
+DocumentationPartResponseMetadataTypeDef = TypedDict(
+    "DocumentationPartResponseMetadataTypeDef",
+    {
+        "id": str,
+        "location": DocumentationPartLocationOutputTypeDef,
+        "properties": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DocumentationPartTypeDef = TypedDict(
+    "DocumentationPartTypeDef",
+    {
+        "id": str,
+        "location": DocumentationPartLocationOutputTypeDef,
+        "properties": str,
+    },
+    total=False,
+)
+
 DocumentationVersionsTypeDef = TypedDict(
     "DocumentationVersionsTypeDef",
     {
         "position": str,
         "items": List[DocumentationVersionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RestApiResponseMetadataTypeDef = TypedDict(
+    "RestApiResponseMetadataTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "description": str,
+        "createdDate": datetime,
+        "version": str,
+        "warnings": List[str],
+        "binaryMediaTypes": List[str],
+        "minimumCompressionSize": int,
+        "apiKeySource": ApiKeySourceTypeType,
+        "endpointConfiguration": EndpointConfigurationOutputTypeDef,
+        "policy": str,
+        "tags": Dict[str, str],
+        "disableExecuteApiEndpoint": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RestApiTypeDef = TypedDict(
+    "RestApiTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "description": str,
+        "createdDate": datetime,
+        "version": str,
+        "warnings": List[str],
+        "binaryMediaTypes": List[str],
+        "minimumCompressionSize": int,
+        "apiKeySource": ApiKeySourceTypeType,
+        "endpointConfiguration": EndpointConfigurationOutputTypeDef,
+        "policy": str,
+        "tags": Dict[str, str],
+        "disableExecuteApiEndpoint": bool,
+    },
+    total=False,
+)
+
 DomainNameResponseMetadataTypeDef = TypedDict(
     "DomainNameResponseMetadataTypeDef",
     {
         "domainName": str,
         "certificateName": str,
         "certificateArn": str,
         "certificateUploadDate": datetime,
         "regionalDomainName": str,
         "regionalHostedZoneId": str,
         "regionalCertificateName": str,
         "regionalCertificateArn": str,
         "distributionDomainName": str,
         "distributionHostedZoneId": str,
-        "endpointConfiguration": EndpointConfigurationTypeDef,
+        "endpointConfiguration": EndpointConfigurationOutputTypeDef,
         "domainNameStatus": DomainNameStatusType,
         "domainNameStatusMessage": str,
         "securityPolicy": SecurityPolicyType,
         "tags": Dict[str, str],
         "mutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "ownershipVerificationCertificateArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2784,15 +2872,15 @@
         "certificateUploadDate": datetime,
         "regionalDomainName": str,
         "regionalHostedZoneId": str,
         "regionalCertificateName": str,
         "regionalCertificateArn": str,
         "distributionDomainName": str,
         "distributionHostedZoneId": str,
-        "endpointConfiguration": EndpointConfigurationTypeDef,
+        "endpointConfiguration": EndpointConfigurationOutputTypeDef,
         "domainNameStatus": DomainNameStatusType,
         "domainNameStatusMessage": str,
         "securityPolicy": SecurityPolicyType,
         "tags": Dict[str, str],
         "mutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "ownershipVerificationCertificateArn": str,
     },
@@ -2821,15 +2909,15 @@
         "requestTemplates": Dict[str, str],
         "passthroughBehavior": str,
         "contentHandling": ContentHandlingStrategyType,
         "timeoutInMillis": int,
         "cacheNamespace": str,
         "cacheKeyParameters": List[str],
         "integrationResponses": Dict[str, IntegrationResponseTypeDef],
-        "tlsConfig": TlsConfigTypeDef,
+        "tlsConfig": TlsConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
@@ -2843,70 +2931,34 @@
         "requestTemplates": Dict[str, str],
         "passthroughBehavior": str,
         "contentHandling": ContentHandlingStrategyType,
         "timeoutInMillis": int,
         "cacheNamespace": str,
         "cacheKeyParameters": List[str],
         "integrationResponses": Dict[str, IntegrationResponseTypeDef],
-        "tlsConfig": TlsConfigTypeDef,
+        "tlsConfig": TlsConfigOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredPutIntegrationRequestRequestTypeDef = TypedDict(
-    "_RequiredPutIntegrationRequestRequestTypeDef",
-    {
-        "restApiId": str,
-        "resourceId": str,
-        "httpMethod": str,
-        "type": IntegrationTypeType,
-    },
-)
-_OptionalPutIntegrationRequestRequestTypeDef = TypedDict(
-    "_OptionalPutIntegrationRequestRequestTypeDef",
-    {
-        "integrationHttpMethod": str,
-        "uri": str,
-        "connectionType": ConnectionTypeType,
-        "connectionId": str,
-        "credentials": str,
-        "requestParameters": Mapping[str, str],
-        "requestTemplates": Mapping[str, str],
-        "passthroughBehavior": str,
-        "cacheNamespace": str,
-        "cacheKeyParameters": Sequence[str],
-        "contentHandling": ContentHandlingStrategyType,
-        "timeoutInMillis": int,
-        "tlsConfig": TlsConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class PutIntegrationRequestRequestTypeDef(
-    _RequiredPutIntegrationRequestRequestTypeDef, _OptionalPutIntegrationRequestRequestTypeDef
-):
-    pass
-
-
 StageResponseMetadataTypeDef = TypedDict(
     "StageResponseMetadataTypeDef",
     {
         "deploymentId": str,
         "clientCertificateId": str,
         "stageName": str,
         "description": str,
         "cacheClusterEnabled": bool,
         "cacheClusterSize": CacheClusterSizeType,
         "cacheClusterStatus": CacheClusterStatusType,
         "methodSettings": Dict[str, MethodSettingTypeDef],
         "variables": Dict[str, str],
         "documentationVersion": str,
         "accessLogSettings": AccessLogSettingsTypeDef,
-        "canarySettings": CanarySettingsTypeDef,
+        "canarySettings": CanarySettingsOutputTypeDef,
         "tracingEnabled": bool,
         "webAclArn": str,
         "tags": Dict[str, str],
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2922,15 +2974,15 @@
         "cacheClusterEnabled": bool,
         "cacheClusterSize": CacheClusterSizeType,
         "cacheClusterStatus": CacheClusterStatusType,
         "methodSettings": Dict[str, MethodSettingTypeDef],
         "variables": Dict[str, str],
         "documentationVersion": str,
         "accessLogSettings": AccessLogSettingsTypeDef,
-        "canarySettings": CanarySettingsTypeDef,
+        "canarySettings": CanarySettingsOutputTypeDef,
         "tracingEnabled": bool,
         "webAclArn": str,
         "tags": Dict[str, str],
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
     },
     total=False,
@@ -3419,14 +3471,50 @@
 
 class UpdateVpcLinkRequestRequestTypeDef(
     _RequiredUpdateVpcLinkRequestRequestTypeDef, _OptionalUpdateVpcLinkRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredPutIntegrationRequestRequestTypeDef = TypedDict(
+    "_RequiredPutIntegrationRequestRequestTypeDef",
+    {
+        "restApiId": str,
+        "resourceId": str,
+        "httpMethod": str,
+        "type": IntegrationTypeType,
+    },
+)
+_OptionalPutIntegrationRequestRequestTypeDef = TypedDict(
+    "_OptionalPutIntegrationRequestRequestTypeDef",
+    {
+        "integrationHttpMethod": str,
+        "uri": str,
+        "connectionType": ConnectionTypeType,
+        "connectionId": str,
+        "credentials": str,
+        "requestParameters": Mapping[str, str],
+        "requestTemplates": Mapping[str, str],
+        "passthroughBehavior": str,
+        "cacheNamespace": str,
+        "cacheKeyParameters": Sequence[str],
+        "contentHandling": ContentHandlingStrategyType,
+        "timeoutInMillis": int,
+        "tlsConfig": TlsConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class PutIntegrationRequestRequestTypeDef(
+    _RequiredPutIntegrationRequestRequestTypeDef, _OptionalPutIntegrationRequestRequestTypeDef
+):
+    pass
+
+
 RequestValidatorsTypeDef = TypedDict(
     "RequestValidatorsTypeDef",
     {
         "position": str,
         "items": List[RequestValidatorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3468,14 +3556,44 @@
     {
         "position": str,
         "items": List[VpcLinkTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+UsagePlanResponseMetadataTypeDef = TypedDict(
+    "UsagePlanResponseMetadataTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "description": str,
+        "apiStages": List[ApiStageOutputTypeDef],
+        "throttle": ThrottleSettingsOutputTypeDef,
+        "quota": QuotaSettingsOutputTypeDef,
+        "productCode": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UsagePlanTypeDef = TypedDict(
+    "UsagePlanTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "description": str,
+        "apiStages": List[ApiStageOutputTypeDef],
+        "throttle": ThrottleSettingsOutputTypeDef,
+        "quota": QuotaSettingsOutputTypeDef,
+        "productCode": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredCreateUsagePlanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUsagePlanRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateUsagePlanRequestRequestTypeDef = TypedDict(
@@ -3493,44 +3611,23 @@
 
 class CreateUsagePlanRequestRequestTypeDef(
     _RequiredCreateUsagePlanRequestRequestTypeDef, _OptionalCreateUsagePlanRequestRequestTypeDef
 ):
     pass
 
 
-UsagePlanResponseMetadataTypeDef = TypedDict(
-    "UsagePlanResponseMetadataTypeDef",
+DeploymentsTypeDef = TypedDict(
+    "DeploymentsTypeDef",
     {
-        "id": str,
-        "name": str,
-        "description": str,
-        "apiStages": List[ApiStageTypeDef],
-        "throttle": ThrottleSettingsTypeDef,
-        "quota": QuotaSettingsTypeDef,
-        "productCode": str,
-        "tags": Dict[str, str],
+        "position": str,
+        "items": List[DeploymentTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UsagePlanTypeDef = TypedDict(
-    "UsagePlanTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "description": str,
-        "apiStages": List[ApiStageTypeDef],
-        "throttle": ThrottleSettingsTypeDef,
-        "quota": QuotaSettingsTypeDef,
-        "productCode": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 DocumentationPartsTypeDef = TypedDict(
     "DocumentationPartsTypeDef",
     {
         "position": str,
         "items": List[DocumentationPartTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3541,23 +3638,14 @@
     {
         "position": str,
         "items": List[RestApiTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeploymentsTypeDef = TypedDict(
-    "DeploymentsTypeDef",
-    {
-        "position": str,
-        "items": List[DeploymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DomainNamesTypeDef = TypedDict(
     "DomainNamesTypeDef",
     {
         "position": str,
         "items": List[DomainNameTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway/type_defs.pyi` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,22 +45,24 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessLogSettingsTypeDef",
-    "ThrottleSettingsTypeDef",
+    "ThrottleSettingsOutputTypeDef",
     "ApiKeyIdsTypeDef",
     "ApiKeyResponseMetadataTypeDef",
     "ApiKeyTypeDef",
+    "ThrottleSettingsTypeDef",
     "AuthorizerResponseMetadataTypeDef",
     "AuthorizerTypeDef",
     "BasePathMappingResponseMetadataTypeDef",
     "BasePathMappingTypeDef",
+    "CanarySettingsOutputTypeDef",
     "CanarySettingsTypeDef",
     "ClientCertificateResponseMetadataTypeDef",
     "ClientCertificateTypeDef",
     "StageKeyTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
     "CreateBasePathMappingRequestRequestTypeDef",
     "DeploymentCanarySettingsTypeDef",
@@ -93,16 +95,18 @@
     "DeleteRestApiRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeleteUsagePlanKeyRequestRequestTypeDef",
     "DeleteUsagePlanRequestRequestTypeDef",
     "DeleteVpcLinkRequestRequestTypeDef",
     "MethodSnapshotTypeDef",
     "DocumentationPartIdsTypeDef",
+    "DocumentationPartLocationOutputTypeDef",
     "DocumentationVersionResponseMetadataTypeDef",
     "DocumentationVersionTypeDef",
+    "EndpointConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportResponseTypeDef",
     "FlushStageAuthorizersCacheRequestRequestTypeDef",
     "FlushStageCacheRequestRequestTypeDef",
     "GatewayResponseResponseMetadataTypeDef",
     "GatewayResponseTypeDef",
@@ -170,28 +174,30 @@
     "GetVpcLinkRequestRequestTypeDef",
     "GetVpcLinksRequestGetVpcLinksPaginateTypeDef",
     "GetVpcLinksRequestRequestTypeDef",
     "ImportApiKeysRequestRequestTypeDef",
     "ImportDocumentationPartsRequestRequestTypeDef",
     "ImportRestApiRequestRequestTypeDef",
     "IntegrationResponseTypeDef",
-    "TlsConfigTypeDef",
+    "TlsConfigOutputTypeDef",
     "IntegrationResponseResponseMetadataTypeDef",
     "MethodResponseTypeDef",
     "MethodResponseResponseMetadataTypeDef",
     "MethodSettingTypeDef",
     "ModelResponseMetadataTypeDef",
     "ModelTypeDef",
     "PaginatorConfigTypeDef",
     "PatchOperationTypeDef",
     "PutGatewayResponseRequestRequestTypeDef",
+    "TlsConfigTypeDef",
     "PutIntegrationResponseRequestRequestTypeDef",
     "PutMethodRequestRequestTypeDef",
     "PutMethodResponseRequestRequestTypeDef",
     "PutRestApiRequestRequestTypeDef",
+    "QuotaSettingsOutputTypeDef",
     "RequestValidatorResponseMetadataTypeDef",
     "RequestValidatorTypeDef",
     "ResponseMetadataTypeDef",
     "SdkConfigurationPropertyTypeDef",
     "SdkResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TagsTypeDef",
@@ -203,38 +209,38 @@
     "UntagResourceRequestRequestTypeDef",
     "UsagePlanKeyResponseMetadataTypeDef",
     "UsagePlanKeyTypeDef",
     "UsageTypeDef",
     "VpcLinkResponseMetadataTypeDef",
     "VpcLinkTypeDef",
     "AccountTypeDef",
-    "ApiStageTypeDef",
+    "ApiStageOutputTypeDef",
     "ApiKeysTypeDef",
+    "ApiStageTypeDef",
     "AuthorizersTypeDef",
     "BasePathMappingsTypeDef",
     "CreateStageRequestRequestTypeDef",
     "ClientCertificatesTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "CreateDocumentationPartRequestRequestTypeDef",
-    "DocumentationPartResponseMetadataTypeDef",
-    "DocumentationPartTypeDef",
     "CreateRestApiRequestRequestTypeDef",
-    "RestApiResponseMetadataTypeDef",
-    "RestApiTypeDef",
     "CreateDomainNameRequestRequestTypeDef",
     "DeploymentResponseMetadataTypeDef",
     "DeploymentTypeDef",
+    "DocumentationPartResponseMetadataTypeDef",
+    "DocumentationPartTypeDef",
     "DocumentationVersionsTypeDef",
+    "RestApiResponseMetadataTypeDef",
+    "RestApiTypeDef",
     "DomainNameResponseMetadataTypeDef",
     "DomainNameTypeDef",
     "GatewayResponsesTypeDef",
     "IntegrationResponseMetadataTypeDef",
     "IntegrationTypeDef",
-    "PutIntegrationRequestRequestTypeDef",
     "StageResponseMetadataTypeDef",
     "StageTypeDef",
     "ModelsTypeDef",
     "UpdateAccountRequestRequestTypeDef",
     "UpdateApiKeyRequestRequestTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
     "UpdateBasePathMappingRequestRequestTypeDef",
@@ -252,25 +258,26 @@
     "UpdateRequestValidatorRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateRestApiRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
     "UpdateUsagePlanRequestRequestTypeDef",
     "UpdateUsageRequestRequestTypeDef",
     "UpdateVpcLinkRequestRequestTypeDef",
+    "PutIntegrationRequestRequestTypeDef",
     "RequestValidatorsTypeDef",
     "SdkTypeResponseMetadataTypeDef",
     "SdkTypeTypeDef",
     "UsagePlanKeysTypeDef",
     "VpcLinksTypeDef",
-    "CreateUsagePlanRequestRequestTypeDef",
     "UsagePlanResponseMetadataTypeDef",
     "UsagePlanTypeDef",
+    "CreateUsagePlanRequestRequestTypeDef",
+    "DeploymentsTypeDef",
     "DocumentationPartsTypeDef",
     "RestApisTypeDef",
-    "DeploymentsTypeDef",
     "DomainNamesTypeDef",
     "MethodResponseMetadataTypeDef",
     "MethodTypeDef",
     "StagesTypeDef",
     "SdkTypesTypeDef",
     "UsagePlansTypeDef",
     "ResourceResponseMetadataTypeDef",
@@ -283,16 +290,16 @@
     {
         "format": str,
         "destinationArn": str,
     },
     total=False,
 )
 
-ThrottleSettingsTypeDef = TypedDict(
-    "ThrottleSettingsTypeDef",
+ThrottleSettingsOutputTypeDef = TypedDict(
+    "ThrottleSettingsOutputTypeDef",
     {
         "burstLimit": int,
         "rateLimit": float,
     },
     total=False,
 )
 
@@ -335,14 +342,23 @@
         "lastUpdatedDate": datetime,
         "stageKeys": List[str],
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+ThrottleSettingsTypeDef = TypedDict(
+    "ThrottleSettingsTypeDef",
+    {
+        "burstLimit": int,
+        "rateLimit": float,
+    },
+    total=False,
+)
+
 AuthorizerResponseMetadataTypeDef = TypedDict(
     "AuthorizerResponseMetadataTypeDef",
     {
         "id": str,
         "name": str,
         "type": AuthorizerTypeType,
         "providerARNs": List[str],
@@ -389,14 +405,25 @@
         "basePath": str,
         "restApiId": str,
         "stage": str,
     },
     total=False,
 )
 
+CanarySettingsOutputTypeDef = TypedDict(
+    "CanarySettingsOutputTypeDef",
+    {
+        "percentTraffic": float,
+        "deploymentId": str,
+        "stageVariableOverrides": Dict[str, str],
+        "useStageCache": bool,
+    },
+    total=False,
+)
+
 CanarySettingsTypeDef = TypedDict(
     "CanarySettingsTypeDef",
     {
         "percentTraffic": float,
         "deploymentId": str,
         "stageVariableOverrides": Mapping[str, str],
         "useStageCache": bool,
@@ -835,14 +862,36 @@
     {
         "ids": List[str],
         "warnings": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDocumentationPartLocationOutputTypeDef = TypedDict(
+    "_RequiredDocumentationPartLocationOutputTypeDef",
+    {
+        "type": DocumentationPartTypeType,
+    },
+)
+_OptionalDocumentationPartLocationOutputTypeDef = TypedDict(
+    "_OptionalDocumentationPartLocationOutputTypeDef",
+    {
+        "path": str,
+        "method": str,
+        "statusCode": str,
+        "name": str,
+    },
+    total=False,
+)
+
+class DocumentationPartLocationOutputTypeDef(
+    _RequiredDocumentationPartLocationOutputTypeDef, _OptionalDocumentationPartLocationOutputTypeDef
+):
+    pass
+
 DocumentationVersionResponseMetadataTypeDef = TypedDict(
     "DocumentationVersionResponseMetadataTypeDef",
     {
         "version": str,
         "createdDate": datetime,
         "description": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -855,14 +904,23 @@
         "version": str,
         "createdDate": datetime,
         "description": str,
     },
     total=False,
 )
 
+EndpointConfigurationOutputTypeDef = TypedDict(
+    "EndpointConfigurationOutputTypeDef",
+    {
+        "types": List[EndpointTypeType],
+        "vpcEndpointIds": List[str],
+    },
+    total=False,
+)
+
 MutualTlsAuthenticationTypeDef = TypedDict(
     "MutualTlsAuthenticationTypeDef",
     {
         "truststoreUri": str,
         "truststoreVersion": str,
         "truststoreWarnings": List[str],
     },
@@ -1907,16 +1965,16 @@
         "responseParameters": Dict[str, str],
         "responseTemplates": Dict[str, str],
         "contentHandling": ContentHandlingStrategyType,
     },
     total=False,
 )
 
-TlsConfigTypeDef = TypedDict(
-    "TlsConfigTypeDef",
+TlsConfigOutputTypeDef = TypedDict(
+    "TlsConfigOutputTypeDef",
     {
         "insecureSkipVerification": bool,
     },
     total=False,
 )
 
 IntegrationResponseResponseMetadataTypeDef = TypedDict(
@@ -2032,14 +2090,22 @@
 
 class PutGatewayResponseRequestRequestTypeDef(
     _RequiredPutGatewayResponseRequestRequestTypeDef,
     _OptionalPutGatewayResponseRequestRequestTypeDef,
 ):
     pass
 
+TlsConfigTypeDef = TypedDict(
+    "TlsConfigTypeDef",
+    {
+        "insecureSkipVerification": bool,
+    },
+    total=False,
+)
+
 _RequiredPutIntegrationResponseRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntegrationResponseRequestRequestTypeDef",
     {
         "restApiId": str,
         "resourceId": str,
         "httpMethod": str,
         "statusCode": str,
@@ -2131,14 +2197,24 @@
 )
 
 class PutRestApiRequestRequestTypeDef(
     _RequiredPutRestApiRequestRequestTypeDef, _OptionalPutRestApiRequestRequestTypeDef
 ):
     pass
 
+QuotaSettingsOutputTypeDef = TypedDict(
+    "QuotaSettingsOutputTypeDef",
+    {
+        "limit": int,
+        "offset": int,
+        "period": QuotaPeriodTypeType,
+    },
+    total=False,
+)
+
 RequestValidatorResponseMetadataTypeDef = TypedDict(
     "RequestValidatorResponseMetadataTypeDef",
     {
         "id": str,
         "name": str,
         "validateRequestBody": bool,
         "validateRequestParameters": bool,
@@ -2363,41 +2439,51 @@
     total=False,
 )
 
 AccountTypeDef = TypedDict(
     "AccountTypeDef",
     {
         "cloudwatchRoleArn": str,
-        "throttleSettings": ThrottleSettingsTypeDef,
+        "throttleSettings": ThrottleSettingsOutputTypeDef,
         "features": List[str],
         "apiKeyVersion": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ApiStageTypeDef = TypedDict(
-    "ApiStageTypeDef",
+ApiStageOutputTypeDef = TypedDict(
+    "ApiStageOutputTypeDef",
     {
         "apiId": str,
         "stage": str,
-        "throttle": Mapping[str, ThrottleSettingsTypeDef],
+        "throttle": Dict[str, ThrottleSettingsOutputTypeDef],
     },
     total=False,
 )
 
 ApiKeysTypeDef = TypedDict(
     "ApiKeysTypeDef",
     {
         "warnings": List[str],
         "position": str,
         "items": List[ApiKeyTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ApiStageTypeDef = TypedDict(
+    "ApiStageTypeDef",
+    {
+        "apiId": str,
+        "stage": str,
+        "throttle": Mapping[str, ThrottleSettingsTypeDef],
+    },
+    total=False,
+)
+
 AuthorizersTypeDef = TypedDict(
     "AuthorizersTypeDef",
     {
         "position": str,
         "items": List[AuthorizerTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2495,34 +2581,14 @@
     {
         "restApiId": str,
         "location": DocumentationPartLocationTypeDef,
         "properties": str,
     },
 )
 
-DocumentationPartResponseMetadataTypeDef = TypedDict(
-    "DocumentationPartResponseMetadataTypeDef",
-    {
-        "id": str,
-        "location": DocumentationPartLocationTypeDef,
-        "properties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DocumentationPartTypeDef = TypedDict(
-    "DocumentationPartTypeDef",
-    {
-        "id": str,
-        "location": DocumentationPartLocationTypeDef,
-        "properties": str,
-    },
-    total=False,
-)
-
 _RequiredCreateRestApiRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRestApiRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateRestApiRequestRequestTypeDef = TypedDict(
@@ -2543,54 +2609,14 @@
 )
 
 class CreateRestApiRequestRequestTypeDef(
     _RequiredCreateRestApiRequestRequestTypeDef, _OptionalCreateRestApiRequestRequestTypeDef
 ):
     pass
 
-RestApiResponseMetadataTypeDef = TypedDict(
-    "RestApiResponseMetadataTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "description": str,
-        "createdDate": datetime,
-        "version": str,
-        "warnings": List[str],
-        "binaryMediaTypes": List[str],
-        "minimumCompressionSize": int,
-        "apiKeySource": ApiKeySourceTypeType,
-        "endpointConfiguration": EndpointConfigurationTypeDef,
-        "policy": str,
-        "tags": Dict[str, str],
-        "disableExecuteApiEndpoint": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RestApiTypeDef = TypedDict(
-    "RestApiTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "description": str,
-        "createdDate": datetime,
-        "version": str,
-        "warnings": List[str],
-        "binaryMediaTypes": List[str],
-        "minimumCompressionSize": int,
-        "apiKeySource": ApiKeySourceTypeType,
-        "endpointConfiguration": EndpointConfigurationTypeDef,
-        "policy": str,
-        "tags": Dict[str, str],
-        "disableExecuteApiEndpoint": bool,
-    },
-    total=False,
-)
-
 _RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainNameRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 _OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
@@ -2635,37 +2661,97 @@
         "description": str,
         "createdDate": datetime,
         "apiSummary": Dict[str, Dict[str, MethodSnapshotTypeDef]],
     },
     total=False,
 )
 
+DocumentationPartResponseMetadataTypeDef = TypedDict(
+    "DocumentationPartResponseMetadataTypeDef",
+    {
+        "id": str,
+        "location": DocumentationPartLocationOutputTypeDef,
+        "properties": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DocumentationPartTypeDef = TypedDict(
+    "DocumentationPartTypeDef",
+    {
+        "id": str,
+        "location": DocumentationPartLocationOutputTypeDef,
+        "properties": str,
+    },
+    total=False,
+)
+
 DocumentationVersionsTypeDef = TypedDict(
     "DocumentationVersionsTypeDef",
     {
         "position": str,
         "items": List[DocumentationVersionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RestApiResponseMetadataTypeDef = TypedDict(
+    "RestApiResponseMetadataTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "description": str,
+        "createdDate": datetime,
+        "version": str,
+        "warnings": List[str],
+        "binaryMediaTypes": List[str],
+        "minimumCompressionSize": int,
+        "apiKeySource": ApiKeySourceTypeType,
+        "endpointConfiguration": EndpointConfigurationOutputTypeDef,
+        "policy": str,
+        "tags": Dict[str, str],
+        "disableExecuteApiEndpoint": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RestApiTypeDef = TypedDict(
+    "RestApiTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "description": str,
+        "createdDate": datetime,
+        "version": str,
+        "warnings": List[str],
+        "binaryMediaTypes": List[str],
+        "minimumCompressionSize": int,
+        "apiKeySource": ApiKeySourceTypeType,
+        "endpointConfiguration": EndpointConfigurationOutputTypeDef,
+        "policy": str,
+        "tags": Dict[str, str],
+        "disableExecuteApiEndpoint": bool,
+    },
+    total=False,
+)
+
 DomainNameResponseMetadataTypeDef = TypedDict(
     "DomainNameResponseMetadataTypeDef",
     {
         "domainName": str,
         "certificateName": str,
         "certificateArn": str,
         "certificateUploadDate": datetime,
         "regionalDomainName": str,
         "regionalHostedZoneId": str,
         "regionalCertificateName": str,
         "regionalCertificateArn": str,
         "distributionDomainName": str,
         "distributionHostedZoneId": str,
-        "endpointConfiguration": EndpointConfigurationTypeDef,
+        "endpointConfiguration": EndpointConfigurationOutputTypeDef,
         "domainNameStatus": DomainNameStatusType,
         "domainNameStatusMessage": str,
         "securityPolicy": SecurityPolicyType,
         "tags": Dict[str, str],
         "mutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "ownershipVerificationCertificateArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -2681,15 +2767,15 @@
         "certificateUploadDate": datetime,
         "regionalDomainName": str,
         "regionalHostedZoneId": str,
         "regionalCertificateName": str,
         "regionalCertificateArn": str,
         "distributionDomainName": str,
         "distributionHostedZoneId": str,
-        "endpointConfiguration": EndpointConfigurationTypeDef,
+        "endpointConfiguration": EndpointConfigurationOutputTypeDef,
         "domainNameStatus": DomainNameStatusType,
         "domainNameStatusMessage": str,
         "securityPolicy": SecurityPolicyType,
         "tags": Dict[str, str],
         "mutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "ownershipVerificationCertificateArn": str,
     },
@@ -2718,15 +2804,15 @@
         "requestTemplates": Dict[str, str],
         "passthroughBehavior": str,
         "contentHandling": ContentHandlingStrategyType,
         "timeoutInMillis": int,
         "cacheNamespace": str,
         "cacheKeyParameters": List[str],
         "integrationResponses": Dict[str, IntegrationResponseTypeDef],
-        "tlsConfig": TlsConfigTypeDef,
+        "tlsConfig": TlsConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
@@ -2740,68 +2826,34 @@
         "requestTemplates": Dict[str, str],
         "passthroughBehavior": str,
         "contentHandling": ContentHandlingStrategyType,
         "timeoutInMillis": int,
         "cacheNamespace": str,
         "cacheKeyParameters": List[str],
         "integrationResponses": Dict[str, IntegrationResponseTypeDef],
-        "tlsConfig": TlsConfigTypeDef,
+        "tlsConfig": TlsConfigOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredPutIntegrationRequestRequestTypeDef = TypedDict(
-    "_RequiredPutIntegrationRequestRequestTypeDef",
-    {
-        "restApiId": str,
-        "resourceId": str,
-        "httpMethod": str,
-        "type": IntegrationTypeType,
-    },
-)
-_OptionalPutIntegrationRequestRequestTypeDef = TypedDict(
-    "_OptionalPutIntegrationRequestRequestTypeDef",
-    {
-        "integrationHttpMethod": str,
-        "uri": str,
-        "connectionType": ConnectionTypeType,
-        "connectionId": str,
-        "credentials": str,
-        "requestParameters": Mapping[str, str],
-        "requestTemplates": Mapping[str, str],
-        "passthroughBehavior": str,
-        "cacheNamespace": str,
-        "cacheKeyParameters": Sequence[str],
-        "contentHandling": ContentHandlingStrategyType,
-        "timeoutInMillis": int,
-        "tlsConfig": TlsConfigTypeDef,
-    },
-    total=False,
-)
-
-class PutIntegrationRequestRequestTypeDef(
-    _RequiredPutIntegrationRequestRequestTypeDef, _OptionalPutIntegrationRequestRequestTypeDef
-):
-    pass
-
 StageResponseMetadataTypeDef = TypedDict(
     "StageResponseMetadataTypeDef",
     {
         "deploymentId": str,
         "clientCertificateId": str,
         "stageName": str,
         "description": str,
         "cacheClusterEnabled": bool,
         "cacheClusterSize": CacheClusterSizeType,
         "cacheClusterStatus": CacheClusterStatusType,
         "methodSettings": Dict[str, MethodSettingTypeDef],
         "variables": Dict[str, str],
         "documentationVersion": str,
         "accessLogSettings": AccessLogSettingsTypeDef,
-        "canarySettings": CanarySettingsTypeDef,
+        "canarySettings": CanarySettingsOutputTypeDef,
         "tracingEnabled": bool,
         "webAclArn": str,
         "tags": Dict[str, str],
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2817,15 +2869,15 @@
         "cacheClusterEnabled": bool,
         "cacheClusterSize": CacheClusterSizeType,
         "cacheClusterStatus": CacheClusterStatusType,
         "methodSettings": Dict[str, MethodSettingTypeDef],
         "variables": Dict[str, str],
         "documentationVersion": str,
         "accessLogSettings": AccessLogSettingsTypeDef,
-        "canarySettings": CanarySettingsTypeDef,
+        "canarySettings": CanarySettingsOutputTypeDef,
         "tracingEnabled": bool,
         "webAclArn": str,
         "tags": Dict[str, str],
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
     },
     total=False,
@@ -3272,14 +3324,48 @@
 )
 
 class UpdateVpcLinkRequestRequestTypeDef(
     _RequiredUpdateVpcLinkRequestRequestTypeDef, _OptionalUpdateVpcLinkRequestRequestTypeDef
 ):
     pass
 
+_RequiredPutIntegrationRequestRequestTypeDef = TypedDict(
+    "_RequiredPutIntegrationRequestRequestTypeDef",
+    {
+        "restApiId": str,
+        "resourceId": str,
+        "httpMethod": str,
+        "type": IntegrationTypeType,
+    },
+)
+_OptionalPutIntegrationRequestRequestTypeDef = TypedDict(
+    "_OptionalPutIntegrationRequestRequestTypeDef",
+    {
+        "integrationHttpMethod": str,
+        "uri": str,
+        "connectionType": ConnectionTypeType,
+        "connectionId": str,
+        "credentials": str,
+        "requestParameters": Mapping[str, str],
+        "requestTemplates": Mapping[str, str],
+        "passthroughBehavior": str,
+        "cacheNamespace": str,
+        "cacheKeyParameters": Sequence[str],
+        "contentHandling": ContentHandlingStrategyType,
+        "timeoutInMillis": int,
+        "tlsConfig": TlsConfigTypeDef,
+    },
+    total=False,
+)
+
+class PutIntegrationRequestRequestTypeDef(
+    _RequiredPutIntegrationRequestRequestTypeDef, _OptionalPutIntegrationRequestRequestTypeDef
+):
+    pass
+
 RequestValidatorsTypeDef = TypedDict(
     "RequestValidatorsTypeDef",
     {
         "position": str,
         "items": List[RequestValidatorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3321,14 +3407,44 @@
     {
         "position": str,
         "items": List[VpcLinkTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+UsagePlanResponseMetadataTypeDef = TypedDict(
+    "UsagePlanResponseMetadataTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "description": str,
+        "apiStages": List[ApiStageOutputTypeDef],
+        "throttle": ThrottleSettingsOutputTypeDef,
+        "quota": QuotaSettingsOutputTypeDef,
+        "productCode": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UsagePlanTypeDef = TypedDict(
+    "UsagePlanTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "description": str,
+        "apiStages": List[ApiStageOutputTypeDef],
+        "throttle": ThrottleSettingsOutputTypeDef,
+        "quota": QuotaSettingsOutputTypeDef,
+        "productCode": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredCreateUsagePlanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUsagePlanRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateUsagePlanRequestRequestTypeDef = TypedDict(
@@ -3344,44 +3460,23 @@
 )
 
 class CreateUsagePlanRequestRequestTypeDef(
     _RequiredCreateUsagePlanRequestRequestTypeDef, _OptionalCreateUsagePlanRequestRequestTypeDef
 ):
     pass
 
-UsagePlanResponseMetadataTypeDef = TypedDict(
-    "UsagePlanResponseMetadataTypeDef",
+DeploymentsTypeDef = TypedDict(
+    "DeploymentsTypeDef",
     {
-        "id": str,
-        "name": str,
-        "description": str,
-        "apiStages": List[ApiStageTypeDef],
-        "throttle": ThrottleSettingsTypeDef,
-        "quota": QuotaSettingsTypeDef,
-        "productCode": str,
-        "tags": Dict[str, str],
+        "position": str,
+        "items": List[DeploymentTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UsagePlanTypeDef = TypedDict(
-    "UsagePlanTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "description": str,
-        "apiStages": List[ApiStageTypeDef],
-        "throttle": ThrottleSettingsTypeDef,
-        "quota": QuotaSettingsTypeDef,
-        "productCode": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 DocumentationPartsTypeDef = TypedDict(
     "DocumentationPartsTypeDef",
     {
         "position": str,
         "items": List[DocumentationPartTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3392,23 +3487,14 @@
     {
         "position": str,
         "items": List[RestApiTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeploymentsTypeDef = TypedDict(
-    "DeploymentsTypeDef",
-    {
-        "position": str,
-        "items": List[DeploymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DomainNamesTypeDef = TypedDict(
     "DomainNamesTypeDef",
     {
         "position": str,
         "items": List[DomainNameTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway.egg-info/PKG-INFO` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigateway
-Version: 1.28.0
-Summary: Type annotations for boto3.APIGateway 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.APIGateway 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-apigateway"></a>
 
 # mypy-boto3-apigateway
 
 [![PyPI - mypy-boto3-apigateway](https://img.shields.io/pypi/v/mypy-boto3-apigateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apigateway?color=blue)](https://pypistats.org/packages/mypy-boto3-apigateway)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigateway)](https://pepy.tech/project/mypy-boto3-apigateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.APIGateway 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
+[boto3.APIGateway 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
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
 [mypy-boto3-apigateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/).
 
 See how it helps to find and fix potential bugs:
 
@@ -405,22 +405,24 @@
 
 `mypy_boto3_apigateway.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigateway.type_defs import (
     AccessLogSettingsTypeDef,
-    ThrottleSettingsTypeDef,
+    ThrottleSettingsOutputTypeDef,
     ApiKeyIdsTypeDef,
     ApiKeyResponseMetadataTypeDef,
     ApiKeyTypeDef,
+    ThrottleSettingsTypeDef,
     AuthorizerResponseMetadataTypeDef,
     AuthorizerTypeDef,
     BasePathMappingResponseMetadataTypeDef,
     BasePathMappingTypeDef,
+    CanarySettingsOutputTypeDef,
     CanarySettingsTypeDef,
     ClientCertificateResponseMetadataTypeDef,
     ClientCertificateTypeDef,
     StageKeyTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
     CreateBasePathMappingRequestRequestTypeDef,
     DeploymentCanarySettingsTypeDef,
@@ -453,16 +455,18 @@
     DeleteRestApiRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteUsagePlanKeyRequestRequestTypeDef,
     DeleteUsagePlanRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     MethodSnapshotTypeDef,
     DocumentationPartIdsTypeDef,
+    DocumentationPartLocationOutputTypeDef,
     DocumentationVersionResponseMetadataTypeDef,
     DocumentationVersionTypeDef,
+    EndpointConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportResponseTypeDef,
     FlushStageAuthorizersCacheRequestRequestTypeDef,
     FlushStageCacheRequestRequestTypeDef,
     GatewayResponseResponseMetadataTypeDef,
     GatewayResponseTypeDef,
@@ -530,28 +534,30 @@
     GetVpcLinkRequestRequestTypeDef,
     GetVpcLinksRequestGetVpcLinksPaginateTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     ImportApiKeysRequestRequestTypeDef,
     ImportDocumentationPartsRequestRequestTypeDef,
     ImportRestApiRequestRequestTypeDef,
     IntegrationResponseTypeDef,
-    TlsConfigTypeDef,
+    TlsConfigOutputTypeDef,
     IntegrationResponseResponseMetadataTypeDef,
     MethodResponseTypeDef,
     MethodResponseResponseMetadataTypeDef,
     MethodSettingTypeDef,
     ModelResponseMetadataTypeDef,
     ModelTypeDef,
     PaginatorConfigTypeDef,
     PatchOperationTypeDef,
     PutGatewayResponseRequestRequestTypeDef,
+    TlsConfigTypeDef,
     PutIntegrationResponseRequestRequestTypeDef,
     PutMethodRequestRequestTypeDef,
     PutMethodResponseRequestRequestTypeDef,
     PutRestApiRequestRequestTypeDef,
+    QuotaSettingsOutputTypeDef,
     RequestValidatorResponseMetadataTypeDef,
     RequestValidatorTypeDef,
     ResponseMetadataTypeDef,
     SdkConfigurationPropertyTypeDef,
     SdkResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TagsTypeDef,
@@ -563,38 +569,38 @@
     UntagResourceRequestRequestTypeDef,
     UsagePlanKeyResponseMetadataTypeDef,
     UsagePlanKeyTypeDef,
     UsageTypeDef,
     VpcLinkResponseMetadataTypeDef,
     VpcLinkTypeDef,
     AccountTypeDef,
-    ApiStageTypeDef,
+    ApiStageOutputTypeDef,
     ApiKeysTypeDef,
+    ApiStageTypeDef,
     AuthorizersTypeDef,
     BasePathMappingsTypeDef,
     CreateStageRequestRequestTypeDef,
     ClientCertificatesTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     CreateDocumentationPartRequestRequestTypeDef,
-    DocumentationPartResponseMetadataTypeDef,
-    DocumentationPartTypeDef,
     CreateRestApiRequestRequestTypeDef,
-    RestApiResponseMetadataTypeDef,
-    RestApiTypeDef,
     CreateDomainNameRequestRequestTypeDef,
     DeploymentResponseMetadataTypeDef,
     DeploymentTypeDef,
+    DocumentationPartResponseMetadataTypeDef,
+    DocumentationPartTypeDef,
     DocumentationVersionsTypeDef,
+    RestApiResponseMetadataTypeDef,
+    RestApiTypeDef,
     DomainNameResponseMetadataTypeDef,
     DomainNameTypeDef,
     GatewayResponsesTypeDef,
     IntegrationResponseMetadataTypeDef,
     IntegrationTypeDef,
-    PutIntegrationRequestRequestTypeDef,
     StageResponseMetadataTypeDef,
     StageTypeDef,
     ModelsTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateApiKeyRequestRequestTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
     UpdateBasePathMappingRequestRequestTypeDef,
@@ -612,25 +618,26 @@
     UpdateRequestValidatorRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateRestApiRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
     UpdateUsagePlanRequestRequestTypeDef,
     UpdateUsageRequestRequestTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
+    PutIntegrationRequestRequestTypeDef,
     RequestValidatorsTypeDef,
     SdkTypeResponseMetadataTypeDef,
     SdkTypeTypeDef,
     UsagePlanKeysTypeDef,
     VpcLinksTypeDef,
-    CreateUsagePlanRequestRequestTypeDef,
     UsagePlanResponseMetadataTypeDef,
     UsagePlanTypeDef,
+    CreateUsagePlanRequestRequestTypeDef,
+    DeploymentsTypeDef,
     DocumentationPartsTypeDef,
     RestApisTypeDef,
-    DeploymentsTypeDef,
     DomainNamesTypeDef,
     MethodResponseMetadataTypeDef,
     MethodTypeDef,
     StagesTypeDef,
     SdkTypesTypeDef,
     UsagePlansTypeDef,
     ResourceResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-apigateway-1.28.0/mypy_boto3_apigateway.egg-info/SOURCES.txt` & `mypy-boto3-apigateway-1.28.12/mypy_boto3_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.0/setup.py` & `mypy-boto3-apigateway-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apigateway",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_apigateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.APIGateway 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.APIGateway 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

