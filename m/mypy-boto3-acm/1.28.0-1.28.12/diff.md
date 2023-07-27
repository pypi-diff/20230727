# Comparing `tmp/mypy-boto3-acm-1.28.0.tar.gz` & `tmp/mypy-boto3-acm-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-acm-1.28.0.tar", last modified: Thu Jul  6 20:58:51 2023, max compression
+gzip compressed data, was "mypy-boto3-acm-1.28.12.tar", last modified: Thu Jul 27 05:34:13 2023, max compression
```

## Comparing `mypy-boto3-acm-1.28.0.tar` & `mypy-boto3-acm-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.654206 mypy-boto3-acm-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-07-06 20:58:51.654206 mypy-boto3-acm-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.638206 mypy-boto3-acm-1.28.0/mypy_boto3_acm/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-06 20:32:31.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-07-06 20:32:31.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.638206 mypy-boto3-acm-1.28.0/mypy_boto3_acm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-07-06 20:58:51.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-06 20:58:51.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:51.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:51.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:51.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:58:51.000000 mypy-boto3-acm-1.28.0/mypy_boto3_acm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:51.654206 mypy-boto3-acm-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:32:30.000000 mypy-boto3-acm-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.844594 mypy-boto3-acm-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:16:52.000000 mypy-boto3-acm-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-27 05:34:13.844594 mypy-boto3-acm-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-07-27 05:16:52.000000 mypy-boto3-acm-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.840594 mypy-boto3-acm-1.28.12/mypy_boto3_acm/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-27 05:16:52.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-27 05:16:52.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15609 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15592 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:16:52.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.844594 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-27 05:34:13.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:34:13.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:13.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:13.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:13.844594 mypy-boto3-acm-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:16:52.000000 mypy-boto3-acm-1.28.12/setup.py
```

### Comparing `mypy-boto3-acm-1.28.0/LICENSE` & `mypy-boto3-acm-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.0/PKG-INFO` & `mypy-boto3-acm-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm
-Version: 1.28.0
-Summary: Type annotations for boto3.ACM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ACM 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-acm"></a>
 
 # mypy-boto3-acm
 
 [![PyPI - mypy-boto3-acm](https://img.shields.io/pypi/v/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-acm?color=blue)](https://pypistats.org/packages/mypy-boto3-acm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm)](https://pepy.tech/project/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,50 +357,53 @@
 
 `mypy_boto3_acm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_acm.type_defs import (
     TagTypeDef,
-    CertificateOptionsTypeDef,
+    CertificateOptionsOutputTypeDef,
     ExtendedKeyUsageTypeDef,
     KeyUsageTypeDef,
+    CertificateOptionsTypeDef,
     CertificateSummaryTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DomainValidationOptionTypeDef,
     ResourceRecordTypeDef,
+    ExpiryEventsConfigurationOutputTypeDef,
     ExpiryEventsConfigurationTypeDef,
     ExportCertificateRequestRequestTypeDef,
     FiltersTypeDef,
     GetCertificateRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForCertificateRequestRequestTypeDef,
+    TagOutputTypeDef,
     RenewCertificateRequestRequestTypeDef,
     ResendValidationEmailRequestRequestTypeDef,
     AddTagsToCertificateRequestRequestTypeDef,
     ImportCertificateRequestRequestTypeDef,
     RemoveTagsFromCertificateRequestRequestTypeDef,
     UpdateCertificateOptionsRequestRequestTypeDef,
     DescribeCertificateRequestCertificateValidatedWaitTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportCertificateResponseTypeDef,
     GetCertificateResponseTypeDef,
     ImportCertificateResponseTypeDef,
     ListCertificatesResponseTypeDef,
-    ListTagsForCertificateResponseTypeDef,
     RequestCertificateResponseTypeDef,
     RequestCertificateRequestRequestTypeDef,
     DomainValidationTypeDef,
     GetAccountConfigurationResponseTypeDef,
     PutAccountConfigurationRequestRequestTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListTagsForCertificateResponseTypeDef,
     RenewalSummaryTypeDef,
     CertificateDetailTypeDef,
     DescribeCertificateResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
```

### Comparing `mypy-boto3-acm-1.28.0/README.md` & `mypy-boto3-acm-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-acm"></a>
 
 # mypy-boto3-acm
 
 [![PyPI - mypy-boto3-acm](https://img.shields.io/pypi/v/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-acm?color=blue)](https://pypistats.org/packages/mypy-boto3-acm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm)](https://pepy.tech/project/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,50 +325,53 @@
 
 `mypy_boto3_acm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_acm.type_defs import (
     TagTypeDef,
-    CertificateOptionsTypeDef,
+    CertificateOptionsOutputTypeDef,
     ExtendedKeyUsageTypeDef,
     KeyUsageTypeDef,
+    CertificateOptionsTypeDef,
     CertificateSummaryTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DomainValidationOptionTypeDef,
     ResourceRecordTypeDef,
+    ExpiryEventsConfigurationOutputTypeDef,
     ExpiryEventsConfigurationTypeDef,
     ExportCertificateRequestRequestTypeDef,
     FiltersTypeDef,
     GetCertificateRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForCertificateRequestRequestTypeDef,
+    TagOutputTypeDef,
     RenewCertificateRequestRequestTypeDef,
     ResendValidationEmailRequestRequestTypeDef,
     AddTagsToCertificateRequestRequestTypeDef,
     ImportCertificateRequestRequestTypeDef,
     RemoveTagsFromCertificateRequestRequestTypeDef,
     UpdateCertificateOptionsRequestRequestTypeDef,
     DescribeCertificateRequestCertificateValidatedWaitTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportCertificateResponseTypeDef,
     GetCertificateResponseTypeDef,
     ImportCertificateResponseTypeDef,
     ListCertificatesResponseTypeDef,
-    ListTagsForCertificateResponseTypeDef,
     RequestCertificateResponseTypeDef,
     RequestCertificateRequestRequestTypeDef,
     DomainValidationTypeDef,
     GetAccountConfigurationResponseTypeDef,
     PutAccountConfigurationRequestRequestTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListTagsForCertificateResponseTypeDef,
     RenewalSummaryTypeDef,
     CertificateDetailTypeDef,
     DescribeCertificateResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
```

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/__init__.py` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/__init__.pyi` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/__main__.py` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ACM 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ACM 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM\nOther"
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

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/client.py` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/client.pyi` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/literals.py` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,14 +243,15 @@
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
@@ -329,26 +330,28 @@
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

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/literals.pyi` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,15 @@
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
@@ -327,26 +328,28 @@
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

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/paginator.py` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/paginator.pyi` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/type_defs.py` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,50 +41,53 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "CertificateOptionsTypeDef",
+    "CertificateOptionsOutputTypeDef",
     "ExtendedKeyUsageTypeDef",
     "KeyUsageTypeDef",
+    "CertificateOptionsTypeDef",
     "CertificateSummaryTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DomainValidationOptionTypeDef",
     "ResourceRecordTypeDef",
+    "ExpiryEventsConfigurationOutputTypeDef",
     "ExpiryEventsConfigurationTypeDef",
     "ExportCertificateRequestRequestTypeDef",
     "FiltersTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListTagsForCertificateRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "RenewCertificateRequestRequestTypeDef",
     "ResendValidationEmailRequestRequestTypeDef",
     "AddTagsToCertificateRequestRequestTypeDef",
     "ImportCertificateRequestRequestTypeDef",
     "RemoveTagsFromCertificateRequestRequestTypeDef",
     "UpdateCertificateOptionsRequestRequestTypeDef",
     "DescribeCertificateRequestCertificateValidatedWaitTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportCertificateResponseTypeDef",
     "GetCertificateResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "ListCertificatesResponseTypeDef",
-    "ListTagsForCertificateResponseTypeDef",
     "RequestCertificateResponseTypeDef",
     "RequestCertificateRequestRequestTypeDef",
     "DomainValidationTypeDef",
     "GetAccountConfigurationResponseTypeDef",
     "PutAccountConfigurationRequestRequestTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListTagsForCertificateResponseTypeDef",
     "RenewalSummaryTypeDef",
     "CertificateDetailTypeDef",
     "DescribeCertificateResponseTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
@@ -101,16 +104,16 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
-CertificateOptionsTypeDef = TypedDict(
-    "CertificateOptionsTypeDef",
+CertificateOptionsOutputTypeDef = TypedDict(
+    "CertificateOptionsOutputTypeDef",
     {
         "CertificateTransparencyLoggingPreference": CertificateTransparencyLoggingPreferenceType,
     },
     total=False,
 )
 
 ExtendedKeyUsageTypeDef = TypedDict(
@@ -126,14 +129,22 @@
     "KeyUsageTypeDef",
     {
         "Name": KeyUsageNameType,
     },
     total=False,
 )
 
+CertificateOptionsTypeDef = TypedDict(
+    "CertificateOptionsTypeDef",
+    {
+        "CertificateTransparencyLoggingPreference": CertificateTransparencyLoggingPreferenceType,
+    },
+    total=False,
+)
+
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "CertificateArn": str,
         "DomainName": str,
         "SubjectAlternativeNameSummaries": List[str],
         "HasAdditionalSubjectAlternativeNames": bool,
@@ -202,14 +213,22 @@
     {
         "Name": str,
         "Type": Literal["CNAME"],
         "Value": str,
     },
 )
 
+ExpiryEventsConfigurationOutputTypeDef = TypedDict(
+    "ExpiryEventsConfigurationOutputTypeDef",
+    {
+        "DaysBeforeExpiry": int,
+    },
+    total=False,
+)
+
 ExpiryEventsConfigurationTypeDef = TypedDict(
     "ExpiryEventsConfigurationTypeDef",
     {
         "DaysBeforeExpiry": int,
     },
     total=False,
 )
@@ -252,14 +271,33 @@
 ListTagsForCertificateRequestRequestTypeDef = TypedDict(
     "ListTagsForCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
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
 RenewCertificateRequestRequestTypeDef = TypedDict(
     "RenewCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
@@ -381,22 +419,14 @@
     {
         "NextToken": str,
         "CertificateSummaryList": List[CertificateSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForCertificateResponseTypeDef = TypedDict(
-    "ListTagsForCertificateResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RequestCertificateResponseTypeDef = TypedDict(
     "RequestCertificateResponseTypeDef",
     {
         "CertificateArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -452,15 +482,15 @@
 class DomainValidationTypeDef(_RequiredDomainValidationTypeDef, _OptionalDomainValidationTypeDef):
     pass
 
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
-        "ExpiryEvents": ExpiryEventsConfigurationTypeDef,
+        "ExpiryEvents": ExpiryEventsConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAccountConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAccountConfigurationRequestRequestTypeDef",
     {
@@ -504,14 +534,22 @@
         "SortBy": Literal["CREATED_AT"],
         "SortOrder": SortOrderType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListTagsForCertificateResponseTypeDef = TypedDict(
+    "ListTagsForCertificateResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredRenewalSummaryTypeDef = TypedDict(
     "_RequiredRenewalSummaryTypeDef",
     {
         "RenewalStatus": RenewalStatusType,
         "DomainValidationOptions": List[DomainValidationTypeDef],
         "UpdatedAt": datetime,
     },
@@ -553,15 +591,15 @@
         "FailureReason": FailureReasonType,
         "Type": CertificateTypeType,
         "RenewalSummary": RenewalSummaryTypeDef,
         "KeyUsages": List[KeyUsageTypeDef],
         "ExtendedKeyUsages": List[ExtendedKeyUsageTypeDef],
         "CertificateAuthorityArn": str,
         "RenewalEligibility": RenewalEligibilityType,
-        "Options": CertificateOptionsTypeDef,
+        "Options": CertificateOptionsOutputTypeDef,
     },
     total=False,
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
```

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/type_defs.pyi` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -40,50 +40,53 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "CertificateOptionsTypeDef",
+    "CertificateOptionsOutputTypeDef",
     "ExtendedKeyUsageTypeDef",
     "KeyUsageTypeDef",
+    "CertificateOptionsTypeDef",
     "CertificateSummaryTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DomainValidationOptionTypeDef",
     "ResourceRecordTypeDef",
+    "ExpiryEventsConfigurationOutputTypeDef",
     "ExpiryEventsConfigurationTypeDef",
     "ExportCertificateRequestRequestTypeDef",
     "FiltersTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListTagsForCertificateRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "RenewCertificateRequestRequestTypeDef",
     "ResendValidationEmailRequestRequestTypeDef",
     "AddTagsToCertificateRequestRequestTypeDef",
     "ImportCertificateRequestRequestTypeDef",
     "RemoveTagsFromCertificateRequestRequestTypeDef",
     "UpdateCertificateOptionsRequestRequestTypeDef",
     "DescribeCertificateRequestCertificateValidatedWaitTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportCertificateResponseTypeDef",
     "GetCertificateResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "ListCertificatesResponseTypeDef",
-    "ListTagsForCertificateResponseTypeDef",
     "RequestCertificateResponseTypeDef",
     "RequestCertificateRequestRequestTypeDef",
     "DomainValidationTypeDef",
     "GetAccountConfigurationResponseTypeDef",
     "PutAccountConfigurationRequestRequestTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListTagsForCertificateResponseTypeDef",
     "RenewalSummaryTypeDef",
     "CertificateDetailTypeDef",
     "DescribeCertificateResponseTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
@@ -98,16 +101,16 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-CertificateOptionsTypeDef = TypedDict(
-    "CertificateOptionsTypeDef",
+CertificateOptionsOutputTypeDef = TypedDict(
+    "CertificateOptionsOutputTypeDef",
     {
         "CertificateTransparencyLoggingPreference": CertificateTransparencyLoggingPreferenceType,
     },
     total=False,
 )
 
 ExtendedKeyUsageTypeDef = TypedDict(
@@ -123,14 +126,22 @@
     "KeyUsageTypeDef",
     {
         "Name": KeyUsageNameType,
     },
     total=False,
 )
 
+CertificateOptionsTypeDef = TypedDict(
+    "CertificateOptionsTypeDef",
+    {
+        "CertificateTransparencyLoggingPreference": CertificateTransparencyLoggingPreferenceType,
+    },
+    total=False,
+)
+
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "CertificateArn": str,
         "DomainName": str,
         "SubjectAlternativeNameSummaries": List[str],
         "HasAdditionalSubjectAlternativeNames": bool,
@@ -199,14 +210,22 @@
     {
         "Name": str,
         "Type": Literal["CNAME"],
         "Value": str,
     },
 )
 
+ExpiryEventsConfigurationOutputTypeDef = TypedDict(
+    "ExpiryEventsConfigurationOutputTypeDef",
+    {
+        "DaysBeforeExpiry": int,
+    },
+    total=False,
+)
+
 ExpiryEventsConfigurationTypeDef = TypedDict(
     "ExpiryEventsConfigurationTypeDef",
     {
         "DaysBeforeExpiry": int,
     },
     total=False,
 )
@@ -249,14 +268,31 @@
 ListTagsForCertificateRequestRequestTypeDef = TypedDict(
     "ListTagsForCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
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
 RenewCertificateRequestRequestTypeDef = TypedDict(
     "RenewCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
@@ -374,22 +410,14 @@
     {
         "NextToken": str,
         "CertificateSummaryList": List[CertificateSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForCertificateResponseTypeDef = TypedDict(
-    "ListTagsForCertificateResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 RequestCertificateResponseTypeDef = TypedDict(
     "RequestCertificateResponseTypeDef",
     {
         "CertificateArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -441,15 +469,15 @@
 
 class DomainValidationTypeDef(_RequiredDomainValidationTypeDef, _OptionalDomainValidationTypeDef):
     pass
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
-        "ExpiryEvents": ExpiryEventsConfigurationTypeDef,
+        "ExpiryEvents": ExpiryEventsConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAccountConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAccountConfigurationRequestRequestTypeDef",
     {
@@ -491,14 +519,22 @@
         "SortBy": Literal["CREATED_AT"],
         "SortOrder": SortOrderType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListTagsForCertificateResponseTypeDef = TypedDict(
+    "ListTagsForCertificateResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredRenewalSummaryTypeDef = TypedDict(
     "_RequiredRenewalSummaryTypeDef",
     {
         "RenewalStatus": RenewalStatusType,
         "DomainValidationOptions": List[DomainValidationTypeDef],
         "UpdatedAt": datetime,
     },
@@ -538,15 +574,15 @@
         "FailureReason": FailureReasonType,
         "Type": CertificateTypeType,
         "RenewalSummary": RenewalSummaryTypeDef,
         "KeyUsages": List[KeyUsageTypeDef],
         "ExtendedKeyUsages": List[ExtendedKeyUsageTypeDef],
         "CertificateAuthorityArn": str,
         "RenewalEligibility": RenewalEligibilityType,
-        "Options": CertificateOptionsTypeDef,
+        "Options": CertificateOptionsOutputTypeDef,
     },
     total=False,
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
```

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/waiter.py` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm/waiter.pyi` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm.egg-info/PKG-INFO` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm
-Version: 1.28.0
-Summary: Type annotations for boto3.ACM 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ACM 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-acm"></a>
 
 # mypy-boto3-acm
 
 [![PyPI - mypy-boto3-acm](https://img.shields.io/pypi/v/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-acm?color=blue)](https://pypistats.org/packages/mypy-boto3-acm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm)](https://pepy.tech/project/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,50 +357,53 @@
 
 `mypy_boto3_acm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_acm.type_defs import (
     TagTypeDef,
-    CertificateOptionsTypeDef,
+    CertificateOptionsOutputTypeDef,
     ExtendedKeyUsageTypeDef,
     KeyUsageTypeDef,
+    CertificateOptionsTypeDef,
     CertificateSummaryTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DomainValidationOptionTypeDef,
     ResourceRecordTypeDef,
+    ExpiryEventsConfigurationOutputTypeDef,
     ExpiryEventsConfigurationTypeDef,
     ExportCertificateRequestRequestTypeDef,
     FiltersTypeDef,
     GetCertificateRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForCertificateRequestRequestTypeDef,
+    TagOutputTypeDef,
     RenewCertificateRequestRequestTypeDef,
     ResendValidationEmailRequestRequestTypeDef,
     AddTagsToCertificateRequestRequestTypeDef,
     ImportCertificateRequestRequestTypeDef,
     RemoveTagsFromCertificateRequestRequestTypeDef,
     UpdateCertificateOptionsRequestRequestTypeDef,
     DescribeCertificateRequestCertificateValidatedWaitTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportCertificateResponseTypeDef,
     GetCertificateResponseTypeDef,
     ImportCertificateResponseTypeDef,
     ListCertificatesResponseTypeDef,
-    ListTagsForCertificateResponseTypeDef,
     RequestCertificateResponseTypeDef,
     RequestCertificateRequestRequestTypeDef,
     DomainValidationTypeDef,
     GetAccountConfigurationResponseTypeDef,
     PutAccountConfigurationRequestRequestTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListTagsForCertificateResponseTypeDef,
     RenewalSummaryTypeDef,
     CertificateDetailTypeDef,
     DescribeCertificateResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
```

### Comparing `mypy-boto3-acm-1.28.0/mypy_boto3_acm.egg-info/SOURCES.txt` & `mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.0/setup.py` & `mypy-boto3-acm-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-acm",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_acm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ACM 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ACM 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

