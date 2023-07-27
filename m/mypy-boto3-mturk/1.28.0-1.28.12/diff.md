# Comparing `tmp/mypy-boto3-mturk-1.28.0.tar.gz` & `tmp/mypy-boto3-mturk-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mturk-1.28.0.tar", last modified: Thu Jul  6 21:00:11 2023, max compression
+gzip compressed data, was "mypy-boto3-mturk-1.28.12.tar", last modified: Thu Jul 27 05:35:04 2023, max compression
```

## Comparing `mypy-boto3-mturk-1.28.0.tar` & `mypy-boto3-mturk-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.510378 mypy-boto3-mturk-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-06 21:00:11.502378 mypy-boto3-mturk-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.490378 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33295 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33240 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37576 2023-07-06 20:47:59.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37521 2023-07-06 20:47:59.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:58.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.502378 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-06 21:00:11.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 21:00:11.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:11.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:11.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:11.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 21:00:11.000000 mypy-boto3-mturk-1.28.0/mypy_boto3_mturk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:11.510378 mypy-boto3-mturk-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 20:47:57.000000 mypy-boto3-mturk-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.496428 mypy-boto3-mturk-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18357 2023-07-27 05:35:04.492428 mypy-boto3-mturk-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.488428 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33295 2023-07-27 05:26:48.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33240 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-27 05:26:48.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-07-27 05:26:48.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-27 05:26:48.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-27 05:26:48.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39632 2023-07-27 05:26:49.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-07-27 05:26:48.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.488428 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18357 2023-07-27 05:35:04.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:35:04.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:04.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:35:04.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:04.496428 mypy-boto3-mturk-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/setup.py
```

### Comparing `mypy-boto3-mturk-1.28.0/LICENSE` & `mypy-boto3-mturk-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.0/PKG-INFO` & `mypy-boto3-mturk-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mturk
-Version: 1.28.0
-Summary: Type annotations for boto3.MTurk 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MTurk 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mturk"></a>
 
 # mypy-boto3-mturk
 
 [![PyPI - mypy-boto3-mturk](https://img.shields.io/pypi/v/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mturk?color=blue)](https://pypistats.org/packages/mypy-boto3-mturk)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mturk)](https://pepy.tech/project/mypy-boto3-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MTurk 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[boto3.MTurk 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -414,19 +414,21 @@
     ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
     ListReviewableHITsRequestRequestTypeDef,
     ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
     ListWorkerBlocksRequestRequestTypeDef,
     WorkerBlockTypeDef,
     ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListWorkersWithQualificationTypeRequestRequestTypeDef,
+    LocaleOutputTypeDef,
     LocaleTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersFailureStatusTypeDef,
     NotifyWorkersRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    ParameterMapEntryOutputTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
@@ -438,36 +440,39 @@
     ListBonusPaymentsResponseTypeDef,
     CreateQualificationTypeResponseTypeDef,
     GetQualificationTypeResponseTypeDef,
     ListQualificationTypesResponseTypeDef,
     UpdateQualificationTypeResponseTypeDef,
     ListQualificationRequestsResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
-    QualificationRequirementTypeDef,
+    QualificationRequirementOutputTypeDef,
     QualificationTypeDef,
+    QualificationRequirementTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
+    PolicyParameterOutputTypeDef,
     PolicyParameterTypeDef,
     ReviewReportTypeDef,
-    CreateHITTypeRequestRequestTypeDef,
     HITTypeDef,
     GetQualificationScoreResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
+    CreateHITTypeRequestRequestTypeDef,
+    ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     CreateHITResponseTypeDef,
     CreateHITWithHITTypeResponseTypeDef,
     GetAssignmentResponseTypeDef,
     GetHITResponseTypeDef,
     ListHITsForQualificationTypeResponseTypeDef,
     ListHITsResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
+    ListReviewPolicyResultsForHITResponseTypeDef,
     CreateHITRequestRequestTypeDef,
     CreateHITWithHITTypeRequestRequestTypeDef,
-    ListReviewPolicyResultsForHITResponseTypeDef,
 )
 
 
 def get_structure() -> AcceptQualificationRequestRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mturk-1.28.0/README.md` & `mypy-boto3-mturk-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mturk"></a>
 
 # mypy-boto3-mturk
 
 [![PyPI - mypy-boto3-mturk](https://img.shields.io/pypi/v/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mturk?color=blue)](https://pypistats.org/packages/mypy-boto3-mturk)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mturk)](https://pepy.tech/project/mypy-boto3-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MTurk 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[boto3.MTurk 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -382,19 +382,21 @@
     ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
     ListReviewableHITsRequestRequestTypeDef,
     ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
     ListWorkerBlocksRequestRequestTypeDef,
     WorkerBlockTypeDef,
     ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListWorkersWithQualificationTypeRequestRequestTypeDef,
+    LocaleOutputTypeDef,
     LocaleTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersFailureStatusTypeDef,
     NotifyWorkersRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    ParameterMapEntryOutputTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
@@ -406,36 +408,39 @@
     ListBonusPaymentsResponseTypeDef,
     CreateQualificationTypeResponseTypeDef,
     GetQualificationTypeResponseTypeDef,
     ListQualificationTypesResponseTypeDef,
     UpdateQualificationTypeResponseTypeDef,
     ListQualificationRequestsResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
-    QualificationRequirementTypeDef,
+    QualificationRequirementOutputTypeDef,
     QualificationTypeDef,
+    QualificationRequirementTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
+    PolicyParameterOutputTypeDef,
     PolicyParameterTypeDef,
     ReviewReportTypeDef,
-    CreateHITTypeRequestRequestTypeDef,
     HITTypeDef,
     GetQualificationScoreResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
+    CreateHITTypeRequestRequestTypeDef,
+    ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     CreateHITResponseTypeDef,
     CreateHITWithHITTypeResponseTypeDef,
     GetAssignmentResponseTypeDef,
     GetHITResponseTypeDef,
     ListHITsForQualificationTypeResponseTypeDef,
     ListHITsResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
+    ListReviewPolicyResultsForHITResponseTypeDef,
     CreateHITRequestRequestTypeDef,
     CreateHITWithHITTypeRequestRequestTypeDef,
-    ListReviewPolicyResultsForHITResponseTypeDef,
 )
 
 
 def get_structure() -> AcceptQualificationRequestRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/__init__.py` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/__init__.pyi` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/__main__.py` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MTurk 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.MTurk 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk\nOther"
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

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/client.py` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/client.pyi` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/literals.py` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,15 @@
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
@@ -300,26 +301,28 @@
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

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/literals.pyi` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,15 @@
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
@@ -298,26 +299,28 @@
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

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/paginator.py` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/paginator.pyi` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/type_defs.py` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,19 +77,21 @@
     "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
     "ListReviewableHITsRequestRequestTypeDef",
     "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
     "ListWorkerBlocksRequestRequestTypeDef",
     "WorkerBlockTypeDef",
     "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListWorkersWithQualificationTypeRequestRequestTypeDef",
+    "LocaleOutputTypeDef",
     "LocaleTypeDef",
     "NotificationSpecificationTypeDef",
     "NotifyWorkersFailureStatusTypeDef",
     "NotifyWorkersRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "ParameterMapEntryOutputTypeDef",
     "ParameterMapEntryTypeDef",
     "RejectAssignmentRequestRequestTypeDef",
     "RejectQualificationRequestRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ReviewActionDetailTypeDef",
     "ReviewResultDetailTypeDef",
     "SendBonusRequestRequestTypeDef",
@@ -101,36 +103,39 @@
     "ListBonusPaymentsResponseTypeDef",
     "CreateQualificationTypeResponseTypeDef",
     "GetQualificationTypeResponseTypeDef",
     "ListQualificationTypesResponseTypeDef",
     "UpdateQualificationTypeResponseTypeDef",
     "ListQualificationRequestsResponseTypeDef",
     "ListWorkerBlocksResponseTypeDef",
-    "QualificationRequirementTypeDef",
+    "QualificationRequirementOutputTypeDef",
     "QualificationTypeDef",
+    "QualificationRequirementTypeDef",
     "SendTestEventNotificationRequestRequestTypeDef",
     "UpdateNotificationSettingsRequestRequestTypeDef",
     "NotifyWorkersResponseTypeDef",
+    "PolicyParameterOutputTypeDef",
     "PolicyParameterTypeDef",
     "ReviewReportTypeDef",
-    "CreateHITTypeRequestRequestTypeDef",
     "HITTypeDef",
     "GetQualificationScoreResponseTypeDef",
     "ListWorkersWithQualificationTypeResponseTypeDef",
+    "CreateHITTypeRequestRequestTypeDef",
+    "ReviewPolicyOutputTypeDef",
     "ReviewPolicyTypeDef",
     "CreateHITResponseTypeDef",
     "CreateHITWithHITTypeResponseTypeDef",
     "GetAssignmentResponseTypeDef",
     "GetHITResponseTypeDef",
     "ListHITsForQualificationTypeResponseTypeDef",
     "ListHITsResponseTypeDef",
     "ListReviewableHITsResponseTypeDef",
+    "ListReviewPolicyResultsForHITResponseTypeDef",
     "CreateHITRequestRequestTypeDef",
     "CreateHITWithHITTypeRequestRequestTypeDef",
-    "ListReviewPolicyResultsForHITResponseTypeDef",
 )
 
 _RequiredAcceptQualificationRequestRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptQualificationRequestRequestRequestTypeDef",
     {
         "QualificationRequestId": str,
     },
@@ -764,14 +769,33 @@
 class ListWorkersWithQualificationTypeRequestRequestTypeDef(
     _RequiredListWorkersWithQualificationTypeRequestRequestTypeDef,
     _OptionalListWorkersWithQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredLocaleOutputTypeDef = TypedDict(
+    "_RequiredLocaleOutputTypeDef",
+    {
+        "Country": str,
+    },
+)
+_OptionalLocaleOutputTypeDef = TypedDict(
+    "_OptionalLocaleOutputTypeDef",
+    {
+        "Subdivision": str,
+    },
+    total=False,
+)
+
+
+class LocaleOutputTypeDef(_RequiredLocaleOutputTypeDef, _OptionalLocaleOutputTypeDef):
+    pass
+
+
 _RequiredLocaleTypeDef = TypedDict(
     "_RequiredLocaleTypeDef",
     {
         "Country": str,
     },
 )
 _OptionalLocaleTypeDef = TypedDict(
@@ -822,14 +846,23 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ParameterMapEntryOutputTypeDef = TypedDict(
+    "ParameterMapEntryOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+    },
+    total=False,
+)
+
 ParameterMapEntryTypeDef = TypedDict(
     "ParameterMapEntryTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -1065,52 +1098,77 @@
         "NextToken": str,
         "NumResults": int,
         "WorkerBlocks": List[WorkerBlockTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredQualificationRequirementTypeDef = TypedDict(
-    "_RequiredQualificationRequirementTypeDef",
+_RequiredQualificationRequirementOutputTypeDef = TypedDict(
+    "_RequiredQualificationRequirementOutputTypeDef",
     {
         "QualificationTypeId": str,
         "Comparator": ComparatorType,
     },
 )
-_OptionalQualificationRequirementTypeDef = TypedDict(
-    "_OptionalQualificationRequirementTypeDef",
+_OptionalQualificationRequirementOutputTypeDef = TypedDict(
+    "_OptionalQualificationRequirementOutputTypeDef",
     {
-        "IntegerValues": Sequence[int],
-        "LocaleValues": Sequence[LocaleTypeDef],
+        "IntegerValues": List[int],
+        "LocaleValues": List[LocaleOutputTypeDef],
         "RequiredToPreview": bool,
         "ActionsGuarded": HITAccessActionsType,
     },
     total=False,
 )
 
 
-class QualificationRequirementTypeDef(
-    _RequiredQualificationRequirementTypeDef, _OptionalQualificationRequirementTypeDef
+class QualificationRequirementOutputTypeDef(
+    _RequiredQualificationRequirementOutputTypeDef, _OptionalQualificationRequirementOutputTypeDef
 ):
     pass
 
 
 QualificationTypeDef = TypedDict(
     "QualificationTypeDef",
     {
         "QualificationTypeId": str,
         "WorkerId": str,
         "GrantTime": datetime,
         "IntegerValue": int,
-        "LocaleValue": LocaleTypeDef,
+        "LocaleValue": LocaleOutputTypeDef,
         "Status": QualificationStatusType,
     },
     total=False,
 )
 
+_RequiredQualificationRequirementTypeDef = TypedDict(
+    "_RequiredQualificationRequirementTypeDef",
+    {
+        "QualificationTypeId": str,
+        "Comparator": ComparatorType,
+    },
+)
+_OptionalQualificationRequirementTypeDef = TypedDict(
+    "_OptionalQualificationRequirementTypeDef",
+    {
+        "IntegerValues": Sequence[int],
+        "LocaleValues": Sequence[LocaleTypeDef],
+        "RequiredToPreview": bool,
+        "ActionsGuarded": HITAccessActionsType,
+    },
+    total=False,
+)
+
+
+class QualificationRequirementTypeDef(
+    _RequiredQualificationRequirementTypeDef, _OptionalQualificationRequirementTypeDef
+):
+    pass
+
+
 SendTestEventNotificationRequestRequestTypeDef = TypedDict(
     "SendTestEventNotificationRequestRequestTypeDef",
     {
         "Notification": NotificationSpecificationTypeDef,
         "TestEventType": EventTypeType,
     },
 )
@@ -1142,14 +1200,24 @@
     "NotifyWorkersResponseTypeDef",
     {
         "NotifyWorkersFailureStatuses": List[NotifyWorkersFailureStatusTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PolicyParameterOutputTypeDef = TypedDict(
+    "PolicyParameterOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+        "MapEntries": List[ParameterMapEntryOutputTypeDef],
+    },
+    total=False,
+)
+
 PolicyParameterTypeDef = TypedDict(
     "PolicyParameterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "MapEntries": Sequence[ParameterMapEntryTypeDef],
     },
@@ -1161,40 +1229,14 @@
     {
         "ReviewResults": List[ReviewResultDetailTypeDef],
         "ReviewActions": List[ReviewActionDetailTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHITTypeRequestRequestTypeDef",
-    {
-        "AssignmentDurationInSeconds": int,
-        "Reward": str,
-        "Title": str,
-        "Description": str,
-    },
-)
-_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHITTypeRequestRequestTypeDef",
-    {
-        "AutoApprovalDelayInSeconds": int,
-        "Keywords": str,
-        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateHITTypeRequestRequestTypeDef(
-    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
-):
-    pass
-
-
 HITTypeDef = TypedDict(
     "HITTypeDef",
     {
         "HITId": str,
         "HITTypeId": str,
         "HITGroupId": str,
         "HITLayoutId": str,
@@ -1206,15 +1248,15 @@
         "HITStatus": HITStatusType,
         "MaxAssignments": int,
         "Reward": str,
         "AutoApprovalDelayInSeconds": int,
         "Expiration": datetime,
         "AssignmentDurationInSeconds": int,
         "RequesterAnnotation": str,
-        "QualificationRequirements": List[QualificationRequirementTypeDef],
+        "QualificationRequirements": List[QualificationRequirementOutputTypeDef],
         "HITReviewStatus": HITReviewStatusType,
         "NumberOfAssignmentsPending": int,
         "NumberOfAssignmentsAvailable": int,
         "NumberOfAssignmentsCompleted": int,
     },
     total=False,
 )
@@ -1233,14 +1275,61 @@
         "NextToken": str,
         "NumResults": int,
         "Qualifications": List[QualificationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHITTypeRequestRequestTypeDef",
+    {
+        "AssignmentDurationInSeconds": int,
+        "Reward": str,
+        "Title": str,
+        "Description": str,
+    },
+)
+_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHITTypeRequestRequestTypeDef",
+    {
+        "AutoApprovalDelayInSeconds": int,
+        "Keywords": str,
+        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateHITTypeRequestRequestTypeDef(
+    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredReviewPolicyOutputTypeDef = TypedDict(
+    "_RequiredReviewPolicyOutputTypeDef",
+    {
+        "PolicyName": str,
+    },
+)
+_OptionalReviewPolicyOutputTypeDef = TypedDict(
+    "_OptionalReviewPolicyOutputTypeDef",
+    {
+        "Parameters": List[PolicyParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ReviewPolicyOutputTypeDef(
+    _RequiredReviewPolicyOutputTypeDef, _OptionalReviewPolicyOutputTypeDef
+):
+    pass
+
+
 _RequiredReviewPolicyTypeDef = TypedDict(
     "_RequiredReviewPolicyTypeDef",
     {
         "PolicyName": str,
     },
 )
 _OptionalReviewPolicyTypeDef = TypedDict(
@@ -1315,14 +1404,27 @@
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
+    "ListReviewPolicyResultsForHITResponseTypeDef",
+    {
+        "HITId": str,
+        "AssignmentReviewPolicy": ReviewPolicyOutputTypeDef,
+        "HITReviewPolicy": ReviewPolicyOutputTypeDef,
+        "AssignmentReviewReport": ReviewReportTypeDef,
+        "HITReviewReport": ReviewReportTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateHITRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHITRequestRequestTypeDef",
     {
         "LifetimeInSeconds": int,
         "AssignmentDurationInSeconds": int,
         "Reward": str,
         "Title": str,
@@ -1378,21 +1480,7 @@
 
 
 class CreateHITWithHITTypeRequestRequestTypeDef(
     _RequiredCreateHITWithHITTypeRequestRequestTypeDef,
     _OptionalCreateHITWithHITTypeRequestRequestTypeDef,
 ):
     pass
-
-
-ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
-    "ListReviewPolicyResultsForHITResponseTypeDef",
-    {
-        "HITId": str,
-        "AssignmentReviewPolicy": ReviewPolicyTypeDef,
-        "HITReviewPolicy": ReviewPolicyTypeDef,
-        "AssignmentReviewReport": ReviewReportTypeDef,
-        "HITReviewReport": ReviewReportTypeDef,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk/type_defs.pyi` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -76,19 +76,21 @@
     "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
     "ListReviewableHITsRequestRequestTypeDef",
     "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
     "ListWorkerBlocksRequestRequestTypeDef",
     "WorkerBlockTypeDef",
     "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListWorkersWithQualificationTypeRequestRequestTypeDef",
+    "LocaleOutputTypeDef",
     "LocaleTypeDef",
     "NotificationSpecificationTypeDef",
     "NotifyWorkersFailureStatusTypeDef",
     "NotifyWorkersRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "ParameterMapEntryOutputTypeDef",
     "ParameterMapEntryTypeDef",
     "RejectAssignmentRequestRequestTypeDef",
     "RejectQualificationRequestRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ReviewActionDetailTypeDef",
     "ReviewResultDetailTypeDef",
     "SendBonusRequestRequestTypeDef",
@@ -100,36 +102,39 @@
     "ListBonusPaymentsResponseTypeDef",
     "CreateQualificationTypeResponseTypeDef",
     "GetQualificationTypeResponseTypeDef",
     "ListQualificationTypesResponseTypeDef",
     "UpdateQualificationTypeResponseTypeDef",
     "ListQualificationRequestsResponseTypeDef",
     "ListWorkerBlocksResponseTypeDef",
-    "QualificationRequirementTypeDef",
+    "QualificationRequirementOutputTypeDef",
     "QualificationTypeDef",
+    "QualificationRequirementTypeDef",
     "SendTestEventNotificationRequestRequestTypeDef",
     "UpdateNotificationSettingsRequestRequestTypeDef",
     "NotifyWorkersResponseTypeDef",
+    "PolicyParameterOutputTypeDef",
     "PolicyParameterTypeDef",
     "ReviewReportTypeDef",
-    "CreateHITTypeRequestRequestTypeDef",
     "HITTypeDef",
     "GetQualificationScoreResponseTypeDef",
     "ListWorkersWithQualificationTypeResponseTypeDef",
+    "CreateHITTypeRequestRequestTypeDef",
+    "ReviewPolicyOutputTypeDef",
     "ReviewPolicyTypeDef",
     "CreateHITResponseTypeDef",
     "CreateHITWithHITTypeResponseTypeDef",
     "GetAssignmentResponseTypeDef",
     "GetHITResponseTypeDef",
     "ListHITsForQualificationTypeResponseTypeDef",
     "ListHITsResponseTypeDef",
     "ListReviewableHITsResponseTypeDef",
+    "ListReviewPolicyResultsForHITResponseTypeDef",
     "CreateHITRequestRequestTypeDef",
     "CreateHITWithHITTypeRequestRequestTypeDef",
-    "ListReviewPolicyResultsForHITResponseTypeDef",
 )
 
 _RequiredAcceptQualificationRequestRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptQualificationRequestRequestRequestTypeDef",
     {
         "QualificationRequestId": str,
     },
@@ -731,14 +736,31 @@
 
 class ListWorkersWithQualificationTypeRequestRequestTypeDef(
     _RequiredListWorkersWithQualificationTypeRequestRequestTypeDef,
     _OptionalListWorkersWithQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
+_RequiredLocaleOutputTypeDef = TypedDict(
+    "_RequiredLocaleOutputTypeDef",
+    {
+        "Country": str,
+    },
+)
+_OptionalLocaleOutputTypeDef = TypedDict(
+    "_OptionalLocaleOutputTypeDef",
+    {
+        "Subdivision": str,
+    },
+    total=False,
+)
+
+class LocaleOutputTypeDef(_RequiredLocaleOutputTypeDef, _OptionalLocaleOutputTypeDef):
+    pass
+
 _RequiredLocaleTypeDef = TypedDict(
     "_RequiredLocaleTypeDef",
     {
         "Country": str,
     },
 )
 _OptionalLocaleTypeDef = TypedDict(
@@ -787,14 +809,23 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ParameterMapEntryOutputTypeDef = TypedDict(
+    "ParameterMapEntryOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+    },
+    total=False,
+)
+
 ParameterMapEntryTypeDef = TypedDict(
     "ParameterMapEntryTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -1022,50 +1053,73 @@
         "NextToken": str,
         "NumResults": int,
         "WorkerBlocks": List[WorkerBlockTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredQualificationRequirementTypeDef = TypedDict(
-    "_RequiredQualificationRequirementTypeDef",
+_RequiredQualificationRequirementOutputTypeDef = TypedDict(
+    "_RequiredQualificationRequirementOutputTypeDef",
     {
         "QualificationTypeId": str,
         "Comparator": ComparatorType,
     },
 )
-_OptionalQualificationRequirementTypeDef = TypedDict(
-    "_OptionalQualificationRequirementTypeDef",
+_OptionalQualificationRequirementOutputTypeDef = TypedDict(
+    "_OptionalQualificationRequirementOutputTypeDef",
     {
-        "IntegerValues": Sequence[int],
-        "LocaleValues": Sequence[LocaleTypeDef],
+        "IntegerValues": List[int],
+        "LocaleValues": List[LocaleOutputTypeDef],
         "RequiredToPreview": bool,
         "ActionsGuarded": HITAccessActionsType,
     },
     total=False,
 )
 
-class QualificationRequirementTypeDef(
-    _RequiredQualificationRequirementTypeDef, _OptionalQualificationRequirementTypeDef
+class QualificationRequirementOutputTypeDef(
+    _RequiredQualificationRequirementOutputTypeDef, _OptionalQualificationRequirementOutputTypeDef
 ):
     pass
 
 QualificationTypeDef = TypedDict(
     "QualificationTypeDef",
     {
         "QualificationTypeId": str,
         "WorkerId": str,
         "GrantTime": datetime,
         "IntegerValue": int,
-        "LocaleValue": LocaleTypeDef,
+        "LocaleValue": LocaleOutputTypeDef,
         "Status": QualificationStatusType,
     },
     total=False,
 )
 
+_RequiredQualificationRequirementTypeDef = TypedDict(
+    "_RequiredQualificationRequirementTypeDef",
+    {
+        "QualificationTypeId": str,
+        "Comparator": ComparatorType,
+    },
+)
+_OptionalQualificationRequirementTypeDef = TypedDict(
+    "_OptionalQualificationRequirementTypeDef",
+    {
+        "IntegerValues": Sequence[int],
+        "LocaleValues": Sequence[LocaleTypeDef],
+        "RequiredToPreview": bool,
+        "ActionsGuarded": HITAccessActionsType,
+    },
+    total=False,
+)
+
+class QualificationRequirementTypeDef(
+    _RequiredQualificationRequirementTypeDef, _OptionalQualificationRequirementTypeDef
+):
+    pass
+
 SendTestEventNotificationRequestRequestTypeDef = TypedDict(
     "SendTestEventNotificationRequestRequestTypeDef",
     {
         "Notification": NotificationSpecificationTypeDef,
         "TestEventType": EventTypeType,
     },
 )
@@ -1095,14 +1149,24 @@
     "NotifyWorkersResponseTypeDef",
     {
         "NotifyWorkersFailureStatuses": List[NotifyWorkersFailureStatusTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PolicyParameterOutputTypeDef = TypedDict(
+    "PolicyParameterOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+        "MapEntries": List[ParameterMapEntryOutputTypeDef],
+    },
+    total=False,
+)
+
 PolicyParameterTypeDef = TypedDict(
     "PolicyParameterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "MapEntries": Sequence[ParameterMapEntryTypeDef],
     },
@@ -1114,38 +1178,14 @@
     {
         "ReviewResults": List[ReviewResultDetailTypeDef],
         "ReviewActions": List[ReviewActionDetailTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHITTypeRequestRequestTypeDef",
-    {
-        "AssignmentDurationInSeconds": int,
-        "Reward": str,
-        "Title": str,
-        "Description": str,
-    },
-)
-_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHITTypeRequestRequestTypeDef",
-    {
-        "AutoApprovalDelayInSeconds": int,
-        "Keywords": str,
-        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
-    },
-    total=False,
-)
-
-class CreateHITTypeRequestRequestTypeDef(
-    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
-):
-    pass
-
 HITTypeDef = TypedDict(
     "HITTypeDef",
     {
         "HITId": str,
         "HITTypeId": str,
         "HITGroupId": str,
         "HITLayoutId": str,
@@ -1157,15 +1197,15 @@
         "HITStatus": HITStatusType,
         "MaxAssignments": int,
         "Reward": str,
         "AutoApprovalDelayInSeconds": int,
         "Expiration": datetime,
         "AssignmentDurationInSeconds": int,
         "RequesterAnnotation": str,
-        "QualificationRequirements": List[QualificationRequirementTypeDef],
+        "QualificationRequirements": List[QualificationRequirementOutputTypeDef],
         "HITReviewStatus": HITReviewStatusType,
         "NumberOfAssignmentsPending": int,
         "NumberOfAssignmentsAvailable": int,
         "NumberOfAssignmentsCompleted": int,
     },
     total=False,
 )
@@ -1184,14 +1224,57 @@
         "NextToken": str,
         "NumResults": int,
         "Qualifications": List[QualificationTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHITTypeRequestRequestTypeDef",
+    {
+        "AssignmentDurationInSeconds": int,
+        "Reward": str,
+        "Title": str,
+        "Description": str,
+    },
+)
+_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHITTypeRequestRequestTypeDef",
+    {
+        "AutoApprovalDelayInSeconds": int,
+        "Keywords": str,
+        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
+    },
+    total=False,
+)
+
+class CreateHITTypeRequestRequestTypeDef(
+    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
+):
+    pass
+
+_RequiredReviewPolicyOutputTypeDef = TypedDict(
+    "_RequiredReviewPolicyOutputTypeDef",
+    {
+        "PolicyName": str,
+    },
+)
+_OptionalReviewPolicyOutputTypeDef = TypedDict(
+    "_OptionalReviewPolicyOutputTypeDef",
+    {
+        "Parameters": List[PolicyParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+class ReviewPolicyOutputTypeDef(
+    _RequiredReviewPolicyOutputTypeDef, _OptionalReviewPolicyOutputTypeDef
+):
+    pass
+
 _RequiredReviewPolicyTypeDef = TypedDict(
     "_RequiredReviewPolicyTypeDef",
     {
         "PolicyName": str,
     },
 )
 _OptionalReviewPolicyTypeDef = TypedDict(
@@ -1264,14 +1347,27 @@
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
+    "ListReviewPolicyResultsForHITResponseTypeDef",
+    {
+        "HITId": str,
+        "AssignmentReviewPolicy": ReviewPolicyOutputTypeDef,
+        "HITReviewPolicy": ReviewPolicyOutputTypeDef,
+        "AssignmentReviewReport": ReviewReportTypeDef,
+        "HITReviewReport": ReviewReportTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateHITRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHITRequestRequestTypeDef",
     {
         "LifetimeInSeconds": int,
         "AssignmentDurationInSeconds": int,
         "Reward": str,
         "Title": str,
@@ -1324,20 +1420,7 @@
 )
 
 class CreateHITWithHITTypeRequestRequestTypeDef(
     _RequiredCreateHITWithHITTypeRequestRequestTypeDef,
     _OptionalCreateHITWithHITTypeRequestRequestTypeDef,
 ):
     pass
-
-ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
-    "ListReviewPolicyResultsForHITResponseTypeDef",
-    {
-        "HITId": str,
-        "AssignmentReviewPolicy": ReviewPolicyTypeDef,
-        "HITReviewPolicy": ReviewPolicyTypeDef,
-        "AssignmentReviewReport": ReviewReportTypeDef,
-        "HITReviewReport": ReviewReportTypeDef,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk.egg-info/PKG-INFO` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mturk
-Version: 1.28.0
-Summary: Type annotations for boto3.MTurk 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MTurk 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mturk"></a>
 
 # mypy-boto3-mturk
 
 [![PyPI - mypy-boto3-mturk](https://img.shields.io/pypi/v/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mturk?color=blue)](https://pypistats.org/packages/mypy-boto3-mturk)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mturk)](https://pepy.tech/project/mypy-boto3-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MTurk 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[boto3.MTurk 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -414,19 +414,21 @@
     ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
     ListReviewableHITsRequestRequestTypeDef,
     ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
     ListWorkerBlocksRequestRequestTypeDef,
     WorkerBlockTypeDef,
     ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListWorkersWithQualificationTypeRequestRequestTypeDef,
+    LocaleOutputTypeDef,
     LocaleTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersFailureStatusTypeDef,
     NotifyWorkersRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    ParameterMapEntryOutputTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
@@ -438,36 +440,39 @@
     ListBonusPaymentsResponseTypeDef,
     CreateQualificationTypeResponseTypeDef,
     GetQualificationTypeResponseTypeDef,
     ListQualificationTypesResponseTypeDef,
     UpdateQualificationTypeResponseTypeDef,
     ListQualificationRequestsResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
-    QualificationRequirementTypeDef,
+    QualificationRequirementOutputTypeDef,
     QualificationTypeDef,
+    QualificationRequirementTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
+    PolicyParameterOutputTypeDef,
     PolicyParameterTypeDef,
     ReviewReportTypeDef,
-    CreateHITTypeRequestRequestTypeDef,
     HITTypeDef,
     GetQualificationScoreResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
+    CreateHITTypeRequestRequestTypeDef,
+    ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     CreateHITResponseTypeDef,
     CreateHITWithHITTypeResponseTypeDef,
     GetAssignmentResponseTypeDef,
     GetHITResponseTypeDef,
     ListHITsForQualificationTypeResponseTypeDef,
     ListHITsResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
+    ListReviewPolicyResultsForHITResponseTypeDef,
     CreateHITRequestRequestTypeDef,
     CreateHITWithHITTypeRequestRequestTypeDef,
-    ListReviewPolicyResultsForHITResponseTypeDef,
 )
 
 
 def get_structure() -> AcceptQualificationRequestRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mturk-1.28.0/mypy_boto3_mturk.egg-info/SOURCES.txt` & `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.0/setup.py` & `mypy-boto3-mturk-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mturk",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_mturk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MTurk 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MTurk 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

