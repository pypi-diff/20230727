# Comparing `tmp/mypy-boto3-healthlake-1.28.0.tar.gz` & `tmp/mypy-boto3-healthlake-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-healthlake-1.28.0.tar", last modified: Thu Jul  6 20:59:42 2023, max compression
+gzip compressed data, was "mypy-boto3-healthlake-1.28.12.tar", last modified: Thu Jul 27 05:34:45 2023, max compression
```

## Comparing `mypy-boto3-healthlake-1.28.0.tar` & `mypy-boto3-healthlake-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:42.066317 mypy-boto3-healthlake-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-06 20:59:42.066317 mypy-boto3-healthlake-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:42.066317 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:42:36.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:42.066317 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-06 20:59:41.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-06 20:59:41.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:41.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:41.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:41.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:41.000000 mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:42.066317 mypy-boto3-healthlake-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:42:35.000000 mypy-boto3-healthlake-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.736496 mypy-boto3-healthlake-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-07-27 05:34:45.736496 mypy-boto3-healthlake-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.736496 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-27 05:23:18.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-07-27 05:23:18.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16502 2023-07-27 05:23:18.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-07-27 05:23:18.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.736496 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-07-27 05:34:45.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 05:34:45.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:45.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:45.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:45.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:45.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:45.736496 mypy-boto3-healthlake-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/setup.py
```

### Comparing `mypy-boto3-healthlake-1.28.0/LICENSE` & `mypy-boto3-healthlake-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.28.0/PKG-INFO` & `mypy-boto3-healthlake-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-healthlake
-Version: 1.28.0
-Summary: Type annotations for boto3.HealthLake 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.HealthLake 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-healthlake"></a>
 
 # mypy-boto3-healthlake
 
 [![PyPI - mypy-boto3-healthlake](https://img.shields.io/pypi/v/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-healthlake?color=blue)](https://pypistats.org/packages/mypy-boto3-healthlake)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-healthlake)](https://pepy.tech/project/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,36 +306,44 @@
 ```python
 from mypy_boto3_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
     CreateFHIRDatastoreResponseTypeDef,
     DatastoreFilterTypeDef,
+    IdentityProviderConfigurationOutputTypeDef,
+    PreloadDataConfigOutputTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
     DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
+    KmsEncryptionConfigOutputTypeDef,
     KmsEncryptionConfigTypeDef,
     ListFHIRExportJobsRequestRequestTypeDef,
     ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     ResponseMetadataTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListFHIRDatastoresRequestRequestTypeDef,
+    SseConfigurationOutputTypeDef,
     SseConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    OutputDataConfigOutputTypeDef,
     OutputDataConfigTypeDef,
-    CreateFHIRDatastoreRequestRequestTypeDef,
     DatastorePropertiesTypeDef,
+    CreateFHIRDatastoreRequestRequestTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
     StartFHIRExportJobRequestRequestTypeDef,
     StartFHIRImportJobRequestRequestTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
     ListFHIRDatastoresResponseTypeDef,
     DescribeFHIRExportJobResponseTypeDef,
```

### Comparing `mypy-boto3-healthlake-1.28.0/README.md` & `mypy-boto3-healthlake-1.28.12/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-healthlake"></a>
 
 # mypy-boto3-healthlake
 
 [![PyPI - mypy-boto3-healthlake](https://img.shields.io/pypi/v/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-healthlake?color=blue)](https://pypistats.org/packages/mypy-boto3-healthlake)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-healthlake)](https://pepy.tech/project/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -274,36 +274,44 @@
 ```python
 from mypy_boto3_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
     CreateFHIRDatastoreResponseTypeDef,
     DatastoreFilterTypeDef,
+    IdentityProviderConfigurationOutputTypeDef,
+    PreloadDataConfigOutputTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
     DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
+    KmsEncryptionConfigOutputTypeDef,
     KmsEncryptionConfigTypeDef,
     ListFHIRExportJobsRequestRequestTypeDef,
     ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     ResponseMetadataTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListFHIRDatastoresRequestRequestTypeDef,
+    SseConfigurationOutputTypeDef,
     SseConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    OutputDataConfigOutputTypeDef,
     OutputDataConfigTypeDef,
-    CreateFHIRDatastoreRequestRequestTypeDef,
     DatastorePropertiesTypeDef,
+    CreateFHIRDatastoreRequestRequestTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
     StartFHIRExportJobRequestRequestTypeDef,
     StartFHIRImportJobRequestRequestTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
     ListFHIRDatastoresResponseTypeDef,
     DescribeFHIRExportJobResponseTypeDef,
```

### Comparing `mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/__main__.py` & `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.HealthLake 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.HealthLake 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake\nOther"
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

### Comparing `mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/client.py` & `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,33 +109,33 @@
         SseConfiguration: SseConfigurationTypeDef = ...,
         PreloadDataConfig: PreloadDataConfigTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdentityProviderConfiguration: IdentityProviderConfigurationTypeDef = ...
     ) -> CreateFHIRDatastoreResponseTypeDef:
         """
-        Creates a Data Store that can ingest and export FHIR formatted data.
+        Creates a data store that can ingest and export FHIR formatted data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.create_fhir_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#create_fhir_datastore)
         """
 
     def delete_fhir_datastore(self, *, DatastoreId: str) -> DeleteFHIRDatastoreResponseTypeDef:
         """
-        Deletes a Data Store.
+        Deletes a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.delete_fhir_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#delete_fhir_datastore)
         """
 
     def describe_fhir_datastore(self, *, DatastoreId: str) -> DescribeFHIRDatastoreResponseTypeDef:
         """
-        Gets the properties associated with the FHIR Data Store, including the Data
-        Store ID, Data Store ARN, Data Store name, Data Store status, created at, Data
-        Store type version, and Data Store endpoint.
+        Gets the properties associated with the FHIR data store, including the data
+        store ID, data store ARN, data store name, data store status, when the data
+        store was created, data store type version, and the data store's endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.describe_fhir_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#describe_fhir_datastore)
         """
 
     def describe_fhir_export_job(
         self, *, DatastoreId: str, JobId: str
@@ -173,16 +173,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#generate_presigned_url)
         """
 
     def list_fhir_datastores(
         self, *, Filter: DatastoreFilterTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListFHIRDatastoresResponseTypeDef:
         """
-        Lists all FHIR Data Stores that are in the user’s account, regardless of Data
-        Store status.
+        Lists all FHIR data stores that are in the user’s account, regardless of data
+        store status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_datastores)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#list_fhir_datastores)
         """
 
     def list_fhir_export_jobs(
         self,
@@ -218,15 +218,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#list_fhir_import_jobs)
         """
 
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
-        Returns a list of all existing tags associated with a Data Store.
+        Returns a list of all existing tags associated with a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#list_tags_for_resource)
         """
 
     def start_fhir_export_job(
         self,
@@ -259,20 +259,20 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.start_fhir_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#start_fhir_import_job)
         """
 
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
-        Adds a user specified key and value tag to a Data Store.
+        Adds a user specified key and value tag to a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#tag_resource)
         """
 
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes tags from a Data Store.
+        Removes tags from a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#untag_resource)
         """
```

### Comparing `mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/client.pyi` & `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -102,31 +102,31 @@
         SseConfiguration: SseConfigurationTypeDef = ...,
         PreloadDataConfig: PreloadDataConfigTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         IdentityProviderConfiguration: IdentityProviderConfigurationTypeDef = ...
     ) -> CreateFHIRDatastoreResponseTypeDef:
         """
-        Creates a Data Store that can ingest and export FHIR formatted data.
+        Creates a data store that can ingest and export FHIR formatted data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.create_fhir_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#create_fhir_datastore)
         """
     def delete_fhir_datastore(self, *, DatastoreId: str) -> DeleteFHIRDatastoreResponseTypeDef:
         """
-        Deletes a Data Store.
+        Deletes a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.delete_fhir_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#delete_fhir_datastore)
         """
     def describe_fhir_datastore(self, *, DatastoreId: str) -> DescribeFHIRDatastoreResponseTypeDef:
         """
-        Gets the properties associated with the FHIR Data Store, including the Data
-        Store ID, Data Store ARN, Data Store name, Data Store status, created at, Data
-        Store type version, and Data Store endpoint.
+        Gets the properties associated with the FHIR data store, including the data
+        store ID, data store ARN, data store name, data store status, when the data
+        store was created, data store type version, and the data store's endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.describe_fhir_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#describe_fhir_datastore)
         """
     def describe_fhir_export_job(
         self, *, DatastoreId: str, JobId: str
     ) -> DescribeFHIRExportJobResponseTypeDef:
@@ -160,16 +160,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#generate_presigned_url)
         """
     def list_fhir_datastores(
         self, *, Filter: DatastoreFilterTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListFHIRDatastoresResponseTypeDef:
         """
-        Lists all FHIR Data Stores that are in the user’s account, regardless of Data
-        Store status.
+        Lists all FHIR data stores that are in the user’s account, regardless of data
+        store status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_datastores)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#list_fhir_datastores)
         """
     def list_fhir_export_jobs(
         self,
         *,
@@ -202,15 +202,15 @@
         Lists all FHIR import jobs associated with an account and their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_fhir_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#list_fhir_import_jobs)
         """
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
-        Returns a list of all existing tags associated with a Data Store.
+        Returns a list of all existing tags associated with a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#list_tags_for_resource)
         """
     def start_fhir_export_job(
         self,
         *,
@@ -240,19 +240,19 @@
         Begins a FHIR Import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.start_fhir_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#start_fhir_import_job)
         """
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
-        Adds a user specified key and value tag to a Data Store.
+        Adds a user specified key and value tag to a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#tag_resource)
         """
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes tags from a Data Store.
+        Removes tags from a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#untag_resource)
         """
```

### Comparing `mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/literals.py` & `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthorizationStrategyType",
     "CmkTypeType",
     "DatastoreStatusType",
     "FHIRVersionType",
     "JobStatusType",
     "PreloadDataTypeType",
     "HealthLakeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AuthorizationStrategyType = Literal["AWS_AUTH", "SMART_ON_FHIR_V1"]
 CmkTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
 DatastoreStatusType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING"]
 FHIRVersionType = Literal["R4"]
 JobStatusType = Literal[
     "CANCEL_COMPLETED",
     "CANCEL_FAILED",
@@ -165,14 +163,15 @@
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
@@ -251,26 +250,28 @@
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

### Comparing `mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/literals.pyi` & `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AuthorizationStrategyType",
     "CmkTypeType",
     "DatastoreStatusType",
     "FHIRVersionType",
     "JobStatusType",
     "PreloadDataTypeType",
     "HealthLakeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AuthorizationStrategyType = Literal["AWS_AUTH", "SMART_ON_FHIR_V1"]
 CmkTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
 DatastoreStatusType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING"]
 FHIRVersionType = Literal["R4"]
 JobStatusType = Literal[
     "CANCEL_COMPLETED",
     "CANCEL_FAILED",
@@ -163,14 +165,15 @@
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
@@ -249,26 +252,28 @@
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

### Comparing `mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/type_defs.py` & `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/type_defs.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -22,43 +22,50 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
     "CreateFHIRDatastoreResponseTypeDef",
     "DatastoreFilterTypeDef",
+    "IdentityProviderConfigurationOutputTypeDef",
+    "PreloadDataConfigOutputTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     "DeleteFHIRDatastoreResponseTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
     "DescribeFHIRImportJobRequestRequestTypeDef",
+    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
+    "KmsEncryptionConfigOutputTypeDef",
     "KmsEncryptionConfigTypeDef",
     "ListFHIRExportJobsRequestRequestTypeDef",
     "ListFHIRImportJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "S3ConfigurationOutputTypeDef",
     "S3ConfigurationTypeDef",
     "ResponseMetadataTypeDef",
     "StartFHIRExportJobResponseTypeDef",
     "StartFHIRImportJobResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListFHIRDatastoresRequestRequestTypeDef",
+    "SseConfigurationOutputTypeDef",
     "SseConfigurationTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "OutputDataConfigOutputTypeDef",
     "OutputDataConfigTypeDef",
-    "CreateFHIRDatastoreRequestRequestTypeDef",
     "DatastorePropertiesTypeDef",
+    "CreateFHIRDatastoreRequestRequestTypeDef",
     "ExportJobPropertiesTypeDef",
     "ImportJobPropertiesTypeDef",
     "StartFHIRExportJobRequestRequestTypeDef",
     "StartFHIRImportJobRequestRequestTypeDef",
     "DescribeFHIRDatastoreResponseTypeDef",
     "ListFHIRDatastoresResponseTypeDef",
     "DescribeFHIRExportJobResponseTypeDef",
@@ -79,21 +86,19 @@
         "FineGrainedAuthorizationEnabled": bool,
         "Metadata": str,
         "IdpLambdaArn": str,
     },
     total=False,
 )
 
-
 class IdentityProviderConfigurationTypeDef(
     _RequiredIdentityProviderConfigurationTypeDef, _OptionalIdentityProviderConfigurationTypeDef
 ):
     pass
 
-
 PreloadDataConfigTypeDef = TypedDict(
     "PreloadDataConfigTypeDef",
     {
         "PreloadDataType": Literal["SYNTHEA"],
     },
 )
 
@@ -123,14 +128,43 @@
         "DatastoreStatus": DatastoreStatusType,
         "CreatedBefore": Union[datetime, str],
         "CreatedAfter": Union[datetime, str],
     },
     total=False,
 )
 
+_RequiredIdentityProviderConfigurationOutputTypeDef = TypedDict(
+    "_RequiredIdentityProviderConfigurationOutputTypeDef",
+    {
+        "AuthorizationStrategy": AuthorizationStrategyType,
+    },
+)
+_OptionalIdentityProviderConfigurationOutputTypeDef = TypedDict(
+    "_OptionalIdentityProviderConfigurationOutputTypeDef",
+    {
+        "FineGrainedAuthorizationEnabled": bool,
+        "Metadata": str,
+        "IdpLambdaArn": str,
+    },
+    total=False,
+)
+
+class IdentityProviderConfigurationOutputTypeDef(
+    _RequiredIdentityProviderConfigurationOutputTypeDef,
+    _OptionalIdentityProviderConfigurationOutputTypeDef,
+):
+    pass
+
+PreloadDataConfigOutputTypeDef = TypedDict(
+    "PreloadDataConfigOutputTypeDef",
+    {
+        "PreloadDataType": Literal["SYNTHEA"],
+    },
+)
+
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
@@ -164,43 +198,68 @@
     "DescribeFHIRImportJobRequestRequestTypeDef",
     {
         "DatastoreId": str,
         "JobId": str,
     },
 )
 
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+    total=False,
+)
+
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
     total=False,
 )
 
+_RequiredKmsEncryptionConfigOutputTypeDef = TypedDict(
+    "_RequiredKmsEncryptionConfigOutputTypeDef",
+    {
+        "CmkType": CmkTypeType,
+    },
+)
+_OptionalKmsEncryptionConfigOutputTypeDef = TypedDict(
+    "_OptionalKmsEncryptionConfigOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+class KmsEncryptionConfigOutputTypeDef(
+    _RequiredKmsEncryptionConfigOutputTypeDef, _OptionalKmsEncryptionConfigOutputTypeDef
+):
+    pass
+
 _RequiredKmsEncryptionConfigTypeDef = TypedDict(
     "_RequiredKmsEncryptionConfigTypeDef",
     {
         "CmkType": CmkTypeType,
     },
 )
 _OptionalKmsEncryptionConfigTypeDef = TypedDict(
     "_OptionalKmsEncryptionConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class KmsEncryptionConfigTypeDef(
     _RequiredKmsEncryptionConfigTypeDef, _OptionalKmsEncryptionConfigTypeDef
 ):
     pass
 
-
 _RequiredListFHIRExportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListFHIRExportJobsRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 _OptionalListFHIRExportJobsRequestRequestTypeDef = TypedDict(
@@ -212,22 +271,20 @@
         "JobStatus": JobStatusType,
         "SubmittedBefore": Union[datetime, str],
         "SubmittedAfter": Union[datetime, str],
     },
     total=False,
 )
 
-
 class ListFHIRExportJobsRequestRequestTypeDef(
     _RequiredListFHIRExportJobsRequestRequestTypeDef,
     _OptionalListFHIRExportJobsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListFHIRImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListFHIRImportJobsRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 _OptionalListFHIRImportJobsRequestRequestTypeDef = TypedDict(
@@ -239,29 +296,43 @@
         "JobStatus": JobStatusType,
         "SubmittedBefore": Union[datetime, str],
         "SubmittedAfter": Union[datetime, str],
     },
     total=False,
 )
 
-
 class ListFHIRImportJobsRequestRequestTypeDef(
     _RequiredListFHIRImportJobsRequestRequestTypeDef,
     _OptionalListFHIRImportJobsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+S3ConfigurationOutputTypeDef = TypedDict(
+    "S3ConfigurationOutputTypeDef",
+    {
+        "S3Uri": str,
+        "KmsKeyId": str,
+    },
+)
+
 S3ConfigurationTypeDef = TypedDict(
     "S3ConfigurationTypeDef",
     {
         "S3Uri": str,
         "KmsKeyId": str,
     },
 )
@@ -301,22 +372,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -327,56 +390,52 @@
         "Filter": DatastoreFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+SseConfigurationOutputTypeDef = TypedDict(
+    "SseConfigurationOutputTypeDef",
+    {
+        "KmsEncryptionConfig": KmsEncryptionConfigOutputTypeDef,
+    },
+)
+
 SseConfigurationTypeDef = TypedDict(
     "SseConfigurationTypeDef",
     {
         "KmsEncryptionConfig": KmsEncryptionConfigTypeDef,
     },
 )
 
-OutputDataConfigTypeDef = TypedDict(
-    "OutputDataConfigTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "S3Configuration": S3ConfigurationTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFHIRDatastoreRequestRequestTypeDef",
+OutputDataConfigOutputTypeDef = TypedDict(
+    "OutputDataConfigOutputTypeDef",
     {
-        "DatastoreTypeVersion": Literal["R4"],
+        "S3Configuration": S3ConfigurationOutputTypeDef,
     },
+    total=False,
 )
-_OptionalCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFHIRDatastoreRequestRequestTypeDef",
+
+OutputDataConfigTypeDef = TypedDict(
+    "OutputDataConfigTypeDef",
     {
-        "DatastoreName": str,
-        "SseConfiguration": SseConfigurationTypeDef,
-        "PreloadDataConfig": PreloadDataConfigTypeDef,
-        "ClientToken": str,
-        "Tags": Sequence[TagTypeDef],
-        "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
+        "S3Configuration": S3ConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class CreateFHIRDatastoreRequestRequestTypeDef(
-    _RequiredCreateFHIRDatastoreRequestRequestTypeDef,
-    _OptionalCreateFHIRDatastoreRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredDatastorePropertiesTypeDef = TypedDict(
     "_RequiredDatastorePropertiesTypeDef",
     {
         "DatastoreId": str,
         "DatastoreArn": str,
         "DatastoreStatus": DatastoreStatusType,
         "DatastoreTypeVersion": Literal["R4"],
@@ -384,85 +443,104 @@
     },
 )
 _OptionalDatastorePropertiesTypeDef = TypedDict(
     "_OptionalDatastorePropertiesTypeDef",
     {
         "DatastoreName": str,
         "CreatedAt": datetime,
-        "SseConfiguration": SseConfigurationTypeDef,
-        "PreloadDataConfig": PreloadDataConfigTypeDef,
-        "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
+        "SseConfiguration": SseConfigurationOutputTypeDef,
+        "PreloadDataConfig": PreloadDataConfigOutputTypeDef,
+        "IdentityProviderConfiguration": IdentityProviderConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class DatastorePropertiesTypeDef(
     _RequiredDatastorePropertiesTypeDef, _OptionalDatastorePropertiesTypeDef
 ):
     pass
 
+_RequiredCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFHIRDatastoreRequestRequestTypeDef",
+    {
+        "DatastoreTypeVersion": Literal["R4"],
+    },
+)
+_OptionalCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFHIRDatastoreRequestRequestTypeDef",
+    {
+        "DatastoreName": str,
+        "SseConfiguration": SseConfigurationTypeDef,
+        "PreloadDataConfig": PreloadDataConfigTypeDef,
+        "ClientToken": str,
+        "Tags": Sequence[TagTypeDef],
+        "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class CreateFHIRDatastoreRequestRequestTypeDef(
+    _RequiredCreateFHIRDatastoreRequestRequestTypeDef,
+    _OptionalCreateFHIRDatastoreRequestRequestTypeDef,
+):
+    pass
 
 _RequiredExportJobPropertiesTypeDef = TypedDict(
     "_RequiredExportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "SubmitTime": datetime,
         "DatastoreId": str,
-        "OutputDataConfig": OutputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
     },
 )
 _OptionalExportJobPropertiesTypeDef = TypedDict(
     "_OptionalExportJobPropertiesTypeDef",
     {
         "JobName": str,
         "EndTime": datetime,
         "DataAccessRoleArn": str,
         "Message": str,
     },
     total=False,
 )
 
-
 class ExportJobPropertiesTypeDef(
     _RequiredExportJobPropertiesTypeDef, _OptionalExportJobPropertiesTypeDef
 ):
     pass
 
-
 _RequiredImportJobPropertiesTypeDef = TypedDict(
     "_RequiredImportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "SubmitTime": datetime,
         "DatastoreId": str,
-        "InputDataConfig": InputDataConfigTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
     },
 )
 _OptionalImportJobPropertiesTypeDef = TypedDict(
     "_OptionalImportJobPropertiesTypeDef",
     {
         "JobName": str,
         "EndTime": datetime,
-        "JobOutputDataConfig": OutputDataConfigTypeDef,
+        "JobOutputDataConfig": OutputDataConfigOutputTypeDef,
         "DataAccessRoleArn": str,
         "Message": str,
     },
     total=False,
 )
 
-
 class ImportJobPropertiesTypeDef(
     _RequiredImportJobPropertiesTypeDef, _OptionalImportJobPropertiesTypeDef
 ):
     pass
 
-
 _RequiredStartFHIRExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartFHIRExportJobRequestRequestTypeDef",
     {
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DatastoreId": str,
         "DataAccessRoleArn": str,
         "ClientToken": str,
@@ -472,22 +550,20 @@
     "_OptionalStartFHIRExportJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
     total=False,
 )
 
-
 class StartFHIRExportJobRequestRequestTypeDef(
     _RequiredStartFHIRExportJobRequestRequestTypeDef,
     _OptionalStartFHIRExportJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartFHIRImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartFHIRImportJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "JobOutputDataConfig": OutputDataConfigTypeDef,
         "DatastoreId": str,
         "DataAccessRoleArn": str,
@@ -498,22 +574,20 @@
     "_OptionalStartFHIRImportJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
     total=False,
 )
 
-
 class StartFHIRImportJobRequestRequestTypeDef(
     _RequiredStartFHIRImportJobRequestRequestTypeDef,
     _OptionalStartFHIRImportJobRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeFHIRDatastoreResponseTypeDef = TypedDict(
     "DescribeFHIRDatastoreResponseTypeDef",
     {
         "DatastoreProperties": DatastorePropertiesTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake/type_defs.pyi` & `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/type_defs.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,42 +22,51 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
     "CreateFHIRDatastoreResponseTypeDef",
     "DatastoreFilterTypeDef",
+    "IdentityProviderConfigurationOutputTypeDef",
+    "PreloadDataConfigOutputTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     "DeleteFHIRDatastoreResponseTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
     "DescribeFHIRImportJobRequestRequestTypeDef",
+    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
+    "KmsEncryptionConfigOutputTypeDef",
     "KmsEncryptionConfigTypeDef",
     "ListFHIRExportJobsRequestRequestTypeDef",
     "ListFHIRImportJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "S3ConfigurationOutputTypeDef",
     "S3ConfigurationTypeDef",
     "ResponseMetadataTypeDef",
     "StartFHIRExportJobResponseTypeDef",
     "StartFHIRImportJobResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListFHIRDatastoresRequestRequestTypeDef",
+    "SseConfigurationOutputTypeDef",
     "SseConfigurationTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "OutputDataConfigOutputTypeDef",
     "OutputDataConfigTypeDef",
-    "CreateFHIRDatastoreRequestRequestTypeDef",
     "DatastorePropertiesTypeDef",
+    "CreateFHIRDatastoreRequestRequestTypeDef",
     "ExportJobPropertiesTypeDef",
     "ImportJobPropertiesTypeDef",
     "StartFHIRExportJobRequestRequestTypeDef",
     "StartFHIRImportJobRequestRequestTypeDef",
     "DescribeFHIRDatastoreResponseTypeDef",
     "ListFHIRDatastoresResponseTypeDef",
     "DescribeFHIRExportJobResponseTypeDef",
@@ -78,19 +87,21 @@
         "FineGrainedAuthorizationEnabled": bool,
         "Metadata": str,
         "IdpLambdaArn": str,
     },
     total=False,
 )
 
+
 class IdentityProviderConfigurationTypeDef(
     _RequiredIdentityProviderConfigurationTypeDef, _OptionalIdentityProviderConfigurationTypeDef
 ):
     pass
 
+
 PreloadDataConfigTypeDef = TypedDict(
     "PreloadDataConfigTypeDef",
     {
         "PreloadDataType": Literal["SYNTHEA"],
     },
 )
 
@@ -120,14 +131,45 @@
         "DatastoreStatus": DatastoreStatusType,
         "CreatedBefore": Union[datetime, str],
         "CreatedAfter": Union[datetime, str],
     },
     total=False,
 )
 
+_RequiredIdentityProviderConfigurationOutputTypeDef = TypedDict(
+    "_RequiredIdentityProviderConfigurationOutputTypeDef",
+    {
+        "AuthorizationStrategy": AuthorizationStrategyType,
+    },
+)
+_OptionalIdentityProviderConfigurationOutputTypeDef = TypedDict(
+    "_OptionalIdentityProviderConfigurationOutputTypeDef",
+    {
+        "FineGrainedAuthorizationEnabled": bool,
+        "Metadata": str,
+        "IdpLambdaArn": str,
+    },
+    total=False,
+)
+
+
+class IdentityProviderConfigurationOutputTypeDef(
+    _RequiredIdentityProviderConfigurationOutputTypeDef,
+    _OptionalIdentityProviderConfigurationOutputTypeDef,
+):
+    pass
+
+
+PreloadDataConfigOutputTypeDef = TypedDict(
+    "PreloadDataConfigOutputTypeDef",
+    {
+        "PreloadDataType": Literal["SYNTHEA"],
+    },
+)
+
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
@@ -161,41 +203,72 @@
     "DescribeFHIRImportJobRequestRequestTypeDef",
     {
         "DatastoreId": str,
         "JobId": str,
     },
 )
 
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+    total=False,
+)
+
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
     total=False,
 )
 
+_RequiredKmsEncryptionConfigOutputTypeDef = TypedDict(
+    "_RequiredKmsEncryptionConfigOutputTypeDef",
+    {
+        "CmkType": CmkTypeType,
+    },
+)
+_OptionalKmsEncryptionConfigOutputTypeDef = TypedDict(
+    "_OptionalKmsEncryptionConfigOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class KmsEncryptionConfigOutputTypeDef(
+    _RequiredKmsEncryptionConfigOutputTypeDef, _OptionalKmsEncryptionConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredKmsEncryptionConfigTypeDef = TypedDict(
     "_RequiredKmsEncryptionConfigTypeDef",
     {
         "CmkType": CmkTypeType,
     },
 )
 _OptionalKmsEncryptionConfigTypeDef = TypedDict(
     "_OptionalKmsEncryptionConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class KmsEncryptionConfigTypeDef(
     _RequiredKmsEncryptionConfigTypeDef, _OptionalKmsEncryptionConfigTypeDef
 ):
     pass
 
+
 _RequiredListFHIRExportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListFHIRExportJobsRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 _OptionalListFHIRExportJobsRequestRequestTypeDef = TypedDict(
@@ -207,20 +280,22 @@
         "JobStatus": JobStatusType,
         "SubmittedBefore": Union[datetime, str],
         "SubmittedAfter": Union[datetime, str],
     },
     total=False,
 )
 
+
 class ListFHIRExportJobsRequestRequestTypeDef(
     _RequiredListFHIRExportJobsRequestRequestTypeDef,
     _OptionalListFHIRExportJobsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListFHIRImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListFHIRImportJobsRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 _OptionalListFHIRImportJobsRequestRequestTypeDef = TypedDict(
@@ -232,27 +307,45 @@
         "JobStatus": JobStatusType,
         "SubmittedBefore": Union[datetime, str],
         "SubmittedAfter": Union[datetime, str],
     },
     total=False,
 )
 
+
 class ListFHIRImportJobsRequestRequestTypeDef(
     _RequiredListFHIRImportJobsRequestRequestTypeDef,
     _OptionalListFHIRImportJobsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+S3ConfigurationOutputTypeDef = TypedDict(
+    "S3ConfigurationOutputTypeDef",
+    {
+        "S3Uri": str,
+        "KmsKeyId": str,
+    },
+)
+
 S3ConfigurationTypeDef = TypedDict(
     "S3ConfigurationTypeDef",
     {
         "S3Uri": str,
         "KmsKeyId": str,
     },
 )
@@ -292,22 +385,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -318,54 +403,52 @@
         "Filter": DatastoreFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+SseConfigurationOutputTypeDef = TypedDict(
+    "SseConfigurationOutputTypeDef",
+    {
+        "KmsEncryptionConfig": KmsEncryptionConfigOutputTypeDef,
+    },
+)
+
 SseConfigurationTypeDef = TypedDict(
     "SseConfigurationTypeDef",
     {
         "KmsEncryptionConfig": KmsEncryptionConfigTypeDef,
     },
 )
 
-OutputDataConfigTypeDef = TypedDict(
-    "OutputDataConfigTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "S3Configuration": S3ConfigurationTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-_RequiredCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFHIRDatastoreRequestRequestTypeDef",
+OutputDataConfigOutputTypeDef = TypedDict(
+    "OutputDataConfigOutputTypeDef",
     {
-        "DatastoreTypeVersion": Literal["R4"],
+        "S3Configuration": S3ConfigurationOutputTypeDef,
     },
+    total=False,
 )
-_OptionalCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFHIRDatastoreRequestRequestTypeDef",
+
+OutputDataConfigTypeDef = TypedDict(
+    "OutputDataConfigTypeDef",
     {
-        "DatastoreName": str,
-        "SseConfiguration": SseConfigurationTypeDef,
-        "PreloadDataConfig": PreloadDataConfigTypeDef,
-        "ClientToken": str,
-        "Tags": Sequence[TagTypeDef],
-        "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
+        "S3Configuration": S3ConfigurationTypeDef,
     },
     total=False,
 )
 
-class CreateFHIRDatastoreRequestRequestTypeDef(
-    _RequiredCreateFHIRDatastoreRequestRequestTypeDef,
-    _OptionalCreateFHIRDatastoreRequestRequestTypeDef,
-):
-    pass
-
 _RequiredDatastorePropertiesTypeDef = TypedDict(
     "_RequiredDatastorePropertiesTypeDef",
     {
         "DatastoreId": str,
         "DatastoreArn": str,
         "DatastoreStatus": DatastoreStatusType,
         "DatastoreTypeVersion": Literal["R4"],
@@ -373,79 +456,112 @@
     },
 )
 _OptionalDatastorePropertiesTypeDef = TypedDict(
     "_OptionalDatastorePropertiesTypeDef",
     {
         "DatastoreName": str,
         "CreatedAt": datetime,
+        "SseConfiguration": SseConfigurationOutputTypeDef,
+        "PreloadDataConfig": PreloadDataConfigOutputTypeDef,
+        "IdentityProviderConfiguration": IdentityProviderConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class DatastorePropertiesTypeDef(
+    _RequiredDatastorePropertiesTypeDef, _OptionalDatastorePropertiesTypeDef
+):
+    pass
+
+
+_RequiredCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFHIRDatastoreRequestRequestTypeDef",
+    {
+        "DatastoreTypeVersion": Literal["R4"],
+    },
+)
+_OptionalCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFHIRDatastoreRequestRequestTypeDef",
+    {
+        "DatastoreName": str,
         "SseConfiguration": SseConfigurationTypeDef,
         "PreloadDataConfig": PreloadDataConfigTypeDef,
+        "ClientToken": str,
+        "Tags": Sequence[TagTypeDef],
         "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
-class DatastorePropertiesTypeDef(
-    _RequiredDatastorePropertiesTypeDef, _OptionalDatastorePropertiesTypeDef
+
+class CreateFHIRDatastoreRequestRequestTypeDef(
+    _RequiredCreateFHIRDatastoreRequestRequestTypeDef,
+    _OptionalCreateFHIRDatastoreRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredExportJobPropertiesTypeDef = TypedDict(
     "_RequiredExportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "SubmitTime": datetime,
         "DatastoreId": str,
-        "OutputDataConfig": OutputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigOutputTypeDef,
     },
 )
 _OptionalExportJobPropertiesTypeDef = TypedDict(
     "_OptionalExportJobPropertiesTypeDef",
     {
         "JobName": str,
         "EndTime": datetime,
         "DataAccessRoleArn": str,
         "Message": str,
     },
     total=False,
 )
 
+
 class ExportJobPropertiesTypeDef(
     _RequiredExportJobPropertiesTypeDef, _OptionalExportJobPropertiesTypeDef
 ):
     pass
 
+
 _RequiredImportJobPropertiesTypeDef = TypedDict(
     "_RequiredImportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "SubmitTime": datetime,
         "DatastoreId": str,
-        "InputDataConfig": InputDataConfigTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
     },
 )
 _OptionalImportJobPropertiesTypeDef = TypedDict(
     "_OptionalImportJobPropertiesTypeDef",
     {
         "JobName": str,
         "EndTime": datetime,
-        "JobOutputDataConfig": OutputDataConfigTypeDef,
+        "JobOutputDataConfig": OutputDataConfigOutputTypeDef,
         "DataAccessRoleArn": str,
         "Message": str,
     },
     total=False,
 )
 
+
 class ImportJobPropertiesTypeDef(
     _RequiredImportJobPropertiesTypeDef, _OptionalImportJobPropertiesTypeDef
 ):
     pass
 
+
 _RequiredStartFHIRExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartFHIRExportJobRequestRequestTypeDef",
     {
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DatastoreId": str,
         "DataAccessRoleArn": str,
         "ClientToken": str,
@@ -455,20 +571,22 @@
     "_OptionalStartFHIRExportJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
     total=False,
 )
 
+
 class StartFHIRExportJobRequestRequestTypeDef(
     _RequiredStartFHIRExportJobRequestRequestTypeDef,
     _OptionalStartFHIRExportJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartFHIRImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartFHIRImportJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "JobOutputDataConfig": OutputDataConfigTypeDef,
         "DatastoreId": str,
         "DataAccessRoleArn": str,
@@ -479,20 +597,22 @@
     "_OptionalStartFHIRImportJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
     total=False,
 )
 
+
 class StartFHIRImportJobRequestRequestTypeDef(
     _RequiredStartFHIRImportJobRequestRequestTypeDef,
     _OptionalStartFHIRImportJobRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeFHIRDatastoreResponseTypeDef = TypedDict(
     "DescribeFHIRDatastoreResponseTypeDef",
     {
         "DatastoreProperties": DatastorePropertiesTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake.egg-info/PKG-INFO` & `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-healthlake
-Version: 1.28.0
-Summary: Type annotations for boto3.HealthLake 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.HealthLake 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-healthlake"></a>
 
 # mypy-boto3-healthlake
 
 [![PyPI - mypy-boto3-healthlake](https://img.shields.io/pypi/v/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-healthlake?color=blue)](https://pypistats.org/packages/mypy-boto3-healthlake)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-healthlake)](https://pepy.tech/project/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,36 +306,44 @@
 ```python
 from mypy_boto3_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
     CreateFHIRDatastoreResponseTypeDef,
     DatastoreFilterTypeDef,
+    IdentityProviderConfigurationOutputTypeDef,
+    PreloadDataConfigOutputTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
     DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
+    KmsEncryptionConfigOutputTypeDef,
     KmsEncryptionConfigTypeDef,
     ListFHIRExportJobsRequestRequestTypeDef,
     ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     ResponseMetadataTypeDef,
     StartFHIRExportJobResponseTypeDef,
     StartFHIRImportJobResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListFHIRDatastoresRequestRequestTypeDef,
+    SseConfigurationOutputTypeDef,
     SseConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    OutputDataConfigOutputTypeDef,
     OutputDataConfigTypeDef,
-    CreateFHIRDatastoreRequestRequestTypeDef,
     DatastorePropertiesTypeDef,
+    CreateFHIRDatastoreRequestRequestTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
     StartFHIRExportJobRequestRequestTypeDef,
     StartFHIRImportJobRequestRequestTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
     ListFHIRDatastoresResponseTypeDef,
     DescribeFHIRExportJobResponseTypeDef,
```

### Comparing `mypy-boto3-healthlake-1.28.0/mypy_boto3_healthlake.egg-info/SOURCES.txt` & `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.28.0/setup.py` & `mypy-boto3-healthlake-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-healthlake",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_healthlake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.HealthLake 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.HealthLake 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

