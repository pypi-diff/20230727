# Comparing `tmp/mypy-boto3-devicefarm-1.28.0.tar.gz` & `tmp/mypy-boto3-devicefarm-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-devicefarm-1.28.0.tar", last modified: Thu Jul  6 20:59:23 2023, max compression
+gzip compressed data, was "mypy-boto3-devicefarm-1.28.12.tar", last modified: Thu Jul 27 05:34:33 2023, max compression
```

## Comparing `mypy-boto3-devicefarm-1.28.0.tar` & `mypy-boto3-devicefarm-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:23.370276 mypy-boto3-devicefarm-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:40.000000 mypy-boto3-devicefarm-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24704 2023-07-06 20:59:23.370276 mypy-boto3-devicefarm-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-07-06 20:37:40.000000 mypy-boto3-devicefarm-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:23.358276 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-06 20:37:40.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-06 20:37:40.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:37:40.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57697 2023-07-06 20:37:40.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57593 2023-07-06 20:37:40.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-07-06 20:37:42.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15714 2023-07-06 20:37:42.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-07-06 20:37:40.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-07-06 20:37:40.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:40.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    73250 2023-07-06 20:37:44.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    73159 2023-07-06 20:37:43.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:40.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:23.370276 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24704 2023-07-06 20:59:23.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 20:59:23.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:23.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:23.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:23.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:23.000000 mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:23.370276 mypy-boto3-devicefarm-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:37:39.000000 mypy-boto3-devicefarm-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.944535 mypy-boto3-devicefarm-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-07-27 05:34:33.944535 mypy-boto3-devicefarm-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.940535 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57697 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57593 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-27 05:20:08.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-27 05:20:08.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-07-27 05:20:08.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    74980 2023-07-27 05:20:10.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74889 2023-07-27 05:20:09.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.944535 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-07-27 05:34:33.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:33.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:33.000000 mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:33.944535 mypy-boto3-devicefarm-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:20:07.000000 mypy-boto3-devicefarm-1.28.12/setup.py
```

### Comparing `mypy-boto3-devicefarm-1.28.0/LICENSE` & `mypy-boto3-devicefarm-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.0/PKG-INFO` & `mypy-boto3-devicefarm-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devicefarm
-Version: 1.28.0
-Summary: Type annotations for boto3.DeviceFarm 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DeviceFarm 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-devicefarm"></a>
 
 # mypy-boto3-devicefarm
 
 [![PyPI - mypy-boto3-devicefarm](https://img.shields.io/pypi/v/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devicefarm?color=blue)](https://pypistats.org/packages/mypy-boto3-devicefarm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devicefarm)](https://pepy.tech/project/mypy-boto3-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DeviceFarm 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[boto3.DeviceFarm 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -441,27 +441,30 @@
     TestGridVpcConfigTypeDef,
     CreateTestGridUrlRequestRequestTypeDef,
     CreateTestGridUrlResultTypeDef,
     CreateUploadRequestRequestTypeDef,
     UploadTypeDef,
     CreateVPCEConfigurationRequestRequestTypeDef,
     VPCEConfigurationTypeDef,
+    CustomerArtifactPathsOutputTypeDef,
     CustomerArtifactPathsTypeDef,
     DeleteDevicePoolRequestRequestTypeDef,
     DeleteInstanceProfileRequestRequestTypeDef,
     DeleteNetworkProfileRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteRemoteAccessSessionRequestRequestTypeDef,
     DeleteRunRequestRequestTypeDef,
     DeleteTestGridProjectRequestRequestTypeDef,
     DeleteUploadRequestRequestTypeDef,
     DeleteVPCEConfigurationRequestRequestTypeDef,
+    DeviceFilterOutputTypeDef,
     DeviceFilterTypeDef,
     DeviceMinutesTypeDef,
     IncompatibilityMessageTypeDef,
+    RuleOutputTypeDef,
     ResolutionTypeDef,
     ExecutionConfigurationTypeDef,
     GetDeviceInstanceRequestRequestTypeDef,
     ScheduleRunTestTypeDef,
     GetDevicePoolRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
@@ -507,117 +510,122 @@
     ListRunsRequestRequestTypeDef,
     ListSamplesRequestListSamplesPaginateTypeDef,
     ListSamplesRequestRequestTypeDef,
     SampleTypeDef,
     ListSuitesRequestListSuitesPaginateTypeDef,
     ListSuitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ListTestGridProjectsRequestRequestTypeDef,
     ListTestGridSessionActionsRequestRequestTypeDef,
     TestGridSessionActionTypeDef,
     ListTestGridSessionArtifactsRequestRequestTypeDef,
     TestGridSessionArtifactTypeDef,
     ListTestGridSessionsRequestRequestTypeDef,
     ListTestsRequestListTestsPaginateTypeDef,
     ListTestsRequestRequestTypeDef,
     ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
     ListUniqueProblemsRequestRequestTypeDef,
     ListUploadsRequestListUploadsPaginateTypeDef,
     ListUploadsRequestRequestTypeDef,
     ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     ListVPCEConfigurationsRequestRequestTypeDef,
+    LocationOutputTypeDef,
     LocationTypeDef,
     MonetaryAmountTypeDef,
     PaginatorConfigTypeDef,
     ProblemDetailTypeDef,
+    VpcConfigOutputTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
+    RadiosOutputTypeDef,
     RadiosTypeDef,
     RenewOfferingRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     StopJobRequestRequestTypeDef,
     StopRemoteAccessSessionRequestRequestTypeDef,
     StopRunRequestRequestTypeDef,
+    TagTypeDef,
+    TestGridVpcConfigOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceInstanceRequestRequestTypeDef,
     UpdateInstanceProfileRequestRequestTypeDef,
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateUploadRequestRequestTypeDef,
     UpdateVPCEConfigurationRequestRequestTypeDef,
     AccountSettingsTypeDef,
     ListArtifactsResultTypeDef,
     CreateDevicePoolRequestRequestTypeDef,
-    DevicePoolTypeDef,
     UpdateDevicePoolRequestRequestTypeDef,
     CreateInstanceProfileResultTypeDef,
     DeviceInstanceTypeDef,
     GetInstanceProfileResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     CreateNetworkProfileResultTypeDef,
     GetNetworkProfileResultTypeDef,
     ListNetworkProfilesResultTypeDef,
     UpdateNetworkProfileResultTypeDef,
     CreateProjectRequestRequestTypeDef,
-    ProjectTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateRemoteAccessSessionRequestRequestTypeDef,
     CreateTestGridProjectRequestRequestTypeDef,
-    TestGridProjectTypeDef,
     UpdateTestGridProjectRequestRequestTypeDef,
     CreateUploadResultTypeDef,
     GetUploadResultTypeDef,
     InstallToRemoteAccessSessionResultTypeDef,
     ListUploadsResultTypeDef,
     UpdateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
     GetVPCEConfigurationResultTypeDef,
     ListVPCEConfigurationsResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
-    DeviceSelectionConfigurationTypeDef,
     DeviceSelectionResultTypeDef,
+    DeviceSelectionConfigurationTypeDef,
     ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     SuiteTypeDef,
     TestTypeDef,
+    DevicePoolTypeDef,
     GetTestGridSessionResultTypeDef,
     ListTestGridSessionsResultTypeDef,
     ListOfferingPromotionsResultTypeDef,
     ListSamplesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ListTestGridSessionActionsResultTypeDef,
     ListTestGridSessionArtifactsResultTypeDef,
     RecurringChargeTypeDef,
+    ProjectTypeDef,
     ScheduleRunConfigurationTypeDef,
+    TagResourceRequestRequestTypeDef,
+    TestGridProjectTypeDef,
     GetAccountSettingsResultTypeDef,
-    CreateDevicePoolResultTypeDef,
-    GetDevicePoolResultTypeDef,
-    ListDevicePoolsResultTypeDef,
-    UpdateDevicePoolResultTypeDef,
     DeviceTypeDef,
     GetDeviceInstanceResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     UpdateDeviceInstanceResultTypeDef,
-    CreateProjectResultTypeDef,
-    GetProjectResultTypeDef,
-    ListProjectsResultTypeDef,
-    UpdateProjectResultTypeDef,
-    CreateTestGridProjectResultTypeDef,
-    GetTestGridProjectResultTypeDef,
-    ListTestGridProjectsResultTypeDef,
-    UpdateTestGridProjectResultTypeDef,
     RunTypeDef,
     GetSuiteResultTypeDef,
     ListSuitesResultTypeDef,
     GetTestResultTypeDef,
     ListTestsResultTypeDef,
+    CreateDevicePoolResultTypeDef,
+    GetDevicePoolResultTypeDef,
+    ListDevicePoolsResultTypeDef,
+    UpdateDevicePoolResultTypeDef,
     OfferingTypeDef,
+    CreateProjectResultTypeDef,
+    GetProjectResultTypeDef,
+    ListProjectsResultTypeDef,
+    UpdateProjectResultTypeDef,
     GetDevicePoolCompatibilityRequestRequestTypeDef,
     ScheduleRunRequestRequestTypeDef,
+    CreateTestGridProjectResultTypeDef,
+    GetTestGridProjectResultTypeDef,
+    ListTestGridProjectsResultTypeDef,
+    UpdateTestGridProjectResultTypeDef,
     DevicePoolCompatibilityResultTypeDef,
     GetDeviceResultTypeDef,
     JobTypeDef,
     ListDevicesResultTypeDef,
     ProblemTypeDef,
     RemoteAccessSessionTypeDef,
     GetRunResultTypeDef,
```

### Comparing `mypy-boto3-devicefarm-1.28.0/README.md` & `mypy-boto3-devicefarm-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-devicefarm"></a>
 
 # mypy-boto3-devicefarm
 
 [![PyPI - mypy-boto3-devicefarm](https://img.shields.io/pypi/v/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devicefarm?color=blue)](https://pypistats.org/packages/mypy-boto3-devicefarm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devicefarm)](https://pepy.tech/project/mypy-boto3-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DeviceFarm 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[boto3.DeviceFarm 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -409,27 +409,30 @@
     TestGridVpcConfigTypeDef,
     CreateTestGridUrlRequestRequestTypeDef,
     CreateTestGridUrlResultTypeDef,
     CreateUploadRequestRequestTypeDef,
     UploadTypeDef,
     CreateVPCEConfigurationRequestRequestTypeDef,
     VPCEConfigurationTypeDef,
+    CustomerArtifactPathsOutputTypeDef,
     CustomerArtifactPathsTypeDef,
     DeleteDevicePoolRequestRequestTypeDef,
     DeleteInstanceProfileRequestRequestTypeDef,
     DeleteNetworkProfileRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteRemoteAccessSessionRequestRequestTypeDef,
     DeleteRunRequestRequestTypeDef,
     DeleteTestGridProjectRequestRequestTypeDef,
     DeleteUploadRequestRequestTypeDef,
     DeleteVPCEConfigurationRequestRequestTypeDef,
+    DeviceFilterOutputTypeDef,
     DeviceFilterTypeDef,
     DeviceMinutesTypeDef,
     IncompatibilityMessageTypeDef,
+    RuleOutputTypeDef,
     ResolutionTypeDef,
     ExecutionConfigurationTypeDef,
     GetDeviceInstanceRequestRequestTypeDef,
     ScheduleRunTestTypeDef,
     GetDevicePoolRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
@@ -475,117 +478,122 @@
     ListRunsRequestRequestTypeDef,
     ListSamplesRequestListSamplesPaginateTypeDef,
     ListSamplesRequestRequestTypeDef,
     SampleTypeDef,
     ListSuitesRequestListSuitesPaginateTypeDef,
     ListSuitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ListTestGridProjectsRequestRequestTypeDef,
     ListTestGridSessionActionsRequestRequestTypeDef,
     TestGridSessionActionTypeDef,
     ListTestGridSessionArtifactsRequestRequestTypeDef,
     TestGridSessionArtifactTypeDef,
     ListTestGridSessionsRequestRequestTypeDef,
     ListTestsRequestListTestsPaginateTypeDef,
     ListTestsRequestRequestTypeDef,
     ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
     ListUniqueProblemsRequestRequestTypeDef,
     ListUploadsRequestListUploadsPaginateTypeDef,
     ListUploadsRequestRequestTypeDef,
     ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     ListVPCEConfigurationsRequestRequestTypeDef,
+    LocationOutputTypeDef,
     LocationTypeDef,
     MonetaryAmountTypeDef,
     PaginatorConfigTypeDef,
     ProblemDetailTypeDef,
+    VpcConfigOutputTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
+    RadiosOutputTypeDef,
     RadiosTypeDef,
     RenewOfferingRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     StopJobRequestRequestTypeDef,
     StopRemoteAccessSessionRequestRequestTypeDef,
     StopRunRequestRequestTypeDef,
+    TagTypeDef,
+    TestGridVpcConfigOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceInstanceRequestRequestTypeDef,
     UpdateInstanceProfileRequestRequestTypeDef,
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateUploadRequestRequestTypeDef,
     UpdateVPCEConfigurationRequestRequestTypeDef,
     AccountSettingsTypeDef,
     ListArtifactsResultTypeDef,
     CreateDevicePoolRequestRequestTypeDef,
-    DevicePoolTypeDef,
     UpdateDevicePoolRequestRequestTypeDef,
     CreateInstanceProfileResultTypeDef,
     DeviceInstanceTypeDef,
     GetInstanceProfileResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     CreateNetworkProfileResultTypeDef,
     GetNetworkProfileResultTypeDef,
     ListNetworkProfilesResultTypeDef,
     UpdateNetworkProfileResultTypeDef,
     CreateProjectRequestRequestTypeDef,
-    ProjectTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateRemoteAccessSessionRequestRequestTypeDef,
     CreateTestGridProjectRequestRequestTypeDef,
-    TestGridProjectTypeDef,
     UpdateTestGridProjectRequestRequestTypeDef,
     CreateUploadResultTypeDef,
     GetUploadResultTypeDef,
     InstallToRemoteAccessSessionResultTypeDef,
     ListUploadsResultTypeDef,
     UpdateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
     GetVPCEConfigurationResultTypeDef,
     ListVPCEConfigurationsResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
-    DeviceSelectionConfigurationTypeDef,
     DeviceSelectionResultTypeDef,
+    DeviceSelectionConfigurationTypeDef,
     ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     SuiteTypeDef,
     TestTypeDef,
+    DevicePoolTypeDef,
     GetTestGridSessionResultTypeDef,
     ListTestGridSessionsResultTypeDef,
     ListOfferingPromotionsResultTypeDef,
     ListSamplesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ListTestGridSessionActionsResultTypeDef,
     ListTestGridSessionArtifactsResultTypeDef,
     RecurringChargeTypeDef,
+    ProjectTypeDef,
     ScheduleRunConfigurationTypeDef,
+    TagResourceRequestRequestTypeDef,
+    TestGridProjectTypeDef,
     GetAccountSettingsResultTypeDef,
-    CreateDevicePoolResultTypeDef,
-    GetDevicePoolResultTypeDef,
-    ListDevicePoolsResultTypeDef,
-    UpdateDevicePoolResultTypeDef,
     DeviceTypeDef,
     GetDeviceInstanceResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     UpdateDeviceInstanceResultTypeDef,
-    CreateProjectResultTypeDef,
-    GetProjectResultTypeDef,
-    ListProjectsResultTypeDef,
-    UpdateProjectResultTypeDef,
-    CreateTestGridProjectResultTypeDef,
-    GetTestGridProjectResultTypeDef,
-    ListTestGridProjectsResultTypeDef,
-    UpdateTestGridProjectResultTypeDef,
     RunTypeDef,
     GetSuiteResultTypeDef,
     ListSuitesResultTypeDef,
     GetTestResultTypeDef,
     ListTestsResultTypeDef,
+    CreateDevicePoolResultTypeDef,
+    GetDevicePoolResultTypeDef,
+    ListDevicePoolsResultTypeDef,
+    UpdateDevicePoolResultTypeDef,
     OfferingTypeDef,
+    CreateProjectResultTypeDef,
+    GetProjectResultTypeDef,
+    ListProjectsResultTypeDef,
+    UpdateProjectResultTypeDef,
     GetDevicePoolCompatibilityRequestRequestTypeDef,
     ScheduleRunRequestRequestTypeDef,
+    CreateTestGridProjectResultTypeDef,
+    GetTestGridProjectResultTypeDef,
+    ListTestGridProjectsResultTypeDef,
+    UpdateTestGridProjectResultTypeDef,
     DevicePoolCompatibilityResultTypeDef,
     GetDeviceResultTypeDef,
     JobTypeDef,
     ListDevicesResultTypeDef,
     ProblemTypeDef,
     RemoteAccessSessionTypeDef,
     GetRunResultTypeDef,
```

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/__init__.py` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/__init__.pyi` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/__main__.py` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DeviceFarm 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.DeviceFarm 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm\nOther"
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

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/client.py` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/client.pyi` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/literals.py` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,14 +390,15 @@
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
@@ -476,26 +477,28 @@
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

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/literals.pyi` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -388,14 +388,15 @@
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
@@ -474,26 +475,28 @@
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

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/paginator.py` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/paginator.pyi` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/type_defs.py` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,27 +68,30 @@
     "TestGridVpcConfigTypeDef",
     "CreateTestGridUrlRequestRequestTypeDef",
     "CreateTestGridUrlResultTypeDef",
     "CreateUploadRequestRequestTypeDef",
     "UploadTypeDef",
     "CreateVPCEConfigurationRequestRequestTypeDef",
     "VPCEConfigurationTypeDef",
+    "CustomerArtifactPathsOutputTypeDef",
     "CustomerArtifactPathsTypeDef",
     "DeleteDevicePoolRequestRequestTypeDef",
     "DeleteInstanceProfileRequestRequestTypeDef",
     "DeleteNetworkProfileRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteRemoteAccessSessionRequestRequestTypeDef",
     "DeleteRunRequestRequestTypeDef",
     "DeleteTestGridProjectRequestRequestTypeDef",
     "DeleteUploadRequestRequestTypeDef",
     "DeleteVPCEConfigurationRequestRequestTypeDef",
+    "DeviceFilterOutputTypeDef",
     "DeviceFilterTypeDef",
     "DeviceMinutesTypeDef",
     "IncompatibilityMessageTypeDef",
+    "RuleOutputTypeDef",
     "ResolutionTypeDef",
     "ExecutionConfigurationTypeDef",
     "GetDeviceInstanceRequestRequestTypeDef",
     "ScheduleRunTestTypeDef",
     "GetDevicePoolRequestRequestTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetInstanceProfileRequestRequestTypeDef",
@@ -134,117 +137,122 @@
     "ListRunsRequestRequestTypeDef",
     "ListSamplesRequestListSamplesPaginateTypeDef",
     "ListSamplesRequestRequestTypeDef",
     "SampleTypeDef",
     "ListSuitesRequestListSuitesPaginateTypeDef",
     "ListSuitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ListTestGridProjectsRequestRequestTypeDef",
     "ListTestGridSessionActionsRequestRequestTypeDef",
     "TestGridSessionActionTypeDef",
     "ListTestGridSessionArtifactsRequestRequestTypeDef",
     "TestGridSessionArtifactTypeDef",
     "ListTestGridSessionsRequestRequestTypeDef",
     "ListTestsRequestListTestsPaginateTypeDef",
     "ListTestsRequestRequestTypeDef",
     "ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
     "ListUniqueProblemsRequestRequestTypeDef",
     "ListUploadsRequestListUploadsPaginateTypeDef",
     "ListUploadsRequestRequestTypeDef",
     "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
     "ListVPCEConfigurationsRequestRequestTypeDef",
+    "LocationOutputTypeDef",
     "LocationTypeDef",
     "MonetaryAmountTypeDef",
     "PaginatorConfigTypeDef",
     "ProblemDetailTypeDef",
+    "VpcConfigOutputTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
+    "RadiosOutputTypeDef",
     "RadiosTypeDef",
     "RenewOfferingRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "StopJobRequestRequestTypeDef",
     "StopRemoteAccessSessionRequestRequestTypeDef",
     "StopRunRequestRequestTypeDef",
+    "TagTypeDef",
+    "TestGridVpcConfigOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceInstanceRequestRequestTypeDef",
     "UpdateInstanceProfileRequestRequestTypeDef",
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateUploadRequestRequestTypeDef",
     "UpdateVPCEConfigurationRequestRequestTypeDef",
     "AccountSettingsTypeDef",
     "ListArtifactsResultTypeDef",
     "CreateDevicePoolRequestRequestTypeDef",
-    "DevicePoolTypeDef",
     "UpdateDevicePoolRequestRequestTypeDef",
     "CreateInstanceProfileResultTypeDef",
     "DeviceInstanceTypeDef",
     "GetInstanceProfileResultTypeDef",
     "ListInstanceProfilesResultTypeDef",
     "UpdateInstanceProfileResultTypeDef",
     "CreateNetworkProfileResultTypeDef",
     "GetNetworkProfileResultTypeDef",
     "ListNetworkProfilesResultTypeDef",
     "UpdateNetworkProfileResultTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "ProjectTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "CreateRemoteAccessSessionRequestRequestTypeDef",
     "CreateTestGridProjectRequestRequestTypeDef",
-    "TestGridProjectTypeDef",
     "UpdateTestGridProjectRequestRequestTypeDef",
     "CreateUploadResultTypeDef",
     "GetUploadResultTypeDef",
     "InstallToRemoteAccessSessionResultTypeDef",
     "ListUploadsResultTypeDef",
     "UpdateUploadResultTypeDef",
     "CreateVPCEConfigurationResultTypeDef",
     "GetVPCEConfigurationResultTypeDef",
     "ListVPCEConfigurationsResultTypeDef",
     "UpdateVPCEConfigurationResultTypeDef",
-    "DeviceSelectionConfigurationTypeDef",
     "DeviceSelectionResultTypeDef",
+    "DeviceSelectionConfigurationTypeDef",
     "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "SuiteTypeDef",
     "TestTypeDef",
+    "DevicePoolTypeDef",
     "GetTestGridSessionResultTypeDef",
     "ListTestGridSessionsResultTypeDef",
     "ListOfferingPromotionsResultTypeDef",
     "ListSamplesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "ListTestGridSessionActionsResultTypeDef",
     "ListTestGridSessionArtifactsResultTypeDef",
     "RecurringChargeTypeDef",
+    "ProjectTypeDef",
     "ScheduleRunConfigurationTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "TestGridProjectTypeDef",
     "GetAccountSettingsResultTypeDef",
-    "CreateDevicePoolResultTypeDef",
-    "GetDevicePoolResultTypeDef",
-    "ListDevicePoolsResultTypeDef",
-    "UpdateDevicePoolResultTypeDef",
     "DeviceTypeDef",
     "GetDeviceInstanceResultTypeDef",
     "ListDeviceInstancesResultTypeDef",
     "UpdateDeviceInstanceResultTypeDef",
-    "CreateProjectResultTypeDef",
-    "GetProjectResultTypeDef",
-    "ListProjectsResultTypeDef",
-    "UpdateProjectResultTypeDef",
-    "CreateTestGridProjectResultTypeDef",
-    "GetTestGridProjectResultTypeDef",
-    "ListTestGridProjectsResultTypeDef",
-    "UpdateTestGridProjectResultTypeDef",
     "RunTypeDef",
     "GetSuiteResultTypeDef",
     "ListSuitesResultTypeDef",
     "GetTestResultTypeDef",
     "ListTestsResultTypeDef",
+    "CreateDevicePoolResultTypeDef",
+    "GetDevicePoolResultTypeDef",
+    "ListDevicePoolsResultTypeDef",
+    "UpdateDevicePoolResultTypeDef",
     "OfferingTypeDef",
+    "CreateProjectResultTypeDef",
+    "GetProjectResultTypeDef",
+    "ListProjectsResultTypeDef",
+    "UpdateProjectResultTypeDef",
     "GetDevicePoolCompatibilityRequestRequestTypeDef",
     "ScheduleRunRequestRequestTypeDef",
+    "CreateTestGridProjectResultTypeDef",
+    "GetTestGridProjectResultTypeDef",
+    "ListTestGridProjectsResultTypeDef",
+    "UpdateTestGridProjectResultTypeDef",
     "DevicePoolCompatibilityResultTypeDef",
     "GetDeviceResultTypeDef",
     "JobTypeDef",
     "ListDevicesResultTypeDef",
     "ProblemTypeDef",
     "RemoteAccessSessionTypeDef",
     "GetRunResultTypeDef",
@@ -530,14 +538,24 @@
         "vpceServiceName": str,
         "serviceDnsName": str,
         "vpceConfigurationDescription": str,
     },
     total=False,
 )
 
+CustomerArtifactPathsOutputTypeDef = TypedDict(
+    "CustomerArtifactPathsOutputTypeDef",
+    {
+        "iosPaths": List[str],
+        "androidPaths": List[str],
+        "deviceHostPaths": List[str],
+    },
+    total=False,
+)
+
 CustomerArtifactPathsTypeDef = TypedDict(
     "CustomerArtifactPathsTypeDef",
     {
         "iosPaths": Sequence[str],
         "androidPaths": Sequence[str],
         "deviceHostPaths": Sequence[str],
     },
@@ -603,20 +621,29 @@
 DeleteVPCEConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteVPCEConfigurationRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+DeviceFilterOutputTypeDef = TypedDict(
+    "DeviceFilterOutputTypeDef",
+    {
+        "attribute": DeviceFilterAttributeType,
+        "operator": RuleOperatorType,
+        "values": List[str],
+    },
+)
+
 DeviceFilterTypeDef = TypedDict(
     "DeviceFilterTypeDef",
     {
         "attribute": DeviceFilterAttributeType,
         "operator": RuleOperatorType,
-        "values": List[str],
+        "values": Sequence[str],
     },
 )
 
 DeviceMinutesTypeDef = TypedDict(
     "DeviceMinutesTypeDef",
     {
         "total": float,
@@ -631,14 +658,24 @@
     {
         "message": str,
         "type": DeviceAttributeType,
     },
     total=False,
 )
 
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "attribute": DeviceAttributeType,
+        "operator": RuleOperatorType,
+        "value": str,
+    },
+    total=False,
+)
+
 ResolutionTypeDef = TypedDict(
     "ResolutionTypeDef",
     {
         "width": int,
         "height": int,
     },
     total=False,
@@ -1295,16 +1332,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 ListTestGridProjectsRequestRequestTypeDef = TypedDict(
@@ -1558,14 +1595,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+LocationOutputTypeDef = TypedDict(
+    "LocationOutputTypeDef",
+    {
+        "latitude": float,
+        "longitude": float,
+    },
+)
+
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "latitude": float,
         "longitude": float,
     },
 )
@@ -1594,14 +1639,23 @@
     {
         "arn": str,
         "name": str,
     },
     total=False,
 )
 
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
+    {
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
+        "vpcId": str,
+    },
+)
+
 _RequiredPurchaseOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseOfferingRequestRequestTypeDef",
     {
         "offeringId": str,
         "quantity": int,
     },
 )
@@ -1616,14 +1670,25 @@
 
 class PurchaseOfferingRequestRequestTypeDef(
     _RequiredPurchaseOfferingRequestRequestTypeDef, _OptionalPurchaseOfferingRequestRequestTypeDef
 ):
     pass
 
 
+RadiosOutputTypeDef = TypedDict(
+    "RadiosOutputTypeDef",
+    {
+        "wifi": bool,
+        "bluetooth": bool,
+        "nfc": bool,
+        "gps": bool,
+    },
+    total=False,
+)
+
 RadiosTypeDef = TypedDict(
     "RadiosTypeDef",
     {
         "wifi": bool,
         "bluetooth": bool,
         "nfc": bool,
         "gps": bool,
@@ -1667,14 +1732,31 @@
 StopRunRequestRequestTypeDef = TypedDict(
     "StopRunRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+TestGridVpcConfigOutputTypeDef = TypedDict(
+    "TestGridVpcConfigOutputTypeDef",
+    {
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
+        "vpcId": str,
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1852,27 +1934,14 @@
 
 class CreateDevicePoolRequestRequestTypeDef(
     _RequiredCreateDevicePoolRequestRequestTypeDef, _OptionalCreateDevicePoolRequestRequestTypeDef
 ):
     pass
 
 
-DevicePoolTypeDef = TypedDict(
-    "DevicePoolTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "type": DevicePoolTypeType,
-        "rules": List[RuleTypeDef],
-        "maxDevices": int,
-    },
-    total=False,
-)
-
 _RequiredUpdateDevicePoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDevicePoolRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateDevicePoolRequestRequestTypeDef = TypedDict(
@@ -1991,26 +2060,14 @@
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
 
-ProjectTypeDef = TypedDict(
-    "ProjectTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "defaultJobTimeoutMinutes": int,
-        "created": datetime,
-        "vpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -2081,26 +2138,14 @@
 class CreateTestGridProjectRequestRequestTypeDef(
     _RequiredCreateTestGridProjectRequestRequestTypeDef,
     _OptionalCreateTestGridProjectRequestRequestTypeDef,
 ):
     pass
 
 
-TestGridProjectTypeDef = TypedDict(
-    "TestGridProjectTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "vpcConfig": TestGridVpcConfigTypeDef,
-        "created": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateTestGridProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTestGridProjectRequestRequestTypeDef",
     {
         "projectArn": str,
     },
 )
 _OptionalUpdateTestGridProjectRequestRequestTypeDef = TypedDict(
@@ -2191,30 +2236,30 @@
     "UpdateVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeviceSelectionConfigurationTypeDef = TypedDict(
-    "DeviceSelectionConfigurationTypeDef",
+DeviceSelectionResultTypeDef = TypedDict(
+    "DeviceSelectionResultTypeDef",
     {
-        "filters": Sequence[DeviceFilterTypeDef],
+        "filters": List[DeviceFilterOutputTypeDef],
+        "matchedDevicesCount": int,
         "maxDevices": int,
     },
+    total=False,
 )
 
-DeviceSelectionResultTypeDef = TypedDict(
-    "DeviceSelectionResultTypeDef",
+DeviceSelectionConfigurationTypeDef = TypedDict(
+    "DeviceSelectionConfigurationTypeDef",
     {
-        "filters": List[DeviceFilterTypeDef],
-        "matchedDevicesCount": int,
+        "filters": Sequence[DeviceFilterTypeDef],
         "maxDevices": int,
     },
-    total=False,
 )
 
 ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
     "ListDevicesRequestListDevicesPaginateTypeDef",
     {
         "arn": str,
         "filters": Sequence[DeviceFilterTypeDef],
@@ -2265,14 +2310,27 @@
         "counters": CountersTypeDef,
         "message": str,
         "deviceMinutes": DeviceMinutesTypeDef,
     },
     total=False,
 )
 
+DevicePoolTypeDef = TypedDict(
+    "DevicePoolTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "type": DevicePoolTypeType,
+        "rules": List[RuleOutputTypeDef],
+        "maxDevices": int,
+    },
+    total=False,
+)
+
 GetTestGridSessionResultTypeDef = TypedDict(
     "GetTestGridSessionResultTypeDef",
     {
         "testGridSession": TestGridSessionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2303,27 +2361,19 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 ListTestGridSessionActionsResultTypeDef = TypedDict(
     "ListTestGridSessionActionsResultTypeDef",
     {
         "actions": List[TestGridSessionActionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2343,14 +2393,26 @@
     {
         "cost": MonetaryAmountTypeDef,
         "frequency": Literal["MONTHLY"],
     },
     total=False,
 )
 
+ProjectTypeDef = TypedDict(
+    "ProjectTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "defaultJobTimeoutMinutes": int,
+        "created": datetime,
+        "vpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ScheduleRunConfigurationTypeDef = TypedDict(
     "ScheduleRunConfigurationTypeDef",
     {
         "extraDataPackageArn": str,
         "networkProfileArn": str,
         "locale": str,
         "location": LocationTypeDef,
@@ -2359,51 +2421,38 @@
         "radios": RadiosTypeDef,
         "auxiliaryApps": Sequence[str],
         "billingMethod": BillingMethodType,
     },
     total=False,
 )
 
-GetAccountSettingsResultTypeDef = TypedDict(
-    "GetAccountSettingsResultTypeDef",
-    {
-        "accountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDevicePoolResultTypeDef = TypedDict(
-    "CreateDevicePoolResultTypeDef",
-    {
-        "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDevicePoolResultTypeDef = TypedDict(
-    "GetDevicePoolResultTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-ListDevicePoolsResultTypeDef = TypedDict(
-    "ListDevicePoolsResultTypeDef",
+TestGridProjectTypeDef = TypedDict(
+    "TestGridProjectTypeDef",
     {
-        "devicePools": List[DevicePoolTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "arn": str,
+        "name": str,
+        "description": str,
+        "vpcConfig": TestGridVpcConfigOutputTypeDef,
+        "created": datetime,
     },
+    total=False,
 )
 
-UpdateDevicePoolResultTypeDef = TypedDict(
-    "UpdateDevicePoolResultTypeDef",
+GetAccountSettingsResultTypeDef = TypedDict(
+    "GetAccountSettingsResultTypeDef",
     {
-        "devicePool": DevicePoolTypeDef,
+        "accountSettings": AccountSettingsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
@@ -2453,80 +2502,14 @@
     "UpdateDeviceInstanceResultTypeDef",
     {
         "deviceInstance": DeviceInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateProjectResultTypeDef = TypedDict(
-    "CreateProjectResultTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetProjectResultTypeDef = TypedDict(
-    "GetProjectResultTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListProjectsResultTypeDef = TypedDict(
-    "ListProjectsResultTypeDef",
-    {
-        "projects": List[ProjectTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateProjectResultTypeDef = TypedDict(
-    "UpdateProjectResultTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTestGridProjectResultTypeDef = TypedDict(
-    "CreateTestGridProjectResultTypeDef",
-    {
-        "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetTestGridProjectResultTypeDef = TypedDict(
-    "GetTestGridProjectResultTypeDef",
-    {
-        "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTestGridProjectsResultTypeDef = TypedDict(
-    "ListTestGridProjectsResultTypeDef",
-    {
-        "testGridProjects": List[TestGridProjectTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateTestGridProjectResultTypeDef = TypedDict(
-    "UpdateTestGridProjectResultTypeDef",
-    {
-        "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RunTypeDef = TypedDict(
     "RunTypeDef",
     {
         "arn": str,
         "name": str,
         "type": TestTypeType,
         "platform": DevicePlatformType,
@@ -2546,22 +2529,22 @@
         "resultCode": ExecutionResultCodeType,
         "seed": int,
         "appUpload": str,
         "eventCount": int,
         "jobTimeoutMinutes": int,
         "devicePoolArn": str,
         "locale": str,
-        "radios": RadiosTypeDef,
-        "location": LocationTypeDef,
-        "customerArtifactPaths": CustomerArtifactPathsTypeDef,
+        "radios": RadiosOutputTypeDef,
+        "location": LocationOutputTypeDef,
+        "customerArtifactPaths": CustomerArtifactPathsOutputTypeDef,
         "webUrl": str,
         "skipAppResign": bool,
         "testSpecArn": str,
         "deviceSelectionResult": DeviceSelectionResultTypeDef,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
 GetSuiteResultTypeDef = TypedDict(
     "GetSuiteResultTypeDef",
     {
@@ -2592,26 +2575,92 @@
     {
         "tests": List[TestTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateDevicePoolResultTypeDef = TypedDict(
+    "CreateDevicePoolResultTypeDef",
+    {
+        "devicePool": DevicePoolTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDevicePoolResultTypeDef = TypedDict(
+    "GetDevicePoolResultTypeDef",
+    {
+        "devicePool": DevicePoolTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDevicePoolsResultTypeDef = TypedDict(
+    "ListDevicePoolsResultTypeDef",
+    {
+        "devicePools": List[DevicePoolTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateDevicePoolResultTypeDef = TypedDict(
+    "UpdateDevicePoolResultTypeDef",
+    {
+        "devicePool": DevicePoolTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "id": str,
         "description": str,
         "type": Literal["RECURRING"],
         "platform": DevicePlatformType,
         "recurringCharges": List[RecurringChargeTypeDef],
     },
     total=False,
 )
 
+CreateProjectResultTypeDef = TypedDict(
+    "CreateProjectResultTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetProjectResultTypeDef = TypedDict(
+    "GetProjectResultTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListProjectsResultTypeDef = TypedDict(
+    "ListProjectsResultTypeDef",
+    {
+        "projects": List[ProjectTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateProjectResultTypeDef = TypedDict(
+    "UpdateProjectResultTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDevicePoolCompatibilityRequestRequestTypeDef = TypedDict(
     "_RequiredGetDevicePoolCompatibilityRequestRequestTypeDef",
     {
         "devicePoolArn": str,
     },
 )
 _OptionalGetDevicePoolCompatibilityRequestRequestTypeDef = TypedDict(
@@ -2656,14 +2705,47 @@
 
 class ScheduleRunRequestRequestTypeDef(
     _RequiredScheduleRunRequestRequestTypeDef, _OptionalScheduleRunRequestRequestTypeDef
 ):
     pass
 
 
+CreateTestGridProjectResultTypeDef = TypedDict(
+    "CreateTestGridProjectResultTypeDef",
+    {
+        "testGridProject": TestGridProjectTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetTestGridProjectResultTypeDef = TypedDict(
+    "GetTestGridProjectResultTypeDef",
+    {
+        "testGridProject": TestGridProjectTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTestGridProjectsResultTypeDef = TypedDict(
+    "ListTestGridProjectsResultTypeDef",
+    {
+        "testGridProjects": List[TestGridProjectTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateTestGridProjectResultTypeDef = TypedDict(
+    "UpdateTestGridProjectResultTypeDef",
+    {
+        "testGridProject": TestGridProjectTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DevicePoolCompatibilityResultTypeDef = TypedDict(
     "DevicePoolCompatibilityResultTypeDef",
     {
         "device": DeviceTypeDef,
         "compatible": bool,
         "incompatibilityMessages": List[IncompatibilityMessageTypeDef],
     },
@@ -2743,15 +2825,15 @@
         "clientId": str,
         "billingMethod": BillingMethodType,
         "deviceMinutes": DeviceMinutesTypeDef,
         "endpoint": str,
         "deviceUdid": str,
         "interactionMode": InteractionModeType,
         "skipAppResign": bool,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
 GetRunResultTypeDef = TypedDict(
     "GetRunResultTypeDef",
     {
```

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm/type_defs.pyi` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -67,27 +67,30 @@
     "TestGridVpcConfigTypeDef",
     "CreateTestGridUrlRequestRequestTypeDef",
     "CreateTestGridUrlResultTypeDef",
     "CreateUploadRequestRequestTypeDef",
     "UploadTypeDef",
     "CreateVPCEConfigurationRequestRequestTypeDef",
     "VPCEConfigurationTypeDef",
+    "CustomerArtifactPathsOutputTypeDef",
     "CustomerArtifactPathsTypeDef",
     "DeleteDevicePoolRequestRequestTypeDef",
     "DeleteInstanceProfileRequestRequestTypeDef",
     "DeleteNetworkProfileRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteRemoteAccessSessionRequestRequestTypeDef",
     "DeleteRunRequestRequestTypeDef",
     "DeleteTestGridProjectRequestRequestTypeDef",
     "DeleteUploadRequestRequestTypeDef",
     "DeleteVPCEConfigurationRequestRequestTypeDef",
+    "DeviceFilterOutputTypeDef",
     "DeviceFilterTypeDef",
     "DeviceMinutesTypeDef",
     "IncompatibilityMessageTypeDef",
+    "RuleOutputTypeDef",
     "ResolutionTypeDef",
     "ExecutionConfigurationTypeDef",
     "GetDeviceInstanceRequestRequestTypeDef",
     "ScheduleRunTestTypeDef",
     "GetDevicePoolRequestRequestTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetInstanceProfileRequestRequestTypeDef",
@@ -133,117 +136,122 @@
     "ListRunsRequestRequestTypeDef",
     "ListSamplesRequestListSamplesPaginateTypeDef",
     "ListSamplesRequestRequestTypeDef",
     "SampleTypeDef",
     "ListSuitesRequestListSuitesPaginateTypeDef",
     "ListSuitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ListTestGridProjectsRequestRequestTypeDef",
     "ListTestGridSessionActionsRequestRequestTypeDef",
     "TestGridSessionActionTypeDef",
     "ListTestGridSessionArtifactsRequestRequestTypeDef",
     "TestGridSessionArtifactTypeDef",
     "ListTestGridSessionsRequestRequestTypeDef",
     "ListTestsRequestListTestsPaginateTypeDef",
     "ListTestsRequestRequestTypeDef",
     "ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef",
     "ListUniqueProblemsRequestRequestTypeDef",
     "ListUploadsRequestListUploadsPaginateTypeDef",
     "ListUploadsRequestRequestTypeDef",
     "ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef",
     "ListVPCEConfigurationsRequestRequestTypeDef",
+    "LocationOutputTypeDef",
     "LocationTypeDef",
     "MonetaryAmountTypeDef",
     "PaginatorConfigTypeDef",
     "ProblemDetailTypeDef",
+    "VpcConfigOutputTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
+    "RadiosOutputTypeDef",
     "RadiosTypeDef",
     "RenewOfferingRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "StopJobRequestRequestTypeDef",
     "StopRemoteAccessSessionRequestRequestTypeDef",
     "StopRunRequestRequestTypeDef",
+    "TagTypeDef",
+    "TestGridVpcConfigOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceInstanceRequestRequestTypeDef",
     "UpdateInstanceProfileRequestRequestTypeDef",
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateUploadRequestRequestTypeDef",
     "UpdateVPCEConfigurationRequestRequestTypeDef",
     "AccountSettingsTypeDef",
     "ListArtifactsResultTypeDef",
     "CreateDevicePoolRequestRequestTypeDef",
-    "DevicePoolTypeDef",
     "UpdateDevicePoolRequestRequestTypeDef",
     "CreateInstanceProfileResultTypeDef",
     "DeviceInstanceTypeDef",
     "GetInstanceProfileResultTypeDef",
     "ListInstanceProfilesResultTypeDef",
     "UpdateInstanceProfileResultTypeDef",
     "CreateNetworkProfileResultTypeDef",
     "GetNetworkProfileResultTypeDef",
     "ListNetworkProfilesResultTypeDef",
     "UpdateNetworkProfileResultTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "ProjectTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "CreateRemoteAccessSessionRequestRequestTypeDef",
     "CreateTestGridProjectRequestRequestTypeDef",
-    "TestGridProjectTypeDef",
     "UpdateTestGridProjectRequestRequestTypeDef",
     "CreateUploadResultTypeDef",
     "GetUploadResultTypeDef",
     "InstallToRemoteAccessSessionResultTypeDef",
     "ListUploadsResultTypeDef",
     "UpdateUploadResultTypeDef",
     "CreateVPCEConfigurationResultTypeDef",
     "GetVPCEConfigurationResultTypeDef",
     "ListVPCEConfigurationsResultTypeDef",
     "UpdateVPCEConfigurationResultTypeDef",
-    "DeviceSelectionConfigurationTypeDef",
     "DeviceSelectionResultTypeDef",
+    "DeviceSelectionConfigurationTypeDef",
     "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "SuiteTypeDef",
     "TestTypeDef",
+    "DevicePoolTypeDef",
     "GetTestGridSessionResultTypeDef",
     "ListTestGridSessionsResultTypeDef",
     "ListOfferingPromotionsResultTypeDef",
     "ListSamplesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "ListTestGridSessionActionsResultTypeDef",
     "ListTestGridSessionArtifactsResultTypeDef",
     "RecurringChargeTypeDef",
+    "ProjectTypeDef",
     "ScheduleRunConfigurationTypeDef",
+    "TagResourceRequestRequestTypeDef",
+    "TestGridProjectTypeDef",
     "GetAccountSettingsResultTypeDef",
-    "CreateDevicePoolResultTypeDef",
-    "GetDevicePoolResultTypeDef",
-    "ListDevicePoolsResultTypeDef",
-    "UpdateDevicePoolResultTypeDef",
     "DeviceTypeDef",
     "GetDeviceInstanceResultTypeDef",
     "ListDeviceInstancesResultTypeDef",
     "UpdateDeviceInstanceResultTypeDef",
-    "CreateProjectResultTypeDef",
-    "GetProjectResultTypeDef",
-    "ListProjectsResultTypeDef",
-    "UpdateProjectResultTypeDef",
-    "CreateTestGridProjectResultTypeDef",
-    "GetTestGridProjectResultTypeDef",
-    "ListTestGridProjectsResultTypeDef",
-    "UpdateTestGridProjectResultTypeDef",
     "RunTypeDef",
     "GetSuiteResultTypeDef",
     "ListSuitesResultTypeDef",
     "GetTestResultTypeDef",
     "ListTestsResultTypeDef",
+    "CreateDevicePoolResultTypeDef",
+    "GetDevicePoolResultTypeDef",
+    "ListDevicePoolsResultTypeDef",
+    "UpdateDevicePoolResultTypeDef",
     "OfferingTypeDef",
+    "CreateProjectResultTypeDef",
+    "GetProjectResultTypeDef",
+    "ListProjectsResultTypeDef",
+    "UpdateProjectResultTypeDef",
     "GetDevicePoolCompatibilityRequestRequestTypeDef",
     "ScheduleRunRequestRequestTypeDef",
+    "CreateTestGridProjectResultTypeDef",
+    "GetTestGridProjectResultTypeDef",
+    "ListTestGridProjectsResultTypeDef",
+    "UpdateTestGridProjectResultTypeDef",
     "DevicePoolCompatibilityResultTypeDef",
     "GetDeviceResultTypeDef",
     "JobTypeDef",
     "ListDevicesResultTypeDef",
     "ProblemTypeDef",
     "RemoteAccessSessionTypeDef",
     "GetRunResultTypeDef",
@@ -521,14 +529,24 @@
         "vpceServiceName": str,
         "serviceDnsName": str,
         "vpceConfigurationDescription": str,
     },
     total=False,
 )
 
+CustomerArtifactPathsOutputTypeDef = TypedDict(
+    "CustomerArtifactPathsOutputTypeDef",
+    {
+        "iosPaths": List[str],
+        "androidPaths": List[str],
+        "deviceHostPaths": List[str],
+    },
+    total=False,
+)
+
 CustomerArtifactPathsTypeDef = TypedDict(
     "CustomerArtifactPathsTypeDef",
     {
         "iosPaths": Sequence[str],
         "androidPaths": Sequence[str],
         "deviceHostPaths": Sequence[str],
     },
@@ -594,20 +612,29 @@
 DeleteVPCEConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteVPCEConfigurationRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+DeviceFilterOutputTypeDef = TypedDict(
+    "DeviceFilterOutputTypeDef",
+    {
+        "attribute": DeviceFilterAttributeType,
+        "operator": RuleOperatorType,
+        "values": List[str],
+    },
+)
+
 DeviceFilterTypeDef = TypedDict(
     "DeviceFilterTypeDef",
     {
         "attribute": DeviceFilterAttributeType,
         "operator": RuleOperatorType,
-        "values": List[str],
+        "values": Sequence[str],
     },
 )
 
 DeviceMinutesTypeDef = TypedDict(
     "DeviceMinutesTypeDef",
     {
         "total": float,
@@ -622,14 +649,24 @@
     {
         "message": str,
         "type": DeviceAttributeType,
     },
     total=False,
 )
 
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "attribute": DeviceAttributeType,
+        "operator": RuleOperatorType,
+        "value": str,
+    },
+    total=False,
+)
+
 ResolutionTypeDef = TypedDict(
     "ResolutionTypeDef",
     {
         "width": int,
         "height": int,
     },
     total=False,
@@ -1252,16 +1289,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 ListTestGridProjectsRequestRequestTypeDef = TypedDict(
@@ -1497,14 +1534,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+LocationOutputTypeDef = TypedDict(
+    "LocationOutputTypeDef",
+    {
+        "latitude": float,
+        "longitude": float,
+    },
+)
+
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "latitude": float,
         "longitude": float,
     },
 )
@@ -1533,14 +1578,23 @@
     {
         "arn": str,
         "name": str,
     },
     total=False,
 )
 
+VpcConfigOutputTypeDef = TypedDict(
+    "VpcConfigOutputTypeDef",
+    {
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
+        "vpcId": str,
+    },
+)
+
 _RequiredPurchaseOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseOfferingRequestRequestTypeDef",
     {
         "offeringId": str,
         "quantity": int,
     },
 )
@@ -1553,14 +1607,25 @@
 )
 
 class PurchaseOfferingRequestRequestTypeDef(
     _RequiredPurchaseOfferingRequestRequestTypeDef, _OptionalPurchaseOfferingRequestRequestTypeDef
 ):
     pass
 
+RadiosOutputTypeDef = TypedDict(
+    "RadiosOutputTypeDef",
+    {
+        "wifi": bool,
+        "bluetooth": bool,
+        "nfc": bool,
+        "gps": bool,
+    },
+    total=False,
+)
+
 RadiosTypeDef = TypedDict(
     "RadiosTypeDef",
     {
         "wifi": bool,
         "bluetooth": bool,
         "nfc": bool,
         "gps": bool,
@@ -1604,14 +1669,31 @@
 StopRunRequestRequestTypeDef = TypedDict(
     "StopRunRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+TestGridVpcConfigOutputTypeDef = TypedDict(
+    "TestGridVpcConfigOutputTypeDef",
+    {
+        "securityGroupIds": List[str],
+        "subnetIds": List[str],
+        "vpcId": str,
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1777,27 +1859,14 @@
 )
 
 class CreateDevicePoolRequestRequestTypeDef(
     _RequiredCreateDevicePoolRequestRequestTypeDef, _OptionalCreateDevicePoolRequestRequestTypeDef
 ):
     pass
 
-DevicePoolTypeDef = TypedDict(
-    "DevicePoolTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "type": DevicePoolTypeType,
-        "rules": List[RuleTypeDef],
-        "maxDevices": int,
-    },
-    total=False,
-)
-
 _RequiredUpdateDevicePoolRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDevicePoolRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateDevicePoolRequestRequestTypeDef = TypedDict(
@@ -1912,26 +1981,14 @@
 )
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-ProjectTypeDef = TypedDict(
-    "ProjectTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "defaultJobTimeoutMinutes": int,
-        "created": datetime,
-        "vpcConfig": VpcConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -1996,26 +2053,14 @@
 
 class CreateTestGridProjectRequestRequestTypeDef(
     _RequiredCreateTestGridProjectRequestRequestTypeDef,
     _OptionalCreateTestGridProjectRequestRequestTypeDef,
 ):
     pass
 
-TestGridProjectTypeDef = TypedDict(
-    "TestGridProjectTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "vpcConfig": TestGridVpcConfigTypeDef,
-        "created": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateTestGridProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTestGridProjectRequestRequestTypeDef",
     {
         "projectArn": str,
     },
 )
 _OptionalUpdateTestGridProjectRequestRequestTypeDef = TypedDict(
@@ -2104,30 +2149,30 @@
     "UpdateVPCEConfigurationResultTypeDef",
     {
         "vpceConfiguration": VPCEConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeviceSelectionConfigurationTypeDef = TypedDict(
-    "DeviceSelectionConfigurationTypeDef",
+DeviceSelectionResultTypeDef = TypedDict(
+    "DeviceSelectionResultTypeDef",
     {
-        "filters": Sequence[DeviceFilterTypeDef],
+        "filters": List[DeviceFilterOutputTypeDef],
+        "matchedDevicesCount": int,
         "maxDevices": int,
     },
+    total=False,
 )
 
-DeviceSelectionResultTypeDef = TypedDict(
-    "DeviceSelectionResultTypeDef",
+DeviceSelectionConfigurationTypeDef = TypedDict(
+    "DeviceSelectionConfigurationTypeDef",
     {
-        "filters": List[DeviceFilterTypeDef],
-        "matchedDevicesCount": int,
+        "filters": Sequence[DeviceFilterTypeDef],
         "maxDevices": int,
     },
-    total=False,
 )
 
 ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
     "ListDevicesRequestListDevicesPaginateTypeDef",
     {
         "arn": str,
         "filters": Sequence[DeviceFilterTypeDef],
@@ -2178,14 +2223,27 @@
         "counters": CountersTypeDef,
         "message": str,
         "deviceMinutes": DeviceMinutesTypeDef,
     },
     total=False,
 )
 
+DevicePoolTypeDef = TypedDict(
+    "DevicePoolTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "type": DevicePoolTypeType,
+        "rules": List[RuleOutputTypeDef],
+        "maxDevices": int,
+    },
+    total=False,
+)
+
 GetTestGridSessionResultTypeDef = TypedDict(
     "GetTestGridSessionResultTypeDef",
     {
         "testGridSession": TestGridSessionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2216,27 +2274,19 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 ListTestGridSessionActionsResultTypeDef = TypedDict(
     "ListTestGridSessionActionsResultTypeDef",
     {
         "actions": List[TestGridSessionActionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2256,14 +2306,26 @@
     {
         "cost": MonetaryAmountTypeDef,
         "frequency": Literal["MONTHLY"],
     },
     total=False,
 )
 
+ProjectTypeDef = TypedDict(
+    "ProjectTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "defaultJobTimeoutMinutes": int,
+        "created": datetime,
+        "vpcConfig": VpcConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 ScheduleRunConfigurationTypeDef = TypedDict(
     "ScheduleRunConfigurationTypeDef",
     {
         "extraDataPackageArn": str,
         "networkProfileArn": str,
         "locale": str,
         "location": LocationTypeDef,
@@ -2272,51 +2334,38 @@
         "radios": RadiosTypeDef,
         "auxiliaryApps": Sequence[str],
         "billingMethod": BillingMethodType,
     },
     total=False,
 )
 
-GetAccountSettingsResultTypeDef = TypedDict(
-    "GetAccountSettingsResultTypeDef",
-    {
-        "accountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDevicePoolResultTypeDef = TypedDict(
-    "CreateDevicePoolResultTypeDef",
-    {
-        "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDevicePoolResultTypeDef = TypedDict(
-    "GetDevicePoolResultTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "devicePool": DevicePoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-ListDevicePoolsResultTypeDef = TypedDict(
-    "ListDevicePoolsResultTypeDef",
+TestGridProjectTypeDef = TypedDict(
+    "TestGridProjectTypeDef",
     {
-        "devicePools": List[DevicePoolTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "arn": str,
+        "name": str,
+        "description": str,
+        "vpcConfig": TestGridVpcConfigOutputTypeDef,
+        "created": datetime,
     },
+    total=False,
 )
 
-UpdateDevicePoolResultTypeDef = TypedDict(
-    "UpdateDevicePoolResultTypeDef",
+GetAccountSettingsResultTypeDef = TypedDict(
+    "GetAccountSettingsResultTypeDef",
     {
-        "devicePool": DevicePoolTypeDef,
+        "accountSettings": AccountSettingsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
@@ -2366,80 +2415,14 @@
     "UpdateDeviceInstanceResultTypeDef",
     {
         "deviceInstance": DeviceInstanceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateProjectResultTypeDef = TypedDict(
-    "CreateProjectResultTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetProjectResultTypeDef = TypedDict(
-    "GetProjectResultTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListProjectsResultTypeDef = TypedDict(
-    "ListProjectsResultTypeDef",
-    {
-        "projects": List[ProjectTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateProjectResultTypeDef = TypedDict(
-    "UpdateProjectResultTypeDef",
-    {
-        "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTestGridProjectResultTypeDef = TypedDict(
-    "CreateTestGridProjectResultTypeDef",
-    {
-        "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetTestGridProjectResultTypeDef = TypedDict(
-    "GetTestGridProjectResultTypeDef",
-    {
-        "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTestGridProjectsResultTypeDef = TypedDict(
-    "ListTestGridProjectsResultTypeDef",
-    {
-        "testGridProjects": List[TestGridProjectTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateTestGridProjectResultTypeDef = TypedDict(
-    "UpdateTestGridProjectResultTypeDef",
-    {
-        "testGridProject": TestGridProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RunTypeDef = TypedDict(
     "RunTypeDef",
     {
         "arn": str,
         "name": str,
         "type": TestTypeType,
         "platform": DevicePlatformType,
@@ -2459,22 +2442,22 @@
         "resultCode": ExecutionResultCodeType,
         "seed": int,
         "appUpload": str,
         "eventCount": int,
         "jobTimeoutMinutes": int,
         "devicePoolArn": str,
         "locale": str,
-        "radios": RadiosTypeDef,
-        "location": LocationTypeDef,
-        "customerArtifactPaths": CustomerArtifactPathsTypeDef,
+        "radios": RadiosOutputTypeDef,
+        "location": LocationOutputTypeDef,
+        "customerArtifactPaths": CustomerArtifactPathsOutputTypeDef,
         "webUrl": str,
         "skipAppResign": bool,
         "testSpecArn": str,
         "deviceSelectionResult": DeviceSelectionResultTypeDef,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
 GetSuiteResultTypeDef = TypedDict(
     "GetSuiteResultTypeDef",
     {
@@ -2505,26 +2488,92 @@
     {
         "tests": List[TestTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateDevicePoolResultTypeDef = TypedDict(
+    "CreateDevicePoolResultTypeDef",
+    {
+        "devicePool": DevicePoolTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetDevicePoolResultTypeDef = TypedDict(
+    "GetDevicePoolResultTypeDef",
+    {
+        "devicePool": DevicePoolTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDevicePoolsResultTypeDef = TypedDict(
+    "ListDevicePoolsResultTypeDef",
+    {
+        "devicePools": List[DevicePoolTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateDevicePoolResultTypeDef = TypedDict(
+    "UpdateDevicePoolResultTypeDef",
+    {
+        "devicePool": DevicePoolTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "id": str,
         "description": str,
         "type": Literal["RECURRING"],
         "platform": DevicePlatformType,
         "recurringCharges": List[RecurringChargeTypeDef],
     },
     total=False,
 )
 
+CreateProjectResultTypeDef = TypedDict(
+    "CreateProjectResultTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetProjectResultTypeDef = TypedDict(
+    "GetProjectResultTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListProjectsResultTypeDef = TypedDict(
+    "ListProjectsResultTypeDef",
+    {
+        "projects": List[ProjectTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateProjectResultTypeDef = TypedDict(
+    "UpdateProjectResultTypeDef",
+    {
+        "project": ProjectTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetDevicePoolCompatibilityRequestRequestTypeDef = TypedDict(
     "_RequiredGetDevicePoolCompatibilityRequestRequestTypeDef",
     {
         "devicePoolArn": str,
     },
 )
 _OptionalGetDevicePoolCompatibilityRequestRequestTypeDef = TypedDict(
@@ -2565,14 +2614,47 @@
 )
 
 class ScheduleRunRequestRequestTypeDef(
     _RequiredScheduleRunRequestRequestTypeDef, _OptionalScheduleRunRequestRequestTypeDef
 ):
     pass
 
+CreateTestGridProjectResultTypeDef = TypedDict(
+    "CreateTestGridProjectResultTypeDef",
+    {
+        "testGridProject": TestGridProjectTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetTestGridProjectResultTypeDef = TypedDict(
+    "GetTestGridProjectResultTypeDef",
+    {
+        "testGridProject": TestGridProjectTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListTestGridProjectsResultTypeDef = TypedDict(
+    "ListTestGridProjectsResultTypeDef",
+    {
+        "testGridProjects": List[TestGridProjectTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateTestGridProjectResultTypeDef = TypedDict(
+    "UpdateTestGridProjectResultTypeDef",
+    {
+        "testGridProject": TestGridProjectTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DevicePoolCompatibilityResultTypeDef = TypedDict(
     "DevicePoolCompatibilityResultTypeDef",
     {
         "device": DeviceTypeDef,
         "compatible": bool,
         "incompatibilityMessages": List[IncompatibilityMessageTypeDef],
     },
@@ -2652,15 +2734,15 @@
         "clientId": str,
         "billingMethod": BillingMethodType,
         "deviceMinutes": DeviceMinutesTypeDef,
         "endpoint": str,
         "deviceUdid": str,
         "interactionMode": InteractionModeType,
         "skipAppResign": bool,
-        "vpcConfig": VpcConfigTypeDef,
+        "vpcConfig": VpcConfigOutputTypeDef,
     },
     total=False,
 )
 
 GetRunResultTypeDef = TypedDict(
     "GetRunResultTypeDef",
     {
```

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm.egg-info/PKG-INFO` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devicefarm
-Version: 1.28.0
-Summary: Type annotations for boto3.DeviceFarm 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DeviceFarm 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-devicefarm"></a>
 
 # mypy-boto3-devicefarm
 
 [![PyPI - mypy-boto3-devicefarm](https://img.shields.io/pypi/v/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devicefarm.svg?color=blue)](https://pypi.org/project/mypy-boto3-devicefarm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devicefarm?color=blue)](https://pypistats.org/packages/mypy-boto3-devicefarm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-devicefarm)](https://pepy.tech/project/mypy-boto3-devicefarm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DeviceFarm 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
+[boto3.DeviceFarm 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm)
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -441,27 +441,30 @@
     TestGridVpcConfigTypeDef,
     CreateTestGridUrlRequestRequestTypeDef,
     CreateTestGridUrlResultTypeDef,
     CreateUploadRequestRequestTypeDef,
     UploadTypeDef,
     CreateVPCEConfigurationRequestRequestTypeDef,
     VPCEConfigurationTypeDef,
+    CustomerArtifactPathsOutputTypeDef,
     CustomerArtifactPathsTypeDef,
     DeleteDevicePoolRequestRequestTypeDef,
     DeleteInstanceProfileRequestRequestTypeDef,
     DeleteNetworkProfileRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteRemoteAccessSessionRequestRequestTypeDef,
     DeleteRunRequestRequestTypeDef,
     DeleteTestGridProjectRequestRequestTypeDef,
     DeleteUploadRequestRequestTypeDef,
     DeleteVPCEConfigurationRequestRequestTypeDef,
+    DeviceFilterOutputTypeDef,
     DeviceFilterTypeDef,
     DeviceMinutesTypeDef,
     IncompatibilityMessageTypeDef,
+    RuleOutputTypeDef,
     ResolutionTypeDef,
     ExecutionConfigurationTypeDef,
     GetDeviceInstanceRequestRequestTypeDef,
     ScheduleRunTestTypeDef,
     GetDevicePoolRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
@@ -507,117 +510,122 @@
     ListRunsRequestRequestTypeDef,
     ListSamplesRequestListSamplesPaginateTypeDef,
     ListSamplesRequestRequestTypeDef,
     SampleTypeDef,
     ListSuitesRequestListSuitesPaginateTypeDef,
     ListSuitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ListTestGridProjectsRequestRequestTypeDef,
     ListTestGridSessionActionsRequestRequestTypeDef,
     TestGridSessionActionTypeDef,
     ListTestGridSessionArtifactsRequestRequestTypeDef,
     TestGridSessionArtifactTypeDef,
     ListTestGridSessionsRequestRequestTypeDef,
     ListTestsRequestListTestsPaginateTypeDef,
     ListTestsRequestRequestTypeDef,
     ListUniqueProblemsRequestListUniqueProblemsPaginateTypeDef,
     ListUniqueProblemsRequestRequestTypeDef,
     ListUploadsRequestListUploadsPaginateTypeDef,
     ListUploadsRequestRequestTypeDef,
     ListVPCEConfigurationsRequestListVPCEConfigurationsPaginateTypeDef,
     ListVPCEConfigurationsRequestRequestTypeDef,
+    LocationOutputTypeDef,
     LocationTypeDef,
     MonetaryAmountTypeDef,
     PaginatorConfigTypeDef,
     ProblemDetailTypeDef,
+    VpcConfigOutputTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
+    RadiosOutputTypeDef,
     RadiosTypeDef,
     RenewOfferingRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     StopJobRequestRequestTypeDef,
     StopRemoteAccessSessionRequestRequestTypeDef,
     StopRunRequestRequestTypeDef,
+    TagTypeDef,
+    TestGridVpcConfigOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceInstanceRequestRequestTypeDef,
     UpdateInstanceProfileRequestRequestTypeDef,
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateUploadRequestRequestTypeDef,
     UpdateVPCEConfigurationRequestRequestTypeDef,
     AccountSettingsTypeDef,
     ListArtifactsResultTypeDef,
     CreateDevicePoolRequestRequestTypeDef,
-    DevicePoolTypeDef,
     UpdateDevicePoolRequestRequestTypeDef,
     CreateInstanceProfileResultTypeDef,
     DeviceInstanceTypeDef,
     GetInstanceProfileResultTypeDef,
     ListInstanceProfilesResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     CreateNetworkProfileResultTypeDef,
     GetNetworkProfileResultTypeDef,
     ListNetworkProfilesResultTypeDef,
     UpdateNetworkProfileResultTypeDef,
     CreateProjectRequestRequestTypeDef,
-    ProjectTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateRemoteAccessSessionRequestRequestTypeDef,
     CreateTestGridProjectRequestRequestTypeDef,
-    TestGridProjectTypeDef,
     UpdateTestGridProjectRequestRequestTypeDef,
     CreateUploadResultTypeDef,
     GetUploadResultTypeDef,
     InstallToRemoteAccessSessionResultTypeDef,
     ListUploadsResultTypeDef,
     UpdateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
     GetVPCEConfigurationResultTypeDef,
     ListVPCEConfigurationsResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
-    DeviceSelectionConfigurationTypeDef,
     DeviceSelectionResultTypeDef,
+    DeviceSelectionConfigurationTypeDef,
     ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     SuiteTypeDef,
     TestTypeDef,
+    DevicePoolTypeDef,
     GetTestGridSessionResultTypeDef,
     ListTestGridSessionsResultTypeDef,
     ListOfferingPromotionsResultTypeDef,
     ListSamplesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     ListTestGridSessionActionsResultTypeDef,
     ListTestGridSessionArtifactsResultTypeDef,
     RecurringChargeTypeDef,
+    ProjectTypeDef,
     ScheduleRunConfigurationTypeDef,
+    TagResourceRequestRequestTypeDef,
+    TestGridProjectTypeDef,
     GetAccountSettingsResultTypeDef,
-    CreateDevicePoolResultTypeDef,
-    GetDevicePoolResultTypeDef,
-    ListDevicePoolsResultTypeDef,
-    UpdateDevicePoolResultTypeDef,
     DeviceTypeDef,
     GetDeviceInstanceResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     UpdateDeviceInstanceResultTypeDef,
-    CreateProjectResultTypeDef,
-    GetProjectResultTypeDef,
-    ListProjectsResultTypeDef,
-    UpdateProjectResultTypeDef,
-    CreateTestGridProjectResultTypeDef,
-    GetTestGridProjectResultTypeDef,
-    ListTestGridProjectsResultTypeDef,
-    UpdateTestGridProjectResultTypeDef,
     RunTypeDef,
     GetSuiteResultTypeDef,
     ListSuitesResultTypeDef,
     GetTestResultTypeDef,
     ListTestsResultTypeDef,
+    CreateDevicePoolResultTypeDef,
+    GetDevicePoolResultTypeDef,
+    ListDevicePoolsResultTypeDef,
+    UpdateDevicePoolResultTypeDef,
     OfferingTypeDef,
+    CreateProjectResultTypeDef,
+    GetProjectResultTypeDef,
+    ListProjectsResultTypeDef,
+    UpdateProjectResultTypeDef,
     GetDevicePoolCompatibilityRequestRequestTypeDef,
     ScheduleRunRequestRequestTypeDef,
+    CreateTestGridProjectResultTypeDef,
+    GetTestGridProjectResultTypeDef,
+    ListTestGridProjectsResultTypeDef,
+    UpdateTestGridProjectResultTypeDef,
     DevicePoolCompatibilityResultTypeDef,
     GetDeviceResultTypeDef,
     JobTypeDef,
     ListDevicesResultTypeDef,
     ProblemTypeDef,
     RemoteAccessSessionTypeDef,
     GetRunResultTypeDef,
```

### Comparing `mypy-boto3-devicefarm-1.28.0/mypy_boto3_devicefarm.egg-info/SOURCES.txt` & `mypy-boto3-devicefarm-1.28.12/mypy_boto3_devicefarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.0/setup.py` & `mypy-boto3-devicefarm-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-devicefarm",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_devicefarm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DeviceFarm 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.DeviceFarm 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

