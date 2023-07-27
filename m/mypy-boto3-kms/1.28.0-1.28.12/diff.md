# Comparing `tmp/mypy-boto3-kms-1.28.0.tar.gz` & `tmp/mypy-boto3-kms-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kms-1.28.0.tar", last modified: Thu Jul  6 20:59:57 2023, max compression
+gzip compressed data, was "mypy-boto3-kms-1.28.12.tar", last modified: Thu Jul 27 05:34:55 2023, max compression
```

## Comparing `mypy-boto3-kms-1.28.0.tar` & `mypy-boto3-kms-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.238349 mypy-boto3-kms-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-07-06 20:59:57.238349 mypy-boto3-kms-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.230349 mypy-boto3-kms-1.28.0/mypy_boto3_kms/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-07-06 20:45:00.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41185 2023-07-06 20:45:00.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-07-06 20:45:00.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-06 20:45:00.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-06 20:45:00.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-06 20:45:00.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41014 2023-07-06 20:45:02.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40953 2023-07-06 20:45:01.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.238349 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-07-06 20:59:56.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 20:59:57.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:56.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:56.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:56.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:56.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:57.238349 mypy-boto3-kms-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.140462 mypy-boto3-kms-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17835 2023-07-27 05:34:55.128462 mypy-boto3-kms-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.128462 mypy-boto3-kms-1.28.12/mypy_boto3_kms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41185 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-27 05:24:50.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-07-27 05:24:50.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41426 2023-07-27 05:24:50.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41365 2023-07-27 05:24:50.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.128462 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17835 2023-07-27 05:34:54.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:55.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:54.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:54.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:54.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:54.000000 mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:55.140462 mypy-boto3-kms-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:24:49.000000 mypy-boto3-kms-1.28.12/setup.py
```

### Comparing `mypy-boto3-kms-1.28.0/LICENSE` & `mypy-boto3-kms-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.0/PKG-INFO` & `mypy-boto3-kms-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.28.0
-Summary: Type annotations for boto3.KMS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.KMS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-kms"></a>
 
 # mypy-boto3-kms
 
 [![PyPI - mypy-boto3-kms](https://img.shields.io/pypi/v/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kms?color=blue)](https://pypistats.org/packages/mypy-boto3-kms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kms)](https://pepy.tech/project/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [mypy-boto3-kms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,28 +407,30 @@
     GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusRequestRequestTypeDef,
     GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportRequestRequestTypeDef,
     GetParametersForImportResponseTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GetPublicKeyResponseTypeDef,
+    GrantConstraintsOutputTypeDef,
     ImportKeyMaterialRequestRequestTypeDef,
     KeyListEntryTypeDef,
     XksKeyConfigurationTypeTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListAliasesRequestRequestTypeDef,
     ListGrantsRequestListGrantsPaginateTypeDef,
     ListGrantsRequestRequestTypeDef,
     ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     ListKeyPoliciesRequestRequestTypeDef,
     ListKeyPoliciesResponseTypeDef,
     ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
     ListResourceTagsRequestListResourceTagsPaginateTypeDef,
     ListResourceTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     ListRetirableGrantsRequestRequestTypeDef,
     MultiRegionKeyTypeDef,
     PaginatorConfigTypeDef,
     PutKeyPolicyRequestRequestTypeDef,
     ReEncryptRequestRequestTypeDef,
     ReEncryptResponseTypeDef,
@@ -447,28 +449,28 @@
     VerifyMacResponseTypeDef,
     VerifyRequestRequestTypeDef,
     VerifyResponseTypeDef,
     ListAliasesResponseTypeDef,
     CreateCustomKeyStoreRequestRequestTypeDef,
     UpdateCustomKeyStoreRequestRequestTypeDef,
     CreateGrantRequestRequestTypeDef,
-    GrantListEntryTypeDef,
     CreateKeyRequestRequestTypeDef,
-    ListResourceTagsResponseTypeDef,
     ReplicateKeyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomKeyStoresListEntryTypeDef,
     DecryptRequestRequestTypeDef,
     GenerateDataKeyPairRequestRequestTypeDef,
     GenerateDataKeyRequestRequestTypeDef,
     GenerateRandomRequestRequestTypeDef,
+    GrantListEntryTypeDef,
     ListKeysResponseTypeDef,
+    ListResourceTagsResponseTypeDef,
     MultiRegionConfigurationTypeDef,
-    ListGrantsResponseTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
+    ListGrantsResponseTypeDef,
     KeyMetadataTypeDef,
     CreateKeyResponseTypeDef,
     DescribeKeyResponseTypeDef,
     ReplicateKeyResponseTypeDef,
 )
```

### Comparing `mypy-boto3-kms-1.28.0/README.md` & `mypy-boto3-kms-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-kms"></a>
 
 # mypy-boto3-kms
 
 [![PyPI - mypy-boto3-kms](https://img.shields.io/pypi/v/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kms?color=blue)](https://pypistats.org/packages/mypy-boto3-kms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kms)](https://pepy.tech/project/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [mypy-boto3-kms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,28 +375,30 @@
     GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusRequestRequestTypeDef,
     GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportRequestRequestTypeDef,
     GetParametersForImportResponseTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GetPublicKeyResponseTypeDef,
+    GrantConstraintsOutputTypeDef,
     ImportKeyMaterialRequestRequestTypeDef,
     KeyListEntryTypeDef,
     XksKeyConfigurationTypeTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListAliasesRequestRequestTypeDef,
     ListGrantsRequestListGrantsPaginateTypeDef,
     ListGrantsRequestRequestTypeDef,
     ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     ListKeyPoliciesRequestRequestTypeDef,
     ListKeyPoliciesResponseTypeDef,
     ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
     ListResourceTagsRequestListResourceTagsPaginateTypeDef,
     ListResourceTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     ListRetirableGrantsRequestRequestTypeDef,
     MultiRegionKeyTypeDef,
     PaginatorConfigTypeDef,
     PutKeyPolicyRequestRequestTypeDef,
     ReEncryptRequestRequestTypeDef,
     ReEncryptResponseTypeDef,
@@ -415,28 +417,28 @@
     VerifyMacResponseTypeDef,
     VerifyRequestRequestTypeDef,
     VerifyResponseTypeDef,
     ListAliasesResponseTypeDef,
     CreateCustomKeyStoreRequestRequestTypeDef,
     UpdateCustomKeyStoreRequestRequestTypeDef,
     CreateGrantRequestRequestTypeDef,
-    GrantListEntryTypeDef,
     CreateKeyRequestRequestTypeDef,
-    ListResourceTagsResponseTypeDef,
     ReplicateKeyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomKeyStoresListEntryTypeDef,
     DecryptRequestRequestTypeDef,
     GenerateDataKeyPairRequestRequestTypeDef,
     GenerateDataKeyRequestRequestTypeDef,
     GenerateRandomRequestRequestTypeDef,
+    GrantListEntryTypeDef,
     ListKeysResponseTypeDef,
+    ListResourceTagsResponseTypeDef,
     MultiRegionConfigurationTypeDef,
-    ListGrantsResponseTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
+    ListGrantsResponseTypeDef,
     KeyMetadataTypeDef,
     CreateKeyResponseTypeDef,
     DescribeKeyResponseTypeDef,
     ReplicateKeyResponseTypeDef,
 )
```

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms/__init__.py` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms/__init__.pyi` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms/__main__.py` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KMS 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.KMS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS\nOther"
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

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms/client.py` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms/client.pyi` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms/literals.py` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,15 @@
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
@@ -391,26 +392,28 @@
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

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms/literals.pyi` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -303,14 +303,15 @@
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
@@ -389,26 +390,28 @@
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

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms/paginator.py` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms/paginator.pyi` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms/type_defs.py` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasListEntryTypeDef",
     "CancelKeyDeletionRequestRequestTypeDef",
     "CancelKeyDeletionResponseTypeDef",
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "XksProxyAuthenticationCredentialTypeTypeDef",
@@ -92,28 +91,30 @@
     "GetKeyPolicyResponseTypeDef",
     "GetKeyRotationStatusRequestRequestTypeDef",
     "GetKeyRotationStatusResponseTypeDef",
     "GetParametersForImportRequestRequestTypeDef",
     "GetParametersForImportResponseTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GetPublicKeyResponseTypeDef",
+    "GrantConstraintsOutputTypeDef",
     "ImportKeyMaterialRequestRequestTypeDef",
     "KeyListEntryTypeDef",
     "XksKeyConfigurationTypeTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListGrantsRequestListGrantsPaginateTypeDef",
     "ListGrantsRequestRequestTypeDef",
     "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     "ListKeyPoliciesRequestRequestTypeDef",
     "ListKeyPoliciesResponseTypeDef",
     "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
     "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
     "ListResourceTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     "ListRetirableGrantsRequestRequestTypeDef",
     "MultiRegionKeyTypeDef",
     "PaginatorConfigTypeDef",
     "PutKeyPolicyRequestRequestTypeDef",
     "ReEncryptRequestRequestTypeDef",
     "ReEncryptResponseTypeDef",
@@ -132,28 +133,28 @@
     "VerifyMacResponseTypeDef",
     "VerifyRequestRequestTypeDef",
     "VerifyResponseTypeDef",
     "ListAliasesResponseTypeDef",
     "CreateCustomKeyStoreRequestRequestTypeDef",
     "UpdateCustomKeyStoreRequestRequestTypeDef",
     "CreateGrantRequestRequestTypeDef",
-    "GrantListEntryTypeDef",
     "CreateKeyRequestRequestTypeDef",
-    "ListResourceTagsResponseTypeDef",
     "ReplicateKeyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomKeyStoresListEntryTypeDef",
     "DecryptRequestRequestTypeDef",
     "GenerateDataKeyPairRequestRequestTypeDef",
     "GenerateDataKeyRequestRequestTypeDef",
     "GenerateRandomRequestRequestTypeDef",
+    "GrantListEntryTypeDef",
     "ListKeysResponseTypeDef",
+    "ListResourceTagsResponseTypeDef",
     "MultiRegionConfigurationTypeDef",
-    "ListGrantsResponseTypeDef",
     "DescribeCustomKeyStoresResponseTypeDef",
+    "ListGrantsResponseTypeDef",
     "KeyMetadataTypeDef",
     "CreateKeyResponseTypeDef",
     "DescribeKeyResponseTypeDef",
     "ReplicateKeyResponseTypeDef",
 )
 
 AliasListEntryTypeDef = TypedDict(
@@ -324,21 +325,19 @@
     "_OptionalDescribeKeyRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
-
 class DescribeKeyRequestRequestTypeDef(
     _RequiredDescribeKeyRequestRequestTypeDef, _OptionalDescribeKeyRequestRequestTypeDef
 ):
     pass
 
-
 DisableKeyRequestRequestTypeDef = TypedDict(
     "DisableKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -391,21 +390,19 @@
         "GrantTokens": Sequence[str],
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class EncryptRequestRequestTypeDef(
     _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
 ):
     pass
 
-
 EncryptResponseTypeDef = TypedDict(
     "EncryptResponseTypeDef",
     {
         "CiphertextBlob": bytes,
         "KeyId": str,
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -438,22 +435,20 @@
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
-
 GenerateDataKeyPairWithoutPlaintextResponseTypeDef = TypedDict(
     "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
     {
         "PrivateKeyCiphertextBlob": bytes,
         "PublicKey": bytes,
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
@@ -486,22 +481,20 @@
         "NumberOfBytes": int,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
-
 GenerateDataKeyWithoutPlaintextResponseTypeDef = TypedDict(
     "GenerateDataKeyWithoutPlaintextResponseTypeDef",
     {
         "CiphertextBlob": bytes,
         "KeyId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -520,21 +513,19 @@
     {
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class GenerateMacRequestRequestTypeDef(
     _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
 ):
     pass
 
-
 GenerateMacResponseTypeDef = TypedDict(
     "GenerateMacResponseTypeDef",
     {
         "Mac": bytes,
         "MacAlgorithm": MacAlgorithmSpecType,
         "KeyId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -611,35 +602,42 @@
     "_OptionalGetPublicKeyRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
-
 class GetPublicKeyRequestRequestTypeDef(
     _RequiredGetPublicKeyRequestRequestTypeDef, _OptionalGetPublicKeyRequestRequestTypeDef
 ):
     pass
 
-
 GetPublicKeyResponseTypeDef = TypedDict(
     "GetPublicKeyResponseTypeDef",
     {
         "KeyId": str,
         "PublicKey": bytes,
         "CustomerMasterKeySpec": CustomerMasterKeySpecType,
         "KeySpec": KeySpecType,
         "KeyUsage": KeyUsageTypeType,
         "EncryptionAlgorithms": List[EncryptionAlgorithmSpecType],
         "SigningAlgorithms": List[SigningAlgorithmSpecType],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GrantConstraintsOutputTypeDef = TypedDict(
+    "GrantConstraintsOutputTypeDef",
+    {
+        "EncryptionContextSubset": Dict[str, str],
+        "EncryptionContextEquals": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredImportKeyMaterialRequestRequestTypeDef = TypedDict(
     "_RequiredImportKeyMaterialRequestRequestTypeDef",
     {
         "KeyId": str,
         "ImportToken": Union[str, bytes, IO[Any], StreamingBody],
         "EncryptedKeyMaterial": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -649,21 +647,19 @@
     {
         "ValidTo": Union[datetime, str],
         "ExpirationModel": ExpirationModelTypeType,
     },
     total=False,
 )
 
-
 class ImportKeyMaterialRequestRequestTypeDef(
     _RequiredImportKeyMaterialRequestRequestTypeDef, _OptionalImportKeyMaterialRequestRequestTypeDef
 ):
     pass
 
-
 KeyListEntryTypeDef = TypedDict(
     "KeyListEntryTypeDef",
     {
         "KeyId": str,
         "KeyArn": str,
     },
     total=False,
@@ -708,22 +704,20 @@
         "GrantId": str,
         "GranteePrincipal": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListGrantsRequestListGrantsPaginateTypeDef(
     _RequiredListGrantsRequestListGrantsPaginateTypeDef,
     _OptionalListGrantsRequestListGrantsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListGrantsRequestRequestTypeDef = TypedDict(
     "_RequiredListGrantsRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListGrantsRequestRequestTypeDef = TypedDict(
@@ -733,43 +727,39 @@
         "Marker": str,
         "GrantId": str,
         "GranteePrincipal": str,
     },
     total=False,
 )
 
-
 class ListGrantsRequestRequestTypeDef(
     _RequiredListGrantsRequestRequestTypeDef, _OptionalListGrantsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
     "_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
     "_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef(
     _RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     _OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListKeyPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListKeyPoliciesRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListKeyPoliciesRequestRequestTypeDef = TypedDict(
@@ -777,21 +767,19 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListKeyPoliciesRequestRequestTypeDef(
     _RequiredListKeyPoliciesRequestRequestTypeDef, _OptionalListKeyPoliciesRequestRequestTypeDef
 ):
     pass
 
-
 ListKeyPoliciesResponseTypeDef = TypedDict(
     "ListKeyPoliciesResponseTypeDef",
     {
         "PolicyNames": List[str],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -825,22 +813,20 @@
     "_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListResourceTagsRequestListResourceTagsPaginateTypeDef(
     _RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef,
     _OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListResourceTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceTagsRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListResourceTagsRequestRequestTypeDef = TypedDict(
@@ -848,20 +834,26 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListResourceTagsRequestRequestTypeDef(
     _RequiredListResourceTagsRequestRequestTypeDef, _OptionalListResourceTagsRequestRequestTypeDef
 ):
     pass
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "TagKey": str,
+        "TagValue": str,
+    },
+)
 
 _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
     "_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     {
         "RetiringPrincipal": str,
     },
 )
@@ -869,22 +861,20 @@
     "_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
     _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListRetirableGrantsRequestRequestTypeDef = TypedDict(
     "_RequiredListRetirableGrantsRequestRequestTypeDef",
     {
         "RetiringPrincipal": str,
     },
 )
 _OptionalListRetirableGrantsRequestRequestTypeDef = TypedDict(
@@ -892,22 +882,20 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class ListRetirableGrantsRequestRequestTypeDef(
     _RequiredListRetirableGrantsRequestRequestTypeDef,
     _OptionalListRetirableGrantsRequestRequestTypeDef,
 ):
     pass
 
-
 MultiRegionKeyTypeDef = TypedDict(
     "MultiRegionKeyTypeDef",
     {
         "Arn": str,
         "Region": str,
     },
     total=False,
@@ -935,21 +923,19 @@
     "_OptionalPutKeyPolicyRequestRequestTypeDef",
     {
         "BypassPolicyLockoutSafetyCheck": bool,
     },
     total=False,
 )
 
-
 class PutKeyPolicyRequestRequestTypeDef(
     _RequiredPutKeyPolicyRequestRequestTypeDef, _OptionalPutKeyPolicyRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredReEncryptRequestRequestTypeDef = TypedDict(
     "_RequiredReEncryptRequestRequestTypeDef",
     {
         "CiphertextBlob": Union[str, bytes, IO[Any], StreamingBody],
         "DestinationKeyId": str,
     },
 )
@@ -963,21 +949,19 @@
         "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class ReEncryptRequestRequestTypeDef(
     _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
 ):
     pass
 
-
 ReEncryptResponseTypeDef = TypedDict(
     "ReEncryptResponseTypeDef",
     {
         "CiphertextBlob": bytes,
         "SourceKeyId": str,
         "KeyId": str,
         "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
@@ -1019,43 +1003,39 @@
     "_OptionalRevokeGrantRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class RevokeGrantRequestRequestTypeDef(
     _RequiredRevokeGrantRequestRequestTypeDef, _OptionalRevokeGrantRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "_RequiredScheduleKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "_OptionalScheduleKeyDeletionRequestRequestTypeDef",
     {
         "PendingWindowInDays": int,
     },
     total=False,
 )
 
-
 class ScheduleKeyDeletionRequestRequestTypeDef(
     _RequiredScheduleKeyDeletionRequestRequestTypeDef,
     _OptionalScheduleKeyDeletionRequestRequestTypeDef,
 ):
     pass
 
-
 ScheduleKeyDeletionResponseTypeDef = TypedDict(
     "ScheduleKeyDeletionResponseTypeDef",
     {
         "KeyId": str,
         "DeletionDate": datetime,
         "KeyState": KeyStateType,
         "PendingWindowInDays": int,
@@ -1077,21 +1057,19 @@
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class SignRequestRequestTypeDef(
     _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
 ):
     pass
 
-
 SignResponseTypeDef = TypedDict(
     "SignResponseTypeDef",
     {
         "KeyId": str,
         "Signature": bytes,
         "SigningAlgorithm": SigningAlgorithmSpecType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1144,21 +1122,19 @@
     {
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class VerifyMacRequestRequestTypeDef(
     _RequiredVerifyMacRequestRequestTypeDef, _OptionalVerifyMacRequestRequestTypeDef
 ):
     pass
 
-
 VerifyMacResponseTypeDef = TypedDict(
     "VerifyMacResponseTypeDef",
     {
         "KeyId": str,
         "MacValid": bool,
         "MacAlgorithm": MacAlgorithmSpecType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1180,21 +1156,19 @@
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class VerifyRequestRequestTypeDef(
     _RequiredVerifyRequestRequestTypeDef, _OptionalVerifyRequestRequestTypeDef
 ):
     pass
 
-
 VerifyResponseTypeDef = TypedDict(
     "VerifyResponseTypeDef",
     {
         "KeyId": str,
         "SignatureValid": bool,
         "SigningAlgorithm": SigningAlgorithmSpecType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1229,22 +1203,20 @@
         "XksProxyVpcEndpointServiceName": str,
         "XksProxyAuthenticationCredential": XksProxyAuthenticationCredentialTypeTypeDef,
         "XksProxyConnectivity": XksProxyConnectivityTypeType,
     },
     total=False,
 )
 
-
 class CreateCustomKeyStoreRequestRequestTypeDef(
     _RequiredCreateCustomKeyStoreRequestRequestTypeDef,
     _OptionalCreateCustomKeyStoreRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
     },
 )
 _OptionalUpdateCustomKeyStoreRequestRequestTypeDef = TypedDict(
@@ -1258,22 +1230,20 @@
         "XksProxyVpcEndpointServiceName": str,
         "XksProxyAuthenticationCredential": XksProxyAuthenticationCredentialTypeTypeDef,
         "XksProxyConnectivity": XksProxyConnectivityTypeType,
     },
     total=False,
 )
 
-
 class UpdateCustomKeyStoreRequestRequestTypeDef(
     _RequiredUpdateCustomKeyStoreRequestRequestTypeDef,
     _OptionalUpdateCustomKeyStoreRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateGrantRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGrantRequestRequestTypeDef",
     {
         "KeyId": str,
         "GranteePrincipal": str,
         "Operations": Sequence[GrantOperationType],
     },
@@ -1286,37 +1256,19 @@
         "GrantTokens": Sequence[str],
         "Name": str,
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class CreateGrantRequestRequestTypeDef(
     _RequiredCreateGrantRequestRequestTypeDef, _OptionalCreateGrantRequestRequestTypeDef
 ):
     pass
 
-
-GrantListEntryTypeDef = TypedDict(
-    "GrantListEntryTypeDef",
-    {
-        "KeyId": str,
-        "GrantId": str,
-        "Name": str,
-        "CreationDate": datetime,
-        "GranteePrincipal": str,
-        "RetiringPrincipal": str,
-        "IssuingAccount": str,
-        "Operations": List[GrantOperationType],
-        "Constraints": GrantConstraintsTypeDef,
-    },
-    total=False,
-)
-
 CreateKeyRequestRequestTypeDef = TypedDict(
     "CreateKeyRequestRequestTypeDef",
     {
         "Policy": str,
         "Description": str,
         "KeyUsage": KeyUsageTypeType,
         "CustomerMasterKeySpec": CustomerMasterKeySpecType,
@@ -1327,24 +1279,14 @@
         "Tags": Sequence[TagTypeDef],
         "MultiRegion": bool,
         "XksKeyId": str,
     },
     total=False,
 )
 
-ListResourceTagsResponseTypeDef = TypedDict(
-    "ListResourceTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextMarker": str,
-        "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredReplicateKeyRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateKeyRequestRequestTypeDef",
     {
         "KeyId": str,
         "ReplicaRegion": str,
     },
 )
@@ -1355,21 +1297,19 @@
         "BypassPolicyLockoutSafetyCheck": bool,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ReplicateKeyRequestRequestTypeDef(
     _RequiredReplicateKeyRequestRequestTypeDef, _OptionalReplicateKeyRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "KeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1405,21 +1345,19 @@
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "Recipient": RecipientInfoTypeDef,
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class DecryptRequestRequestTypeDef(
     _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyPairRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
     },
 )
@@ -1430,22 +1368,20 @@
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class GenerateDataKeyPairRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGenerateDataKeyRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalGenerateDataKeyRequestRequestTypeDef = TypedDict(
@@ -1457,65 +1393,89 @@
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class GenerateDataKeyRequestRequestTypeDef(
     _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
 ):
     pass
 
-
 GenerateRandomRequestRequestTypeDef = TypedDict(
     "GenerateRandomRequestRequestTypeDef",
     {
         "NumberOfBytes": int,
         "CustomKeyStoreId": str,
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
+GrantListEntryTypeDef = TypedDict(
+    "GrantListEntryTypeDef",
+    {
+        "KeyId": str,
+        "GrantId": str,
+        "Name": str,
+        "CreationDate": datetime,
+        "GranteePrincipal": str,
+        "RetiringPrincipal": str,
+        "IssuingAccount": str,
+        "Operations": List[GrantOperationType],
+        "Constraints": GrantConstraintsOutputTypeDef,
+    },
+    total=False,
+)
+
 ListKeysResponseTypeDef = TypedDict(
     "ListKeysResponseTypeDef",
     {
         "Keys": List[KeyListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListResourceTagsResponseTypeDef = TypedDict(
+    "ListResourceTagsResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextMarker": str,
+        "Truncated": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MultiRegionConfigurationTypeDef = TypedDict(
     "MultiRegionConfigurationTypeDef",
     {
         "MultiRegionKeyType": MultiRegionKeyTypeType,
         "PrimaryKey": MultiRegionKeyTypeDef,
         "ReplicaKeys": List[MultiRegionKeyTypeDef],
     },
     total=False,
 )
 
-ListGrantsResponseTypeDef = TypedDict(
-    "ListGrantsResponseTypeDef",
+DescribeCustomKeyStoresResponseTypeDef = TypedDict(
+    "DescribeCustomKeyStoresResponseTypeDef",
     {
-        "Grants": List[GrantListEntryTypeDef],
+        "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeCustomKeyStoresResponseTypeDef = TypedDict(
-    "DescribeCustomKeyStoresResponseTypeDef",
+ListGrantsResponseTypeDef = TypedDict(
+    "ListGrantsResponseTypeDef",
     {
-        "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
+        "Grants": List[GrantListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredKeyMetadataTypeDef = TypedDict(
@@ -1550,19 +1510,17 @@
         "PendingDeletionWindowInDays": int,
         "MacAlgorithms": List[MacAlgorithmSpecType],
         "XksKeyConfiguration": XksKeyConfigurationTypeTypeDef,
     },
     total=False,
 )
 
-
 class KeyMetadataTypeDef(_RequiredKeyMetadataTypeDef, _OptionalKeyMetadataTypeDef):
     pass
 
-
 CreateKeyResponseTypeDef = TypedDict(
     "CreateKeyResponseTypeDef",
     {
         "KeyMetadata": KeyMetadataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1576,11 +1534,11 @@
 )
 
 ReplicateKeyResponseTypeDef = TypedDict(
     "ReplicateKeyResponseTypeDef",
     {
         "ReplicaKeyMetadata": KeyMetadataTypeDef,
         "ReplicaPolicy": str,
-        "ReplicaTags": List[TagTypeDef],
+        "ReplicaTags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms/type_defs.pyi` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AliasListEntryTypeDef",
     "CancelKeyDeletionRequestRequestTypeDef",
     "CancelKeyDeletionResponseTypeDef",
     "ConnectCustomKeyStoreRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "XksProxyAuthenticationCredentialTypeTypeDef",
@@ -91,28 +92,30 @@
     "GetKeyPolicyResponseTypeDef",
     "GetKeyRotationStatusRequestRequestTypeDef",
     "GetKeyRotationStatusResponseTypeDef",
     "GetParametersForImportRequestRequestTypeDef",
     "GetParametersForImportResponseTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GetPublicKeyResponseTypeDef",
+    "GrantConstraintsOutputTypeDef",
     "ImportKeyMaterialRequestRequestTypeDef",
     "KeyListEntryTypeDef",
     "XksKeyConfigurationTypeTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListGrantsRequestListGrantsPaginateTypeDef",
     "ListGrantsRequestRequestTypeDef",
     "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     "ListKeyPoliciesRequestRequestTypeDef",
     "ListKeyPoliciesResponseTypeDef",
     "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
     "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
     "ListResourceTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     "ListRetirableGrantsRequestRequestTypeDef",
     "MultiRegionKeyTypeDef",
     "PaginatorConfigTypeDef",
     "PutKeyPolicyRequestRequestTypeDef",
     "ReEncryptRequestRequestTypeDef",
     "ReEncryptResponseTypeDef",
@@ -131,28 +134,28 @@
     "VerifyMacResponseTypeDef",
     "VerifyRequestRequestTypeDef",
     "VerifyResponseTypeDef",
     "ListAliasesResponseTypeDef",
     "CreateCustomKeyStoreRequestRequestTypeDef",
     "UpdateCustomKeyStoreRequestRequestTypeDef",
     "CreateGrantRequestRequestTypeDef",
-    "GrantListEntryTypeDef",
     "CreateKeyRequestRequestTypeDef",
-    "ListResourceTagsResponseTypeDef",
     "ReplicateKeyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomKeyStoresListEntryTypeDef",
     "DecryptRequestRequestTypeDef",
     "GenerateDataKeyPairRequestRequestTypeDef",
     "GenerateDataKeyRequestRequestTypeDef",
     "GenerateRandomRequestRequestTypeDef",
+    "GrantListEntryTypeDef",
     "ListKeysResponseTypeDef",
+    "ListResourceTagsResponseTypeDef",
     "MultiRegionConfigurationTypeDef",
-    "ListGrantsResponseTypeDef",
     "DescribeCustomKeyStoresResponseTypeDef",
+    "ListGrantsResponseTypeDef",
     "KeyMetadataTypeDef",
     "CreateKeyResponseTypeDef",
     "DescribeKeyResponseTypeDef",
     "ReplicateKeyResponseTypeDef",
 )
 
 AliasListEntryTypeDef = TypedDict(
@@ -323,19 +326,21 @@
     "_OptionalDescribeKeyRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
+
 class DescribeKeyRequestRequestTypeDef(
     _RequiredDescribeKeyRequestRequestTypeDef, _OptionalDescribeKeyRequestRequestTypeDef
 ):
     pass
 
+
 DisableKeyRequestRequestTypeDef = TypedDict(
     "DisableKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -388,19 +393,21 @@
         "GrantTokens": Sequence[str],
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class EncryptRequestRequestTypeDef(
     _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
 ):
     pass
 
+
 EncryptResponseTypeDef = TypedDict(
     "EncryptResponseTypeDef",
     {
         "CiphertextBlob": bytes,
         "KeyId": str,
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -433,20 +440,22 @@
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
+
 GenerateDataKeyPairWithoutPlaintextResponseTypeDef = TypedDict(
     "GenerateDataKeyPairWithoutPlaintextResponseTypeDef",
     {
         "PrivateKeyCiphertextBlob": bytes,
         "PublicKey": bytes,
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
@@ -479,20 +488,22 @@
         "NumberOfBytes": int,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
 ):
     pass
 
+
 GenerateDataKeyWithoutPlaintextResponseTypeDef = TypedDict(
     "GenerateDataKeyWithoutPlaintextResponseTypeDef",
     {
         "CiphertextBlob": bytes,
         "KeyId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -511,19 +522,21 @@
     {
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class GenerateMacRequestRequestTypeDef(
     _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
 ):
     pass
 
+
 GenerateMacResponseTypeDef = TypedDict(
     "GenerateMacResponseTypeDef",
     {
         "Mac": bytes,
         "MacAlgorithm": MacAlgorithmSpecType,
         "KeyId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -600,33 +613,44 @@
     "_OptionalGetPublicKeyRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
     },
     total=False,
 )
 
+
 class GetPublicKeyRequestRequestTypeDef(
     _RequiredGetPublicKeyRequestRequestTypeDef, _OptionalGetPublicKeyRequestRequestTypeDef
 ):
     pass
 
+
 GetPublicKeyResponseTypeDef = TypedDict(
     "GetPublicKeyResponseTypeDef",
     {
         "KeyId": str,
         "PublicKey": bytes,
         "CustomerMasterKeySpec": CustomerMasterKeySpecType,
         "KeySpec": KeySpecType,
         "KeyUsage": KeyUsageTypeType,
         "EncryptionAlgorithms": List[EncryptionAlgorithmSpecType],
         "SigningAlgorithms": List[SigningAlgorithmSpecType],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GrantConstraintsOutputTypeDef = TypedDict(
+    "GrantConstraintsOutputTypeDef",
+    {
+        "EncryptionContextSubset": Dict[str, str],
+        "EncryptionContextEquals": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredImportKeyMaterialRequestRequestTypeDef = TypedDict(
     "_RequiredImportKeyMaterialRequestRequestTypeDef",
     {
         "KeyId": str,
         "ImportToken": Union[str, bytes, IO[Any], StreamingBody],
         "EncryptedKeyMaterial": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -636,19 +660,21 @@
     {
         "ValidTo": Union[datetime, str],
         "ExpirationModel": ExpirationModelTypeType,
     },
     total=False,
 )
 
+
 class ImportKeyMaterialRequestRequestTypeDef(
     _RequiredImportKeyMaterialRequestRequestTypeDef, _OptionalImportKeyMaterialRequestRequestTypeDef
 ):
     pass
 
+
 KeyListEntryTypeDef = TypedDict(
     "KeyListEntryTypeDef",
     {
         "KeyId": str,
         "KeyArn": str,
     },
     total=False,
@@ -693,20 +719,22 @@
         "GrantId": str,
         "GranteePrincipal": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListGrantsRequestListGrantsPaginateTypeDef(
     _RequiredListGrantsRequestListGrantsPaginateTypeDef,
     _OptionalListGrantsRequestListGrantsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListGrantsRequestRequestTypeDef = TypedDict(
     "_RequiredListGrantsRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListGrantsRequestRequestTypeDef = TypedDict(
@@ -716,39 +744,43 @@
         "Marker": str,
         "GrantId": str,
         "GranteePrincipal": str,
     },
     total=False,
 )
 
+
 class ListGrantsRequestRequestTypeDef(
     _RequiredListGrantsRequestRequestTypeDef, _OptionalListGrantsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
     "_RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
     "_OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef(
     _RequiredListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     _OptionalListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListKeyPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListKeyPoliciesRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListKeyPoliciesRequestRequestTypeDef = TypedDict(
@@ -756,19 +788,21 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListKeyPoliciesRequestRequestTypeDef(
     _RequiredListKeyPoliciesRequestRequestTypeDef, _OptionalListKeyPoliciesRequestRequestTypeDef
 ):
     pass
 
+
 ListKeyPoliciesResponseTypeDef = TypedDict(
     "ListKeyPoliciesResponseTypeDef",
     {
         "PolicyNames": List[str],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -802,20 +836,22 @@
     "_OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListResourceTagsRequestListResourceTagsPaginateTypeDef(
     _RequiredListResourceTagsRequestListResourceTagsPaginateTypeDef,
     _OptionalListResourceTagsRequestListResourceTagsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListResourceTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceTagsRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalListResourceTagsRequestRequestTypeDef = TypedDict(
@@ -823,39 +859,51 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListResourceTagsRequestRequestTypeDef(
     _RequiredListResourceTagsRequestRequestTypeDef, _OptionalListResourceTagsRequestRequestTypeDef
 ):
     pass
 
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "TagKey": str,
+        "TagValue": str,
+    },
+)
+
 _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
     "_RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     {
         "RetiringPrincipal": str,
     },
 )
 _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = TypedDict(
     "_OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
     _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListRetirableGrantsRequestRequestTypeDef = TypedDict(
     "_RequiredListRetirableGrantsRequestRequestTypeDef",
     {
         "RetiringPrincipal": str,
     },
 )
 _OptionalListRetirableGrantsRequestRequestTypeDef = TypedDict(
@@ -863,20 +911,22 @@
     {
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class ListRetirableGrantsRequestRequestTypeDef(
     _RequiredListRetirableGrantsRequestRequestTypeDef,
     _OptionalListRetirableGrantsRequestRequestTypeDef,
 ):
     pass
 
+
 MultiRegionKeyTypeDef = TypedDict(
     "MultiRegionKeyTypeDef",
     {
         "Arn": str,
         "Region": str,
     },
     total=False,
@@ -904,19 +954,21 @@
     "_OptionalPutKeyPolicyRequestRequestTypeDef",
     {
         "BypassPolicyLockoutSafetyCheck": bool,
     },
     total=False,
 )
 
+
 class PutKeyPolicyRequestRequestTypeDef(
     _RequiredPutKeyPolicyRequestRequestTypeDef, _OptionalPutKeyPolicyRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredReEncryptRequestRequestTypeDef = TypedDict(
     "_RequiredReEncryptRequestRequestTypeDef",
     {
         "CiphertextBlob": Union[str, bytes, IO[Any], StreamingBody],
         "DestinationKeyId": str,
     },
 )
@@ -930,19 +982,21 @@
         "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class ReEncryptRequestRequestTypeDef(
     _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
 ):
     pass
 
+
 ReEncryptResponseTypeDef = TypedDict(
     "ReEncryptResponseTypeDef",
     {
         "CiphertextBlob": bytes,
         "SourceKeyId": str,
         "KeyId": str,
         "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
@@ -984,39 +1038,43 @@
     "_OptionalRevokeGrantRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class RevokeGrantRequestRequestTypeDef(
     _RequiredRevokeGrantRequestRequestTypeDef, _OptionalRevokeGrantRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "_RequiredScheduleKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "_OptionalScheduleKeyDeletionRequestRequestTypeDef",
     {
         "PendingWindowInDays": int,
     },
     total=False,
 )
 
+
 class ScheduleKeyDeletionRequestRequestTypeDef(
     _RequiredScheduleKeyDeletionRequestRequestTypeDef,
     _OptionalScheduleKeyDeletionRequestRequestTypeDef,
 ):
     pass
 
+
 ScheduleKeyDeletionResponseTypeDef = TypedDict(
     "ScheduleKeyDeletionResponseTypeDef",
     {
         "KeyId": str,
         "DeletionDate": datetime,
         "KeyState": KeyStateType,
         "PendingWindowInDays": int,
@@ -1038,19 +1096,21 @@
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class SignRequestRequestTypeDef(
     _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
 ):
     pass
 
+
 SignResponseTypeDef = TypedDict(
     "SignResponseTypeDef",
     {
         "KeyId": str,
         "Signature": bytes,
         "SigningAlgorithm": SigningAlgorithmSpecType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1103,19 +1163,21 @@
     {
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class VerifyMacRequestRequestTypeDef(
     _RequiredVerifyMacRequestRequestTypeDef, _OptionalVerifyMacRequestRequestTypeDef
 ):
     pass
 
+
 VerifyMacResponseTypeDef = TypedDict(
     "VerifyMacResponseTypeDef",
     {
         "KeyId": str,
         "MacValid": bool,
         "MacAlgorithm": MacAlgorithmSpecType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1137,19 +1199,21 @@
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class VerifyRequestRequestTypeDef(
     _RequiredVerifyRequestRequestTypeDef, _OptionalVerifyRequestRequestTypeDef
 ):
     pass
 
+
 VerifyResponseTypeDef = TypedDict(
     "VerifyResponseTypeDef",
     {
         "KeyId": str,
         "SignatureValid": bool,
         "SigningAlgorithm": SigningAlgorithmSpecType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1184,20 +1248,22 @@
         "XksProxyVpcEndpointServiceName": str,
         "XksProxyAuthenticationCredential": XksProxyAuthenticationCredentialTypeTypeDef,
         "XksProxyConnectivity": XksProxyConnectivityTypeType,
     },
     total=False,
 )
 
+
 class CreateCustomKeyStoreRequestRequestTypeDef(
     _RequiredCreateCustomKeyStoreRequestRequestTypeDef,
     _OptionalCreateCustomKeyStoreRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateCustomKeyStoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCustomKeyStoreRequestRequestTypeDef",
     {
         "CustomKeyStoreId": str,
     },
 )
 _OptionalUpdateCustomKeyStoreRequestRequestTypeDef = TypedDict(
@@ -1211,20 +1277,22 @@
         "XksProxyVpcEndpointServiceName": str,
         "XksProxyAuthenticationCredential": XksProxyAuthenticationCredentialTypeTypeDef,
         "XksProxyConnectivity": XksProxyConnectivityTypeType,
     },
     total=False,
 )
 
+
 class UpdateCustomKeyStoreRequestRequestTypeDef(
     _RequiredUpdateCustomKeyStoreRequestRequestTypeDef,
     _OptionalUpdateCustomKeyStoreRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateGrantRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGrantRequestRequestTypeDef",
     {
         "KeyId": str,
         "GranteePrincipal": str,
         "Operations": Sequence[GrantOperationType],
     },
@@ -1237,34 +1305,20 @@
         "GrantTokens": Sequence[str],
         "Name": str,
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class CreateGrantRequestRequestTypeDef(
     _RequiredCreateGrantRequestRequestTypeDef, _OptionalCreateGrantRequestRequestTypeDef
 ):
     pass
 
-GrantListEntryTypeDef = TypedDict(
-    "GrantListEntryTypeDef",
-    {
-        "KeyId": str,
-        "GrantId": str,
-        "Name": str,
-        "CreationDate": datetime,
-        "GranteePrincipal": str,
-        "RetiringPrincipal": str,
-        "IssuingAccount": str,
-        "Operations": List[GrantOperationType],
-        "Constraints": GrantConstraintsTypeDef,
-    },
-    total=False,
-)
 
 CreateKeyRequestRequestTypeDef = TypedDict(
     "CreateKeyRequestRequestTypeDef",
     {
         "Policy": str,
         "Description": str,
         "KeyUsage": KeyUsageTypeType,
@@ -1276,24 +1330,14 @@
         "Tags": Sequence[TagTypeDef],
         "MultiRegion": bool,
         "XksKeyId": str,
     },
     total=False,
 )
 
-ListResourceTagsResponseTypeDef = TypedDict(
-    "ListResourceTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextMarker": str,
-        "Truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredReplicateKeyRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateKeyRequestRequestTypeDef",
     {
         "KeyId": str,
         "ReplicaRegion": str,
     },
 )
@@ -1304,19 +1348,21 @@
         "BypassPolicyLockoutSafetyCheck": bool,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ReplicateKeyRequestRequestTypeDef(
     _RequiredReplicateKeyRequestRequestTypeDef, _OptionalReplicateKeyRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "KeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1352,19 +1398,21 @@
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "Recipient": RecipientInfoTypeDef,
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class DecryptRequestRequestTypeDef(
     _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyPairRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
     },
 )
@@ -1375,20 +1423,22 @@
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class GenerateDataKeyPairRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGenerateDataKeyRequestRequestTypeDef = TypedDict(
     "_RequiredGenerateDataKeyRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
 _OptionalGenerateDataKeyRequestRequestTypeDef = TypedDict(
@@ -1400,63 +1450,91 @@
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class GenerateDataKeyRequestRequestTypeDef(
     _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
 ):
     pass
 
+
 GenerateRandomRequestRequestTypeDef = TypedDict(
     "GenerateRandomRequestRequestTypeDef",
     {
         "NumberOfBytes": int,
         "CustomKeyStoreId": str,
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
+GrantListEntryTypeDef = TypedDict(
+    "GrantListEntryTypeDef",
+    {
+        "KeyId": str,
+        "GrantId": str,
+        "Name": str,
+        "CreationDate": datetime,
+        "GranteePrincipal": str,
+        "RetiringPrincipal": str,
+        "IssuingAccount": str,
+        "Operations": List[GrantOperationType],
+        "Constraints": GrantConstraintsOutputTypeDef,
+    },
+    total=False,
+)
+
 ListKeysResponseTypeDef = TypedDict(
     "ListKeysResponseTypeDef",
     {
         "Keys": List[KeyListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListResourceTagsResponseTypeDef = TypedDict(
+    "ListResourceTagsResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextMarker": str,
+        "Truncated": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MultiRegionConfigurationTypeDef = TypedDict(
     "MultiRegionConfigurationTypeDef",
     {
         "MultiRegionKeyType": MultiRegionKeyTypeType,
         "PrimaryKey": MultiRegionKeyTypeDef,
         "ReplicaKeys": List[MultiRegionKeyTypeDef],
     },
     total=False,
 )
 
-ListGrantsResponseTypeDef = TypedDict(
-    "ListGrantsResponseTypeDef",
+DescribeCustomKeyStoresResponseTypeDef = TypedDict(
+    "DescribeCustomKeyStoresResponseTypeDef",
     {
-        "Grants": List[GrantListEntryTypeDef],
+        "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeCustomKeyStoresResponseTypeDef = TypedDict(
-    "DescribeCustomKeyStoresResponseTypeDef",
+ListGrantsResponseTypeDef = TypedDict(
+    "ListGrantsResponseTypeDef",
     {
-        "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
+        "Grants": List[GrantListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredKeyMetadataTypeDef = TypedDict(
@@ -1491,17 +1569,19 @@
         "PendingDeletionWindowInDays": int,
         "MacAlgorithms": List[MacAlgorithmSpecType],
         "XksKeyConfiguration": XksKeyConfigurationTypeTypeDef,
     },
     total=False,
 )
 
+
 class KeyMetadataTypeDef(_RequiredKeyMetadataTypeDef, _OptionalKeyMetadataTypeDef):
     pass
 
+
 CreateKeyResponseTypeDef = TypedDict(
     "CreateKeyResponseTypeDef",
     {
         "KeyMetadata": KeyMetadataTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1515,11 +1595,11 @@
 )
 
 ReplicateKeyResponseTypeDef = TypedDict(
     "ReplicateKeyResponseTypeDef",
     {
         "ReplicaKeyMetadata": KeyMetadataTypeDef,
         "ReplicaPolicy": str,
-        "ReplicaTags": List[TagTypeDef],
+        "ReplicaTags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/PKG-INFO` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.28.0
-Summary: Type annotations for boto3.KMS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.KMS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-kms"></a>
 
 # mypy-boto3-kms
 
 [![PyPI - mypy-boto3-kms](https://img.shields.io/pypi/v/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kms?color=blue)](https://pypistats.org/packages/mypy-boto3-kms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kms)](https://pepy.tech/project/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
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
 [mypy-boto3-kms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,28 +407,30 @@
     GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusRequestRequestTypeDef,
     GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportRequestRequestTypeDef,
     GetParametersForImportResponseTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GetPublicKeyResponseTypeDef,
+    GrantConstraintsOutputTypeDef,
     ImportKeyMaterialRequestRequestTypeDef,
     KeyListEntryTypeDef,
     XksKeyConfigurationTypeTypeDef,
     ListAliasesRequestListAliasesPaginateTypeDef,
     ListAliasesRequestRequestTypeDef,
     ListGrantsRequestListGrantsPaginateTypeDef,
     ListGrantsRequestRequestTypeDef,
     ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef,
     ListKeyPoliciesRequestRequestTypeDef,
     ListKeyPoliciesResponseTypeDef,
     ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
     ListResourceTagsRequestListResourceTagsPaginateTypeDef,
     ListResourceTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     ListRetirableGrantsRequestRequestTypeDef,
     MultiRegionKeyTypeDef,
     PaginatorConfigTypeDef,
     PutKeyPolicyRequestRequestTypeDef,
     ReEncryptRequestRequestTypeDef,
     ReEncryptResponseTypeDef,
@@ -447,28 +449,28 @@
     VerifyMacResponseTypeDef,
     VerifyRequestRequestTypeDef,
     VerifyResponseTypeDef,
     ListAliasesResponseTypeDef,
     CreateCustomKeyStoreRequestRequestTypeDef,
     UpdateCustomKeyStoreRequestRequestTypeDef,
     CreateGrantRequestRequestTypeDef,
-    GrantListEntryTypeDef,
     CreateKeyRequestRequestTypeDef,
-    ListResourceTagsResponseTypeDef,
     ReplicateKeyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomKeyStoresListEntryTypeDef,
     DecryptRequestRequestTypeDef,
     GenerateDataKeyPairRequestRequestTypeDef,
     GenerateDataKeyRequestRequestTypeDef,
     GenerateRandomRequestRequestTypeDef,
+    GrantListEntryTypeDef,
     ListKeysResponseTypeDef,
+    ListResourceTagsResponseTypeDef,
     MultiRegionConfigurationTypeDef,
-    ListGrantsResponseTypeDef,
     DescribeCustomKeyStoresResponseTypeDef,
+    ListGrantsResponseTypeDef,
     KeyMetadataTypeDef,
     CreateKeyResponseTypeDef,
     DescribeKeyResponseTypeDef,
     ReplicateKeyResponseTypeDef,
 )
```

### Comparing `mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/SOURCES.txt` & `mypy-boto3-kms-1.28.12/mypy_boto3_kms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.28.0/setup.py` & `mypy-boto3-kms-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kms",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_kms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KMS 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.KMS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

