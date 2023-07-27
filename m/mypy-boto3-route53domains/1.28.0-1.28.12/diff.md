# Comparing `tmp/mypy-boto3-route53domains-1.28.0.tar.gz` & `tmp/mypy-boto3-route53domains-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53domains-1.28.0.tar", last modified: Thu Jul  6 21:00:29 2023, max compression
+gzip compressed data, was "mypy-boto3-route53domains-1.28.12.tar", last modified: Thu Jul 27 11:49:33 2023, max compression
```

## Comparing `mypy-boto3-route53domains-1.28.0.tar` & `mypy-boto3-route53domains-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:29.366414 mypy-boto3-route53domains-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:40.000000 mypy-boto3-route53domains-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-07-06 21:00:29.366414 mypy-boto3-route53domains-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-07-06 20:53:40.000000 mypy-boto3-route53domains-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:29.358414 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-06 20:53:40.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-06 20:53:40.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:53:40.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28933 2023-07-06 20:53:41.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28888 2023-07-06 20:53:41.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-07-06 20:53:41.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-07-06 20:53:41.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-06 20:53:41.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-06 20:53:41.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:40.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27578 2023-07-06 20:53:42.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27557 2023-07-06 20:53:42.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:40.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:29.366414 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-07-06 21:00:29.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 21:00:29.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:29.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:29.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:29.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 21:00:29.000000 mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:29.366414 mypy-boto3-route53domains-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-06 20:53:40.000000 mypy-boto3-route53domains-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.037239 mypy-boto3-route53domains-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-07-27 11:49:33.033239 mypy-boto3-route53domains-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.029239 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28933 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28888 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-27 11:44:55.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-07-27 11:44:55.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28843 2023-07-27 11:44:55.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28820 2023-07-27 11:44:55.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.033239 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-07-27 11:49:32.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 11:49:32.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:32.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:32.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:33.037239 mypy-boto3-route53domains-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/setup.py
```

### Comparing `mypy-boto3-route53domains-1.28.0/LICENSE` & `mypy-boto3-route53domains-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.0/PKG-INFO` & `mypy-boto3-route53domains-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53domains
-Version: 1.28.0
-Summary: Type annotations for boto3.Route53Domains 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Route53Domains 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-route53domains"></a>
 
 # mypy-boto3-route53domains
 
 [![PyPI - mypy-boto3-route53domains](https://img.shields.io/pypi/v/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53domains?color=blue)](https://pypistats.org/packages/mypy-boto3-route53domains)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53domains)](https://pepy.tech/project/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,92 +345,96 @@
 
 `mypy_boto3_route53domains.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53domains.type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    ResponseMetadataTypeDef,
     DnssecSigningAttributesTypeDef,
-    AssociateDelegationSignerToDomainResponseTypeDef,
     BillingRecordTypeDef,
     CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef,
-    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityRequestRequestTypeDef,
-    CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityRequestRequestTypeDef,
     DomainTransferabilityTypeDef,
     ConsentTypeDef,
+    ExtraParamOutputTypeDef,
     ExtraParamTypeDef,
     DeleteDomainRequestRequestTypeDef,
-    DeleteDomainResponseTypeDef,
     DeleteTagsForDomainRequestRequestTypeDef,
     DisableDomainAutoRenewRequestRequestTypeDef,
     DisableDomainTransferLockRequestRequestTypeDef,
-    DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainRequestRequestTypeDef,
-    DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecKeyTypeDef,
     PriceWithCurrencyTypeDef,
     DomainSuggestionTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableDomainAutoRenewRequestRequestTypeDef,
     EnableDomainTransferLockRequestRequestTypeDef,
-    EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
     GetContactReachabilityStatusRequestRequestTypeDef,
-    GetContactReachabilityStatusResponseTypeDef,
     GetDomainDetailRequestRequestTypeDef,
-    NameserverTypeDef,
+    NameserverOutputTypeDef,
     GetDomainSuggestionsRequestRequestTypeDef,
     GetOperationDetailRequestRequestTypeDef,
-    GetOperationDetailResponseTypeDef,
+    PaginatorConfigTypeDef,
     SortConditionTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
-    ListPricesRequestListPricesPaginateTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
-    TagTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
+    NameserverTypeDef,
     PushDomainRequestRequestTypeDef,
-    RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainRequestRequestTypeDef,
-    RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
-    ResendContactReachabilityEmailResponseTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
+    TagTypeDef,
+    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
+    UpdateDomainContactPrivacyRequestRequestTypeDef,
+    ViewBillingRequestRequestTypeDef,
+    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    AssociateDelegationSignerToDomainResponseTypeDef,
+    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
+    CheckDomainAvailabilityResponseTypeDef,
+    DeleteDomainResponseTypeDef,
+    DisableDomainTransferLockResponseTypeDef,
+    DisassociateDelegationSignerFromDomainResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnableDomainTransferLockResponseTypeDef,
+    GetContactReachabilityStatusResponseTypeDef,
+    GetOperationDetailResponseTypeDef,
+    RegisterDomainResponseTypeDef,
+    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    RenewDomainResponseTypeDef,
+    ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     TransferDomainResponseTypeDef,
-    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
-    UpdateDomainContactPrivacyRequestRequestTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
-    ViewBillingRequestRequestTypeDef,
-    ViewBillingRequestViewBillingPaginateTypeDef,
     AssociateDelegationSignerToDomainRequestRequestTypeDef,
     ViewBillingResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
+    ContactDetailOutputTypeDef,
     ContactDetailTypeDef,
     DomainPriceTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     ListDomainsResponseTypeDef,
-    UpdateDomainNameserversRequestRequestTypeDef,
+    ListOperationsRequestListOperationsPaginateTypeDef,
+    ListPricesRequestListPricesPaginateTypeDef,
+    ViewBillingRequestViewBillingPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
+    UpdateDomainNameserversRequestRequestTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
     GetDomainDetailResponseTypeDef,
     RegisterDomainRequestRequestTypeDef,
     TransferDomainRequestRequestTypeDef,
     UpdateDomainContactRequestRequestTypeDef,
     ListPricesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-route53domains-1.28.0/README.md` & `mypy-boto3-route53domains-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-route53domains"></a>
 
 # mypy-boto3-route53domains
 
 [![PyPI - mypy-boto3-route53domains](https://img.shields.io/pypi/v/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53domains?color=blue)](https://pypistats.org/packages/mypy-boto3-route53domains)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53domains)](https://pepy.tech/project/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,92 +313,96 @@
 
 `mypy_boto3_route53domains.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53domains.type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    ResponseMetadataTypeDef,
     DnssecSigningAttributesTypeDef,
-    AssociateDelegationSignerToDomainResponseTypeDef,
     BillingRecordTypeDef,
     CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef,
-    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityRequestRequestTypeDef,
-    CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityRequestRequestTypeDef,
     DomainTransferabilityTypeDef,
     ConsentTypeDef,
+    ExtraParamOutputTypeDef,
     ExtraParamTypeDef,
     DeleteDomainRequestRequestTypeDef,
-    DeleteDomainResponseTypeDef,
     DeleteTagsForDomainRequestRequestTypeDef,
     DisableDomainAutoRenewRequestRequestTypeDef,
     DisableDomainTransferLockRequestRequestTypeDef,
-    DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainRequestRequestTypeDef,
-    DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecKeyTypeDef,
     PriceWithCurrencyTypeDef,
     DomainSuggestionTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableDomainAutoRenewRequestRequestTypeDef,
     EnableDomainTransferLockRequestRequestTypeDef,
-    EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
     GetContactReachabilityStatusRequestRequestTypeDef,
-    GetContactReachabilityStatusResponseTypeDef,
     GetDomainDetailRequestRequestTypeDef,
-    NameserverTypeDef,
+    NameserverOutputTypeDef,
     GetDomainSuggestionsRequestRequestTypeDef,
     GetOperationDetailRequestRequestTypeDef,
-    GetOperationDetailResponseTypeDef,
+    PaginatorConfigTypeDef,
     SortConditionTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
-    ListPricesRequestListPricesPaginateTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
-    TagTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
+    NameserverTypeDef,
     PushDomainRequestRequestTypeDef,
-    RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainRequestRequestTypeDef,
-    RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
-    ResendContactReachabilityEmailResponseTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
+    TagTypeDef,
+    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
+    UpdateDomainContactPrivacyRequestRequestTypeDef,
+    ViewBillingRequestRequestTypeDef,
+    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    AssociateDelegationSignerToDomainResponseTypeDef,
+    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
+    CheckDomainAvailabilityResponseTypeDef,
+    DeleteDomainResponseTypeDef,
+    DisableDomainTransferLockResponseTypeDef,
+    DisassociateDelegationSignerFromDomainResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnableDomainTransferLockResponseTypeDef,
+    GetContactReachabilityStatusResponseTypeDef,
+    GetOperationDetailResponseTypeDef,
+    RegisterDomainResponseTypeDef,
+    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    RenewDomainResponseTypeDef,
+    ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     TransferDomainResponseTypeDef,
-    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
-    UpdateDomainContactPrivacyRequestRequestTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
-    ViewBillingRequestRequestTypeDef,
-    ViewBillingRequestViewBillingPaginateTypeDef,
     AssociateDelegationSignerToDomainRequestRequestTypeDef,
     ViewBillingResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
+    ContactDetailOutputTypeDef,
     ContactDetailTypeDef,
     DomainPriceTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     ListDomainsResponseTypeDef,
-    UpdateDomainNameserversRequestRequestTypeDef,
+    ListOperationsRequestListOperationsPaginateTypeDef,
+    ListPricesRequestListPricesPaginateTypeDef,
+    ViewBillingRequestViewBillingPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
+    UpdateDomainNameserversRequestRequestTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
     GetDomainDetailResponseTypeDef,
     RegisterDomainRequestRequestTypeDef,
     TransferDomainRequestRequestTypeDef,
     UpdateDomainContactRequestRequestTypeDef,
     ListPricesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/__init__.py` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/__init__.pyi` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/__main__.py` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53Domains 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.Route53Domains 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains\nOther"
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

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/client.py` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/client.pyi` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/literals.py` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,14 +503,15 @@
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
@@ -589,26 +590,28 @@
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

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/literals.pyi` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -501,14 +501,15 @@
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
@@ -587,26 +588,28 @@
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

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/paginator.py` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """
 
     def paginate(
         self,
         *,
         FilterConditions: Sequence[FilterConditionTypeDef] = ...,
         SortCondition: SortConditionTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listdomainspaginator)
         """
 
 
@@ -95,30 +95,30 @@
         self,
         *,
         SubmittedSince: Union[datetime, str] = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listoperationspaginator)
         """
 
 
 class ListPricesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListPrices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listpricespaginator)
     """
 
     def paginate(
-        self, *, Tld: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Tld: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPricesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListPrices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listpricespaginator)
         """
 
 
@@ -129,13 +129,13 @@
     """
 
     def paginate(
         self,
         *,
         Start: Union[datetime, str] = ...,
         End: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ViewBillingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#viewbillingpaginator)
         """
```

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/paginator.pyi` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     """
 
     def paginate(
         self,
         *,
         FilterConditions: Sequence[FilterConditionTypeDef] = ...,
         SortCondition: SortConditionTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listdomainspaginator)
         """
 
 class ListOperationsPaginator(Paginator):
@@ -90,29 +90,29 @@
         self,
         *,
         SubmittedSince: Union[datetime, str] = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listoperationspaginator)
         """
 
 class ListPricesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListPrices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listpricespaginator)
     """
 
     def paginate(
-        self, *, Tld: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Tld: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPricesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListPrices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#listpricespaginator)
         """
 
 class ViewBillingPaginator(Paginator):
@@ -122,13 +122,13 @@
     """
 
     def paginate(
         self,
         *,
         Start: Union[datetime, str] = ...,
         End: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ViewBillingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/paginators/#viewbillingpaginator)
         """
```

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/type_defs.py` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -35,95 +35,98 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
-    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DnssecSigningAttributesTypeDef",
-    "AssociateDelegationSignerToDomainResponseTypeDef",
     "BillingRecordTypeDef",
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
-    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     "CheckDomainAvailabilityRequestRequestTypeDef",
-    "CheckDomainAvailabilityResponseTypeDef",
     "CheckDomainTransferabilityRequestRequestTypeDef",
     "DomainTransferabilityTypeDef",
     "ConsentTypeDef",
+    "ExtraParamOutputTypeDef",
     "ExtraParamTypeDef",
     "DeleteDomainRequestRequestTypeDef",
-    "DeleteDomainResponseTypeDef",
     "DeleteTagsForDomainRequestRequestTypeDef",
     "DisableDomainAutoRenewRequestRequestTypeDef",
     "DisableDomainTransferLockRequestRequestTypeDef",
-    "DisableDomainTransferLockResponseTypeDef",
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
-    "DisassociateDelegationSignerFromDomainResponseTypeDef",
     "DnssecKeyTypeDef",
     "PriceWithCurrencyTypeDef",
     "DomainSuggestionTypeDef",
     "DomainSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableDomainAutoRenewRequestRequestTypeDef",
     "EnableDomainTransferLockRequestRequestTypeDef",
-    "EnableDomainTransferLockResponseTypeDef",
     "FilterConditionTypeDef",
     "GetContactReachabilityStatusRequestRequestTypeDef",
-    "GetContactReachabilityStatusResponseTypeDef",
     "GetDomainDetailRequestRequestTypeDef",
-    "NameserverTypeDef",
+    "NameserverOutputTypeDef",
     "GetDomainSuggestionsRequestRequestTypeDef",
     "GetOperationDetailRequestRequestTypeDef",
-    "GetOperationDetailResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "SortConditionTypeDef",
-    "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "OperationSummaryTypeDef",
-    "ListPricesRequestListPricesPaginateTypeDef",
     "ListPricesRequestRequestTypeDef",
     "ListTagsForDomainRequestRequestTypeDef",
-    "TagTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
+    "NameserverTypeDef",
     "PushDomainRequestRequestTypeDef",
-    "RegisterDomainResponseTypeDef",
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
-    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
     "RenewDomainRequestRequestTypeDef",
-    "RenewDomainResponseTypeDef",
     "ResendContactReachabilityEmailRequestRequestTypeDef",
-    "ResendContactReachabilityEmailResponseTypeDef",
     "ResendOperationAuthorizationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
+    "TagTypeDef",
+    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
+    "UpdateDomainContactPrivacyRequestRequestTypeDef",
+    "ViewBillingRequestRequestTypeDef",
+    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    "AssociateDelegationSignerToDomainResponseTypeDef",
+    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
+    "CheckDomainAvailabilityResponseTypeDef",
+    "DeleteDomainResponseTypeDef",
+    "DisableDomainTransferLockResponseTypeDef",
+    "DisassociateDelegationSignerFromDomainResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EnableDomainTransferLockResponseTypeDef",
+    "GetContactReachabilityStatusResponseTypeDef",
+    "GetOperationDetailResponseTypeDef",
+    "RegisterDomainResponseTypeDef",
+    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    "RenewDomainResponseTypeDef",
+    "ResendContactReachabilityEmailResponseTypeDef",
     "RetrieveDomainAuthCodeResponseTypeDef",
     "TransferDomainResponseTypeDef",
-    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     "TransferDomainToAnotherAwsAccountResponseTypeDef",
-    "UpdateDomainContactPrivacyRequestRequestTypeDef",
     "UpdateDomainContactPrivacyResponseTypeDef",
     "UpdateDomainContactResponseTypeDef",
     "UpdateDomainNameserversResponseTypeDef",
-    "ViewBillingRequestRequestTypeDef",
-    "ViewBillingRequestViewBillingPaginateTypeDef",
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     "ViewBillingResponseTypeDef",
     "CheckDomainTransferabilityResponseTypeDef",
+    "ContactDetailOutputTypeDef",
     "ContactDetailTypeDef",
     "DomainPriceTypeDef",
     "GetDomainSuggestionsResponseTypeDef",
     "ListDomainsResponseTypeDef",
-    "UpdateDomainNameserversRequestRequestTypeDef",
+    "ListOperationsRequestListOperationsPaginateTypeDef",
+    "ListPricesRequestListPricesPaginateTypeDef",
+    "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListTagsForDomainResponseTypeDef",
+    "UpdateDomainNameserversRequestRequestTypeDef",
     "UpdateTagsForDomainRequestRequestTypeDef",
     "GetDomainDetailResponseTypeDef",
     "RegisterDomainRequestRequestTypeDef",
     "TransferDomainRequestRequestTypeDef",
     "UpdateDomainContactRequestRequestTypeDef",
     "ListPricesResponseTypeDef",
 )
@@ -132,40 +135,35 @@
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "Password": str,
     },
 )
 
-AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
-    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DnssecSigningAttributesTypeDef = TypedDict(
     "DnssecSigningAttributesTypeDef",
     {
         "Algorithm": int,
         "Flags": int,
         "PublicKey": str,
     },
     total=False,
 )
 
-AssociateDelegationSignerToDomainResponseTypeDef = TypedDict(
-    "AssociateDelegationSignerToDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BillingRecordTypeDef = TypedDict(
     "BillingRecordTypeDef",
     {
         "DomainName": str,
         "Operation": OperationTypeType,
         "InvoiceId": str,
         "BillDate": datetime,
@@ -177,74 +175,54 @@
 CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-CancelDomainTransferToAnotherAwsAccountResponseTypeDef = TypedDict(
-    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCheckDomainAvailabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCheckDomainAvailabilityRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCheckDomainAvailabilityRequestRequestTypeDef = TypedDict(
     "_OptionalCheckDomainAvailabilityRequestRequestTypeDef",
     {
         "IdnLangCode": str,
     },
     total=False,
 )
 
-
 class CheckDomainAvailabilityRequestRequestTypeDef(
     _RequiredCheckDomainAvailabilityRequestRequestTypeDef,
     _OptionalCheckDomainAvailabilityRequestRequestTypeDef,
 ):
     pass
 
-
-CheckDomainAvailabilityResponseTypeDef = TypedDict(
-    "CheckDomainAvailabilityResponseTypeDef",
-    {
-        "Availability": DomainAvailabilityType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCheckDomainTransferabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCheckDomainTransferabilityRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCheckDomainTransferabilityRequestRequestTypeDef = TypedDict(
     "_OptionalCheckDomainTransferabilityRequestRequestTypeDef",
     {
         "AuthCode": str,
     },
     total=False,
 )
 
-
 class CheckDomainTransferabilityRequestRequestTypeDef(
     _RequiredCheckDomainTransferabilityRequestRequestTypeDef,
     _OptionalCheckDomainTransferabilityRequestRequestTypeDef,
 ):
     pass
 
-
 DomainTransferabilityTypeDef = TypedDict(
     "DomainTransferabilityTypeDef",
     {
         "Transferable": TransferableType,
     },
     total=False,
 )
@@ -253,14 +231,22 @@
     "ConsentTypeDef",
     {
         "MaxPrice": float,
         "Currency": str,
     },
 )
 
+ExtraParamOutputTypeDef = TypedDict(
+    "ExtraParamOutputTypeDef",
+    {
+        "Name": ExtraParamNameType,
+        "Value": str,
+    },
+)
+
 ExtraParamTypeDef = TypedDict(
     "ExtraParamTypeDef",
     {
         "Name": ExtraParamNameType,
         "Value": str,
     },
 )
@@ -268,22 +254,14 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTagsForDomainRequestRequestTypeDef = TypedDict(
     "DeleteTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "TagsToDelete": Sequence[str],
     },
 )
@@ -298,38 +276,22 @@
 DisableDomainTransferLockRequestRequestTypeDef = TypedDict(
     "DisableDomainTransferLockRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DisableDomainTransferLockResponseTypeDef = TypedDict(
-    "DisableDomainTransferLockResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateDelegationSignerFromDomainRequestRequestTypeDef = TypedDict(
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Id": str,
     },
 )
 
-DisassociateDelegationSignerFromDomainResponseTypeDef = TypedDict(
-    "DisassociateDelegationSignerFromDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DnssecKeyTypeDef = TypedDict(
     "DnssecKeyTypeDef",
     {
         "Algorithm": int,
         "Flags": int,
         "PublicKey": str,
         "DigestType": int,
@@ -364,43 +326,28 @@
         "AutoRenew": bool,
         "TransferLock": bool,
         "Expiry": datetime,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableDomainAutoRenewRequestRequestTypeDef = TypedDict(
     "EnableDomainAutoRenewRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
 EnableDomainTransferLockRequestRequestTypeDef = TypedDict(
     "EnableDomainTransferLockRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-EnableDomainTransferLockResponseTypeDef = TypedDict(
-    "EnableDomainTransferLockResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "Operator": OperatorType,
         "Values": Sequence[str],
     },
@@ -410,49 +357,38 @@
     "GetContactReachabilityStatusRequestRequestTypeDef",
     {
         "domainName": str,
     },
     total=False,
 )
 
-GetContactReachabilityStatusResponseTypeDef = TypedDict(
-    "GetContactReachabilityStatusResponseTypeDef",
-    {
-        "domainName": str,
-        "status": ReachabilityStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDomainDetailRequestRequestTypeDef = TypedDict(
     "GetDomainDetailRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-_RequiredNameserverTypeDef = TypedDict(
-    "_RequiredNameserverTypeDef",
+_RequiredNameserverOutputTypeDef = TypedDict(
+    "_RequiredNameserverOutputTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalNameserverTypeDef = TypedDict(
-    "_OptionalNameserverTypeDef",
+_OptionalNameserverOutputTypeDef = TypedDict(
+    "_OptionalNameserverOutputTypeDef",
     {
         "GlueIps": List[str],
     },
     total=False,
 )
 
-
-class NameserverTypeDef(_RequiredNameserverTypeDef, _OptionalNameserverTypeDef):
+class NameserverOutputTypeDef(_RequiredNameserverOutputTypeDef, _OptionalNameserverOutputTypeDef):
     pass
 
-
 GetDomainSuggestionsRequestRequestTypeDef = TypedDict(
     "GetDomainSuggestionsRequestRequestTypeDef",
     {
         "DomainName": str,
         "SuggestionCount": int,
         "OnlyAvailable": bool,
     },
@@ -461,50 +397,32 @@
 GetOperationDetailRequestRequestTypeDef = TypedDict(
     "GetOperationDetailRequestRequestTypeDef",
     {
         "OperationId": str,
     },
 )
 
-GetOperationDetailResponseTypeDef = TypedDict(
-    "GetOperationDetailResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "OperationId": str,
-        "Status": OperationStatusType,
-        "Message": str,
-        "DomainName": str,
-        "Type": OperationTypeType,
-        "SubmittedDate": datetime,
-        "LastUpdatedDate": datetime,
-        "StatusFlag": StatusFlagType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
 SortConditionTypeDef = TypedDict(
     "SortConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "SortOrder": SortOrderType,
     },
 )
 
-ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
-    "ListOperationsRequestListOperationsPaginateTypeDef",
-    {
-        "SubmittedSince": Union[datetime, str],
-        "Status": Sequence[OperationStatusType],
-        "Type": Sequence[OperationTypeType],
-        "SortBy": Literal["SubmittedDate"],
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOperationsRequestRequestTypeDef = TypedDict(
     "ListOperationsRequestRequestTypeDef",
     {
         "SubmittedSince": Union[datetime, str],
         "Marker": str,
         "MaxItems": int,
         "Status": Sequence[OperationStatusType],
@@ -526,23 +444,14 @@
         "Message": str,
         "StatusFlag": StatusFlagType,
         "LastUpdatedDate": datetime,
     },
     total=False,
 )
 
-ListPricesRequestListPricesPaginateTypeDef = TypedDict(
-    "ListPricesRequestListPricesPaginateTypeDef",
-    {
-        "Tld": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPricesRequestRequestTypeDef = TypedDict(
     "ListPricesRequestRequestTypeDef",
     {
         "Tld": str,
         "Marker": str,
         "MaxItems": int,
     },
@@ -552,64 +461,55 @@
 ListTagsForDomainRequestRequestTypeDef = TypedDict(
     "ListTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
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
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredNameserverTypeDef = TypedDict(
+    "_RequiredNameserverTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+    },
+)
+_OptionalNameserverTypeDef = TypedDict(
+    "_OptionalNameserverTypeDef",
+    {
+        "GlueIps": Sequence[str],
     },
     total=False,
 )
 
+class NameserverTypeDef(_RequiredNameserverTypeDef, _OptionalNameserverTypeDef):
+    pass
+
 PushDomainRequestRequestTypeDef = TypedDict(
     "PushDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Target": str,
     },
 )
 
-RegisterDomainResponseTypeDef = TypedDict(
-    "RegisterDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-RejectDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
-    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRenewDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRenewDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "CurrentExpiryYear": int,
     },
 )
@@ -617,105 +517,58 @@
     "_OptionalRenewDomainRequestRequestTypeDef",
     {
         "DurationInYears": int,
     },
     total=False,
 )
 
-
 class RenewDomainRequestRequestTypeDef(
     _RequiredRenewDomainRequestRequestTypeDef, _OptionalRenewDomainRequestRequestTypeDef
 ):
     pass
 
-
-RenewDomainResponseTypeDef = TypedDict(
-    "RenewDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResendContactReachabilityEmailRequestRequestTypeDef = TypedDict(
     "ResendContactReachabilityEmailRequestRequestTypeDef",
     {
         "domainName": str,
     },
     total=False,
 )
 
-ResendContactReachabilityEmailResponseTypeDef = TypedDict(
-    "ResendContactReachabilityEmailResponseTypeDef",
-    {
-        "domainName": str,
-        "emailAddress": str,
-        "isAlreadyVerified": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResendOperationAuthorizationRequestRequestTypeDef = TypedDict(
     "ResendOperationAuthorizationRequestRequestTypeDef",
     {
         "OperationId": str,
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
 RetrieveDomainAuthCodeRequestRequestTypeDef = TypedDict(
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-RetrieveDomainAuthCodeResponseTypeDef = TypedDict(
-    "RetrieveDomainAuthCodeResponseTypeDef",
-    {
-        "AuthCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TransferDomainResponseTypeDef = TypedDict(
-    "TransferDomainResponseTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Value": str,
     },
+    total=False,
 )
 
 TransferDomainToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "AccountId": str,
     },
 )
 
-TransferDomainToAnotherAwsAccountResponseTypeDef = TypedDict(
-    "TransferDomainToAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "Password": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
@@ -724,65 +577,207 @@
         "AdminPrivacy": bool,
         "RegistrantPrivacy": bool,
         "TechPrivacy": bool,
     },
     total=False,
 )
 
-
 class UpdateDomainContactPrivacyRequestRequestTypeDef(
     _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef,
     _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef,
 ):
     pass
 
+ViewBillingRequestRequestTypeDef = TypedDict(
+    "ViewBillingRequestRequestTypeDef",
+    {
+        "Start": Union[datetime, str],
+        "End": Union[datetime, str],
+        "Marker": str,
+        "MaxItems": int,
+    },
+    total=False,
+)
 
-UpdateDomainContactPrivacyResponseTypeDef = TypedDict(
-    "UpdateDomainContactPrivacyResponseTypeDef",
+AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
+    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDomainContactResponseTypeDef = TypedDict(
-    "UpdateDomainContactResponseTypeDef",
+AssociateDelegationSignerToDomainResponseTypeDef = TypedDict(
+    "AssociateDelegationSignerToDomainResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDomainNameserversResponseTypeDef = TypedDict(
-    "UpdateDomainNameserversResponseTypeDef",
+CancelDomainTransferToAnotherAwsAccountResponseTypeDef = TypedDict(
+    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ViewBillingRequestRequestTypeDef = TypedDict(
-    "ViewBillingRequestRequestTypeDef",
+CheckDomainAvailabilityResponseTypeDef = TypedDict(
+    "CheckDomainAvailabilityResponseTypeDef",
     {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "Marker": str,
-        "MaxItems": int,
+        "Availability": DomainAvailabilityType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
-    "ViewBillingRequestViewBillingPaginateTypeDef",
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
     {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableDomainTransferLockResponseTypeDef = TypedDict(
+    "DisableDomainTransferLockResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateDelegationSignerFromDomainResponseTypeDef = TypedDict(
+    "DisassociateDelegationSignerFromDomainResponseTypeDef",
+    {
+        "OperationId": str,
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
+EnableDomainTransferLockResponseTypeDef = TypedDict(
+    "EnableDomainTransferLockResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContactReachabilityStatusResponseTypeDef = TypedDict(
+    "GetContactReachabilityStatusResponseTypeDef",
+    {
+        "domainName": str,
+        "status": ReachabilityStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOperationDetailResponseTypeDef = TypedDict(
+    "GetOperationDetailResponseTypeDef",
+    {
+        "OperationId": str,
+        "Status": OperationStatusType,
+        "Message": str,
+        "DomainName": str,
+        "Type": OperationTypeType,
+        "SubmittedDate": datetime,
+        "LastUpdatedDate": datetime,
+        "StatusFlag": StatusFlagType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterDomainResponseTypeDef = TypedDict(
+    "RegisterDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RejectDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
+    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RenewDomainResponseTypeDef = TypedDict(
+    "RenewDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResendContactReachabilityEmailResponseTypeDef = TypedDict(
+    "ResendContactReachabilityEmailResponseTypeDef",
+    {
+        "domainName": str,
+        "emailAddress": str,
+        "isAlreadyVerified": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetrieveDomainAuthCodeResponseTypeDef = TypedDict(
+    "RetrieveDomainAuthCodeResponseTypeDef",
+    {
+        "AuthCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TransferDomainResponseTypeDef = TypedDict(
+    "TransferDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TransferDomainToAnotherAwsAccountResponseTypeDef = TypedDict(
+    "TransferDomainToAnotherAwsAccountResponseTypeDef",
+    {
+        "OperationId": str,
+        "Password": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainContactPrivacyResponseTypeDef = TypedDict(
+    "UpdateDomainContactPrivacyResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainContactResponseTypeDef = TypedDict(
+    "UpdateDomainContactResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainNameserversResponseTypeDef = TypedDict(
+    "UpdateDomainNameserversResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 AssociateDelegationSignerToDomainRequestRequestTypeDef = TypedDict(
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "SigningAttributes": DnssecSigningAttributesTypeDef,
@@ -790,24 +785,45 @@
 )
 
 ViewBillingResponseTypeDef = TypedDict(
     "ViewBillingResponseTypeDef",
     {
         "NextPageMarker": str,
         "BillingRecords": List[BillingRecordTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CheckDomainTransferabilityResponseTypeDef = TypedDict(
     "CheckDomainTransferabilityResponseTypeDef",
     {
         "Transferability": DomainTransferabilityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ContactDetailOutputTypeDef = TypedDict(
+    "ContactDetailOutputTypeDef",
+    {
+        "FirstName": str,
+        "LastName": str,
+        "ContactType": ContactTypeType,
+        "OrganizationName": str,
+        "AddressLine1": str,
+        "AddressLine2": str,
+        "City": str,
+        "State": str,
+        "CountryCode": CountryCodeType,
+        "ZipCode": str,
+        "PhoneNumber": str,
+        "Email": str,
+        "Fax": str,
+        "ExtraParams": List[ExtraParamOutputTypeDef],
     },
+    total=False,
 )
 
 ContactDetailTypeDef = TypedDict(
     "ContactDetailTypeDef",
     {
         "FirstName": str,
         "LastName": str,
@@ -818,15 +834,15 @@
         "City": str,
         "State": str,
         "CountryCode": CountryCodeType,
         "ZipCode": str,
         "PhoneNumber": str,
         "Email": str,
         "Fax": str,
-        "ExtraParams": List[ExtraParamTypeDef],
+        "ExtraParams": Sequence[ExtraParamTypeDef],
     },
     total=False,
 )
 
 DomainPriceTypeDef = TypedDict(
     "DomainPriceTypeDef",
     {
@@ -840,56 +856,65 @@
     total=False,
 )
 
 GetDomainSuggestionsResponseTypeDef = TypedDict(
     "GetDomainSuggestionsResponseTypeDef",
     {
         "SuggestionsList": List[DomainSuggestionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
+ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
+    "ListOperationsRequestListOperationsPaginateTypeDef",
     {
-        "DomainName": str,
-        "Nameservers": Sequence[NameserverTypeDef],
+        "SubmittedSince": Union[datetime, str],
+        "Status": Sequence[OperationStatusType],
+        "Type": Sequence[OperationTypeType],
+        "SortBy": Literal["SubmittedDate"],
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
+
+ListPricesRequestListPricesPaginateTypeDef = TypedDict(
+    "ListPricesRequestListPricesPaginateTypeDef",
     {
-        "FIAuthKey": str,
+        "Tld": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class UpdateDomainNameserversRequestRequestTypeDef(
-    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
-    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
-):
-    pass
-
+ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
+    "ViewBillingRequestViewBillingPaginateTypeDef",
+    {
+        "Start": Union[datetime, str],
+        "End": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
     "ListDomainsRequestListDomainsPaginateTypeDef",
     {
         "FilterConditions": Sequence[FilterConditionTypeDef],
         "SortCondition": SortConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
@@ -902,57 +927,76 @@
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForDomainResponseTypeDef = TypedDict(
     "ListTagsForDomainResponseTypeDef",
     {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "Nameservers": Sequence[NameserverTypeDef],
+    },
+)
+_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
+    {
+        "FIAuthKey": str,
+    },
+    total=False,
+)
+
+class UpdateDomainNameserversRequestRequestTypeDef(
+    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
+    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTagsForDomainRequestRequestTypeDef",
     {
         "TagsToUpdate": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class UpdateTagsForDomainRequestRequestTypeDef(
     _RequiredUpdateTagsForDomainRequestRequestTypeDef,
     _OptionalUpdateTagsForDomainRequestRequestTypeDef,
 ):
     pass
 
-
 GetDomainDetailResponseTypeDef = TypedDict(
     "GetDomainDetailResponseTypeDef",
     {
         "DomainName": str,
-        "Nameservers": List[NameserverTypeDef],
+        "Nameservers": List[NameserverOutputTypeDef],
         "AutoRenew": bool,
-        "AdminContact": ContactDetailTypeDef,
-        "RegistrantContact": ContactDetailTypeDef,
-        "TechContact": ContactDetailTypeDef,
+        "AdminContact": ContactDetailOutputTypeDef,
+        "RegistrantContact": ContactDetailOutputTypeDef,
+        "TechContact": ContactDetailOutputTypeDef,
         "AdminPrivacy": bool,
         "RegistrantPrivacy": bool,
         "TechPrivacy": bool,
         "RegistrarName": str,
         "WhoIsServer": str,
         "RegistrarUrl": str,
         "AbuseContactEmail": str,
@@ -961,15 +1005,15 @@
         "CreationDate": datetime,
         "UpdatedDate": datetime,
         "ExpirationDate": datetime,
         "Reseller": str,
         "DnsSec": str,
         "StatusList": List[str],
         "DnssecKeys": List[DnssecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -987,21 +1031,19 @@
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
 )
 
-
 class RegisterDomainRequestRequestTypeDef(
     _RequiredRegisterDomainRequestRequestTypeDef, _OptionalRegisterDomainRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredTransferDomainRequestRequestTypeDef = TypedDict(
     "_RequiredTransferDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
@@ -1018,21 +1060,19 @@
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
 )
 
-
 class TransferDomainRequestRequestTypeDef(
     _RequiredTransferDomainRequestRequestTypeDef, _OptionalTransferDomainRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainContactRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
@@ -1042,23 +1082,21 @@
         "RegistrantContact": ContactDetailTypeDef,
         "TechContact": ContactDetailTypeDef,
         "Consent": ConsentTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDomainContactRequestRequestTypeDef(
     _RequiredUpdateDomainContactRequestRequestTypeDef,
     _OptionalUpdateDomainContactRequestRequestTypeDef,
 ):
     pass
 
-
 ListPricesResponseTypeDef = TypedDict(
     "ListPricesResponseTypeDef",
     {
         "Prices": List[DomainPriceTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains/type_defs.pyi` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,94 +35,99 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
-    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DnssecSigningAttributesTypeDef",
-    "AssociateDelegationSignerToDomainResponseTypeDef",
     "BillingRecordTypeDef",
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
-    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     "CheckDomainAvailabilityRequestRequestTypeDef",
-    "CheckDomainAvailabilityResponseTypeDef",
     "CheckDomainTransferabilityRequestRequestTypeDef",
     "DomainTransferabilityTypeDef",
     "ConsentTypeDef",
+    "ExtraParamOutputTypeDef",
     "ExtraParamTypeDef",
     "DeleteDomainRequestRequestTypeDef",
-    "DeleteDomainResponseTypeDef",
     "DeleteTagsForDomainRequestRequestTypeDef",
     "DisableDomainAutoRenewRequestRequestTypeDef",
     "DisableDomainTransferLockRequestRequestTypeDef",
-    "DisableDomainTransferLockResponseTypeDef",
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
-    "DisassociateDelegationSignerFromDomainResponseTypeDef",
     "DnssecKeyTypeDef",
     "PriceWithCurrencyTypeDef",
     "DomainSuggestionTypeDef",
     "DomainSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableDomainAutoRenewRequestRequestTypeDef",
     "EnableDomainTransferLockRequestRequestTypeDef",
-    "EnableDomainTransferLockResponseTypeDef",
     "FilterConditionTypeDef",
     "GetContactReachabilityStatusRequestRequestTypeDef",
-    "GetContactReachabilityStatusResponseTypeDef",
     "GetDomainDetailRequestRequestTypeDef",
-    "NameserverTypeDef",
+    "NameserverOutputTypeDef",
     "GetDomainSuggestionsRequestRequestTypeDef",
     "GetOperationDetailRequestRequestTypeDef",
-    "GetOperationDetailResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "SortConditionTypeDef",
-    "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "OperationSummaryTypeDef",
-    "ListPricesRequestListPricesPaginateTypeDef",
     "ListPricesRequestRequestTypeDef",
     "ListTagsForDomainRequestRequestTypeDef",
-    "TagTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
+    "NameserverTypeDef",
     "PushDomainRequestRequestTypeDef",
-    "RegisterDomainResponseTypeDef",
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
-    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
     "RenewDomainRequestRequestTypeDef",
-    "RenewDomainResponseTypeDef",
     "ResendContactReachabilityEmailRequestRequestTypeDef",
-    "ResendContactReachabilityEmailResponseTypeDef",
     "ResendOperationAuthorizationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
+    "TagTypeDef",
+    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
+    "UpdateDomainContactPrivacyRequestRequestTypeDef",
+    "ViewBillingRequestRequestTypeDef",
+    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    "AssociateDelegationSignerToDomainResponseTypeDef",
+    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
+    "CheckDomainAvailabilityResponseTypeDef",
+    "DeleteDomainResponseTypeDef",
+    "DisableDomainTransferLockResponseTypeDef",
+    "DisassociateDelegationSignerFromDomainResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EnableDomainTransferLockResponseTypeDef",
+    "GetContactReachabilityStatusResponseTypeDef",
+    "GetOperationDetailResponseTypeDef",
+    "RegisterDomainResponseTypeDef",
+    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    "RenewDomainResponseTypeDef",
+    "ResendContactReachabilityEmailResponseTypeDef",
     "RetrieveDomainAuthCodeResponseTypeDef",
     "TransferDomainResponseTypeDef",
-    "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     "TransferDomainToAnotherAwsAccountResponseTypeDef",
-    "UpdateDomainContactPrivacyRequestRequestTypeDef",
     "UpdateDomainContactPrivacyResponseTypeDef",
     "UpdateDomainContactResponseTypeDef",
     "UpdateDomainNameserversResponseTypeDef",
-    "ViewBillingRequestRequestTypeDef",
-    "ViewBillingRequestViewBillingPaginateTypeDef",
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     "ViewBillingResponseTypeDef",
     "CheckDomainTransferabilityResponseTypeDef",
+    "ContactDetailOutputTypeDef",
     "ContactDetailTypeDef",
     "DomainPriceTypeDef",
     "GetDomainSuggestionsResponseTypeDef",
     "ListDomainsResponseTypeDef",
-    "UpdateDomainNameserversRequestRequestTypeDef",
+    "ListOperationsRequestListOperationsPaginateTypeDef",
+    "ListPricesRequestListPricesPaginateTypeDef",
+    "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListTagsForDomainResponseTypeDef",
+    "UpdateDomainNameserversRequestRequestTypeDef",
     "UpdateTagsForDomainRequestRequestTypeDef",
     "GetDomainDetailResponseTypeDef",
     "RegisterDomainRequestRequestTypeDef",
     "TransferDomainRequestRequestTypeDef",
     "UpdateDomainContactRequestRequestTypeDef",
     "ListPricesResponseTypeDef",
 )
@@ -131,40 +136,35 @@
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "Password": str,
     },
 )
 
-AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
-    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DnssecSigningAttributesTypeDef = TypedDict(
     "DnssecSigningAttributesTypeDef",
     {
         "Algorithm": int,
         "Flags": int,
         "PublicKey": str,
     },
     total=False,
 )
 
-AssociateDelegationSignerToDomainResponseTypeDef = TypedDict(
-    "AssociateDelegationSignerToDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BillingRecordTypeDef = TypedDict(
     "BillingRecordTypeDef",
     {
         "DomainName": str,
         "Operation": OperationTypeType,
         "InvoiceId": str,
         "BillDate": datetime,
@@ -176,49 +176,35 @@
 CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-CancelDomainTransferToAnotherAwsAccountResponseTypeDef = TypedDict(
-    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCheckDomainAvailabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCheckDomainAvailabilityRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCheckDomainAvailabilityRequestRequestTypeDef = TypedDict(
     "_OptionalCheckDomainAvailabilityRequestRequestTypeDef",
     {
         "IdnLangCode": str,
     },
     total=False,
 )
 
+
 class CheckDomainAvailabilityRequestRequestTypeDef(
     _RequiredCheckDomainAvailabilityRequestRequestTypeDef,
     _OptionalCheckDomainAvailabilityRequestRequestTypeDef,
 ):
     pass
 
-CheckDomainAvailabilityResponseTypeDef = TypedDict(
-    "CheckDomainAvailabilityResponseTypeDef",
-    {
-        "Availability": DomainAvailabilityType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCheckDomainTransferabilityRequestRequestTypeDef = TypedDict(
     "_RequiredCheckDomainTransferabilityRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
@@ -226,20 +212,22 @@
     "_OptionalCheckDomainTransferabilityRequestRequestTypeDef",
     {
         "AuthCode": str,
     },
     total=False,
 )
 
+
 class CheckDomainTransferabilityRequestRequestTypeDef(
     _RequiredCheckDomainTransferabilityRequestRequestTypeDef,
     _OptionalCheckDomainTransferabilityRequestRequestTypeDef,
 ):
     pass
 
+
 DomainTransferabilityTypeDef = TypedDict(
     "DomainTransferabilityTypeDef",
     {
         "Transferable": TransferableType,
     },
     total=False,
 )
@@ -248,14 +236,22 @@
     "ConsentTypeDef",
     {
         "MaxPrice": float,
         "Currency": str,
     },
 )
 
+ExtraParamOutputTypeDef = TypedDict(
+    "ExtraParamOutputTypeDef",
+    {
+        "Name": ExtraParamNameType,
+        "Value": str,
+    },
+)
+
 ExtraParamTypeDef = TypedDict(
     "ExtraParamTypeDef",
     {
         "Name": ExtraParamNameType,
         "Value": str,
     },
 )
@@ -263,22 +259,14 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTagsForDomainRequestRequestTypeDef = TypedDict(
     "DeleteTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "TagsToDelete": Sequence[str],
     },
 )
@@ -293,38 +281,22 @@
 DisableDomainTransferLockRequestRequestTypeDef = TypedDict(
     "DisableDomainTransferLockRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DisableDomainTransferLockResponseTypeDef = TypedDict(
-    "DisableDomainTransferLockResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateDelegationSignerFromDomainRequestRequestTypeDef = TypedDict(
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Id": str,
     },
 )
 
-DisassociateDelegationSignerFromDomainResponseTypeDef = TypedDict(
-    "DisassociateDelegationSignerFromDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DnssecKeyTypeDef = TypedDict(
     "DnssecKeyTypeDef",
     {
         "Algorithm": int,
         "Flags": int,
         "PublicKey": str,
         "DigestType": int,
@@ -359,43 +331,28 @@
         "AutoRenew": bool,
         "TransferLock": bool,
         "Expiry": datetime,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableDomainAutoRenewRequestRequestTypeDef = TypedDict(
     "EnableDomainAutoRenewRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
 EnableDomainTransferLockRequestRequestTypeDef = TypedDict(
     "EnableDomainTransferLockRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-EnableDomainTransferLockResponseTypeDef = TypedDict(
-    "EnableDomainTransferLockResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "Operator": OperatorType,
         "Values": Sequence[str],
     },
@@ -405,47 +362,40 @@
     "GetContactReachabilityStatusRequestRequestTypeDef",
     {
         "domainName": str,
     },
     total=False,
 )
 
-GetContactReachabilityStatusResponseTypeDef = TypedDict(
-    "GetContactReachabilityStatusResponseTypeDef",
-    {
-        "domainName": str,
-        "status": ReachabilityStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDomainDetailRequestRequestTypeDef = TypedDict(
     "GetDomainDetailRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-_RequiredNameserverTypeDef = TypedDict(
-    "_RequiredNameserverTypeDef",
+_RequiredNameserverOutputTypeDef = TypedDict(
+    "_RequiredNameserverOutputTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalNameserverTypeDef = TypedDict(
-    "_OptionalNameserverTypeDef",
+_OptionalNameserverOutputTypeDef = TypedDict(
+    "_OptionalNameserverOutputTypeDef",
     {
         "GlueIps": List[str],
     },
     total=False,
 )
 
-class NameserverTypeDef(_RequiredNameserverTypeDef, _OptionalNameserverTypeDef):
+
+class NameserverOutputTypeDef(_RequiredNameserverOutputTypeDef, _OptionalNameserverOutputTypeDef):
     pass
 
+
 GetDomainSuggestionsRequestRequestTypeDef = TypedDict(
     "GetDomainSuggestionsRequestRequestTypeDef",
     {
         "DomainName": str,
         "SuggestionCount": int,
         "OnlyAvailable": bool,
     },
@@ -454,50 +404,32 @@
 GetOperationDetailRequestRequestTypeDef = TypedDict(
     "GetOperationDetailRequestRequestTypeDef",
     {
         "OperationId": str,
     },
 )
 
-GetOperationDetailResponseTypeDef = TypedDict(
-    "GetOperationDetailResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "OperationId": str,
-        "Status": OperationStatusType,
-        "Message": str,
-        "DomainName": str,
-        "Type": OperationTypeType,
-        "SubmittedDate": datetime,
-        "LastUpdatedDate": datetime,
-        "StatusFlag": StatusFlagType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
 SortConditionTypeDef = TypedDict(
     "SortConditionTypeDef",
     {
         "Name": ListDomainsAttributeNameType,
         "SortOrder": SortOrderType,
     },
 )
 
-ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
-    "ListOperationsRequestListOperationsPaginateTypeDef",
-    {
-        "SubmittedSince": Union[datetime, str],
-        "Status": Sequence[OperationStatusType],
-        "Type": Sequence[OperationTypeType],
-        "SortBy": Literal["SubmittedDate"],
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOperationsRequestRequestTypeDef = TypedDict(
     "ListOperationsRequestRequestTypeDef",
     {
         "SubmittedSince": Union[datetime, str],
         "Marker": str,
         "MaxItems": int,
         "Status": Sequence[OperationStatusType],
@@ -519,23 +451,14 @@
         "Message": str,
         "StatusFlag": StatusFlagType,
         "LastUpdatedDate": datetime,
     },
     total=False,
 )
 
-ListPricesRequestListPricesPaginateTypeDef = TypedDict(
-    "ListPricesRequestListPricesPaginateTypeDef",
-    {
-        "Tld": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPricesRequestRequestTypeDef = TypedDict(
     "ListPricesRequestRequestTypeDef",
     {
         "Tld": str,
         "Marker": str,
         "MaxItems": int,
     },
@@ -545,64 +468,57 @@
 ListTagsForDomainRequestRequestTypeDef = TypedDict(
     "ListTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
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
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredNameserverTypeDef = TypedDict(
+    "_RequiredNameserverTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Name": str,
+    },
+)
+_OptionalNameserverTypeDef = TypedDict(
+    "_OptionalNameserverTypeDef",
+    {
+        "GlueIps": Sequence[str],
     },
     total=False,
 )
 
+
+class NameserverTypeDef(_RequiredNameserverTypeDef, _OptionalNameserverTypeDef):
+    pass
+
+
 PushDomainRequestRequestTypeDef = TypedDict(
     "PushDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Target": str,
     },
 )
 
-RegisterDomainResponseTypeDef = TypedDict(
-    "RegisterDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-RejectDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
-    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRenewDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRenewDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "CurrentExpiryYear": int,
     },
 )
@@ -610,103 +526,60 @@
     "_OptionalRenewDomainRequestRequestTypeDef",
     {
         "DurationInYears": int,
     },
     total=False,
 )
 
+
 class RenewDomainRequestRequestTypeDef(
     _RequiredRenewDomainRequestRequestTypeDef, _OptionalRenewDomainRequestRequestTypeDef
 ):
     pass
 
-RenewDomainResponseTypeDef = TypedDict(
-    "RenewDomainResponseTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ResendContactReachabilityEmailRequestRequestTypeDef = TypedDict(
     "ResendContactReachabilityEmailRequestRequestTypeDef",
     {
         "domainName": str,
     },
     total=False,
 )
 
-ResendContactReachabilityEmailResponseTypeDef = TypedDict(
-    "ResendContactReachabilityEmailResponseTypeDef",
-    {
-        "domainName": str,
-        "emailAddress": str,
-        "isAlreadyVerified": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResendOperationAuthorizationRequestRequestTypeDef = TypedDict(
     "ResendOperationAuthorizationRequestRequestTypeDef",
     {
         "OperationId": str,
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
 RetrieveDomainAuthCodeRequestRequestTypeDef = TypedDict(
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-RetrieveDomainAuthCodeResponseTypeDef = TypedDict(
-    "RetrieveDomainAuthCodeResponseTypeDef",
-    {
-        "AuthCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TransferDomainResponseTypeDef = TypedDict(
-    "TransferDomainResponseTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Value": str,
     },
+    total=False,
 )
 
 TransferDomainToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "AccountId": str,
     },
 )
 
-TransferDomainToAnotherAwsAccountResponseTypeDef = TypedDict(
-    "TransferDomainToAnotherAwsAccountResponseTypeDef",
-    {
-        "OperationId": str,
-        "Password": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainContactPrivacyRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef = TypedDict(
@@ -715,63 +588,209 @@
         "AdminPrivacy": bool,
         "RegistrantPrivacy": bool,
         "TechPrivacy": bool,
     },
     total=False,
 )
 
+
 class UpdateDomainContactPrivacyRequestRequestTypeDef(
     _RequiredUpdateDomainContactPrivacyRequestRequestTypeDef,
     _OptionalUpdateDomainContactPrivacyRequestRequestTypeDef,
 ):
     pass
 
-UpdateDomainContactPrivacyResponseTypeDef = TypedDict(
-    "UpdateDomainContactPrivacyResponseTypeDef",
+
+ViewBillingRequestRequestTypeDef = TypedDict(
+    "ViewBillingRequestRequestTypeDef",
+    {
+        "Start": Union[datetime, str],
+        "End": Union[datetime, str],
+        "Marker": str,
+        "MaxItems": int,
+    },
+    total=False,
+)
+
+AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
+    "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDomainContactResponseTypeDef = TypedDict(
-    "UpdateDomainContactResponseTypeDef",
+AssociateDelegationSignerToDomainResponseTypeDef = TypedDict(
+    "AssociateDelegationSignerToDomainResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDomainNameserversResponseTypeDef = TypedDict(
-    "UpdateDomainNameserversResponseTypeDef",
+CancelDomainTransferToAnotherAwsAccountResponseTypeDef = TypedDict(
+    "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     {
         "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ViewBillingRequestRequestTypeDef = TypedDict(
-    "ViewBillingRequestRequestTypeDef",
+CheckDomainAvailabilityResponseTypeDef = TypedDict(
+    "CheckDomainAvailabilityResponseTypeDef",
     {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "Marker": str,
-        "MaxItems": int,
+        "Availability": DomainAvailabilityType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
-    "ViewBillingRequestViewBillingPaginateTypeDef",
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
     {
-        "Start": Union[datetime, str],
-        "End": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableDomainTransferLockResponseTypeDef = TypedDict(
+    "DisableDomainTransferLockResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateDelegationSignerFromDomainResponseTypeDef = TypedDict(
+    "DisassociateDelegationSignerFromDomainResponseTypeDef",
+    {
+        "OperationId": str,
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
+EnableDomainTransferLockResponseTypeDef = TypedDict(
+    "EnableDomainTransferLockResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContactReachabilityStatusResponseTypeDef = TypedDict(
+    "GetContactReachabilityStatusResponseTypeDef",
+    {
+        "domainName": str,
+        "status": ReachabilityStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOperationDetailResponseTypeDef = TypedDict(
+    "GetOperationDetailResponseTypeDef",
+    {
+        "OperationId": str,
+        "Status": OperationStatusType,
+        "Message": str,
+        "DomainName": str,
+        "Type": OperationTypeType,
+        "SubmittedDate": datetime,
+        "LastUpdatedDate": datetime,
+        "StatusFlag": StatusFlagType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterDomainResponseTypeDef = TypedDict(
+    "RegisterDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RejectDomainTransferFromAnotherAwsAccountResponseTypeDef = TypedDict(
+    "RejectDomainTransferFromAnotherAwsAccountResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RenewDomainResponseTypeDef = TypedDict(
+    "RenewDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResendContactReachabilityEmailResponseTypeDef = TypedDict(
+    "ResendContactReachabilityEmailResponseTypeDef",
+    {
+        "domainName": str,
+        "emailAddress": str,
+        "isAlreadyVerified": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetrieveDomainAuthCodeResponseTypeDef = TypedDict(
+    "RetrieveDomainAuthCodeResponseTypeDef",
+    {
+        "AuthCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TransferDomainResponseTypeDef = TypedDict(
+    "TransferDomainResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TransferDomainToAnotherAwsAccountResponseTypeDef = TypedDict(
+    "TransferDomainToAnotherAwsAccountResponseTypeDef",
+    {
+        "OperationId": str,
+        "Password": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainContactPrivacyResponseTypeDef = TypedDict(
+    "UpdateDomainContactPrivacyResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainContactResponseTypeDef = TypedDict(
+    "UpdateDomainContactResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainNameserversResponseTypeDef = TypedDict(
+    "UpdateDomainNameserversResponseTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 AssociateDelegationSignerToDomainRequestRequestTypeDef = TypedDict(
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "SigningAttributes": DnssecSigningAttributesTypeDef,
@@ -779,24 +798,45 @@
 )
 
 ViewBillingResponseTypeDef = TypedDict(
     "ViewBillingResponseTypeDef",
     {
         "NextPageMarker": str,
         "BillingRecords": List[BillingRecordTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CheckDomainTransferabilityResponseTypeDef = TypedDict(
     "CheckDomainTransferabilityResponseTypeDef",
     {
         "Transferability": DomainTransferabilityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ContactDetailOutputTypeDef = TypedDict(
+    "ContactDetailOutputTypeDef",
+    {
+        "FirstName": str,
+        "LastName": str,
+        "ContactType": ContactTypeType,
+        "OrganizationName": str,
+        "AddressLine1": str,
+        "AddressLine2": str,
+        "City": str,
+        "State": str,
+        "CountryCode": CountryCodeType,
+        "ZipCode": str,
+        "PhoneNumber": str,
+        "Email": str,
+        "Fax": str,
+        "ExtraParams": List[ExtraParamOutputTypeDef],
     },
+    total=False,
 )
 
 ContactDetailTypeDef = TypedDict(
     "ContactDetailTypeDef",
     {
         "FirstName": str,
         "LastName": str,
@@ -807,15 +847,15 @@
         "City": str,
         "State": str,
         "CountryCode": CountryCodeType,
         "ZipCode": str,
         "PhoneNumber": str,
         "Email": str,
         "Fax": str,
-        "ExtraParams": List[ExtraParamTypeDef],
+        "ExtraParams": Sequence[ExtraParamTypeDef],
     },
     total=False,
 )
 
 DomainPriceTypeDef = TypedDict(
     "DomainPriceTypeDef",
     {
@@ -829,54 +869,65 @@
     total=False,
 )
 
 GetDomainSuggestionsResponseTypeDef = TypedDict(
     "GetDomainSuggestionsResponseTypeDef",
     {
         "SuggestionsList": List[DomainSuggestionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
+ListOperationsRequestListOperationsPaginateTypeDef = TypedDict(
+    "ListOperationsRequestListOperationsPaginateTypeDef",
     {
-        "DomainName": str,
-        "Nameservers": Sequence[NameserverTypeDef],
+        "SubmittedSince": Union[datetime, str],
+        "Status": Sequence[OperationStatusType],
+        "Type": Sequence[OperationTypeType],
+        "SortBy": Literal["SubmittedDate"],
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
+
+ListPricesRequestListPricesPaginateTypeDef = TypedDict(
+    "ListPricesRequestListPricesPaginateTypeDef",
     {
-        "FIAuthKey": str,
+        "Tld": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class UpdateDomainNameserversRequestRequestTypeDef(
-    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
-    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
-):
-    pass
+ViewBillingRequestViewBillingPaginateTypeDef = TypedDict(
+    "ViewBillingRequestViewBillingPaginateTypeDef",
+    {
+        "Start": Union[datetime, str],
+        "End": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
     "ListDomainsRequestListDomainsPaginateTypeDef",
     {
         "FilterConditions": Sequence[FilterConditionTypeDef],
         "SortCondition": SortConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
@@ -889,55 +940,80 @@
 )
 
 ListOperationsResponseTypeDef = TypedDict(
     "ListOperationsResponseTypeDef",
     {
         "Operations": List[OperationSummaryTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForDomainResponseTypeDef = TypedDict(
     "ListTagsForDomainResponseTypeDef",
     {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "Nameservers": Sequence[NameserverTypeDef],
+    },
+)
+_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
+    {
+        "FIAuthKey": str,
+    },
+    total=False,
+)
+
+
+class UpdateDomainNameserversRequestRequestTypeDef(
+    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
+    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTagsForDomainRequestRequestTypeDef",
     {
         "TagsToUpdate": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class UpdateTagsForDomainRequestRequestTypeDef(
     _RequiredUpdateTagsForDomainRequestRequestTypeDef,
     _OptionalUpdateTagsForDomainRequestRequestTypeDef,
 ):
     pass
 
+
 GetDomainDetailResponseTypeDef = TypedDict(
     "GetDomainDetailResponseTypeDef",
     {
         "DomainName": str,
-        "Nameservers": List[NameserverTypeDef],
+        "Nameservers": List[NameserverOutputTypeDef],
         "AutoRenew": bool,
-        "AdminContact": ContactDetailTypeDef,
-        "RegistrantContact": ContactDetailTypeDef,
-        "TechContact": ContactDetailTypeDef,
+        "AdminContact": ContactDetailOutputTypeDef,
+        "RegistrantContact": ContactDetailOutputTypeDef,
+        "TechContact": ContactDetailOutputTypeDef,
         "AdminPrivacy": bool,
         "RegistrantPrivacy": bool,
         "TechPrivacy": bool,
         "RegistrarName": str,
         "WhoIsServer": str,
         "RegistrarUrl": str,
         "AbuseContactEmail": str,
@@ -946,15 +1022,15 @@
         "CreationDate": datetime,
         "UpdatedDate": datetime,
         "ExpirationDate": datetime,
         "Reseller": str,
         "DnsSec": str,
         "StatusList": List[str],
         "DnssecKeys": List[DnssecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -972,19 +1048,21 @@
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
 )
 
+
 class RegisterDomainRequestRequestTypeDef(
     _RequiredRegisterDomainRequestRequestTypeDef, _OptionalRegisterDomainRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredTransferDomainRequestRequestTypeDef = TypedDict(
     "_RequiredTransferDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
@@ -1001,19 +1079,21 @@
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
 )
 
+
 class TransferDomainRequestRequestTypeDef(
     _RequiredTransferDomainRequestRequestTypeDef, _OptionalTransferDomainRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainContactRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
@@ -1023,21 +1103,23 @@
         "RegistrantContact": ContactDetailTypeDef,
         "TechContact": ContactDetailTypeDef,
         "Consent": ConsentTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDomainContactRequestRequestTypeDef(
     _RequiredUpdateDomainContactRequestRequestTypeDef,
     _OptionalUpdateDomainContactRequestRequestTypeDef,
 ):
     pass
 
+
 ListPricesResponseTypeDef = TypedDict(
     "ListPricesResponseTypeDef",
     {
         "Prices": List[DomainPriceTypeDef],
         "NextPageMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains.egg-info/PKG-INFO` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53domains
-Version: 1.28.0
-Summary: Type annotations for boto3.Route53Domains 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Route53Domains 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-route53domains"></a>
 
 # mypy-boto3-route53domains
 
 [![PyPI - mypy-boto3-route53domains](https://img.shields.io/pypi/v/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53domains?color=blue)](https://pypistats.org/packages/mypy-boto3-route53domains)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53domains)](https://pepy.tech/project/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,92 +345,96 @@
 
 `mypy_boto3_route53domains.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53domains.type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    ResponseMetadataTypeDef,
     DnssecSigningAttributesTypeDef,
-    AssociateDelegationSignerToDomainResponseTypeDef,
     BillingRecordTypeDef,
     CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef,
-    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityRequestRequestTypeDef,
-    CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityRequestRequestTypeDef,
     DomainTransferabilityTypeDef,
     ConsentTypeDef,
+    ExtraParamOutputTypeDef,
     ExtraParamTypeDef,
     DeleteDomainRequestRequestTypeDef,
-    DeleteDomainResponseTypeDef,
     DeleteTagsForDomainRequestRequestTypeDef,
     DisableDomainAutoRenewRequestRequestTypeDef,
     DisableDomainTransferLockRequestRequestTypeDef,
-    DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainRequestRequestTypeDef,
-    DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecKeyTypeDef,
     PriceWithCurrencyTypeDef,
     DomainSuggestionTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableDomainAutoRenewRequestRequestTypeDef,
     EnableDomainTransferLockRequestRequestTypeDef,
-    EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
     GetContactReachabilityStatusRequestRequestTypeDef,
-    GetContactReachabilityStatusResponseTypeDef,
     GetDomainDetailRequestRequestTypeDef,
-    NameserverTypeDef,
+    NameserverOutputTypeDef,
     GetDomainSuggestionsRequestRequestTypeDef,
     GetOperationDetailRequestRequestTypeDef,
-    GetOperationDetailResponseTypeDef,
+    PaginatorConfigTypeDef,
     SortConditionTypeDef,
-    ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
-    ListPricesRequestListPricesPaginateTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
-    TagTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
+    NameserverTypeDef,
     PushDomainRequestRequestTypeDef,
-    RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
-    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainRequestRequestTypeDef,
-    RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
-    ResendContactReachabilityEmailResponseTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
+    TagTypeDef,
+    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
+    UpdateDomainContactPrivacyRequestRequestTypeDef,
+    ViewBillingRequestRequestTypeDef,
+    AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    AssociateDelegationSignerToDomainResponseTypeDef,
+    CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
+    CheckDomainAvailabilityResponseTypeDef,
+    DeleteDomainResponseTypeDef,
+    DisableDomainTransferLockResponseTypeDef,
+    DisassociateDelegationSignerFromDomainResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EnableDomainTransferLockResponseTypeDef,
+    GetContactReachabilityStatusResponseTypeDef,
+    GetOperationDetailResponseTypeDef,
+    RegisterDomainResponseTypeDef,
+    RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
+    RenewDomainResponseTypeDef,
+    ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     TransferDomainResponseTypeDef,
-    TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     TransferDomainToAnotherAwsAccountResponseTypeDef,
-    UpdateDomainContactPrivacyRequestRequestTypeDef,
     UpdateDomainContactPrivacyResponseTypeDef,
     UpdateDomainContactResponseTypeDef,
     UpdateDomainNameserversResponseTypeDef,
-    ViewBillingRequestRequestTypeDef,
-    ViewBillingRequestViewBillingPaginateTypeDef,
     AssociateDelegationSignerToDomainRequestRequestTypeDef,
     ViewBillingResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
+    ContactDetailOutputTypeDef,
     ContactDetailTypeDef,
     DomainPriceTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     ListDomainsResponseTypeDef,
-    UpdateDomainNameserversRequestRequestTypeDef,
+    ListOperationsRequestListOperationsPaginateTypeDef,
+    ListPricesRequestListPricesPaginateTypeDef,
+    ViewBillingRequestViewBillingPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
+    UpdateDomainNameserversRequestRequestTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
     GetDomainDetailResponseTypeDef,
     RegisterDomainRequestRequestTypeDef,
     TransferDomainRequestRequestTypeDef,
     UpdateDomainContactRequestRequestTypeDef,
     ListPricesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-route53domains-1.28.0/mypy_boto3_route53domains.egg-info/SOURCES.txt` & `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.0/setup.py` & `mypy-boto3-route53domains-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53domains",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_route53domains"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53Domains 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Route53Domains 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

