# Comparing `tmp/mypy-boto3-textract-1.28.0.tar.gz` & `tmp/mypy-boto3-textract-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-textract-1.28.0.tar", last modified: Thu Jul  6 21:00:46 2023, max compression
+gzip compressed data, was "mypy-boto3-textract-1.28.12.tar", last modified: Thu Jul 27 11:49:46 2023, max compression
```

## Comparing `mypy-boto3-textract-1.28.0.tar` & `mypy-boto3-textract-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.494449 mypy-boto3-textract-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:06.000000 mypy-boto3-textract-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-07-06 21:00:46.494449 mypy-boto3-textract-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-07-06 20:57:06.000000 mypy-boto3-textract-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.490449 mypy-boto3-textract-1.28.0/mypy_boto3_textract/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 20:57:06.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-06 20:57:06.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:57:06.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-07-06 20:57:06.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-07-06 20:57:06.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-06 20:57:07.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-07-06 20:57:07.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:06.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22944 2023-07-06 20:57:11.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-07-06 20:57:11.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:06.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.490449 mypy-boto3-textract-1.28.0/mypy_boto3_textract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-07-06 21:00:46.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 21:00:46.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:46.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:46.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:46.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:46.000000 mypy-boto3-textract-1.28.0/mypy_boto3_textract.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:46.494449 mypy-boto3-textract-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:57:06.000000 mypy-boto3-textract-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.401432 mypy-boto3-textract-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-07-27 11:49:46.397432 mypy-boto3-textract-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.385431 mypy-boto3-textract-1.28.12/mypy_boto3_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23317 2023-07-27 11:47:57.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23288 2023-07-27 11:47:57.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.397432 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-07-27 11:49:46.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 11:49:46.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:46.000000 mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:46.401432 mypy-boto3-textract-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:47:56.000000 mypy-boto3-textract-1.28.12/setup.py
```

### Comparing `mypy-boto3-textract-1.28.0/LICENSE` & `mypy-boto3-textract-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.28.0/PKG-INFO` & `mypy-boto3-textract-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-textract
-Version: 1.28.0
-Summary: Type annotations for boto3.Textract 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Textract 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-textract"></a>
 
 # mypy-boto3-textract
 
 [![PyPI - mypy-boto3-textract](https://img.shields.io/pypi/v/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-textract?color=blue)](https://pypistats.org/packages/mypy-boto3-textract)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-textract)](https://pepy.tech/project/mypy-boto3-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Textract 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
+[boto3.Textract 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
 [mypy-boto3-textract docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,16 +306,17 @@
 `mypy_boto3_textract.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_textract.type_defs import (
     DocumentMetadataTypeDef,
     HumanLoopActivationOutputTypeDef,
+    ResponseMetadataTypeDef,
     NormalizedValueTypeDef,
-    QueryTypeDef,
+    QueryOutputTypeDef,
     RelationshipTypeDef,
     BoundingBoxTypeDef,
     DetectedSignatureTypeDef,
     SplitDocumentTypeDef,
     UndetectedSignatureTypeDef,
     S3ObjectTypeDef,
     ExpenseCurrencyTypeDef,
@@ -328,41 +329,41 @@
     GetExpenseAnalysisRequestRequestTypeDef,
     GetLendingAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryRequestRequestTypeDef,
     HumanLoopDataAttributesTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     PredictionTypeDef,
-    ResponseMetadataTypeDef,
+    QueryTypeDef,
     StartDocumentAnalysisResponseTypeDef,
     StartDocumentTextDetectionResponseTypeDef,
     StartExpenseAnalysisResponseTypeDef,
     StartLendingAnalysisResponseTypeDef,
     AnalyzeIDDetectionsTypeDef,
-    QueriesConfigTypeDef,
     DocumentGroupTypeDef,
     DocumentLocationTypeDef,
     DocumentTypeDef,
     GeometryTypeDef,
     HumanLoopConfigTypeDef,
     PageClassificationTypeDef,
+    QueriesConfigTypeDef,
     IdentityDocumentFieldTypeDef,
     LendingSummaryTypeDef,
-    StartDocumentAnalysisRequestRequestTypeDef,
     StartDocumentTextDetectionRequestRequestTypeDef,
     StartExpenseAnalysisRequestRequestTypeDef,
     StartLendingAnalysisRequestRequestTypeDef,
     AnalyzeExpenseRequestRequestTypeDef,
     AnalyzeIDRequestRequestTypeDef,
     DetectDocumentTextRequestRequestTypeDef,
     BlockTypeDef,
     ExpenseDetectionTypeDef,
     LendingDetectionTypeDef,
     SignatureDetectionTypeDef,
     AnalyzeDocumentRequestRequestTypeDef,
+    StartDocumentAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryResponseTypeDef,
     AnalyzeDocumentResponseTypeDef,
     DetectDocumentTextResponseTypeDef,
     GetDocumentAnalysisResponseTypeDef,
     GetDocumentTextDetectionResponseTypeDef,
     IdentityDocumentTypeDef,
     ExpenseFieldTypeDef,
```

### Comparing `mypy-boto3-textract-1.28.0/README.md` & `mypy-boto3-textract-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-textract"></a>
 
 # mypy-boto3-textract
 
 [![PyPI - mypy-boto3-textract](https://img.shields.io/pypi/v/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-textract?color=blue)](https://pypistats.org/packages/mypy-boto3-textract)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-textract)](https://pepy.tech/project/mypy-boto3-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Textract 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
+[boto3.Textract 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
 [mypy-boto3-textract docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/).
 
 See how it helps to find and fix potential bugs:
 
@@ -274,16 +274,17 @@
 `mypy_boto3_textract.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_textract.type_defs import (
     DocumentMetadataTypeDef,
     HumanLoopActivationOutputTypeDef,
+    ResponseMetadataTypeDef,
     NormalizedValueTypeDef,
-    QueryTypeDef,
+    QueryOutputTypeDef,
     RelationshipTypeDef,
     BoundingBoxTypeDef,
     DetectedSignatureTypeDef,
     SplitDocumentTypeDef,
     UndetectedSignatureTypeDef,
     S3ObjectTypeDef,
     ExpenseCurrencyTypeDef,
@@ -296,41 +297,41 @@
     GetExpenseAnalysisRequestRequestTypeDef,
     GetLendingAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryRequestRequestTypeDef,
     HumanLoopDataAttributesTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     PredictionTypeDef,
-    ResponseMetadataTypeDef,
+    QueryTypeDef,
     StartDocumentAnalysisResponseTypeDef,
     StartDocumentTextDetectionResponseTypeDef,
     StartExpenseAnalysisResponseTypeDef,
     StartLendingAnalysisResponseTypeDef,
     AnalyzeIDDetectionsTypeDef,
-    QueriesConfigTypeDef,
     DocumentGroupTypeDef,
     DocumentLocationTypeDef,
     DocumentTypeDef,
     GeometryTypeDef,
     HumanLoopConfigTypeDef,
     PageClassificationTypeDef,
+    QueriesConfigTypeDef,
     IdentityDocumentFieldTypeDef,
     LendingSummaryTypeDef,
-    StartDocumentAnalysisRequestRequestTypeDef,
     StartDocumentTextDetectionRequestRequestTypeDef,
     StartExpenseAnalysisRequestRequestTypeDef,
     StartLendingAnalysisRequestRequestTypeDef,
     AnalyzeExpenseRequestRequestTypeDef,
     AnalyzeIDRequestRequestTypeDef,
     DetectDocumentTextRequestRequestTypeDef,
     BlockTypeDef,
     ExpenseDetectionTypeDef,
     LendingDetectionTypeDef,
     SignatureDetectionTypeDef,
     AnalyzeDocumentRequestRequestTypeDef,
+    StartDocumentAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryResponseTypeDef,
     AnalyzeDocumentResponseTypeDef,
     DetectDocumentTextResponseTypeDef,
     GetDocumentAnalysisResponseTypeDef,
     GetDocumentTextDetectionResponseTypeDef,
     IdentityDocumentTypeDef,
     ExpenseFieldTypeDef,
```

### Comparing `mypy-boto3-textract-1.28.0/mypy_boto3_textract/__main__.py` & `mypy-boto3-textract-1.28.12/mypy_boto3_textract/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Textract 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Textract 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract\nOther"
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

### Comparing `mypy-boto3-textract-1.28.0/mypy_boto3_textract/client.py` & `mypy-boto3-textract-1.28.12/mypy_boto3_textract/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.28.0/mypy_boto3_textract/client.pyi` & `mypy-boto3-textract-1.28.12/mypy_boto3_textract/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.28.0/mypy_boto3_textract/literals.py` & `mypy-boto3-textract-1.28.12/mypy_boto3_textract/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
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
@@ -282,26 +283,28 @@
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

### Comparing `mypy-boto3-textract-1.28.0/mypy_boto3_textract/literals.pyi` & `mypy-boto3-textract-1.28.12/mypy_boto3_textract/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,15 @@
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
@@ -280,26 +281,28 @@
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

### Comparing `mypy-boto3-textract-1.28.0/mypy_boto3_textract/type_defs.py` & `mypy-boto3-textract-1.28.12/mypy_boto3_textract/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,17 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DocumentMetadataTypeDef",
     "HumanLoopActivationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "NormalizedValueTypeDef",
-    "QueryTypeDef",
+    "QueryOutputTypeDef",
     "RelationshipTypeDef",
     "BoundingBoxTypeDef",
     "DetectedSignatureTypeDef",
     "SplitDocumentTypeDef",
     "UndetectedSignatureTypeDef",
     "S3ObjectTypeDef",
     "ExpenseCurrencyTypeDef",
@@ -58,41 +59,41 @@
     "GetExpenseAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryRequestRequestTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "NotificationChannelTypeDef",
     "OutputConfigTypeDef",
     "PredictionTypeDef",
-    "ResponseMetadataTypeDef",
+    "QueryTypeDef",
     "StartDocumentAnalysisResponseTypeDef",
     "StartDocumentTextDetectionResponseTypeDef",
     "StartExpenseAnalysisResponseTypeDef",
     "StartLendingAnalysisResponseTypeDef",
     "AnalyzeIDDetectionsTypeDef",
-    "QueriesConfigTypeDef",
     "DocumentGroupTypeDef",
     "DocumentLocationTypeDef",
     "DocumentTypeDef",
     "GeometryTypeDef",
     "HumanLoopConfigTypeDef",
     "PageClassificationTypeDef",
+    "QueriesConfigTypeDef",
     "IdentityDocumentFieldTypeDef",
     "LendingSummaryTypeDef",
-    "StartDocumentAnalysisRequestRequestTypeDef",
     "StartDocumentTextDetectionRequestRequestTypeDef",
     "StartExpenseAnalysisRequestRequestTypeDef",
     "StartLendingAnalysisRequestRequestTypeDef",
     "AnalyzeExpenseRequestRequestTypeDef",
     "AnalyzeIDRequestRequestTypeDef",
     "DetectDocumentTextRequestRequestTypeDef",
     "BlockTypeDef",
     "ExpenseDetectionTypeDef",
     "LendingDetectionTypeDef",
     "SignatureDetectionTypeDef",
     "AnalyzeDocumentRequestRequestTypeDef",
+    "StartDocumentAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryResponseTypeDef",
     "AnalyzeDocumentResponseTypeDef",
     "DetectDocumentTextResponseTypeDef",
     "GetDocumentAnalysisResponseTypeDef",
     "GetDocumentTextDetectionResponseTypeDef",
     "IdentityDocumentTypeDef",
     "ExpenseFieldTypeDef",
@@ -123,40 +124,51 @@
         "HumanLoopArn": str,
         "HumanLoopActivationReasons": List[str],
         "HumanLoopActivationConditionsEvaluationResults": str,
     },
     total=False,
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
 NormalizedValueTypeDef = TypedDict(
     "NormalizedValueTypeDef",
     {
         "Value": str,
         "ValueType": Literal["DATE"],
     },
     total=False,
 )
 
-_RequiredQueryTypeDef = TypedDict(
-    "_RequiredQueryTypeDef",
+_RequiredQueryOutputTypeDef = TypedDict(
+    "_RequiredQueryOutputTypeDef",
     {
         "Text": str,
     },
 )
-_OptionalQueryTypeDef = TypedDict(
-    "_OptionalQueryTypeDef",
+_OptionalQueryOutputTypeDef = TypedDict(
+    "_OptionalQueryOutputTypeDef",
     {
         "Alias": str,
-        "Pages": Sequence[str],
+        "Pages": List[str],
     },
     total=False,
 )
 
 
-class QueryTypeDef(_RequiredQueryTypeDef, _OptionalQueryTypeDef):
+class QueryOutputTypeDef(_RequiredQueryOutputTypeDef, _OptionalQueryOutputTypeDef):
     pass
 
 
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "Type": RelationshipTypeType,
@@ -395,54 +407,63 @@
     {
         "Value": str,
         "Confidence": float,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredQueryTypeDef = TypedDict(
+    "_RequiredQueryTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Text": str,
     },
 )
+_OptionalQueryTypeDef = TypedDict(
+    "_OptionalQueryTypeDef",
+    {
+        "Alias": str,
+        "Pages": Sequence[str],
+    },
+    total=False,
+)
+
+
+class QueryTypeDef(_RequiredQueryTypeDef, _OptionalQueryTypeDef):
+    pass
+
 
 StartDocumentAnalysisResponseTypeDef = TypedDict(
     "StartDocumentAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDocumentTextDetectionResponseTypeDef = TypedDict(
     "StartDocumentTextDetectionResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartExpenseAnalysisResponseTypeDef = TypedDict(
     "StartExpenseAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartLendingAnalysisResponseTypeDef = TypedDict(
     "StartLendingAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAnalyzeIDDetectionsTypeDef = TypedDict(
     "_RequiredAnalyzeIDDetectionsTypeDef",
     {
         "Text": str,
@@ -460,21 +481,14 @@
 
 class AnalyzeIDDetectionsTypeDef(
     _RequiredAnalyzeIDDetectionsTypeDef, _OptionalAnalyzeIDDetectionsTypeDef
 ):
     pass
 
 
-QueriesConfigTypeDef = TypedDict(
-    "QueriesConfigTypeDef",
-    {
-        "Queries": Sequence[QueryTypeDef],
-    },
-)
-
 DocumentGroupTypeDef = TypedDict(
     "DocumentGroupTypeDef",
     {
         "Type": str,
         "SplitDocuments": List[SplitDocumentTypeDef],
         "DetectedSignatures": List[DetectedSignatureTypeDef],
         "UndetectedSignatures": List[UndetectedSignatureTypeDef],
@@ -532,14 +546,21 @@
     "PageClassificationTypeDef",
     {
         "PageType": List[PredictionTypeDef],
         "PageNumber": List[PredictionTypeDef],
     },
 )
 
+QueriesConfigTypeDef = TypedDict(
+    "QueriesConfigTypeDef",
+    {
+        "Queries": Sequence[QueryTypeDef],
+    },
+)
+
 IdentityDocumentFieldTypeDef = TypedDict(
     "IdentityDocumentFieldTypeDef",
     {
         "Type": AnalyzeIDDetectionsTypeDef,
         "ValueDetection": AnalyzeIDDetectionsTypeDef,
     },
     total=False,
@@ -550,42 +571,14 @@
     {
         "DocumentGroups": List[DocumentGroupTypeDef],
         "UndetectedDocumentTypes": List[str],
     },
     total=False,
 )
 
-_RequiredStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDocumentAnalysisRequestRequestTypeDef",
-    {
-        "DocumentLocation": DocumentLocationTypeDef,
-        "FeatureTypes": Sequence[FeatureTypeType],
-    },
-)
-_OptionalStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDocumentAnalysisRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "JobTag": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "OutputConfig": OutputConfigTypeDef,
-        "KMSKeyId": str,
-        "QueriesConfig": QueriesConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class StartDocumentAnalysisRequestRequestTypeDef(
-    _RequiredStartDocumentAnalysisRequestRequestTypeDef,
-    _OptionalStartDocumentAnalysisRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredStartDocumentTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartDocumentTextDetectionRequestRequestTypeDef",
     {
         "DocumentLocation": DocumentLocationTypeDef,
     },
 )
 _OptionalStartDocumentTextDetectionRequestRequestTypeDef = TypedDict(
@@ -694,15 +687,15 @@
         "ColumnSpan": int,
         "Geometry": GeometryTypeDef,
         "Id": str,
         "Relationships": List[RelationshipTypeDef],
         "EntityTypes": List[EntityTypeType],
         "SelectionStatus": SelectionStatusType,
         "Page": int,
-        "Query": QueryTypeDef,
+        "Query": QueryOutputTypeDef,
     },
     total=False,
 )
 
 ExpenseDetectionTypeDef = TypedDict(
     "ExpenseDetectionTypeDef",
     {
@@ -752,73 +745,101 @@
 
 class AnalyzeDocumentRequestRequestTypeDef(
     _RequiredAnalyzeDocumentRequestRequestTypeDef, _OptionalAnalyzeDocumentRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDocumentAnalysisRequestRequestTypeDef",
+    {
+        "DocumentLocation": DocumentLocationTypeDef,
+        "FeatureTypes": Sequence[FeatureTypeType],
+    },
+)
+_OptionalStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDocumentAnalysisRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "JobTag": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "OutputConfig": OutputConfigTypeDef,
+        "KMSKeyId": str,
+        "QueriesConfig": QueriesConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class StartDocumentAnalysisRequestRequestTypeDef(
+    _RequiredStartDocumentAnalysisRequestRequestTypeDef,
+    _OptionalStartDocumentAnalysisRequestRequestTypeDef,
+):
+    pass
+
+
 GetLendingAnalysisSummaryResponseTypeDef = TypedDict(
     "GetLendingAnalysisSummaryResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "Summary": LendingSummaryTypeDef,
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeLendingModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AnalyzeDocumentResponseTypeDef = TypedDict(
     "AnalyzeDocumentResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "Blocks": List[BlockTypeDef],
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
         "AnalyzeDocumentModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectDocumentTextResponseTypeDef = TypedDict(
     "DetectDocumentTextResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "Blocks": List[BlockTypeDef],
         "DetectDocumentTextModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentAnalysisResponseTypeDef = TypedDict(
     "GetDocumentAnalysisResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Blocks": List[BlockTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeDocumentModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentTextDetectionResponseTypeDef = TypedDict(
     "GetDocumentTextDetectionResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Blocks": List[BlockTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "DetectDocumentTextModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IdentityDocumentTypeDef = TypedDict(
     "IdentityDocumentTypeDef",
     {
         "DocumentIndex": int,
@@ -853,15 +874,15 @@
 
 AnalyzeIDResponseTypeDef = TypedDict(
     "AnalyzeIDResponseTypeDef",
     {
         "IdentityDocuments": List[IdentityDocumentTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "AnalyzeIDModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LineItemFieldsTypeDef = TypedDict(
     "LineItemFieldsTypeDef",
     {
         "LineItemExpenseFields": List[ExpenseFieldTypeDef],
@@ -899,15 +920,15 @@
 )
 
 AnalyzeExpenseResponseTypeDef = TypedDict(
     "AnalyzeExpenseResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "ExpenseDocuments": List[ExpenseDocumentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExtractionTypeDef = TypedDict(
     "ExtractionTypeDef",
     {
         "LendingDocument": LendingDocumentTypeDef,
@@ -923,15 +944,15 @@
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "ExpenseDocuments": List[ExpenseDocumentTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeExpenseModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LendingResultTypeDef = TypedDict(
     "LendingResultTypeDef",
     {
         "Page": int,
@@ -947,10 +968,10 @@
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Results": List[LendingResultTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeLendingModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-textract-1.28.0/mypy_boto3_textract/type_defs.pyi` & `mypy-boto3-textract-1.28.12/mypy_boto3_textract/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,17 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DocumentMetadataTypeDef",
     "HumanLoopActivationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "NormalizedValueTypeDef",
-    "QueryTypeDef",
+    "QueryOutputTypeDef",
     "RelationshipTypeDef",
     "BoundingBoxTypeDef",
     "DetectedSignatureTypeDef",
     "SplitDocumentTypeDef",
     "UndetectedSignatureTypeDef",
     "S3ObjectTypeDef",
     "ExpenseCurrencyTypeDef",
@@ -57,41 +58,41 @@
     "GetExpenseAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryRequestRequestTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "NotificationChannelTypeDef",
     "OutputConfigTypeDef",
     "PredictionTypeDef",
-    "ResponseMetadataTypeDef",
+    "QueryTypeDef",
     "StartDocumentAnalysisResponseTypeDef",
     "StartDocumentTextDetectionResponseTypeDef",
     "StartExpenseAnalysisResponseTypeDef",
     "StartLendingAnalysisResponseTypeDef",
     "AnalyzeIDDetectionsTypeDef",
-    "QueriesConfigTypeDef",
     "DocumentGroupTypeDef",
     "DocumentLocationTypeDef",
     "DocumentTypeDef",
     "GeometryTypeDef",
     "HumanLoopConfigTypeDef",
     "PageClassificationTypeDef",
+    "QueriesConfigTypeDef",
     "IdentityDocumentFieldTypeDef",
     "LendingSummaryTypeDef",
-    "StartDocumentAnalysisRequestRequestTypeDef",
     "StartDocumentTextDetectionRequestRequestTypeDef",
     "StartExpenseAnalysisRequestRequestTypeDef",
     "StartLendingAnalysisRequestRequestTypeDef",
     "AnalyzeExpenseRequestRequestTypeDef",
     "AnalyzeIDRequestRequestTypeDef",
     "DetectDocumentTextRequestRequestTypeDef",
     "BlockTypeDef",
     "ExpenseDetectionTypeDef",
     "LendingDetectionTypeDef",
     "SignatureDetectionTypeDef",
     "AnalyzeDocumentRequestRequestTypeDef",
+    "StartDocumentAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryResponseTypeDef",
     "AnalyzeDocumentResponseTypeDef",
     "DetectDocumentTextResponseTypeDef",
     "GetDocumentAnalysisResponseTypeDef",
     "GetDocumentTextDetectionResponseTypeDef",
     "IdentityDocumentTypeDef",
     "ExpenseFieldTypeDef",
@@ -122,39 +123,50 @@
         "HumanLoopArn": str,
         "HumanLoopActivationReasons": List[str],
         "HumanLoopActivationConditionsEvaluationResults": str,
     },
     total=False,
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
 NormalizedValueTypeDef = TypedDict(
     "NormalizedValueTypeDef",
     {
         "Value": str,
         "ValueType": Literal["DATE"],
     },
     total=False,
 )
 
-_RequiredQueryTypeDef = TypedDict(
-    "_RequiredQueryTypeDef",
+_RequiredQueryOutputTypeDef = TypedDict(
+    "_RequiredQueryOutputTypeDef",
     {
         "Text": str,
     },
 )
-_OptionalQueryTypeDef = TypedDict(
-    "_OptionalQueryTypeDef",
+_OptionalQueryOutputTypeDef = TypedDict(
+    "_OptionalQueryOutputTypeDef",
     {
         "Alias": str,
-        "Pages": Sequence[str],
+        "Pages": List[str],
     },
     total=False,
 )
 
-class QueryTypeDef(_RequiredQueryTypeDef, _OptionalQueryTypeDef):
+class QueryOutputTypeDef(_RequiredQueryOutputTypeDef, _OptionalQueryOutputTypeDef):
     pass
 
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "Type": RelationshipTypeType,
         "Ids": List[str],
@@ -382,54 +394,61 @@
     {
         "Value": str,
         "Confidence": float,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredQueryTypeDef = TypedDict(
+    "_RequiredQueryTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Text": str,
+    },
+)
+_OptionalQueryTypeDef = TypedDict(
+    "_OptionalQueryTypeDef",
+    {
+        "Alias": str,
+        "Pages": Sequence[str],
     },
+    total=False,
 )
 
+class QueryTypeDef(_RequiredQueryTypeDef, _OptionalQueryTypeDef):
+    pass
+
 StartDocumentAnalysisResponseTypeDef = TypedDict(
     "StartDocumentAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDocumentTextDetectionResponseTypeDef = TypedDict(
     "StartDocumentTextDetectionResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartExpenseAnalysisResponseTypeDef = TypedDict(
     "StartExpenseAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartLendingAnalysisResponseTypeDef = TypedDict(
     "StartLendingAnalysisResponseTypeDef",
     {
         "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAnalyzeIDDetectionsTypeDef = TypedDict(
     "_RequiredAnalyzeIDDetectionsTypeDef",
     {
         "Text": str,
@@ -445,21 +464,14 @@
 )
 
 class AnalyzeIDDetectionsTypeDef(
     _RequiredAnalyzeIDDetectionsTypeDef, _OptionalAnalyzeIDDetectionsTypeDef
 ):
     pass
 
-QueriesConfigTypeDef = TypedDict(
-    "QueriesConfigTypeDef",
-    {
-        "Queries": Sequence[QueryTypeDef],
-    },
-)
-
 DocumentGroupTypeDef = TypedDict(
     "DocumentGroupTypeDef",
     {
         "Type": str,
         "SplitDocuments": List[SplitDocumentTypeDef],
         "DetectedSignatures": List[DetectedSignatureTypeDef],
         "UndetectedSignatures": List[UndetectedSignatureTypeDef],
@@ -515,14 +527,21 @@
     "PageClassificationTypeDef",
     {
         "PageType": List[PredictionTypeDef],
         "PageNumber": List[PredictionTypeDef],
     },
 )
 
+QueriesConfigTypeDef = TypedDict(
+    "QueriesConfigTypeDef",
+    {
+        "Queries": Sequence[QueryTypeDef],
+    },
+)
+
 IdentityDocumentFieldTypeDef = TypedDict(
     "IdentityDocumentFieldTypeDef",
     {
         "Type": AnalyzeIDDetectionsTypeDef,
         "ValueDetection": AnalyzeIDDetectionsTypeDef,
     },
     total=False,
@@ -533,40 +552,14 @@
     {
         "DocumentGroups": List[DocumentGroupTypeDef],
         "UndetectedDocumentTypes": List[str],
     },
     total=False,
 )
 
-_RequiredStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDocumentAnalysisRequestRequestTypeDef",
-    {
-        "DocumentLocation": DocumentLocationTypeDef,
-        "FeatureTypes": Sequence[FeatureTypeType],
-    },
-)
-_OptionalStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDocumentAnalysisRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "JobTag": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "OutputConfig": OutputConfigTypeDef,
-        "KMSKeyId": str,
-        "QueriesConfig": QueriesConfigTypeDef,
-    },
-    total=False,
-)
-
-class StartDocumentAnalysisRequestRequestTypeDef(
-    _RequiredStartDocumentAnalysisRequestRequestTypeDef,
-    _OptionalStartDocumentAnalysisRequestRequestTypeDef,
-):
-    pass
-
 _RequiredStartDocumentTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartDocumentTextDetectionRequestRequestTypeDef",
     {
         "DocumentLocation": DocumentLocationTypeDef,
     },
 )
 _OptionalStartDocumentTextDetectionRequestRequestTypeDef = TypedDict(
@@ -669,15 +662,15 @@
         "ColumnSpan": int,
         "Geometry": GeometryTypeDef,
         "Id": str,
         "Relationships": List[RelationshipTypeDef],
         "EntityTypes": List[EntityTypeType],
         "SelectionStatus": SelectionStatusType,
         "Page": int,
-        "Query": QueryTypeDef,
+        "Query": QueryOutputTypeDef,
     },
     total=False,
 )
 
 ExpenseDetectionTypeDef = TypedDict(
     "ExpenseDetectionTypeDef",
     {
@@ -725,73 +718,99 @@
 )
 
 class AnalyzeDocumentRequestRequestTypeDef(
     _RequiredAnalyzeDocumentRequestRequestTypeDef, _OptionalAnalyzeDocumentRequestRequestTypeDef
 ):
     pass
 
+_RequiredStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDocumentAnalysisRequestRequestTypeDef",
+    {
+        "DocumentLocation": DocumentLocationTypeDef,
+        "FeatureTypes": Sequence[FeatureTypeType],
+    },
+)
+_OptionalStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDocumentAnalysisRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "JobTag": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "OutputConfig": OutputConfigTypeDef,
+        "KMSKeyId": str,
+        "QueriesConfig": QueriesConfigTypeDef,
+    },
+    total=False,
+)
+
+class StartDocumentAnalysisRequestRequestTypeDef(
+    _RequiredStartDocumentAnalysisRequestRequestTypeDef,
+    _OptionalStartDocumentAnalysisRequestRequestTypeDef,
+):
+    pass
+
 GetLendingAnalysisSummaryResponseTypeDef = TypedDict(
     "GetLendingAnalysisSummaryResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "Summary": LendingSummaryTypeDef,
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeLendingModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AnalyzeDocumentResponseTypeDef = TypedDict(
     "AnalyzeDocumentResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "Blocks": List[BlockTypeDef],
         "HumanLoopActivationOutput": HumanLoopActivationOutputTypeDef,
         "AnalyzeDocumentModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectDocumentTextResponseTypeDef = TypedDict(
     "DetectDocumentTextResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "Blocks": List[BlockTypeDef],
         "DetectDocumentTextModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentAnalysisResponseTypeDef = TypedDict(
     "GetDocumentAnalysisResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Blocks": List[BlockTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeDocumentModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDocumentTextDetectionResponseTypeDef = TypedDict(
     "GetDocumentTextDetectionResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Blocks": List[BlockTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "DetectDocumentTextModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IdentityDocumentTypeDef = TypedDict(
     "IdentityDocumentTypeDef",
     {
         "DocumentIndex": int,
@@ -826,15 +845,15 @@
 
 AnalyzeIDResponseTypeDef = TypedDict(
     "AnalyzeIDResponseTypeDef",
     {
         "IdentityDocuments": List[IdentityDocumentTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "AnalyzeIDModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LineItemFieldsTypeDef = TypedDict(
     "LineItemFieldsTypeDef",
     {
         "LineItemExpenseFields": List[ExpenseFieldTypeDef],
@@ -872,15 +891,15 @@
 )
 
 AnalyzeExpenseResponseTypeDef = TypedDict(
     "AnalyzeExpenseResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "ExpenseDocuments": List[ExpenseDocumentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExtractionTypeDef = TypedDict(
     "ExtractionTypeDef",
     {
         "LendingDocument": LendingDocumentTypeDef,
@@ -896,15 +915,15 @@
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "ExpenseDocuments": List[ExpenseDocumentTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeExpenseModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LendingResultTypeDef = TypedDict(
     "LendingResultTypeDef",
     {
         "Page": int,
@@ -920,10 +939,10 @@
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "NextToken": str,
         "Results": List[LendingResultTypeDef],
         "Warnings": List[WarningTypeDef],
         "StatusMessage": str,
         "AnalyzeLendingModelVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-textract-1.28.0/mypy_boto3_textract.egg-info/PKG-INFO` & `mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-textract
-Version: 1.28.0
-Summary: Type annotations for boto3.Textract 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Textract 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-textract"></a>
 
 # mypy-boto3-textract
 
 [![PyPI - mypy-boto3-textract](https://img.shields.io/pypi/v/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-textract.svg?color=blue)](https://pypi.org/project/mypy-boto3-textract)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-textract?color=blue)](https://pypistats.org/packages/mypy-boto3-textract)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-textract)](https://pepy.tech/project/mypy-boto3-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Textract 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
+[boto3.Textract 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
 [mypy-boto3-textract docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_textract/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,16 +306,17 @@
 `mypy_boto3_textract.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_textract.type_defs import (
     DocumentMetadataTypeDef,
     HumanLoopActivationOutputTypeDef,
+    ResponseMetadataTypeDef,
     NormalizedValueTypeDef,
-    QueryTypeDef,
+    QueryOutputTypeDef,
     RelationshipTypeDef,
     BoundingBoxTypeDef,
     DetectedSignatureTypeDef,
     SplitDocumentTypeDef,
     UndetectedSignatureTypeDef,
     S3ObjectTypeDef,
     ExpenseCurrencyTypeDef,
@@ -328,41 +329,41 @@
     GetExpenseAnalysisRequestRequestTypeDef,
     GetLendingAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryRequestRequestTypeDef,
     HumanLoopDataAttributesTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     PredictionTypeDef,
-    ResponseMetadataTypeDef,
+    QueryTypeDef,
     StartDocumentAnalysisResponseTypeDef,
     StartDocumentTextDetectionResponseTypeDef,
     StartExpenseAnalysisResponseTypeDef,
     StartLendingAnalysisResponseTypeDef,
     AnalyzeIDDetectionsTypeDef,
-    QueriesConfigTypeDef,
     DocumentGroupTypeDef,
     DocumentLocationTypeDef,
     DocumentTypeDef,
     GeometryTypeDef,
     HumanLoopConfigTypeDef,
     PageClassificationTypeDef,
+    QueriesConfigTypeDef,
     IdentityDocumentFieldTypeDef,
     LendingSummaryTypeDef,
-    StartDocumentAnalysisRequestRequestTypeDef,
     StartDocumentTextDetectionRequestRequestTypeDef,
     StartExpenseAnalysisRequestRequestTypeDef,
     StartLendingAnalysisRequestRequestTypeDef,
     AnalyzeExpenseRequestRequestTypeDef,
     AnalyzeIDRequestRequestTypeDef,
     DetectDocumentTextRequestRequestTypeDef,
     BlockTypeDef,
     ExpenseDetectionTypeDef,
     LendingDetectionTypeDef,
     SignatureDetectionTypeDef,
     AnalyzeDocumentRequestRequestTypeDef,
+    StartDocumentAnalysisRequestRequestTypeDef,
     GetLendingAnalysisSummaryResponseTypeDef,
     AnalyzeDocumentResponseTypeDef,
     DetectDocumentTextResponseTypeDef,
     GetDocumentAnalysisResponseTypeDef,
     GetDocumentTextDetectionResponseTypeDef,
     IdentityDocumentTypeDef,
     ExpenseFieldTypeDef,
```

### Comparing `mypy-boto3-textract-1.28.0/mypy_boto3_textract.egg-info/SOURCES.txt` & `mypy-boto3-textract-1.28.12/mypy_boto3_textract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-textract-1.28.0/setup.py` & `mypy-boto3-textract-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-textract",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_textract"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Textract 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Textract 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

