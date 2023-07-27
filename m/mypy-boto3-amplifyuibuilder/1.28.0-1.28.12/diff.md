# Comparing `tmp/mypy-boto3-amplifyuibuilder-1.28.0.tar.gz` & `tmp/mypy-boto3-amplifyuibuilder-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplifyuibuilder-1.28.0.tar", last modified: Thu Jul  6 20:58:55 2023, max compression
+gzip compressed data, was "mypy-boto3-amplifyuibuilder-1.28.12.tar", last modified: Thu Jul 27 05:34:16 2023, max compression
```

## Comparing `mypy-boto3-amplifyuibuilder-1.28.0.tar` & `mypy-boto3-amplifyuibuilder-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.394214 mypy-boto3-amplifyuibuilder-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:32:50.000000 mypy-boto3-amplifyuibuilder-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18372 2023-07-06 20:58:55.390214 mypy-boto3-amplifyuibuilder-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-07-06 20:32:50.000000 mypy-boto3-amplifyuibuilder-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.386214 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-06 20:32:50.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-06 20:32:50.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-06 20:32:50.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-07-06 20:32:51.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21995 2023-07-06 20:32:50.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-07-06 20:32:51.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-06 20:32:51.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-07-06 20:32:51.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-07-06 20:32:51.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:50.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48015 2023-07-06 20:32:52.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47923 2023-07-06 20:32:52.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:32:50.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.390214 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18372 2023-07-06 20:58:55.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 20:58:55.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:55.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 20:58:55.000000 mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:55.394214 mypy-boto3-amplifyuibuilder-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 20:32:50.000000 mypy-boto3-amplifyuibuilder-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.320584 mypy-boto3-amplifyuibuilder-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-07-27 05:34:16.316584 mypy-boto3-amplifyuibuilder-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.308584 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21995 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65450 2023-07-27 05:17:07.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65332 2023-07-27 05:17:06.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.316584 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-07-27 05:34:16.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:34:16.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:16.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:16.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:16.320584 mypy-boto3-amplifyuibuilder-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/setup.py
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/LICENSE` & `mypy-boto3-amplifyuibuilder-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/PKG-INFO` & `mypy-boto3-amplifyuibuilder-1.28.12/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifyuibuilder
-Version: 1.28.0
-Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-amplifyuibuilder"></a>
 
 # mypy-boto3-amplifyuibuilder
 
 [![PyPI - mypy-boto3-amplifyuibuilder](https://img.shields.io/pypi/v/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplifyuibuilder?color=blue)](https://pypistats.org/packages/mypy-boto3-amplifyuibuilder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifyuibuilder)](https://pepy.tech/project/mypy-boto3-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyUIBuilder 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[boto3.AmplifyUIBuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
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
 [mypy-boto3-amplifyuibuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,36 +355,54 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
+    ActionParametersOutputTypeDef,
     ActionParametersTypeDef,
+    CodegenFeatureFlagsOutputTypeDef,
     CodegenFeatureFlagsTypeDef,
+    CodegenGenericDataEnumOutputTypeDef,
     CodegenGenericDataEnumTypeDef,
+    CodegenGenericDataFieldOutputTypeDef,
     CodegenGenericDataFieldTypeDef,
+    CodegenGenericDataModelOutputTypeDef,
     CodegenGenericDataModelTypeDef,
+    CodegenGenericDataNonModelOutputTypeDef,
     CodegenGenericDataNonModelTypeDef,
+    CodegenGenericDataRelationshipTypeOutputTypeDef,
     CodegenGenericDataRelationshipTypeTypeDef,
     CodegenJobAssetTypeDef,
+    CodegenJobGenericDataSchemaOutputTypeDef,
     CodegenJobGenericDataSchemaTypeDef,
+    CodegenJobRenderConfigOutputTypeDef,
     CodegenJobRenderConfigTypeDef,
     CodegenJobSummaryTypeDef,
     CodegenJobTypeDef,
+    ComponentBindingPropertiesValueOutputTypeDef,
+    ComponentBindingPropertiesValuePropertiesOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
     ComponentBindingPropertiesValueTypeDef,
+    ComponentChildOutputTypeDef,
     ComponentChildTypeDef,
+    ComponentConditionPropertyOutputTypeDef,
     ComponentConditionPropertyTypeDef,
+    ComponentDataConfigurationOutputTypeDef,
     ComponentDataConfigurationTypeDef,
+    ComponentEventOutputTypeDef,
     ComponentEventTypeDef,
+    ComponentPropertyBindingPropertiesOutputTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
+    ComponentPropertyOutputTypeDef,
     ComponentPropertyTypeDef,
     ComponentSummaryTypeDef,
     ComponentTypeDef,
+    ComponentVariantOutputTypeDef,
     ComponentVariantTypeDef,
     CreateComponentDataTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateComponentResponseTypeDef,
     CreateFormDataTypeDef,
     CreateFormRequestRequestTypeDef,
     CreateFormResponseTypeDef,
@@ -403,28 +421,43 @@
     ExportComponentsResponseTypeDef,
     ExportFormsRequestExportFormsPaginateTypeDef,
     ExportFormsRequestRequestTypeDef,
     ExportFormsResponseTypeDef,
     ExportThemesRequestExportThemesPaginateTypeDef,
     ExportThemesRequestRequestTypeDef,
     ExportThemesResponseTypeDef,
+    FieldConfigOutputTypeDef,
     FieldConfigTypeDef,
+    FieldInputConfigOutputTypeDef,
     FieldInputConfigTypeDef,
+    FieldPositionOutputTypeDef,
     FieldPositionTypeDef,
+    FieldValidationConfigurationOutputTypeDef,
     FieldValidationConfigurationTypeDef,
+    FileUploaderFieldConfigOutputTypeDef,
     FileUploaderFieldConfigTypeDef,
+    FormBindingElementOutputTypeDef,
     FormBindingElementTypeDef,
+    FormButtonOutputTypeDef,
     FormButtonTypeDef,
+    FormCTAOutputTypeDef,
     FormCTATypeDef,
+    FormDataTypeConfigOutputTypeDef,
     FormDataTypeConfigTypeDef,
+    FormInputBindingPropertiesValueOutputTypeDef,
+    FormInputBindingPropertiesValuePropertiesOutputTypeDef,
     FormInputBindingPropertiesValuePropertiesTypeDef,
     FormInputBindingPropertiesValueTypeDef,
+    FormInputValuePropertyBindingPropertiesOutputTypeDef,
     FormInputValuePropertyBindingPropertiesTypeDef,
+    FormInputValuePropertyOutputTypeDef,
     FormInputValuePropertyTypeDef,
+    FormStyleConfigOutputTypeDef,
     FormStyleConfigTypeDef,
+    FormStyleOutputTypeDef,
     FormStyleTypeDef,
     FormSummaryTypeDef,
     FormTypeDef,
     GetCodegenJobRequestRequestTypeDef,
     GetCodegenJobResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetComponentResponseTypeDef,
@@ -442,48 +475,57 @@
     ListComponentsResponseTypeDef,
     ListFormsRequestListFormsPaginateTypeDef,
     ListFormsRequestRequestTypeDef,
     ListFormsResponseTypeDef,
     ListThemesRequestListThemesPaginateTypeDef,
     ListThemesRequestRequestTypeDef,
     ListThemesResponseTypeDef,
+    MutationActionSetStateParameterOutputTypeDef,
     MutationActionSetStateParameterTypeDef,
     PaginatorConfigTypeDef,
+    PredicateOutputTypeDef,
     PredicateTypeDef,
     PutMetadataFlagBodyTypeDef,
     PutMetadataFlagRequestRequestTypeDef,
+    ReactStartCodegenJobDataOutputTypeDef,
     ReactStartCodegenJobDataTypeDef,
     RefreshTokenRequestBodyTypeDef,
     RefreshTokenRequestRequestTypeDef,
     RefreshTokenResponseTypeDef,
     ResponseMetadataTypeDef,
+    SectionalElementOutputTypeDef,
     SectionalElementTypeDef,
+    SortPropertyOutputTypeDef,
     SortPropertyTypeDef,
     StartCodegenJobDataTypeDef,
     StartCodegenJobRequestRequestTypeDef,
     StartCodegenJobResponseTypeDef,
     ThemeSummaryTypeDef,
     ThemeTypeDef,
+    ThemeValueOutputTypeDef,
     ThemeValueTypeDef,
+    ThemeValuesOutputTypeDef,
     ThemeValuesTypeDef,
     UpdateComponentDataTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateComponentResponseTypeDef,
     UpdateFormDataTypeDef,
     UpdateFormRequestRequestTypeDef,
     UpdateFormResponseTypeDef,
     UpdateThemeDataTypeDef,
     UpdateThemeRequestRequestTypeDef,
     UpdateThemeResponseTypeDef,
+    ValueMappingOutputTypeDef,
     ValueMappingTypeDef,
+    ValueMappingsOutputTypeDef,
     ValueMappingsTypeDef,
 )
 
 
-def get_structure() -> ActionParametersTypeDef:
+def get_structure() -> ActionParametersOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/README.md` & `mypy-boto3-amplifyuibuilder-1.28.12/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-amplifyuibuilder"></a>
 
 # mypy-boto3-amplifyuibuilder
 
 [![PyPI - mypy-boto3-amplifyuibuilder](https://img.shields.io/pypi/v/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplifyuibuilder?color=blue)](https://pypistats.org/packages/mypy-boto3-amplifyuibuilder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifyuibuilder)](https://pepy.tech/project/mypy-boto3-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyUIBuilder 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[boto3.AmplifyUIBuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
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
 [mypy-boto3-amplifyuibuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,36 +323,54 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
+    ActionParametersOutputTypeDef,
     ActionParametersTypeDef,
+    CodegenFeatureFlagsOutputTypeDef,
     CodegenFeatureFlagsTypeDef,
+    CodegenGenericDataEnumOutputTypeDef,
     CodegenGenericDataEnumTypeDef,
+    CodegenGenericDataFieldOutputTypeDef,
     CodegenGenericDataFieldTypeDef,
+    CodegenGenericDataModelOutputTypeDef,
     CodegenGenericDataModelTypeDef,
+    CodegenGenericDataNonModelOutputTypeDef,
     CodegenGenericDataNonModelTypeDef,
+    CodegenGenericDataRelationshipTypeOutputTypeDef,
     CodegenGenericDataRelationshipTypeTypeDef,
     CodegenJobAssetTypeDef,
+    CodegenJobGenericDataSchemaOutputTypeDef,
     CodegenJobGenericDataSchemaTypeDef,
+    CodegenJobRenderConfigOutputTypeDef,
     CodegenJobRenderConfigTypeDef,
     CodegenJobSummaryTypeDef,
     CodegenJobTypeDef,
+    ComponentBindingPropertiesValueOutputTypeDef,
+    ComponentBindingPropertiesValuePropertiesOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
     ComponentBindingPropertiesValueTypeDef,
+    ComponentChildOutputTypeDef,
     ComponentChildTypeDef,
+    ComponentConditionPropertyOutputTypeDef,
     ComponentConditionPropertyTypeDef,
+    ComponentDataConfigurationOutputTypeDef,
     ComponentDataConfigurationTypeDef,
+    ComponentEventOutputTypeDef,
     ComponentEventTypeDef,
+    ComponentPropertyBindingPropertiesOutputTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
+    ComponentPropertyOutputTypeDef,
     ComponentPropertyTypeDef,
     ComponentSummaryTypeDef,
     ComponentTypeDef,
+    ComponentVariantOutputTypeDef,
     ComponentVariantTypeDef,
     CreateComponentDataTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateComponentResponseTypeDef,
     CreateFormDataTypeDef,
     CreateFormRequestRequestTypeDef,
     CreateFormResponseTypeDef,
@@ -371,28 +389,43 @@
     ExportComponentsResponseTypeDef,
     ExportFormsRequestExportFormsPaginateTypeDef,
     ExportFormsRequestRequestTypeDef,
     ExportFormsResponseTypeDef,
     ExportThemesRequestExportThemesPaginateTypeDef,
     ExportThemesRequestRequestTypeDef,
     ExportThemesResponseTypeDef,
+    FieldConfigOutputTypeDef,
     FieldConfigTypeDef,
+    FieldInputConfigOutputTypeDef,
     FieldInputConfigTypeDef,
+    FieldPositionOutputTypeDef,
     FieldPositionTypeDef,
+    FieldValidationConfigurationOutputTypeDef,
     FieldValidationConfigurationTypeDef,
+    FileUploaderFieldConfigOutputTypeDef,
     FileUploaderFieldConfigTypeDef,
+    FormBindingElementOutputTypeDef,
     FormBindingElementTypeDef,
+    FormButtonOutputTypeDef,
     FormButtonTypeDef,
+    FormCTAOutputTypeDef,
     FormCTATypeDef,
+    FormDataTypeConfigOutputTypeDef,
     FormDataTypeConfigTypeDef,
+    FormInputBindingPropertiesValueOutputTypeDef,
+    FormInputBindingPropertiesValuePropertiesOutputTypeDef,
     FormInputBindingPropertiesValuePropertiesTypeDef,
     FormInputBindingPropertiesValueTypeDef,
+    FormInputValuePropertyBindingPropertiesOutputTypeDef,
     FormInputValuePropertyBindingPropertiesTypeDef,
+    FormInputValuePropertyOutputTypeDef,
     FormInputValuePropertyTypeDef,
+    FormStyleConfigOutputTypeDef,
     FormStyleConfigTypeDef,
+    FormStyleOutputTypeDef,
     FormStyleTypeDef,
     FormSummaryTypeDef,
     FormTypeDef,
     GetCodegenJobRequestRequestTypeDef,
     GetCodegenJobResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetComponentResponseTypeDef,
@@ -410,48 +443,57 @@
     ListComponentsResponseTypeDef,
     ListFormsRequestListFormsPaginateTypeDef,
     ListFormsRequestRequestTypeDef,
     ListFormsResponseTypeDef,
     ListThemesRequestListThemesPaginateTypeDef,
     ListThemesRequestRequestTypeDef,
     ListThemesResponseTypeDef,
+    MutationActionSetStateParameterOutputTypeDef,
     MutationActionSetStateParameterTypeDef,
     PaginatorConfigTypeDef,
+    PredicateOutputTypeDef,
     PredicateTypeDef,
     PutMetadataFlagBodyTypeDef,
     PutMetadataFlagRequestRequestTypeDef,
+    ReactStartCodegenJobDataOutputTypeDef,
     ReactStartCodegenJobDataTypeDef,
     RefreshTokenRequestBodyTypeDef,
     RefreshTokenRequestRequestTypeDef,
     RefreshTokenResponseTypeDef,
     ResponseMetadataTypeDef,
+    SectionalElementOutputTypeDef,
     SectionalElementTypeDef,
+    SortPropertyOutputTypeDef,
     SortPropertyTypeDef,
     StartCodegenJobDataTypeDef,
     StartCodegenJobRequestRequestTypeDef,
     StartCodegenJobResponseTypeDef,
     ThemeSummaryTypeDef,
     ThemeTypeDef,
+    ThemeValueOutputTypeDef,
     ThemeValueTypeDef,
+    ThemeValuesOutputTypeDef,
     ThemeValuesTypeDef,
     UpdateComponentDataTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateComponentResponseTypeDef,
     UpdateFormDataTypeDef,
     UpdateFormRequestRequestTypeDef,
     UpdateFormResponseTypeDef,
     UpdateThemeDataTypeDef,
     UpdateThemeRequestRequestTypeDef,
     UpdateThemeResponseTypeDef,
+    ValueMappingOutputTypeDef,
     ValueMappingTypeDef,
+    ValueMappingsOutputTypeDef,
     ValueMappingsTypeDef,
 )
 
 
-def get_structure() -> ActionParametersTypeDef:
+def get_structure() -> ActionParametersOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/__init__.py` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/__init__.pyi` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/__main__.py` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AmplifyUIBuilder 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.AmplifyUIBuilder 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder\nOther"
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

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/client.py` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/client.pyi` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/literals.py` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/literals.pyi`

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
     "CodegenGenericDataFieldDataTypeType",
     "CodegenJobGenericDataSourceTypeType",
     "CodegenJobStatusType",
     "ExportComponentsPaginatorName",
     "ExportFormsPaginatorName",
     "ExportThemesPaginatorName",
@@ -45,15 +44,14 @@
     "AmplifyUIBuilderServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CodegenGenericDataFieldDataTypeType = Literal[
     "AWSDate",
     "AWSDateTime",
     "AWSEmail",
     "AWSIPAddress",
     "AWSJSON",
     "AWSPhone",
@@ -206,14 +204,15 @@
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
@@ -292,26 +291,28 @@
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

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/literals.pyi` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/literals.py`

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
     "CodegenGenericDataFieldDataTypeType",
     "CodegenJobGenericDataSourceTypeType",
     "CodegenJobStatusType",
     "ExportComponentsPaginatorName",
     "ExportFormsPaginatorName",
     "ExportThemesPaginatorName",
@@ -44,14 +45,15 @@
     "AmplifyUIBuilderServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 CodegenGenericDataFieldDataTypeType = Literal[
     "AWSDate",
     "AWSDateTime",
     "AWSEmail",
     "AWSIPAddress",
     "AWSJSON",
     "AWSPhone",
@@ -204,14 +206,15 @@
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
@@ -290,26 +293,28 @@
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

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/paginator.py` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/paginator.pyi` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/type_defs.py` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/type_defs.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplifyuibuilder service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplifyuibuilder.type_defs import ActionParametersTypeDef
+    from mypy_boto3_amplifyuibuilder.type_defs import ActionParametersOutputTypeDef
 
-    data: ActionParametersTypeDef = {...}
+    data: ActionParametersOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -37,36 +37,54 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ActionParametersOutputTypeDef",
     "ActionParametersTypeDef",
+    "CodegenFeatureFlagsOutputTypeDef",
     "CodegenFeatureFlagsTypeDef",
+    "CodegenGenericDataEnumOutputTypeDef",
     "CodegenGenericDataEnumTypeDef",
+    "CodegenGenericDataFieldOutputTypeDef",
     "CodegenGenericDataFieldTypeDef",
+    "CodegenGenericDataModelOutputTypeDef",
     "CodegenGenericDataModelTypeDef",
+    "CodegenGenericDataNonModelOutputTypeDef",
     "CodegenGenericDataNonModelTypeDef",
+    "CodegenGenericDataRelationshipTypeOutputTypeDef",
     "CodegenGenericDataRelationshipTypeTypeDef",
     "CodegenJobAssetTypeDef",
+    "CodegenJobGenericDataSchemaOutputTypeDef",
     "CodegenJobGenericDataSchemaTypeDef",
+    "CodegenJobRenderConfigOutputTypeDef",
     "CodegenJobRenderConfigTypeDef",
     "CodegenJobSummaryTypeDef",
     "CodegenJobTypeDef",
+    "ComponentBindingPropertiesValueOutputTypeDef",
+    "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     "ComponentBindingPropertiesValueTypeDef",
+    "ComponentChildOutputTypeDef",
     "ComponentChildTypeDef",
+    "ComponentConditionPropertyOutputTypeDef",
     "ComponentConditionPropertyTypeDef",
+    "ComponentDataConfigurationOutputTypeDef",
     "ComponentDataConfigurationTypeDef",
+    "ComponentEventOutputTypeDef",
     "ComponentEventTypeDef",
+    "ComponentPropertyBindingPropertiesOutputTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
+    "ComponentPropertyOutputTypeDef",
     "ComponentPropertyTypeDef",
     "ComponentSummaryTypeDef",
     "ComponentTypeDef",
+    "ComponentVariantOutputTypeDef",
     "ComponentVariantTypeDef",
     "CreateComponentDataTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "CreateComponentResponseTypeDef",
     "CreateFormDataTypeDef",
     "CreateFormRequestRequestTypeDef",
     "CreateFormResponseTypeDef",
@@ -85,28 +103,43 @@
     "ExportComponentsResponseTypeDef",
     "ExportFormsRequestExportFormsPaginateTypeDef",
     "ExportFormsRequestRequestTypeDef",
     "ExportFormsResponseTypeDef",
     "ExportThemesRequestExportThemesPaginateTypeDef",
     "ExportThemesRequestRequestTypeDef",
     "ExportThemesResponseTypeDef",
+    "FieldConfigOutputTypeDef",
     "FieldConfigTypeDef",
+    "FieldInputConfigOutputTypeDef",
     "FieldInputConfigTypeDef",
+    "FieldPositionOutputTypeDef",
     "FieldPositionTypeDef",
+    "FieldValidationConfigurationOutputTypeDef",
     "FieldValidationConfigurationTypeDef",
+    "FileUploaderFieldConfigOutputTypeDef",
     "FileUploaderFieldConfigTypeDef",
+    "FormBindingElementOutputTypeDef",
     "FormBindingElementTypeDef",
+    "FormButtonOutputTypeDef",
     "FormButtonTypeDef",
+    "FormCTAOutputTypeDef",
     "FormCTATypeDef",
+    "FormDataTypeConfigOutputTypeDef",
     "FormDataTypeConfigTypeDef",
+    "FormInputBindingPropertiesValueOutputTypeDef",
+    "FormInputBindingPropertiesValuePropertiesOutputTypeDef",
     "FormInputBindingPropertiesValuePropertiesTypeDef",
     "FormInputBindingPropertiesValueTypeDef",
+    "FormInputValuePropertyBindingPropertiesOutputTypeDef",
     "FormInputValuePropertyBindingPropertiesTypeDef",
+    "FormInputValuePropertyOutputTypeDef",
     "FormInputValuePropertyTypeDef",
+    "FormStyleConfigOutputTypeDef",
     "FormStyleConfigTypeDef",
+    "FormStyleOutputTypeDef",
     "FormStyleTypeDef",
     "FormSummaryTypeDef",
     "FormTypeDef",
     "GetCodegenJobRequestRequestTypeDef",
     "GetCodegenJobResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetComponentResponseTypeDef",
@@ -124,46 +157,71 @@
     "ListComponentsResponseTypeDef",
     "ListFormsRequestListFormsPaginateTypeDef",
     "ListFormsRequestRequestTypeDef",
     "ListFormsResponseTypeDef",
     "ListThemesRequestListThemesPaginateTypeDef",
     "ListThemesRequestRequestTypeDef",
     "ListThemesResponseTypeDef",
+    "MutationActionSetStateParameterOutputTypeDef",
     "MutationActionSetStateParameterTypeDef",
     "PaginatorConfigTypeDef",
+    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "PutMetadataFlagBodyTypeDef",
     "PutMetadataFlagRequestRequestTypeDef",
+    "ReactStartCodegenJobDataOutputTypeDef",
     "ReactStartCodegenJobDataTypeDef",
     "RefreshTokenRequestBodyTypeDef",
     "RefreshTokenRequestRequestTypeDef",
     "RefreshTokenResponseTypeDef",
     "ResponseMetadataTypeDef",
+    "SectionalElementOutputTypeDef",
     "SectionalElementTypeDef",
+    "SortPropertyOutputTypeDef",
     "SortPropertyTypeDef",
     "StartCodegenJobDataTypeDef",
     "StartCodegenJobRequestRequestTypeDef",
     "StartCodegenJobResponseTypeDef",
     "ThemeSummaryTypeDef",
     "ThemeTypeDef",
+    "ThemeValueOutputTypeDef",
     "ThemeValueTypeDef",
+    "ThemeValuesOutputTypeDef",
     "ThemeValuesTypeDef",
     "UpdateComponentDataTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateComponentResponseTypeDef",
     "UpdateFormDataTypeDef",
     "UpdateFormRequestRequestTypeDef",
     "UpdateFormResponseTypeDef",
     "UpdateThemeDataTypeDef",
     "UpdateThemeRequestRequestTypeDef",
     "UpdateThemeResponseTypeDef",
+    "ValueMappingOutputTypeDef",
     "ValueMappingTypeDef",
+    "ValueMappingsOutputTypeDef",
     "ValueMappingsTypeDef",
 )
 
+ActionParametersOutputTypeDef = TypedDict(
+    "ActionParametersOutputTypeDef",
+    {
+        "type": "ComponentPropertyOutputTypeDef",
+        "url": "ComponentPropertyOutputTypeDef",
+        "anchor": "ComponentPropertyOutputTypeDef",
+        "target": "ComponentPropertyOutputTypeDef",
+        "global": "ComponentPropertyOutputTypeDef",
+        "model": str,
+        "id": "ComponentPropertyOutputTypeDef",
+        "fields": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "state": "MutationActionSetStateParameterOutputTypeDef",
+    },
+    total=False,
+)
+
 ActionParametersTypeDef = TypedDict(
     "ActionParametersTypeDef",
     {
         "type": "ComponentPropertyTypeDef",
         "url": "ComponentPropertyTypeDef",
         "anchor": "ComponentPropertyTypeDef",
         "target": "ComponentPropertyTypeDef",
@@ -172,30 +230,71 @@
         "id": "ComponentPropertyTypeDef",
         "fields": Mapping[str, "ComponentPropertyTypeDef"],
         "state": "MutationActionSetStateParameterTypeDef",
     },
     total=False,
 )
 
+CodegenFeatureFlagsOutputTypeDef = TypedDict(
+    "CodegenFeatureFlagsOutputTypeDef",
+    {
+        "isRelationshipSupported": bool,
+        "isNonModelSupported": bool,
+    },
+    total=False,
+)
+
 CodegenFeatureFlagsTypeDef = TypedDict(
     "CodegenFeatureFlagsTypeDef",
     {
         "isRelationshipSupported": bool,
         "isNonModelSupported": bool,
     },
     total=False,
 )
 
+CodegenGenericDataEnumOutputTypeDef = TypedDict(
+    "CodegenGenericDataEnumOutputTypeDef",
+    {
+        "values": List[str],
+    },
+)
+
 CodegenGenericDataEnumTypeDef = TypedDict(
     "CodegenGenericDataEnumTypeDef",
     {
-        "values": List[str],
+        "values": Sequence[str],
     },
 )
 
+_RequiredCodegenGenericDataFieldOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataFieldOutputTypeDef",
+    {
+        "dataType": CodegenGenericDataFieldDataTypeType,
+        "dataTypeValue": str,
+        "required": bool,
+        "readOnly": bool,
+        "isArray": bool,
+    },
+)
+_OptionalCodegenGenericDataFieldOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataFieldOutputTypeDef",
+    {
+        "relationship": "CodegenGenericDataRelationshipTypeOutputTypeDef",
+    },
+    total=False,
+)
+
+
+class CodegenGenericDataFieldOutputTypeDef(
+    _RequiredCodegenGenericDataFieldOutputTypeDef, _OptionalCodegenGenericDataFieldOutputTypeDef
+):
+    pass
+
+
 _RequiredCodegenGenericDataFieldTypeDef = TypedDict(
     "_RequiredCodegenGenericDataFieldTypeDef",
     {
         "dataType": CodegenGenericDataFieldDataTypeType,
         "dataTypeValue": str,
         "required": bool,
         "readOnly": bool,
@@ -213,19 +312,41 @@
 
 class CodegenGenericDataFieldTypeDef(
     _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
 ):
     pass
 
 
+_RequiredCodegenGenericDataModelOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataModelOutputTypeDef",
+    {
+        "fields": Dict[str, "CodegenGenericDataFieldOutputTypeDef"],
+        "primaryKeys": List[str],
+    },
+)
+_OptionalCodegenGenericDataModelOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataModelOutputTypeDef",
+    {
+        "isJoinTable": bool,
+    },
+    total=False,
+)
+
+
+class CodegenGenericDataModelOutputTypeDef(
+    _RequiredCodegenGenericDataModelOutputTypeDef, _OptionalCodegenGenericDataModelOutputTypeDef
+):
+    pass
+
+
 _RequiredCodegenGenericDataModelTypeDef = TypedDict(
     "_RequiredCodegenGenericDataModelTypeDef",
     {
-        "fields": Dict[str, "CodegenGenericDataFieldTypeDef"],
-        "primaryKeys": List[str],
+        "fields": Mapping[str, "CodegenGenericDataFieldTypeDef"],
+        "primaryKeys": Sequence[str],
     },
 )
 _OptionalCodegenGenericDataModelTypeDef = TypedDict(
     "_OptionalCodegenGenericDataModelTypeDef",
     {
         "isJoinTable": bool,
     },
@@ -235,37 +356,73 @@
 
 class CodegenGenericDataModelTypeDef(
     _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
 ):
     pass
 
 
+CodegenGenericDataNonModelOutputTypeDef = TypedDict(
+    "CodegenGenericDataNonModelOutputTypeDef",
+    {
+        "fields": Dict[str, "CodegenGenericDataFieldOutputTypeDef"],
+    },
+)
+
 CodegenGenericDataNonModelTypeDef = TypedDict(
     "CodegenGenericDataNonModelTypeDef",
     {
-        "fields": Dict[str, "CodegenGenericDataFieldTypeDef"],
+        "fields": Mapping[str, "CodegenGenericDataFieldTypeDef"],
     },
 )
 
+_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef",
+    {
+        "type": GenericDataRelationshipTypeType,
+        "relatedModelName": str,
+    },
+)
+_OptionalCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataRelationshipTypeOutputTypeDef",
+    {
+        "relatedModelFields": List[str],
+        "canUnlinkAssociatedModel": bool,
+        "relatedJoinFieldName": str,
+        "relatedJoinTableName": str,
+        "belongsToFieldOnRelatedModel": str,
+        "associatedFields": List[str],
+        "isHasManyIndex": bool,
+    },
+    total=False,
+)
+
+
+class CodegenGenericDataRelationshipTypeOutputTypeDef(
+    _RequiredCodegenGenericDataRelationshipTypeOutputTypeDef,
+    _OptionalCodegenGenericDataRelationshipTypeOutputTypeDef,
+):
+    pass
+
+
 _RequiredCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
     "_RequiredCodegenGenericDataRelationshipTypeTypeDef",
     {
         "type": GenericDataRelationshipTypeType,
         "relatedModelName": str,
     },
 )
 _OptionalCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
     "_OptionalCodegenGenericDataRelationshipTypeTypeDef",
     {
-        "relatedModelFields": List[str],
+        "relatedModelFields": Sequence[str],
         "canUnlinkAssociatedModel": bool,
         "relatedJoinFieldName": str,
         "relatedJoinTableName": str,
         "belongsToFieldOnRelatedModel": str,
-        "associatedFields": List[str],
+        "associatedFields": Sequence[str],
         "isHasManyIndex": bool,
     },
     total=False,
 )
 
 
 class CodegenGenericDataRelationshipTypeTypeDef(
@@ -279,22 +436,40 @@
     "CodegenJobAssetTypeDef",
     {
         "downloadUrl": str,
     },
     total=False,
 )
 
+CodegenJobGenericDataSchemaOutputTypeDef = TypedDict(
+    "CodegenJobGenericDataSchemaOutputTypeDef",
+    {
+        "dataSourceType": Literal["DataStore"],
+        "models": Dict[str, "CodegenGenericDataModelOutputTypeDef"],
+        "enums": Dict[str, "CodegenGenericDataEnumOutputTypeDef"],
+        "nonModels": Dict[str, "CodegenGenericDataNonModelOutputTypeDef"],
+    },
+)
+
 CodegenJobGenericDataSchemaTypeDef = TypedDict(
     "CodegenJobGenericDataSchemaTypeDef",
     {
         "dataSourceType": Literal["DataStore"],
-        "models": Dict[str, "CodegenGenericDataModelTypeDef"],
-        "enums": Dict[str, "CodegenGenericDataEnumTypeDef"],
-        "nonModels": Dict[str, "CodegenGenericDataNonModelTypeDef"],
+        "models": Mapping[str, "CodegenGenericDataModelTypeDef"],
+        "enums": Mapping[str, "CodegenGenericDataEnumTypeDef"],
+        "nonModels": Mapping[str, "CodegenGenericDataNonModelTypeDef"],
+    },
+)
+
+CodegenJobRenderConfigOutputTypeDef = TypedDict(
+    "CodegenJobRenderConfigOutputTypeDef",
+    {
+        "react": "ReactStartCodegenJobDataOutputTypeDef",
     },
+    total=False,
 )
 
 CodegenJobRenderConfigTypeDef = TypedDict(
     "CodegenJobRenderConfigTypeDef",
     {
         "react": "ReactStartCodegenJobDataTypeDef",
     },
@@ -332,18 +507,18 @@
         "appId": str,
         "environmentName": str,
     },
 )
 _OptionalCodegenJobTypeDef = TypedDict(
     "_OptionalCodegenJobTypeDef",
     {
-        "renderConfig": "CodegenJobRenderConfigTypeDef",
-        "genericDataSchema": "CodegenJobGenericDataSchemaTypeDef",
+        "renderConfig": "CodegenJobRenderConfigOutputTypeDef",
+        "genericDataSchema": "CodegenJobGenericDataSchemaOutputTypeDef",
         "autoGenerateForms": bool,
-        "features": "CodegenFeatureFlagsTypeDef",
+        "features": "CodegenFeatureFlagsOutputTypeDef",
         "status": CodegenJobStatusType,
         "statusMessage": str,
         "asset": "CodegenJobAssetTypeDef",
         "tags": Dict[str, str],
         "createdAt": datetime,
         "modifiedAt": datetime,
     },
@@ -351,14 +526,39 @@
 )
 
 
 class CodegenJobTypeDef(_RequiredCodegenJobTypeDef, _OptionalCodegenJobTypeDef):
     pass
 
 
+ComponentBindingPropertiesValueOutputTypeDef = TypedDict(
+    "ComponentBindingPropertiesValueOutputTypeDef",
+    {
+        "type": str,
+        "bindingProperties": "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
+        "defaultValue": str,
+    },
+    total=False,
+)
+
+ComponentBindingPropertiesValuePropertiesOutputTypeDef = TypedDict(
+    "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
+    {
+        "model": str,
+        "field": str,
+        "predicates": List["PredicateOutputTypeDef"],
+        "userAttribute": str,
+        "bucket": str,
+        "key": str,
+        "defaultValue": str,
+        "slotName": str,
+    },
+    total=False,
+)
+
 ComponentBindingPropertiesValuePropertiesTypeDef = TypedDict(
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     {
         "model": str,
         "field": str,
         "predicates": Sequence["PredicateTypeDef"],
         "userAttribute": str,
@@ -376,14 +576,39 @@
         "type": str,
         "bindingProperties": "ComponentBindingPropertiesValuePropertiesTypeDef",
         "defaultValue": str,
     },
     total=False,
 )
 
+_RequiredComponentChildOutputTypeDef = TypedDict(
+    "_RequiredComponentChildOutputTypeDef",
+    {
+        "componentType": str,
+        "name": str,
+        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
+    },
+)
+_OptionalComponentChildOutputTypeDef = TypedDict(
+    "_OptionalComponentChildOutputTypeDef",
+    {
+        "children": List[Dict[str, Any]],
+        "events": Dict[str, "ComponentEventOutputTypeDef"],
+        "sourceId": str,
+    },
+    total=False,
+)
+
+
+class ComponentChildOutputTypeDef(
+    _RequiredComponentChildOutputTypeDef, _OptionalComponentChildOutputTypeDef
+):
+    pass
+
+
 _RequiredComponentChildTypeDef = TypedDict(
     "_RequiredComponentChildTypeDef",
     {
         "componentType": str,
         "name": str,
         "properties": Mapping[str, "ComponentPropertyTypeDef"],
     },
@@ -399,28 +624,66 @@
 )
 
 
 class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
     pass
 
 
+ComponentConditionPropertyOutputTypeDef = TypedDict(
+    "ComponentConditionPropertyOutputTypeDef",
+    {
+        "property": str,
+        "field": str,
+        "operator": str,
+        "operand": str,
+        "then": Dict[str, Any],
+        "else": Dict[str, Any],
+        "operandType": str,
+    },
+    total=False,
+)
+
 ComponentConditionPropertyTypeDef = TypedDict(
     "ComponentConditionPropertyTypeDef",
     {
         "property": str,
         "field": str,
         "operator": str,
         "operand": str,
         "then": Dict[str, Any],
         "else": Dict[str, Any],
         "operandType": str,
     },
     total=False,
 )
 
+_RequiredComponentDataConfigurationOutputTypeDef = TypedDict(
+    "_RequiredComponentDataConfigurationOutputTypeDef",
+    {
+        "model": str,
+    },
+)
+_OptionalComponentDataConfigurationOutputTypeDef = TypedDict(
+    "_OptionalComponentDataConfigurationOutputTypeDef",
+    {
+        "sort": List["SortPropertyOutputTypeDef"],
+        "predicate": "PredicateOutputTypeDef",
+        "identifiers": List[str],
+    },
+    total=False,
+)
+
+
+class ComponentDataConfigurationOutputTypeDef(
+    _RequiredComponentDataConfigurationOutputTypeDef,
+    _OptionalComponentDataConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredComponentDataConfigurationTypeDef = TypedDict(
     "_RequiredComponentDataConfigurationTypeDef",
     {
         "model": str,
     },
 )
 _OptionalComponentDataConfigurationTypeDef = TypedDict(
@@ -436,24 +699,56 @@
 
 class ComponentDataConfigurationTypeDef(
     _RequiredComponentDataConfigurationTypeDef, _OptionalComponentDataConfigurationTypeDef
 ):
     pass
 
 
+ComponentEventOutputTypeDef = TypedDict(
+    "ComponentEventOutputTypeDef",
+    {
+        "action": str,
+        "parameters": "ActionParametersOutputTypeDef",
+        "bindingEvent": str,
+    },
+    total=False,
+)
+
 ComponentEventTypeDef = TypedDict(
     "ComponentEventTypeDef",
     {
         "action": str,
         "parameters": "ActionParametersTypeDef",
         "bindingEvent": str,
     },
     total=False,
 )
 
+_RequiredComponentPropertyBindingPropertiesOutputTypeDef = TypedDict(
+    "_RequiredComponentPropertyBindingPropertiesOutputTypeDef",
+    {
+        "property": str,
+    },
+)
+_OptionalComponentPropertyBindingPropertiesOutputTypeDef = TypedDict(
+    "_OptionalComponentPropertyBindingPropertiesOutputTypeDef",
+    {
+        "field": str,
+    },
+    total=False,
+)
+
+
+class ComponentPropertyBindingPropertiesOutputTypeDef(
+    _RequiredComponentPropertyBindingPropertiesOutputTypeDef,
+    _OptionalComponentPropertyBindingPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredComponentPropertyBindingPropertiesTypeDef = TypedDict(
     "_RequiredComponentPropertyBindingPropertiesTypeDef",
     {
         "property": str,
     },
 )
 _OptionalComponentPropertyBindingPropertiesTypeDef = TypedDict(
@@ -468,14 +763,36 @@
 class ComponentPropertyBindingPropertiesTypeDef(
     _RequiredComponentPropertyBindingPropertiesTypeDef,
     _OptionalComponentPropertyBindingPropertiesTypeDef,
 ):
     pass
 
 
+ComponentPropertyOutputTypeDef = TypedDict(
+    "ComponentPropertyOutputTypeDef",
+    {
+        "value": str,
+        "bindingProperties": "ComponentPropertyBindingPropertiesOutputTypeDef",
+        "collectionBindingProperties": "ComponentPropertyBindingPropertiesOutputTypeDef",
+        "defaultValue": str,
+        "model": str,
+        "bindings": Dict[str, "FormBindingElementOutputTypeDef"],
+        "event": str,
+        "userAttribute": str,
+        "concat": List[Dict[str, Any]],
+        "condition": Dict[str, Any],
+        "configured": bool,
+        "type": str,
+        "importedValue": str,
+        "componentName": str,
+        "property": str,
+    },
+    total=False,
+)
+
 ComponentPropertyTypeDef = TypedDict(
     "ComponentPropertyTypeDef",
     {
         "value": str,
         "bindingProperties": "ComponentPropertyBindingPropertiesTypeDef",
         "collectionBindingProperties": "ComponentPropertyBindingPropertiesTypeDef",
         "defaultValue": str,
@@ -509,40 +826,49 @@
     "_RequiredComponentTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "componentType": str,
-        "properties": Dict[str, "ComponentPropertyTypeDef"],
-        "variants": List["ComponentVariantTypeDef"],
+        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "variants": List["ComponentVariantOutputTypeDef"],
         "overrides": Dict[str, Dict[str, str]],
-        "bindingProperties": Dict[str, "ComponentBindingPropertiesValueTypeDef"],
+        "bindingProperties": Dict[str, "ComponentBindingPropertiesValueOutputTypeDef"],
         "createdAt": datetime,
     },
 )
 _OptionalComponentTypeDef = TypedDict(
     "_OptionalComponentTypeDef",
     {
         "sourceId": str,
-        "children": List["ComponentChildTypeDef"],
-        "collectionProperties": Dict[str, "ComponentDataConfigurationTypeDef"],
+        "children": List["ComponentChildOutputTypeDef"],
+        "collectionProperties": Dict[str, "ComponentDataConfigurationOutputTypeDef"],
         "modifiedAt": datetime,
         "tags": Dict[str, str],
-        "events": Dict[str, "ComponentEventTypeDef"],
+        "events": Dict[str, "ComponentEventOutputTypeDef"],
         "schemaVersion": str,
     },
     total=False,
 )
 
 
 class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
     pass
 
 
+ComponentVariantOutputTypeDef = TypedDict(
+    "ComponentVariantOutputTypeDef",
+    {
+        "variantValues": Dict[str, str],
+        "overrides": Dict[str, Dict[str, str]],
+    },
+    total=False,
+)
+
 ComponentVariantTypeDef = TypedDict(
     "ComponentVariantTypeDef",
     {
         "variantValues": Mapping[str, str],
         "overrides": Mapping[str, Mapping[str, str]],
     },
     total=False,
@@ -952,26 +1278,73 @@
     {
         "entities": List["ThemeTypeDef"],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FieldConfigOutputTypeDef = TypedDict(
+    "FieldConfigOutputTypeDef",
+    {
+        "label": str,
+        "position": "FieldPositionOutputTypeDef",
+        "excluded": bool,
+        "inputType": "FieldInputConfigOutputTypeDef",
+        "validations": List["FieldValidationConfigurationOutputTypeDef"],
+    },
+    total=False,
+)
+
 FieldConfigTypeDef = TypedDict(
     "FieldConfigTypeDef",
     {
         "label": str,
         "position": "FieldPositionTypeDef",
         "excluded": bool,
         "inputType": "FieldInputConfigTypeDef",
         "validations": Sequence["FieldValidationConfigurationTypeDef"],
     },
     total=False,
 )
 
+_RequiredFieldInputConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldInputConfigOutputTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalFieldInputConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldInputConfigOutputTypeDef",
+    {
+        "required": bool,
+        "readOnly": bool,
+        "placeholder": str,
+        "defaultValue": str,
+        "descriptiveText": str,
+        "defaultChecked": bool,
+        "defaultCountryCode": str,
+        "valueMappings": "ValueMappingsOutputTypeDef",
+        "name": str,
+        "minValue": float,
+        "maxValue": float,
+        "step": float,
+        "value": str,
+        "isArray": bool,
+        "fileUploaderConfig": "FileUploaderFieldConfigOutputTypeDef",
+    },
+    total=False,
+)
+
+
+class FieldInputConfigOutputTypeDef(
+    _RequiredFieldInputConfigOutputTypeDef, _OptionalFieldInputConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredFieldInputConfigTypeDef = TypedDict(
     "_RequiredFieldInputConfigTypeDef",
     {
         "type": str,
     },
 )
 _OptionalFieldInputConfigTypeDef = TypedDict(
@@ -997,24 +1370,58 @@
 )
 
 
 class FieldInputConfigTypeDef(_RequiredFieldInputConfigTypeDef, _OptionalFieldInputConfigTypeDef):
     pass
 
 
+FieldPositionOutputTypeDef = TypedDict(
+    "FieldPositionOutputTypeDef",
+    {
+        "fixed": Literal["first"],
+        "rightOf": str,
+        "below": str,
+    },
+    total=False,
+)
+
 FieldPositionTypeDef = TypedDict(
     "FieldPositionTypeDef",
     {
         "fixed": Literal["first"],
         "rightOf": str,
         "below": str,
     },
     total=False,
 )
 
+_RequiredFieldValidationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFieldValidationConfigurationOutputTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalFieldValidationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFieldValidationConfigurationOutputTypeDef",
+    {
+        "strValues": List[str],
+        "numValues": List[int],
+        "validationMessage": str,
+    },
+    total=False,
+)
+
+
+class FieldValidationConfigurationOutputTypeDef(
+    _RequiredFieldValidationConfigurationOutputTypeDef,
+    _OptionalFieldValidationConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredFieldValidationConfigurationTypeDef = TypedDict(
     "_RequiredFieldValidationConfigurationTypeDef",
     {
         "type": str,
     },
 )
 _OptionalFieldValidationConfigurationTypeDef = TypedDict(
@@ -1030,14 +1437,39 @@
 
 class FieldValidationConfigurationTypeDef(
     _RequiredFieldValidationConfigurationTypeDef, _OptionalFieldValidationConfigurationTypeDef
 ):
     pass
 
 
+_RequiredFileUploaderFieldConfigOutputTypeDef = TypedDict(
+    "_RequiredFileUploaderFieldConfigOutputTypeDef",
+    {
+        "accessLevel": StorageAccessLevelType,
+        "acceptedFileTypes": List[str],
+    },
+)
+_OptionalFileUploaderFieldConfigOutputTypeDef = TypedDict(
+    "_OptionalFileUploaderFieldConfigOutputTypeDef",
+    {
+        "showThumbnails": bool,
+        "isResumable": bool,
+        "maxFileCount": int,
+        "maxSize": int,
+    },
+    total=False,
+)
+
+
+class FileUploaderFieldConfigOutputTypeDef(
+    _RequiredFileUploaderFieldConfigOutputTypeDef, _OptionalFileUploaderFieldConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredFileUploaderFieldConfigTypeDef = TypedDict(
     "_RequiredFileUploaderFieldConfigTypeDef",
     {
         "accessLevel": StorageAccessLevelType,
         "acceptedFileTypes": Sequence[str],
     },
 )
@@ -1055,51 +1487,105 @@
 
 class FileUploaderFieldConfigTypeDef(
     _RequiredFileUploaderFieldConfigTypeDef, _OptionalFileUploaderFieldConfigTypeDef
 ):
     pass
 
 
+FormBindingElementOutputTypeDef = TypedDict(
+    "FormBindingElementOutputTypeDef",
+    {
+        "element": str,
+        "property": str,
+    },
+)
+
 FormBindingElementTypeDef = TypedDict(
     "FormBindingElementTypeDef",
     {
         "element": str,
         "property": str,
     },
 )
 
+FormButtonOutputTypeDef = TypedDict(
+    "FormButtonOutputTypeDef",
+    {
+        "excluded": bool,
+        "children": str,
+        "position": "FieldPositionOutputTypeDef",
+    },
+    total=False,
+)
+
 FormButtonTypeDef = TypedDict(
     "FormButtonTypeDef",
     {
         "excluded": bool,
         "children": str,
         "position": "FieldPositionTypeDef",
     },
     total=False,
 )
 
+FormCTAOutputTypeDef = TypedDict(
+    "FormCTAOutputTypeDef",
+    {
+        "position": FormButtonsPositionType,
+        "clear": "FormButtonOutputTypeDef",
+        "cancel": "FormButtonOutputTypeDef",
+        "submit": "FormButtonOutputTypeDef",
+    },
+    total=False,
+)
+
 FormCTATypeDef = TypedDict(
     "FormCTATypeDef",
     {
         "position": FormButtonsPositionType,
         "clear": "FormButtonTypeDef",
         "cancel": "FormButtonTypeDef",
         "submit": "FormButtonTypeDef",
     },
     total=False,
 )
 
+FormDataTypeConfigOutputTypeDef = TypedDict(
+    "FormDataTypeConfigOutputTypeDef",
+    {
+        "dataSourceType": FormDataSourceTypeType,
+        "dataTypeName": str,
+    },
+)
+
 FormDataTypeConfigTypeDef = TypedDict(
     "FormDataTypeConfigTypeDef",
     {
         "dataSourceType": FormDataSourceTypeType,
         "dataTypeName": str,
     },
 )
 
+FormInputBindingPropertiesValueOutputTypeDef = TypedDict(
+    "FormInputBindingPropertiesValueOutputTypeDef",
+    {
+        "type": str,
+        "bindingProperties": "FormInputBindingPropertiesValuePropertiesOutputTypeDef",
+    },
+    total=False,
+)
+
+FormInputBindingPropertiesValuePropertiesOutputTypeDef = TypedDict(
+    "FormInputBindingPropertiesValuePropertiesOutputTypeDef",
+    {
+        "model": str,
+    },
+    total=False,
+)
+
 FormInputBindingPropertiesValuePropertiesTypeDef = TypedDict(
     "FormInputBindingPropertiesValuePropertiesTypeDef",
     {
         "model": str,
     },
     total=False,
 )
@@ -1109,14 +1595,36 @@
     {
         "type": str,
         "bindingProperties": "FormInputBindingPropertiesValuePropertiesTypeDef",
     },
     total=False,
 )
 
+_RequiredFormInputValuePropertyBindingPropertiesOutputTypeDef = TypedDict(
+    "_RequiredFormInputValuePropertyBindingPropertiesOutputTypeDef",
+    {
+        "property": str,
+    },
+)
+_OptionalFormInputValuePropertyBindingPropertiesOutputTypeDef = TypedDict(
+    "_OptionalFormInputValuePropertyBindingPropertiesOutputTypeDef",
+    {
+        "field": str,
+    },
+    total=False,
+)
+
+
+class FormInputValuePropertyBindingPropertiesOutputTypeDef(
+    _RequiredFormInputValuePropertyBindingPropertiesOutputTypeDef,
+    _OptionalFormInputValuePropertyBindingPropertiesOutputTypeDef,
+):
+    pass
+
+
 _RequiredFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
     "_RequiredFormInputValuePropertyBindingPropertiesTypeDef",
     {
         "property": str,
     },
 )
 _OptionalFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
@@ -1131,48 +1639,77 @@
 class FormInputValuePropertyBindingPropertiesTypeDef(
     _RequiredFormInputValuePropertyBindingPropertiesTypeDef,
     _OptionalFormInputValuePropertyBindingPropertiesTypeDef,
 ):
     pass
 
 
+FormInputValuePropertyOutputTypeDef = TypedDict(
+    "FormInputValuePropertyOutputTypeDef",
+    {
+        "value": str,
+        "bindingProperties": "FormInputValuePropertyBindingPropertiesOutputTypeDef",
+        "concat": List[Dict[str, Any]],
+    },
+    total=False,
+)
+
 FormInputValuePropertyTypeDef = TypedDict(
     "FormInputValuePropertyTypeDef",
     {
         "value": str,
         "bindingProperties": "FormInputValuePropertyBindingPropertiesTypeDef",
         "concat": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+FormStyleConfigOutputTypeDef = TypedDict(
+    "FormStyleConfigOutputTypeDef",
+    {
+        "tokenReference": str,
+        "value": str,
+    },
+    total=False,
+)
+
 FormStyleConfigTypeDef = TypedDict(
     "FormStyleConfigTypeDef",
     {
         "tokenReference": str,
         "value": str,
     },
     total=False,
 )
 
+FormStyleOutputTypeDef = TypedDict(
+    "FormStyleOutputTypeDef",
+    {
+        "horizontalGap": "FormStyleConfigOutputTypeDef",
+        "verticalGap": "FormStyleConfigOutputTypeDef",
+        "outerPadding": "FormStyleConfigOutputTypeDef",
+    },
+    total=False,
+)
+
 FormStyleTypeDef = TypedDict(
     "FormStyleTypeDef",
     {
         "horizontalGap": "FormStyleConfigTypeDef",
         "verticalGap": "FormStyleConfigTypeDef",
         "outerPadding": "FormStyleConfigTypeDef",
     },
     total=False,
 )
 
 FormSummaryTypeDef = TypedDict(
     "FormSummaryTypeDef",
     {
         "appId": str,
-        "dataType": "FormDataTypeConfigTypeDef",
+        "dataType": "FormDataTypeConfigOutputTypeDef",
         "environmentName": str,
         "formActionType": FormActionTypeType,
         "id": str,
         "name": str,
     },
 )
 
@@ -1180,26 +1717,26 @@
     "_RequiredFormTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "formActionType": FormActionTypeType,
-        "style": "FormStyleTypeDef",
-        "dataType": "FormDataTypeConfigTypeDef",
-        "fields": Dict[str, "FieldConfigTypeDef"],
-        "sectionalElements": Dict[str, "SectionalElementTypeDef"],
+        "style": "FormStyleOutputTypeDef",
+        "dataType": "FormDataTypeConfigOutputTypeDef",
+        "fields": Dict[str, "FieldConfigOutputTypeDef"],
+        "sectionalElements": Dict[str, "SectionalElementOutputTypeDef"],
         "schemaVersion": str,
     },
 )
 _OptionalFormTypeDef = TypedDict(
     "_OptionalFormTypeDef",
     {
         "tags": Dict[str, str],
-        "cta": "FormCTATypeDef",
+        "cta": "FormCTAOutputTypeDef",
         "labelDecorator": LabelDecoratorType,
     },
     total=False,
 )
 
 
 class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
@@ -1506,14 +2043,23 @@
     {
         "entities": List["ThemeSummaryTypeDef"],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MutationActionSetStateParameterOutputTypeDef = TypedDict(
+    "MutationActionSetStateParameterOutputTypeDef",
+    {
+        "componentName": str,
+        "property": str,
+        "set": "ComponentPropertyOutputTypeDef",
+    },
+)
+
 MutationActionSetStateParameterTypeDef = TypedDict(
     "MutationActionSetStateParameterTypeDef",
     {
         "componentName": str,
         "property": str,
         "set": "ComponentPropertyTypeDef",
     },
@@ -1525,14 +2071,27 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PredicateOutputTypeDef = TypedDict(
+    "PredicateOutputTypeDef",
+    {
+        "or": List[Dict[str, Any]],
+        "and": List[Dict[str, Any]],
+        "field": str,
+        "operator": str,
+        "operand": str,
+        "operandType": str,
+    },
+    total=False,
+)
+
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "or": Sequence[Dict[str, Any]],
         "and": Sequence[Dict[str, Any]],
         "field": str,
         "operator": str,
@@ -1555,14 +2114,26 @@
         "appId": str,
         "environmentName": str,
         "featureName": str,
         "body": "PutMetadataFlagBodyTypeDef",
     },
 )
 
+ReactStartCodegenJobDataOutputTypeDef = TypedDict(
+    "ReactStartCodegenJobDataOutputTypeDef",
+    {
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
+    },
+    total=False,
+)
+
 ReactStartCodegenJobDataTypeDef = TypedDict(
     "ReactStartCodegenJobDataTypeDef",
     {
         "module": JSModuleType,
         "target": JSTargetType,
         "script": JSScriptType,
         "renderTypeDeclarations": bool,
@@ -1616,14 +2187,39 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredSectionalElementOutputTypeDef = TypedDict(
+    "_RequiredSectionalElementOutputTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalSectionalElementOutputTypeDef = TypedDict(
+    "_OptionalSectionalElementOutputTypeDef",
+    {
+        "position": "FieldPositionOutputTypeDef",
+        "text": str,
+        "level": int,
+        "orientation": str,
+        "excluded": bool,
+    },
+    total=False,
+)
+
+
+class SectionalElementOutputTypeDef(
+    _RequiredSectionalElementOutputTypeDef, _OptionalSectionalElementOutputTypeDef
+):
+    pass
+
+
 _RequiredSectionalElementTypeDef = TypedDict(
     "_RequiredSectionalElementTypeDef",
     {
         "type": str,
     },
 )
 _OptionalSectionalElementTypeDef = TypedDict(
@@ -1639,14 +2235,22 @@
 )
 
 
 class SectionalElementTypeDef(_RequiredSectionalElementTypeDef, _OptionalSectionalElementTypeDef):
     pass
 
 
+SortPropertyOutputTypeDef = TypedDict(
+    "SortPropertyOutputTypeDef",
+    {
+        "field": str,
+        "direction": SortDirectionType,
+    },
+)
+
 SortPropertyTypeDef = TypedDict(
     "SortPropertyTypeDef",
     {
         "field": str,
         "direction": SortDirectionType,
     },
 )
@@ -1720,41 +2324,59 @@
     "_RequiredThemeTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "createdAt": datetime,
-        "values": List["ThemeValuesTypeDef"],
+        "values": List["ThemeValuesOutputTypeDef"],
     },
 )
 _OptionalThemeTypeDef = TypedDict(
     "_OptionalThemeTypeDef",
     {
         "modifiedAt": datetime,
-        "overrides": List["ThemeValuesTypeDef"],
+        "overrides": List["ThemeValuesOutputTypeDef"],
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
 class ThemeTypeDef(_RequiredThemeTypeDef, _OptionalThemeTypeDef):
     pass
 
 
+ThemeValueOutputTypeDef = TypedDict(
+    "ThemeValueOutputTypeDef",
+    {
+        "value": str,
+        "children": List[Dict[str, Any]],
+    },
+    total=False,
+)
+
 ThemeValueTypeDef = TypedDict(
     "ThemeValueTypeDef",
     {
         "value": str,
         "children": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+ThemeValuesOutputTypeDef = TypedDict(
+    "ThemeValuesOutputTypeDef",
+    {
+        "key": str,
+        "value": Dict[str, Any],
+    },
+    total=False,
+)
+
 ThemeValuesTypeDef = TypedDict(
     "ThemeValuesTypeDef",
     {
         "key": str,
         "value": Dict[str, Any],
     },
     total=False,
@@ -1908,14 +2530,35 @@
     "UpdateThemeResponseTypeDef",
     {
         "entity": "ThemeTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredValueMappingOutputTypeDef = TypedDict(
+    "_RequiredValueMappingOutputTypeDef",
+    {
+        "value": "FormInputValuePropertyOutputTypeDef",
+    },
+)
+_OptionalValueMappingOutputTypeDef = TypedDict(
+    "_OptionalValueMappingOutputTypeDef",
+    {
+        "displayValue": "FormInputValuePropertyOutputTypeDef",
+    },
+    total=False,
+)
+
+
+class ValueMappingOutputTypeDef(
+    _RequiredValueMappingOutputTypeDef, _OptionalValueMappingOutputTypeDef
+):
+    pass
+
+
 _RequiredValueMappingTypeDef = TypedDict(
     "_RequiredValueMappingTypeDef",
     {
         "value": "FormInputValuePropertyTypeDef",
     },
 )
 _OptionalValueMappingTypeDef = TypedDict(
@@ -1927,14 +2570,35 @@
 )
 
 
 class ValueMappingTypeDef(_RequiredValueMappingTypeDef, _OptionalValueMappingTypeDef):
     pass
 
 
+_RequiredValueMappingsOutputTypeDef = TypedDict(
+    "_RequiredValueMappingsOutputTypeDef",
+    {
+        "values": List["ValueMappingOutputTypeDef"],
+    },
+)
+_OptionalValueMappingsOutputTypeDef = TypedDict(
+    "_OptionalValueMappingsOutputTypeDef",
+    {
+        "bindingProperties": Dict[str, "FormInputBindingPropertiesValueOutputTypeDef"],
+    },
+    total=False,
+)
+
+
+class ValueMappingsOutputTypeDef(
+    _RequiredValueMappingsOutputTypeDef, _OptionalValueMappingsOutputTypeDef
+):
+    pass
+
+
 _RequiredValueMappingsTypeDef = TypedDict(
     "_RequiredValueMappingsTypeDef",
     {
         "values": Sequence["ValueMappingTypeDef"],
     },
 )
 _OptionalValueMappingsTypeDef = TypedDict(
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder/type_defs.pyi` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplifyuibuilder service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplifyuibuilder.type_defs import ActionParametersTypeDef
+    from mypy_boto3_amplifyuibuilder.type_defs import ActionParametersOutputTypeDef
 
-    data: ActionParametersTypeDef = {...}
+    data: ActionParametersOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -36,36 +36,54 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ActionParametersOutputTypeDef",
     "ActionParametersTypeDef",
+    "CodegenFeatureFlagsOutputTypeDef",
     "CodegenFeatureFlagsTypeDef",
+    "CodegenGenericDataEnumOutputTypeDef",
     "CodegenGenericDataEnumTypeDef",
+    "CodegenGenericDataFieldOutputTypeDef",
     "CodegenGenericDataFieldTypeDef",
+    "CodegenGenericDataModelOutputTypeDef",
     "CodegenGenericDataModelTypeDef",
+    "CodegenGenericDataNonModelOutputTypeDef",
     "CodegenGenericDataNonModelTypeDef",
+    "CodegenGenericDataRelationshipTypeOutputTypeDef",
     "CodegenGenericDataRelationshipTypeTypeDef",
     "CodegenJobAssetTypeDef",
+    "CodegenJobGenericDataSchemaOutputTypeDef",
     "CodegenJobGenericDataSchemaTypeDef",
+    "CodegenJobRenderConfigOutputTypeDef",
     "CodegenJobRenderConfigTypeDef",
     "CodegenJobSummaryTypeDef",
     "CodegenJobTypeDef",
+    "ComponentBindingPropertiesValueOutputTypeDef",
+    "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     "ComponentBindingPropertiesValueTypeDef",
+    "ComponentChildOutputTypeDef",
     "ComponentChildTypeDef",
+    "ComponentConditionPropertyOutputTypeDef",
     "ComponentConditionPropertyTypeDef",
+    "ComponentDataConfigurationOutputTypeDef",
     "ComponentDataConfigurationTypeDef",
+    "ComponentEventOutputTypeDef",
     "ComponentEventTypeDef",
+    "ComponentPropertyBindingPropertiesOutputTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
+    "ComponentPropertyOutputTypeDef",
     "ComponentPropertyTypeDef",
     "ComponentSummaryTypeDef",
     "ComponentTypeDef",
+    "ComponentVariantOutputTypeDef",
     "ComponentVariantTypeDef",
     "CreateComponentDataTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "CreateComponentResponseTypeDef",
     "CreateFormDataTypeDef",
     "CreateFormRequestRequestTypeDef",
     "CreateFormResponseTypeDef",
@@ -84,28 +102,43 @@
     "ExportComponentsResponseTypeDef",
     "ExportFormsRequestExportFormsPaginateTypeDef",
     "ExportFormsRequestRequestTypeDef",
     "ExportFormsResponseTypeDef",
     "ExportThemesRequestExportThemesPaginateTypeDef",
     "ExportThemesRequestRequestTypeDef",
     "ExportThemesResponseTypeDef",
+    "FieldConfigOutputTypeDef",
     "FieldConfigTypeDef",
+    "FieldInputConfigOutputTypeDef",
     "FieldInputConfigTypeDef",
+    "FieldPositionOutputTypeDef",
     "FieldPositionTypeDef",
+    "FieldValidationConfigurationOutputTypeDef",
     "FieldValidationConfigurationTypeDef",
+    "FileUploaderFieldConfigOutputTypeDef",
     "FileUploaderFieldConfigTypeDef",
+    "FormBindingElementOutputTypeDef",
     "FormBindingElementTypeDef",
+    "FormButtonOutputTypeDef",
     "FormButtonTypeDef",
+    "FormCTAOutputTypeDef",
     "FormCTATypeDef",
+    "FormDataTypeConfigOutputTypeDef",
     "FormDataTypeConfigTypeDef",
+    "FormInputBindingPropertiesValueOutputTypeDef",
+    "FormInputBindingPropertiesValuePropertiesOutputTypeDef",
     "FormInputBindingPropertiesValuePropertiesTypeDef",
     "FormInputBindingPropertiesValueTypeDef",
+    "FormInputValuePropertyBindingPropertiesOutputTypeDef",
     "FormInputValuePropertyBindingPropertiesTypeDef",
+    "FormInputValuePropertyOutputTypeDef",
     "FormInputValuePropertyTypeDef",
+    "FormStyleConfigOutputTypeDef",
     "FormStyleConfigTypeDef",
+    "FormStyleOutputTypeDef",
     "FormStyleTypeDef",
     "FormSummaryTypeDef",
     "FormTypeDef",
     "GetCodegenJobRequestRequestTypeDef",
     "GetCodegenJobResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetComponentResponseTypeDef",
@@ -123,46 +156,71 @@
     "ListComponentsResponseTypeDef",
     "ListFormsRequestListFormsPaginateTypeDef",
     "ListFormsRequestRequestTypeDef",
     "ListFormsResponseTypeDef",
     "ListThemesRequestListThemesPaginateTypeDef",
     "ListThemesRequestRequestTypeDef",
     "ListThemesResponseTypeDef",
+    "MutationActionSetStateParameterOutputTypeDef",
     "MutationActionSetStateParameterTypeDef",
     "PaginatorConfigTypeDef",
+    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "PutMetadataFlagBodyTypeDef",
     "PutMetadataFlagRequestRequestTypeDef",
+    "ReactStartCodegenJobDataOutputTypeDef",
     "ReactStartCodegenJobDataTypeDef",
     "RefreshTokenRequestBodyTypeDef",
     "RefreshTokenRequestRequestTypeDef",
     "RefreshTokenResponseTypeDef",
     "ResponseMetadataTypeDef",
+    "SectionalElementOutputTypeDef",
     "SectionalElementTypeDef",
+    "SortPropertyOutputTypeDef",
     "SortPropertyTypeDef",
     "StartCodegenJobDataTypeDef",
     "StartCodegenJobRequestRequestTypeDef",
     "StartCodegenJobResponseTypeDef",
     "ThemeSummaryTypeDef",
     "ThemeTypeDef",
+    "ThemeValueOutputTypeDef",
     "ThemeValueTypeDef",
+    "ThemeValuesOutputTypeDef",
     "ThemeValuesTypeDef",
     "UpdateComponentDataTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateComponentResponseTypeDef",
     "UpdateFormDataTypeDef",
     "UpdateFormRequestRequestTypeDef",
     "UpdateFormResponseTypeDef",
     "UpdateThemeDataTypeDef",
     "UpdateThemeRequestRequestTypeDef",
     "UpdateThemeResponseTypeDef",
+    "ValueMappingOutputTypeDef",
     "ValueMappingTypeDef",
+    "ValueMappingsOutputTypeDef",
     "ValueMappingsTypeDef",
 )
 
+ActionParametersOutputTypeDef = TypedDict(
+    "ActionParametersOutputTypeDef",
+    {
+        "type": "ComponentPropertyOutputTypeDef",
+        "url": "ComponentPropertyOutputTypeDef",
+        "anchor": "ComponentPropertyOutputTypeDef",
+        "target": "ComponentPropertyOutputTypeDef",
+        "global": "ComponentPropertyOutputTypeDef",
+        "model": str,
+        "id": "ComponentPropertyOutputTypeDef",
+        "fields": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "state": "MutationActionSetStateParameterOutputTypeDef",
+    },
+    total=False,
+)
+
 ActionParametersTypeDef = TypedDict(
     "ActionParametersTypeDef",
     {
         "type": "ComponentPropertyTypeDef",
         "url": "ComponentPropertyTypeDef",
         "anchor": "ComponentPropertyTypeDef",
         "target": "ComponentPropertyTypeDef",
@@ -171,29 +229,68 @@
         "id": "ComponentPropertyTypeDef",
         "fields": Mapping[str, "ComponentPropertyTypeDef"],
         "state": "MutationActionSetStateParameterTypeDef",
     },
     total=False,
 )
 
+CodegenFeatureFlagsOutputTypeDef = TypedDict(
+    "CodegenFeatureFlagsOutputTypeDef",
+    {
+        "isRelationshipSupported": bool,
+        "isNonModelSupported": bool,
+    },
+    total=False,
+)
+
 CodegenFeatureFlagsTypeDef = TypedDict(
     "CodegenFeatureFlagsTypeDef",
     {
         "isRelationshipSupported": bool,
         "isNonModelSupported": bool,
     },
     total=False,
 )
 
+CodegenGenericDataEnumOutputTypeDef = TypedDict(
+    "CodegenGenericDataEnumOutputTypeDef",
+    {
+        "values": List[str],
+    },
+)
+
 CodegenGenericDataEnumTypeDef = TypedDict(
     "CodegenGenericDataEnumTypeDef",
     {
-        "values": List[str],
+        "values": Sequence[str],
+    },
+)
+
+_RequiredCodegenGenericDataFieldOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataFieldOutputTypeDef",
+    {
+        "dataType": CodegenGenericDataFieldDataTypeType,
+        "dataTypeValue": str,
+        "required": bool,
+        "readOnly": bool,
+        "isArray": bool,
     },
 )
+_OptionalCodegenGenericDataFieldOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataFieldOutputTypeDef",
+    {
+        "relationship": "CodegenGenericDataRelationshipTypeOutputTypeDef",
+    },
+    total=False,
+)
+
+class CodegenGenericDataFieldOutputTypeDef(
+    _RequiredCodegenGenericDataFieldOutputTypeDef, _OptionalCodegenGenericDataFieldOutputTypeDef
+):
+    pass
 
 _RequiredCodegenGenericDataFieldTypeDef = TypedDict(
     "_RequiredCodegenGenericDataFieldTypeDef",
     {
         "dataType": CodegenGenericDataFieldDataTypeType,
         "dataTypeValue": str,
         "required": bool,
@@ -210,19 +307,39 @@
 )
 
 class CodegenGenericDataFieldTypeDef(
     _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
 ):
     pass
 
+_RequiredCodegenGenericDataModelOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataModelOutputTypeDef",
+    {
+        "fields": Dict[str, "CodegenGenericDataFieldOutputTypeDef"],
+        "primaryKeys": List[str],
+    },
+)
+_OptionalCodegenGenericDataModelOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataModelOutputTypeDef",
+    {
+        "isJoinTable": bool,
+    },
+    total=False,
+)
+
+class CodegenGenericDataModelOutputTypeDef(
+    _RequiredCodegenGenericDataModelOutputTypeDef, _OptionalCodegenGenericDataModelOutputTypeDef
+):
+    pass
+
 _RequiredCodegenGenericDataModelTypeDef = TypedDict(
     "_RequiredCodegenGenericDataModelTypeDef",
     {
-        "fields": Dict[str, "CodegenGenericDataFieldTypeDef"],
-        "primaryKeys": List[str],
+        "fields": Mapping[str, "CodegenGenericDataFieldTypeDef"],
+        "primaryKeys": Sequence[str],
     },
 )
 _OptionalCodegenGenericDataModelTypeDef = TypedDict(
     "_OptionalCodegenGenericDataModelTypeDef",
     {
         "isJoinTable": bool,
     },
@@ -230,37 +347,71 @@
 )
 
 class CodegenGenericDataModelTypeDef(
     _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
 ):
     pass
 
+CodegenGenericDataNonModelOutputTypeDef = TypedDict(
+    "CodegenGenericDataNonModelOutputTypeDef",
+    {
+        "fields": Dict[str, "CodegenGenericDataFieldOutputTypeDef"],
+    },
+)
+
 CodegenGenericDataNonModelTypeDef = TypedDict(
     "CodegenGenericDataNonModelTypeDef",
     {
-        "fields": Dict[str, "CodegenGenericDataFieldTypeDef"],
+        "fields": Mapping[str, "CodegenGenericDataFieldTypeDef"],
+    },
+)
+
+_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef",
+    {
+        "type": GenericDataRelationshipTypeType,
+        "relatedModelName": str,
+    },
+)
+_OptionalCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataRelationshipTypeOutputTypeDef",
+    {
+        "relatedModelFields": List[str],
+        "canUnlinkAssociatedModel": bool,
+        "relatedJoinFieldName": str,
+        "relatedJoinTableName": str,
+        "belongsToFieldOnRelatedModel": str,
+        "associatedFields": List[str],
+        "isHasManyIndex": bool,
     },
+    total=False,
 )
 
+class CodegenGenericDataRelationshipTypeOutputTypeDef(
+    _RequiredCodegenGenericDataRelationshipTypeOutputTypeDef,
+    _OptionalCodegenGenericDataRelationshipTypeOutputTypeDef,
+):
+    pass
+
 _RequiredCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
     "_RequiredCodegenGenericDataRelationshipTypeTypeDef",
     {
         "type": GenericDataRelationshipTypeType,
         "relatedModelName": str,
     },
 )
 _OptionalCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
     "_OptionalCodegenGenericDataRelationshipTypeTypeDef",
     {
-        "relatedModelFields": List[str],
+        "relatedModelFields": Sequence[str],
         "canUnlinkAssociatedModel": bool,
         "relatedJoinFieldName": str,
         "relatedJoinTableName": str,
         "belongsToFieldOnRelatedModel": str,
-        "associatedFields": List[str],
+        "associatedFields": Sequence[str],
         "isHasManyIndex": bool,
     },
     total=False,
 )
 
 class CodegenGenericDataRelationshipTypeTypeDef(
     _RequiredCodegenGenericDataRelationshipTypeTypeDef,
@@ -272,24 +423,42 @@
     "CodegenJobAssetTypeDef",
     {
         "downloadUrl": str,
     },
     total=False,
 )
 
+CodegenJobGenericDataSchemaOutputTypeDef = TypedDict(
+    "CodegenJobGenericDataSchemaOutputTypeDef",
+    {
+        "dataSourceType": Literal["DataStore"],
+        "models": Dict[str, "CodegenGenericDataModelOutputTypeDef"],
+        "enums": Dict[str, "CodegenGenericDataEnumOutputTypeDef"],
+        "nonModels": Dict[str, "CodegenGenericDataNonModelOutputTypeDef"],
+    },
+)
+
 CodegenJobGenericDataSchemaTypeDef = TypedDict(
     "CodegenJobGenericDataSchemaTypeDef",
     {
         "dataSourceType": Literal["DataStore"],
-        "models": Dict[str, "CodegenGenericDataModelTypeDef"],
-        "enums": Dict[str, "CodegenGenericDataEnumTypeDef"],
-        "nonModels": Dict[str, "CodegenGenericDataNonModelTypeDef"],
+        "models": Mapping[str, "CodegenGenericDataModelTypeDef"],
+        "enums": Mapping[str, "CodegenGenericDataEnumTypeDef"],
+        "nonModels": Mapping[str, "CodegenGenericDataNonModelTypeDef"],
     },
 )
 
+CodegenJobRenderConfigOutputTypeDef = TypedDict(
+    "CodegenJobRenderConfigOutputTypeDef",
+    {
+        "react": "ReactStartCodegenJobDataOutputTypeDef",
+    },
+    total=False,
+)
+
 CodegenJobRenderConfigTypeDef = TypedDict(
     "CodegenJobRenderConfigTypeDef",
     {
         "react": "ReactStartCodegenJobDataTypeDef",
     },
     total=False,
 )
@@ -323,31 +492,56 @@
         "appId": str,
         "environmentName": str,
     },
 )
 _OptionalCodegenJobTypeDef = TypedDict(
     "_OptionalCodegenJobTypeDef",
     {
-        "renderConfig": "CodegenJobRenderConfigTypeDef",
-        "genericDataSchema": "CodegenJobGenericDataSchemaTypeDef",
+        "renderConfig": "CodegenJobRenderConfigOutputTypeDef",
+        "genericDataSchema": "CodegenJobGenericDataSchemaOutputTypeDef",
         "autoGenerateForms": bool,
-        "features": "CodegenFeatureFlagsTypeDef",
+        "features": "CodegenFeatureFlagsOutputTypeDef",
         "status": CodegenJobStatusType,
         "statusMessage": str,
         "asset": "CodegenJobAssetTypeDef",
         "tags": Dict[str, str],
         "createdAt": datetime,
         "modifiedAt": datetime,
     },
     total=False,
 )
 
 class CodegenJobTypeDef(_RequiredCodegenJobTypeDef, _OptionalCodegenJobTypeDef):
     pass
 
+ComponentBindingPropertiesValueOutputTypeDef = TypedDict(
+    "ComponentBindingPropertiesValueOutputTypeDef",
+    {
+        "type": str,
+        "bindingProperties": "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
+        "defaultValue": str,
+    },
+    total=False,
+)
+
+ComponentBindingPropertiesValuePropertiesOutputTypeDef = TypedDict(
+    "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
+    {
+        "model": str,
+        "field": str,
+        "predicates": List["PredicateOutputTypeDef"],
+        "userAttribute": str,
+        "bucket": str,
+        "key": str,
+        "defaultValue": str,
+        "slotName": str,
+    },
+    total=False,
+)
+
 ComponentBindingPropertiesValuePropertiesTypeDef = TypedDict(
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     {
         "model": str,
         "field": str,
         "predicates": Sequence["PredicateTypeDef"],
         "userAttribute": str,
@@ -365,14 +559,37 @@
         "type": str,
         "bindingProperties": "ComponentBindingPropertiesValuePropertiesTypeDef",
         "defaultValue": str,
     },
     total=False,
 )
 
+_RequiredComponentChildOutputTypeDef = TypedDict(
+    "_RequiredComponentChildOutputTypeDef",
+    {
+        "componentType": str,
+        "name": str,
+        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
+    },
+)
+_OptionalComponentChildOutputTypeDef = TypedDict(
+    "_OptionalComponentChildOutputTypeDef",
+    {
+        "children": List[Dict[str, Any]],
+        "events": Dict[str, "ComponentEventOutputTypeDef"],
+        "sourceId": str,
+    },
+    total=False,
+)
+
+class ComponentChildOutputTypeDef(
+    _RequiredComponentChildOutputTypeDef, _OptionalComponentChildOutputTypeDef
+):
+    pass
+
 _RequiredComponentChildTypeDef = TypedDict(
     "_RequiredComponentChildTypeDef",
     {
         "componentType": str,
         "name": str,
         "properties": Mapping[str, "ComponentPropertyTypeDef"],
     },
@@ -386,28 +603,64 @@
     },
     total=False,
 )
 
 class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
     pass
 
+ComponentConditionPropertyOutputTypeDef = TypedDict(
+    "ComponentConditionPropertyOutputTypeDef",
+    {
+        "property": str,
+        "field": str,
+        "operator": str,
+        "operand": str,
+        "then": Dict[str, Any],
+        "else": Dict[str, Any],
+        "operandType": str,
+    },
+    total=False,
+)
+
 ComponentConditionPropertyTypeDef = TypedDict(
     "ComponentConditionPropertyTypeDef",
     {
         "property": str,
         "field": str,
         "operator": str,
         "operand": str,
         "then": Dict[str, Any],
         "else": Dict[str, Any],
         "operandType": str,
     },
     total=False,
 )
 
+_RequiredComponentDataConfigurationOutputTypeDef = TypedDict(
+    "_RequiredComponentDataConfigurationOutputTypeDef",
+    {
+        "model": str,
+    },
+)
+_OptionalComponentDataConfigurationOutputTypeDef = TypedDict(
+    "_OptionalComponentDataConfigurationOutputTypeDef",
+    {
+        "sort": List["SortPropertyOutputTypeDef"],
+        "predicate": "PredicateOutputTypeDef",
+        "identifiers": List[str],
+    },
+    total=False,
+)
+
+class ComponentDataConfigurationOutputTypeDef(
+    _RequiredComponentDataConfigurationOutputTypeDef,
+    _OptionalComponentDataConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredComponentDataConfigurationTypeDef = TypedDict(
     "_RequiredComponentDataConfigurationTypeDef",
     {
         "model": str,
     },
 )
 _OptionalComponentDataConfigurationTypeDef = TypedDict(
@@ -421,24 +674,54 @@
 )
 
 class ComponentDataConfigurationTypeDef(
     _RequiredComponentDataConfigurationTypeDef, _OptionalComponentDataConfigurationTypeDef
 ):
     pass
 
+ComponentEventOutputTypeDef = TypedDict(
+    "ComponentEventOutputTypeDef",
+    {
+        "action": str,
+        "parameters": "ActionParametersOutputTypeDef",
+        "bindingEvent": str,
+    },
+    total=False,
+)
+
 ComponentEventTypeDef = TypedDict(
     "ComponentEventTypeDef",
     {
         "action": str,
         "parameters": "ActionParametersTypeDef",
         "bindingEvent": str,
     },
     total=False,
 )
 
+_RequiredComponentPropertyBindingPropertiesOutputTypeDef = TypedDict(
+    "_RequiredComponentPropertyBindingPropertiesOutputTypeDef",
+    {
+        "property": str,
+    },
+)
+_OptionalComponentPropertyBindingPropertiesOutputTypeDef = TypedDict(
+    "_OptionalComponentPropertyBindingPropertiesOutputTypeDef",
+    {
+        "field": str,
+    },
+    total=False,
+)
+
+class ComponentPropertyBindingPropertiesOutputTypeDef(
+    _RequiredComponentPropertyBindingPropertiesOutputTypeDef,
+    _OptionalComponentPropertyBindingPropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredComponentPropertyBindingPropertiesTypeDef = TypedDict(
     "_RequiredComponentPropertyBindingPropertiesTypeDef",
     {
         "property": str,
     },
 )
 _OptionalComponentPropertyBindingPropertiesTypeDef = TypedDict(
@@ -451,14 +734,36 @@
 
 class ComponentPropertyBindingPropertiesTypeDef(
     _RequiredComponentPropertyBindingPropertiesTypeDef,
     _OptionalComponentPropertyBindingPropertiesTypeDef,
 ):
     pass
 
+ComponentPropertyOutputTypeDef = TypedDict(
+    "ComponentPropertyOutputTypeDef",
+    {
+        "value": str,
+        "bindingProperties": "ComponentPropertyBindingPropertiesOutputTypeDef",
+        "collectionBindingProperties": "ComponentPropertyBindingPropertiesOutputTypeDef",
+        "defaultValue": str,
+        "model": str,
+        "bindings": Dict[str, "FormBindingElementOutputTypeDef"],
+        "event": str,
+        "userAttribute": str,
+        "concat": List[Dict[str, Any]],
+        "condition": Dict[str, Any],
+        "configured": bool,
+        "type": str,
+        "importedValue": str,
+        "componentName": str,
+        "property": str,
+    },
+    total=False,
+)
+
 ComponentPropertyTypeDef = TypedDict(
     "ComponentPropertyTypeDef",
     {
         "value": str,
         "bindingProperties": "ComponentPropertyBindingPropertiesTypeDef",
         "collectionBindingProperties": "ComponentPropertyBindingPropertiesTypeDef",
         "defaultValue": str,
@@ -492,38 +797,47 @@
     "_RequiredComponentTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "componentType": str,
-        "properties": Dict[str, "ComponentPropertyTypeDef"],
-        "variants": List["ComponentVariantTypeDef"],
+        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "variants": List["ComponentVariantOutputTypeDef"],
         "overrides": Dict[str, Dict[str, str]],
-        "bindingProperties": Dict[str, "ComponentBindingPropertiesValueTypeDef"],
+        "bindingProperties": Dict[str, "ComponentBindingPropertiesValueOutputTypeDef"],
         "createdAt": datetime,
     },
 )
 _OptionalComponentTypeDef = TypedDict(
     "_OptionalComponentTypeDef",
     {
         "sourceId": str,
-        "children": List["ComponentChildTypeDef"],
-        "collectionProperties": Dict[str, "ComponentDataConfigurationTypeDef"],
+        "children": List["ComponentChildOutputTypeDef"],
+        "collectionProperties": Dict[str, "ComponentDataConfigurationOutputTypeDef"],
         "modifiedAt": datetime,
         "tags": Dict[str, str],
-        "events": Dict[str, "ComponentEventTypeDef"],
+        "events": Dict[str, "ComponentEventOutputTypeDef"],
         "schemaVersion": str,
     },
     total=False,
 )
 
 class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
     pass
 
+ComponentVariantOutputTypeDef = TypedDict(
+    "ComponentVariantOutputTypeDef",
+    {
+        "variantValues": Dict[str, str],
+        "overrides": Dict[str, Dict[str, str]],
+    },
+    total=False,
+)
+
 ComponentVariantTypeDef = TypedDict(
     "ComponentVariantTypeDef",
     {
         "variantValues": Mapping[str, str],
         "overrides": Mapping[str, Mapping[str, str]],
     },
     total=False,
@@ -907,26 +1221,71 @@
     {
         "entities": List["ThemeTypeDef"],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FieldConfigOutputTypeDef = TypedDict(
+    "FieldConfigOutputTypeDef",
+    {
+        "label": str,
+        "position": "FieldPositionOutputTypeDef",
+        "excluded": bool,
+        "inputType": "FieldInputConfigOutputTypeDef",
+        "validations": List["FieldValidationConfigurationOutputTypeDef"],
+    },
+    total=False,
+)
+
 FieldConfigTypeDef = TypedDict(
     "FieldConfigTypeDef",
     {
         "label": str,
         "position": "FieldPositionTypeDef",
         "excluded": bool,
         "inputType": "FieldInputConfigTypeDef",
         "validations": Sequence["FieldValidationConfigurationTypeDef"],
     },
     total=False,
 )
 
+_RequiredFieldInputConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldInputConfigOutputTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalFieldInputConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldInputConfigOutputTypeDef",
+    {
+        "required": bool,
+        "readOnly": bool,
+        "placeholder": str,
+        "defaultValue": str,
+        "descriptiveText": str,
+        "defaultChecked": bool,
+        "defaultCountryCode": str,
+        "valueMappings": "ValueMappingsOutputTypeDef",
+        "name": str,
+        "minValue": float,
+        "maxValue": float,
+        "step": float,
+        "value": str,
+        "isArray": bool,
+        "fileUploaderConfig": "FileUploaderFieldConfigOutputTypeDef",
+    },
+    total=False,
+)
+
+class FieldInputConfigOutputTypeDef(
+    _RequiredFieldInputConfigOutputTypeDef, _OptionalFieldInputConfigOutputTypeDef
+):
+    pass
+
 _RequiredFieldInputConfigTypeDef = TypedDict(
     "_RequiredFieldInputConfigTypeDef",
     {
         "type": str,
     },
 )
 _OptionalFieldInputConfigTypeDef = TypedDict(
@@ -950,24 +1309,56 @@
     },
     total=False,
 )
 
 class FieldInputConfigTypeDef(_RequiredFieldInputConfigTypeDef, _OptionalFieldInputConfigTypeDef):
     pass
 
+FieldPositionOutputTypeDef = TypedDict(
+    "FieldPositionOutputTypeDef",
+    {
+        "fixed": Literal["first"],
+        "rightOf": str,
+        "below": str,
+    },
+    total=False,
+)
+
 FieldPositionTypeDef = TypedDict(
     "FieldPositionTypeDef",
     {
         "fixed": Literal["first"],
         "rightOf": str,
         "below": str,
     },
     total=False,
 )
 
+_RequiredFieldValidationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFieldValidationConfigurationOutputTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalFieldValidationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFieldValidationConfigurationOutputTypeDef",
+    {
+        "strValues": List[str],
+        "numValues": List[int],
+        "validationMessage": str,
+    },
+    total=False,
+)
+
+class FieldValidationConfigurationOutputTypeDef(
+    _RequiredFieldValidationConfigurationOutputTypeDef,
+    _OptionalFieldValidationConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredFieldValidationConfigurationTypeDef = TypedDict(
     "_RequiredFieldValidationConfigurationTypeDef",
     {
         "type": str,
     },
 )
 _OptionalFieldValidationConfigurationTypeDef = TypedDict(
@@ -981,14 +1372,37 @@
 )
 
 class FieldValidationConfigurationTypeDef(
     _RequiredFieldValidationConfigurationTypeDef, _OptionalFieldValidationConfigurationTypeDef
 ):
     pass
 
+_RequiredFileUploaderFieldConfigOutputTypeDef = TypedDict(
+    "_RequiredFileUploaderFieldConfigOutputTypeDef",
+    {
+        "accessLevel": StorageAccessLevelType,
+        "acceptedFileTypes": List[str],
+    },
+)
+_OptionalFileUploaderFieldConfigOutputTypeDef = TypedDict(
+    "_OptionalFileUploaderFieldConfigOutputTypeDef",
+    {
+        "showThumbnails": bool,
+        "isResumable": bool,
+        "maxFileCount": int,
+        "maxSize": int,
+    },
+    total=False,
+)
+
+class FileUploaderFieldConfigOutputTypeDef(
+    _RequiredFileUploaderFieldConfigOutputTypeDef, _OptionalFileUploaderFieldConfigOutputTypeDef
+):
+    pass
+
 _RequiredFileUploaderFieldConfigTypeDef = TypedDict(
     "_RequiredFileUploaderFieldConfigTypeDef",
     {
         "accessLevel": StorageAccessLevelType,
         "acceptedFileTypes": Sequence[str],
     },
 )
@@ -1004,51 +1418,105 @@
 )
 
 class FileUploaderFieldConfigTypeDef(
     _RequiredFileUploaderFieldConfigTypeDef, _OptionalFileUploaderFieldConfigTypeDef
 ):
     pass
 
+FormBindingElementOutputTypeDef = TypedDict(
+    "FormBindingElementOutputTypeDef",
+    {
+        "element": str,
+        "property": str,
+    },
+)
+
 FormBindingElementTypeDef = TypedDict(
     "FormBindingElementTypeDef",
     {
         "element": str,
         "property": str,
     },
 )
 
+FormButtonOutputTypeDef = TypedDict(
+    "FormButtonOutputTypeDef",
+    {
+        "excluded": bool,
+        "children": str,
+        "position": "FieldPositionOutputTypeDef",
+    },
+    total=False,
+)
+
 FormButtonTypeDef = TypedDict(
     "FormButtonTypeDef",
     {
         "excluded": bool,
         "children": str,
         "position": "FieldPositionTypeDef",
     },
     total=False,
 )
 
+FormCTAOutputTypeDef = TypedDict(
+    "FormCTAOutputTypeDef",
+    {
+        "position": FormButtonsPositionType,
+        "clear": "FormButtonOutputTypeDef",
+        "cancel": "FormButtonOutputTypeDef",
+        "submit": "FormButtonOutputTypeDef",
+    },
+    total=False,
+)
+
 FormCTATypeDef = TypedDict(
     "FormCTATypeDef",
     {
         "position": FormButtonsPositionType,
         "clear": "FormButtonTypeDef",
         "cancel": "FormButtonTypeDef",
         "submit": "FormButtonTypeDef",
     },
     total=False,
 )
 
+FormDataTypeConfigOutputTypeDef = TypedDict(
+    "FormDataTypeConfigOutputTypeDef",
+    {
+        "dataSourceType": FormDataSourceTypeType,
+        "dataTypeName": str,
+    },
+)
+
 FormDataTypeConfigTypeDef = TypedDict(
     "FormDataTypeConfigTypeDef",
     {
         "dataSourceType": FormDataSourceTypeType,
         "dataTypeName": str,
     },
 )
 
+FormInputBindingPropertiesValueOutputTypeDef = TypedDict(
+    "FormInputBindingPropertiesValueOutputTypeDef",
+    {
+        "type": str,
+        "bindingProperties": "FormInputBindingPropertiesValuePropertiesOutputTypeDef",
+    },
+    total=False,
+)
+
+FormInputBindingPropertiesValuePropertiesOutputTypeDef = TypedDict(
+    "FormInputBindingPropertiesValuePropertiesOutputTypeDef",
+    {
+        "model": str,
+    },
+    total=False,
+)
+
 FormInputBindingPropertiesValuePropertiesTypeDef = TypedDict(
     "FormInputBindingPropertiesValuePropertiesTypeDef",
     {
         "model": str,
     },
     total=False,
 )
@@ -1058,14 +1526,34 @@
     {
         "type": str,
         "bindingProperties": "FormInputBindingPropertiesValuePropertiesTypeDef",
     },
     total=False,
 )
 
+_RequiredFormInputValuePropertyBindingPropertiesOutputTypeDef = TypedDict(
+    "_RequiredFormInputValuePropertyBindingPropertiesOutputTypeDef",
+    {
+        "property": str,
+    },
+)
+_OptionalFormInputValuePropertyBindingPropertiesOutputTypeDef = TypedDict(
+    "_OptionalFormInputValuePropertyBindingPropertiesOutputTypeDef",
+    {
+        "field": str,
+    },
+    total=False,
+)
+
+class FormInputValuePropertyBindingPropertiesOutputTypeDef(
+    _RequiredFormInputValuePropertyBindingPropertiesOutputTypeDef,
+    _OptionalFormInputValuePropertyBindingPropertiesOutputTypeDef,
+):
+    pass
+
 _RequiredFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
     "_RequiredFormInputValuePropertyBindingPropertiesTypeDef",
     {
         "property": str,
     },
 )
 _OptionalFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
@@ -1078,48 +1566,77 @@
 
 class FormInputValuePropertyBindingPropertiesTypeDef(
     _RequiredFormInputValuePropertyBindingPropertiesTypeDef,
     _OptionalFormInputValuePropertyBindingPropertiesTypeDef,
 ):
     pass
 
+FormInputValuePropertyOutputTypeDef = TypedDict(
+    "FormInputValuePropertyOutputTypeDef",
+    {
+        "value": str,
+        "bindingProperties": "FormInputValuePropertyBindingPropertiesOutputTypeDef",
+        "concat": List[Dict[str, Any]],
+    },
+    total=False,
+)
+
 FormInputValuePropertyTypeDef = TypedDict(
     "FormInputValuePropertyTypeDef",
     {
         "value": str,
         "bindingProperties": "FormInputValuePropertyBindingPropertiesTypeDef",
         "concat": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+FormStyleConfigOutputTypeDef = TypedDict(
+    "FormStyleConfigOutputTypeDef",
+    {
+        "tokenReference": str,
+        "value": str,
+    },
+    total=False,
+)
+
 FormStyleConfigTypeDef = TypedDict(
     "FormStyleConfigTypeDef",
     {
         "tokenReference": str,
         "value": str,
     },
     total=False,
 )
 
+FormStyleOutputTypeDef = TypedDict(
+    "FormStyleOutputTypeDef",
+    {
+        "horizontalGap": "FormStyleConfigOutputTypeDef",
+        "verticalGap": "FormStyleConfigOutputTypeDef",
+        "outerPadding": "FormStyleConfigOutputTypeDef",
+    },
+    total=False,
+)
+
 FormStyleTypeDef = TypedDict(
     "FormStyleTypeDef",
     {
         "horizontalGap": "FormStyleConfigTypeDef",
         "verticalGap": "FormStyleConfigTypeDef",
         "outerPadding": "FormStyleConfigTypeDef",
     },
     total=False,
 )
 
 FormSummaryTypeDef = TypedDict(
     "FormSummaryTypeDef",
     {
         "appId": str,
-        "dataType": "FormDataTypeConfigTypeDef",
+        "dataType": "FormDataTypeConfigOutputTypeDef",
         "environmentName": str,
         "formActionType": FormActionTypeType,
         "id": str,
         "name": str,
     },
 )
 
@@ -1127,26 +1644,26 @@
     "_RequiredFormTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "formActionType": FormActionTypeType,
-        "style": "FormStyleTypeDef",
-        "dataType": "FormDataTypeConfigTypeDef",
-        "fields": Dict[str, "FieldConfigTypeDef"],
-        "sectionalElements": Dict[str, "SectionalElementTypeDef"],
+        "style": "FormStyleOutputTypeDef",
+        "dataType": "FormDataTypeConfigOutputTypeDef",
+        "fields": Dict[str, "FieldConfigOutputTypeDef"],
+        "sectionalElements": Dict[str, "SectionalElementOutputTypeDef"],
         "schemaVersion": str,
     },
 )
 _OptionalFormTypeDef = TypedDict(
     "_OptionalFormTypeDef",
     {
         "tags": Dict[str, str],
-        "cta": "FormCTATypeDef",
+        "cta": "FormCTAOutputTypeDef",
         "labelDecorator": LabelDecoratorType,
     },
     total=False,
 )
 
 class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
     pass
@@ -1435,14 +1952,23 @@
     {
         "entities": List["ThemeSummaryTypeDef"],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MutationActionSetStateParameterOutputTypeDef = TypedDict(
+    "MutationActionSetStateParameterOutputTypeDef",
+    {
+        "componentName": str,
+        "property": str,
+        "set": "ComponentPropertyOutputTypeDef",
+    },
+)
+
 MutationActionSetStateParameterTypeDef = TypedDict(
     "MutationActionSetStateParameterTypeDef",
     {
         "componentName": str,
         "property": str,
         "set": "ComponentPropertyTypeDef",
     },
@@ -1454,14 +1980,27 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PredicateOutputTypeDef = TypedDict(
+    "PredicateOutputTypeDef",
+    {
+        "or": List[Dict[str, Any]],
+        "and": List[Dict[str, Any]],
+        "field": str,
+        "operator": str,
+        "operand": str,
+        "operandType": str,
+    },
+    total=False,
+)
+
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "or": Sequence[Dict[str, Any]],
         "and": Sequence[Dict[str, Any]],
         "field": str,
         "operator": str,
@@ -1484,14 +2023,26 @@
         "appId": str,
         "environmentName": str,
         "featureName": str,
         "body": "PutMetadataFlagBodyTypeDef",
     },
 )
 
+ReactStartCodegenJobDataOutputTypeDef = TypedDict(
+    "ReactStartCodegenJobDataOutputTypeDef",
+    {
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
+    },
+    total=False,
+)
+
 ReactStartCodegenJobDataTypeDef = TypedDict(
     "ReactStartCodegenJobDataTypeDef",
     {
         "module": JSModuleType,
         "target": JSTargetType,
         "script": JSScriptType,
         "renderTypeDeclarations": bool,
@@ -1543,14 +2094,37 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredSectionalElementOutputTypeDef = TypedDict(
+    "_RequiredSectionalElementOutputTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalSectionalElementOutputTypeDef = TypedDict(
+    "_OptionalSectionalElementOutputTypeDef",
+    {
+        "position": "FieldPositionOutputTypeDef",
+        "text": str,
+        "level": int,
+        "orientation": str,
+        "excluded": bool,
+    },
+    total=False,
+)
+
+class SectionalElementOutputTypeDef(
+    _RequiredSectionalElementOutputTypeDef, _OptionalSectionalElementOutputTypeDef
+):
+    pass
+
 _RequiredSectionalElementTypeDef = TypedDict(
     "_RequiredSectionalElementTypeDef",
     {
         "type": str,
     },
 )
 _OptionalSectionalElementTypeDef = TypedDict(
@@ -1564,14 +2138,22 @@
     },
     total=False,
 )
 
 class SectionalElementTypeDef(_RequiredSectionalElementTypeDef, _OptionalSectionalElementTypeDef):
     pass
 
+SortPropertyOutputTypeDef = TypedDict(
+    "SortPropertyOutputTypeDef",
+    {
+        "field": str,
+        "direction": SortDirectionType,
+    },
+)
+
 SortPropertyTypeDef = TypedDict(
     "SortPropertyTypeDef",
     {
         "field": str,
         "direction": SortDirectionType,
     },
 )
@@ -1641,39 +2223,57 @@
     "_RequiredThemeTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "createdAt": datetime,
-        "values": List["ThemeValuesTypeDef"],
+        "values": List["ThemeValuesOutputTypeDef"],
     },
 )
 _OptionalThemeTypeDef = TypedDict(
     "_OptionalThemeTypeDef",
     {
         "modifiedAt": datetime,
-        "overrides": List["ThemeValuesTypeDef"],
+        "overrides": List["ThemeValuesOutputTypeDef"],
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class ThemeTypeDef(_RequiredThemeTypeDef, _OptionalThemeTypeDef):
     pass
 
+ThemeValueOutputTypeDef = TypedDict(
+    "ThemeValueOutputTypeDef",
+    {
+        "value": str,
+        "children": List[Dict[str, Any]],
+    },
+    total=False,
+)
+
 ThemeValueTypeDef = TypedDict(
     "ThemeValueTypeDef",
     {
         "value": str,
         "children": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+ThemeValuesOutputTypeDef = TypedDict(
+    "ThemeValuesOutputTypeDef",
+    {
+        "key": str,
+        "value": Dict[str, Any],
+    },
+    total=False,
+)
+
 ThemeValuesTypeDef = TypedDict(
     "ThemeValuesTypeDef",
     {
         "key": str,
         "value": Dict[str, Any],
     },
     total=False,
@@ -1819,14 +2419,33 @@
     "UpdateThemeResponseTypeDef",
     {
         "entity": "ThemeTypeDef",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredValueMappingOutputTypeDef = TypedDict(
+    "_RequiredValueMappingOutputTypeDef",
+    {
+        "value": "FormInputValuePropertyOutputTypeDef",
+    },
+)
+_OptionalValueMappingOutputTypeDef = TypedDict(
+    "_OptionalValueMappingOutputTypeDef",
+    {
+        "displayValue": "FormInputValuePropertyOutputTypeDef",
+    },
+    total=False,
+)
+
+class ValueMappingOutputTypeDef(
+    _RequiredValueMappingOutputTypeDef, _OptionalValueMappingOutputTypeDef
+):
+    pass
+
 _RequiredValueMappingTypeDef = TypedDict(
     "_RequiredValueMappingTypeDef",
     {
         "value": "FormInputValuePropertyTypeDef",
     },
 )
 _OptionalValueMappingTypeDef = TypedDict(
@@ -1836,14 +2455,33 @@
     },
     total=False,
 )
 
 class ValueMappingTypeDef(_RequiredValueMappingTypeDef, _OptionalValueMappingTypeDef):
     pass
 
+_RequiredValueMappingsOutputTypeDef = TypedDict(
+    "_RequiredValueMappingsOutputTypeDef",
+    {
+        "values": List["ValueMappingOutputTypeDef"],
+    },
+)
+_OptionalValueMappingsOutputTypeDef = TypedDict(
+    "_OptionalValueMappingsOutputTypeDef",
+    {
+        "bindingProperties": Dict[str, "FormInputBindingPropertiesValueOutputTypeDef"],
+    },
+    total=False,
+)
+
+class ValueMappingsOutputTypeDef(
+    _RequiredValueMappingsOutputTypeDef, _OptionalValueMappingsOutputTypeDef
+):
+    pass
+
 _RequiredValueMappingsTypeDef = TypedDict(
     "_RequiredValueMappingsTypeDef",
     {
         "values": Sequence["ValueMappingTypeDef"],
     },
 )
 _OptionalValueMappingsTypeDef = TypedDict(
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifyuibuilder
-Version: 1.28.0
-Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-amplifyuibuilder"></a>
 
 # mypy-boto3-amplifyuibuilder
 
 [![PyPI - mypy-boto3-amplifyuibuilder](https://img.shields.io/pypi/v/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-amplifyuibuilder?color=blue)](https://pypistats.org/packages/mypy-boto3-amplifyuibuilder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifyuibuilder)](https://pepy.tech/project/mypy-boto3-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyUIBuilder 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[boto3.AmplifyUIBuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
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
 [mypy-boto3-amplifyuibuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,36 +355,54 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
+    ActionParametersOutputTypeDef,
     ActionParametersTypeDef,
+    CodegenFeatureFlagsOutputTypeDef,
     CodegenFeatureFlagsTypeDef,
+    CodegenGenericDataEnumOutputTypeDef,
     CodegenGenericDataEnumTypeDef,
+    CodegenGenericDataFieldOutputTypeDef,
     CodegenGenericDataFieldTypeDef,
+    CodegenGenericDataModelOutputTypeDef,
     CodegenGenericDataModelTypeDef,
+    CodegenGenericDataNonModelOutputTypeDef,
     CodegenGenericDataNonModelTypeDef,
+    CodegenGenericDataRelationshipTypeOutputTypeDef,
     CodegenGenericDataRelationshipTypeTypeDef,
     CodegenJobAssetTypeDef,
+    CodegenJobGenericDataSchemaOutputTypeDef,
     CodegenJobGenericDataSchemaTypeDef,
+    CodegenJobRenderConfigOutputTypeDef,
     CodegenJobRenderConfigTypeDef,
     CodegenJobSummaryTypeDef,
     CodegenJobTypeDef,
+    ComponentBindingPropertiesValueOutputTypeDef,
+    ComponentBindingPropertiesValuePropertiesOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
     ComponentBindingPropertiesValueTypeDef,
+    ComponentChildOutputTypeDef,
     ComponentChildTypeDef,
+    ComponentConditionPropertyOutputTypeDef,
     ComponentConditionPropertyTypeDef,
+    ComponentDataConfigurationOutputTypeDef,
     ComponentDataConfigurationTypeDef,
+    ComponentEventOutputTypeDef,
     ComponentEventTypeDef,
+    ComponentPropertyBindingPropertiesOutputTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
+    ComponentPropertyOutputTypeDef,
     ComponentPropertyTypeDef,
     ComponentSummaryTypeDef,
     ComponentTypeDef,
+    ComponentVariantOutputTypeDef,
     ComponentVariantTypeDef,
     CreateComponentDataTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateComponentResponseTypeDef,
     CreateFormDataTypeDef,
     CreateFormRequestRequestTypeDef,
     CreateFormResponseTypeDef,
@@ -403,28 +421,43 @@
     ExportComponentsResponseTypeDef,
     ExportFormsRequestExportFormsPaginateTypeDef,
     ExportFormsRequestRequestTypeDef,
     ExportFormsResponseTypeDef,
     ExportThemesRequestExportThemesPaginateTypeDef,
     ExportThemesRequestRequestTypeDef,
     ExportThemesResponseTypeDef,
+    FieldConfigOutputTypeDef,
     FieldConfigTypeDef,
+    FieldInputConfigOutputTypeDef,
     FieldInputConfigTypeDef,
+    FieldPositionOutputTypeDef,
     FieldPositionTypeDef,
+    FieldValidationConfigurationOutputTypeDef,
     FieldValidationConfigurationTypeDef,
+    FileUploaderFieldConfigOutputTypeDef,
     FileUploaderFieldConfigTypeDef,
+    FormBindingElementOutputTypeDef,
     FormBindingElementTypeDef,
+    FormButtonOutputTypeDef,
     FormButtonTypeDef,
+    FormCTAOutputTypeDef,
     FormCTATypeDef,
+    FormDataTypeConfigOutputTypeDef,
     FormDataTypeConfigTypeDef,
+    FormInputBindingPropertiesValueOutputTypeDef,
+    FormInputBindingPropertiesValuePropertiesOutputTypeDef,
     FormInputBindingPropertiesValuePropertiesTypeDef,
     FormInputBindingPropertiesValueTypeDef,
+    FormInputValuePropertyBindingPropertiesOutputTypeDef,
     FormInputValuePropertyBindingPropertiesTypeDef,
+    FormInputValuePropertyOutputTypeDef,
     FormInputValuePropertyTypeDef,
+    FormStyleConfigOutputTypeDef,
     FormStyleConfigTypeDef,
+    FormStyleOutputTypeDef,
     FormStyleTypeDef,
     FormSummaryTypeDef,
     FormTypeDef,
     GetCodegenJobRequestRequestTypeDef,
     GetCodegenJobResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetComponentResponseTypeDef,
@@ -442,48 +475,57 @@
     ListComponentsResponseTypeDef,
     ListFormsRequestListFormsPaginateTypeDef,
     ListFormsRequestRequestTypeDef,
     ListFormsResponseTypeDef,
     ListThemesRequestListThemesPaginateTypeDef,
     ListThemesRequestRequestTypeDef,
     ListThemesResponseTypeDef,
+    MutationActionSetStateParameterOutputTypeDef,
     MutationActionSetStateParameterTypeDef,
     PaginatorConfigTypeDef,
+    PredicateOutputTypeDef,
     PredicateTypeDef,
     PutMetadataFlagBodyTypeDef,
     PutMetadataFlagRequestRequestTypeDef,
+    ReactStartCodegenJobDataOutputTypeDef,
     ReactStartCodegenJobDataTypeDef,
     RefreshTokenRequestBodyTypeDef,
     RefreshTokenRequestRequestTypeDef,
     RefreshTokenResponseTypeDef,
     ResponseMetadataTypeDef,
+    SectionalElementOutputTypeDef,
     SectionalElementTypeDef,
+    SortPropertyOutputTypeDef,
     SortPropertyTypeDef,
     StartCodegenJobDataTypeDef,
     StartCodegenJobRequestRequestTypeDef,
     StartCodegenJobResponseTypeDef,
     ThemeSummaryTypeDef,
     ThemeTypeDef,
+    ThemeValueOutputTypeDef,
     ThemeValueTypeDef,
+    ThemeValuesOutputTypeDef,
     ThemeValuesTypeDef,
     UpdateComponentDataTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateComponentResponseTypeDef,
     UpdateFormDataTypeDef,
     UpdateFormRequestRequestTypeDef,
     UpdateFormResponseTypeDef,
     UpdateThemeDataTypeDef,
     UpdateThemeRequestRequestTypeDef,
     UpdateThemeResponseTypeDef,
+    ValueMappingOutputTypeDef,
     ValueMappingTypeDef,
+    ValueMappingsOutputTypeDef,
     ValueMappingsTypeDef,
 )
 
 
-def get_structure() -> ActionParametersTypeDef:
+def get_structure() -> ActionParametersOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt` & `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.0/setup.py` & `mypy-boto3-amplifyuibuilder-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplifyuibuilder",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_amplifyuibuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AmplifyUIBuilder 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.AmplifyUIBuilder 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

