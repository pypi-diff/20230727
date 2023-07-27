# Comparing `tmp/mypy-boto3-acm-pca-1.28.0.tar.gz` & `tmp/mypy-boto3-acm-pca-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-acm-pca-1.28.0.tar", last modified: Thu Jul  6 20:58:51 2023, max compression
+gzip compressed data, was "mypy-boto3-acm-pca-1.28.12.tar", last modified: Thu Jul 27 05:34:13 2023, max compression
```

## Comparing `mypy-boto3-acm-pca-1.28.0.tar` & `mypy-boto3-acm-pca-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.674206 mypy-boto3-acm-pca-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-07-06 20:58:51.670206 mypy-boto3-acm-pca-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15676 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.666206 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22345 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-07-06 20:32:34.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27299 2023-07-06 20:32:33.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.670206 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-07-06 20:58:51.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 20:58:51.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:51.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:51.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:51.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:58:51.000000 mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:51.674206 mypy-boto3-acm-pca-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-06 20:32:32.000000 mypy-boto3-acm-pca-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.844594 mypy-boto3-acm-pca-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-07-27 05:34:13.844594 mypy-boto3-acm-pca-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.824594 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22381 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22345 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32740 2023-07-27 05:16:55.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32687 2023-07-27 05:16:55.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.824594 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-07-27 05:34:13.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 05:34:13.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:13.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:13.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:13.844594 mypy-boto3-acm-pca-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-27 05:16:53.000000 mypy-boto3-acm-pca-1.28.12/setup.py
```

### Comparing `mypy-boto3-acm-pca-1.28.0/LICENSE` & `mypy-boto3-acm-pca-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.0/PKG-INFO` & `mypy-boto3-acm-pca-1.28.12/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-acm-pca
-Version: 1.28.0
-Summary: Type annotations for boto3.ACMPCA 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 acm-pca type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-acm-pca"></a>
 
 # mypy-boto3-acm-pca
 
 [![PyPI - mypy-boto3-acm-pca](https://img.shields.io/pypi/v/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-acm-pca?color=blue)](https://pypistats.org/packages/mypy-boto3-acm-pca)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm-pca)](https://pepy.tech/project/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,87 +345,101 @@
 ### Typed dictionaries
 
 `mypy_boto3_acm_pca.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_acm_pca.type_defs import (
+    CustomAttributeOutputTypeDef,
     CustomAttributeTypeDef,
+    AccessMethodOutputTypeDef,
     AccessMethodTypeDef,
     CreateCertificateAuthorityAuditReportRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreatePermissionRequestRequestTypeDef,
+    CrlConfigurationOutputTypeDef,
     CrlConfigurationTypeDef,
+    KeyUsageOutputTypeDef,
     KeyUsageTypeDef,
     CustomExtensionTypeDef,
     DeleteCertificateAuthorityRequestRequestTypeDef,
     DeletePermissionRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateAuthorityAuditReportRequestRequestTypeDef,
     DescribeCertificateAuthorityRequestRequestTypeDef,
+    EdiPartyNameOutputTypeDef,
     EdiPartyNameTypeDef,
     ExtendedKeyUsageTypeDef,
+    OtherNameOutputTypeDef,
     OtherNameTypeDef,
     GetCertificateAuthorityCertificateRequestRequestTypeDef,
     GetCertificateAuthorityCsrRequestRequestTypeDef,
     GetCertificateRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     ValidityTypeDef,
     PaginatorConfigTypeDef,
     ListCertificateAuthoritiesRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
+    OcspConfigurationOutputTypeDef,
     OcspConfigurationTypeDef,
     QualifierTypeDef,
     PutPolicyRequestRequestTypeDef,
     RestoreCertificateAuthorityRequestRequestTypeDef,
     RevokeCertificateRequestRequestTypeDef,
+    ASN1SubjectOutputTypeDef,
     ASN1SubjectTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
     GetCertificateResponseTypeDef,
     GetPolicyResponseTypeDef,
     IssueCertificateResponseTypeDef,
-    ListTagsResponseTypeDef,
     TagCertificateAuthorityRequestRequestTypeDef,
     UntagCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
     GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
     GetCertificateRequestCertificateIssuedWaitTypeDef,
     ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListPermissionsResponseTypeDef,
+    ListTagsResponseTypeDef,
+    RevocationConfigurationOutputTypeDef,
     RevocationConfigurationTypeDef,
     PolicyQualifierInfoTypeDef,
+    GeneralNameOutputTypeDef,
     GeneralNameTypeDef,
     UpdateCertificateAuthorityRequestRequestTypeDef,
     PolicyInformationTypeDef,
+    AccessDescriptionOutputTypeDef,
     AccessDescriptionTypeDef,
     ExtensionsTypeDef,
+    CsrExtensionsOutputTypeDef,
     CsrExtensionsTypeDef,
     ApiPassthroughTypeDef,
+    CertificateAuthorityConfigurationOutputTypeDef,
     CertificateAuthorityConfigurationTypeDef,
     IssueCertificateRequestRequestTypeDef,
     CertificateAuthorityTypeDef,
     CreateCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     ListCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> CustomAttributeTypeDef:
+def get_structure() -> CustomAttributeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-acm-pca-1.28.0/README.md` & `mypy-boto3-acm-pca-1.28.12/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-acm-pca
+Version: 1.28.12
+Summary: Type annotations for boto3.ACMPCA 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 acm-pca type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-acm-pca"></a>
 
 # mypy-boto3-acm-pca
 
 [![PyPI - mypy-boto3-acm-pca](https://img.shields.io/pypi/v/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-acm-pca?color=blue)](https://pypistats.org/packages/mypy-boto3-acm-pca)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm-pca)](https://pepy.tech/project/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,87 +377,101 @@
 ### Typed dictionaries
 
 `mypy_boto3_acm_pca.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_acm_pca.type_defs import (
+    CustomAttributeOutputTypeDef,
     CustomAttributeTypeDef,
+    AccessMethodOutputTypeDef,
     AccessMethodTypeDef,
     CreateCertificateAuthorityAuditReportRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreatePermissionRequestRequestTypeDef,
+    CrlConfigurationOutputTypeDef,
     CrlConfigurationTypeDef,
+    KeyUsageOutputTypeDef,
     KeyUsageTypeDef,
     CustomExtensionTypeDef,
     DeleteCertificateAuthorityRequestRequestTypeDef,
     DeletePermissionRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateAuthorityAuditReportRequestRequestTypeDef,
     DescribeCertificateAuthorityRequestRequestTypeDef,
+    EdiPartyNameOutputTypeDef,
     EdiPartyNameTypeDef,
     ExtendedKeyUsageTypeDef,
+    OtherNameOutputTypeDef,
     OtherNameTypeDef,
     GetCertificateAuthorityCertificateRequestRequestTypeDef,
     GetCertificateAuthorityCsrRequestRequestTypeDef,
     GetCertificateRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     ValidityTypeDef,
     PaginatorConfigTypeDef,
     ListCertificateAuthoritiesRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
+    OcspConfigurationOutputTypeDef,
     OcspConfigurationTypeDef,
     QualifierTypeDef,
     PutPolicyRequestRequestTypeDef,
     RestoreCertificateAuthorityRequestRequestTypeDef,
     RevokeCertificateRequestRequestTypeDef,
+    ASN1SubjectOutputTypeDef,
     ASN1SubjectTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
     GetCertificateResponseTypeDef,
     GetPolicyResponseTypeDef,
     IssueCertificateResponseTypeDef,
-    ListTagsResponseTypeDef,
     TagCertificateAuthorityRequestRequestTypeDef,
     UntagCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
     GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
     GetCertificateRequestCertificateIssuedWaitTypeDef,
     ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListPermissionsResponseTypeDef,
+    ListTagsResponseTypeDef,
+    RevocationConfigurationOutputTypeDef,
     RevocationConfigurationTypeDef,
     PolicyQualifierInfoTypeDef,
+    GeneralNameOutputTypeDef,
     GeneralNameTypeDef,
     UpdateCertificateAuthorityRequestRequestTypeDef,
     PolicyInformationTypeDef,
+    AccessDescriptionOutputTypeDef,
     AccessDescriptionTypeDef,
     ExtensionsTypeDef,
+    CsrExtensionsOutputTypeDef,
     CsrExtensionsTypeDef,
     ApiPassthroughTypeDef,
+    CertificateAuthorityConfigurationOutputTypeDef,
     CertificateAuthorityConfigurationTypeDef,
     IssueCertificateRequestRequestTypeDef,
     CertificateAuthorityTypeDef,
     CreateCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     ListCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> CustomAttributeTypeDef:
+def get_structure() -> CustomAttributeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/__init__.py` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/__init__.pyi` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/__main__.py` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ACMPCA 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ACMPCA 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA\nOther"
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

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/client.py` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/client.pyi` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/literals.py` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,15 @@
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
@@ -307,26 +308,28 @@
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

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/literals.pyi` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,15 @@
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
@@ -305,26 +306,28 @@
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

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/paginator.py` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/paginator.pyi` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/type_defs.py` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/type_defs.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for acm-pca service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_acm_pca.type_defs import CustomAttributeTypeDef
+    from mypy_boto3_acm_pca.type_defs import CustomAttributeOutputTypeDef
 
-    data: CustomAttributeTypeDef = {...}
+    data: CustomAttributeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -41,95 +41,125 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "CustomAttributeOutputTypeDef",
     "CustomAttributeTypeDef",
+    "AccessMethodOutputTypeDef",
     "AccessMethodTypeDef",
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreatePermissionRequestRequestTypeDef",
+    "CrlConfigurationOutputTypeDef",
     "CrlConfigurationTypeDef",
+    "KeyUsageOutputTypeDef",
     "KeyUsageTypeDef",
     "CustomExtensionTypeDef",
     "DeleteCertificateAuthorityRequestRequestTypeDef",
     "DeletePermissionRequestRequestTypeDef",
     "DeletePolicyRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCertificateAuthorityAuditReportRequestRequestTypeDef",
     "DescribeCertificateAuthorityRequestRequestTypeDef",
+    "EdiPartyNameOutputTypeDef",
     "EdiPartyNameTypeDef",
     "ExtendedKeyUsageTypeDef",
+    "OtherNameOutputTypeDef",
     "OtherNameTypeDef",
     "GetCertificateAuthorityCertificateRequestRequestTypeDef",
     "GetCertificateAuthorityCsrRequestRequestTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "ValidityTypeDef",
     "PaginatorConfigTypeDef",
     "ListCertificateAuthoritiesRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "OcspConfigurationOutputTypeDef",
     "OcspConfigurationTypeDef",
     "QualifierTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "RestoreCertificateAuthorityRequestRequestTypeDef",
     "RevokeCertificateRequestRequestTypeDef",
+    "ASN1SubjectOutputTypeDef",
     "ASN1SubjectTypeDef",
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     "CreateCertificateAuthorityResponseTypeDef",
     "DescribeCertificateAuthorityAuditReportResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCertificateAuthorityCertificateResponseTypeDef",
     "GetCertificateAuthorityCsrResponseTypeDef",
     "GetCertificateResponseTypeDef",
     "GetPolicyResponseTypeDef",
     "IssueCertificateResponseTypeDef",
-    "ListTagsResponseTypeDef",
     "TagCertificateAuthorityRequestRequestTypeDef",
     "UntagCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef",
     "GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     "GetCertificateRequestCertificateIssuedWaitTypeDef",
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListPermissionsResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "RevocationConfigurationOutputTypeDef",
     "RevocationConfigurationTypeDef",
     "PolicyQualifierInfoTypeDef",
+    "GeneralNameOutputTypeDef",
     "GeneralNameTypeDef",
     "UpdateCertificateAuthorityRequestRequestTypeDef",
     "PolicyInformationTypeDef",
+    "AccessDescriptionOutputTypeDef",
     "AccessDescriptionTypeDef",
     "ExtensionsTypeDef",
+    "CsrExtensionsOutputTypeDef",
     "CsrExtensionsTypeDef",
     "ApiPassthroughTypeDef",
+    "CertificateAuthorityConfigurationOutputTypeDef",
     "CertificateAuthorityConfigurationTypeDef",
     "IssueCertificateRequestRequestTypeDef",
     "CertificateAuthorityTypeDef",
     "CreateCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityResponseTypeDef",
     "ListCertificateAuthoritiesResponseTypeDef",
 )
 
+CustomAttributeOutputTypeDef = TypedDict(
+    "CustomAttributeOutputTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "Value": str,
+    },
+)
+
 CustomAttributeTypeDef = TypedDict(
     "CustomAttributeTypeDef",
     {
         "ObjectIdentifier": str,
         "Value": str,
     },
 )
 
+AccessMethodOutputTypeDef = TypedDict(
+    "AccessMethodOutputTypeDef",
+    {
+        "CustomObjectIdentifier": str,
+        "AccessMethodType": AccessMethodTypeType,
+    },
+    total=False,
+)
+
 AccessMethodTypeDef = TypedDict(
     "AccessMethodTypeDef",
     {
         "CustomObjectIdentifier": str,
         "AccessMethodType": AccessMethodTypeType,
     },
     total=False,
@@ -165,19 +195,17 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 _RequiredCreatePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePermissionRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Principal": str,
         "Actions": Sequence[ActionTypeType],
     },
@@ -186,20 +214,40 @@
     "_OptionalCreatePermissionRequestRequestTypeDef",
     {
         "SourceAccount": str,
     },
     total=False,
 )
 
-
 class CreatePermissionRequestRequestTypeDef(
     _RequiredCreatePermissionRequestRequestTypeDef, _OptionalCreatePermissionRequestRequestTypeDef
 ):
     pass
 
+_RequiredCrlConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCrlConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalCrlConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCrlConfigurationOutputTypeDef",
+    {
+        "ExpirationInDays": int,
+        "CustomCname": str,
+        "S3BucketName": str,
+        "S3ObjectAcl": S3ObjectAclType,
+    },
+    total=False,
+)
+
+class CrlConfigurationOutputTypeDef(
+    _RequiredCrlConfigurationOutputTypeDef, _OptionalCrlConfigurationOutputTypeDef
+):
+    pass
 
 _RequiredCrlConfigurationTypeDef = TypedDict(
     "_RequiredCrlConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
@@ -210,18 +258,32 @@
         "CustomCname": str,
         "S3BucketName": str,
         "S3ObjectAcl": S3ObjectAclType,
     },
     total=False,
 )
 
-
 class CrlConfigurationTypeDef(_RequiredCrlConfigurationTypeDef, _OptionalCrlConfigurationTypeDef):
     pass
 
+KeyUsageOutputTypeDef = TypedDict(
+    "KeyUsageOutputTypeDef",
+    {
+        "DigitalSignature": bool,
+        "NonRepudiation": bool,
+        "KeyEncipherment": bool,
+        "DataEncipherment": bool,
+        "KeyAgreement": bool,
+        "KeyCertSign": bool,
+        "CRLSign": bool,
+        "EncipherOnly": bool,
+        "DecipherOnly": bool,
+    },
+    total=False,
+)
 
 KeyUsageTypeDef = TypedDict(
     "KeyUsageTypeDef",
     {
         "DigitalSignature": bool,
         "NonRepudiation": bool,
         "KeyEncipherment": bool,
@@ -246,41 +308,37 @@
     "_OptionalCustomExtensionTypeDef",
     {
         "Critical": bool,
     },
     total=False,
 )
 
-
 class CustomExtensionTypeDef(_RequiredCustomExtensionTypeDef, _OptionalCustomExtensionTypeDef):
     pass
 
-
 _RequiredDeleteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 _OptionalDeleteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteCertificateAuthorityRequestRequestTypeDef",
     {
         "PermanentDeletionTimeInDays": int,
     },
     total=False,
 )
 
-
 class DeleteCertificateAuthorityRequestRequestTypeDef(
     _RequiredDeleteCertificateAuthorityRequestRequestTypeDef,
     _OptionalDeleteCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeletePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePermissionRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Principal": str,
     },
 )
@@ -288,21 +346,19 @@
     "_OptionalDeletePermissionRequestRequestTypeDef",
     {
         "SourceAccount": str,
     },
     total=False,
 )
 
-
 class DeletePermissionRequestRequestTypeDef(
     _RequiredDeletePermissionRequestRequestTypeDef, _OptionalDeletePermissionRequestRequestTypeDef
 ):
     pass
 
-
 DeletePolicyRequestRequestTypeDef = TypedDict(
     "DeletePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -326,42 +382,67 @@
 DescribeCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "DescribeCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 
+_RequiredEdiPartyNameOutputTypeDef = TypedDict(
+    "_RequiredEdiPartyNameOutputTypeDef",
+    {
+        "PartyName": str,
+    },
+)
+_OptionalEdiPartyNameOutputTypeDef = TypedDict(
+    "_OptionalEdiPartyNameOutputTypeDef",
+    {
+        "NameAssigner": str,
+    },
+    total=False,
+)
+
+class EdiPartyNameOutputTypeDef(
+    _RequiredEdiPartyNameOutputTypeDef, _OptionalEdiPartyNameOutputTypeDef
+):
+    pass
+
 _RequiredEdiPartyNameTypeDef = TypedDict(
     "_RequiredEdiPartyNameTypeDef",
     {
         "PartyName": str,
     },
 )
 _OptionalEdiPartyNameTypeDef = TypedDict(
     "_OptionalEdiPartyNameTypeDef",
     {
         "NameAssigner": str,
     },
     total=False,
 )
 
-
 class EdiPartyNameTypeDef(_RequiredEdiPartyNameTypeDef, _OptionalEdiPartyNameTypeDef):
     pass
 
-
 ExtendedKeyUsageTypeDef = TypedDict(
     "ExtendedKeyUsageTypeDef",
     {
         "ExtendedKeyUsageType": ExtendedKeyUsageTypeType,
         "ExtendedKeyUsageObjectIdentifier": str,
     },
     total=False,
 )
 
+OtherNameOutputTypeDef = TypedDict(
+    "OtherNameOutputTypeDef",
+    {
+        "TypeId": str,
+        "Value": str,
+    },
+)
+
 OtherNameTypeDef = TypedDict(
     "OtherNameTypeDef",
     {
         "TypeId": str,
         "Value": str,
     },
 )
@@ -406,22 +487,20 @@
     "_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef",
     {
         "CertificateChain": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-
 class ImportCertificateAuthorityCertificateRequestRequestTypeDef(
     _RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef,
     _OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef,
 ):
     pass
 
-
 ValidityTypeDef = TypedDict(
     "ValidityTypeDef",
     {
         "Value": int,
         "Type": ValidityPeriodTypeType,
     },
 )
@@ -457,21 +536,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListPermissionsRequestRequestTypeDef(
     _RequiredListPermissionsRequestRequestTypeDef, _OptionalListPermissionsRequestRequestTypeDef
 ):
     pass
 
-
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CreatedAt": datetime,
         "Principal": str,
         "SourceAccount": str,
@@ -492,20 +569,54 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+_RequiredOcspConfigurationOutputTypeDef = TypedDict(
+    "_RequiredOcspConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalOcspConfigurationOutputTypeDef = TypedDict(
+    "_OptionalOcspConfigurationOutputTypeDef",
+    {
+        "OcspCustomCname": str,
+    },
+    total=False,
+)
+
+class OcspConfigurationOutputTypeDef(
+    _RequiredOcspConfigurationOutputTypeDef, _OptionalOcspConfigurationOutputTypeDef
+):
+    pass
 
 _RequiredOcspConfigurationTypeDef = TypedDict(
     "_RequiredOcspConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
@@ -513,21 +624,19 @@
     "_OptionalOcspConfigurationTypeDef",
     {
         "OcspCustomCname": str,
     },
     total=False,
 )
 
-
 class OcspConfigurationTypeDef(
     _RequiredOcspConfigurationTypeDef, _OptionalOcspConfigurationTypeDef
 ):
     pass
 
-
 QualifierTypeDef = TypedDict(
     "QualifierTypeDef",
     {
         "CpsUri": str,
     },
 )
 
@@ -551,14 +660,36 @@
     {
         "CertificateAuthorityArn": str,
         "CertificateSerial": str,
         "RevocationReason": RevocationReasonType,
     },
 )
 
+ASN1SubjectOutputTypeDef = TypedDict(
+    "ASN1SubjectOutputTypeDef",
+    {
+        "Country": str,
+        "Organization": str,
+        "OrganizationalUnit": str,
+        "DistinguishedNameQualifier": str,
+        "State": str,
+        "CommonName": str,
+        "SerialNumber": str,
+        "Locality": str,
+        "Title": str,
+        "Surname": str,
+        "GivenName": str,
+        "Initials": str,
+        "Pseudonym": str,
+        "GenerationQualifier": str,
+        "CustomAttributes": List[CustomAttributeOutputTypeDef],
+    },
+    total=False,
+)
+
 ASN1SubjectTypeDef = TypedDict(
     "ASN1SubjectTypeDef",
     {
         "Country": str,
         "Organization": str,
         "OrganizationalUnit": str,
         "DistinguishedNameQualifier": str,
@@ -650,23 +781,14 @@
     "IssueCertificateResponseTypeDef",
     {
         "CertificateArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TagCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "TagCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -690,44 +812,40 @@
     "_OptionalDescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef(
     _RequiredDescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
     _OptionalDescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef = TypedDict(
     "_RequiredGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 _OptionalGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef = TypedDict(
     "_OptionalGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef(
     _RequiredGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
     _OptionalGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetCertificateRequestCertificateIssuedWaitTypeDef = TypedDict(
     "_RequiredGetCertificateRequestCertificateIssuedWaitTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CertificateArn": str,
     },
 )
@@ -735,22 +853,20 @@
     "_OptionalGetCertificateRequestCertificateIssuedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetCertificateRequestCertificateIssuedWaitTypeDef(
     _RequiredGetCertificateRequestCertificateIssuedWaitTypeDef,
     _OptionalGetCertificateRequestCertificateIssuedWaitTypeDef,
 ):
     pass
 
-
 ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef = TypedDict(
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     {
         "ResourceOwner": ResourceOwnerType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -766,52 +882,66 @@
     "_OptionalListPermissionsRequestListPermissionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListPermissionsRequestListPermissionsPaginateTypeDef(
     _RequiredListPermissionsRequestListPermissionsPaginateTypeDef,
     _OptionalListPermissionsRequestListPermissionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_RequiredListTagsRequestListTagsPaginateTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 _OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_OptionalListTagsRequestListTagsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTagsRequestListTagsPaginateTypeDef(
     _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
 ):
     pass
 
-
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "Permissions": List[PermissionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RevocationConfigurationOutputTypeDef = TypedDict(
+    "RevocationConfigurationOutputTypeDef",
+    {
+        "CrlConfiguration": CrlConfigurationOutputTypeDef,
+        "OcspConfiguration": OcspConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 RevocationConfigurationTypeDef = TypedDict(
     "RevocationConfigurationTypeDef",
     {
         "CrlConfiguration": CrlConfigurationTypeDef,
         "OcspConfiguration": OcspConfigurationTypeDef,
     },
     total=False,
@@ -821,14 +951,29 @@
     "PolicyQualifierInfoTypeDef",
     {
         "PolicyQualifierId": Literal["CPS"],
         "Qualifier": QualifierTypeDef,
     },
 )
 
+GeneralNameOutputTypeDef = TypedDict(
+    "GeneralNameOutputTypeDef",
+    {
+        "OtherName": OtherNameOutputTypeDef,
+        "Rfc822Name": str,
+        "DnsName": str,
+        "DirectoryName": ASN1SubjectOutputTypeDef,
+        "EdiPartyName": EdiPartyNameOutputTypeDef,
+        "UniformResourceIdentifier": str,
+        "IpAddress": str,
+        "RegisteredId": str,
+    },
+    total=False,
+)
+
 GeneralNameTypeDef = TypedDict(
     "GeneralNameTypeDef",
     {
         "OtherName": OtherNameTypeDef,
         "Rfc822Name": str,
         "DnsName": str,
         "DirectoryName": ASN1SubjectTypeDef,
@@ -851,42 +996,46 @@
     {
         "RevocationConfiguration": RevocationConfigurationTypeDef,
         "Status": CertificateAuthorityStatusType,
     },
     total=False,
 )
 
-
 class UpdateCertificateAuthorityRequestRequestTypeDef(
     _RequiredUpdateCertificateAuthorityRequestRequestTypeDef,
     _OptionalUpdateCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPolicyInformationTypeDef = TypedDict(
     "_RequiredPolicyInformationTypeDef",
     {
         "CertPolicyId": str,
     },
 )
 _OptionalPolicyInformationTypeDef = TypedDict(
     "_OptionalPolicyInformationTypeDef",
     {
         "PolicyQualifiers": Sequence[PolicyQualifierInfoTypeDef],
     },
     total=False,
 )
 
-
 class PolicyInformationTypeDef(
     _RequiredPolicyInformationTypeDef, _OptionalPolicyInformationTypeDef
 ):
     pass
 
+AccessDescriptionOutputTypeDef = TypedDict(
+    "AccessDescriptionOutputTypeDef",
+    {
+        "AccessMethod": AccessMethodOutputTypeDef,
+        "AccessLocation": GeneralNameOutputTypeDef,
+    },
+)
 
 AccessDescriptionTypeDef = TypedDict(
     "AccessDescriptionTypeDef",
     {
         "AccessMethod": AccessMethodTypeDef,
         "AccessLocation": GeneralNameTypeDef,
     },
@@ -900,14 +1049,23 @@
         "KeyUsage": KeyUsageTypeDef,
         "SubjectAlternativeNames": Sequence[GeneralNameTypeDef],
         "CustomExtensions": Sequence[CustomExtensionTypeDef],
     },
     total=False,
 )
 
+CsrExtensionsOutputTypeDef = TypedDict(
+    "CsrExtensionsOutputTypeDef",
+    {
+        "KeyUsage": KeyUsageOutputTypeDef,
+        "SubjectInformationAccess": List[AccessDescriptionOutputTypeDef],
+    },
+    total=False,
+)
+
 CsrExtensionsTypeDef = TypedDict(
     "CsrExtensionsTypeDef",
     {
         "KeyUsage": KeyUsageTypeDef,
         "SubjectInformationAccess": Sequence[AccessDescriptionTypeDef],
     },
     total=False,
@@ -918,14 +1076,36 @@
     {
         "Extensions": ExtensionsTypeDef,
         "Subject": ASN1SubjectTypeDef,
     },
     total=False,
 )
 
+_RequiredCertificateAuthorityConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCertificateAuthorityConfigurationOutputTypeDef",
+    {
+        "KeyAlgorithm": KeyAlgorithmType,
+        "SigningAlgorithm": SigningAlgorithmType,
+        "Subject": ASN1SubjectOutputTypeDef,
+    },
+)
+_OptionalCertificateAuthorityConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCertificateAuthorityConfigurationOutputTypeDef",
+    {
+        "CsrExtensions": CsrExtensionsOutputTypeDef,
+    },
+    total=False,
+)
+
+class CertificateAuthorityConfigurationOutputTypeDef(
+    _RequiredCertificateAuthorityConfigurationOutputTypeDef,
+    _OptionalCertificateAuthorityConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredCertificateAuthorityConfigurationTypeDef = TypedDict(
     "_RequiredCertificateAuthorityConfigurationTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "SigningAlgorithm": SigningAlgorithmType,
         "Subject": ASN1SubjectTypeDef,
     },
@@ -934,22 +1114,20 @@
     "_OptionalCertificateAuthorityConfigurationTypeDef",
     {
         "CsrExtensions": CsrExtensionsTypeDef,
     },
     total=False,
 )
 
-
 class CertificateAuthorityConfigurationTypeDef(
     _RequiredCertificateAuthorityConfigurationTypeDef,
     _OptionalCertificateAuthorityConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredIssueCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredIssueCertificateRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Csr": Union[str, bytes, IO[Any], StreamingBody],
         "SigningAlgorithm": SigningAlgorithmType,
         "Validity": ValidityTypeDef,
@@ -962,36 +1140,34 @@
         "TemplateArn": str,
         "ValidityNotBefore": ValidityTypeDef,
         "IdempotencyToken": str,
     },
     total=False,
 )
 
-
 class IssueCertificateRequestRequestTypeDef(
     _RequiredIssueCertificateRequestRequestTypeDef, _OptionalIssueCertificateRequestRequestTypeDef
 ):
     pass
 
-
 CertificateAuthorityTypeDef = TypedDict(
     "CertificateAuthorityTypeDef",
     {
         "Arn": str,
         "OwnerAccount": str,
         "CreatedAt": datetime,
         "LastStateChangeAt": datetime,
         "Type": CertificateAuthorityTypeType,
         "Serial": str,
         "Status": CertificateAuthorityStatusType,
         "NotBefore": datetime,
         "NotAfter": datetime,
         "FailureReason": FailureReasonType,
-        "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
-        "RevocationConfiguration": RevocationConfigurationTypeDef,
+        "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationOutputTypeDef,
+        "RevocationConfiguration": RevocationConfigurationOutputTypeDef,
         "RestorableUntil": datetime,
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
 
@@ -1010,22 +1186,20 @@
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "Tags": Sequence[TagTypeDef],
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
 
-
 class CreateCertificateAuthorityRequestRequestTypeDef(
     _RequiredCreateCertificateAuthorityRequestRequestTypeDef,
     _OptionalCreateCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeCertificateAuthorityResponseTypeDef = TypedDict(
     "DescribeCertificateAuthorityResponseTypeDef",
     {
         "CertificateAuthority": CertificateAuthorityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/type_defs.pyi` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/type_defs.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for acm-pca service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_acm_pca.type_defs import CustomAttributeTypeDef
+    from mypy_boto3_acm_pca.type_defs import CustomAttributeOutputTypeDef
 
-    data: CustomAttributeTypeDef = {...}
+    data: CustomAttributeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -41,94 +41,126 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "CustomAttributeOutputTypeDef",
     "CustomAttributeTypeDef",
+    "AccessMethodOutputTypeDef",
     "AccessMethodTypeDef",
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreatePermissionRequestRequestTypeDef",
+    "CrlConfigurationOutputTypeDef",
     "CrlConfigurationTypeDef",
+    "KeyUsageOutputTypeDef",
     "KeyUsageTypeDef",
     "CustomExtensionTypeDef",
     "DeleteCertificateAuthorityRequestRequestTypeDef",
     "DeletePermissionRequestRequestTypeDef",
     "DeletePolicyRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCertificateAuthorityAuditReportRequestRequestTypeDef",
     "DescribeCertificateAuthorityRequestRequestTypeDef",
+    "EdiPartyNameOutputTypeDef",
     "EdiPartyNameTypeDef",
     "ExtendedKeyUsageTypeDef",
+    "OtherNameOutputTypeDef",
     "OtherNameTypeDef",
     "GetCertificateAuthorityCertificateRequestRequestTypeDef",
     "GetCertificateAuthorityCsrRequestRequestTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "ValidityTypeDef",
     "PaginatorConfigTypeDef",
     "ListCertificateAuthoritiesRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "OcspConfigurationOutputTypeDef",
     "OcspConfigurationTypeDef",
     "QualifierTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "RestoreCertificateAuthorityRequestRequestTypeDef",
     "RevokeCertificateRequestRequestTypeDef",
+    "ASN1SubjectOutputTypeDef",
     "ASN1SubjectTypeDef",
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     "CreateCertificateAuthorityResponseTypeDef",
     "DescribeCertificateAuthorityAuditReportResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCertificateAuthorityCertificateResponseTypeDef",
     "GetCertificateAuthorityCsrResponseTypeDef",
     "GetCertificateResponseTypeDef",
     "GetPolicyResponseTypeDef",
     "IssueCertificateResponseTypeDef",
-    "ListTagsResponseTypeDef",
     "TagCertificateAuthorityRequestRequestTypeDef",
     "UntagCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef",
     "GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     "GetCertificateRequestCertificateIssuedWaitTypeDef",
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListPermissionsResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "RevocationConfigurationOutputTypeDef",
     "RevocationConfigurationTypeDef",
     "PolicyQualifierInfoTypeDef",
+    "GeneralNameOutputTypeDef",
     "GeneralNameTypeDef",
     "UpdateCertificateAuthorityRequestRequestTypeDef",
     "PolicyInformationTypeDef",
+    "AccessDescriptionOutputTypeDef",
     "AccessDescriptionTypeDef",
     "ExtensionsTypeDef",
+    "CsrExtensionsOutputTypeDef",
     "CsrExtensionsTypeDef",
     "ApiPassthroughTypeDef",
+    "CertificateAuthorityConfigurationOutputTypeDef",
     "CertificateAuthorityConfigurationTypeDef",
     "IssueCertificateRequestRequestTypeDef",
     "CertificateAuthorityTypeDef",
     "CreateCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityResponseTypeDef",
     "ListCertificateAuthoritiesResponseTypeDef",
 )
 
+CustomAttributeOutputTypeDef = TypedDict(
+    "CustomAttributeOutputTypeDef",
+    {
+        "ObjectIdentifier": str,
+        "Value": str,
+    },
+)
+
 CustomAttributeTypeDef = TypedDict(
     "CustomAttributeTypeDef",
     {
         "ObjectIdentifier": str,
         "Value": str,
     },
 )
 
+AccessMethodOutputTypeDef = TypedDict(
+    "AccessMethodOutputTypeDef",
+    {
+        "CustomObjectIdentifier": str,
+        "AccessMethodType": AccessMethodTypeType,
+    },
+    total=False,
+)
+
 AccessMethodTypeDef = TypedDict(
     "AccessMethodTypeDef",
     {
         "CustomObjectIdentifier": str,
         "AccessMethodType": AccessMethodTypeType,
     },
     total=False,
@@ -164,17 +196,19 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 _RequiredCreatePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePermissionRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Principal": str,
         "Actions": Sequence[ActionTypeType],
     },
@@ -183,19 +217,45 @@
     "_OptionalCreatePermissionRequestRequestTypeDef",
     {
         "SourceAccount": str,
     },
     total=False,
 )
 
+
 class CreatePermissionRequestRequestTypeDef(
     _RequiredCreatePermissionRequestRequestTypeDef, _OptionalCreatePermissionRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredCrlConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCrlConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalCrlConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCrlConfigurationOutputTypeDef",
+    {
+        "ExpirationInDays": int,
+        "CustomCname": str,
+        "S3BucketName": str,
+        "S3ObjectAcl": S3ObjectAclType,
+    },
+    total=False,
+)
+
+
+class CrlConfigurationOutputTypeDef(
+    _RequiredCrlConfigurationOutputTypeDef, _OptionalCrlConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredCrlConfigurationTypeDef = TypedDict(
     "_RequiredCrlConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCrlConfigurationTypeDef = TypedDict(
@@ -205,17 +265,35 @@
         "CustomCname": str,
         "S3BucketName": str,
         "S3ObjectAcl": S3ObjectAclType,
     },
     total=False,
 )
 
+
 class CrlConfigurationTypeDef(_RequiredCrlConfigurationTypeDef, _OptionalCrlConfigurationTypeDef):
     pass
 
+
+KeyUsageOutputTypeDef = TypedDict(
+    "KeyUsageOutputTypeDef",
+    {
+        "DigitalSignature": bool,
+        "NonRepudiation": bool,
+        "KeyEncipherment": bool,
+        "DataEncipherment": bool,
+        "KeyAgreement": bool,
+        "KeyCertSign": bool,
+        "CRLSign": bool,
+        "EncipherOnly": bool,
+        "DecipherOnly": bool,
+    },
+    total=False,
+)
+
 KeyUsageTypeDef = TypedDict(
     "KeyUsageTypeDef",
     {
         "DigitalSignature": bool,
         "NonRepudiation": bool,
         "KeyEncipherment": bool,
         "DataEncipherment": bool,
@@ -239,37 +317,41 @@
     "_OptionalCustomExtensionTypeDef",
     {
         "Critical": bool,
     },
     total=False,
 )
 
+
 class CustomExtensionTypeDef(_RequiredCustomExtensionTypeDef, _OptionalCustomExtensionTypeDef):
     pass
 
+
 _RequiredDeleteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 _OptionalDeleteCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteCertificateAuthorityRequestRequestTypeDef",
     {
         "PermanentDeletionTimeInDays": int,
     },
     total=False,
 )
 
+
 class DeleteCertificateAuthorityRequestRequestTypeDef(
     _RequiredDeleteCertificateAuthorityRequestRequestTypeDef,
     _OptionalDeleteCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeletePermissionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePermissionRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Principal": str,
     },
 )
@@ -277,19 +359,21 @@
     "_OptionalDeletePermissionRequestRequestTypeDef",
     {
         "SourceAccount": str,
     },
     total=False,
 )
 
+
 class DeletePermissionRequestRequestTypeDef(
     _RequiredDeletePermissionRequestRequestTypeDef, _OptionalDeletePermissionRequestRequestTypeDef
 ):
     pass
 
+
 DeletePolicyRequestRequestTypeDef = TypedDict(
     "DeletePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -313,40 +397,71 @@
 DescribeCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "DescribeCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 
+_RequiredEdiPartyNameOutputTypeDef = TypedDict(
+    "_RequiredEdiPartyNameOutputTypeDef",
+    {
+        "PartyName": str,
+    },
+)
+_OptionalEdiPartyNameOutputTypeDef = TypedDict(
+    "_OptionalEdiPartyNameOutputTypeDef",
+    {
+        "NameAssigner": str,
+    },
+    total=False,
+)
+
+
+class EdiPartyNameOutputTypeDef(
+    _RequiredEdiPartyNameOutputTypeDef, _OptionalEdiPartyNameOutputTypeDef
+):
+    pass
+
+
 _RequiredEdiPartyNameTypeDef = TypedDict(
     "_RequiredEdiPartyNameTypeDef",
     {
         "PartyName": str,
     },
 )
 _OptionalEdiPartyNameTypeDef = TypedDict(
     "_OptionalEdiPartyNameTypeDef",
     {
         "NameAssigner": str,
     },
     total=False,
 )
 
+
 class EdiPartyNameTypeDef(_RequiredEdiPartyNameTypeDef, _OptionalEdiPartyNameTypeDef):
     pass
 
+
 ExtendedKeyUsageTypeDef = TypedDict(
     "ExtendedKeyUsageTypeDef",
     {
         "ExtendedKeyUsageType": ExtendedKeyUsageTypeType,
         "ExtendedKeyUsageObjectIdentifier": str,
     },
     total=False,
 )
 
+OtherNameOutputTypeDef = TypedDict(
+    "OtherNameOutputTypeDef",
+    {
+        "TypeId": str,
+        "Value": str,
+    },
+)
+
 OtherNameTypeDef = TypedDict(
     "OtherNameTypeDef",
     {
         "TypeId": str,
         "Value": str,
     },
 )
@@ -391,20 +506,22 @@
     "_OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef",
     {
         "CertificateChain": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
+
 class ImportCertificateAuthorityCertificateRequestRequestTypeDef(
     _RequiredImportCertificateAuthorityCertificateRequestRequestTypeDef,
     _OptionalImportCertificateAuthorityCertificateRequestRequestTypeDef,
 ):
     pass
 
+
 ValidityTypeDef = TypedDict(
     "ValidityTypeDef",
     {
         "Value": int,
         "Type": ValidityPeriodTypeType,
     },
 )
@@ -440,19 +557,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListPermissionsRequestRequestTypeDef(
     _RequiredListPermissionsRequestRequestTypeDef, _OptionalListPermissionsRequestRequestTypeDef
 ):
     pass
 
+
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CreatedAt": datetime,
         "Principal": str,
         "SourceAccount": str,
@@ -473,38 +592,82 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+
+_RequiredOcspConfigurationOutputTypeDef = TypedDict(
+    "_RequiredOcspConfigurationOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalOcspConfigurationOutputTypeDef = TypedDict(
+    "_OptionalOcspConfigurationOutputTypeDef",
+    {
+        "OcspCustomCname": str,
+    },
+    total=False,
+)
+
+
+class OcspConfigurationOutputTypeDef(
+    _RequiredOcspConfigurationOutputTypeDef, _OptionalOcspConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredOcspConfigurationTypeDef = TypedDict(
     "_RequiredOcspConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalOcspConfigurationTypeDef = TypedDict(
     "_OptionalOcspConfigurationTypeDef",
     {
         "OcspCustomCname": str,
     },
     total=False,
 )
 
+
 class OcspConfigurationTypeDef(
     _RequiredOcspConfigurationTypeDef, _OptionalOcspConfigurationTypeDef
 ):
     pass
 
+
 QualifierTypeDef = TypedDict(
     "QualifierTypeDef",
     {
         "CpsUri": str,
     },
 )
 
@@ -528,14 +691,36 @@
     {
         "CertificateAuthorityArn": str,
         "CertificateSerial": str,
         "RevocationReason": RevocationReasonType,
     },
 )
 
+ASN1SubjectOutputTypeDef = TypedDict(
+    "ASN1SubjectOutputTypeDef",
+    {
+        "Country": str,
+        "Organization": str,
+        "OrganizationalUnit": str,
+        "DistinguishedNameQualifier": str,
+        "State": str,
+        "CommonName": str,
+        "SerialNumber": str,
+        "Locality": str,
+        "Title": str,
+        "Surname": str,
+        "GivenName": str,
+        "Initials": str,
+        "Pseudonym": str,
+        "GenerationQualifier": str,
+        "CustomAttributes": List[CustomAttributeOutputTypeDef],
+    },
+    total=False,
+)
+
 ASN1SubjectTypeDef = TypedDict(
     "ASN1SubjectTypeDef",
     {
         "Country": str,
         "Organization": str,
         "OrganizationalUnit": str,
         "DistinguishedNameQualifier": str,
@@ -627,23 +812,14 @@
     "IssueCertificateResponseTypeDef",
     {
         "CertificateArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TagCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "TagCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -667,40 +843,44 @@
     "_OptionalDescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef(
     _RequiredDescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
     _OptionalDescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef = TypedDict(
     "_RequiredGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 _OptionalGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef = TypedDict(
     "_OptionalGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef(
     _RequiredGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
     _OptionalGetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetCertificateRequestCertificateIssuedWaitTypeDef = TypedDict(
     "_RequiredGetCertificateRequestCertificateIssuedWaitTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CertificateArn": str,
     },
 )
@@ -708,20 +888,22 @@
     "_OptionalGetCertificateRequestCertificateIssuedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetCertificateRequestCertificateIssuedWaitTypeDef(
     _RequiredGetCertificateRequestCertificateIssuedWaitTypeDef,
     _OptionalGetCertificateRequestCertificateIssuedWaitTypeDef,
 ):
     pass
 
+
 ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef = TypedDict(
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     {
         "ResourceOwner": ResourceOwnerType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -737,48 +919,70 @@
     "_OptionalListPermissionsRequestListPermissionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListPermissionsRequestListPermissionsPaginateTypeDef(
     _RequiredListPermissionsRequestListPermissionsPaginateTypeDef,
     _OptionalListPermissionsRequestListPermissionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_RequiredListTagsRequestListTagsPaginateTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 _OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
     "_OptionalListTagsRequestListTagsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTagsRequestListTagsPaginateTypeDef(
     _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
 ):
     pass
 
+
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "Permissions": List[PermissionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RevocationConfigurationOutputTypeDef = TypedDict(
+    "RevocationConfigurationOutputTypeDef",
+    {
+        "CrlConfiguration": CrlConfigurationOutputTypeDef,
+        "OcspConfiguration": OcspConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 RevocationConfigurationTypeDef = TypedDict(
     "RevocationConfigurationTypeDef",
     {
         "CrlConfiguration": CrlConfigurationTypeDef,
         "OcspConfiguration": OcspConfigurationTypeDef,
     },
     total=False,
@@ -788,14 +992,29 @@
     "PolicyQualifierInfoTypeDef",
     {
         "PolicyQualifierId": Literal["CPS"],
         "Qualifier": QualifierTypeDef,
     },
 )
 
+GeneralNameOutputTypeDef = TypedDict(
+    "GeneralNameOutputTypeDef",
+    {
+        "OtherName": OtherNameOutputTypeDef,
+        "Rfc822Name": str,
+        "DnsName": str,
+        "DirectoryName": ASN1SubjectOutputTypeDef,
+        "EdiPartyName": EdiPartyNameOutputTypeDef,
+        "UniformResourceIdentifier": str,
+        "IpAddress": str,
+        "RegisteredId": str,
+    },
+    total=False,
+)
+
 GeneralNameTypeDef = TypedDict(
     "GeneralNameTypeDef",
     {
         "OtherName": OtherNameTypeDef,
         "Rfc822Name": str,
         "DnsName": str,
         "DirectoryName": ASN1SubjectTypeDef,
@@ -818,39 +1037,51 @@
     {
         "RevocationConfiguration": RevocationConfigurationTypeDef,
         "Status": CertificateAuthorityStatusType,
     },
     total=False,
 )
 
+
 class UpdateCertificateAuthorityRequestRequestTypeDef(
     _RequiredUpdateCertificateAuthorityRequestRequestTypeDef,
     _OptionalUpdateCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPolicyInformationTypeDef = TypedDict(
     "_RequiredPolicyInformationTypeDef",
     {
         "CertPolicyId": str,
     },
 )
 _OptionalPolicyInformationTypeDef = TypedDict(
     "_OptionalPolicyInformationTypeDef",
     {
         "PolicyQualifiers": Sequence[PolicyQualifierInfoTypeDef],
     },
     total=False,
 )
 
+
 class PolicyInformationTypeDef(
     _RequiredPolicyInformationTypeDef, _OptionalPolicyInformationTypeDef
 ):
     pass
 
+
+AccessDescriptionOutputTypeDef = TypedDict(
+    "AccessDescriptionOutputTypeDef",
+    {
+        "AccessMethod": AccessMethodOutputTypeDef,
+        "AccessLocation": GeneralNameOutputTypeDef,
+    },
+)
+
 AccessDescriptionTypeDef = TypedDict(
     "AccessDescriptionTypeDef",
     {
         "AccessMethod": AccessMethodTypeDef,
         "AccessLocation": GeneralNameTypeDef,
     },
 )
@@ -863,14 +1094,23 @@
         "KeyUsage": KeyUsageTypeDef,
         "SubjectAlternativeNames": Sequence[GeneralNameTypeDef],
         "CustomExtensions": Sequence[CustomExtensionTypeDef],
     },
     total=False,
 )
 
+CsrExtensionsOutputTypeDef = TypedDict(
+    "CsrExtensionsOutputTypeDef",
+    {
+        "KeyUsage": KeyUsageOutputTypeDef,
+        "SubjectInformationAccess": List[AccessDescriptionOutputTypeDef],
+    },
+    total=False,
+)
+
 CsrExtensionsTypeDef = TypedDict(
     "CsrExtensionsTypeDef",
     {
         "KeyUsage": KeyUsageTypeDef,
         "SubjectInformationAccess": Sequence[AccessDescriptionTypeDef],
     },
     total=False,
@@ -881,14 +1121,38 @@
     {
         "Extensions": ExtensionsTypeDef,
         "Subject": ASN1SubjectTypeDef,
     },
     total=False,
 )
 
+_RequiredCertificateAuthorityConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCertificateAuthorityConfigurationOutputTypeDef",
+    {
+        "KeyAlgorithm": KeyAlgorithmType,
+        "SigningAlgorithm": SigningAlgorithmType,
+        "Subject": ASN1SubjectOutputTypeDef,
+    },
+)
+_OptionalCertificateAuthorityConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCertificateAuthorityConfigurationOutputTypeDef",
+    {
+        "CsrExtensions": CsrExtensionsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CertificateAuthorityConfigurationOutputTypeDef(
+    _RequiredCertificateAuthorityConfigurationOutputTypeDef,
+    _OptionalCertificateAuthorityConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredCertificateAuthorityConfigurationTypeDef = TypedDict(
     "_RequiredCertificateAuthorityConfigurationTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "SigningAlgorithm": SigningAlgorithmType,
         "Subject": ASN1SubjectTypeDef,
     },
@@ -897,20 +1161,22 @@
     "_OptionalCertificateAuthorityConfigurationTypeDef",
     {
         "CsrExtensions": CsrExtensionsTypeDef,
     },
     total=False,
 )
 
+
 class CertificateAuthorityConfigurationTypeDef(
     _RequiredCertificateAuthorityConfigurationTypeDef,
     _OptionalCertificateAuthorityConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredIssueCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredIssueCertificateRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Csr": Union[str, bytes, IO[Any], StreamingBody],
         "SigningAlgorithm": SigningAlgorithmType,
         "Validity": ValidityTypeDef,
@@ -923,34 +1189,36 @@
         "TemplateArn": str,
         "ValidityNotBefore": ValidityTypeDef,
         "IdempotencyToken": str,
     },
     total=False,
 )
 
+
 class IssueCertificateRequestRequestTypeDef(
     _RequiredIssueCertificateRequestRequestTypeDef, _OptionalIssueCertificateRequestRequestTypeDef
 ):
     pass
 
+
 CertificateAuthorityTypeDef = TypedDict(
     "CertificateAuthorityTypeDef",
     {
         "Arn": str,
         "OwnerAccount": str,
         "CreatedAt": datetime,
         "LastStateChangeAt": datetime,
         "Type": CertificateAuthorityTypeType,
         "Serial": str,
         "Status": CertificateAuthorityStatusType,
         "NotBefore": datetime,
         "NotAfter": datetime,
         "FailureReason": FailureReasonType,
-        "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
-        "RevocationConfiguration": RevocationConfigurationTypeDef,
+        "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationOutputTypeDef,
+        "RevocationConfiguration": RevocationConfigurationOutputTypeDef,
         "RestorableUntil": datetime,
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
 
@@ -969,20 +1237,22 @@
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "Tags": Sequence[TagTypeDef],
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
 
+
 class CreateCertificateAuthorityRequestRequestTypeDef(
     _RequiredCreateCertificateAuthorityRequestRequestTypeDef,
     _OptionalCreateCertificateAuthorityRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeCertificateAuthorityResponseTypeDef = TypedDict(
     "DescribeCertificateAuthorityResponseTypeDef",
     {
         "CertificateAuthority": CertificateAuthorityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/waiter.py` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca/waiter.pyi` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca.egg-info/PKG-INFO` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm-pca
-Version: 1.28.0
-Summary: Type annotations for boto3.ACMPCA 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ACMPCA 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-acm-pca"></a>
 
 # mypy-boto3-acm-pca
 
 [![PyPI - mypy-boto3-acm-pca](https://img.shields.io/pypi/v/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-acm-pca?color=blue)](https://pypistats.org/packages/mypy-boto3-acm-pca)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm-pca)](https://pepy.tech/project/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,87 +377,101 @@
 ### Typed dictionaries
 
 `mypy_boto3_acm_pca.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_acm_pca.type_defs import (
+    CustomAttributeOutputTypeDef,
     CustomAttributeTypeDef,
+    AccessMethodOutputTypeDef,
     AccessMethodTypeDef,
     CreateCertificateAuthorityAuditReportRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreatePermissionRequestRequestTypeDef,
+    CrlConfigurationOutputTypeDef,
     CrlConfigurationTypeDef,
+    KeyUsageOutputTypeDef,
     KeyUsageTypeDef,
     CustomExtensionTypeDef,
     DeleteCertificateAuthorityRequestRequestTypeDef,
     DeletePermissionRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateAuthorityAuditReportRequestRequestTypeDef,
     DescribeCertificateAuthorityRequestRequestTypeDef,
+    EdiPartyNameOutputTypeDef,
     EdiPartyNameTypeDef,
     ExtendedKeyUsageTypeDef,
+    OtherNameOutputTypeDef,
     OtherNameTypeDef,
     GetCertificateAuthorityCertificateRequestRequestTypeDef,
     GetCertificateAuthorityCsrRequestRequestTypeDef,
     GetCertificateRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     ValidityTypeDef,
     PaginatorConfigTypeDef,
     ListCertificateAuthoritiesRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
+    OcspConfigurationOutputTypeDef,
     OcspConfigurationTypeDef,
     QualifierTypeDef,
     PutPolicyRequestRequestTypeDef,
     RestoreCertificateAuthorityRequestRequestTypeDef,
     RevokeCertificateRequestRequestTypeDef,
+    ASN1SubjectOutputTypeDef,
     ASN1SubjectTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
     GetCertificateResponseTypeDef,
     GetPolicyResponseTypeDef,
     IssueCertificateResponseTypeDef,
-    ListTagsResponseTypeDef,
     TagCertificateAuthorityRequestRequestTypeDef,
     UntagCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
     GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
     GetCertificateRequestCertificateIssuedWaitTypeDef,
     ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListPermissionsResponseTypeDef,
+    ListTagsResponseTypeDef,
+    RevocationConfigurationOutputTypeDef,
     RevocationConfigurationTypeDef,
     PolicyQualifierInfoTypeDef,
+    GeneralNameOutputTypeDef,
     GeneralNameTypeDef,
     UpdateCertificateAuthorityRequestRequestTypeDef,
     PolicyInformationTypeDef,
+    AccessDescriptionOutputTypeDef,
     AccessDescriptionTypeDef,
     ExtensionsTypeDef,
+    CsrExtensionsOutputTypeDef,
     CsrExtensionsTypeDef,
     ApiPassthroughTypeDef,
+    CertificateAuthorityConfigurationOutputTypeDef,
     CertificateAuthorityConfigurationTypeDef,
     IssueCertificateRequestRequestTypeDef,
     CertificateAuthorityTypeDef,
     CreateCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     ListCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> CustomAttributeTypeDef:
+def get_structure() -> CustomAttributeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-acm-pca-1.28.0/mypy_boto3_acm_pca.egg-info/SOURCES.txt` & `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.0/setup.py` & `mypy-boto3-acm-pca-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-acm-pca",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_acm_pca"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ACMPCA 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ACMPCA 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

