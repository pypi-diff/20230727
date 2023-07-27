# Comparing `tmp/mypy-boto3-comprehendmedical-1.28.0.tar.gz` & `tmp/mypy-boto3-comprehendmedical-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-comprehendmedical-1.28.0.tar", last modified: Thu Jul  6 20:59:17 2023, max compression
+gzip compressed data, was "mypy-boto3-comprehendmedical-1.28.12.tar", last modified: Thu Jul 27 05:34:30 2023, max compression
```

## Comparing `mypy-boto3-comprehendmedical-1.28.0.tar` & `mypy-boto3-comprehendmedical-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:17.954263 mypy-boto3-comprehendmedical-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:37.000000 mypy-boto3-comprehendmedical-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-07-06 20:59:17.954263 mypy-boto3-comprehendmedical-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-07-06 20:36:37.000000 mypy-boto3-comprehendmedical-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:17.954263 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-06 20:36:37.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 20:36:37.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 20:36:37.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-07-06 20:36:37.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-07-06 20:36:37.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-06 20:36:37.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-07-06 20:36:37.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:37.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24942 2023-07-06 20:36:39.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24927 2023-07-06 20:36:39.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:37.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:17.954263 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-07-06 20:59:17.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-06 20:59:17.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:17.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:17.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:17.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:59:17.000000 mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:17.954263 mypy-boto3-comprehendmedical-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-06 20:36:37.000000 mypy-boto3-comprehendmedical-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:30.620545 mypy-boto3-comprehendmedical-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15900 2023-07-27 05:34:30.620545 mypy-boto3-comprehendmedical-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:30.620545 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-07-27 05:19:29.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25853 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:30.620545 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15900 2023-07-27 05:34:30.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-27 05:34:30.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:30.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:30.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:30.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:30.000000 mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:30.620545 mypy-boto3-comprehendmedical-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-27 05:19:28.000000 mypy-boto3-comprehendmedical-1.28.12/setup.py
```

### Comparing `mypy-boto3-comprehendmedical-1.28.0/LICENSE` & `mypy-boto3-comprehendmedical-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.0/PKG-INFO` & `mypy-boto3-comprehendmedical-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehendmedical
-Version: 1.28.0
-Summary: Type annotations for boto3.ComprehendMedical 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ComprehendMedical 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-comprehendmedical"></a>
 
 # mypy-boto3-comprehendmedical
 
 [![PyPI - mypy-boto3-comprehendmedical](https://img.shields.io/pypi/v/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehendmedical?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehendmedical)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehendmedical)](https://pepy.tech/project/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
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
 [mypy-boto3-comprehendmedical docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,30 +320,32 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
     ComprehendMedicalAsyncJobFilterTypeDef,
-    InputDataConfigTypeDef,
-    OutputDataConfigTypeDef,
+    InputDataConfigOutputTypeDef,
+    OutputDataConfigOutputTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
     DescribeSNOMEDCTInferenceJobRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     DetectEntitiesV2RequestRequestTypeDef,
     DetectPHIRequestRequestTypeDef,
     ICD10CMTraitTypeDef,
     ICD10CMConceptTypeDef,
     InferICD10CMRequestRequestTypeDef,
     InferRxNormRequestRequestTypeDef,
     InferSNOMEDCTRequestRequestTypeDef,
     SNOMEDCTDetailsTypeDef,
+    InputDataConfigTypeDef,
+    OutputDataConfigTypeDef,
     ResponseMetadataTypeDef,
     RxNormTraitTypeDef,
     RxNormConceptTypeDef,
     SNOMEDCTConceptTypeDef,
     SNOMEDCTTraitTypeDef,
     StartEntitiesDetectionV2JobResponseTypeDef,
     StartICD10CMInferenceJobResponseTypeDef,
@@ -363,20 +365,20 @@
     AttributeTypeDef,
     ListEntitiesDetectionV2JobsRequestRequestTypeDef,
     ListICD10CMInferenceJobsRequestRequestTypeDef,
     ListPHIDetectionJobsRequestRequestTypeDef,
     ListRxNormInferenceJobsRequestRequestTypeDef,
     ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
+    ICD10CMAttributeTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
-    ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
     DescribePHIDetectionJobResponseTypeDef,
```

### Comparing `mypy-boto3-comprehendmedical-1.28.0/README.md` & `mypy-boto3-comprehendmedical-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-comprehendmedical"></a>
 
 # mypy-boto3-comprehendmedical
 
 [![PyPI - mypy-boto3-comprehendmedical](https://img.shields.io/pypi/v/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehendmedical?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehendmedical)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehendmedical)](https://pepy.tech/project/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
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
 [mypy-boto3-comprehendmedical docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,30 +288,32 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
     ComprehendMedicalAsyncJobFilterTypeDef,
-    InputDataConfigTypeDef,
-    OutputDataConfigTypeDef,
+    InputDataConfigOutputTypeDef,
+    OutputDataConfigOutputTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
     DescribeSNOMEDCTInferenceJobRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     DetectEntitiesV2RequestRequestTypeDef,
     DetectPHIRequestRequestTypeDef,
     ICD10CMTraitTypeDef,
     ICD10CMConceptTypeDef,
     InferICD10CMRequestRequestTypeDef,
     InferRxNormRequestRequestTypeDef,
     InferSNOMEDCTRequestRequestTypeDef,
     SNOMEDCTDetailsTypeDef,
+    InputDataConfigTypeDef,
+    OutputDataConfigTypeDef,
     ResponseMetadataTypeDef,
     RxNormTraitTypeDef,
     RxNormConceptTypeDef,
     SNOMEDCTConceptTypeDef,
     SNOMEDCTTraitTypeDef,
     StartEntitiesDetectionV2JobResponseTypeDef,
     StartICD10CMInferenceJobResponseTypeDef,
@@ -331,20 +333,20 @@
     AttributeTypeDef,
     ListEntitiesDetectionV2JobsRequestRequestTypeDef,
     ListICD10CMInferenceJobsRequestRequestTypeDef,
     ListPHIDetectionJobsRequestRequestTypeDef,
     ListRxNormInferenceJobsRequestRequestTypeDef,
     ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
+    ICD10CMAttributeTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
-    ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
     DescribePHIDetectionJobResponseTypeDef,
```

### Comparing `mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/__main__.py` & `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ComprehendMedical 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ComprehendMedical 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical\nOther"
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

### Comparing `mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/client.py` & `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/client.pyi` & `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/literals.py` & `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,14 +310,15 @@
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
@@ -396,26 +397,28 @@
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

### Comparing `mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/literals.pyi` & `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -308,14 +308,15 @@
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
@@ -394,26 +395,28 @@
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

### Comparing `mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/type_defs.py` & `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,30 +45,32 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TraitTypeDef",
     "CharactersTypeDef",
     "ComprehendMedicalAsyncJobFilterTypeDef",
-    "InputDataConfigTypeDef",
-    "OutputDataConfigTypeDef",
+    "InputDataConfigOutputTypeDef",
+    "OutputDataConfigOutputTypeDef",
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     "DescribePHIDetectionJobRequestRequestTypeDef",
     "DescribeRxNormInferenceJobRequestRequestTypeDef",
     "DescribeSNOMEDCTInferenceJobRequestRequestTypeDef",
     "DetectEntitiesRequestRequestTypeDef",
     "DetectEntitiesV2RequestRequestTypeDef",
     "DetectPHIRequestRequestTypeDef",
     "ICD10CMTraitTypeDef",
     "ICD10CMConceptTypeDef",
     "InferICD10CMRequestRequestTypeDef",
     "InferRxNormRequestRequestTypeDef",
     "InferSNOMEDCTRequestRequestTypeDef",
     "SNOMEDCTDetailsTypeDef",
+    "InputDataConfigTypeDef",
+    "OutputDataConfigTypeDef",
     "ResponseMetadataTypeDef",
     "RxNormTraitTypeDef",
     "RxNormConceptTypeDef",
     "SNOMEDCTConceptTypeDef",
     "SNOMEDCTTraitTypeDef",
     "StartEntitiesDetectionV2JobResponseTypeDef",
     "StartICD10CMInferenceJobResponseTypeDef",
@@ -88,20 +90,20 @@
     "AttributeTypeDef",
     "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
     "ListICD10CMInferenceJobsRequestRequestTypeDef",
     "ListPHIDetectionJobsRequestRequestTypeDef",
     "ListRxNormInferenceJobsRequestRequestTypeDef",
     "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
+    "ICD10CMAttributeTypeDef",
     "StartEntitiesDetectionV2JobRequestRequestTypeDef",
     "StartICD10CMInferenceJobRequestRequestTypeDef",
     "StartPHIDetectionJobRequestRequestTypeDef",
     "StartRxNormInferenceJobRequestRequestTypeDef",
     "StartSNOMEDCTInferenceJobRequestRequestTypeDef",
-    "ICD10CMAttributeTypeDef",
     "RxNormAttributeTypeDef",
     "SNOMEDCTAttributeTypeDef",
     "EntityTypeDef",
     "UnmappedAttributeTypeDef",
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     "DescribeICD10CMInferenceJobResponseTypeDef",
     "DescribePHIDetectionJobResponseTypeDef",
@@ -147,49 +149,53 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredInputDataConfigTypeDef = TypedDict(
-    "_RequiredInputDataConfigTypeDef",
+_RequiredInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredInputDataConfigOutputTypeDef",
     {
         "S3Bucket": str,
     },
 )
-_OptionalInputDataConfigTypeDef = TypedDict(
-    "_OptionalInputDataConfigTypeDef",
+_OptionalInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalInputDataConfigOutputTypeDef",
     {
         "S3Key": str,
     },
     total=False,
 )
 
 
-class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
+class InputDataConfigOutputTypeDef(
+    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
+):
     pass
 
 
-_RequiredOutputDataConfigTypeDef = TypedDict(
-    "_RequiredOutputDataConfigTypeDef",
+_RequiredOutputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredOutputDataConfigOutputTypeDef",
     {
         "S3Bucket": str,
     },
 )
-_OptionalOutputDataConfigTypeDef = TypedDict(
-    "_OptionalOutputDataConfigTypeDef",
+_OptionalOutputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalOutputDataConfigOutputTypeDef",
     {
         "S3Key": str,
     },
     total=False,
 )
 
 
-class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
+class OutputDataConfigOutputTypeDef(
+    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
+):
     pass
 
 
 DescribeEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
@@ -291,14 +297,52 @@
         "Edition": str,
         "Language": str,
         "VersionDate": str,
     },
     total=False,
 )
 
+_RequiredInputDataConfigTypeDef = TypedDict(
+    "_RequiredInputDataConfigTypeDef",
+    {
+        "S3Bucket": str,
+    },
+)
+_OptionalInputDataConfigTypeDef = TypedDict(
+    "_OptionalInputDataConfigTypeDef",
+    {
+        "S3Key": str,
+    },
+    total=False,
+)
+
+
+class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
+    pass
+
+
+_RequiredOutputDataConfigTypeDef = TypedDict(
+    "_RequiredOutputDataConfigTypeDef",
+    {
+        "S3Bucket": str,
+    },
+)
+_OptionalOutputDataConfigTypeDef = TypedDict(
+    "_OptionalOutputDataConfigTypeDef",
+    {
+        "S3Key": str,
+    },
+    total=False,
+)
+
+
+class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
+    pass
+
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -532,25 +576,42 @@
         "JobId": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "ExpirationTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
         "LanguageCode": Literal["en"],
         "DataAccessRoleArn": str,
         "ManifestFilePath": str,
         "KMSKey": str,
         "ModelVersion": str,
     },
     total=False,
 )
 
+ICD10CMAttributeTypeDef = TypedDict(
+    "ICD10CMAttributeTypeDef",
+    {
+        "Type": ICD10CMAttributeTypeType,
+        "Score": float,
+        "RelationshipScore": float,
+        "Id": int,
+        "BeginOffset": int,
+        "EndOffset": int,
+        "Text": str,
+        "Traits": List[ICD10CMTraitTypeDef],
+        "Category": ICD10CMEntityTypeType,
+        "RelationshipType": ICD10CMRelationshipTypeType,
+    },
+    total=False,
+)
+
 _RequiredStartEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "_RequiredStartEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": Literal["en"],
@@ -678,31 +739,14 @@
 class StartSNOMEDCTInferenceJobRequestRequestTypeDef(
     _RequiredStartSNOMEDCTInferenceJobRequestRequestTypeDef,
     _OptionalStartSNOMEDCTInferenceJobRequestRequestTypeDef,
 ):
     pass
 
 
-ICD10CMAttributeTypeDef = TypedDict(
-    "ICD10CMAttributeTypeDef",
-    {
-        "Type": ICD10CMAttributeTypeType,
-        "Score": float,
-        "RelationshipScore": float,
-        "Id": int,
-        "BeginOffset": int,
-        "EndOffset": int,
-        "Text": str,
-        "Traits": List[ICD10CMTraitTypeDef],
-        "Category": ICD10CMEntityTypeType,
-        "RelationshipType": ICD10CMRelationshipTypeType,
-    },
-    total=False,
-)
-
 RxNormAttributeTypeDef = TypedDict(
     "RxNormAttributeTypeDef",
     {
         "Type": RxNormAttributeTypeType,
         "Score": float,
         "RelationshipScore": float,
         "Id": int,
```

### Comparing `mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical/type_defs.pyi` & `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,30 +44,32 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TraitTypeDef",
     "CharactersTypeDef",
     "ComprehendMedicalAsyncJobFilterTypeDef",
-    "InputDataConfigTypeDef",
-    "OutputDataConfigTypeDef",
+    "InputDataConfigOutputTypeDef",
+    "OutputDataConfigOutputTypeDef",
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     "DescribePHIDetectionJobRequestRequestTypeDef",
     "DescribeRxNormInferenceJobRequestRequestTypeDef",
     "DescribeSNOMEDCTInferenceJobRequestRequestTypeDef",
     "DetectEntitiesRequestRequestTypeDef",
     "DetectEntitiesV2RequestRequestTypeDef",
     "DetectPHIRequestRequestTypeDef",
     "ICD10CMTraitTypeDef",
     "ICD10CMConceptTypeDef",
     "InferICD10CMRequestRequestTypeDef",
     "InferRxNormRequestRequestTypeDef",
     "InferSNOMEDCTRequestRequestTypeDef",
     "SNOMEDCTDetailsTypeDef",
+    "InputDataConfigTypeDef",
+    "OutputDataConfigTypeDef",
     "ResponseMetadataTypeDef",
     "RxNormTraitTypeDef",
     "RxNormConceptTypeDef",
     "SNOMEDCTConceptTypeDef",
     "SNOMEDCTTraitTypeDef",
     "StartEntitiesDetectionV2JobResponseTypeDef",
     "StartICD10CMInferenceJobResponseTypeDef",
@@ -87,20 +89,20 @@
     "AttributeTypeDef",
     "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
     "ListICD10CMInferenceJobsRequestRequestTypeDef",
     "ListPHIDetectionJobsRequestRequestTypeDef",
     "ListRxNormInferenceJobsRequestRequestTypeDef",
     "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
+    "ICD10CMAttributeTypeDef",
     "StartEntitiesDetectionV2JobRequestRequestTypeDef",
     "StartICD10CMInferenceJobRequestRequestTypeDef",
     "StartPHIDetectionJobRequestRequestTypeDef",
     "StartRxNormInferenceJobRequestRequestTypeDef",
     "StartSNOMEDCTInferenceJobRequestRequestTypeDef",
-    "ICD10CMAttributeTypeDef",
     "RxNormAttributeTypeDef",
     "SNOMEDCTAttributeTypeDef",
     "EntityTypeDef",
     "UnmappedAttributeTypeDef",
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     "DescribeICD10CMInferenceJobResponseTypeDef",
     "DescribePHIDetectionJobResponseTypeDef",
@@ -146,46 +148,50 @@
         "JobStatus": JobStatusType,
         "SubmitTimeBefore": Union[datetime, str],
         "SubmitTimeAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredInputDataConfigTypeDef = TypedDict(
-    "_RequiredInputDataConfigTypeDef",
+_RequiredInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredInputDataConfigOutputTypeDef",
     {
         "S3Bucket": str,
     },
 )
-_OptionalInputDataConfigTypeDef = TypedDict(
-    "_OptionalInputDataConfigTypeDef",
+_OptionalInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalInputDataConfigOutputTypeDef",
     {
         "S3Key": str,
     },
     total=False,
 )
 
-class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
+class InputDataConfigOutputTypeDef(
+    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
+):
     pass
 
-_RequiredOutputDataConfigTypeDef = TypedDict(
-    "_RequiredOutputDataConfigTypeDef",
+_RequiredOutputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredOutputDataConfigOutputTypeDef",
     {
         "S3Bucket": str,
     },
 )
-_OptionalOutputDataConfigTypeDef = TypedDict(
-    "_OptionalOutputDataConfigTypeDef",
+_OptionalOutputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalOutputDataConfigOutputTypeDef",
     {
         "S3Key": str,
     },
     total=False,
 )
 
-class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
+class OutputDataConfigOutputTypeDef(
+    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
+):
     pass
 
 DescribeEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
@@ -286,14 +292,48 @@
         "Edition": str,
         "Language": str,
         "VersionDate": str,
     },
     total=False,
 )
 
+_RequiredInputDataConfigTypeDef = TypedDict(
+    "_RequiredInputDataConfigTypeDef",
+    {
+        "S3Bucket": str,
+    },
+)
+_OptionalInputDataConfigTypeDef = TypedDict(
+    "_OptionalInputDataConfigTypeDef",
+    {
+        "S3Key": str,
+    },
+    total=False,
+)
+
+class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
+    pass
+
+_RequiredOutputDataConfigTypeDef = TypedDict(
+    "_RequiredOutputDataConfigTypeDef",
+    {
+        "S3Bucket": str,
+    },
+)
+_OptionalOutputDataConfigTypeDef = TypedDict(
+    "_OptionalOutputDataConfigTypeDef",
+    {
+        "S3Key": str,
+    },
+    total=False,
+)
+
+class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
+    pass
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -527,25 +567,42 @@
         "JobId": str,
         "JobName": str,
         "JobStatus": JobStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "ExpirationTime": datetime,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
         "LanguageCode": Literal["en"],
         "DataAccessRoleArn": str,
         "ManifestFilePath": str,
         "KMSKey": str,
         "ModelVersion": str,
     },
     total=False,
 )
 
+ICD10CMAttributeTypeDef = TypedDict(
+    "ICD10CMAttributeTypeDef",
+    {
+        "Type": ICD10CMAttributeTypeType,
+        "Score": float,
+        "RelationshipScore": float,
+        "Id": int,
+        "BeginOffset": int,
+        "EndOffset": int,
+        "Text": str,
+        "Traits": List[ICD10CMTraitTypeDef],
+        "Category": ICD10CMEntityTypeType,
+        "RelationshipType": ICD10CMRelationshipTypeType,
+    },
+    total=False,
+)
+
 _RequiredStartEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "_RequiredStartEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "LanguageCode": Literal["en"],
@@ -663,31 +720,14 @@
 
 class StartSNOMEDCTInferenceJobRequestRequestTypeDef(
     _RequiredStartSNOMEDCTInferenceJobRequestRequestTypeDef,
     _OptionalStartSNOMEDCTInferenceJobRequestRequestTypeDef,
 ):
     pass
 
-ICD10CMAttributeTypeDef = TypedDict(
-    "ICD10CMAttributeTypeDef",
-    {
-        "Type": ICD10CMAttributeTypeType,
-        "Score": float,
-        "RelationshipScore": float,
-        "Id": int,
-        "BeginOffset": int,
-        "EndOffset": int,
-        "Text": str,
-        "Traits": List[ICD10CMTraitTypeDef],
-        "Category": ICD10CMEntityTypeType,
-        "RelationshipType": ICD10CMRelationshipTypeType,
-    },
-    total=False,
-)
-
 RxNormAttributeTypeDef = TypedDict(
     "RxNormAttributeTypeDef",
     {
         "Type": RxNormAttributeTypeType,
         "Score": float,
         "RelationshipScore": float,
         "Id": int,
```

### Comparing `mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical.egg-info/PKG-INFO` & `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehendmedical
-Version: 1.28.0
-Summary: Type annotations for boto3.ComprehendMedical 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ComprehendMedical 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-comprehendmedical"></a>
 
 # mypy-boto3-comprehendmedical
 
 [![PyPI - mypy-boto3-comprehendmedical](https://img.shields.io/pypi/v/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehendmedical?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehendmedical)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-comprehendmedical)](https://pepy.tech/project/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
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
 [mypy-boto3-comprehendmedical docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,30 +320,32 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
     ComprehendMedicalAsyncJobFilterTypeDef,
-    InputDataConfigTypeDef,
-    OutputDataConfigTypeDef,
+    InputDataConfigOutputTypeDef,
+    OutputDataConfigOutputTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
     DescribeSNOMEDCTInferenceJobRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     DetectEntitiesV2RequestRequestTypeDef,
     DetectPHIRequestRequestTypeDef,
     ICD10CMTraitTypeDef,
     ICD10CMConceptTypeDef,
     InferICD10CMRequestRequestTypeDef,
     InferRxNormRequestRequestTypeDef,
     InferSNOMEDCTRequestRequestTypeDef,
     SNOMEDCTDetailsTypeDef,
+    InputDataConfigTypeDef,
+    OutputDataConfigTypeDef,
     ResponseMetadataTypeDef,
     RxNormTraitTypeDef,
     RxNormConceptTypeDef,
     SNOMEDCTConceptTypeDef,
     SNOMEDCTTraitTypeDef,
     StartEntitiesDetectionV2JobResponseTypeDef,
     StartICD10CMInferenceJobResponseTypeDef,
@@ -363,20 +365,20 @@
     AttributeTypeDef,
     ListEntitiesDetectionV2JobsRequestRequestTypeDef,
     ListICD10CMInferenceJobsRequestRequestTypeDef,
     ListPHIDetectionJobsRequestRequestTypeDef,
     ListRxNormInferenceJobsRequestRequestTypeDef,
     ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
+    ICD10CMAttributeTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
-    ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
     DescribePHIDetectionJobResponseTypeDef,
```

### Comparing `mypy-boto3-comprehendmedical-1.28.0/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt` & `mypy-boto3-comprehendmedical-1.28.12/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.28.0/setup.py` & `mypy-boto3-comprehendmedical-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-comprehendmedical",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_comprehendmedical"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ComprehendMedical 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ComprehendMedical 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

