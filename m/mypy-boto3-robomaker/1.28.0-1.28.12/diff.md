# Comparing `tmp/mypy-boto3-robomaker-1.28.0.tar.gz` & `tmp/mypy-boto3-robomaker-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-robomaker-1.28.0.tar", last modified: Thu Jul  6 21:00:26 2023, max compression
+gzip compressed data, was "mypy-boto3-robomaker-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
```

## Comparing `mypy-boto3-robomaker-1.28.0.tar` & `mypy-boto3-robomaker-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.886409 mypy-boto3-robomaker-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:22.000000 mypy-boto3-robomaker-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-07-06 21:00:26.886409 mypy-boto3-robomaker-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20258 2023-07-06 20:53:22.000000 mypy-boto3-robomaker-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.874409 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-06 20:53:22.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-06 20:53:22.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:53:22.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42233 2023-07-06 20:53:23.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42158 2023-07-06 20:53:23.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-06 20:53:23.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-07-06 20:53:23.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-07-06 20:53:23.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-07-06 20:53:23.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:22.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63609 2023-07-06 20:53:25.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63554 2023-07-06 20:53:24.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:22.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.886409 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-07-06 21:00:26.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 21:00:26.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:26.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:26.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:26.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 21:00:26.000000 mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:26.886409 mypy-boto3-robomaker-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:53:22.000000 mypy-boto3-robomaker-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.421214 mypy-boto3-robomaker-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-07-27 11:49:30.421214 mypy-boto3-robomaker-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.421214 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42233 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42158 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-07-27 11:44:44.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-07-27 11:44:44.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-07-27 11:44:44.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-07-27 11:44:47.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72951 2023-07-27 11:44:45.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.421214 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-07-27 11:49:30.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 11:49:30.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 11:49:30.000000 mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.421214 mypy-boto3-robomaker-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 11:44:43.000000 mypy-boto3-robomaker-1.28.12/setup.py
```

### Comparing `mypy-boto3-robomaker-1.28.0/LICENSE` & `mypy-boto3-robomaker-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.0/PKG-INFO` & `mypy-boto3-robomaker-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-robomaker
-Version: 1.28.0
-Summary: Type annotations for boto3.RoboMaker 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.RoboMaker 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-robomaker"></a>
 
 # mypy-boto3-robomaker
 
 [![PyPI - mypy-boto3-robomaker](https://img.shields.io/pypi/v/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-robomaker?color=blue)](https://pypistats.org/packages/mypy-boto3-robomaker)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-robomaker)](https://pepy.tech/project/mypy-boto3-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RoboMaker 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[boto3.RoboMaker 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,176 +389,200 @@
 
 `mypy_boto3_robomaker.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
-    BatchDeleteWorldsResponseTypeDef,
+    ResponseMetadataTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
+    BatchPolicyOutputTypeDef,
     BatchPolicyTypeDef,
     CancelDeploymentJobRequestRequestTypeDef,
     CancelSimulationJobBatchRequestRequestTypeDef,
     CancelSimulationJobRequestRequestTypeDef,
     CancelWorldExportJobRequestRequestTypeDef,
     CancelWorldGenerationJobRequestRequestTypeDef,
+    ComputeOutputTypeDef,
     ComputeResponseTypeDef,
     ComputeTypeDef,
     CreateFleetRequestRequestTypeDef,
-    CreateFleetResponseTypeDef,
     EnvironmentTypeDef,
     RobotSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
+    EnvironmentOutputTypeDef,
+    RobotSoftwareSuiteOutputTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
-    CreateRobotResponseTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
+    RenderingEngineOutputTypeDef,
+    SimulationSoftwareSuiteOutputTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
     DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
+    LoggingConfigOutputTypeDef,
+    OutputLocationOutputTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
+    WorldCountOutputTypeDef,
     TemplateLocationTypeDef,
-    CreateWorldTemplateResponseTypeDef,
+    DataSourceConfigOutputTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
+    DeploymentLaunchConfigOutputTypeDef,
     DeploymentLaunchConfigTypeDef,
+    S3ObjectOutputTypeDef,
     S3ObjectTypeDef,
     DeregisterRobotRequestRequestTypeDef,
-    DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobRequestRequestTypeDef,
     DescribeFleetRequestRequestTypeDef,
     RobotTypeDef,
     DescribeRobotApplicationRequestRequestTypeDef,
     DescribeRobotRequestRequestTypeDef,
-    DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationRequestRequestTypeDef,
     DescribeSimulationJobBatchRequestRequestTypeDef,
     SimulationJobSummaryTypeDef,
     DescribeSimulationJobRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeWorldExportJobRequestRequestTypeDef,
     DescribeWorldGenerationJobRequestRequestTypeDef,
     DescribeWorldRequestRequestTypeDef,
-    DescribeWorldResponseTypeDef,
     DescribeWorldTemplateRequestRequestTypeDef,
-    DescribeWorldTemplateResponseTypeDef,
     WorldFailureTypeDef,
     FilterTypeDef,
     FleetTypeDef,
     GetWorldTemplateBodyRequestRequestTypeDef,
-    GetWorldTemplateBodyResponseTypeDef,
+    PaginatorConfigTypeDef,
     SimulationJobBatchSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
     ListWorldTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     WorldSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    PortMappingOutputTypeDef,
     PortMappingTypeDef,
     ProgressDetailTypeDef,
     RegisterRobotRequestRequestTypeDef,
-    RegisterRobotResponseTypeDef,
-    ResponseMetadataTypeDef,
     RestartSimulationJobRequestRequestTypeDef,
+    ToolOutputTypeDef,
+    UploadConfigurationOutputTypeDef,
     ToolTypeDef,
     UploadConfigurationTypeDef,
+    WorldConfigOutputTypeDef,
     WorldConfigTypeDef,
+    VPCConfigOutputTypeDef,
     SyncDeploymentJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    BatchDeleteWorldsResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    CreateRobotResponseTypeDef,
+    CreateWorldTemplateResponseTypeDef,
+    DeregisterRobotResponseTypeDef,
+    DescribeRobotResponseTypeDef,
+    DescribeWorldResponseTypeDef,
+    DescribeWorldTemplateResponseTypeDef,
+    GetWorldTemplateBodyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterRobotResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
-    RobotApplicationSummaryTypeDef,
     CreateRobotApplicationRequestRequestTypeDef,
     UpdateRobotApplicationRequestRequestTypeDef,
+    RobotApplicationSummaryTypeDef,
     CreateRobotApplicationResponseTypeDef,
     CreateRobotApplicationVersionResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     CreateSimulationApplicationRequestRequestTypeDef,
+    UpdateSimulationApplicationRequestRequestTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     DescribeSimulationApplicationResponseTypeDef,
     SimulationApplicationSummaryTypeDef,
-    UpdateSimulationApplicationRequestRequestTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     CreateWorldExportJobRequestRequestTypeDef,
     CreateWorldExportJobResponseTypeDef,
     DescribeWorldExportJobResponseTypeDef,
     WorldExportJobSummaryTypeDef,
     CreateWorldGenerationJobRequestRequestTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     WorldGenerationJobSummaryTypeDef,
     CreateWorldTemplateRequestRequestTypeDef,
     UpdateWorldTemplateRequestRequestTypeDef,
     DataSourceTypeDef,
+    DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
+    DeploymentConfigOutputTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
     FailureSummaryTypeDef,
-    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
     ListDeploymentJobsRequestRequestTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
-    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
     ListRobotApplicationsRequestRequestTypeDef,
-    ListRobotsRequestListRobotsPaginateTypeDef,
     ListRobotsRequestRequestTypeDef,
-    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
     ListSimulationApplicationsRequestRequestTypeDef,
-    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
     ListSimulationJobBatchesRequestRequestTypeDef,
-    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
     ListSimulationJobsRequestRequestTypeDef,
-    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
     ListWorldExportJobsRequestRequestTypeDef,
-    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
     ListWorldGenerationJobsRequestRequestTypeDef,
-    ListWorldsRequestListWorldsPaginateTypeDef,
     ListWorldsRequestRequestTypeDef,
     ListFleetsResponseTypeDef,
+    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
+    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
+    ListRobotsRequestListRobotsPaginateTypeDef,
+    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
+    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
+    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
+    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
+    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
+    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
+    ListWorldsRequestListWorldsPaginateTypeDef,
     ListSimulationJobBatchesResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     ListWorldsResponseTypeDef,
+    PortForwardingConfigOutputTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
     ListWorldExportJobsResponseTypeDef,
     ListWorldGenerationJobsResponseTypeDef,
-    CreateDeploymentJobRequestRequestTypeDef,
     CreateDeploymentJobResponseTypeDef,
     DeploymentJobTypeDef,
     SyncDeploymentJobResponseTypeDef,
+    CreateDeploymentJobRequestRequestTypeDef,
     FinishedWorldsSummaryTypeDef,
+    LaunchConfigOutputTypeDef,
     LaunchConfigTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     ListDeploymentJobsResponseTypeDef,
     DescribeWorldGenerationJobResponseTypeDef,
+    RobotApplicationConfigOutputTypeDef,
+    SimulationApplicationConfigOutputTypeDef,
     RobotApplicationConfigTypeDef,
     SimulationApplicationConfigTypeDef,
-    CreateSimulationJobRequestRequestTypeDef,
     CreateSimulationJobResponseTypeDef,
     DescribeSimulationJobResponseTypeDef,
-    SimulationJobRequestTypeDef,
+    SimulationJobRequestOutputTypeDef,
     SimulationJobTypeDef,
+    CreateSimulationJobRequestRequestTypeDef,
+    SimulationJobRequestTypeDef,
     FailedCreateSimulationJobRequestTypeDef,
-    StartSimulationJobBatchRequestRequestTypeDef,
     BatchDescribeSimulationJobResponseTypeDef,
+    StartSimulationJobBatchRequestRequestTypeDef,
     DescribeSimulationJobBatchResponseTypeDef,
     StartSimulationJobBatchResponseTypeDef,
 )
 
 
 def get_structure() -> BatchDeleteWorldsRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-robomaker-1.28.0/README.md` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-robomaker
+Version: 1.28.12
+Summary: Type annotations for boto3.RoboMaker 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 robomaker type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-robomaker"></a>
 
 # mypy-boto3-robomaker
 
 [![PyPI - mypy-boto3-robomaker](https://img.shields.io/pypi/v/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-robomaker?color=blue)](https://pypistats.org/packages/mypy-boto3-robomaker)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-robomaker)](https://pepy.tech/project/mypy-boto3-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RoboMaker 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[boto3.RoboMaker 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,176 +389,200 @@
 
 `mypy_boto3_robomaker.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
-    BatchDeleteWorldsResponseTypeDef,
+    ResponseMetadataTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
+    BatchPolicyOutputTypeDef,
     BatchPolicyTypeDef,
     CancelDeploymentJobRequestRequestTypeDef,
     CancelSimulationJobBatchRequestRequestTypeDef,
     CancelSimulationJobRequestRequestTypeDef,
     CancelWorldExportJobRequestRequestTypeDef,
     CancelWorldGenerationJobRequestRequestTypeDef,
+    ComputeOutputTypeDef,
     ComputeResponseTypeDef,
     ComputeTypeDef,
     CreateFleetRequestRequestTypeDef,
-    CreateFleetResponseTypeDef,
     EnvironmentTypeDef,
     RobotSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
+    EnvironmentOutputTypeDef,
+    RobotSoftwareSuiteOutputTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
-    CreateRobotResponseTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
+    RenderingEngineOutputTypeDef,
+    SimulationSoftwareSuiteOutputTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
     DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
+    LoggingConfigOutputTypeDef,
+    OutputLocationOutputTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
+    WorldCountOutputTypeDef,
     TemplateLocationTypeDef,
-    CreateWorldTemplateResponseTypeDef,
+    DataSourceConfigOutputTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
+    DeploymentLaunchConfigOutputTypeDef,
     DeploymentLaunchConfigTypeDef,
+    S3ObjectOutputTypeDef,
     S3ObjectTypeDef,
     DeregisterRobotRequestRequestTypeDef,
-    DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobRequestRequestTypeDef,
     DescribeFleetRequestRequestTypeDef,
     RobotTypeDef,
     DescribeRobotApplicationRequestRequestTypeDef,
     DescribeRobotRequestRequestTypeDef,
-    DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationRequestRequestTypeDef,
     DescribeSimulationJobBatchRequestRequestTypeDef,
     SimulationJobSummaryTypeDef,
     DescribeSimulationJobRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeWorldExportJobRequestRequestTypeDef,
     DescribeWorldGenerationJobRequestRequestTypeDef,
     DescribeWorldRequestRequestTypeDef,
-    DescribeWorldResponseTypeDef,
     DescribeWorldTemplateRequestRequestTypeDef,
-    DescribeWorldTemplateResponseTypeDef,
     WorldFailureTypeDef,
     FilterTypeDef,
     FleetTypeDef,
     GetWorldTemplateBodyRequestRequestTypeDef,
-    GetWorldTemplateBodyResponseTypeDef,
+    PaginatorConfigTypeDef,
     SimulationJobBatchSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
     ListWorldTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     WorldSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    PortMappingOutputTypeDef,
     PortMappingTypeDef,
     ProgressDetailTypeDef,
     RegisterRobotRequestRequestTypeDef,
-    RegisterRobotResponseTypeDef,
-    ResponseMetadataTypeDef,
     RestartSimulationJobRequestRequestTypeDef,
+    ToolOutputTypeDef,
+    UploadConfigurationOutputTypeDef,
     ToolTypeDef,
     UploadConfigurationTypeDef,
+    WorldConfigOutputTypeDef,
     WorldConfigTypeDef,
+    VPCConfigOutputTypeDef,
     SyncDeploymentJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    BatchDeleteWorldsResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    CreateRobotResponseTypeDef,
+    CreateWorldTemplateResponseTypeDef,
+    DeregisterRobotResponseTypeDef,
+    DescribeRobotResponseTypeDef,
+    DescribeWorldResponseTypeDef,
+    DescribeWorldTemplateResponseTypeDef,
+    GetWorldTemplateBodyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterRobotResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
-    RobotApplicationSummaryTypeDef,
     CreateRobotApplicationRequestRequestTypeDef,
     UpdateRobotApplicationRequestRequestTypeDef,
+    RobotApplicationSummaryTypeDef,
     CreateRobotApplicationResponseTypeDef,
     CreateRobotApplicationVersionResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     CreateSimulationApplicationRequestRequestTypeDef,
+    UpdateSimulationApplicationRequestRequestTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     DescribeSimulationApplicationResponseTypeDef,
     SimulationApplicationSummaryTypeDef,
-    UpdateSimulationApplicationRequestRequestTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     CreateWorldExportJobRequestRequestTypeDef,
     CreateWorldExportJobResponseTypeDef,
     DescribeWorldExportJobResponseTypeDef,
     WorldExportJobSummaryTypeDef,
     CreateWorldGenerationJobRequestRequestTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     WorldGenerationJobSummaryTypeDef,
     CreateWorldTemplateRequestRequestTypeDef,
     UpdateWorldTemplateRequestRequestTypeDef,
     DataSourceTypeDef,
+    DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
+    DeploymentConfigOutputTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
     FailureSummaryTypeDef,
-    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
     ListDeploymentJobsRequestRequestTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
-    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
     ListRobotApplicationsRequestRequestTypeDef,
-    ListRobotsRequestListRobotsPaginateTypeDef,
     ListRobotsRequestRequestTypeDef,
-    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
     ListSimulationApplicationsRequestRequestTypeDef,
-    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
     ListSimulationJobBatchesRequestRequestTypeDef,
-    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
     ListSimulationJobsRequestRequestTypeDef,
-    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
     ListWorldExportJobsRequestRequestTypeDef,
-    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
     ListWorldGenerationJobsRequestRequestTypeDef,
-    ListWorldsRequestListWorldsPaginateTypeDef,
     ListWorldsRequestRequestTypeDef,
     ListFleetsResponseTypeDef,
+    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
+    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
+    ListRobotsRequestListRobotsPaginateTypeDef,
+    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
+    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
+    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
+    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
+    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
+    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
+    ListWorldsRequestListWorldsPaginateTypeDef,
     ListSimulationJobBatchesResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     ListWorldsResponseTypeDef,
+    PortForwardingConfigOutputTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
     ListWorldExportJobsResponseTypeDef,
     ListWorldGenerationJobsResponseTypeDef,
-    CreateDeploymentJobRequestRequestTypeDef,
     CreateDeploymentJobResponseTypeDef,
     DeploymentJobTypeDef,
     SyncDeploymentJobResponseTypeDef,
+    CreateDeploymentJobRequestRequestTypeDef,
     FinishedWorldsSummaryTypeDef,
+    LaunchConfigOutputTypeDef,
     LaunchConfigTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     ListDeploymentJobsResponseTypeDef,
     DescribeWorldGenerationJobResponseTypeDef,
+    RobotApplicationConfigOutputTypeDef,
+    SimulationApplicationConfigOutputTypeDef,
     RobotApplicationConfigTypeDef,
     SimulationApplicationConfigTypeDef,
-    CreateSimulationJobRequestRequestTypeDef,
     CreateSimulationJobResponseTypeDef,
     DescribeSimulationJobResponseTypeDef,
-    SimulationJobRequestTypeDef,
+    SimulationJobRequestOutputTypeDef,
     SimulationJobTypeDef,
+    CreateSimulationJobRequestRequestTypeDef,
+    SimulationJobRequestTypeDef,
     FailedCreateSimulationJobRequestTypeDef,
-    StartSimulationJobBatchRequestRequestTypeDef,
     BatchDescribeSimulationJobResponseTypeDef,
+    StartSimulationJobBatchRequestRequestTypeDef,
     DescribeSimulationJobBatchResponseTypeDef,
     StartSimulationJobBatchResponseTypeDef,
 )
 
 
 def get_structure() -> BatchDeleteWorldsRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/__init__.py` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/__init__.pyi` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/__main__.py` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RoboMaker 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.RoboMaker 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker\nOther"
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

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/client.py` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/client.pyi` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/literals.py` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,14 +318,15 @@
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
@@ -404,26 +405,28 @@
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

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/literals.pyi` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,15 @@
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
@@ -402,26 +403,28 @@
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

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/paginator.py` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listdeploymentjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListDeploymentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listdeploymentjobspaginator)
         """
 
 
@@ -108,15 +108,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listfleetspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listfleetspaginator)
         """
 
 
@@ -127,15 +127,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRobotApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobotApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listrobotapplicationspaginator)
         """
 
 
@@ -145,15 +145,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listrobotspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRobotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listrobotspaginator)
         """
 
 
@@ -164,15 +164,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSimulationApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationapplicationspaginator)
         """
 
 
@@ -182,15 +182,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobbatchespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSimulationJobBatchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobBatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobbatchespaginator)
         """
 
 
@@ -200,15 +200,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSimulationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobspaginator)
         """
 
 
@@ -218,15 +218,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorldExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldexportjobspaginator)
         """
 
 
@@ -236,30 +236,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldgenerationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorldGenerationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldGenerationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldgenerationjobspaginator)
         """
 
 
 class ListWorldTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorldTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldtemplatespaginator)
         """
 
 
@@ -269,13 +269,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorldsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorlds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldspaginator)
         """
```

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/paginator.pyi` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listdeploymentjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeploymentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListDeploymentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listdeploymentjobspaginator)
         """
 
 class ListFleetsPaginator(Paginator):
@@ -104,15 +104,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listfleetspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listfleetspaginator)
         """
 
 class ListRobotApplicationsPaginator(Paginator):
@@ -122,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRobotApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobotApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listrobotapplicationspaginator)
         """
 
 class ListRobotsPaginator(Paginator):
@@ -139,15 +139,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listrobotspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRobotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listrobotspaginator)
         """
 
 class ListSimulationApplicationsPaginator(Paginator):
@@ -157,15 +157,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSimulationApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationapplicationspaginator)
         """
 
 class ListSimulationJobBatchesPaginator(Paginator):
@@ -174,15 +174,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobbatchespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSimulationJobBatchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobBatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobbatchespaginator)
         """
 
 class ListSimulationJobsPaginator(Paginator):
@@ -191,15 +191,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSimulationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listsimulationjobspaginator)
         """
 
 class ListWorldExportJobsPaginator(Paginator):
@@ -208,15 +208,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorldExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldexportjobspaginator)
         """
 
 class ListWorldGenerationJobsPaginator(Paginator):
@@ -225,29 +225,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldgenerationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorldGenerationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldGenerationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldgenerationjobspaginator)
         """
 
 class ListWorldTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorldTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldtemplatespaginator)
         """
 
 class ListWorldsPaginator(Paginator):
@@ -256,13 +256,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorldsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorlds.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/paginators/#listworldspaginator)
         """
```

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/type_defs.py` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,202 +46,238 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchDeleteWorldsRequestRequestTypeDef",
-    "BatchDeleteWorldsResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDescribeSimulationJobRequestRequestTypeDef",
+    "BatchPolicyOutputTypeDef",
     "BatchPolicyTypeDef",
     "CancelDeploymentJobRequestRequestTypeDef",
     "CancelSimulationJobBatchRequestRequestTypeDef",
     "CancelSimulationJobRequestRequestTypeDef",
     "CancelWorldExportJobRequestRequestTypeDef",
     "CancelWorldGenerationJobRequestRequestTypeDef",
+    "ComputeOutputTypeDef",
     "ComputeResponseTypeDef",
     "ComputeTypeDef",
     "CreateFleetRequestRequestTypeDef",
-    "CreateFleetResponseTypeDef",
     "EnvironmentTypeDef",
     "RobotSoftwareSuiteTypeDef",
     "SourceConfigTypeDef",
+    "EnvironmentOutputTypeDef",
+    "RobotSoftwareSuiteOutputTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
-    "CreateRobotResponseTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
+    "RenderingEngineOutputTypeDef",
+    "SimulationSoftwareSuiteOutputTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
     "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
+    "LoggingConfigOutputTypeDef",
+    "OutputLocationOutputTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
+    "WorldCountOutputTypeDef",
     "TemplateLocationTypeDef",
-    "CreateWorldTemplateResponseTypeDef",
+    "DataSourceConfigOutputTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
+    "DeploymentLaunchConfigOutputTypeDef",
     "DeploymentLaunchConfigTypeDef",
+    "S3ObjectOutputTypeDef",
     "S3ObjectTypeDef",
     "DeregisterRobotRequestRequestTypeDef",
-    "DeregisterRobotResponseTypeDef",
     "DescribeDeploymentJobRequestRequestTypeDef",
     "DescribeFleetRequestRequestTypeDef",
     "RobotTypeDef",
     "DescribeRobotApplicationRequestRequestTypeDef",
     "DescribeRobotRequestRequestTypeDef",
-    "DescribeRobotResponseTypeDef",
     "DescribeSimulationApplicationRequestRequestTypeDef",
     "DescribeSimulationJobBatchRequestRequestTypeDef",
     "SimulationJobSummaryTypeDef",
     "DescribeSimulationJobRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeWorldExportJobRequestRequestTypeDef",
     "DescribeWorldGenerationJobRequestRequestTypeDef",
     "DescribeWorldRequestRequestTypeDef",
-    "DescribeWorldResponseTypeDef",
     "DescribeWorldTemplateRequestRequestTypeDef",
-    "DescribeWorldTemplateResponseTypeDef",
     "WorldFailureTypeDef",
     "FilterTypeDef",
     "FleetTypeDef",
     "GetWorldTemplateBodyRequestRequestTypeDef",
-    "GetWorldTemplateBodyResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "SimulationJobBatchSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
     "ListWorldTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "WorldSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "PortMappingOutputTypeDef",
     "PortMappingTypeDef",
     "ProgressDetailTypeDef",
     "RegisterRobotRequestRequestTypeDef",
-    "RegisterRobotResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RestartSimulationJobRequestRequestTypeDef",
+    "ToolOutputTypeDef",
+    "UploadConfigurationOutputTypeDef",
     "ToolTypeDef",
     "UploadConfigurationTypeDef",
+    "WorldConfigOutputTypeDef",
     "WorldConfigTypeDef",
+    "VPCConfigOutputTypeDef",
     "SyncDeploymentJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "BatchDeleteWorldsResponseTypeDef",
+    "CreateFleetResponseTypeDef",
+    "CreateRobotResponseTypeDef",
+    "CreateWorldTemplateResponseTypeDef",
+    "DeregisterRobotResponseTypeDef",
+    "DescribeRobotResponseTypeDef",
+    "DescribeWorldResponseTypeDef",
+    "DescribeWorldTemplateResponseTypeDef",
+    "GetWorldTemplateBodyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterRobotResponseTypeDef",
     "UpdateWorldTemplateResponseTypeDef",
-    "RobotApplicationSummaryTypeDef",
     "CreateRobotApplicationRequestRequestTypeDef",
     "UpdateRobotApplicationRequestRequestTypeDef",
+    "RobotApplicationSummaryTypeDef",
     "CreateRobotApplicationResponseTypeDef",
     "CreateRobotApplicationVersionResponseTypeDef",
     "DescribeRobotApplicationResponseTypeDef",
     "UpdateRobotApplicationResponseTypeDef",
     "CreateSimulationApplicationRequestRequestTypeDef",
+    "UpdateSimulationApplicationRequestRequestTypeDef",
     "CreateSimulationApplicationResponseTypeDef",
     "CreateSimulationApplicationVersionResponseTypeDef",
     "DescribeSimulationApplicationResponseTypeDef",
     "SimulationApplicationSummaryTypeDef",
-    "UpdateSimulationApplicationRequestRequestTypeDef",
     "UpdateSimulationApplicationResponseTypeDef",
     "CreateWorldExportJobRequestRequestTypeDef",
     "CreateWorldExportJobResponseTypeDef",
     "DescribeWorldExportJobResponseTypeDef",
     "WorldExportJobSummaryTypeDef",
     "CreateWorldGenerationJobRequestRequestTypeDef",
     "CreateWorldGenerationJobResponseTypeDef",
     "WorldGenerationJobSummaryTypeDef",
     "CreateWorldTemplateRequestRequestTypeDef",
     "UpdateWorldTemplateRequestRequestTypeDef",
     "DataSourceTypeDef",
+    "DeploymentApplicationConfigOutputTypeDef",
     "DeploymentApplicationConfigTypeDef",
+    "DeploymentConfigOutputTypeDef",
     "DeploymentConfigTypeDef",
     "DescribeFleetResponseTypeDef",
     "ListRobotsResponseTypeDef",
     "ListSimulationJobsResponseTypeDef",
     "FailureSummaryTypeDef",
-    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
     "ListDeploymentJobsRequestRequestTypeDef",
-    "ListFleetsRequestListFleetsPaginateTypeDef",
     "ListFleetsRequestRequestTypeDef",
-    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
     "ListRobotApplicationsRequestRequestTypeDef",
-    "ListRobotsRequestListRobotsPaginateTypeDef",
     "ListRobotsRequestRequestTypeDef",
-    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
     "ListSimulationApplicationsRequestRequestTypeDef",
-    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
     "ListSimulationJobBatchesRequestRequestTypeDef",
-    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
     "ListSimulationJobsRequestRequestTypeDef",
-    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     "ListWorldExportJobsRequestRequestTypeDef",
-    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     "ListWorldGenerationJobsRequestRequestTypeDef",
-    "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListWorldsRequestRequestTypeDef",
     "ListFleetsResponseTypeDef",
+    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
+    "ListFleetsRequestListFleetsPaginateTypeDef",
+    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
+    "ListRobotsRequestListRobotsPaginateTypeDef",
+    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
+    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
+    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
+    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
+    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
+    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
+    "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListSimulationJobBatchesResponseTypeDef",
     "ListWorldTemplatesResponseTypeDef",
     "ListWorldsResponseTypeDef",
+    "PortForwardingConfigOutputTypeDef",
     "PortForwardingConfigTypeDef",
     "RobotDeploymentTypeDef",
     "ListRobotApplicationsResponseTypeDef",
     "ListSimulationApplicationsResponseTypeDef",
     "ListWorldExportJobsResponseTypeDef",
     "ListWorldGenerationJobsResponseTypeDef",
-    "CreateDeploymentJobRequestRequestTypeDef",
     "CreateDeploymentJobResponseTypeDef",
     "DeploymentJobTypeDef",
     "SyncDeploymentJobResponseTypeDef",
+    "CreateDeploymentJobRequestRequestTypeDef",
     "FinishedWorldsSummaryTypeDef",
+    "LaunchConfigOutputTypeDef",
     "LaunchConfigTypeDef",
     "DescribeDeploymentJobResponseTypeDef",
     "ListDeploymentJobsResponseTypeDef",
     "DescribeWorldGenerationJobResponseTypeDef",
+    "RobotApplicationConfigOutputTypeDef",
+    "SimulationApplicationConfigOutputTypeDef",
     "RobotApplicationConfigTypeDef",
     "SimulationApplicationConfigTypeDef",
-    "CreateSimulationJobRequestRequestTypeDef",
     "CreateSimulationJobResponseTypeDef",
     "DescribeSimulationJobResponseTypeDef",
-    "SimulationJobRequestTypeDef",
+    "SimulationJobRequestOutputTypeDef",
     "SimulationJobTypeDef",
+    "CreateSimulationJobRequestRequestTypeDef",
+    "SimulationJobRequestTypeDef",
     "FailedCreateSimulationJobRequestTypeDef",
-    "StartSimulationJobBatchRequestRequestTypeDef",
     "BatchDescribeSimulationJobResponseTypeDef",
+    "StartSimulationJobBatchRequestRequestTypeDef",
     "DescribeSimulationJobBatchResponseTypeDef",
     "StartSimulationJobBatchResponseTypeDef",
 )
 
 BatchDeleteWorldsRequestRequestTypeDef = TypedDict(
     "BatchDeleteWorldsRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
     },
 )
 
-BatchDeleteWorldsResponseTypeDef = TypedDict(
-    "BatchDeleteWorldsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "unprocessedWorlds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BatchDescribeSimulationJobRequestRequestTypeDef = TypedDict(
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     {
         "jobs": Sequence[str],
     },
 )
 
+BatchPolicyOutputTypeDef = TypedDict(
+    "BatchPolicyOutputTypeDef",
+    {
+        "timeoutInSeconds": int,
+        "maxConcurrency": int,
+    },
+    total=False,
+)
+
 BatchPolicyTypeDef = TypedDict(
     "BatchPolicyTypeDef",
     {
         "timeoutInSeconds": int,
         "maxConcurrency": int,
     },
     total=False,
@@ -278,14 +314,24 @@
 CancelWorldGenerationJobRequestRequestTypeDef = TypedDict(
     "CancelWorldGenerationJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
+ComputeOutputTypeDef = TypedDict(
+    "ComputeOutputTypeDef",
+    {
+        "simulationUnitLimit": int,
+        "computeType": ComputeTypeType,
+        "gpuUnitLimit": int,
+    },
+    total=False,
+)
+
 ComputeResponseTypeDef = TypedDict(
     "ComputeResponseTypeDef",
     {
         "simulationUnitLimit": int,
         "computeType": ComputeTypeType,
         "gpuUnitLimit": int,
     },
@@ -319,25 +365,14 @@
 
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
 
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "uri": str,
     },
     total=False,
 )
@@ -357,14 +392,31 @@
         "s3Bucket": str,
         "s3Key": str,
         "architecture": ArchitectureType,
     },
     total=False,
 )
 
+EnvironmentOutputTypeDef = TypedDict(
+    "EnvironmentOutputTypeDef",
+    {
+        "uri": str,
+    },
+    total=False,
+)
+
+RobotSoftwareSuiteOutputTypeDef = TypedDict(
+    "RobotSoftwareSuiteOutputTypeDef",
+    {
+        "name": RobotSoftwareSuiteTypeType,
+        "version": RobotSoftwareSuiteVersionTypeType,
+    },
+    total=False,
+)
+
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
         "etag": str,
         "architecture": ArchitectureType,
@@ -415,27 +467,14 @@
 
 class CreateRobotRequestRequestTypeDef(
     _RequiredCreateRobotRequestRequestTypeDef, _OptionalCreateRobotRequestRequestTypeDef
 ):
     pass
 
 
-CreateRobotResponseTypeDef = TypedDict(
-    "CreateRobotResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "createdAt": datetime,
-        "greengrassGroupId": str,
-        "architecture": ArchitectureType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RenderingEngineTypeDef = TypedDict(
     "RenderingEngineTypeDef",
     {
         "name": Literal["OGRE"],
         "version": str,
     },
     total=False,
@@ -446,14 +485,32 @@
     {
         "name": SimulationSoftwareSuiteTypeType,
         "version": str,
     },
     total=False,
 )
 
+RenderingEngineOutputTypeDef = TypedDict(
+    "RenderingEngineOutputTypeDef",
+    {
+        "name": Literal["OGRE"],
+        "version": str,
+    },
+    total=False,
+)
+
+SimulationSoftwareSuiteOutputTypeDef = TypedDict(
+    "SimulationSoftwareSuiteOutputTypeDef",
+    {
+        "name": SimulationSoftwareSuiteTypeType,
+        "version": str,
+    },
+    total=False,
+)
+
 _RequiredCreateSimulationApplicationVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSimulationApplicationVersionRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalCreateSimulationApplicationVersionRequestRequestTypeDef = TypedDict(
@@ -529,14 +586,31 @@
 )
 
 
 class VPCConfigTypeDef(_RequiredVPCConfigTypeDef, _OptionalVPCConfigTypeDef):
     pass
 
 
+LoggingConfigOutputTypeDef = TypedDict(
+    "LoggingConfigOutputTypeDef",
+    {
+        "recordAllRosTopics": bool,
+    },
+    total=False,
+)
+
+OutputLocationOutputTypeDef = TypedDict(
+    "OutputLocationOutputTypeDef",
+    {
+        "s3Bucket": str,
+        "s3Prefix": str,
+    },
+    total=False,
+)
+
 VPCConfigResponseTypeDef = TypedDict(
     "VPCConfigResponseTypeDef",
     {
         "subnets": List[str],
         "securityGroups": List[str],
         "vpcId": str,
         "assignPublicIp": bool,
@@ -549,33 +623,54 @@
     {
         "floorplanCount": int,
         "interiorCountPerFloorplan": int,
     },
     total=False,
 )
 
+WorldCountOutputTypeDef = TypedDict(
+    "WorldCountOutputTypeDef",
+    {
+        "floorplanCount": int,
+        "interiorCountPerFloorplan": int,
+    },
+    total=False,
+)
+
 TemplateLocationTypeDef = TypedDict(
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
 
-CreateWorldTemplateResponseTypeDef = TypedDict(
-    "CreateWorldTemplateResponseTypeDef",
+_RequiredDataSourceConfigOutputTypeDef = TypedDict(
+    "_RequiredDataSourceConfigOutputTypeDef",
     {
-        "arn": str,
-        "clientRequestToken": str,
-        "createdAt": datetime,
         "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "s3Bucket": str,
+        "s3Keys": List[str],
     },
 )
+_OptionalDataSourceConfigOutputTypeDef = TypedDict(
+    "_OptionalDataSourceConfigOutputTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
+    },
+    total=False,
+)
+
+
+class DataSourceConfigOutputTypeDef(
+    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
+):
+    pass
+
 
 S3KeyOutputTypeDef = TypedDict(
     "S3KeyOutputTypeDef",
     {
         "s3Key": str,
         "etag": str,
     },
@@ -643,14 +738,38 @@
 DeleteWorldTemplateRequestRequestTypeDef = TypedDict(
     "DeleteWorldTemplateRequestRequestTypeDef",
     {
         "template": str,
     },
 )
 
+_RequiredDeploymentLaunchConfigOutputTypeDef = TypedDict(
+    "_RequiredDeploymentLaunchConfigOutputTypeDef",
+    {
+        "packageName": str,
+        "launchFile": str,
+    },
+)
+_OptionalDeploymentLaunchConfigOutputTypeDef = TypedDict(
+    "_OptionalDeploymentLaunchConfigOutputTypeDef",
+    {
+        "preLaunchFile": str,
+        "postLaunchFile": str,
+        "environmentVariables": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class DeploymentLaunchConfigOutputTypeDef(
+    _RequiredDeploymentLaunchConfigOutputTypeDef, _OptionalDeploymentLaunchConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredDeploymentLaunchConfigTypeDef = TypedDict(
     "_RequiredDeploymentLaunchConfigTypeDef",
     {
         "packageName": str,
         "launchFile": str,
     },
 )
@@ -667,14 +786,34 @@
 
 class DeploymentLaunchConfigTypeDef(
     _RequiredDeploymentLaunchConfigTypeDef, _OptionalDeploymentLaunchConfigTypeDef
 ):
     pass
 
 
+_RequiredS3ObjectOutputTypeDef = TypedDict(
+    "_RequiredS3ObjectOutputTypeDef",
+    {
+        "bucket": str,
+        "key": str,
+    },
+)
+_OptionalS3ObjectOutputTypeDef = TypedDict(
+    "_OptionalS3ObjectOutputTypeDef",
+    {
+        "etag": str,
+    },
+    total=False,
+)
+
+
+class S3ObjectOutputTypeDef(_RequiredS3ObjectOutputTypeDef, _OptionalS3ObjectOutputTypeDef):
+    pass
+
+
 _RequiredS3ObjectTypeDef = TypedDict(
     "_RequiredS3ObjectTypeDef",
     {
         "bucket": str,
         "key": str,
     },
 )
@@ -695,23 +834,14 @@
     "DeregisterRobotRequestRequestTypeDef",
     {
         "fleet": str,
         "robot": str,
     },
 )
 
-DeregisterRobotResponseTypeDef = TypedDict(
-    "DeregisterRobotResponseTypeDef",
-    {
-        "fleet": str,
-        "robot": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeploymentJobRequestRequestTypeDef = TypedDict(
     "DescribeDeploymentJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
@@ -763,31 +893,14 @@
 DescribeRobotRequestRequestTypeDef = TypedDict(
     "DescribeRobotRequestRequestTypeDef",
     {
         "robot": str,
     },
 )
 
-DescribeRobotResponseTypeDef = TypedDict(
-    "DescribeRobotResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "fleetArn": str,
-        "status": RobotStatusType,
-        "greengrassGroupId": str,
-        "createdAt": datetime,
-        "architecture": ArchitectureType,
-        "lastDeploymentJob": str,
-        "lastDeploymentTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSimulationApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalDescribeSimulationApplicationRequestRequestTypeDef = TypedDict(
@@ -862,48 +975,21 @@
 DescribeWorldRequestRequestTypeDef = TypedDict(
     "DescribeWorldRequestRequestTypeDef",
     {
         "world": str,
     },
 )
 
-DescribeWorldResponseTypeDef = TypedDict(
-    "DescribeWorldResponseTypeDef",
-    {
-        "arn": str,
-        "generationJob": str,
-        "template": str,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-        "worldDescriptionBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeWorldTemplateRequestRequestTypeDef = TypedDict(
     "DescribeWorldTemplateRequestRequestTypeDef",
     {
         "template": str,
     },
 )
 
-DescribeWorldTemplateResponseTypeDef = TypedDict(
-    "DescribeWorldTemplateResponseTypeDef",
-    {
-        "arn": str,
-        "clientRequestToken": str,
-        "name": str,
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "tags": Dict[str, str],
-        "version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorldFailureTypeDef = TypedDict(
     "WorldFailureTypeDef",
     {
         "failureCode": WorldGenerationJobErrorCodeType,
         "sampleFailureReason": str,
         "failureCount": int,
     },
@@ -937,20 +1023,22 @@
     {
         "template": str,
         "generationJob": str,
     },
     total=False,
 )
 
-GetWorldTemplateBodyResponseTypeDef = TypedDict(
-    "GetWorldTemplateBodyResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "templateBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
 SimulationJobBatchSummaryTypeDef = TypedDict(
     "SimulationJobBatchSummaryTypeDef",
     {
         "arn": str,
         "lastUpdatedAt": datetime,
@@ -966,30 +1054,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = TypedDict(
-    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorldTemplatesRequestRequestTypeDef = TypedDict(
     "ListWorldTemplatesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1014,24 +1086,36 @@
         "createdAt": datetime,
         "generationJob": str,
         "template": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredPortMappingOutputTypeDef = TypedDict(
+    "_RequiredPortMappingOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "jobPort": int,
+        "applicationPort": int,
+    },
+)
+_OptionalPortMappingOutputTypeDef = TypedDict(
+    "_OptionalPortMappingOutputTypeDef",
+    {
+        "enableOnPublicIp": bool,
     },
     total=False,
 )
 
+
+class PortMappingOutputTypeDef(
+    _RequiredPortMappingOutputTypeDef, _OptionalPortMappingOutputTypeDef
+):
+    pass
+
+
 _RequiredPortMappingTypeDef = TypedDict(
     "_RequiredPortMappingTypeDef",
     {
         "jobPort": int,
         "applicationPort": int,
     },
 )
@@ -1063,38 +1147,49 @@
     "RegisterRobotRequestRequestTypeDef",
     {
         "fleet": str,
         "robot": str,
     },
 )
 
-RegisterRobotResponseTypeDef = TypedDict(
-    "RegisterRobotResponseTypeDef",
+RestartSimulationJobRequestRequestTypeDef = TypedDict(
+    "RestartSimulationJobRequestRequestTypeDef",
     {
-        "fleet": str,
-        "robot": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "job": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredToolOutputTypeDef = TypedDict(
+    "_RequiredToolOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "name": str,
+        "command": str,
+    },
+)
+_OptionalToolOutputTypeDef = TypedDict(
+    "_OptionalToolOutputTypeDef",
+    {
+        "streamUI": bool,
+        "streamOutputToCloudWatch": bool,
+        "exitBehavior": ExitBehaviorType,
     },
+    total=False,
 )
 
-RestartSimulationJobRequestRequestTypeDef = TypedDict(
-    "RestartSimulationJobRequestRequestTypeDef",
+
+class ToolOutputTypeDef(_RequiredToolOutputTypeDef, _OptionalToolOutputTypeDef):
+    pass
+
+
+UploadConfigurationOutputTypeDef = TypedDict(
+    "UploadConfigurationOutputTypeDef",
     {
-        "job": str,
+        "name": str,
+        "path": str,
+        "uploadBehavior": UploadBehaviorType,
     },
 )
 
 _RequiredToolTypeDef = TypedDict(
     "_RequiredToolTypeDef",
     {
         "name": str,
@@ -1121,22 +1216,50 @@
     {
         "name": str,
         "path": str,
         "uploadBehavior": UploadBehaviorType,
     },
 )
 
+WorldConfigOutputTypeDef = TypedDict(
+    "WorldConfigOutputTypeDef",
+    {
+        "world": str,
+    },
+    total=False,
+)
+
 WorldConfigTypeDef = TypedDict(
     "WorldConfigTypeDef",
     {
         "world": str,
     },
     total=False,
 )
 
+_RequiredVPCConfigOutputTypeDef = TypedDict(
+    "_RequiredVPCConfigOutputTypeDef",
+    {
+        "subnets": List[str],
+    },
+)
+_OptionalVPCConfigOutputTypeDef = TypedDict(
+    "_OptionalVPCConfigOutputTypeDef",
+    {
+        "securityGroups": List[str],
+        "assignPublicIp": bool,
+    },
+    total=False,
+)
+
+
+class VPCConfigOutputTypeDef(_RequiredVPCConfigOutputTypeDef, _OptionalVPCConfigOutputTypeDef):
+    pass
+
+
 SyncDeploymentJobRequestRequestTypeDef = TypedDict(
     "SyncDeploymentJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
         "fleet": str,
     },
 )
@@ -1153,35 +1276,145 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateWorldTemplateResponseTypeDef = TypedDict(
-    "UpdateWorldTemplateResponseTypeDef",
+BatchDeleteWorldsResponseTypeDef = TypedDict(
+    "BatchDeleteWorldsResponseTypeDef",
+    {
+        "unprocessedWorlds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RobotApplicationSummaryTypeDef = TypedDict(
-    "RobotApplicationSummaryTypeDef",
+CreateRobotResponseTypeDef = TypedDict(
+    "CreateRobotResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "createdAt": datetime,
+        "greengrassGroupId": str,
+        "architecture": ArchitectureType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorldTemplateResponseTypeDef = TypedDict(
+    "CreateWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "clientRequestToken": str,
+        "createdAt": datetime,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterRobotResponseTypeDef = TypedDict(
+    "DeregisterRobotResponseTypeDef",
     {
+        "fleet": str,
+        "robot": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRobotResponseTypeDef = TypedDict(
+    "DescribeRobotResponseTypeDef",
+    {
+        "arn": str,
         "name": str,
+        "fleetArn": str,
+        "status": RobotStatusType,
+        "greengrassGroupId": str,
+        "createdAt": datetime,
+        "architecture": ArchitectureType,
+        "lastDeploymentJob": str,
+        "lastDeploymentTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorldResponseTypeDef = TypedDict(
+    "DescribeWorldResponseTypeDef",
+    {
         "arn": str,
+        "generationJob": str,
+        "template": str,
+        "createdAt": datetime,
+        "tags": Dict[str, str],
+        "worldDescriptionBody": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorldTemplateResponseTypeDef = TypedDict(
+    "DescribeWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "clientRequestToken": str,
+        "name": str,
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "tags": Dict[str, str],
         "version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorldTemplateBodyResponseTypeDef = TypedDict(
+    "GetWorldTemplateBodyResponseTypeDef",
+    {
+        "templateBody": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterRobotResponseTypeDef = TypedDict(
+    "RegisterRobotResponseTypeDef",
+    {
+        "fleet": str,
+        "robot": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorldTemplateResponseTypeDef = TypedDict(
+    "UpdateWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "createdAt": datetime,
         "lastUpdatedAt": datetime,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateRobotApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRobotApplicationRequestRequestTypeDef",
     {
         "name": str,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
@@ -1226,74 +1459,86 @@
 class UpdateRobotApplicationRequestRequestTypeDef(
     _RequiredUpdateRobotApplicationRequestRequestTypeDef,
     _OptionalUpdateRobotApplicationRequestRequestTypeDef,
 ):
     pass
 
 
+RobotApplicationSummaryTypeDef = TypedDict(
+    "RobotApplicationSummaryTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "version": str,
+        "lastUpdatedAt": datetime,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+    },
+    total=False,
+)
+
 CreateRobotApplicationResponseTypeDef = TypedDict(
     "CreateRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
-        "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "environment": EnvironmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRobotApplicationVersionResponseTypeDef = TypedDict(
     "CreateRobotApplicationVersionResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "environment": EnvironmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRobotApplicationResponseTypeDef = TypedDict(
     "DescribeRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "imageDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRobotApplicationResponseTypeDef = TypedDict(
     "UpdateRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "environment": EnvironmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSimulationApplicationRequestRequestTypeDef",
     {
         "name": str,
@@ -1316,122 +1561,122 @@
 class CreateSimulationApplicationRequestRequestTypeDef(
     _RequiredCreateSimulationApplicationRequestRequestTypeDef,
     _OptionalCreateSimulationApplicationRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSimulationApplicationRequestRequestTypeDef",
+    {
+        "application": str,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+    },
+)
+_OptionalUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSimulationApplicationRequestRequestTypeDef",
+    {
+        "sources": Sequence[SourceConfigTypeDef],
+        "renderingEngine": RenderingEngineTypeDef,
+        "currentRevisionId": str,
+        "environment": EnvironmentTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateSimulationApplicationRequestRequestTypeDef(
+    _RequiredUpdateSimulationApplicationRequestRequestTypeDef,
+    _OptionalUpdateSimulationApplicationRequestRequestTypeDef,
+):
+    pass
+
+
 CreateSimulationApplicationResponseTypeDef = TypedDict(
     "CreateSimulationApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-        "renderingEngine": RenderingEngineTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "renderingEngine": RenderingEngineOutputTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
-        "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "environment": EnvironmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSimulationApplicationVersionResponseTypeDef = TypedDict(
     "CreateSimulationApplicationVersionResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-        "renderingEngine": RenderingEngineTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "renderingEngine": RenderingEngineOutputTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "environment": EnvironmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationApplicationResponseTypeDef = TypedDict(
     "DescribeSimulationApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-        "renderingEngine": RenderingEngineTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "renderingEngine": RenderingEngineOutputTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "imageDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SimulationApplicationSummaryTypeDef = TypedDict(
     "SimulationApplicationSummaryTypeDef",
     {
         "name": str,
         "arn": str,
         "version": str,
         "lastUpdatedAt": datetime,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSimulationApplicationRequestRequestTypeDef",
-    {
-        "application": str,
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-    },
-)
-_OptionalUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSimulationApplicationRequestRequestTypeDef",
-    {
-        "sources": Sequence[SourceConfigTypeDef],
-        "renderingEngine": RenderingEngineTypeDef,
-        "currentRevisionId": str,
-        "environment": EnvironmentTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateSimulationApplicationRequestRequestTypeDef(
-    _RequiredUpdateSimulationApplicationRequestRequestTypeDef,
-    _OptionalUpdateSimulationApplicationRequestRequestTypeDef,
-):
-    pass
-
-
 UpdateSimulationApplicationResponseTypeDef = TypedDict(
     "UpdateSimulationApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-        "renderingEngine": RenderingEngineTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "renderingEngine": RenderingEngineOutputTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "environment": EnvironmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWorldExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorldExportJobRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
@@ -1460,46 +1705,46 @@
     "CreateWorldExportJobResponseTypeDef",
     {
         "arn": str,
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldExportJobErrorCodeType,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorldExportJobResponseTypeDef = TypedDict(
     "DescribeWorldExportJobResponseTypeDef",
     {
         "arn": str,
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldExportJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
         "worlds": List[str],
-        "outputLocation": OutputLocationTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorldExportJobSummaryTypeDef = TypedDict(
     "WorldExportJobSummaryTypeDef",
     {
         "arn": str,
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "worlds": List[str],
-        "outputLocation": OutputLocationTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateWorldGenerationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorldGenerationJobRequestRequestTypeDef",
     {
@@ -1530,29 +1775,29 @@
     {
         "arn": str,
         "status": WorldGenerationJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldGenerationJobErrorCodeType,
         "clientRequestToken": str,
         "template": str,
-        "worldCount": WorldCountTypeDef,
+        "worldCount": WorldCountOutputTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorldGenerationJobSummaryTypeDef = TypedDict(
     "WorldGenerationJobSummaryTypeDef",
     {
         "arn": str,
         "template": str,
         "createdAt": datetime,
         "status": WorldGenerationJobStatusType,
-        "worldCount": WorldCountTypeDef,
+        "worldCount": WorldCountOutputTypeDef,
         "succeededWorldCount": int,
         "failedWorldCount": int,
     },
     total=False,
 )
 
 CreateWorldTemplateRequestRequestTypeDef = TypedDict(
@@ -1599,23 +1844,43 @@
         "s3Keys": List[S3KeyOutputTypeDef],
         "type": DataSourceTypeType,
         "destination": str,
     },
     total=False,
 )
 
+DeploymentApplicationConfigOutputTypeDef = TypedDict(
+    "DeploymentApplicationConfigOutputTypeDef",
+    {
+        "application": str,
+        "applicationVersion": str,
+        "launchConfig": DeploymentLaunchConfigOutputTypeDef,
+    },
+)
+
 DeploymentApplicationConfigTypeDef = TypedDict(
     "DeploymentApplicationConfigTypeDef",
     {
         "application": str,
         "applicationVersion": str,
         "launchConfig": DeploymentLaunchConfigTypeDef,
     },
 )
 
+DeploymentConfigOutputTypeDef = TypedDict(
+    "DeploymentConfigOutputTypeDef",
+    {
+        "concurrentDeploymentPercentage": int,
+        "failureThresholdPercentage": int,
+        "robotDeploymentTimeoutInSeconds": int,
+        "downloadConditionFile": S3ObjectOutputTypeDef,
+    },
+    total=False,
+)
+
 DeploymentConfigTypeDef = TypedDict(
     "DeploymentConfigTypeDef",
     {
         "concurrentDeploymentPercentage": int,
         "failureThresholdPercentage": int,
         "robotDeploymentTimeoutInSeconds": int,
         "downloadConditionFile": S3ObjectTypeDef,
@@ -1630,279 +1895,295 @@
         "arn": str,
         "robots": List[RobotTypeDef],
         "createdAt": datetime,
         "lastDeploymentStatus": DeploymentStatusType,
         "lastDeploymentJob": str,
         "lastDeploymentTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRobotsResponseTypeDef = TypedDict(
     "ListRobotsResponseTypeDef",
     {
         "robots": List[RobotTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSimulationJobsResponseTypeDef = TypedDict(
     "ListSimulationJobsResponseTypeDef",
     {
         "simulationJobSummaries": List[SimulationJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailureSummaryTypeDef = TypedDict(
     "FailureSummaryTypeDef",
     {
         "totalFailureCount": int,
         "failures": List[WorldFailureTypeDef],
     },
     total=False,
 )
 
-ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = TypedDict(
-    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
+ListDeploymentJobsRequestRequestTypeDef = TypedDict(
+    "ListDeploymentJobsRequestRequestTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-ListDeploymentJobsRequestRequestTypeDef = TypedDict(
-    "ListDeploymentJobsRequestRequestTypeDef",
+ListFleetsRequestRequestTypeDef = TypedDict(
+    "ListFleetsRequestRequestTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
         "nextToken": str,
         "maxResults": int,
+        "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
-    "ListFleetsRequestListFleetsPaginateTypeDef",
+ListRobotApplicationsRequestRequestTypeDef = TypedDict(
+    "ListRobotApplicationsRequestRequestTypeDef",
     {
+        "versionQualifier": str,
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListFleetsRequestRequestTypeDef = TypedDict(
-    "ListFleetsRequestRequestTypeDef",
+ListRobotsRequestRequestTypeDef = TypedDict(
+    "ListRobotsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = TypedDict(
-    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
+ListSimulationApplicationsRequestRequestTypeDef = TypedDict(
+    "ListSimulationApplicationsRequestRequestTypeDef",
     {
         "versionQualifier": str,
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListRobotApplicationsRequestRequestTypeDef = TypedDict(
-    "ListRobotApplicationsRequestRequestTypeDef",
+ListSimulationJobBatchesRequestRequestTypeDef = TypedDict(
+    "ListSimulationJobBatchesRequestRequestTypeDef",
     {
-        "versionQualifier": str,
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListRobotsRequestListRobotsPaginateTypeDef = TypedDict(
-    "ListRobotsRequestListRobotsPaginateTypeDef",
+ListSimulationJobsRequestRequestTypeDef = TypedDict(
+    "ListSimulationJobsRequestRequestTypeDef",
     {
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListRobotsRequestRequestTypeDef = TypedDict(
-    "ListRobotsRequestRequestTypeDef",
+ListWorldExportJobsRequestRequestTypeDef = TypedDict(
+    "ListWorldExportJobsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = TypedDict(
-    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
+ListWorldGenerationJobsRequestRequestTypeDef = TypedDict(
+    "ListWorldGenerationJobsRequestRequestTypeDef",
     {
-        "versionQualifier": str,
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListSimulationApplicationsRequestRequestTypeDef = TypedDict(
-    "ListSimulationApplicationsRequestRequestTypeDef",
+ListWorldsRequestRequestTypeDef = TypedDict(
+    "ListWorldsRequestRequestTypeDef",
     {
-        "versionQualifier": str,
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = TypedDict(
-    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
+ListFleetsResponseTypeDef = TypedDict(
+    "ListFleetsResponseTypeDef",
+    {
+        "fleetDetails": List[FleetTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = TypedDict(
+    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobBatchesRequestRequestTypeDef = TypedDict(
-    "ListSimulationJobBatchesRequestRequestTypeDef",
+ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
+    "ListFleetsRequestListFleetsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = TypedDict(
-    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
+ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = TypedDict(
+    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
     {
+        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobsRequestRequestTypeDef = TypedDict(
-    "ListSimulationJobsRequestRequestTypeDef",
+ListRobotsRequestListRobotsPaginateTypeDef = TypedDict(
+    "ListRobotsRequestListRobotsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = TypedDict(
-    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
+ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = TypedDict(
+    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
     {
+        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldExportJobsRequestRequestTypeDef = TypedDict(
-    "ListWorldExportJobsRequestRequestTypeDef",
+ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = TypedDict(
+    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = TypedDict(
-    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
+ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = TypedDict(
+    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldGenerationJobsRequestRequestTypeDef = TypedDict(
-    "ListWorldGenerationJobsRequestRequestTypeDef",
+ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = TypedDict(
+    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldsRequestListWorldsPaginateTypeDef = TypedDict(
-    "ListWorldsRequestListWorldsPaginateTypeDef",
+ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = TypedDict(
+    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldsRequestRequestTypeDef = TypedDict(
-    "ListWorldsRequestRequestTypeDef",
+ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = TypedDict(
+    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
-        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListFleetsResponseTypeDef = TypedDict(
-    "ListFleetsResponseTypeDef",
+ListWorldsRequestListWorldsPaginateTypeDef = TypedDict(
+    "ListWorldsRequestListWorldsPaginateTypeDef",
     {
-        "fleetDetails": List[FleetTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListSimulationJobBatchesResponseTypeDef = TypedDict(
     "ListSimulationJobBatchesResponseTypeDef",
     {
         "simulationJobBatchSummaries": List[SimulationJobBatchSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldTemplatesResponseTypeDef = TypedDict(
     "ListWorldTemplatesResponseTypeDef",
     {
         "templateSummaries": List[TemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldsResponseTypeDef = TypedDict(
     "ListWorldsResponseTypeDef",
     {
         "worldSummaries": List[WorldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PortForwardingConfigOutputTypeDef = TypedDict(
+    "PortForwardingConfigOutputTypeDef",
+    {
+        "portMappings": List[PortMappingOutputTypeDef],
+    },
+    total=False,
+)
+
 PortForwardingConfigTypeDef = TypedDict(
     "PortForwardingConfigTypeDef",
     {
-        "portMappings": List[PortMappingTypeDef],
+        "portMappings": Sequence[PortMappingTypeDef],
     },
     total=False,
 )
 
 RobotDeploymentTypeDef = TypedDict(
     "RobotDeploymentTypeDef",
     {
@@ -1918,290 +2199,325 @@
 )
 
 ListRobotApplicationsResponseTypeDef = TypedDict(
     "ListRobotApplicationsResponseTypeDef",
     {
         "robotApplicationSummaries": List[RobotApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSimulationApplicationsResponseTypeDef = TypedDict(
     "ListSimulationApplicationsResponseTypeDef",
     {
         "simulationApplicationSummaries": List[SimulationApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldExportJobsResponseTypeDef = TypedDict(
     "ListWorldExportJobsResponseTypeDef",
     {
         "worldExportJobSummaries": List[WorldExportJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldGenerationJobsResponseTypeDef = TypedDict(
     "ListWorldGenerationJobsResponseTypeDef",
     {
         "worldGenerationJobSummaries": List[WorldGenerationJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "fleet": str,
-        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
-    },
-)
-_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDeploymentJobRequestRequestTypeDef(
-    _RequiredCreateDeploymentJobRequestRequestTypeDef,
-    _OptionalCreateDeploymentJobRequestRequestTypeDef,
-):
-    pass
-
-
 CreateDeploymentJobResponseTypeDef = TypedDict(
     "CreateDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
-        "deploymentConfig": DeploymentConfigTypeDef,
+        "deploymentConfig": DeploymentConfigOutputTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentJobTypeDef = TypedDict(
     "DeploymentJobTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
-        "deploymentConfig": DeploymentConfigTypeDef,
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
+        "deploymentConfig": DeploymentConfigOutputTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
     },
     total=False,
 )
 
 SyncDeploymentJobResponseTypeDef = TypedDict(
     "SyncDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentConfig": DeploymentConfigOutputTypeDef,
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "fleet": str,
+        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
+    },
+)
+_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "deploymentConfig": DeploymentConfigTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDeploymentJobRequestRequestTypeDef(
+    _RequiredCreateDeploymentJobRequestRequestTypeDef,
+    _OptionalCreateDeploymentJobRequestRequestTypeDef,
+):
+    pass
+
+
 FinishedWorldsSummaryTypeDef = TypedDict(
     "FinishedWorldsSummaryTypeDef",
     {
         "finishedCount": int,
         "succeededWorlds": List[str],
         "failureSummary": FailureSummaryTypeDef,
     },
     total=False,
 )
 
+LaunchConfigOutputTypeDef = TypedDict(
+    "LaunchConfigOutputTypeDef",
+    {
+        "packageName": str,
+        "launchFile": str,
+        "environmentVariables": Dict[str, str],
+        "portForwardingConfig": PortForwardingConfigOutputTypeDef,
+        "streamUI": bool,
+        "command": List[str],
+    },
+    total=False,
+)
+
 LaunchConfigTypeDef = TypedDict(
     "LaunchConfigTypeDef",
     {
         "packageName": str,
         "launchFile": str,
-        "environmentVariables": Dict[str, str],
+        "environmentVariables": Mapping[str, str],
         "portForwardingConfig": PortForwardingConfigTypeDef,
         "streamUI": bool,
-        "command": List[str],
+        "command": Sequence[str],
     },
     total=False,
 )
 
 DescribeDeploymentJobResponseTypeDef = TypedDict(
     "DescribeDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentConfig": DeploymentConfigOutputTypeDef,
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "robotDeploymentSummary": List[RobotDeploymentTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeploymentJobsResponseTypeDef = TypedDict(
     "ListDeploymentJobsResponseTypeDef",
     {
         "deploymentJobs": List[DeploymentJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorldGenerationJobResponseTypeDef = TypedDict(
     "DescribeWorldGenerationJobResponseTypeDef",
     {
         "arn": str,
         "status": WorldGenerationJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldGenerationJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
         "template": str,
-        "worldCount": WorldCountTypeDef,
+        "worldCount": WorldCountOutputTypeDef,
         "finishedWorldsSummary": FinishedWorldsSummaryTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRobotApplicationConfigTypeDef = TypedDict(
-    "_RequiredRobotApplicationConfigTypeDef",
+_RequiredRobotApplicationConfigOutputTypeDef = TypedDict(
+    "_RequiredRobotApplicationConfigOutputTypeDef",
     {
         "application": str,
-        "launchConfig": LaunchConfigTypeDef,
+        "launchConfig": LaunchConfigOutputTypeDef,
     },
 )
-_OptionalRobotApplicationConfigTypeDef = TypedDict(
-    "_OptionalRobotApplicationConfigTypeDef",
+_OptionalRobotApplicationConfigOutputTypeDef = TypedDict(
+    "_OptionalRobotApplicationConfigOutputTypeDef",
     {
         "applicationVersion": str,
-        "uploadConfigurations": List[UploadConfigurationTypeDef],
+        "uploadConfigurations": List[UploadConfigurationOutputTypeDef],
         "useDefaultUploadConfigurations": bool,
-        "tools": List[ToolTypeDef],
+        "tools": List[ToolOutputTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
 
-class RobotApplicationConfigTypeDef(
-    _RequiredRobotApplicationConfigTypeDef, _OptionalRobotApplicationConfigTypeDef
+class RobotApplicationConfigOutputTypeDef(
+    _RequiredRobotApplicationConfigOutputTypeDef, _OptionalRobotApplicationConfigOutputTypeDef
 ):
     pass
 
 
-_RequiredSimulationApplicationConfigTypeDef = TypedDict(
-    "_RequiredSimulationApplicationConfigTypeDef",
+_RequiredSimulationApplicationConfigOutputTypeDef = TypedDict(
+    "_RequiredSimulationApplicationConfigOutputTypeDef",
+    {
+        "application": str,
+        "launchConfig": LaunchConfigOutputTypeDef,
+    },
+)
+_OptionalSimulationApplicationConfigOutputTypeDef = TypedDict(
+    "_OptionalSimulationApplicationConfigOutputTypeDef",
+    {
+        "applicationVersion": str,
+        "uploadConfigurations": List[UploadConfigurationOutputTypeDef],
+        "worldConfigs": List[WorldConfigOutputTypeDef],
+        "useDefaultUploadConfigurations": bool,
+        "tools": List[ToolOutputTypeDef],
+        "useDefaultTools": bool,
+    },
+    total=False,
+)
+
+
+class SimulationApplicationConfigOutputTypeDef(
+    _RequiredSimulationApplicationConfigOutputTypeDef,
+    _OptionalSimulationApplicationConfigOutputTypeDef,
+):
+    pass
+
+
+_RequiredRobotApplicationConfigTypeDef = TypedDict(
+    "_RequiredRobotApplicationConfigTypeDef",
     {
         "application": str,
         "launchConfig": LaunchConfigTypeDef,
     },
 )
-_OptionalSimulationApplicationConfigTypeDef = TypedDict(
-    "_OptionalSimulationApplicationConfigTypeDef",
+_OptionalRobotApplicationConfigTypeDef = TypedDict(
+    "_OptionalRobotApplicationConfigTypeDef",
     {
         "applicationVersion": str,
-        "uploadConfigurations": List[UploadConfigurationTypeDef],
-        "worldConfigs": List[WorldConfigTypeDef],
+        "uploadConfigurations": Sequence[UploadConfigurationTypeDef],
         "useDefaultUploadConfigurations": bool,
-        "tools": List[ToolTypeDef],
+        "tools": Sequence[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
 
-class SimulationApplicationConfigTypeDef(
-    _RequiredSimulationApplicationConfigTypeDef, _OptionalSimulationApplicationConfigTypeDef
+class RobotApplicationConfigTypeDef(
+    _RequiredRobotApplicationConfigTypeDef, _OptionalRobotApplicationConfigTypeDef
 ):
     pass
 
 
-_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSimulationJobRequestRequestTypeDef",
+_RequiredSimulationApplicationConfigTypeDef = TypedDict(
+    "_RequiredSimulationApplicationConfigTypeDef",
     {
-        "maxJobDurationInSeconds": int,
-        "iamRole": str,
+        "application": str,
+        "launchConfig": LaunchConfigTypeDef,
     },
 )
-_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSimulationJobRequestRequestTypeDef",
+_OptionalSimulationApplicationConfigTypeDef = TypedDict(
+    "_OptionalSimulationApplicationConfigTypeDef",
     {
-        "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
-        "failureBehavior": FailureBehaviorType,
-        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
-        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
-        "dataSources": Sequence[DataSourceConfigTypeDef],
-        "tags": Mapping[str, str],
-        "vpcConfig": VPCConfigTypeDef,
-        "compute": ComputeTypeDef,
+        "applicationVersion": str,
+        "uploadConfigurations": Sequence[UploadConfigurationTypeDef],
+        "worldConfigs": Sequence[WorldConfigTypeDef],
+        "useDefaultUploadConfigurations": bool,
+        "tools": Sequence[ToolTypeDef],
+        "useDefaultTools": bool,
     },
     total=False,
 )
 
 
-class CreateSimulationJobRequestRequestTypeDef(
-    _RequiredCreateSimulationJobRequestRequestTypeDef,
-    _OptionalCreateSimulationJobRequestRequestTypeDef,
+class SimulationApplicationConfigTypeDef(
+    _RequiredSimulationApplicationConfigTypeDef, _OptionalSimulationApplicationConfigTypeDef
 ):
     pass
 
 
 CreateSimulationJobResponseTypeDef = TypedDict(
     "CreateSimulationJobResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobStatusType,
         "lastStartedAt": datetime,
         "lastUpdatedAt": datetime,
         "failureBehavior": FailureBehaviorType,
         "failureCode": SimulationJobErrorCodeType,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
+        "loggingConfig": LoggingConfigOutputTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "compute": ComputeResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationJobResponseTypeDef = TypedDict(
     "DescribeSimulationJobResponseTypeDef",
     {
         "arn": str,
@@ -2209,57 +2525,57 @@
         "status": SimulationJobStatusType,
         "lastStartedAt": datetime,
         "lastUpdatedAt": datetime,
         "failureBehavior": FailureBehaviorType,
         "failureCode": SimulationJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
+        "loggingConfig": LoggingConfigOutputTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSimulationJobRequestTypeDef = TypedDict(
-    "_RequiredSimulationJobRequestTypeDef",
+_RequiredSimulationJobRequestOutputTypeDef = TypedDict(
+    "_RequiredSimulationJobRequestOutputTypeDef",
     {
         "maxJobDurationInSeconds": int,
     },
 )
-_OptionalSimulationJobRequestTypeDef = TypedDict(
-    "_OptionalSimulationJobRequestTypeDef",
+_OptionalSimulationJobRequestOutputTypeDef = TypedDict(
+    "_OptionalSimulationJobRequestOutputTypeDef",
     {
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
+        "loggingConfig": LoggingConfigOutputTypeDef,
         "iamRole": str,
         "failureBehavior": FailureBehaviorType,
         "useDefaultApplications": bool,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
-        "dataSources": List[DataSourceConfigTypeDef],
-        "vpcConfig": VPCConfigTypeDef,
-        "compute": ComputeTypeDef,
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
+        "dataSources": List[DataSourceConfigOutputTypeDef],
+        "vpcConfig": VPCConfigOutputTypeDef,
+        "compute": ComputeOutputTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class SimulationJobRequestTypeDef(
-    _RequiredSimulationJobRequestTypeDef, _OptionalSimulationJobRequestTypeDef
+class SimulationJobRequestOutputTypeDef(
+    _RequiredSimulationJobRequestOutputTypeDef, _OptionalSimulationJobRequestOutputTypeDef
 ):
     pass
 
 
 SimulationJobTypeDef = TypedDict(
     "SimulationJobTypeDef",
     {
@@ -2268,41 +2584,113 @@
         "status": SimulationJobStatusType,
         "lastStartedAt": datetime,
         "lastUpdatedAt": datetime,
         "failureBehavior": FailureBehaviorType,
         "failureCode": SimulationJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
+        "loggingConfig": LoggingConfigOutputTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSimulationJobRequestRequestTypeDef",
+    {
+        "maxJobDurationInSeconds": int,
+        "iamRole": str,
+    },
+)
+_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSimulationJobRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
+        "failureBehavior": FailureBehaviorType,
+        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
+        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
+        "dataSources": Sequence[DataSourceConfigTypeDef],
+        "tags": Mapping[str, str],
+        "vpcConfig": VPCConfigTypeDef,
+        "compute": ComputeTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateSimulationJobRequestRequestTypeDef(
+    _RequiredCreateSimulationJobRequestRequestTypeDef,
+    _OptionalCreateSimulationJobRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSimulationJobRequestTypeDef = TypedDict(
+    "_RequiredSimulationJobRequestTypeDef",
+    {
+        "maxJobDurationInSeconds": int,
+    },
+)
+_OptionalSimulationJobRequestTypeDef = TypedDict(
+    "_OptionalSimulationJobRequestTypeDef",
+    {
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
+        "iamRole": str,
+        "failureBehavior": FailureBehaviorType,
+        "useDefaultApplications": bool,
+        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
+        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
+        "dataSources": Sequence[DataSourceConfigTypeDef],
+        "vpcConfig": VPCConfigTypeDef,
+        "compute": ComputeTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class SimulationJobRequestTypeDef(
+    _RequiredSimulationJobRequestTypeDef, _OptionalSimulationJobRequestTypeDef
+):
+    pass
+
+
 FailedCreateSimulationJobRequestTypeDef = TypedDict(
     "FailedCreateSimulationJobRequestTypeDef",
     {
-        "request": SimulationJobRequestTypeDef,
+        "request": SimulationJobRequestOutputTypeDef,
         "failureReason": str,
         "failureCode": SimulationJobErrorCodeType,
         "failedAt": datetime,
     },
     total=False,
 )
 
+BatchDescribeSimulationJobResponseTypeDef = TypedDict(
+    "BatchDescribeSimulationJobResponseTypeDef",
+    {
+        "jobs": List[SimulationJobTypeDef],
+        "unprocessedJobs": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
     "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
     {
         "createSimulationJobRequests": Sequence[SimulationJobRequestTypeDef],
     },
 )
 _OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
@@ -2319,52 +2707,43 @@
 class StartSimulationJobBatchRequestRequestTypeDef(
     _RequiredStartSimulationJobBatchRequestRequestTypeDef,
     _OptionalStartSimulationJobBatchRequestRequestTypeDef,
 ):
     pass
 
 
-BatchDescribeSimulationJobResponseTypeDef = TypedDict(
-    "BatchDescribeSimulationJobResponseTypeDef",
-    {
-        "jobs": List[SimulationJobTypeDef],
-        "unprocessedJobs": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSimulationJobBatchResponseTypeDef = TypedDict(
     "DescribeSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "lastUpdatedAt": datetime,
         "createdAt": datetime,
         "clientRequestToken": str,
-        "batchPolicy": BatchPolicyTypeDef,
+        "batchPolicy": BatchPolicyOutputTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
-        "pendingRequests": List[SimulationJobRequestTypeDef],
+        "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSimulationJobBatchResponseTypeDef = TypedDict(
     "StartSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "createdAt": datetime,
         "clientRequestToken": str,
-        "batchPolicy": BatchPolicyTypeDef,
+        "batchPolicy": BatchPolicyOutputTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
-        "pendingRequests": List[SimulationJobRequestTypeDef],
+        "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker/type_defs.pyi` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -45,202 +45,238 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchDeleteWorldsRequestRequestTypeDef",
-    "BatchDeleteWorldsResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDescribeSimulationJobRequestRequestTypeDef",
+    "BatchPolicyOutputTypeDef",
     "BatchPolicyTypeDef",
     "CancelDeploymentJobRequestRequestTypeDef",
     "CancelSimulationJobBatchRequestRequestTypeDef",
     "CancelSimulationJobRequestRequestTypeDef",
     "CancelWorldExportJobRequestRequestTypeDef",
     "CancelWorldGenerationJobRequestRequestTypeDef",
+    "ComputeOutputTypeDef",
     "ComputeResponseTypeDef",
     "ComputeTypeDef",
     "CreateFleetRequestRequestTypeDef",
-    "CreateFleetResponseTypeDef",
     "EnvironmentTypeDef",
     "RobotSoftwareSuiteTypeDef",
     "SourceConfigTypeDef",
+    "EnvironmentOutputTypeDef",
+    "RobotSoftwareSuiteOutputTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
-    "CreateRobotResponseTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
+    "RenderingEngineOutputTypeDef",
+    "SimulationSoftwareSuiteOutputTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
     "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
+    "LoggingConfigOutputTypeDef",
+    "OutputLocationOutputTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
+    "WorldCountOutputTypeDef",
     "TemplateLocationTypeDef",
-    "CreateWorldTemplateResponseTypeDef",
+    "DataSourceConfigOutputTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
+    "DeploymentLaunchConfigOutputTypeDef",
     "DeploymentLaunchConfigTypeDef",
+    "S3ObjectOutputTypeDef",
     "S3ObjectTypeDef",
     "DeregisterRobotRequestRequestTypeDef",
-    "DeregisterRobotResponseTypeDef",
     "DescribeDeploymentJobRequestRequestTypeDef",
     "DescribeFleetRequestRequestTypeDef",
     "RobotTypeDef",
     "DescribeRobotApplicationRequestRequestTypeDef",
     "DescribeRobotRequestRequestTypeDef",
-    "DescribeRobotResponseTypeDef",
     "DescribeSimulationApplicationRequestRequestTypeDef",
     "DescribeSimulationJobBatchRequestRequestTypeDef",
     "SimulationJobSummaryTypeDef",
     "DescribeSimulationJobRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeWorldExportJobRequestRequestTypeDef",
     "DescribeWorldGenerationJobRequestRequestTypeDef",
     "DescribeWorldRequestRequestTypeDef",
-    "DescribeWorldResponseTypeDef",
     "DescribeWorldTemplateRequestRequestTypeDef",
-    "DescribeWorldTemplateResponseTypeDef",
     "WorldFailureTypeDef",
     "FilterTypeDef",
     "FleetTypeDef",
     "GetWorldTemplateBodyRequestRequestTypeDef",
-    "GetWorldTemplateBodyResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "SimulationJobBatchSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
     "ListWorldTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "WorldSummaryTypeDef",
-    "PaginatorConfigTypeDef",
+    "PortMappingOutputTypeDef",
     "PortMappingTypeDef",
     "ProgressDetailTypeDef",
     "RegisterRobotRequestRequestTypeDef",
-    "RegisterRobotResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RestartSimulationJobRequestRequestTypeDef",
+    "ToolOutputTypeDef",
+    "UploadConfigurationOutputTypeDef",
     "ToolTypeDef",
     "UploadConfigurationTypeDef",
+    "WorldConfigOutputTypeDef",
     "WorldConfigTypeDef",
+    "VPCConfigOutputTypeDef",
     "SyncDeploymentJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "BatchDeleteWorldsResponseTypeDef",
+    "CreateFleetResponseTypeDef",
+    "CreateRobotResponseTypeDef",
+    "CreateWorldTemplateResponseTypeDef",
+    "DeregisterRobotResponseTypeDef",
+    "DescribeRobotResponseTypeDef",
+    "DescribeWorldResponseTypeDef",
+    "DescribeWorldTemplateResponseTypeDef",
+    "GetWorldTemplateBodyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterRobotResponseTypeDef",
     "UpdateWorldTemplateResponseTypeDef",
-    "RobotApplicationSummaryTypeDef",
     "CreateRobotApplicationRequestRequestTypeDef",
     "UpdateRobotApplicationRequestRequestTypeDef",
+    "RobotApplicationSummaryTypeDef",
     "CreateRobotApplicationResponseTypeDef",
     "CreateRobotApplicationVersionResponseTypeDef",
     "DescribeRobotApplicationResponseTypeDef",
     "UpdateRobotApplicationResponseTypeDef",
     "CreateSimulationApplicationRequestRequestTypeDef",
+    "UpdateSimulationApplicationRequestRequestTypeDef",
     "CreateSimulationApplicationResponseTypeDef",
     "CreateSimulationApplicationVersionResponseTypeDef",
     "DescribeSimulationApplicationResponseTypeDef",
     "SimulationApplicationSummaryTypeDef",
-    "UpdateSimulationApplicationRequestRequestTypeDef",
     "UpdateSimulationApplicationResponseTypeDef",
     "CreateWorldExportJobRequestRequestTypeDef",
     "CreateWorldExportJobResponseTypeDef",
     "DescribeWorldExportJobResponseTypeDef",
     "WorldExportJobSummaryTypeDef",
     "CreateWorldGenerationJobRequestRequestTypeDef",
     "CreateWorldGenerationJobResponseTypeDef",
     "WorldGenerationJobSummaryTypeDef",
     "CreateWorldTemplateRequestRequestTypeDef",
     "UpdateWorldTemplateRequestRequestTypeDef",
     "DataSourceTypeDef",
+    "DeploymentApplicationConfigOutputTypeDef",
     "DeploymentApplicationConfigTypeDef",
+    "DeploymentConfigOutputTypeDef",
     "DeploymentConfigTypeDef",
     "DescribeFleetResponseTypeDef",
     "ListRobotsResponseTypeDef",
     "ListSimulationJobsResponseTypeDef",
     "FailureSummaryTypeDef",
-    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
     "ListDeploymentJobsRequestRequestTypeDef",
-    "ListFleetsRequestListFleetsPaginateTypeDef",
     "ListFleetsRequestRequestTypeDef",
-    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
     "ListRobotApplicationsRequestRequestTypeDef",
-    "ListRobotsRequestListRobotsPaginateTypeDef",
     "ListRobotsRequestRequestTypeDef",
-    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
     "ListSimulationApplicationsRequestRequestTypeDef",
-    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
     "ListSimulationJobBatchesRequestRequestTypeDef",
-    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
     "ListSimulationJobsRequestRequestTypeDef",
-    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     "ListWorldExportJobsRequestRequestTypeDef",
-    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     "ListWorldGenerationJobsRequestRequestTypeDef",
-    "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListWorldsRequestRequestTypeDef",
     "ListFleetsResponseTypeDef",
+    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
+    "ListFleetsRequestListFleetsPaginateTypeDef",
+    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
+    "ListRobotsRequestListRobotsPaginateTypeDef",
+    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
+    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
+    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
+    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
+    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
+    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
+    "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListSimulationJobBatchesResponseTypeDef",
     "ListWorldTemplatesResponseTypeDef",
     "ListWorldsResponseTypeDef",
+    "PortForwardingConfigOutputTypeDef",
     "PortForwardingConfigTypeDef",
     "RobotDeploymentTypeDef",
     "ListRobotApplicationsResponseTypeDef",
     "ListSimulationApplicationsResponseTypeDef",
     "ListWorldExportJobsResponseTypeDef",
     "ListWorldGenerationJobsResponseTypeDef",
-    "CreateDeploymentJobRequestRequestTypeDef",
     "CreateDeploymentJobResponseTypeDef",
     "DeploymentJobTypeDef",
     "SyncDeploymentJobResponseTypeDef",
+    "CreateDeploymentJobRequestRequestTypeDef",
     "FinishedWorldsSummaryTypeDef",
+    "LaunchConfigOutputTypeDef",
     "LaunchConfigTypeDef",
     "DescribeDeploymentJobResponseTypeDef",
     "ListDeploymentJobsResponseTypeDef",
     "DescribeWorldGenerationJobResponseTypeDef",
+    "RobotApplicationConfigOutputTypeDef",
+    "SimulationApplicationConfigOutputTypeDef",
     "RobotApplicationConfigTypeDef",
     "SimulationApplicationConfigTypeDef",
-    "CreateSimulationJobRequestRequestTypeDef",
     "CreateSimulationJobResponseTypeDef",
     "DescribeSimulationJobResponseTypeDef",
-    "SimulationJobRequestTypeDef",
+    "SimulationJobRequestOutputTypeDef",
     "SimulationJobTypeDef",
+    "CreateSimulationJobRequestRequestTypeDef",
+    "SimulationJobRequestTypeDef",
     "FailedCreateSimulationJobRequestTypeDef",
-    "StartSimulationJobBatchRequestRequestTypeDef",
     "BatchDescribeSimulationJobResponseTypeDef",
+    "StartSimulationJobBatchRequestRequestTypeDef",
     "DescribeSimulationJobBatchResponseTypeDef",
     "StartSimulationJobBatchResponseTypeDef",
 )
 
 BatchDeleteWorldsRequestRequestTypeDef = TypedDict(
     "BatchDeleteWorldsRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
     },
 )
 
-BatchDeleteWorldsResponseTypeDef = TypedDict(
-    "BatchDeleteWorldsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "unprocessedWorlds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BatchDescribeSimulationJobRequestRequestTypeDef = TypedDict(
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     {
         "jobs": Sequence[str],
     },
 )
 
+BatchPolicyOutputTypeDef = TypedDict(
+    "BatchPolicyOutputTypeDef",
+    {
+        "timeoutInSeconds": int,
+        "maxConcurrency": int,
+    },
+    total=False,
+)
+
 BatchPolicyTypeDef = TypedDict(
     "BatchPolicyTypeDef",
     {
         "timeoutInSeconds": int,
         "maxConcurrency": int,
     },
     total=False,
@@ -277,14 +313,24 @@
 CancelWorldGenerationJobRequestRequestTypeDef = TypedDict(
     "CancelWorldGenerationJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
+ComputeOutputTypeDef = TypedDict(
+    "ComputeOutputTypeDef",
+    {
+        "simulationUnitLimit": int,
+        "computeType": ComputeTypeType,
+        "gpuUnitLimit": int,
+    },
+    total=False,
+)
+
 ComputeResponseTypeDef = TypedDict(
     "ComputeResponseTypeDef",
     {
         "simulationUnitLimit": int,
         "computeType": ComputeTypeType,
         "gpuUnitLimit": int,
     },
@@ -316,25 +362,14 @@
 )
 
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "uri": str,
     },
     total=False,
 )
@@ -354,14 +389,31 @@
         "s3Bucket": str,
         "s3Key": str,
         "architecture": ArchitectureType,
     },
     total=False,
 )
 
+EnvironmentOutputTypeDef = TypedDict(
+    "EnvironmentOutputTypeDef",
+    {
+        "uri": str,
+    },
+    total=False,
+)
+
+RobotSoftwareSuiteOutputTypeDef = TypedDict(
+    "RobotSoftwareSuiteOutputTypeDef",
+    {
+        "name": RobotSoftwareSuiteTypeType,
+        "version": RobotSoftwareSuiteVersionTypeType,
+    },
+    total=False,
+)
+
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
         "etag": str,
         "architecture": ArchitectureType,
@@ -408,27 +460,14 @@
 )
 
 class CreateRobotRequestRequestTypeDef(
     _RequiredCreateRobotRequestRequestTypeDef, _OptionalCreateRobotRequestRequestTypeDef
 ):
     pass
 
-CreateRobotResponseTypeDef = TypedDict(
-    "CreateRobotResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "createdAt": datetime,
-        "greengrassGroupId": str,
-        "architecture": ArchitectureType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RenderingEngineTypeDef = TypedDict(
     "RenderingEngineTypeDef",
     {
         "name": Literal["OGRE"],
         "version": str,
     },
     total=False,
@@ -439,14 +478,32 @@
     {
         "name": SimulationSoftwareSuiteTypeType,
         "version": str,
     },
     total=False,
 )
 
+RenderingEngineOutputTypeDef = TypedDict(
+    "RenderingEngineOutputTypeDef",
+    {
+        "name": Literal["OGRE"],
+        "version": str,
+    },
+    total=False,
+)
+
+SimulationSoftwareSuiteOutputTypeDef = TypedDict(
+    "SimulationSoftwareSuiteOutputTypeDef",
+    {
+        "name": SimulationSoftwareSuiteTypeType,
+        "version": str,
+    },
+    total=False,
+)
+
 _RequiredCreateSimulationApplicationVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSimulationApplicationVersionRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalCreateSimulationApplicationVersionRequestRequestTypeDef = TypedDict(
@@ -516,14 +573,31 @@
     },
     total=False,
 )
 
 class VPCConfigTypeDef(_RequiredVPCConfigTypeDef, _OptionalVPCConfigTypeDef):
     pass
 
+LoggingConfigOutputTypeDef = TypedDict(
+    "LoggingConfigOutputTypeDef",
+    {
+        "recordAllRosTopics": bool,
+    },
+    total=False,
+)
+
+OutputLocationOutputTypeDef = TypedDict(
+    "OutputLocationOutputTypeDef",
+    {
+        "s3Bucket": str,
+        "s3Prefix": str,
+    },
+    total=False,
+)
+
 VPCConfigResponseTypeDef = TypedDict(
     "VPCConfigResponseTypeDef",
     {
         "subnets": List[str],
         "securityGroups": List[str],
         "vpcId": str,
         "assignPublicIp": bool,
@@ -536,34 +610,53 @@
     {
         "floorplanCount": int,
         "interiorCountPerFloorplan": int,
     },
     total=False,
 )
 
+WorldCountOutputTypeDef = TypedDict(
+    "WorldCountOutputTypeDef",
+    {
+        "floorplanCount": int,
+        "interiorCountPerFloorplan": int,
+    },
+    total=False,
+)
+
 TemplateLocationTypeDef = TypedDict(
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
 
-CreateWorldTemplateResponseTypeDef = TypedDict(
-    "CreateWorldTemplateResponseTypeDef",
+_RequiredDataSourceConfigOutputTypeDef = TypedDict(
+    "_RequiredDataSourceConfigOutputTypeDef",
     {
-        "arn": str,
-        "clientRequestToken": str,
-        "createdAt": datetime,
         "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "s3Bucket": str,
+        "s3Keys": List[str],
+    },
+)
+_OptionalDataSourceConfigOutputTypeDef = TypedDict(
+    "_OptionalDataSourceConfigOutputTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
     },
+    total=False,
 )
 
+class DataSourceConfigOutputTypeDef(
+    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
+):
+    pass
+
 S3KeyOutputTypeDef = TypedDict(
     "S3KeyOutputTypeDef",
     {
         "s3Key": str,
         "etag": str,
     },
     total=False,
@@ -626,14 +719,36 @@
 DeleteWorldTemplateRequestRequestTypeDef = TypedDict(
     "DeleteWorldTemplateRequestRequestTypeDef",
     {
         "template": str,
     },
 )
 
+_RequiredDeploymentLaunchConfigOutputTypeDef = TypedDict(
+    "_RequiredDeploymentLaunchConfigOutputTypeDef",
+    {
+        "packageName": str,
+        "launchFile": str,
+    },
+)
+_OptionalDeploymentLaunchConfigOutputTypeDef = TypedDict(
+    "_OptionalDeploymentLaunchConfigOutputTypeDef",
+    {
+        "preLaunchFile": str,
+        "postLaunchFile": str,
+        "environmentVariables": Dict[str, str],
+    },
+    total=False,
+)
+
+class DeploymentLaunchConfigOutputTypeDef(
+    _RequiredDeploymentLaunchConfigOutputTypeDef, _OptionalDeploymentLaunchConfigOutputTypeDef
+):
+    pass
+
 _RequiredDeploymentLaunchConfigTypeDef = TypedDict(
     "_RequiredDeploymentLaunchConfigTypeDef",
     {
         "packageName": str,
         "launchFile": str,
     },
 )
@@ -648,14 +763,32 @@
 )
 
 class DeploymentLaunchConfigTypeDef(
     _RequiredDeploymentLaunchConfigTypeDef, _OptionalDeploymentLaunchConfigTypeDef
 ):
     pass
 
+_RequiredS3ObjectOutputTypeDef = TypedDict(
+    "_RequiredS3ObjectOutputTypeDef",
+    {
+        "bucket": str,
+        "key": str,
+    },
+)
+_OptionalS3ObjectOutputTypeDef = TypedDict(
+    "_OptionalS3ObjectOutputTypeDef",
+    {
+        "etag": str,
+    },
+    total=False,
+)
+
+class S3ObjectOutputTypeDef(_RequiredS3ObjectOutputTypeDef, _OptionalS3ObjectOutputTypeDef):
+    pass
+
 _RequiredS3ObjectTypeDef = TypedDict(
     "_RequiredS3ObjectTypeDef",
     {
         "bucket": str,
         "key": str,
     },
 )
@@ -674,23 +807,14 @@
     "DeregisterRobotRequestRequestTypeDef",
     {
         "fleet": str,
         "robot": str,
     },
 )
 
-DeregisterRobotResponseTypeDef = TypedDict(
-    "DeregisterRobotResponseTypeDef",
-    {
-        "fleet": str,
-        "robot": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeploymentJobRequestRequestTypeDef = TypedDict(
     "DescribeDeploymentJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
@@ -740,31 +864,14 @@
 DescribeRobotRequestRequestTypeDef = TypedDict(
     "DescribeRobotRequestRequestTypeDef",
     {
         "robot": str,
     },
 )
 
-DescribeRobotResponseTypeDef = TypedDict(
-    "DescribeRobotResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "fleetArn": str,
-        "status": RobotStatusType,
-        "greengrassGroupId": str,
-        "createdAt": datetime,
-        "architecture": ArchitectureType,
-        "lastDeploymentJob": str,
-        "lastDeploymentTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSimulationApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalDescribeSimulationApplicationRequestRequestTypeDef = TypedDict(
@@ -837,48 +944,21 @@
 DescribeWorldRequestRequestTypeDef = TypedDict(
     "DescribeWorldRequestRequestTypeDef",
     {
         "world": str,
     },
 )
 
-DescribeWorldResponseTypeDef = TypedDict(
-    "DescribeWorldResponseTypeDef",
-    {
-        "arn": str,
-        "generationJob": str,
-        "template": str,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-        "worldDescriptionBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeWorldTemplateRequestRequestTypeDef = TypedDict(
     "DescribeWorldTemplateRequestRequestTypeDef",
     {
         "template": str,
     },
 )
 
-DescribeWorldTemplateResponseTypeDef = TypedDict(
-    "DescribeWorldTemplateResponseTypeDef",
-    {
-        "arn": str,
-        "clientRequestToken": str,
-        "name": str,
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "tags": Dict[str, str],
-        "version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorldFailureTypeDef = TypedDict(
     "WorldFailureTypeDef",
     {
         "failureCode": WorldGenerationJobErrorCodeType,
         "sampleFailureReason": str,
         "failureCount": int,
     },
@@ -912,20 +992,22 @@
     {
         "template": str,
         "generationJob": str,
     },
     total=False,
 )
 
-GetWorldTemplateBodyResponseTypeDef = TypedDict(
-    "GetWorldTemplateBodyResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "templateBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
 SimulationJobBatchSummaryTypeDef = TypedDict(
     "SimulationJobBatchSummaryTypeDef",
     {
         "arn": str,
         "lastUpdatedAt": datetime,
@@ -941,30 +1023,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = TypedDict(
-    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorldTemplatesRequestRequestTypeDef = TypedDict(
     "ListWorldTemplatesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -989,24 +1055,34 @@
         "createdAt": datetime,
         "generationJob": str,
         "template": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredPortMappingOutputTypeDef = TypedDict(
+    "_RequiredPortMappingOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "jobPort": int,
+        "applicationPort": int,
+    },
+)
+_OptionalPortMappingOutputTypeDef = TypedDict(
+    "_OptionalPortMappingOutputTypeDef",
+    {
+        "enableOnPublicIp": bool,
     },
     total=False,
 )
 
+class PortMappingOutputTypeDef(
+    _RequiredPortMappingOutputTypeDef, _OptionalPortMappingOutputTypeDef
+):
+    pass
+
 _RequiredPortMappingTypeDef = TypedDict(
     "_RequiredPortMappingTypeDef",
     {
         "jobPort": int,
         "applicationPort": int,
     },
 )
@@ -1036,38 +1112,47 @@
     "RegisterRobotRequestRequestTypeDef",
     {
         "fleet": str,
         "robot": str,
     },
 )
 
-RegisterRobotResponseTypeDef = TypedDict(
-    "RegisterRobotResponseTypeDef",
+RestartSimulationJobRequestRequestTypeDef = TypedDict(
+    "RestartSimulationJobRequestRequestTypeDef",
     {
-        "fleet": str,
-        "robot": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "job": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredToolOutputTypeDef = TypedDict(
+    "_RequiredToolOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "name": str,
+        "command": str,
+    },
+)
+_OptionalToolOutputTypeDef = TypedDict(
+    "_OptionalToolOutputTypeDef",
+    {
+        "streamUI": bool,
+        "streamOutputToCloudWatch": bool,
+        "exitBehavior": ExitBehaviorType,
     },
+    total=False,
 )
 
-RestartSimulationJobRequestRequestTypeDef = TypedDict(
-    "RestartSimulationJobRequestRequestTypeDef",
+class ToolOutputTypeDef(_RequiredToolOutputTypeDef, _OptionalToolOutputTypeDef):
+    pass
+
+UploadConfigurationOutputTypeDef = TypedDict(
+    "UploadConfigurationOutputTypeDef",
     {
-        "job": str,
+        "name": str,
+        "path": str,
+        "uploadBehavior": UploadBehaviorType,
     },
 )
 
 _RequiredToolTypeDef = TypedDict(
     "_RequiredToolTypeDef",
     {
         "name": str,
@@ -1092,22 +1177,48 @@
     {
         "name": str,
         "path": str,
         "uploadBehavior": UploadBehaviorType,
     },
 )
 
+WorldConfigOutputTypeDef = TypedDict(
+    "WorldConfigOutputTypeDef",
+    {
+        "world": str,
+    },
+    total=False,
+)
+
 WorldConfigTypeDef = TypedDict(
     "WorldConfigTypeDef",
     {
         "world": str,
     },
     total=False,
 )
 
+_RequiredVPCConfigOutputTypeDef = TypedDict(
+    "_RequiredVPCConfigOutputTypeDef",
+    {
+        "subnets": List[str],
+    },
+)
+_OptionalVPCConfigOutputTypeDef = TypedDict(
+    "_OptionalVPCConfigOutputTypeDef",
+    {
+        "securityGroups": List[str],
+        "assignPublicIp": bool,
+    },
+    total=False,
+)
+
+class VPCConfigOutputTypeDef(_RequiredVPCConfigOutputTypeDef, _OptionalVPCConfigOutputTypeDef):
+    pass
+
 SyncDeploymentJobRequestRequestTypeDef = TypedDict(
     "SyncDeploymentJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
         "fleet": str,
     },
 )
@@ -1124,35 +1235,145 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateWorldTemplateResponseTypeDef = TypedDict(
-    "UpdateWorldTemplateResponseTypeDef",
+BatchDeleteWorldsResponseTypeDef = TypedDict(
+    "BatchDeleteWorldsResponseTypeDef",
+    {
+        "unprocessedWorlds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RobotApplicationSummaryTypeDef = TypedDict(
-    "RobotApplicationSummaryTypeDef",
+CreateRobotResponseTypeDef = TypedDict(
+    "CreateRobotResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "createdAt": datetime,
+        "greengrassGroupId": str,
+        "architecture": ArchitectureType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorldTemplateResponseTypeDef = TypedDict(
+    "CreateWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "clientRequestToken": str,
+        "createdAt": datetime,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterRobotResponseTypeDef = TypedDict(
+    "DeregisterRobotResponseTypeDef",
+    {
+        "fleet": str,
+        "robot": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRobotResponseTypeDef = TypedDict(
+    "DescribeRobotResponseTypeDef",
     {
+        "arn": str,
         "name": str,
+        "fleetArn": str,
+        "status": RobotStatusType,
+        "greengrassGroupId": str,
+        "createdAt": datetime,
+        "architecture": ArchitectureType,
+        "lastDeploymentJob": str,
+        "lastDeploymentTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorldResponseTypeDef = TypedDict(
+    "DescribeWorldResponseTypeDef",
+    {
+        "arn": str,
+        "generationJob": str,
+        "template": str,
+        "createdAt": datetime,
+        "tags": Dict[str, str],
+        "worldDescriptionBody": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorldTemplateResponseTypeDef = TypedDict(
+    "DescribeWorldTemplateResponseTypeDef",
+    {
         "arn": str,
+        "clientRequestToken": str,
+        "name": str,
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "tags": Dict[str, str],
         "version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorldTemplateBodyResponseTypeDef = TypedDict(
+    "GetWorldTemplateBodyResponseTypeDef",
+    {
+        "templateBody": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterRobotResponseTypeDef = TypedDict(
+    "RegisterRobotResponseTypeDef",
+    {
+        "fleet": str,
+        "robot": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorldTemplateResponseTypeDef = TypedDict(
+    "UpdateWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "createdAt": datetime,
         "lastUpdatedAt": datetime,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateRobotApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRobotApplicationRequestRequestTypeDef",
     {
         "name": str,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
@@ -1193,74 +1414,86 @@
 
 class UpdateRobotApplicationRequestRequestTypeDef(
     _RequiredUpdateRobotApplicationRequestRequestTypeDef,
     _OptionalUpdateRobotApplicationRequestRequestTypeDef,
 ):
     pass
 
+RobotApplicationSummaryTypeDef = TypedDict(
+    "RobotApplicationSummaryTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "version": str,
+        "lastUpdatedAt": datetime,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+    },
+    total=False,
+)
+
 CreateRobotApplicationResponseTypeDef = TypedDict(
     "CreateRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
-        "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "environment": EnvironmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRobotApplicationVersionResponseTypeDef = TypedDict(
     "CreateRobotApplicationVersionResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "environment": EnvironmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRobotApplicationResponseTypeDef = TypedDict(
     "DescribeRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "imageDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRobotApplicationResponseTypeDef = TypedDict(
     "UpdateRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "environment": EnvironmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSimulationApplicationRequestRequestTypeDef",
     {
         "name": str,
@@ -1281,120 +1514,120 @@
 
 class CreateSimulationApplicationRequestRequestTypeDef(
     _RequiredCreateSimulationApplicationRequestRequestTypeDef,
     _OptionalCreateSimulationApplicationRequestRequestTypeDef,
 ):
     pass
 
+_RequiredUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSimulationApplicationRequestRequestTypeDef",
+    {
+        "application": str,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
+    },
+)
+_OptionalUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSimulationApplicationRequestRequestTypeDef",
+    {
+        "sources": Sequence[SourceConfigTypeDef],
+        "renderingEngine": RenderingEngineTypeDef,
+        "currentRevisionId": str,
+        "environment": EnvironmentTypeDef,
+    },
+    total=False,
+)
+
+class UpdateSimulationApplicationRequestRequestTypeDef(
+    _RequiredUpdateSimulationApplicationRequestRequestTypeDef,
+    _OptionalUpdateSimulationApplicationRequestRequestTypeDef,
+):
+    pass
+
 CreateSimulationApplicationResponseTypeDef = TypedDict(
     "CreateSimulationApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-        "renderingEngine": RenderingEngineTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "renderingEngine": RenderingEngineOutputTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
-        "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "environment": EnvironmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSimulationApplicationVersionResponseTypeDef = TypedDict(
     "CreateSimulationApplicationVersionResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-        "renderingEngine": RenderingEngineTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "renderingEngine": RenderingEngineOutputTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "environment": EnvironmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationApplicationResponseTypeDef = TypedDict(
     "DescribeSimulationApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-        "renderingEngine": RenderingEngineTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "renderingEngine": RenderingEngineOutputTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
-        "environment": EnvironmentTypeDef,
+        "environment": EnvironmentOutputTypeDef,
         "imageDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SimulationApplicationSummaryTypeDef = TypedDict(
     "SimulationApplicationSummaryTypeDef",
     {
         "name": str,
         "arn": str,
         "version": str,
         "lastUpdatedAt": datetime,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSimulationApplicationRequestRequestTypeDef",
-    {
-        "application": str,
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-    },
-)
-_OptionalUpdateSimulationApplicationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSimulationApplicationRequestRequestTypeDef",
-    {
-        "sources": Sequence[SourceConfigTypeDef],
-        "renderingEngine": RenderingEngineTypeDef,
-        "currentRevisionId": str,
-        "environment": EnvironmentTypeDef,
-    },
-    total=False,
-)
-
-class UpdateSimulationApplicationRequestRequestTypeDef(
-    _RequiredUpdateSimulationApplicationRequestRequestTypeDef,
-    _OptionalUpdateSimulationApplicationRequestRequestTypeDef,
-):
-    pass
-
 UpdateSimulationApplicationResponseTypeDef = TypedDict(
     "UpdateSimulationApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
-        "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
-        "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
-        "renderingEngine": RenderingEngineTypeDef,
+        "simulationSoftwareSuite": SimulationSoftwareSuiteOutputTypeDef,
+        "robotSoftwareSuite": RobotSoftwareSuiteOutputTypeDef,
+        "renderingEngine": RenderingEngineOutputTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
-        "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "environment": EnvironmentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWorldExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorldExportJobRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
@@ -1421,46 +1654,46 @@
     "CreateWorldExportJobResponseTypeDef",
     {
         "arn": str,
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldExportJobErrorCodeType,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorldExportJobResponseTypeDef = TypedDict(
     "DescribeWorldExportJobResponseTypeDef",
     {
         "arn": str,
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldExportJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
         "worlds": List[str],
-        "outputLocation": OutputLocationTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorldExportJobSummaryTypeDef = TypedDict(
     "WorldExportJobSummaryTypeDef",
     {
         "arn": str,
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "worlds": List[str],
-        "outputLocation": OutputLocationTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateWorldGenerationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorldGenerationJobRequestRequestTypeDef",
     {
@@ -1489,29 +1722,29 @@
     {
         "arn": str,
         "status": WorldGenerationJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldGenerationJobErrorCodeType,
         "clientRequestToken": str,
         "template": str,
-        "worldCount": WorldCountTypeDef,
+        "worldCount": WorldCountOutputTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorldGenerationJobSummaryTypeDef = TypedDict(
     "WorldGenerationJobSummaryTypeDef",
     {
         "arn": str,
         "template": str,
         "createdAt": datetime,
         "status": WorldGenerationJobStatusType,
-        "worldCount": WorldCountTypeDef,
+        "worldCount": WorldCountOutputTypeDef,
         "succeededWorldCount": int,
         "failedWorldCount": int,
     },
     total=False,
 )
 
 CreateWorldTemplateRequestRequestTypeDef = TypedDict(
@@ -1556,23 +1789,43 @@
         "s3Keys": List[S3KeyOutputTypeDef],
         "type": DataSourceTypeType,
         "destination": str,
     },
     total=False,
 )
 
+DeploymentApplicationConfigOutputTypeDef = TypedDict(
+    "DeploymentApplicationConfigOutputTypeDef",
+    {
+        "application": str,
+        "applicationVersion": str,
+        "launchConfig": DeploymentLaunchConfigOutputTypeDef,
+    },
+)
+
 DeploymentApplicationConfigTypeDef = TypedDict(
     "DeploymentApplicationConfigTypeDef",
     {
         "application": str,
         "applicationVersion": str,
         "launchConfig": DeploymentLaunchConfigTypeDef,
     },
 )
 
+DeploymentConfigOutputTypeDef = TypedDict(
+    "DeploymentConfigOutputTypeDef",
+    {
+        "concurrentDeploymentPercentage": int,
+        "failureThresholdPercentage": int,
+        "robotDeploymentTimeoutInSeconds": int,
+        "downloadConditionFile": S3ObjectOutputTypeDef,
+    },
+    total=False,
+)
+
 DeploymentConfigTypeDef = TypedDict(
     "DeploymentConfigTypeDef",
     {
         "concurrentDeploymentPercentage": int,
         "failureThresholdPercentage": int,
         "robotDeploymentTimeoutInSeconds": int,
         "downloadConditionFile": S3ObjectTypeDef,
@@ -1587,279 +1840,295 @@
         "arn": str,
         "robots": List[RobotTypeDef],
         "createdAt": datetime,
         "lastDeploymentStatus": DeploymentStatusType,
         "lastDeploymentJob": str,
         "lastDeploymentTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRobotsResponseTypeDef = TypedDict(
     "ListRobotsResponseTypeDef",
     {
         "robots": List[RobotTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSimulationJobsResponseTypeDef = TypedDict(
     "ListSimulationJobsResponseTypeDef",
     {
         "simulationJobSummaries": List[SimulationJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailureSummaryTypeDef = TypedDict(
     "FailureSummaryTypeDef",
     {
         "totalFailureCount": int,
         "failures": List[WorldFailureTypeDef],
     },
     total=False,
 )
 
-ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = TypedDict(
-    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
+ListDeploymentJobsRequestRequestTypeDef = TypedDict(
+    "ListDeploymentJobsRequestRequestTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-ListDeploymentJobsRequestRequestTypeDef = TypedDict(
-    "ListDeploymentJobsRequestRequestTypeDef",
+ListFleetsRequestRequestTypeDef = TypedDict(
+    "ListFleetsRequestRequestTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
         "nextToken": str,
         "maxResults": int,
+        "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
-    "ListFleetsRequestListFleetsPaginateTypeDef",
+ListRobotApplicationsRequestRequestTypeDef = TypedDict(
+    "ListRobotApplicationsRequestRequestTypeDef",
     {
+        "versionQualifier": str,
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListFleetsRequestRequestTypeDef = TypedDict(
-    "ListFleetsRequestRequestTypeDef",
+ListRobotsRequestRequestTypeDef = TypedDict(
+    "ListRobotsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = TypedDict(
-    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
+ListSimulationApplicationsRequestRequestTypeDef = TypedDict(
+    "ListSimulationApplicationsRequestRequestTypeDef",
     {
         "versionQualifier": str,
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListRobotApplicationsRequestRequestTypeDef = TypedDict(
-    "ListRobotApplicationsRequestRequestTypeDef",
+ListSimulationJobBatchesRequestRequestTypeDef = TypedDict(
+    "ListSimulationJobBatchesRequestRequestTypeDef",
     {
-        "versionQualifier": str,
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListRobotsRequestListRobotsPaginateTypeDef = TypedDict(
-    "ListRobotsRequestListRobotsPaginateTypeDef",
+ListSimulationJobsRequestRequestTypeDef = TypedDict(
+    "ListSimulationJobsRequestRequestTypeDef",
     {
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListRobotsRequestRequestTypeDef = TypedDict(
-    "ListRobotsRequestRequestTypeDef",
+ListWorldExportJobsRequestRequestTypeDef = TypedDict(
+    "ListWorldExportJobsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = TypedDict(
-    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
+ListWorldGenerationJobsRequestRequestTypeDef = TypedDict(
+    "ListWorldGenerationJobsRequestRequestTypeDef",
     {
-        "versionQualifier": str,
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListSimulationApplicationsRequestRequestTypeDef = TypedDict(
-    "ListSimulationApplicationsRequestRequestTypeDef",
+ListWorldsRequestRequestTypeDef = TypedDict(
+    "ListWorldsRequestRequestTypeDef",
     {
-        "versionQualifier": str,
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = TypedDict(
-    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
+ListFleetsResponseTypeDef = TypedDict(
+    "ListFleetsResponseTypeDef",
+    {
+        "fleetDetails": List[FleetTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = TypedDict(
+    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobBatchesRequestRequestTypeDef = TypedDict(
-    "ListSimulationJobBatchesRequestRequestTypeDef",
+ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
+    "ListFleetsRequestListFleetsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = TypedDict(
-    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
+ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = TypedDict(
+    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
     {
+        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobsRequestRequestTypeDef = TypedDict(
-    "ListSimulationJobsRequestRequestTypeDef",
+ListRobotsRequestListRobotsPaginateTypeDef = TypedDict(
+    "ListRobotsRequestListRobotsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = TypedDict(
-    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
+ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = TypedDict(
+    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
     {
+        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldExportJobsRequestRequestTypeDef = TypedDict(
-    "ListWorldExportJobsRequestRequestTypeDef",
+ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = TypedDict(
+    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = TypedDict(
-    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
+ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = TypedDict(
+    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldGenerationJobsRequestRequestTypeDef = TypedDict(
-    "ListWorldGenerationJobsRequestRequestTypeDef",
+ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = TypedDict(
+    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldsRequestListWorldsPaginateTypeDef = TypedDict(
-    "ListWorldsRequestListWorldsPaginateTypeDef",
+ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = TypedDict(
+    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldsRequestRequestTypeDef = TypedDict(
-    "ListWorldsRequestRequestTypeDef",
+ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = TypedDict(
+    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
-        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListFleetsResponseTypeDef = TypedDict(
-    "ListFleetsResponseTypeDef",
+ListWorldsRequestListWorldsPaginateTypeDef = TypedDict(
+    "ListWorldsRequestListWorldsPaginateTypeDef",
     {
-        "fleetDetails": List[FleetTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListSimulationJobBatchesResponseTypeDef = TypedDict(
     "ListSimulationJobBatchesResponseTypeDef",
     {
         "simulationJobBatchSummaries": List[SimulationJobBatchSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldTemplatesResponseTypeDef = TypedDict(
     "ListWorldTemplatesResponseTypeDef",
     {
         "templateSummaries": List[TemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldsResponseTypeDef = TypedDict(
     "ListWorldsResponseTypeDef",
     {
         "worldSummaries": List[WorldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PortForwardingConfigOutputTypeDef = TypedDict(
+    "PortForwardingConfigOutputTypeDef",
+    {
+        "portMappings": List[PortMappingOutputTypeDef],
     },
+    total=False,
 )
 
 PortForwardingConfigTypeDef = TypedDict(
     "PortForwardingConfigTypeDef",
     {
-        "portMappings": List[PortMappingTypeDef],
+        "portMappings": Sequence[PortMappingTypeDef],
     },
     total=False,
 )
 
 RobotDeploymentTypeDef = TypedDict(
     "RobotDeploymentTypeDef",
     {
@@ -1875,195 +2144,258 @@
 )
 
 ListRobotApplicationsResponseTypeDef = TypedDict(
     "ListRobotApplicationsResponseTypeDef",
     {
         "robotApplicationSummaries": List[RobotApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSimulationApplicationsResponseTypeDef = TypedDict(
     "ListSimulationApplicationsResponseTypeDef",
     {
         "simulationApplicationSummaries": List[SimulationApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldExportJobsResponseTypeDef = TypedDict(
     "ListWorldExportJobsResponseTypeDef",
     {
         "worldExportJobSummaries": List[WorldExportJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldGenerationJobsResponseTypeDef = TypedDict(
     "ListWorldGenerationJobsResponseTypeDef",
     {
         "worldGenerationJobSummaries": List[WorldGenerationJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "fleet": str,
-        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
-    },
-)
-_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDeploymentJobRequestRequestTypeDef(
-    _RequiredCreateDeploymentJobRequestRequestTypeDef,
-    _OptionalCreateDeploymentJobRequestRequestTypeDef,
-):
-    pass
-
 CreateDeploymentJobResponseTypeDef = TypedDict(
     "CreateDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
-        "deploymentConfig": DeploymentConfigTypeDef,
+        "deploymentConfig": DeploymentConfigOutputTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentJobTypeDef = TypedDict(
     "DeploymentJobTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
-        "deploymentConfig": DeploymentConfigTypeDef,
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
+        "deploymentConfig": DeploymentConfigOutputTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
     },
     total=False,
 )
 
 SyncDeploymentJobResponseTypeDef = TypedDict(
     "SyncDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentConfig": DeploymentConfigOutputTypeDef,
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "fleet": str,
+        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
     },
 )
+_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "deploymentConfig": DeploymentConfigTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDeploymentJobRequestRequestTypeDef(
+    _RequiredCreateDeploymentJobRequestRequestTypeDef,
+    _OptionalCreateDeploymentJobRequestRequestTypeDef,
+):
+    pass
 
 FinishedWorldsSummaryTypeDef = TypedDict(
     "FinishedWorldsSummaryTypeDef",
     {
         "finishedCount": int,
         "succeededWorlds": List[str],
         "failureSummary": FailureSummaryTypeDef,
     },
     total=False,
 )
 
+LaunchConfigOutputTypeDef = TypedDict(
+    "LaunchConfigOutputTypeDef",
+    {
+        "packageName": str,
+        "launchFile": str,
+        "environmentVariables": Dict[str, str],
+        "portForwardingConfig": PortForwardingConfigOutputTypeDef,
+        "streamUI": bool,
+        "command": List[str],
+    },
+    total=False,
+)
+
 LaunchConfigTypeDef = TypedDict(
     "LaunchConfigTypeDef",
     {
         "packageName": str,
         "launchFile": str,
-        "environmentVariables": Dict[str, str],
+        "environmentVariables": Mapping[str, str],
         "portForwardingConfig": PortForwardingConfigTypeDef,
         "streamUI": bool,
-        "command": List[str],
+        "command": Sequence[str],
     },
     total=False,
 )
 
 DescribeDeploymentJobResponseTypeDef = TypedDict(
     "DescribeDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentConfig": DeploymentConfigOutputTypeDef,
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "robotDeploymentSummary": List[RobotDeploymentTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeploymentJobsResponseTypeDef = TypedDict(
     "ListDeploymentJobsResponseTypeDef",
     {
         "deploymentJobs": List[DeploymentJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorldGenerationJobResponseTypeDef = TypedDict(
     "DescribeWorldGenerationJobResponseTypeDef",
     {
         "arn": str,
         "status": WorldGenerationJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldGenerationJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
         "template": str,
-        "worldCount": WorldCountTypeDef,
+        "worldCount": WorldCountOutputTypeDef,
         "finishedWorldsSummary": FinishedWorldsSummaryTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredRobotApplicationConfigOutputTypeDef = TypedDict(
+    "_RequiredRobotApplicationConfigOutputTypeDef",
+    {
+        "application": str,
+        "launchConfig": LaunchConfigOutputTypeDef,
+    },
+)
+_OptionalRobotApplicationConfigOutputTypeDef = TypedDict(
+    "_OptionalRobotApplicationConfigOutputTypeDef",
+    {
+        "applicationVersion": str,
+        "uploadConfigurations": List[UploadConfigurationOutputTypeDef],
+        "useDefaultUploadConfigurations": bool,
+        "tools": List[ToolOutputTypeDef],
+        "useDefaultTools": bool,
+    },
+    total=False,
+)
+
+class RobotApplicationConfigOutputTypeDef(
+    _RequiredRobotApplicationConfigOutputTypeDef, _OptionalRobotApplicationConfigOutputTypeDef
+):
+    pass
+
+_RequiredSimulationApplicationConfigOutputTypeDef = TypedDict(
+    "_RequiredSimulationApplicationConfigOutputTypeDef",
+    {
+        "application": str,
+        "launchConfig": LaunchConfigOutputTypeDef,
     },
 )
+_OptionalSimulationApplicationConfigOutputTypeDef = TypedDict(
+    "_OptionalSimulationApplicationConfigOutputTypeDef",
+    {
+        "applicationVersion": str,
+        "uploadConfigurations": List[UploadConfigurationOutputTypeDef],
+        "worldConfigs": List[WorldConfigOutputTypeDef],
+        "useDefaultUploadConfigurations": bool,
+        "tools": List[ToolOutputTypeDef],
+        "useDefaultTools": bool,
+    },
+    total=False,
+)
+
+class SimulationApplicationConfigOutputTypeDef(
+    _RequiredSimulationApplicationConfigOutputTypeDef,
+    _OptionalSimulationApplicationConfigOutputTypeDef,
+):
+    pass
 
 _RequiredRobotApplicationConfigTypeDef = TypedDict(
     "_RequiredRobotApplicationConfigTypeDef",
     {
         "application": str,
         "launchConfig": LaunchConfigTypeDef,
     },
 )
 _OptionalRobotApplicationConfigTypeDef = TypedDict(
     "_OptionalRobotApplicationConfigTypeDef",
     {
         "applicationVersion": str,
-        "uploadConfigurations": List[UploadConfigurationTypeDef],
+        "uploadConfigurations": Sequence[UploadConfigurationTypeDef],
         "useDefaultUploadConfigurations": bool,
-        "tools": List[ToolTypeDef],
+        "tools": Sequence[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
 class RobotApplicationConfigTypeDef(
     _RequiredRobotApplicationConfigTypeDef, _OptionalRobotApplicationConfigTypeDef
@@ -2077,80 +2409,50 @@
         "launchConfig": LaunchConfigTypeDef,
     },
 )
 _OptionalSimulationApplicationConfigTypeDef = TypedDict(
     "_OptionalSimulationApplicationConfigTypeDef",
     {
         "applicationVersion": str,
-        "uploadConfigurations": List[UploadConfigurationTypeDef],
-        "worldConfigs": List[WorldConfigTypeDef],
+        "uploadConfigurations": Sequence[UploadConfigurationTypeDef],
+        "worldConfigs": Sequence[WorldConfigTypeDef],
         "useDefaultUploadConfigurations": bool,
-        "tools": List[ToolTypeDef],
+        "tools": Sequence[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
 class SimulationApplicationConfigTypeDef(
     _RequiredSimulationApplicationConfigTypeDef, _OptionalSimulationApplicationConfigTypeDef
 ):
     pass
 
-_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSimulationJobRequestRequestTypeDef",
-    {
-        "maxJobDurationInSeconds": int,
-        "iamRole": str,
-    },
-)
-_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSimulationJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
-        "failureBehavior": FailureBehaviorType,
-        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
-        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
-        "dataSources": Sequence[DataSourceConfigTypeDef],
-        "tags": Mapping[str, str],
-        "vpcConfig": VPCConfigTypeDef,
-        "compute": ComputeTypeDef,
-    },
-    total=False,
-)
-
-class CreateSimulationJobRequestRequestTypeDef(
-    _RequiredCreateSimulationJobRequestRequestTypeDef,
-    _OptionalCreateSimulationJobRequestRequestTypeDef,
-):
-    pass
-
 CreateSimulationJobResponseTypeDef = TypedDict(
     "CreateSimulationJobResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobStatusType,
         "lastStartedAt": datetime,
         "lastUpdatedAt": datetime,
         "failureBehavior": FailureBehaviorType,
         "failureCode": SimulationJobErrorCodeType,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
+        "loggingConfig": LoggingConfigOutputTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "compute": ComputeResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationJobResponseTypeDef = TypedDict(
     "DescribeSimulationJobResponseTypeDef",
     {
         "arn": str,
@@ -2158,56 +2460,56 @@
         "status": SimulationJobStatusType,
         "lastStartedAt": datetime,
         "lastUpdatedAt": datetime,
         "failureBehavior": FailureBehaviorType,
         "failureCode": SimulationJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
+        "loggingConfig": LoggingConfigOutputTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSimulationJobRequestTypeDef = TypedDict(
-    "_RequiredSimulationJobRequestTypeDef",
+_RequiredSimulationJobRequestOutputTypeDef = TypedDict(
+    "_RequiredSimulationJobRequestOutputTypeDef",
     {
         "maxJobDurationInSeconds": int,
     },
 )
-_OptionalSimulationJobRequestTypeDef = TypedDict(
-    "_OptionalSimulationJobRequestTypeDef",
+_OptionalSimulationJobRequestOutputTypeDef = TypedDict(
+    "_OptionalSimulationJobRequestOutputTypeDef",
     {
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
+        "loggingConfig": LoggingConfigOutputTypeDef,
         "iamRole": str,
         "failureBehavior": FailureBehaviorType,
         "useDefaultApplications": bool,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
-        "dataSources": List[DataSourceConfigTypeDef],
-        "vpcConfig": VPCConfigTypeDef,
-        "compute": ComputeTypeDef,
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
+        "dataSources": List[DataSourceConfigOutputTypeDef],
+        "vpcConfig": VPCConfigOutputTypeDef,
+        "compute": ComputeOutputTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-class SimulationJobRequestTypeDef(
-    _RequiredSimulationJobRequestTypeDef, _OptionalSimulationJobRequestTypeDef
+class SimulationJobRequestOutputTypeDef(
+    _RequiredSimulationJobRequestOutputTypeDef, _OptionalSimulationJobRequestOutputTypeDef
 ):
     pass
 
 SimulationJobTypeDef = TypedDict(
     "SimulationJobTypeDef",
     {
         "arn": str,
@@ -2215,41 +2517,109 @@
         "status": SimulationJobStatusType,
         "lastStartedAt": datetime,
         "lastUpdatedAt": datetime,
         "failureBehavior": FailureBehaviorType,
         "failureCode": SimulationJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
+        "outputLocation": OutputLocationOutputTypeDef,
+        "loggingConfig": LoggingConfigOutputTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSimulationJobRequestRequestTypeDef",
+    {
+        "maxJobDurationInSeconds": int,
+        "iamRole": str,
+    },
+)
+_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSimulationJobRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
+        "failureBehavior": FailureBehaviorType,
+        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
+        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
+        "dataSources": Sequence[DataSourceConfigTypeDef],
+        "tags": Mapping[str, str],
+        "vpcConfig": VPCConfigTypeDef,
+        "compute": ComputeTypeDef,
+    },
+    total=False,
+)
+
+class CreateSimulationJobRequestRequestTypeDef(
+    _RequiredCreateSimulationJobRequestRequestTypeDef,
+    _OptionalCreateSimulationJobRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSimulationJobRequestTypeDef = TypedDict(
+    "_RequiredSimulationJobRequestTypeDef",
+    {
+        "maxJobDurationInSeconds": int,
+    },
+)
+_OptionalSimulationJobRequestTypeDef = TypedDict(
+    "_OptionalSimulationJobRequestTypeDef",
+    {
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
+        "iamRole": str,
+        "failureBehavior": FailureBehaviorType,
+        "useDefaultApplications": bool,
+        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
+        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
+        "dataSources": Sequence[DataSourceConfigTypeDef],
+        "vpcConfig": VPCConfigTypeDef,
+        "compute": ComputeTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class SimulationJobRequestTypeDef(
+    _RequiredSimulationJobRequestTypeDef, _OptionalSimulationJobRequestTypeDef
+):
+    pass
+
 FailedCreateSimulationJobRequestTypeDef = TypedDict(
     "FailedCreateSimulationJobRequestTypeDef",
     {
-        "request": SimulationJobRequestTypeDef,
+        "request": SimulationJobRequestOutputTypeDef,
         "failureReason": str,
         "failureCode": SimulationJobErrorCodeType,
         "failedAt": datetime,
     },
     total=False,
 )
 
+BatchDescribeSimulationJobResponseTypeDef = TypedDict(
+    "BatchDescribeSimulationJobResponseTypeDef",
+    {
+        "jobs": List[SimulationJobTypeDef],
+        "unprocessedJobs": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
     "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
     {
         "createSimulationJobRequests": Sequence[SimulationJobRequestTypeDef],
     },
 )
 _OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
@@ -2264,52 +2634,43 @@
 
 class StartSimulationJobBatchRequestRequestTypeDef(
     _RequiredStartSimulationJobBatchRequestRequestTypeDef,
     _OptionalStartSimulationJobBatchRequestRequestTypeDef,
 ):
     pass
 
-BatchDescribeSimulationJobResponseTypeDef = TypedDict(
-    "BatchDescribeSimulationJobResponseTypeDef",
-    {
-        "jobs": List[SimulationJobTypeDef],
-        "unprocessedJobs": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSimulationJobBatchResponseTypeDef = TypedDict(
     "DescribeSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "lastUpdatedAt": datetime,
         "createdAt": datetime,
         "clientRequestToken": str,
-        "batchPolicy": BatchPolicyTypeDef,
+        "batchPolicy": BatchPolicyOutputTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
-        "pendingRequests": List[SimulationJobRequestTypeDef],
+        "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSimulationJobBatchResponseTypeDef = TypedDict(
     "StartSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "createdAt": datetime,
         "clientRequestToken": str,
-        "batchPolicy": BatchPolicyTypeDef,
+        "batchPolicy": BatchPolicyOutputTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
-        "pendingRequests": List[SimulationJobRequestTypeDef],
+        "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker.egg-info/PKG-INFO` & `mypy-boto3-robomaker-1.28.12/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-robomaker
-Version: 1.28.0
-Summary: Type annotations for boto3.RoboMaker 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 robomaker type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-robomaker"></a>
 
 # mypy-boto3-robomaker
 
 [![PyPI - mypy-boto3-robomaker](https://img.shields.io/pypi/v/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-robomaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-robomaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-robomaker?color=blue)](https://pypistats.org/packages/mypy-boto3-robomaker)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-robomaker)](https://pepy.tech/project/mypy-boto3-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RoboMaker 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
+[boto3.RoboMaker 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,176 +357,200 @@
 
 `mypy_boto3_robomaker.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
-    BatchDeleteWorldsResponseTypeDef,
+    ResponseMetadataTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
+    BatchPolicyOutputTypeDef,
     BatchPolicyTypeDef,
     CancelDeploymentJobRequestRequestTypeDef,
     CancelSimulationJobBatchRequestRequestTypeDef,
     CancelSimulationJobRequestRequestTypeDef,
     CancelWorldExportJobRequestRequestTypeDef,
     CancelWorldGenerationJobRequestRequestTypeDef,
+    ComputeOutputTypeDef,
     ComputeResponseTypeDef,
     ComputeTypeDef,
     CreateFleetRequestRequestTypeDef,
-    CreateFleetResponseTypeDef,
     EnvironmentTypeDef,
     RobotSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
+    EnvironmentOutputTypeDef,
+    RobotSoftwareSuiteOutputTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
-    CreateRobotResponseTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
+    RenderingEngineOutputTypeDef,
+    SimulationSoftwareSuiteOutputTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
     DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
+    LoggingConfigOutputTypeDef,
+    OutputLocationOutputTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
+    WorldCountOutputTypeDef,
     TemplateLocationTypeDef,
-    CreateWorldTemplateResponseTypeDef,
+    DataSourceConfigOutputTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
+    DeploymentLaunchConfigOutputTypeDef,
     DeploymentLaunchConfigTypeDef,
+    S3ObjectOutputTypeDef,
     S3ObjectTypeDef,
     DeregisterRobotRequestRequestTypeDef,
-    DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobRequestRequestTypeDef,
     DescribeFleetRequestRequestTypeDef,
     RobotTypeDef,
     DescribeRobotApplicationRequestRequestTypeDef,
     DescribeRobotRequestRequestTypeDef,
-    DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationRequestRequestTypeDef,
     DescribeSimulationJobBatchRequestRequestTypeDef,
     SimulationJobSummaryTypeDef,
     DescribeSimulationJobRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeWorldExportJobRequestRequestTypeDef,
     DescribeWorldGenerationJobRequestRequestTypeDef,
     DescribeWorldRequestRequestTypeDef,
-    DescribeWorldResponseTypeDef,
     DescribeWorldTemplateRequestRequestTypeDef,
-    DescribeWorldTemplateResponseTypeDef,
     WorldFailureTypeDef,
     FilterTypeDef,
     FleetTypeDef,
     GetWorldTemplateBodyRequestRequestTypeDef,
-    GetWorldTemplateBodyResponseTypeDef,
+    PaginatorConfigTypeDef,
     SimulationJobBatchSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
     ListWorldTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     WorldSummaryTypeDef,
-    PaginatorConfigTypeDef,
+    PortMappingOutputTypeDef,
     PortMappingTypeDef,
     ProgressDetailTypeDef,
     RegisterRobotRequestRequestTypeDef,
-    RegisterRobotResponseTypeDef,
-    ResponseMetadataTypeDef,
     RestartSimulationJobRequestRequestTypeDef,
+    ToolOutputTypeDef,
+    UploadConfigurationOutputTypeDef,
     ToolTypeDef,
     UploadConfigurationTypeDef,
+    WorldConfigOutputTypeDef,
     WorldConfigTypeDef,
+    VPCConfigOutputTypeDef,
     SyncDeploymentJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    BatchDeleteWorldsResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    CreateRobotResponseTypeDef,
+    CreateWorldTemplateResponseTypeDef,
+    DeregisterRobotResponseTypeDef,
+    DescribeRobotResponseTypeDef,
+    DescribeWorldResponseTypeDef,
+    DescribeWorldTemplateResponseTypeDef,
+    GetWorldTemplateBodyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterRobotResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
-    RobotApplicationSummaryTypeDef,
     CreateRobotApplicationRequestRequestTypeDef,
     UpdateRobotApplicationRequestRequestTypeDef,
+    RobotApplicationSummaryTypeDef,
     CreateRobotApplicationResponseTypeDef,
     CreateRobotApplicationVersionResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     CreateSimulationApplicationRequestRequestTypeDef,
+    UpdateSimulationApplicationRequestRequestTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     DescribeSimulationApplicationResponseTypeDef,
     SimulationApplicationSummaryTypeDef,
-    UpdateSimulationApplicationRequestRequestTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     CreateWorldExportJobRequestRequestTypeDef,
     CreateWorldExportJobResponseTypeDef,
     DescribeWorldExportJobResponseTypeDef,
     WorldExportJobSummaryTypeDef,
     CreateWorldGenerationJobRequestRequestTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     WorldGenerationJobSummaryTypeDef,
     CreateWorldTemplateRequestRequestTypeDef,
     UpdateWorldTemplateRequestRequestTypeDef,
     DataSourceTypeDef,
+    DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
+    DeploymentConfigOutputTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
     FailureSummaryTypeDef,
-    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
     ListDeploymentJobsRequestRequestTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
-    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
     ListRobotApplicationsRequestRequestTypeDef,
-    ListRobotsRequestListRobotsPaginateTypeDef,
     ListRobotsRequestRequestTypeDef,
-    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
     ListSimulationApplicationsRequestRequestTypeDef,
-    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
     ListSimulationJobBatchesRequestRequestTypeDef,
-    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
     ListSimulationJobsRequestRequestTypeDef,
-    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
     ListWorldExportJobsRequestRequestTypeDef,
-    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
     ListWorldGenerationJobsRequestRequestTypeDef,
-    ListWorldsRequestListWorldsPaginateTypeDef,
     ListWorldsRequestRequestTypeDef,
     ListFleetsResponseTypeDef,
+    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
+    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
+    ListRobotsRequestListRobotsPaginateTypeDef,
+    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
+    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
+    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
+    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
+    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
+    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
+    ListWorldsRequestListWorldsPaginateTypeDef,
     ListSimulationJobBatchesResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     ListWorldsResponseTypeDef,
+    PortForwardingConfigOutputTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
     ListWorldExportJobsResponseTypeDef,
     ListWorldGenerationJobsResponseTypeDef,
-    CreateDeploymentJobRequestRequestTypeDef,
     CreateDeploymentJobResponseTypeDef,
     DeploymentJobTypeDef,
     SyncDeploymentJobResponseTypeDef,
+    CreateDeploymentJobRequestRequestTypeDef,
     FinishedWorldsSummaryTypeDef,
+    LaunchConfigOutputTypeDef,
     LaunchConfigTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     ListDeploymentJobsResponseTypeDef,
     DescribeWorldGenerationJobResponseTypeDef,
+    RobotApplicationConfigOutputTypeDef,
+    SimulationApplicationConfigOutputTypeDef,
     RobotApplicationConfigTypeDef,
     SimulationApplicationConfigTypeDef,
-    CreateSimulationJobRequestRequestTypeDef,
     CreateSimulationJobResponseTypeDef,
     DescribeSimulationJobResponseTypeDef,
-    SimulationJobRequestTypeDef,
+    SimulationJobRequestOutputTypeDef,
     SimulationJobTypeDef,
+    CreateSimulationJobRequestRequestTypeDef,
+    SimulationJobRequestTypeDef,
     FailedCreateSimulationJobRequestTypeDef,
-    StartSimulationJobBatchRequestRequestTypeDef,
     BatchDescribeSimulationJobResponseTypeDef,
+    StartSimulationJobBatchRequestRequestTypeDef,
     DescribeSimulationJobBatchResponseTypeDef,
     StartSimulationJobBatchResponseTypeDef,
 )
 
 
 def get_structure() -> BatchDeleteWorldsRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-robomaker-1.28.0/mypy_boto3_robomaker.egg-info/SOURCES.txt` & `mypy-boto3-robomaker-1.28.12/mypy_boto3_robomaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.0/setup.py` & `mypy-boto3-robomaker-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-robomaker",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_robomaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RoboMaker 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.RoboMaker 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

