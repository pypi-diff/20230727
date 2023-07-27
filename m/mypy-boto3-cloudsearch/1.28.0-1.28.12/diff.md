# Comparing `tmp/mypy-boto3-cloudsearch-1.28.0.tar.gz` & `tmp/mypy-boto3-cloudsearch-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudsearch-1.28.0.tar", last modified: Thu Jul  6 20:59:10 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudsearch-1.28.12.tar", last modified: Thu Jul 27 05:34:26 2023, max compression
```

## Comparing `mypy-boto3-cloudsearch-1.28.0.tar` & `mypy-boto3-cloudsearch-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:10.650246 mypy-boto3-cloudsearch-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:27.000000 mypy-boto3-cloudsearch-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-07-06 20:59:10.638246 mypy-boto3-cloudsearch-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-07-06 20:35:27.000000 mypy-boto3-cloudsearch-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:10.638246 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-06 20:35:27.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 20:35:27.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 20:35:27.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-07-06 20:35:28.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-07-06 20:35:27.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-07-06 20:35:28.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-07-06 20:35:28.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:27.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25506 2023-07-06 20:35:28.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:27.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:10.638246 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:10.650246 mypy-boto3-cloudsearch-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 20:35:27.000000 mypy-boto3-cloudsearch-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.068559 mypy-boto3-cloudsearch-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15955 2023-07-27 05:34:26.056559 mypy-boto3-cloudsearch-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14452 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.056559 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-07-27 05:18:45.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-27 05:18:45.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-07-27 05:18:45.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32448 2023-07-27 05:18:45.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32417 2023-07-27 05:18:45.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.056559 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15955 2023-07-27 05:34:25.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-27 05:34:25.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:25.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:25.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:25.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:25.000000 mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:26.068559 mypy-boto3-cloudsearch-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:18:44.000000 mypy-boto3-cloudsearch-1.28.12/setup.py
```

### Comparing `mypy-boto3-cloudsearch-1.28.0/LICENSE` & `mypy-boto3-cloudsearch-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.0/PKG-INFO` & `mypy-boto3-cloudsearch-1.28.12/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudsearch
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudSearch 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudSearch 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudsearch"></a>
 
 # mypy-boto3-cloudsearch
 
 [![PyPI - mypy-boto3-cloudsearch](https://img.shields.io/pypi/v/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudsearch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudsearch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudsearch)](https://pepy.tech/project/mypy-boto3-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearch 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[boto3.CloudSearch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
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
 [mypy-boto3-cloudsearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,19 +303,22 @@
 
 `mypy_boto3_cloudsearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudsearch.type_defs import (
     OptionStatusTypeDef,
+    AnalysisOptionsOutputTypeDef,
     AnalysisOptionsTypeDef,
     BuildSuggestersRequestRequestTypeDef,
     BuildSuggestersResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
+    DateArrayOptionsOutputTypeDef,
     DateArrayOptionsTypeDef,
+    DateOptionsOutputTypeDef,
     DateOptionsTypeDef,
     ExpressionTypeDef,
     DeleteAnalysisSchemeRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteExpressionRequestRequestTypeDef,
     DeleteIndexFieldRequestRequestTypeDef,
     DeleteSuggesterRequestRequestTypeDef,
@@ -324,64 +327,80 @@
     DescribeDomainEndpointOptionsRequestRequestTypeDef,
     DescribeDomainsRequestRequestTypeDef,
     DescribeExpressionsRequestRequestTypeDef,
     DescribeIndexFieldsRequestRequestTypeDef,
     DescribeScalingParametersRequestRequestTypeDef,
     DescribeServiceAccessPoliciesRequestRequestTypeDef,
     DescribeSuggestersRequestRequestTypeDef,
+    DocumentSuggesterOptionsOutputTypeDef,
     DocumentSuggesterOptionsTypeDef,
+    DomainEndpointOptionsOutputTypeDef,
     DomainEndpointOptionsTypeDef,
     LimitsTypeDef,
     ServiceEndpointTypeDef,
+    DoubleArrayOptionsOutputTypeDef,
     DoubleArrayOptionsTypeDef,
+    DoubleOptionsOutputTypeDef,
     DoubleOptionsTypeDef,
+    ExpressionOutputTypeDef,
     IndexDocumentsRequestRequestTypeDef,
     IndexDocumentsResponseTypeDef,
+    IntArrayOptionsOutputTypeDef,
+    IntOptionsOutputTypeDef,
+    LatLonOptionsOutputTypeDef,
+    LiteralArrayOptionsOutputTypeDef,
+    LiteralOptionsOutputTypeDef,
+    TextArrayOptionsOutputTypeDef,
+    TextOptionsOutputTypeDef,
     IntArrayOptionsTypeDef,
     IntOptionsTypeDef,
     LatLonOptionsTypeDef,
     LiteralArrayOptionsTypeDef,
     LiteralOptionsTypeDef,
     TextArrayOptionsTypeDef,
     TextOptionsTypeDef,
     ListDomainNamesResponseTypeDef,
     ResponseMetadataTypeDef,
+    ScalingParametersOutputTypeDef,
     ScalingParametersTypeDef,
     UpdateAvailabilityOptionsRequestRequestTypeDef,
     UpdateServiceAccessPoliciesRequestRequestTypeDef,
     AccessPoliciesStatusTypeDef,
     AvailabilityOptionsStatusTypeDef,
+    AnalysisSchemeOutputTypeDef,
     AnalysisSchemeTypeDef,
     DefineExpressionRequestRequestTypeDef,
-    ExpressionStatusTypeDef,
+    SuggesterOutputTypeDef,
     SuggesterTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     UpdateDomainEndpointOptionsRequestRequestTypeDef,
     DomainStatusTypeDef,
+    ExpressionStatusTypeDef,
+    IndexFieldOutputTypeDef,
     IndexFieldTypeDef,
     ScalingParametersStatusTypeDef,
     UpdateScalingParametersRequestRequestTypeDef,
     DescribeServiceAccessPoliciesResponseTypeDef,
     UpdateServiceAccessPoliciesResponseTypeDef,
     DescribeAvailabilityOptionsResponseTypeDef,
     UpdateAvailabilityOptionsResponseTypeDef,
     AnalysisSchemeStatusTypeDef,
     DefineAnalysisSchemeRequestRequestTypeDef,
-    DefineExpressionResponseTypeDef,
-    DeleteExpressionResponseTypeDef,
-    DescribeExpressionsResponseTypeDef,
-    DefineSuggesterRequestRequestTypeDef,
     SuggesterStatusTypeDef,
+    DefineSuggesterRequestRequestTypeDef,
     DescribeDomainEndpointOptionsResponseTypeDef,
     UpdateDomainEndpointOptionsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DescribeDomainsResponseTypeDef,
-    DefineIndexFieldRequestRequestTypeDef,
+    DefineExpressionResponseTypeDef,
+    DeleteExpressionResponseTypeDef,
+    DescribeExpressionsResponseTypeDef,
     IndexFieldStatusTypeDef,
+    DefineIndexFieldRequestRequestTypeDef,
     DescribeScalingParametersResponseTypeDef,
     UpdateScalingParametersResponseTypeDef,
     DefineAnalysisSchemeResponseTypeDef,
     DeleteAnalysisSchemeResponseTypeDef,
     DescribeAnalysisSchemesResponseTypeDef,
     DefineSuggesterResponseTypeDef,
     DeleteSuggesterResponseTypeDef,
```

### Comparing `mypy-boto3-cloudsearch-1.28.0/README.md` & `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-cloudsearch
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudSearch 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 cloudsearch type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-cloudsearch"></a>
 
 # mypy-boto3-cloudsearch
 
 [![PyPI - mypy-boto3-cloudsearch](https://img.shields.io/pypi/v/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudsearch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudsearch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudsearch)](https://pepy.tech/project/mypy-boto3-cloudsearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearch 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
+[boto3.CloudSearch 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch)
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
 [mypy-boto3-cloudsearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,19 +303,22 @@
 
 `mypy_boto3_cloudsearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudsearch.type_defs import (
     OptionStatusTypeDef,
+    AnalysisOptionsOutputTypeDef,
     AnalysisOptionsTypeDef,
     BuildSuggestersRequestRequestTypeDef,
     BuildSuggestersResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
+    DateArrayOptionsOutputTypeDef,
     DateArrayOptionsTypeDef,
+    DateOptionsOutputTypeDef,
     DateOptionsTypeDef,
     ExpressionTypeDef,
     DeleteAnalysisSchemeRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteExpressionRequestRequestTypeDef,
     DeleteIndexFieldRequestRequestTypeDef,
     DeleteSuggesterRequestRequestTypeDef,
@@ -292,64 +327,80 @@
     DescribeDomainEndpointOptionsRequestRequestTypeDef,
     DescribeDomainsRequestRequestTypeDef,
     DescribeExpressionsRequestRequestTypeDef,
     DescribeIndexFieldsRequestRequestTypeDef,
     DescribeScalingParametersRequestRequestTypeDef,
     DescribeServiceAccessPoliciesRequestRequestTypeDef,
     DescribeSuggestersRequestRequestTypeDef,
+    DocumentSuggesterOptionsOutputTypeDef,
     DocumentSuggesterOptionsTypeDef,
+    DomainEndpointOptionsOutputTypeDef,
     DomainEndpointOptionsTypeDef,
     LimitsTypeDef,
     ServiceEndpointTypeDef,
+    DoubleArrayOptionsOutputTypeDef,
     DoubleArrayOptionsTypeDef,
+    DoubleOptionsOutputTypeDef,
     DoubleOptionsTypeDef,
+    ExpressionOutputTypeDef,
     IndexDocumentsRequestRequestTypeDef,
     IndexDocumentsResponseTypeDef,
+    IntArrayOptionsOutputTypeDef,
+    IntOptionsOutputTypeDef,
+    LatLonOptionsOutputTypeDef,
+    LiteralArrayOptionsOutputTypeDef,
+    LiteralOptionsOutputTypeDef,
+    TextArrayOptionsOutputTypeDef,
+    TextOptionsOutputTypeDef,
     IntArrayOptionsTypeDef,
     IntOptionsTypeDef,
     LatLonOptionsTypeDef,
     LiteralArrayOptionsTypeDef,
     LiteralOptionsTypeDef,
     TextArrayOptionsTypeDef,
     TextOptionsTypeDef,
     ListDomainNamesResponseTypeDef,
     ResponseMetadataTypeDef,
+    ScalingParametersOutputTypeDef,
     ScalingParametersTypeDef,
     UpdateAvailabilityOptionsRequestRequestTypeDef,
     UpdateServiceAccessPoliciesRequestRequestTypeDef,
     AccessPoliciesStatusTypeDef,
     AvailabilityOptionsStatusTypeDef,
+    AnalysisSchemeOutputTypeDef,
     AnalysisSchemeTypeDef,
     DefineExpressionRequestRequestTypeDef,
-    ExpressionStatusTypeDef,
+    SuggesterOutputTypeDef,
     SuggesterTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     UpdateDomainEndpointOptionsRequestRequestTypeDef,
     DomainStatusTypeDef,
+    ExpressionStatusTypeDef,
+    IndexFieldOutputTypeDef,
     IndexFieldTypeDef,
     ScalingParametersStatusTypeDef,
     UpdateScalingParametersRequestRequestTypeDef,
     DescribeServiceAccessPoliciesResponseTypeDef,
     UpdateServiceAccessPoliciesResponseTypeDef,
     DescribeAvailabilityOptionsResponseTypeDef,
     UpdateAvailabilityOptionsResponseTypeDef,
     AnalysisSchemeStatusTypeDef,
     DefineAnalysisSchemeRequestRequestTypeDef,
-    DefineExpressionResponseTypeDef,
-    DeleteExpressionResponseTypeDef,
-    DescribeExpressionsResponseTypeDef,
-    DefineSuggesterRequestRequestTypeDef,
     SuggesterStatusTypeDef,
+    DefineSuggesterRequestRequestTypeDef,
     DescribeDomainEndpointOptionsResponseTypeDef,
     UpdateDomainEndpointOptionsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DescribeDomainsResponseTypeDef,
-    DefineIndexFieldRequestRequestTypeDef,
+    DefineExpressionResponseTypeDef,
+    DeleteExpressionResponseTypeDef,
+    DescribeExpressionsResponseTypeDef,
     IndexFieldStatusTypeDef,
+    DefineIndexFieldRequestRequestTypeDef,
     DescribeScalingParametersResponseTypeDef,
     UpdateScalingParametersResponseTypeDef,
     DefineAnalysisSchemeResponseTypeDef,
     DeleteAnalysisSchemeResponseTypeDef,
     DescribeAnalysisSchemesResponseTypeDef,
     DefineSuggesterResponseTypeDef,
     DeleteSuggesterResponseTypeDef,
```

### Comparing `mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/__main__.py` & `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudSearch 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudSearch 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch\nOther"
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

### Comparing `mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/client.py` & `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/client.pyi` & `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/literals.py` & `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,15 @@
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
@@ -309,26 +310,28 @@
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

### Comparing `mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/literals.pyi` & `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/literals.pyi`

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

### Comparing `mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/type_defs.py` & `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/type_defs.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -26,22 +26,24 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "OptionStatusTypeDef",
+    "AnalysisOptionsOutputTypeDef",
     "AnalysisOptionsTypeDef",
     "BuildSuggestersRequestRequestTypeDef",
     "BuildSuggestersResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
+    "DateArrayOptionsOutputTypeDef",
     "DateArrayOptionsTypeDef",
+    "DateOptionsOutputTypeDef",
     "DateOptionsTypeDef",
     "ExpressionTypeDef",
     "DeleteAnalysisSchemeRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteExpressionRequestRequestTypeDef",
     "DeleteIndexFieldRequestRequestTypeDef",
     "DeleteSuggesterRequestRequestTypeDef",
@@ -50,64 +52,80 @@
     "DescribeDomainEndpointOptionsRequestRequestTypeDef",
     "DescribeDomainsRequestRequestTypeDef",
     "DescribeExpressionsRequestRequestTypeDef",
     "DescribeIndexFieldsRequestRequestTypeDef",
     "DescribeScalingParametersRequestRequestTypeDef",
     "DescribeServiceAccessPoliciesRequestRequestTypeDef",
     "DescribeSuggestersRequestRequestTypeDef",
+    "DocumentSuggesterOptionsOutputTypeDef",
     "DocumentSuggesterOptionsTypeDef",
+    "DomainEndpointOptionsOutputTypeDef",
     "DomainEndpointOptionsTypeDef",
     "LimitsTypeDef",
     "ServiceEndpointTypeDef",
+    "DoubleArrayOptionsOutputTypeDef",
     "DoubleArrayOptionsTypeDef",
+    "DoubleOptionsOutputTypeDef",
     "DoubleOptionsTypeDef",
+    "ExpressionOutputTypeDef",
     "IndexDocumentsRequestRequestTypeDef",
     "IndexDocumentsResponseTypeDef",
+    "IntArrayOptionsOutputTypeDef",
+    "IntOptionsOutputTypeDef",
+    "LatLonOptionsOutputTypeDef",
+    "LiteralArrayOptionsOutputTypeDef",
+    "LiteralOptionsOutputTypeDef",
+    "TextArrayOptionsOutputTypeDef",
+    "TextOptionsOutputTypeDef",
     "IntArrayOptionsTypeDef",
     "IntOptionsTypeDef",
     "LatLonOptionsTypeDef",
     "LiteralArrayOptionsTypeDef",
     "LiteralOptionsTypeDef",
     "TextArrayOptionsTypeDef",
     "TextOptionsTypeDef",
     "ListDomainNamesResponseTypeDef",
     "ResponseMetadataTypeDef",
+    "ScalingParametersOutputTypeDef",
     "ScalingParametersTypeDef",
     "UpdateAvailabilityOptionsRequestRequestTypeDef",
     "UpdateServiceAccessPoliciesRequestRequestTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AvailabilityOptionsStatusTypeDef",
+    "AnalysisSchemeOutputTypeDef",
     "AnalysisSchemeTypeDef",
     "DefineExpressionRequestRequestTypeDef",
-    "ExpressionStatusTypeDef",
+    "SuggesterOutputTypeDef",
     "SuggesterTypeDef",
     "DomainEndpointOptionsStatusTypeDef",
     "UpdateDomainEndpointOptionsRequestRequestTypeDef",
     "DomainStatusTypeDef",
+    "ExpressionStatusTypeDef",
+    "IndexFieldOutputTypeDef",
     "IndexFieldTypeDef",
     "ScalingParametersStatusTypeDef",
     "UpdateScalingParametersRequestRequestTypeDef",
     "DescribeServiceAccessPoliciesResponseTypeDef",
     "UpdateServiceAccessPoliciesResponseTypeDef",
     "DescribeAvailabilityOptionsResponseTypeDef",
     "UpdateAvailabilityOptionsResponseTypeDef",
     "AnalysisSchemeStatusTypeDef",
     "DefineAnalysisSchemeRequestRequestTypeDef",
-    "DefineExpressionResponseTypeDef",
-    "DeleteExpressionResponseTypeDef",
-    "DescribeExpressionsResponseTypeDef",
-    "DefineSuggesterRequestRequestTypeDef",
     "SuggesterStatusTypeDef",
+    "DefineSuggesterRequestRequestTypeDef",
     "DescribeDomainEndpointOptionsResponseTypeDef",
     "UpdateDomainEndpointOptionsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DeleteDomainResponseTypeDef",
     "DescribeDomainsResponseTypeDef",
-    "DefineIndexFieldRequestRequestTypeDef",
+    "DefineExpressionResponseTypeDef",
+    "DeleteExpressionResponseTypeDef",
+    "DescribeExpressionsResponseTypeDef",
     "IndexFieldStatusTypeDef",
+    "DefineIndexFieldRequestRequestTypeDef",
     "DescribeScalingParametersResponseTypeDef",
     "UpdateScalingParametersResponseTypeDef",
     "DefineAnalysisSchemeResponseTypeDef",
     "DeleteAnalysisSchemeResponseTypeDef",
     "DescribeAnalysisSchemesResponseTypeDef",
     "DefineSuggesterResponseTypeDef",
     "DeleteSuggesterResponseTypeDef",
@@ -130,18 +148,28 @@
     {
         "UpdateVersion": int,
         "PendingDeletion": bool,
     },
     total=False,
 )
 
-
 class OptionStatusTypeDef(_RequiredOptionStatusTypeDef, _OptionalOptionStatusTypeDef):
     pass
 
+AnalysisOptionsOutputTypeDef = TypedDict(
+    "AnalysisOptionsOutputTypeDef",
+    {
+        "Synonyms": str,
+        "Stopwords": str,
+        "StemmingDictionary": str,
+        "JapaneseTokenizationDictionary": str,
+        "AlgorithmicStemming": AlgorithmicStemmingType,
+    },
+    total=False,
+)
 
 AnalysisOptionsTypeDef = TypedDict(
     "AnalysisOptionsTypeDef",
     {
         "Synonyms": str,
         "Stopwords": str,
         "StemmingDictionary": str,
@@ -169,26 +197,51 @@
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+DateArrayOptionsOutputTypeDef = TypedDict(
+    "DateArrayOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceFields": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+    },
+    total=False,
+)
+
 DateArrayOptionsTypeDef = TypedDict(
     "DateArrayOptionsTypeDef",
     {
         "DefaultValue": str,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
         "ReturnEnabled": bool,
     },
     total=False,
 )
 
+DateOptionsOutputTypeDef = TypedDict(
+    "DateOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceField": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+        "SortEnabled": bool,
+    },
+    total=False,
+)
+
 DateOptionsTypeDef = TypedDict(
     "DateOptionsTypeDef",
     {
         "DefaultValue": str,
         "SourceField": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
@@ -256,66 +309,60 @@
     {
         "AnalysisSchemeNames": Sequence[str],
         "Deployed": bool,
     },
     total=False,
 )
 
-
 class DescribeAnalysisSchemesRequestRequestTypeDef(
     _RequiredDescribeAnalysisSchemesRequestRequestTypeDef,
     _OptionalDescribeAnalysisSchemesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeAvailabilityOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAvailabilityOptionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalDescribeAvailabilityOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeAvailabilityOptionsRequestRequestTypeDef",
     {
         "Deployed": bool,
     },
     total=False,
 )
 
-
 class DescribeAvailabilityOptionsRequestRequestTypeDef(
     _RequiredDescribeAvailabilityOptionsRequestRequestTypeDef,
     _OptionalDescribeAvailabilityOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeDomainEndpointOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDomainEndpointOptionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalDescribeDomainEndpointOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeDomainEndpointOptionsRequestRequestTypeDef",
     {
         "Deployed": bool,
     },
     total=False,
 )
 
-
 class DescribeDomainEndpointOptionsRequestRequestTypeDef(
     _RequiredDescribeDomainEndpointOptionsRequestRequestTypeDef,
     _OptionalDescribeDomainEndpointOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeDomainsRequestRequestTypeDef = TypedDict(
     "DescribeDomainsRequestRequestTypeDef",
     {
         "DomainNames": Sequence[str],
     },
     total=False,
 )
@@ -331,22 +378,20 @@
     {
         "ExpressionNames": Sequence[str],
         "Deployed": bool,
     },
     total=False,
 )
 
-
 class DescribeExpressionsRequestRequestTypeDef(
     _RequiredDescribeExpressionsRequestRequestTypeDef,
     _OptionalDescribeExpressionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeIndexFieldsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeIndexFieldsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalDescribeIndexFieldsRequestRequestTypeDef = TypedDict(
@@ -354,22 +399,20 @@
     {
         "FieldNames": Sequence[str],
         "Deployed": bool,
     },
     total=False,
 )
 
-
 class DescribeIndexFieldsRequestRequestTypeDef(
     _RequiredDescribeIndexFieldsRequestRequestTypeDef,
     _OptionalDescribeIndexFieldsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeScalingParametersRequestRequestTypeDef = TypedDict(
     "DescribeScalingParametersRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -383,22 +426,20 @@
     "_OptionalDescribeServiceAccessPoliciesRequestRequestTypeDef",
     {
         "Deployed": bool,
     },
     total=False,
 )
 
-
 class DescribeServiceAccessPoliciesRequestRequestTypeDef(
     _RequiredDescribeServiceAccessPoliciesRequestRequestTypeDef,
     _OptionalDescribeServiceAccessPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeSuggestersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSuggestersRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalDescribeSuggestersRequestRequestTypeDef = TypedDict(
@@ -406,21 +447,39 @@
     {
         "SuggesterNames": Sequence[str],
         "Deployed": bool,
     },
     total=False,
 )
 
-
 class DescribeSuggestersRequestRequestTypeDef(
     _RequiredDescribeSuggestersRequestRequestTypeDef,
     _OptionalDescribeSuggestersRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDocumentSuggesterOptionsOutputTypeDef = TypedDict(
+    "_RequiredDocumentSuggesterOptionsOutputTypeDef",
+    {
+        "SourceField": str,
+    },
+)
+_OptionalDocumentSuggesterOptionsOutputTypeDef = TypedDict(
+    "_OptionalDocumentSuggesterOptionsOutputTypeDef",
+    {
+        "FuzzyMatching": SuggesterFuzzyMatchingType,
+        "SortExpression": str,
+    },
+    total=False,
+)
+
+class DocumentSuggesterOptionsOutputTypeDef(
+    _RequiredDocumentSuggesterOptionsOutputTypeDef, _OptionalDocumentSuggesterOptionsOutputTypeDef
+):
+    pass
 
 _RequiredDocumentSuggesterOptionsTypeDef = TypedDict(
     "_RequiredDocumentSuggesterOptionsTypeDef",
     {
         "SourceField": str,
     },
 )
@@ -429,20 +488,27 @@
     {
         "FuzzyMatching": SuggesterFuzzyMatchingType,
         "SortExpression": str,
     },
     total=False,
 )
 
-
 class DocumentSuggesterOptionsTypeDef(
     _RequiredDocumentSuggesterOptionsTypeDef, _OptionalDocumentSuggesterOptionsTypeDef
 ):
     pass
 
+DomainEndpointOptionsOutputTypeDef = TypedDict(
+    "DomainEndpointOptionsOutputTypeDef",
+    {
+        "EnforceHTTPS": bool,
+        "TLSSecurityPolicy": TLSSecurityPolicyType,
+    },
+    total=False,
+)
 
 DomainEndpointOptionsTypeDef = TypedDict(
     "DomainEndpointOptionsTypeDef",
     {
         "EnforceHTTPS": bool,
         "TLSSecurityPolicy": TLSSecurityPolicyType,
     },
@@ -461,39 +527,72 @@
     "ServiceEndpointTypeDef",
     {
         "Endpoint": str,
     },
     total=False,
 )
 
+DoubleArrayOptionsOutputTypeDef = TypedDict(
+    "DoubleArrayOptionsOutputTypeDef",
+    {
+        "DefaultValue": float,
+        "SourceFields": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+    },
+    total=False,
+)
+
 DoubleArrayOptionsTypeDef = TypedDict(
     "DoubleArrayOptionsTypeDef",
     {
         "DefaultValue": float,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
         "ReturnEnabled": bool,
     },
     total=False,
 )
 
+DoubleOptionsOutputTypeDef = TypedDict(
+    "DoubleOptionsOutputTypeDef",
+    {
+        "DefaultValue": float,
+        "SourceField": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+        "SortEnabled": bool,
+    },
+    total=False,
+)
+
 DoubleOptionsTypeDef = TypedDict(
     "DoubleOptionsTypeDef",
     {
         "DefaultValue": float,
         "SourceField": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
         "ReturnEnabled": bool,
         "SortEnabled": bool,
     },
     total=False,
 )
 
+ExpressionOutputTypeDef = TypedDict(
+    "ExpressionOutputTypeDef",
+    {
+        "ExpressionName": str,
+        "ExpressionValue": str,
+    },
+)
+
 IndexDocumentsRequestRequestTypeDef = TypedDict(
     "IndexDocumentsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -501,14 +600,102 @@
     "IndexDocumentsResponseTypeDef",
     {
         "FieldNames": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IntArrayOptionsOutputTypeDef = TypedDict(
+    "IntArrayOptionsOutputTypeDef",
+    {
+        "DefaultValue": int,
+        "SourceFields": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+    },
+    total=False,
+)
+
+IntOptionsOutputTypeDef = TypedDict(
+    "IntOptionsOutputTypeDef",
+    {
+        "DefaultValue": int,
+        "SourceField": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+        "SortEnabled": bool,
+    },
+    total=False,
+)
+
+LatLonOptionsOutputTypeDef = TypedDict(
+    "LatLonOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceField": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+        "SortEnabled": bool,
+    },
+    total=False,
+)
+
+LiteralArrayOptionsOutputTypeDef = TypedDict(
+    "LiteralArrayOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceFields": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+    },
+    total=False,
+)
+
+LiteralOptionsOutputTypeDef = TypedDict(
+    "LiteralOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceField": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+        "SortEnabled": bool,
+    },
+    total=False,
+)
+
+TextArrayOptionsOutputTypeDef = TypedDict(
+    "TextArrayOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceFields": str,
+        "ReturnEnabled": bool,
+        "HighlightEnabled": bool,
+        "AnalysisScheme": str,
+    },
+    total=False,
+)
+
+TextOptionsOutputTypeDef = TypedDict(
+    "TextOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceField": str,
+        "ReturnEnabled": bool,
+        "SortEnabled": bool,
+        "HighlightEnabled": bool,
+        "AnalysisScheme": str,
+    },
+    total=False,
+)
+
 IntArrayOptionsTypeDef = TypedDict(
     "IntArrayOptionsTypeDef",
     {
         "DefaultValue": int,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
@@ -608,14 +795,24 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+ScalingParametersOutputTypeDef = TypedDict(
+    "ScalingParametersOutputTypeDef",
+    {
+        "DesiredInstanceType": PartitionInstanceTypeType,
+        "DesiredReplicationCount": int,
+        "DesiredPartitionCount": int,
+    },
+    total=False,
+)
+
 ScalingParametersTypeDef = TypedDict(
     "ScalingParametersTypeDef",
     {
         "DesiredInstanceType": PartitionInstanceTypeType,
         "DesiredReplicationCount": int,
         "DesiredPartitionCount": int,
     },
@@ -650,14 +847,34 @@
     "AvailabilityOptionsStatusTypeDef",
     {
         "Options": bool,
         "Status": OptionStatusTypeDef,
     },
 )
 
+_RequiredAnalysisSchemeOutputTypeDef = TypedDict(
+    "_RequiredAnalysisSchemeOutputTypeDef",
+    {
+        "AnalysisSchemeName": str,
+        "AnalysisSchemeLanguage": AnalysisSchemeLanguageType,
+    },
+)
+_OptionalAnalysisSchemeOutputTypeDef = TypedDict(
+    "_OptionalAnalysisSchemeOutputTypeDef",
+    {
+        "AnalysisOptions": AnalysisOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+class AnalysisSchemeOutputTypeDef(
+    _RequiredAnalysisSchemeOutputTypeDef, _OptionalAnalysisSchemeOutputTypeDef
+):
+    pass
+
 _RequiredAnalysisSchemeTypeDef = TypedDict(
     "_RequiredAnalysisSchemeTypeDef",
     {
         "AnalysisSchemeName": str,
         "AnalysisSchemeLanguage": AnalysisSchemeLanguageType,
     },
 )
@@ -665,47 +882,45 @@
     "_OptionalAnalysisSchemeTypeDef",
     {
         "AnalysisOptions": AnalysisOptionsTypeDef,
     },
     total=False,
 )
 
-
 class AnalysisSchemeTypeDef(_RequiredAnalysisSchemeTypeDef, _OptionalAnalysisSchemeTypeDef):
     pass
 
-
 DefineExpressionRequestRequestTypeDef = TypedDict(
     "DefineExpressionRequestRequestTypeDef",
     {
         "DomainName": str,
         "Expression": ExpressionTypeDef,
     },
 )
 
-ExpressionStatusTypeDef = TypedDict(
-    "ExpressionStatusTypeDef",
+SuggesterOutputTypeDef = TypedDict(
+    "SuggesterOutputTypeDef",
     {
-        "Options": ExpressionTypeDef,
-        "Status": OptionStatusTypeDef,
+        "SuggesterName": str,
+        "DocumentSuggesterOptions": DocumentSuggesterOptionsOutputTypeDef,
     },
 )
 
 SuggesterTypeDef = TypedDict(
     "SuggesterTypeDef",
     {
         "SuggesterName": str,
         "DocumentSuggesterOptions": DocumentSuggesterOptionsTypeDef,
     },
 )
 
 DomainEndpointOptionsStatusTypeDef = TypedDict(
     "DomainEndpointOptionsStatusTypeDef",
     {
-        "Options": DomainEndpointOptionsTypeDef,
+        "Options": DomainEndpointOptionsOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 UpdateDomainEndpointOptionsRequestRequestTypeDef = TypedDict(
     "UpdateDomainEndpointOptionsRequestRequestTypeDef",
     {
@@ -735,18 +950,52 @@
         "SearchPartitionCount": int,
         "SearchInstanceCount": int,
         "Limits": LimitsTypeDef,
     },
     total=False,
 )
 
-
 class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
     pass
 
+ExpressionStatusTypeDef = TypedDict(
+    "ExpressionStatusTypeDef",
+    {
+        "Options": ExpressionOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+_RequiredIndexFieldOutputTypeDef = TypedDict(
+    "_RequiredIndexFieldOutputTypeDef",
+    {
+        "IndexFieldName": str,
+        "IndexFieldType": IndexFieldTypeType,
+    },
+)
+_OptionalIndexFieldOutputTypeDef = TypedDict(
+    "_OptionalIndexFieldOutputTypeDef",
+    {
+        "IntOptions": IntOptionsOutputTypeDef,
+        "DoubleOptions": DoubleOptionsOutputTypeDef,
+        "LiteralOptions": LiteralOptionsOutputTypeDef,
+        "TextOptions": TextOptionsOutputTypeDef,
+        "DateOptions": DateOptionsOutputTypeDef,
+        "LatLonOptions": LatLonOptionsOutputTypeDef,
+        "IntArrayOptions": IntArrayOptionsOutputTypeDef,
+        "DoubleArrayOptions": DoubleArrayOptionsOutputTypeDef,
+        "LiteralArrayOptions": LiteralArrayOptionsOutputTypeDef,
+        "TextArrayOptions": TextArrayOptionsOutputTypeDef,
+        "DateArrayOptions": DateArrayOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+class IndexFieldOutputTypeDef(_RequiredIndexFieldOutputTypeDef, _OptionalIndexFieldOutputTypeDef):
+    pass
 
 _RequiredIndexFieldTypeDef = TypedDict(
     "_RequiredIndexFieldTypeDef",
     {
         "IndexFieldName": str,
         "IndexFieldType": IndexFieldTypeType,
     },
@@ -765,23 +1014,21 @@
         "LiteralArrayOptions": LiteralArrayOptionsTypeDef,
         "TextArrayOptions": TextArrayOptionsTypeDef,
         "DateArrayOptions": DateArrayOptionsTypeDef,
     },
     total=False,
 )
 
-
 class IndexFieldTypeDef(_RequiredIndexFieldTypeDef, _OptionalIndexFieldTypeDef):
     pass
 
-
 ScalingParametersStatusTypeDef = TypedDict(
     "ScalingParametersStatusTypeDef",
     {
-        "Options": ScalingParametersTypeDef,
+        "Options": ScalingParametersOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 UpdateScalingParametersRequestRequestTypeDef = TypedDict(
     "UpdateScalingParametersRequestRequestTypeDef",
     {
@@ -821,67 +1068,43 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AnalysisSchemeStatusTypeDef = TypedDict(
     "AnalysisSchemeStatusTypeDef",
     {
-        "Options": AnalysisSchemeTypeDef,
+        "Options": AnalysisSchemeOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 DefineAnalysisSchemeRequestRequestTypeDef = TypedDict(
     "DefineAnalysisSchemeRequestRequestTypeDef",
     {
         "DomainName": str,
         "AnalysisScheme": AnalysisSchemeTypeDef,
     },
 )
 
-DefineExpressionResponseTypeDef = TypedDict(
-    "DefineExpressionResponseTypeDef",
-    {
-        "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteExpressionResponseTypeDef = TypedDict(
-    "DeleteExpressionResponseTypeDef",
-    {
-        "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeExpressionsResponseTypeDef = TypedDict(
-    "DescribeExpressionsResponseTypeDef",
+SuggesterStatusTypeDef = TypedDict(
+    "SuggesterStatusTypeDef",
     {
-        "Expressions": List[ExpressionStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Options": SuggesterOutputTypeDef,
+        "Status": OptionStatusTypeDef,
     },
 )
 
 DefineSuggesterRequestRequestTypeDef = TypedDict(
     "DefineSuggesterRequestRequestTypeDef",
     {
         "DomainName": str,
         "Suggester": SuggesterTypeDef,
     },
 )
 
-SuggesterStatusTypeDef = TypedDict(
-    "SuggesterStatusTypeDef",
-    {
-        "Options": SuggesterTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
 DescribeDomainEndpointOptionsResponseTypeDef = TypedDict(
     "DescribeDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -914,30 +1137,54 @@
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DefineIndexFieldRequestRequestTypeDef = TypedDict(
-    "DefineIndexFieldRequestRequestTypeDef",
+DefineExpressionResponseTypeDef = TypedDict(
+    "DefineExpressionResponseTypeDef",
     {
-        "DomainName": str,
-        "IndexField": IndexFieldTypeDef,
+        "Expression": ExpressionStatusTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteExpressionResponseTypeDef = TypedDict(
+    "DeleteExpressionResponseTypeDef",
+    {
+        "Expression": ExpressionStatusTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeExpressionsResponseTypeDef = TypedDict(
+    "DescribeExpressionsResponseTypeDef",
+    {
+        "Expressions": List[ExpressionStatusTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IndexFieldStatusTypeDef = TypedDict(
     "IndexFieldStatusTypeDef",
     {
-        "Options": IndexFieldTypeDef,
+        "Options": IndexFieldOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
+DefineIndexFieldRequestRequestTypeDef = TypedDict(
+    "DefineIndexFieldRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "IndexField": IndexFieldTypeDef,
+    },
+)
+
 DescribeScalingParametersResponseTypeDef = TypedDict(
     "DescribeScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch/type_defs.pyi` & `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch/type_defs.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,21 +26,25 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "OptionStatusTypeDef",
+    "AnalysisOptionsOutputTypeDef",
     "AnalysisOptionsTypeDef",
     "BuildSuggestersRequestRequestTypeDef",
     "BuildSuggestersResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
+    "DateArrayOptionsOutputTypeDef",
     "DateArrayOptionsTypeDef",
+    "DateOptionsOutputTypeDef",
     "DateOptionsTypeDef",
     "ExpressionTypeDef",
     "DeleteAnalysisSchemeRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteExpressionRequestRequestTypeDef",
     "DeleteIndexFieldRequestRequestTypeDef",
     "DeleteSuggesterRequestRequestTypeDef",
@@ -49,64 +53,80 @@
     "DescribeDomainEndpointOptionsRequestRequestTypeDef",
     "DescribeDomainsRequestRequestTypeDef",
     "DescribeExpressionsRequestRequestTypeDef",
     "DescribeIndexFieldsRequestRequestTypeDef",
     "DescribeScalingParametersRequestRequestTypeDef",
     "DescribeServiceAccessPoliciesRequestRequestTypeDef",
     "DescribeSuggestersRequestRequestTypeDef",
+    "DocumentSuggesterOptionsOutputTypeDef",
     "DocumentSuggesterOptionsTypeDef",
+    "DomainEndpointOptionsOutputTypeDef",
     "DomainEndpointOptionsTypeDef",
     "LimitsTypeDef",
     "ServiceEndpointTypeDef",
+    "DoubleArrayOptionsOutputTypeDef",
     "DoubleArrayOptionsTypeDef",
+    "DoubleOptionsOutputTypeDef",
     "DoubleOptionsTypeDef",
+    "ExpressionOutputTypeDef",
     "IndexDocumentsRequestRequestTypeDef",
     "IndexDocumentsResponseTypeDef",
+    "IntArrayOptionsOutputTypeDef",
+    "IntOptionsOutputTypeDef",
+    "LatLonOptionsOutputTypeDef",
+    "LiteralArrayOptionsOutputTypeDef",
+    "LiteralOptionsOutputTypeDef",
+    "TextArrayOptionsOutputTypeDef",
+    "TextOptionsOutputTypeDef",
     "IntArrayOptionsTypeDef",
     "IntOptionsTypeDef",
     "LatLonOptionsTypeDef",
     "LiteralArrayOptionsTypeDef",
     "LiteralOptionsTypeDef",
     "TextArrayOptionsTypeDef",
     "TextOptionsTypeDef",
     "ListDomainNamesResponseTypeDef",
     "ResponseMetadataTypeDef",
+    "ScalingParametersOutputTypeDef",
     "ScalingParametersTypeDef",
     "UpdateAvailabilityOptionsRequestRequestTypeDef",
     "UpdateServiceAccessPoliciesRequestRequestTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AvailabilityOptionsStatusTypeDef",
+    "AnalysisSchemeOutputTypeDef",
     "AnalysisSchemeTypeDef",
     "DefineExpressionRequestRequestTypeDef",
-    "ExpressionStatusTypeDef",
+    "SuggesterOutputTypeDef",
     "SuggesterTypeDef",
     "DomainEndpointOptionsStatusTypeDef",
     "UpdateDomainEndpointOptionsRequestRequestTypeDef",
     "DomainStatusTypeDef",
+    "ExpressionStatusTypeDef",
+    "IndexFieldOutputTypeDef",
     "IndexFieldTypeDef",
     "ScalingParametersStatusTypeDef",
     "UpdateScalingParametersRequestRequestTypeDef",
     "DescribeServiceAccessPoliciesResponseTypeDef",
     "UpdateServiceAccessPoliciesResponseTypeDef",
     "DescribeAvailabilityOptionsResponseTypeDef",
     "UpdateAvailabilityOptionsResponseTypeDef",
     "AnalysisSchemeStatusTypeDef",
     "DefineAnalysisSchemeRequestRequestTypeDef",
-    "DefineExpressionResponseTypeDef",
-    "DeleteExpressionResponseTypeDef",
-    "DescribeExpressionsResponseTypeDef",
-    "DefineSuggesterRequestRequestTypeDef",
     "SuggesterStatusTypeDef",
+    "DefineSuggesterRequestRequestTypeDef",
     "DescribeDomainEndpointOptionsResponseTypeDef",
     "UpdateDomainEndpointOptionsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DeleteDomainResponseTypeDef",
     "DescribeDomainsResponseTypeDef",
-    "DefineIndexFieldRequestRequestTypeDef",
+    "DefineExpressionResponseTypeDef",
+    "DeleteExpressionResponseTypeDef",
+    "DescribeExpressionsResponseTypeDef",
     "IndexFieldStatusTypeDef",
+    "DefineIndexFieldRequestRequestTypeDef",
     "DescribeScalingParametersResponseTypeDef",
     "UpdateScalingParametersResponseTypeDef",
     "DefineAnalysisSchemeResponseTypeDef",
     "DeleteAnalysisSchemeResponseTypeDef",
     "DescribeAnalysisSchemesResponseTypeDef",
     "DefineSuggesterResponseTypeDef",
     "DeleteSuggesterResponseTypeDef",
@@ -129,17 +149,31 @@
     {
         "UpdateVersion": int,
         "PendingDeletion": bool,
     },
     total=False,
 )
 
+
 class OptionStatusTypeDef(_RequiredOptionStatusTypeDef, _OptionalOptionStatusTypeDef):
     pass
 
+
+AnalysisOptionsOutputTypeDef = TypedDict(
+    "AnalysisOptionsOutputTypeDef",
+    {
+        "Synonyms": str,
+        "Stopwords": str,
+        "StemmingDictionary": str,
+        "JapaneseTokenizationDictionary": str,
+        "AlgorithmicStemming": AlgorithmicStemmingType,
+    },
+    total=False,
+)
+
 AnalysisOptionsTypeDef = TypedDict(
     "AnalysisOptionsTypeDef",
     {
         "Synonyms": str,
         "Stopwords": str,
         "StemmingDictionary": str,
         "JapaneseTokenizationDictionary": str,
@@ -166,26 +200,51 @@
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+DateArrayOptionsOutputTypeDef = TypedDict(
+    "DateArrayOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceFields": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+    },
+    total=False,
+)
+
 DateArrayOptionsTypeDef = TypedDict(
     "DateArrayOptionsTypeDef",
     {
         "DefaultValue": str,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
         "ReturnEnabled": bool,
     },
     total=False,
 )
 
+DateOptionsOutputTypeDef = TypedDict(
+    "DateOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceField": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+        "SortEnabled": bool,
+    },
+    total=False,
+)
+
 DateOptionsTypeDef = TypedDict(
     "DateOptionsTypeDef",
     {
         "DefaultValue": str,
         "SourceField": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
@@ -253,60 +312,66 @@
     {
         "AnalysisSchemeNames": Sequence[str],
         "Deployed": bool,
     },
     total=False,
 )
 
+
 class DescribeAnalysisSchemesRequestRequestTypeDef(
     _RequiredDescribeAnalysisSchemesRequestRequestTypeDef,
     _OptionalDescribeAnalysisSchemesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeAvailabilityOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAvailabilityOptionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalDescribeAvailabilityOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeAvailabilityOptionsRequestRequestTypeDef",
     {
         "Deployed": bool,
     },
     total=False,
 )
 
+
 class DescribeAvailabilityOptionsRequestRequestTypeDef(
     _RequiredDescribeAvailabilityOptionsRequestRequestTypeDef,
     _OptionalDescribeAvailabilityOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeDomainEndpointOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDomainEndpointOptionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalDescribeDomainEndpointOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeDomainEndpointOptionsRequestRequestTypeDef",
     {
         "Deployed": bool,
     },
     total=False,
 )
 
+
 class DescribeDomainEndpointOptionsRequestRequestTypeDef(
     _RequiredDescribeDomainEndpointOptionsRequestRequestTypeDef,
     _OptionalDescribeDomainEndpointOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeDomainsRequestRequestTypeDef = TypedDict(
     "DescribeDomainsRequestRequestTypeDef",
     {
         "DomainNames": Sequence[str],
     },
     total=False,
 )
@@ -322,20 +387,22 @@
     {
         "ExpressionNames": Sequence[str],
         "Deployed": bool,
     },
     total=False,
 )
 
+
 class DescribeExpressionsRequestRequestTypeDef(
     _RequiredDescribeExpressionsRequestRequestTypeDef,
     _OptionalDescribeExpressionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeIndexFieldsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeIndexFieldsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalDescribeIndexFieldsRequestRequestTypeDef = TypedDict(
@@ -343,20 +410,22 @@
     {
         "FieldNames": Sequence[str],
         "Deployed": bool,
     },
     total=False,
 )
 
+
 class DescribeIndexFieldsRequestRequestTypeDef(
     _RequiredDescribeIndexFieldsRequestRequestTypeDef,
     _OptionalDescribeIndexFieldsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeScalingParametersRequestRequestTypeDef = TypedDict(
     "DescribeScalingParametersRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -370,20 +439,22 @@
     "_OptionalDescribeServiceAccessPoliciesRequestRequestTypeDef",
     {
         "Deployed": bool,
     },
     total=False,
 )
 
+
 class DescribeServiceAccessPoliciesRequestRequestTypeDef(
     _RequiredDescribeServiceAccessPoliciesRequestRequestTypeDef,
     _OptionalDescribeServiceAccessPoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeSuggestersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSuggestersRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalDescribeSuggestersRequestRequestTypeDef = TypedDict(
@@ -391,20 +462,44 @@
     {
         "SuggesterNames": Sequence[str],
         "Deployed": bool,
     },
     total=False,
 )
 
+
 class DescribeSuggestersRequestRequestTypeDef(
     _RequiredDescribeSuggestersRequestRequestTypeDef,
     _OptionalDescribeSuggestersRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredDocumentSuggesterOptionsOutputTypeDef = TypedDict(
+    "_RequiredDocumentSuggesterOptionsOutputTypeDef",
+    {
+        "SourceField": str,
+    },
+)
+_OptionalDocumentSuggesterOptionsOutputTypeDef = TypedDict(
+    "_OptionalDocumentSuggesterOptionsOutputTypeDef",
+    {
+        "FuzzyMatching": SuggesterFuzzyMatchingType,
+        "SortExpression": str,
+    },
+    total=False,
+)
+
+
+class DocumentSuggesterOptionsOutputTypeDef(
+    _RequiredDocumentSuggesterOptionsOutputTypeDef, _OptionalDocumentSuggesterOptionsOutputTypeDef
+):
+    pass
+
+
 _RequiredDocumentSuggesterOptionsTypeDef = TypedDict(
     "_RequiredDocumentSuggesterOptionsTypeDef",
     {
         "SourceField": str,
     },
 )
 _OptionalDocumentSuggesterOptionsTypeDef = TypedDict(
@@ -412,19 +507,30 @@
     {
         "FuzzyMatching": SuggesterFuzzyMatchingType,
         "SortExpression": str,
     },
     total=False,
 )
 
+
 class DocumentSuggesterOptionsTypeDef(
     _RequiredDocumentSuggesterOptionsTypeDef, _OptionalDocumentSuggesterOptionsTypeDef
 ):
     pass
 
+
+DomainEndpointOptionsOutputTypeDef = TypedDict(
+    "DomainEndpointOptionsOutputTypeDef",
+    {
+        "EnforceHTTPS": bool,
+        "TLSSecurityPolicy": TLSSecurityPolicyType,
+    },
+    total=False,
+)
+
 DomainEndpointOptionsTypeDef = TypedDict(
     "DomainEndpointOptionsTypeDef",
     {
         "EnforceHTTPS": bool,
         "TLSSecurityPolicy": TLSSecurityPolicyType,
     },
     total=False,
@@ -442,39 +548,72 @@
     "ServiceEndpointTypeDef",
     {
         "Endpoint": str,
     },
     total=False,
 )
 
+DoubleArrayOptionsOutputTypeDef = TypedDict(
+    "DoubleArrayOptionsOutputTypeDef",
+    {
+        "DefaultValue": float,
+        "SourceFields": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+    },
+    total=False,
+)
+
 DoubleArrayOptionsTypeDef = TypedDict(
     "DoubleArrayOptionsTypeDef",
     {
         "DefaultValue": float,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
         "ReturnEnabled": bool,
     },
     total=False,
 )
 
+DoubleOptionsOutputTypeDef = TypedDict(
+    "DoubleOptionsOutputTypeDef",
+    {
+        "DefaultValue": float,
+        "SourceField": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+        "SortEnabled": bool,
+    },
+    total=False,
+)
+
 DoubleOptionsTypeDef = TypedDict(
     "DoubleOptionsTypeDef",
     {
         "DefaultValue": float,
         "SourceField": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
         "ReturnEnabled": bool,
         "SortEnabled": bool,
     },
     total=False,
 )
 
+ExpressionOutputTypeDef = TypedDict(
+    "ExpressionOutputTypeDef",
+    {
+        "ExpressionName": str,
+        "ExpressionValue": str,
+    },
+)
+
 IndexDocumentsRequestRequestTypeDef = TypedDict(
     "IndexDocumentsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -482,14 +621,102 @@
     "IndexDocumentsResponseTypeDef",
     {
         "FieldNames": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IntArrayOptionsOutputTypeDef = TypedDict(
+    "IntArrayOptionsOutputTypeDef",
+    {
+        "DefaultValue": int,
+        "SourceFields": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+    },
+    total=False,
+)
+
+IntOptionsOutputTypeDef = TypedDict(
+    "IntOptionsOutputTypeDef",
+    {
+        "DefaultValue": int,
+        "SourceField": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+        "SortEnabled": bool,
+    },
+    total=False,
+)
+
+LatLonOptionsOutputTypeDef = TypedDict(
+    "LatLonOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceField": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+        "SortEnabled": bool,
+    },
+    total=False,
+)
+
+LiteralArrayOptionsOutputTypeDef = TypedDict(
+    "LiteralArrayOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceFields": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+    },
+    total=False,
+)
+
+LiteralOptionsOutputTypeDef = TypedDict(
+    "LiteralOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceField": str,
+        "FacetEnabled": bool,
+        "SearchEnabled": bool,
+        "ReturnEnabled": bool,
+        "SortEnabled": bool,
+    },
+    total=False,
+)
+
+TextArrayOptionsOutputTypeDef = TypedDict(
+    "TextArrayOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceFields": str,
+        "ReturnEnabled": bool,
+        "HighlightEnabled": bool,
+        "AnalysisScheme": str,
+    },
+    total=False,
+)
+
+TextOptionsOutputTypeDef = TypedDict(
+    "TextOptionsOutputTypeDef",
+    {
+        "DefaultValue": str,
+        "SourceField": str,
+        "ReturnEnabled": bool,
+        "SortEnabled": bool,
+        "HighlightEnabled": bool,
+        "AnalysisScheme": str,
+    },
+    total=False,
+)
+
 IntArrayOptionsTypeDef = TypedDict(
     "IntArrayOptionsTypeDef",
     {
         "DefaultValue": int,
         "SourceFields": str,
         "FacetEnabled": bool,
         "SearchEnabled": bool,
@@ -589,14 +816,24 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+ScalingParametersOutputTypeDef = TypedDict(
+    "ScalingParametersOutputTypeDef",
+    {
+        "DesiredInstanceType": PartitionInstanceTypeType,
+        "DesiredReplicationCount": int,
+        "DesiredPartitionCount": int,
+    },
+    total=False,
+)
+
 ScalingParametersTypeDef = TypedDict(
     "ScalingParametersTypeDef",
     {
         "DesiredInstanceType": PartitionInstanceTypeType,
         "DesiredReplicationCount": int,
         "DesiredPartitionCount": int,
     },
@@ -631,14 +868,36 @@
     "AvailabilityOptionsStatusTypeDef",
     {
         "Options": bool,
         "Status": OptionStatusTypeDef,
     },
 )
 
+_RequiredAnalysisSchemeOutputTypeDef = TypedDict(
+    "_RequiredAnalysisSchemeOutputTypeDef",
+    {
+        "AnalysisSchemeName": str,
+        "AnalysisSchemeLanguage": AnalysisSchemeLanguageType,
+    },
+)
+_OptionalAnalysisSchemeOutputTypeDef = TypedDict(
+    "_OptionalAnalysisSchemeOutputTypeDef",
+    {
+        "AnalysisOptions": AnalysisOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class AnalysisSchemeOutputTypeDef(
+    _RequiredAnalysisSchemeOutputTypeDef, _OptionalAnalysisSchemeOutputTypeDef
+):
+    pass
+
+
 _RequiredAnalysisSchemeTypeDef = TypedDict(
     "_RequiredAnalysisSchemeTypeDef",
     {
         "AnalysisSchemeName": str,
         "AnalysisSchemeLanguage": AnalysisSchemeLanguageType,
     },
 )
@@ -646,45 +905,47 @@
     "_OptionalAnalysisSchemeTypeDef",
     {
         "AnalysisOptions": AnalysisOptionsTypeDef,
     },
     total=False,
 )
 
+
 class AnalysisSchemeTypeDef(_RequiredAnalysisSchemeTypeDef, _OptionalAnalysisSchemeTypeDef):
     pass
 
+
 DefineExpressionRequestRequestTypeDef = TypedDict(
     "DefineExpressionRequestRequestTypeDef",
     {
         "DomainName": str,
         "Expression": ExpressionTypeDef,
     },
 )
 
-ExpressionStatusTypeDef = TypedDict(
-    "ExpressionStatusTypeDef",
+SuggesterOutputTypeDef = TypedDict(
+    "SuggesterOutputTypeDef",
     {
-        "Options": ExpressionTypeDef,
-        "Status": OptionStatusTypeDef,
+        "SuggesterName": str,
+        "DocumentSuggesterOptions": DocumentSuggesterOptionsOutputTypeDef,
     },
 )
 
 SuggesterTypeDef = TypedDict(
     "SuggesterTypeDef",
     {
         "SuggesterName": str,
         "DocumentSuggesterOptions": DocumentSuggesterOptionsTypeDef,
     },
 )
 
 DomainEndpointOptionsStatusTypeDef = TypedDict(
     "DomainEndpointOptionsStatusTypeDef",
     {
-        "Options": DomainEndpointOptionsTypeDef,
+        "Options": DomainEndpointOptionsOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 UpdateDomainEndpointOptionsRequestRequestTypeDef = TypedDict(
     "UpdateDomainEndpointOptionsRequestRequestTypeDef",
     {
@@ -714,17 +975,57 @@
         "SearchPartitionCount": int,
         "SearchInstanceCount": int,
         "Limits": LimitsTypeDef,
     },
     total=False,
 )
 
+
 class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
     pass
 
+
+ExpressionStatusTypeDef = TypedDict(
+    "ExpressionStatusTypeDef",
+    {
+        "Options": ExpressionOutputTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+_RequiredIndexFieldOutputTypeDef = TypedDict(
+    "_RequiredIndexFieldOutputTypeDef",
+    {
+        "IndexFieldName": str,
+        "IndexFieldType": IndexFieldTypeType,
+    },
+)
+_OptionalIndexFieldOutputTypeDef = TypedDict(
+    "_OptionalIndexFieldOutputTypeDef",
+    {
+        "IntOptions": IntOptionsOutputTypeDef,
+        "DoubleOptions": DoubleOptionsOutputTypeDef,
+        "LiteralOptions": LiteralOptionsOutputTypeDef,
+        "TextOptions": TextOptionsOutputTypeDef,
+        "DateOptions": DateOptionsOutputTypeDef,
+        "LatLonOptions": LatLonOptionsOutputTypeDef,
+        "IntArrayOptions": IntArrayOptionsOutputTypeDef,
+        "DoubleArrayOptions": DoubleArrayOptionsOutputTypeDef,
+        "LiteralArrayOptions": LiteralArrayOptionsOutputTypeDef,
+        "TextArrayOptions": TextArrayOptionsOutputTypeDef,
+        "DateArrayOptions": DateArrayOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class IndexFieldOutputTypeDef(_RequiredIndexFieldOutputTypeDef, _OptionalIndexFieldOutputTypeDef):
+    pass
+
+
 _RequiredIndexFieldTypeDef = TypedDict(
     "_RequiredIndexFieldTypeDef",
     {
         "IndexFieldName": str,
         "IndexFieldType": IndexFieldTypeType,
     },
 )
@@ -742,21 +1043,23 @@
         "LiteralArrayOptions": LiteralArrayOptionsTypeDef,
         "TextArrayOptions": TextArrayOptionsTypeDef,
         "DateArrayOptions": DateArrayOptionsTypeDef,
     },
     total=False,
 )
 
+
 class IndexFieldTypeDef(_RequiredIndexFieldTypeDef, _OptionalIndexFieldTypeDef):
     pass
 
+
 ScalingParametersStatusTypeDef = TypedDict(
     "ScalingParametersStatusTypeDef",
     {
-        "Options": ScalingParametersTypeDef,
+        "Options": ScalingParametersOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 UpdateScalingParametersRequestRequestTypeDef = TypedDict(
     "UpdateScalingParametersRequestRequestTypeDef",
     {
@@ -796,67 +1099,43 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AnalysisSchemeStatusTypeDef = TypedDict(
     "AnalysisSchemeStatusTypeDef",
     {
-        "Options": AnalysisSchemeTypeDef,
+        "Options": AnalysisSchemeOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 DefineAnalysisSchemeRequestRequestTypeDef = TypedDict(
     "DefineAnalysisSchemeRequestRequestTypeDef",
     {
         "DomainName": str,
         "AnalysisScheme": AnalysisSchemeTypeDef,
     },
 )
 
-DefineExpressionResponseTypeDef = TypedDict(
-    "DefineExpressionResponseTypeDef",
-    {
-        "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteExpressionResponseTypeDef = TypedDict(
-    "DeleteExpressionResponseTypeDef",
-    {
-        "Expression": ExpressionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeExpressionsResponseTypeDef = TypedDict(
-    "DescribeExpressionsResponseTypeDef",
+SuggesterStatusTypeDef = TypedDict(
+    "SuggesterStatusTypeDef",
     {
-        "Expressions": List[ExpressionStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Options": SuggesterOutputTypeDef,
+        "Status": OptionStatusTypeDef,
     },
 )
 
 DefineSuggesterRequestRequestTypeDef = TypedDict(
     "DefineSuggesterRequestRequestTypeDef",
     {
         "DomainName": str,
         "Suggester": SuggesterTypeDef,
     },
 )
 
-SuggesterStatusTypeDef = TypedDict(
-    "SuggesterStatusTypeDef",
-    {
-        "Options": SuggesterTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
 DescribeDomainEndpointOptionsResponseTypeDef = TypedDict(
     "DescribeDomainEndpointOptionsResponseTypeDef",
     {
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -889,30 +1168,54 @@
     "DescribeDomainsResponseTypeDef",
     {
         "DomainStatusList": List[DomainStatusTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DefineIndexFieldRequestRequestTypeDef = TypedDict(
-    "DefineIndexFieldRequestRequestTypeDef",
+DefineExpressionResponseTypeDef = TypedDict(
+    "DefineExpressionResponseTypeDef",
     {
-        "DomainName": str,
-        "IndexField": IndexFieldTypeDef,
+        "Expression": ExpressionStatusTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteExpressionResponseTypeDef = TypedDict(
+    "DeleteExpressionResponseTypeDef",
+    {
+        "Expression": ExpressionStatusTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeExpressionsResponseTypeDef = TypedDict(
+    "DescribeExpressionsResponseTypeDef",
+    {
+        "Expressions": List[ExpressionStatusTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IndexFieldStatusTypeDef = TypedDict(
     "IndexFieldStatusTypeDef",
     {
-        "Options": IndexFieldTypeDef,
+        "Options": IndexFieldOutputTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
+DefineIndexFieldRequestRequestTypeDef = TypedDict(
+    "DefineIndexFieldRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "IndexField": IndexFieldTypeDef,
+    },
+)
+
 DescribeScalingParametersResponseTypeDef = TypedDict(
     "DescribeScalingParametersResponseTypeDef",
     {
         "ScalingParameters": ScalingParametersStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudsearch-1.28.0/mypy_boto3_cloudsearch.egg-info/SOURCES.txt` & `mypy-boto3-cloudsearch-1.28.12/mypy_boto3_cloudsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.0/setup.py` & `mypy-boto3-cloudsearch-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudsearch",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cloudsearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudSearch 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CloudSearch 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

