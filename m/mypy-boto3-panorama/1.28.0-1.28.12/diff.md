# Comparing `tmp/mypy-boto3-panorama-1.28.0.tar.gz` & `tmp/mypy-boto3-panorama-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-panorama-1.28.0.tar", last modified: Thu Jul  6 21:00:16 2023, max compression
+gzip compressed data, was "mypy-boto3-panorama-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
```

## Comparing `mypy-boto3-panorama-1.28.0.tar` & `mypy-boto3-panorama-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:16.262388 mypy-boto3-panorama-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:00.000000 mypy-boto3-panorama-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-07-06 21:00:16.258388 mypy-boto3-panorama-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-07-06 20:49:00.000000 mypy-boto3-panorama-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:16.250388 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 20:49:00.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-06 20:49:00.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:49:00.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23775 2023-07-06 20:49:00.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23734 2023-07-06 20:49:00.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-07-06 20:49:01.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-07-06 20:49:00.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:00.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37354 2023-07-06 20:49:02.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37313 2023-07-06 20:49:01.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:00.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:16.258388 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-07-06 21:00:16.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 21:00:16.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:16.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:16.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:16.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:16.000000 mypy-boto3-panorama-1.28.0/mypy_boto3_panorama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:16.262388 mypy-boto3-panorama-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:49:00.000000 mypy-boto3-panorama-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.793132 mypy-boto3-panorama-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:10.000000 mypy-boto3-panorama-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16866 2023-07-27 11:49:21.793132 mypy-boto3-panorama-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15375 2023-07-27 11:41:10.000000 mypy-boto3-panorama-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.793132 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 11:41:10.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 11:41:10.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23775 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23734 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40902 2023-07-27 11:41:12.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40856 2023-07-27 11:41:11.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:10.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.793132 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16866 2023-07-27 11:49:21.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 11:49:21.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:21.000000 mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.793132 mypy-boto3-panorama-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:41:10.000000 mypy-boto3-panorama-1.28.12/setup.py
```

### Comparing `mypy-boto3-panorama-1.28.0/LICENSE` & `mypy-boto3-panorama-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.0/PKG-INFO` & `mypy-boto3-panorama-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-panorama
-Version: 1.28.0
-Summary: Type annotations for boto3.Panorama 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Panorama 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-panorama"></a>
 
 # mypy-boto3-panorama
 
 [![PyPI - mypy-boto3-panorama](https://img.shields.io/pypi/v/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-panorama?color=blue)](https://pypistats.org/packages/mypy-boto3-panorama)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-panorama)](https://pepy.tech/project/mypy-boto3-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Panorama 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[boto3.Panorama 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,39 +324,38 @@
 
 ```python
 from mypy_boto3_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    CreateApplicationInstanceResponseTypeDef,
+    ResponseMetadataTypeDef,
     JobTypeDef,
     JobResourceTagsTypeDef,
-    CreateNodeFromTemplateJobResponseTypeDef,
-    CreatePackageImportJobResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
-    DeleteDeviceResponseTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
+    ManifestOverridesPayloadOutputTypeDef,
+    ManifestPayloadOutputTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
-    DescribeDeviceJobResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
+    JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
-    DescribePackageVersionResponseTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
+    StaticIpConnectionInfoOutputTypeDef,
     StaticIpConnectionInfoTypeDef,
     EthernetStatusTypeDef,
     ListApplicationInstanceDependenciesRequestRequestTypeDef,
     PackageObjectTypeDef,
     ListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     NodeInstanceTypeDef,
     ListApplicationInstancesRequestRequestTypeDef,
@@ -367,67 +366,80 @@
     ListNodesRequestRequestTypeDef,
     NodeTypeDef,
     ListPackageImportJobsRequestRequestTypeDef,
     PackageImportJobTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageListItemTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    NtpPayloadOutputTypeDef,
     NtpPayloadTypeDef,
     NtpStatusTypeDef,
     NodeInputPortTypeDef,
     NodeOutputPortTypeDef,
     NodeSignalTypeDef,
     OutPutS3LocationTypeDef,
+    PackageVersionOutputConfigOutputTypeDef,
     PackageVersionOutputConfigTypeDef,
+    S3LocationOutputTypeDef,
     S3LocationTypeDef,
-    ProvisionDeviceResponseTypeDef,
     RegisterPackageVersionRequestRequestTypeDef,
     RemoveApplicationInstanceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SignalApplicationInstanceNodeInstancesResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceMetadataRequestRequestTypeDef,
-    UpdateDeviceMetadataResponseTypeDef,
     ApplicationInstanceTypeDef,
-    DescribeApplicationInstanceResponseTypeDef,
     CreateApplicationInstanceRequestRequestTypeDef,
-    DescribeApplicationInstanceDetailsResponseTypeDef,
+    CreateApplicationInstanceResponseTypeDef,
+    CreateNodeFromTemplateJobResponseTypeDef,
+    CreatePackageImportJobResponseTypeDef,
+    DeleteDeviceResponseTypeDef,
+    DescribeApplicationInstanceResponseTypeDef,
+    DescribeDeviceJobResponseTypeDef,
+    DescribePackageVersionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ProvisionDeviceResponseTypeDef,
+    SignalApplicationInstanceNodeInstancesResponseTypeDef,
+    UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
     CreateNodeFromTemplateJobRequestRequestTypeDef,
-    DescribeNodeFromTemplateJobResponseTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
+    DescribeApplicationInstanceDetailsResponseTypeDef,
     DeviceTypeDef,
+    DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
+    EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     NetworkStatusTypeDef,
     NodeInterfaceTypeDef,
     SignalApplicationInstanceNodeInstancesRequestRequestTypeDef,
     PackageImportJobOutputTypeDef,
+    PackageImportJobOutputConfigOutputTypeDef,
     PackageImportJobOutputConfigTypeDef,
+    PackageVersionInputConfigOutputTypeDef,
     PackageVersionInputConfigTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesResponseTypeDef,
     CreateJobForDevicesRequestRequestTypeDef,
+    NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
     DescribeNodeResponseTypeDef,
+    PackageImportJobInputConfigOutputTypeDef,
     PackageImportJobInputConfigTypeDef,
     DescribeDeviceResponseTypeDef,
     ProvisionDeviceRequestRequestTypeDef,
-    CreatePackageImportJobRequestRequestTypeDef,
     DescribePackageImportJobResponseTypeDef,
+    CreatePackageImportJobRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AlternateSoftwareMetadataTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-panorama-1.28.0/README.md` & `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-panorama
+Version: 1.28.12
+Summary: Type annotations for boto3.Panorama 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 panorama type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-panorama"></a>
 
 # mypy-boto3-panorama
 
 [![PyPI - mypy-boto3-panorama](https://img.shields.io/pypi/v/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-panorama?color=blue)](https://pypistats.org/packages/mypy-boto3-panorama)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-panorama)](https://pepy.tech/project/mypy-boto3-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Panorama 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[boto3.Panorama 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,39 +324,38 @@
 
 ```python
 from mypy_boto3_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    CreateApplicationInstanceResponseTypeDef,
+    ResponseMetadataTypeDef,
     JobTypeDef,
     JobResourceTagsTypeDef,
-    CreateNodeFromTemplateJobResponseTypeDef,
-    CreatePackageImportJobResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
-    DeleteDeviceResponseTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
+    ManifestOverridesPayloadOutputTypeDef,
+    ManifestPayloadOutputTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
-    DescribeDeviceJobResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
+    JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
-    DescribePackageVersionResponseTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
+    StaticIpConnectionInfoOutputTypeDef,
     StaticIpConnectionInfoTypeDef,
     EthernetStatusTypeDef,
     ListApplicationInstanceDependenciesRequestRequestTypeDef,
     PackageObjectTypeDef,
     ListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     NodeInstanceTypeDef,
     ListApplicationInstancesRequestRequestTypeDef,
@@ -335,67 +366,80 @@
     ListNodesRequestRequestTypeDef,
     NodeTypeDef,
     ListPackageImportJobsRequestRequestTypeDef,
     PackageImportJobTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageListItemTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    NtpPayloadOutputTypeDef,
     NtpPayloadTypeDef,
     NtpStatusTypeDef,
     NodeInputPortTypeDef,
     NodeOutputPortTypeDef,
     NodeSignalTypeDef,
     OutPutS3LocationTypeDef,
+    PackageVersionOutputConfigOutputTypeDef,
     PackageVersionOutputConfigTypeDef,
+    S3LocationOutputTypeDef,
     S3LocationTypeDef,
-    ProvisionDeviceResponseTypeDef,
     RegisterPackageVersionRequestRequestTypeDef,
     RemoveApplicationInstanceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SignalApplicationInstanceNodeInstancesResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceMetadataRequestRequestTypeDef,
-    UpdateDeviceMetadataResponseTypeDef,
     ApplicationInstanceTypeDef,
-    DescribeApplicationInstanceResponseTypeDef,
     CreateApplicationInstanceRequestRequestTypeDef,
-    DescribeApplicationInstanceDetailsResponseTypeDef,
+    CreateApplicationInstanceResponseTypeDef,
+    CreateNodeFromTemplateJobResponseTypeDef,
+    CreatePackageImportJobResponseTypeDef,
+    DeleteDeviceResponseTypeDef,
+    DescribeApplicationInstanceResponseTypeDef,
+    DescribeDeviceJobResponseTypeDef,
+    DescribePackageVersionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ProvisionDeviceResponseTypeDef,
+    SignalApplicationInstanceNodeInstancesResponseTypeDef,
+    UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
     CreateNodeFromTemplateJobRequestRequestTypeDef,
-    DescribeNodeFromTemplateJobResponseTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
+    DescribeApplicationInstanceDetailsResponseTypeDef,
     DeviceTypeDef,
+    DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
+    EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     NetworkStatusTypeDef,
     NodeInterfaceTypeDef,
     SignalApplicationInstanceNodeInstancesRequestRequestTypeDef,
     PackageImportJobOutputTypeDef,
+    PackageImportJobOutputConfigOutputTypeDef,
     PackageImportJobOutputConfigTypeDef,
+    PackageVersionInputConfigOutputTypeDef,
     PackageVersionInputConfigTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesResponseTypeDef,
     CreateJobForDevicesRequestRequestTypeDef,
+    NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
     DescribeNodeResponseTypeDef,
+    PackageImportJobInputConfigOutputTypeDef,
     PackageImportJobInputConfigTypeDef,
     DescribeDeviceResponseTypeDef,
     ProvisionDeviceRequestRequestTypeDef,
-    CreatePackageImportJobRequestRequestTypeDef,
     DescribePackageImportJobResponseTypeDef,
+    CreatePackageImportJobRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AlternateSoftwareMetadataTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/__main__.py` & `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Panorama 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Panorama 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama\nOther"
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

### Comparing `mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/client.py` & `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/client.pyi` & `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/literals.py` & `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,14 +243,15 @@
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
@@ -329,26 +330,28 @@
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

### Comparing `mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/literals.pyi` & `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,15 @@
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
@@ -327,26 +328,28 @@
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

### Comparing `mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/type_defs.py` & `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,39 +53,38 @@
 
 
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
-    "CreateApplicationInstanceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "JobTypeDef",
     "JobResourceTagsTypeDef",
-    "CreateNodeFromTemplateJobResponseTypeDef",
-    "CreatePackageImportJobResponseTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
-    "DeleteDeviceResponseTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
+    "ManifestOverridesPayloadOutputTypeDef",
+    "ManifestPayloadOutputTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
-    "DescribeDeviceJobResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
+    "JobResourceTagsOutputTypeDef",
     "DescribeNodeRequestRequestTypeDef",
     "DescribePackageImportJobRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
-    "DescribePackageVersionResponseTypeDef",
     "OTAJobConfigTypeDef",
     "DeviceJobTypeDef",
+    "StaticIpConnectionInfoOutputTypeDef",
     "StaticIpConnectionInfoTypeDef",
     "EthernetStatusTypeDef",
     "ListApplicationInstanceDependenciesRequestRequestTypeDef",
     "PackageObjectTypeDef",
     "ListApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "NodeInstanceTypeDef",
     "ListApplicationInstancesRequestRequestTypeDef",
@@ -96,67 +95,80 @@
     "ListNodesRequestRequestTypeDef",
     "NodeTypeDef",
     "ListPackageImportJobsRequestRequestTypeDef",
     "PackageImportJobTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "PackageListItemTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "NtpPayloadOutputTypeDef",
     "NtpPayloadTypeDef",
     "NtpStatusTypeDef",
     "NodeInputPortTypeDef",
     "NodeOutputPortTypeDef",
     "NodeSignalTypeDef",
     "OutPutS3LocationTypeDef",
+    "PackageVersionOutputConfigOutputTypeDef",
     "PackageVersionOutputConfigTypeDef",
+    "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
-    "ProvisionDeviceResponseTypeDef",
     "RegisterPackageVersionRequestRequestTypeDef",
     "RemoveApplicationInstanceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceMetadataRequestRequestTypeDef",
-    "UpdateDeviceMetadataResponseTypeDef",
     "ApplicationInstanceTypeDef",
-    "DescribeApplicationInstanceResponseTypeDef",
     "CreateApplicationInstanceRequestRequestTypeDef",
-    "DescribeApplicationInstanceDetailsResponseTypeDef",
+    "CreateApplicationInstanceResponseTypeDef",
+    "CreateNodeFromTemplateJobResponseTypeDef",
+    "CreatePackageImportJobResponseTypeDef",
+    "DeleteDeviceResponseTypeDef",
+    "DescribeApplicationInstanceResponseTypeDef",
+    "DescribeDeviceJobResponseTypeDef",
+    "DescribePackageVersionResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ProvisionDeviceResponseTypeDef",
+    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
+    "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
     "CreateNodeFromTemplateJobRequestRequestTypeDef",
-    "DescribeNodeFromTemplateJobResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
+    "DescribeApplicationInstanceDetailsResponseTypeDef",
     "DeviceTypeDef",
+    "DescribeNodeFromTemplateJobResponseTypeDef",
     "DeviceJobConfigTypeDef",
     "ListDevicesJobsResponseTypeDef",
+    "EthernetPayloadOutputTypeDef",
     "EthernetPayloadTypeDef",
     "ListApplicationInstanceDependenciesResponseTypeDef",
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     "ListNodeFromTemplateJobsResponseTypeDef",
     "ListNodesResponseTypeDef",
     "ListPackageImportJobsResponseTypeDef",
     "ListPackagesResponseTypeDef",
     "NetworkStatusTypeDef",
     "NodeInterfaceTypeDef",
     "SignalApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "PackageImportJobOutputTypeDef",
+    "PackageImportJobOutputConfigOutputTypeDef",
     "PackageImportJobOutputConfigTypeDef",
+    "PackageVersionInputConfigOutputTypeDef",
     "PackageVersionInputConfigTypeDef",
     "ListApplicationInstancesResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "CreateJobForDevicesRequestRequestTypeDef",
+    "NetworkPayloadOutputTypeDef",
     "NetworkPayloadTypeDef",
     "DescribeNodeResponseTypeDef",
+    "PackageImportJobInputConfigOutputTypeDef",
     "PackageImportJobInputConfigTypeDef",
     "DescribeDeviceResponseTypeDef",
     "ProvisionDeviceRequestRequestTypeDef",
-    "CreatePackageImportJobRequestRequestTypeDef",
     "DescribePackageImportJobResponseTypeDef",
+    "CreatePackageImportJobRequestRequestTypeDef",
 )
 
 AlternateSoftwareMetadataTypeDef = TypedDict(
     "AlternateSoftwareMetadataTypeDef",
     {
         "Version": str,
     },
@@ -185,19 +197,22 @@
     "ManifestPayloadTypeDef",
     {
         "PayloadData": str,
     },
     total=False,
 )
 
-CreateApplicationInstanceResponseTypeDef = TypedDict(
-    "CreateApplicationInstanceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApplicationInstanceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "DeviceId": str,
@@ -210,30 +225,14 @@
     "JobResourceTagsTypeDef",
     {
         "ResourceType": Literal["PACKAGE"],
         "Tags": Mapping[str, str],
     },
 )
 
-CreateNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "CreateNodeFromTemplateJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePackageImportJobResponseTypeDef = TypedDict(
-    "CreatePackageImportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "PackageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
@@ -265,22 +264,14 @@
 DeleteDeviceRequestRequestTypeDef = TypedDict(
     "DeleteDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-DeleteDeviceResponseTypeDef = TypedDict(
-    "DeleteDeviceResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeletePackageRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePackageRequestRequestTypeDef",
     {
         "PackageId": str,
     },
 )
 _OptionalDeletePackageRequestRequestTypeDef = TypedDict(
@@ -326,44 +317,44 @@
 DescribeApplicationInstanceDetailsRequestRequestTypeDef = TypedDict(
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
+ManifestOverridesPayloadOutputTypeDef = TypedDict(
+    "ManifestOverridesPayloadOutputTypeDef",
+    {
+        "PayloadData": str,
+    },
+    total=False,
+)
+
+ManifestPayloadOutputTypeDef = TypedDict(
+    "ManifestPayloadOutputTypeDef",
+    {
+        "PayloadData": str,
+    },
+    total=False,
+)
+
 DescribeApplicationInstanceRequestRequestTypeDef = TypedDict(
     "DescribeApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
 DescribeDeviceJobRequestRequestTypeDef = TypedDict(
     "DescribeDeviceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-DescribeDeviceJobResponseTypeDef = TypedDict(
-    "DescribeDeviceJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "DeviceArn": str,
-        "DeviceId": str,
-        "DeviceName": str,
-        "DeviceType": DeviceTypeType,
-        "ImageVersion": str,
-        "JobId": str,
-        "JobType": JobTypeType,
-        "Status": UpdateProgressType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
@@ -380,14 +371,22 @@
 DescribeNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+JobResourceTagsOutputTypeDef = TypedDict(
+    "JobResourceTagsOutputTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Dict[str, str],
+    },
+)
+
 _RequiredDescribeNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeRequestRequestTypeDef",
     {
         "NodeId": str,
     },
 )
 _OptionalDescribeNodeRequestRequestTypeDef = TypedDict(
@@ -439,31 +438,14 @@
 class DescribePackageVersionRequestRequestTypeDef(
     _RequiredDescribePackageVersionRequestRequestTypeDef,
     _OptionalDescribePackageVersionRequestRequestTypeDef,
 ):
     pass
 
 
-DescribePackageVersionResponseTypeDef = TypedDict(
-    "DescribePackageVersionResponseTypeDef",
-    {
-        "IsLatestPatch": bool,
-        "OwnerAccount": str,
-        "PackageArn": str,
-        "PackageId": str,
-        "PackageName": str,
-        "PackageVersion": str,
-        "PatchVersion": str,
-        "RegisteredTime": datetime,
-        "Status": PackageVersionStatusType,
-        "StatusDescription": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredOTAJobConfigTypeDef = TypedDict(
     "_RequiredOTAJobConfigTypeDef",
     {
         "ImageVersion": str,
     },
 )
 _OptionalOTAJobConfigTypeDef = TypedDict(
@@ -487,19 +469,29 @@
         "DeviceName": str,
         "JobId": str,
         "JobType": JobTypeType,
     },
     total=False,
 )
 
+StaticIpConnectionInfoOutputTypeDef = TypedDict(
+    "StaticIpConnectionInfoOutputTypeDef",
+    {
+        "DefaultGateway": str,
+        "Dns": List[str],
+        "IpAddress": str,
+        "Mask": str,
+    },
+)
+
 StaticIpConnectionInfoTypeDef = TypedDict(
     "StaticIpConnectionInfoTypeDef",
     {
         "DefaultGateway": str,
-        "Dns": List[str],
+        "Dns": Sequence[str],
         "IpAddress": str,
         "Mask": str,
     },
 )
 
 EthernetStatusTypeDef = TypedDict(
     "EthernetStatusTypeDef",
@@ -734,26 +726,25 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+NtpPayloadOutputTypeDef = TypedDict(
+    "NtpPayloadOutputTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NtpServers": List[str],
     },
 )
 
 NtpPayloadTypeDef = TypedDict(
     "NtpPayloadTypeDef",
     {
-        "NtpServers": List[str],
+        "NtpServers": Sequence[str],
     },
 )
 
 NtpStatusTypeDef = TypedDict(
     "NtpStatusTypeDef",
     {
         "ConnectionStatus": NetworkConnectionStatusType,
@@ -797,14 +788,37 @@
     "OutPutS3LocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
 )
 
+_RequiredPackageVersionOutputConfigOutputTypeDef = TypedDict(
+    "_RequiredPackageVersionOutputConfigOutputTypeDef",
+    {
+        "PackageName": str,
+        "PackageVersion": str,
+    },
+)
+_OptionalPackageVersionOutputConfigOutputTypeDef = TypedDict(
+    "_OptionalPackageVersionOutputConfigOutputTypeDef",
+    {
+        "MarkLatest": bool,
+    },
+    total=False,
+)
+
+
+class PackageVersionOutputConfigOutputTypeDef(
+    _RequiredPackageVersionOutputConfigOutputTypeDef,
+    _OptionalPackageVersionOutputConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredPackageVersionOutputConfigTypeDef = TypedDict(
     "_RequiredPackageVersionOutputConfigTypeDef",
     {
         "PackageName": str,
         "PackageVersion": str,
     },
 )
@@ -819,14 +833,34 @@
 
 class PackageVersionOutputConfigTypeDef(
     _RequiredPackageVersionOutputConfigTypeDef, _OptionalPackageVersionOutputConfigTypeDef
 ):
     pass
 
 
+_RequiredS3LocationOutputTypeDef = TypedDict(
+    "_RequiredS3LocationOutputTypeDef",
+    {
+        "BucketName": str,
+        "ObjectKey": str,
+    },
+)
+_OptionalS3LocationOutputTypeDef = TypedDict(
+    "_OptionalS3LocationOutputTypeDef",
+    {
+        "Region": str,
+    },
+    total=False,
+)
+
+
+class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
+    pass
+
+
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
 )
@@ -839,26 +873,14 @@
 )
 
 
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
 
-ProvisionDeviceResponseTypeDef = TypedDict(
-    "ProvisionDeviceResponseTypeDef",
-    {
-        "Arn": str,
-        "Certificates": bytes,
-        "DeviceId": str,
-        "IotThingName": str,
-        "Status": DeviceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -883,33 +905,14 @@
 RemoveApplicationInstanceRequestRequestTypeDef = TypedDict(
     "RemoveApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
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
-SignalApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
-    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -940,22 +943,14 @@
 class UpdateDeviceMetadataRequestRequestTypeDef(
     _RequiredUpdateDeviceMetadataRequestRequestTypeDef,
     _OptionalUpdateDeviceMetadataRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateDeviceMetadataResponseTypeDef = TypedDict(
-    "UpdateDeviceMetadataResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ApplicationInstanceTypeDef = TypedDict(
     "ApplicationInstanceTypeDef",
     {
         "ApplicationInstanceId": str,
         "Arn": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
@@ -967,36 +962,14 @@
         "Status": ApplicationInstanceStatusType,
         "StatusDescription": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-DescribeApplicationInstanceResponseTypeDef = TypedDict(
-    "DescribeApplicationInstanceResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ApplicationInstanceIdToReplace": str,
-        "Arn": str,
-        "CreatedTime": datetime,
-        "DefaultRuntimeContextDevice": str,
-        "DefaultRuntimeContextDeviceName": str,
-        "Description": str,
-        "HealthStatus": ApplicationInstanceHealthStatusType,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "RuntimeContextStates": List[ReportedRuntimeContextStateTypeDef],
-        "RuntimeRoleArn": str,
-        "Status": ApplicationInstanceStatusType,
-        "StatusDescription": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateApplicationInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationInstanceRequestRequestTypeDef",
     {
         "DefaultRuntimeContextDevice": str,
         "ManifestPayload": ManifestPayloadTypeDef,
     },
 )
@@ -1017,34 +990,142 @@
 class CreateApplicationInstanceRequestRequestTypeDef(
     _RequiredCreateApplicationInstanceRequestRequestTypeDef,
     _OptionalCreateApplicationInstanceRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeApplicationInstanceDetailsResponseTypeDef = TypedDict(
-    "DescribeApplicationInstanceDetailsResponseTypeDef",
+CreateApplicationInstanceResponseTypeDef = TypedDict(
+    "CreateApplicationInstanceResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "CreateNodeFromTemplateJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePackageImportJobResponseTypeDef = TypedDict(
+    "CreatePackageImportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDeviceResponseTypeDef = TypedDict(
+    "DeleteDeviceResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeApplicationInstanceResponseTypeDef = TypedDict(
+    "DescribeApplicationInstanceResponseTypeDef",
     {
         "ApplicationInstanceId": str,
         "ApplicationInstanceIdToReplace": str,
+        "Arn": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
+        "DefaultRuntimeContextDeviceName": str,
         "Description": str,
-        "ManifestOverridesPayload": ManifestOverridesPayloadTypeDef,
-        "ManifestPayload": ManifestPayloadTypeDef,
+        "HealthStatus": ApplicationInstanceHealthStatusType,
+        "LastUpdatedTime": datetime,
         "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RuntimeContextStates": List[ReportedRuntimeContextStateTypeDef],
+        "RuntimeRoleArn": str,
+        "Status": ApplicationInstanceStatusType,
+        "StatusDescription": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDeviceJobResponseTypeDef = TypedDict(
+    "DescribeDeviceJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "DeviceArn": str,
+        "DeviceId": str,
+        "DeviceName": str,
+        "DeviceType": DeviceTypeType,
+        "ImageVersion": str,
+        "JobId": str,
+        "JobType": JobTypeType,
+        "Status": UpdateProgressType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePackageVersionResponseTypeDef = TypedDict(
+    "DescribePackageVersionResponseTypeDef",
+    {
+        "IsLatestPatch": bool,
+        "OwnerAccount": str,
+        "PackageArn": str,
+        "PackageId": str,
+        "PackageName": str,
+        "PackageVersion": str,
+        "PatchVersion": str,
+        "RegisteredTime": datetime,
+        "Status": PackageVersionStatusType,
+        "StatusDescription": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProvisionDeviceResponseTypeDef = TypedDict(
+    "ProvisionDeviceResponseTypeDef",
+    {
+        "Arn": str,
+        "Certificates": bytes,
+        "DeviceId": str,
+        "IotThingName": str,
+        "Status": DeviceStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SignalApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
+    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDeviceMetadataResponseTypeDef = TypedDict(
+    "UpdateDeviceMetadataResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJobForDevicesResponseTypeDef = TypedDict(
     "CreateJobForDevicesResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
     {
         "NodeName": str,
@@ -1067,55 +1148,51 @@
 class CreateNodeFromTemplateJobRequestRequestTypeDef(
     _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
     _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "DescribeNodeFromTemplateJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsTypeDef],
-        "LastUpdatedTime": datetime,
-        "NodeDescription": str,
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "Status": NodeFromTemplateJobStatusType,
-        "StatusMessage": str,
-        "TemplateParameters": Dict[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "Arn": str,
         "PackageId": str,
         "StorageLocation": StorageLocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackageResponseTypeDef = TypedDict(
     "DescribePackageResponseTypeDef",
     {
         "Arn": str,
         "CreatedTime": datetime,
         "PackageId": str,
         "PackageName": str,
         "ReadAccessPrincipalArns": List[str],
         "StorageLocation": StorageLocationTypeDef,
         "Tags": Dict[str, str],
         "WriteAccessPrincipalArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeApplicationInstanceDetailsResponseTypeDef = TypedDict(
+    "DescribeApplicationInstanceDetailsResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ApplicationInstanceIdToReplace": str,
+        "CreatedTime": datetime,
+        "DefaultRuntimeContextDevice": str,
+        "Description": str,
+        "ManifestOverridesPayload": ManifestOverridesPayloadOutputTypeDef,
+        "ManifestPayload": ManifestPayloadOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "Brand": DeviceBrandType,
@@ -1131,31 +1208,71 @@
         "ProvisioningStatus": DeviceStatusType,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
     },
     total=False,
 )
 
+DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "DescribeNodeFromTemplateJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "LastUpdatedTime": datetime,
+        "NodeDescription": str,
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "Status": NodeFromTemplateJobStatusType,
+        "StatusMessage": str,
+        "TemplateParameters": Dict[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeviceJobConfigTypeDef = TypedDict(
     "DeviceJobConfigTypeDef",
     {
         "OTAJobConfig": OTAJobConfigTypeDef,
     },
     total=False,
 )
 
 ListDevicesJobsResponseTypeDef = TypedDict(
     "ListDevicesJobsResponseTypeDef",
     {
         "DeviceJobs": List[DeviceJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredEthernetPayloadOutputTypeDef = TypedDict(
+    "_RequiredEthernetPayloadOutputTypeDef",
+    {
+        "ConnectionType": ConnectionTypeType,
+    },
+)
+_OptionalEthernetPayloadOutputTypeDef = TypedDict(
+    "_OptionalEthernetPayloadOutputTypeDef",
+    {
+        "StaticIpConnectionInfo": StaticIpConnectionInfoOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class EthernetPayloadOutputTypeDef(
+    _RequiredEthernetPayloadOutputTypeDef, _OptionalEthernetPayloadOutputTypeDef
+):
+    pass
+
+
 _RequiredEthernetPayloadTypeDef = TypedDict(
     "_RequiredEthernetPayloadTypeDef",
     {
         "ConnectionType": ConnectionTypeType,
     },
 )
 _OptionalEthernetPayloadTypeDef = TypedDict(
@@ -1172,60 +1289,60 @@
 
 
 ListApplicationInstanceDependenciesResponseTypeDef = TypedDict(
     "ListApplicationInstanceDependenciesResponseTypeDef",
     {
         "NextToken": str,
         "PackageObjects": List[PackageObjectTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     {
         "NextToken": str,
         "NodeInstances": List[NodeInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNodeFromTemplateJobsResponseTypeDef = TypedDict(
     "ListNodeFromTemplateJobsResponseTypeDef",
     {
         "NextToken": str,
         "NodeFromTemplateJobs": List[NodeFromTemplateJobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
         "NextToken": str,
         "Nodes": List[NodeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackageImportJobsResponseTypeDef = TypedDict(
     "ListPackageImportJobsResponseTypeDef",
     {
         "NextToken": str,
         "PackageImportJobs": List[PackageImportJobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesResponseTypeDef = TypedDict(
     "ListPackagesResponseTypeDef",
     {
         "NextToken": str,
         "Packages": List[PackageListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkStatusTypeDef = TypedDict(
     "NetworkStatusTypeDef",
     {
         "Ethernet0Status": EthernetStatusTypeDef,
@@ -1258,44 +1375,59 @@
         "OutputS3Location": OutPutS3LocationTypeDef,
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
 )
 
+PackageImportJobOutputConfigOutputTypeDef = TypedDict(
+    "PackageImportJobOutputConfigOutputTypeDef",
+    {
+        "PackageVersionOutputConfig": PackageVersionOutputConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 PackageImportJobOutputConfigTypeDef = TypedDict(
     "PackageImportJobOutputConfigTypeDef",
     {
         "PackageVersionOutputConfig": PackageVersionOutputConfigTypeDef,
     },
     total=False,
 )
 
+PackageVersionInputConfigOutputTypeDef = TypedDict(
+    "PackageVersionInputConfigOutputTypeDef",
+    {
+        "S3Location": S3LocationOutputTypeDef,
+    },
+)
+
 PackageVersionInputConfigTypeDef = TypedDict(
     "PackageVersionInputConfigTypeDef",
     {
         "S3Location": S3LocationTypeDef,
     },
 )
 
 ListApplicationInstancesResponseTypeDef = TypedDict(
     "ListApplicationInstancesResponseTypeDef",
     {
         "ApplicationInstances": List[ApplicationInstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateJobForDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobForDevicesRequestRequestTypeDef",
     {
         "DeviceIds": Sequence[str],
@@ -1314,14 +1446,24 @@
 class CreateJobForDevicesRequestRequestTypeDef(
     _RequiredCreateJobForDevicesRequestRequestTypeDef,
     _OptionalCreateJobForDevicesRequestRequestTypeDef,
 ):
     pass
 
 
+NetworkPayloadOutputTypeDef = TypedDict(
+    "NetworkPayloadOutputTypeDef",
+    {
+        "Ethernet0": EthernetPayloadOutputTypeDef,
+        "Ethernet1": EthernetPayloadOutputTypeDef,
+        "Ntp": NtpPayloadOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkPayloadTypeDef = TypedDict(
     "NetworkPayloadTypeDef",
     {
         "Ethernet0": EthernetPayloadTypeDef,
         "Ethernet1": EthernetPayloadTypeDef,
         "Ntp": NtpPayloadTypeDef,
     },
@@ -1341,18 +1483,26 @@
         "NodeInterface": NodeInterfaceTypeDef,
         "OwnerAccount": str,
         "PackageArn": str,
         "PackageId": str,
         "PackageName": str,
         "PackageVersion": str,
         "PatchVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PackageImportJobInputConfigOutputTypeDef = TypedDict(
+    "PackageImportJobInputConfigOutputTypeDef",
+    {
+        "PackageVersionInputConfig": PackageVersionInputConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 PackageImportJobInputConfigTypeDef = TypedDict(
     "PackageImportJobInputConfigTypeDef",
     {
         "PackageVersionInputConfig": PackageVersionInputConfigTypeDef,
     },
     total=False,
 )
@@ -1371,20 +1521,20 @@
         "DeviceConnectionStatus": DeviceConnectionStatusType,
         "DeviceId": str,
         "LatestAlternateSoftware": str,
         "LatestDeviceJob": LatestDeviceJobTypeDef,
         "LatestSoftware": str,
         "LeaseExpirationTime": datetime,
         "Name": str,
-        "NetworkingConfiguration": NetworkPayloadTypeDef,
+        "NetworkingConfiguration": NetworkPayloadOutputTypeDef,
         "ProvisioningStatus": DeviceStatusType,
         "SerialNumber": str,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredProvisionDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionDeviceRequestRequestTypeDef",
     {
         "Name": str,
@@ -1403,14 +1553,32 @@
 
 class ProvisionDeviceRequestRequestTypeDef(
     _RequiredProvisionDeviceRequestRequestTypeDef, _OptionalProvisionDeviceRequestRequestTypeDef
 ):
     pass
 
 
+DescribePackageImportJobResponseTypeDef = TypedDict(
+    "DescribePackageImportJobResponseTypeDef",
+    {
+        "ClientToken": str,
+        "CreatedTime": datetime,
+        "InputConfig": PackageImportJobInputConfigOutputTypeDef,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "JobType": PackageImportJobTypeType,
+        "LastUpdatedTime": datetime,
+        "Output": PackageImportJobOutputTypeDef,
+        "OutputConfig": PackageImportJobOutputConfigOutputTypeDef,
+        "Status": PackageImportJobStatusType,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageImportJobRequestRequestTypeDef",
     {
         "ClientToken": str,
         "InputConfig": PackageImportJobInputConfigTypeDef,
         "JobType": PackageImportJobTypeType,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
@@ -1426,26 +1594,7 @@
 
 
 class CreatePackageImportJobRequestRequestTypeDef(
     _RequiredCreatePackageImportJobRequestRequestTypeDef,
     _OptionalCreatePackageImportJobRequestRequestTypeDef,
 ):
     pass
-
-
-DescribePackageImportJobResponseTypeDef = TypedDict(
-    "DescribePackageImportJobResponseTypeDef",
-    {
-        "ClientToken": str,
-        "CreatedTime": datetime,
-        "InputConfig": PackageImportJobInputConfigTypeDef,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsTypeDef],
-        "JobType": PackageImportJobTypeType,
-        "LastUpdatedTime": datetime,
-        "Output": PackageImportJobOutputTypeDef,
-        "OutputConfig": PackageImportJobOutputConfigTypeDef,
-        "Status": PackageImportJobStatusType,
-        "StatusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-panorama-1.28.0/mypy_boto3_panorama/type_defs.pyi` & `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -52,39 +52,38 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
-    "CreateApplicationInstanceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "JobTypeDef",
     "JobResourceTagsTypeDef",
-    "CreateNodeFromTemplateJobResponseTypeDef",
-    "CreatePackageImportJobResponseTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
-    "DeleteDeviceResponseTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
+    "ManifestOverridesPayloadOutputTypeDef",
+    "ManifestPayloadOutputTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
-    "DescribeDeviceJobResponseTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
+    "JobResourceTagsOutputTypeDef",
     "DescribeNodeRequestRequestTypeDef",
     "DescribePackageImportJobRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
-    "DescribePackageVersionResponseTypeDef",
     "OTAJobConfigTypeDef",
     "DeviceJobTypeDef",
+    "StaticIpConnectionInfoOutputTypeDef",
     "StaticIpConnectionInfoTypeDef",
     "EthernetStatusTypeDef",
     "ListApplicationInstanceDependenciesRequestRequestTypeDef",
     "PackageObjectTypeDef",
     "ListApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "NodeInstanceTypeDef",
     "ListApplicationInstancesRequestRequestTypeDef",
@@ -95,67 +94,80 @@
     "ListNodesRequestRequestTypeDef",
     "NodeTypeDef",
     "ListPackageImportJobsRequestRequestTypeDef",
     "PackageImportJobTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "PackageListItemTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "NtpPayloadOutputTypeDef",
     "NtpPayloadTypeDef",
     "NtpStatusTypeDef",
     "NodeInputPortTypeDef",
     "NodeOutputPortTypeDef",
     "NodeSignalTypeDef",
     "OutPutS3LocationTypeDef",
+    "PackageVersionOutputConfigOutputTypeDef",
     "PackageVersionOutputConfigTypeDef",
+    "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
-    "ProvisionDeviceResponseTypeDef",
     "RegisterPackageVersionRequestRequestTypeDef",
     "RemoveApplicationInstanceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceMetadataRequestRequestTypeDef",
-    "UpdateDeviceMetadataResponseTypeDef",
     "ApplicationInstanceTypeDef",
-    "DescribeApplicationInstanceResponseTypeDef",
     "CreateApplicationInstanceRequestRequestTypeDef",
-    "DescribeApplicationInstanceDetailsResponseTypeDef",
+    "CreateApplicationInstanceResponseTypeDef",
+    "CreateNodeFromTemplateJobResponseTypeDef",
+    "CreatePackageImportJobResponseTypeDef",
+    "DeleteDeviceResponseTypeDef",
+    "DescribeApplicationInstanceResponseTypeDef",
+    "DescribeDeviceJobResponseTypeDef",
+    "DescribePackageVersionResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ProvisionDeviceResponseTypeDef",
+    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
+    "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
     "CreateNodeFromTemplateJobRequestRequestTypeDef",
-    "DescribeNodeFromTemplateJobResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
+    "DescribeApplicationInstanceDetailsResponseTypeDef",
     "DeviceTypeDef",
+    "DescribeNodeFromTemplateJobResponseTypeDef",
     "DeviceJobConfigTypeDef",
     "ListDevicesJobsResponseTypeDef",
+    "EthernetPayloadOutputTypeDef",
     "EthernetPayloadTypeDef",
     "ListApplicationInstanceDependenciesResponseTypeDef",
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     "ListNodeFromTemplateJobsResponseTypeDef",
     "ListNodesResponseTypeDef",
     "ListPackageImportJobsResponseTypeDef",
     "ListPackagesResponseTypeDef",
     "NetworkStatusTypeDef",
     "NodeInterfaceTypeDef",
     "SignalApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "PackageImportJobOutputTypeDef",
+    "PackageImportJobOutputConfigOutputTypeDef",
     "PackageImportJobOutputConfigTypeDef",
+    "PackageVersionInputConfigOutputTypeDef",
     "PackageVersionInputConfigTypeDef",
     "ListApplicationInstancesResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "CreateJobForDevicesRequestRequestTypeDef",
+    "NetworkPayloadOutputTypeDef",
     "NetworkPayloadTypeDef",
     "DescribeNodeResponseTypeDef",
+    "PackageImportJobInputConfigOutputTypeDef",
     "PackageImportJobInputConfigTypeDef",
     "DescribeDeviceResponseTypeDef",
     "ProvisionDeviceRequestRequestTypeDef",
-    "CreatePackageImportJobRequestRequestTypeDef",
     "DescribePackageImportJobResponseTypeDef",
+    "CreatePackageImportJobRequestRequestTypeDef",
 )
 
 AlternateSoftwareMetadataTypeDef = TypedDict(
     "AlternateSoftwareMetadataTypeDef",
     {
         "Version": str,
     },
@@ -184,19 +196,22 @@
     "ManifestPayloadTypeDef",
     {
         "PayloadData": str,
     },
     total=False,
 )
 
-CreateApplicationInstanceResponseTypeDef = TypedDict(
-    "CreateApplicationInstanceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApplicationInstanceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "DeviceId": str,
@@ -209,30 +224,14 @@
     "JobResourceTagsTypeDef",
     {
         "ResourceType": Literal["PACKAGE"],
         "Tags": Mapping[str, str],
     },
 )
 
-CreateNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "CreateNodeFromTemplateJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePackageImportJobResponseTypeDef = TypedDict(
-    "CreatePackageImportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "PackageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
@@ -262,22 +261,14 @@
 DeleteDeviceRequestRequestTypeDef = TypedDict(
     "DeleteDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-DeleteDeviceResponseTypeDef = TypedDict(
-    "DeleteDeviceResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeletePackageRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePackageRequestRequestTypeDef",
     {
         "PackageId": str,
     },
 )
 _OptionalDeletePackageRequestRequestTypeDef = TypedDict(
@@ -319,44 +310,44 @@
 DescribeApplicationInstanceDetailsRequestRequestTypeDef = TypedDict(
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
+ManifestOverridesPayloadOutputTypeDef = TypedDict(
+    "ManifestOverridesPayloadOutputTypeDef",
+    {
+        "PayloadData": str,
+    },
+    total=False,
+)
+
+ManifestPayloadOutputTypeDef = TypedDict(
+    "ManifestPayloadOutputTypeDef",
+    {
+        "PayloadData": str,
+    },
+    total=False,
+)
+
 DescribeApplicationInstanceRequestRequestTypeDef = TypedDict(
     "DescribeApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
 DescribeDeviceJobRequestRequestTypeDef = TypedDict(
     "DescribeDeviceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-DescribeDeviceJobResponseTypeDef = TypedDict(
-    "DescribeDeviceJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "DeviceArn": str,
-        "DeviceId": str,
-        "DeviceName": str,
-        "DeviceType": DeviceTypeType,
-        "ImageVersion": str,
-        "JobId": str,
-        "JobType": JobTypeType,
-        "Status": UpdateProgressType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
@@ -373,14 +364,22 @@
 DescribeNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+JobResourceTagsOutputTypeDef = TypedDict(
+    "JobResourceTagsOutputTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Dict[str, str],
+    },
+)
+
 _RequiredDescribeNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeRequestRequestTypeDef",
     {
         "NodeId": str,
     },
 )
 _OptionalDescribeNodeRequestRequestTypeDef = TypedDict(
@@ -428,31 +427,14 @@
 
 class DescribePackageVersionRequestRequestTypeDef(
     _RequiredDescribePackageVersionRequestRequestTypeDef,
     _OptionalDescribePackageVersionRequestRequestTypeDef,
 ):
     pass
 
-DescribePackageVersionResponseTypeDef = TypedDict(
-    "DescribePackageVersionResponseTypeDef",
-    {
-        "IsLatestPatch": bool,
-        "OwnerAccount": str,
-        "PackageArn": str,
-        "PackageId": str,
-        "PackageName": str,
-        "PackageVersion": str,
-        "PatchVersion": str,
-        "RegisteredTime": datetime,
-        "Status": PackageVersionStatusType,
-        "StatusDescription": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredOTAJobConfigTypeDef = TypedDict(
     "_RequiredOTAJobConfigTypeDef",
     {
         "ImageVersion": str,
     },
 )
 _OptionalOTAJobConfigTypeDef = TypedDict(
@@ -474,19 +456,29 @@
         "DeviceName": str,
         "JobId": str,
         "JobType": JobTypeType,
     },
     total=False,
 )
 
+StaticIpConnectionInfoOutputTypeDef = TypedDict(
+    "StaticIpConnectionInfoOutputTypeDef",
+    {
+        "DefaultGateway": str,
+        "Dns": List[str],
+        "IpAddress": str,
+        "Mask": str,
+    },
+)
+
 StaticIpConnectionInfoTypeDef = TypedDict(
     "StaticIpConnectionInfoTypeDef",
     {
         "DefaultGateway": str,
-        "Dns": List[str],
+        "Dns": Sequence[str],
         "IpAddress": str,
         "Mask": str,
     },
 )
 
 EthernetStatusTypeDef = TypedDict(
     "EthernetStatusTypeDef",
@@ -713,26 +705,25 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+NtpPayloadOutputTypeDef = TypedDict(
+    "NtpPayloadOutputTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NtpServers": List[str],
     },
 )
 
 NtpPayloadTypeDef = TypedDict(
     "NtpPayloadTypeDef",
     {
-        "NtpServers": List[str],
+        "NtpServers": Sequence[str],
     },
 )
 
 NtpStatusTypeDef = TypedDict(
     "NtpStatusTypeDef",
     {
         "ConnectionStatus": NetworkConnectionStatusType,
@@ -776,14 +767,35 @@
     "OutPutS3LocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
 )
 
+_RequiredPackageVersionOutputConfigOutputTypeDef = TypedDict(
+    "_RequiredPackageVersionOutputConfigOutputTypeDef",
+    {
+        "PackageName": str,
+        "PackageVersion": str,
+    },
+)
+_OptionalPackageVersionOutputConfigOutputTypeDef = TypedDict(
+    "_OptionalPackageVersionOutputConfigOutputTypeDef",
+    {
+        "MarkLatest": bool,
+    },
+    total=False,
+)
+
+class PackageVersionOutputConfigOutputTypeDef(
+    _RequiredPackageVersionOutputConfigOutputTypeDef,
+    _OptionalPackageVersionOutputConfigOutputTypeDef,
+):
+    pass
+
 _RequiredPackageVersionOutputConfigTypeDef = TypedDict(
     "_RequiredPackageVersionOutputConfigTypeDef",
     {
         "PackageName": str,
         "PackageVersion": str,
     },
 )
@@ -796,14 +808,32 @@
 )
 
 class PackageVersionOutputConfigTypeDef(
     _RequiredPackageVersionOutputConfigTypeDef, _OptionalPackageVersionOutputConfigTypeDef
 ):
     pass
 
+_RequiredS3LocationOutputTypeDef = TypedDict(
+    "_RequiredS3LocationOutputTypeDef",
+    {
+        "BucketName": str,
+        "ObjectKey": str,
+    },
+)
+_OptionalS3LocationOutputTypeDef = TypedDict(
+    "_OptionalS3LocationOutputTypeDef",
+    {
+        "Region": str,
+    },
+    total=False,
+)
+
+class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
+    pass
+
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
 )
@@ -814,26 +844,14 @@
     },
     total=False,
 )
 
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-ProvisionDeviceResponseTypeDef = TypedDict(
-    "ProvisionDeviceResponseTypeDef",
-    {
-        "Arn": str,
-        "Certificates": bytes,
-        "DeviceId": str,
-        "IotThingName": str,
-        "Status": DeviceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterPackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterPackageVersionRequestRequestTypeDef",
     {
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
@@ -856,33 +874,14 @@
 RemoveApplicationInstanceRequestRequestTypeDef = TypedDict(
     "RemoveApplicationInstanceRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 
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
-SignalApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
-    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -911,22 +910,14 @@
 
 class UpdateDeviceMetadataRequestRequestTypeDef(
     _RequiredUpdateDeviceMetadataRequestRequestTypeDef,
     _OptionalUpdateDeviceMetadataRequestRequestTypeDef,
 ):
     pass
 
-UpdateDeviceMetadataResponseTypeDef = TypedDict(
-    "UpdateDeviceMetadataResponseTypeDef",
-    {
-        "DeviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ApplicationInstanceTypeDef = TypedDict(
     "ApplicationInstanceTypeDef",
     {
         "ApplicationInstanceId": str,
         "Arn": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
@@ -938,36 +929,14 @@
         "Status": ApplicationInstanceStatusType,
         "StatusDescription": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-DescribeApplicationInstanceResponseTypeDef = TypedDict(
-    "DescribeApplicationInstanceResponseTypeDef",
-    {
-        "ApplicationInstanceId": str,
-        "ApplicationInstanceIdToReplace": str,
-        "Arn": str,
-        "CreatedTime": datetime,
-        "DefaultRuntimeContextDevice": str,
-        "DefaultRuntimeContextDeviceName": str,
-        "Description": str,
-        "HealthStatus": ApplicationInstanceHealthStatusType,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "RuntimeContextStates": List[ReportedRuntimeContextStateTypeDef],
-        "RuntimeRoleArn": str,
-        "Status": ApplicationInstanceStatusType,
-        "StatusDescription": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateApplicationInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationInstanceRequestRequestTypeDef",
     {
         "DefaultRuntimeContextDevice": str,
         "ManifestPayload": ManifestPayloadTypeDef,
     },
 )
@@ -986,34 +955,142 @@
 
 class CreateApplicationInstanceRequestRequestTypeDef(
     _RequiredCreateApplicationInstanceRequestRequestTypeDef,
     _OptionalCreateApplicationInstanceRequestRequestTypeDef,
 ):
     pass
 
-DescribeApplicationInstanceDetailsResponseTypeDef = TypedDict(
-    "DescribeApplicationInstanceDetailsResponseTypeDef",
+CreateApplicationInstanceResponseTypeDef = TypedDict(
+    "CreateApplicationInstanceResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "CreateNodeFromTemplateJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePackageImportJobResponseTypeDef = TypedDict(
+    "CreatePackageImportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDeviceResponseTypeDef = TypedDict(
+    "DeleteDeviceResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeApplicationInstanceResponseTypeDef = TypedDict(
+    "DescribeApplicationInstanceResponseTypeDef",
     {
         "ApplicationInstanceId": str,
         "ApplicationInstanceIdToReplace": str,
+        "Arn": str,
         "CreatedTime": datetime,
         "DefaultRuntimeContextDevice": str,
+        "DefaultRuntimeContextDeviceName": str,
         "Description": str,
-        "ManifestOverridesPayload": ManifestOverridesPayloadTypeDef,
-        "ManifestPayload": ManifestPayloadTypeDef,
+        "HealthStatus": ApplicationInstanceHealthStatusType,
+        "LastUpdatedTime": datetime,
         "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RuntimeContextStates": List[ReportedRuntimeContextStateTypeDef],
+        "RuntimeRoleArn": str,
+        "Status": ApplicationInstanceStatusType,
+        "StatusDescription": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDeviceJobResponseTypeDef = TypedDict(
+    "DescribeDeviceJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "DeviceArn": str,
+        "DeviceId": str,
+        "DeviceName": str,
+        "DeviceType": DeviceTypeType,
+        "ImageVersion": str,
+        "JobId": str,
+        "JobType": JobTypeType,
+        "Status": UpdateProgressType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePackageVersionResponseTypeDef = TypedDict(
+    "DescribePackageVersionResponseTypeDef",
+    {
+        "IsLatestPatch": bool,
+        "OwnerAccount": str,
+        "PackageArn": str,
+        "PackageId": str,
+        "PackageName": str,
+        "PackageVersion": str,
+        "PatchVersion": str,
+        "RegisteredTime": datetime,
+        "Status": PackageVersionStatusType,
+        "StatusDescription": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ProvisionDeviceResponseTypeDef = TypedDict(
+    "ProvisionDeviceResponseTypeDef",
+    {
+        "Arn": str,
+        "Certificates": bytes,
+        "DeviceId": str,
+        "IotThingName": str,
+        "Status": DeviceStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SignalApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
+    "SignalApplicationInstanceNodeInstancesResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDeviceMetadataResponseTypeDef = TypedDict(
+    "UpdateDeviceMetadataResponseTypeDef",
+    {
+        "DeviceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJobForDevicesResponseTypeDef = TypedDict(
     "CreateJobForDevicesResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
     {
         "NodeName": str,
@@ -1034,55 +1111,51 @@
 
 class CreateNodeFromTemplateJobRequestRequestTypeDef(
     _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
     _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
 ):
     pass
 
-DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "DescribeNodeFromTemplateJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsTypeDef],
-        "LastUpdatedTime": datetime,
-        "NodeDescription": str,
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "Status": NodeFromTemplateJobStatusType,
-        "StatusMessage": str,
-        "TemplateParameters": Dict[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "Arn": str,
         "PackageId": str,
         "StorageLocation": StorageLocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePackageResponseTypeDef = TypedDict(
     "DescribePackageResponseTypeDef",
     {
         "Arn": str,
         "CreatedTime": datetime,
         "PackageId": str,
         "PackageName": str,
         "ReadAccessPrincipalArns": List[str],
         "StorageLocation": StorageLocationTypeDef,
         "Tags": Dict[str, str],
         "WriteAccessPrincipalArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeApplicationInstanceDetailsResponseTypeDef = TypedDict(
+    "DescribeApplicationInstanceDetailsResponseTypeDef",
+    {
+        "ApplicationInstanceId": str,
+        "ApplicationInstanceIdToReplace": str,
+        "CreatedTime": datetime,
+        "DefaultRuntimeContextDevice": str,
+        "Description": str,
+        "ManifestOverridesPayload": ManifestOverridesPayloadOutputTypeDef,
+        "ManifestPayload": ManifestPayloadOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "Brand": DeviceBrandType,
@@ -1098,31 +1171,69 @@
         "ProvisioningStatus": DeviceStatusType,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
     },
     total=False,
 )
 
+DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "DescribeNodeFromTemplateJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "LastUpdatedTime": datetime,
+        "NodeDescription": str,
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "Status": NodeFromTemplateJobStatusType,
+        "StatusMessage": str,
+        "TemplateParameters": Dict[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeviceJobConfigTypeDef = TypedDict(
     "DeviceJobConfigTypeDef",
     {
         "OTAJobConfig": OTAJobConfigTypeDef,
     },
     total=False,
 )
 
 ListDevicesJobsResponseTypeDef = TypedDict(
     "ListDevicesJobsResponseTypeDef",
     {
         "DeviceJobs": List[DeviceJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredEthernetPayloadOutputTypeDef = TypedDict(
+    "_RequiredEthernetPayloadOutputTypeDef",
+    {
+        "ConnectionType": ConnectionTypeType,
+    },
+)
+_OptionalEthernetPayloadOutputTypeDef = TypedDict(
+    "_OptionalEthernetPayloadOutputTypeDef",
+    {
+        "StaticIpConnectionInfo": StaticIpConnectionInfoOutputTypeDef,
+    },
+    total=False,
+)
+
+class EthernetPayloadOutputTypeDef(
+    _RequiredEthernetPayloadOutputTypeDef, _OptionalEthernetPayloadOutputTypeDef
+):
+    pass
+
 _RequiredEthernetPayloadTypeDef = TypedDict(
     "_RequiredEthernetPayloadTypeDef",
     {
         "ConnectionType": ConnectionTypeType,
     },
 )
 _OptionalEthernetPayloadTypeDef = TypedDict(
@@ -1137,60 +1248,60 @@
     pass
 
 ListApplicationInstanceDependenciesResponseTypeDef = TypedDict(
     "ListApplicationInstanceDependenciesResponseTypeDef",
     {
         "NextToken": str,
         "PackageObjects": List[PackageObjectTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationInstanceNodeInstancesResponseTypeDef = TypedDict(
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     {
         "NextToken": str,
         "NodeInstances": List[NodeInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNodeFromTemplateJobsResponseTypeDef = TypedDict(
     "ListNodeFromTemplateJobsResponseTypeDef",
     {
         "NextToken": str,
         "NodeFromTemplateJobs": List[NodeFromTemplateJobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
         "NextToken": str,
         "Nodes": List[NodeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackageImportJobsResponseTypeDef = TypedDict(
     "ListPackageImportJobsResponseTypeDef",
     {
         "NextToken": str,
         "PackageImportJobs": List[PackageImportJobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesResponseTypeDef = TypedDict(
     "ListPackagesResponseTypeDef",
     {
         "NextToken": str,
         "Packages": List[PackageListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkStatusTypeDef = TypedDict(
     "NetworkStatusTypeDef",
     {
         "Ethernet0Status": EthernetStatusTypeDef,
@@ -1223,44 +1334,59 @@
         "OutputS3Location": OutPutS3LocationTypeDef,
         "PackageId": str,
         "PackageVersion": str,
         "PatchVersion": str,
     },
 )
 
+PackageImportJobOutputConfigOutputTypeDef = TypedDict(
+    "PackageImportJobOutputConfigOutputTypeDef",
+    {
+        "PackageVersionOutputConfig": PackageVersionOutputConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 PackageImportJobOutputConfigTypeDef = TypedDict(
     "PackageImportJobOutputConfigTypeDef",
     {
         "PackageVersionOutputConfig": PackageVersionOutputConfigTypeDef,
     },
     total=False,
 )
 
+PackageVersionInputConfigOutputTypeDef = TypedDict(
+    "PackageVersionInputConfigOutputTypeDef",
+    {
+        "S3Location": S3LocationOutputTypeDef,
+    },
+)
+
 PackageVersionInputConfigTypeDef = TypedDict(
     "PackageVersionInputConfigTypeDef",
     {
         "S3Location": S3LocationTypeDef,
     },
 )
 
 ListApplicationInstancesResponseTypeDef = TypedDict(
     "ListApplicationInstancesResponseTypeDef",
     {
         "ApplicationInstances": List[ApplicationInstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateJobForDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobForDevicesRequestRequestTypeDef",
     {
         "DeviceIds": Sequence[str],
@@ -1277,14 +1403,24 @@
 
 class CreateJobForDevicesRequestRequestTypeDef(
     _RequiredCreateJobForDevicesRequestRequestTypeDef,
     _OptionalCreateJobForDevicesRequestRequestTypeDef,
 ):
     pass
 
+NetworkPayloadOutputTypeDef = TypedDict(
+    "NetworkPayloadOutputTypeDef",
+    {
+        "Ethernet0": EthernetPayloadOutputTypeDef,
+        "Ethernet1": EthernetPayloadOutputTypeDef,
+        "Ntp": NtpPayloadOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkPayloadTypeDef = TypedDict(
     "NetworkPayloadTypeDef",
     {
         "Ethernet0": EthernetPayloadTypeDef,
         "Ethernet1": EthernetPayloadTypeDef,
         "Ntp": NtpPayloadTypeDef,
     },
@@ -1304,18 +1440,26 @@
         "NodeInterface": NodeInterfaceTypeDef,
         "OwnerAccount": str,
         "PackageArn": str,
         "PackageId": str,
         "PackageName": str,
         "PackageVersion": str,
         "PatchVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PackageImportJobInputConfigOutputTypeDef = TypedDict(
+    "PackageImportJobInputConfigOutputTypeDef",
+    {
+        "PackageVersionInputConfig": PackageVersionInputConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 PackageImportJobInputConfigTypeDef = TypedDict(
     "PackageImportJobInputConfigTypeDef",
     {
         "PackageVersionInputConfig": PackageVersionInputConfigTypeDef,
     },
     total=False,
 )
@@ -1334,20 +1478,20 @@
         "DeviceConnectionStatus": DeviceConnectionStatusType,
         "DeviceId": str,
         "LatestAlternateSoftware": str,
         "LatestDeviceJob": LatestDeviceJobTypeDef,
         "LatestSoftware": str,
         "LeaseExpirationTime": datetime,
         "Name": str,
-        "NetworkingConfiguration": NetworkPayloadTypeDef,
+        "NetworkingConfiguration": NetworkPayloadOutputTypeDef,
         "ProvisioningStatus": DeviceStatusType,
         "SerialNumber": str,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredProvisionDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionDeviceRequestRequestTypeDef",
     {
         "Name": str,
@@ -1364,14 +1508,32 @@
 )
 
 class ProvisionDeviceRequestRequestTypeDef(
     _RequiredProvisionDeviceRequestRequestTypeDef, _OptionalProvisionDeviceRequestRequestTypeDef
 ):
     pass
 
+DescribePackageImportJobResponseTypeDef = TypedDict(
+    "DescribePackageImportJobResponseTypeDef",
+    {
+        "ClientToken": str,
+        "CreatedTime": datetime,
+        "InputConfig": PackageImportJobInputConfigOutputTypeDef,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "JobType": PackageImportJobTypeType,
+        "LastUpdatedTime": datetime,
+        "Output": PackageImportJobOutputTypeDef,
+        "OutputConfig": PackageImportJobOutputConfigOutputTypeDef,
+        "Status": PackageImportJobStatusType,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageImportJobRequestRequestTypeDef",
     {
         "ClientToken": str,
         "InputConfig": PackageImportJobInputConfigTypeDef,
         "JobType": PackageImportJobTypeType,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
@@ -1386,25 +1548,7 @@
 )
 
 class CreatePackageImportJobRequestRequestTypeDef(
     _RequiredCreatePackageImportJobRequestRequestTypeDef,
     _OptionalCreatePackageImportJobRequestRequestTypeDef,
 ):
     pass
-
-DescribePackageImportJobResponseTypeDef = TypedDict(
-    "DescribePackageImportJobResponseTypeDef",
-    {
-        "ClientToken": str,
-        "CreatedTime": datetime,
-        "InputConfig": PackageImportJobInputConfigTypeDef,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsTypeDef],
-        "JobType": PackageImportJobTypeType,
-        "LastUpdatedTime": datetime,
-        "Output": PackageImportJobOutputTypeDef,
-        "OutputConfig": PackageImportJobOutputConfigTypeDef,
-        "Status": PackageImportJobStatusType,
-        "StatusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `mypy-boto3-panorama-1.28.0/mypy_boto3_panorama.egg-info/PKG-INFO` & `mypy-boto3-panorama-1.28.12/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-panorama
-Version: 1.28.0
-Summary: Type annotations for boto3.Panorama 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 panorama type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-panorama"></a>
 
 # mypy-boto3-panorama
 
 [![PyPI - mypy-boto3-panorama](https://img.shields.io/pypi/v/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-panorama.svg?color=blue)](https://pypi.org/project/mypy-boto3-panorama)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-panorama?color=blue)](https://pypistats.org/packages/mypy-boto3-panorama)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-panorama)](https://pepy.tech/project/mypy-boto3-panorama)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Panorama 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
+[boto3.Panorama 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama)
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
 [mypy-boto3-panorama docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_panorama/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,39 +292,38 @@
 
 ```python
 from mypy_boto3_panorama.type_defs import (
     AlternateSoftwareMetadataTypeDef,
     ReportedRuntimeContextStateTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    CreateApplicationInstanceResponseTypeDef,
+    ResponseMetadataTypeDef,
     JobTypeDef,
     JobResourceTagsTypeDef,
-    CreateNodeFromTemplateJobResponseTypeDef,
-    CreatePackageImportJobResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
     StorageLocationTypeDef,
     DeleteDeviceRequestRequestTypeDef,
-    DeleteDeviceResponseTypeDef,
     DeletePackageRequestRequestTypeDef,
     DeregisterPackageVersionRequestRequestTypeDef,
     DescribeApplicationInstanceDetailsRequestRequestTypeDef,
+    ManifestOverridesPayloadOutputTypeDef,
+    ManifestPayloadOutputTypeDef,
     DescribeApplicationInstanceRequestRequestTypeDef,
     DescribeDeviceJobRequestRequestTypeDef,
-    DescribeDeviceJobResponseTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     LatestDeviceJobTypeDef,
     DescribeNodeFromTemplateJobRequestRequestTypeDef,
+    JobResourceTagsOutputTypeDef,
     DescribeNodeRequestRequestTypeDef,
     DescribePackageImportJobRequestRequestTypeDef,
     DescribePackageRequestRequestTypeDef,
     DescribePackageVersionRequestRequestTypeDef,
-    DescribePackageVersionResponseTypeDef,
     OTAJobConfigTypeDef,
     DeviceJobTypeDef,
+    StaticIpConnectionInfoOutputTypeDef,
     StaticIpConnectionInfoTypeDef,
     EthernetStatusTypeDef,
     ListApplicationInstanceDependenciesRequestRequestTypeDef,
     PackageObjectTypeDef,
     ListApplicationInstanceNodeInstancesRequestRequestTypeDef,
     NodeInstanceTypeDef,
     ListApplicationInstancesRequestRequestTypeDef,
@@ -367,67 +334,80 @@
     ListNodesRequestRequestTypeDef,
     NodeTypeDef,
     ListPackageImportJobsRequestRequestTypeDef,
     PackageImportJobTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageListItemTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    NtpPayloadOutputTypeDef,
     NtpPayloadTypeDef,
     NtpStatusTypeDef,
     NodeInputPortTypeDef,
     NodeOutputPortTypeDef,
     NodeSignalTypeDef,
     OutPutS3LocationTypeDef,
+    PackageVersionOutputConfigOutputTypeDef,
     PackageVersionOutputConfigTypeDef,
+    S3LocationOutputTypeDef,
     S3LocationTypeDef,
-    ProvisionDeviceResponseTypeDef,
     RegisterPackageVersionRequestRequestTypeDef,
     RemoveApplicationInstanceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SignalApplicationInstanceNodeInstancesResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceMetadataRequestRequestTypeDef,
-    UpdateDeviceMetadataResponseTypeDef,
     ApplicationInstanceTypeDef,
-    DescribeApplicationInstanceResponseTypeDef,
     CreateApplicationInstanceRequestRequestTypeDef,
-    DescribeApplicationInstanceDetailsResponseTypeDef,
+    CreateApplicationInstanceResponseTypeDef,
+    CreateNodeFromTemplateJobResponseTypeDef,
+    CreatePackageImportJobResponseTypeDef,
+    DeleteDeviceResponseTypeDef,
+    DescribeApplicationInstanceResponseTypeDef,
+    DescribeDeviceJobResponseTypeDef,
+    DescribePackageVersionResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ProvisionDeviceResponseTypeDef,
+    SignalApplicationInstanceNodeInstancesResponseTypeDef,
+    UpdateDeviceMetadataResponseTypeDef,
     CreateJobForDevicesResponseTypeDef,
     CreateNodeFromTemplateJobRequestRequestTypeDef,
-    DescribeNodeFromTemplateJobResponseTypeDef,
     CreatePackageResponseTypeDef,
     DescribePackageResponseTypeDef,
+    DescribeApplicationInstanceDetailsResponseTypeDef,
     DeviceTypeDef,
+    DescribeNodeFromTemplateJobResponseTypeDef,
     DeviceJobConfigTypeDef,
     ListDevicesJobsResponseTypeDef,
+    EthernetPayloadOutputTypeDef,
     EthernetPayloadTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     NetworkStatusTypeDef,
     NodeInterfaceTypeDef,
     SignalApplicationInstanceNodeInstancesRequestRequestTypeDef,
     PackageImportJobOutputTypeDef,
+    PackageImportJobOutputConfigOutputTypeDef,
     PackageImportJobOutputConfigTypeDef,
+    PackageVersionInputConfigOutputTypeDef,
     PackageVersionInputConfigTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesResponseTypeDef,
     CreateJobForDevicesRequestRequestTypeDef,
+    NetworkPayloadOutputTypeDef,
     NetworkPayloadTypeDef,
     DescribeNodeResponseTypeDef,
+    PackageImportJobInputConfigOutputTypeDef,
     PackageImportJobInputConfigTypeDef,
     DescribeDeviceResponseTypeDef,
     ProvisionDeviceRequestRequestTypeDef,
-    CreatePackageImportJobRequestRequestTypeDef,
     DescribePackageImportJobResponseTypeDef,
+    CreatePackageImportJobRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AlternateSoftwareMetadataTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-panorama-1.28.0/mypy_boto3_panorama.egg-info/SOURCES.txt` & `mypy-boto3-panorama-1.28.12/mypy_boto3_panorama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-panorama-1.28.0/setup.py` & `mypy-boto3-panorama-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-panorama",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_panorama"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Panorama 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Panorama 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

