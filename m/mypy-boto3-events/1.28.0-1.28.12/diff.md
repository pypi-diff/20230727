# Comparing `tmp/mypy-boto3-events-1.28.0.tar.gz` & `tmp/mypy-boto3-events-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-events-1.28.0.tar", last modified: Thu Jul  6 20:59:34 2023, max compression
+gzip compressed data, was "mypy-boto3-events-1.28.12.tar", last modified: Thu Jul 27 05:34:40 2023, max compression
```

## Comparing `mypy-boto3-events-1.28.0.tar` & `mypy-boto3-events-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:34.294301 mypy-boto3-events-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:48.000000 mypy-boto3-events-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19759 2023-07-06 20:59:34.290301 mypy-boto3-events-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-07-06 20:40:48.000000 mypy-boto3-events-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:34.274301 mypy-boto3-events-1.28.0/mypy_boto3_events/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-06 20:40:48.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 20:40:48.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-06 20:40:48.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37779 2023-07-06 20:40:49.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37713 2023-07-06 20:40:49.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-06 20:40:49.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-07-06 20:40:49.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-06 20:40:49.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-06 20:40:49.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:48.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59050 2023-07-06 20:40:53.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58981 2023-07-06 20:40:52.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:48.000000 mypy-boto3-events-1.28.0/mypy_boto3_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:34.290301 mypy-boto3-events-1.28.0/mypy_boto3_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19759 2023-07-06 20:59:34.000000 mypy-boto3-events-1.28.0/mypy_boto3_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 20:59:34.000000 mypy-boto3-events-1.28.0/mypy_boto3_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:34.000000 mypy-boto3-events-1.28.0/mypy_boto3_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:34.000000 mypy-boto3-events-1.28.0/mypy_boto3_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:34.000000 mypy-boto3-events-1.28.0/mypy_boto3_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 20:59:34.000000 mypy-boto3-events-1.28.0/mypy_boto3_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:34.294301 mypy-boto3-events-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-06 20:40:48.000000 mypy-boto3-events-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.920513 mypy-boto3-events-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-07-27 05:34:40.920513 mypy-boto3-events-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19456 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.912513 mypy-boto3-events-1.28.12/mypy_boto3_events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37779 2023-07-27 05:22:09.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37713 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-27 05:22:09.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-27 05:22:09.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-27 05:22:09.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-27 05:22:09.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69913 2023-07-27 05:22:10.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69828 2023-07-27 05:22:09.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/mypy_boto3_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.920513 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-07-27 05:34:40.000000 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:40.000000 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:40.000000 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:40.000000 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:40.000000 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:40.000000 mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:40.920513 mypy-boto3-events-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-27 05:22:08.000000 mypy-boto3-events-1.28.12/setup.py
```

### Comparing `mypy-boto3-events-1.28.0/LICENSE` & `mypy-boto3-events-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.0/PKG-INFO` & `mypy-boto3-events-1.28.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-events
-Version: 1.28.0
-Summary: Type annotations for boto3.EventBridge 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EventBridge 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-events"></a>
 
 # mypy-boto3-events
 
 [![PyPI - mypy-boto3-events](https://img.shields.io/pypi/v/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-events?color=blue)](https://pypistats.org/packages/mypy-boto3-events)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-events)](https://pepy.tech/project/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,43 +349,53 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_events.type_defs import (
     ActivateEventSourceRequestRequestTypeDef,
     ApiDestinationTypeDef,
     ArchiveTypeDef,
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
+    BatchArrayPropertiesOutputTypeDef,
     BatchArrayPropertiesTypeDef,
+    BatchRetryStrategyOutputTypeDef,
     BatchRetryStrategyTypeDef,
     CancelReplayRequestRequestTypeDef,
     CancelReplayResponseTypeDef,
+    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ConditionTypeDef,
     ConnectionApiKeyAuthResponseParametersTypeDef,
     ConnectionBasicAuthResponseParametersTypeDef,
+    ConnectionBodyParameterOutputTypeDef,
     ConnectionBodyParameterTypeDef,
+    ConnectionHeaderParameterOutputTypeDef,
     ConnectionHeaderParameterTypeDef,
+    ConnectionQueryStringParameterOutputTypeDef,
     ConnectionQueryStringParameterTypeDef,
     ConnectionOAuthClientResponseParametersTypeDef,
     ConnectionTypeDef,
     CreateApiDestinationRequestRequestTypeDef,
     CreateApiDestinationResponseTypeDef,
     CreateArchiveRequestRequestTypeDef,
     CreateArchiveResponseTypeDef,
     CreateConnectionApiKeyAuthRequestParametersTypeDef,
     CreateConnectionBasicAuthRequestParametersTypeDef,
     CreateConnectionOAuthClientRequestParametersTypeDef,
     CreateConnectionResponseTypeDef,
     EndpointEventBusTypeDef,
     ReplicationConfigTypeDef,
+    EndpointEventBusOutputTypeDef,
+    ReplicationConfigOutputTypeDef,
     TagTypeDef,
     CreateEventBusResponseTypeDef,
     CreatePartnerEventSourceRequestRequestTypeDef,
     CreatePartnerEventSourceResponseTypeDef,
     DeactivateEventSourceRequestRequestTypeDef,
+    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeauthorizeConnectionRequestRequestTypeDef,
     DeauthorizeConnectionResponseTypeDef,
     DeleteApiDestinationRequestRequestTypeDef,
     DeleteArchiveRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteConnectionResponseTypeDef,
@@ -402,28 +412,36 @@
     DescribeEventBusRequestRequestTypeDef,
     DescribeEventBusResponseTypeDef,
     DescribeEventSourceRequestRequestTypeDef,
     DescribeEventSourceResponseTypeDef,
     DescribePartnerEventSourceRequestRequestTypeDef,
     DescribePartnerEventSourceResponseTypeDef,
     DescribeReplayRequestRequestTypeDef,
-    ReplayDestinationTypeDef,
+    ReplayDestinationOutputTypeDef,
     DescribeRuleRequestRequestTypeDef,
     DescribeRuleResponseTypeDef,
     DisableRuleRequestRequestTypeDef,
+    PlacementConstraintOutputTypeDef,
+    PlacementStrategyOutputTypeDef,
+    TagOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableRuleRequestRequestTypeDef,
     EventBusTypeDef,
     EventSourceTypeDef,
+    PrimaryOutputTypeDef,
+    SecondaryOutputTypeDef,
     PrimaryTypeDef,
     SecondaryTypeDef,
+    HttpParametersOutputTypeDef,
     HttpParametersTypeDef,
+    InputTransformerOutputTypeDef,
     InputTransformerTypeDef,
+    KinesisParametersOutputTypeDef,
     KinesisParametersTypeDef,
     ListApiDestinationsRequestRequestTypeDef,
     ListArchivesRequestRequestTypeDef,
     ListConnectionsRequestRequestTypeDef,
     ListEndpointsRequestRequestTypeDef,
     ListEventBusesRequestRequestTypeDef,
     ListEventSourcesRequestRequestTypeDef,
@@ -445,22 +463,28 @@
     PaginatorConfigTypeDef,
     PutEventsRequestEntryTypeDef,
     PutEventsResultEntryTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResultEntryTypeDef,
     PutRuleResponseTypeDef,
     PutTargetsResultEntryTypeDef,
+    RedshiftDataParametersOutputTypeDef,
     RedshiftDataParametersTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RemoveTargetsRequestRequestTypeDef,
     RemoveTargetsResultEntryTypeDef,
+    ReplayDestinationTypeDef,
     ResponseMetadataTypeDef,
+    RetryPolicyOutputTypeDef,
     RetryPolicyTypeDef,
+    RunCommandTargetOutputTypeDef,
     RunCommandTargetTypeDef,
+    SageMakerPipelineParameterOutputTypeDef,
     SageMakerPipelineParameterTypeDef,
+    SqsParametersOutputTypeDef,
     SqsParametersTypeDef,
     StartReplayResponseTypeDef,
     TestEventPatternRequestRequestTypeDef,
     TestEventPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiDestinationRequestRequestTypeDef,
     UpdateApiDestinationResponseTypeDef,
@@ -468,55 +492,64 @@
     UpdateArchiveResponseTypeDef,
     UpdateConnectionApiKeyAuthRequestParametersTypeDef,
     UpdateConnectionBasicAuthRequestParametersTypeDef,
     UpdateConnectionOAuthClientRequestParametersTypeDef,
     UpdateConnectionResponseTypeDef,
     ListApiDestinationsResponseTypeDef,
     ListArchivesResponseTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
+    BatchParametersOutputTypeDef,
     BatchParametersTypeDef,
     PutPermissionRequestRequestTypeDef,
+    ConnectionHttpParametersOutputTypeDef,
     ConnectionHttpParametersTypeDef,
     ListConnectionsResponseTypeDef,
     CreateEventBusRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutRuleRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     DescribeReplayResponseTypeDef,
-    StartReplayRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListEventBusesResponseTypeDef,
     ListEventSourcesResponseTypeDef,
+    FailoverConfigOutputTypeDef,
     FailoverConfigTypeDef,
     ListPartnerEventSourceAccountsResponseTypeDef,
     ListPartnerEventSourcesResponseTypeDef,
     ListReplaysResponseTypeDef,
     ListRulesResponseTypeDef,
     PutEventsRequestRequestTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestRequestTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
+    StartReplayRequestRequestTypeDef,
+    RunCommandParametersOutputTypeDef,
     RunCommandParametersTypeDef,
+    SageMakerPipelineParametersOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
+    EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ConnectionOAuthResponseParametersTypeDef,
     CreateConnectionOAuthRequestParametersTypeDef,
     UpdateConnectionOAuthRequestParametersTypeDef,
+    RoutingConfigOutputTypeDef,
     RoutingConfigTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
     ConnectionAuthResponseParametersTypeDef,
     CreateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
-    CreateEndpointRequestRequestTypeDef,
     CreateEndpointResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     EndpointTypeDef,
-    UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
+    CreateEndpointRequestRequestTypeDef,
+    UpdateEndpointRequestRequestTypeDef,
     ListTargetsByRuleResponseTypeDef,
     PutTargetsRequestRequestTypeDef,
     DescribeConnectionResponseTypeDef,
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     ListEndpointsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-events-1.28.0/README.md` & `mypy-boto3-events-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-events"></a>
 
 # mypy-boto3-events
 
 [![PyPI - mypy-boto3-events](https://img.shields.io/pypi/v/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-events?color=blue)](https://pypistats.org/packages/mypy-boto3-events)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-events)](https://pepy.tech/project/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,43 +317,53 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_events.type_defs import (
     ActivateEventSourceRequestRequestTypeDef,
     ApiDestinationTypeDef,
     ArchiveTypeDef,
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
+    BatchArrayPropertiesOutputTypeDef,
     BatchArrayPropertiesTypeDef,
+    BatchRetryStrategyOutputTypeDef,
     BatchRetryStrategyTypeDef,
     CancelReplayRequestRequestTypeDef,
     CancelReplayResponseTypeDef,
+    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ConditionTypeDef,
     ConnectionApiKeyAuthResponseParametersTypeDef,
     ConnectionBasicAuthResponseParametersTypeDef,
+    ConnectionBodyParameterOutputTypeDef,
     ConnectionBodyParameterTypeDef,
+    ConnectionHeaderParameterOutputTypeDef,
     ConnectionHeaderParameterTypeDef,
+    ConnectionQueryStringParameterOutputTypeDef,
     ConnectionQueryStringParameterTypeDef,
     ConnectionOAuthClientResponseParametersTypeDef,
     ConnectionTypeDef,
     CreateApiDestinationRequestRequestTypeDef,
     CreateApiDestinationResponseTypeDef,
     CreateArchiveRequestRequestTypeDef,
     CreateArchiveResponseTypeDef,
     CreateConnectionApiKeyAuthRequestParametersTypeDef,
     CreateConnectionBasicAuthRequestParametersTypeDef,
     CreateConnectionOAuthClientRequestParametersTypeDef,
     CreateConnectionResponseTypeDef,
     EndpointEventBusTypeDef,
     ReplicationConfigTypeDef,
+    EndpointEventBusOutputTypeDef,
+    ReplicationConfigOutputTypeDef,
     TagTypeDef,
     CreateEventBusResponseTypeDef,
     CreatePartnerEventSourceRequestRequestTypeDef,
     CreatePartnerEventSourceResponseTypeDef,
     DeactivateEventSourceRequestRequestTypeDef,
+    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeauthorizeConnectionRequestRequestTypeDef,
     DeauthorizeConnectionResponseTypeDef,
     DeleteApiDestinationRequestRequestTypeDef,
     DeleteArchiveRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteConnectionResponseTypeDef,
@@ -370,28 +380,36 @@
     DescribeEventBusRequestRequestTypeDef,
     DescribeEventBusResponseTypeDef,
     DescribeEventSourceRequestRequestTypeDef,
     DescribeEventSourceResponseTypeDef,
     DescribePartnerEventSourceRequestRequestTypeDef,
     DescribePartnerEventSourceResponseTypeDef,
     DescribeReplayRequestRequestTypeDef,
-    ReplayDestinationTypeDef,
+    ReplayDestinationOutputTypeDef,
     DescribeRuleRequestRequestTypeDef,
     DescribeRuleResponseTypeDef,
     DisableRuleRequestRequestTypeDef,
+    PlacementConstraintOutputTypeDef,
+    PlacementStrategyOutputTypeDef,
+    TagOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableRuleRequestRequestTypeDef,
     EventBusTypeDef,
     EventSourceTypeDef,
+    PrimaryOutputTypeDef,
+    SecondaryOutputTypeDef,
     PrimaryTypeDef,
     SecondaryTypeDef,
+    HttpParametersOutputTypeDef,
     HttpParametersTypeDef,
+    InputTransformerOutputTypeDef,
     InputTransformerTypeDef,
+    KinesisParametersOutputTypeDef,
     KinesisParametersTypeDef,
     ListApiDestinationsRequestRequestTypeDef,
     ListArchivesRequestRequestTypeDef,
     ListConnectionsRequestRequestTypeDef,
     ListEndpointsRequestRequestTypeDef,
     ListEventBusesRequestRequestTypeDef,
     ListEventSourcesRequestRequestTypeDef,
@@ -413,22 +431,28 @@
     PaginatorConfigTypeDef,
     PutEventsRequestEntryTypeDef,
     PutEventsResultEntryTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResultEntryTypeDef,
     PutRuleResponseTypeDef,
     PutTargetsResultEntryTypeDef,
+    RedshiftDataParametersOutputTypeDef,
     RedshiftDataParametersTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RemoveTargetsRequestRequestTypeDef,
     RemoveTargetsResultEntryTypeDef,
+    ReplayDestinationTypeDef,
     ResponseMetadataTypeDef,
+    RetryPolicyOutputTypeDef,
     RetryPolicyTypeDef,
+    RunCommandTargetOutputTypeDef,
     RunCommandTargetTypeDef,
+    SageMakerPipelineParameterOutputTypeDef,
     SageMakerPipelineParameterTypeDef,
+    SqsParametersOutputTypeDef,
     SqsParametersTypeDef,
     StartReplayResponseTypeDef,
     TestEventPatternRequestRequestTypeDef,
     TestEventPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiDestinationRequestRequestTypeDef,
     UpdateApiDestinationResponseTypeDef,
@@ -436,55 +460,64 @@
     UpdateArchiveResponseTypeDef,
     UpdateConnectionApiKeyAuthRequestParametersTypeDef,
     UpdateConnectionBasicAuthRequestParametersTypeDef,
     UpdateConnectionOAuthClientRequestParametersTypeDef,
     UpdateConnectionResponseTypeDef,
     ListApiDestinationsResponseTypeDef,
     ListArchivesResponseTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
+    BatchParametersOutputTypeDef,
     BatchParametersTypeDef,
     PutPermissionRequestRequestTypeDef,
+    ConnectionHttpParametersOutputTypeDef,
     ConnectionHttpParametersTypeDef,
     ListConnectionsResponseTypeDef,
     CreateEventBusRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutRuleRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     DescribeReplayResponseTypeDef,
-    StartReplayRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListEventBusesResponseTypeDef,
     ListEventSourcesResponseTypeDef,
+    FailoverConfigOutputTypeDef,
     FailoverConfigTypeDef,
     ListPartnerEventSourceAccountsResponseTypeDef,
     ListPartnerEventSourcesResponseTypeDef,
     ListReplaysResponseTypeDef,
     ListRulesResponseTypeDef,
     PutEventsRequestRequestTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestRequestTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
+    StartReplayRequestRequestTypeDef,
+    RunCommandParametersOutputTypeDef,
     RunCommandParametersTypeDef,
+    SageMakerPipelineParametersOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
+    EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ConnectionOAuthResponseParametersTypeDef,
     CreateConnectionOAuthRequestParametersTypeDef,
     UpdateConnectionOAuthRequestParametersTypeDef,
+    RoutingConfigOutputTypeDef,
     RoutingConfigTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
     ConnectionAuthResponseParametersTypeDef,
     CreateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
-    CreateEndpointRequestRequestTypeDef,
     CreateEndpointResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     EndpointTypeDef,
-    UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
+    CreateEndpointRequestRequestTypeDef,
+    UpdateEndpointRequestRequestTypeDef,
     ListTargetsByRuleResponseTypeDef,
     PutTargetsRequestRequestTypeDef,
     DescribeConnectionResponseTypeDef,
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     ListEndpointsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events/__init__.py` & `mypy-boto3-events-1.28.12/mypy_boto3_events/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events/__init__.pyi` & `mypy-boto3-events-1.28.12/mypy_boto3_events/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events/__main__.py` & `mypy-boto3-events-1.28.12/mypy_boto3_events/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EventBridge 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.EventBridge 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge\nOther"
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

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events/client.py` & `mypy-boto3-events-1.28.12/mypy_boto3_events/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events/client.pyi` & `mypy-boto3-events-1.28.12/mypy_boto3_events/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events/literals.py` & `mypy-boto3-events-1.28.12/mypy_boto3_events/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,15 @@
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
@@ -274,26 +275,28 @@
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

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events/literals.pyi` & `mypy-boto3-events-1.28.12/mypy_boto3_events/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,15 @@
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
@@ -272,26 +273,28 @@
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

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events/paginator.py` & `mypy-boto3-events-1.28.12/mypy_boto3_events/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events/paginator.pyi` & `mypy-boto3-events-1.28.12/mypy_boto3_events/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events/type_defs.py` & `mypy-boto3-events-1.28.12/mypy_boto3_events/type_defs.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_events.type_defs import ActivateEventSourceRequestRequestTypeDef
 
     data: ActivateEventSourceRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApiDestinationHttpMethodType,
     ApiDestinationStateType,
     ArchiveStateType,
     AssignPublicIpType,
     ConnectionAuthorizationTypeType,
@@ -43,43 +43,53 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActivateEventSourceRequestRequestTypeDef",
     "ApiDestinationTypeDef",
     "ArchiveTypeDef",
+    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
+    "BatchArrayPropertiesOutputTypeDef",
     "BatchArrayPropertiesTypeDef",
+    "BatchRetryStrategyOutputTypeDef",
     "BatchRetryStrategyTypeDef",
     "CancelReplayRequestRequestTypeDef",
     "CancelReplayResponseTypeDef",
+    "CapacityProviderStrategyItemOutputTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "ConditionTypeDef",
     "ConnectionApiKeyAuthResponseParametersTypeDef",
     "ConnectionBasicAuthResponseParametersTypeDef",
+    "ConnectionBodyParameterOutputTypeDef",
     "ConnectionBodyParameterTypeDef",
+    "ConnectionHeaderParameterOutputTypeDef",
     "ConnectionHeaderParameterTypeDef",
+    "ConnectionQueryStringParameterOutputTypeDef",
     "ConnectionQueryStringParameterTypeDef",
     "ConnectionOAuthClientResponseParametersTypeDef",
     "ConnectionTypeDef",
     "CreateApiDestinationRequestRequestTypeDef",
     "CreateApiDestinationResponseTypeDef",
     "CreateArchiveRequestRequestTypeDef",
     "CreateArchiveResponseTypeDef",
     "CreateConnectionApiKeyAuthRequestParametersTypeDef",
     "CreateConnectionBasicAuthRequestParametersTypeDef",
     "CreateConnectionOAuthClientRequestParametersTypeDef",
     "CreateConnectionResponseTypeDef",
     "EndpointEventBusTypeDef",
     "ReplicationConfigTypeDef",
+    "EndpointEventBusOutputTypeDef",
+    "ReplicationConfigOutputTypeDef",
     "TagTypeDef",
     "CreateEventBusResponseTypeDef",
     "CreatePartnerEventSourceRequestRequestTypeDef",
     "CreatePartnerEventSourceResponseTypeDef",
     "DeactivateEventSourceRequestRequestTypeDef",
+    "DeadLetterConfigOutputTypeDef",
     "DeadLetterConfigTypeDef",
     "DeauthorizeConnectionRequestRequestTypeDef",
     "DeauthorizeConnectionResponseTypeDef",
     "DeleteApiDestinationRequestRequestTypeDef",
     "DeleteArchiveRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteConnectionResponseTypeDef",
@@ -96,28 +106,36 @@
     "DescribeEventBusRequestRequestTypeDef",
     "DescribeEventBusResponseTypeDef",
     "DescribeEventSourceRequestRequestTypeDef",
     "DescribeEventSourceResponseTypeDef",
     "DescribePartnerEventSourceRequestRequestTypeDef",
     "DescribePartnerEventSourceResponseTypeDef",
     "DescribeReplayRequestRequestTypeDef",
-    "ReplayDestinationTypeDef",
+    "ReplayDestinationOutputTypeDef",
     "DescribeRuleRequestRequestTypeDef",
     "DescribeRuleResponseTypeDef",
     "DisableRuleRequestRequestTypeDef",
+    "PlacementConstraintOutputTypeDef",
+    "PlacementStrategyOutputTypeDef",
+    "TagOutputTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableRuleRequestRequestTypeDef",
     "EventBusTypeDef",
     "EventSourceTypeDef",
+    "PrimaryOutputTypeDef",
+    "SecondaryOutputTypeDef",
     "PrimaryTypeDef",
     "SecondaryTypeDef",
+    "HttpParametersOutputTypeDef",
     "HttpParametersTypeDef",
+    "InputTransformerOutputTypeDef",
     "InputTransformerTypeDef",
+    "KinesisParametersOutputTypeDef",
     "KinesisParametersTypeDef",
     "ListApiDestinationsRequestRequestTypeDef",
     "ListArchivesRequestRequestTypeDef",
     "ListConnectionsRequestRequestTypeDef",
     "ListEndpointsRequestRequestTypeDef",
     "ListEventBusesRequestRequestTypeDef",
     "ListEventSourcesRequestRequestTypeDef",
@@ -139,22 +157,28 @@
     "PaginatorConfigTypeDef",
     "PutEventsRequestEntryTypeDef",
     "PutEventsResultEntryTypeDef",
     "PutPartnerEventsRequestEntryTypeDef",
     "PutPartnerEventsResultEntryTypeDef",
     "PutRuleResponseTypeDef",
     "PutTargetsResultEntryTypeDef",
+    "RedshiftDataParametersOutputTypeDef",
     "RedshiftDataParametersTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RemoveTargetsRequestRequestTypeDef",
     "RemoveTargetsResultEntryTypeDef",
+    "ReplayDestinationTypeDef",
     "ResponseMetadataTypeDef",
+    "RetryPolicyOutputTypeDef",
     "RetryPolicyTypeDef",
+    "RunCommandTargetOutputTypeDef",
     "RunCommandTargetTypeDef",
+    "SageMakerPipelineParameterOutputTypeDef",
     "SageMakerPipelineParameterTypeDef",
+    "SqsParametersOutputTypeDef",
     "SqsParametersTypeDef",
     "StartReplayResponseTypeDef",
     "TestEventPatternRequestRequestTypeDef",
     "TestEventPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiDestinationRequestRequestTypeDef",
     "UpdateApiDestinationResponseTypeDef",
@@ -162,55 +186,64 @@
     "UpdateArchiveResponseTypeDef",
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     "UpdateConnectionBasicAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthClientRequestParametersTypeDef",
     "UpdateConnectionResponseTypeDef",
     "ListApiDestinationsResponseTypeDef",
     "ListArchivesResponseTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
+    "BatchParametersOutputTypeDef",
     "BatchParametersTypeDef",
     "PutPermissionRequestRequestTypeDef",
+    "ConnectionHttpParametersOutputTypeDef",
     "ConnectionHttpParametersTypeDef",
     "ListConnectionsResponseTypeDef",
     "CreateEventBusRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PutRuleRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DescribeReplayResponseTypeDef",
-    "StartReplayRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListEventBusesResponseTypeDef",
     "ListEventSourcesResponseTypeDef",
+    "FailoverConfigOutputTypeDef",
     "FailoverConfigTypeDef",
     "ListPartnerEventSourceAccountsResponseTypeDef",
     "ListPartnerEventSourcesResponseTypeDef",
     "ListReplaysResponseTypeDef",
     "ListRulesResponseTypeDef",
     "PutEventsRequestRequestTypeDef",
     "PutEventsResponseTypeDef",
     "PutPartnerEventsRequestRequestTypeDef",
     "PutPartnerEventsResponseTypeDef",
     "PutTargetsResponseTypeDef",
     "RemoveTargetsResponseTypeDef",
+    "StartReplayRequestRequestTypeDef",
+    "RunCommandParametersOutputTypeDef",
     "RunCommandParametersTypeDef",
+    "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
+    "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ConnectionOAuthResponseParametersTypeDef",
     "CreateConnectionOAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthRequestParametersTypeDef",
+    "RoutingConfigOutputTypeDef",
     "RoutingConfigTypeDef",
+    "TargetOutputTypeDef",
     "TargetTypeDef",
     "ConnectionAuthResponseParametersTypeDef",
     "CreateConnectionAuthRequestParametersTypeDef",
     "UpdateConnectionAuthRequestParametersTypeDef",
-    "CreateEndpointRequestRequestTypeDef",
     "CreateEndpointResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "EndpointTypeDef",
-    "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
+    "CreateEndpointRequestRequestTypeDef",
+    "UpdateEndpointRequestRequestTypeDef",
     "ListTargetsByRuleResponseTypeDef",
     "PutTargetsRequestRequestTypeDef",
     "DescribeConnectionResponseTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "ListEndpointsResponseTypeDef",
 )
@@ -249,44 +282,82 @@
         "SizeBytes": int,
         "EventCount": int,
         "CreationTime": datetime,
     },
     total=False,
 )
 
+_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAwsVpcConfigurationOutputTypeDef",
+    {
+        "Subnets": List[str],
+    },
+)
+_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAwsVpcConfigurationOutputTypeDef",
+    {
+        "SecurityGroups": List[str],
+        "AssignPublicIp": AssignPublicIpType,
+    },
+    total=False,
+)
+
+
+class AwsVpcConfigurationOutputTypeDef(
+    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
-        "Subnets": List[str],
+        "Subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
     "_OptionalAwsVpcConfigurationTypeDef",
     {
-        "SecurityGroups": List[str],
+        "SecurityGroups": Sequence[str],
         "AssignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
 
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
 
+BatchArrayPropertiesOutputTypeDef = TypedDict(
+    "BatchArrayPropertiesOutputTypeDef",
+    {
+        "Size": int,
+    },
+    total=False,
+)
+
 BatchArrayPropertiesTypeDef = TypedDict(
     "BatchArrayPropertiesTypeDef",
     {
         "Size": int,
     },
     total=False,
 )
 
+BatchRetryStrategyOutputTypeDef = TypedDict(
+    "BatchRetryStrategyOutputTypeDef",
+    {
+        "Attempts": int,
+    },
+    total=False,
+)
+
 BatchRetryStrategyTypeDef = TypedDict(
     "BatchRetryStrategyTypeDef",
     {
         "Attempts": int,
     },
     total=False,
 )
@@ -304,14 +375,37 @@
         "ReplayArn": str,
         "State": ReplayStateType,
         "StateReason": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCapacityProviderStrategyItemOutputTypeDef = TypedDict(
+    "_RequiredCapacityProviderStrategyItemOutputTypeDef",
+    {
+        "capacityProvider": str,
+    },
+)
+_OptionalCapacityProviderStrategyItemOutputTypeDef = TypedDict(
+    "_OptionalCapacityProviderStrategyItemOutputTypeDef",
+    {
+        "weight": int,
+        "base": int,
+    },
+    total=False,
+)
+
+
+class CapacityProviderStrategyItemOutputTypeDef(
+    _RequiredCapacityProviderStrategyItemOutputTypeDef,
+    _OptionalCapacityProviderStrategyItemOutputTypeDef,
+):
+    pass
+
+
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -351,34 +445,64 @@
     "ConnectionBasicAuthResponseParametersTypeDef",
     {
         "Username": str,
     },
     total=False,
 )
 
+ConnectionBodyParameterOutputTypeDef = TypedDict(
+    "ConnectionBodyParameterOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "IsValueSecret": bool,
+    },
+    total=False,
+)
+
 ConnectionBodyParameterTypeDef = TypedDict(
     "ConnectionBodyParameterTypeDef",
     {
         "Key": str,
         "Value": str,
         "IsValueSecret": bool,
     },
     total=False,
 )
 
+ConnectionHeaderParameterOutputTypeDef = TypedDict(
+    "ConnectionHeaderParameterOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "IsValueSecret": bool,
+    },
+    total=False,
+)
+
 ConnectionHeaderParameterTypeDef = TypedDict(
     "ConnectionHeaderParameterTypeDef",
     {
         "Key": str,
         "Value": str,
         "IsValueSecret": bool,
     },
     total=False,
 )
 
+ConnectionQueryStringParameterOutputTypeDef = TypedDict(
+    "ConnectionQueryStringParameterOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "IsValueSecret": bool,
+    },
+    total=False,
+)
+
 ConnectionQueryStringParameterTypeDef = TypedDict(
     "ConnectionQueryStringParameterTypeDef",
     {
         "Key": str,
         "Value": str,
         "IsValueSecret": bool,
     },
@@ -526,14 +650,29 @@
     "ReplicationConfigTypeDef",
     {
         "State": ReplicationStateType,
     },
     total=False,
 )
 
+EndpointEventBusOutputTypeDef = TypedDict(
+    "EndpointEventBusOutputTypeDef",
+    {
+        "EventBusArn": str,
+    },
+)
+
+ReplicationConfigOutputTypeDef = TypedDict(
+    "ReplicationConfigOutputTypeDef",
+    {
+        "State": ReplicationStateType,
+    },
+    total=False,
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -565,14 +704,22 @@
 DeactivateEventSourceRequestRequestTypeDef = TypedDict(
     "DeactivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeadLetterConfigOutputTypeDef = TypedDict(
+    "DeadLetterConfigOutputTypeDef",
+    {
+        "Arn": str,
+    },
+    total=False,
+)
+
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
@@ -807,31 +954,31 @@
 DescribeReplayRequestRequestTypeDef = TypedDict(
     "DescribeReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
 
-_RequiredReplayDestinationTypeDef = TypedDict(
-    "_RequiredReplayDestinationTypeDef",
+_RequiredReplayDestinationOutputTypeDef = TypedDict(
+    "_RequiredReplayDestinationOutputTypeDef",
     {
         "Arn": str,
     },
 )
-_OptionalReplayDestinationTypeDef = TypedDict(
-    "_OptionalReplayDestinationTypeDef",
+_OptionalReplayDestinationOutputTypeDef = TypedDict(
+    "_OptionalReplayDestinationOutputTypeDef",
     {
         "FilterArns": List[str],
     },
     total=False,
 )
 
 
-class ReplayDestinationTypeDef(
-    _RequiredReplayDestinationTypeDef, _OptionalReplayDestinationTypeDef
+class ReplayDestinationOutputTypeDef(
+    _RequiredReplayDestinationOutputTypeDef, _OptionalReplayDestinationOutputTypeDef
 ):
     pass
 
 
 _RequiredDescribeRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRuleRequestRequestTypeDef",
     {
@@ -887,14 +1034,40 @@
 
 class DisableRuleRequestRequestTypeDef(
     _RequiredDisableRuleRequestRequestTypeDef, _OptionalDisableRuleRequestRequestTypeDef
 ):
     pass
 
 
+PlacementConstraintOutputTypeDef = TypedDict(
+    "PlacementConstraintOutputTypeDef",
+    {
+        "type": PlacementConstraintTypeType,
+        "expression": str,
+    },
+    total=False,
+)
+
+PlacementStrategyOutputTypeDef = TypedDict(
+    "PlacementStrategyOutputTypeDef",
+    {
+        "type": PlacementStrategyTypeType,
+        "field": str,
+    },
+    total=False,
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 PlacementConstraintTypeDef = TypedDict(
     "PlacementConstraintTypeDef",
     {
         "type": PlacementConstraintTypeType,
         "expression": str,
     },
     total=False,
@@ -956,57 +1129,109 @@
         "ExpirationTime": datetime,
         "Name": str,
         "State": EventSourceStateType,
     },
     total=False,
 )
 
+PrimaryOutputTypeDef = TypedDict(
+    "PrimaryOutputTypeDef",
+    {
+        "HealthCheck": str,
+    },
+)
+
+SecondaryOutputTypeDef = TypedDict(
+    "SecondaryOutputTypeDef",
+    {
+        "Route": str,
+    },
+)
+
 PrimaryTypeDef = TypedDict(
     "PrimaryTypeDef",
     {
         "HealthCheck": str,
     },
 )
 
 SecondaryTypeDef = TypedDict(
     "SecondaryTypeDef",
     {
         "Route": str,
     },
 )
 
-HttpParametersTypeDef = TypedDict(
-    "HttpParametersTypeDef",
+HttpParametersOutputTypeDef = TypedDict(
+    "HttpParametersOutputTypeDef",
     {
         "PathParameterValues": List[str],
         "HeaderParameters": Dict[str, str],
         "QueryStringParameters": Dict[str, str],
     },
     total=False,
 )
 
+HttpParametersTypeDef = TypedDict(
+    "HttpParametersTypeDef",
+    {
+        "PathParameterValues": Sequence[str],
+        "HeaderParameters": Mapping[str, str],
+        "QueryStringParameters": Mapping[str, str],
+    },
+    total=False,
+)
+
+_RequiredInputTransformerOutputTypeDef = TypedDict(
+    "_RequiredInputTransformerOutputTypeDef",
+    {
+        "InputTemplate": str,
+    },
+)
+_OptionalInputTransformerOutputTypeDef = TypedDict(
+    "_OptionalInputTransformerOutputTypeDef",
+    {
+        "InputPathsMap": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class InputTransformerOutputTypeDef(
+    _RequiredInputTransformerOutputTypeDef, _OptionalInputTransformerOutputTypeDef
+):
+    pass
+
+
 _RequiredInputTransformerTypeDef = TypedDict(
     "_RequiredInputTransformerTypeDef",
     {
         "InputTemplate": str,
     },
 )
 _OptionalInputTransformerTypeDef = TypedDict(
     "_OptionalInputTransformerTypeDef",
     {
-        "InputPathsMap": Dict[str, str],
+        "InputPathsMap": Mapping[str, str],
     },
     total=False,
 )
 
 
 class InputTransformerTypeDef(_RequiredInputTransformerTypeDef, _OptionalInputTransformerTypeDef):
     pass
 
 
+KinesisParametersOutputTypeDef = TypedDict(
+    "KinesisParametersOutputTypeDef",
+    {
+        "PartitionKeyPath": str,
+    },
+)
+
 KinesisParametersTypeDef = TypedDict(
     "KinesisParametersTypeDef",
     {
         "PartitionKeyPath": str,
     },
 )
 
@@ -1385,29 +1610,55 @@
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+_RequiredRedshiftDataParametersOutputTypeDef = TypedDict(
+    "_RequiredRedshiftDataParametersOutputTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalRedshiftDataParametersOutputTypeDef = TypedDict(
+    "_OptionalRedshiftDataParametersOutputTypeDef",
+    {
+        "SecretManagerArn": str,
+        "DbUser": str,
+        "Sql": str,
+        "StatementName": str,
+        "WithEvent": bool,
+        "Sqls": List[str],
+    },
+    total=False,
+)
+
+
+class RedshiftDataParametersOutputTypeDef(
+    _RequiredRedshiftDataParametersOutputTypeDef, _OptionalRedshiftDataParametersOutputTypeDef
+):
+    pass
+
+
 _RequiredRedshiftDataParametersTypeDef = TypedDict(
     "_RequiredRedshiftDataParametersTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalRedshiftDataParametersTypeDef = TypedDict(
     "_OptionalRedshiftDataParametersTypeDef",
     {
         "SecretManagerArn": str,
         "DbUser": str,
         "Sql": str,
         "StatementName": str,
         "WithEvent": bool,
-        "Sqls": List[str],
+        "Sqls": Sequence[str],
     },
     total=False,
 )
 
 
 class RedshiftDataParametersTypeDef(
     _RequiredRedshiftDataParametersTypeDef, _OptionalRedshiftDataParametersTypeDef
@@ -1454,50 +1705,104 @@
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+_RequiredReplayDestinationTypeDef = TypedDict(
+    "_RequiredReplayDestinationTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalReplayDestinationTypeDef = TypedDict(
+    "_OptionalReplayDestinationTypeDef",
+    {
+        "FilterArns": Sequence[str],
+    },
+    total=False,
+)
+
+
+class ReplayDestinationTypeDef(
+    _RequiredReplayDestinationTypeDef, _OptionalReplayDestinationTypeDef
+):
+    pass
+
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+RetryPolicyOutputTypeDef = TypedDict(
+    "RetryPolicyOutputTypeDef",
+    {
+        "MaximumRetryAttempts": int,
+        "MaximumEventAgeInSeconds": int,
+    },
+    total=False,
+)
+
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
     },
     total=False,
 )
 
+RunCommandTargetOutputTypeDef = TypedDict(
+    "RunCommandTargetOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+    },
+)
+
 RunCommandTargetTypeDef = TypedDict(
     "RunCommandTargetTypeDef",
     {
         "Key": str,
-        "Values": List[str],
+        "Values": Sequence[str],
+    },
+)
+
+SageMakerPipelineParameterOutputTypeDef = TypedDict(
+    "SageMakerPipelineParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
     },
 )
 
 SageMakerPipelineParameterTypeDef = TypedDict(
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+SqsParametersOutputTypeDef = TypedDict(
+    "SqsParametersOutputTypeDef",
+    {
+        "MessageGroupId": str,
+    },
+    total=False,
+)
+
 SqsParametersTypeDef = TypedDict(
     "SqsParametersTypeDef",
     {
         "MessageGroupId": str,
     },
     total=False,
 )
@@ -1661,22 +1966,53 @@
     {
         "Archives": List[ArchiveTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredBatchParametersOutputTypeDef = TypedDict(
+    "_RequiredBatchParametersOutputTypeDef",
+    {
+        "JobDefinition": str,
+        "JobName": str,
+    },
+)
+_OptionalBatchParametersOutputTypeDef = TypedDict(
+    "_OptionalBatchParametersOutputTypeDef",
+    {
+        "ArrayProperties": BatchArrayPropertiesOutputTypeDef,
+        "RetryStrategy": BatchRetryStrategyOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class BatchParametersOutputTypeDef(
+    _RequiredBatchParametersOutputTypeDef, _OptionalBatchParametersOutputTypeDef
+):
+    pass
+
+
 _RequiredBatchParametersTypeDef = TypedDict(
     "_RequiredBatchParametersTypeDef",
     {
         "JobDefinition": str,
         "JobName": str,
     },
 )
@@ -1703,14 +2039,24 @@
         "StatementId": str,
         "Condition": ConditionTypeDef,
         "Policy": str,
     },
     total=False,
 )
 
+ConnectionHttpParametersOutputTypeDef = TypedDict(
+    "ConnectionHttpParametersOutputTypeDef",
+    {
+        "HeaderParameters": List[ConnectionHeaderParameterOutputTypeDef],
+        "QueryStringParameters": List[ConnectionQueryStringParameterOutputTypeDef],
+        "BodyParameters": List[ConnectionBodyParameterOutputTypeDef],
+    },
+    total=False,
+)
+
 ConnectionHttpParametersTypeDef = TypedDict(
     "ConnectionHttpParametersTypeDef",
     {
         "HeaderParameters": Sequence[ConnectionHeaderParameterTypeDef],
         "QueryStringParameters": Sequence[ConnectionQueryStringParameterTypeDef],
         "BodyParameters": Sequence[ConnectionBodyParameterTypeDef],
     },
@@ -1744,22 +2090,14 @@
 
 class CreateEventBusRequestRequestTypeDef(
     _RequiredCreateEventBusRequestRequestTypeDef, _OptionalCreateEventBusRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalPutRuleRequestRequestTypeDef = TypedDict(
@@ -1796,49 +2134,32 @@
     {
         "ReplayName": str,
         "ReplayArn": str,
         "Description": str,
         "State": ReplayStateType,
         "StateReason": str,
         "EventSourceArn": str,
-        "Destination": ReplayDestinationTypeDef,
+        "Destination": ReplayDestinationOutputTypeDef,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartReplayRequestRequestTypeDef = TypedDict(
-    "_RequiredStartReplayRequestRequestTypeDef",
-    {
-        "ReplayName": str,
-        "EventSourceArn": str,
-        "EventStartTime": Union[datetime, str],
-        "EventEndTime": Union[datetime, str],
-        "Destination": ReplayDestinationTypeDef,
-    },
-)
-_OptionalStartReplayRequestRequestTypeDef = TypedDict(
-    "_OptionalStartReplayRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "Description": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class StartReplayRequestRequestTypeDef(
-    _RequiredStartReplayRequestRequestTypeDef, _OptionalStartReplayRequestRequestTypeDef
-):
-    pass
-
-
 ListEventBusesResponseTypeDef = TypedDict(
     "ListEventBusesResponseTypeDef",
     {
         "EventBuses": List[EventBusTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1849,14 +2170,22 @@
     {
         "EventSources": List[EventSourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FailoverConfigOutputTypeDef = TypedDict(
+    "FailoverConfigOutputTypeDef",
+    {
+        "Primary": PrimaryOutputTypeDef,
+        "Secondary": SecondaryOutputTypeDef,
+    },
+)
+
 FailoverConfigTypeDef = TypedDict(
     "FailoverConfigTypeDef",
     {
         "Primary": PrimaryTypeDef,
         "Secondary": SecondaryTypeDef,
     },
 )
@@ -1957,51 +2286,124 @@
     {
         "FailedEntryCount": int,
         "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredStartReplayRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReplayRequestRequestTypeDef",
+    {
+        "ReplayName": str,
+        "EventSourceArn": str,
+        "EventStartTime": Union[datetime, str],
+        "EventEndTime": Union[datetime, str],
+        "Destination": ReplayDestinationTypeDef,
+    },
+)
+_OptionalStartReplayRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReplayRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class StartReplayRequestRequestTypeDef(
+    _RequiredStartReplayRequestRequestTypeDef, _OptionalStartReplayRequestRequestTypeDef
+):
+    pass
+
+
+RunCommandParametersOutputTypeDef = TypedDict(
+    "RunCommandParametersOutputTypeDef",
+    {
+        "RunCommandTargets": List[RunCommandTargetOutputTypeDef],
+    },
+)
+
 RunCommandParametersTypeDef = TypedDict(
     "RunCommandParametersTypeDef",
     {
-        "RunCommandTargets": List[RunCommandTargetTypeDef],
+        "RunCommandTargets": Sequence[RunCommandTargetTypeDef],
+    },
+)
+
+SageMakerPipelineParametersOutputTypeDef = TypedDict(
+    "SageMakerPipelineParametersOutputTypeDef",
+    {
+        "PipelineParameterList": List[SageMakerPipelineParameterOutputTypeDef],
     },
+    total=False,
 )
 
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
-        "PipelineParameterList": List[SageMakerPipelineParameterTypeDef],
+        "PipelineParameterList": Sequence[SageMakerPipelineParameterTypeDef],
+    },
+    total=False,
+)
+
+_RequiredEcsParametersOutputTypeDef = TypedDict(
+    "_RequiredEcsParametersOutputTypeDef",
+    {
+        "TaskDefinitionArn": str,
+    },
+)
+_OptionalEcsParametersOutputTypeDef = TypedDict(
+    "_OptionalEcsParametersOutputTypeDef",
+    {
+        "TaskCount": int,
+        "LaunchType": LaunchTypeType,
+        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
+        "PlatformVersion": str,
+        "Group": str,
+        "CapacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "EnableECSManagedTags": bool,
+        "EnableExecuteCommand": bool,
+        "PlacementConstraints": List[PlacementConstraintOutputTypeDef],
+        "PlacementStrategy": List[PlacementStrategyOutputTypeDef],
+        "PropagateTags": Literal["TASK_DEFINITION"],
+        "ReferenceId": str,
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
+
+class EcsParametersOutputTypeDef(
+    _RequiredEcsParametersOutputTypeDef, _OptionalEcsParametersOutputTypeDef
+):
+    pass
+
+
 _RequiredEcsParametersTypeDef = TypedDict(
     "_RequiredEcsParametersTypeDef",
     {
         "TaskDefinitionArn": str,
     },
 )
 _OptionalEcsParametersTypeDef = TypedDict(
     "_OptionalEcsParametersTypeDef",
     {
         "TaskCount": int,
         "LaunchType": LaunchTypeType,
         "NetworkConfiguration": NetworkConfigurationTypeDef,
         "PlatformVersion": str,
         "Group": str,
-        "CapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "CapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
         "EnableECSManagedTags": bool,
         "EnableExecuteCommand": bool,
-        "PlacementConstraints": List[PlacementConstraintTypeDef],
-        "PlacementStrategy": List[PlacementStrategyTypeDef],
+        "PlacementConstraints": Sequence[PlacementConstraintTypeDef],
+        "PlacementStrategy": Sequence[PlacementStrategyTypeDef],
         "PropagateTags": Literal["TASK_DEFINITION"],
         "ReferenceId": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class EcsParametersTypeDef(_RequiredEcsParametersTypeDef, _OptionalEcsParametersTypeDef):
     pass
@@ -2009,15 +2411,15 @@
 
 ConnectionOAuthResponseParametersTypeDef = TypedDict(
     "ConnectionOAuthResponseParametersTypeDef",
     {
         "ClientParameters": ConnectionOAuthClientResponseParametersTypeDef,
         "AuthorizationEndpoint": str,
         "HttpMethod": ConnectionOAuthHttpMethodType,
-        "OAuthHttpParameters": ConnectionHttpParametersTypeDef,
+        "OAuthHttpParameters": ConnectionHttpParametersOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateConnectionOAuthRequestParametersTypeDef = TypedDict(
     "_RequiredCreateConnectionOAuthRequestParametersTypeDef",
     {
@@ -2049,21 +2451,61 @@
         "AuthorizationEndpoint": str,
         "HttpMethod": ConnectionOAuthHttpMethodType,
         "OAuthHttpParameters": ConnectionHttpParametersTypeDef,
     },
     total=False,
 )
 
+RoutingConfigOutputTypeDef = TypedDict(
+    "RoutingConfigOutputTypeDef",
+    {
+        "FailoverConfig": FailoverConfigOutputTypeDef,
+    },
+)
+
 RoutingConfigTypeDef = TypedDict(
     "RoutingConfigTypeDef",
     {
         "FailoverConfig": FailoverConfigTypeDef,
     },
 )
 
+_RequiredTargetOutputTypeDef = TypedDict(
+    "_RequiredTargetOutputTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+    },
+)
+_OptionalTargetOutputTypeDef = TypedDict(
+    "_OptionalTargetOutputTypeDef",
+    {
+        "RoleArn": str,
+        "Input": str,
+        "InputPath": str,
+        "InputTransformer": InputTransformerOutputTypeDef,
+        "KinesisParameters": KinesisParametersOutputTypeDef,
+        "RunCommandParameters": RunCommandParametersOutputTypeDef,
+        "EcsParameters": EcsParametersOutputTypeDef,
+        "BatchParameters": BatchParametersOutputTypeDef,
+        "SqsParameters": SqsParametersOutputTypeDef,
+        "HttpParameters": HttpParametersOutputTypeDef,
+        "RedshiftDataParameters": RedshiftDataParametersOutputTypeDef,
+        "SageMakerPipelineParameters": SageMakerPipelineParametersOutputTypeDef,
+        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
+        "RetryPolicy": RetryPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
+    pass
+
+
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
@@ -2095,15 +2537,15 @@
 
 ConnectionAuthResponseParametersTypeDef = TypedDict(
     "ConnectionAuthResponseParametersTypeDef",
     {
         "BasicAuthParameters": ConnectionBasicAuthResponseParametersTypeDef,
         "OAuthParameters": ConnectionOAuthResponseParametersTypeDef,
         "ApiKeyAuthParameters": ConnectionApiKeyAuthResponseParametersTypeDef,
-        "InvocationHttpParameters": ConnectionHttpParametersTypeDef,
+        "InvocationHttpParameters": ConnectionHttpParametersOutputTypeDef,
     },
     total=False,
 )
 
 CreateConnectionAuthRequestParametersTypeDef = TypedDict(
     "CreateConnectionAuthRequestParametersTypeDef",
     {
@@ -2122,62 +2564,37 @@
         "OAuthParameters": UpdateConnectionOAuthRequestParametersTypeDef,
         "ApiKeyAuthParameters": UpdateConnectionApiKeyAuthRequestParametersTypeDef,
         "InvocationHttpParameters": ConnectionHttpParametersTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEndpointRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoutingConfig": RoutingConfigTypeDef,
-        "EventBuses": Sequence[EndpointEventBusTypeDef],
-    },
-)
-_OptionalCreateEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEndpointRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ReplicationConfig": ReplicationConfigTypeDef,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
-
-class CreateEndpointRequestRequestTypeDef(
-    _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
-):
-    pass
-
-
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
-        "RoutingConfig": RoutingConfigTypeDef,
-        "ReplicationConfig": ReplicationConfigTypeDef,
-        "EventBuses": List[EndpointEventBusTypeDef],
+        "RoutingConfig": RoutingConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "EventBuses": List[EndpointEventBusOutputTypeDef],
         "RoleArn": str,
         "State": EndpointStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointResponseTypeDef = TypedDict(
     "DescribeEndpointResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "Arn": str,
-        "RoutingConfig": RoutingConfigTypeDef,
-        "ReplicationConfig": ReplicationConfigTypeDef,
-        "EventBuses": List[EndpointEventBusTypeDef],
+        "RoutingConfig": RoutingConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "EventBuses": List[EndpointEventBusOutputTypeDef],
         "RoleArn": str,
         "EndpointId": str,
         "EndpointUrl": str,
         "State": EndpointStateType,
         "StateReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
@@ -2187,73 +2604,98 @@
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Name": str,
         "Description": str,
         "Arn": str,
-        "RoutingConfig": RoutingConfigTypeDef,
-        "ReplicationConfig": ReplicationConfigTypeDef,
-        "EventBuses": List[EndpointEventBusTypeDef],
+        "RoutingConfig": RoutingConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "EventBuses": List[EndpointEventBusOutputTypeDef],
         "RoleArn": str,
         "EndpointId": str,
         "EndpointUrl": str,
         "State": EndpointStateType,
         "StateReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEndpointRequestRequestTypeDef",
+UpdateEndpointResponseTypeDef = TypedDict(
+    "UpdateEndpointResponseTypeDef",
     {
         "Name": str,
+        "Arn": str,
+        "RoutingConfig": RoutingConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "EventBuses": List[EndpointEventBusOutputTypeDef],
+        "RoleArn": str,
+        "EndpointId": str,
+        "EndpointUrl": str,
+        "State": EndpointStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEndpointRequestRequestTypeDef",
+
+_RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEndpointRequestRequestTypeDef",
     {
-        "Description": str,
+        "Name": str,
         "RoutingConfig": RoutingConfigTypeDef,
-        "ReplicationConfig": ReplicationConfigTypeDef,
         "EventBuses": Sequence[EndpointEventBusTypeDef],
+    },
+)
+_OptionalCreateEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEndpointRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ReplicationConfig": ReplicationConfigTypeDef,
         "RoleArn": str,
     },
     total=False,
 )
 
 
-class UpdateEndpointRequestRequestTypeDef(
-    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
+class CreateEndpointRequestRequestTypeDef(
+    _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
 ):
     pass
 
 
-UpdateEndpointResponseTypeDef = TypedDict(
-    "UpdateEndpointResponseTypeDef",
+_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEndpointRequestRequestTypeDef",
     {
         "Name": str,
-        "Arn": str,
+    },
+)
+_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEndpointRequestRequestTypeDef",
+    {
+        "Description": str,
         "RoutingConfig": RoutingConfigTypeDef,
         "ReplicationConfig": ReplicationConfigTypeDef,
-        "EventBuses": List[EndpointEventBusTypeDef],
+        "EventBuses": Sequence[EndpointEventBusTypeDef],
         "RoleArn": str,
-        "EndpointId": str,
-        "EndpointUrl": str,
-        "State": EndpointStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+
+class UpdateEndpointRequestRequestTypeDef(
+    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
+):
+    pass
+
+
 ListTargetsByRuleResponseTypeDef = TypedDict(
     "ListTargetsByRuleResponseTypeDef",
     {
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredPutTargetsRequestRequestTypeDef",
```

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events/type_defs.pyi` & `mypy-boto3-events-1.28.12/mypy_boto3_events/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_events.type_defs import ActivateEventSourceRequestRequestTypeDef
 
     data: ActivateEventSourceRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ApiDestinationHttpMethodType,
     ApiDestinationStateType,
     ArchiveStateType,
     AssignPublicIpType,
     ConnectionAuthorizationTypeType,
@@ -42,43 +42,53 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActivateEventSourceRequestRequestTypeDef",
     "ApiDestinationTypeDef",
     "ArchiveTypeDef",
+    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
+    "BatchArrayPropertiesOutputTypeDef",
     "BatchArrayPropertiesTypeDef",
+    "BatchRetryStrategyOutputTypeDef",
     "BatchRetryStrategyTypeDef",
     "CancelReplayRequestRequestTypeDef",
     "CancelReplayResponseTypeDef",
+    "CapacityProviderStrategyItemOutputTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "ConditionTypeDef",
     "ConnectionApiKeyAuthResponseParametersTypeDef",
     "ConnectionBasicAuthResponseParametersTypeDef",
+    "ConnectionBodyParameterOutputTypeDef",
     "ConnectionBodyParameterTypeDef",
+    "ConnectionHeaderParameterOutputTypeDef",
     "ConnectionHeaderParameterTypeDef",
+    "ConnectionQueryStringParameterOutputTypeDef",
     "ConnectionQueryStringParameterTypeDef",
     "ConnectionOAuthClientResponseParametersTypeDef",
     "ConnectionTypeDef",
     "CreateApiDestinationRequestRequestTypeDef",
     "CreateApiDestinationResponseTypeDef",
     "CreateArchiveRequestRequestTypeDef",
     "CreateArchiveResponseTypeDef",
     "CreateConnectionApiKeyAuthRequestParametersTypeDef",
     "CreateConnectionBasicAuthRequestParametersTypeDef",
     "CreateConnectionOAuthClientRequestParametersTypeDef",
     "CreateConnectionResponseTypeDef",
     "EndpointEventBusTypeDef",
     "ReplicationConfigTypeDef",
+    "EndpointEventBusOutputTypeDef",
+    "ReplicationConfigOutputTypeDef",
     "TagTypeDef",
     "CreateEventBusResponseTypeDef",
     "CreatePartnerEventSourceRequestRequestTypeDef",
     "CreatePartnerEventSourceResponseTypeDef",
     "DeactivateEventSourceRequestRequestTypeDef",
+    "DeadLetterConfigOutputTypeDef",
     "DeadLetterConfigTypeDef",
     "DeauthorizeConnectionRequestRequestTypeDef",
     "DeauthorizeConnectionResponseTypeDef",
     "DeleteApiDestinationRequestRequestTypeDef",
     "DeleteArchiveRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteConnectionResponseTypeDef",
@@ -95,28 +105,36 @@
     "DescribeEventBusRequestRequestTypeDef",
     "DescribeEventBusResponseTypeDef",
     "DescribeEventSourceRequestRequestTypeDef",
     "DescribeEventSourceResponseTypeDef",
     "DescribePartnerEventSourceRequestRequestTypeDef",
     "DescribePartnerEventSourceResponseTypeDef",
     "DescribeReplayRequestRequestTypeDef",
-    "ReplayDestinationTypeDef",
+    "ReplayDestinationOutputTypeDef",
     "DescribeRuleRequestRequestTypeDef",
     "DescribeRuleResponseTypeDef",
     "DisableRuleRequestRequestTypeDef",
+    "PlacementConstraintOutputTypeDef",
+    "PlacementStrategyOutputTypeDef",
+    "TagOutputTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableRuleRequestRequestTypeDef",
     "EventBusTypeDef",
     "EventSourceTypeDef",
+    "PrimaryOutputTypeDef",
+    "SecondaryOutputTypeDef",
     "PrimaryTypeDef",
     "SecondaryTypeDef",
+    "HttpParametersOutputTypeDef",
     "HttpParametersTypeDef",
+    "InputTransformerOutputTypeDef",
     "InputTransformerTypeDef",
+    "KinesisParametersOutputTypeDef",
     "KinesisParametersTypeDef",
     "ListApiDestinationsRequestRequestTypeDef",
     "ListArchivesRequestRequestTypeDef",
     "ListConnectionsRequestRequestTypeDef",
     "ListEndpointsRequestRequestTypeDef",
     "ListEventBusesRequestRequestTypeDef",
     "ListEventSourcesRequestRequestTypeDef",
@@ -138,22 +156,28 @@
     "PaginatorConfigTypeDef",
     "PutEventsRequestEntryTypeDef",
     "PutEventsResultEntryTypeDef",
     "PutPartnerEventsRequestEntryTypeDef",
     "PutPartnerEventsResultEntryTypeDef",
     "PutRuleResponseTypeDef",
     "PutTargetsResultEntryTypeDef",
+    "RedshiftDataParametersOutputTypeDef",
     "RedshiftDataParametersTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RemoveTargetsRequestRequestTypeDef",
     "RemoveTargetsResultEntryTypeDef",
+    "ReplayDestinationTypeDef",
     "ResponseMetadataTypeDef",
+    "RetryPolicyOutputTypeDef",
     "RetryPolicyTypeDef",
+    "RunCommandTargetOutputTypeDef",
     "RunCommandTargetTypeDef",
+    "SageMakerPipelineParameterOutputTypeDef",
     "SageMakerPipelineParameterTypeDef",
+    "SqsParametersOutputTypeDef",
     "SqsParametersTypeDef",
     "StartReplayResponseTypeDef",
     "TestEventPatternRequestRequestTypeDef",
     "TestEventPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiDestinationRequestRequestTypeDef",
     "UpdateApiDestinationResponseTypeDef",
@@ -161,55 +185,64 @@
     "UpdateArchiveResponseTypeDef",
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     "UpdateConnectionBasicAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthClientRequestParametersTypeDef",
     "UpdateConnectionResponseTypeDef",
     "ListApiDestinationsResponseTypeDef",
     "ListArchivesResponseTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
+    "BatchParametersOutputTypeDef",
     "BatchParametersTypeDef",
     "PutPermissionRequestRequestTypeDef",
+    "ConnectionHttpParametersOutputTypeDef",
     "ConnectionHttpParametersTypeDef",
     "ListConnectionsResponseTypeDef",
     "CreateEventBusRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PutRuleRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DescribeReplayResponseTypeDef",
-    "StartReplayRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListEventBusesResponseTypeDef",
     "ListEventSourcesResponseTypeDef",
+    "FailoverConfigOutputTypeDef",
     "FailoverConfigTypeDef",
     "ListPartnerEventSourceAccountsResponseTypeDef",
     "ListPartnerEventSourcesResponseTypeDef",
     "ListReplaysResponseTypeDef",
     "ListRulesResponseTypeDef",
     "PutEventsRequestRequestTypeDef",
     "PutEventsResponseTypeDef",
     "PutPartnerEventsRequestRequestTypeDef",
     "PutPartnerEventsResponseTypeDef",
     "PutTargetsResponseTypeDef",
     "RemoveTargetsResponseTypeDef",
+    "StartReplayRequestRequestTypeDef",
+    "RunCommandParametersOutputTypeDef",
     "RunCommandParametersTypeDef",
+    "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
+    "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ConnectionOAuthResponseParametersTypeDef",
     "CreateConnectionOAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthRequestParametersTypeDef",
+    "RoutingConfigOutputTypeDef",
     "RoutingConfigTypeDef",
+    "TargetOutputTypeDef",
     "TargetTypeDef",
     "ConnectionAuthResponseParametersTypeDef",
     "CreateConnectionAuthRequestParametersTypeDef",
     "UpdateConnectionAuthRequestParametersTypeDef",
-    "CreateEndpointRequestRequestTypeDef",
     "CreateEndpointResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "EndpointTypeDef",
-    "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
+    "CreateEndpointRequestRequestTypeDef",
+    "UpdateEndpointRequestRequestTypeDef",
     "ListTargetsByRuleResponseTypeDef",
     "PutTargetsRequestRequestTypeDef",
     "DescribeConnectionResponseTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "ListEndpointsResponseTypeDef",
 )
@@ -248,42 +281,78 @@
         "SizeBytes": int,
         "EventCount": int,
         "CreationTime": datetime,
     },
     total=False,
 )
 
+_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAwsVpcConfigurationOutputTypeDef",
+    {
+        "Subnets": List[str],
+    },
+)
+_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAwsVpcConfigurationOutputTypeDef",
+    {
+        "SecurityGroups": List[str],
+        "AssignPublicIp": AssignPublicIpType,
+    },
+    total=False,
+)
+
+class AwsVpcConfigurationOutputTypeDef(
+    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
-        "Subnets": List[str],
+        "Subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
     "_OptionalAwsVpcConfigurationTypeDef",
     {
-        "SecurityGroups": List[str],
+        "SecurityGroups": Sequence[str],
         "AssignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
 ):
     pass
 
+BatchArrayPropertiesOutputTypeDef = TypedDict(
+    "BatchArrayPropertiesOutputTypeDef",
+    {
+        "Size": int,
+    },
+    total=False,
+)
+
 BatchArrayPropertiesTypeDef = TypedDict(
     "BatchArrayPropertiesTypeDef",
     {
         "Size": int,
     },
     total=False,
 )
 
+BatchRetryStrategyOutputTypeDef = TypedDict(
+    "BatchRetryStrategyOutputTypeDef",
+    {
+        "Attempts": int,
+    },
+    total=False,
+)
+
 BatchRetryStrategyTypeDef = TypedDict(
     "BatchRetryStrategyTypeDef",
     {
         "Attempts": int,
     },
     total=False,
 )
@@ -301,14 +370,35 @@
         "ReplayArn": str,
         "State": ReplayStateType,
         "StateReason": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCapacityProviderStrategyItemOutputTypeDef = TypedDict(
+    "_RequiredCapacityProviderStrategyItemOutputTypeDef",
+    {
+        "capacityProvider": str,
+    },
+)
+_OptionalCapacityProviderStrategyItemOutputTypeDef = TypedDict(
+    "_OptionalCapacityProviderStrategyItemOutputTypeDef",
+    {
+        "weight": int,
+        "base": int,
+    },
+    total=False,
+)
+
+class CapacityProviderStrategyItemOutputTypeDef(
+    _RequiredCapacityProviderStrategyItemOutputTypeDef,
+    _OptionalCapacityProviderStrategyItemOutputTypeDef,
+):
+    pass
+
 _RequiredCapacityProviderStrategyItemTypeDef = TypedDict(
     "_RequiredCapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
     },
 )
 _OptionalCapacityProviderStrategyItemTypeDef = TypedDict(
@@ -346,34 +436,64 @@
     "ConnectionBasicAuthResponseParametersTypeDef",
     {
         "Username": str,
     },
     total=False,
 )
 
+ConnectionBodyParameterOutputTypeDef = TypedDict(
+    "ConnectionBodyParameterOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "IsValueSecret": bool,
+    },
+    total=False,
+)
+
 ConnectionBodyParameterTypeDef = TypedDict(
     "ConnectionBodyParameterTypeDef",
     {
         "Key": str,
         "Value": str,
         "IsValueSecret": bool,
     },
     total=False,
 )
 
+ConnectionHeaderParameterOutputTypeDef = TypedDict(
+    "ConnectionHeaderParameterOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "IsValueSecret": bool,
+    },
+    total=False,
+)
+
 ConnectionHeaderParameterTypeDef = TypedDict(
     "ConnectionHeaderParameterTypeDef",
     {
         "Key": str,
         "Value": str,
         "IsValueSecret": bool,
     },
     total=False,
 )
 
+ConnectionQueryStringParameterOutputTypeDef = TypedDict(
+    "ConnectionQueryStringParameterOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "IsValueSecret": bool,
+    },
+    total=False,
+)
+
 ConnectionQueryStringParameterTypeDef = TypedDict(
     "ConnectionQueryStringParameterTypeDef",
     {
         "Key": str,
         "Value": str,
         "IsValueSecret": bool,
     },
@@ -517,14 +637,29 @@
     "ReplicationConfigTypeDef",
     {
         "State": ReplicationStateType,
     },
     total=False,
 )
 
+EndpointEventBusOutputTypeDef = TypedDict(
+    "EndpointEventBusOutputTypeDef",
+    {
+        "EventBusArn": str,
+    },
+)
+
+ReplicationConfigOutputTypeDef = TypedDict(
+    "ReplicationConfigOutputTypeDef",
+    {
+        "State": ReplicationStateType,
+    },
+    total=False,
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -556,14 +691,22 @@
 DeactivateEventSourceRequestRequestTypeDef = TypedDict(
     "DeactivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+DeadLetterConfigOutputTypeDef = TypedDict(
+    "DeadLetterConfigOutputTypeDef",
+    {
+        "Arn": str,
+    },
+    total=False,
+)
+
 DeadLetterConfigTypeDef = TypedDict(
     "DeadLetterConfigTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
@@ -794,30 +937,30 @@
 DescribeReplayRequestRequestTypeDef = TypedDict(
     "DescribeReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
 
-_RequiredReplayDestinationTypeDef = TypedDict(
-    "_RequiredReplayDestinationTypeDef",
+_RequiredReplayDestinationOutputTypeDef = TypedDict(
+    "_RequiredReplayDestinationOutputTypeDef",
     {
         "Arn": str,
     },
 )
-_OptionalReplayDestinationTypeDef = TypedDict(
-    "_OptionalReplayDestinationTypeDef",
+_OptionalReplayDestinationOutputTypeDef = TypedDict(
+    "_OptionalReplayDestinationOutputTypeDef",
     {
         "FilterArns": List[str],
     },
     total=False,
 )
 
-class ReplayDestinationTypeDef(
-    _RequiredReplayDestinationTypeDef, _OptionalReplayDestinationTypeDef
+class ReplayDestinationOutputTypeDef(
+    _RequiredReplayDestinationOutputTypeDef, _OptionalReplayDestinationOutputTypeDef
 ):
     pass
 
 _RequiredDescribeRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRuleRequestRequestTypeDef",
     {
         "Name": str,
@@ -868,14 +1011,40 @@
 )
 
 class DisableRuleRequestRequestTypeDef(
     _RequiredDisableRuleRequestRequestTypeDef, _OptionalDisableRuleRequestRequestTypeDef
 ):
     pass
 
+PlacementConstraintOutputTypeDef = TypedDict(
+    "PlacementConstraintOutputTypeDef",
+    {
+        "type": PlacementConstraintTypeType,
+        "expression": str,
+    },
+    total=False,
+)
+
+PlacementStrategyOutputTypeDef = TypedDict(
+    "PlacementStrategyOutputTypeDef",
+    {
+        "type": PlacementStrategyTypeType,
+        "field": str,
+    },
+    total=False,
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 PlacementConstraintTypeDef = TypedDict(
     "PlacementConstraintTypeDef",
     {
         "type": PlacementConstraintTypeType,
         "expression": str,
     },
     total=False,
@@ -935,55 +1104,105 @@
         "ExpirationTime": datetime,
         "Name": str,
         "State": EventSourceStateType,
     },
     total=False,
 )
 
+PrimaryOutputTypeDef = TypedDict(
+    "PrimaryOutputTypeDef",
+    {
+        "HealthCheck": str,
+    },
+)
+
+SecondaryOutputTypeDef = TypedDict(
+    "SecondaryOutputTypeDef",
+    {
+        "Route": str,
+    },
+)
+
 PrimaryTypeDef = TypedDict(
     "PrimaryTypeDef",
     {
         "HealthCheck": str,
     },
 )
 
 SecondaryTypeDef = TypedDict(
     "SecondaryTypeDef",
     {
         "Route": str,
     },
 )
 
-HttpParametersTypeDef = TypedDict(
-    "HttpParametersTypeDef",
+HttpParametersOutputTypeDef = TypedDict(
+    "HttpParametersOutputTypeDef",
     {
         "PathParameterValues": List[str],
         "HeaderParameters": Dict[str, str],
         "QueryStringParameters": Dict[str, str],
     },
     total=False,
 )
 
+HttpParametersTypeDef = TypedDict(
+    "HttpParametersTypeDef",
+    {
+        "PathParameterValues": Sequence[str],
+        "HeaderParameters": Mapping[str, str],
+        "QueryStringParameters": Mapping[str, str],
+    },
+    total=False,
+)
+
+_RequiredInputTransformerOutputTypeDef = TypedDict(
+    "_RequiredInputTransformerOutputTypeDef",
+    {
+        "InputTemplate": str,
+    },
+)
+_OptionalInputTransformerOutputTypeDef = TypedDict(
+    "_OptionalInputTransformerOutputTypeDef",
+    {
+        "InputPathsMap": Dict[str, str],
+    },
+    total=False,
+)
+
+class InputTransformerOutputTypeDef(
+    _RequiredInputTransformerOutputTypeDef, _OptionalInputTransformerOutputTypeDef
+):
+    pass
+
 _RequiredInputTransformerTypeDef = TypedDict(
     "_RequiredInputTransformerTypeDef",
     {
         "InputTemplate": str,
     },
 )
 _OptionalInputTransformerTypeDef = TypedDict(
     "_OptionalInputTransformerTypeDef",
     {
-        "InputPathsMap": Dict[str, str],
+        "InputPathsMap": Mapping[str, str],
     },
     total=False,
 )
 
 class InputTransformerTypeDef(_RequiredInputTransformerTypeDef, _OptionalInputTransformerTypeDef):
     pass
 
+KinesisParametersOutputTypeDef = TypedDict(
+    "KinesisParametersOutputTypeDef",
+    {
+        "PartitionKeyPath": str,
+    },
+)
+
 KinesisParametersTypeDef = TypedDict(
     "KinesisParametersTypeDef",
     {
         "PartitionKeyPath": str,
     },
 )
 
@@ -1350,29 +1569,53 @@
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+_RequiredRedshiftDataParametersOutputTypeDef = TypedDict(
+    "_RequiredRedshiftDataParametersOutputTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalRedshiftDataParametersOutputTypeDef = TypedDict(
+    "_OptionalRedshiftDataParametersOutputTypeDef",
+    {
+        "SecretManagerArn": str,
+        "DbUser": str,
+        "Sql": str,
+        "StatementName": str,
+        "WithEvent": bool,
+        "Sqls": List[str],
+    },
+    total=False,
+)
+
+class RedshiftDataParametersOutputTypeDef(
+    _RequiredRedshiftDataParametersOutputTypeDef, _OptionalRedshiftDataParametersOutputTypeDef
+):
+    pass
+
 _RequiredRedshiftDataParametersTypeDef = TypedDict(
     "_RequiredRedshiftDataParametersTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalRedshiftDataParametersTypeDef = TypedDict(
     "_OptionalRedshiftDataParametersTypeDef",
     {
         "SecretManagerArn": str,
         "DbUser": str,
         "Sql": str,
         "StatementName": str,
         "WithEvent": bool,
-        "Sqls": List[str],
+        "Sqls": Sequence[str],
     },
     total=False,
 )
 
 class RedshiftDataParametersTypeDef(
     _RequiredRedshiftDataParametersTypeDef, _OptionalRedshiftDataParametersTypeDef
 ):
@@ -1415,50 +1658,102 @@
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
+_RequiredReplayDestinationTypeDef = TypedDict(
+    "_RequiredReplayDestinationTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalReplayDestinationTypeDef = TypedDict(
+    "_OptionalReplayDestinationTypeDef",
+    {
+        "FilterArns": Sequence[str],
+    },
+    total=False,
+)
+
+class ReplayDestinationTypeDef(
+    _RequiredReplayDestinationTypeDef, _OptionalReplayDestinationTypeDef
+):
+    pass
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+RetryPolicyOutputTypeDef = TypedDict(
+    "RetryPolicyOutputTypeDef",
+    {
+        "MaximumRetryAttempts": int,
+        "MaximumEventAgeInSeconds": int,
+    },
+    total=False,
+)
+
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
     },
     total=False,
 )
 
+RunCommandTargetOutputTypeDef = TypedDict(
+    "RunCommandTargetOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+    },
+)
+
 RunCommandTargetTypeDef = TypedDict(
     "RunCommandTargetTypeDef",
     {
         "Key": str,
-        "Values": List[str],
+        "Values": Sequence[str],
+    },
+)
+
+SageMakerPipelineParameterOutputTypeDef = TypedDict(
+    "SageMakerPipelineParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
     },
 )
 
 SageMakerPipelineParameterTypeDef = TypedDict(
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+SqsParametersOutputTypeDef = TypedDict(
+    "SqsParametersOutputTypeDef",
+    {
+        "MessageGroupId": str,
+    },
+    total=False,
+)
+
 SqsParametersTypeDef = TypedDict(
     "SqsParametersTypeDef",
     {
         "MessageGroupId": str,
     },
     total=False,
 )
@@ -1618,22 +1913,51 @@
     {
         "Archives": List[ArchiveTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredBatchParametersOutputTypeDef = TypedDict(
+    "_RequiredBatchParametersOutputTypeDef",
+    {
+        "JobDefinition": str,
+        "JobName": str,
+    },
+)
+_OptionalBatchParametersOutputTypeDef = TypedDict(
+    "_OptionalBatchParametersOutputTypeDef",
+    {
+        "ArrayProperties": BatchArrayPropertiesOutputTypeDef,
+        "RetryStrategy": BatchRetryStrategyOutputTypeDef,
+    },
+    total=False,
+)
+
+class BatchParametersOutputTypeDef(
+    _RequiredBatchParametersOutputTypeDef, _OptionalBatchParametersOutputTypeDef
+):
+    pass
+
 _RequiredBatchParametersTypeDef = TypedDict(
     "_RequiredBatchParametersTypeDef",
     {
         "JobDefinition": str,
         "JobName": str,
     },
 )
@@ -1658,14 +1982,24 @@
         "StatementId": str,
         "Condition": ConditionTypeDef,
         "Policy": str,
     },
     total=False,
 )
 
+ConnectionHttpParametersOutputTypeDef = TypedDict(
+    "ConnectionHttpParametersOutputTypeDef",
+    {
+        "HeaderParameters": List[ConnectionHeaderParameterOutputTypeDef],
+        "QueryStringParameters": List[ConnectionQueryStringParameterOutputTypeDef],
+        "BodyParameters": List[ConnectionBodyParameterOutputTypeDef],
+    },
+    total=False,
+)
+
 ConnectionHttpParametersTypeDef = TypedDict(
     "ConnectionHttpParametersTypeDef",
     {
         "HeaderParameters": Sequence[ConnectionHeaderParameterTypeDef],
         "QueryStringParameters": Sequence[ConnectionQueryStringParameterTypeDef],
         "BodyParameters": Sequence[ConnectionBodyParameterTypeDef],
     },
@@ -1697,22 +2031,14 @@
 )
 
 class CreateEventBusRequestRequestTypeDef(
     _RequiredCreateEventBusRequestRequestTypeDef, _OptionalCreateEventBusRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalPutRuleRequestRequestTypeDef = TypedDict(
@@ -1747,47 +2073,32 @@
     {
         "ReplayName": str,
         "ReplayArn": str,
         "Description": str,
         "State": ReplayStateType,
         "StateReason": str,
         "EventSourceArn": str,
-        "Destination": ReplayDestinationTypeDef,
+        "Destination": ReplayDestinationOutputTypeDef,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartReplayRequestRequestTypeDef = TypedDict(
-    "_RequiredStartReplayRequestRequestTypeDef",
-    {
-        "ReplayName": str,
-        "EventSourceArn": str,
-        "EventStartTime": Union[datetime, str],
-        "EventEndTime": Union[datetime, str],
-        "Destination": ReplayDestinationTypeDef,
-    },
-)
-_OptionalStartReplayRequestRequestTypeDef = TypedDict(
-    "_OptionalStartReplayRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "Description": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class StartReplayRequestRequestTypeDef(
-    _RequiredStartReplayRequestRequestTypeDef, _OptionalStartReplayRequestRequestTypeDef
-):
-    pass
-
 ListEventBusesResponseTypeDef = TypedDict(
     "ListEventBusesResponseTypeDef",
     {
         "EventBuses": List[EventBusTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1798,14 +2109,22 @@
     {
         "EventSources": List[EventSourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FailoverConfigOutputTypeDef = TypedDict(
+    "FailoverConfigOutputTypeDef",
+    {
+        "Primary": PrimaryOutputTypeDef,
+        "Secondary": SecondaryOutputTypeDef,
+    },
+)
+
 FailoverConfigTypeDef = TypedDict(
     "FailoverConfigTypeDef",
     {
         "Primary": PrimaryTypeDef,
         "Secondary": SecondaryTypeDef,
     },
 )
@@ -1904,65 +2223,134 @@
     {
         "FailedEntryCount": int,
         "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredStartReplayRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReplayRequestRequestTypeDef",
+    {
+        "ReplayName": str,
+        "EventSourceArn": str,
+        "EventStartTime": Union[datetime, str],
+        "EventEndTime": Union[datetime, str],
+        "Destination": ReplayDestinationTypeDef,
+    },
+)
+_OptionalStartReplayRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReplayRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class StartReplayRequestRequestTypeDef(
+    _RequiredStartReplayRequestRequestTypeDef, _OptionalStartReplayRequestRequestTypeDef
+):
+    pass
+
+RunCommandParametersOutputTypeDef = TypedDict(
+    "RunCommandParametersOutputTypeDef",
+    {
+        "RunCommandTargets": List[RunCommandTargetOutputTypeDef],
+    },
+)
+
 RunCommandParametersTypeDef = TypedDict(
     "RunCommandParametersTypeDef",
     {
-        "RunCommandTargets": List[RunCommandTargetTypeDef],
+        "RunCommandTargets": Sequence[RunCommandTargetTypeDef],
     },
 )
 
+SageMakerPipelineParametersOutputTypeDef = TypedDict(
+    "SageMakerPipelineParametersOutputTypeDef",
+    {
+        "PipelineParameterList": List[SageMakerPipelineParameterOutputTypeDef],
+    },
+    total=False,
+)
+
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
-        "PipelineParameterList": List[SageMakerPipelineParameterTypeDef],
+        "PipelineParameterList": Sequence[SageMakerPipelineParameterTypeDef],
     },
     total=False,
 )
 
+_RequiredEcsParametersOutputTypeDef = TypedDict(
+    "_RequiredEcsParametersOutputTypeDef",
+    {
+        "TaskDefinitionArn": str,
+    },
+)
+_OptionalEcsParametersOutputTypeDef = TypedDict(
+    "_OptionalEcsParametersOutputTypeDef",
+    {
+        "TaskCount": int,
+        "LaunchType": LaunchTypeType,
+        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
+        "PlatformVersion": str,
+        "Group": str,
+        "CapacityProviderStrategy": List[CapacityProviderStrategyItemOutputTypeDef],
+        "EnableECSManagedTags": bool,
+        "EnableExecuteCommand": bool,
+        "PlacementConstraints": List[PlacementConstraintOutputTypeDef],
+        "PlacementStrategy": List[PlacementStrategyOutputTypeDef],
+        "PropagateTags": Literal["TASK_DEFINITION"],
+        "ReferenceId": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+class EcsParametersOutputTypeDef(
+    _RequiredEcsParametersOutputTypeDef, _OptionalEcsParametersOutputTypeDef
+):
+    pass
+
 _RequiredEcsParametersTypeDef = TypedDict(
     "_RequiredEcsParametersTypeDef",
     {
         "TaskDefinitionArn": str,
     },
 )
 _OptionalEcsParametersTypeDef = TypedDict(
     "_OptionalEcsParametersTypeDef",
     {
         "TaskCount": int,
         "LaunchType": LaunchTypeType,
         "NetworkConfiguration": NetworkConfigurationTypeDef,
         "PlatformVersion": str,
         "Group": str,
-        "CapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "CapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
         "EnableECSManagedTags": bool,
         "EnableExecuteCommand": bool,
-        "PlacementConstraints": List[PlacementConstraintTypeDef],
-        "PlacementStrategy": List[PlacementStrategyTypeDef],
+        "PlacementConstraints": Sequence[PlacementConstraintTypeDef],
+        "PlacementStrategy": Sequence[PlacementStrategyTypeDef],
         "PropagateTags": Literal["TASK_DEFINITION"],
         "ReferenceId": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class EcsParametersTypeDef(_RequiredEcsParametersTypeDef, _OptionalEcsParametersTypeDef):
     pass
 
 ConnectionOAuthResponseParametersTypeDef = TypedDict(
     "ConnectionOAuthResponseParametersTypeDef",
     {
         "ClientParameters": ConnectionOAuthClientResponseParametersTypeDef,
         "AuthorizationEndpoint": str,
         "HttpMethod": ConnectionOAuthHttpMethodType,
-        "OAuthHttpParameters": ConnectionHttpParametersTypeDef,
+        "OAuthHttpParameters": ConnectionHttpParametersOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateConnectionOAuthRequestParametersTypeDef = TypedDict(
     "_RequiredCreateConnectionOAuthRequestParametersTypeDef",
     {
@@ -1992,21 +2380,59 @@
         "AuthorizationEndpoint": str,
         "HttpMethod": ConnectionOAuthHttpMethodType,
         "OAuthHttpParameters": ConnectionHttpParametersTypeDef,
     },
     total=False,
 )
 
+RoutingConfigOutputTypeDef = TypedDict(
+    "RoutingConfigOutputTypeDef",
+    {
+        "FailoverConfig": FailoverConfigOutputTypeDef,
+    },
+)
+
 RoutingConfigTypeDef = TypedDict(
     "RoutingConfigTypeDef",
     {
         "FailoverConfig": FailoverConfigTypeDef,
     },
 )
 
+_RequiredTargetOutputTypeDef = TypedDict(
+    "_RequiredTargetOutputTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+    },
+)
+_OptionalTargetOutputTypeDef = TypedDict(
+    "_OptionalTargetOutputTypeDef",
+    {
+        "RoleArn": str,
+        "Input": str,
+        "InputPath": str,
+        "InputTransformer": InputTransformerOutputTypeDef,
+        "KinesisParameters": KinesisParametersOutputTypeDef,
+        "RunCommandParameters": RunCommandParametersOutputTypeDef,
+        "EcsParameters": EcsParametersOutputTypeDef,
+        "BatchParameters": BatchParametersOutputTypeDef,
+        "SqsParameters": SqsParametersOutputTypeDef,
+        "HttpParameters": HttpParametersOutputTypeDef,
+        "RedshiftDataParameters": RedshiftDataParametersOutputTypeDef,
+        "SageMakerPipelineParameters": SageMakerPipelineParametersOutputTypeDef,
+        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
+        "RetryPolicy": RetryPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
+class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
+    pass
+
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
@@ -2036,15 +2462,15 @@
 
 ConnectionAuthResponseParametersTypeDef = TypedDict(
     "ConnectionAuthResponseParametersTypeDef",
     {
         "BasicAuthParameters": ConnectionBasicAuthResponseParametersTypeDef,
         "OAuthParameters": ConnectionOAuthResponseParametersTypeDef,
         "ApiKeyAuthParameters": ConnectionApiKeyAuthResponseParametersTypeDef,
-        "InvocationHttpParameters": ConnectionHttpParametersTypeDef,
+        "InvocationHttpParameters": ConnectionHttpParametersOutputTypeDef,
     },
     total=False,
 )
 
 CreateConnectionAuthRequestParametersTypeDef = TypedDict(
     "CreateConnectionAuthRequestParametersTypeDef",
     {
@@ -2063,60 +2489,37 @@
         "OAuthParameters": UpdateConnectionOAuthRequestParametersTypeDef,
         "ApiKeyAuthParameters": UpdateConnectionApiKeyAuthRequestParametersTypeDef,
         "InvocationHttpParameters": ConnectionHttpParametersTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEndpointRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RoutingConfig": RoutingConfigTypeDef,
-        "EventBuses": Sequence[EndpointEventBusTypeDef],
-    },
-)
-_OptionalCreateEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEndpointRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ReplicationConfig": ReplicationConfigTypeDef,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
-class CreateEndpointRequestRequestTypeDef(
-    _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
-):
-    pass
-
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
-        "RoutingConfig": RoutingConfigTypeDef,
-        "ReplicationConfig": ReplicationConfigTypeDef,
-        "EventBuses": List[EndpointEventBusTypeDef],
+        "RoutingConfig": RoutingConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "EventBuses": List[EndpointEventBusOutputTypeDef],
         "RoleArn": str,
         "State": EndpointStateType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeEndpointResponseTypeDef = TypedDict(
     "DescribeEndpointResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "Arn": str,
-        "RoutingConfig": RoutingConfigTypeDef,
-        "ReplicationConfig": ReplicationConfigTypeDef,
-        "EventBuses": List[EndpointEventBusTypeDef],
+        "RoutingConfig": RoutingConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "EventBuses": List[EndpointEventBusOutputTypeDef],
         "RoleArn": str,
         "EndpointId": str,
         "EndpointUrl": str,
         "State": EndpointStateType,
         "StateReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
@@ -2126,71 +2529,94 @@
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Name": str,
         "Description": str,
         "Arn": str,
-        "RoutingConfig": RoutingConfigTypeDef,
-        "ReplicationConfig": ReplicationConfigTypeDef,
-        "EventBuses": List[EndpointEventBusTypeDef],
+        "RoutingConfig": RoutingConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "EventBuses": List[EndpointEventBusOutputTypeDef],
         "RoleArn": str,
         "EndpointId": str,
         "EndpointUrl": str,
         "State": EndpointStateType,
         "StateReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEndpointRequestRequestTypeDef",
+UpdateEndpointResponseTypeDef = TypedDict(
+    "UpdateEndpointResponseTypeDef",
     {
         "Name": str,
+        "Arn": str,
+        "RoutingConfig": RoutingConfigOutputTypeDef,
+        "ReplicationConfig": ReplicationConfigOutputTypeDef,
+        "EventBuses": List[EndpointEventBusOutputTypeDef],
+        "RoleArn": str,
+        "EndpointId": str,
+        "EndpointUrl": str,
+        "State": EndpointStateType,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEndpointRequestRequestTypeDef",
+
+_RequiredCreateEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEndpointRequestRequestTypeDef",
     {
-        "Description": str,
+        "Name": str,
         "RoutingConfig": RoutingConfigTypeDef,
-        "ReplicationConfig": ReplicationConfigTypeDef,
         "EventBuses": Sequence[EndpointEventBusTypeDef],
+    },
+)
+_OptionalCreateEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEndpointRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ReplicationConfig": ReplicationConfigTypeDef,
         "RoleArn": str,
     },
     total=False,
 )
 
-class UpdateEndpointRequestRequestTypeDef(
-    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
+class CreateEndpointRequestRequestTypeDef(
+    _RequiredCreateEndpointRequestRequestTypeDef, _OptionalCreateEndpointRequestRequestTypeDef
 ):
     pass
 
-UpdateEndpointResponseTypeDef = TypedDict(
-    "UpdateEndpointResponseTypeDef",
+_RequiredUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEndpointRequestRequestTypeDef",
     {
         "Name": str,
-        "Arn": str,
+    },
+)
+_OptionalUpdateEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEndpointRequestRequestTypeDef",
+    {
+        "Description": str,
         "RoutingConfig": RoutingConfigTypeDef,
         "ReplicationConfig": ReplicationConfigTypeDef,
-        "EventBuses": List[EndpointEventBusTypeDef],
+        "EventBuses": Sequence[EndpointEventBusTypeDef],
         "RoleArn": str,
-        "EndpointId": str,
-        "EndpointUrl": str,
-        "State": EndpointStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
+class UpdateEndpointRequestRequestTypeDef(
+    _RequiredUpdateEndpointRequestRequestTypeDef, _OptionalUpdateEndpointRequestRequestTypeDef
+):
+    pass
+
 ListTargetsByRuleResponseTypeDef = TypedDict(
     "ListTargetsByRuleResponseTypeDef",
     {
-        "Targets": List[TargetTypeDef],
+        "Targets": List[TargetOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredPutTargetsRequestRequestTypeDef",
```

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events.egg-info/PKG-INFO` & `mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-events
-Version: 1.28.0
-Summary: Type annotations for boto3.EventBridge 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.EventBridge 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-events"></a>
 
 # mypy-boto3-events
 
 [![PyPI - mypy-boto3-events](https://img.shields.io/pypi/v/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-events?color=blue)](https://pypistats.org/packages/mypy-boto3-events)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-events)](https://pepy.tech/project/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,43 +349,53 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_events.type_defs import (
     ActivateEventSourceRequestRequestTypeDef,
     ApiDestinationTypeDef,
     ArchiveTypeDef,
+    AwsVpcConfigurationOutputTypeDef,
     AwsVpcConfigurationTypeDef,
+    BatchArrayPropertiesOutputTypeDef,
     BatchArrayPropertiesTypeDef,
+    BatchRetryStrategyOutputTypeDef,
     BatchRetryStrategyTypeDef,
     CancelReplayRequestRequestTypeDef,
     CancelReplayResponseTypeDef,
+    CapacityProviderStrategyItemOutputTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ConditionTypeDef,
     ConnectionApiKeyAuthResponseParametersTypeDef,
     ConnectionBasicAuthResponseParametersTypeDef,
+    ConnectionBodyParameterOutputTypeDef,
     ConnectionBodyParameterTypeDef,
+    ConnectionHeaderParameterOutputTypeDef,
     ConnectionHeaderParameterTypeDef,
+    ConnectionQueryStringParameterOutputTypeDef,
     ConnectionQueryStringParameterTypeDef,
     ConnectionOAuthClientResponseParametersTypeDef,
     ConnectionTypeDef,
     CreateApiDestinationRequestRequestTypeDef,
     CreateApiDestinationResponseTypeDef,
     CreateArchiveRequestRequestTypeDef,
     CreateArchiveResponseTypeDef,
     CreateConnectionApiKeyAuthRequestParametersTypeDef,
     CreateConnectionBasicAuthRequestParametersTypeDef,
     CreateConnectionOAuthClientRequestParametersTypeDef,
     CreateConnectionResponseTypeDef,
     EndpointEventBusTypeDef,
     ReplicationConfigTypeDef,
+    EndpointEventBusOutputTypeDef,
+    ReplicationConfigOutputTypeDef,
     TagTypeDef,
     CreateEventBusResponseTypeDef,
     CreatePartnerEventSourceRequestRequestTypeDef,
     CreatePartnerEventSourceResponseTypeDef,
     DeactivateEventSourceRequestRequestTypeDef,
+    DeadLetterConfigOutputTypeDef,
     DeadLetterConfigTypeDef,
     DeauthorizeConnectionRequestRequestTypeDef,
     DeauthorizeConnectionResponseTypeDef,
     DeleteApiDestinationRequestRequestTypeDef,
     DeleteArchiveRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteConnectionResponseTypeDef,
@@ -402,28 +412,36 @@
     DescribeEventBusRequestRequestTypeDef,
     DescribeEventBusResponseTypeDef,
     DescribeEventSourceRequestRequestTypeDef,
     DescribeEventSourceResponseTypeDef,
     DescribePartnerEventSourceRequestRequestTypeDef,
     DescribePartnerEventSourceResponseTypeDef,
     DescribeReplayRequestRequestTypeDef,
-    ReplayDestinationTypeDef,
+    ReplayDestinationOutputTypeDef,
     DescribeRuleRequestRequestTypeDef,
     DescribeRuleResponseTypeDef,
     DisableRuleRequestRequestTypeDef,
+    PlacementConstraintOutputTypeDef,
+    PlacementStrategyOutputTypeDef,
+    TagOutputTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableRuleRequestRequestTypeDef,
     EventBusTypeDef,
     EventSourceTypeDef,
+    PrimaryOutputTypeDef,
+    SecondaryOutputTypeDef,
     PrimaryTypeDef,
     SecondaryTypeDef,
+    HttpParametersOutputTypeDef,
     HttpParametersTypeDef,
+    InputTransformerOutputTypeDef,
     InputTransformerTypeDef,
+    KinesisParametersOutputTypeDef,
     KinesisParametersTypeDef,
     ListApiDestinationsRequestRequestTypeDef,
     ListArchivesRequestRequestTypeDef,
     ListConnectionsRequestRequestTypeDef,
     ListEndpointsRequestRequestTypeDef,
     ListEventBusesRequestRequestTypeDef,
     ListEventSourcesRequestRequestTypeDef,
@@ -445,22 +463,28 @@
     PaginatorConfigTypeDef,
     PutEventsRequestEntryTypeDef,
     PutEventsResultEntryTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResultEntryTypeDef,
     PutRuleResponseTypeDef,
     PutTargetsResultEntryTypeDef,
+    RedshiftDataParametersOutputTypeDef,
     RedshiftDataParametersTypeDef,
     RemovePermissionRequestRequestTypeDef,
     RemoveTargetsRequestRequestTypeDef,
     RemoveTargetsResultEntryTypeDef,
+    ReplayDestinationTypeDef,
     ResponseMetadataTypeDef,
+    RetryPolicyOutputTypeDef,
     RetryPolicyTypeDef,
+    RunCommandTargetOutputTypeDef,
     RunCommandTargetTypeDef,
+    SageMakerPipelineParameterOutputTypeDef,
     SageMakerPipelineParameterTypeDef,
+    SqsParametersOutputTypeDef,
     SqsParametersTypeDef,
     StartReplayResponseTypeDef,
     TestEventPatternRequestRequestTypeDef,
     TestEventPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiDestinationRequestRequestTypeDef,
     UpdateApiDestinationResponseTypeDef,
@@ -468,55 +492,64 @@
     UpdateArchiveResponseTypeDef,
     UpdateConnectionApiKeyAuthRequestParametersTypeDef,
     UpdateConnectionBasicAuthRequestParametersTypeDef,
     UpdateConnectionOAuthClientRequestParametersTypeDef,
     UpdateConnectionResponseTypeDef,
     ListApiDestinationsResponseTypeDef,
     ListArchivesResponseTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
+    BatchParametersOutputTypeDef,
     BatchParametersTypeDef,
     PutPermissionRequestRequestTypeDef,
+    ConnectionHttpParametersOutputTypeDef,
     ConnectionHttpParametersTypeDef,
     ListConnectionsResponseTypeDef,
     CreateEventBusRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PutRuleRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     DescribeReplayResponseTypeDef,
-    StartReplayRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListEventBusesResponseTypeDef,
     ListEventSourcesResponseTypeDef,
+    FailoverConfigOutputTypeDef,
     FailoverConfigTypeDef,
     ListPartnerEventSourceAccountsResponseTypeDef,
     ListPartnerEventSourcesResponseTypeDef,
     ListReplaysResponseTypeDef,
     ListRulesResponseTypeDef,
     PutEventsRequestRequestTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestRequestTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
+    StartReplayRequestRequestTypeDef,
+    RunCommandParametersOutputTypeDef,
     RunCommandParametersTypeDef,
+    SageMakerPipelineParametersOutputTypeDef,
     SageMakerPipelineParametersTypeDef,
+    EcsParametersOutputTypeDef,
     EcsParametersTypeDef,
     ConnectionOAuthResponseParametersTypeDef,
     CreateConnectionOAuthRequestParametersTypeDef,
     UpdateConnectionOAuthRequestParametersTypeDef,
+    RoutingConfigOutputTypeDef,
     RoutingConfigTypeDef,
+    TargetOutputTypeDef,
     TargetTypeDef,
     ConnectionAuthResponseParametersTypeDef,
     CreateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
-    CreateEndpointRequestRequestTypeDef,
     CreateEndpointResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     EndpointTypeDef,
-    UpdateEndpointRequestRequestTypeDef,
     UpdateEndpointResponseTypeDef,
+    CreateEndpointRequestRequestTypeDef,
+    UpdateEndpointRequestRequestTypeDef,
     ListTargetsByRuleResponseTypeDef,
     PutTargetsRequestRequestTypeDef,
     DescribeConnectionResponseTypeDef,
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     ListEndpointsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-events-1.28.0/mypy_boto3_events.egg-info/SOURCES.txt` & `mypy-boto3-events-1.28.12/mypy_boto3_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-events-1.28.0/setup.py` & `mypy-boto3-events-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-events",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EventBridge 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.EventBridge 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

