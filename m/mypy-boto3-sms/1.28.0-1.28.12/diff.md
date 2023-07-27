# Comparing `tmp/mypy-boto3-sms-1.28.0.tar.gz` & `tmp/mypy-boto3-sms-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sms-1.28.0.tar", last modified: Thu Jul  6 21:00:39 2023, max compression
+gzip compressed data, was "mypy-boto3-sms-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
```

## Comparing `mypy-boto3-sms-1.28.0.tar` & `mypy-boto3-sms-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:39.698435 mypy-boto3-sms-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:02.000000 mypy-boto3-sms-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-07-06 21:00:39.694435 mypy-boto3-sms-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-07-06 20:56:02.000000 mypy-boto3-sms-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:39.678435 mypy-boto3-sms-1.28.0/mypy_boto3_sms/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-06 20:56:03.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-06 20:56:02.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:56:03.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-07-06 20:56:03.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25822 2023-07-06 20:56:03.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-07-06 20:56:03.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-07-06 20:56:03.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-06 20:56:03.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-06 20:56:03.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:03.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28504 2023-07-06 20:56:04.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28487 2023-07-06 20:56:04.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:02.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:39.694435 mypy-boto3-sms-1.28.0/mypy_boto3_sms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-07-06 21:00:39.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 21:00:39.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:39.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:39.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:39.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:39.000000 mypy-boto3-sms-1.28.0/mypy_boto3_sms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:39.698435 mypy-boto3-sms-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:56:02.000000 mypy-boto3-sms-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.077315 mypy-boto3-sms-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17464 2023-07-27 11:49:41.077315 mypy-boto3-sms-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.077315 mypy-boto3-sms-1.28.12/mypy_boto3_sms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-07-27 11:47:03.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25822 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-07-27 11:47:03.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-07-27 11:47:03.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-27 11:47:03.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-07-27 11:47:03.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34042 2023-07-27 11:47:04.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34025 2023-07-27 11:47:03.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.077315 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17464 2023-07-27 11:49:40.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:40.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:40.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:40.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:40.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:40.000000 mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.077315 mypy-boto3-sms-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:02.000000 mypy-boto3-sms-1.28.12/setup.py
```

### Comparing `mypy-boto3-sms-1.28.0/LICENSE` & `mypy-boto3-sms-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.0/PKG-INFO` & `mypy-boto3-sms-1.28.12/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sms
-Version: 1.28.0
-Summary: Type annotations for boto3.SMS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SMS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sms"></a>
 
 # mypy-boto3-sms
 
 [![PyPI - mypy-boto3-sms](https://img.shields.io/pypi/v/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sms?color=blue)](https://pypistats.org/packages/mypy-boto3-sms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sms)](https://pepy.tech/project/mypy-boto3-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SMS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[boto3.SMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [mypy-boto3-sms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,95 +357,113 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     CreateReplicationJobRequestRequestTypeDef,
-    CreateReplicationJobResponseTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
-    S3LocationTypeDef,
+    S3LocationOutputTypeDef,
     GenerateTemplateRequestRequestTypeDef,
     GetAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
     GetAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputRequestRequestTypeDef,
-    GetConnectorsRequestGetConnectorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetConnectorsRequestRequestTypeDef,
-    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
     GetReplicationJobsRequestRequestTypeDef,
-    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     GetReplicationRunsRequestRequestTypeDef,
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
-    ListAppsRequestListAppsPaginateTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
-    PaginatorConfigTypeDef,
     ReplicationRunStageDetailsTypeDef,
-    ResponseMetadataTypeDef,
+    S3LocationTypeDef,
+    ServerReplicationParametersOutputTypeDef,
     ServerReplicationParametersTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
-    StartOnDemandReplicationRunResponseTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
     UpdateReplicationJobRequestRequestTypeDef,
+    VmServerAddressOutputTypeDef,
     AppSummaryTypeDef,
+    CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
+    StartOnDemandReplicationRunResponseTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
-    SourceTypeDef,
-    UserDataTypeDef,
+    SourceOutputTypeDef,
+    UserDataOutputTypeDef,
+    GetConnectorsRequestGetConnectorsPaginateTypeDef,
+    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
+    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+    ListAppsRequestListAppsPaginateTypeDef,
     GetServersRequestGetServersPaginateTypeDef,
     GetServersRequestRequestTypeDef,
     VmServerTypeDef,
     NotifyAppValidationOutputRequestRequestTypeDef,
     ReplicationRunTypeDef,
+    SourceTypeDef,
+    UserDataTypeDef,
+    VmServerOutputTypeDef,
     ListAppsResponseTypeDef,
     AppValidationOutputTypeDef,
+    SSMValidationParametersOutputTypeDef,
+    UserDataValidationParametersOutputTypeDef,
+    ServerTypeDef,
     SSMValidationParametersTypeDef,
     UserDataValidationParametersTypeDef,
-    ServerTypeDef,
     ReplicationJobTypeDef,
-    AppValidationConfigurationTypeDef,
-    GetServersResponseTypeDef,
+    ServerOutputTypeDef,
+    AppValidationConfigurationOutputTypeDef,
     ServerGroupTypeDef,
     ServerLaunchConfigurationTypeDef,
     ServerReplicationConfigurationTypeDef,
+    AppValidationConfigurationTypeDef,
     ServerValidationConfigurationTypeDef,
-    ServerValidationOutputTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
+    GetServersResponseTypeDef,
+    ServerGroupOutputTypeDef,
+    ServerLaunchConfigurationOutputTypeDef,
+    ServerReplicationConfigurationOutputTypeDef,
+    ServerValidationConfigurationOutputTypeDef,
+    ServerValidationOutputTypeDef,
     CreateAppRequestRequestTypeDef,
-    CreateAppResponseTypeDef,
-    GetAppResponseTypeDef,
     UpdateAppRequestRequestTypeDef,
-    UpdateAppResponseTypeDef,
     ServerGroupLaunchConfigurationTypeDef,
     ServerGroupReplicationConfigurationTypeDef,
     ServerGroupValidationConfigurationTypeDef,
+    CreateAppResponseTypeDef,
+    GetAppResponseTypeDef,
+    UpdateAppResponseTypeDef,
+    ServerGroupLaunchConfigurationOutputTypeDef,
+    ServerGroupReplicationConfigurationOutputTypeDef,
+    ServerGroupValidationConfigurationOutputTypeDef,
     ValidationOutputTypeDef,
-    GetAppLaunchConfigurationResponseTypeDef,
     PutAppLaunchConfigurationRequestRequestTypeDef,
-    GetAppReplicationConfigurationResponseTypeDef,
     PutAppReplicationConfigurationRequestRequestTypeDef,
-    GetAppValidationConfigurationResponseTypeDef,
     PutAppValidationConfigurationRequestRequestTypeDef,
+    GetAppLaunchConfigurationResponseTypeDef,
+    GetAppReplicationConfigurationResponseTypeDef,
+    GetAppValidationConfigurationResponseTypeDef,
     GetAppValidationOutputResponseTypeDef,
 )
 
 
 def get_structure() -> LaunchDetailsTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sms-1.28.0/README.md` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-sms
+Version: 1.28.12
+Summary: Type annotations for boto3.SMS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 sms type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-sms"></a>
 
 # mypy-boto3-sms
 
 [![PyPI - mypy-boto3-sms](https://img.shields.io/pypi/v/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sms?color=blue)](https://pypistats.org/packages/mypy-boto3-sms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sms)](https://pepy.tech/project/mypy-boto3-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SMS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[boto3.SMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [mypy-boto3-sms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,95 +357,113 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     CreateReplicationJobRequestRequestTypeDef,
-    CreateReplicationJobResponseTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
-    S3LocationTypeDef,
+    S3LocationOutputTypeDef,
     GenerateTemplateRequestRequestTypeDef,
     GetAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
     GetAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputRequestRequestTypeDef,
-    GetConnectorsRequestGetConnectorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetConnectorsRequestRequestTypeDef,
-    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
     GetReplicationJobsRequestRequestTypeDef,
-    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     GetReplicationRunsRequestRequestTypeDef,
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
-    ListAppsRequestListAppsPaginateTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
-    PaginatorConfigTypeDef,
     ReplicationRunStageDetailsTypeDef,
-    ResponseMetadataTypeDef,
+    S3LocationTypeDef,
+    ServerReplicationParametersOutputTypeDef,
     ServerReplicationParametersTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
-    StartOnDemandReplicationRunResponseTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
     UpdateReplicationJobRequestRequestTypeDef,
+    VmServerAddressOutputTypeDef,
     AppSummaryTypeDef,
+    CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
+    StartOnDemandReplicationRunResponseTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
-    SourceTypeDef,
-    UserDataTypeDef,
+    SourceOutputTypeDef,
+    UserDataOutputTypeDef,
+    GetConnectorsRequestGetConnectorsPaginateTypeDef,
+    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
+    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+    ListAppsRequestListAppsPaginateTypeDef,
     GetServersRequestGetServersPaginateTypeDef,
     GetServersRequestRequestTypeDef,
     VmServerTypeDef,
     NotifyAppValidationOutputRequestRequestTypeDef,
     ReplicationRunTypeDef,
+    SourceTypeDef,
+    UserDataTypeDef,
+    VmServerOutputTypeDef,
     ListAppsResponseTypeDef,
     AppValidationOutputTypeDef,
+    SSMValidationParametersOutputTypeDef,
+    UserDataValidationParametersOutputTypeDef,
+    ServerTypeDef,
     SSMValidationParametersTypeDef,
     UserDataValidationParametersTypeDef,
-    ServerTypeDef,
     ReplicationJobTypeDef,
-    AppValidationConfigurationTypeDef,
-    GetServersResponseTypeDef,
+    ServerOutputTypeDef,
+    AppValidationConfigurationOutputTypeDef,
     ServerGroupTypeDef,
     ServerLaunchConfigurationTypeDef,
     ServerReplicationConfigurationTypeDef,
+    AppValidationConfigurationTypeDef,
     ServerValidationConfigurationTypeDef,
-    ServerValidationOutputTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
+    GetServersResponseTypeDef,
+    ServerGroupOutputTypeDef,
+    ServerLaunchConfigurationOutputTypeDef,
+    ServerReplicationConfigurationOutputTypeDef,
+    ServerValidationConfigurationOutputTypeDef,
+    ServerValidationOutputTypeDef,
     CreateAppRequestRequestTypeDef,
-    CreateAppResponseTypeDef,
-    GetAppResponseTypeDef,
     UpdateAppRequestRequestTypeDef,
-    UpdateAppResponseTypeDef,
     ServerGroupLaunchConfigurationTypeDef,
     ServerGroupReplicationConfigurationTypeDef,
     ServerGroupValidationConfigurationTypeDef,
+    CreateAppResponseTypeDef,
+    GetAppResponseTypeDef,
+    UpdateAppResponseTypeDef,
+    ServerGroupLaunchConfigurationOutputTypeDef,
+    ServerGroupReplicationConfigurationOutputTypeDef,
+    ServerGroupValidationConfigurationOutputTypeDef,
     ValidationOutputTypeDef,
-    GetAppLaunchConfigurationResponseTypeDef,
     PutAppLaunchConfigurationRequestRequestTypeDef,
-    GetAppReplicationConfigurationResponseTypeDef,
     PutAppReplicationConfigurationRequestRequestTypeDef,
-    GetAppValidationConfigurationResponseTypeDef,
     PutAppValidationConfigurationRequestRequestTypeDef,
+    GetAppLaunchConfigurationResponseTypeDef,
+    GetAppReplicationConfigurationResponseTypeDef,
+    GetAppValidationConfigurationResponseTypeDef,
     GetAppValidationOutputResponseTypeDef,
 )
 
 
 def get_structure() -> LaunchDetailsTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms/__init__.py` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms/__init__.pyi` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms/__main__.py` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SMS 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SMS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS\nOther"
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

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms/client.py` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms/client.pyi` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms/literals.py` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AppLaunchConfigurationStatusType",
     "AppLaunchStatusType",
     "AppReplicationConfigurationStatusType",
     "AppReplicationStatusType",
     "AppStatusType",
     "AppValidationStrategyType",
@@ -47,15 +46,14 @@
     "SMSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AppLaunchConfigurationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
 AppLaunchStatusType = Literal[
     "CONFIGURATION_INVALID",
     "CONFIGURATION_IN_PROGRESS",
     "DELTA_LAUNCH_FAILED",
     "DELTA_LAUNCH_IN_PROGRESS",
     "LAUNCHED",
@@ -240,14 +238,15 @@
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
@@ -326,26 +325,28 @@
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

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms/literals.pyi` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AppLaunchConfigurationStatusType",
     "AppLaunchStatusType",
     "AppReplicationConfigurationStatusType",
     "AppReplicationStatusType",
     "AppStatusType",
     "AppValidationStrategyType",
@@ -46,14 +47,15 @@
     "SMSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AppLaunchConfigurationStatusType = Literal["CONFIGURED", "NOT_CONFIGURED"]
 AppLaunchStatusType = Literal[
     "CONFIGURATION_INVALID",
     "CONFIGURATION_IN_PROGRESS",
     "DELTA_LAUNCH_FAILED",
     "DELTA_LAUNCH_IN_PROGRESS",
     "LAUNCHED",
@@ -238,14 +240,15 @@
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
@@ -324,26 +327,28 @@
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

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms/paginator.py` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,45 +63,45 @@
 class GetConnectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getconnectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getconnectorspaginator)
         """
 
 
 class GetReplicationJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationjobspaginator)
     """
 
     def paginate(
-        self, *, replicationJobId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, replicationJobId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetReplicationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationjobspaginator)
         """
 
 
 class GetReplicationRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationrunspaginator)
     """
 
     def paginate(
-        self, *, replicationJobId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, replicationJobId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetReplicationRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationrunspaginator)
         """
 
 
@@ -111,28 +111,28 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getserverspaginator)
     """
 
     def paginate(
         self,
         *,
         vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getserverspaginator)
         """
 
 
 class ListAppsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#listappspaginator)
     """
 
     def paginate(
-        self, *, appIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAppsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#listappspaginator)
         """
```

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms/paginator.pyi` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,43 +60,43 @@
 class GetConnectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getconnectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetConnectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getconnectorspaginator)
         """
 
 class GetReplicationJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationjobspaginator)
     """
 
     def paginate(
-        self, *, replicationJobId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, replicationJobId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetReplicationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationjobspaginator)
         """
 
 class GetReplicationRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationrunspaginator)
     """
 
     def paginate(
-        self, *, replicationJobId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, replicationJobId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetReplicationRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getreplicationrunspaginator)
         """
 
 class GetServersPaginator(Paginator):
@@ -105,27 +105,27 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getserverspaginator)
     """
 
     def paginate(
         self,
         *,
         vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#getserverspaginator)
         """
 
 class ListAppsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#listappspaginator)
     """
 
     def paginate(
-        self, *, appIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAppsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/paginators/#listappspaginator)
         """
```

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms/type_defs.py` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,95 +44,113 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "LaunchDetailsTypeDef",
     "ConnectorTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "CreateReplicationJobRequestRequestTypeDef",
-    "CreateReplicationJobResponseTypeDef",
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     "DeleteAppReplicationConfigurationRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppValidationConfigurationRequestRequestTypeDef",
     "DeleteReplicationJobRequestRequestTypeDef",
     "DisassociateConnectorRequestRequestTypeDef",
     "GenerateChangeSetRequestRequestTypeDef",
-    "S3LocationTypeDef",
+    "S3LocationOutputTypeDef",
     "GenerateTemplateRequestRequestTypeDef",
     "GetAppLaunchConfigurationRequestRequestTypeDef",
     "GetAppReplicationConfigurationRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
     "GetAppValidationConfigurationRequestRequestTypeDef",
     "GetAppValidationOutputRequestRequestTypeDef",
-    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetConnectorsRequestRequestTypeDef",
-    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
     "GetReplicationJobsRequestRequestTypeDef",
-    "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
     "GetReplicationRunsRequestRequestTypeDef",
     "VmServerAddressTypeDef",
     "ImportAppCatalogRequestRequestTypeDef",
     "LaunchAppRequestRequestTypeDef",
-    "ListAppsRequestListAppsPaginateTypeDef",
     "ListAppsRequestRequestTypeDef",
     "NotificationContextTypeDef",
-    "PaginatorConfigTypeDef",
     "ReplicationRunStageDetailsTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3LocationTypeDef",
+    "ServerReplicationParametersOutputTypeDef",
     "ServerReplicationParametersTypeDef",
     "StartAppReplicationRequestRequestTypeDef",
     "StartOnDemandAppReplicationRequestRequestTypeDef",
     "StartOnDemandReplicationRunRequestRequestTypeDef",
-    "StartOnDemandReplicationRunResponseTypeDef",
     "StopAppReplicationRequestRequestTypeDef",
     "TerminateAppRequestRequestTypeDef",
     "UpdateReplicationJobRequestRequestTypeDef",
+    "VmServerAddressOutputTypeDef",
     "AppSummaryTypeDef",
+    "CreateReplicationJobResponseTypeDef",
     "GetConnectorsResponseTypeDef",
+    "StartOnDemandReplicationRunResponseTypeDef",
     "GenerateChangeSetResponseTypeDef",
     "GenerateTemplateResponseTypeDef",
     "SSMOutputTypeDef",
-    "SourceTypeDef",
-    "UserDataTypeDef",
+    "SourceOutputTypeDef",
+    "UserDataOutputTypeDef",
+    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
+    "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    "ListAppsRequestListAppsPaginateTypeDef",
     "GetServersRequestGetServersPaginateTypeDef",
     "GetServersRequestRequestTypeDef",
     "VmServerTypeDef",
     "NotifyAppValidationOutputRequestRequestTypeDef",
     "ReplicationRunTypeDef",
+    "SourceTypeDef",
+    "UserDataTypeDef",
+    "VmServerOutputTypeDef",
     "ListAppsResponseTypeDef",
     "AppValidationOutputTypeDef",
+    "SSMValidationParametersOutputTypeDef",
+    "UserDataValidationParametersOutputTypeDef",
+    "ServerTypeDef",
     "SSMValidationParametersTypeDef",
     "UserDataValidationParametersTypeDef",
-    "ServerTypeDef",
     "ReplicationJobTypeDef",
-    "AppValidationConfigurationTypeDef",
-    "GetServersResponseTypeDef",
+    "ServerOutputTypeDef",
+    "AppValidationConfigurationOutputTypeDef",
     "ServerGroupTypeDef",
     "ServerLaunchConfigurationTypeDef",
     "ServerReplicationConfigurationTypeDef",
+    "AppValidationConfigurationTypeDef",
     "ServerValidationConfigurationTypeDef",
-    "ServerValidationOutputTypeDef",
     "GetReplicationJobsResponseTypeDef",
     "GetReplicationRunsResponseTypeDef",
+    "GetServersResponseTypeDef",
+    "ServerGroupOutputTypeDef",
+    "ServerLaunchConfigurationOutputTypeDef",
+    "ServerReplicationConfigurationOutputTypeDef",
+    "ServerValidationConfigurationOutputTypeDef",
+    "ServerValidationOutputTypeDef",
     "CreateAppRequestRequestTypeDef",
-    "CreateAppResponseTypeDef",
-    "GetAppResponseTypeDef",
     "UpdateAppRequestRequestTypeDef",
-    "UpdateAppResponseTypeDef",
     "ServerGroupLaunchConfigurationTypeDef",
     "ServerGroupReplicationConfigurationTypeDef",
     "ServerGroupValidationConfigurationTypeDef",
+    "CreateAppResponseTypeDef",
+    "GetAppResponseTypeDef",
+    "UpdateAppResponseTypeDef",
+    "ServerGroupLaunchConfigurationOutputTypeDef",
+    "ServerGroupReplicationConfigurationOutputTypeDef",
+    "ServerGroupValidationConfigurationOutputTypeDef",
     "ValidationOutputTypeDef",
-    "GetAppLaunchConfigurationResponseTypeDef",
     "PutAppLaunchConfigurationRequestRequestTypeDef",
-    "GetAppReplicationConfigurationResponseTypeDef",
     "PutAppReplicationConfigurationRequestRequestTypeDef",
-    "GetAppValidationConfigurationResponseTypeDef",
     "PutAppValidationConfigurationRequestRequestTypeDef",
+    "GetAppLaunchConfigurationResponseTypeDef",
+    "GetAppReplicationConfigurationResponseTypeDef",
+    "GetAppValidationConfigurationResponseTypeDef",
     "GetAppValidationOutputResponseTypeDef",
 )
 
 LaunchDetailsTypeDef = TypedDict(
     "LaunchDetailsTypeDef",
     {
         "latestLaunchTime": datetime,
@@ -164,14 +182,34 @@
     {
         "key": str,
         "value": str,
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
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 _RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationJobRequestRequestTypeDef",
     {
         "serverId": str,
         "seedReplicationTime": Union[datetime, str],
     },
 )
@@ -194,22 +232,14 @@
 class CreateReplicationJobRequestRequestTypeDef(
     _RequiredCreateReplicationJobRequestRequestTypeDef,
     _OptionalCreateReplicationJobRequestRequestTypeDef,
 ):
     pass
 
 
-CreateReplicationJobResponseTypeDef = TypedDict(
-    "CreateReplicationJobResponseTypeDef",
-    {
-        "replicationJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -258,16 +288,16 @@
     {
         "appId": str,
         "changesetFormat": OutputFormatType,
     },
     total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
     {
         "bucket": str,
         "key": str,
     },
     total=False,
 )
 
@@ -314,72 +344,43 @@
 GetAppValidationOutputRequestRequestTypeDef = TypedDict(
     "GetAppValidationOutputRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 
-GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
-    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetConnectorsRequestRequestTypeDef = TypedDict(
     "GetConnectorsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = TypedDict(
-    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
-    {
-        "replicationJobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetReplicationJobsRequestRequestTypeDef = TypedDict(
     "GetReplicationJobsRequestRequestTypeDef",
     {
         "replicationJobId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
-    "_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    {
-        "replicationJobId": str,
-    },
-)
-_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
-    "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
-    _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-    _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetReplicationRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetReplicationRunsRequestRequestTypeDef",
     {
         "replicationJobId": str,
     },
 )
 _OptionalGetReplicationRunsRequestRequestTypeDef = TypedDict(
@@ -420,23 +421,14 @@
     "LaunchAppRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
 
-ListAppsRequestListAppsPaginateTypeDef = TypedDict(
-    "ListAppsRequestListAppsPaginateTypeDef",
-    {
-        "appIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAppsRequestRequestTypeDef = TypedDict(
     "ListAppsRequestRequestTypeDef",
     {
         "appIds": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
@@ -449,48 +441,50 @@
         "validationId": str,
         "status": ValidationStatusType,
         "statusMessage": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ReplicationRunStageDetailsTypeDef = TypedDict(
+    "ReplicationRunStageDetailsTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "stage": str,
+        "stageProgress": str,
     },
     total=False,
 )
 
-ReplicationRunStageDetailsTypeDef = TypedDict(
-    "ReplicationRunStageDetailsTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
-        "stage": str,
-        "stageProgress": str,
+        "bucket": str,
+        "key": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ServerReplicationParametersOutputTypeDef = TypedDict(
+    "ServerReplicationParametersOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "seedTime": datetime,
+        "frequency": int,
+        "runOnce": bool,
+        "licenseType": LicenseTypeType,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
     },
+    total=False,
 )
 
 ServerReplicationParametersTypeDef = TypedDict(
     "ServerReplicationParametersTypeDef",
     {
-        "seedTime": datetime,
+        "seedTime": Union[datetime, str],
         "frequency": int,
         "runOnce": bool,
         "licenseType": LicenseTypeType,
         "numberOfRecentAmisToKeep": int,
         "encrypted": bool,
         "kmsKeyId": str,
     },
@@ -545,22 +539,14 @@
 class StartOnDemandReplicationRunRequestRequestTypeDef(
     _RequiredStartOnDemandReplicationRunRequestRequestTypeDef,
     _OptionalStartOnDemandReplicationRunRequestRequestTypeDef,
 ):
     pass
 
 
-StartOnDemandReplicationRunResponseTypeDef = TypedDict(
-    "StartOnDemandReplicationRunResponseTypeDef",
-    {
-        "replicationRunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopAppReplicationRequestRequestTypeDef = TypedDict(
     "StopAppReplicationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -598,14 +584,23 @@
 class UpdateReplicationJobRequestRequestTypeDef(
     _RequiredUpdateReplicationJobRequestRequestTypeDef,
     _OptionalUpdateReplicationJobRequestRequestTypeDef,
 ):
     pass
 
 
+VmServerAddressOutputTypeDef = TypedDict(
+    "VmServerAddressOutputTypeDef",
+    {
+        "vmManagerId": str,
+        "vmId": str,
+    },
+    total=False,
+)
+
 AppSummaryTypeDef = TypedDict(
     "AppSummaryTypeDef",
     {
         "appId": str,
         "importedAppId": str,
         "name": str,
         "description": str,
@@ -624,68 +619,132 @@
         "roleName": str,
         "totalServerGroups": int,
         "totalServers": int,
     },
     total=False,
 )
 
+CreateReplicationJobResponseTypeDef = TypedDict(
+    "CreateReplicationJobResponseTypeDef",
+    {
+        "replicationJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetConnectorsResponseTypeDef = TypedDict(
     "GetConnectorsResponseTypeDef",
     {
         "connectorList": List[ConnectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartOnDemandReplicationRunResponseTypeDef = TypedDict(
+    "StartOnDemandReplicationRunResponseTypeDef",
+    {
+        "replicationRunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GenerateChangeSetResponseTypeDef = TypedDict(
     "GenerateChangeSetResponseTypeDef",
     {
-        "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "s3Location": S3LocationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GenerateTemplateResponseTypeDef = TypedDict(
     "GenerateTemplateResponseTypeDef",
     {
-        "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "s3Location": S3LocationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SSMOutputTypeDef = TypedDict(
     "SSMOutputTypeDef",
     {
-        "s3Location": S3LocationTypeDef,
+        "s3Location": S3LocationOutputTypeDef,
     },
     total=False,
 )
 
-SourceTypeDef = TypedDict(
-    "SourceTypeDef",
+SourceOutputTypeDef = TypedDict(
+    "SourceOutputTypeDef",
     {
-        "s3Location": S3LocationTypeDef,
+        "s3Location": S3LocationOutputTypeDef,
     },
     total=False,
 )
 
-UserDataTypeDef = TypedDict(
-    "UserDataTypeDef",
+UserDataOutputTypeDef = TypedDict(
+    "UserDataOutputTypeDef",
     {
-        "s3Location": S3LocationTypeDef,
+        "s3Location": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
+GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
+    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = TypedDict(
+    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
+    {
+        "replicationJobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
+    "_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    {
+        "replicationJobId": str,
+    },
+)
+_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
+    "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
+    _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+    _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+):
+    pass
+
+
+ListAppsRequestListAppsPaginateTypeDef = TypedDict(
+    "ListAppsRequestListAppsPaginateTypeDef",
+    {
+        "appIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetServersRequestGetServersPaginateTypeDef = TypedDict(
     "GetServersRequestGetServersPaginateTypeDef",
     {
         "vmServerAddressList": Sequence[VmServerAddressTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetServersRequestRequestTypeDef = TypedDict(
     "GetServersRequestRequestTypeDef",
     {
@@ -744,48 +803,76 @@
         "description": str,
         "encrypted": bool,
         "kmsKeyId": str,
     },
     total=False,
 )
 
+SourceTypeDef = TypedDict(
+    "SourceTypeDef",
+    {
+        "s3Location": S3LocationTypeDef,
+    },
+    total=False,
+)
+
+UserDataTypeDef = TypedDict(
+    "UserDataTypeDef",
+    {
+        "s3Location": S3LocationTypeDef,
+    },
+    total=False,
+)
+
+VmServerOutputTypeDef = TypedDict(
+    "VmServerOutputTypeDef",
+    {
+        "vmServerAddress": VmServerAddressOutputTypeDef,
+        "vmName": str,
+        "vmManagerName": str,
+        "vmManagerType": VmManagerTypeType,
+        "vmPath": str,
+    },
+    total=False,
+)
+
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "apps": List[AppSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AppValidationOutputTypeDef = TypedDict(
     "AppValidationOutputTypeDef",
     {
         "ssmOutput": SSMOutputTypeDef,
     },
     total=False,
 )
 
-SSMValidationParametersTypeDef = TypedDict(
-    "SSMValidationParametersTypeDef",
+SSMValidationParametersOutputTypeDef = TypedDict(
+    "SSMValidationParametersOutputTypeDef",
     {
-        "source": SourceTypeDef,
+        "source": SourceOutputTypeDef,
         "instanceId": str,
         "scriptType": ScriptTypeType,
         "command": str,
         "executionTimeoutSeconds": int,
         "outputS3BucketName": str,
     },
     total=False,
 )
 
-UserDataValidationParametersTypeDef = TypedDict(
-    "UserDataValidationParametersTypeDef",
+UserDataValidationParametersOutputTypeDef = TypedDict(
+    "UserDataValidationParametersOutputTypeDef",
     {
-        "source": SourceTypeDef,
+        "source": SourceOutputTypeDef,
         "scriptType": ScriptTypeType,
     },
     total=False,
 )
 
 ServerTypeDef = TypedDict(
     "ServerTypeDef",
@@ -795,21 +882,43 @@
         "vmServer": VmServerTypeDef,
         "replicationJobId": str,
         "replicationJobTerminated": bool,
     },
     total=False,
 )
 
+SSMValidationParametersTypeDef = TypedDict(
+    "SSMValidationParametersTypeDef",
+    {
+        "source": SourceTypeDef,
+        "instanceId": str,
+        "scriptType": ScriptTypeType,
+        "command": str,
+        "executionTimeoutSeconds": int,
+        "outputS3BucketName": str,
+    },
+    total=False,
+)
+
+UserDataValidationParametersTypeDef = TypedDict(
+    "UserDataValidationParametersTypeDef",
+    {
+        "source": SourceTypeDef,
+        "scriptType": ScriptTypeType,
+    },
+    total=False,
+)
+
 ReplicationJobTypeDef = TypedDict(
     "ReplicationJobTypeDef",
     {
         "replicationJobId": str,
         "serverId": str,
         "serverType": Literal["VIRTUAL_MACHINE"],
-        "vmServer": VmServerTypeDef,
+        "vmServer": VmServerOutputTypeDef,
         "seedReplicationTime": datetime,
         "frequency": int,
         "runOnce": bool,
         "nextReplicationRunStartTime": datetime,
         "licenseType": LicenseTypeType,
         "roleName": str,
         "latestAmiId": str,
@@ -820,34 +929,35 @@
         "encrypted": bool,
         "kmsKeyId": str,
         "replicationRunList": List[ReplicationRunTypeDef],
     },
     total=False,
 )
 
-AppValidationConfigurationTypeDef = TypedDict(
-    "AppValidationConfigurationTypeDef",
+ServerOutputTypeDef = TypedDict(
+    "ServerOutputTypeDef",
     {
-        "validationId": str,
-        "name": str,
-        "appValidationStrategy": Literal["SSM"],
-        "ssmValidationParameters": SSMValidationParametersTypeDef,
+        "serverId": str,
+        "serverType": Literal["VIRTUAL_MACHINE"],
+        "vmServer": VmServerOutputTypeDef,
+        "replicationJobId": str,
+        "replicationJobTerminated": bool,
     },
     total=False,
 )
 
-GetServersResponseTypeDef = TypedDict(
-    "GetServersResponseTypeDef",
+AppValidationConfigurationOutputTypeDef = TypedDict(
+    "AppValidationConfigurationOutputTypeDef",
     {
-        "lastModifiedOn": datetime,
-        "serverCatalogStatus": ServerCatalogStatusType,
-        "serverList": List[ServerTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "validationId": str,
+        "name": str,
+        "appValidationStrategy": Literal["SSM"],
+        "ssmValidationParameters": SSMValidationParametersOutputTypeDef,
     },
+    total=False,
 )
 
 ServerGroupTypeDef = TypedDict(
     "ServerGroupTypeDef",
     {
         "serverGroupId": str,
         "name": str,
@@ -880,133 +990,233 @@
     {
         "server": ServerTypeDef,
         "serverReplicationParameters": ServerReplicationParametersTypeDef,
     },
     total=False,
 )
 
-ServerValidationConfigurationTypeDef = TypedDict(
-    "ServerValidationConfigurationTypeDef",
+AppValidationConfigurationTypeDef = TypedDict(
+    "AppValidationConfigurationTypeDef",
     {
-        "server": ServerTypeDef,
         "validationId": str,
         "name": str,
-        "serverValidationStrategy": Literal["USERDATA"],
-        "userDataValidationParameters": UserDataValidationParametersTypeDef,
+        "appValidationStrategy": Literal["SSM"],
+        "ssmValidationParameters": SSMValidationParametersTypeDef,
     },
     total=False,
 )
 
-ServerValidationOutputTypeDef = TypedDict(
-    "ServerValidationOutputTypeDef",
+ServerValidationConfigurationTypeDef = TypedDict(
+    "ServerValidationConfigurationTypeDef",
     {
         "server": ServerTypeDef,
+        "validationId": str,
+        "name": str,
+        "serverValidationStrategy": Literal["USERDATA"],
+        "userDataValidationParameters": UserDataValidationParametersTypeDef,
     },
     total=False,
 )
 
 GetReplicationJobsResponseTypeDef = TypedDict(
     "GetReplicationJobsResponseTypeDef",
     {
         "replicationJobList": List[ReplicationJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReplicationRunsResponseTypeDef = TypedDict(
     "GetReplicationRunsResponseTypeDef",
     {
         "replicationJob": ReplicationJobTypeDef,
         "replicationRunList": List[ReplicationRunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
+GetServersResponseTypeDef = TypedDict(
+    "GetServersResponseTypeDef",
+    {
+        "lastModifiedOn": datetime,
+        "serverCatalogStatus": ServerCatalogStatusType,
+        "serverList": List[ServerOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerGroupOutputTypeDef = TypedDict(
+    "ServerGroupOutputTypeDef",
     {
+        "serverGroupId": str,
         "name": str,
-        "description": str,
-        "roleName": str,
-        "clientToken": str,
-        "serverGroups": Sequence[ServerGroupTypeDef],
-        "tags": Sequence[TagTypeDef],
+        "serverList": List[ServerOutputTypeDef],
     },
     total=False,
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+ServerLaunchConfigurationOutputTypeDef = TypedDict(
+    "ServerLaunchConfigurationOutputTypeDef",
     {
-        "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupTypeDef],
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "server": ServerOutputTypeDef,
+        "logicalId": str,
+        "vpc": str,
+        "subnet": str,
+        "securityGroup": str,
+        "ec2KeyName": str,
+        "userData": UserDataOutputTypeDef,
+        "instanceType": str,
+        "associatePublicIpAddress": bool,
+        "iamInstanceProfileName": str,
+        "configureScript": S3LocationOutputTypeDef,
+        "configureScriptType": ScriptTypeType,
     },
+    total=False,
 )
 
-GetAppResponseTypeDef = TypedDict(
-    "GetAppResponseTypeDef",
+ServerReplicationConfigurationOutputTypeDef = TypedDict(
+    "ServerReplicationConfigurationOutputTypeDef",
     {
-        "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupTypeDef],
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "server": ServerOutputTypeDef,
+        "serverReplicationParameters": ServerReplicationParametersOutputTypeDef,
+    },
+    total=False,
+)
+
+ServerValidationConfigurationOutputTypeDef = TypedDict(
+    "ServerValidationConfigurationOutputTypeDef",
+    {
+        "server": ServerOutputTypeDef,
+        "validationId": str,
+        "name": str,
+        "serverValidationStrategy": Literal["USERDATA"],
+        "userDataValidationParameters": UserDataValidationParametersOutputTypeDef,
     },
+    total=False,
 )
 
-UpdateAppRequestRequestTypeDef = TypedDict(
-    "UpdateAppRequestRequestTypeDef",
+ServerValidationOutputTypeDef = TypedDict(
+    "ServerValidationOutputTypeDef",
+    {
+        "server": ServerOutputTypeDef,
+    },
+    total=False,
+)
+
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
     {
-        "appId": str,
         "name": str,
         "description": str,
         "roleName": str,
+        "clientToken": str,
         "serverGroups": Sequence[ServerGroupTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-UpdateAppResponseTypeDef = TypedDict(
-    "UpdateAppResponseTypeDef",
+UpdateAppRequestRequestTypeDef = TypedDict(
+    "UpdateAppRequestRequestTypeDef",
     {
-        "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupTypeDef],
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "name": str,
+        "description": str,
+        "roleName": str,
+        "serverGroups": Sequence[ServerGroupTypeDef],
+        "tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
 ServerGroupLaunchConfigurationTypeDef = TypedDict(
     "ServerGroupLaunchConfigurationTypeDef",
     {
         "serverGroupId": str,
         "launchOrder": int,
-        "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
+        "serverLaunchConfigurations": Sequence[ServerLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
 ServerGroupReplicationConfigurationTypeDef = TypedDict(
     "ServerGroupReplicationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverReplicationConfigurations": List[ServerReplicationConfigurationTypeDef],
+        "serverReplicationConfigurations": Sequence[ServerReplicationConfigurationTypeDef],
     },
     total=False,
 )
 
 ServerGroupValidationConfigurationTypeDef = TypedDict(
     "ServerGroupValidationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverValidationConfigurations": List[ServerValidationConfigurationTypeDef],
+        "serverValidationConfigurations": Sequence[ServerValidationConfigurationTypeDef],
+    },
+    total=False,
+)
+
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
+    {
+        "appSummary": AppSummaryTypeDef,
+        "serverGroups": List[ServerGroupOutputTypeDef],
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppResponseTypeDef = TypedDict(
+    "GetAppResponseTypeDef",
+    {
+        "appSummary": AppSummaryTypeDef,
+        "serverGroups": List[ServerGroupOutputTypeDef],
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppResponseTypeDef = TypedDict(
+    "UpdateAppResponseTypeDef",
+    {
+        "appSummary": AppSummaryTypeDef,
+        "serverGroups": List[ServerGroupOutputTypeDef],
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerGroupLaunchConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupLaunchConfigurationOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "launchOrder": int,
+        "serverLaunchConfigurations": List[ServerLaunchConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+ServerGroupReplicationConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupReplicationConfigurationOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "serverReplicationConfigurations": List[ServerReplicationConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+ServerGroupValidationConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupValidationConfigurationOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "serverValidationConfigurations": List[ServerValidationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
 ValidationOutputTypeDef = TypedDict(
     "ValidationOutputTypeDef",
     {
@@ -1017,64 +1227,36 @@
         "latestValidationTime": datetime,
         "appValidationOutput": AppValidationOutputTypeDef,
         "serverValidationOutput": ServerValidationOutputTypeDef,
     },
     total=False,
 )
 
-GetAppLaunchConfigurationResponseTypeDef = TypedDict(
-    "GetAppLaunchConfigurationResponseTypeDef",
-    {
-        "appId": str,
-        "roleName": str,
-        "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
         "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
-GetAppReplicationConfigurationResponseTypeDef = TypedDict(
-    "GetAppReplicationConfigurationResponseTypeDef",
-    {
-        "serverGroupReplicationConfigurations": List[ServerGroupReplicationConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppReplicationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
         "serverGroupReplicationConfigurations": Sequence[
             ServerGroupReplicationConfigurationTypeDef
         ],
     },
     total=False,
 )
 
-GetAppValidationConfigurationResponseTypeDef = TypedDict(
-    "GetAppValidationConfigurationResponseTypeDef",
-    {
-        "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
-        "serverGroupValidationConfigurations": List[ServerGroupValidationConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 _OptionalPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
@@ -1090,14 +1272,46 @@
 class PutAppValidationConfigurationRequestRequestTypeDef(
     _RequiredPutAppValidationConfigurationRequestRequestTypeDef,
     _OptionalPutAppValidationConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+GetAppLaunchConfigurationResponseTypeDef = TypedDict(
+    "GetAppLaunchConfigurationResponseTypeDef",
+    {
+        "appId": str,
+        "roleName": str,
+        "autoLaunch": bool,
+        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppReplicationConfigurationResponseTypeDef = TypedDict(
+    "GetAppReplicationConfigurationResponseTypeDef",
+    {
+        "serverGroupReplicationConfigurations": List[
+            ServerGroupReplicationConfigurationOutputTypeDef
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppValidationConfigurationResponseTypeDef = TypedDict(
+    "GetAppValidationConfigurationResponseTypeDef",
+    {
+        "appValidationConfigurations": List[AppValidationConfigurationOutputTypeDef],
+        "serverGroupValidationConfigurations": List[
+            ServerGroupValidationConfigurationOutputTypeDef
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetAppValidationOutputResponseTypeDef = TypedDict(
     "GetAppValidationOutputResponseTypeDef",
     {
         "validationOutputList": List[ValidationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms/type_defs.pyi` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -43,95 +43,113 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "LaunchDetailsTypeDef",
     "ConnectorTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
+    "TagOutputTypeDef",
     "CreateReplicationJobRequestRequestTypeDef",
-    "CreateReplicationJobResponseTypeDef",
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     "DeleteAppReplicationConfigurationRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAppValidationConfigurationRequestRequestTypeDef",
     "DeleteReplicationJobRequestRequestTypeDef",
     "DisassociateConnectorRequestRequestTypeDef",
     "GenerateChangeSetRequestRequestTypeDef",
-    "S3LocationTypeDef",
+    "S3LocationOutputTypeDef",
     "GenerateTemplateRequestRequestTypeDef",
     "GetAppLaunchConfigurationRequestRequestTypeDef",
     "GetAppReplicationConfigurationRequestRequestTypeDef",
     "GetAppRequestRequestTypeDef",
     "GetAppValidationConfigurationRequestRequestTypeDef",
     "GetAppValidationOutputRequestRequestTypeDef",
-    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetConnectorsRequestRequestTypeDef",
-    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
     "GetReplicationJobsRequestRequestTypeDef",
-    "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
     "GetReplicationRunsRequestRequestTypeDef",
     "VmServerAddressTypeDef",
     "ImportAppCatalogRequestRequestTypeDef",
     "LaunchAppRequestRequestTypeDef",
-    "ListAppsRequestListAppsPaginateTypeDef",
     "ListAppsRequestRequestTypeDef",
     "NotificationContextTypeDef",
-    "PaginatorConfigTypeDef",
     "ReplicationRunStageDetailsTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3LocationTypeDef",
+    "ServerReplicationParametersOutputTypeDef",
     "ServerReplicationParametersTypeDef",
     "StartAppReplicationRequestRequestTypeDef",
     "StartOnDemandAppReplicationRequestRequestTypeDef",
     "StartOnDemandReplicationRunRequestRequestTypeDef",
-    "StartOnDemandReplicationRunResponseTypeDef",
     "StopAppReplicationRequestRequestTypeDef",
     "TerminateAppRequestRequestTypeDef",
     "UpdateReplicationJobRequestRequestTypeDef",
+    "VmServerAddressOutputTypeDef",
     "AppSummaryTypeDef",
+    "CreateReplicationJobResponseTypeDef",
     "GetConnectorsResponseTypeDef",
+    "StartOnDemandReplicationRunResponseTypeDef",
     "GenerateChangeSetResponseTypeDef",
     "GenerateTemplateResponseTypeDef",
     "SSMOutputTypeDef",
-    "SourceTypeDef",
-    "UserDataTypeDef",
+    "SourceOutputTypeDef",
+    "UserDataOutputTypeDef",
+    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
+    "GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    "ListAppsRequestListAppsPaginateTypeDef",
     "GetServersRequestGetServersPaginateTypeDef",
     "GetServersRequestRequestTypeDef",
     "VmServerTypeDef",
     "NotifyAppValidationOutputRequestRequestTypeDef",
     "ReplicationRunTypeDef",
+    "SourceTypeDef",
+    "UserDataTypeDef",
+    "VmServerOutputTypeDef",
     "ListAppsResponseTypeDef",
     "AppValidationOutputTypeDef",
+    "SSMValidationParametersOutputTypeDef",
+    "UserDataValidationParametersOutputTypeDef",
+    "ServerTypeDef",
     "SSMValidationParametersTypeDef",
     "UserDataValidationParametersTypeDef",
-    "ServerTypeDef",
     "ReplicationJobTypeDef",
-    "AppValidationConfigurationTypeDef",
-    "GetServersResponseTypeDef",
+    "ServerOutputTypeDef",
+    "AppValidationConfigurationOutputTypeDef",
     "ServerGroupTypeDef",
     "ServerLaunchConfigurationTypeDef",
     "ServerReplicationConfigurationTypeDef",
+    "AppValidationConfigurationTypeDef",
     "ServerValidationConfigurationTypeDef",
-    "ServerValidationOutputTypeDef",
     "GetReplicationJobsResponseTypeDef",
     "GetReplicationRunsResponseTypeDef",
+    "GetServersResponseTypeDef",
+    "ServerGroupOutputTypeDef",
+    "ServerLaunchConfigurationOutputTypeDef",
+    "ServerReplicationConfigurationOutputTypeDef",
+    "ServerValidationConfigurationOutputTypeDef",
+    "ServerValidationOutputTypeDef",
     "CreateAppRequestRequestTypeDef",
-    "CreateAppResponseTypeDef",
-    "GetAppResponseTypeDef",
     "UpdateAppRequestRequestTypeDef",
-    "UpdateAppResponseTypeDef",
     "ServerGroupLaunchConfigurationTypeDef",
     "ServerGroupReplicationConfigurationTypeDef",
     "ServerGroupValidationConfigurationTypeDef",
+    "CreateAppResponseTypeDef",
+    "GetAppResponseTypeDef",
+    "UpdateAppResponseTypeDef",
+    "ServerGroupLaunchConfigurationOutputTypeDef",
+    "ServerGroupReplicationConfigurationOutputTypeDef",
+    "ServerGroupValidationConfigurationOutputTypeDef",
     "ValidationOutputTypeDef",
-    "GetAppLaunchConfigurationResponseTypeDef",
     "PutAppLaunchConfigurationRequestRequestTypeDef",
-    "GetAppReplicationConfigurationResponseTypeDef",
     "PutAppReplicationConfigurationRequestRequestTypeDef",
-    "GetAppValidationConfigurationResponseTypeDef",
     "PutAppValidationConfigurationRequestRequestTypeDef",
+    "GetAppLaunchConfigurationResponseTypeDef",
+    "GetAppReplicationConfigurationResponseTypeDef",
+    "GetAppValidationConfigurationResponseTypeDef",
     "GetAppValidationOutputResponseTypeDef",
 )
 
 LaunchDetailsTypeDef = TypedDict(
     "LaunchDetailsTypeDef",
     {
         "latestLaunchTime": datetime,
@@ -163,14 +181,34 @@
     {
         "key": str,
         "value": str,
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
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+    total=False,
+)
+
 _RequiredCreateReplicationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationJobRequestRequestTypeDef",
     {
         "serverId": str,
         "seedReplicationTime": Union[datetime, str],
     },
 )
@@ -191,22 +229,14 @@
 
 class CreateReplicationJobRequestRequestTypeDef(
     _RequiredCreateReplicationJobRequestRequestTypeDef,
     _OptionalCreateReplicationJobRequestRequestTypeDef,
 ):
     pass
 
-CreateReplicationJobResponseTypeDef = TypedDict(
-    "CreateReplicationJobResponseTypeDef",
-    {
-        "replicationJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -255,16 +285,16 @@
     {
         "appId": str,
         "changesetFormat": OutputFormatType,
     },
     total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
     {
         "bucket": str,
         "key": str,
     },
     total=False,
 )
 
@@ -311,70 +341,43 @@
 GetAppValidationOutputRequestRequestTypeDef = TypedDict(
     "GetAppValidationOutputRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 
-GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
-    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetConnectorsRequestRequestTypeDef = TypedDict(
     "GetConnectorsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = TypedDict(
-    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
-    {
-        "replicationJobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetReplicationJobsRequestRequestTypeDef = TypedDict(
     "GetReplicationJobsRequestRequestTypeDef",
     {
         "replicationJobId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
-    "_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    {
-        "replicationJobId": str,
-    },
-)
-_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
-    "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
-    _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-    _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetReplicationRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetReplicationRunsRequestRequestTypeDef",
     {
         "replicationJobId": str,
     },
 )
 _OptionalGetReplicationRunsRequestRequestTypeDef = TypedDict(
@@ -413,23 +416,14 @@
     "LaunchAppRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
 
-ListAppsRequestListAppsPaginateTypeDef = TypedDict(
-    "ListAppsRequestListAppsPaginateTypeDef",
-    {
-        "appIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAppsRequestRequestTypeDef = TypedDict(
     "ListAppsRequestRequestTypeDef",
     {
         "appIds": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
@@ -442,48 +436,50 @@
         "validationId": str,
         "status": ValidationStatusType,
         "statusMessage": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ReplicationRunStageDetailsTypeDef = TypedDict(
+    "ReplicationRunStageDetailsTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "stage": str,
+        "stageProgress": str,
     },
     total=False,
 )
 
-ReplicationRunStageDetailsTypeDef = TypedDict(
-    "ReplicationRunStageDetailsTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
-        "stage": str,
-        "stageProgress": str,
+        "bucket": str,
+        "key": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ServerReplicationParametersOutputTypeDef = TypedDict(
+    "ServerReplicationParametersOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "seedTime": datetime,
+        "frequency": int,
+        "runOnce": bool,
+        "licenseType": LicenseTypeType,
+        "numberOfRecentAmisToKeep": int,
+        "encrypted": bool,
+        "kmsKeyId": str,
     },
+    total=False,
 )
 
 ServerReplicationParametersTypeDef = TypedDict(
     "ServerReplicationParametersTypeDef",
     {
-        "seedTime": datetime,
+        "seedTime": Union[datetime, str],
         "frequency": int,
         "runOnce": bool,
         "licenseType": LicenseTypeType,
         "numberOfRecentAmisToKeep": int,
         "encrypted": bool,
         "kmsKeyId": str,
     },
@@ -534,22 +530,14 @@
 
 class StartOnDemandReplicationRunRequestRequestTypeDef(
     _RequiredStartOnDemandReplicationRunRequestRequestTypeDef,
     _OptionalStartOnDemandReplicationRunRequestRequestTypeDef,
 ):
     pass
 
-StartOnDemandReplicationRunResponseTypeDef = TypedDict(
-    "StartOnDemandReplicationRunResponseTypeDef",
-    {
-        "replicationRunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopAppReplicationRequestRequestTypeDef = TypedDict(
     "StopAppReplicationRequestRequestTypeDef",
     {
         "appId": str,
     },
     total=False,
 )
@@ -585,14 +573,23 @@
 
 class UpdateReplicationJobRequestRequestTypeDef(
     _RequiredUpdateReplicationJobRequestRequestTypeDef,
     _OptionalUpdateReplicationJobRequestRequestTypeDef,
 ):
     pass
 
+VmServerAddressOutputTypeDef = TypedDict(
+    "VmServerAddressOutputTypeDef",
+    {
+        "vmManagerId": str,
+        "vmId": str,
+    },
+    total=False,
+)
+
 AppSummaryTypeDef = TypedDict(
     "AppSummaryTypeDef",
     {
         "appId": str,
         "importedAppId": str,
         "name": str,
         "description": str,
@@ -611,68 +608,130 @@
         "roleName": str,
         "totalServerGroups": int,
         "totalServers": int,
     },
     total=False,
 )
 
+CreateReplicationJobResponseTypeDef = TypedDict(
+    "CreateReplicationJobResponseTypeDef",
+    {
+        "replicationJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetConnectorsResponseTypeDef = TypedDict(
     "GetConnectorsResponseTypeDef",
     {
         "connectorList": List[ConnectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartOnDemandReplicationRunResponseTypeDef = TypedDict(
+    "StartOnDemandReplicationRunResponseTypeDef",
+    {
+        "replicationRunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GenerateChangeSetResponseTypeDef = TypedDict(
     "GenerateChangeSetResponseTypeDef",
     {
-        "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "s3Location": S3LocationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GenerateTemplateResponseTypeDef = TypedDict(
     "GenerateTemplateResponseTypeDef",
     {
-        "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "s3Location": S3LocationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SSMOutputTypeDef = TypedDict(
     "SSMOutputTypeDef",
     {
-        "s3Location": S3LocationTypeDef,
+        "s3Location": S3LocationOutputTypeDef,
     },
     total=False,
 )
 
-SourceTypeDef = TypedDict(
-    "SourceTypeDef",
+SourceOutputTypeDef = TypedDict(
+    "SourceOutputTypeDef",
     {
-        "s3Location": S3LocationTypeDef,
+        "s3Location": S3LocationOutputTypeDef,
     },
     total=False,
 )
 
-UserDataTypeDef = TypedDict(
-    "UserDataTypeDef",
+UserDataOutputTypeDef = TypedDict(
+    "UserDataOutputTypeDef",
     {
-        "s3Location": S3LocationTypeDef,
+        "s3Location": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
+GetConnectorsRequestGetConnectorsPaginateTypeDef = TypedDict(
+    "GetConnectorsRequestGetConnectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = TypedDict(
+    "GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef",
+    {
+        "replicationJobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
+    "_RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    {
+        "replicationJobId": str,
+    },
+)
+_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = TypedDict(
+    "_OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(
+    _RequiredGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+    _OptionalGetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+):
+    pass
+
+ListAppsRequestListAppsPaginateTypeDef = TypedDict(
+    "ListAppsRequestListAppsPaginateTypeDef",
+    {
+        "appIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetServersRequestGetServersPaginateTypeDef = TypedDict(
     "GetServersRequestGetServersPaginateTypeDef",
     {
         "vmServerAddressList": Sequence[VmServerAddressTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetServersRequestRequestTypeDef = TypedDict(
     "GetServersRequestRequestTypeDef",
     {
@@ -729,48 +788,76 @@
         "description": str,
         "encrypted": bool,
         "kmsKeyId": str,
     },
     total=False,
 )
 
+SourceTypeDef = TypedDict(
+    "SourceTypeDef",
+    {
+        "s3Location": S3LocationTypeDef,
+    },
+    total=False,
+)
+
+UserDataTypeDef = TypedDict(
+    "UserDataTypeDef",
+    {
+        "s3Location": S3LocationTypeDef,
+    },
+    total=False,
+)
+
+VmServerOutputTypeDef = TypedDict(
+    "VmServerOutputTypeDef",
+    {
+        "vmServerAddress": VmServerAddressOutputTypeDef,
+        "vmName": str,
+        "vmManagerName": str,
+        "vmManagerType": VmManagerTypeType,
+        "vmPath": str,
+    },
+    total=False,
+)
+
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "apps": List[AppSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AppValidationOutputTypeDef = TypedDict(
     "AppValidationOutputTypeDef",
     {
         "ssmOutput": SSMOutputTypeDef,
     },
     total=False,
 )
 
-SSMValidationParametersTypeDef = TypedDict(
-    "SSMValidationParametersTypeDef",
+SSMValidationParametersOutputTypeDef = TypedDict(
+    "SSMValidationParametersOutputTypeDef",
     {
-        "source": SourceTypeDef,
+        "source": SourceOutputTypeDef,
         "instanceId": str,
         "scriptType": ScriptTypeType,
         "command": str,
         "executionTimeoutSeconds": int,
         "outputS3BucketName": str,
     },
     total=False,
 )
 
-UserDataValidationParametersTypeDef = TypedDict(
-    "UserDataValidationParametersTypeDef",
+UserDataValidationParametersOutputTypeDef = TypedDict(
+    "UserDataValidationParametersOutputTypeDef",
     {
-        "source": SourceTypeDef,
+        "source": SourceOutputTypeDef,
         "scriptType": ScriptTypeType,
     },
     total=False,
 )
 
 ServerTypeDef = TypedDict(
     "ServerTypeDef",
@@ -780,21 +867,43 @@
         "vmServer": VmServerTypeDef,
         "replicationJobId": str,
         "replicationJobTerminated": bool,
     },
     total=False,
 )
 
+SSMValidationParametersTypeDef = TypedDict(
+    "SSMValidationParametersTypeDef",
+    {
+        "source": SourceTypeDef,
+        "instanceId": str,
+        "scriptType": ScriptTypeType,
+        "command": str,
+        "executionTimeoutSeconds": int,
+        "outputS3BucketName": str,
+    },
+    total=False,
+)
+
+UserDataValidationParametersTypeDef = TypedDict(
+    "UserDataValidationParametersTypeDef",
+    {
+        "source": SourceTypeDef,
+        "scriptType": ScriptTypeType,
+    },
+    total=False,
+)
+
 ReplicationJobTypeDef = TypedDict(
     "ReplicationJobTypeDef",
     {
         "replicationJobId": str,
         "serverId": str,
         "serverType": Literal["VIRTUAL_MACHINE"],
-        "vmServer": VmServerTypeDef,
+        "vmServer": VmServerOutputTypeDef,
         "seedReplicationTime": datetime,
         "frequency": int,
         "runOnce": bool,
         "nextReplicationRunStartTime": datetime,
         "licenseType": LicenseTypeType,
         "roleName": str,
         "latestAmiId": str,
@@ -805,34 +914,35 @@
         "encrypted": bool,
         "kmsKeyId": str,
         "replicationRunList": List[ReplicationRunTypeDef],
     },
     total=False,
 )
 
-AppValidationConfigurationTypeDef = TypedDict(
-    "AppValidationConfigurationTypeDef",
+ServerOutputTypeDef = TypedDict(
+    "ServerOutputTypeDef",
     {
-        "validationId": str,
-        "name": str,
-        "appValidationStrategy": Literal["SSM"],
-        "ssmValidationParameters": SSMValidationParametersTypeDef,
+        "serverId": str,
+        "serverType": Literal["VIRTUAL_MACHINE"],
+        "vmServer": VmServerOutputTypeDef,
+        "replicationJobId": str,
+        "replicationJobTerminated": bool,
     },
     total=False,
 )
 
-GetServersResponseTypeDef = TypedDict(
-    "GetServersResponseTypeDef",
+AppValidationConfigurationOutputTypeDef = TypedDict(
+    "AppValidationConfigurationOutputTypeDef",
     {
-        "lastModifiedOn": datetime,
-        "serverCatalogStatus": ServerCatalogStatusType,
-        "serverList": List[ServerTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "validationId": str,
+        "name": str,
+        "appValidationStrategy": Literal["SSM"],
+        "ssmValidationParameters": SSMValidationParametersOutputTypeDef,
     },
+    total=False,
 )
 
 ServerGroupTypeDef = TypedDict(
     "ServerGroupTypeDef",
     {
         "serverGroupId": str,
         "name": str,
@@ -865,133 +975,233 @@
     {
         "server": ServerTypeDef,
         "serverReplicationParameters": ServerReplicationParametersTypeDef,
     },
     total=False,
 )
 
-ServerValidationConfigurationTypeDef = TypedDict(
-    "ServerValidationConfigurationTypeDef",
+AppValidationConfigurationTypeDef = TypedDict(
+    "AppValidationConfigurationTypeDef",
     {
-        "server": ServerTypeDef,
         "validationId": str,
         "name": str,
-        "serverValidationStrategy": Literal["USERDATA"],
-        "userDataValidationParameters": UserDataValidationParametersTypeDef,
+        "appValidationStrategy": Literal["SSM"],
+        "ssmValidationParameters": SSMValidationParametersTypeDef,
     },
     total=False,
 )
 
-ServerValidationOutputTypeDef = TypedDict(
-    "ServerValidationOutputTypeDef",
+ServerValidationConfigurationTypeDef = TypedDict(
+    "ServerValidationConfigurationTypeDef",
     {
         "server": ServerTypeDef,
+        "validationId": str,
+        "name": str,
+        "serverValidationStrategy": Literal["USERDATA"],
+        "userDataValidationParameters": UserDataValidationParametersTypeDef,
     },
     total=False,
 )
 
 GetReplicationJobsResponseTypeDef = TypedDict(
     "GetReplicationJobsResponseTypeDef",
     {
         "replicationJobList": List[ReplicationJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReplicationRunsResponseTypeDef = TypedDict(
     "GetReplicationRunsResponseTypeDef",
     {
         "replicationJob": ReplicationJobTypeDef,
         "replicationRunList": List[ReplicationRunTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAppRequestRequestTypeDef = TypedDict(
-    "CreateAppRequestRequestTypeDef",
+GetServersResponseTypeDef = TypedDict(
+    "GetServersResponseTypeDef",
+    {
+        "lastModifiedOn": datetime,
+        "serverCatalogStatus": ServerCatalogStatusType,
+        "serverList": List[ServerOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerGroupOutputTypeDef = TypedDict(
+    "ServerGroupOutputTypeDef",
     {
+        "serverGroupId": str,
         "name": str,
-        "description": str,
-        "roleName": str,
-        "clientToken": str,
-        "serverGroups": Sequence[ServerGroupTypeDef],
-        "tags": Sequence[TagTypeDef],
+        "serverList": List[ServerOutputTypeDef],
     },
     total=False,
 )
 
-CreateAppResponseTypeDef = TypedDict(
-    "CreateAppResponseTypeDef",
+ServerLaunchConfigurationOutputTypeDef = TypedDict(
+    "ServerLaunchConfigurationOutputTypeDef",
     {
-        "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupTypeDef],
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "server": ServerOutputTypeDef,
+        "logicalId": str,
+        "vpc": str,
+        "subnet": str,
+        "securityGroup": str,
+        "ec2KeyName": str,
+        "userData": UserDataOutputTypeDef,
+        "instanceType": str,
+        "associatePublicIpAddress": bool,
+        "iamInstanceProfileName": str,
+        "configureScript": S3LocationOutputTypeDef,
+        "configureScriptType": ScriptTypeType,
     },
+    total=False,
 )
 
-GetAppResponseTypeDef = TypedDict(
-    "GetAppResponseTypeDef",
+ServerReplicationConfigurationOutputTypeDef = TypedDict(
+    "ServerReplicationConfigurationOutputTypeDef",
     {
-        "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupTypeDef],
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "server": ServerOutputTypeDef,
+        "serverReplicationParameters": ServerReplicationParametersOutputTypeDef,
     },
+    total=False,
 )
 
-UpdateAppRequestRequestTypeDef = TypedDict(
-    "UpdateAppRequestRequestTypeDef",
+ServerValidationConfigurationOutputTypeDef = TypedDict(
+    "ServerValidationConfigurationOutputTypeDef",
+    {
+        "server": ServerOutputTypeDef,
+        "validationId": str,
+        "name": str,
+        "serverValidationStrategy": Literal["USERDATA"],
+        "userDataValidationParameters": UserDataValidationParametersOutputTypeDef,
+    },
+    total=False,
+)
+
+ServerValidationOutputTypeDef = TypedDict(
+    "ServerValidationOutputTypeDef",
+    {
+        "server": ServerOutputTypeDef,
+    },
+    total=False,
+)
+
+CreateAppRequestRequestTypeDef = TypedDict(
+    "CreateAppRequestRequestTypeDef",
     {
-        "appId": str,
         "name": str,
         "description": str,
         "roleName": str,
+        "clientToken": str,
         "serverGroups": Sequence[ServerGroupTypeDef],
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-UpdateAppResponseTypeDef = TypedDict(
-    "UpdateAppResponseTypeDef",
+UpdateAppRequestRequestTypeDef = TypedDict(
+    "UpdateAppRequestRequestTypeDef",
     {
-        "appSummary": AppSummaryTypeDef,
-        "serverGroups": List[ServerGroupTypeDef],
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "name": str,
+        "description": str,
+        "roleName": str,
+        "serverGroups": Sequence[ServerGroupTypeDef],
+        "tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
 ServerGroupLaunchConfigurationTypeDef = TypedDict(
     "ServerGroupLaunchConfigurationTypeDef",
     {
         "serverGroupId": str,
         "launchOrder": int,
-        "serverLaunchConfigurations": List[ServerLaunchConfigurationTypeDef],
+        "serverLaunchConfigurations": Sequence[ServerLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
 ServerGroupReplicationConfigurationTypeDef = TypedDict(
     "ServerGroupReplicationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverReplicationConfigurations": List[ServerReplicationConfigurationTypeDef],
+        "serverReplicationConfigurations": Sequence[ServerReplicationConfigurationTypeDef],
     },
     total=False,
 )
 
 ServerGroupValidationConfigurationTypeDef = TypedDict(
     "ServerGroupValidationConfigurationTypeDef",
     {
         "serverGroupId": str,
-        "serverValidationConfigurations": List[ServerValidationConfigurationTypeDef],
+        "serverValidationConfigurations": Sequence[ServerValidationConfigurationTypeDef],
+    },
+    total=False,
+)
+
+CreateAppResponseTypeDef = TypedDict(
+    "CreateAppResponseTypeDef",
+    {
+        "appSummary": AppSummaryTypeDef,
+        "serverGroups": List[ServerGroupOutputTypeDef],
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppResponseTypeDef = TypedDict(
+    "GetAppResponseTypeDef",
+    {
+        "appSummary": AppSummaryTypeDef,
+        "serverGroups": List[ServerGroupOutputTypeDef],
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAppResponseTypeDef = TypedDict(
+    "UpdateAppResponseTypeDef",
+    {
+        "appSummary": AppSummaryTypeDef,
+        "serverGroups": List[ServerGroupOutputTypeDef],
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ServerGroupLaunchConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupLaunchConfigurationOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "launchOrder": int,
+        "serverLaunchConfigurations": List[ServerLaunchConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+ServerGroupReplicationConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupReplicationConfigurationOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "serverReplicationConfigurations": List[ServerReplicationConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+ServerGroupValidationConfigurationOutputTypeDef = TypedDict(
+    "ServerGroupValidationConfigurationOutputTypeDef",
+    {
+        "serverGroupId": str,
+        "serverValidationConfigurations": List[ServerValidationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
 ValidationOutputTypeDef = TypedDict(
     "ValidationOutputTypeDef",
     {
@@ -1002,64 +1212,36 @@
         "latestValidationTime": datetime,
         "appValidationOutput": AppValidationOutputTypeDef,
         "serverValidationOutput": ServerValidationOutputTypeDef,
     },
     total=False,
 )
 
-GetAppLaunchConfigurationResponseTypeDef = TypedDict(
-    "GetAppLaunchConfigurationResponseTypeDef",
-    {
-        "appId": str,
-        "roleName": str,
-        "autoLaunch": bool,
-        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutAppLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppLaunchConfigurationRequestRequestTypeDef",
     {
         "appId": str,
         "roleName": str,
         "autoLaunch": bool,
         "serverGroupLaunchConfigurations": Sequence[ServerGroupLaunchConfigurationTypeDef],
     },
     total=False,
 )
 
-GetAppReplicationConfigurationResponseTypeDef = TypedDict(
-    "GetAppReplicationConfigurationResponseTypeDef",
-    {
-        "serverGroupReplicationConfigurations": List[ServerGroupReplicationConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutAppReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutAppReplicationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
         "serverGroupReplicationConfigurations": Sequence[
             ServerGroupReplicationConfigurationTypeDef
         ],
     },
     total=False,
 )
 
-GetAppValidationConfigurationResponseTypeDef = TypedDict(
-    "GetAppValidationConfigurationResponseTypeDef",
-    {
-        "appValidationConfigurations": List[AppValidationConfigurationTypeDef],
-        "serverGroupValidationConfigurations": List[ServerGroupValidationConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppValidationConfigurationRequestRequestTypeDef",
     {
         "appId": str,
     },
 )
 _OptionalPutAppValidationConfigurationRequestRequestTypeDef = TypedDict(
@@ -1073,14 +1255,46 @@
 
 class PutAppValidationConfigurationRequestRequestTypeDef(
     _RequiredPutAppValidationConfigurationRequestRequestTypeDef,
     _OptionalPutAppValidationConfigurationRequestRequestTypeDef,
 ):
     pass
 
+GetAppLaunchConfigurationResponseTypeDef = TypedDict(
+    "GetAppLaunchConfigurationResponseTypeDef",
+    {
+        "appId": str,
+        "roleName": str,
+        "autoLaunch": bool,
+        "serverGroupLaunchConfigurations": List[ServerGroupLaunchConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppReplicationConfigurationResponseTypeDef = TypedDict(
+    "GetAppReplicationConfigurationResponseTypeDef",
+    {
+        "serverGroupReplicationConfigurations": List[
+            ServerGroupReplicationConfigurationOutputTypeDef
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppValidationConfigurationResponseTypeDef = TypedDict(
+    "GetAppValidationConfigurationResponseTypeDef",
+    {
+        "appValidationConfigurations": List[AppValidationConfigurationOutputTypeDef],
+        "serverGroupValidationConfigurations": List[
+            ServerGroupValidationConfigurationOutputTypeDef
+        ],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetAppValidationOutputResponseTypeDef = TypedDict(
     "GetAppValidationOutputResponseTypeDef",
     {
         "validationOutputList": List[ValidationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms.egg-info/PKG-INFO` & `mypy-boto3-sms-1.28.12/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-sms
-Version: 1.28.0
-Summary: Type annotations for boto3.SMS 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sms type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-sms"></a>
 
 # mypy-boto3-sms
 
 [![PyPI - mypy-boto3-sms](https://img.shields.io/pypi/v/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sms.svg?color=blue)](https://pypi.org/project/mypy-boto3-sms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sms?color=blue)](https://pypistats.org/packages/mypy-boto3-sms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sms)](https://pepy.tech/project/mypy-boto3-sms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SMS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
+[boto3.SMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
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
 [mypy-boto3-sms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,95 +325,113 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sms.type_defs import (
     LaunchDetailsTypeDef,
     ConnectorTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
+    TagOutputTypeDef,
     CreateReplicationJobRequestRequestTypeDef,
-    CreateReplicationJobResponseTypeDef,
     DeleteAppLaunchConfigurationRequestRequestTypeDef,
     DeleteAppReplicationConfigurationRequestRequestTypeDef,
     DeleteAppRequestRequestTypeDef,
     DeleteAppValidationConfigurationRequestRequestTypeDef,
     DeleteReplicationJobRequestRequestTypeDef,
     DisassociateConnectorRequestRequestTypeDef,
     GenerateChangeSetRequestRequestTypeDef,
-    S3LocationTypeDef,
+    S3LocationOutputTypeDef,
     GenerateTemplateRequestRequestTypeDef,
     GetAppLaunchConfigurationRequestRequestTypeDef,
     GetAppReplicationConfigurationRequestRequestTypeDef,
     GetAppRequestRequestTypeDef,
     GetAppValidationConfigurationRequestRequestTypeDef,
     GetAppValidationOutputRequestRequestTypeDef,
-    GetConnectorsRequestGetConnectorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetConnectorsRequestRequestTypeDef,
-    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
     GetReplicationJobsRequestRequestTypeDef,
-    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
     GetReplicationRunsRequestRequestTypeDef,
     VmServerAddressTypeDef,
     ImportAppCatalogRequestRequestTypeDef,
     LaunchAppRequestRequestTypeDef,
-    ListAppsRequestListAppsPaginateTypeDef,
     ListAppsRequestRequestTypeDef,
     NotificationContextTypeDef,
-    PaginatorConfigTypeDef,
     ReplicationRunStageDetailsTypeDef,
-    ResponseMetadataTypeDef,
+    S3LocationTypeDef,
+    ServerReplicationParametersOutputTypeDef,
     ServerReplicationParametersTypeDef,
     StartAppReplicationRequestRequestTypeDef,
     StartOnDemandAppReplicationRequestRequestTypeDef,
     StartOnDemandReplicationRunRequestRequestTypeDef,
-    StartOnDemandReplicationRunResponseTypeDef,
     StopAppReplicationRequestRequestTypeDef,
     TerminateAppRequestRequestTypeDef,
     UpdateReplicationJobRequestRequestTypeDef,
+    VmServerAddressOutputTypeDef,
     AppSummaryTypeDef,
+    CreateReplicationJobResponseTypeDef,
     GetConnectorsResponseTypeDef,
+    StartOnDemandReplicationRunResponseTypeDef,
     GenerateChangeSetResponseTypeDef,
     GenerateTemplateResponseTypeDef,
     SSMOutputTypeDef,
-    SourceTypeDef,
-    UserDataTypeDef,
+    SourceOutputTypeDef,
+    UserDataOutputTypeDef,
+    GetConnectorsRequestGetConnectorsPaginateTypeDef,
+    GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef,
+    GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef,
+    ListAppsRequestListAppsPaginateTypeDef,
     GetServersRequestGetServersPaginateTypeDef,
     GetServersRequestRequestTypeDef,
     VmServerTypeDef,
     NotifyAppValidationOutputRequestRequestTypeDef,
     ReplicationRunTypeDef,
+    SourceTypeDef,
+    UserDataTypeDef,
+    VmServerOutputTypeDef,
     ListAppsResponseTypeDef,
     AppValidationOutputTypeDef,
+    SSMValidationParametersOutputTypeDef,
+    UserDataValidationParametersOutputTypeDef,
+    ServerTypeDef,
     SSMValidationParametersTypeDef,
     UserDataValidationParametersTypeDef,
-    ServerTypeDef,
     ReplicationJobTypeDef,
-    AppValidationConfigurationTypeDef,
-    GetServersResponseTypeDef,
+    ServerOutputTypeDef,
+    AppValidationConfigurationOutputTypeDef,
     ServerGroupTypeDef,
     ServerLaunchConfigurationTypeDef,
     ServerReplicationConfigurationTypeDef,
+    AppValidationConfigurationTypeDef,
     ServerValidationConfigurationTypeDef,
-    ServerValidationOutputTypeDef,
     GetReplicationJobsResponseTypeDef,
     GetReplicationRunsResponseTypeDef,
+    GetServersResponseTypeDef,
+    ServerGroupOutputTypeDef,
+    ServerLaunchConfigurationOutputTypeDef,
+    ServerReplicationConfigurationOutputTypeDef,
+    ServerValidationConfigurationOutputTypeDef,
+    ServerValidationOutputTypeDef,
     CreateAppRequestRequestTypeDef,
-    CreateAppResponseTypeDef,
-    GetAppResponseTypeDef,
     UpdateAppRequestRequestTypeDef,
-    UpdateAppResponseTypeDef,
     ServerGroupLaunchConfigurationTypeDef,
     ServerGroupReplicationConfigurationTypeDef,
     ServerGroupValidationConfigurationTypeDef,
+    CreateAppResponseTypeDef,
+    GetAppResponseTypeDef,
+    UpdateAppResponseTypeDef,
+    ServerGroupLaunchConfigurationOutputTypeDef,
+    ServerGroupReplicationConfigurationOutputTypeDef,
+    ServerGroupValidationConfigurationOutputTypeDef,
     ValidationOutputTypeDef,
-    GetAppLaunchConfigurationResponseTypeDef,
     PutAppLaunchConfigurationRequestRequestTypeDef,
-    GetAppReplicationConfigurationResponseTypeDef,
     PutAppReplicationConfigurationRequestRequestTypeDef,
-    GetAppValidationConfigurationResponseTypeDef,
     PutAppValidationConfigurationRequestRequestTypeDef,
+    GetAppLaunchConfigurationResponseTypeDef,
+    GetAppReplicationConfigurationResponseTypeDef,
+    GetAppValidationConfigurationResponseTypeDef,
     GetAppValidationOutputResponseTypeDef,
 )
 
 
 def get_structure() -> LaunchDetailsTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-sms-1.28.0/mypy_boto3_sms.egg-info/SOURCES.txt` & `mypy-boto3-sms-1.28.12/mypy_boto3_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sms-1.28.0/setup.py` & `mypy-boto3-sms-1.28.12/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sms",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SMS 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SMS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

