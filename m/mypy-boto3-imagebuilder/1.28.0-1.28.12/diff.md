# Comparing `tmp/mypy-boto3-imagebuilder-1.28.0.tar.gz` & `tmp/mypy-boto3-imagebuilder-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-imagebuilder-1.28.0.tar", last modified: Thu Jul  6 20:59:44 2023, max compression
+gzip compressed data, was "mypy-boto3-imagebuilder-1.28.12.tar", last modified: Thu Jul 27 05:34:46 2023, max compression
```

## Comparing `mypy-boto3-imagebuilder-1.28.0.tar` & `mypy-boto3-imagebuilder-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:43.986322 mypy-boto3-imagebuilder-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:42:53.000000 mypy-boto3-imagebuilder-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-07-06 20:59:43.986322 mypy-boto3-imagebuilder-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-07-06 20:42:53.000000 mypy-boto3-imagebuilder-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:43.986322 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-06 20:42:53.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-06 20:42:53.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:42:53.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41846 2023-07-06 20:42:54.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41783 2023-07-06 20:42:53.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-06 20:42:56.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-07-06 20:42:56.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:53.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    66675 2023-07-06 20:42:58.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    66620 2023-07-06 20:42:57.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:42:53.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:43.986322 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-07-06 20:59:43.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-06 20:59:43.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:43.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:43.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:43.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:43.000000 mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:43.986322 mypy-boto3-imagebuilder-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:42:53.000000 mypy-boto3-imagebuilder-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.900492 mypy-boto3-imagebuilder-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20617 2023-07-27 05:34:46.900492 mypy-boto3-imagebuilder-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.900492 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41846 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41783 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-27 05:23:31.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75575 2023-07-27 05:23:32.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75508 2023-07-27 05:23:31.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.900492 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20617 2023-07-27 05:34:46.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 05:34:46.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:46.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:46.000000 mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:46.900492 mypy-boto3-imagebuilder-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:23:29.000000 mypy-boto3-imagebuilder-1.28.12/setup.py
```

### Comparing `mypy-boto3-imagebuilder-1.28.0/LICENSE` & `mypy-boto3-imagebuilder-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.0/PKG-INFO` & `mypy-boto3-imagebuilder-1.28.12/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-imagebuilder
-Version: 1.28.0
-Summary: Type annotations for boto3.imagebuilder 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.imagebuilder 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-imagebuilder"></a>
 
 # mypy-boto3-imagebuilder
 
 [![PyPI - mypy-boto3-imagebuilder](https://img.shields.io/pypi/v/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-imagebuilder?color=blue)](https://pypistats.org/packages/mypy-boto3-imagebuilder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-imagebuilder)](https://pepy.tech/project/mypy-boto3-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.imagebuilder 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[boto3.imagebuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [mypy-boto3-imagebuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,23 +316,27 @@
 
 `mypy_boto3_imagebuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_imagebuilder.type_defs import (
     SeverityCountsTypeDef,
+    SystemsManagerAgentOutputTypeDef,
     SystemsManagerAgentTypeDef,
+    LaunchPermissionConfigurationOutputTypeDef,
     LaunchPermissionConfigurationTypeDef,
     ImageStateTypeDef,
     CancelImageCreationRequestRequestTypeDef,
     CancelImageCreationResponseTypeDef,
+    ComponentParameterOutputTypeDef,
     ComponentParameterTypeDef,
     ComponentParameterDetailTypeDef,
     ComponentStateTypeDef,
     ComponentVersionTypeDef,
+    TargetContainerRepositoryOutputTypeDef,
     TargetContainerRepositoryTypeDef,
     ContainerRecipeSummaryTypeDef,
     ContainerTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateComponentResponseTypeDef,
     CreateContainerRecipeResponseTypeDef,
     CreateDistributionConfigurationResponseTypeDef,
@@ -356,18 +360,24 @@
     DeleteImageRecipeRequestRequestTypeDef,
     DeleteImageRecipeResponseTypeDef,
     DeleteImageRequestRequestTypeDef,
     DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationRequestRequestTypeDef,
     DeleteInfrastructureConfigurationResponseTypeDef,
     DistributionConfigurationSummaryTypeDef,
+    LaunchTemplateConfigurationOutputTypeDef,
+    S3ExportConfigurationOutputTypeDef,
     LaunchTemplateConfigurationTypeDef,
     S3ExportConfigurationTypeDef,
+    EbsInstanceBlockDeviceSpecificationOutputTypeDef,
     EbsInstanceBlockDeviceSpecificationTypeDef,
+    EcrConfigurationOutputTypeDef,
     EcrConfigurationTypeDef,
+    FastLaunchLaunchTemplateSpecificationOutputTypeDef,
+    FastLaunchSnapshotConfigurationOutputTypeDef,
     FastLaunchLaunchTemplateSpecificationTypeDef,
     FastLaunchSnapshotConfigurationTypeDef,
     FilterTypeDef,
     GetComponentPolicyRequestRequestTypeDef,
     GetComponentPolicyResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetContainerRecipePolicyRequestRequestTypeDef,
@@ -383,31 +393,35 @@
     GetImageRequestRequestTypeDef,
     GetInfrastructureConfigurationRequestRequestTypeDef,
     GetWorkflowExecutionRequestRequestTypeDef,
     GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionRequestRequestTypeDef,
     GetWorkflowStepExecutionResponseTypeDef,
     ImagePackageTypeDef,
+    ImageTestsConfigurationOutputTypeDef,
+    ScheduleOutputTypeDef,
     ImageRecipeSummaryTypeDef,
     ImageScanFindingsFilterTypeDef,
     ImageScanStateTypeDef,
     ImageVersionTypeDef,
     ImportComponentRequestRequestTypeDef,
     ImportComponentResponseTypeDef,
     ImportVmImageRequestRequestTypeDef,
     ImportVmImageResponseTypeDef,
     InfrastructureConfigurationSummaryTypeDef,
+    InstanceMetadataOptionsOutputTypeDef,
     ListComponentBuildVersionsRequestRequestTypeDef,
     ListImagePackagesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowExecutionsRequestRequestTypeDef,
     WorkflowExecutionMetadataTypeDef,
     ListWorkflowStepExecutionsRequestRequestTypeDef,
     WorkflowStepMetadataTypeDef,
+    S3LogsOutputTypeDef,
     S3LogsTypeDef,
     VulnerablePackageTypeDef,
     PutComponentPolicyRequestRequestTypeDef,
     PutComponentPolicyResponseTypeDef,
     PutContainerRecipePolicyRequestRequestTypeDef,
     PutContainerRecipePolicyResponseTypeDef,
     PutImagePolicyRequestRequestTypeDef,
@@ -423,27 +437,34 @@
     UpdateDistributionConfigurationResponseTypeDef,
     UpdateImagePipelineResponseTypeDef,
     UpdateInfrastructureConfigurationResponseTypeDef,
     AccountAggregationTypeDef,
     ImageAggregationTypeDef,
     ImagePipelineAggregationTypeDef,
     VulnerabilityIdAggregationTypeDef,
+    AdditionalInstanceConfigurationOutputTypeDef,
     AdditionalInstanceConfigurationTypeDef,
+    AmiDistributionConfigurationOutputTypeDef,
     AmiDistributionConfigurationTypeDef,
     AmiTypeDef,
+    ComponentConfigurationOutputTypeDef,
     ComponentConfigurationTypeDef,
     ComponentSummaryTypeDef,
     ComponentTypeDef,
     ListComponentsResponseTypeDef,
+    ContainerDistributionConfigurationOutputTypeDef,
     ContainerDistributionConfigurationTypeDef,
     ListContainerRecipesResponseTypeDef,
     CvssScoreDetailsTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
+    InstanceBlockDeviceMappingOutputTypeDef,
     InstanceBlockDeviceMappingTypeDef,
+    ImageScanningConfigurationOutputTypeDef,
     ImageScanningConfigurationTypeDef,
+    FastLaunchConfigurationOutputTypeDef,
     FastLaunchConfigurationTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListContainerRecipesRequestRequestTypeDef,
     ListDistributionConfigurationsRequestRequestTypeDef,
     ListImageBuildVersionsRequestRequestTypeDef,
     ListImagePipelineImagesRequestRequestTypeDef,
     ListImagePipelinesRequestRequestTypeDef,
@@ -454,43 +475,46 @@
     ListImagePackagesResponseTypeDef,
     ListImageRecipesResponseTypeDef,
     ListImageScanFindingsRequestRequestTypeDef,
     ListImagesResponseTypeDef,
     ListInfrastructureConfigurationsResponseTypeDef,
     ListWorkflowExecutionsResponseTypeDef,
     ListWorkflowStepExecutionsResponseTypeDef,
+    LoggingOutputTypeDef,
     LoggingTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ImageScanFindingAggregationTypeDef,
     OutputResourcesTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     GetComponentResponseTypeDef,
     InspectorScoreDetailsTypeDef,
-    CreateImageRecipeRequestRequestTypeDef,
     ImageRecipeTypeDef,
+    InstanceConfigurationOutputTypeDef,
+    CreateImageRecipeRequestRequestTypeDef,
     InstanceConfigurationTypeDef,
+    ImagePipelineTypeDef,
     CreateImagePipelineRequestRequestTypeDef,
     CreateImageRequestRequestTypeDef,
-    ImagePipelineTypeDef,
     UpdateImagePipelineRequestRequestTypeDef,
+    DistributionOutputTypeDef,
     DistributionTypeDef,
-    CreateInfrastructureConfigurationRequestRequestTypeDef,
     InfrastructureConfigurationTypeDef,
+    CreateInfrastructureConfigurationRequestRequestTypeDef,
     UpdateInfrastructureConfigurationRequestRequestTypeDef,
     ListImageScanFindingAggregationsResponseTypeDef,
     ImageSummaryTypeDef,
     ImageScanFindingTypeDef,
     GetImageRecipeResponseTypeDef,
     ContainerRecipeTypeDef,
     CreateContainerRecipeRequestRequestTypeDef,
     GetImagePipelineResponseTypeDef,
     ListImagePipelinesResponseTypeDef,
-    CreateDistributionConfigurationRequestRequestTypeDef,
     DistributionConfigurationTypeDef,
+    CreateDistributionConfigurationRequestRequestTypeDef,
     UpdateDistributionConfigurationRequestRequestTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePipelineImagesResponseTypeDef,
     ListImageScanFindingsResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
```

### Comparing `mypy-boto3-imagebuilder-1.28.0/README.md` & `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-imagebuilder
+Version: 1.28.12
+Summary: Type annotations for boto3.imagebuilder 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 imagebuilder type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-imagebuilder"></a>
 
 # mypy-boto3-imagebuilder
 
 [![PyPI - mypy-boto3-imagebuilder](https://img.shields.io/pypi/v/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-imagebuilder?color=blue)](https://pypistats.org/packages/mypy-boto3-imagebuilder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-imagebuilder)](https://pepy.tech/project/mypy-boto3-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.imagebuilder 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[boto3.imagebuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [mypy-boto3-imagebuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,23 +316,27 @@
 
 `mypy_boto3_imagebuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_imagebuilder.type_defs import (
     SeverityCountsTypeDef,
+    SystemsManagerAgentOutputTypeDef,
     SystemsManagerAgentTypeDef,
+    LaunchPermissionConfigurationOutputTypeDef,
     LaunchPermissionConfigurationTypeDef,
     ImageStateTypeDef,
     CancelImageCreationRequestRequestTypeDef,
     CancelImageCreationResponseTypeDef,
+    ComponentParameterOutputTypeDef,
     ComponentParameterTypeDef,
     ComponentParameterDetailTypeDef,
     ComponentStateTypeDef,
     ComponentVersionTypeDef,
+    TargetContainerRepositoryOutputTypeDef,
     TargetContainerRepositoryTypeDef,
     ContainerRecipeSummaryTypeDef,
     ContainerTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateComponentResponseTypeDef,
     CreateContainerRecipeResponseTypeDef,
     CreateDistributionConfigurationResponseTypeDef,
@@ -324,18 +360,24 @@
     DeleteImageRecipeRequestRequestTypeDef,
     DeleteImageRecipeResponseTypeDef,
     DeleteImageRequestRequestTypeDef,
     DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationRequestRequestTypeDef,
     DeleteInfrastructureConfigurationResponseTypeDef,
     DistributionConfigurationSummaryTypeDef,
+    LaunchTemplateConfigurationOutputTypeDef,
+    S3ExportConfigurationOutputTypeDef,
     LaunchTemplateConfigurationTypeDef,
     S3ExportConfigurationTypeDef,
+    EbsInstanceBlockDeviceSpecificationOutputTypeDef,
     EbsInstanceBlockDeviceSpecificationTypeDef,
+    EcrConfigurationOutputTypeDef,
     EcrConfigurationTypeDef,
+    FastLaunchLaunchTemplateSpecificationOutputTypeDef,
+    FastLaunchSnapshotConfigurationOutputTypeDef,
     FastLaunchLaunchTemplateSpecificationTypeDef,
     FastLaunchSnapshotConfigurationTypeDef,
     FilterTypeDef,
     GetComponentPolicyRequestRequestTypeDef,
     GetComponentPolicyResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetContainerRecipePolicyRequestRequestTypeDef,
@@ -351,31 +393,35 @@
     GetImageRequestRequestTypeDef,
     GetInfrastructureConfigurationRequestRequestTypeDef,
     GetWorkflowExecutionRequestRequestTypeDef,
     GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionRequestRequestTypeDef,
     GetWorkflowStepExecutionResponseTypeDef,
     ImagePackageTypeDef,
+    ImageTestsConfigurationOutputTypeDef,
+    ScheduleOutputTypeDef,
     ImageRecipeSummaryTypeDef,
     ImageScanFindingsFilterTypeDef,
     ImageScanStateTypeDef,
     ImageVersionTypeDef,
     ImportComponentRequestRequestTypeDef,
     ImportComponentResponseTypeDef,
     ImportVmImageRequestRequestTypeDef,
     ImportVmImageResponseTypeDef,
     InfrastructureConfigurationSummaryTypeDef,
+    InstanceMetadataOptionsOutputTypeDef,
     ListComponentBuildVersionsRequestRequestTypeDef,
     ListImagePackagesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowExecutionsRequestRequestTypeDef,
     WorkflowExecutionMetadataTypeDef,
     ListWorkflowStepExecutionsRequestRequestTypeDef,
     WorkflowStepMetadataTypeDef,
+    S3LogsOutputTypeDef,
     S3LogsTypeDef,
     VulnerablePackageTypeDef,
     PutComponentPolicyRequestRequestTypeDef,
     PutComponentPolicyResponseTypeDef,
     PutContainerRecipePolicyRequestRequestTypeDef,
     PutContainerRecipePolicyResponseTypeDef,
     PutImagePolicyRequestRequestTypeDef,
@@ -391,27 +437,34 @@
     UpdateDistributionConfigurationResponseTypeDef,
     UpdateImagePipelineResponseTypeDef,
     UpdateInfrastructureConfigurationResponseTypeDef,
     AccountAggregationTypeDef,
     ImageAggregationTypeDef,
     ImagePipelineAggregationTypeDef,
     VulnerabilityIdAggregationTypeDef,
+    AdditionalInstanceConfigurationOutputTypeDef,
     AdditionalInstanceConfigurationTypeDef,
+    AmiDistributionConfigurationOutputTypeDef,
     AmiDistributionConfigurationTypeDef,
     AmiTypeDef,
+    ComponentConfigurationOutputTypeDef,
     ComponentConfigurationTypeDef,
     ComponentSummaryTypeDef,
     ComponentTypeDef,
     ListComponentsResponseTypeDef,
+    ContainerDistributionConfigurationOutputTypeDef,
     ContainerDistributionConfigurationTypeDef,
     ListContainerRecipesResponseTypeDef,
     CvssScoreDetailsTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
+    InstanceBlockDeviceMappingOutputTypeDef,
     InstanceBlockDeviceMappingTypeDef,
+    ImageScanningConfigurationOutputTypeDef,
     ImageScanningConfigurationTypeDef,
+    FastLaunchConfigurationOutputTypeDef,
     FastLaunchConfigurationTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListContainerRecipesRequestRequestTypeDef,
     ListDistributionConfigurationsRequestRequestTypeDef,
     ListImageBuildVersionsRequestRequestTypeDef,
     ListImagePipelineImagesRequestRequestTypeDef,
     ListImagePipelinesRequestRequestTypeDef,
@@ -422,43 +475,46 @@
     ListImagePackagesResponseTypeDef,
     ListImageRecipesResponseTypeDef,
     ListImageScanFindingsRequestRequestTypeDef,
     ListImagesResponseTypeDef,
     ListInfrastructureConfigurationsResponseTypeDef,
     ListWorkflowExecutionsResponseTypeDef,
     ListWorkflowStepExecutionsResponseTypeDef,
+    LoggingOutputTypeDef,
     LoggingTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ImageScanFindingAggregationTypeDef,
     OutputResourcesTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     GetComponentResponseTypeDef,
     InspectorScoreDetailsTypeDef,
-    CreateImageRecipeRequestRequestTypeDef,
     ImageRecipeTypeDef,
+    InstanceConfigurationOutputTypeDef,
+    CreateImageRecipeRequestRequestTypeDef,
     InstanceConfigurationTypeDef,
+    ImagePipelineTypeDef,
     CreateImagePipelineRequestRequestTypeDef,
     CreateImageRequestRequestTypeDef,
-    ImagePipelineTypeDef,
     UpdateImagePipelineRequestRequestTypeDef,
+    DistributionOutputTypeDef,
     DistributionTypeDef,
-    CreateInfrastructureConfigurationRequestRequestTypeDef,
     InfrastructureConfigurationTypeDef,
+    CreateInfrastructureConfigurationRequestRequestTypeDef,
     UpdateInfrastructureConfigurationRequestRequestTypeDef,
     ListImageScanFindingAggregationsResponseTypeDef,
     ImageSummaryTypeDef,
     ImageScanFindingTypeDef,
     GetImageRecipeResponseTypeDef,
     ContainerRecipeTypeDef,
     CreateContainerRecipeRequestRequestTypeDef,
     GetImagePipelineResponseTypeDef,
     ListImagePipelinesResponseTypeDef,
-    CreateDistributionConfigurationRequestRequestTypeDef,
     DistributionConfigurationTypeDef,
+    CreateDistributionConfigurationRequestRequestTypeDef,
     UpdateDistributionConfigurationRequestRequestTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePipelineImagesResponseTypeDef,
     ListImageScanFindingsResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
```

### Comparing `mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/__main__.py` & `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.imagebuilder 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.imagebuilder 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder\nOther"
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

### Comparing `mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/client.py` & `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/client.pyi` & `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/literals.py` & `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,14 +206,15 @@
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
@@ -292,26 +293,28 @@
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

### Comparing `mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/literals.pyi` & `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -204,14 +204,15 @@
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
@@ -290,26 +291,28 @@
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

### Comparing `mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/type_defs.py` & `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,23 +42,27 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "SeverityCountsTypeDef",
+    "SystemsManagerAgentOutputTypeDef",
     "SystemsManagerAgentTypeDef",
+    "LaunchPermissionConfigurationOutputTypeDef",
     "LaunchPermissionConfigurationTypeDef",
     "ImageStateTypeDef",
     "CancelImageCreationRequestRequestTypeDef",
     "CancelImageCreationResponseTypeDef",
+    "ComponentParameterOutputTypeDef",
     "ComponentParameterTypeDef",
     "ComponentParameterDetailTypeDef",
     "ComponentStateTypeDef",
     "ComponentVersionTypeDef",
+    "TargetContainerRepositoryOutputTypeDef",
     "TargetContainerRepositoryTypeDef",
     "ContainerRecipeSummaryTypeDef",
     "ContainerTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "CreateComponentResponseTypeDef",
     "CreateContainerRecipeResponseTypeDef",
     "CreateDistributionConfigurationResponseTypeDef",
@@ -82,18 +86,24 @@
     "DeleteImageRecipeRequestRequestTypeDef",
     "DeleteImageRecipeResponseTypeDef",
     "DeleteImageRequestRequestTypeDef",
     "DeleteImageResponseTypeDef",
     "DeleteInfrastructureConfigurationRequestRequestTypeDef",
     "DeleteInfrastructureConfigurationResponseTypeDef",
     "DistributionConfigurationSummaryTypeDef",
+    "LaunchTemplateConfigurationOutputTypeDef",
+    "S3ExportConfigurationOutputTypeDef",
     "LaunchTemplateConfigurationTypeDef",
     "S3ExportConfigurationTypeDef",
+    "EbsInstanceBlockDeviceSpecificationOutputTypeDef",
     "EbsInstanceBlockDeviceSpecificationTypeDef",
+    "EcrConfigurationOutputTypeDef",
     "EcrConfigurationTypeDef",
+    "FastLaunchLaunchTemplateSpecificationOutputTypeDef",
+    "FastLaunchSnapshotConfigurationOutputTypeDef",
     "FastLaunchLaunchTemplateSpecificationTypeDef",
     "FastLaunchSnapshotConfigurationTypeDef",
     "FilterTypeDef",
     "GetComponentPolicyRequestRequestTypeDef",
     "GetComponentPolicyResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetContainerRecipePolicyRequestRequestTypeDef",
@@ -109,31 +119,35 @@
     "GetImageRequestRequestTypeDef",
     "GetInfrastructureConfigurationRequestRequestTypeDef",
     "GetWorkflowExecutionRequestRequestTypeDef",
     "GetWorkflowExecutionResponseTypeDef",
     "GetWorkflowStepExecutionRequestRequestTypeDef",
     "GetWorkflowStepExecutionResponseTypeDef",
     "ImagePackageTypeDef",
+    "ImageTestsConfigurationOutputTypeDef",
+    "ScheduleOutputTypeDef",
     "ImageRecipeSummaryTypeDef",
     "ImageScanFindingsFilterTypeDef",
     "ImageScanStateTypeDef",
     "ImageVersionTypeDef",
     "ImportComponentRequestRequestTypeDef",
     "ImportComponentResponseTypeDef",
     "ImportVmImageRequestRequestTypeDef",
     "ImportVmImageResponseTypeDef",
     "InfrastructureConfigurationSummaryTypeDef",
+    "InstanceMetadataOptionsOutputTypeDef",
     "ListComponentBuildVersionsRequestRequestTypeDef",
     "ListImagePackagesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListWorkflowExecutionsRequestRequestTypeDef",
     "WorkflowExecutionMetadataTypeDef",
     "ListWorkflowStepExecutionsRequestRequestTypeDef",
     "WorkflowStepMetadataTypeDef",
+    "S3LogsOutputTypeDef",
     "S3LogsTypeDef",
     "VulnerablePackageTypeDef",
     "PutComponentPolicyRequestRequestTypeDef",
     "PutComponentPolicyResponseTypeDef",
     "PutContainerRecipePolicyRequestRequestTypeDef",
     "PutContainerRecipePolicyResponseTypeDef",
     "PutImagePolicyRequestRequestTypeDef",
@@ -149,27 +163,34 @@
     "UpdateDistributionConfigurationResponseTypeDef",
     "UpdateImagePipelineResponseTypeDef",
     "UpdateInfrastructureConfigurationResponseTypeDef",
     "AccountAggregationTypeDef",
     "ImageAggregationTypeDef",
     "ImagePipelineAggregationTypeDef",
     "VulnerabilityIdAggregationTypeDef",
+    "AdditionalInstanceConfigurationOutputTypeDef",
     "AdditionalInstanceConfigurationTypeDef",
+    "AmiDistributionConfigurationOutputTypeDef",
     "AmiDistributionConfigurationTypeDef",
     "AmiTypeDef",
+    "ComponentConfigurationOutputTypeDef",
     "ComponentConfigurationTypeDef",
     "ComponentSummaryTypeDef",
     "ComponentTypeDef",
     "ListComponentsResponseTypeDef",
+    "ContainerDistributionConfigurationOutputTypeDef",
     "ContainerDistributionConfigurationTypeDef",
     "ListContainerRecipesResponseTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDistributionConfigurationsResponseTypeDef",
+    "InstanceBlockDeviceMappingOutputTypeDef",
     "InstanceBlockDeviceMappingTypeDef",
+    "ImageScanningConfigurationOutputTypeDef",
     "ImageScanningConfigurationTypeDef",
+    "FastLaunchConfigurationOutputTypeDef",
     "FastLaunchConfigurationTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListContainerRecipesRequestRequestTypeDef",
     "ListDistributionConfigurationsRequestRequestTypeDef",
     "ListImageBuildVersionsRequestRequestTypeDef",
     "ListImagePipelineImagesRequestRequestTypeDef",
     "ListImagePipelinesRequestRequestTypeDef",
@@ -180,43 +201,46 @@
     "ListImagePackagesResponseTypeDef",
     "ListImageRecipesResponseTypeDef",
     "ListImageScanFindingsRequestRequestTypeDef",
     "ListImagesResponseTypeDef",
     "ListInfrastructureConfigurationsResponseTypeDef",
     "ListWorkflowExecutionsResponseTypeDef",
     "ListWorkflowStepExecutionsResponseTypeDef",
+    "LoggingOutputTypeDef",
     "LoggingTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "ImageScanFindingAggregationTypeDef",
     "OutputResourcesTypeDef",
     "ListComponentBuildVersionsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "InspectorScoreDetailsTypeDef",
-    "CreateImageRecipeRequestRequestTypeDef",
     "ImageRecipeTypeDef",
+    "InstanceConfigurationOutputTypeDef",
+    "CreateImageRecipeRequestRequestTypeDef",
     "InstanceConfigurationTypeDef",
+    "ImagePipelineTypeDef",
     "CreateImagePipelineRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
-    "ImagePipelineTypeDef",
     "UpdateImagePipelineRequestRequestTypeDef",
+    "DistributionOutputTypeDef",
     "DistributionTypeDef",
-    "CreateInfrastructureConfigurationRequestRequestTypeDef",
     "InfrastructureConfigurationTypeDef",
+    "CreateInfrastructureConfigurationRequestRequestTypeDef",
     "UpdateInfrastructureConfigurationRequestRequestTypeDef",
     "ListImageScanFindingAggregationsResponseTypeDef",
     "ImageSummaryTypeDef",
     "ImageScanFindingTypeDef",
     "GetImageRecipeResponseTypeDef",
     "ContainerRecipeTypeDef",
     "CreateContainerRecipeRequestRequestTypeDef",
     "GetImagePipelineResponseTypeDef",
     "ListImagePipelinesResponseTypeDef",
-    "CreateDistributionConfigurationRequestRequestTypeDef",
     "DistributionConfigurationTypeDef",
+    "CreateDistributionConfigurationRequestRequestTypeDef",
     "UpdateDistributionConfigurationRequestRequestTypeDef",
     "GetInfrastructureConfigurationResponseTypeDef",
     "ListImageBuildVersionsResponseTypeDef",
     "ListImagePipelineImagesResponseTypeDef",
     "ListImageScanFindingsResponseTypeDef",
     "GetContainerRecipeResponseTypeDef",
     "GetDistributionConfigurationResponseTypeDef",
@@ -231,22 +255,41 @@
         "critical": int,
         "high": int,
         "medium": int,
     },
     total=False,
 )
 
+SystemsManagerAgentOutputTypeDef = TypedDict(
+    "SystemsManagerAgentOutputTypeDef",
+    {
+        "uninstallAfterBuild": bool,
+    },
+    total=False,
+)
+
 SystemsManagerAgentTypeDef = TypedDict(
     "SystemsManagerAgentTypeDef",
     {
         "uninstallAfterBuild": bool,
     },
     total=False,
 )
 
+LaunchPermissionConfigurationOutputTypeDef = TypedDict(
+    "LaunchPermissionConfigurationOutputTypeDef",
+    {
+        "userIds": List[str],
+        "userGroups": List[str],
+        "organizationArns": List[str],
+        "organizationalUnitArns": List[str],
+    },
+    total=False,
+)
+
 LaunchPermissionConfigurationTypeDef = TypedDict(
     "LaunchPermissionConfigurationTypeDef",
     {
         "userIds": Sequence[str],
         "userGroups": Sequence[str],
         "organizationArns": Sequence[str],
         "organizationalUnitArns": Sequence[str],
@@ -277,14 +320,22 @@
         "requestId": str,
         "clientToken": str,
         "imageBuildVersionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ComponentParameterOutputTypeDef = TypedDict(
+    "ComponentParameterOutputTypeDef",
+    {
+        "name": str,
+        "value": List[str],
+    },
+)
+
 ComponentParameterTypeDef = TypedDict(
     "ComponentParameterTypeDef",
     {
         "name": str,
         "value": Sequence[str],
     },
 )
@@ -333,14 +384,22 @@
         "type": ComponentTypeType,
         "owner": str,
         "dateCreated": str,
     },
     total=False,
 )
 
+TargetContainerRepositoryOutputTypeDef = TypedDict(
+    "TargetContainerRepositoryOutputTypeDef",
+    {
+        "service": Literal["ECR"],
+        "repositoryName": str,
+    },
+)
+
 TargetContainerRepositoryTypeDef = TypedDict(
     "TargetContainerRepositoryTypeDef",
     {
         "service": Literal["ECR"],
         "repositoryName": str,
     },
 )
@@ -639,14 +698,60 @@
         "dateUpdated": str,
         "tags": Dict[str, str],
         "regions": List[str],
     },
     total=False,
 )
 
+_RequiredLaunchTemplateConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLaunchTemplateConfigurationOutputTypeDef",
+    {
+        "launchTemplateId": str,
+    },
+)
+_OptionalLaunchTemplateConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLaunchTemplateConfigurationOutputTypeDef",
+    {
+        "accountId": str,
+        "setDefaultVersion": bool,
+    },
+    total=False,
+)
+
+
+class LaunchTemplateConfigurationOutputTypeDef(
+    _RequiredLaunchTemplateConfigurationOutputTypeDef,
+    _OptionalLaunchTemplateConfigurationOutputTypeDef,
+):
+    pass
+
+
+_RequiredS3ExportConfigurationOutputTypeDef = TypedDict(
+    "_RequiredS3ExportConfigurationOutputTypeDef",
+    {
+        "roleName": str,
+        "diskImageFormat": DiskImageFormatType,
+        "s3Bucket": str,
+    },
+)
+_OptionalS3ExportConfigurationOutputTypeDef = TypedDict(
+    "_OptionalS3ExportConfigurationOutputTypeDef",
+    {
+        "s3Prefix": str,
+    },
+    total=False,
+)
+
+
+class S3ExportConfigurationOutputTypeDef(
+    _RequiredS3ExportConfigurationOutputTypeDef, _OptionalS3ExportConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredLaunchTemplateConfigurationTypeDef = TypedDict(
     "_RequiredLaunchTemplateConfigurationTypeDef",
     {
         "launchTemplateId": str,
     },
 )
 _OptionalLaunchTemplateConfigurationTypeDef = TypedDict(
@@ -684,14 +789,29 @@
 
 class S3ExportConfigurationTypeDef(
     _RequiredS3ExportConfigurationTypeDef, _OptionalS3ExportConfigurationTypeDef
 ):
     pass
 
 
+EbsInstanceBlockDeviceSpecificationOutputTypeDef = TypedDict(
+    "EbsInstanceBlockDeviceSpecificationOutputTypeDef",
+    {
+        "encrypted": bool,
+        "deleteOnTermination": bool,
+        "iops": int,
+        "kmsKeyId": str,
+        "snapshotId": str,
+        "volumeSize": int,
+        "volumeType": EbsVolumeTypeType,
+        "throughput": int,
+    },
+    total=False,
+)
+
 EbsInstanceBlockDeviceSpecificationTypeDef = TypedDict(
     "EbsInstanceBlockDeviceSpecificationTypeDef",
     {
         "encrypted": bool,
         "deleteOnTermination": bool,
         "iops": int,
         "kmsKeyId": str,
@@ -699,23 +819,50 @@
         "volumeSize": int,
         "volumeType": EbsVolumeTypeType,
         "throughput": int,
     },
     total=False,
 )
 
+EcrConfigurationOutputTypeDef = TypedDict(
+    "EcrConfigurationOutputTypeDef",
+    {
+        "repositoryName": str,
+        "containerTags": List[str],
+    },
+    total=False,
+)
+
 EcrConfigurationTypeDef = TypedDict(
     "EcrConfigurationTypeDef",
     {
         "repositoryName": str,
         "containerTags": Sequence[str],
     },
     total=False,
 )
 
+FastLaunchLaunchTemplateSpecificationOutputTypeDef = TypedDict(
+    "FastLaunchLaunchTemplateSpecificationOutputTypeDef",
+    {
+        "launchTemplateId": str,
+        "launchTemplateName": str,
+        "launchTemplateVersion": str,
+    },
+    total=False,
+)
+
+FastLaunchSnapshotConfigurationOutputTypeDef = TypedDict(
+    "FastLaunchSnapshotConfigurationOutputTypeDef",
+    {
+        "targetResourceCount": int,
+    },
+    total=False,
+)
+
 FastLaunchLaunchTemplateSpecificationTypeDef = TypedDict(
     "FastLaunchLaunchTemplateSpecificationTypeDef",
     {
         "launchTemplateId": str,
         "launchTemplateName": str,
         "launchTemplateVersion": str,
     },
@@ -915,14 +1062,33 @@
     {
         "packageName": str,
         "packageVersion": str,
     },
     total=False,
 )
 
+ImageTestsConfigurationOutputTypeDef = TypedDict(
+    "ImageTestsConfigurationOutputTypeDef",
+    {
+        "imageTestsEnabled": bool,
+        "timeoutMinutes": int,
+    },
+    total=False,
+)
+
+ScheduleOutputTypeDef = TypedDict(
+    "ScheduleOutputTypeDef",
+    {
+        "scheduleExpression": str,
+        "timezone": str,
+        "pipelineExecutionStartCondition": PipelineExecutionStartConditionType,
+    },
+    total=False,
+)
+
 ImageRecipeSummaryTypeDef = TypedDict(
     "ImageRecipeSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "platform": PlatformType,
         "owner": str,
@@ -1058,14 +1224,23 @@
         "tags": Dict[str, str],
         "instanceTypes": List[str],
         "instanceProfileName": str,
     },
     total=False,
 )
 
+InstanceMetadataOptionsOutputTypeDef = TypedDict(
+    "InstanceMetadataOptionsOutputTypeDef",
+    {
+        "httpTokens": str,
+        "httpPutResponseHopLimit": int,
+    },
+    total=False,
+)
+
 _RequiredListComponentBuildVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentBuildVersionsRequestRequestTypeDef",
     {
         "componentVersionArn": str,
     },
 )
 _OptionalListComponentBuildVersionsRequestRequestTypeDef = TypedDict(
@@ -1200,14 +1375,23 @@
         "outputs": str,
         "startTime": str,
         "endTime": str,
     },
     total=False,
 )
 
+S3LogsOutputTypeDef = TypedDict(
+    "S3LogsOutputTypeDef",
+    {
+        "s3BucketName": str,
+        "s3KeyPrefix": str,
+    },
+    total=False,
+)
+
 S3LogsTypeDef = TypedDict(
     "S3LogsTypeDef",
     {
         "s3BucketName": str,
         "s3KeyPrefix": str,
     },
     total=False,
@@ -1414,23 +1598,45 @@
     {
         "vulnerabilityId": str,
         "severityCounts": SeverityCountsTypeDef,
     },
     total=False,
 )
 
+AdditionalInstanceConfigurationOutputTypeDef = TypedDict(
+    "AdditionalInstanceConfigurationOutputTypeDef",
+    {
+        "systemsManagerAgent": SystemsManagerAgentOutputTypeDef,
+        "userDataOverride": str,
+    },
+    total=False,
+)
+
 AdditionalInstanceConfigurationTypeDef = TypedDict(
     "AdditionalInstanceConfigurationTypeDef",
     {
         "systemsManagerAgent": SystemsManagerAgentTypeDef,
         "userDataOverride": str,
     },
     total=False,
 )
 
+AmiDistributionConfigurationOutputTypeDef = TypedDict(
+    "AmiDistributionConfigurationOutputTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "targetAccountIds": List[str],
+        "amiTags": Dict[str, str],
+        "kmsKeyId": str,
+        "launchPermission": LaunchPermissionConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 AmiDistributionConfigurationTypeDef = TypedDict(
     "AmiDistributionConfigurationTypeDef",
     {
         "name": str,
         "description": str,
         "targetAccountIds": Sequence[str],
         "amiTags": Mapping[str, str],
@@ -1449,14 +1655,35 @@
         "description": str,
         "state": ImageStateTypeDef,
         "accountId": str,
     },
     total=False,
 )
 
+_RequiredComponentConfigurationOutputTypeDef = TypedDict(
+    "_RequiredComponentConfigurationOutputTypeDef",
+    {
+        "componentArn": str,
+    },
+)
+_OptionalComponentConfigurationOutputTypeDef = TypedDict(
+    "_OptionalComponentConfigurationOutputTypeDef",
+    {
+        "parameters": List[ComponentParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ComponentConfigurationOutputTypeDef(
+    _RequiredComponentConfigurationOutputTypeDef, _OptionalComponentConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredComponentConfigurationTypeDef = TypedDict(
     "_RequiredComponentConfigurationTypeDef",
     {
         "componentArn": str,
     },
 )
 _OptionalComponentConfigurationTypeDef = TypedDict(
@@ -1526,14 +1753,37 @@
         "requestId": str,
         "componentVersionList": List[ComponentVersionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredContainerDistributionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredContainerDistributionConfigurationOutputTypeDef",
+    {
+        "targetRepository": TargetContainerRepositoryOutputTypeDef,
+    },
+)
+_OptionalContainerDistributionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalContainerDistributionConfigurationOutputTypeDef",
+    {
+        "description": str,
+        "containerTags": List[str],
+    },
+    total=False,
+)
+
+
+class ContainerDistributionConfigurationOutputTypeDef(
+    _RequiredContainerDistributionConfigurationOutputTypeDef,
+    _OptionalContainerDistributionConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredContainerDistributionConfigurationTypeDef = TypedDict(
     "_RequiredContainerDistributionConfigurationTypeDef",
     {
         "targetRepository": TargetContainerRepositoryTypeDef,
     },
 )
 _OptionalContainerDistributionConfigurationTypeDef = TypedDict(
@@ -1582,34 +1832,78 @@
         "requestId": str,
         "distributionConfigurationSummaryList": List[DistributionConfigurationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+InstanceBlockDeviceMappingOutputTypeDef = TypedDict(
+    "InstanceBlockDeviceMappingOutputTypeDef",
+    {
+        "deviceName": str,
+        "ebs": EbsInstanceBlockDeviceSpecificationOutputTypeDef,
+        "virtualName": str,
+        "noDevice": str,
+    },
+    total=False,
+)
+
 InstanceBlockDeviceMappingTypeDef = TypedDict(
     "InstanceBlockDeviceMappingTypeDef",
     {
         "deviceName": str,
         "ebs": EbsInstanceBlockDeviceSpecificationTypeDef,
         "virtualName": str,
         "noDevice": str,
     },
     total=False,
 )
 
+ImageScanningConfigurationOutputTypeDef = TypedDict(
+    "ImageScanningConfigurationOutputTypeDef",
+    {
+        "imageScanningEnabled": bool,
+        "ecrConfiguration": EcrConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ImageScanningConfigurationTypeDef = TypedDict(
     "ImageScanningConfigurationTypeDef",
     {
         "imageScanningEnabled": bool,
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredFastLaunchConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFastLaunchConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalFastLaunchConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFastLaunchConfigurationOutputTypeDef",
+    {
+        "snapshotConfiguration": FastLaunchSnapshotConfigurationOutputTypeDef,
+        "maxParallelLaunches": int,
+        "launchTemplate": FastLaunchLaunchTemplateSpecificationOutputTypeDef,
+        "accountId": str,
+    },
+    total=False,
+)
+
+
+class FastLaunchConfigurationOutputTypeDef(
+    _RequiredFastLaunchConfigurationOutputTypeDef, _OptionalFastLaunchConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredFastLaunchConfigurationTypeDef = TypedDict(
     "_RequiredFastLaunchConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalFastLaunchConfigurationTypeDef = TypedDict(
@@ -1836,14 +2130,22 @@
         "imageBuildVersionArn": str,
         "message": str,
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LoggingOutputTypeDef = TypedDict(
+    "LoggingOutputTypeDef",
+    {
+        "s3Logs": S3LogsOutputTypeDef,
+    },
+    total=False,
+)
+
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "s3Logs": S3LogsTypeDef,
     },
     total=False,
 )
@@ -1928,14 +2230,44 @@
     "InspectorScoreDetailsTypeDef",
     {
         "adjustedCvss": CvssScoreDetailsTypeDef,
     },
     total=False,
 )
 
+ImageRecipeTypeDef = TypedDict(
+    "ImageRecipeTypeDef",
+    {
+        "arn": str,
+        "type": ImageTypeType,
+        "name": str,
+        "description": str,
+        "platform": PlatformType,
+        "owner": str,
+        "version": str,
+        "components": List[ComponentConfigurationOutputTypeDef],
+        "parentImage": str,
+        "blockDeviceMappings": List[InstanceBlockDeviceMappingOutputTypeDef],
+        "dateCreated": str,
+        "tags": Dict[str, str],
+        "workingDirectory": str,
+        "additionalInstanceConfiguration": AdditionalInstanceConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+InstanceConfigurationOutputTypeDef = TypedDict(
+    "InstanceConfigurationOutputTypeDef",
+    {
+        "image": str,
+        "blockDeviceMappings": List[InstanceBlockDeviceMappingOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageRecipeRequestRequestTypeDef",
     {
         "name": str,
         "semanticVersion": str,
         "components": Sequence[ComponentConfigurationTypeDef],
         "parentImage": str,
@@ -1957,40 +2289,44 @@
 
 class CreateImageRecipeRequestRequestTypeDef(
     _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
 ):
     pass
 
 
-ImageRecipeTypeDef = TypedDict(
-    "ImageRecipeTypeDef",
+InstanceConfigurationTypeDef = TypedDict(
+    "InstanceConfigurationTypeDef",
+    {
+        "image": str,
+        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
+    },
+    total=False,
+)
+
+ImagePipelineTypeDef = TypedDict(
+    "ImagePipelineTypeDef",
     {
         "arn": str,
-        "type": ImageTypeType,
         "name": str,
         "description": str,
         "platform": PlatformType,
-        "owner": str,
-        "version": str,
-        "components": List[ComponentConfigurationTypeDef],
-        "parentImage": str,
-        "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
+        "enhancedImageMetadataEnabled": bool,
+        "imageRecipeArn": str,
+        "containerRecipeArn": str,
+        "infrastructureConfigurationArn": str,
+        "distributionConfigurationArn": str,
+        "imageTestsConfiguration": ImageTestsConfigurationOutputTypeDef,
+        "schedule": ScheduleOutputTypeDef,
+        "status": PipelineStatusType,
         "dateCreated": str,
+        "dateUpdated": str,
+        "dateLastRun": str,
+        "dateNextRun": str,
         "tags": Dict[str, str],
-        "workingDirectory": str,
-        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
-    },
-    total=False,
-)
-
-InstanceConfigurationTypeDef = TypedDict(
-    "InstanceConfigurationTypeDef",
-    {
-        "image": str,
-        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
+        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImagePipelineRequestRequestTypeDef",
     {
@@ -2048,39 +2384,14 @@
 
 class CreateImageRequestRequestTypeDef(
     _RequiredCreateImageRequestRequestTypeDef, _OptionalCreateImageRequestRequestTypeDef
 ):
     pass
 
 
-ImagePipelineTypeDef = TypedDict(
-    "ImagePipelineTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "platform": PlatformType,
-        "enhancedImageMetadataEnabled": bool,
-        "imageRecipeArn": str,
-        "containerRecipeArn": str,
-        "infrastructureConfigurationArn": str,
-        "distributionConfigurationArn": str,
-        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
-        "schedule": ScheduleTypeDef,
-        "status": PipelineStatusType,
-        "dateCreated": str,
-        "dateUpdated": str,
-        "dateLastRun": str,
-        "dateNextRun": str,
-        "tags": Dict[str, str],
-        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImagePipelineRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
         "infrastructureConfigurationArn": str,
         "clientToken": str,
     },
@@ -2105,14 +2416,40 @@
 class UpdateImagePipelineRequestRequestTypeDef(
     _RequiredUpdateImagePipelineRequestRequestTypeDef,
     _OptionalUpdateImagePipelineRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDistributionOutputTypeDef = TypedDict(
+    "_RequiredDistributionOutputTypeDef",
+    {
+        "region": str,
+    },
+)
+_OptionalDistributionOutputTypeDef = TypedDict(
+    "_OptionalDistributionOutputTypeDef",
+    {
+        "amiDistributionConfiguration": AmiDistributionConfigurationOutputTypeDef,
+        "containerDistributionConfiguration": ContainerDistributionConfigurationOutputTypeDef,
+        "licenseConfigurationArns": List[str],
+        "launchTemplateConfigurations": List[LaunchTemplateConfigurationOutputTypeDef],
+        "s3ExportConfiguration": S3ExportConfigurationOutputTypeDef,
+        "fastLaunchConfigurations": List[FastLaunchConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class DistributionOutputTypeDef(
+    _RequiredDistributionOutputTypeDef, _OptionalDistributionOutputTypeDef
+):
+    pass
+
+
 _RequiredDistributionTypeDef = TypedDict(
     "_RequiredDistributionTypeDef",
     {
         "region": str,
     },
 )
 _OptionalDistributionTypeDef = TypedDict(
@@ -2129,14 +2466,37 @@
 )
 
 
 class DistributionTypeDef(_RequiredDistributionTypeDef, _OptionalDistributionTypeDef):
     pass
 
 
+InfrastructureConfigurationTypeDef = TypedDict(
+    "InfrastructureConfigurationTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "instanceTypes": List[str],
+        "instanceProfileName": str,
+        "securityGroupIds": List[str],
+        "subnetId": str,
+        "logging": LoggingOutputTypeDef,
+        "keyPair": str,
+        "terminateInstanceOnFailure": bool,
+        "snsTopicArn": str,
+        "dateCreated": str,
+        "dateUpdated": str,
+        "resourceTags": Dict[str, str],
+        "instanceMetadataOptions": InstanceMetadataOptionsOutputTypeDef,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredCreateInfrastructureConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInfrastructureConfigurationRequestRequestTypeDef",
     {
         "name": str,
         "instanceProfileName": str,
         "clientToken": str,
     },
@@ -2163,37 +2523,14 @@
 class CreateInfrastructureConfigurationRequestRequestTypeDef(
     _RequiredCreateInfrastructureConfigurationRequestRequestTypeDef,
     _OptionalCreateInfrastructureConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-InfrastructureConfigurationTypeDef = TypedDict(
-    "InfrastructureConfigurationTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "instanceTypes": List[str],
-        "instanceProfileName": str,
-        "securityGroupIds": List[str],
-        "subnetId": str,
-        "logging": LoggingTypeDef,
-        "keyPair": str,
-        "terminateInstanceOnFailure": bool,
-        "snsTopicArn": str,
-        "dateCreated": str,
-        "dateUpdated": str,
-        "resourceTags": Dict[str, str],
-        "instanceMetadataOptions": InstanceMetadataOptionsTypeDef,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredUpdateInfrastructureConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInfrastructureConfigurationRequestRequestTypeDef",
     {
         "infrastructureConfigurationArn": str,
         "instanceProfileName": str,
         "clientToken": str,
     },
@@ -2290,24 +2627,24 @@
         "arn": str,
         "containerType": Literal["DOCKER"],
         "name": str,
         "description": str,
         "platform": PlatformType,
         "owner": str,
         "version": str,
-        "components": List[ComponentConfigurationTypeDef],
-        "instanceConfiguration": InstanceConfigurationTypeDef,
+        "components": List[ComponentConfigurationOutputTypeDef],
+        "instanceConfiguration": InstanceConfigurationOutputTypeDef,
         "dockerfileTemplateData": str,
         "kmsKeyId": str,
         "encrypted": bool,
         "parentImage": str,
         "dateCreated": str,
         "tags": Dict[str, str],
         "workingDirectory": str,
-        "targetRepository": TargetContainerRepositoryTypeDef,
+        "targetRepository": TargetContainerRepositoryOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerRecipeRequestRequestTypeDef",
     {
@@ -2359,62 +2696,62 @@
         "requestId": str,
         "imagePipelineList": List[ImagePipelineTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
+_RequiredDistributionConfigurationTypeDef = TypedDict(
+    "_RequiredDistributionConfigurationTypeDef",
     {
-        "name": str,
-        "distributions": Sequence[DistributionTypeDef],
-        "clientToken": str,
+        "timeoutMinutes": int,
     },
 )
-_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
+_OptionalDistributionConfigurationTypeDef = TypedDict(
+    "_OptionalDistributionConfigurationTypeDef",
     {
+        "arn": str,
+        "name": str,
         "description": str,
-        "tags": Mapping[str, str],
+        "distributions": List[DistributionOutputTypeDef],
+        "dateCreated": str,
+        "dateUpdated": str,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class CreateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
+class DistributionConfigurationTypeDef(
+    _RequiredDistributionConfigurationTypeDef, _OptionalDistributionConfigurationTypeDef
 ):
     pass
 
 
-_RequiredDistributionConfigurationTypeDef = TypedDict(
-    "_RequiredDistributionConfigurationTypeDef",
+_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
     {
-        "timeoutMinutes": int,
+        "name": str,
+        "distributions": Sequence[DistributionTypeDef],
+        "clientToken": str,
     },
 )
-_OptionalDistributionConfigurationTypeDef = TypedDict(
-    "_OptionalDistributionConfigurationTypeDef",
+_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
     {
-        "arn": str,
-        "name": str,
         "description": str,
-        "distributions": List[DistributionTypeDef],
-        "dateCreated": str,
-        "dateUpdated": str,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class DistributionConfigurationTypeDef(
-    _RequiredDistributionConfigurationTypeDef, _OptionalDistributionConfigurationTypeDef
+class CreateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
 _RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
     {
@@ -2509,22 +2846,22 @@
         "state": ImageStateTypeDef,
         "imageRecipe": ImageRecipeTypeDef,
         "containerRecipe": ContainerRecipeTypeDef,
         "sourcePipelineName": str,
         "sourcePipelineArn": str,
         "infrastructureConfiguration": InfrastructureConfigurationTypeDef,
         "distributionConfiguration": DistributionConfigurationTypeDef,
-        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
+        "imageTestsConfiguration": ImageTestsConfigurationOutputTypeDef,
         "dateCreated": str,
         "outputResources": OutputResourcesTypeDef,
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
         "scanState": ImageScanStateTypeDef,
-        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
+        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 GetImageResponseTypeDef = TypedDict(
     "GetImageResponseTypeDef",
     {
```

### Comparing `mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder/type_defs.pyi` & `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -41,23 +41,27 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "SeverityCountsTypeDef",
+    "SystemsManagerAgentOutputTypeDef",
     "SystemsManagerAgentTypeDef",
+    "LaunchPermissionConfigurationOutputTypeDef",
     "LaunchPermissionConfigurationTypeDef",
     "ImageStateTypeDef",
     "CancelImageCreationRequestRequestTypeDef",
     "CancelImageCreationResponseTypeDef",
+    "ComponentParameterOutputTypeDef",
     "ComponentParameterTypeDef",
     "ComponentParameterDetailTypeDef",
     "ComponentStateTypeDef",
     "ComponentVersionTypeDef",
+    "TargetContainerRepositoryOutputTypeDef",
     "TargetContainerRepositoryTypeDef",
     "ContainerRecipeSummaryTypeDef",
     "ContainerTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "CreateComponentResponseTypeDef",
     "CreateContainerRecipeResponseTypeDef",
     "CreateDistributionConfigurationResponseTypeDef",
@@ -81,18 +85,24 @@
     "DeleteImageRecipeRequestRequestTypeDef",
     "DeleteImageRecipeResponseTypeDef",
     "DeleteImageRequestRequestTypeDef",
     "DeleteImageResponseTypeDef",
     "DeleteInfrastructureConfigurationRequestRequestTypeDef",
     "DeleteInfrastructureConfigurationResponseTypeDef",
     "DistributionConfigurationSummaryTypeDef",
+    "LaunchTemplateConfigurationOutputTypeDef",
+    "S3ExportConfigurationOutputTypeDef",
     "LaunchTemplateConfigurationTypeDef",
     "S3ExportConfigurationTypeDef",
+    "EbsInstanceBlockDeviceSpecificationOutputTypeDef",
     "EbsInstanceBlockDeviceSpecificationTypeDef",
+    "EcrConfigurationOutputTypeDef",
     "EcrConfigurationTypeDef",
+    "FastLaunchLaunchTemplateSpecificationOutputTypeDef",
+    "FastLaunchSnapshotConfigurationOutputTypeDef",
     "FastLaunchLaunchTemplateSpecificationTypeDef",
     "FastLaunchSnapshotConfigurationTypeDef",
     "FilterTypeDef",
     "GetComponentPolicyRequestRequestTypeDef",
     "GetComponentPolicyResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetContainerRecipePolicyRequestRequestTypeDef",
@@ -108,31 +118,35 @@
     "GetImageRequestRequestTypeDef",
     "GetInfrastructureConfigurationRequestRequestTypeDef",
     "GetWorkflowExecutionRequestRequestTypeDef",
     "GetWorkflowExecutionResponseTypeDef",
     "GetWorkflowStepExecutionRequestRequestTypeDef",
     "GetWorkflowStepExecutionResponseTypeDef",
     "ImagePackageTypeDef",
+    "ImageTestsConfigurationOutputTypeDef",
+    "ScheduleOutputTypeDef",
     "ImageRecipeSummaryTypeDef",
     "ImageScanFindingsFilterTypeDef",
     "ImageScanStateTypeDef",
     "ImageVersionTypeDef",
     "ImportComponentRequestRequestTypeDef",
     "ImportComponentResponseTypeDef",
     "ImportVmImageRequestRequestTypeDef",
     "ImportVmImageResponseTypeDef",
     "InfrastructureConfigurationSummaryTypeDef",
+    "InstanceMetadataOptionsOutputTypeDef",
     "ListComponentBuildVersionsRequestRequestTypeDef",
     "ListImagePackagesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListWorkflowExecutionsRequestRequestTypeDef",
     "WorkflowExecutionMetadataTypeDef",
     "ListWorkflowStepExecutionsRequestRequestTypeDef",
     "WorkflowStepMetadataTypeDef",
+    "S3LogsOutputTypeDef",
     "S3LogsTypeDef",
     "VulnerablePackageTypeDef",
     "PutComponentPolicyRequestRequestTypeDef",
     "PutComponentPolicyResponseTypeDef",
     "PutContainerRecipePolicyRequestRequestTypeDef",
     "PutContainerRecipePolicyResponseTypeDef",
     "PutImagePolicyRequestRequestTypeDef",
@@ -148,27 +162,34 @@
     "UpdateDistributionConfigurationResponseTypeDef",
     "UpdateImagePipelineResponseTypeDef",
     "UpdateInfrastructureConfigurationResponseTypeDef",
     "AccountAggregationTypeDef",
     "ImageAggregationTypeDef",
     "ImagePipelineAggregationTypeDef",
     "VulnerabilityIdAggregationTypeDef",
+    "AdditionalInstanceConfigurationOutputTypeDef",
     "AdditionalInstanceConfigurationTypeDef",
+    "AmiDistributionConfigurationOutputTypeDef",
     "AmiDistributionConfigurationTypeDef",
     "AmiTypeDef",
+    "ComponentConfigurationOutputTypeDef",
     "ComponentConfigurationTypeDef",
     "ComponentSummaryTypeDef",
     "ComponentTypeDef",
     "ListComponentsResponseTypeDef",
+    "ContainerDistributionConfigurationOutputTypeDef",
     "ContainerDistributionConfigurationTypeDef",
     "ListContainerRecipesResponseTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDistributionConfigurationsResponseTypeDef",
+    "InstanceBlockDeviceMappingOutputTypeDef",
     "InstanceBlockDeviceMappingTypeDef",
+    "ImageScanningConfigurationOutputTypeDef",
     "ImageScanningConfigurationTypeDef",
+    "FastLaunchConfigurationOutputTypeDef",
     "FastLaunchConfigurationTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListContainerRecipesRequestRequestTypeDef",
     "ListDistributionConfigurationsRequestRequestTypeDef",
     "ListImageBuildVersionsRequestRequestTypeDef",
     "ListImagePipelineImagesRequestRequestTypeDef",
     "ListImagePipelinesRequestRequestTypeDef",
@@ -179,43 +200,46 @@
     "ListImagePackagesResponseTypeDef",
     "ListImageRecipesResponseTypeDef",
     "ListImageScanFindingsRequestRequestTypeDef",
     "ListImagesResponseTypeDef",
     "ListInfrastructureConfigurationsResponseTypeDef",
     "ListWorkflowExecutionsResponseTypeDef",
     "ListWorkflowStepExecutionsResponseTypeDef",
+    "LoggingOutputTypeDef",
     "LoggingTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "ImageScanFindingAggregationTypeDef",
     "OutputResourcesTypeDef",
     "ListComponentBuildVersionsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "InspectorScoreDetailsTypeDef",
-    "CreateImageRecipeRequestRequestTypeDef",
     "ImageRecipeTypeDef",
+    "InstanceConfigurationOutputTypeDef",
+    "CreateImageRecipeRequestRequestTypeDef",
     "InstanceConfigurationTypeDef",
+    "ImagePipelineTypeDef",
     "CreateImagePipelineRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
-    "ImagePipelineTypeDef",
     "UpdateImagePipelineRequestRequestTypeDef",
+    "DistributionOutputTypeDef",
     "DistributionTypeDef",
-    "CreateInfrastructureConfigurationRequestRequestTypeDef",
     "InfrastructureConfigurationTypeDef",
+    "CreateInfrastructureConfigurationRequestRequestTypeDef",
     "UpdateInfrastructureConfigurationRequestRequestTypeDef",
     "ListImageScanFindingAggregationsResponseTypeDef",
     "ImageSummaryTypeDef",
     "ImageScanFindingTypeDef",
     "GetImageRecipeResponseTypeDef",
     "ContainerRecipeTypeDef",
     "CreateContainerRecipeRequestRequestTypeDef",
     "GetImagePipelineResponseTypeDef",
     "ListImagePipelinesResponseTypeDef",
-    "CreateDistributionConfigurationRequestRequestTypeDef",
     "DistributionConfigurationTypeDef",
+    "CreateDistributionConfigurationRequestRequestTypeDef",
     "UpdateDistributionConfigurationRequestRequestTypeDef",
     "GetInfrastructureConfigurationResponseTypeDef",
     "ListImageBuildVersionsResponseTypeDef",
     "ListImagePipelineImagesResponseTypeDef",
     "ListImageScanFindingsResponseTypeDef",
     "GetContainerRecipeResponseTypeDef",
     "GetDistributionConfigurationResponseTypeDef",
@@ -230,22 +254,41 @@
         "critical": int,
         "high": int,
         "medium": int,
     },
     total=False,
 )
 
+SystemsManagerAgentOutputTypeDef = TypedDict(
+    "SystemsManagerAgentOutputTypeDef",
+    {
+        "uninstallAfterBuild": bool,
+    },
+    total=False,
+)
+
 SystemsManagerAgentTypeDef = TypedDict(
     "SystemsManagerAgentTypeDef",
     {
         "uninstallAfterBuild": bool,
     },
     total=False,
 )
 
+LaunchPermissionConfigurationOutputTypeDef = TypedDict(
+    "LaunchPermissionConfigurationOutputTypeDef",
+    {
+        "userIds": List[str],
+        "userGroups": List[str],
+        "organizationArns": List[str],
+        "organizationalUnitArns": List[str],
+    },
+    total=False,
+)
+
 LaunchPermissionConfigurationTypeDef = TypedDict(
     "LaunchPermissionConfigurationTypeDef",
     {
         "userIds": Sequence[str],
         "userGroups": Sequence[str],
         "organizationArns": Sequence[str],
         "organizationalUnitArns": Sequence[str],
@@ -276,14 +319,22 @@
         "requestId": str,
         "clientToken": str,
         "imageBuildVersionArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ComponentParameterOutputTypeDef = TypedDict(
+    "ComponentParameterOutputTypeDef",
+    {
+        "name": str,
+        "value": List[str],
+    },
+)
+
 ComponentParameterTypeDef = TypedDict(
     "ComponentParameterTypeDef",
     {
         "name": str,
         "value": Sequence[str],
     },
 )
@@ -330,14 +381,22 @@
         "type": ComponentTypeType,
         "owner": str,
         "dateCreated": str,
     },
     total=False,
 )
 
+TargetContainerRepositoryOutputTypeDef = TypedDict(
+    "TargetContainerRepositoryOutputTypeDef",
+    {
+        "service": Literal["ECR"],
+        "repositoryName": str,
+    },
+)
+
 TargetContainerRepositoryTypeDef = TypedDict(
     "TargetContainerRepositoryTypeDef",
     {
         "service": Literal["ECR"],
         "repositoryName": str,
     },
 )
@@ -634,14 +693,56 @@
         "dateUpdated": str,
         "tags": Dict[str, str],
         "regions": List[str],
     },
     total=False,
 )
 
+_RequiredLaunchTemplateConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLaunchTemplateConfigurationOutputTypeDef",
+    {
+        "launchTemplateId": str,
+    },
+)
+_OptionalLaunchTemplateConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLaunchTemplateConfigurationOutputTypeDef",
+    {
+        "accountId": str,
+        "setDefaultVersion": bool,
+    },
+    total=False,
+)
+
+class LaunchTemplateConfigurationOutputTypeDef(
+    _RequiredLaunchTemplateConfigurationOutputTypeDef,
+    _OptionalLaunchTemplateConfigurationOutputTypeDef,
+):
+    pass
+
+_RequiredS3ExportConfigurationOutputTypeDef = TypedDict(
+    "_RequiredS3ExportConfigurationOutputTypeDef",
+    {
+        "roleName": str,
+        "diskImageFormat": DiskImageFormatType,
+        "s3Bucket": str,
+    },
+)
+_OptionalS3ExportConfigurationOutputTypeDef = TypedDict(
+    "_OptionalS3ExportConfigurationOutputTypeDef",
+    {
+        "s3Prefix": str,
+    },
+    total=False,
+)
+
+class S3ExportConfigurationOutputTypeDef(
+    _RequiredS3ExportConfigurationOutputTypeDef, _OptionalS3ExportConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredLaunchTemplateConfigurationTypeDef = TypedDict(
     "_RequiredLaunchTemplateConfigurationTypeDef",
     {
         "launchTemplateId": str,
     },
 )
 _OptionalLaunchTemplateConfigurationTypeDef = TypedDict(
@@ -675,14 +776,29 @@
 )
 
 class S3ExportConfigurationTypeDef(
     _RequiredS3ExportConfigurationTypeDef, _OptionalS3ExportConfigurationTypeDef
 ):
     pass
 
+EbsInstanceBlockDeviceSpecificationOutputTypeDef = TypedDict(
+    "EbsInstanceBlockDeviceSpecificationOutputTypeDef",
+    {
+        "encrypted": bool,
+        "deleteOnTermination": bool,
+        "iops": int,
+        "kmsKeyId": str,
+        "snapshotId": str,
+        "volumeSize": int,
+        "volumeType": EbsVolumeTypeType,
+        "throughput": int,
+    },
+    total=False,
+)
+
 EbsInstanceBlockDeviceSpecificationTypeDef = TypedDict(
     "EbsInstanceBlockDeviceSpecificationTypeDef",
     {
         "encrypted": bool,
         "deleteOnTermination": bool,
         "iops": int,
         "kmsKeyId": str,
@@ -690,23 +806,50 @@
         "volumeSize": int,
         "volumeType": EbsVolumeTypeType,
         "throughput": int,
     },
     total=False,
 )
 
+EcrConfigurationOutputTypeDef = TypedDict(
+    "EcrConfigurationOutputTypeDef",
+    {
+        "repositoryName": str,
+        "containerTags": List[str],
+    },
+    total=False,
+)
+
 EcrConfigurationTypeDef = TypedDict(
     "EcrConfigurationTypeDef",
     {
         "repositoryName": str,
         "containerTags": Sequence[str],
     },
     total=False,
 )
 
+FastLaunchLaunchTemplateSpecificationOutputTypeDef = TypedDict(
+    "FastLaunchLaunchTemplateSpecificationOutputTypeDef",
+    {
+        "launchTemplateId": str,
+        "launchTemplateName": str,
+        "launchTemplateVersion": str,
+    },
+    total=False,
+)
+
+FastLaunchSnapshotConfigurationOutputTypeDef = TypedDict(
+    "FastLaunchSnapshotConfigurationOutputTypeDef",
+    {
+        "targetResourceCount": int,
+    },
+    total=False,
+)
+
 FastLaunchLaunchTemplateSpecificationTypeDef = TypedDict(
     "FastLaunchLaunchTemplateSpecificationTypeDef",
     {
         "launchTemplateId": str,
         "launchTemplateName": str,
         "launchTemplateVersion": str,
     },
@@ -906,14 +1049,33 @@
     {
         "packageName": str,
         "packageVersion": str,
     },
     total=False,
 )
 
+ImageTestsConfigurationOutputTypeDef = TypedDict(
+    "ImageTestsConfigurationOutputTypeDef",
+    {
+        "imageTestsEnabled": bool,
+        "timeoutMinutes": int,
+    },
+    total=False,
+)
+
+ScheduleOutputTypeDef = TypedDict(
+    "ScheduleOutputTypeDef",
+    {
+        "scheduleExpression": str,
+        "timezone": str,
+        "pipelineExecutionStartCondition": PipelineExecutionStartConditionType,
+    },
+    total=False,
+)
+
 ImageRecipeSummaryTypeDef = TypedDict(
     "ImageRecipeSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "platform": PlatformType,
         "owner": str,
@@ -1045,14 +1207,23 @@
         "tags": Dict[str, str],
         "instanceTypes": List[str],
         "instanceProfileName": str,
     },
     total=False,
 )
 
+InstanceMetadataOptionsOutputTypeDef = TypedDict(
+    "InstanceMetadataOptionsOutputTypeDef",
+    {
+        "httpTokens": str,
+        "httpPutResponseHopLimit": int,
+    },
+    total=False,
+)
+
 _RequiredListComponentBuildVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentBuildVersionsRequestRequestTypeDef",
     {
         "componentVersionArn": str,
     },
 )
 _OptionalListComponentBuildVersionsRequestRequestTypeDef = TypedDict(
@@ -1179,14 +1350,23 @@
         "outputs": str,
         "startTime": str,
         "endTime": str,
     },
     total=False,
 )
 
+S3LogsOutputTypeDef = TypedDict(
+    "S3LogsOutputTypeDef",
+    {
+        "s3BucketName": str,
+        "s3KeyPrefix": str,
+    },
+    total=False,
+)
+
 S3LogsTypeDef = TypedDict(
     "S3LogsTypeDef",
     {
         "s3BucketName": str,
         "s3KeyPrefix": str,
     },
     total=False,
@@ -1393,23 +1573,45 @@
     {
         "vulnerabilityId": str,
         "severityCounts": SeverityCountsTypeDef,
     },
     total=False,
 )
 
+AdditionalInstanceConfigurationOutputTypeDef = TypedDict(
+    "AdditionalInstanceConfigurationOutputTypeDef",
+    {
+        "systemsManagerAgent": SystemsManagerAgentOutputTypeDef,
+        "userDataOverride": str,
+    },
+    total=False,
+)
+
 AdditionalInstanceConfigurationTypeDef = TypedDict(
     "AdditionalInstanceConfigurationTypeDef",
     {
         "systemsManagerAgent": SystemsManagerAgentTypeDef,
         "userDataOverride": str,
     },
     total=False,
 )
 
+AmiDistributionConfigurationOutputTypeDef = TypedDict(
+    "AmiDistributionConfigurationOutputTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "targetAccountIds": List[str],
+        "amiTags": Dict[str, str],
+        "kmsKeyId": str,
+        "launchPermission": LaunchPermissionConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 AmiDistributionConfigurationTypeDef = TypedDict(
     "AmiDistributionConfigurationTypeDef",
     {
         "name": str,
         "description": str,
         "targetAccountIds": Sequence[str],
         "amiTags": Mapping[str, str],
@@ -1428,14 +1630,33 @@
         "description": str,
         "state": ImageStateTypeDef,
         "accountId": str,
     },
     total=False,
 )
 
+_RequiredComponentConfigurationOutputTypeDef = TypedDict(
+    "_RequiredComponentConfigurationOutputTypeDef",
+    {
+        "componentArn": str,
+    },
+)
+_OptionalComponentConfigurationOutputTypeDef = TypedDict(
+    "_OptionalComponentConfigurationOutputTypeDef",
+    {
+        "parameters": List[ComponentParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+class ComponentConfigurationOutputTypeDef(
+    _RequiredComponentConfigurationOutputTypeDef, _OptionalComponentConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredComponentConfigurationTypeDef = TypedDict(
     "_RequiredComponentConfigurationTypeDef",
     {
         "componentArn": str,
     },
 )
 _OptionalComponentConfigurationTypeDef = TypedDict(
@@ -1503,14 +1724,35 @@
         "requestId": str,
         "componentVersionList": List[ComponentVersionTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredContainerDistributionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredContainerDistributionConfigurationOutputTypeDef",
+    {
+        "targetRepository": TargetContainerRepositoryOutputTypeDef,
+    },
+)
+_OptionalContainerDistributionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalContainerDistributionConfigurationOutputTypeDef",
+    {
+        "description": str,
+        "containerTags": List[str],
+    },
+    total=False,
+)
+
+class ContainerDistributionConfigurationOutputTypeDef(
+    _RequiredContainerDistributionConfigurationOutputTypeDef,
+    _OptionalContainerDistributionConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredContainerDistributionConfigurationTypeDef = TypedDict(
     "_RequiredContainerDistributionConfigurationTypeDef",
     {
         "targetRepository": TargetContainerRepositoryTypeDef,
     },
 )
 _OptionalContainerDistributionConfigurationTypeDef = TypedDict(
@@ -1557,34 +1799,76 @@
         "requestId": str,
         "distributionConfigurationSummaryList": List[DistributionConfigurationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+InstanceBlockDeviceMappingOutputTypeDef = TypedDict(
+    "InstanceBlockDeviceMappingOutputTypeDef",
+    {
+        "deviceName": str,
+        "ebs": EbsInstanceBlockDeviceSpecificationOutputTypeDef,
+        "virtualName": str,
+        "noDevice": str,
+    },
+    total=False,
+)
+
 InstanceBlockDeviceMappingTypeDef = TypedDict(
     "InstanceBlockDeviceMappingTypeDef",
     {
         "deviceName": str,
         "ebs": EbsInstanceBlockDeviceSpecificationTypeDef,
         "virtualName": str,
         "noDevice": str,
     },
     total=False,
 )
 
+ImageScanningConfigurationOutputTypeDef = TypedDict(
+    "ImageScanningConfigurationOutputTypeDef",
+    {
+        "imageScanningEnabled": bool,
+        "ecrConfiguration": EcrConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ImageScanningConfigurationTypeDef = TypedDict(
     "ImageScanningConfigurationTypeDef",
     {
         "imageScanningEnabled": bool,
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredFastLaunchConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFastLaunchConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalFastLaunchConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFastLaunchConfigurationOutputTypeDef",
+    {
+        "snapshotConfiguration": FastLaunchSnapshotConfigurationOutputTypeDef,
+        "maxParallelLaunches": int,
+        "launchTemplate": FastLaunchLaunchTemplateSpecificationOutputTypeDef,
+        "accountId": str,
+    },
+    total=False,
+)
+
+class FastLaunchConfigurationOutputTypeDef(
+    _RequiredFastLaunchConfigurationOutputTypeDef, _OptionalFastLaunchConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredFastLaunchConfigurationTypeDef = TypedDict(
     "_RequiredFastLaunchConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalFastLaunchConfigurationTypeDef = TypedDict(
@@ -1805,14 +2089,22 @@
         "imageBuildVersionArn": str,
         "message": str,
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LoggingOutputTypeDef = TypedDict(
+    "LoggingOutputTypeDef",
+    {
+        "s3Logs": S3LogsOutputTypeDef,
+    },
+    total=False,
+)
+
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "s3Logs": S3LogsTypeDef,
     },
     total=False,
 )
@@ -1895,14 +2187,44 @@
     "InspectorScoreDetailsTypeDef",
     {
         "adjustedCvss": CvssScoreDetailsTypeDef,
     },
     total=False,
 )
 
+ImageRecipeTypeDef = TypedDict(
+    "ImageRecipeTypeDef",
+    {
+        "arn": str,
+        "type": ImageTypeType,
+        "name": str,
+        "description": str,
+        "platform": PlatformType,
+        "owner": str,
+        "version": str,
+        "components": List[ComponentConfigurationOutputTypeDef],
+        "parentImage": str,
+        "blockDeviceMappings": List[InstanceBlockDeviceMappingOutputTypeDef],
+        "dateCreated": str,
+        "tags": Dict[str, str],
+        "workingDirectory": str,
+        "additionalInstanceConfiguration": AdditionalInstanceConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+InstanceConfigurationOutputTypeDef = TypedDict(
+    "InstanceConfigurationOutputTypeDef",
+    {
+        "image": str,
+        "blockDeviceMappings": List[InstanceBlockDeviceMappingOutputTypeDef],
+    },
+    total=False,
+)
+
 _RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageRecipeRequestRequestTypeDef",
     {
         "name": str,
         "semanticVersion": str,
         "components": Sequence[ComponentConfigurationTypeDef],
         "parentImage": str,
@@ -1922,40 +2244,44 @@
 )
 
 class CreateImageRecipeRequestRequestTypeDef(
     _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
 ):
     pass
 
-ImageRecipeTypeDef = TypedDict(
-    "ImageRecipeTypeDef",
+InstanceConfigurationTypeDef = TypedDict(
+    "InstanceConfigurationTypeDef",
+    {
+        "image": str,
+        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
+    },
+    total=False,
+)
+
+ImagePipelineTypeDef = TypedDict(
+    "ImagePipelineTypeDef",
     {
         "arn": str,
-        "type": ImageTypeType,
         "name": str,
         "description": str,
         "platform": PlatformType,
-        "owner": str,
-        "version": str,
-        "components": List[ComponentConfigurationTypeDef],
-        "parentImage": str,
-        "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
+        "enhancedImageMetadataEnabled": bool,
+        "imageRecipeArn": str,
+        "containerRecipeArn": str,
+        "infrastructureConfigurationArn": str,
+        "distributionConfigurationArn": str,
+        "imageTestsConfiguration": ImageTestsConfigurationOutputTypeDef,
+        "schedule": ScheduleOutputTypeDef,
+        "status": PipelineStatusType,
         "dateCreated": str,
+        "dateUpdated": str,
+        "dateLastRun": str,
+        "dateNextRun": str,
         "tags": Dict[str, str],
-        "workingDirectory": str,
-        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
-    },
-    total=False,
-)
-
-InstanceConfigurationTypeDef = TypedDict(
-    "InstanceConfigurationTypeDef",
-    {
-        "image": str,
-        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
+        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImagePipelineRequestRequestTypeDef",
     {
@@ -2009,39 +2335,14 @@
 )
 
 class CreateImageRequestRequestTypeDef(
     _RequiredCreateImageRequestRequestTypeDef, _OptionalCreateImageRequestRequestTypeDef
 ):
     pass
 
-ImagePipelineTypeDef = TypedDict(
-    "ImagePipelineTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "platform": PlatformType,
-        "enhancedImageMetadataEnabled": bool,
-        "imageRecipeArn": str,
-        "containerRecipeArn": str,
-        "infrastructureConfigurationArn": str,
-        "distributionConfigurationArn": str,
-        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
-        "schedule": ScheduleTypeDef,
-        "status": PipelineStatusType,
-        "dateCreated": str,
-        "dateUpdated": str,
-        "dateLastRun": str,
-        "dateNextRun": str,
-        "tags": Dict[str, str],
-        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImagePipelineRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
         "infrastructureConfigurationArn": str,
         "clientToken": str,
     },
@@ -2064,14 +2365,38 @@
 
 class UpdateImagePipelineRequestRequestTypeDef(
     _RequiredUpdateImagePipelineRequestRequestTypeDef,
     _OptionalUpdateImagePipelineRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDistributionOutputTypeDef = TypedDict(
+    "_RequiredDistributionOutputTypeDef",
+    {
+        "region": str,
+    },
+)
+_OptionalDistributionOutputTypeDef = TypedDict(
+    "_OptionalDistributionOutputTypeDef",
+    {
+        "amiDistributionConfiguration": AmiDistributionConfigurationOutputTypeDef,
+        "containerDistributionConfiguration": ContainerDistributionConfigurationOutputTypeDef,
+        "licenseConfigurationArns": List[str],
+        "launchTemplateConfigurations": List[LaunchTemplateConfigurationOutputTypeDef],
+        "s3ExportConfiguration": S3ExportConfigurationOutputTypeDef,
+        "fastLaunchConfigurations": List[FastLaunchConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+class DistributionOutputTypeDef(
+    _RequiredDistributionOutputTypeDef, _OptionalDistributionOutputTypeDef
+):
+    pass
+
 _RequiredDistributionTypeDef = TypedDict(
     "_RequiredDistributionTypeDef",
     {
         "region": str,
     },
 )
 _OptionalDistributionTypeDef = TypedDict(
@@ -2086,14 +2411,37 @@
     },
     total=False,
 )
 
 class DistributionTypeDef(_RequiredDistributionTypeDef, _OptionalDistributionTypeDef):
     pass
 
+InfrastructureConfigurationTypeDef = TypedDict(
+    "InfrastructureConfigurationTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "instanceTypes": List[str],
+        "instanceProfileName": str,
+        "securityGroupIds": List[str],
+        "subnetId": str,
+        "logging": LoggingOutputTypeDef,
+        "keyPair": str,
+        "terminateInstanceOnFailure": bool,
+        "snsTopicArn": str,
+        "dateCreated": str,
+        "dateUpdated": str,
+        "resourceTags": Dict[str, str],
+        "instanceMetadataOptions": InstanceMetadataOptionsOutputTypeDef,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredCreateInfrastructureConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInfrastructureConfigurationRequestRequestTypeDef",
     {
         "name": str,
         "instanceProfileName": str,
         "clientToken": str,
     },
@@ -2118,37 +2466,14 @@
 
 class CreateInfrastructureConfigurationRequestRequestTypeDef(
     _RequiredCreateInfrastructureConfigurationRequestRequestTypeDef,
     _OptionalCreateInfrastructureConfigurationRequestRequestTypeDef,
 ):
     pass
 
-InfrastructureConfigurationTypeDef = TypedDict(
-    "InfrastructureConfigurationTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "instanceTypes": List[str],
-        "instanceProfileName": str,
-        "securityGroupIds": List[str],
-        "subnetId": str,
-        "logging": LoggingTypeDef,
-        "keyPair": str,
-        "terminateInstanceOnFailure": bool,
-        "snsTopicArn": str,
-        "dateCreated": str,
-        "dateUpdated": str,
-        "resourceTags": Dict[str, str],
-        "instanceMetadataOptions": InstanceMetadataOptionsTypeDef,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredUpdateInfrastructureConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInfrastructureConfigurationRequestRequestTypeDef",
     {
         "infrastructureConfigurationArn": str,
         "instanceProfileName": str,
         "clientToken": str,
     },
@@ -2243,24 +2568,24 @@
         "arn": str,
         "containerType": Literal["DOCKER"],
         "name": str,
         "description": str,
         "platform": PlatformType,
         "owner": str,
         "version": str,
-        "components": List[ComponentConfigurationTypeDef],
-        "instanceConfiguration": InstanceConfigurationTypeDef,
+        "components": List[ComponentConfigurationOutputTypeDef],
+        "instanceConfiguration": InstanceConfigurationOutputTypeDef,
         "dockerfileTemplateData": str,
         "kmsKeyId": str,
         "encrypted": bool,
         "parentImage": str,
         "dateCreated": str,
         "tags": Dict[str, str],
         "workingDirectory": str,
-        "targetRepository": TargetContainerRepositoryTypeDef,
+        "targetRepository": TargetContainerRepositoryOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerRecipeRequestRequestTypeDef",
     {
@@ -2310,62 +2635,62 @@
         "requestId": str,
         "imagePipelineList": List[ImagePipelineTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "name": str,
-        "distributions": Sequence[DistributionTypeDef],
-        "clientToken": str,
-    },
-)
-_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
 _RequiredDistributionConfigurationTypeDef = TypedDict(
     "_RequiredDistributionConfigurationTypeDef",
     {
         "timeoutMinutes": int,
     },
 )
 _OptionalDistributionConfigurationTypeDef = TypedDict(
     "_OptionalDistributionConfigurationTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
-        "distributions": List[DistributionTypeDef],
+        "distributions": List[DistributionOutputTypeDef],
         "dateCreated": str,
         "dateUpdated": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class DistributionConfigurationTypeDef(
     _RequiredDistributionConfigurationTypeDef, _OptionalDistributionConfigurationTypeDef
 ):
     pass
 
+_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "name": str,
+        "distributions": Sequence[DistributionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
     {
         "distributionConfigurationArn": str,
         "distributions": Sequence[DistributionTypeDef],
         "clientToken": str,
     },
@@ -2454,22 +2779,22 @@
         "state": ImageStateTypeDef,
         "imageRecipe": ImageRecipeTypeDef,
         "containerRecipe": ContainerRecipeTypeDef,
         "sourcePipelineName": str,
         "sourcePipelineArn": str,
         "infrastructureConfiguration": InfrastructureConfigurationTypeDef,
         "distributionConfiguration": DistributionConfigurationTypeDef,
-        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
+        "imageTestsConfiguration": ImageTestsConfigurationOutputTypeDef,
         "dateCreated": str,
         "outputResources": OutputResourcesTypeDef,
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
         "scanState": ImageScanStateTypeDef,
-        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
+        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 GetImageResponseTypeDef = TypedDict(
     "GetImageResponseTypeDef",
     {
```

### Comparing `mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder.egg-info/PKG-INFO` & `mypy-boto3-imagebuilder-1.28.12/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-imagebuilder
-Version: 1.28.0
-Summary: Type annotations for boto3.imagebuilder 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 imagebuilder type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-imagebuilder"></a>
 
 # mypy-boto3-imagebuilder
 
 [![PyPI - mypy-boto3-imagebuilder](https://img.shields.io/pypi/v/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-imagebuilder?color=blue)](https://pypistats.org/packages/mypy-boto3-imagebuilder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-imagebuilder)](https://pepy.tech/project/mypy-boto3-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.imagebuilder 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[boto3.imagebuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [mypy-boto3-imagebuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,23 +284,27 @@
 
 `mypy_boto3_imagebuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_imagebuilder.type_defs import (
     SeverityCountsTypeDef,
+    SystemsManagerAgentOutputTypeDef,
     SystemsManagerAgentTypeDef,
+    LaunchPermissionConfigurationOutputTypeDef,
     LaunchPermissionConfigurationTypeDef,
     ImageStateTypeDef,
     CancelImageCreationRequestRequestTypeDef,
     CancelImageCreationResponseTypeDef,
+    ComponentParameterOutputTypeDef,
     ComponentParameterTypeDef,
     ComponentParameterDetailTypeDef,
     ComponentStateTypeDef,
     ComponentVersionTypeDef,
+    TargetContainerRepositoryOutputTypeDef,
     TargetContainerRepositoryTypeDef,
     ContainerRecipeSummaryTypeDef,
     ContainerTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateComponentResponseTypeDef,
     CreateContainerRecipeResponseTypeDef,
     CreateDistributionConfigurationResponseTypeDef,
@@ -356,18 +328,24 @@
     DeleteImageRecipeRequestRequestTypeDef,
     DeleteImageRecipeResponseTypeDef,
     DeleteImageRequestRequestTypeDef,
     DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationRequestRequestTypeDef,
     DeleteInfrastructureConfigurationResponseTypeDef,
     DistributionConfigurationSummaryTypeDef,
+    LaunchTemplateConfigurationOutputTypeDef,
+    S3ExportConfigurationOutputTypeDef,
     LaunchTemplateConfigurationTypeDef,
     S3ExportConfigurationTypeDef,
+    EbsInstanceBlockDeviceSpecificationOutputTypeDef,
     EbsInstanceBlockDeviceSpecificationTypeDef,
+    EcrConfigurationOutputTypeDef,
     EcrConfigurationTypeDef,
+    FastLaunchLaunchTemplateSpecificationOutputTypeDef,
+    FastLaunchSnapshotConfigurationOutputTypeDef,
     FastLaunchLaunchTemplateSpecificationTypeDef,
     FastLaunchSnapshotConfigurationTypeDef,
     FilterTypeDef,
     GetComponentPolicyRequestRequestTypeDef,
     GetComponentPolicyResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetContainerRecipePolicyRequestRequestTypeDef,
@@ -383,31 +361,35 @@
     GetImageRequestRequestTypeDef,
     GetInfrastructureConfigurationRequestRequestTypeDef,
     GetWorkflowExecutionRequestRequestTypeDef,
     GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionRequestRequestTypeDef,
     GetWorkflowStepExecutionResponseTypeDef,
     ImagePackageTypeDef,
+    ImageTestsConfigurationOutputTypeDef,
+    ScheduleOutputTypeDef,
     ImageRecipeSummaryTypeDef,
     ImageScanFindingsFilterTypeDef,
     ImageScanStateTypeDef,
     ImageVersionTypeDef,
     ImportComponentRequestRequestTypeDef,
     ImportComponentResponseTypeDef,
     ImportVmImageRequestRequestTypeDef,
     ImportVmImageResponseTypeDef,
     InfrastructureConfigurationSummaryTypeDef,
+    InstanceMetadataOptionsOutputTypeDef,
     ListComponentBuildVersionsRequestRequestTypeDef,
     ListImagePackagesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowExecutionsRequestRequestTypeDef,
     WorkflowExecutionMetadataTypeDef,
     ListWorkflowStepExecutionsRequestRequestTypeDef,
     WorkflowStepMetadataTypeDef,
+    S3LogsOutputTypeDef,
     S3LogsTypeDef,
     VulnerablePackageTypeDef,
     PutComponentPolicyRequestRequestTypeDef,
     PutComponentPolicyResponseTypeDef,
     PutContainerRecipePolicyRequestRequestTypeDef,
     PutContainerRecipePolicyResponseTypeDef,
     PutImagePolicyRequestRequestTypeDef,
@@ -423,27 +405,34 @@
     UpdateDistributionConfigurationResponseTypeDef,
     UpdateImagePipelineResponseTypeDef,
     UpdateInfrastructureConfigurationResponseTypeDef,
     AccountAggregationTypeDef,
     ImageAggregationTypeDef,
     ImagePipelineAggregationTypeDef,
     VulnerabilityIdAggregationTypeDef,
+    AdditionalInstanceConfigurationOutputTypeDef,
     AdditionalInstanceConfigurationTypeDef,
+    AmiDistributionConfigurationOutputTypeDef,
     AmiDistributionConfigurationTypeDef,
     AmiTypeDef,
+    ComponentConfigurationOutputTypeDef,
     ComponentConfigurationTypeDef,
     ComponentSummaryTypeDef,
     ComponentTypeDef,
     ListComponentsResponseTypeDef,
+    ContainerDistributionConfigurationOutputTypeDef,
     ContainerDistributionConfigurationTypeDef,
     ListContainerRecipesResponseTypeDef,
     CvssScoreDetailsTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
+    InstanceBlockDeviceMappingOutputTypeDef,
     InstanceBlockDeviceMappingTypeDef,
+    ImageScanningConfigurationOutputTypeDef,
     ImageScanningConfigurationTypeDef,
+    FastLaunchConfigurationOutputTypeDef,
     FastLaunchConfigurationTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListContainerRecipesRequestRequestTypeDef,
     ListDistributionConfigurationsRequestRequestTypeDef,
     ListImageBuildVersionsRequestRequestTypeDef,
     ListImagePipelineImagesRequestRequestTypeDef,
     ListImagePipelinesRequestRequestTypeDef,
@@ -454,43 +443,46 @@
     ListImagePackagesResponseTypeDef,
     ListImageRecipesResponseTypeDef,
     ListImageScanFindingsRequestRequestTypeDef,
     ListImagesResponseTypeDef,
     ListInfrastructureConfigurationsResponseTypeDef,
     ListWorkflowExecutionsResponseTypeDef,
     ListWorkflowStepExecutionsResponseTypeDef,
+    LoggingOutputTypeDef,
     LoggingTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ImageScanFindingAggregationTypeDef,
     OutputResourcesTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     GetComponentResponseTypeDef,
     InspectorScoreDetailsTypeDef,
-    CreateImageRecipeRequestRequestTypeDef,
     ImageRecipeTypeDef,
+    InstanceConfigurationOutputTypeDef,
+    CreateImageRecipeRequestRequestTypeDef,
     InstanceConfigurationTypeDef,
+    ImagePipelineTypeDef,
     CreateImagePipelineRequestRequestTypeDef,
     CreateImageRequestRequestTypeDef,
-    ImagePipelineTypeDef,
     UpdateImagePipelineRequestRequestTypeDef,
+    DistributionOutputTypeDef,
     DistributionTypeDef,
-    CreateInfrastructureConfigurationRequestRequestTypeDef,
     InfrastructureConfigurationTypeDef,
+    CreateInfrastructureConfigurationRequestRequestTypeDef,
     UpdateInfrastructureConfigurationRequestRequestTypeDef,
     ListImageScanFindingAggregationsResponseTypeDef,
     ImageSummaryTypeDef,
     ImageScanFindingTypeDef,
     GetImageRecipeResponseTypeDef,
     ContainerRecipeTypeDef,
     CreateContainerRecipeRequestRequestTypeDef,
     GetImagePipelineResponseTypeDef,
     ListImagePipelinesResponseTypeDef,
-    CreateDistributionConfigurationRequestRequestTypeDef,
     DistributionConfigurationTypeDef,
+    CreateDistributionConfigurationRequestRequestTypeDef,
     UpdateDistributionConfigurationRequestRequestTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePipelineImagesResponseTypeDef,
     ListImageScanFindingsResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
```

### Comparing `mypy-boto3-imagebuilder-1.28.0/mypy_boto3_imagebuilder.egg-info/SOURCES.txt` & `mypy-boto3-imagebuilder-1.28.12/mypy_boto3_imagebuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.0/setup.py` & `mypy-boto3-imagebuilder-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-imagebuilder",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_imagebuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.imagebuilder 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.imagebuilder 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

