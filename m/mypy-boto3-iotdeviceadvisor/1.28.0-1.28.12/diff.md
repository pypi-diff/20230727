# Comparing `tmp/mypy-boto3-iotdeviceadvisor-1.28.0.tar.gz` & `tmp/mypy-boto3-iotdeviceadvisor-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotdeviceadvisor-1.28.0.tar", last modified: Thu Jul  6 20:59:47 2023, max compression
+gzip compressed data, was "mypy-boto3-iotdeviceadvisor-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
```

## Comparing `mypy-boto3-iotdeviceadvisor-1.28.0.tar` & `mypy-boto3-iotdeviceadvisor-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.638329 mypy-boto3-iotdeviceadvisor-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-06 20:59:47.638329 mypy-boto3-iotdeviceadvisor-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12178 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.634329 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-06 20:43:43.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.638329 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-06 20:59:47.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-06 20:59:47.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:47.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 20:59:47.000000 mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:47.638329 mypy-boto3-iotdeviceadvisor-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 20:43:42.000000 mypy-boto3-iotdeviceadvisor-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.292483 mypy-boto3-iotdeviceadvisor-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-27 05:34:49.292483 mypy-boto3-iotdeviceadvisor-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.292483 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-27 05:24:00.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-27 05:24:00.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-07-27 05:24:00.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-07-27 05:24:00.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.292483 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-27 05:34:49.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 05:34:49.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:49.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:49.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.292483 mypy-boto3-iotdeviceadvisor-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/setup.py
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/LICENSE` & `mypy-boto3-iotdeviceadvisor-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/PKG-INFO` & `mypy-boto3-iotdeviceadvisor-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotdeviceadvisor
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotdeviceadvisor"></a>
 
 # mypy-boto3-iotdeviceadvisor
 
 [![PyPI - mypy-boto3-iotdeviceadvisor](https://img.shields.io/pypi/v/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotdeviceadvisor?color=blue)](https://pypistats.org/packages/mypy-boto3-iotdeviceadvisor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotdeviceadvisor)](https://pepy.tech/project/mypy-boto3-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDeviceAdvisor 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[boto3.IoTDeviceAdvisor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,14 +305,15 @@
 `mypy_boto3_iotdeviceadvisor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotdeviceadvisor.type_defs import (
     CreateSuiteDefinitionResponseTypeDef,
     DeleteSuiteDefinitionRequestRequestTypeDef,
+    DeviceUnderTestOutputTypeDef,
     DeviceUnderTestTypeDef,
     GetEndpointRequestRequestTypeDef,
     GetEndpointResponseTypeDef,
     GetSuiteDefinitionRequestRequestTypeDef,
     GetSuiteRunReportRequestRequestTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunRequestRequestTypeDef,
@@ -324,23 +325,25 @@
     ResponseMetadataTypeDef,
     StartSuiteRunResponseTypeDef,
     StopSuiteRunRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestCaseScenarioTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
+    SuiteDefinitionConfigurationOutputTypeDef,
     SuiteDefinitionInformationTypeDef,
+    SuiteRunConfigurationOutputTypeDef,
+    SuiteDefinitionConfigurationTypeDef,
     SuiteRunConfigurationTypeDef,
     ListSuiteRunsResponseTypeDef,
     TestCaseRunTypeDef,
-    CreateSuiteDefinitionRequestRequestTypeDef,
     GetSuiteDefinitionResponseTypeDef,
-    UpdateSuiteDefinitionRequestRequestTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
+    CreateSuiteDefinitionRequestRequestTypeDef,
+    UpdateSuiteDefinitionRequestRequestTypeDef,
     StartSuiteRunRequestRequestTypeDef,
     GroupResultTypeDef,
     TestResultTypeDef,
     GetSuiteRunResponseTypeDef,
 )
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/README.md` & `mypy-boto3-iotdeviceadvisor-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-iotdeviceadvisor"></a>
 
 # mypy-boto3-iotdeviceadvisor
 
 [![PyPI - mypy-boto3-iotdeviceadvisor](https://img.shields.io/pypi/v/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotdeviceadvisor?color=blue)](https://pypistats.org/packages/mypy-boto3-iotdeviceadvisor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotdeviceadvisor)](https://pepy.tech/project/mypy-boto3-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDeviceAdvisor 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[boto3.IoTDeviceAdvisor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -273,14 +273,15 @@
 `mypy_boto3_iotdeviceadvisor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotdeviceadvisor.type_defs import (
     CreateSuiteDefinitionResponseTypeDef,
     DeleteSuiteDefinitionRequestRequestTypeDef,
+    DeviceUnderTestOutputTypeDef,
     DeviceUnderTestTypeDef,
     GetEndpointRequestRequestTypeDef,
     GetEndpointResponseTypeDef,
     GetSuiteDefinitionRequestRequestTypeDef,
     GetSuiteRunReportRequestRequestTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunRequestRequestTypeDef,
@@ -292,23 +293,25 @@
     ResponseMetadataTypeDef,
     StartSuiteRunResponseTypeDef,
     StopSuiteRunRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestCaseScenarioTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
+    SuiteDefinitionConfigurationOutputTypeDef,
     SuiteDefinitionInformationTypeDef,
+    SuiteRunConfigurationOutputTypeDef,
+    SuiteDefinitionConfigurationTypeDef,
     SuiteRunConfigurationTypeDef,
     ListSuiteRunsResponseTypeDef,
     TestCaseRunTypeDef,
-    CreateSuiteDefinitionRequestRequestTypeDef,
     GetSuiteDefinitionResponseTypeDef,
-    UpdateSuiteDefinitionRequestRequestTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
+    CreateSuiteDefinitionRequestRequestTypeDef,
+    UpdateSuiteDefinitionRequestRequestTypeDef,
     StartSuiteRunRequestRequestTypeDef,
     GroupResultTypeDef,
     TestResultTypeDef,
     GetSuiteRunResponseTypeDef,
 )
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/__main__.py` & `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTDeviceAdvisor 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoTDeviceAdvisor 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor\nOther"
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

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/client.py` & `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/client.pyi` & `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/literals.py` & `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
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
@@ -271,26 +272,28 @@
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

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/literals.pyi` & `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,15 @@
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
@@ -269,26 +270,28 @@
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

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/type_defs.py` & `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateSuiteDefinitionResponseTypeDef",
     "DeleteSuiteDefinitionRequestRequestTypeDef",
+    "DeviceUnderTestOutputTypeDef",
     "DeviceUnderTestTypeDef",
     "GetEndpointRequestRequestTypeDef",
     "GetEndpointResponseTypeDef",
     "GetSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteRunReportRequestRequestTypeDef",
     "GetSuiteRunReportResponseTypeDef",
     "GetSuiteRunRequestRequestTypeDef",
@@ -48,23 +48,25 @@
     "ResponseMetadataTypeDef",
     "StartSuiteRunResponseTypeDef",
     "StopSuiteRunRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestCaseScenarioTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateSuiteDefinitionResponseTypeDef",
-    "SuiteDefinitionConfigurationTypeDef",
+    "SuiteDefinitionConfigurationOutputTypeDef",
     "SuiteDefinitionInformationTypeDef",
+    "SuiteRunConfigurationOutputTypeDef",
+    "SuiteDefinitionConfigurationTypeDef",
     "SuiteRunConfigurationTypeDef",
     "ListSuiteRunsResponseTypeDef",
     "TestCaseRunTypeDef",
-    "CreateSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteDefinitionResponseTypeDef",
-    "UpdateSuiteDefinitionRequestRequestTypeDef",
     "ListSuiteDefinitionsResponseTypeDef",
+    "CreateSuiteDefinitionRequestRequestTypeDef",
+    "UpdateSuiteDefinitionRequestRequestTypeDef",
     "StartSuiteRunRequestRequestTypeDef",
     "GroupResultTypeDef",
     "TestResultTypeDef",
     "GetSuiteRunResponseTypeDef",
 )
 
 CreateSuiteDefinitionResponseTypeDef = TypedDict(
@@ -81,14 +83,24 @@
 DeleteSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
     },
 )
 
+DeviceUnderTestOutputTypeDef = TypedDict(
+    "DeviceUnderTestOutputTypeDef",
+    {
+        "thingArn": str,
+        "certificateArn": str,
+        "deviceRoleArn": str,
+    },
+    total=False,
+)
+
 DeviceUnderTestTypeDef = TypedDict(
     "DeviceUnderTestTypeDef",
     {
         "thingArn": str,
         "certificateArn": str,
         "deviceRoleArn": str,
     },
@@ -124,22 +136,20 @@
     "_OptionalGetSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionVersion": str,
     },
     total=False,
 )
 
-
 class GetSuiteDefinitionRequestRequestTypeDef(
     _RequiredGetSuiteDefinitionRequestRequestTypeDef,
     _OptionalGetSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 GetSuiteRunReportRequestRequestTypeDef = TypedDict(
     "GetSuiteRunReportRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
@@ -279,76 +289,117 @@
         "suiteDefinitionVersion": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredSuiteDefinitionConfigurationTypeDef = TypedDict(
-    "_RequiredSuiteDefinitionConfigurationTypeDef",
+_RequiredSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSuiteDefinitionConfigurationOutputTypeDef",
     {
         "suiteDefinitionName": str,
         "rootGroup": str,
         "devicePermissionRoleArn": str,
     },
 )
-_OptionalSuiteDefinitionConfigurationTypeDef = TypedDict(
-    "_OptionalSuiteDefinitionConfigurationTypeDef",
+_OptionalSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSuiteDefinitionConfigurationOutputTypeDef",
     {
-        "devices": Sequence[DeviceUnderTestTypeDef],
+        "devices": List[DeviceUnderTestOutputTypeDef],
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
     },
     total=False,
 )
 
-
-class SuiteDefinitionConfigurationTypeDef(
-    _RequiredSuiteDefinitionConfigurationTypeDef, _OptionalSuiteDefinitionConfigurationTypeDef
+class SuiteDefinitionConfigurationOutputTypeDef(
+    _RequiredSuiteDefinitionConfigurationOutputTypeDef,
+    _OptionalSuiteDefinitionConfigurationOutputTypeDef,
 ):
     pass
 
-
 SuiteDefinitionInformationTypeDef = TypedDict(
     "SuiteDefinitionInformationTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionName": str,
-        "defaultDevices": List[DeviceUnderTestTypeDef],
+        "defaultDevices": List[DeviceUnderTestOutputTypeDef],
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
         "createdAt": datetime,
     },
     total=False,
 )
 
+_RequiredSuiteRunConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSuiteRunConfigurationOutputTypeDef",
+    {
+        "primaryDevice": DeviceUnderTestOutputTypeDef,
+    },
+)
+_OptionalSuiteRunConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSuiteRunConfigurationOutputTypeDef",
+    {
+        "selectedTestList": List[str],
+        "parallelRun": bool,
+    },
+    total=False,
+)
+
+class SuiteRunConfigurationOutputTypeDef(
+    _RequiredSuiteRunConfigurationOutputTypeDef, _OptionalSuiteRunConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredSuiteDefinitionConfigurationTypeDef = TypedDict(
+    "_RequiredSuiteDefinitionConfigurationTypeDef",
+    {
+        "suiteDefinitionName": str,
+        "rootGroup": str,
+        "devicePermissionRoleArn": str,
+    },
+)
+_OptionalSuiteDefinitionConfigurationTypeDef = TypedDict(
+    "_OptionalSuiteDefinitionConfigurationTypeDef",
+    {
+        "devices": Sequence[DeviceUnderTestTypeDef],
+        "intendedForQualification": bool,
+        "isLongDurationTest": bool,
+        "protocol": ProtocolType,
+    },
+    total=False,
+)
+
+class SuiteDefinitionConfigurationTypeDef(
+    _RequiredSuiteDefinitionConfigurationTypeDef, _OptionalSuiteDefinitionConfigurationTypeDef
+):
+    pass
+
 _RequiredSuiteRunConfigurationTypeDef = TypedDict(
     "_RequiredSuiteRunConfigurationTypeDef",
     {
         "primaryDevice": DeviceUnderTestTypeDef,
     },
 )
 _OptionalSuiteRunConfigurationTypeDef = TypedDict(
     "_OptionalSuiteRunConfigurationTypeDef",
     {
-        "selectedTestList": List[str],
+        "selectedTestList": Sequence[str],
         "parallelRun": bool,
     },
     total=False,
 )
 
-
 class SuiteRunConfigurationTypeDef(
     _RequiredSuiteRunConfigurationTypeDef, _OptionalSuiteRunConfigurationTypeDef
 ):
     pass
 
-
 ListSuiteRunsResponseTypeDef = TypedDict(
     "ListSuiteRunsResponseTypeDef",
     {
         "suiteRunsList": List[SuiteRunInformationTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -367,68 +418,66 @@
         "warnings": str,
         "failure": str,
         "testScenarios": List[TestCaseScenarioTypeDef],
     },
     total=False,
 )
 
+GetSuiteDefinitionResponseTypeDef = TypedDict(
+    "GetSuiteDefinitionResponseTypeDef",
+    {
+        "suiteDefinitionId": str,
+        "suiteDefinitionArn": str,
+        "suiteDefinitionVersion": str,
+        "latestVersion": str,
+        "suiteDefinitionConfiguration": SuiteDefinitionConfigurationOutputTypeDef,
+        "createdAt": datetime,
+        "lastModifiedAt": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSuiteDefinitionsResponseTypeDef = TypedDict(
+    "ListSuiteDefinitionsResponseTypeDef",
+    {
+        "suiteDefinitionInformationList": List[SuiteDefinitionInformationTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
 _OptionalCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateSuiteDefinitionRequestRequestTypeDef(
     _RequiredCreateSuiteDefinitionRequestRequestTypeDef,
     _OptionalCreateSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
-GetSuiteDefinitionResponseTypeDef = TypedDict(
-    "GetSuiteDefinitionResponseTypeDef",
-    {
-        "suiteDefinitionId": str,
-        "suiteDefinitionArn": str,
-        "suiteDefinitionVersion": str,
-        "latestVersion": str,
-        "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
-        "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
 
-ListSuiteDefinitionsResponseTypeDef = TypedDict(
-    "ListSuiteDefinitionsResponseTypeDef",
-    {
-        "suiteDefinitionInformationList": List[SuiteDefinitionInformationTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartSuiteRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunConfiguration": SuiteRunConfigurationTypeDef,
     },
 )
@@ -437,21 +486,19 @@
     {
         "suiteDefinitionVersion": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartSuiteRunRequestRequestTypeDef(
     _RequiredStartSuiteRunRequestRequestTypeDef, _OptionalStartSuiteRunRequestRequestTypeDef
 ):
     pass
 
-
 GroupResultTypeDef = TypedDict(
     "GroupResultTypeDef",
     {
         "groupId": str,
         "groupName": str,
         "tests": List[TestCaseRunTypeDef],
     },
@@ -469,15 +516,15 @@
 GetSuiteRunResponseTypeDef = TypedDict(
     "GetSuiteRunResponseTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionVersion": str,
         "suiteRunId": str,
         "suiteRunArn": str,
-        "suiteRunConfiguration": SuiteRunConfigurationTypeDef,
+        "suiteRunConfiguration": SuiteRunConfigurationOutputTypeDef,
         "testResult": TestResultTypeDef,
         "startTime": datetime,
         "endTime": datetime,
         "status": SuiteRunStatusType,
         "errorReason": str,
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor/type_defs.pyi` & `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,17 +25,19 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CreateSuiteDefinitionResponseTypeDef",
     "DeleteSuiteDefinitionRequestRequestTypeDef",
+    "DeviceUnderTestOutputTypeDef",
     "DeviceUnderTestTypeDef",
     "GetEndpointRequestRequestTypeDef",
     "GetEndpointResponseTypeDef",
     "GetSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteRunReportRequestRequestTypeDef",
     "GetSuiteRunReportResponseTypeDef",
     "GetSuiteRunRequestRequestTypeDef",
@@ -47,23 +49,25 @@
     "ResponseMetadataTypeDef",
     "StartSuiteRunResponseTypeDef",
     "StopSuiteRunRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestCaseScenarioTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateSuiteDefinitionResponseTypeDef",
-    "SuiteDefinitionConfigurationTypeDef",
+    "SuiteDefinitionConfigurationOutputTypeDef",
     "SuiteDefinitionInformationTypeDef",
+    "SuiteRunConfigurationOutputTypeDef",
+    "SuiteDefinitionConfigurationTypeDef",
     "SuiteRunConfigurationTypeDef",
     "ListSuiteRunsResponseTypeDef",
     "TestCaseRunTypeDef",
-    "CreateSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteDefinitionResponseTypeDef",
-    "UpdateSuiteDefinitionRequestRequestTypeDef",
     "ListSuiteDefinitionsResponseTypeDef",
+    "CreateSuiteDefinitionRequestRequestTypeDef",
+    "UpdateSuiteDefinitionRequestRequestTypeDef",
     "StartSuiteRunRequestRequestTypeDef",
     "GroupResultTypeDef",
     "TestResultTypeDef",
     "GetSuiteRunResponseTypeDef",
 )
 
 CreateSuiteDefinitionResponseTypeDef = TypedDict(
@@ -80,14 +84,24 @@
 DeleteSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
     },
 )
 
+DeviceUnderTestOutputTypeDef = TypedDict(
+    "DeviceUnderTestOutputTypeDef",
+    {
+        "thingArn": str,
+        "certificateArn": str,
+        "deviceRoleArn": str,
+    },
+    total=False,
+)
+
 DeviceUnderTestTypeDef = TypedDict(
     "DeviceUnderTestTypeDef",
     {
         "thingArn": str,
         "certificateArn": str,
         "deviceRoleArn": str,
     },
@@ -123,20 +137,22 @@
     "_OptionalGetSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionVersion": str,
     },
     total=False,
 )
 
+
 class GetSuiteDefinitionRequestRequestTypeDef(
     _RequiredGetSuiteDefinitionRequestRequestTypeDef,
     _OptionalGetSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 GetSuiteRunReportRequestRequestTypeDef = TypedDict(
     "GetSuiteRunReportRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
@@ -276,72 +292,125 @@
         "suiteDefinitionVersion": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredSuiteDefinitionConfigurationTypeDef = TypedDict(
-    "_RequiredSuiteDefinitionConfigurationTypeDef",
+_RequiredSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSuiteDefinitionConfigurationOutputTypeDef",
     {
         "suiteDefinitionName": str,
         "rootGroup": str,
         "devicePermissionRoleArn": str,
     },
 )
-_OptionalSuiteDefinitionConfigurationTypeDef = TypedDict(
-    "_OptionalSuiteDefinitionConfigurationTypeDef",
+_OptionalSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSuiteDefinitionConfigurationOutputTypeDef",
     {
-        "devices": Sequence[DeviceUnderTestTypeDef],
+        "devices": List[DeviceUnderTestOutputTypeDef],
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
     },
     total=False,
 )
 
-class SuiteDefinitionConfigurationTypeDef(
-    _RequiredSuiteDefinitionConfigurationTypeDef, _OptionalSuiteDefinitionConfigurationTypeDef
+
+class SuiteDefinitionConfigurationOutputTypeDef(
+    _RequiredSuiteDefinitionConfigurationOutputTypeDef,
+    _OptionalSuiteDefinitionConfigurationOutputTypeDef,
 ):
     pass
 
+
 SuiteDefinitionInformationTypeDef = TypedDict(
     "SuiteDefinitionInformationTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionName": str,
-        "defaultDevices": List[DeviceUnderTestTypeDef],
+        "defaultDevices": List[DeviceUnderTestOutputTypeDef],
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
         "createdAt": datetime,
     },
     total=False,
 )
 
+_RequiredSuiteRunConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSuiteRunConfigurationOutputTypeDef",
+    {
+        "primaryDevice": DeviceUnderTestOutputTypeDef,
+    },
+)
+_OptionalSuiteRunConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSuiteRunConfigurationOutputTypeDef",
+    {
+        "selectedTestList": List[str],
+        "parallelRun": bool,
+    },
+    total=False,
+)
+
+
+class SuiteRunConfigurationOutputTypeDef(
+    _RequiredSuiteRunConfigurationOutputTypeDef, _OptionalSuiteRunConfigurationOutputTypeDef
+):
+    pass
+
+
+_RequiredSuiteDefinitionConfigurationTypeDef = TypedDict(
+    "_RequiredSuiteDefinitionConfigurationTypeDef",
+    {
+        "suiteDefinitionName": str,
+        "rootGroup": str,
+        "devicePermissionRoleArn": str,
+    },
+)
+_OptionalSuiteDefinitionConfigurationTypeDef = TypedDict(
+    "_OptionalSuiteDefinitionConfigurationTypeDef",
+    {
+        "devices": Sequence[DeviceUnderTestTypeDef],
+        "intendedForQualification": bool,
+        "isLongDurationTest": bool,
+        "protocol": ProtocolType,
+    },
+    total=False,
+)
+
+
+class SuiteDefinitionConfigurationTypeDef(
+    _RequiredSuiteDefinitionConfigurationTypeDef, _OptionalSuiteDefinitionConfigurationTypeDef
+):
+    pass
+
+
 _RequiredSuiteRunConfigurationTypeDef = TypedDict(
     "_RequiredSuiteRunConfigurationTypeDef",
     {
         "primaryDevice": DeviceUnderTestTypeDef,
     },
 )
 _OptionalSuiteRunConfigurationTypeDef = TypedDict(
     "_OptionalSuiteRunConfigurationTypeDef",
     {
-        "selectedTestList": List[str],
+        "selectedTestList": Sequence[str],
         "parallelRun": bool,
     },
     total=False,
 )
 
+
 class SuiteRunConfigurationTypeDef(
     _RequiredSuiteRunConfigurationTypeDef, _OptionalSuiteRunConfigurationTypeDef
 ):
     pass
 
+
 ListSuiteRunsResponseTypeDef = TypedDict(
     "ListSuiteRunsResponseTypeDef",
     {
         "suiteRunsList": List[SuiteRunInformationTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -360,66 +429,68 @@
         "warnings": str,
         "failure": str,
         "testScenarios": List[TestCaseScenarioTypeDef],
     },
     total=False,
 )
 
+GetSuiteDefinitionResponseTypeDef = TypedDict(
+    "GetSuiteDefinitionResponseTypeDef",
+    {
+        "suiteDefinitionId": str,
+        "suiteDefinitionArn": str,
+        "suiteDefinitionVersion": str,
+        "latestVersion": str,
+        "suiteDefinitionConfiguration": SuiteDefinitionConfigurationOutputTypeDef,
+        "createdAt": datetime,
+        "lastModifiedAt": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListSuiteDefinitionsResponseTypeDef = TypedDict(
+    "ListSuiteDefinitionsResponseTypeDef",
+    {
+        "suiteDefinitionInformationList": List[SuiteDefinitionInformationTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
 _OptionalCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateSuiteDefinitionRequestRequestTypeDef(
     _RequiredCreateSuiteDefinitionRequestRequestTypeDef,
     _OptionalCreateSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
-GetSuiteDefinitionResponseTypeDef = TypedDict(
-    "GetSuiteDefinitionResponseTypeDef",
-    {
-        "suiteDefinitionId": str,
-        "suiteDefinitionArn": str,
-        "suiteDefinitionVersion": str,
-        "latestVersion": str,
-        "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
-        "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UpdateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
 
-ListSuiteDefinitionsResponseTypeDef = TypedDict(
-    "ListSuiteDefinitionsResponseTypeDef",
-    {
-        "suiteDefinitionInformationList": List[SuiteDefinitionInformationTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartSuiteRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunConfiguration": SuiteRunConfigurationTypeDef,
     },
 )
@@ -428,19 +499,21 @@
     {
         "suiteDefinitionVersion": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartSuiteRunRequestRequestTypeDef(
     _RequiredStartSuiteRunRequestRequestTypeDef, _OptionalStartSuiteRunRequestRequestTypeDef
 ):
     pass
 
+
 GroupResultTypeDef = TypedDict(
     "GroupResultTypeDef",
     {
         "groupId": str,
         "groupName": str,
         "tests": List[TestCaseRunTypeDef],
     },
@@ -458,15 +531,15 @@
 GetSuiteRunResponseTypeDef = TypedDict(
     "GetSuiteRunResponseTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionVersion": str,
         "suiteRunId": str,
         "suiteRunArn": str,
-        "suiteRunConfiguration": SuiteRunConfigurationTypeDef,
+        "suiteRunConfiguration": SuiteRunConfigurationOutputTypeDef,
         "testResult": TestResultTypeDef,
         "startTime": datetime,
         "endTime": datetime,
         "status": SuiteRunStatusType,
         "errorReason": str,
         "tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO` & `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotdeviceadvisor
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotdeviceadvisor"></a>
 
 # mypy-boto3-iotdeviceadvisor
 
 [![PyPI - mypy-boto3-iotdeviceadvisor](https://img.shields.io/pypi/v/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotdeviceadvisor?color=blue)](https://pypistats.org/packages/mypy-boto3-iotdeviceadvisor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotdeviceadvisor)](https://pepy.tech/project/mypy-boto3-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDeviceAdvisor 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[boto3.IoTDeviceAdvisor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,14 +305,15 @@
 `mypy_boto3_iotdeviceadvisor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotdeviceadvisor.type_defs import (
     CreateSuiteDefinitionResponseTypeDef,
     DeleteSuiteDefinitionRequestRequestTypeDef,
+    DeviceUnderTestOutputTypeDef,
     DeviceUnderTestTypeDef,
     GetEndpointRequestRequestTypeDef,
     GetEndpointResponseTypeDef,
     GetSuiteDefinitionRequestRequestTypeDef,
     GetSuiteRunReportRequestRequestTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunRequestRequestTypeDef,
@@ -324,23 +325,25 @@
     ResponseMetadataTypeDef,
     StartSuiteRunResponseTypeDef,
     StopSuiteRunRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestCaseScenarioTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
+    SuiteDefinitionConfigurationOutputTypeDef,
     SuiteDefinitionInformationTypeDef,
+    SuiteRunConfigurationOutputTypeDef,
+    SuiteDefinitionConfigurationTypeDef,
     SuiteRunConfigurationTypeDef,
     ListSuiteRunsResponseTypeDef,
     TestCaseRunTypeDef,
-    CreateSuiteDefinitionRequestRequestTypeDef,
     GetSuiteDefinitionResponseTypeDef,
-    UpdateSuiteDefinitionRequestRequestTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
+    CreateSuiteDefinitionRequestRequestTypeDef,
+    UpdateSuiteDefinitionRequestRequestTypeDef,
     StartSuiteRunRequestRequestTypeDef,
     GroupResultTypeDef,
     TestResultTypeDef,
     GetSuiteRunResponseTypeDef,
 )
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt` & `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.0/setup.py` & `mypy-boto3-iotdeviceadvisor-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotdeviceadvisor",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iotdeviceadvisor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTDeviceAdvisor 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.IoTDeviceAdvisor 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

