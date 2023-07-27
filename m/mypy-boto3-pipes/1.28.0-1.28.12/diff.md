# Comparing `tmp/mypy-boto3-pipes-1.28.0.tar.gz` & `tmp/mypy-boto3-pipes-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pipes-1.28.0.tar", last modified: Thu Jul  6 21:00:19 2023, max compression
+gzip compressed data, was "mypy-boto3-pipes-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
```

## Comparing `mypy-boto3-pipes-1.28.0.tar` & `mypy-boto3-pipes-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:19.846395 mypy-boto3-pipes-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:40.000000 mypy-boto3-pipes-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-06 21:00:19.838395 mypy-boto3-pipes-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-07-06 20:49:40.000000 mypy-boto3-pipes-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:19.838395 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-06 20:49:40.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-06 20:49:40.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-06 20:49:40.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-07-06 20:49:41.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-06 20:49:40.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-06 20:49:41.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-06 20:49:41.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 20:49:41.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-06 20:49:41.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:40.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31881 2023-07-06 20:49:42.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31851 2023-07-06 20:49:41.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:40.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:19.838395 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-06 21:00:19.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 21:00:19.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:19.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:19.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:19.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 21:00:19.000000 mypy-boto3-pipes-1.28.0/mypy_boto3_pipes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:19.846395 mypy-boto3-pipes-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-06 20:49:40.000000 mypy-boto3-pipes-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.893162 mypy-boto3-pipes-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18250 2023-07-27 11:49:24.885162 mypy-boto3-pipes-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52078 2023-07-27 11:41:42.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52026 2023-07-27 11:41:41.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18250 2023-07-27 11:49:24.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 11:49:24.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 11:49:24.000000 mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.893162 mypy-boto3-pipes-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-27 11:41:40.000000 mypy-boto3-pipes-1.28.12/setup.py
```

### Comparing `mypy-boto3-pipes-1.28.0/LICENSE` & `mypy-boto3-pipes-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.0/PKG-INFO` & `mypy-boto3-pipes-1.28.12/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pipes
-Version: 1.28.0
-Summary: Type annotations for boto3.EventBridgePipes 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EventBridgePipes 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-pipes"></a>
 
 # mypy-boto3-pipes
 
 [![PyPI - mypy-boto3-pipes](https://img.shields.io/pypi/v/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pipes?color=blue)](https://pypistats.org/packages/mypy-boto3-pipes)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pipes)](https://pepy.tech/project/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,97 +336,146 @@
 ### Typed dictionaries
 
 `mypy_boto3_pipes.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pipes.type_defs import (
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
+    BatchArrayPropertiesOutputTypeDef,
     BatchArrayPropertiesTypeDef,
+    BatchEnvironmentVariableOutputTypeDef,
+    BatchResourceRequirementOutputTypeDef,
     BatchEnvironmentVariableTypeDef,
     BatchResourceRequirementTypeDef,
+    BatchJobDependencyOutputTypeDef,
     BatchJobDependencyTypeDef,
+    BatchRetryStrategyOutputTypeDef,
     BatchRetryStrategyTypeDef,
+    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
-    CreatePipeResponseTypeDef,
+    ResponseMetadataTypeDef,
+    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeletePipeRequestRequestTypeDef,
-    DeletePipeResponseTypeDef,
     DescribePipeRequestRequestTypeDef,
+    EcsEnvironmentFileOutputTypeDef,
+    EcsEnvironmentVariableOutputTypeDef,
+    EcsResourceRequirementOutputTypeDef,
     EcsEnvironmentFileTypeDef,
     EcsEnvironmentVariableTypeDef,
     EcsResourceRequirementTypeDef,
+    EcsEphemeralStorageOutputTypeDef,
     EcsEphemeralStorageTypeDef,
+    EcsInferenceAcceleratorOverrideOutputTypeDef,
     EcsInferenceAcceleratorOverrideTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
-    ListPipesRequestListPipesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPipesRequestRequestTypeDef,
     PipeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    MQBrokerAccessCredentialsOutputTypeDef,
     MQBrokerAccessCredentialsTypeDef,
+    MSKAccessCredentialsOutputTypeDef,
     MSKAccessCredentialsTypeDef,
-    PaginatorConfigTypeDef,
+    PipeEnrichmentHttpParametersOutputTypeDef,
     PipeEnrichmentHttpParametersTypeDef,
+    PipeSourceSqsQueueParametersOutputTypeDef,
     PipeSourceSqsQueueParametersTypeDef,
+    SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef,
+    SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
     SelfManagedKafkaAccessConfigurationVpcTypeDef,
+    PipeTargetCloudWatchLogsParametersOutputTypeDef,
     PipeTargetCloudWatchLogsParametersTypeDef,
+    PlacementConstraintOutputTypeDef,
+    PlacementStrategyOutputTypeDef,
+    TagOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     TagTypeDef,
+    PipeTargetEventBridgeEventBusParametersOutputTypeDef,
     PipeTargetEventBridgeEventBusParametersTypeDef,
+    PipeTargetHttpParametersOutputTypeDef,
     PipeTargetHttpParametersTypeDef,
+    PipeTargetKinesisStreamParametersOutputTypeDef,
     PipeTargetKinesisStreamParametersTypeDef,
+    PipeTargetLambdaFunctionParametersOutputTypeDef,
     PipeTargetLambdaFunctionParametersTypeDef,
+    PipeTargetRedshiftDataParametersOutputTypeDef,
+    PipeTargetSqsQueueParametersOutputTypeDef,
+    PipeTargetStateMachineParametersOutputTypeDef,
     PipeTargetRedshiftDataParametersTypeDef,
     PipeTargetSqsQueueParametersTypeDef,
     PipeTargetStateMachineParametersTypeDef,
+    SageMakerPipelineParameterOutputTypeDef,
     SageMakerPipelineParameterTypeDef,
-    ResponseMetadataTypeDef,
     StartPipeRequestRequestTypeDef,
-    StartPipeResponseTypeDef,
     StopPipeRequestRequestTypeDef,
-    StopPipeResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdatePipeResponseTypeDef,
     UpdatePipeSourceSqsQueueParametersTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
+    BatchContainerOverridesOutputTypeDef,
     BatchContainerOverridesTypeDef,
+    CreatePipeResponseTypeDef,
+    DeletePipeResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartPipeResponseTypeDef,
+    StopPipeResponseTypeDef,
+    UpdatePipeResponseTypeDef,
+    PipeSourceDynamoDBStreamParametersOutputTypeDef,
+    PipeSourceKinesisStreamParametersOutputTypeDef,
     PipeSourceDynamoDBStreamParametersTypeDef,
     PipeSourceKinesisStreamParametersTypeDef,
     UpdatePipeSourceDynamoDBStreamParametersTypeDef,
     UpdatePipeSourceKinesisStreamParametersTypeDef,
+    EcsContainerOverrideOutputTypeDef,
     EcsContainerOverrideTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
+    ListPipesRequestListPipesPaginateTypeDef,
     ListPipesResponseTypeDef,
+    PipeSourceActiveMQBrokerParametersOutputTypeDef,
+    PipeSourceRabbitMQBrokerParametersOutputTypeDef,
     PipeSourceActiveMQBrokerParametersTypeDef,
     PipeSourceRabbitMQBrokerParametersTypeDef,
     UpdatePipeSourceActiveMQBrokerParametersTypeDef,
     UpdatePipeSourceRabbitMQBrokerParametersTypeDef,
+    PipeSourceManagedStreamingKafkaParametersOutputTypeDef,
     PipeSourceManagedStreamingKafkaParametersTypeDef,
     UpdatePipeSourceManagedStreamingKafkaParametersTypeDef,
+    PipeEnrichmentParametersOutputTypeDef,
     PipeEnrichmentParametersTypeDef,
+    PipeSourceSelfManagedKafkaParametersOutputTypeDef,
     PipeSourceSelfManagedKafkaParametersTypeDef,
     UpdatePipeSourceSelfManagedKafkaParametersTypeDef,
+    PipeTargetSageMakerPipelineParametersOutputTypeDef,
     PipeTargetSageMakerPipelineParametersTypeDef,
+    PipeTargetBatchJobParametersOutputTypeDef,
     PipeTargetBatchJobParametersTypeDef,
+    EcsTaskOverrideOutputTypeDef,
     EcsTaskOverrideTypeDef,
+    PipeSourceParametersOutputTypeDef,
     PipeSourceParametersTypeDef,
     UpdatePipeSourceParametersTypeDef,
+    PipeTargetEcsTaskParametersOutputTypeDef,
     PipeTargetEcsTaskParametersTypeDef,
+    PipeTargetParametersOutputTypeDef,
     PipeTargetParametersTypeDef,
-    CreatePipeRequestRequestTypeDef,
     DescribePipeResponseTypeDef,
+    CreatePipeRequestRequestTypeDef,
     UpdatePipeRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AwsVpcConfigurationTypeDef:
+def get_structure() -> AwsVpcConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pipes-1.28.0/README.md` & `mypy-boto3-pipes-1.28.12/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-pipes"></a>
 
 # mypy-boto3-pipes
 
 [![PyPI - mypy-boto3-pipes](https://img.shields.io/pypi/v/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pipes?color=blue)](https://pypistats.org/packages/mypy-boto3-pipes)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pipes)](https://pepy.tech/project/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,97 +304,146 @@
 ### Typed dictionaries
 
 `mypy_boto3_pipes.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pipes.type_defs import (
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
+    BatchArrayPropertiesOutputTypeDef,
     BatchArrayPropertiesTypeDef,
+    BatchEnvironmentVariableOutputTypeDef,
+    BatchResourceRequirementOutputTypeDef,
     BatchEnvironmentVariableTypeDef,
     BatchResourceRequirementTypeDef,
+    BatchJobDependencyOutputTypeDef,
     BatchJobDependencyTypeDef,
+    BatchRetryStrategyOutputTypeDef,
     BatchRetryStrategyTypeDef,
+    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
-    CreatePipeResponseTypeDef,
+    ResponseMetadataTypeDef,
+    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeletePipeRequestRequestTypeDef,
-    DeletePipeResponseTypeDef,
     DescribePipeRequestRequestTypeDef,
+    EcsEnvironmentFileOutputTypeDef,
+    EcsEnvironmentVariableOutputTypeDef,
+    EcsResourceRequirementOutputTypeDef,
     EcsEnvironmentFileTypeDef,
     EcsEnvironmentVariableTypeDef,
     EcsResourceRequirementTypeDef,
+    EcsEphemeralStorageOutputTypeDef,
     EcsEphemeralStorageTypeDef,
+    EcsInferenceAcceleratorOverrideOutputTypeDef,
     EcsInferenceAcceleratorOverrideTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
-    ListPipesRequestListPipesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPipesRequestRequestTypeDef,
     PipeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    MQBrokerAccessCredentialsOutputTypeDef,
     MQBrokerAccessCredentialsTypeDef,
+    MSKAccessCredentialsOutputTypeDef,
     MSKAccessCredentialsTypeDef,
-    PaginatorConfigTypeDef,
+    PipeEnrichmentHttpParametersOutputTypeDef,
     PipeEnrichmentHttpParametersTypeDef,
+    PipeSourceSqsQueueParametersOutputTypeDef,
     PipeSourceSqsQueueParametersTypeDef,
+    SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef,
+    SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
     SelfManagedKafkaAccessConfigurationVpcTypeDef,
+    PipeTargetCloudWatchLogsParametersOutputTypeDef,
     PipeTargetCloudWatchLogsParametersTypeDef,
+    PlacementConstraintOutputTypeDef,
+    PlacementStrategyOutputTypeDef,
+    TagOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     TagTypeDef,
+    PipeTargetEventBridgeEventBusParametersOutputTypeDef,
     PipeTargetEventBridgeEventBusParametersTypeDef,
+    PipeTargetHttpParametersOutputTypeDef,
     PipeTargetHttpParametersTypeDef,
+    PipeTargetKinesisStreamParametersOutputTypeDef,
     PipeTargetKinesisStreamParametersTypeDef,
+    PipeTargetLambdaFunctionParametersOutputTypeDef,
     PipeTargetLambdaFunctionParametersTypeDef,
+    PipeTargetRedshiftDataParametersOutputTypeDef,
+    PipeTargetSqsQueueParametersOutputTypeDef,
+    PipeTargetStateMachineParametersOutputTypeDef,
     PipeTargetRedshiftDataParametersTypeDef,
     PipeTargetSqsQueueParametersTypeDef,
     PipeTargetStateMachineParametersTypeDef,
+    SageMakerPipelineParameterOutputTypeDef,
     SageMakerPipelineParameterTypeDef,
-    ResponseMetadataTypeDef,
     StartPipeRequestRequestTypeDef,
-    StartPipeResponseTypeDef,
     StopPipeRequestRequestTypeDef,
-    StopPipeResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdatePipeResponseTypeDef,
     UpdatePipeSourceSqsQueueParametersTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
+    BatchContainerOverridesOutputTypeDef,
     BatchContainerOverridesTypeDef,
+    CreatePipeResponseTypeDef,
+    DeletePipeResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartPipeResponseTypeDef,
+    StopPipeResponseTypeDef,
+    UpdatePipeResponseTypeDef,
+    PipeSourceDynamoDBStreamParametersOutputTypeDef,
+    PipeSourceKinesisStreamParametersOutputTypeDef,
     PipeSourceDynamoDBStreamParametersTypeDef,
     PipeSourceKinesisStreamParametersTypeDef,
     UpdatePipeSourceDynamoDBStreamParametersTypeDef,
     UpdatePipeSourceKinesisStreamParametersTypeDef,
+    EcsContainerOverrideOutputTypeDef,
     EcsContainerOverrideTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
+    ListPipesRequestListPipesPaginateTypeDef,
     ListPipesResponseTypeDef,
+    PipeSourceActiveMQBrokerParametersOutputTypeDef,
+    PipeSourceRabbitMQBrokerParametersOutputTypeDef,
     PipeSourceActiveMQBrokerParametersTypeDef,
     PipeSourceRabbitMQBrokerParametersTypeDef,
     UpdatePipeSourceActiveMQBrokerParametersTypeDef,
     UpdatePipeSourceRabbitMQBrokerParametersTypeDef,
+    PipeSourceManagedStreamingKafkaParametersOutputTypeDef,
     PipeSourceManagedStreamingKafkaParametersTypeDef,
     UpdatePipeSourceManagedStreamingKafkaParametersTypeDef,
+    PipeEnrichmentParametersOutputTypeDef,
     PipeEnrichmentParametersTypeDef,
+    PipeSourceSelfManagedKafkaParametersOutputTypeDef,
     PipeSourceSelfManagedKafkaParametersTypeDef,
     UpdatePipeSourceSelfManagedKafkaParametersTypeDef,
+    PipeTargetSageMakerPipelineParametersOutputTypeDef,
     PipeTargetSageMakerPipelineParametersTypeDef,
+    PipeTargetBatchJobParametersOutputTypeDef,
     PipeTargetBatchJobParametersTypeDef,
+    EcsTaskOverrideOutputTypeDef,
     EcsTaskOverrideTypeDef,
+    PipeSourceParametersOutputTypeDef,
     PipeSourceParametersTypeDef,
     UpdatePipeSourceParametersTypeDef,
+    PipeTargetEcsTaskParametersOutputTypeDef,
     PipeTargetEcsTaskParametersTypeDef,
+    PipeTargetParametersOutputTypeDef,
     PipeTargetParametersTypeDef,
-    CreatePipeRequestRequestTypeDef,
     DescribePipeResponseTypeDef,
+    CreatePipeRequestRequestTypeDef,
     UpdatePipeRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AwsVpcConfigurationTypeDef:
+def get_structure() -> AwsVpcConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/__init__.py` & `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/__init__.pyi` & `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/__main__.py` & `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridgePipes 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.EventBridgePipes 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes\nOther"
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

### Comparing `mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/client.py` & `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/client.pyi` & `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/literals.py` & `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,15 @@
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
@@ -280,26 +281,28 @@
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

### Comparing `mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/literals.pyi` & `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,15 @@
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
@@ -278,26 +279,28 @@
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

### Comparing `mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/paginator.py` & `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,38 +24,35 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import PipeStateType, RequestedPipeStateType
 from .type_defs import ListPipesResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListPipesPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListPipesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Paginator.ListPipes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/paginators/#listpipespaginator)
     """
 
     def paginate(
         self,
         *,
         CurrentState: PipeStateType = ...,
         DesiredState: RequestedPipeStateType = ...,
         NamePrefix: str = ...,
         SourcePrefix: str = ...,
         TargetPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Paginator.ListPipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/paginators/#listpipespaginator)
         """
```

### Comparing `mypy-boto3-pipes-1.28.0/mypy_boto3_pipes/paginator.pyi` & `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,35 +24,38 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import PipeStateType, RequestedPipeStateType
 from .type_defs import ListPipesResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListPipesPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListPipesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Paginator.ListPipes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/paginators/#listpipespaginator)
     """
 
     def paginate(
         self,
         *,
         CurrentState: PipeStateType = ...,
         DesiredState: RequestedPipeStateType = ...,
         NamePrefix: str = ...,
         SourcePrefix: str = ...,
         TargetPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Paginator.ListPipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/paginators/#listpipespaginator)
         """
```

### Comparing `mypy-boto3-pipes-1.28.0/mypy_boto3_pipes.egg-info/PKG-INFO` & `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pipes
-Version: 1.28.0
-Summary: Type annotations for boto3.EventBridgePipes 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EventBridgePipes 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-pipes"></a>
 
 # mypy-boto3-pipes
 
 [![PyPI - mypy-boto3-pipes](https://img.shields.io/pypi/v/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pipes.svg?color=blue)](https://pypi.org/project/mypy-boto3-pipes)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pipes?color=blue)](https://pypistats.org/packages/mypy-boto3-pipes)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pipes)](https://pepy.tech/project/mypy-boto3-pipes)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridgePipes 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
+[boto3.EventBridgePipes 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
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
 [mypy-boto3-pipes docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pipes/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,97 +336,146 @@
 ### Typed dictionaries
 
 `mypy_boto3_pipes.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pipes.type_defs import (
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
+    BatchArrayPropertiesOutputTypeDef,
     BatchArrayPropertiesTypeDef,
+    BatchEnvironmentVariableOutputTypeDef,
+    BatchResourceRequirementOutputTypeDef,
     BatchEnvironmentVariableTypeDef,
     BatchResourceRequirementTypeDef,
+    BatchJobDependencyOutputTypeDef,
     BatchJobDependencyTypeDef,
+    BatchRetryStrategyOutputTypeDef,
     BatchRetryStrategyTypeDef,
+    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
-    CreatePipeResponseTypeDef,
+    ResponseMetadataTypeDef,
+    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeletePipeRequestRequestTypeDef,
-    DeletePipeResponseTypeDef,
     DescribePipeRequestRequestTypeDef,
+    EcsEnvironmentFileOutputTypeDef,
+    EcsEnvironmentVariableOutputTypeDef,
+    EcsResourceRequirementOutputTypeDef,
     EcsEnvironmentFileTypeDef,
     EcsEnvironmentVariableTypeDef,
     EcsResourceRequirementTypeDef,
+    EcsEphemeralStorageOutputTypeDef,
     EcsEphemeralStorageTypeDef,
+    EcsInferenceAcceleratorOverrideOutputTypeDef,
     EcsInferenceAcceleratorOverrideTypeDef,
+    FilterOutputTypeDef,
     FilterTypeDef,
-    ListPipesRequestListPipesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPipesRequestRequestTypeDef,
     PipeTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    MQBrokerAccessCredentialsOutputTypeDef,
     MQBrokerAccessCredentialsTypeDef,
+    MSKAccessCredentialsOutputTypeDef,
     MSKAccessCredentialsTypeDef,
-    PaginatorConfigTypeDef,
+    PipeEnrichmentHttpParametersOutputTypeDef,
     PipeEnrichmentHttpParametersTypeDef,
+    PipeSourceSqsQueueParametersOutputTypeDef,
     PipeSourceSqsQueueParametersTypeDef,
+    SelfManagedKafkaAccessConfigurationCredentialsOutputTypeDef,
+    SelfManagedKafkaAccessConfigurationVpcOutputTypeDef,
     SelfManagedKafkaAccessConfigurationCredentialsTypeDef,
     SelfManagedKafkaAccessConfigurationVpcTypeDef,
+    PipeTargetCloudWatchLogsParametersOutputTypeDef,
     PipeTargetCloudWatchLogsParametersTypeDef,
+    PlacementConstraintOutputTypeDef,
+    PlacementStrategyOutputTypeDef,
+    TagOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     TagTypeDef,
+    PipeTargetEventBridgeEventBusParametersOutputTypeDef,
     PipeTargetEventBridgeEventBusParametersTypeDef,
+    PipeTargetHttpParametersOutputTypeDef,
     PipeTargetHttpParametersTypeDef,
+    PipeTargetKinesisStreamParametersOutputTypeDef,
     PipeTargetKinesisStreamParametersTypeDef,
+    PipeTargetLambdaFunctionParametersOutputTypeDef,
     PipeTargetLambdaFunctionParametersTypeDef,
+    PipeTargetRedshiftDataParametersOutputTypeDef,
+    PipeTargetSqsQueueParametersOutputTypeDef,
+    PipeTargetStateMachineParametersOutputTypeDef,
     PipeTargetRedshiftDataParametersTypeDef,
     PipeTargetSqsQueueParametersTypeDef,
     PipeTargetStateMachineParametersTypeDef,
+    SageMakerPipelineParameterOutputTypeDef,
     SageMakerPipelineParameterTypeDef,
-    ResponseMetadataTypeDef,
     StartPipeRequestRequestTypeDef,
-    StartPipeResponseTypeDef,
     StopPipeRequestRequestTypeDef,
-    StopPipeResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdatePipeResponseTypeDef,
     UpdatePipeSourceSqsQueueParametersTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
+    BatchContainerOverridesOutputTypeDef,
     BatchContainerOverridesTypeDef,
+    CreatePipeResponseTypeDef,
+    DeletePipeResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartPipeResponseTypeDef,
+    StopPipeResponseTypeDef,
+    UpdatePipeResponseTypeDef,
+    PipeSourceDynamoDBStreamParametersOutputTypeDef,
+    PipeSourceKinesisStreamParametersOutputTypeDef,
     PipeSourceDynamoDBStreamParametersTypeDef,
     PipeSourceKinesisStreamParametersTypeDef,
     UpdatePipeSourceDynamoDBStreamParametersTypeDef,
     UpdatePipeSourceKinesisStreamParametersTypeDef,
+    EcsContainerOverrideOutputTypeDef,
     EcsContainerOverrideTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
+    ListPipesRequestListPipesPaginateTypeDef,
     ListPipesResponseTypeDef,
+    PipeSourceActiveMQBrokerParametersOutputTypeDef,
+    PipeSourceRabbitMQBrokerParametersOutputTypeDef,
     PipeSourceActiveMQBrokerParametersTypeDef,
     PipeSourceRabbitMQBrokerParametersTypeDef,
     UpdatePipeSourceActiveMQBrokerParametersTypeDef,
     UpdatePipeSourceRabbitMQBrokerParametersTypeDef,
+    PipeSourceManagedStreamingKafkaParametersOutputTypeDef,
     PipeSourceManagedStreamingKafkaParametersTypeDef,
     UpdatePipeSourceManagedStreamingKafkaParametersTypeDef,
+    PipeEnrichmentParametersOutputTypeDef,
     PipeEnrichmentParametersTypeDef,
+    PipeSourceSelfManagedKafkaParametersOutputTypeDef,
     PipeSourceSelfManagedKafkaParametersTypeDef,
     UpdatePipeSourceSelfManagedKafkaParametersTypeDef,
+    PipeTargetSageMakerPipelineParametersOutputTypeDef,
     PipeTargetSageMakerPipelineParametersTypeDef,
+    PipeTargetBatchJobParametersOutputTypeDef,
     PipeTargetBatchJobParametersTypeDef,
+    EcsTaskOverrideOutputTypeDef,
     EcsTaskOverrideTypeDef,
+    PipeSourceParametersOutputTypeDef,
     PipeSourceParametersTypeDef,
     UpdatePipeSourceParametersTypeDef,
+    PipeTargetEcsTaskParametersOutputTypeDef,
     PipeTargetEcsTaskParametersTypeDef,
+    PipeTargetParametersOutputTypeDef,
     PipeTargetParametersTypeDef,
-    CreatePipeRequestRequestTypeDef,
     DescribePipeResponseTypeDef,
+    CreatePipeRequestRequestTypeDef,
     UpdatePipeRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AwsVpcConfigurationTypeDef:
+def get_structure() -> AwsVpcConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-pipes-1.28.0/mypy_boto3_pipes.egg-info/SOURCES.txt` & `mypy-boto3-pipes-1.28.12/mypy_boto3_pipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pipes-1.28.0/setup.py` & `mypy-boto3-pipes-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pipes",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_pipes"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EventBridgePipes 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.EventBridgePipes 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

