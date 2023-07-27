# Comparing `tmp/mypy-boto3-payment-cryptography-data-1.28.0.tar.gz` & `tmp/mypy-boto3-payment-cryptography-data-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-payment-cryptography-data-1.28.0.tar", last modified: Thu Jul  6 21:00:16 2023, max compression
+gzip compressed data, was "mypy-boto3-payment-cryptography-data-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
```

## Comparing `mypy-boto3-payment-cryptography-data-1.28.0.tar` & `mypy-boto3-payment-cryptography-data-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:16.410388 mypy-boto3-payment-cryptography-data-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:04.000000 mypy-boto3-payment-cryptography-data-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-07-06 21:00:16.406388 mypy-boto3-payment-cryptography-data-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-06 20:49:04.000000 mypy-boto3-payment-cryptography-data-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:16.406388 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-06 20:49:04.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-06 20:49:04.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-06 20:49:04.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-06 20:49:04.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-06 20:49:04.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-06 20:49:07.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-07-06 20:49:04.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:04.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24022 2023-07-06 20:49:07.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-07-06 20:49:07.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:04.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:16.406388 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-07-06 21:00:16.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-06 21:00:16.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:16.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:16.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:16.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 21:00:16.000000 mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:16.410388 mypy-boto3-payment-cryptography-data-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-06 20:49:04.000000 mypy-boto3-payment-cryptography-data-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.845133 mypy-boto3-payment-cryptography-data-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:14.000000 mypy-boto3-payment-cryptography-data-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15354 2023-07-27 11:49:21.845133 mypy-boto3-payment-cryptography-data-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-07-27 11:41:14.000000 mypy-boto3-payment-cryptography-data-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.837133 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-27 11:41:14.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-27 11:41:14.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-27 11:41:14.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-27 11:41:14.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-27 11:41:14.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-07-27 11:41:14.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-07-27 11:41:14.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:14.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24000 2023-07-27 11:41:15.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23976 2023-07-27 11:41:15.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:14.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.845133 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15354 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.845133 mypy-boto3-payment-cryptography-data-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-27 11:41:14.000000 mypy-boto3-payment-cryptography-data-1.28.12/setup.py
```

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/LICENSE` & `mypy-boto3-payment-cryptography-data-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/PKG-INFO` & `mypy-boto3-payment-cryptography-data-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography-data
-Version: 1.28.0
-Summary: Type annotations for boto3.PaymentCryptographyDataPlane 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PaymentCryptographyDataPlane 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-payment-cryptography-data"></a>
 
 # mypy-boto3-payment-cryptography-data
 
 [![PyPI - mypy-boto3-payment-cryptography-data](https://img.shields.io/pypi/v/mypy-boto3-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-payment-cryptography-data?color=blue)](https://pypistats.org/packages/mypy-boto3-payment-cryptography-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-payment-cryptography-data)](https://pepy.tech/project/mypy-boto3-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyDataPlane 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[boto3.PaymentCryptographyDataPlane 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
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
 [mypy-boto3-payment-cryptography-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,49 +316,49 @@
     CardVerificationValue1TypeDef,
     CardVerificationValue2TypeDef,
     DynamicCardVerificationCodeTypeDef,
     DynamicCardVerificationValueTypeDef,
     DiscoverDynamicCardVerificationCodeTypeDef,
     CryptogramVerificationArpcMethod1TypeDef,
     CryptogramVerificationArpcMethod2TypeDef,
-    DecryptDataOutputTypeDef,
+    ResponseMetadataTypeDef,
     DukptAttributesTypeDef,
     DukptDerivationAttributesTypeDef,
     DukptEncryptionAttributesTypeDef,
-    EncryptDataOutputTypeDef,
     SymmetricEncryptionAttributesTypeDef,
-    GenerateCardValidationDataOutputTypeDef,
-    GenerateMacOutputTypeDef,
     PinDataTypeDef,
     Ibm3624NaturalPinTypeDef,
     Ibm3624PinFromOffsetTypeDef,
     Ibm3624PinOffsetTypeDef,
     Ibm3624PinVerificationTypeDef,
     Ibm3624RandomPinTypeDef,
     MacAlgorithmDukptTypeDef,
     SessionKeyDerivationValueTypeDef,
     VisaPinTypeDef,
     VisaPinVerificationValueTypeDef,
     VisaPinVerificationTypeDef,
-    ReEncryptDataOutputTypeDef,
-    ResponseMetadataTypeDef,
     SessionKeyAmexTypeDef,
     SessionKeyEmv2000TypeDef,
     SessionKeyEmvCommonTypeDef,
     SessionKeyMastercardTypeDef,
     SessionKeyVisaTypeDef,
-    TranslatePinDataOutputTypeDef,
     TranslationPinDataIsoFormat034TypeDef,
+    CardGenerationAttributesTypeDef,
+    CardVerificationAttributesTypeDef,
+    CryptogramAuthResponseTypeDef,
+    DecryptDataOutputTypeDef,
+    EncryptDataOutputTypeDef,
+    GenerateCardValidationDataOutputTypeDef,
+    GenerateMacOutputTypeDef,
+    ReEncryptDataOutputTypeDef,
+    TranslatePinDataOutputTypeDef,
     VerifyAuthRequestCryptogramOutputTypeDef,
     VerifyCardValidationDataOutputTypeDef,
     VerifyMacOutputTypeDef,
     VerifyPinDataOutputTypeDef,
-    CardGenerationAttributesTypeDef,
-    CardVerificationAttributesTypeDef,
-    CryptogramAuthResponseTypeDef,
     EncryptionDecryptionAttributesTypeDef,
     ReEncryptionAttributesTypeDef,
     GeneratePinDataOutputTypeDef,
     MacAlgorithmEmvTypeDef,
     PinGenerationAttributesTypeDef,
     PinVerificationAttributesTypeDef,
     SessionKeyDerivationTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/README.md` & `mypy-boto3-payment-cryptography-data-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-payment-cryptography-data"></a>
 
 # mypy-boto3-payment-cryptography-data
 
 [![PyPI - mypy-boto3-payment-cryptography-data](https://img.shields.io/pypi/v/mypy-boto3-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-payment-cryptography-data?color=blue)](https://pypistats.org/packages/mypy-boto3-payment-cryptography-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-payment-cryptography-data)](https://pepy.tech/project/mypy-boto3-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyDataPlane 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[boto3.PaymentCryptographyDataPlane 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
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
 [mypy-boto3-payment-cryptography-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,49 +284,49 @@
     CardVerificationValue1TypeDef,
     CardVerificationValue2TypeDef,
     DynamicCardVerificationCodeTypeDef,
     DynamicCardVerificationValueTypeDef,
     DiscoverDynamicCardVerificationCodeTypeDef,
     CryptogramVerificationArpcMethod1TypeDef,
     CryptogramVerificationArpcMethod2TypeDef,
-    DecryptDataOutputTypeDef,
+    ResponseMetadataTypeDef,
     DukptAttributesTypeDef,
     DukptDerivationAttributesTypeDef,
     DukptEncryptionAttributesTypeDef,
-    EncryptDataOutputTypeDef,
     SymmetricEncryptionAttributesTypeDef,
-    GenerateCardValidationDataOutputTypeDef,
-    GenerateMacOutputTypeDef,
     PinDataTypeDef,
     Ibm3624NaturalPinTypeDef,
     Ibm3624PinFromOffsetTypeDef,
     Ibm3624PinOffsetTypeDef,
     Ibm3624PinVerificationTypeDef,
     Ibm3624RandomPinTypeDef,
     MacAlgorithmDukptTypeDef,
     SessionKeyDerivationValueTypeDef,
     VisaPinTypeDef,
     VisaPinVerificationValueTypeDef,
     VisaPinVerificationTypeDef,
-    ReEncryptDataOutputTypeDef,
-    ResponseMetadataTypeDef,
     SessionKeyAmexTypeDef,
     SessionKeyEmv2000TypeDef,
     SessionKeyEmvCommonTypeDef,
     SessionKeyMastercardTypeDef,
     SessionKeyVisaTypeDef,
-    TranslatePinDataOutputTypeDef,
     TranslationPinDataIsoFormat034TypeDef,
+    CardGenerationAttributesTypeDef,
+    CardVerificationAttributesTypeDef,
+    CryptogramAuthResponseTypeDef,
+    DecryptDataOutputTypeDef,
+    EncryptDataOutputTypeDef,
+    GenerateCardValidationDataOutputTypeDef,
+    GenerateMacOutputTypeDef,
+    ReEncryptDataOutputTypeDef,
+    TranslatePinDataOutputTypeDef,
     VerifyAuthRequestCryptogramOutputTypeDef,
     VerifyCardValidationDataOutputTypeDef,
     VerifyMacOutputTypeDef,
     VerifyPinDataOutputTypeDef,
-    CardGenerationAttributesTypeDef,
-    CardVerificationAttributesTypeDef,
-    CryptogramAuthResponseTypeDef,
     EncryptionDecryptionAttributesTypeDef,
     ReEncryptionAttributesTypeDef,
     GeneratePinDataOutputTypeDef,
     MacAlgorithmEmvTypeDef,
     PinGenerationAttributesTypeDef,
     PinVerificationAttributesTypeDef,
     SessionKeyDerivationTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/__init__.py` & `mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/__init__.pyi` & `mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/__main__.py` & `mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PaymentCryptographyDataPlane 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.PaymentCryptographyDataPlane 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane\nOther"
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

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/client.py` & `mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/client.pyi` & `mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/literals.py` & `mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/literals.py`

 * *Files 1% similar despite different names*

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

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/literals.pyi` & `mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,15 @@
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
@@ -254,26 +255,28 @@
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

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/type_defs.py` & `mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,49 +40,49 @@
     "CardVerificationValue1TypeDef",
     "CardVerificationValue2TypeDef",
     "DynamicCardVerificationCodeTypeDef",
     "DynamicCardVerificationValueTypeDef",
     "DiscoverDynamicCardVerificationCodeTypeDef",
     "CryptogramVerificationArpcMethod1TypeDef",
     "CryptogramVerificationArpcMethod2TypeDef",
-    "DecryptDataOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DukptAttributesTypeDef",
     "DukptDerivationAttributesTypeDef",
     "DukptEncryptionAttributesTypeDef",
-    "EncryptDataOutputTypeDef",
     "SymmetricEncryptionAttributesTypeDef",
-    "GenerateCardValidationDataOutputTypeDef",
-    "GenerateMacOutputTypeDef",
     "PinDataTypeDef",
     "Ibm3624NaturalPinTypeDef",
     "Ibm3624PinFromOffsetTypeDef",
     "Ibm3624PinOffsetTypeDef",
     "Ibm3624PinVerificationTypeDef",
     "Ibm3624RandomPinTypeDef",
     "MacAlgorithmDukptTypeDef",
     "SessionKeyDerivationValueTypeDef",
     "VisaPinTypeDef",
     "VisaPinVerificationValueTypeDef",
     "VisaPinVerificationTypeDef",
-    "ReEncryptDataOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SessionKeyAmexTypeDef",
     "SessionKeyEmv2000TypeDef",
     "SessionKeyEmvCommonTypeDef",
     "SessionKeyMastercardTypeDef",
     "SessionKeyVisaTypeDef",
-    "TranslatePinDataOutputTypeDef",
     "TranslationPinDataIsoFormat034TypeDef",
+    "CardGenerationAttributesTypeDef",
+    "CardVerificationAttributesTypeDef",
+    "CryptogramAuthResponseTypeDef",
+    "DecryptDataOutputTypeDef",
+    "EncryptDataOutputTypeDef",
+    "GenerateCardValidationDataOutputTypeDef",
+    "GenerateMacOutputTypeDef",
+    "ReEncryptDataOutputTypeDef",
+    "TranslatePinDataOutputTypeDef",
     "VerifyAuthRequestCryptogramOutputTypeDef",
     "VerifyCardValidationDataOutputTypeDef",
     "VerifyMacOutputTypeDef",
     "VerifyPinDataOutputTypeDef",
-    "CardGenerationAttributesTypeDef",
-    "CardVerificationAttributesTypeDef",
-    "CryptogramAuthResponseTypeDef",
     "EncryptionDecryptionAttributesTypeDef",
     "ReEncryptionAttributesTypeDef",
     "GeneratePinDataOutputTypeDef",
     "MacAlgorithmEmvTypeDef",
     "PinGenerationAttributesTypeDef",
     "PinVerificationAttributesTypeDef",
     "SessionKeyDerivationTypeDef",
@@ -202,21 +202,22 @@
 class CryptogramVerificationArpcMethod2TypeDef(
     _RequiredCryptogramVerificationArpcMethod2TypeDef,
     _OptionalCryptogramVerificationArpcMethod2TypeDef,
 ):
     pass
 
 
-DecryptDataOutputTypeDef = TypedDict(
-    "DecryptDataOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "PlainText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DukptAttributesTypeDef = TypedDict(
     "DukptAttributesTypeDef",
     {
         "DukptDerivationType": DukptDerivationTypeType,
@@ -266,24 +267,14 @@
 
 class DukptEncryptionAttributesTypeDef(
     _RequiredDukptEncryptionAttributesTypeDef, _OptionalDukptEncryptionAttributesTypeDef
 ):
     pass
 
 
-EncryptDataOutputTypeDef = TypedDict(
-    "EncryptDataOutputTypeDef",
-    {
-        "CipherText": str,
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSymmetricEncryptionAttributesTypeDef = TypedDict(
     "_RequiredSymmetricEncryptionAttributesTypeDef",
     {
         "Mode": EncryptionModeType,
     },
 )
 _OptionalSymmetricEncryptionAttributesTypeDef = TypedDict(
@@ -298,34 +289,14 @@
 
 class SymmetricEncryptionAttributesTypeDef(
     _RequiredSymmetricEncryptionAttributesTypeDef, _OptionalSymmetricEncryptionAttributesTypeDef
 ):
     pass
 
 
-GenerateCardValidationDataOutputTypeDef = TypedDict(
-    "GenerateCardValidationDataOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ValidationData": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateMacOutputTypeDef = TypedDict(
-    "GenerateMacOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "Mac": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PinDataTypeDef = TypedDict(
     "PinDataTypeDef",
     {
         "PinOffset": str,
         "VerificationValue": str,
     },
     total=False,
@@ -429,35 +400,14 @@
     "VisaPinVerificationTypeDef",
     {
         "PinVerificationKeyIndex": int,
         "VerificationValue": str,
     },
 )
 
-ReEncryptDataOutputTypeDef = TypedDict(
-    "ReEncryptDataOutputTypeDef",
-    {
-        "CipherText": str,
-        "KeyArn": str,
-        "KeyCheckValue": str,
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
 SessionKeyAmexTypeDef = TypedDict(
     "SessionKeyAmexTypeDef",
     {
         "PanSequenceNumber": str,
         "PrimaryAccountNumber": str,
     },
 )
@@ -494,70 +444,21 @@
     "SessionKeyVisaTypeDef",
     {
         "PanSequenceNumber": str,
         "PrimaryAccountNumber": str,
     },
 )
 
-TranslatePinDataOutputTypeDef = TypedDict(
-    "TranslatePinDataOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "PinBlock": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TranslationPinDataIsoFormat034TypeDef = TypedDict(
     "TranslationPinDataIsoFormat034TypeDef",
     {
         "PrimaryAccountNumber": str,
     },
 )
 
-VerifyAuthRequestCryptogramOutputTypeDef = TypedDict(
-    "VerifyAuthRequestCryptogramOutputTypeDef",
-    {
-        "AuthResponseValue": str,
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-VerifyCardValidationDataOutputTypeDef = TypedDict(
-    "VerifyCardValidationDataOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-VerifyMacOutputTypeDef = TypedDict(
-    "VerifyMacOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-VerifyPinDataOutputTypeDef = TypedDict(
-    "VerifyPinDataOutputTypeDef",
-    {
-        "EncryptionKeyArn": str,
-        "EncryptionKeyCheckValue": str,
-        "VerificationKeyArn": str,
-        "VerificationKeyCheckValue": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CardGenerationAttributesTypeDef = TypedDict(
     "CardGenerationAttributesTypeDef",
     {
         "AmexCardSecurityCodeVersion1": AmexCardSecurityCodeVersion1TypeDef,
         "AmexCardSecurityCodeVersion2": AmexCardSecurityCodeVersion2TypeDef,
         "CardHolderVerificationValue": CardHolderVerificationValueTypeDef,
         "CardVerificationValue1": CardVerificationValue1TypeDef,
@@ -588,14 +489,113 @@
     {
         "ArpcMethod1": CryptogramVerificationArpcMethod1TypeDef,
         "ArpcMethod2": CryptogramVerificationArpcMethod2TypeDef,
     },
     total=False,
 )
 
+DecryptDataOutputTypeDef = TypedDict(
+    "DecryptDataOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "PlainText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EncryptDataOutputTypeDef = TypedDict(
+    "EncryptDataOutputTypeDef",
+    {
+        "CipherText": str,
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateCardValidationDataOutputTypeDef = TypedDict(
+    "GenerateCardValidationDataOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ValidationData": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateMacOutputTypeDef = TypedDict(
+    "GenerateMacOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "Mac": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReEncryptDataOutputTypeDef = TypedDict(
+    "ReEncryptDataOutputTypeDef",
+    {
+        "CipherText": str,
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TranslatePinDataOutputTypeDef = TypedDict(
+    "TranslatePinDataOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "PinBlock": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyAuthRequestCryptogramOutputTypeDef = TypedDict(
+    "VerifyAuthRequestCryptogramOutputTypeDef",
+    {
+        "AuthResponseValue": str,
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyCardValidationDataOutputTypeDef = TypedDict(
+    "VerifyCardValidationDataOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyMacOutputTypeDef = TypedDict(
+    "VerifyMacOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyPinDataOutputTypeDef = TypedDict(
+    "VerifyPinDataOutputTypeDef",
+    {
+        "EncryptionKeyArn": str,
+        "EncryptionKeyCheckValue": str,
+        "VerificationKeyArn": str,
+        "VerificationKeyCheckValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EncryptionDecryptionAttributesTypeDef = TypedDict(
     "EncryptionDecryptionAttributesTypeDef",
     {
         "Asymmetric": AsymmetricEncryptionAttributesTypeDef,
         "Dukpt": DukptEncryptionAttributesTypeDef,
         "Symmetric": SymmetricEncryptionAttributesTypeDef,
     },
@@ -616,15 +616,15 @@
     {
         "EncryptedPinBlock": str,
         "EncryptionKeyArn": str,
         "EncryptionKeyCheckValue": str,
         "GenerationKeyArn": str,
         "GenerationKeyCheckValue": str,
         "PinData": PinDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MacAlgorithmEmvTypeDef = TypedDict(
     "MacAlgorithmEmvTypeDef",
     {
         "MajorKeyDerivationMode": MajorKeyDerivationModeType,
```

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data/type_defs.pyi` & `mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -39,49 +39,49 @@
     "CardVerificationValue1TypeDef",
     "CardVerificationValue2TypeDef",
     "DynamicCardVerificationCodeTypeDef",
     "DynamicCardVerificationValueTypeDef",
     "DiscoverDynamicCardVerificationCodeTypeDef",
     "CryptogramVerificationArpcMethod1TypeDef",
     "CryptogramVerificationArpcMethod2TypeDef",
-    "DecryptDataOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DukptAttributesTypeDef",
     "DukptDerivationAttributesTypeDef",
     "DukptEncryptionAttributesTypeDef",
-    "EncryptDataOutputTypeDef",
     "SymmetricEncryptionAttributesTypeDef",
-    "GenerateCardValidationDataOutputTypeDef",
-    "GenerateMacOutputTypeDef",
     "PinDataTypeDef",
     "Ibm3624NaturalPinTypeDef",
     "Ibm3624PinFromOffsetTypeDef",
     "Ibm3624PinOffsetTypeDef",
     "Ibm3624PinVerificationTypeDef",
     "Ibm3624RandomPinTypeDef",
     "MacAlgorithmDukptTypeDef",
     "SessionKeyDerivationValueTypeDef",
     "VisaPinTypeDef",
     "VisaPinVerificationValueTypeDef",
     "VisaPinVerificationTypeDef",
-    "ReEncryptDataOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SessionKeyAmexTypeDef",
     "SessionKeyEmv2000TypeDef",
     "SessionKeyEmvCommonTypeDef",
     "SessionKeyMastercardTypeDef",
     "SessionKeyVisaTypeDef",
-    "TranslatePinDataOutputTypeDef",
     "TranslationPinDataIsoFormat034TypeDef",
+    "CardGenerationAttributesTypeDef",
+    "CardVerificationAttributesTypeDef",
+    "CryptogramAuthResponseTypeDef",
+    "DecryptDataOutputTypeDef",
+    "EncryptDataOutputTypeDef",
+    "GenerateCardValidationDataOutputTypeDef",
+    "GenerateMacOutputTypeDef",
+    "ReEncryptDataOutputTypeDef",
+    "TranslatePinDataOutputTypeDef",
     "VerifyAuthRequestCryptogramOutputTypeDef",
     "VerifyCardValidationDataOutputTypeDef",
     "VerifyMacOutputTypeDef",
     "VerifyPinDataOutputTypeDef",
-    "CardGenerationAttributesTypeDef",
-    "CardVerificationAttributesTypeDef",
-    "CryptogramAuthResponseTypeDef",
     "EncryptionDecryptionAttributesTypeDef",
     "ReEncryptionAttributesTypeDef",
     "GeneratePinDataOutputTypeDef",
     "MacAlgorithmEmvTypeDef",
     "PinGenerationAttributesTypeDef",
     "PinVerificationAttributesTypeDef",
     "SessionKeyDerivationTypeDef",
@@ -199,21 +199,22 @@
 
 class CryptogramVerificationArpcMethod2TypeDef(
     _RequiredCryptogramVerificationArpcMethod2TypeDef,
     _OptionalCryptogramVerificationArpcMethod2TypeDef,
 ):
     pass
 
-DecryptDataOutputTypeDef = TypedDict(
-    "DecryptDataOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "PlainText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DukptAttributesTypeDef = TypedDict(
     "DukptAttributesTypeDef",
     {
         "DukptDerivationType": DukptDerivationTypeType,
@@ -259,24 +260,14 @@
 )
 
 class DukptEncryptionAttributesTypeDef(
     _RequiredDukptEncryptionAttributesTypeDef, _OptionalDukptEncryptionAttributesTypeDef
 ):
     pass
 
-EncryptDataOutputTypeDef = TypedDict(
-    "EncryptDataOutputTypeDef",
-    {
-        "CipherText": str,
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSymmetricEncryptionAttributesTypeDef = TypedDict(
     "_RequiredSymmetricEncryptionAttributesTypeDef",
     {
         "Mode": EncryptionModeType,
     },
 )
 _OptionalSymmetricEncryptionAttributesTypeDef = TypedDict(
@@ -289,34 +280,14 @@
 )
 
 class SymmetricEncryptionAttributesTypeDef(
     _RequiredSymmetricEncryptionAttributesTypeDef, _OptionalSymmetricEncryptionAttributesTypeDef
 ):
     pass
 
-GenerateCardValidationDataOutputTypeDef = TypedDict(
-    "GenerateCardValidationDataOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ValidationData": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GenerateMacOutputTypeDef = TypedDict(
-    "GenerateMacOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "Mac": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PinDataTypeDef = TypedDict(
     "PinDataTypeDef",
     {
         "PinOffset": str,
         "VerificationValue": str,
     },
     total=False,
@@ -418,35 +389,14 @@
     "VisaPinVerificationTypeDef",
     {
         "PinVerificationKeyIndex": int,
         "VerificationValue": str,
     },
 )
 
-ReEncryptDataOutputTypeDef = TypedDict(
-    "ReEncryptDataOutputTypeDef",
-    {
-        "CipherText": str,
-        "KeyArn": str,
-        "KeyCheckValue": str,
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
 SessionKeyAmexTypeDef = TypedDict(
     "SessionKeyAmexTypeDef",
     {
         "PanSequenceNumber": str,
         "PrimaryAccountNumber": str,
     },
 )
@@ -483,70 +433,21 @@
     "SessionKeyVisaTypeDef",
     {
         "PanSequenceNumber": str,
         "PrimaryAccountNumber": str,
     },
 )
 
-TranslatePinDataOutputTypeDef = TypedDict(
-    "TranslatePinDataOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "PinBlock": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TranslationPinDataIsoFormat034TypeDef = TypedDict(
     "TranslationPinDataIsoFormat034TypeDef",
     {
         "PrimaryAccountNumber": str,
     },
 )
 
-VerifyAuthRequestCryptogramOutputTypeDef = TypedDict(
-    "VerifyAuthRequestCryptogramOutputTypeDef",
-    {
-        "AuthResponseValue": str,
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-VerifyCardValidationDataOutputTypeDef = TypedDict(
-    "VerifyCardValidationDataOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-VerifyMacOutputTypeDef = TypedDict(
-    "VerifyMacOutputTypeDef",
-    {
-        "KeyArn": str,
-        "KeyCheckValue": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-VerifyPinDataOutputTypeDef = TypedDict(
-    "VerifyPinDataOutputTypeDef",
-    {
-        "EncryptionKeyArn": str,
-        "EncryptionKeyCheckValue": str,
-        "VerificationKeyArn": str,
-        "VerificationKeyCheckValue": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CardGenerationAttributesTypeDef = TypedDict(
     "CardGenerationAttributesTypeDef",
     {
         "AmexCardSecurityCodeVersion1": AmexCardSecurityCodeVersion1TypeDef,
         "AmexCardSecurityCodeVersion2": AmexCardSecurityCodeVersion2TypeDef,
         "CardHolderVerificationValue": CardHolderVerificationValueTypeDef,
         "CardVerificationValue1": CardVerificationValue1TypeDef,
@@ -577,14 +478,113 @@
     {
         "ArpcMethod1": CryptogramVerificationArpcMethod1TypeDef,
         "ArpcMethod2": CryptogramVerificationArpcMethod2TypeDef,
     },
     total=False,
 )
 
+DecryptDataOutputTypeDef = TypedDict(
+    "DecryptDataOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "PlainText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EncryptDataOutputTypeDef = TypedDict(
+    "EncryptDataOutputTypeDef",
+    {
+        "CipherText": str,
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateCardValidationDataOutputTypeDef = TypedDict(
+    "GenerateCardValidationDataOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ValidationData": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GenerateMacOutputTypeDef = TypedDict(
+    "GenerateMacOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "Mac": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReEncryptDataOutputTypeDef = TypedDict(
+    "ReEncryptDataOutputTypeDef",
+    {
+        "CipherText": str,
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TranslatePinDataOutputTypeDef = TypedDict(
+    "TranslatePinDataOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "PinBlock": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyAuthRequestCryptogramOutputTypeDef = TypedDict(
+    "VerifyAuthRequestCryptogramOutputTypeDef",
+    {
+        "AuthResponseValue": str,
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyCardValidationDataOutputTypeDef = TypedDict(
+    "VerifyCardValidationDataOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyMacOutputTypeDef = TypedDict(
+    "VerifyMacOutputTypeDef",
+    {
+        "KeyArn": str,
+        "KeyCheckValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyPinDataOutputTypeDef = TypedDict(
+    "VerifyPinDataOutputTypeDef",
+    {
+        "EncryptionKeyArn": str,
+        "EncryptionKeyCheckValue": str,
+        "VerificationKeyArn": str,
+        "VerificationKeyCheckValue": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EncryptionDecryptionAttributesTypeDef = TypedDict(
     "EncryptionDecryptionAttributesTypeDef",
     {
         "Asymmetric": AsymmetricEncryptionAttributesTypeDef,
         "Dukpt": DukptEncryptionAttributesTypeDef,
         "Symmetric": SymmetricEncryptionAttributesTypeDef,
     },
@@ -605,15 +605,15 @@
     {
         "EncryptedPinBlock": str,
         "EncryptionKeyArn": str,
         "EncryptionKeyCheckValue": str,
         "GenerationKeyArn": str,
         "GenerationKeyCheckValue": str,
         "PinData": PinDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MacAlgorithmEmvTypeDef = TypedDict(
     "MacAlgorithmEmvTypeDef",
     {
         "MajorKeyDerivationMode": MajorKeyDerivationModeType,
```

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data.egg-info/PKG-INFO` & `mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography-data
-Version: 1.28.0
-Summary: Type annotations for boto3.PaymentCryptographyDataPlane 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PaymentCryptographyDataPlane 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-payment-cryptography-data"></a>
 
 # mypy-boto3-payment-cryptography-data
 
 [![PyPI - mypy-boto3-payment-cryptography-data](https://img.shields.io/pypi/v/mypy-boto3-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-payment-cryptography-data?color=blue)](https://pypistats.org/packages/mypy-boto3-payment-cryptography-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-payment-cryptography-data)](https://pepy.tech/project/mypy-boto3-payment-cryptography-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyDataPlane 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
+[boto3.PaymentCryptographyDataPlane 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#PaymentCryptographyDataPlane)
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
 [mypy-boto3-payment-cryptography-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,49 +316,49 @@
     CardVerificationValue1TypeDef,
     CardVerificationValue2TypeDef,
     DynamicCardVerificationCodeTypeDef,
     DynamicCardVerificationValueTypeDef,
     DiscoverDynamicCardVerificationCodeTypeDef,
     CryptogramVerificationArpcMethod1TypeDef,
     CryptogramVerificationArpcMethod2TypeDef,
-    DecryptDataOutputTypeDef,
+    ResponseMetadataTypeDef,
     DukptAttributesTypeDef,
     DukptDerivationAttributesTypeDef,
     DukptEncryptionAttributesTypeDef,
-    EncryptDataOutputTypeDef,
     SymmetricEncryptionAttributesTypeDef,
-    GenerateCardValidationDataOutputTypeDef,
-    GenerateMacOutputTypeDef,
     PinDataTypeDef,
     Ibm3624NaturalPinTypeDef,
     Ibm3624PinFromOffsetTypeDef,
     Ibm3624PinOffsetTypeDef,
     Ibm3624PinVerificationTypeDef,
     Ibm3624RandomPinTypeDef,
     MacAlgorithmDukptTypeDef,
     SessionKeyDerivationValueTypeDef,
     VisaPinTypeDef,
     VisaPinVerificationValueTypeDef,
     VisaPinVerificationTypeDef,
-    ReEncryptDataOutputTypeDef,
-    ResponseMetadataTypeDef,
     SessionKeyAmexTypeDef,
     SessionKeyEmv2000TypeDef,
     SessionKeyEmvCommonTypeDef,
     SessionKeyMastercardTypeDef,
     SessionKeyVisaTypeDef,
-    TranslatePinDataOutputTypeDef,
     TranslationPinDataIsoFormat034TypeDef,
+    CardGenerationAttributesTypeDef,
+    CardVerificationAttributesTypeDef,
+    CryptogramAuthResponseTypeDef,
+    DecryptDataOutputTypeDef,
+    EncryptDataOutputTypeDef,
+    GenerateCardValidationDataOutputTypeDef,
+    GenerateMacOutputTypeDef,
+    ReEncryptDataOutputTypeDef,
+    TranslatePinDataOutputTypeDef,
     VerifyAuthRequestCryptogramOutputTypeDef,
     VerifyCardValidationDataOutputTypeDef,
     VerifyMacOutputTypeDef,
     VerifyPinDataOutputTypeDef,
-    CardGenerationAttributesTypeDef,
-    CardVerificationAttributesTypeDef,
-    CryptogramAuthResponseTypeDef,
     EncryptionDecryptionAttributesTypeDef,
     ReEncryptionAttributesTypeDef,
     GeneratePinDataOutputTypeDef,
     MacAlgorithmEmvTypeDef,
     PinGenerationAttributesTypeDef,
     PinVerificationAttributesTypeDef,
     SessionKeyDerivationTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/mypy_boto3_payment_cryptography_data.egg-info/SOURCES.txt` & `mypy-boto3-payment-cryptography-data-1.28.12/mypy_boto3_payment_cryptography_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-data-1.28.0/setup.py` & `mypy-boto3-payment-cryptography-data-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-payment-cryptography-data",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_payment_cryptography_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PaymentCryptographyDataPlane 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.PaymentCryptographyDataPlane 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

