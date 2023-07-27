# Comparing `tmp/mypy-boto3-support-1.28.0.tar.gz` & `tmp/mypy-boto3-support-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-support-1.28.0.tar", last modified: Thu Jul  6 21:00:45 2023, max compression
+gzip compressed data, was "mypy-boto3-support-1.28.12.tar", last modified: Thu Jul 27 11:49:44 2023, max compression
```

## Comparing `mypy-boto3-support-1.28.0.tar` & `mypy-boto3-support-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:45.878448 mypy-boto3-support-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-06 21:00:45.878448 mypy-boto3-support-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:45.866448 mypy-boto3-support-1.28.0/mypy_boto3_support/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14850 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-07-06 20:56:59.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-07-06 20:56:59.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/mypy_boto3_support/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:45.878448 mypy-boto3-support-1.28.0/mypy_boto3_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-06 21:00:45.000000 mypy-boto3-support-1.28.0/mypy_boto3_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 21:00:45.000000 mypy-boto3-support-1.28.0/mypy_boto3_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:45.000000 mypy-boto3-support-1.28.0/mypy_boto3_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:45.000000 mypy-boto3-support-1.28.0/mypy_boto3_support.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:45.000000 mypy-boto3-support-1.28.0/mypy_boto3_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 21:00:45.000000 mypy-boto3-support-1.28.0/mypy_boto3_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:45.878448 mypy-boto3-support-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:56:58.000000 mypy-boto3-support-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.833373 mypy-boto3-support-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-07-27 11:49:44.833373 mypy-boto3-support-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.833373 mypy-boto3-support-1.28.12/mypy_boto3_support/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14850 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/mypy_boto3_support/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:44.833373 mypy-boto3-support-1.28.12/mypy_boto3_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-07-27 11:49:44.000000 mypy-boto3-support-1.28.12/mypy_boto3_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 11:49:44.000000 mypy-boto3-support-1.28.12/mypy_boto3_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:44.000000 mypy-boto3-support-1.28.12/mypy_boto3_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:44.000000 mypy-boto3-support-1.28.12/mypy_boto3_support.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:44.000000 mypy-boto3-support-1.28.12/mypy_boto3_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 11:49:44.000000 mypy-boto3-support-1.28.12/mypy_boto3_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:44.833373 mypy-boto3-support-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 11:47:48.000000 mypy-boto3-support-1.28.12/setup.py
```

### Comparing `mypy-boto3-support-1.28.0/LICENSE` & `mypy-boto3-support-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.0/PKG-INFO` & `mypy-boto3-support-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-support
-Version: 1.28.0
-Summary: Type annotations for boto3.Support 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Support 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-support"></a>
 
 # mypy-boto3-support
 
 [![PyPI - mypy-boto3-support](https://img.shields.io/pypi/v/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-support?color=blue)](https://pypistats.org/packages/mypy-boto3-support)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-support)](https://pepy.tech/project/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,53 +322,54 @@
 
 `mypy_boto3_support.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_support.type_defs import (
     AttachmentTypeDef,
-    AddAttachmentsToSetResponseTypeDef,
+    ResponseMetadataTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
-    AddCommunicationToCaseResponseTypeDef,
     AttachmentDetailsTypeDef,
+    AttachmentOutputTypeDef,
     CategoryTypeDef,
     DateIntervalTypeDef,
     SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
-    CreateCaseResponseTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
-    DescribeCasesRequestDescribeCasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCasesRequestRequestTypeDef,
-    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeCommunicationsRequestRequestTypeDef,
     DescribeCreateCaseOptionsRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     DescribeSeverityLevelsRequestRequestTypeDef,
     SeverityLevelTypeDef,
     DescribeSupportedLanguagesRequestRequestTypeDef,
     SupportedLanguageTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef,
     TrustedAdvisorCheckRefreshStatusTypeDef,
     DescribeTrustedAdvisorCheckResultRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef,
     DescribeTrustedAdvisorChecksRequestRequestTypeDef,
     TrustedAdvisorCheckDescriptionTypeDef,
-    PaginatorConfigTypeDef,
     RefreshTrustedAdvisorCheckRequestRequestTypeDef,
     ResolveCaseRequestRequestTypeDef,
-    ResolveCaseResponseTypeDef,
-    ResponseMetadataTypeDef,
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
     AddAttachmentsToSetRequestRequestTypeDef,
-    DescribeAttachmentResponseTypeDef,
+    AddAttachmentsToSetResponseTypeDef,
+    AddCommunicationToCaseResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
+    DescribeAttachmentResponseTypeDef,
     ServiceTypeDef,
     CommunicationTypeOptionsTypeDef,
+    DescribeCasesRequestDescribeCasesPaginateTypeDef,
+    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
     DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     TrustedAdvisorCategorySpecificSummaryTypeDef,
     DescribeCommunicationsResponseTypeDef,
```

### Comparing `mypy-boto3-support-1.28.0/README.md` & `mypy-boto3-support-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-support"></a>
 
 # mypy-boto3-support
 
 [![PyPI - mypy-boto3-support](https://img.shields.io/pypi/v/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-support?color=blue)](https://pypistats.org/packages/mypy-boto3-support)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-support)](https://pepy.tech/project/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,53 +290,54 @@
 
 `mypy_boto3_support.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_support.type_defs import (
     AttachmentTypeDef,
-    AddAttachmentsToSetResponseTypeDef,
+    ResponseMetadataTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
-    AddCommunicationToCaseResponseTypeDef,
     AttachmentDetailsTypeDef,
+    AttachmentOutputTypeDef,
     CategoryTypeDef,
     DateIntervalTypeDef,
     SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
-    CreateCaseResponseTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
-    DescribeCasesRequestDescribeCasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCasesRequestRequestTypeDef,
-    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeCommunicationsRequestRequestTypeDef,
     DescribeCreateCaseOptionsRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     DescribeSeverityLevelsRequestRequestTypeDef,
     SeverityLevelTypeDef,
     DescribeSupportedLanguagesRequestRequestTypeDef,
     SupportedLanguageTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef,
     TrustedAdvisorCheckRefreshStatusTypeDef,
     DescribeTrustedAdvisorCheckResultRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef,
     DescribeTrustedAdvisorChecksRequestRequestTypeDef,
     TrustedAdvisorCheckDescriptionTypeDef,
-    PaginatorConfigTypeDef,
     RefreshTrustedAdvisorCheckRequestRequestTypeDef,
     ResolveCaseRequestRequestTypeDef,
-    ResolveCaseResponseTypeDef,
-    ResponseMetadataTypeDef,
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
     AddAttachmentsToSetRequestRequestTypeDef,
-    DescribeAttachmentResponseTypeDef,
+    AddAttachmentsToSetResponseTypeDef,
+    AddCommunicationToCaseResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
+    DescribeAttachmentResponseTypeDef,
     ServiceTypeDef,
     CommunicationTypeOptionsTypeDef,
+    DescribeCasesRequestDescribeCasesPaginateTypeDef,
+    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
     DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     TrustedAdvisorCategorySpecificSummaryTypeDef,
     DescribeCommunicationsResponseTypeDef,
```

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support/__init__.py` & `mypy-boto3-support-1.28.12/mypy_boto3_support/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support/__init__.pyi` & `mypy-boto3-support-1.28.12/mypy_boto3_support/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support/__main__.py` & `mypy-boto3-support-1.28.12/mypy_boto3_support/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Support 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Support 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support\nOther"
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

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support/client.py` & `mypy-boto3-support-1.28.12/mypy_boto3_support/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support/client.pyi` & `mypy-boto3-support-1.28.12/mypy_boto3_support/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support/literals.py` & `mypy-boto3-support-1.28.12/mypy_boto3_support/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
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
@@ -233,26 +234,28 @@
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

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support/literals.pyi` & `mypy-boto3-support-1.28.12/mypy_boto3_support/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,15 @@
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
@@ -231,26 +232,28 @@
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

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support/paginator.py` & `mypy-boto3-support-1.28.12/mypy_boto3_support/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         caseIdList: Sequence[str] = ...,
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         language: str = ...,
         includeCommunications: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/paginators/#describecasespaginator)
         """
 
 
@@ -76,13 +76,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeCommunicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCommunications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/paginators/#describecommunicationspaginator)
         """
```

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support/paginator.pyi` & `mypy-boto3-support-1.28.12/mypy_boto3_support/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         caseIdList: Sequence[str] = ...,
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         language: str = ...,
         includeCommunications: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/paginators/#describecasespaginator)
         """
 
 class DescribeCommunicationsPaginator(Paginator):
@@ -72,13 +72,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeCommunicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCommunications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/paginators/#describecommunicationspaginator)
         """
```

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support/type_defs.py` & `mypy-boto3-support-1.28.12/mypy_boto3_support/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,53 +20,54 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AttachmentTypeDef",
-    "AddAttachmentsToSetResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
-    "AddCommunicationToCaseResponseTypeDef",
     "AttachmentDetailsTypeDef",
+    "AttachmentOutputTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
     "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
-    "CreateCaseResponseTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
-    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCasesRequestRequestTypeDef",
-    "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeCommunicationsRequestRequestTypeDef",
     "DescribeCreateCaseOptionsRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "DescribeSeverityLevelsRequestRequestTypeDef",
     "SeverityLevelTypeDef",
     "DescribeSupportedLanguagesRequestRequestTypeDef",
     "SupportedLanguageTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef",
     "TrustedAdvisorCheckRefreshStatusTypeDef",
     "DescribeTrustedAdvisorCheckResultRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef",
     "DescribeTrustedAdvisorChecksRequestRequestTypeDef",
     "TrustedAdvisorCheckDescriptionTypeDef",
-    "PaginatorConfigTypeDef",
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     "ResolveCaseRequestRequestTypeDef",
-    "ResolveCaseResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
     "AddAttachmentsToSetRequestRequestTypeDef",
-    "DescribeAttachmentResponseTypeDef",
+    "AddAttachmentsToSetResponseTypeDef",
+    "AddCommunicationToCaseResponseTypeDef",
+    "CreateCaseResponseTypeDef",
+    "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
+    "DescribeAttachmentResponseTypeDef",
     "ServiceTypeDef",
     "CommunicationTypeOptionsTypeDef",
+    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+    "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
     "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     "DescribeCommunicationsResponseTypeDef",
@@ -86,20 +87,22 @@
     {
         "fileName": str,
         "data": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-AddAttachmentsToSetResponseTypeDef = TypedDict(
-    "AddAttachmentsToSetResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "attachmentSetId": str,
-        "expiryTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredAddCommunicationToCaseRequestRequestTypeDef = TypedDict(
     "_RequiredAddCommunicationToCaseRequestRequestTypeDef",
     {
         "communicationBody": str,
@@ -119,27 +122,28 @@
 class AddCommunicationToCaseRequestRequestTypeDef(
     _RequiredAddCommunicationToCaseRequestRequestTypeDef,
     _OptionalAddCommunicationToCaseRequestRequestTypeDef,
 ):
     pass
 
 
-AddCommunicationToCaseResponseTypeDef = TypedDict(
-    "AddCommunicationToCaseResponseTypeDef",
+AttachmentDetailsTypeDef = TypedDict(
+    "AttachmentDetailsTypeDef",
     {
-        "result": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "attachmentId": str,
+        "fileName": str,
     },
+    total=False,
 )
 
-AttachmentDetailsTypeDef = TypedDict(
-    "AttachmentDetailsTypeDef",
+AttachmentOutputTypeDef = TypedDict(
+    "AttachmentOutputTypeDef",
     {
-        "attachmentId": str,
         "fileName": str,
+        "data": bytes,
     },
     total=False,
 )
 
 CategoryTypeDef = TypedDict(
     "CategoryTypeDef",
     {
@@ -191,40 +195,27 @@
 
 class CreateCaseRequestRequestTypeDef(
     _RequiredCreateCaseRequestRequestTypeDef, _OptionalCreateCaseRequestRequestTypeDef
 ):
     pass
 
 
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAttachmentRequestRequestTypeDef = TypedDict(
     "DescribeAttachmentRequestRequestTypeDef",
     {
         "attachmentId": str,
     },
 )
 
-DescribeCasesRequestDescribeCasesPaginateTypeDef = TypedDict(
-    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "caseIdList": Sequence[str],
-        "displayId": str,
-        "afterTime": str,
-        "beforeTime": str,
-        "includeResolvedCases": bool,
-        "language": str,
-        "includeCommunications": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeCasesRequestRequestTypeDef = TypedDict(
     "DescribeCasesRequestRequestTypeDef",
     {
@@ -237,38 +228,14 @@
         "maxResults": int,
         "language": str,
         "includeCommunications": bool,
     },
     total=False,
 )
 
-_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
-    {
-        "caseId": str,
-    },
-)
-_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
-    {
-        "beforeTime": str,
-        "afterTime": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef(
-    _RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-    _OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeCommunicationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommunicationsRequestRequestTypeDef",
     {
         "caseId": str,
     },
 )
 _OptionalDescribeCommunicationsRequestRequestTypeDef = TypedDict(
@@ -404,24 +371,14 @@
         "name": str,
         "description": str,
         "category": str,
         "metadata": List[str],
     },
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
 RefreshTrustedAdvisorCheckRequestRequestTypeDef = TypedDict(
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     {
         "checkId": str,
     },
 )
 
@@ -429,34 +386,14 @@
     "ResolveCaseRequestRequestTypeDef",
     {
         "caseId": str,
     },
     total=False,
 )
 
-ResolveCaseResponseTypeDef = TypedDict(
-    "ResolveCaseResponseTypeDef",
-    {
-        "initialCaseStatus": str,
-        "finalCaseStatus": str,
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
 TrustedAdvisorCostOptimizingSummaryTypeDef = TypedDict(
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     {
         "estimatedMonthlySavings": float,
         "estimatedPercentMonthlySavings": float,
     },
 )
@@ -513,19 +450,45 @@
 class AddAttachmentsToSetRequestRequestTypeDef(
     _RequiredAddAttachmentsToSetRequestRequestTypeDef,
     _OptionalAddAttachmentsToSetRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeAttachmentResponseTypeDef = TypedDict(
-    "DescribeAttachmentResponseTypeDef",
+AddAttachmentsToSetResponseTypeDef = TypedDict(
+    "AddAttachmentsToSetResponseTypeDef",
+    {
+        "attachmentSetId": str,
+        "expiryTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddCommunicationToCaseResponseTypeDef = TypedDict(
+    "AddCommunicationToCaseResponseTypeDef",
+    {
+        "result": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
+    {
+        "caseId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResolveCaseResponseTypeDef = TypedDict(
+    "ResolveCaseResponseTypeDef",
     {
-        "attachment": AttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "initialCaseStatus": str,
+        "finalCaseStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommunicationTypeDef = TypedDict(
     "CommunicationTypeDef",
     {
         "caseId": str,
@@ -533,14 +496,22 @@
         "submittedBy": str,
         "timeCreated": str,
         "attachmentSet": List[AttachmentDetailsTypeDef],
     },
     total=False,
 )
 
+DescribeAttachmentResponseTypeDef = TypedDict(
+    "DescribeAttachmentResponseTypeDef",
+    {
+        "attachment": AttachmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "code": str,
         "name": str,
         "categories": List[CategoryTypeDef],
     },
@@ -553,51 +524,90 @@
         "type": str,
         "supportedHours": List[SupportedHourTypeDef],
         "datesWithoutSupport": List[DateIntervalTypeDef],
     },
     total=False,
 )
 
+DescribeCasesRequestDescribeCasesPaginateTypeDef = TypedDict(
+    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+    {
+        "caseIdList": Sequence[str],
+        "displayId": str,
+        "afterTime": str,
+        "beforeTime": str,
+        "includeResolvedCases": bool,
+        "language": str,
+        "includeCommunications": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    {
+        "caseId": str,
+    },
+)
+_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    {
+        "beforeTime": str,
+        "afterTime": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef(
+    _RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+    _OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+):
+    pass
+
+
 DescribeSeverityLevelsResponseTypeDef = TypedDict(
     "DescribeSeverityLevelsResponseTypeDef",
     {
         "severityLevels": List[SeverityLevelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSupportedLanguagesResponseTypeDef = TypedDict(
     "DescribeSupportedLanguagesResponseTypeDef",
     {
         "supportedLanguages": List[SupportedLanguageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     {
         "statuses": List[TrustedAdvisorCheckRefreshStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RefreshTrustedAdvisorCheckResponseTypeDef = TypedDict(
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     {
         "status": TrustedAdvisorCheckRefreshStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustedAdvisorChecksResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     {
         "checks": List[TrustedAdvisorCheckDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrustedAdvisorCategorySpecificSummaryTypeDef = TypedDict(
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     {
         "costOptimizing": TrustedAdvisorCostOptimizingSummaryTypeDef,
@@ -606,15 +616,15 @@
 )
 
 DescribeCommunicationsResponseTypeDef = TypedDict(
     "DescribeCommunicationsResponseTypeDef",
     {
         "communications": List[CommunicationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecentCaseCommunicationsTypeDef = TypedDict(
     "RecentCaseCommunicationsTypeDef",
     {
         "communications": List[CommunicationTypeDef],
@@ -623,24 +633,24 @@
     total=False,
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCreateCaseOptionsResponseTypeDef = TypedDict(
     "DescribeCreateCaseOptionsResponseTypeDef",
     {
         "languageAvailability": str,
         "communicationTypes": List[CommunicationTypeOptionsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrustedAdvisorCheckResultTypeDef = TypedDict(
     "TrustedAdvisorCheckResultTypeDef",
     {
         "checkId": str,
@@ -696,27 +706,27 @@
     total=False,
 )
 
 DescribeTrustedAdvisorCheckResultResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     {
         "result": TrustedAdvisorCheckResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustedAdvisorCheckSummariesResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     {
         "summaries": List[TrustedAdvisorCheckSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCasesResponseTypeDef = TypedDict(
     "DescribeCasesResponseTypeDef",
     {
         "cases": List[CaseDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support/type_defs.pyi` & `mypy-boto3-support-1.28.12/mypy_boto3_support/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -19,53 +19,54 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttachmentTypeDef",
-    "AddAttachmentsToSetResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
-    "AddCommunicationToCaseResponseTypeDef",
     "AttachmentDetailsTypeDef",
+    "AttachmentOutputTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
     "SupportedHourTypeDef",
     "CreateCaseRequestRequestTypeDef",
-    "CreateCaseResponseTypeDef",
     "DescribeAttachmentRequestRequestTypeDef",
-    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCasesRequestRequestTypeDef",
-    "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeCommunicationsRequestRequestTypeDef",
     "DescribeCreateCaseOptionsRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "DescribeSeverityLevelsRequestRequestTypeDef",
     "SeverityLevelTypeDef",
     "DescribeSupportedLanguagesRequestRequestTypeDef",
     "SupportedLanguageTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef",
     "TrustedAdvisorCheckRefreshStatusTypeDef",
     "DescribeTrustedAdvisorCheckResultRequestRequestTypeDef",
     "DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef",
     "DescribeTrustedAdvisorChecksRequestRequestTypeDef",
     "TrustedAdvisorCheckDescriptionTypeDef",
-    "PaginatorConfigTypeDef",
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     "ResolveCaseRequestRequestTypeDef",
-    "ResolveCaseResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     "TrustedAdvisorResourceDetailTypeDef",
     "TrustedAdvisorResourcesSummaryTypeDef",
     "AddAttachmentsToSetRequestRequestTypeDef",
-    "DescribeAttachmentResponseTypeDef",
+    "AddAttachmentsToSetResponseTypeDef",
+    "AddCommunicationToCaseResponseTypeDef",
+    "CreateCaseResponseTypeDef",
+    "ResolveCaseResponseTypeDef",
     "CommunicationTypeDef",
+    "DescribeAttachmentResponseTypeDef",
     "ServiceTypeDef",
     "CommunicationTypeOptionsTypeDef",
+    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+    "DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
     "DescribeSeverityLevelsResponseTypeDef",
     "DescribeSupportedLanguagesResponseTypeDef",
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     "DescribeCommunicationsResponseTypeDef",
@@ -85,20 +86,22 @@
     {
         "fileName": str,
         "data": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-AddAttachmentsToSetResponseTypeDef = TypedDict(
-    "AddAttachmentsToSetResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "attachmentSetId": str,
-        "expiryTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredAddCommunicationToCaseRequestRequestTypeDef = TypedDict(
     "_RequiredAddCommunicationToCaseRequestRequestTypeDef",
     {
         "communicationBody": str,
@@ -116,27 +119,28 @@
 
 class AddCommunicationToCaseRequestRequestTypeDef(
     _RequiredAddCommunicationToCaseRequestRequestTypeDef,
     _OptionalAddCommunicationToCaseRequestRequestTypeDef,
 ):
     pass
 
-AddCommunicationToCaseResponseTypeDef = TypedDict(
-    "AddCommunicationToCaseResponseTypeDef",
+AttachmentDetailsTypeDef = TypedDict(
+    "AttachmentDetailsTypeDef",
     {
-        "result": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "attachmentId": str,
+        "fileName": str,
     },
+    total=False,
 )
 
-AttachmentDetailsTypeDef = TypedDict(
-    "AttachmentDetailsTypeDef",
+AttachmentOutputTypeDef = TypedDict(
+    "AttachmentOutputTypeDef",
     {
-        "attachmentId": str,
         "fileName": str,
+        "data": bytes,
     },
     total=False,
 )
 
 CategoryTypeDef = TypedDict(
     "CategoryTypeDef",
     {
@@ -186,40 +190,27 @@
 )
 
 class CreateCaseRequestRequestTypeDef(
     _RequiredCreateCaseRequestRequestTypeDef, _OptionalCreateCaseRequestRequestTypeDef
 ):
     pass
 
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAttachmentRequestRequestTypeDef = TypedDict(
     "DescribeAttachmentRequestRequestTypeDef",
     {
         "attachmentId": str,
     },
 )
 
-DescribeCasesRequestDescribeCasesPaginateTypeDef = TypedDict(
-    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "caseIdList": Sequence[str],
-        "displayId": str,
-        "afterTime": str,
-        "beforeTime": str,
-        "includeResolvedCases": bool,
-        "language": str,
-        "includeCommunications": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeCasesRequestRequestTypeDef = TypedDict(
     "DescribeCasesRequestRequestTypeDef",
     {
@@ -232,36 +223,14 @@
         "maxResults": int,
         "language": str,
         "includeCommunications": bool,
     },
     total=False,
 )
 
-_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
-    {
-        "caseId": str,
-    },
-)
-_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
-    {
-        "beforeTime": str,
-        "afterTime": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef(
-    _RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-    _OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeCommunicationsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCommunicationsRequestRequestTypeDef",
     {
         "caseId": str,
     },
 )
 _OptionalDescribeCommunicationsRequestRequestTypeDef = TypedDict(
@@ -393,24 +362,14 @@
         "name": str,
         "description": str,
         "category": str,
         "metadata": List[str],
     },
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
 RefreshTrustedAdvisorCheckRequestRequestTypeDef = TypedDict(
     "RefreshTrustedAdvisorCheckRequestRequestTypeDef",
     {
         "checkId": str,
     },
 )
 
@@ -418,34 +377,14 @@
     "ResolveCaseRequestRequestTypeDef",
     {
         "caseId": str,
     },
     total=False,
 )
 
-ResolveCaseResponseTypeDef = TypedDict(
-    "ResolveCaseResponseTypeDef",
-    {
-        "initialCaseStatus": str,
-        "finalCaseStatus": str,
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
 TrustedAdvisorCostOptimizingSummaryTypeDef = TypedDict(
     "TrustedAdvisorCostOptimizingSummaryTypeDef",
     {
         "estimatedMonthlySavings": float,
         "estimatedPercentMonthlySavings": float,
     },
 )
@@ -498,19 +437,45 @@
 
 class AddAttachmentsToSetRequestRequestTypeDef(
     _RequiredAddAttachmentsToSetRequestRequestTypeDef,
     _OptionalAddAttachmentsToSetRequestRequestTypeDef,
 ):
     pass
 
-DescribeAttachmentResponseTypeDef = TypedDict(
-    "DescribeAttachmentResponseTypeDef",
+AddAttachmentsToSetResponseTypeDef = TypedDict(
+    "AddAttachmentsToSetResponseTypeDef",
+    {
+        "attachmentSetId": str,
+        "expiryTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddCommunicationToCaseResponseTypeDef = TypedDict(
+    "AddCommunicationToCaseResponseTypeDef",
+    {
+        "result": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
+    {
+        "caseId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResolveCaseResponseTypeDef = TypedDict(
+    "ResolveCaseResponseTypeDef",
     {
-        "attachment": AttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "initialCaseStatus": str,
+        "finalCaseStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CommunicationTypeDef = TypedDict(
     "CommunicationTypeDef",
     {
         "caseId": str,
@@ -518,14 +483,22 @@
         "submittedBy": str,
         "timeCreated": str,
         "attachmentSet": List[AttachmentDetailsTypeDef],
     },
     total=False,
 )
 
+DescribeAttachmentResponseTypeDef = TypedDict(
+    "DescribeAttachmentResponseTypeDef",
+    {
+        "attachment": AttachmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "code": str,
         "name": str,
         "categories": List[CategoryTypeDef],
     },
@@ -538,51 +511,88 @@
         "type": str,
         "supportedHours": List[SupportedHourTypeDef],
         "datesWithoutSupport": List[DateIntervalTypeDef],
     },
     total=False,
 )
 
+DescribeCasesRequestDescribeCasesPaginateTypeDef = TypedDict(
+    "DescribeCasesRequestDescribeCasesPaginateTypeDef",
+    {
+        "caseIdList": Sequence[str],
+        "displayId": str,
+        "afterTime": str,
+        "beforeTime": str,
+        "includeResolvedCases": bool,
+        "language": str,
+        "includeCommunications": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    {
+        "caseId": str,
+    },
+)
+_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef",
+    {
+        "beforeTime": str,
+        "afterTime": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef(
+    _RequiredDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+    _OptionalDescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
+):
+    pass
+
 DescribeSeverityLevelsResponseTypeDef = TypedDict(
     "DescribeSeverityLevelsResponseTypeDef",
     {
         "severityLevels": List[SeverityLevelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSupportedLanguagesResponseTypeDef = TypedDict(
     "DescribeSupportedLanguagesResponseTypeDef",
     {
         "supportedLanguages": List[SupportedLanguageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef",
     {
         "statuses": List[TrustedAdvisorCheckRefreshStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RefreshTrustedAdvisorCheckResponseTypeDef = TypedDict(
     "RefreshTrustedAdvisorCheckResponseTypeDef",
     {
         "status": TrustedAdvisorCheckRefreshStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustedAdvisorChecksResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorChecksResponseTypeDef",
     {
         "checks": List[TrustedAdvisorCheckDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrustedAdvisorCategorySpecificSummaryTypeDef = TypedDict(
     "TrustedAdvisorCategorySpecificSummaryTypeDef",
     {
         "costOptimizing": TrustedAdvisorCostOptimizingSummaryTypeDef,
@@ -591,15 +601,15 @@
 )
 
 DescribeCommunicationsResponseTypeDef = TypedDict(
     "DescribeCommunicationsResponseTypeDef",
     {
         "communications": List[CommunicationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecentCaseCommunicationsTypeDef = TypedDict(
     "RecentCaseCommunicationsTypeDef",
     {
         "communications": List[CommunicationTypeDef],
@@ -608,24 +618,24 @@
     total=False,
 )
 
 DescribeServicesResponseTypeDef = TypedDict(
     "DescribeServicesResponseTypeDef",
     {
         "services": List[ServiceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCreateCaseOptionsResponseTypeDef = TypedDict(
     "DescribeCreateCaseOptionsResponseTypeDef",
     {
         "languageAvailability": str,
         "communicationTypes": List[CommunicationTypeOptionsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrustedAdvisorCheckResultTypeDef = TypedDict(
     "TrustedAdvisorCheckResultTypeDef",
     {
         "checkId": str,
@@ -679,27 +689,27 @@
     total=False,
 )
 
 DescribeTrustedAdvisorCheckResultResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckResultResponseTypeDef",
     {
         "result": TrustedAdvisorCheckResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustedAdvisorCheckSummariesResponseTypeDef = TypedDict(
     "DescribeTrustedAdvisorCheckSummariesResponseTypeDef",
     {
         "summaries": List[TrustedAdvisorCheckSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCasesResponseTypeDef = TypedDict(
     "DescribeCasesResponseTypeDef",
     {
         "cases": List[CaseDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support.egg-info/PKG-INFO` & `mypy-boto3-support-1.28.12/mypy_boto3_support.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-support
-Version: 1.28.0
-Summary: Type annotations for boto3.Support 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Support 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-support"></a>
 
 # mypy-boto3-support
 
 [![PyPI - mypy-boto3-support](https://img.shields.io/pypi/v/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-support.svg?color=blue)](https://pypi.org/project/mypy-boto3-support)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-support?color=blue)](https://pypistats.org/packages/mypy-boto3-support)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-support)](https://pepy.tech/project/mypy-boto3-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Support 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[boto3.Support 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [mypy-boto3-support docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_support/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,53 +322,54 @@
 
 `mypy_boto3_support.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_support.type_defs import (
     AttachmentTypeDef,
-    AddAttachmentsToSetResponseTypeDef,
+    ResponseMetadataTypeDef,
     AddCommunicationToCaseRequestRequestTypeDef,
-    AddCommunicationToCaseResponseTypeDef,
     AttachmentDetailsTypeDef,
+    AttachmentOutputTypeDef,
     CategoryTypeDef,
     DateIntervalTypeDef,
     SupportedHourTypeDef,
     CreateCaseRequestRequestTypeDef,
-    CreateCaseResponseTypeDef,
     DescribeAttachmentRequestRequestTypeDef,
-    DescribeCasesRequestDescribeCasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCasesRequestRequestTypeDef,
-    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeCommunicationsRequestRequestTypeDef,
     DescribeCreateCaseOptionsRequestRequestTypeDef,
     DescribeServicesRequestRequestTypeDef,
     DescribeSeverityLevelsRequestRequestTypeDef,
     SeverityLevelTypeDef,
     DescribeSupportedLanguagesRequestRequestTypeDef,
     SupportedLanguageTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef,
     TrustedAdvisorCheckRefreshStatusTypeDef,
     DescribeTrustedAdvisorCheckResultRequestRequestTypeDef,
     DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef,
     DescribeTrustedAdvisorChecksRequestRequestTypeDef,
     TrustedAdvisorCheckDescriptionTypeDef,
-    PaginatorConfigTypeDef,
     RefreshTrustedAdvisorCheckRequestRequestTypeDef,
     ResolveCaseRequestRequestTypeDef,
-    ResolveCaseResponseTypeDef,
-    ResponseMetadataTypeDef,
     TrustedAdvisorCostOptimizingSummaryTypeDef,
     TrustedAdvisorResourceDetailTypeDef,
     TrustedAdvisorResourcesSummaryTypeDef,
     AddAttachmentsToSetRequestRequestTypeDef,
-    DescribeAttachmentResponseTypeDef,
+    AddAttachmentsToSetResponseTypeDef,
+    AddCommunicationToCaseResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    ResolveCaseResponseTypeDef,
     CommunicationTypeDef,
+    DescribeAttachmentResponseTypeDef,
     ServiceTypeDef,
     CommunicationTypeOptionsTypeDef,
+    DescribeCasesRequestDescribeCasesPaginateTypeDef,
+    DescribeCommunicationsRequestDescribeCommunicationsPaginateTypeDef,
     DescribeSeverityLevelsResponseTypeDef,
     DescribeSupportedLanguagesResponseTypeDef,
     DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef,
     RefreshTrustedAdvisorCheckResponseTypeDef,
     DescribeTrustedAdvisorChecksResponseTypeDef,
     TrustedAdvisorCategorySpecificSummaryTypeDef,
     DescribeCommunicationsResponseTypeDef,
```

### Comparing `mypy-boto3-support-1.28.0/mypy_boto3_support.egg-info/SOURCES.txt` & `mypy-boto3-support-1.28.12/mypy_boto3_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-support-1.28.0/setup.py` & `mypy-boto3-support-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-support",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_support"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Support 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Support 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

