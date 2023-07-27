# Comparing `tmp/mypy-boto3-payment-cryptography-1.28.0.tar.gz` & `tmp/mypy-boto3-payment-cryptography-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-payment-cryptography-1.28.0.tar", last modified: Thu Jul  6 21:00:17 2023, max compression
+gzip compressed data, was "mypy-boto3-payment-cryptography-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
```

## Comparing `mypy-boto3-payment-cryptography-1.28.0.tar` & `mypy-boto3-payment-cryptography-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:17.974391 mypy-boto3-payment-cryptography-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:02.000000 mypy-boto3-payment-cryptography-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-06 21:00:17.970391 mypy-boto3-payment-cryptography-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-07-06 20:49:02.000000 mypy-boto3-payment-cryptography-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:17.966391 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-06 20:49:02.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-06 20:49:02.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-06 20:49:02.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-07-06 20:49:03.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-06 20:49:02.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-07-06 20:49:03.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-07-06 20:49:03.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-06 20:49:03.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-06 20:49:03.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:02.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17687 2023-07-06 20:49:03.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17663 2023-07-06 20:49:03.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:02.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:17.970391 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-06 21:00:17.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-06 21:00:17.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:17.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:17.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:17.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 21:00:17.000000 mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:17.974391 mypy-boto3-payment-cryptography-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-06 20:49:02.000000 mypy-boto3-payment-cryptography-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.781132 mypy-boto3-payment-cryptography-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15793 2023-07-27 11:49:21.781132 mypy-boto3-payment-cryptography-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.781132 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.781132 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15793 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.781132 mypy-boto3-payment-cryptography-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/setup.py
```

### Comparing `mypy-boto3-payment-cryptography-1.28.0/LICENSE` & `mypy-boto3-payment-cryptography-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.0/PKG-INFO` & `mypy-boto3-payment-cryptography-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography
-Version: 1.28.0
-Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-payment-cryptography"></a>
 
 # mypy-boto3-payment-cryptography
 
 [![PyPI - mypy-boto3-payment-cryptography](https://img.shields.io/pypi/v/mypy-boto3-payment-cryptography.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-payment-cryptography?color=blue)](https://pypistats.org/packages/mypy-boto3-payment-cryptography)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-payment-cryptography)](https://pepy.tech/project/mypy-boto3-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyControlPlane 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[boto3.PaymentCryptographyControlPlane 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
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
 [mypy-boto3-payment-cryptography docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,57 +340,60 @@
 `mypy_boto3_payment_cryptography.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_payment_cryptography.type_defs import (
     AliasTypeDef,
     CreateAliasInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     DeleteAliasInputRequestTypeDef,
     DeleteKeyInputRequestTypeDef,
     ExportTr31KeyBlockTypeDef,
     ExportTr34KeyBlockTypeDef,
     WrappedKeyTypeDef,
     GetAliasInputRequestTypeDef,
     GetKeyInputRequestTypeDef,
     GetParametersForExportInputRequestTypeDef,
-    GetParametersForExportOutputTypeDef,
     GetParametersForImportInputRequestTypeDef,
-    GetParametersForImportOutputTypeDef,
     GetPublicKeyCertificateInputRequestTypeDef,
-    GetPublicKeyCertificateOutputTypeDef,
     ImportTr31KeyBlockTypeDef,
     ImportTr34KeyBlockTypeDef,
+    KeyModesOfUseOutputTypeDef,
     KeyModesOfUseTypeDef,
-    ListAliasesInputListAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAliasesInputRequestTypeDef,
-    ListKeysInputListKeysPaginateTypeDef,
     ListKeysInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     RestoreKeyInputRequestTypeDef,
     StartKeyUsageInputRequestTypeDef,
     StopKeyUsageInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateAliasInputRequestTypeDef,
     CreateAliasOutputTypeDef,
     GetAliasOutputTypeDef,
+    GetParametersForExportOutputTypeDef,
+    GetParametersForImportOutputTypeDef,
+    GetPublicKeyCertificateOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ExportKeyMaterialTypeDef,
     ExportKeyOutputTypeDef,
+    KeyAttributesOutputTypeDef,
     KeyAttributesTypeDef,
+    ListAliasesInputListAliasesPaginateTypeDef,
+    ListKeysInputListKeysPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ExportKeyInputRequestTypeDef,
-    CreateKeyInputRequestTypeDef,
     KeySummaryTypeDef,
     KeyTypeDef,
+    CreateKeyInputRequestTypeDef,
     RootCertificatePublicKeyTypeDef,
     TrustedCertificatePublicKeyTypeDef,
     ListKeysOutputTypeDef,
     CreateKeyOutputTypeDef,
     DeleteKeyOutputTypeDef,
     GetKeyOutputTypeDef,
     ImportKeyOutputTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.28.0/README.md` & `mypy-boto3-payment-cryptography-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-payment-cryptography"></a>
 
 # mypy-boto3-payment-cryptography
 
 [![PyPI - mypy-boto3-payment-cryptography](https://img.shields.io/pypi/v/mypy-boto3-payment-cryptography.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-payment-cryptography?color=blue)](https://pypistats.org/packages/mypy-boto3-payment-cryptography)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-payment-cryptography)](https://pepy.tech/project/mypy-boto3-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyControlPlane 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[boto3.PaymentCryptographyControlPlane 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
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
 [mypy-boto3-payment-cryptography docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
 
@@ -308,57 +308,60 @@
 `mypy_boto3_payment_cryptography.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_payment_cryptography.type_defs import (
     AliasTypeDef,
     CreateAliasInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     DeleteAliasInputRequestTypeDef,
     DeleteKeyInputRequestTypeDef,
     ExportTr31KeyBlockTypeDef,
     ExportTr34KeyBlockTypeDef,
     WrappedKeyTypeDef,
     GetAliasInputRequestTypeDef,
     GetKeyInputRequestTypeDef,
     GetParametersForExportInputRequestTypeDef,
-    GetParametersForExportOutputTypeDef,
     GetParametersForImportInputRequestTypeDef,
-    GetParametersForImportOutputTypeDef,
     GetPublicKeyCertificateInputRequestTypeDef,
-    GetPublicKeyCertificateOutputTypeDef,
     ImportTr31KeyBlockTypeDef,
     ImportTr34KeyBlockTypeDef,
+    KeyModesOfUseOutputTypeDef,
     KeyModesOfUseTypeDef,
-    ListAliasesInputListAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAliasesInputRequestTypeDef,
-    ListKeysInputListKeysPaginateTypeDef,
     ListKeysInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     RestoreKeyInputRequestTypeDef,
     StartKeyUsageInputRequestTypeDef,
     StopKeyUsageInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateAliasInputRequestTypeDef,
     CreateAliasOutputTypeDef,
     GetAliasOutputTypeDef,
+    GetParametersForExportOutputTypeDef,
+    GetParametersForImportOutputTypeDef,
+    GetPublicKeyCertificateOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ExportKeyMaterialTypeDef,
     ExportKeyOutputTypeDef,
+    KeyAttributesOutputTypeDef,
     KeyAttributesTypeDef,
+    ListAliasesInputListAliasesPaginateTypeDef,
+    ListKeysInputListKeysPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ExportKeyInputRequestTypeDef,
-    CreateKeyInputRequestTypeDef,
     KeySummaryTypeDef,
     KeyTypeDef,
+    CreateKeyInputRequestTypeDef,
     RootCertificatePublicKeyTypeDef,
     TrustedCertificatePublicKeyTypeDef,
     ListKeysOutputTypeDef,
     CreateKeyOutputTypeDef,
     DeleteKeyOutputTypeDef,
     GetKeyOutputTypeDef,
     ImportKeyOutputTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/__init__.py` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/__init__.pyi` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/__main__.py` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PaymentCryptographyControlPlane 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.PaymentCryptographyControlPlane 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane\nOther"
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

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/client.py` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/client.pyi` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/literals.py` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,15 @@
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
@@ -283,26 +284,28 @@
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

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/literals.pyi` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,15 @@
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
@@ -281,26 +282,28 @@
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

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/paginator.py` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,61 +33,56 @@
     ListKeysOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListAliasesPaginator", "ListKeysPaginator", "ListTagsForResourcePaginator")
 
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
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listaliasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAliasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listaliasespaginator)
         """
 
-
 class ListKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, KeyState: KeyStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyState: KeyStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listkeyspaginator)
         """
 
-
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/paginator.pyi` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,56 +33,61 @@
     ListKeysOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListAliasesPaginator", "ListKeysPaginator", "ListTagsForResourcePaginator")
 
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
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listaliasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAliasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listaliasespaginator)
         """
 
+
 class ListKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, KeyState: KeyStateType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, KeyState: KeyStateType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listkeyspaginator)
         """
 
+
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/type_defs.py` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,57 +35,60 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AliasTypeDef",
     "CreateAliasInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DeleteAliasInputRequestTypeDef",
     "DeleteKeyInputRequestTypeDef",
     "ExportTr31KeyBlockTypeDef",
     "ExportTr34KeyBlockTypeDef",
     "WrappedKeyTypeDef",
     "GetAliasInputRequestTypeDef",
     "GetKeyInputRequestTypeDef",
     "GetParametersForExportInputRequestTypeDef",
-    "GetParametersForExportOutputTypeDef",
     "GetParametersForImportInputRequestTypeDef",
-    "GetParametersForImportOutputTypeDef",
     "GetPublicKeyCertificateInputRequestTypeDef",
-    "GetPublicKeyCertificateOutputTypeDef",
     "ImportTr31KeyBlockTypeDef",
     "ImportTr34KeyBlockTypeDef",
+    "KeyModesOfUseOutputTypeDef",
     "KeyModesOfUseTypeDef",
-    "ListAliasesInputListAliasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAliasesInputRequestTypeDef",
-    "ListKeysInputListKeysPaginateTypeDef",
     "ListKeysInputRequestTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "RestoreKeyInputRequestTypeDef",
     "StartKeyUsageInputRequestTypeDef",
     "StopKeyUsageInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateAliasInputRequestTypeDef",
     "CreateAliasOutputTypeDef",
     "GetAliasOutputTypeDef",
+    "GetParametersForExportOutputTypeDef",
+    "GetParametersForImportOutputTypeDef",
+    "GetPublicKeyCertificateOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ExportKeyMaterialTypeDef",
     "ExportKeyOutputTypeDef",
+    "KeyAttributesOutputTypeDef",
     "KeyAttributesTypeDef",
+    "ListAliasesInputListAliasesPaginateTypeDef",
+    "ListKeysInputListKeysPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ExportKeyInputRequestTypeDef",
-    "CreateKeyInputRequestTypeDef",
     "KeySummaryTypeDef",
     "KeyTypeDef",
+    "CreateKeyInputRequestTypeDef",
     "RootCertificatePublicKeyTypeDef",
     "TrustedCertificatePublicKeyTypeDef",
     "ListKeysOutputTypeDef",
     "CreateKeyOutputTypeDef",
     "DeleteKeyOutputTypeDef",
     "GetKeyOutputTypeDef",
     "ImportKeyOutputTypeDef",
@@ -132,14 +135,25 @@
 
 class CreateAliasInputRequestTypeDef(
     _RequiredCreateAliasInputRequestTypeDef, _OptionalCreateAliasInputRequestTypeDef
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
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -241,62 +255,29 @@
     "GetParametersForExportInputRequestTypeDef",
     {
         "KeyMaterialType": KeyMaterialTypeType,
         "SigningKeyAlgorithm": KeyAlgorithmType,
     },
 )
 
-GetParametersForExportOutputTypeDef = TypedDict(
-    "GetParametersForExportOutputTypeDef",
-    {
-        "ExportToken": str,
-        "ParametersValidUntilTimestamp": datetime,
-        "SigningKeyAlgorithm": KeyAlgorithmType,
-        "SigningKeyCertificate": str,
-        "SigningKeyCertificateChain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetParametersForImportInputRequestTypeDef = TypedDict(
     "GetParametersForImportInputRequestTypeDef",
     {
         "KeyMaterialType": KeyMaterialTypeType,
         "WrappingKeyAlgorithm": KeyAlgorithmType,
     },
 )
 
-GetParametersForImportOutputTypeDef = TypedDict(
-    "GetParametersForImportOutputTypeDef",
-    {
-        "ImportToken": str,
-        "ParametersValidUntilTimestamp": datetime,
-        "WrappingKeyAlgorithm": KeyAlgorithmType,
-        "WrappingKeyCertificate": str,
-        "WrappingKeyCertificateChain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPublicKeyCertificateInputRequestTypeDef = TypedDict(
     "GetPublicKeyCertificateInputRequestTypeDef",
     {
         "KeyIdentifier": str,
     },
 )
 
-GetPublicKeyCertificateOutputTypeDef = TypedDict(
-    "GetPublicKeyCertificateOutputTypeDef",
-    {
-        "KeyCertificate": str,
-        "KeyCertificateChain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImportTr31KeyBlockTypeDef = TypedDict(
     "ImportTr31KeyBlockTypeDef",
     {
         "WrappedKeyBlock": str,
         "WrappingKeyIdentifier": str,
     },
 )
@@ -322,14 +303,30 @@
 
 class ImportTr34KeyBlockTypeDef(
     _RequiredImportTr34KeyBlockTypeDef, _OptionalImportTr34KeyBlockTypeDef
 ):
     pass
 
 
+KeyModesOfUseOutputTypeDef = TypedDict(
+    "KeyModesOfUseOutputTypeDef",
+    {
+        "Decrypt": bool,
+        "DeriveKey": bool,
+        "Encrypt": bool,
+        "Generate": bool,
+        "NoRestrictions": bool,
+        "Sign": bool,
+        "Unwrap": bool,
+        "Verify": bool,
+        "Wrap": bool,
+    },
+    total=False,
+)
+
 KeyModesOfUseTypeDef = TypedDict(
     "KeyModesOfUseTypeDef",
     {
         "Decrypt": bool,
         "DeriveKey": bool,
         "Encrypt": bool,
         "Generate": bool,
@@ -338,72 +335,43 @@
         "Unwrap": bool,
         "Verify": bool,
         "Wrap": bool,
     },
     total=False,
 )
 
-ListAliasesInputListAliasesPaginateTypeDef = TypedDict(
-    "ListAliasesInputListAliasesPaginateTypeDef",
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
 
 ListAliasesInputRequestTypeDef = TypedDict(
     "ListAliasesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListKeysInputListKeysPaginateTypeDef = TypedDict(
-    "ListKeysInputListKeysPaginateTypeDef",
-    {
-        "KeyState": KeyStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKeysInputRequestTypeDef = TypedDict(
     "ListKeysInputRequestTypeDef",
     {
         "KeyState": KeyStateType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -418,35 +386,33 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
     },
-    total=False,
 )
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Value": str,
     },
+    total=False,
 )
 
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+
 RestoreKeyInputRequestTypeDef = TypedDict(
     "RestoreKeyInputRequestTypeDef",
     {
         "KeyIdentifier": str,
     },
 )
 
@@ -493,49 +459,73 @@
     pass
 
 
 CreateAliasOutputTypeDef = TypedDict(
     "CreateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAliasOutputTypeDef = TypedDict(
     "GetAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetParametersForExportOutputTypeDef = TypedDict(
+    "GetParametersForExportOutputTypeDef",
+    {
+        "ExportToken": str,
+        "ParametersValidUntilTimestamp": datetime,
+        "SigningKeyAlgorithm": KeyAlgorithmType,
+        "SigningKeyCertificate": str,
+        "SigningKeyCertificateChain": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetParametersForImportOutputTypeDef = TypedDict(
+    "GetParametersForImportOutputTypeDef",
+    {
+        "ImportToken": str,
+        "ParametersValidUntilTimestamp": datetime,
+        "WrappingKeyAlgorithm": KeyAlgorithmType,
+        "WrappingKeyCertificate": str,
+        "WrappingKeyCertificateChain": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPublicKeyCertificateOutputTypeDef = TypedDict(
+    "GetPublicKeyCertificateOutputTypeDef",
+    {
+        "KeyCertificate": str,
+        "KeyCertificateChain": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAliasesOutputTypeDef = TypedDict(
     "ListAliasesOutputTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAliasOutputTypeDef = TypedDict(
     "UpdateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
@@ -552,80 +542,114 @@
     total=False,
 )
 
 ExportKeyOutputTypeDef = TypedDict(
     "ExportKeyOutputTypeDef",
     {
         "WrappedKey": WrappedKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KeyAttributesOutputTypeDef = TypedDict(
+    "KeyAttributesOutputTypeDef",
+    {
+        "KeyAlgorithm": KeyAlgorithmType,
+        "KeyClass": KeyClassType,
+        "KeyModesOfUse": KeyModesOfUseOutputTypeDef,
+        "KeyUsage": KeyUsageType,
     },
 )
 
 KeyAttributesTypeDef = TypedDict(
     "KeyAttributesTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "KeyClass": KeyClassType,
         "KeyModesOfUse": KeyModesOfUseTypeDef,
         "KeyUsage": KeyUsageType,
     },
 )
 
-ExportKeyInputRequestTypeDef = TypedDict(
-    "ExportKeyInputRequestTypeDef",
+ListAliasesInputListAliasesPaginateTypeDef = TypedDict(
+    "ListAliasesInputListAliasesPaginateTypeDef",
     {
-        "ExportKeyIdentifier": str,
-        "KeyMaterial": ExportKeyMaterialTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredCreateKeyInputRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyInputRequestTypeDef",
+ListKeysInputListKeysPaginateTypeDef = TypedDict(
+    "ListKeysInputListKeysPaginateTypeDef",
     {
-        "Exportable": bool,
-        "KeyAttributes": KeyAttributesTypeDef,
+        "KeyState": KeyStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalCreateKeyInputRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyInputRequestTypeDef",
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     {
-        "Enabled": bool,
-        "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
-        "Tags": Sequence[TagTypeDef],
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class CreateKeyInputRequestTypeDef(
-    _RequiredCreateKeyInputRequestTypeDef, _OptionalCreateKeyInputRequestTypeDef
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
 ):
     pass
 
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportKeyInputRequestTypeDef = TypedDict(
+    "ExportKeyInputRequestTypeDef",
+    {
+        "ExportKeyIdentifier": str,
+        "KeyMaterial": ExportKeyMaterialTypeDef,
+    },
+)
+
 KeySummaryTypeDef = TypedDict(
     "KeySummaryTypeDef",
     {
         "Enabled": bool,
         "Exportable": bool,
         "KeyArn": str,
-        "KeyAttributes": KeyAttributesTypeDef,
+        "KeyAttributes": KeyAttributesOutputTypeDef,
         "KeyCheckValue": str,
         "KeyState": KeyStateType,
     },
 )
 
 _RequiredKeyTypeDef = TypedDict(
     "_RequiredKeyTypeDef",
     {
         "CreateTimestamp": datetime,
         "Enabled": bool,
         "Exportable": bool,
         "KeyArn": str,
-        "KeyAttributes": KeyAttributesTypeDef,
+        "KeyAttributes": KeyAttributesOutputTypeDef,
         "KeyCheckValue": str,
         "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
         "KeyOrigin": KeyOriginType,
         "KeyState": KeyStateType,
     },
 )
 _OptionalKeyTypeDef = TypedDict(
@@ -640,14 +664,38 @@
 )
 
 
 class KeyTypeDef(_RequiredKeyTypeDef, _OptionalKeyTypeDef):
     pass
 
 
+_RequiredCreateKeyInputRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyInputRequestTypeDef",
+    {
+        "Exportable": bool,
+        "KeyAttributes": KeyAttributesTypeDef,
+    },
+)
+_OptionalCreateKeyInputRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyInputRequestTypeDef",
+    {
+        "Enabled": bool,
+        "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateKeyInputRequestTypeDef(
+    _RequiredCreateKeyInputRequestTypeDef, _OptionalCreateKeyInputRequestTypeDef
+):
+    pass
+
+
 RootCertificatePublicKeyTypeDef = TypedDict(
     "RootCertificatePublicKeyTypeDef",
     {
         "KeyAttributes": KeyAttributesTypeDef,
         "PublicKeyCertificate": str,
     },
 )
@@ -662,71 +710,71 @@
 )
 
 ListKeysOutputTypeDef = TypedDict(
     "ListKeysOutputTypeDef",
     {
         "Keys": List[KeySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateKeyOutputTypeDef = TypedDict(
     "CreateKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteKeyOutputTypeDef = TypedDict(
     "DeleteKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKeyOutputTypeDef = TypedDict(
     "GetKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportKeyOutputTypeDef = TypedDict(
     "ImportKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreKeyOutputTypeDef = TypedDict(
     "RestoreKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartKeyUsageOutputTypeDef = TypedDict(
     "StartKeyUsageOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopKeyUsageOutputTypeDef = TypedDict(
     "StopKeyUsageOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportKeyMaterialTypeDef = TypedDict(
     "ImportKeyMaterialTypeDef",
     {
         "RootCertificatePublicKey": RootCertificatePublicKeyTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography/type_defs.pyi` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -34,57 +34,60 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AliasTypeDef",
     "CreateAliasInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DeleteAliasInputRequestTypeDef",
     "DeleteKeyInputRequestTypeDef",
     "ExportTr31KeyBlockTypeDef",
     "ExportTr34KeyBlockTypeDef",
     "WrappedKeyTypeDef",
     "GetAliasInputRequestTypeDef",
     "GetKeyInputRequestTypeDef",
     "GetParametersForExportInputRequestTypeDef",
-    "GetParametersForExportOutputTypeDef",
     "GetParametersForImportInputRequestTypeDef",
-    "GetParametersForImportOutputTypeDef",
     "GetPublicKeyCertificateInputRequestTypeDef",
-    "GetPublicKeyCertificateOutputTypeDef",
     "ImportTr31KeyBlockTypeDef",
     "ImportTr34KeyBlockTypeDef",
+    "KeyModesOfUseOutputTypeDef",
     "KeyModesOfUseTypeDef",
-    "ListAliasesInputListAliasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAliasesInputRequestTypeDef",
-    "ListKeysInputListKeysPaginateTypeDef",
     "ListKeysInputRequestTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "RestoreKeyInputRequestTypeDef",
     "StartKeyUsageInputRequestTypeDef",
     "StopKeyUsageInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateAliasInputRequestTypeDef",
     "CreateAliasOutputTypeDef",
     "GetAliasOutputTypeDef",
+    "GetParametersForExportOutputTypeDef",
+    "GetParametersForImportOutputTypeDef",
+    "GetPublicKeyCertificateOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ExportKeyMaterialTypeDef",
     "ExportKeyOutputTypeDef",
+    "KeyAttributesOutputTypeDef",
     "KeyAttributesTypeDef",
+    "ListAliasesInputListAliasesPaginateTypeDef",
+    "ListKeysInputListKeysPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ExportKeyInputRequestTypeDef",
-    "CreateKeyInputRequestTypeDef",
     "KeySummaryTypeDef",
     "KeyTypeDef",
+    "CreateKeyInputRequestTypeDef",
     "RootCertificatePublicKeyTypeDef",
     "TrustedCertificatePublicKeyTypeDef",
     "ListKeysOutputTypeDef",
     "CreateKeyOutputTypeDef",
     "DeleteKeyOutputTypeDef",
     "GetKeyOutputTypeDef",
     "ImportKeyOutputTypeDef",
@@ -127,14 +130,25 @@
 )
 
 class CreateAliasInputRequestTypeDef(
     _RequiredCreateAliasInputRequestTypeDef, _OptionalCreateAliasInputRequestTypeDef
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
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -230,62 +244,29 @@
     "GetParametersForExportInputRequestTypeDef",
     {
         "KeyMaterialType": KeyMaterialTypeType,
         "SigningKeyAlgorithm": KeyAlgorithmType,
     },
 )
 
-GetParametersForExportOutputTypeDef = TypedDict(
-    "GetParametersForExportOutputTypeDef",
-    {
-        "ExportToken": str,
-        "ParametersValidUntilTimestamp": datetime,
-        "SigningKeyAlgorithm": KeyAlgorithmType,
-        "SigningKeyCertificate": str,
-        "SigningKeyCertificateChain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetParametersForImportInputRequestTypeDef = TypedDict(
     "GetParametersForImportInputRequestTypeDef",
     {
         "KeyMaterialType": KeyMaterialTypeType,
         "WrappingKeyAlgorithm": KeyAlgorithmType,
     },
 )
 
-GetParametersForImportOutputTypeDef = TypedDict(
-    "GetParametersForImportOutputTypeDef",
-    {
-        "ImportToken": str,
-        "ParametersValidUntilTimestamp": datetime,
-        "WrappingKeyAlgorithm": KeyAlgorithmType,
-        "WrappingKeyCertificate": str,
-        "WrappingKeyCertificateChain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPublicKeyCertificateInputRequestTypeDef = TypedDict(
     "GetPublicKeyCertificateInputRequestTypeDef",
     {
         "KeyIdentifier": str,
     },
 )
 
-GetPublicKeyCertificateOutputTypeDef = TypedDict(
-    "GetPublicKeyCertificateOutputTypeDef",
-    {
-        "KeyCertificate": str,
-        "KeyCertificateChain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImportTr31KeyBlockTypeDef = TypedDict(
     "ImportTr31KeyBlockTypeDef",
     {
         "WrappedKeyBlock": str,
         "WrappingKeyIdentifier": str,
     },
 )
@@ -309,14 +290,30 @@
 )
 
 class ImportTr34KeyBlockTypeDef(
     _RequiredImportTr34KeyBlockTypeDef, _OptionalImportTr34KeyBlockTypeDef
 ):
     pass
 
+KeyModesOfUseOutputTypeDef = TypedDict(
+    "KeyModesOfUseOutputTypeDef",
+    {
+        "Decrypt": bool,
+        "DeriveKey": bool,
+        "Encrypt": bool,
+        "Generate": bool,
+        "NoRestrictions": bool,
+        "Sign": bool,
+        "Unwrap": bool,
+        "Verify": bool,
+        "Wrap": bool,
+    },
+    total=False,
+)
+
 KeyModesOfUseTypeDef = TypedDict(
     "KeyModesOfUseTypeDef",
     {
         "Decrypt": bool,
         "DeriveKey": bool,
         "Encrypt": bool,
         "Generate": bool,
@@ -325,70 +322,43 @@
         "Unwrap": bool,
         "Verify": bool,
         "Wrap": bool,
     },
     total=False,
 )
 
-ListAliasesInputListAliasesPaginateTypeDef = TypedDict(
-    "ListAliasesInputListAliasesPaginateTypeDef",
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
 
 ListAliasesInputRequestTypeDef = TypedDict(
     "ListAliasesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListKeysInputListKeysPaginateTypeDef = TypedDict(
-    "ListKeysInputListKeysPaginateTypeDef",
-    {
-        "KeyState": KeyStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKeysInputRequestTypeDef = TypedDict(
     "ListKeysInputRequestTypeDef",
     {
         "KeyState": KeyStateType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -401,35 +371,31 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
     },
-    total=False,
 )
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Value": str,
     },
+    total=False,
 )
 
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
 RestoreKeyInputRequestTypeDef = TypedDict(
     "RestoreKeyInputRequestTypeDef",
     {
         "KeyIdentifier": str,
     },
 )
 
@@ -474,49 +440,73 @@
 ):
     pass
 
 CreateAliasOutputTypeDef = TypedDict(
     "CreateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAliasOutputTypeDef = TypedDict(
     "GetAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetParametersForExportOutputTypeDef = TypedDict(
+    "GetParametersForExportOutputTypeDef",
+    {
+        "ExportToken": str,
+        "ParametersValidUntilTimestamp": datetime,
+        "SigningKeyAlgorithm": KeyAlgorithmType,
+        "SigningKeyCertificate": str,
+        "SigningKeyCertificateChain": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetParametersForImportOutputTypeDef = TypedDict(
+    "GetParametersForImportOutputTypeDef",
+    {
+        "ImportToken": str,
+        "ParametersValidUntilTimestamp": datetime,
+        "WrappingKeyAlgorithm": KeyAlgorithmType,
+        "WrappingKeyCertificate": str,
+        "WrappingKeyCertificateChain": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPublicKeyCertificateOutputTypeDef = TypedDict(
+    "GetPublicKeyCertificateOutputTypeDef",
+    {
+        "KeyCertificate": str,
+        "KeyCertificateChain": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAliasesOutputTypeDef = TypedDict(
     "ListAliasesOutputTypeDef",
     {
         "Aliases": List[AliasTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAliasOutputTypeDef = TypedDict(
     "UpdateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
@@ -533,78 +523,112 @@
     total=False,
 )
 
 ExportKeyOutputTypeDef = TypedDict(
     "ExportKeyOutputTypeDef",
     {
         "WrappedKey": WrappedKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+KeyAttributesOutputTypeDef = TypedDict(
+    "KeyAttributesOutputTypeDef",
+    {
+        "KeyAlgorithm": KeyAlgorithmType,
+        "KeyClass": KeyClassType,
+        "KeyModesOfUse": KeyModesOfUseOutputTypeDef,
+        "KeyUsage": KeyUsageType,
     },
 )
 
 KeyAttributesTypeDef = TypedDict(
     "KeyAttributesTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "KeyClass": KeyClassType,
         "KeyModesOfUse": KeyModesOfUseTypeDef,
         "KeyUsage": KeyUsageType,
     },
 )
 
-ExportKeyInputRequestTypeDef = TypedDict(
-    "ExportKeyInputRequestTypeDef",
+ListAliasesInputListAliasesPaginateTypeDef = TypedDict(
+    "ListAliasesInputListAliasesPaginateTypeDef",
     {
-        "ExportKeyIdentifier": str,
-        "KeyMaterial": ExportKeyMaterialTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredCreateKeyInputRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyInputRequestTypeDef",
+ListKeysInputListKeysPaginateTypeDef = TypedDict(
+    "ListKeysInputListKeysPaginateTypeDef",
     {
-        "Exportable": bool,
-        "KeyAttributes": KeyAttributesTypeDef,
+        "KeyState": KeyStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalCreateKeyInputRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyInputRequestTypeDef",
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     {
-        "Enabled": bool,
-        "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
-        "Tags": Sequence[TagTypeDef],
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class CreateKeyInputRequestTypeDef(
-    _RequiredCreateKeyInputRequestTypeDef, _OptionalCreateKeyInputRequestTypeDef
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportKeyInputRequestTypeDef = TypedDict(
+    "ExportKeyInputRequestTypeDef",
+    {
+        "ExportKeyIdentifier": str,
+        "KeyMaterial": ExportKeyMaterialTypeDef,
+    },
+)
+
 KeySummaryTypeDef = TypedDict(
     "KeySummaryTypeDef",
     {
         "Enabled": bool,
         "Exportable": bool,
         "KeyArn": str,
-        "KeyAttributes": KeyAttributesTypeDef,
+        "KeyAttributes": KeyAttributesOutputTypeDef,
         "KeyCheckValue": str,
         "KeyState": KeyStateType,
     },
 )
 
 _RequiredKeyTypeDef = TypedDict(
     "_RequiredKeyTypeDef",
     {
         "CreateTimestamp": datetime,
         "Enabled": bool,
         "Exportable": bool,
         "KeyArn": str,
-        "KeyAttributes": KeyAttributesTypeDef,
+        "KeyAttributes": KeyAttributesOutputTypeDef,
         "KeyCheckValue": str,
         "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
         "KeyOrigin": KeyOriginType,
         "KeyState": KeyStateType,
     },
 )
 _OptionalKeyTypeDef = TypedDict(
@@ -617,14 +641,36 @@
     },
     total=False,
 )
 
 class KeyTypeDef(_RequiredKeyTypeDef, _OptionalKeyTypeDef):
     pass
 
+_RequiredCreateKeyInputRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyInputRequestTypeDef",
+    {
+        "Exportable": bool,
+        "KeyAttributes": KeyAttributesTypeDef,
+    },
+)
+_OptionalCreateKeyInputRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyInputRequestTypeDef",
+    {
+        "Enabled": bool,
+        "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateKeyInputRequestTypeDef(
+    _RequiredCreateKeyInputRequestTypeDef, _OptionalCreateKeyInputRequestTypeDef
+):
+    pass
+
 RootCertificatePublicKeyTypeDef = TypedDict(
     "RootCertificatePublicKeyTypeDef",
     {
         "KeyAttributes": KeyAttributesTypeDef,
         "PublicKeyCertificate": str,
     },
 )
@@ -639,71 +685,71 @@
 )
 
 ListKeysOutputTypeDef = TypedDict(
     "ListKeysOutputTypeDef",
     {
         "Keys": List[KeySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateKeyOutputTypeDef = TypedDict(
     "CreateKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteKeyOutputTypeDef = TypedDict(
     "DeleteKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKeyOutputTypeDef = TypedDict(
     "GetKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportKeyOutputTypeDef = TypedDict(
     "ImportKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreKeyOutputTypeDef = TypedDict(
     "RestoreKeyOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartKeyUsageOutputTypeDef = TypedDict(
     "StartKeyUsageOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopKeyUsageOutputTypeDef = TypedDict(
     "StopKeyUsageOutputTypeDef",
     {
         "Key": KeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportKeyMaterialTypeDef = TypedDict(
     "ImportKeyMaterialTypeDef",
     {
         "RootCertificatePublicKey": RootCertificatePublicKeyTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography.egg-info/PKG-INFO` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography
-Version: 1.28.0
-Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-payment-cryptography"></a>
 
 # mypy-boto3-payment-cryptography
 
 [![PyPI - mypy-boto3-payment-cryptography](https://img.shields.io/pypi/v/mypy-boto3-payment-cryptography.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-payment-cryptography?color=blue)](https://pypistats.org/packages/mypy-boto3-payment-cryptography)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-payment-cryptography)](https://pepy.tech/project/mypy-boto3-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyControlPlane 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[boto3.PaymentCryptographyControlPlane 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
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
 [mypy-boto3-payment-cryptography docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,57 +340,60 @@
 `mypy_boto3_payment_cryptography.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_payment_cryptography.type_defs import (
     AliasTypeDef,
     CreateAliasInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     DeleteAliasInputRequestTypeDef,
     DeleteKeyInputRequestTypeDef,
     ExportTr31KeyBlockTypeDef,
     ExportTr34KeyBlockTypeDef,
     WrappedKeyTypeDef,
     GetAliasInputRequestTypeDef,
     GetKeyInputRequestTypeDef,
     GetParametersForExportInputRequestTypeDef,
-    GetParametersForExportOutputTypeDef,
     GetParametersForImportInputRequestTypeDef,
-    GetParametersForImportOutputTypeDef,
     GetPublicKeyCertificateInputRequestTypeDef,
-    GetPublicKeyCertificateOutputTypeDef,
     ImportTr31KeyBlockTypeDef,
     ImportTr34KeyBlockTypeDef,
+    KeyModesOfUseOutputTypeDef,
     KeyModesOfUseTypeDef,
-    ListAliasesInputListAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAliasesInputRequestTypeDef,
-    ListKeysInputListKeysPaginateTypeDef,
     ListKeysInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     RestoreKeyInputRequestTypeDef,
     StartKeyUsageInputRequestTypeDef,
     StopKeyUsageInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateAliasInputRequestTypeDef,
     CreateAliasOutputTypeDef,
     GetAliasOutputTypeDef,
+    GetParametersForExportOutputTypeDef,
+    GetParametersForImportOutputTypeDef,
+    GetPublicKeyCertificateOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ExportKeyMaterialTypeDef,
     ExportKeyOutputTypeDef,
+    KeyAttributesOutputTypeDef,
     KeyAttributesTypeDef,
+    ListAliasesInputListAliasesPaginateTypeDef,
+    ListKeysInputListKeysPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ExportKeyInputRequestTypeDef,
-    CreateKeyInputRequestTypeDef,
     KeySummaryTypeDef,
     KeyTypeDef,
+    CreateKeyInputRequestTypeDef,
     RootCertificatePublicKeyTypeDef,
     TrustedCertificatePublicKeyTypeDef,
     ListKeysOutputTypeDef,
     CreateKeyOutputTypeDef,
     DeleteKeyOutputTypeDef,
     GetKeyOutputTypeDef,
     ImportKeyOutputTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.28.0/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt` & `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.0/setup.py` & `mypy-boto3-payment-cryptography-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-payment-cryptography",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_payment_cryptography"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PaymentCryptographyControlPlane 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.PaymentCryptographyControlPlane 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

