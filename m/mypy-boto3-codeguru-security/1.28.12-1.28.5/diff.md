# Comparing `tmp/mypy-boto3-codeguru-security-1.28.12.tar.gz` & `tmp/mypy-boto3-codeguru-security-1.28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguru-security-1.28.12.tar", last modified: Thu Jul 27 05:34:28 2023, max compression
+gzip compressed data, was "mypy-boto3-codeguru-security-1.28.5.tar", last modified: Tue Jul 18 19:32:41 2023, max compression
```

## Comparing `mypy-boto3-codeguru-security-1.28.12.tar` & `mypy-boto3-codeguru-security-1.28.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:28.520552 mypy-boto3-codeguru-security-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-07-27 05:34:28.520552 mypy-boto3-codeguru-security-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:28.512552 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15097 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:28.520552 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-07-27 05:34:28.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:28.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:28.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:28.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:28.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:28.000000 mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:28.520552 mypy-boto3-codeguru-security-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-security-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.754719 mypy-boto3-codeguru-security-1.28.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-18 19:32:41.754719 mypy-boto3-codeguru-security-1.28.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.746719 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:41.750719 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 19:32:41.000000 mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:41.754719 mypy-boto3-codeguru-security-1.28.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-18 19:31:59.000000 mypy-boto3-codeguru-security-1.28.5/setup.py
```

### Comparing `mypy-boto3-codeguru-security-1.28.12/LICENSE` & `mypy-boto3-codeguru-security-1.28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.12/PKG-INFO` & `mypy-boto3-codeguru-security-1.28.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-security
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeGuruSecurity 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.5
+Summary: Type annotations for boto3.CodeGuruSecurity 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeguru-security"></a>
 
 # mypy-boto3-codeguru-security
 
 [![PyPI - mypy-boto3-codeguru-security](https://img.shields.io/pypi/v/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-security)](https://pepy.tech/project/mypy-boto3-codeguru-security)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-security?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-security docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,50 +338,50 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_security.type_defs import (
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
+    ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
     ResourceIdOutputTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
-    CreateUploadUrlResponseTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
-    GetFindingsRequestGetFindingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetMetricsSummaryRequestRequestTypeDef,
     GetScanRequestRequestTypeDef,
-    GetScanResponseTypeDef,
-    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     ListFindingsMetricsRequestRequestTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
     ListScansRequestRequestTypeDef,
     ScanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ScanNameWithFindingNumTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     SuggestedFixTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AccountFindingsMetricTypeDef,
     BatchGetFindingsRequestRequestTypeDef,
+    CreateUploadUrlResponseTypeDef,
+    GetScanResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
+    GetFindingsRequestGetFindingsPaginateTypeDef,
+    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+    ListScansRequestListScansPaginateTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
     VulnerabilityTypeDef,
     GetMetricsSummaryResponseTypeDef,
     FindingTypeDef,
```

### Comparing `mypy-boto3-codeguru-security-1.28.12/README.md` & `mypy-boto3-codeguru-security-1.28.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codeguru-security"></a>
 
 # mypy-boto3-codeguru-security
 
 [![PyPI - mypy-boto3-codeguru-security](https://img.shields.io/pypi/v/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-security)](https://pepy.tech/project/mypy-boto3-codeguru-security)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-security?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-security docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,50 +306,50 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_security.type_defs import (
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
+    ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
     ResourceIdOutputTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
-    CreateUploadUrlResponseTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
-    GetFindingsRequestGetFindingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetMetricsSummaryRequestRequestTypeDef,
     GetScanRequestRequestTypeDef,
-    GetScanResponseTypeDef,
-    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     ListFindingsMetricsRequestRequestTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
     ListScansRequestRequestTypeDef,
     ScanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ScanNameWithFindingNumTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     SuggestedFixTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AccountFindingsMetricTypeDef,
     BatchGetFindingsRequestRequestTypeDef,
+    CreateUploadUrlResponseTypeDef,
+    GetScanResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
+    GetFindingsRequestGetFindingsPaginateTypeDef,
+    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+    ListScansRequestListScansPaginateTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
     VulnerabilityTypeDef,
     GetMetricsSummaryResponseTypeDef,
     FindingTypeDef,
```

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/__init__.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/__init__.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/__main__.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeGuruSecurity 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CodeGuruSecurity 1.28.5\nVersion:         1.28.5\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.5")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/client.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/client.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/literals.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/literals.pyi`

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
     "AnalysisTypeType",
     "ErrorCodeType",
     "GetFindingsPaginatorName",
     "ListFindingsMetricsPaginatorName",
     "ListScansPaginatorName",
     "ScanStateType",
@@ -31,15 +30,14 @@
     "StatusType",
     "CodeGuruSecurityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AnalysisTypeType = Literal["All", "Security"]
 ErrorCodeType = Literal[
     "DUPLICATE_IDENTIFIER",
     "INTERNAL_ERROR",
     "INVALID_FINDING_ID",
     "INVALID_SCAN_NAME",
     "ITEM_DOES_NOT_EXIST",
@@ -167,15 +165,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -254,28 +251,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
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
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/literals.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/literals.py`

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
     "AnalysisTypeType",
     "ErrorCodeType",
     "GetFindingsPaginatorName",
     "ListFindingsMetricsPaginatorName",
     "ListScansPaginatorName",
     "ScanStateType",
@@ -30,14 +31,15 @@
     "StatusType",
     "CodeGuruSecurityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 AnalysisTypeType = Literal["All", "Security"]
 ErrorCodeType = Literal[
     "DUPLICATE_IDENTIFIER",
     "INTERNAL_ERROR",
     "INVALID_FINDING_ID",
     "INVALID_SCAN_NAME",
     "ITEM_DOES_NOT_EXIST",
@@ -165,15 +167,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -252,28 +253,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
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
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/paginator.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     """
 
     def paginate(
         self,
         *,
         scanName: str,
         status: StatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#getfindingspaginator)
         """
 
 
@@ -75,28 +75,28 @@
     """
 
     def paginate(
         self,
         *,
         endDate: Union[datetime, str],
         startDate: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listfindingsmetricspaginator)
         """
 
 
 class ListScansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listscanspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listscanspaginator)
         """
```

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/paginator.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """
 
     def paginate(
         self,
         *,
         scanName: str,
         status: StatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.GetFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#getfindingspaginator)
         """
 
 class ListFindingsMetricsPaginator(Paginator):
@@ -71,27 +71,27 @@
     """
 
     def paginate(
         self,
         *,
         endDate: Union[datetime, str],
         startDate: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListFindingsMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listfindingsmetricspaginator)
         """
 
 class ListScansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listscanspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity.Paginator.ListScans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/paginators/#listscanspaginator)
         """
```

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/type_defs.py` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,50 +30,50 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FindingMetricsValuePerSeverityTypeDef",
     "BatchGetFindingsErrorTypeDef",
     "FindingIdentifierTypeDef",
+    "ResponseMetadataTypeDef",
     "CategoryWithFindingNumTypeDef",
     "CodeLineTypeDef",
     "ResourceIdTypeDef",
     "ResourceIdOutputTypeDef",
     "CreateUploadUrlRequestRequestTypeDef",
-    "CreateUploadUrlResponseTypeDef",
     "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "ResourceTypeDef",
-    "GetFindingsRequestGetFindingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "GetMetricsSummaryRequestRequestTypeDef",
     "GetScanRequestRequestTypeDef",
-    "GetScanResponseTypeDef",
-    "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     "ListFindingsMetricsRequestRequestTypeDef",
-    "ListScansRequestListScansPaginateTypeDef",
     "ListScansRequestRequestTypeDef",
     "ScanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ScanNameWithFindingNumTypeDef",
-    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
     "SuggestedFixTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AccountFindingsMetricTypeDef",
     "BatchGetFindingsRequestRequestTypeDef",
+    "CreateUploadUrlResponseTypeDef",
+    "GetScanResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "FilePathTypeDef",
     "CreateScanRequestRequestTypeDef",
     "CreateScanResponseTypeDef",
     "GetAccountConfigurationResponseTypeDef",
     "UpdateAccountConfigurationResponseTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
+    "GetFindingsRequestGetFindingsPaginateTypeDef",
+    "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    "ListScansRequestListScansPaginateTypeDef",
     "ListScansResponseTypeDef",
     "MetricsSummaryTypeDef",
     "RemediationTypeDef",
     "ListFindingsMetricsResponseTypeDef",
     "VulnerabilityTypeDef",
     "GetMetricsSummaryResponseTypeDef",
     "FindingTypeDef",
@@ -86,15 +86,14 @@
     {
         "critical": float,
         "high": float,
         "info": float,
         "low": float,
         "medium": float,
     },
-    total=False,
 )
 
 BatchGetFindingsErrorTypeDef = TypedDict(
     "BatchGetFindingsErrorTypeDef",
     {
         "errorCode": ErrorCodeType,
         "findingId": str,
@@ -107,30 +106,39 @@
     "FindingIdentifierTypeDef",
     {
         "findingId": str,
         "scanName": str,
     },
 )
 
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
 CategoryWithFindingNumTypeDef = TypedDict(
     "CategoryWithFindingNumTypeDef",
     {
         "categoryName": str,
         "findingNumber": int,
     },
-    total=False,
 )
 
 CodeLineTypeDef = TypedDict(
     "CodeLineTypeDef",
     {
         "content": str,
         "number": int,
     },
-    total=False,
 )
 
 ResourceIdTypeDef = TypedDict(
     "ResourceIdTypeDef",
     {
         "codeArtifactId": str,
     },
@@ -138,40 +146,28 @@
 )
 
 ResourceIdOutputTypeDef = TypedDict(
     "ResourceIdOutputTypeDef",
     {
         "codeArtifactId": str,
     },
-    total=False,
 )
 
 CreateUploadUrlRequestRequestTypeDef = TypedDict(
     "CreateUploadUrlRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 
-CreateUploadUrlResponseTypeDef = TypedDict(
-    "CreateUploadUrlResponseTypeDef",
-    {
-        "codeArtifactId": str,
-        "requestHeaders": Dict[str, str],
-        "s3Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EncryptionConfigOutputTypeDef = TypedDict(
     "EncryptionConfigOutputTypeDef",
     {
         "kmsKeyArn": str,
     },
-    total=False,
 )
 
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "kmsKeyArn": str,
     },
@@ -180,40 +176,26 @@
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "id": str,
         "subResourceId": str,
     },
-    total=False,
 )
 
-_RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
-    "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
-    {
-        "scanName": str,
-    },
-)
-_OptionalGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
-    "_OptionalGetFindingsRequestGetFindingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": StatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetFindingsRequestGetFindingsPaginateTypeDef(
-    _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
-    _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 _OptionalGetFindingsRequestRequestTypeDef = TypedDict(
@@ -257,52 +239,14 @@
 
 class GetScanRequestRequestTypeDef(
     _RequiredGetScanRequestRequestTypeDef, _OptionalGetScanRequestRequestTypeDef
 ):
     pass
 
 
-GetScanResponseTypeDef = TypedDict(
-    "GetScanResponseTypeDef",
-    {
-        "analysisType": AnalysisTypeType,
-        "createdAt": datetime,
-        "numberOfRevisions": int,
-        "runId": str,
-        "scanName": str,
-        "scanNameArn": str,
-        "scanState": ScanStateType,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
-    "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    {
-        "endDate": Union[datetime, str],
-        "startDate": Union[datetime, str],
-    },
-)
-_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
-    "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
-    _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredListFindingsMetricsRequestRequestTypeDef",
     {
         "endDate": Union[datetime, str],
         "startDate": Union[datetime, str],
     },
 )
@@ -319,115 +263,64 @@
 class ListFindingsMetricsRequestRequestTypeDef(
     _RequiredListFindingsMetricsRequestRequestTypeDef,
     _OptionalListFindingsMetricsRequestRequestTypeDef,
 ):
     pass
 
 
-ListScansRequestListScansPaginateTypeDef = TypedDict(
-    "ListScansRequestListScansPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListScansRequestRequestTypeDef = TypedDict(
     "ListScansRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredScanSummaryTypeDef = TypedDict(
-    "_RequiredScanSummaryTypeDef",
+ScanSummaryTypeDef = TypedDict(
+    "ScanSummaryTypeDef",
     {
         "createdAt": datetime,
         "runId": str,
         "scanName": str,
-        "scanState": ScanStateType,
-    },
-)
-_OptionalScanSummaryTypeDef = TypedDict(
-    "_OptionalScanSummaryTypeDef",
-    {
         "scanNameArn": str,
+        "scanState": ScanStateType,
         "updatedAt": datetime,
     },
-    total=False,
 )
 
-
-class ScanSummaryTypeDef(_RequiredScanSummaryTypeDef, _OptionalScanSummaryTypeDef):
-    pass
-
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ScanNameWithFindingNumTypeDef = TypedDict(
     "ScanNameWithFindingNumTypeDef",
     {
         "findingNumber": int,
         "scanName": str,
     },
-    total=False,
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "text": str,
         "url": str,
     },
-    total=False,
 )
 
 SuggestedFixTypeDef = TypedDict(
     "SuggestedFixTypeDef",
     {
         "code": str,
         "description": str,
     },
-    total=False,
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
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -447,34 +340,65 @@
     {
         "closedFindings": FindingMetricsValuePerSeverityTypeDef,
         "date": datetime,
         "meanTimeToClose": FindingMetricsValuePerSeverityTypeDef,
         "newFindings": FindingMetricsValuePerSeverityTypeDef,
         "openFindings": FindingMetricsValuePerSeverityTypeDef,
     },
-    total=False,
 )
 
 BatchGetFindingsRequestRequestTypeDef = TypedDict(
     "BatchGetFindingsRequestRequestTypeDef",
     {
         "findingIdentifiers": Sequence[FindingIdentifierTypeDef],
     },
 )
 
+CreateUploadUrlResponseTypeDef = TypedDict(
+    "CreateUploadUrlResponseTypeDef",
+    {
+        "codeArtifactId": str,
+        "requestHeaders": Dict[str, str],
+        "s3Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetScanResponseTypeDef = TypedDict(
+    "GetScanResponseTypeDef",
+    {
+        "analysisType": AnalysisTypeType,
+        "createdAt": datetime,
+        "numberOfRevisions": int,
+        "runId": str,
+        "scanName": str,
+        "scanNameArn": str,
+        "scanState": ScanStateType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 FilePathTypeDef = TypedDict(
     "FilePathTypeDef",
     {
         "codeSnippet": List[CodeLineTypeDef],
         "endLine": int,
         "name": str,
         "path": str,
         "startLine": int,
     },
-    total=False,
 )
 
 _RequiredCreateScanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScanRequestRequestTypeDef",
     {
         "resourceId": ResourceIdTypeDef,
         "scanName": str,
@@ -502,97 +426,148 @@
     "CreateScanResponseTypeDef",
     {
         "resourceId": ResourceIdOutputTypeDef,
         "runId": str,
         "scanName": str,
         "scanNameArn": str,
         "scanState": ScanStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
         "encryptionConfig": EncryptionConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountConfigurationResponseTypeDef = TypedDict(
     "UpdateAccountConfigurationResponseTypeDef",
     {
         "encryptionConfig": EncryptionConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
     },
 )
 
+_RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
+    "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
+    {
+        "scanName": str,
+    },
+)
+_OptionalGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
+    "_OptionalGetFindingsRequestGetFindingsPaginateTypeDef",
+    {
+        "status": StatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetFindingsRequestGetFindingsPaginateTypeDef(
+    _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
+    _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
+    "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    {
+        "endDate": Union[datetime, str],
+        "startDate": Union[datetime, str],
+    },
+)
+_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
+    "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
+    _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+    _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+):
+    pass
+
+
+ListScansRequestListScansPaginateTypeDef = TypedDict(
+    "ListScansRequestListScansPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListScansResponseTypeDef = TypedDict(
     "ListScansResponseTypeDef",
     {
         "nextToken": str,
         "summaries": List[ScanSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricsSummaryTypeDef = TypedDict(
     "MetricsSummaryTypeDef",
     {
         "categoriesWithMostFindings": List[CategoryWithFindingNumTypeDef],
         "date": datetime,
         "openFindings": FindingMetricsValuePerSeverityTypeDef,
         "scansWithMostOpenCriticalFindings": List[ScanNameWithFindingNumTypeDef],
         "scansWithMostOpenFindings": List[ScanNameWithFindingNumTypeDef],
     },
-    total=False,
 )
 
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
         "suggestedFixes": List[SuggestedFixTypeDef],
     },
-    total=False,
 )
 
 ListFindingsMetricsResponseTypeDef = TypedDict(
     "ListFindingsMetricsResponseTypeDef",
     {
         "findingsMetrics": List[AccountFindingsMetricTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VulnerabilityTypeDef = TypedDict(
     "VulnerabilityTypeDef",
     {
         "filePath": FilePathTypeDef,
         "id": str,
         "itemCount": int,
         "referenceUrls": List[str],
         "relatedVulnerabilities": List[str],
     },
-    total=False,
 )
 
 GetMetricsSummaryResponseTypeDef = TypedDict(
     "GetMetricsSummaryResponseTypeDef",
     {
         "metricsSummary": MetricsSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "createdAt": datetime,
@@ -608,27 +583,26 @@
         "severity": SeverityType,
         "status": StatusType,
         "title": str,
         "type": str,
         "updatedAt": datetime,
         "vulnerability": VulnerabilityTypeDef,
     },
-    total=False,
 )
 
 BatchGetFindingsResponseTypeDef = TypedDict(
     "BatchGetFindingsResponseTypeDef",
     {
         "failedFindings": List[BatchGetFindingsErrorTypeDef],
         "findings": List[FindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security/type_defs.pyi` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -29,50 +29,50 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FindingMetricsValuePerSeverityTypeDef",
     "BatchGetFindingsErrorTypeDef",
     "FindingIdentifierTypeDef",
+    "ResponseMetadataTypeDef",
     "CategoryWithFindingNumTypeDef",
     "CodeLineTypeDef",
     "ResourceIdTypeDef",
     "ResourceIdOutputTypeDef",
     "CreateUploadUrlRequestRequestTypeDef",
-    "CreateUploadUrlResponseTypeDef",
     "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "ResourceTypeDef",
-    "GetFindingsRequestGetFindingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "GetMetricsSummaryRequestRequestTypeDef",
     "GetScanRequestRequestTypeDef",
-    "GetScanResponseTypeDef",
-    "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
     "ListFindingsMetricsRequestRequestTypeDef",
-    "ListScansRequestListScansPaginateTypeDef",
     "ListScansRequestRequestTypeDef",
     "ScanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ScanNameWithFindingNumTypeDef",
-    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
     "SuggestedFixTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AccountFindingsMetricTypeDef",
     "BatchGetFindingsRequestRequestTypeDef",
+    "CreateUploadUrlResponseTypeDef",
+    "GetScanResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "FilePathTypeDef",
     "CreateScanRequestRequestTypeDef",
     "CreateScanResponseTypeDef",
     "GetAccountConfigurationResponseTypeDef",
     "UpdateAccountConfigurationResponseTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
+    "GetFindingsRequestGetFindingsPaginateTypeDef",
+    "ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    "ListScansRequestListScansPaginateTypeDef",
     "ListScansResponseTypeDef",
     "MetricsSummaryTypeDef",
     "RemediationTypeDef",
     "ListFindingsMetricsResponseTypeDef",
     "VulnerabilityTypeDef",
     "GetMetricsSummaryResponseTypeDef",
     "FindingTypeDef",
@@ -85,15 +85,14 @@
     {
         "critical": float,
         "high": float,
         "info": float,
         "low": float,
         "medium": float,
     },
-    total=False,
 )
 
 BatchGetFindingsErrorTypeDef = TypedDict(
     "BatchGetFindingsErrorTypeDef",
     {
         "errorCode": ErrorCodeType,
         "findingId": str,
@@ -106,30 +105,39 @@
     "FindingIdentifierTypeDef",
     {
         "findingId": str,
         "scanName": str,
     },
 )
 
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
 CategoryWithFindingNumTypeDef = TypedDict(
     "CategoryWithFindingNumTypeDef",
     {
         "categoryName": str,
         "findingNumber": int,
     },
-    total=False,
 )
 
 CodeLineTypeDef = TypedDict(
     "CodeLineTypeDef",
     {
         "content": str,
         "number": int,
     },
-    total=False,
 )
 
 ResourceIdTypeDef = TypedDict(
     "ResourceIdTypeDef",
     {
         "codeArtifactId": str,
     },
@@ -137,40 +145,28 @@
 )
 
 ResourceIdOutputTypeDef = TypedDict(
     "ResourceIdOutputTypeDef",
     {
         "codeArtifactId": str,
     },
-    total=False,
 )
 
 CreateUploadUrlRequestRequestTypeDef = TypedDict(
     "CreateUploadUrlRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 
-CreateUploadUrlResponseTypeDef = TypedDict(
-    "CreateUploadUrlResponseTypeDef",
-    {
-        "codeArtifactId": str,
-        "requestHeaders": Dict[str, str],
-        "s3Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EncryptionConfigOutputTypeDef = TypedDict(
     "EncryptionConfigOutputTypeDef",
     {
         "kmsKeyArn": str,
     },
-    total=False,
 )
 
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "kmsKeyArn": str,
     },
@@ -179,38 +175,26 @@
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "id": str,
         "subResourceId": str,
     },
-    total=False,
 )
 
-_RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
-    "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
-    {
-        "scanName": str,
-    },
-)
-_OptionalGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
-    "_OptionalGetFindingsRequestGetFindingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": StatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetFindingsRequestGetFindingsPaginateTypeDef(
-    _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
-    _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "scanName": str,
     },
 )
 _OptionalGetFindingsRequestRequestTypeDef = TypedDict(
@@ -250,50 +234,14 @@
 )
 
 class GetScanRequestRequestTypeDef(
     _RequiredGetScanRequestRequestTypeDef, _OptionalGetScanRequestRequestTypeDef
 ):
     pass
 
-GetScanResponseTypeDef = TypedDict(
-    "GetScanResponseTypeDef",
-    {
-        "analysisType": AnalysisTypeType,
-        "createdAt": datetime,
-        "numberOfRevisions": int,
-        "runId": str,
-        "scanName": str,
-        "scanNameArn": str,
-        "scanState": ScanStateType,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
-    "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    {
-        "endDate": Union[datetime, str],
-        "startDate": Union[datetime, str],
-    },
-)
-_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
-    "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
-    _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-):
-    pass
-
 _RequiredListFindingsMetricsRequestRequestTypeDef = TypedDict(
     "_RequiredListFindingsMetricsRequestRequestTypeDef",
     {
         "endDate": Union[datetime, str],
         "startDate": Union[datetime, str],
     },
 )
@@ -308,113 +256,64 @@
 
 class ListFindingsMetricsRequestRequestTypeDef(
     _RequiredListFindingsMetricsRequestRequestTypeDef,
     _OptionalListFindingsMetricsRequestRequestTypeDef,
 ):
     pass
 
-ListScansRequestListScansPaginateTypeDef = TypedDict(
-    "ListScansRequestListScansPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListScansRequestRequestTypeDef = TypedDict(
     "ListScansRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredScanSummaryTypeDef = TypedDict(
-    "_RequiredScanSummaryTypeDef",
+ScanSummaryTypeDef = TypedDict(
+    "ScanSummaryTypeDef",
     {
         "createdAt": datetime,
         "runId": str,
         "scanName": str,
-        "scanState": ScanStateType,
-    },
-)
-_OptionalScanSummaryTypeDef = TypedDict(
-    "_OptionalScanSummaryTypeDef",
-    {
         "scanNameArn": str,
+        "scanState": ScanStateType,
         "updatedAt": datetime,
     },
-    total=False,
 )
 
-class ScanSummaryTypeDef(_RequiredScanSummaryTypeDef, _OptionalScanSummaryTypeDef):
-    pass
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ScanNameWithFindingNumTypeDef = TypedDict(
     "ScanNameWithFindingNumTypeDef",
     {
         "findingNumber": int,
         "scanName": str,
     },
-    total=False,
-)
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "text": str,
         "url": str,
     },
-    total=False,
 )
 
 SuggestedFixTypeDef = TypedDict(
     "SuggestedFixTypeDef",
     {
         "code": str,
         "description": str,
     },
-    total=False,
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
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
@@ -434,34 +333,65 @@
     {
         "closedFindings": FindingMetricsValuePerSeverityTypeDef,
         "date": datetime,
         "meanTimeToClose": FindingMetricsValuePerSeverityTypeDef,
         "newFindings": FindingMetricsValuePerSeverityTypeDef,
         "openFindings": FindingMetricsValuePerSeverityTypeDef,
     },
-    total=False,
 )
 
 BatchGetFindingsRequestRequestTypeDef = TypedDict(
     "BatchGetFindingsRequestRequestTypeDef",
     {
         "findingIdentifiers": Sequence[FindingIdentifierTypeDef],
     },
 )
 
+CreateUploadUrlResponseTypeDef = TypedDict(
+    "CreateUploadUrlResponseTypeDef",
+    {
+        "codeArtifactId": str,
+        "requestHeaders": Dict[str, str],
+        "s3Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetScanResponseTypeDef = TypedDict(
+    "GetScanResponseTypeDef",
+    {
+        "analysisType": AnalysisTypeType,
+        "createdAt": datetime,
+        "numberOfRevisions": int,
+        "runId": str,
+        "scanName": str,
+        "scanNameArn": str,
+        "scanState": ScanStateType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 FilePathTypeDef = TypedDict(
     "FilePathTypeDef",
     {
         "codeSnippet": List[CodeLineTypeDef],
         "endLine": int,
         "name": str,
         "path": str,
         "startLine": int,
     },
-    total=False,
 )
 
 _RequiredCreateScanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScanRequestRequestTypeDef",
     {
         "resourceId": ResourceIdTypeDef,
         "scanName": str,
@@ -487,97 +417,144 @@
     "CreateScanResponseTypeDef",
     {
         "resourceId": ResourceIdOutputTypeDef,
         "runId": str,
         "scanName": str,
         "scanNameArn": str,
         "scanState": ScanStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
         "encryptionConfig": EncryptionConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountConfigurationResponseTypeDef = TypedDict(
     "UpdateAccountConfigurationResponseTypeDef",
     {
         "encryptionConfig": EncryptionConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountConfigurationRequestRequestTypeDef",
     {
         "encryptionConfig": EncryptionConfigTypeDef,
     },
 )
 
+_RequiredGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
+    "_RequiredGetFindingsRequestGetFindingsPaginateTypeDef",
+    {
+        "scanName": str,
+    },
+)
+_OptionalGetFindingsRequestGetFindingsPaginateTypeDef = TypedDict(
+    "_OptionalGetFindingsRequestGetFindingsPaginateTypeDef",
+    {
+        "status": StatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetFindingsRequestGetFindingsPaginateTypeDef(
+    _RequiredGetFindingsRequestGetFindingsPaginateTypeDef,
+    _OptionalGetFindingsRequestGetFindingsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
+    "_RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    {
+        "endDate": Union[datetime, str],
+        "startDate": Union[datetime, str],
+    },
+)
+_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef = TypedDict(
+    "_OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(
+    _RequiredListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+    _OptionalListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+):
+    pass
+
+ListScansRequestListScansPaginateTypeDef = TypedDict(
+    "ListScansRequestListScansPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListScansResponseTypeDef = TypedDict(
     "ListScansResponseTypeDef",
     {
         "nextToken": str,
         "summaries": List[ScanSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricsSummaryTypeDef = TypedDict(
     "MetricsSummaryTypeDef",
     {
         "categoriesWithMostFindings": List[CategoryWithFindingNumTypeDef],
         "date": datetime,
         "openFindings": FindingMetricsValuePerSeverityTypeDef,
         "scansWithMostOpenCriticalFindings": List[ScanNameWithFindingNumTypeDef],
         "scansWithMostOpenFindings": List[ScanNameWithFindingNumTypeDef],
     },
-    total=False,
 )
 
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
         "suggestedFixes": List[SuggestedFixTypeDef],
     },
-    total=False,
 )
 
 ListFindingsMetricsResponseTypeDef = TypedDict(
     "ListFindingsMetricsResponseTypeDef",
     {
         "findingsMetrics": List[AccountFindingsMetricTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VulnerabilityTypeDef = TypedDict(
     "VulnerabilityTypeDef",
     {
         "filePath": FilePathTypeDef,
         "id": str,
         "itemCount": int,
         "referenceUrls": List[str],
         "relatedVulnerabilities": List[str],
     },
-    total=False,
 )
 
 GetMetricsSummaryResponseTypeDef = TypedDict(
     "GetMetricsSummaryResponseTypeDef",
     {
         "metricsSummary": MetricsSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "createdAt": datetime,
@@ -593,27 +570,26 @@
         "severity": SeverityType,
         "status": StatusType,
         "title": str,
         "type": str,
         "updatedAt": datetime,
         "vulnerability": VulnerabilityTypeDef,
     },
-    total=False,
 )
 
 BatchGetFindingsResponseTypeDef = TypedDict(
     "BatchGetFindingsResponseTypeDef",
     {
         "failedFindings": List[BatchGetFindingsErrorTypeDef],
         "findings": List[FindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security.egg-info/PKG-INFO` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-security
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeGuruSecurity 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.5
+Summary: Type annotations for boto3.CodeGuruSecurity 1.28.5 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeguru-security"></a>
 
 # mypy-boto3-codeguru-security
 
 [![PyPI - mypy-boto3-codeguru-security](https://img.shields.io/pypi/v/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-security.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-security)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-security)](https://pepy.tech/project/mypy-boto3-codeguru-security)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-security?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-security)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruSecurity 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
+[boto3.CodeGuruSecurity 1.28.5](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-security docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,50 +338,50 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_security.type_defs import (
     FindingMetricsValuePerSeverityTypeDef,
     BatchGetFindingsErrorTypeDef,
     FindingIdentifierTypeDef,
+    ResponseMetadataTypeDef,
     CategoryWithFindingNumTypeDef,
     CodeLineTypeDef,
     ResourceIdTypeDef,
     ResourceIdOutputTypeDef,
     CreateUploadUrlRequestRequestTypeDef,
-    CreateUploadUrlResponseTypeDef,
     EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     ResourceTypeDef,
-    GetFindingsRequestGetFindingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetFindingsRequestRequestTypeDef,
     GetMetricsSummaryRequestRequestTypeDef,
     GetScanRequestRequestTypeDef,
-    GetScanResponseTypeDef,
-    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
     ListFindingsMetricsRequestRequestTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
     ListScansRequestRequestTypeDef,
     ScanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ScanNameWithFindingNumTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     SuggestedFixTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AccountFindingsMetricTypeDef,
     BatchGetFindingsRequestRequestTypeDef,
+    CreateUploadUrlResponseTypeDef,
+    GetScanResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     FilePathTypeDef,
     CreateScanRequestRequestTypeDef,
     CreateScanResponseTypeDef,
     GetAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationResponseTypeDef,
     UpdateAccountConfigurationRequestRequestTypeDef,
+    GetFindingsRequestGetFindingsPaginateTypeDef,
+    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
+    ListScansRequestListScansPaginateTypeDef,
     ListScansResponseTypeDef,
     MetricsSummaryTypeDef,
     RemediationTypeDef,
     ListFindingsMetricsResponseTypeDef,
     VulnerabilityTypeDef,
     GetMetricsSummaryResponseTypeDef,
     FindingTypeDef,
```

### Comparing `mypy-boto3-codeguru-security-1.28.12/mypy_boto3_codeguru_security.egg-info/SOURCES.txt` & `mypy-boto3-codeguru-security-1.28.5/mypy_boto3_codeguru_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-security-1.28.12/setup.py` & `mypy-boto3-codeguru-security-1.28.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguru-security",
-    version="1.28.12",
+    version="1.28.5",
     packages=["mypy_boto3_codeguru_security"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruSecurity 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CodeGuruSecurity 1.28.5 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

