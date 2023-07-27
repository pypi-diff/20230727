# Comparing `tmp/mypy-boto3-braket-1.28.0.tar.gz` & `tmp/mypy-boto3-braket-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-braket-1.28.0.tar", last modified: Thu Jul  6 20:59:05 2023, max compression
+gzip compressed data, was "mypy-boto3-braket-1.28.12.tar", last modified: Thu Jul 27 05:34:22 2023, max compression
```

## Comparing `mypy-boto3-braket-1.28.0.tar` & `mypy-boto3-braket-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.422234 mypy-boto3-braket-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:19.000000 mypy-boto3-braket-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14628 2023-07-06 20:59:05.422234 mypy-boto3-braket-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-07-06 20:34:19.000000 mypy-boto3-braket-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.414234 mypy-boto3-braket-1.28.0/mypy_boto3_braket/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-06 20:34:19.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-06 20:34:19.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-06 20:34:19.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-07-06 20:34:19.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-06 20:34:19.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-06 20:34:20.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-06 20:34:20.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-06 20:34:19.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-06 20:34:19.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:19.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17665 2023-07-06 20:34:20.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17634 2023-07-06 20:34:20.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:19.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.422234 mypy-boto3-braket-1.28.0/mypy_boto3_braket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14628 2023-07-06 20:59:05.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 20:59:05.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:05.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 20:59:05.000000 mypy-boto3-braket-1.28.0/mypy_boto3_braket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:05.422234 mypy-boto3-braket-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:34:19.000000 mypy-boto3-braket-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.772567 mypy-boto3-braket-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-07-27 05:34:22.772567 mypy-boto3-braket-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.772567 mypy-boto3-braket-1.28.12/mypy_boto3_braket/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-07-27 05:18:02.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.772567 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-07-27 05:34:22.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:22.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:22.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:22.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:22.772567 mypy-boto3-braket-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/setup.py
```

### Comparing `mypy-boto3-braket-1.28.0/LICENSE` & `mypy-boto3-braket-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.0/PKG-INFO` & `mypy-boto3-braket-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-braket
-Version: 1.28.0
-Summary: Type annotations for boto3.Braket 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Braket 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-braket"></a>
 
 # mypy-boto3-braket
 
 [![PyPI - mypy-boto3-braket](https://img.shields.io/pypi/v/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-braket?color=blue)](https://pypistats.org/packages/mypy-boto3-braket)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-braket)](https://pepy.tech/project/mypy-boto3-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Braket 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[boto3.Braket 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [mypy-boto3-braket docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,65 +338,76 @@
 ### Typed dictionaries
 
 `mypy_boto3_braket.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_braket.type_defs import (
+    ContainerImageOutputTypeDef,
+    ScriptModeConfigOutputTypeDef,
     ContainerImageTypeDef,
     ScriptModeConfigTypeDef,
     CancelJobRequestRequestTypeDef,
     CancelJobResponseTypeDef,
     CancelQuantumTaskRequestRequestTypeDef,
     CancelQuantumTaskResponseTypeDef,
     DeviceConfigTypeDef,
     InstanceConfigTypeDef,
     JobCheckpointConfigTypeDef,
     JobOutputDataConfigTypeDef,
     JobStoppingConditionTypeDef,
     CreateJobResponseTypeDef,
     CreateQuantumTaskRequestRequestTypeDef,
     CreateQuantumTaskResponseTypeDef,
+    S3DataSourceOutputTypeDef,
     S3DataSourceTypeDef,
+    DeviceConfigOutputTypeDef,
     DeviceSummaryTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetDeviceResponseTypeDef,
     GetJobRequestRequestTypeDef,
+    InstanceConfigOutputTypeDef,
+    JobCheckpointConfigOutputTypeDef,
     JobEventDetailsTypeDef,
+    JobOutputDataConfigOutputTypeDef,
+    JobStoppingConditionOutputTypeDef,
     GetQuantumTaskRequestRequestTypeDef,
     GetQuantumTaskResponseTypeDef,
     JobSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QuantumTaskSummaryTypeDef,
     ResponseMetadataTypeDef,
     SearchDevicesFilterTypeDef,
     SearchJobsFilterTypeDef,
     SearchQuantumTasksFilterTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AlgorithmSpecificationOutputTypeDef,
     AlgorithmSpecificationTypeDef,
+    DataSourceOutputTypeDef,
     DataSourceTypeDef,
     SearchDevicesResponseTypeDef,
     SearchJobsResponseTypeDef,
     SearchQuantumTasksResponseTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchJobsRequestRequestTypeDef,
     SearchJobsRequestSearchJobsPaginateTypeDef,
     SearchQuantumTasksRequestRequestTypeDef,
     SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
+    InputFileConfigOutputTypeDef,
     InputFileConfigTypeDef,
-    CreateJobRequestRequestTypeDef,
     GetJobResponseTypeDef,
+    CreateJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ContainerImageTypeDef:
+def get_structure() -> ContainerImageOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-braket-1.28.0/README.md` & `mypy-boto3-braket-1.28.12/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-braket"></a>
 
 # mypy-boto3-braket
 
 [![PyPI - mypy-boto3-braket](https://img.shields.io/pypi/v/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-braket?color=blue)](https://pypistats.org/packages/mypy-boto3-braket)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-braket)](https://pepy.tech/project/mypy-boto3-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Braket 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[boto3.Braket 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [mypy-boto3-braket docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,65 +306,76 @@
 ### Typed dictionaries
 
 `mypy_boto3_braket.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_braket.type_defs import (
+    ContainerImageOutputTypeDef,
+    ScriptModeConfigOutputTypeDef,
     ContainerImageTypeDef,
     ScriptModeConfigTypeDef,
     CancelJobRequestRequestTypeDef,
     CancelJobResponseTypeDef,
     CancelQuantumTaskRequestRequestTypeDef,
     CancelQuantumTaskResponseTypeDef,
     DeviceConfigTypeDef,
     InstanceConfigTypeDef,
     JobCheckpointConfigTypeDef,
     JobOutputDataConfigTypeDef,
     JobStoppingConditionTypeDef,
     CreateJobResponseTypeDef,
     CreateQuantumTaskRequestRequestTypeDef,
     CreateQuantumTaskResponseTypeDef,
+    S3DataSourceOutputTypeDef,
     S3DataSourceTypeDef,
+    DeviceConfigOutputTypeDef,
     DeviceSummaryTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetDeviceResponseTypeDef,
     GetJobRequestRequestTypeDef,
+    InstanceConfigOutputTypeDef,
+    JobCheckpointConfigOutputTypeDef,
     JobEventDetailsTypeDef,
+    JobOutputDataConfigOutputTypeDef,
+    JobStoppingConditionOutputTypeDef,
     GetQuantumTaskRequestRequestTypeDef,
     GetQuantumTaskResponseTypeDef,
     JobSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QuantumTaskSummaryTypeDef,
     ResponseMetadataTypeDef,
     SearchDevicesFilterTypeDef,
     SearchJobsFilterTypeDef,
     SearchQuantumTasksFilterTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AlgorithmSpecificationOutputTypeDef,
     AlgorithmSpecificationTypeDef,
+    DataSourceOutputTypeDef,
     DataSourceTypeDef,
     SearchDevicesResponseTypeDef,
     SearchJobsResponseTypeDef,
     SearchQuantumTasksResponseTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchJobsRequestRequestTypeDef,
     SearchJobsRequestSearchJobsPaginateTypeDef,
     SearchQuantumTasksRequestRequestTypeDef,
     SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
+    InputFileConfigOutputTypeDef,
     InputFileConfigTypeDef,
-    CreateJobRequestRequestTypeDef,
     GetJobResponseTypeDef,
+    CreateJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ContainerImageTypeDef:
+def get_structure() -> ContainerImageOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket/__init__.py` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket/__init__.pyi` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket/__main__.py` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Braket 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Braket 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket\nOther"
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

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket/client.py` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket/client.pyi` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket/literals.py` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,15 @@
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
@@ -312,26 +313,28 @@
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

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket/literals.pyi` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,15 @@
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
@@ -310,26 +311,28 @@
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

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket/paginator.py` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket/paginator.pyi` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket/type_defs.py` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for braket service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_braket.type_defs import ContainerImageTypeDef
+    from mypy_boto3_braket.type_defs import ContainerImageOutputTypeDef
 
-    data: ContainerImageTypeDef = {...}
+    data: ContainerImageOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -29,64 +29,101 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "ContainerImageOutputTypeDef",
+    "ScriptModeConfigOutputTypeDef",
     "ContainerImageTypeDef",
     "ScriptModeConfigTypeDef",
     "CancelJobRequestRequestTypeDef",
     "CancelJobResponseTypeDef",
     "CancelQuantumTaskRequestRequestTypeDef",
     "CancelQuantumTaskResponseTypeDef",
     "DeviceConfigTypeDef",
     "InstanceConfigTypeDef",
     "JobCheckpointConfigTypeDef",
     "JobOutputDataConfigTypeDef",
     "JobStoppingConditionTypeDef",
     "CreateJobResponseTypeDef",
     "CreateQuantumTaskRequestRequestTypeDef",
     "CreateQuantumTaskResponseTypeDef",
+    "S3DataSourceOutputTypeDef",
     "S3DataSourceTypeDef",
+    "DeviceConfigOutputTypeDef",
     "DeviceSummaryTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetDeviceResponseTypeDef",
     "GetJobRequestRequestTypeDef",
+    "InstanceConfigOutputTypeDef",
+    "JobCheckpointConfigOutputTypeDef",
     "JobEventDetailsTypeDef",
+    "JobOutputDataConfigOutputTypeDef",
+    "JobStoppingConditionOutputTypeDef",
     "GetQuantumTaskRequestRequestTypeDef",
     "GetQuantumTaskResponseTypeDef",
     "JobSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "QuantumTaskSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "SearchDevicesFilterTypeDef",
     "SearchJobsFilterTypeDef",
     "SearchQuantumTasksFilterTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AlgorithmSpecificationOutputTypeDef",
     "AlgorithmSpecificationTypeDef",
+    "DataSourceOutputTypeDef",
     "DataSourceTypeDef",
     "SearchDevicesResponseTypeDef",
     "SearchJobsResponseTypeDef",
     "SearchQuantumTasksResponseTypeDef",
     "SearchDevicesRequestRequestTypeDef",
     "SearchDevicesRequestSearchDevicesPaginateTypeDef",
     "SearchJobsRequestRequestTypeDef",
     "SearchJobsRequestSearchJobsPaginateTypeDef",
     "SearchQuantumTasksRequestRequestTypeDef",
     "SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
+    "InputFileConfigOutputTypeDef",
     "InputFileConfigTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "GetJobResponseTypeDef",
+    "CreateJobRequestRequestTypeDef",
+)
+
+ContainerImageOutputTypeDef = TypedDict(
+    "ContainerImageOutputTypeDef",
+    {
+        "uri": str,
+    },
+)
+
+_RequiredScriptModeConfigOutputTypeDef = TypedDict(
+    "_RequiredScriptModeConfigOutputTypeDef",
+    {
+        "entryPoint": str,
+        "s3Uri": str,
+    },
 )
+_OptionalScriptModeConfigOutputTypeDef = TypedDict(
+    "_OptionalScriptModeConfigOutputTypeDef",
+    {
+        "compressionType": CompressionTypeType,
+    },
+    total=False,
+)
+
+class ScriptModeConfigOutputTypeDef(
+    _RequiredScriptModeConfigOutputTypeDef, _OptionalScriptModeConfigOutputTypeDef
+):
+    pass
 
 ContainerImageTypeDef = TypedDict(
     "ContainerImageTypeDef",
     {
         "uri": str,
     },
 )
@@ -102,19 +139,17 @@
     "_OptionalScriptModeConfigTypeDef",
     {
         "compressionType": CompressionTypeType,
     },
     total=False,
 )
 
-
 class ScriptModeConfigTypeDef(_RequiredScriptModeConfigTypeDef, _OptionalScriptModeConfigTypeDef):
     pass
 
-
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
@@ -162,61 +197,55 @@
     "_OptionalInstanceConfigTypeDef",
     {
         "instanceCount": int,
     },
     total=False,
 )
 
-
 class InstanceConfigTypeDef(_RequiredInstanceConfigTypeDef, _OptionalInstanceConfigTypeDef):
     pass
 
-
 _RequiredJobCheckpointConfigTypeDef = TypedDict(
     "_RequiredJobCheckpointConfigTypeDef",
     {
         "s3Uri": str,
     },
 )
 _OptionalJobCheckpointConfigTypeDef = TypedDict(
     "_OptionalJobCheckpointConfigTypeDef",
     {
         "localPath": str,
     },
     total=False,
 )
 
-
 class JobCheckpointConfigTypeDef(
     _RequiredJobCheckpointConfigTypeDef, _OptionalJobCheckpointConfigTypeDef
 ):
     pass
 
-
 _RequiredJobOutputDataConfigTypeDef = TypedDict(
     "_RequiredJobOutputDataConfigTypeDef",
     {
         "s3Path": str,
     },
 )
 _OptionalJobOutputDataConfigTypeDef = TypedDict(
     "_OptionalJobOutputDataConfigTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
 
-
 class JobOutputDataConfigTypeDef(
     _RequiredJobOutputDataConfigTypeDef, _OptionalJobOutputDataConfigTypeDef
 ):
     pass
 
-
 JobStoppingConditionTypeDef = TypedDict(
     "JobStoppingConditionTypeDef",
     {
         "maxRuntimeInSeconds": int,
     },
     total=False,
 )
@@ -246,36 +275,48 @@
         "deviceParameters": str,
         "jobToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateQuantumTaskRequestRequestTypeDef(
     _RequiredCreateQuantumTaskRequestRequestTypeDef, _OptionalCreateQuantumTaskRequestRequestTypeDef
 ):
     pass
 
-
 CreateQuantumTaskResponseTypeDef = TypedDict(
     "CreateQuantumTaskResponseTypeDef",
     {
         "quantumTaskArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+S3DataSourceOutputTypeDef = TypedDict(
+    "S3DataSourceOutputTypeDef",
+    {
+        "s3Uri": str,
+    },
+)
+
 S3DataSourceTypeDef = TypedDict(
     "S3DataSourceTypeDef",
     {
         "s3Uri": str,
     },
 )
 
+DeviceConfigOutputTypeDef = TypedDict(
+    "DeviceConfigOutputTypeDef",
+    {
+        "device": str,
+    },
+)
+
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "deviceArn": str,
         "deviceName": str,
         "deviceStatus": DeviceStatusType,
         "deviceType": DeviceTypeType,
@@ -306,24 +347,90 @@
 GetJobRequestRequestTypeDef = TypedDict(
     "GetJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
+_RequiredInstanceConfigOutputTypeDef = TypedDict(
+    "_RequiredInstanceConfigOutputTypeDef",
+    {
+        "instanceType": InstanceTypeType,
+        "volumeSizeInGb": int,
+    },
+)
+_OptionalInstanceConfigOutputTypeDef = TypedDict(
+    "_OptionalInstanceConfigOutputTypeDef",
+    {
+        "instanceCount": int,
+    },
+    total=False,
+)
+
+class InstanceConfigOutputTypeDef(
+    _RequiredInstanceConfigOutputTypeDef, _OptionalInstanceConfigOutputTypeDef
+):
+    pass
+
+_RequiredJobCheckpointConfigOutputTypeDef = TypedDict(
+    "_RequiredJobCheckpointConfigOutputTypeDef",
+    {
+        "s3Uri": str,
+    },
+)
+_OptionalJobCheckpointConfigOutputTypeDef = TypedDict(
+    "_OptionalJobCheckpointConfigOutputTypeDef",
+    {
+        "localPath": str,
+    },
+    total=False,
+)
+
+class JobCheckpointConfigOutputTypeDef(
+    _RequiredJobCheckpointConfigOutputTypeDef, _OptionalJobCheckpointConfigOutputTypeDef
+):
+    pass
+
 JobEventDetailsTypeDef = TypedDict(
     "JobEventDetailsTypeDef",
     {
         "eventType": JobEventTypeType,
         "message": str,
         "timeOfEvent": datetime,
     },
     total=False,
 )
 
+_RequiredJobOutputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredJobOutputDataConfigOutputTypeDef",
+    {
+        "s3Path": str,
+    },
+)
+_OptionalJobOutputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalJobOutputDataConfigOutputTypeDef",
+    {
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+class JobOutputDataConfigOutputTypeDef(
+    _RequiredJobOutputDataConfigOutputTypeDef, _OptionalJobOutputDataConfigOutputTypeDef
+):
+    pass
+
+JobStoppingConditionOutputTypeDef = TypedDict(
+    "JobStoppingConditionOutputTypeDef",
+    {
+        "maxRuntimeInSeconds": int,
+    },
+    total=False,
+)
+
 GetQuantumTaskRequestRequestTypeDef = TypedDict(
     "GetQuantumTaskRequestRequestTypeDef",
     {
         "quantumTaskArn": str,
     },
 )
 
@@ -362,19 +469,17 @@
         "endedAt": datetime,
         "startedAt": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class JobSummaryTypeDef(_RequiredJobSummaryTypeDef, _OptionalJobSummaryTypeDef):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -413,21 +518,19 @@
     {
         "endedAt": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class QuantumTaskSummaryTypeDef(
     _RequiredQuantumTaskSummaryTypeDef, _OptionalQuantumTaskSummaryTypeDef
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -473,23 +576,39 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+AlgorithmSpecificationOutputTypeDef = TypedDict(
+    "AlgorithmSpecificationOutputTypeDef",
+    {
+        "containerImage": ContainerImageOutputTypeDef,
+        "scriptModeConfig": ScriptModeConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 AlgorithmSpecificationTypeDef = TypedDict(
     "AlgorithmSpecificationTypeDef",
     {
         "containerImage": ContainerImageTypeDef,
         "scriptModeConfig": ScriptModeConfigTypeDef,
     },
     total=False,
 )
 
+DataSourceOutputTypeDef = TypedDict(
+    "DataSourceOutputTypeDef",
+    {
+        "s3DataSource": S3DataSourceOutputTypeDef,
+    },
+)
+
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "s3DataSource": S3DataSourceTypeDef,
     },
 )
 
@@ -531,43 +650,39 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class SearchDevicesRequestRequestTypeDef(
     _RequiredSearchDevicesRequestRequestTypeDef, _OptionalSearchDevicesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef = TypedDict(
     "_RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef",
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
     },
 )
 _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef = TypedDict(
     "_OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchDevicesRequestSearchDevicesPaginateTypeDef(
     _RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef,
     _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchJobsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchJobsRequestRequestTypeDef",
     {
         "filters": Sequence[SearchJobsFilterTypeDef],
     },
 )
 _OptionalSearchJobsRequestRequestTypeDef = TypedDict(
@@ -575,43 +690,39 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class SearchJobsRequestRequestTypeDef(
     _RequiredSearchJobsRequestRequestTypeDef, _OptionalSearchJobsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchJobsRequestSearchJobsPaginateTypeDef = TypedDict(
     "_RequiredSearchJobsRequestSearchJobsPaginateTypeDef",
     {
         "filters": Sequence[SearchJobsFilterTypeDef],
     },
 )
 _OptionalSearchJobsRequestSearchJobsPaginateTypeDef = TypedDict(
     "_OptionalSearchJobsRequestSearchJobsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchJobsRequestSearchJobsPaginateTypeDef(
     _RequiredSearchJobsRequestSearchJobsPaginateTypeDef,
     _OptionalSearchJobsRequestSearchJobsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredSearchQuantumTasksRequestRequestTypeDef = TypedDict(
     "_RequiredSearchQuantumTasksRequestRequestTypeDef",
     {
         "filters": Sequence[SearchQuantumTasksFilterTypeDef],
     },
 )
 _OptionalSearchQuantumTasksRequestRequestTypeDef = TypedDict(
@@ -619,43 +730,59 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class SearchQuantumTasksRequestRequestTypeDef(
     _RequiredSearchQuantumTasksRequestRequestTypeDef,
     _OptionalSearchQuantumTasksRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef = TypedDict(
     "_RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
     {
         "filters": Sequence[SearchQuantumTasksFilterTypeDef],
     },
 )
 _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef = TypedDict(
     "_OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef(
     _RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
     _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
 ):
     pass
 
+_RequiredInputFileConfigOutputTypeDef = TypedDict(
+    "_RequiredInputFileConfigOutputTypeDef",
+    {
+        "channelName": str,
+        "dataSource": DataSourceOutputTypeDef,
+    },
+)
+_OptionalInputFileConfigOutputTypeDef = TypedDict(
+    "_OptionalInputFileConfigOutputTypeDef",
+    {
+        "contentType": str,
+    },
+    total=False,
+)
+
+class InputFileConfigOutputTypeDef(
+    _RequiredInputFileConfigOutputTypeDef, _OptionalInputFileConfigOutputTypeDef
+):
+    pass
 
 _RequiredInputFileConfigTypeDef = TypedDict(
     "_RequiredInputFileConfigTypeDef",
     {
         "channelName": str,
         "dataSource": DataSourceTypeDef,
     },
@@ -664,18 +791,42 @@
     "_OptionalInputFileConfigTypeDef",
     {
         "contentType": str,
     },
     total=False,
 )
 
-
 class InputFileConfigTypeDef(_RequiredInputFileConfigTypeDef, _OptionalInputFileConfigTypeDef):
     pass
 
+GetJobResponseTypeDef = TypedDict(
+    "GetJobResponseTypeDef",
+    {
+        "algorithmSpecification": AlgorithmSpecificationOutputTypeDef,
+        "billableDuration": int,
+        "checkpointConfig": JobCheckpointConfigOutputTypeDef,
+        "createdAt": datetime,
+        "deviceConfig": DeviceConfigOutputTypeDef,
+        "endedAt": datetime,
+        "events": List[JobEventDetailsTypeDef],
+        "failureReason": str,
+        "hyperParameters": Dict[str, str],
+        "inputDataConfig": List[InputFileConfigOutputTypeDef],
+        "instanceConfig": InstanceConfigOutputTypeDef,
+        "jobArn": str,
+        "jobName": str,
+        "outputDataConfig": JobOutputDataConfigOutputTypeDef,
+        "roleArn": str,
+        "startedAt": datetime,
+        "status": JobPrimaryStatusType,
+        "stoppingCondition": JobStoppingConditionOutputTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "algorithmSpecification": AlgorithmSpecificationTypeDef,
         "clientToken": str,
         "deviceConfig": DeviceConfigTypeDef,
@@ -693,39 +844,11 @@
         "inputDataConfig": Sequence[InputFileConfigTypeDef],
         "stoppingCondition": JobStoppingConditionTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
-
-
-GetJobResponseTypeDef = TypedDict(
-    "GetJobResponseTypeDef",
-    {
-        "algorithmSpecification": AlgorithmSpecificationTypeDef,
-        "billableDuration": int,
-        "checkpointConfig": JobCheckpointConfigTypeDef,
-        "createdAt": datetime,
-        "deviceConfig": DeviceConfigTypeDef,
-        "endedAt": datetime,
-        "events": List[JobEventDetailsTypeDef],
-        "failureReason": str,
-        "hyperParameters": Dict[str, str],
-        "inputDataConfig": List[InputFileConfigTypeDef],
-        "instanceConfig": InstanceConfigTypeDef,
-        "jobArn": str,
-        "jobName": str,
-        "outputDataConfig": JobOutputDataConfigTypeDef,
-        "roleArn": str,
-        "startedAt": datetime,
-        "status": JobPrimaryStatusType,
-        "stoppingCondition": JobStoppingConditionTypeDef,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket/type_defs.pyi` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for braket service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_braket.type_defs import ContainerImageTypeDef
+    from mypy_boto3_braket.type_defs import ContainerImageOutputTypeDef
 
-    data: ContainerImageTypeDef = {...}
+    data: ContainerImageOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -29,64 +29,105 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "ContainerImageOutputTypeDef",
+    "ScriptModeConfigOutputTypeDef",
     "ContainerImageTypeDef",
     "ScriptModeConfigTypeDef",
     "CancelJobRequestRequestTypeDef",
     "CancelJobResponseTypeDef",
     "CancelQuantumTaskRequestRequestTypeDef",
     "CancelQuantumTaskResponseTypeDef",
     "DeviceConfigTypeDef",
     "InstanceConfigTypeDef",
     "JobCheckpointConfigTypeDef",
     "JobOutputDataConfigTypeDef",
     "JobStoppingConditionTypeDef",
     "CreateJobResponseTypeDef",
     "CreateQuantumTaskRequestRequestTypeDef",
     "CreateQuantumTaskResponseTypeDef",
+    "S3DataSourceOutputTypeDef",
     "S3DataSourceTypeDef",
+    "DeviceConfigOutputTypeDef",
     "DeviceSummaryTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetDeviceResponseTypeDef",
     "GetJobRequestRequestTypeDef",
+    "InstanceConfigOutputTypeDef",
+    "JobCheckpointConfigOutputTypeDef",
     "JobEventDetailsTypeDef",
+    "JobOutputDataConfigOutputTypeDef",
+    "JobStoppingConditionOutputTypeDef",
     "GetQuantumTaskRequestRequestTypeDef",
     "GetQuantumTaskResponseTypeDef",
     "JobSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "QuantumTaskSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "SearchDevicesFilterTypeDef",
     "SearchJobsFilterTypeDef",
     "SearchQuantumTasksFilterTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AlgorithmSpecificationOutputTypeDef",
     "AlgorithmSpecificationTypeDef",
+    "DataSourceOutputTypeDef",
     "DataSourceTypeDef",
     "SearchDevicesResponseTypeDef",
     "SearchJobsResponseTypeDef",
     "SearchQuantumTasksResponseTypeDef",
     "SearchDevicesRequestRequestTypeDef",
     "SearchDevicesRequestSearchDevicesPaginateTypeDef",
     "SearchJobsRequestRequestTypeDef",
     "SearchJobsRequestSearchJobsPaginateTypeDef",
     "SearchQuantumTasksRequestRequestTypeDef",
     "SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
+    "InputFileConfigOutputTypeDef",
     "InputFileConfigTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "GetJobResponseTypeDef",
+    "CreateJobRequestRequestTypeDef",
+)
+
+ContainerImageOutputTypeDef = TypedDict(
+    "ContainerImageOutputTypeDef",
+    {
+        "uri": str,
+    },
 )
 
+_RequiredScriptModeConfigOutputTypeDef = TypedDict(
+    "_RequiredScriptModeConfigOutputTypeDef",
+    {
+        "entryPoint": str,
+        "s3Uri": str,
+    },
+)
+_OptionalScriptModeConfigOutputTypeDef = TypedDict(
+    "_OptionalScriptModeConfigOutputTypeDef",
+    {
+        "compressionType": CompressionTypeType,
+    },
+    total=False,
+)
+
+
+class ScriptModeConfigOutputTypeDef(
+    _RequiredScriptModeConfigOutputTypeDef, _OptionalScriptModeConfigOutputTypeDef
+):
+    pass
+
+
 ContainerImageTypeDef = TypedDict(
     "ContainerImageTypeDef",
     {
         "uri": str,
     },
 )
 
@@ -101,17 +142,19 @@
     "_OptionalScriptModeConfigTypeDef",
     {
         "compressionType": CompressionTypeType,
     },
     total=False,
 )
 
+
 class ScriptModeConfigTypeDef(_RequiredScriptModeConfigTypeDef, _OptionalScriptModeConfigTypeDef):
     pass
 
+
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
@@ -159,55 +202,61 @@
     "_OptionalInstanceConfigTypeDef",
     {
         "instanceCount": int,
     },
     total=False,
 )
 
+
 class InstanceConfigTypeDef(_RequiredInstanceConfigTypeDef, _OptionalInstanceConfigTypeDef):
     pass
 
+
 _RequiredJobCheckpointConfigTypeDef = TypedDict(
     "_RequiredJobCheckpointConfigTypeDef",
     {
         "s3Uri": str,
     },
 )
 _OptionalJobCheckpointConfigTypeDef = TypedDict(
     "_OptionalJobCheckpointConfigTypeDef",
     {
         "localPath": str,
     },
     total=False,
 )
 
+
 class JobCheckpointConfigTypeDef(
     _RequiredJobCheckpointConfigTypeDef, _OptionalJobCheckpointConfigTypeDef
 ):
     pass
 
+
 _RequiredJobOutputDataConfigTypeDef = TypedDict(
     "_RequiredJobOutputDataConfigTypeDef",
     {
         "s3Path": str,
     },
 )
 _OptionalJobOutputDataConfigTypeDef = TypedDict(
     "_OptionalJobOutputDataConfigTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
 
+
 class JobOutputDataConfigTypeDef(
     _RequiredJobOutputDataConfigTypeDef, _OptionalJobOutputDataConfigTypeDef
 ):
     pass
 
+
 JobStoppingConditionTypeDef = TypedDict(
     "JobStoppingConditionTypeDef",
     {
         "maxRuntimeInSeconds": int,
     },
     total=False,
 )
@@ -237,34 +286,50 @@
         "deviceParameters": str,
         "jobToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateQuantumTaskRequestRequestTypeDef(
     _RequiredCreateQuantumTaskRequestRequestTypeDef, _OptionalCreateQuantumTaskRequestRequestTypeDef
 ):
     pass
 
+
 CreateQuantumTaskResponseTypeDef = TypedDict(
     "CreateQuantumTaskResponseTypeDef",
     {
         "quantumTaskArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+S3DataSourceOutputTypeDef = TypedDict(
+    "S3DataSourceOutputTypeDef",
+    {
+        "s3Uri": str,
+    },
+)
+
 S3DataSourceTypeDef = TypedDict(
     "S3DataSourceTypeDef",
     {
         "s3Uri": str,
     },
 )
 
+DeviceConfigOutputTypeDef = TypedDict(
+    "DeviceConfigOutputTypeDef",
+    {
+        "device": str,
+    },
+)
+
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "deviceArn": str,
         "deviceName": str,
         "deviceStatus": DeviceStatusType,
         "deviceType": DeviceTypeType,
@@ -295,24 +360,96 @@
 GetJobRequestRequestTypeDef = TypedDict(
     "GetJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
+_RequiredInstanceConfigOutputTypeDef = TypedDict(
+    "_RequiredInstanceConfigOutputTypeDef",
+    {
+        "instanceType": InstanceTypeType,
+        "volumeSizeInGb": int,
+    },
+)
+_OptionalInstanceConfigOutputTypeDef = TypedDict(
+    "_OptionalInstanceConfigOutputTypeDef",
+    {
+        "instanceCount": int,
+    },
+    total=False,
+)
+
+
+class InstanceConfigOutputTypeDef(
+    _RequiredInstanceConfigOutputTypeDef, _OptionalInstanceConfigOutputTypeDef
+):
+    pass
+
+
+_RequiredJobCheckpointConfigOutputTypeDef = TypedDict(
+    "_RequiredJobCheckpointConfigOutputTypeDef",
+    {
+        "s3Uri": str,
+    },
+)
+_OptionalJobCheckpointConfigOutputTypeDef = TypedDict(
+    "_OptionalJobCheckpointConfigOutputTypeDef",
+    {
+        "localPath": str,
+    },
+    total=False,
+)
+
+
+class JobCheckpointConfigOutputTypeDef(
+    _RequiredJobCheckpointConfigOutputTypeDef, _OptionalJobCheckpointConfigOutputTypeDef
+):
+    pass
+
+
 JobEventDetailsTypeDef = TypedDict(
     "JobEventDetailsTypeDef",
     {
         "eventType": JobEventTypeType,
         "message": str,
         "timeOfEvent": datetime,
     },
     total=False,
 )
 
+_RequiredJobOutputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredJobOutputDataConfigOutputTypeDef",
+    {
+        "s3Path": str,
+    },
+)
+_OptionalJobOutputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalJobOutputDataConfigOutputTypeDef",
+    {
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class JobOutputDataConfigOutputTypeDef(
+    _RequiredJobOutputDataConfigOutputTypeDef, _OptionalJobOutputDataConfigOutputTypeDef
+):
+    pass
+
+
+JobStoppingConditionOutputTypeDef = TypedDict(
+    "JobStoppingConditionOutputTypeDef",
+    {
+        "maxRuntimeInSeconds": int,
+    },
+    total=False,
+)
+
 GetQuantumTaskRequestRequestTypeDef = TypedDict(
     "GetQuantumTaskRequestRequestTypeDef",
     {
         "quantumTaskArn": str,
     },
 )
 
@@ -351,17 +488,19 @@
         "endedAt": datetime,
         "startedAt": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class JobSummaryTypeDef(_RequiredJobSummaryTypeDef, _OptionalJobSummaryTypeDef):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -400,19 +539,21 @@
     {
         "endedAt": datetime,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class QuantumTaskSummaryTypeDef(
     _RequiredQuantumTaskSummaryTypeDef, _OptionalQuantumTaskSummaryTypeDef
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -458,23 +599,39 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+AlgorithmSpecificationOutputTypeDef = TypedDict(
+    "AlgorithmSpecificationOutputTypeDef",
+    {
+        "containerImage": ContainerImageOutputTypeDef,
+        "scriptModeConfig": ScriptModeConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 AlgorithmSpecificationTypeDef = TypedDict(
     "AlgorithmSpecificationTypeDef",
     {
         "containerImage": ContainerImageTypeDef,
         "scriptModeConfig": ScriptModeConfigTypeDef,
     },
     total=False,
 )
 
+DataSourceOutputTypeDef = TypedDict(
+    "DataSourceOutputTypeDef",
+    {
+        "s3DataSource": S3DataSourceOutputTypeDef,
+    },
+)
+
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "s3DataSource": S3DataSourceTypeDef,
     },
 )
 
@@ -516,39 +673,43 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class SearchDevicesRequestRequestTypeDef(
     _RequiredSearchDevicesRequestRequestTypeDef, _OptionalSearchDevicesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef = TypedDict(
     "_RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef",
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
     },
 )
 _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef = TypedDict(
     "_OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchDevicesRequestSearchDevicesPaginateTypeDef(
     _RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef,
     _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchJobsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchJobsRequestRequestTypeDef",
     {
         "filters": Sequence[SearchJobsFilterTypeDef],
     },
 )
 _OptionalSearchJobsRequestRequestTypeDef = TypedDict(
@@ -556,39 +717,43 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class SearchJobsRequestRequestTypeDef(
     _RequiredSearchJobsRequestRequestTypeDef, _OptionalSearchJobsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchJobsRequestSearchJobsPaginateTypeDef = TypedDict(
     "_RequiredSearchJobsRequestSearchJobsPaginateTypeDef",
     {
         "filters": Sequence[SearchJobsFilterTypeDef],
     },
 )
 _OptionalSearchJobsRequestSearchJobsPaginateTypeDef = TypedDict(
     "_OptionalSearchJobsRequestSearchJobsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchJobsRequestSearchJobsPaginateTypeDef(
     _RequiredSearchJobsRequestSearchJobsPaginateTypeDef,
     _OptionalSearchJobsRequestSearchJobsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredSearchQuantumTasksRequestRequestTypeDef = TypedDict(
     "_RequiredSearchQuantumTasksRequestRequestTypeDef",
     {
         "filters": Sequence[SearchQuantumTasksFilterTypeDef],
     },
 )
 _OptionalSearchQuantumTasksRequestRequestTypeDef = TypedDict(
@@ -596,40 +761,66 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class SearchQuantumTasksRequestRequestTypeDef(
     _RequiredSearchQuantumTasksRequestRequestTypeDef,
     _OptionalSearchQuantumTasksRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef = TypedDict(
     "_RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
     {
         "filters": Sequence[SearchQuantumTasksFilterTypeDef],
     },
 )
 _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef = TypedDict(
     "_OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef(
     _RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
     _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
 ):
     pass
 
+
+_RequiredInputFileConfigOutputTypeDef = TypedDict(
+    "_RequiredInputFileConfigOutputTypeDef",
+    {
+        "channelName": str,
+        "dataSource": DataSourceOutputTypeDef,
+    },
+)
+_OptionalInputFileConfigOutputTypeDef = TypedDict(
+    "_OptionalInputFileConfigOutputTypeDef",
+    {
+        "contentType": str,
+    },
+    total=False,
+)
+
+
+class InputFileConfigOutputTypeDef(
+    _RequiredInputFileConfigOutputTypeDef, _OptionalInputFileConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredInputFileConfigTypeDef = TypedDict(
     "_RequiredInputFileConfigTypeDef",
     {
         "channelName": str,
         "dataSource": DataSourceTypeDef,
     },
 )
@@ -637,17 +828,45 @@
     "_OptionalInputFileConfigTypeDef",
     {
         "contentType": str,
     },
     total=False,
 )
 
+
 class InputFileConfigTypeDef(_RequiredInputFileConfigTypeDef, _OptionalInputFileConfigTypeDef):
     pass
 
+
+GetJobResponseTypeDef = TypedDict(
+    "GetJobResponseTypeDef",
+    {
+        "algorithmSpecification": AlgorithmSpecificationOutputTypeDef,
+        "billableDuration": int,
+        "checkpointConfig": JobCheckpointConfigOutputTypeDef,
+        "createdAt": datetime,
+        "deviceConfig": DeviceConfigOutputTypeDef,
+        "endedAt": datetime,
+        "events": List[JobEventDetailsTypeDef],
+        "failureReason": str,
+        "hyperParameters": Dict[str, str],
+        "inputDataConfig": List[InputFileConfigOutputTypeDef],
+        "instanceConfig": InstanceConfigOutputTypeDef,
+        "jobArn": str,
+        "jobName": str,
+        "outputDataConfig": JobOutputDataConfigOutputTypeDef,
+        "roleArn": str,
+        "startedAt": datetime,
+        "status": JobPrimaryStatusType,
+        "stoppingCondition": JobStoppingConditionOutputTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "algorithmSpecification": AlgorithmSpecificationTypeDef,
         "clientToken": str,
         "deviceConfig": DeviceConfigTypeDef,
         "instanceConfig": InstanceConfigTypeDef,
@@ -664,37 +883,12 @@
         "inputDataConfig": Sequence[InputFileConfigTypeDef],
         "stoppingCondition": JobStoppingConditionTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
-
-GetJobResponseTypeDef = TypedDict(
-    "GetJobResponseTypeDef",
-    {
-        "algorithmSpecification": AlgorithmSpecificationTypeDef,
-        "billableDuration": int,
-        "checkpointConfig": JobCheckpointConfigTypeDef,
-        "createdAt": datetime,
-        "deviceConfig": DeviceConfigTypeDef,
-        "endedAt": datetime,
-        "events": List[JobEventDetailsTypeDef],
-        "failureReason": str,
-        "hyperParameters": Dict[str, str],
-        "inputDataConfig": List[InputFileConfigTypeDef],
-        "instanceConfig": InstanceConfigTypeDef,
-        "jobArn": str,
-        "jobName": str,
-        "outputDataConfig": JobOutputDataConfigTypeDef,
-        "roleArn": str,
-        "startedAt": datetime,
-        "status": JobPrimaryStatusType,
-        "stoppingCondition": JobStoppingConditionTypeDef,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket.egg-info/PKG-INFO` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-braket
-Version: 1.28.0
-Summary: Type annotations for boto3.Braket 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Braket 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-braket"></a>
 
 # mypy-boto3-braket
 
 [![PyPI - mypy-boto3-braket](https://img.shields.io/pypi/v/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-braket?color=blue)](https://pypistats.org/packages/mypy-boto3-braket)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-braket)](https://pepy.tech/project/mypy-boto3-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Braket 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[boto3.Braket 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [mypy-boto3-braket docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,65 +338,76 @@
 ### Typed dictionaries
 
 `mypy_boto3_braket.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_braket.type_defs import (
+    ContainerImageOutputTypeDef,
+    ScriptModeConfigOutputTypeDef,
     ContainerImageTypeDef,
     ScriptModeConfigTypeDef,
     CancelJobRequestRequestTypeDef,
     CancelJobResponseTypeDef,
     CancelQuantumTaskRequestRequestTypeDef,
     CancelQuantumTaskResponseTypeDef,
     DeviceConfigTypeDef,
     InstanceConfigTypeDef,
     JobCheckpointConfigTypeDef,
     JobOutputDataConfigTypeDef,
     JobStoppingConditionTypeDef,
     CreateJobResponseTypeDef,
     CreateQuantumTaskRequestRequestTypeDef,
     CreateQuantumTaskResponseTypeDef,
+    S3DataSourceOutputTypeDef,
     S3DataSourceTypeDef,
+    DeviceConfigOutputTypeDef,
     DeviceSummaryTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetDeviceResponseTypeDef,
     GetJobRequestRequestTypeDef,
+    InstanceConfigOutputTypeDef,
+    JobCheckpointConfigOutputTypeDef,
     JobEventDetailsTypeDef,
+    JobOutputDataConfigOutputTypeDef,
+    JobStoppingConditionOutputTypeDef,
     GetQuantumTaskRequestRequestTypeDef,
     GetQuantumTaskResponseTypeDef,
     JobSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QuantumTaskSummaryTypeDef,
     ResponseMetadataTypeDef,
     SearchDevicesFilterTypeDef,
     SearchJobsFilterTypeDef,
     SearchQuantumTasksFilterTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AlgorithmSpecificationOutputTypeDef,
     AlgorithmSpecificationTypeDef,
+    DataSourceOutputTypeDef,
     DataSourceTypeDef,
     SearchDevicesResponseTypeDef,
     SearchJobsResponseTypeDef,
     SearchQuantumTasksResponseTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchJobsRequestRequestTypeDef,
     SearchJobsRequestSearchJobsPaginateTypeDef,
     SearchQuantumTasksRequestRequestTypeDef,
     SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
+    InputFileConfigOutputTypeDef,
     InputFileConfigTypeDef,
-    CreateJobRequestRequestTypeDef,
     GetJobResponseTypeDef,
+    CreateJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ContainerImageTypeDef:
+def get_structure() -> ContainerImageOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-braket-1.28.0/mypy_boto3_braket.egg-info/SOURCES.txt` & `mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.0/setup.py` & `mypy-boto3-braket-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-braket",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_braket"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Braket 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Braket 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

