# Comparing `tmp/mypy-boto3-glacier-1.28.0.tar.gz` & `tmp/mypy-boto3-glacier-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-glacier-1.28.0.tar", last modified: Thu Jul  6 20:59:38 2023, max compression
+gzip compressed data, was "mypy-boto3-glacier-1.28.12.tar", last modified: Thu Jul 27 05:34:44 2023, max compression
```

## Comparing `mypy-boto3-glacier-1.28.0.tar` & `mypy-boto3-glacier-1.28.12.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:38.658310 mypy-boto3-glacier-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:41:45.000000 mypy-boto3-glacier-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-07-06 20:59:38.646310 mypy-boto3-glacier-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-06 20:41:45.000000 mypy-boto3-glacier-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:38.646310 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-06 20:41:45.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-06 20:41:45.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:41:45.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26623 2023-07-06 20:41:45.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26577 2023-07-06 20:41:45.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-06 20:41:46.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-07-06 20:41:46.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-06 20:41:46.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-06 20:41:46.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:41:45.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39259 2023-07-06 20:41:46.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    39151 2023-07-06 20:41:46.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    38670 2023-07-06 20:41:47.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38598 2023-07-06 20:41:47.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:41:45.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-06 20:41:46.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-06 20:41:46.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:38.646310 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-07-06 20:59:38.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-06 20:59:38.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:38.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:38.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:38.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:59:38.000000 mypy-boto3-glacier-1.28.0/mypy_boto3_glacier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:38.658310 mypy-boto3-glacier-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:41:45.000000 mypy-boto3-glacier-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.140501 mypy-boto3-glacier-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20198 2023-07-27 05:34:44.140501 mypy-boto3-glacier-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.136501 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26611 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26565 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39259 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39151 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42119 2023-07-27 05:22:45.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42045 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-27 05:22:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.140501 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20198 2023-07-27 05:34:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 05:34:44.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:43.000000 mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:44.140501 mypy-boto3-glacier-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:22:43.000000 mypy-boto3-glacier-1.28.12/setup.py
```

### Comparing `mypy-boto3-glacier-1.28.0/LICENSE` & `mypy-boto3-glacier-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.0/PKG-INFO` & `mypy-boto3-glacier-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glacier
-Version: 1.28.0
-Summary: Type annotations for boto3.Glacier 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Glacier 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-glacier"></a>
 
 # mypy-boto3-glacier
 
 [![PyPI - mypy-boto3-glacier](https://img.shields.io/pypi/v/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glacier?color=blue)](https://pypistats.org/packages/mypy-boto3-glacier)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glacier)](https://pepy.tech/project/mypy-boto3-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glacier 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[boto3.Glacier 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
 
@@ -440,46 +440,50 @@
 
 ```python
 from mypy_boto3_glacier.type_defs import (
     AbortMultipartUploadInputRequestTypeDef,
     AbortVaultLockInputRequestTypeDef,
     AddTagsToVaultInputRequestTypeDef,
     ArchiveCreationOutputTypeDef,
+    CSVInputOutputTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
     CompleteMultipartUploadInputMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadInputRequestTypeDef,
     CompleteVaultLockInputRequestTypeDef,
     CreateVaultInputAccountCreateVaultTypeDef,
     CreateVaultInputRequestTypeDef,
     CreateVaultInputServiceResourceCreateVaultTypeDef,
     CreateVaultOutputTypeDef,
+    DataRetrievalRuleOutputTypeDef,
     DataRetrievalRuleTypeDef,
     DeleteArchiveInputRequestTypeDef,
     DeleteVaultAccessPolicyInputRequestTypeDef,
     DeleteVaultInputRequestTypeDef,
     DeleteVaultNotificationsInputRequestTypeDef,
     DescribeJobInputRequestTypeDef,
     DescribeVaultInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeVaultOutputResponseMetadataTypeDef,
     DescribeVaultOutputTypeDef,
+    DescribeVaultResponseMetadataTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionOutputTypeDef,
     EncryptionTypeDef,
     GetDataRetrievalPolicyInputRequestTypeDef,
     GetJobOutputInputJobGetOutputTypeDef,
     GetJobOutputInputRequestTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyInputRequestTypeDef,
-    VaultAccessPolicyTypeDef,
+    VaultAccessPolicyOutputTypeDef,
     GetVaultLockInputRequestTypeDef,
     GetVaultLockOutputTypeDef,
     GetVaultNotificationsInputRequestTypeDef,
-    VaultNotificationConfigTypeDef,
+    VaultNotificationConfigOutputTypeDef,
     InventoryRetrievalJobDescriptionTypeDef,
+    GranteeOutputTypeDef,
     GranteeTypeDef,
     InitiateJobOutputTypeDef,
     InitiateMultipartUploadInputRequestTypeDef,
     InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef,
     InitiateMultipartUploadOutputTypeDef,
     VaultLockPolicyTypeDef,
     InitiateVaultLockOutputTypeDef,
@@ -501,40 +505,49 @@
     ListVaultsInputListVaultsPaginateTypeDef,
     ListVaultsInputRequestTypeDef,
     PaginatorConfigTypeDef,
     PurchaseProvisionedCapacityInputRequestTypeDef,
     PurchaseProvisionedCapacityOutputTypeDef,
     RemoveTagsFromVaultInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    VaultAccessPolicyTypeDef,
+    VaultNotificationConfigTypeDef,
     UploadArchiveInputRequestTypeDef,
     UploadArchiveInputVaultUploadArchiveTypeDef,
     UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
     UploadMultipartPartInputRequestTypeDef,
     UploadMultipartPartOutputTypeDef,
+    InputSerializationOutputTypeDef,
     InputSerializationTypeDef,
+    OutputSerializationOutputTypeDef,
     OutputSerializationTypeDef,
+    DataRetrievalPolicyOutputTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultInputVaultExistsWaitTypeDef,
     DescribeVaultInputVaultNotExistsWaitTypeDef,
     ListVaultsOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
-    SetVaultAccessPolicyInputRequestTypeDef,
     GetVaultNotificationsOutputTypeDef,
-    SetVaultNotificationsInputNotificationSetTypeDef,
-    SetVaultNotificationsInputRequestTypeDef,
+    GrantOutputTypeDef,
     GrantTypeDef,
     InitiateVaultLockInputRequestTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
     ListProvisionedCapacityOutputTypeDef,
+    SetVaultAccessPolicyInputRequestTypeDef,
+    SetVaultNotificationsInputNotificationSetTypeDef,
+    SetVaultNotificationsInputRequestTypeDef,
+    SelectParametersOutputTypeDef,
     SelectParametersResponseMetadataTypeDef,
     SelectParametersTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     SetDataRetrievalPolicyInputRequestTypeDef,
+    S3LocationOutputTypeDef,
     S3LocationTypeDef,
+    OutputLocationOutputTypeDef,
     OutputLocationResponseMetadataTypeDef,
     OutputLocationTypeDef,
     GlacierJobDescriptionResponseMetadataTypeDef,
     GlacierJobDescriptionTypeDef,
     JobParametersTypeDef,
     ListJobsOutputTypeDef,
     InitiateJobInputRequestTypeDef,
```

### Comparing `mypy-boto3-glacier-1.28.0/README.md` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-glacier
+Version: 1.28.12
+Summary: Type annotations for boto3.Glacier 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 glacier type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-glacier"></a>
 
 # mypy-boto3-glacier
 
 [![PyPI - mypy-boto3-glacier](https://img.shields.io/pypi/v/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glacier?color=blue)](https://pypistats.org/packages/mypy-boto3-glacier)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glacier)](https://pepy.tech/project/mypy-boto3-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glacier 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[boto3.Glacier 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,46 +440,50 @@
 
 ```python
 from mypy_boto3_glacier.type_defs import (
     AbortMultipartUploadInputRequestTypeDef,
     AbortVaultLockInputRequestTypeDef,
     AddTagsToVaultInputRequestTypeDef,
     ArchiveCreationOutputTypeDef,
+    CSVInputOutputTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
     CompleteMultipartUploadInputMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadInputRequestTypeDef,
     CompleteVaultLockInputRequestTypeDef,
     CreateVaultInputAccountCreateVaultTypeDef,
     CreateVaultInputRequestTypeDef,
     CreateVaultInputServiceResourceCreateVaultTypeDef,
     CreateVaultOutputTypeDef,
+    DataRetrievalRuleOutputTypeDef,
     DataRetrievalRuleTypeDef,
     DeleteArchiveInputRequestTypeDef,
     DeleteVaultAccessPolicyInputRequestTypeDef,
     DeleteVaultInputRequestTypeDef,
     DeleteVaultNotificationsInputRequestTypeDef,
     DescribeJobInputRequestTypeDef,
     DescribeVaultInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeVaultOutputResponseMetadataTypeDef,
     DescribeVaultOutputTypeDef,
+    DescribeVaultResponseMetadataTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionOutputTypeDef,
     EncryptionTypeDef,
     GetDataRetrievalPolicyInputRequestTypeDef,
     GetJobOutputInputJobGetOutputTypeDef,
     GetJobOutputInputRequestTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyInputRequestTypeDef,
-    VaultAccessPolicyTypeDef,
+    VaultAccessPolicyOutputTypeDef,
     GetVaultLockInputRequestTypeDef,
     GetVaultLockOutputTypeDef,
     GetVaultNotificationsInputRequestTypeDef,
-    VaultNotificationConfigTypeDef,
+    VaultNotificationConfigOutputTypeDef,
     InventoryRetrievalJobDescriptionTypeDef,
+    GranteeOutputTypeDef,
     GranteeTypeDef,
     InitiateJobOutputTypeDef,
     InitiateMultipartUploadInputRequestTypeDef,
     InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef,
     InitiateMultipartUploadOutputTypeDef,
     VaultLockPolicyTypeDef,
     InitiateVaultLockOutputTypeDef,
@@ -469,40 +505,49 @@
     ListVaultsInputListVaultsPaginateTypeDef,
     ListVaultsInputRequestTypeDef,
     PaginatorConfigTypeDef,
     PurchaseProvisionedCapacityInputRequestTypeDef,
     PurchaseProvisionedCapacityOutputTypeDef,
     RemoveTagsFromVaultInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    VaultAccessPolicyTypeDef,
+    VaultNotificationConfigTypeDef,
     UploadArchiveInputRequestTypeDef,
     UploadArchiveInputVaultUploadArchiveTypeDef,
     UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
     UploadMultipartPartInputRequestTypeDef,
     UploadMultipartPartOutputTypeDef,
+    InputSerializationOutputTypeDef,
     InputSerializationTypeDef,
+    OutputSerializationOutputTypeDef,
     OutputSerializationTypeDef,
+    DataRetrievalPolicyOutputTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultInputVaultExistsWaitTypeDef,
     DescribeVaultInputVaultNotExistsWaitTypeDef,
     ListVaultsOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
-    SetVaultAccessPolicyInputRequestTypeDef,
     GetVaultNotificationsOutputTypeDef,
-    SetVaultNotificationsInputNotificationSetTypeDef,
-    SetVaultNotificationsInputRequestTypeDef,
+    GrantOutputTypeDef,
     GrantTypeDef,
     InitiateVaultLockInputRequestTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
     ListProvisionedCapacityOutputTypeDef,
+    SetVaultAccessPolicyInputRequestTypeDef,
+    SetVaultNotificationsInputNotificationSetTypeDef,
+    SetVaultNotificationsInputRequestTypeDef,
+    SelectParametersOutputTypeDef,
     SelectParametersResponseMetadataTypeDef,
     SelectParametersTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     SetDataRetrievalPolicyInputRequestTypeDef,
+    S3LocationOutputTypeDef,
     S3LocationTypeDef,
+    OutputLocationOutputTypeDef,
     OutputLocationResponseMetadataTypeDef,
     OutputLocationTypeDef,
     GlacierJobDescriptionResponseMetadataTypeDef,
     GlacierJobDescriptionTypeDef,
     JobParametersTypeDef,
     ListJobsOutputTypeDef,
     InitiateJobInputRequestTypeDef,
```

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/__init__.py` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/__init__.pyi` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/__main__.py` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Glacier 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Glacier 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier\nOther"
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

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/client.py` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     ListPartsPaginator,
     ListVaultsPaginator,
 )
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
     CreateVaultOutputTypeDef,
     DataRetrievalPolicyTypeDef,
-    DescribeVaultOutputResponseMetadataTypeDef,
+    DescribeVaultResponseMetadataTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     GetVaultLockOutputTypeDef,
     GetVaultNotificationsOutputTypeDef,
     GlacierJobDescriptionResponseMetadataTypeDef,
@@ -235,15 +235,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.describe_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#describe_job)
         """
 
     def describe_vault(
         self, *, vaultName: str, accountId: str = "-"
-    ) -> DescribeVaultOutputResponseMetadataTypeDef:
+    ) -> DescribeVaultResponseMetadataTypeDef:
         """
         This operation returns information about a vault, including the vault's Amazon
         Resource Name (ARN), the date the vault was created, the number of archives it
         contains, and the total size of all the archives in the vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.describe_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#describe_vault)
```

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/client.pyi` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     ListPartsPaginator,
     ListVaultsPaginator,
 )
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
     CreateVaultOutputTypeDef,
     DataRetrievalPolicyTypeDef,
-    DescribeVaultOutputResponseMetadataTypeDef,
+    DescribeVaultResponseMetadataTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     GetVaultLockOutputTypeDef,
     GetVaultNotificationsOutputTypeDef,
     GlacierJobDescriptionResponseMetadataTypeDef,
@@ -217,15 +217,15 @@
         (Glacier) completes the job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.describe_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#describe_job)
         """
     def describe_vault(
         self, *, vaultName: str, accountId: str = "-"
-    ) -> DescribeVaultOutputResponseMetadataTypeDef:
+    ) -> DescribeVaultResponseMetadataTypeDef:
         """
         This operation returns information about a vault, including the vault's Amazon
         Resource Name (ARN), the date the vault was created, the number of archives it
         contains, and the total size of all the archives in the vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.describe_vault)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/client/#describe_vault)
```

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/literals.py` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/literals.pyi`

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
     "ActionCodeType",
     "CannedACLType",
     "EncryptionTypeType",
     "ExpressionTypeType",
     "FileHeaderInfoType",
     "ListJobsPaginatorName",
@@ -40,15 +39,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActionCodeType = Literal["ArchiveRetrieval", "InventoryRetrieval", "Select"]
 CannedACLType = Literal[
     "authenticated-read",
     "aws-exec-read",
     "bucket-owner-full-control",
     "bucket-owner-read",
     "private",
@@ -185,14 +183,15 @@
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
@@ -271,26 +270,28 @@
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

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/literals.pyi` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActionCodeType",
     "CannedACLType",
     "EncryptionTypeType",
     "ExpressionTypeType",
     "FileHeaderInfoType",
     "ListJobsPaginatorName",
@@ -39,14 +40,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 ActionCodeType = Literal["ArchiveRetrieval", "InventoryRetrieval", "Select"]
 CannedACLType = Literal[
     "authenticated-read",
     "aws-exec-read",
     "bucket-owner-full-control",
     "bucket-owner-read",
     "private",
@@ -183,14 +185,15 @@
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
@@ -269,26 +272,28 @@
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

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/paginator.py` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/paginator.pyi` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/service_resource.py` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/service_resource.pyi` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/type_defs.py` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -33,52 +33,55 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbortMultipartUploadInputRequestTypeDef",
     "AbortVaultLockInputRequestTypeDef",
     "AddTagsToVaultInputRequestTypeDef",
     "ArchiveCreationOutputTypeDef",
+    "CSVInputOutputTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
     "CompleteMultipartUploadInputMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadInputRequestTypeDef",
     "CompleteVaultLockInputRequestTypeDef",
     "CreateVaultInputAccountCreateVaultTypeDef",
     "CreateVaultInputRequestTypeDef",
     "CreateVaultInputServiceResourceCreateVaultTypeDef",
     "CreateVaultOutputTypeDef",
+    "DataRetrievalRuleOutputTypeDef",
     "DataRetrievalRuleTypeDef",
     "DeleteArchiveInputRequestTypeDef",
     "DeleteVaultAccessPolicyInputRequestTypeDef",
     "DeleteVaultInputRequestTypeDef",
     "DeleteVaultNotificationsInputRequestTypeDef",
     "DescribeJobInputRequestTypeDef",
     "DescribeVaultInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeVaultOutputResponseMetadataTypeDef",
     "DescribeVaultOutputTypeDef",
+    "DescribeVaultResponseMetadataTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
     "GetDataRetrievalPolicyInputRequestTypeDef",
     "GetJobOutputInputJobGetOutputTypeDef",
     "GetJobOutputInputRequestTypeDef",
     "GetJobOutputOutputTypeDef",
     "GetVaultAccessPolicyInputRequestTypeDef",
-    "VaultAccessPolicyTypeDef",
+    "VaultAccessPolicyOutputTypeDef",
     "GetVaultLockInputRequestTypeDef",
     "GetVaultLockOutputTypeDef",
     "GetVaultNotificationsInputRequestTypeDef",
-    "VaultNotificationConfigTypeDef",
+    "VaultNotificationConfigOutputTypeDef",
     "InventoryRetrievalJobDescriptionTypeDef",
+    "GranteeOutputTypeDef",
     "GranteeTypeDef",
     "InitiateJobOutputTypeDef",
     "InitiateMultipartUploadInputRequestTypeDef",
     "InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef",
     "InitiateMultipartUploadOutputTypeDef",
     "VaultLockPolicyTypeDef",
     "InitiateVaultLockOutputTypeDef",
@@ -100,40 +103,49 @@
     "ListVaultsInputListVaultsPaginateTypeDef",
     "ListVaultsInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "PurchaseProvisionedCapacityInputRequestTypeDef",
     "PurchaseProvisionedCapacityOutputTypeDef",
     "RemoveTagsFromVaultInputRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "VaultAccessPolicyTypeDef",
+    "VaultNotificationConfigTypeDef",
     "UploadArchiveInputRequestTypeDef",
     "UploadArchiveInputVaultUploadArchiveTypeDef",
     "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
     "UploadMultipartPartInputRequestTypeDef",
     "UploadMultipartPartOutputTypeDef",
+    "InputSerializationOutputTypeDef",
     "InputSerializationTypeDef",
+    "OutputSerializationOutputTypeDef",
     "OutputSerializationTypeDef",
+    "DataRetrievalPolicyOutputTypeDef",
     "DataRetrievalPolicyTypeDef",
     "DescribeVaultInputVaultExistsWaitTypeDef",
     "DescribeVaultInputVaultNotExistsWaitTypeDef",
     "ListVaultsOutputTypeDef",
     "GetVaultAccessPolicyOutputTypeDef",
-    "SetVaultAccessPolicyInputRequestTypeDef",
     "GetVaultNotificationsOutputTypeDef",
-    "SetVaultNotificationsInputNotificationSetTypeDef",
-    "SetVaultNotificationsInputRequestTypeDef",
+    "GrantOutputTypeDef",
     "GrantTypeDef",
     "InitiateVaultLockInputRequestTypeDef",
     "ListMultipartUploadsOutputTypeDef",
     "ListPartsOutputTypeDef",
     "ListProvisionedCapacityOutputTypeDef",
+    "SetVaultAccessPolicyInputRequestTypeDef",
+    "SetVaultNotificationsInputNotificationSetTypeDef",
+    "SetVaultNotificationsInputRequestTypeDef",
+    "SelectParametersOutputTypeDef",
     "SelectParametersResponseMetadataTypeDef",
     "SelectParametersTypeDef",
     "GetDataRetrievalPolicyOutputTypeDef",
     "SetDataRetrievalPolicyInputRequestTypeDef",
+    "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
+    "OutputLocationOutputTypeDef",
     "OutputLocationResponseMetadataTypeDef",
     "OutputLocationTypeDef",
     "GlacierJobDescriptionResponseMetadataTypeDef",
     "GlacierJobDescriptionTypeDef",
     "JobParametersTypeDef",
     "ListJobsOutputTypeDef",
     "InitiateJobInputRequestTypeDef",
@@ -150,43 +162,39 @@
     "_OptionalAbortMultipartUploadInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class AbortMultipartUploadInputRequestTypeDef(
     _RequiredAbortMultipartUploadInputRequestTypeDef,
     _OptionalAbortMultipartUploadInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredAbortVaultLockInputRequestTypeDef = TypedDict(
     "_RequiredAbortVaultLockInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalAbortVaultLockInputRequestTypeDef = TypedDict(
     "_OptionalAbortVaultLockInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class AbortVaultLockInputRequestTypeDef(
     _RequiredAbortVaultLockInputRequestTypeDef, _OptionalAbortVaultLockInputRequestTypeDef
 ):
     pass
 
-
 _RequiredAddTagsToVaultInputRequestTypeDef = TypedDict(
     "_RequiredAddTagsToVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalAddTagsToVaultInputRequestTypeDef = TypedDict(
@@ -194,31 +202,42 @@
     {
         "accountId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class AddTagsToVaultInputRequestTypeDef(
     _RequiredAddTagsToVaultInputRequestTypeDef, _OptionalAddTagsToVaultInputRequestTypeDef
 ):
     pass
 
-
 ArchiveCreationOutputTypeDef = TypedDict(
     "ArchiveCreationOutputTypeDef",
     {
         "location": str,
         "checksum": str,
         "archiveId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CSVInputOutputTypeDef = TypedDict(
+    "CSVInputOutputTypeDef",
+    {
+        "FileHeaderInfo": FileHeaderInfoType,
+        "Comments": str,
+        "QuoteEscapeCharacter": str,
+        "RecordDelimiter": str,
+        "FieldDelimiter": str,
+        "QuoteCharacter": str,
+    },
+    total=False,
+)
+
 CSVInputTypeDef = TypedDict(
     "CSVInputTypeDef",
     {
         "FileHeaderInfo": FileHeaderInfoType,
         "Comments": str,
         "QuoteEscapeCharacter": str,
         "RecordDelimiter": str,
@@ -262,22 +281,20 @@
         "accountId": str,
         "archiveSize": str,
         "checksum": str,
     },
     total=False,
 )
 
-
 class CompleteMultipartUploadInputRequestTypeDef(
     _RequiredCompleteMultipartUploadInputRequestTypeDef,
     _OptionalCompleteMultipartUploadInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredCompleteVaultLockInputRequestTypeDef = TypedDict(
     "_RequiredCompleteVaultLockInputRequestTypeDef",
     {
         "vaultName": str,
         "lockId": str,
     },
 )
@@ -285,21 +302,19 @@
     "_OptionalCompleteVaultLockInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class CompleteVaultLockInputRequestTypeDef(
     _RequiredCompleteVaultLockInputRequestTypeDef, _OptionalCompleteVaultLockInputRequestTypeDef
 ):
     pass
 
-
 CreateVaultInputAccountCreateVaultTypeDef = TypedDict(
     "CreateVaultInputAccountCreateVaultTypeDef",
     {
         "vaultName": str,
     },
 )
 
@@ -313,51 +328,56 @@
     "_OptionalCreateVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class CreateVaultInputRequestTypeDef(
     _RequiredCreateVaultInputRequestTypeDef, _OptionalCreateVaultInputRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateVaultInputServiceResourceCreateVaultTypeDef = TypedDict(
     "_RequiredCreateVaultInputServiceResourceCreateVaultTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalCreateVaultInputServiceResourceCreateVaultTypeDef = TypedDict(
     "_OptionalCreateVaultInputServiceResourceCreateVaultTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class CreateVaultInputServiceResourceCreateVaultTypeDef(
     _RequiredCreateVaultInputServiceResourceCreateVaultTypeDef,
     _OptionalCreateVaultInputServiceResourceCreateVaultTypeDef,
 ):
     pass
 
-
 CreateVaultOutputTypeDef = TypedDict(
     "CreateVaultOutputTypeDef",
     {
         "location": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DataRetrievalRuleOutputTypeDef = TypedDict(
+    "DataRetrievalRuleOutputTypeDef",
+    {
+        "Strategy": str,
+        "BytesPerHour": int,
+    },
+    total=False,
+)
+
 DataRetrievalRuleTypeDef = TypedDict(
     "DataRetrievalRuleTypeDef",
     {
         "Strategy": str,
         "BytesPerHour": int,
     },
     total=False,
@@ -374,86 +394,78 @@
     "_OptionalDeleteArchiveInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class DeleteArchiveInputRequestTypeDef(
     _RequiredDeleteArchiveInputRequestTypeDef, _OptionalDeleteArchiveInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVaultAccessPolicyInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDeleteVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_OptionalDeleteVaultAccessPolicyInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class DeleteVaultAccessPolicyInputRequestTypeDef(
     _RequiredDeleteVaultAccessPolicyInputRequestTypeDef,
     _OptionalDeleteVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteVaultInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDeleteVaultInputRequestTypeDef = TypedDict(
     "_OptionalDeleteVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class DeleteVaultInputRequestTypeDef(
     _RequiredDeleteVaultInputRequestTypeDef, _OptionalDeleteVaultInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteVaultNotificationsInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVaultNotificationsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDeleteVaultNotificationsInputRequestTypeDef = TypedDict(
     "_OptionalDeleteVaultNotificationsInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class DeleteVaultNotificationsInputRequestTypeDef(
     _RequiredDeleteVaultNotificationsInputRequestTypeDef,
     _OptionalDeleteVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeJobInputRequestTypeDef = TypedDict(
     "_RequiredDescribeJobInputRequestTypeDef",
     {
         "vaultName": str,
         "jobId": str,
     },
 )
@@ -461,84 +473,90 @@
     "_OptionalDescribeJobInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class DescribeJobInputRequestTypeDef(
     _RequiredDescribeJobInputRequestTypeDef, _OptionalDescribeJobInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeVaultInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDescribeVaultInputRequestTypeDef = TypedDict(
     "_OptionalDescribeVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class DescribeVaultInputRequestTypeDef(
     _RequiredDescribeVaultInputRequestTypeDef, _OptionalDescribeVaultInputRequestTypeDef
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeVaultOutputResponseMetadataTypeDef = TypedDict(
-    "DescribeVaultOutputResponseMetadataTypeDef",
+DescribeVaultOutputTypeDef = TypedDict(
+    "DescribeVaultOutputTypeDef",
     {
         "VaultARN": str,
         "VaultName": str,
         "CreationDate": str,
         "LastInventoryDate": str,
         "NumberOfArchives": int,
         "SizeInBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-DescribeVaultOutputTypeDef = TypedDict(
-    "DescribeVaultOutputTypeDef",
+DescribeVaultResponseMetadataTypeDef = TypedDict(
+    "DescribeVaultResponseMetadataTypeDef",
     {
         "VaultARN": str,
         "VaultName": str,
         "CreationDate": str,
         "LastInventoryDate": str,
         "NumberOfArchives": int,
         "SizeInBytes": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionOutputTypeDef = TypedDict(
+    "EncryptionOutputTypeDef",
+    {
+        "EncryptionType": EncryptionTypeType,
+        "KMSKeyId": str,
+        "KMSContext": str,
+    },
+    total=False,
+)
+
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "EncryptionType": EncryptionTypeType,
         "KMSKeyId": str,
         "KMSContext": str,
     },
@@ -573,21 +591,19 @@
     {
         "accountId": str,
         "range": str,
     },
     total=False,
 )
 
-
 class GetJobOutputInputRequestTypeDef(
     _RequiredGetJobOutputInputRequestTypeDef, _OptionalGetJobOutputInputRequestTypeDef
 ):
     pass
 
-
 GetJobOutputOutputTypeDef = TypedDict(
     "GetJobOutputOutputTypeDef",
     {
         "body": StreamingBody,
         "checksum": str,
         "status": int,
         "contentRange": str,
@@ -608,24 +624,22 @@
     "_OptionalGetVaultAccessPolicyInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class GetVaultAccessPolicyInputRequestTypeDef(
     _RequiredGetVaultAccessPolicyInputRequestTypeDef,
     _OptionalGetVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
-
-VaultAccessPolicyTypeDef = TypedDict(
-    "VaultAccessPolicyTypeDef",
+VaultAccessPolicyOutputTypeDef = TypedDict(
+    "VaultAccessPolicyOutputTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
 
 _RequiredGetVaultLockInputRequestTypeDef = TypedDict(
@@ -638,21 +652,19 @@
     "_OptionalGetVaultLockInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class GetVaultLockInputRequestTypeDef(
     _RequiredGetVaultLockInputRequestTypeDef, _OptionalGetVaultLockInputRequestTypeDef
 ):
     pass
 
-
 GetVaultLockOutputTypeDef = TypedDict(
     "GetVaultLockOutputTypeDef",
     {
         "Policy": str,
         "State": str,
         "ExpirationDate": str,
         "CreationDate": str,
@@ -670,24 +682,22 @@
     "_OptionalGetVaultNotificationsInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class GetVaultNotificationsInputRequestTypeDef(
     _RequiredGetVaultNotificationsInputRequestTypeDef,
     _OptionalGetVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
-
-VaultNotificationConfigTypeDef = TypedDict(
-    "VaultNotificationConfigTypeDef",
+VaultNotificationConfigOutputTypeDef = TypedDict(
+    "VaultNotificationConfigOutputTypeDef",
     {
         "SNSTopic": str,
         "Events": List[str],
     },
     total=False,
 )
 
@@ -699,14 +709,34 @@
         "EndDate": str,
         "Limit": str,
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredGranteeOutputTypeDef = TypedDict(
+    "_RequiredGranteeOutputTypeDef",
+    {
+        "Type": TypeType,
+    },
+)
+_OptionalGranteeOutputTypeDef = TypedDict(
+    "_OptionalGranteeOutputTypeDef",
+    {
+        "DisplayName": str,
+        "URI": str,
+        "ID": str,
+        "EmailAddress": str,
+    },
+    total=False,
+)
+
+class GranteeOutputTypeDef(_RequiredGranteeOutputTypeDef, _OptionalGranteeOutputTypeDef):
+    pass
+
 _RequiredGranteeTypeDef = TypedDict(
     "_RequiredGranteeTypeDef",
     {
         "Type": TypeType,
     },
 )
 _OptionalGranteeTypeDef = TypedDict(
@@ -716,19 +746,17 @@
         "URI": str,
         "ID": str,
         "EmailAddress": str,
     },
     total=False,
 )
 
-
 class GranteeTypeDef(_RequiredGranteeTypeDef, _OptionalGranteeTypeDef):
     pass
 
-
 InitiateJobOutputTypeDef = TypedDict(
     "InitiateJobOutputTypeDef",
     {
         "location": str,
         "jobId": str,
         "jobOutputPath": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -747,22 +775,20 @@
         "accountId": str,
         "archiveDescription": str,
         "partSize": str,
     },
     total=False,
 )
 
-
 class InitiateMultipartUploadInputRequestTypeDef(
     _RequiredInitiateMultipartUploadInputRequestTypeDef,
     _OptionalInitiateMultipartUploadInputRequestTypeDef,
 ):
     pass
 
-
 InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef = TypedDict(
     "InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef",
     {
         "archiveDescription": str,
         "partSize": str,
     },
     total=False,
@@ -829,21 +855,19 @@
         "statuscode": str,
         "completed": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListJobsInputListJobsPaginateTypeDef(
     _RequiredListJobsInputListJobsPaginateTypeDef, _OptionalListJobsInputListJobsPaginateTypeDef
 ):
     pass
 
-
 _RequiredListJobsInputRequestTypeDef = TypedDict(
     "_RequiredListJobsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalListJobsInputRequestTypeDef = TypedDict(
@@ -854,21 +878,19 @@
         "marker": str,
         "statuscode": str,
         "completed": str,
     },
     total=False,
 )
 
-
 class ListJobsInputRequestTypeDef(
     _RequiredListJobsInputRequestTypeDef, _OptionalListJobsInputRequestTypeDef
 ):
     pass
 
-
 _RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
     "_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
     {
         "accountId": str,
         "vaultName": str,
     },
 )
@@ -876,22 +898,20 @@
     "_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef(
     _RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
     _OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListMultipartUploadsInputRequestTypeDef = TypedDict(
     "_RequiredListMultipartUploadsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalListMultipartUploadsInputRequestTypeDef = TypedDict(
@@ -900,22 +920,20 @@
         "accountId": str,
         "marker": str,
         "limit": str,
     },
     total=False,
 )
 
-
 class ListMultipartUploadsInputRequestTypeDef(
     _RequiredListMultipartUploadsInputRequestTypeDef,
     _OptionalListMultipartUploadsInputRequestTypeDef,
 ):
     pass
 
-
 UploadListElementTypeDef = TypedDict(
     "UploadListElementTypeDef",
     {
         "MultipartUploadId": str,
         "VaultARN": str,
         "ArchiveDescription": str,
         "PartSizeInBytes": int,
@@ -936,21 +954,19 @@
     "_OptionalListPartsInputListPartsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListPartsInputListPartsPaginateTypeDef(
     _RequiredListPartsInputListPartsPaginateTypeDef, _OptionalListPartsInputListPartsPaginateTypeDef
 ):
     pass
 
-
 ListPartsInputMultipartUploadPartsTypeDef = TypedDict(
     "ListPartsInputMultipartUploadPartsTypeDef",
     {
         "marker": str,
         "limit": str,
     },
     total=False,
@@ -969,21 +985,19 @@
         "accountId": str,
         "marker": str,
         "limit": str,
     },
     total=False,
 )
 
-
 class ListPartsInputRequestTypeDef(
     _RequiredListPartsInputRequestTypeDef, _OptionalListPartsInputRequestTypeDef
 ):
     pass
 
-
 PartListElementTypeDef = TypedDict(
     "PartListElementTypeDef",
     {
         "RangeInBytes": str,
         "SHA256TreeHash": str,
     },
     total=False,
@@ -1017,21 +1031,19 @@
     "_OptionalListTagsForVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-
 class ListTagsForVaultInputRequestTypeDef(
     _RequiredListTagsForVaultInputRequestTypeDef, _OptionalListTagsForVaultInputRequestTypeDef
 ):
     pass
 
-
 ListTagsForVaultOutputTypeDef = TypedDict(
     "ListTagsForVaultOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1046,22 +1058,20 @@
     "_OptionalListVaultsInputListVaultsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListVaultsInputListVaultsPaginateTypeDef(
     _RequiredListVaultsInputListVaultsPaginateTypeDef,
     _OptionalListVaultsInputListVaultsPaginateTypeDef,
 ):
     pass
 
-
 ListVaultsInputRequestTypeDef = TypedDict(
     "ListVaultsInputRequestTypeDef",
     {
         "accountId": str,
         "marker": str,
         "limit": str,
     },
@@ -1105,32 +1115,47 @@
     {
         "accountId": str,
         "TagKeys": Sequence[str],
     },
     total=False,
 )
 
-
 class RemoveTagsFromVaultInputRequestTypeDef(
     _RequiredRemoveTagsFromVaultInputRequestTypeDef, _OptionalRemoveTagsFromVaultInputRequestTypeDef
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+VaultAccessPolicyTypeDef = TypedDict(
+    "VaultAccessPolicyTypeDef",
+    {
+        "Policy": str,
+    },
+    total=False,
+)
+
+VaultNotificationConfigTypeDef = TypedDict(
+    "VaultNotificationConfigTypeDef",
+    {
+        "SNSTopic": str,
+        "Events": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredUploadArchiveInputRequestTypeDef = TypedDict(
     "_RequiredUploadArchiveInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalUploadArchiveInputRequestTypeDef = TypedDict(
@@ -1140,21 +1165,19 @@
         "archiveDescription": str,
         "checksum": str,
         "body": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-
 class UploadArchiveInputRequestTypeDef(
     _RequiredUploadArchiveInputRequestTypeDef, _OptionalUploadArchiveInputRequestTypeDef
 ):
     pass
 
-
 UploadArchiveInputVaultUploadArchiveTypeDef = TypedDict(
     "UploadArchiveInputVaultUploadArchiveTypeDef",
     {
         "archiveDescription": str,
         "checksum": str,
         "body": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -1185,49 +1208,71 @@
         "checksum": str,
         "range": str,
         "body": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-
 class UploadMultipartPartInputRequestTypeDef(
     _RequiredUploadMultipartPartInputRequestTypeDef, _OptionalUploadMultipartPartInputRequestTypeDef
 ):
     pass
 
-
 UploadMultipartPartOutputTypeDef = TypedDict(
     "UploadMultipartPartOutputTypeDef",
     {
         "checksum": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+InputSerializationOutputTypeDef = TypedDict(
+    "InputSerializationOutputTypeDef",
+    {
+        "csv": CSVInputOutputTypeDef,
+    },
+    total=False,
+)
+
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
         "csv": CSVInputTypeDef,
     },
     total=False,
 )
 
+OutputSerializationOutputTypeDef = TypedDict(
+    "OutputSerializationOutputTypeDef",
+    {
+        "csv": CSVOutputTypeDef,
+    },
+    total=False,
+)
+
 OutputSerializationTypeDef = TypedDict(
     "OutputSerializationTypeDef",
     {
         "csv": CSVOutputTypeDef,
     },
     total=False,
 )
 
+DataRetrievalPolicyOutputTypeDef = TypedDict(
+    "DataRetrievalPolicyOutputTypeDef",
+    {
+        "Rules": List[DataRetrievalRuleOutputTypeDef],
+    },
+    total=False,
+)
+
 DataRetrievalPolicyTypeDef = TypedDict(
     "DataRetrievalPolicyTypeDef",
     {
-        "Rules": List[DataRetrievalRuleTypeDef],
+        "Rules": Sequence[DataRetrievalRuleTypeDef],
     },
     total=False,
 )
 
 _RequiredDescribeVaultInputVaultExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeVaultInputVaultExistsWaitTypeDef",
     {
@@ -1239,22 +1284,20 @@
     "_OptionalDescribeVaultInputVaultExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeVaultInputVaultExistsWaitTypeDef(
     _RequiredDescribeVaultInputVaultExistsWaitTypeDef,
     _OptionalDescribeVaultInputVaultExistsWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeVaultInputVaultNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeVaultInputVaultNotExistsWaitTypeDef",
     {
         "accountId": str,
         "vaultName": str,
     },
 )
@@ -1262,101 +1305,54 @@
     "_OptionalDescribeVaultInputVaultNotExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeVaultInputVaultNotExistsWaitTypeDef(
     _RequiredDescribeVaultInputVaultNotExistsWaitTypeDef,
     _OptionalDescribeVaultInputVaultNotExistsWaitTypeDef,
 ):
     pass
 
-
 ListVaultsOutputTypeDef = TypedDict(
     "ListVaultsOutputTypeDef",
     {
         "VaultList": List[DescribeVaultOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVaultAccessPolicyOutputTypeDef = TypedDict(
     "GetVaultAccessPolicyOutputTypeDef",
     {
-        "policy": VaultAccessPolicyTypeDef,
+        "policy": VaultAccessPolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
-    "_RequiredSetVaultAccessPolicyInputRequestTypeDef",
-    {
-        "vaultName": str,
-    },
-)
-_OptionalSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
-    "_OptionalSetVaultAccessPolicyInputRequestTypeDef",
-    {
-        "accountId": str,
-        "policy": VaultAccessPolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class SetVaultAccessPolicyInputRequestTypeDef(
-    _RequiredSetVaultAccessPolicyInputRequestTypeDef,
-    _OptionalSetVaultAccessPolicyInputRequestTypeDef,
-):
-    pass
-
-
 GetVaultNotificationsOutputTypeDef = TypedDict(
     "GetVaultNotificationsOutputTypeDef",
     {
-        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
+        "vaultNotificationConfig": VaultNotificationConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SetVaultNotificationsInputNotificationSetTypeDef = TypedDict(
-    "SetVaultNotificationsInputNotificationSetTypeDef",
+GrantOutputTypeDef = TypedDict(
+    "GrantOutputTypeDef",
     {
-        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredSetVaultNotificationsInputRequestTypeDef = TypedDict(
-    "_RequiredSetVaultNotificationsInputRequestTypeDef",
-    {
-        "vaultName": str,
-    },
-)
-_OptionalSetVaultNotificationsInputRequestTypeDef = TypedDict(
-    "_OptionalSetVaultNotificationsInputRequestTypeDef",
-    {
-        "accountId": str,
-        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
+        "Grantee": GranteeOutputTypeDef,
+        "Permission": PermissionType,
     },
     total=False,
 )
 
-
-class SetVaultNotificationsInputRequestTypeDef(
-    _RequiredSetVaultNotificationsInputRequestTypeDef,
-    _OptionalSetVaultNotificationsInputRequestTypeDef,
-):
-    pass
-
-
 GrantTypeDef = TypedDict(
     "GrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": PermissionType,
     },
     total=False,
@@ -1373,21 +1369,19 @@
     {
         "accountId": str,
         "policy": VaultLockPolicyTypeDef,
     },
     total=False,
 )
 
-
 class InitiateVaultLockInputRequestTypeDef(
     _RequiredInitiateVaultLockInputRequestTypeDef, _OptionalInitiateVaultLockInputRequestTypeDef
 ):
     pass
 
-
 ListMultipartUploadsOutputTypeDef = TypedDict(
     "ListMultipartUploadsOutputTypeDef",
     {
         "UploadsList": List[UploadListElementTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1411,21 +1405,82 @@
     "ListProvisionedCapacityOutputTypeDef",
     {
         "ProvisionedCapacityList": List[ProvisionedCapacityDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
+    "_RequiredSetVaultAccessPolicyInputRequestTypeDef",
+    {
+        "vaultName": str,
+    },
+)
+_OptionalSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
+    "_OptionalSetVaultAccessPolicyInputRequestTypeDef",
+    {
+        "accountId": str,
+        "policy": VaultAccessPolicyTypeDef,
+    },
+    total=False,
+)
+
+class SetVaultAccessPolicyInputRequestTypeDef(
+    _RequiredSetVaultAccessPolicyInputRequestTypeDef,
+    _OptionalSetVaultAccessPolicyInputRequestTypeDef,
+):
+    pass
+
+SetVaultNotificationsInputNotificationSetTypeDef = TypedDict(
+    "SetVaultNotificationsInputNotificationSetTypeDef",
+    {
+        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSetVaultNotificationsInputRequestTypeDef = TypedDict(
+    "_RequiredSetVaultNotificationsInputRequestTypeDef",
+    {
+        "vaultName": str,
+    },
+)
+_OptionalSetVaultNotificationsInputRequestTypeDef = TypedDict(
+    "_OptionalSetVaultNotificationsInputRequestTypeDef",
+    {
+        "accountId": str,
+        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
+    },
+    total=False,
+)
+
+class SetVaultNotificationsInputRequestTypeDef(
+    _RequiredSetVaultNotificationsInputRequestTypeDef,
+    _OptionalSetVaultNotificationsInputRequestTypeDef,
+):
+    pass
+
+SelectParametersOutputTypeDef = TypedDict(
+    "SelectParametersOutputTypeDef",
+    {
+        "InputSerialization": InputSerializationOutputTypeDef,
+        "ExpressionType": Literal["SQL"],
+        "Expression": str,
+        "OutputSerialization": OutputSerializationOutputTypeDef,
+    },
+    total=False,
+)
+
 SelectParametersResponseMetadataTypeDef = TypedDict(
     "SelectParametersResponseMetadataTypeDef",
     {
-        "InputSerialization": InputSerializationTypeDef,
+        "InputSerialization": InputSerializationOutputTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
-        "OutputSerialization": OutputSerializationTypeDef,
+        "OutputSerialization": OutputSerializationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SelectParametersTypeDef = TypedDict(
     "SelectParametersTypeDef",
     {
@@ -1436,47 +1491,70 @@
     },
     total=False,
 )
 
 GetDataRetrievalPolicyOutputTypeDef = TypedDict(
     "GetDataRetrievalPolicyOutputTypeDef",
     {
-        "Policy": DataRetrievalPolicyTypeDef,
+        "Policy": DataRetrievalPolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetDataRetrievalPolicyInputRequestTypeDef = TypedDict(
     "SetDataRetrievalPolicyInputRequestTypeDef",
     {
         "accountId": str,
         "Policy": DataRetrievalPolicyTypeDef,
     },
     total=False,
 )
 
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
+    {
+        "BucketName": str,
+        "Prefix": str,
+        "Encryption": EncryptionOutputTypeDef,
+        "CannedACL": CannedACLType,
+        "AccessControlList": List[GrantOutputTypeDef],
+        "Tagging": Dict[str, str],
+        "UserMetadata": Dict[str, str],
+        "StorageClass": StorageClassType,
+    },
+    total=False,
+)
+
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "BucketName": str,
         "Prefix": str,
         "Encryption": EncryptionTypeDef,
         "CannedACL": CannedACLType,
-        "AccessControlList": List[GrantTypeDef],
-        "Tagging": Dict[str, str],
-        "UserMetadata": Dict[str, str],
+        "AccessControlList": Sequence[GrantTypeDef],
+        "Tagging": Mapping[str, str],
+        "UserMetadata": Mapping[str, str],
         "StorageClass": StorageClassType,
     },
     total=False,
 )
 
+OutputLocationOutputTypeDef = TypedDict(
+    "OutputLocationOutputTypeDef",
+    {
+        "S3": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
 OutputLocationResponseMetadataTypeDef = TypedDict(
     "OutputLocationResponseMetadataTypeDef",
     {
-        "S3": S3LocationTypeDef,
+        "S3": S3LocationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OutputLocationTypeDef = TypedDict(
     "OutputLocationTypeDef",
     {
@@ -1503,16 +1581,16 @@
         "CompletionDate": str,
         "SHA256TreeHash": str,
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
-        "SelectParameters": SelectParametersTypeDef,
-        "OutputLocation": OutputLocationTypeDef,
+        "SelectParameters": SelectParametersOutputTypeDef,
+        "OutputLocation": OutputLocationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GlacierJobDescriptionTypeDef = TypedDict(
     "GlacierJobDescriptionTypeDef",
     {
@@ -1531,16 +1609,16 @@
         "CompletionDate": str,
         "SHA256TreeHash": str,
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
-        "SelectParameters": SelectParametersTypeDef,
-        "OutputLocation": OutputLocationTypeDef,
+        "SelectParameters": SelectParametersOutputTypeDef,
+        "OutputLocation": OutputLocationOutputTypeDef,
     },
     total=False,
 )
 
 JobParametersTypeDef = TypedDict(
     "JobParametersTypeDef",
     {
@@ -1578,12 +1656,11 @@
     {
         "accountId": str,
         "jobParameters": JobParametersTypeDef,
     },
     total=False,
 )
 
-
 class InitiateJobInputRequestTypeDef(
     _RequiredInitiateJobInputRequestTypeDef, _OptionalInitiateJobInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/type_defs.pyi` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,51 +33,56 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AbortMultipartUploadInputRequestTypeDef",
     "AbortVaultLockInputRequestTypeDef",
     "AddTagsToVaultInputRequestTypeDef",
     "ArchiveCreationOutputTypeDef",
+    "CSVInputOutputTypeDef",
     "CSVInputTypeDef",
     "CSVOutputTypeDef",
     "CompleteMultipartUploadInputMultipartUploadCompleteTypeDef",
     "CompleteMultipartUploadInputRequestTypeDef",
     "CompleteVaultLockInputRequestTypeDef",
     "CreateVaultInputAccountCreateVaultTypeDef",
     "CreateVaultInputRequestTypeDef",
     "CreateVaultInputServiceResourceCreateVaultTypeDef",
     "CreateVaultOutputTypeDef",
+    "DataRetrievalRuleOutputTypeDef",
     "DataRetrievalRuleTypeDef",
     "DeleteArchiveInputRequestTypeDef",
     "DeleteVaultAccessPolicyInputRequestTypeDef",
     "DeleteVaultInputRequestTypeDef",
     "DeleteVaultNotificationsInputRequestTypeDef",
     "DescribeJobInputRequestTypeDef",
     "DescribeVaultInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeVaultOutputResponseMetadataTypeDef",
     "DescribeVaultOutputTypeDef",
+    "DescribeVaultResponseMetadataTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionOutputTypeDef",
     "EncryptionTypeDef",
     "GetDataRetrievalPolicyInputRequestTypeDef",
     "GetJobOutputInputJobGetOutputTypeDef",
     "GetJobOutputInputRequestTypeDef",
     "GetJobOutputOutputTypeDef",
     "GetVaultAccessPolicyInputRequestTypeDef",
-    "VaultAccessPolicyTypeDef",
+    "VaultAccessPolicyOutputTypeDef",
     "GetVaultLockInputRequestTypeDef",
     "GetVaultLockOutputTypeDef",
     "GetVaultNotificationsInputRequestTypeDef",
-    "VaultNotificationConfigTypeDef",
+    "VaultNotificationConfigOutputTypeDef",
     "InventoryRetrievalJobDescriptionTypeDef",
+    "GranteeOutputTypeDef",
     "GranteeTypeDef",
     "InitiateJobOutputTypeDef",
     "InitiateMultipartUploadInputRequestTypeDef",
     "InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef",
     "InitiateMultipartUploadOutputTypeDef",
     "VaultLockPolicyTypeDef",
     "InitiateVaultLockOutputTypeDef",
@@ -99,40 +104,49 @@
     "ListVaultsInputListVaultsPaginateTypeDef",
     "ListVaultsInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "PurchaseProvisionedCapacityInputRequestTypeDef",
     "PurchaseProvisionedCapacityOutputTypeDef",
     "RemoveTagsFromVaultInputRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "VaultAccessPolicyTypeDef",
+    "VaultNotificationConfigTypeDef",
     "UploadArchiveInputRequestTypeDef",
     "UploadArchiveInputVaultUploadArchiveTypeDef",
     "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
     "UploadMultipartPartInputRequestTypeDef",
     "UploadMultipartPartOutputTypeDef",
+    "InputSerializationOutputTypeDef",
     "InputSerializationTypeDef",
+    "OutputSerializationOutputTypeDef",
     "OutputSerializationTypeDef",
+    "DataRetrievalPolicyOutputTypeDef",
     "DataRetrievalPolicyTypeDef",
     "DescribeVaultInputVaultExistsWaitTypeDef",
     "DescribeVaultInputVaultNotExistsWaitTypeDef",
     "ListVaultsOutputTypeDef",
     "GetVaultAccessPolicyOutputTypeDef",
-    "SetVaultAccessPolicyInputRequestTypeDef",
     "GetVaultNotificationsOutputTypeDef",
-    "SetVaultNotificationsInputNotificationSetTypeDef",
-    "SetVaultNotificationsInputRequestTypeDef",
+    "GrantOutputTypeDef",
     "GrantTypeDef",
     "InitiateVaultLockInputRequestTypeDef",
     "ListMultipartUploadsOutputTypeDef",
     "ListPartsOutputTypeDef",
     "ListProvisionedCapacityOutputTypeDef",
+    "SetVaultAccessPolicyInputRequestTypeDef",
+    "SetVaultNotificationsInputNotificationSetTypeDef",
+    "SetVaultNotificationsInputRequestTypeDef",
+    "SelectParametersOutputTypeDef",
     "SelectParametersResponseMetadataTypeDef",
     "SelectParametersTypeDef",
     "GetDataRetrievalPolicyOutputTypeDef",
     "SetDataRetrievalPolicyInputRequestTypeDef",
+    "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
+    "OutputLocationOutputTypeDef",
     "OutputLocationResponseMetadataTypeDef",
     "OutputLocationTypeDef",
     "GlacierJobDescriptionResponseMetadataTypeDef",
     "GlacierJobDescriptionTypeDef",
     "JobParametersTypeDef",
     "ListJobsOutputTypeDef",
     "InitiateJobInputRequestTypeDef",
@@ -149,39 +163,43 @@
     "_OptionalAbortMultipartUploadInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class AbortMultipartUploadInputRequestTypeDef(
     _RequiredAbortMultipartUploadInputRequestTypeDef,
     _OptionalAbortMultipartUploadInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredAbortVaultLockInputRequestTypeDef = TypedDict(
     "_RequiredAbortVaultLockInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalAbortVaultLockInputRequestTypeDef = TypedDict(
     "_OptionalAbortVaultLockInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class AbortVaultLockInputRequestTypeDef(
     _RequiredAbortVaultLockInputRequestTypeDef, _OptionalAbortVaultLockInputRequestTypeDef
 ):
     pass
 
+
 _RequiredAddTagsToVaultInputRequestTypeDef = TypedDict(
     "_RequiredAddTagsToVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalAddTagsToVaultInputRequestTypeDef = TypedDict(
@@ -189,29 +207,44 @@
     {
         "accountId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class AddTagsToVaultInputRequestTypeDef(
     _RequiredAddTagsToVaultInputRequestTypeDef, _OptionalAddTagsToVaultInputRequestTypeDef
 ):
     pass
 
+
 ArchiveCreationOutputTypeDef = TypedDict(
     "ArchiveCreationOutputTypeDef",
     {
         "location": str,
         "checksum": str,
         "archiveId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CSVInputOutputTypeDef = TypedDict(
+    "CSVInputOutputTypeDef",
+    {
+        "FileHeaderInfo": FileHeaderInfoType,
+        "Comments": str,
+        "QuoteEscapeCharacter": str,
+        "RecordDelimiter": str,
+        "FieldDelimiter": str,
+        "QuoteCharacter": str,
+    },
+    total=False,
+)
+
 CSVInputTypeDef = TypedDict(
     "CSVInputTypeDef",
     {
         "FileHeaderInfo": FileHeaderInfoType,
         "Comments": str,
         "QuoteEscapeCharacter": str,
         "RecordDelimiter": str,
@@ -255,20 +288,22 @@
         "accountId": str,
         "archiveSize": str,
         "checksum": str,
     },
     total=False,
 )
 
+
 class CompleteMultipartUploadInputRequestTypeDef(
     _RequiredCompleteMultipartUploadInputRequestTypeDef,
     _OptionalCompleteMultipartUploadInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredCompleteVaultLockInputRequestTypeDef = TypedDict(
     "_RequiredCompleteVaultLockInputRequestTypeDef",
     {
         "vaultName": str,
         "lockId": str,
     },
 )
@@ -276,19 +311,21 @@
     "_OptionalCompleteVaultLockInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class CompleteVaultLockInputRequestTypeDef(
     _RequiredCompleteVaultLockInputRequestTypeDef, _OptionalCompleteVaultLockInputRequestTypeDef
 ):
     pass
 
+
 CreateVaultInputAccountCreateVaultTypeDef = TypedDict(
     "CreateVaultInputAccountCreateVaultTypeDef",
     {
         "vaultName": str,
     },
 )
 
@@ -302,47 +339,60 @@
     "_OptionalCreateVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class CreateVaultInputRequestTypeDef(
     _RequiredCreateVaultInputRequestTypeDef, _OptionalCreateVaultInputRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateVaultInputServiceResourceCreateVaultTypeDef = TypedDict(
     "_RequiredCreateVaultInputServiceResourceCreateVaultTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalCreateVaultInputServiceResourceCreateVaultTypeDef = TypedDict(
     "_OptionalCreateVaultInputServiceResourceCreateVaultTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class CreateVaultInputServiceResourceCreateVaultTypeDef(
     _RequiredCreateVaultInputServiceResourceCreateVaultTypeDef,
     _OptionalCreateVaultInputServiceResourceCreateVaultTypeDef,
 ):
     pass
 
+
 CreateVaultOutputTypeDef = TypedDict(
     "CreateVaultOutputTypeDef",
     {
         "location": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DataRetrievalRuleOutputTypeDef = TypedDict(
+    "DataRetrievalRuleOutputTypeDef",
+    {
+        "Strategy": str,
+        "BytesPerHour": int,
+    },
+    total=False,
+)
+
 DataRetrievalRuleTypeDef = TypedDict(
     "DataRetrievalRuleTypeDef",
     {
         "Strategy": str,
         "BytesPerHour": int,
     },
     total=False,
@@ -359,78 +409,86 @@
     "_OptionalDeleteArchiveInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class DeleteArchiveInputRequestTypeDef(
     _RequiredDeleteArchiveInputRequestTypeDef, _OptionalDeleteArchiveInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVaultAccessPolicyInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDeleteVaultAccessPolicyInputRequestTypeDef = TypedDict(
     "_OptionalDeleteVaultAccessPolicyInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class DeleteVaultAccessPolicyInputRequestTypeDef(
     _RequiredDeleteVaultAccessPolicyInputRequestTypeDef,
     _OptionalDeleteVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteVaultInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDeleteVaultInputRequestTypeDef = TypedDict(
     "_OptionalDeleteVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class DeleteVaultInputRequestTypeDef(
     _RequiredDeleteVaultInputRequestTypeDef, _OptionalDeleteVaultInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteVaultNotificationsInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVaultNotificationsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDeleteVaultNotificationsInputRequestTypeDef = TypedDict(
     "_OptionalDeleteVaultNotificationsInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class DeleteVaultNotificationsInputRequestTypeDef(
     _RequiredDeleteVaultNotificationsInputRequestTypeDef,
     _OptionalDeleteVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeJobInputRequestTypeDef = TypedDict(
     "_RequiredDescribeJobInputRequestTypeDef",
     {
         "vaultName": str,
         "jobId": str,
     },
 )
@@ -438,80 +496,94 @@
     "_OptionalDescribeJobInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class DescribeJobInputRequestTypeDef(
     _RequiredDescribeJobInputRequestTypeDef, _OptionalDescribeJobInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeVaultInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVaultInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalDescribeVaultInputRequestTypeDef = TypedDict(
     "_OptionalDescribeVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class DescribeVaultInputRequestTypeDef(
     _RequiredDescribeVaultInputRequestTypeDef, _OptionalDescribeVaultInputRequestTypeDef
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeVaultOutputResponseMetadataTypeDef = TypedDict(
-    "DescribeVaultOutputResponseMetadataTypeDef",
+DescribeVaultOutputTypeDef = TypedDict(
+    "DescribeVaultOutputTypeDef",
     {
         "VaultARN": str,
         "VaultName": str,
         "CreationDate": str,
         "LastInventoryDate": str,
         "NumberOfArchives": int,
         "SizeInBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-DescribeVaultOutputTypeDef = TypedDict(
-    "DescribeVaultOutputTypeDef",
+DescribeVaultResponseMetadataTypeDef = TypedDict(
+    "DescribeVaultResponseMetadataTypeDef",
     {
         "VaultARN": str,
         "VaultName": str,
         "CreationDate": str,
         "LastInventoryDate": str,
         "NumberOfArchives": int,
         "SizeInBytes": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionOutputTypeDef = TypedDict(
+    "EncryptionOutputTypeDef",
+    {
+        "EncryptionType": EncryptionTypeType,
+        "KMSKeyId": str,
+        "KMSContext": str,
+    },
+    total=False,
+)
+
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "EncryptionType": EncryptionTypeType,
         "KMSKeyId": str,
         "KMSContext": str,
     },
@@ -546,19 +618,21 @@
     {
         "accountId": str,
         "range": str,
     },
     total=False,
 )
 
+
 class GetJobOutputInputRequestTypeDef(
     _RequiredGetJobOutputInputRequestTypeDef, _OptionalGetJobOutputInputRequestTypeDef
 ):
     pass
 
+
 GetJobOutputOutputTypeDef = TypedDict(
     "GetJobOutputOutputTypeDef",
     {
         "body": StreamingBody,
         "checksum": str,
         "status": int,
         "contentRange": str,
@@ -579,22 +653,24 @@
     "_OptionalGetVaultAccessPolicyInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class GetVaultAccessPolicyInputRequestTypeDef(
     _RequiredGetVaultAccessPolicyInputRequestTypeDef,
     _OptionalGetVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
-VaultAccessPolicyTypeDef = TypedDict(
-    "VaultAccessPolicyTypeDef",
+
+VaultAccessPolicyOutputTypeDef = TypedDict(
+    "VaultAccessPolicyOutputTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
 
 _RequiredGetVaultLockInputRequestTypeDef = TypedDict(
@@ -607,19 +683,21 @@
     "_OptionalGetVaultLockInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class GetVaultLockInputRequestTypeDef(
     _RequiredGetVaultLockInputRequestTypeDef, _OptionalGetVaultLockInputRequestTypeDef
 ):
     pass
 
+
 GetVaultLockOutputTypeDef = TypedDict(
     "GetVaultLockOutputTypeDef",
     {
         "Policy": str,
         "State": str,
         "ExpirationDate": str,
         "CreationDate": str,
@@ -637,22 +715,24 @@
     "_OptionalGetVaultNotificationsInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class GetVaultNotificationsInputRequestTypeDef(
     _RequiredGetVaultNotificationsInputRequestTypeDef,
     _OptionalGetVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
-VaultNotificationConfigTypeDef = TypedDict(
-    "VaultNotificationConfigTypeDef",
+
+VaultNotificationConfigOutputTypeDef = TypedDict(
+    "VaultNotificationConfigOutputTypeDef",
     {
         "SNSTopic": str,
         "Events": List[str],
     },
     total=False,
 )
 
@@ -664,14 +744,36 @@
         "EndDate": str,
         "Limit": str,
         "Marker": str,
     },
     total=False,
 )
 
+_RequiredGranteeOutputTypeDef = TypedDict(
+    "_RequiredGranteeOutputTypeDef",
+    {
+        "Type": TypeType,
+    },
+)
+_OptionalGranteeOutputTypeDef = TypedDict(
+    "_OptionalGranteeOutputTypeDef",
+    {
+        "DisplayName": str,
+        "URI": str,
+        "ID": str,
+        "EmailAddress": str,
+    },
+    total=False,
+)
+
+
+class GranteeOutputTypeDef(_RequiredGranteeOutputTypeDef, _OptionalGranteeOutputTypeDef):
+    pass
+
+
 _RequiredGranteeTypeDef = TypedDict(
     "_RequiredGranteeTypeDef",
     {
         "Type": TypeType,
     },
 )
 _OptionalGranteeTypeDef = TypedDict(
@@ -681,17 +783,19 @@
         "URI": str,
         "ID": str,
         "EmailAddress": str,
     },
     total=False,
 )
 
+
 class GranteeTypeDef(_RequiredGranteeTypeDef, _OptionalGranteeTypeDef):
     pass
 
+
 InitiateJobOutputTypeDef = TypedDict(
     "InitiateJobOutputTypeDef",
     {
         "location": str,
         "jobId": str,
         "jobOutputPath": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -710,20 +814,22 @@
         "accountId": str,
         "archiveDescription": str,
         "partSize": str,
     },
     total=False,
 )
 
+
 class InitiateMultipartUploadInputRequestTypeDef(
     _RequiredInitiateMultipartUploadInputRequestTypeDef,
     _OptionalInitiateMultipartUploadInputRequestTypeDef,
 ):
     pass
 
+
 InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef = TypedDict(
     "InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef",
     {
         "archiveDescription": str,
         "partSize": str,
     },
     total=False,
@@ -790,19 +896,21 @@
         "statuscode": str,
         "completed": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListJobsInputListJobsPaginateTypeDef(
     _RequiredListJobsInputListJobsPaginateTypeDef, _OptionalListJobsInputListJobsPaginateTypeDef
 ):
     pass
 
+
 _RequiredListJobsInputRequestTypeDef = TypedDict(
     "_RequiredListJobsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalListJobsInputRequestTypeDef = TypedDict(
@@ -813,19 +921,21 @@
         "marker": str,
         "statuscode": str,
         "completed": str,
     },
     total=False,
 )
 
+
 class ListJobsInputRequestTypeDef(
     _RequiredListJobsInputRequestTypeDef, _OptionalListJobsInputRequestTypeDef
 ):
     pass
 
+
 _RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef = TypedDict(
     "_RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
     {
         "accountId": str,
         "vaultName": str,
     },
 )
@@ -833,20 +943,22 @@
     "_OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef(
     _RequiredListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
     _OptionalListMultipartUploadsInputListMultipartUploadsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListMultipartUploadsInputRequestTypeDef = TypedDict(
     "_RequiredListMultipartUploadsInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalListMultipartUploadsInputRequestTypeDef = TypedDict(
@@ -855,20 +967,22 @@
         "accountId": str,
         "marker": str,
         "limit": str,
     },
     total=False,
 )
 
+
 class ListMultipartUploadsInputRequestTypeDef(
     _RequiredListMultipartUploadsInputRequestTypeDef,
     _OptionalListMultipartUploadsInputRequestTypeDef,
 ):
     pass
 
+
 UploadListElementTypeDef = TypedDict(
     "UploadListElementTypeDef",
     {
         "MultipartUploadId": str,
         "VaultARN": str,
         "ArchiveDescription": str,
         "PartSizeInBytes": int,
@@ -889,19 +1003,21 @@
     "_OptionalListPartsInputListPartsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListPartsInputListPartsPaginateTypeDef(
     _RequiredListPartsInputListPartsPaginateTypeDef, _OptionalListPartsInputListPartsPaginateTypeDef
 ):
     pass
 
+
 ListPartsInputMultipartUploadPartsTypeDef = TypedDict(
     "ListPartsInputMultipartUploadPartsTypeDef",
     {
         "marker": str,
         "limit": str,
     },
     total=False,
@@ -920,19 +1036,21 @@
         "accountId": str,
         "marker": str,
         "limit": str,
     },
     total=False,
 )
 
+
 class ListPartsInputRequestTypeDef(
     _RequiredListPartsInputRequestTypeDef, _OptionalListPartsInputRequestTypeDef
 ):
     pass
 
+
 PartListElementTypeDef = TypedDict(
     "PartListElementTypeDef",
     {
         "RangeInBytes": str,
         "SHA256TreeHash": str,
     },
     total=False,
@@ -966,19 +1084,21 @@
     "_OptionalListTagsForVaultInputRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
+
 class ListTagsForVaultInputRequestTypeDef(
     _RequiredListTagsForVaultInputRequestTypeDef, _OptionalListTagsForVaultInputRequestTypeDef
 ):
     pass
 
+
 ListTagsForVaultOutputTypeDef = TypedDict(
     "ListTagsForVaultOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -993,20 +1113,22 @@
     "_OptionalListVaultsInputListVaultsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListVaultsInputListVaultsPaginateTypeDef(
     _RequiredListVaultsInputListVaultsPaginateTypeDef,
     _OptionalListVaultsInputListVaultsPaginateTypeDef,
 ):
     pass
 
+
 ListVaultsInputRequestTypeDef = TypedDict(
     "ListVaultsInputRequestTypeDef",
     {
         "accountId": str,
         "marker": str,
         "limit": str,
     },
@@ -1050,30 +1172,49 @@
     {
         "accountId": str,
         "TagKeys": Sequence[str],
     },
     total=False,
 )
 
+
 class RemoveTagsFromVaultInputRequestTypeDef(
     _RequiredRemoveTagsFromVaultInputRequestTypeDef, _OptionalRemoveTagsFromVaultInputRequestTypeDef
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+VaultAccessPolicyTypeDef = TypedDict(
+    "VaultAccessPolicyTypeDef",
+    {
+        "Policy": str,
+    },
+    total=False,
+)
+
+VaultNotificationConfigTypeDef = TypedDict(
+    "VaultNotificationConfigTypeDef",
+    {
+        "SNSTopic": str,
+        "Events": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredUploadArchiveInputRequestTypeDef = TypedDict(
     "_RequiredUploadArchiveInputRequestTypeDef",
     {
         "vaultName": str,
     },
 )
 _OptionalUploadArchiveInputRequestTypeDef = TypedDict(
@@ -1083,19 +1224,21 @@
         "archiveDescription": str,
         "checksum": str,
         "body": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
+
 class UploadArchiveInputRequestTypeDef(
     _RequiredUploadArchiveInputRequestTypeDef, _OptionalUploadArchiveInputRequestTypeDef
 ):
     pass
 
+
 UploadArchiveInputVaultUploadArchiveTypeDef = TypedDict(
     "UploadArchiveInputVaultUploadArchiveTypeDef",
     {
         "archiveDescription": str,
         "checksum": str,
         "body": Union[str, bytes, IO[Any], StreamingBody],
     },
@@ -1126,47 +1269,73 @@
         "checksum": str,
         "range": str,
         "body": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
+
 class UploadMultipartPartInputRequestTypeDef(
     _RequiredUploadMultipartPartInputRequestTypeDef, _OptionalUploadMultipartPartInputRequestTypeDef
 ):
     pass
 
+
 UploadMultipartPartOutputTypeDef = TypedDict(
     "UploadMultipartPartOutputTypeDef",
     {
         "checksum": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+InputSerializationOutputTypeDef = TypedDict(
+    "InputSerializationOutputTypeDef",
+    {
+        "csv": CSVInputOutputTypeDef,
+    },
+    total=False,
+)
+
 InputSerializationTypeDef = TypedDict(
     "InputSerializationTypeDef",
     {
         "csv": CSVInputTypeDef,
     },
     total=False,
 )
 
+OutputSerializationOutputTypeDef = TypedDict(
+    "OutputSerializationOutputTypeDef",
+    {
+        "csv": CSVOutputTypeDef,
+    },
+    total=False,
+)
+
 OutputSerializationTypeDef = TypedDict(
     "OutputSerializationTypeDef",
     {
         "csv": CSVOutputTypeDef,
     },
     total=False,
 )
 
+DataRetrievalPolicyOutputTypeDef = TypedDict(
+    "DataRetrievalPolicyOutputTypeDef",
+    {
+        "Rules": List[DataRetrievalRuleOutputTypeDef],
+    },
+    total=False,
+)
+
 DataRetrievalPolicyTypeDef = TypedDict(
     "DataRetrievalPolicyTypeDef",
     {
-        "Rules": List[DataRetrievalRuleTypeDef],
+        "Rules": Sequence[DataRetrievalRuleTypeDef],
     },
     total=False,
 )
 
 _RequiredDescribeVaultInputVaultExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeVaultInputVaultExistsWaitTypeDef",
     {
@@ -1178,20 +1347,22 @@
     "_OptionalDescribeVaultInputVaultExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeVaultInputVaultExistsWaitTypeDef(
     _RequiredDescribeVaultInputVaultExistsWaitTypeDef,
     _OptionalDescribeVaultInputVaultExistsWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeVaultInputVaultNotExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeVaultInputVaultNotExistsWaitTypeDef",
     {
         "accountId": str,
         "vaultName": str,
     },
 )
@@ -1199,95 +1370,56 @@
     "_OptionalDescribeVaultInputVaultNotExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeVaultInputVaultNotExistsWaitTypeDef(
     _RequiredDescribeVaultInputVaultNotExistsWaitTypeDef,
     _OptionalDescribeVaultInputVaultNotExistsWaitTypeDef,
 ):
     pass
 
+
 ListVaultsOutputTypeDef = TypedDict(
     "ListVaultsOutputTypeDef",
     {
         "VaultList": List[DescribeVaultOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetVaultAccessPolicyOutputTypeDef = TypedDict(
     "GetVaultAccessPolicyOutputTypeDef",
     {
-        "policy": VaultAccessPolicyTypeDef,
+        "policy": VaultAccessPolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
-    "_RequiredSetVaultAccessPolicyInputRequestTypeDef",
-    {
-        "vaultName": str,
-    },
-)
-_OptionalSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
-    "_OptionalSetVaultAccessPolicyInputRequestTypeDef",
-    {
-        "accountId": str,
-        "policy": VaultAccessPolicyTypeDef,
-    },
-    total=False,
-)
-
-class SetVaultAccessPolicyInputRequestTypeDef(
-    _RequiredSetVaultAccessPolicyInputRequestTypeDef,
-    _OptionalSetVaultAccessPolicyInputRequestTypeDef,
-):
-    pass
-
 GetVaultNotificationsOutputTypeDef = TypedDict(
     "GetVaultNotificationsOutputTypeDef",
     {
-        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
+        "vaultNotificationConfig": VaultNotificationConfigOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SetVaultNotificationsInputNotificationSetTypeDef = TypedDict(
-    "SetVaultNotificationsInputNotificationSetTypeDef",
+GrantOutputTypeDef = TypedDict(
+    "GrantOutputTypeDef",
     {
-        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredSetVaultNotificationsInputRequestTypeDef = TypedDict(
-    "_RequiredSetVaultNotificationsInputRequestTypeDef",
-    {
-        "vaultName": str,
-    },
-)
-_OptionalSetVaultNotificationsInputRequestTypeDef = TypedDict(
-    "_OptionalSetVaultNotificationsInputRequestTypeDef",
-    {
-        "accountId": str,
-        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
+        "Grantee": GranteeOutputTypeDef,
+        "Permission": PermissionType,
     },
     total=False,
 )
 
-class SetVaultNotificationsInputRequestTypeDef(
-    _RequiredSetVaultNotificationsInputRequestTypeDef,
-    _OptionalSetVaultNotificationsInputRequestTypeDef,
-):
-    pass
-
 GrantTypeDef = TypedDict(
     "GrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": PermissionType,
     },
     total=False,
@@ -1304,19 +1436,21 @@
     {
         "accountId": str,
         "policy": VaultLockPolicyTypeDef,
     },
     total=False,
 )
 
+
 class InitiateVaultLockInputRequestTypeDef(
     _RequiredInitiateVaultLockInputRequestTypeDef, _OptionalInitiateVaultLockInputRequestTypeDef
 ):
     pass
 
+
 ListMultipartUploadsOutputTypeDef = TypedDict(
     "ListMultipartUploadsOutputTypeDef",
     {
         "UploadsList": List[UploadListElementTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1340,21 +1474,86 @@
     "ListProvisionedCapacityOutputTypeDef",
     {
         "ProvisionedCapacityList": List[ProvisionedCapacityDescriptionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
+    "_RequiredSetVaultAccessPolicyInputRequestTypeDef",
+    {
+        "vaultName": str,
+    },
+)
+_OptionalSetVaultAccessPolicyInputRequestTypeDef = TypedDict(
+    "_OptionalSetVaultAccessPolicyInputRequestTypeDef",
+    {
+        "accountId": str,
+        "policy": VaultAccessPolicyTypeDef,
+    },
+    total=False,
+)
+
+
+class SetVaultAccessPolicyInputRequestTypeDef(
+    _RequiredSetVaultAccessPolicyInputRequestTypeDef,
+    _OptionalSetVaultAccessPolicyInputRequestTypeDef,
+):
+    pass
+
+
+SetVaultNotificationsInputNotificationSetTypeDef = TypedDict(
+    "SetVaultNotificationsInputNotificationSetTypeDef",
+    {
+        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSetVaultNotificationsInputRequestTypeDef = TypedDict(
+    "_RequiredSetVaultNotificationsInputRequestTypeDef",
+    {
+        "vaultName": str,
+    },
+)
+_OptionalSetVaultNotificationsInputRequestTypeDef = TypedDict(
+    "_OptionalSetVaultNotificationsInputRequestTypeDef",
+    {
+        "accountId": str,
+        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SetVaultNotificationsInputRequestTypeDef(
+    _RequiredSetVaultNotificationsInputRequestTypeDef,
+    _OptionalSetVaultNotificationsInputRequestTypeDef,
+):
+    pass
+
+
+SelectParametersOutputTypeDef = TypedDict(
+    "SelectParametersOutputTypeDef",
+    {
+        "InputSerialization": InputSerializationOutputTypeDef,
+        "ExpressionType": Literal["SQL"],
+        "Expression": str,
+        "OutputSerialization": OutputSerializationOutputTypeDef,
+    },
+    total=False,
+)
+
 SelectParametersResponseMetadataTypeDef = TypedDict(
     "SelectParametersResponseMetadataTypeDef",
     {
-        "InputSerialization": InputSerializationTypeDef,
+        "InputSerialization": InputSerializationOutputTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
-        "OutputSerialization": OutputSerializationTypeDef,
+        "OutputSerialization": OutputSerializationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SelectParametersTypeDef = TypedDict(
     "SelectParametersTypeDef",
     {
@@ -1365,47 +1564,70 @@
     },
     total=False,
 )
 
 GetDataRetrievalPolicyOutputTypeDef = TypedDict(
     "GetDataRetrievalPolicyOutputTypeDef",
     {
-        "Policy": DataRetrievalPolicyTypeDef,
+        "Policy": DataRetrievalPolicyOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SetDataRetrievalPolicyInputRequestTypeDef = TypedDict(
     "SetDataRetrievalPolicyInputRequestTypeDef",
     {
         "accountId": str,
         "Policy": DataRetrievalPolicyTypeDef,
     },
     total=False,
 )
 
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
+    {
+        "BucketName": str,
+        "Prefix": str,
+        "Encryption": EncryptionOutputTypeDef,
+        "CannedACL": CannedACLType,
+        "AccessControlList": List[GrantOutputTypeDef],
+        "Tagging": Dict[str, str],
+        "UserMetadata": Dict[str, str],
+        "StorageClass": StorageClassType,
+    },
+    total=False,
+)
+
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "BucketName": str,
         "Prefix": str,
         "Encryption": EncryptionTypeDef,
         "CannedACL": CannedACLType,
-        "AccessControlList": List[GrantTypeDef],
-        "Tagging": Dict[str, str],
-        "UserMetadata": Dict[str, str],
+        "AccessControlList": Sequence[GrantTypeDef],
+        "Tagging": Mapping[str, str],
+        "UserMetadata": Mapping[str, str],
         "StorageClass": StorageClassType,
     },
     total=False,
 )
 
+OutputLocationOutputTypeDef = TypedDict(
+    "OutputLocationOutputTypeDef",
+    {
+        "S3": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
 OutputLocationResponseMetadataTypeDef = TypedDict(
     "OutputLocationResponseMetadataTypeDef",
     {
-        "S3": S3LocationTypeDef,
+        "S3": S3LocationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OutputLocationTypeDef = TypedDict(
     "OutputLocationTypeDef",
     {
@@ -1432,16 +1654,16 @@
         "CompletionDate": str,
         "SHA256TreeHash": str,
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
-        "SelectParameters": SelectParametersTypeDef,
-        "OutputLocation": OutputLocationTypeDef,
+        "SelectParameters": SelectParametersOutputTypeDef,
+        "OutputLocation": OutputLocationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GlacierJobDescriptionTypeDef = TypedDict(
     "GlacierJobDescriptionTypeDef",
     {
@@ -1460,16 +1682,16 @@
         "CompletionDate": str,
         "SHA256TreeHash": str,
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
-        "SelectParameters": SelectParametersTypeDef,
-        "OutputLocation": OutputLocationTypeDef,
+        "SelectParameters": SelectParametersOutputTypeDef,
+        "OutputLocation": OutputLocationOutputTypeDef,
     },
     total=False,
 )
 
 JobParametersTypeDef = TypedDict(
     "JobParametersTypeDef",
     {
@@ -1507,11 +1729,12 @@
     {
         "accountId": str,
         "jobParameters": JobParametersTypeDef,
     },
     total=False,
 )
 
+
 class InitiateJobInputRequestTypeDef(
     _RequiredInitiateJobInputRequestTypeDef, _OptionalInitiateJobInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/waiter.py` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier/waiter.pyi` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier.egg-info/PKG-INFO` & `mypy-boto3-glacier-1.28.12/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-glacier
-Version: 1.28.0
-Summary: Type annotations for boto3.Glacier 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 glacier type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-glacier"></a>
 
 # mypy-boto3-glacier
 
 [![PyPI - mypy-boto3-glacier](https://img.shields.io/pypi/v/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glacier.svg?color=blue)](https://pypi.org/project/mypy-boto3-glacier)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glacier?color=blue)](https://pypistats.org/packages/mypy-boto3-glacier)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glacier)](https://pepy.tech/project/mypy-boto3-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glacier 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[boto3.Glacier 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [mypy-boto3-glacier docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glacier/).
 
 See how it helps to find and fix potential bugs:
 
@@ -440,46 +408,50 @@
 
 ```python
 from mypy_boto3_glacier.type_defs import (
     AbortMultipartUploadInputRequestTypeDef,
     AbortVaultLockInputRequestTypeDef,
     AddTagsToVaultInputRequestTypeDef,
     ArchiveCreationOutputTypeDef,
+    CSVInputOutputTypeDef,
     CSVInputTypeDef,
     CSVOutputTypeDef,
     CompleteMultipartUploadInputMultipartUploadCompleteTypeDef,
     CompleteMultipartUploadInputRequestTypeDef,
     CompleteVaultLockInputRequestTypeDef,
     CreateVaultInputAccountCreateVaultTypeDef,
     CreateVaultInputRequestTypeDef,
     CreateVaultInputServiceResourceCreateVaultTypeDef,
     CreateVaultOutputTypeDef,
+    DataRetrievalRuleOutputTypeDef,
     DataRetrievalRuleTypeDef,
     DeleteArchiveInputRequestTypeDef,
     DeleteVaultAccessPolicyInputRequestTypeDef,
     DeleteVaultInputRequestTypeDef,
     DeleteVaultNotificationsInputRequestTypeDef,
     DescribeJobInputRequestTypeDef,
     DescribeVaultInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeVaultOutputResponseMetadataTypeDef,
     DescribeVaultOutputTypeDef,
+    DescribeVaultResponseMetadataTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionOutputTypeDef,
     EncryptionTypeDef,
     GetDataRetrievalPolicyInputRequestTypeDef,
     GetJobOutputInputJobGetOutputTypeDef,
     GetJobOutputInputRequestTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyInputRequestTypeDef,
-    VaultAccessPolicyTypeDef,
+    VaultAccessPolicyOutputTypeDef,
     GetVaultLockInputRequestTypeDef,
     GetVaultLockOutputTypeDef,
     GetVaultNotificationsInputRequestTypeDef,
-    VaultNotificationConfigTypeDef,
+    VaultNotificationConfigOutputTypeDef,
     InventoryRetrievalJobDescriptionTypeDef,
+    GranteeOutputTypeDef,
     GranteeTypeDef,
     InitiateJobOutputTypeDef,
     InitiateMultipartUploadInputRequestTypeDef,
     InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef,
     InitiateMultipartUploadOutputTypeDef,
     VaultLockPolicyTypeDef,
     InitiateVaultLockOutputTypeDef,
@@ -501,40 +473,49 @@
     ListVaultsInputListVaultsPaginateTypeDef,
     ListVaultsInputRequestTypeDef,
     PaginatorConfigTypeDef,
     PurchaseProvisionedCapacityInputRequestTypeDef,
     PurchaseProvisionedCapacityOutputTypeDef,
     RemoveTagsFromVaultInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    VaultAccessPolicyTypeDef,
+    VaultNotificationConfigTypeDef,
     UploadArchiveInputRequestTypeDef,
     UploadArchiveInputVaultUploadArchiveTypeDef,
     UploadMultipartPartInputMultipartUploadUploadPartTypeDef,
     UploadMultipartPartInputRequestTypeDef,
     UploadMultipartPartOutputTypeDef,
+    InputSerializationOutputTypeDef,
     InputSerializationTypeDef,
+    OutputSerializationOutputTypeDef,
     OutputSerializationTypeDef,
+    DataRetrievalPolicyOutputTypeDef,
     DataRetrievalPolicyTypeDef,
     DescribeVaultInputVaultExistsWaitTypeDef,
     DescribeVaultInputVaultNotExistsWaitTypeDef,
     ListVaultsOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
-    SetVaultAccessPolicyInputRequestTypeDef,
     GetVaultNotificationsOutputTypeDef,
-    SetVaultNotificationsInputNotificationSetTypeDef,
-    SetVaultNotificationsInputRequestTypeDef,
+    GrantOutputTypeDef,
     GrantTypeDef,
     InitiateVaultLockInputRequestTypeDef,
     ListMultipartUploadsOutputTypeDef,
     ListPartsOutputTypeDef,
     ListProvisionedCapacityOutputTypeDef,
+    SetVaultAccessPolicyInputRequestTypeDef,
+    SetVaultNotificationsInputNotificationSetTypeDef,
+    SetVaultNotificationsInputRequestTypeDef,
+    SelectParametersOutputTypeDef,
     SelectParametersResponseMetadataTypeDef,
     SelectParametersTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     SetDataRetrievalPolicyInputRequestTypeDef,
+    S3LocationOutputTypeDef,
     S3LocationTypeDef,
+    OutputLocationOutputTypeDef,
     OutputLocationResponseMetadataTypeDef,
     OutputLocationTypeDef,
     GlacierJobDescriptionResponseMetadataTypeDef,
     GlacierJobDescriptionTypeDef,
     JobParametersTypeDef,
     ListJobsOutputTypeDef,
     InitiateJobInputRequestTypeDef,
```

### Comparing `mypy-boto3-glacier-1.28.0/mypy_boto3_glacier.egg-info/SOURCES.txt` & `mypy-boto3-glacier-1.28.12/mypy_boto3_glacier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glacier-1.28.0/setup.py` & `mypy-boto3-glacier-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-glacier",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_glacier"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Glacier 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Glacier 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

