# Comparing `tmp/mypy-boto3-service-quotas-1.28.0.tar.gz` & `tmp/mypy-boto3-service-quotas-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-service-quotas-1.28.0.tar", last modified: Thu Jul  6 21:00:36 2023, max compression
+gzip compressed data, was "mypy-boto3-service-quotas-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
```

## Comparing `mypy-boto3-service-quotas-1.28.0.tar` & `mypy-boto3-service-quotas-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:36.702429 mypy-boto3-service-quotas-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-07-06 21:00:36.702429 mypy-boto3-service-quotas-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:36.686429 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17562 2023-07-06 20:55:33.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17549 2023-07-06 20:55:33.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:36.702429 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-07-06 21:00:36.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 21:00:36.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:36.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:36.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:36.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 21:00:36.000000 mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:36.702429 mypy-boto3-service-quotas-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 20:55:32.000000 mypy-boto3-service-quotas-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.481290 mypy-boto3-service-quotas-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-07-27 11:49:38.481290 mypy-boto3-service-quotas-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.477290 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17651 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.481290 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-07-27 11:49:38.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 11:49:38.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:38.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.481290 mypy-boto3-service-quotas-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 11:46:38.000000 mypy-boto3-service-quotas-1.28.12/setup.py
```

### Comparing `mypy-boto3-service-quotas-1.28.0/LICENSE` & `mypy-boto3-service-quotas-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.0/PKG-INFO` & `mypy-boto3-service-quotas-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-service-quotas
-Version: 1.28.0
-Summary: Type annotations for boto3.ServiceQuotas 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ServiceQuotas 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-service-quotas"></a>
 
 # mypy-boto3-service-quotas
 
 [![PyPI - mypy-boto3-service-quotas](https://img.shields.io/pypi/v/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-service-quotas?color=blue)](https://pypistats.org/packages/mypy-boto3-service-quotas)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-service-quotas)](https://pepy.tech/project/mypy-boto3-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceQuotas 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[boto3.ServiceQuotas 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [mypy-boto3-service-quotas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,53 +354,54 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_service_quotas.type_defs import (
     DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ErrorReasonTypeDef,
     GetAWSDefaultServiceQuotaRequestRequestTypeDef,
-    GetAssociationForServiceQuotaTemplateResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetRequestedServiceQuotaChangeRequestRequestTypeDef,
     RequestedServiceQuotaChangeTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ServiceQuotaIncreaseRequestInTemplateTypeDef,
     GetServiceQuotaRequestRequestTypeDef,
-    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAWSDefaultServiceQuotasRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
-    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
     ListServiceQuotasRequestRequestTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     MetricInfoTypeDef,
-    PaginatorConfigTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
     QuotaPeriodTypeDef,
     RequestServiceQuotaIncreaseRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    TagTypeDef,
     UntagResourceRequestRequestTypeDef,
+    GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
     RequestServiceQuotaIncreaseResponseTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef,
+    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
+    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
+    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ServiceQuotaTypeDef,
+    TagResourceRequestRequestTypeDef,
     GetAWSDefaultServiceQuotaResponseTypeDef,
     GetServiceQuotaResponseTypeDef,
     ListAWSDefaultServiceQuotasResponseTypeDef,
     ListServiceQuotasResponseTypeDef,
 )
```

### Comparing `mypy-boto3-service-quotas-1.28.0/README.md` & `mypy-boto3-service-quotas-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-service-quotas"></a>
 
 # mypy-boto3-service-quotas
 
 [![PyPI - mypy-boto3-service-quotas](https://img.shields.io/pypi/v/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-service-quotas?color=blue)](https://pypistats.org/packages/mypy-boto3-service-quotas)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-service-quotas)](https://pepy.tech/project/mypy-boto3-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceQuotas 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[boto3.ServiceQuotas 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [mypy-boto3-service-quotas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,53 +322,54 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_service_quotas.type_defs import (
     DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ErrorReasonTypeDef,
     GetAWSDefaultServiceQuotaRequestRequestTypeDef,
-    GetAssociationForServiceQuotaTemplateResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetRequestedServiceQuotaChangeRequestRequestTypeDef,
     RequestedServiceQuotaChangeTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ServiceQuotaIncreaseRequestInTemplateTypeDef,
     GetServiceQuotaRequestRequestTypeDef,
-    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAWSDefaultServiceQuotasRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
-    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
     ListServiceQuotasRequestRequestTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     MetricInfoTypeDef,
-    PaginatorConfigTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
     QuotaPeriodTypeDef,
     RequestServiceQuotaIncreaseRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    TagTypeDef,
     UntagResourceRequestRequestTypeDef,
+    GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
     RequestServiceQuotaIncreaseResponseTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef,
+    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
+    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
+    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ServiceQuotaTypeDef,
+    TagResourceRequestRequestTypeDef,
     GetAWSDefaultServiceQuotaResponseTypeDef,
     GetServiceQuotaResponseTypeDef,
     ListAWSDefaultServiceQuotasResponseTypeDef,
     ListServiceQuotasResponseTypeDef,
 )
```

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/__init__.py` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/__init__.pyi` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/__main__.py` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServiceQuotas 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ServiceQuotas 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas\nOther"
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

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/client.py` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/client.pyi` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/literals.py` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,15 @@
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
@@ -261,26 +262,28 @@
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

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/literals.pyi` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
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
@@ -259,26 +260,28 @@
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

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/paginator.py` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 class ListAWSDefaultServiceQuotasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listawsdefaultservicequotaspaginator)
     """
 
     def paginate(
-        self, *, ServiceCode: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServiceCode: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAWSDefaultServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listawsdefaultservicequotaspaginator)
         """
 
 
@@ -86,15 +86,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         Status: RequestStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRequestedServiceQuotaChangeHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listrequestedservicequotachangehistorypaginator)
         """
 
 
@@ -106,15 +106,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         QuotaCode: str,
         Status: RequestStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistoryByQuota.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listrequestedservicequotachangehistorybyquotapaginator)
         """
 
 
@@ -125,43 +125,43 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         AwsRegion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotaIncreaseRequestsInTemplate.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaincreaserequestsintemplatepaginator)
         """
 
 
 class ListServiceQuotasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaspaginator)
     """
 
     def paginate(
-        self, *, ServiceCode: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServiceCode: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaspaginator)
         """
 
 
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicespaginator)
         """
```

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/paginator.pyi` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class ListAWSDefaultServiceQuotasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listawsdefaultservicequotaspaginator)
     """
 
     def paginate(
-        self, *, ServiceCode: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServiceCode: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAWSDefaultServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListAWSDefaultServiceQuotas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listawsdefaultservicequotaspaginator)
         """
 
 class ListRequestedServiceQuotaChangeHistoryPaginator(Paginator):
@@ -82,15 +82,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         Status: RequestStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRequestedServiceQuotaChangeHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listrequestedservicequotachangehistorypaginator)
         """
 
 class ListRequestedServiceQuotaChangeHistoryByQuotaPaginator(Paginator):
@@ -101,15 +101,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         QuotaCode: str,
         Status: RequestStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListRequestedServiceQuotaChangeHistoryByQuota.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listrequestedservicequotachangehistorybyquotapaginator)
         """
 
 class ListServiceQuotaIncreaseRequestsInTemplatePaginator(Paginator):
@@ -119,41 +119,41 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         AwsRegion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotaIncreaseRequestsInTemplate.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaincreaserequestsintemplatepaginator)
         """
 
 class ListServiceQuotasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaspaginator)
     """
 
     def paginate(
-        self, *, ServiceCode: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServiceCode: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceQuotasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServiceQuotas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicequotaspaginator)
         """
 
 class ListServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/paginators/#listservicespaginator)
         """
```

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/type_defs.py` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,53 +28,54 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ErrorReasonTypeDef",
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
-    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     "RequestedServiceQuotaChangeTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ServiceQuotaIncreaseRequestInTemplateTypeDef",
     "GetServiceQuotaRequestRequestTypeDef",
-    "ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAWSDefaultServiceQuotasRequestRequestTypeDef",
-    "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
-    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
-    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
-    "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
     "ListServiceQuotasRequestRequestTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ServiceInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "MetricInfoTypeDef",
-    "PaginatorConfigTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     "QuotaPeriodTypeDef",
     "RequestServiceQuotaIncreaseRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     "RequestServiceQuotaIncreaseResponseTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef",
+    "ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
+    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
+    "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "ServiceQuotaTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     "GetServiceQuotaResponseTypeDef",
     "ListAWSDefaultServiceQuotasResponseTypeDef",
     "ListServiceQuotasResponseTypeDef",
 )
 
 DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef = TypedDict(
@@ -99,19 +100,22 @@
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
 
-GetAssociationForServiceQuotaTemplateResponseTypeDef = TypedDict(
-    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ServiceQuotaTemplateAssociationStatus": ServiceQuotaTemplateAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetRequestedServiceQuotaChangeRequestRequestTypeDef = TypedDict(
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     {
         "RequestId": str,
@@ -167,36 +171,24 @@
     "GetServiceQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
 
-_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
-    "_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
-    {
-        "ServiceCode": str,
-    },
-)
-_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
-    "_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
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
-class ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef(
-    _RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-    _OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef = TypedDict(
     "_RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalListAWSDefaultServiceQuotasRequestRequestTypeDef = TypedDict(
@@ -212,38 +204,14 @@
 class ListAWSDefaultServiceQuotasRequestRequestTypeDef(
     _RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef,
     _OptionalListAWSDefaultServiceQuotasRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
-    "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "QuotaCode": str,
-    },
-)
-_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
-    "_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    {
-        "Status": RequestStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef(
-    _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-    _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef = TypedDict(
     "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
@@ -261,78 +229,36 @@
 class ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef(
     _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
     _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
 ):
     pass
 
 
-ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef = TypedDict(
-    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "Status": RequestStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "Status": RequestStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef = TypedDict(
-    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "AwsRegion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef = TypedDict(
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "AwsRegion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
-    "_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    {
-        "ServiceCode": str,
-    },
-)
-_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
-    "_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListServiceQuotasRequestListServiceQuotasPaginateTypeDef(
-    _RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-    _OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListServiceQuotasRequestRequestTypeDef = TypedDict(
     "_RequiredListServiceQuotasRequestRequestTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalListServiceQuotasRequestRequestTypeDef = TypedDict(
@@ -347,22 +273,14 @@
 
 class ListServiceQuotasRequestRequestTypeDef(
     _RequiredListServiceQuotasRequestRequestTypeDef, _OptionalListServiceQuotasRequestRequestTypeDef
 ):
     pass
 
 
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -380,16 +298,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 MetricInfoTypeDef = TypedDict(
@@ -399,24 +317,14 @@
         "MetricName": str,
         "MetricDimensions": Dict[str, str],
         "MetricStatisticRecommendation": str,
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
 PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef = TypedDict(
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     {
         "QuotaCode": str,
         "ServiceCode": str,
         "AwsRegion": str,
         "DesiredValue": float,
@@ -437,116 +345,209 @@
     {
         "ServiceCode": str,
         "QuotaCode": str,
         "DesiredValue": float,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Key": str,
+        "Value": str,
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+GetAssociationForServiceQuotaTemplateResponseTypeDef = TypedDict(
+    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+    {
+        "ServiceQuotaTemplateAssociationStatus": ServiceQuotaTemplateAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetRequestedServiceQuotaChangeResponseTypeDef = TypedDict(
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     {
         "RequestedQuota": RequestedServiceQuotaChangeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     {
         "NextToken": str,
         "RequestedQuotas": List[RequestedServiceQuotaChangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRequestedServiceQuotaChangeHistoryResponseTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     {
         "NextToken": str,
         "RequestedQuotas": List[RequestedServiceQuotaChangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RequestServiceQuotaIncreaseResponseTypeDef = TypedDict(
     "RequestServiceQuotaIncreaseResponseTypeDef",
     {
         "RequestedQuota": RequestedServiceQuotaChangeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef = TypedDict(
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplate": ServiceQuotaIncreaseRequestInTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef = TypedDict(
     "ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplateList": List[
             ServiceQuotaIncreaseRequestInTemplateTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef = TypedDict(
     "PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplate": ServiceQuotaIncreaseRequestInTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
+    "_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    {
+        "ServiceCode": str,
+    },
+)
+_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
+    "_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef(
+    _RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    _OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
+    "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "QuotaCode": str,
+    },
+)
+_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
+    "_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    {
+        "Status": RequestStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef(
+    _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+    _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+):
+    pass
+
+
+ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef = TypedDict(
+    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "Status": RequestStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef = TypedDict(
+    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "AwsRegion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
+    "_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    {
+        "ServiceCode": str,
+    },
+)
+_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
+    "_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListServiceQuotasRequestListServiceQuotasPaginateTypeDef(
+    _RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+    _OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+):
+    pass
+
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "NextToken": str,
         "Services": List[ServiceInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceQuotaTypeDef = TypedDict(
     "ServiceQuotaTypeDef",
     {
         "ServiceCode": str,
@@ -561,40 +562,48 @@
         "UsageMetric": MetricInfoTypeDef,
         "Period": QuotaPeriodTypeDef,
         "ErrorReason": ErrorReasonTypeDef,
     },
     total=False,
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 GetAWSDefaultServiceQuotaResponseTypeDef = TypedDict(
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceQuotaResponseTypeDef = TypedDict(
     "GetServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAWSDefaultServiceQuotasResponseTypeDef = TypedDict(
     "ListAWSDefaultServiceQuotasResponseTypeDef",
     {
         "NextToken": str,
         "Quotas": List[ServiceQuotaTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceQuotasResponseTypeDef = TypedDict(
     "ListServiceQuotasResponseTypeDef",
     {
         "NextToken": str,
         "Quotas": List[ServiceQuotaTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas/type_defs.pyi` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,53 +27,54 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ErrorReasonTypeDef",
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
-    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     "RequestedServiceQuotaChangeTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef",
     "ServiceQuotaIncreaseRequestInTemplateTypeDef",
     "GetServiceQuotaRequestRequestTypeDef",
-    "ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAWSDefaultServiceQuotasRequestRequestTypeDef",
-    "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
-    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
-    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
-    "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
     "ListServiceQuotasRequestRequestTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ServiceInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "MetricInfoTypeDef",
-    "PaginatorConfigTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     "QuotaPeriodTypeDef",
     "RequestServiceQuotaIncreaseRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     "RequestServiceQuotaIncreaseResponseTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef",
+    "ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
+    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
+    "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "ServiceQuotaTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     "GetServiceQuotaResponseTypeDef",
     "ListAWSDefaultServiceQuotasResponseTypeDef",
     "ListServiceQuotasResponseTypeDef",
 )
 
 DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef = TypedDict(
@@ -98,19 +99,22 @@
     "GetAWSDefaultServiceQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
 
-GetAssociationForServiceQuotaTemplateResponseTypeDef = TypedDict(
-    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ServiceQuotaTemplateAssociationStatus": ServiceQuotaTemplateAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetRequestedServiceQuotaChangeRequestRequestTypeDef = TypedDict(
     "GetRequestedServiceQuotaChangeRequestRequestTypeDef",
     {
         "RequestId": str,
@@ -166,34 +170,24 @@
     "GetServiceQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
 
-_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
-    "_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
-    {
-        "ServiceCode": str,
-    },
-)
-_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
-    "_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
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
 
-class ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef(
-    _RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-    _OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
-):
-    pass
-
 _RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef = TypedDict(
     "_RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalListAWSDefaultServiceQuotasRequestRequestTypeDef = TypedDict(
@@ -207,36 +201,14 @@
 
 class ListAWSDefaultServiceQuotasRequestRequestTypeDef(
     _RequiredListAWSDefaultServiceQuotasRequestRequestTypeDef,
     _OptionalListAWSDefaultServiceQuotasRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
-    "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "QuotaCode": str,
-    },
-)
-_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
-    "_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
-    {
-        "Status": RequestStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef(
-    _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-    _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
-):
-    pass
-
 _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef = TypedDict(
     "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "QuotaCode": str,
     },
 )
@@ -252,76 +224,36 @@
 
 class ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef(
     _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
     _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
 ):
     pass
 
-ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef = TypedDict(
-    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "Status": RequestStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "Status": RequestStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef = TypedDict(
-    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
-    {
-        "ServiceCode": str,
-        "AwsRegion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef = TypedDict(
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
     {
         "ServiceCode": str,
         "AwsRegion": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
-    "_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    {
-        "ServiceCode": str,
-    },
-)
-_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
-    "_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListServiceQuotasRequestListServiceQuotasPaginateTypeDef(
-    _RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-    _OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
-):
-    pass
-
 _RequiredListServiceQuotasRequestRequestTypeDef = TypedDict(
     "_RequiredListServiceQuotasRequestRequestTypeDef",
     {
         "ServiceCode": str,
     },
 )
 _OptionalListServiceQuotasRequestRequestTypeDef = TypedDict(
@@ -334,22 +266,14 @@
 )
 
 class ListServiceQuotasRequestRequestTypeDef(
     _RequiredListServiceQuotasRequestRequestTypeDef, _OptionalListServiceQuotasRequestRequestTypeDef
 ):
     pass
 
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -367,16 +291,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 MetricInfoTypeDef = TypedDict(
@@ -386,24 +310,14 @@
         "MetricName": str,
         "MetricDimensions": Dict[str, str],
         "MetricStatisticRecommendation": str,
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
 PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef = TypedDict(
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     {
         "QuotaCode": str,
         "ServiceCode": str,
         "AwsRegion": str,
         "DesiredValue": float,
@@ -424,116 +338,203 @@
     {
         "ServiceCode": str,
         "QuotaCode": str,
         "DesiredValue": float,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Key": str,
+        "Value": str,
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+GetAssociationForServiceQuotaTemplateResponseTypeDef = TypedDict(
+    "GetAssociationForServiceQuotaTemplateResponseTypeDef",
+    {
+        "ServiceQuotaTemplateAssociationStatus": ServiceQuotaTemplateAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetRequestedServiceQuotaChangeResponseTypeDef = TypedDict(
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     {
         "RequestedQuota": RequestedServiceQuotaChangeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     {
         "NextToken": str,
         "RequestedQuotas": List[RequestedServiceQuotaChangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRequestedServiceQuotaChangeHistoryResponseTypeDef = TypedDict(
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     {
         "NextToken": str,
         "RequestedQuotas": List[RequestedServiceQuotaChangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RequestServiceQuotaIncreaseResponseTypeDef = TypedDict(
     "RequestServiceQuotaIncreaseResponseTypeDef",
     {
         "RequestedQuota": RequestedServiceQuotaChangeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef = TypedDict(
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplate": ServiceQuotaIncreaseRequestInTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef = TypedDict(
     "ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplateList": List[
             ServiceQuotaIncreaseRequestInTemplateTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef = TypedDict(
     "PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef",
     {
         "ServiceQuotaIncreaseRequestInTemplate": ServiceQuotaIncreaseRequestInTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
+    "_RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    {
+        "ServiceCode": str,
+    },
+)
+_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef = TypedDict(
+    "_OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+class ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef(
+    _RequiredListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    _OptionalListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+):
+    pass
+
+_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
+    "_RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "QuotaCode": str,
+    },
+)
+_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef = TypedDict(
+    "_OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
+    {
+        "Status": RequestStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef(
+    _RequiredListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+    _OptionalListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+):
+    pass
+
+ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef = TypedDict(
+    "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "Status": RequestStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef = TypedDict(
+    "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
+    {
+        "ServiceCode": str,
+        "AwsRegion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
+    "_RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    {
+        "ServiceCode": str,
+    },
+)
+_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef = TypedDict(
+    "_OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListServiceQuotasRequestListServiceQuotasPaginateTypeDef(
+    _RequiredListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+    _OptionalListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+):
+    pass
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "NextToken": str,
         "Services": List[ServiceInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceQuotaTypeDef = TypedDict(
     "ServiceQuotaTypeDef",
     {
         "ServiceCode": str,
@@ -548,40 +549,48 @@
         "UsageMetric": MetricInfoTypeDef,
         "Period": QuotaPeriodTypeDef,
         "ErrorReason": ErrorReasonTypeDef,
     },
     total=False,
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 GetAWSDefaultServiceQuotaResponseTypeDef = TypedDict(
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceQuotaResponseTypeDef = TypedDict(
     "GetServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAWSDefaultServiceQuotasResponseTypeDef = TypedDict(
     "ListAWSDefaultServiceQuotasResponseTypeDef",
     {
         "NextToken": str,
         "Quotas": List[ServiceQuotaTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceQuotasResponseTypeDef = TypedDict(
     "ListServiceQuotasResponseTypeDef",
     {
         "NextToken": str,
         "Quotas": List[ServiceQuotaTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas.egg-info/PKG-INFO` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-service-quotas
-Version: 1.28.0
-Summary: Type annotations for boto3.ServiceQuotas 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ServiceQuotas 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-service-quotas"></a>
 
 # mypy-boto3-service-quotas
 
 [![PyPI - mypy-boto3-service-quotas](https://img.shields.io/pypi/v/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-service-quotas?color=blue)](https://pypistats.org/packages/mypy-boto3-service-quotas)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-service-quotas)](https://pepy.tech/project/mypy-boto3-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceQuotas 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[boto3.ServiceQuotas 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [mypy-boto3-service-quotas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,53 +354,54 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_service_quotas.type_defs import (
     DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ErrorReasonTypeDef,
     GetAWSDefaultServiceQuotaRequestRequestTypeDef,
-    GetAssociationForServiceQuotaTemplateResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetRequestedServiceQuotaChangeRequestRequestTypeDef,
     RequestedServiceQuotaChangeTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef,
     ServiceQuotaIncreaseRequestInTemplateTypeDef,
     GetServiceQuotaRequestRequestTypeDef,
-    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAWSDefaultServiceQuotasRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
-    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
-    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
-    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
     ListServiceQuotasRequestRequestTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     MetricInfoTypeDef,
-    PaginatorConfigTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
     QuotaPeriodTypeDef,
     RequestServiceQuotaIncreaseRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    TagTypeDef,
     UntagResourceRequestRequestTypeDef,
+    GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
     RequestServiceQuotaIncreaseResponseTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef,
+    ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef,
+    ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
+    ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
+    ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
+    ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ServiceQuotaTypeDef,
+    TagResourceRequestRequestTypeDef,
     GetAWSDefaultServiceQuotaResponseTypeDef,
     GetServiceQuotaResponseTypeDef,
     ListAWSDefaultServiceQuotasResponseTypeDef,
     ListServiceQuotasResponseTypeDef,
 )
```

### Comparing `mypy-boto3-service-quotas-1.28.0/mypy_boto3_service_quotas.egg-info/SOURCES.txt` & `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.0/setup.py` & `mypy-boto3-service-quotas-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-service-quotas",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_service_quotas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServiceQuotas 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ServiceQuotas 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

