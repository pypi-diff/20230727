# Comparing `tmp/mypy-boto3-gamelift-1.28.0.tar.gz` & `tmp/mypy-boto3-gamelift-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-gamelift-1.28.0.tar", last modified: Thu Jul  6 20:59:38 2023, max compression
+gzip compressed data, was "mypy-boto3-gamelift-1.28.12.tar", last modified: Thu Jul 27 05:34:43 2023, max compression
```

## Comparing `mypy-boto3-gamelift-1.28.0.tar` & `mypy-boto3-gamelift-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:38.506310 mypy-boto3-gamelift-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:41:34.000000 mypy-boto3-gamelift-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-07-06 20:59:38.506310 mypy-boto3-gamelift-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27403 2023-07-06 20:41:34.000000 mypy-boto3-gamelift-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:38.498310 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-06 20:41:34.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-06 20:41:34.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:41:34.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84696 2023-07-06 20:41:35.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    84563 2023-07-06 20:41:35.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20652 2023-07-06 20:41:37.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20650 2023-07-06 20:41:37.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26590 2023-07-06 20:41:35.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26566 2023-07-06 20:41:35.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:41:34.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    98211 2023-07-06 20:41:40.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98112 2023-07-06 20:41:39.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:41:34.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:38.506310 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-07-06 20:59:38.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 20:59:38.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:38.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:38.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:38.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 20:59:38.000000 mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:38.506310 mypy-boto3-gamelift-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:41:34.000000 mypy-boto3-gamelift-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:43.272504 mypy-boto3-gamelift-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:36.000000 mypy-boto3-gamelift-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29553 2023-07-27 05:34:43.272504 mypy-boto3-gamelift-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28062 2023-07-27 05:22:36.000000 mypy-boto3-gamelift-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:43.272504 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-27 05:22:36.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-27 05:22:36.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 05:22:36.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84696 2023-07-27 05:22:38.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84563 2023-07-27 05:22:38.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-07-27 05:22:38.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20728 2023-07-27 05:22:38.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26590 2023-07-27 05:22:38.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26566 2023-07-27 05:22:38.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:36.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   103160 2023-07-27 05:22:40.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103057 2023-07-27 05:22:39.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:36.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:43.272504 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29553 2023-07-27 05:34:43.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:34:43.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:43.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:43.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:43.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:43.000000 mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:43.272504 mypy-boto3-gamelift-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:22:36.000000 mypy-boto3-gamelift-1.28.12/setup.py
```

### Comparing `mypy-boto3-gamelift-1.28.0/LICENSE` & `mypy-boto3-gamelift-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.0/PKG-INFO` & `mypy-boto3-gamelift-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamelift
-Version: 1.28.0
-Summary: Type annotations for boto3.GameLift 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.GameLift 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-gamelift"></a>
 
 # mypy-boto3-gamelift
 
 [![PyPI - mypy-boto3-gamelift](https://img.shields.io/pypi/v/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-gamelift?color=blue)](https://pypistats.org/packages/mypy-boto3-gamelift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamelift)](https://pepy.tech/project/mypy-boto3-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameLift 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[boto3.GameLift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
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
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -457,25 +457,30 @@
 
 `mypy_boto3_gamelift.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_gamelift.type_defs import (
     AcceptMatchInputRequestTypeDef,
-    RoutingStrategyTypeDef,
+    RoutingStrategyOutputTypeDef,
+    AnywhereConfigurationOutputTypeDef,
     AnywhereConfigurationTypeDef,
+    AttributeValueOutputTypeDef,
     AttributeValueTypeDef,
     AwsCredentialsTypeDef,
     BuildTypeDef,
+    CertificateConfigurationOutputTypeDef,
     CertificateConfigurationTypeDef,
     ClaimFilterOptionTypeDef,
     GameServerTypeDef,
     ComputeTypeDef,
+    RoutingStrategyTypeDef,
     TagTypeDef,
     S3LocationTypeDef,
+    S3LocationOutputTypeDef,
     IpPermissionTypeDef,
     LocationConfigurationTypeDef,
     ResourceCreationLimitPolicyTypeDef,
     LocationStateTypeDef,
     InstanceDefinitionTypeDef,
     LaunchTemplateSpecificationTypeDef,
     GamePropertyTypeDef,
@@ -519,14 +524,15 @@
     DescribeFleetEventsInputRequestTypeDef,
     EventTypeDef,
     DescribeFleetLocationAttributesInputRequestTypeDef,
     DescribeFleetLocationCapacityInputRequestTypeDef,
     DescribeFleetLocationUtilizationInputRequestTypeDef,
     FleetUtilizationTypeDef,
     DescribeFleetPortSettingsInputRequestTypeDef,
+    IpPermissionOutputTypeDef,
     DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef,
     DescribeFleetUtilizationInputRequestTypeDef,
     DescribeGameServerGroupInputRequestTypeDef,
     DescribeGameServerInputRequestTypeDef,
     DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef,
     DescribeGameServerInstancesInputRequestTypeDef,
     GameServerInstanceTypeDef,
@@ -551,18 +557,25 @@
     DescribeScalingPoliciesInputDescribeScalingPoliciesPaginateTypeDef,
     DescribeScalingPoliciesInputRequestTypeDef,
     DescribeScriptInputRequestTypeDef,
     DescribeVpcPeeringConnectionsInputRequestTypeDef,
     DesiredPlayerSessionTypeDef,
     EC2InstanceCountsTypeDef,
     EmptyResponseMetadataTypeDef,
+    FilterConfigurationOutputTypeDef,
+    ResourceCreationLimitPolicyOutputTypeDef,
+    GamePropertyOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
+    InstanceDefinitionOutputTypeDef,
     MatchedPlayerSessionTypeDef,
     PlacedPlayerSessionTypeDef,
-    PlayerLatencyTypeDef,
+    PlayerLatencyOutputTypeDef,
+    GameSessionQueueDestinationOutputTypeDef,
+    PlayerLatencyPolicyOutputTypeDef,
+    PriorityConfigurationOutputTypeDef,
     GetComputeAccessInputRequestTypeDef,
     GetComputeAuthTokenInputRequestTypeDef,
     GetComputeAuthTokenOutputTypeDef,
     GetGameSessionLogUrlInputRequestTypeDef,
     GetGameSessionLogUrlOutputTypeDef,
     GetInstanceAccessInputRequestTypeDef,
     InstanceCredentialsTypeDef,
@@ -580,25 +593,29 @@
     ListGameServersInputListGameServersPaginateTypeDef,
     ListGameServersInputRequestTypeDef,
     ListLocationsInputListLocationsPaginateTypeDef,
     ListLocationsInputRequestTypeDef,
     ListScriptsInputListScriptsPaginateTypeDef,
     ListScriptsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
+    PlayerLatencyTypeDef,
     TargetConfigurationTypeDef,
     PutScalingPolicyOutputTypeDef,
     RegisterComputeInputRequestTypeDef,
     RegisterGameServerInputRequestTypeDef,
     RequestUploadCredentialsInputRequestTypeDef,
     ResolveAliasInputRequestTypeDef,
     ResolveAliasOutputTypeDef,
     ResponseMetadataTypeDef,
     ResumeGameServerGroupInputRequestTypeDef,
+    ServerProcessOutputTypeDef,
     ServerProcessTypeDef,
+    TargetConfigurationOutputTypeDef,
     SearchGameSessionsInputRequestTypeDef,
     SearchGameSessionsInputSearchGameSessionsPaginateTypeDef,
     StartFleetActionsInputRequestTypeDef,
     StartFleetActionsOutputTypeDef,
     StopFleetActionsInputRequestTypeDef,
     StopFleetActionsOutputTypeDef,
     StopGameSessionPlacementInputRequestTypeDef,
@@ -612,127 +629,129 @@
     UpdateFleetPortSettingsOutputTypeDef,
     UpdateGameServerInputRequestTypeDef,
     UpdateGameSessionInputRequestTypeDef,
     ValidateMatchmakingRuleSetInputRequestTypeDef,
     ValidateMatchmakingRuleSetOutputTypeDef,
     VpcPeeringConnectionStatusTypeDef,
     AliasTypeDef,
-    UpdateAliasInputRequestTypeDef,
+    PlayerOutputTypeDef,
     PlayerTypeDef,
     GetComputeAccessOutputTypeDef,
     DescribeBuildOutputTypeDef,
     ListBuildsOutputTypeDef,
     UpdateBuildOutputTypeDef,
     ClaimGameServerInputRequestTypeDef,
     ClaimGameServerOutputTypeDef,
     DescribeGameServerOutputTypeDef,
     ListGameServersOutputTypeDef,
     RegisterGameServerOutputTypeDef,
     UpdateGameServerOutputTypeDef,
     DescribeComputeOutputTypeDef,
     ListComputeOutputTypeDef,
     RegisterComputeOutputTypeDef,
+    UpdateAliasInputRequestTypeDef,
     CreateAliasInputRequestTypeDef,
     CreateLocationInputRequestTypeDef,
     CreateMatchmakingRuleSetInputRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateBuildInputRequestTypeDef,
-    CreateBuildOutputTypeDef,
     CreateScriptInputRequestTypeDef,
+    UpdateScriptInputRequestTypeDef,
+    CreateBuildOutputTypeDef,
     RequestUploadCredentialsOutputTypeDef,
     ScriptTypeDef,
-    UpdateScriptInputRequestTypeDef,
-    DescribeFleetPortSettingsOutputTypeDef,
     UpdateFleetPortSettingsInputRequestTypeDef,
     CreateFleetLocationsInputRequestTypeDef,
-    FleetAttributesTypeDef,
     UpdateFleetAttributesInputRequestTypeDef,
     CreateFleetLocationsOutputTypeDef,
     DeleteFleetLocationsOutputTypeDef,
     LocationAttributesTypeDef,
-    GameServerGroupTypeDef,
     UpdateGameServerGroupInputRequestTypeDef,
     CreateGameSessionInputRequestTypeDef,
     CreateMatchmakingConfigurationInputRequestTypeDef,
-    GameSessionTypeDef,
-    MatchmakingConfigurationTypeDef,
     UpdateMatchmakingConfigurationInputRequestTypeDef,
     CreateGameSessionQueueInputRequestTypeDef,
-    GameSessionQueueTypeDef,
     UpdateGameSessionQueueInputRequestTypeDef,
     CreateLocationOutputTypeDef,
     ListLocationsOutputTypeDef,
     CreateMatchmakingRuleSetOutputTypeDef,
     DescribeMatchmakingRuleSetsOutputTypeDef,
     CreatePlayerSessionOutputTypeDef,
     CreatePlayerSessionsOutputTypeDef,
     DescribePlayerSessionsOutputTypeDef,
     CreateVpcPeeringAuthorizationOutputTypeDef,
     DescribeVpcPeeringAuthorizationsOutputTypeDef,
     DescribeEC2InstanceLimitsOutputTypeDef,
     DescribeFleetEventsOutputTypeDef,
     DescribeFleetLocationUtilizationOutputTypeDef,
     DescribeFleetUtilizationOutputTypeDef,
+    DescribeFleetPortSettingsOutputTypeDef,
     DescribeGameServerInstancesOutputTypeDef,
     DescribeInstancesOutputTypeDef,
     FleetCapacityTypeDef,
+    FleetAttributesTypeDef,
+    GameSessionTypeDef,
+    MatchmakingConfigurationTypeDef,
     GameServerGroupAutoScalingPolicyTypeDef,
+    GameServerGroupTypeDef,
     GameSessionConnectionInfoTypeDef,
     GameSessionPlacementTypeDef,
-    StartGameSessionPlacementInputRequestTypeDef,
+    GameSessionQueueTypeDef,
     InstanceAccessTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartGameSessionPlacementInputRequestTypeDef,
     PutScalingPolicyInputRequestTypeDef,
-    ScalingPolicyTypeDef,
+    RuntimeConfigurationOutputTypeDef,
     RuntimeConfigurationTypeDef,
+    ScalingPolicyTypeDef,
     VpcPeeringConnectionTypeDef,
     CreateAliasOutputTypeDef,
     DescribeAliasOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
     StartMatchBackfillInputRequestTypeDef,
     StartMatchmakingInputRequestTypeDef,
     CreateScriptOutputTypeDef,
     DescribeScriptOutputTypeDef,
     ListScriptsOutputTypeDef,
     UpdateScriptOutputTypeDef,
+    DescribeFleetLocationAttributesOutputTypeDef,
+    DescribeFleetCapacityOutputTypeDef,
+    DescribeFleetLocationCapacityOutputTypeDef,
     CreateFleetOutputTypeDef,
     DescribeFleetAttributesOutputTypeDef,
-    DescribeFleetLocationAttributesOutputTypeDef,
-    CreateGameServerGroupOutputTypeDef,
-    DeleteGameServerGroupOutputTypeDef,
-    DescribeGameServerGroupOutputTypeDef,
-    ListGameServerGroupsOutputTypeDef,
-    ResumeGameServerGroupOutputTypeDef,
-    SuspendGameServerGroupOutputTypeDef,
-    UpdateGameServerGroupOutputTypeDef,
     CreateGameSessionOutputTypeDef,
     DescribeGameSessionsOutputTypeDef,
     GameSessionDetailTypeDef,
     SearchGameSessionsOutputTypeDef,
     UpdateGameSessionOutputTypeDef,
     CreateMatchmakingConfigurationOutputTypeDef,
     DescribeMatchmakingConfigurationsOutputTypeDef,
     UpdateMatchmakingConfigurationOutputTypeDef,
-    CreateGameSessionQueueOutputTypeDef,
-    DescribeGameSessionQueuesOutputTypeDef,
-    UpdateGameSessionQueueOutputTypeDef,
-    DescribeFleetCapacityOutputTypeDef,
-    DescribeFleetLocationCapacityOutputTypeDef,
     CreateGameServerGroupInputRequestTypeDef,
+    CreateGameServerGroupOutputTypeDef,
+    DeleteGameServerGroupOutputTypeDef,
+    DescribeGameServerGroupOutputTypeDef,
+    ListGameServerGroupsOutputTypeDef,
+    ResumeGameServerGroupOutputTypeDef,
+    SuspendGameServerGroupOutputTypeDef,
+    UpdateGameServerGroupOutputTypeDef,
     MatchmakingTicketTypeDef,
     DescribeGameSessionPlacementOutputTypeDef,
     StartGameSessionPlacementOutputTypeDef,
     StopGameSessionPlacementOutputTypeDef,
+    CreateGameSessionQueueOutputTypeDef,
+    DescribeGameSessionQueuesOutputTypeDef,
+    UpdateGameSessionQueueOutputTypeDef,
     GetInstanceAccessOutputTypeDef,
-    DescribeScalingPoliciesOutputTypeDef,
-    CreateFleetInputRequestTypeDef,
     DescribeRuntimeConfigurationOutputTypeDef,
-    UpdateRuntimeConfigurationInputRequestTypeDef,
     UpdateRuntimeConfigurationOutputTypeDef,
+    CreateFleetInputRequestTypeDef,
+    UpdateRuntimeConfigurationInputRequestTypeDef,
+    DescribeScalingPoliciesOutputTypeDef,
     DescribeVpcPeeringConnectionsOutputTypeDef,
     DescribeGameSessionDetailsOutputTypeDef,
     DescribeMatchmakingOutputTypeDef,
     StartMatchBackfillOutputTypeDef,
     StartMatchmakingOutputTypeDef,
 )
```

### Comparing `mypy-boto3-gamelift-1.28.0/README.md` & `mypy-boto3-gamelift-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-gamelift"></a>
 
 # mypy-boto3-gamelift
 
 [![PyPI - mypy-boto3-gamelift](https://img.shields.io/pypi/v/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-gamelift?color=blue)](https://pypistats.org/packages/mypy-boto3-gamelift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamelift)](https://pepy.tech/project/mypy-boto3-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameLift 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[boto3.GameLift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
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
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -425,25 +425,30 @@
 
 `mypy_boto3_gamelift.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_gamelift.type_defs import (
     AcceptMatchInputRequestTypeDef,
-    RoutingStrategyTypeDef,
+    RoutingStrategyOutputTypeDef,
+    AnywhereConfigurationOutputTypeDef,
     AnywhereConfigurationTypeDef,
+    AttributeValueOutputTypeDef,
     AttributeValueTypeDef,
     AwsCredentialsTypeDef,
     BuildTypeDef,
+    CertificateConfigurationOutputTypeDef,
     CertificateConfigurationTypeDef,
     ClaimFilterOptionTypeDef,
     GameServerTypeDef,
     ComputeTypeDef,
+    RoutingStrategyTypeDef,
     TagTypeDef,
     S3LocationTypeDef,
+    S3LocationOutputTypeDef,
     IpPermissionTypeDef,
     LocationConfigurationTypeDef,
     ResourceCreationLimitPolicyTypeDef,
     LocationStateTypeDef,
     InstanceDefinitionTypeDef,
     LaunchTemplateSpecificationTypeDef,
     GamePropertyTypeDef,
@@ -487,14 +492,15 @@
     DescribeFleetEventsInputRequestTypeDef,
     EventTypeDef,
     DescribeFleetLocationAttributesInputRequestTypeDef,
     DescribeFleetLocationCapacityInputRequestTypeDef,
     DescribeFleetLocationUtilizationInputRequestTypeDef,
     FleetUtilizationTypeDef,
     DescribeFleetPortSettingsInputRequestTypeDef,
+    IpPermissionOutputTypeDef,
     DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef,
     DescribeFleetUtilizationInputRequestTypeDef,
     DescribeGameServerGroupInputRequestTypeDef,
     DescribeGameServerInputRequestTypeDef,
     DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef,
     DescribeGameServerInstancesInputRequestTypeDef,
     GameServerInstanceTypeDef,
@@ -519,18 +525,25 @@
     DescribeScalingPoliciesInputDescribeScalingPoliciesPaginateTypeDef,
     DescribeScalingPoliciesInputRequestTypeDef,
     DescribeScriptInputRequestTypeDef,
     DescribeVpcPeeringConnectionsInputRequestTypeDef,
     DesiredPlayerSessionTypeDef,
     EC2InstanceCountsTypeDef,
     EmptyResponseMetadataTypeDef,
+    FilterConfigurationOutputTypeDef,
+    ResourceCreationLimitPolicyOutputTypeDef,
+    GamePropertyOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
+    InstanceDefinitionOutputTypeDef,
     MatchedPlayerSessionTypeDef,
     PlacedPlayerSessionTypeDef,
-    PlayerLatencyTypeDef,
+    PlayerLatencyOutputTypeDef,
+    GameSessionQueueDestinationOutputTypeDef,
+    PlayerLatencyPolicyOutputTypeDef,
+    PriorityConfigurationOutputTypeDef,
     GetComputeAccessInputRequestTypeDef,
     GetComputeAuthTokenInputRequestTypeDef,
     GetComputeAuthTokenOutputTypeDef,
     GetGameSessionLogUrlInputRequestTypeDef,
     GetGameSessionLogUrlOutputTypeDef,
     GetInstanceAccessInputRequestTypeDef,
     InstanceCredentialsTypeDef,
@@ -548,25 +561,29 @@
     ListGameServersInputListGameServersPaginateTypeDef,
     ListGameServersInputRequestTypeDef,
     ListLocationsInputListLocationsPaginateTypeDef,
     ListLocationsInputRequestTypeDef,
     ListScriptsInputListScriptsPaginateTypeDef,
     ListScriptsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
+    PlayerLatencyTypeDef,
     TargetConfigurationTypeDef,
     PutScalingPolicyOutputTypeDef,
     RegisterComputeInputRequestTypeDef,
     RegisterGameServerInputRequestTypeDef,
     RequestUploadCredentialsInputRequestTypeDef,
     ResolveAliasInputRequestTypeDef,
     ResolveAliasOutputTypeDef,
     ResponseMetadataTypeDef,
     ResumeGameServerGroupInputRequestTypeDef,
+    ServerProcessOutputTypeDef,
     ServerProcessTypeDef,
+    TargetConfigurationOutputTypeDef,
     SearchGameSessionsInputRequestTypeDef,
     SearchGameSessionsInputSearchGameSessionsPaginateTypeDef,
     StartFleetActionsInputRequestTypeDef,
     StartFleetActionsOutputTypeDef,
     StopFleetActionsInputRequestTypeDef,
     StopFleetActionsOutputTypeDef,
     StopGameSessionPlacementInputRequestTypeDef,
@@ -580,127 +597,129 @@
     UpdateFleetPortSettingsOutputTypeDef,
     UpdateGameServerInputRequestTypeDef,
     UpdateGameSessionInputRequestTypeDef,
     ValidateMatchmakingRuleSetInputRequestTypeDef,
     ValidateMatchmakingRuleSetOutputTypeDef,
     VpcPeeringConnectionStatusTypeDef,
     AliasTypeDef,
-    UpdateAliasInputRequestTypeDef,
+    PlayerOutputTypeDef,
     PlayerTypeDef,
     GetComputeAccessOutputTypeDef,
     DescribeBuildOutputTypeDef,
     ListBuildsOutputTypeDef,
     UpdateBuildOutputTypeDef,
     ClaimGameServerInputRequestTypeDef,
     ClaimGameServerOutputTypeDef,
     DescribeGameServerOutputTypeDef,
     ListGameServersOutputTypeDef,
     RegisterGameServerOutputTypeDef,
     UpdateGameServerOutputTypeDef,
     DescribeComputeOutputTypeDef,
     ListComputeOutputTypeDef,
     RegisterComputeOutputTypeDef,
+    UpdateAliasInputRequestTypeDef,
     CreateAliasInputRequestTypeDef,
     CreateLocationInputRequestTypeDef,
     CreateMatchmakingRuleSetInputRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateBuildInputRequestTypeDef,
-    CreateBuildOutputTypeDef,
     CreateScriptInputRequestTypeDef,
+    UpdateScriptInputRequestTypeDef,
+    CreateBuildOutputTypeDef,
     RequestUploadCredentialsOutputTypeDef,
     ScriptTypeDef,
-    UpdateScriptInputRequestTypeDef,
-    DescribeFleetPortSettingsOutputTypeDef,
     UpdateFleetPortSettingsInputRequestTypeDef,
     CreateFleetLocationsInputRequestTypeDef,
-    FleetAttributesTypeDef,
     UpdateFleetAttributesInputRequestTypeDef,
     CreateFleetLocationsOutputTypeDef,
     DeleteFleetLocationsOutputTypeDef,
     LocationAttributesTypeDef,
-    GameServerGroupTypeDef,
     UpdateGameServerGroupInputRequestTypeDef,
     CreateGameSessionInputRequestTypeDef,
     CreateMatchmakingConfigurationInputRequestTypeDef,
-    GameSessionTypeDef,
-    MatchmakingConfigurationTypeDef,
     UpdateMatchmakingConfigurationInputRequestTypeDef,
     CreateGameSessionQueueInputRequestTypeDef,
-    GameSessionQueueTypeDef,
     UpdateGameSessionQueueInputRequestTypeDef,
     CreateLocationOutputTypeDef,
     ListLocationsOutputTypeDef,
     CreateMatchmakingRuleSetOutputTypeDef,
     DescribeMatchmakingRuleSetsOutputTypeDef,
     CreatePlayerSessionOutputTypeDef,
     CreatePlayerSessionsOutputTypeDef,
     DescribePlayerSessionsOutputTypeDef,
     CreateVpcPeeringAuthorizationOutputTypeDef,
     DescribeVpcPeeringAuthorizationsOutputTypeDef,
     DescribeEC2InstanceLimitsOutputTypeDef,
     DescribeFleetEventsOutputTypeDef,
     DescribeFleetLocationUtilizationOutputTypeDef,
     DescribeFleetUtilizationOutputTypeDef,
+    DescribeFleetPortSettingsOutputTypeDef,
     DescribeGameServerInstancesOutputTypeDef,
     DescribeInstancesOutputTypeDef,
     FleetCapacityTypeDef,
+    FleetAttributesTypeDef,
+    GameSessionTypeDef,
+    MatchmakingConfigurationTypeDef,
     GameServerGroupAutoScalingPolicyTypeDef,
+    GameServerGroupTypeDef,
     GameSessionConnectionInfoTypeDef,
     GameSessionPlacementTypeDef,
-    StartGameSessionPlacementInputRequestTypeDef,
+    GameSessionQueueTypeDef,
     InstanceAccessTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartGameSessionPlacementInputRequestTypeDef,
     PutScalingPolicyInputRequestTypeDef,
-    ScalingPolicyTypeDef,
+    RuntimeConfigurationOutputTypeDef,
     RuntimeConfigurationTypeDef,
+    ScalingPolicyTypeDef,
     VpcPeeringConnectionTypeDef,
     CreateAliasOutputTypeDef,
     DescribeAliasOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
     StartMatchBackfillInputRequestTypeDef,
     StartMatchmakingInputRequestTypeDef,
     CreateScriptOutputTypeDef,
     DescribeScriptOutputTypeDef,
     ListScriptsOutputTypeDef,
     UpdateScriptOutputTypeDef,
+    DescribeFleetLocationAttributesOutputTypeDef,
+    DescribeFleetCapacityOutputTypeDef,
+    DescribeFleetLocationCapacityOutputTypeDef,
     CreateFleetOutputTypeDef,
     DescribeFleetAttributesOutputTypeDef,
-    DescribeFleetLocationAttributesOutputTypeDef,
-    CreateGameServerGroupOutputTypeDef,
-    DeleteGameServerGroupOutputTypeDef,
-    DescribeGameServerGroupOutputTypeDef,
-    ListGameServerGroupsOutputTypeDef,
-    ResumeGameServerGroupOutputTypeDef,
-    SuspendGameServerGroupOutputTypeDef,
-    UpdateGameServerGroupOutputTypeDef,
     CreateGameSessionOutputTypeDef,
     DescribeGameSessionsOutputTypeDef,
     GameSessionDetailTypeDef,
     SearchGameSessionsOutputTypeDef,
     UpdateGameSessionOutputTypeDef,
     CreateMatchmakingConfigurationOutputTypeDef,
     DescribeMatchmakingConfigurationsOutputTypeDef,
     UpdateMatchmakingConfigurationOutputTypeDef,
-    CreateGameSessionQueueOutputTypeDef,
-    DescribeGameSessionQueuesOutputTypeDef,
-    UpdateGameSessionQueueOutputTypeDef,
-    DescribeFleetCapacityOutputTypeDef,
-    DescribeFleetLocationCapacityOutputTypeDef,
     CreateGameServerGroupInputRequestTypeDef,
+    CreateGameServerGroupOutputTypeDef,
+    DeleteGameServerGroupOutputTypeDef,
+    DescribeGameServerGroupOutputTypeDef,
+    ListGameServerGroupsOutputTypeDef,
+    ResumeGameServerGroupOutputTypeDef,
+    SuspendGameServerGroupOutputTypeDef,
+    UpdateGameServerGroupOutputTypeDef,
     MatchmakingTicketTypeDef,
     DescribeGameSessionPlacementOutputTypeDef,
     StartGameSessionPlacementOutputTypeDef,
     StopGameSessionPlacementOutputTypeDef,
+    CreateGameSessionQueueOutputTypeDef,
+    DescribeGameSessionQueuesOutputTypeDef,
+    UpdateGameSessionQueueOutputTypeDef,
     GetInstanceAccessOutputTypeDef,
-    DescribeScalingPoliciesOutputTypeDef,
-    CreateFleetInputRequestTypeDef,
     DescribeRuntimeConfigurationOutputTypeDef,
-    UpdateRuntimeConfigurationInputRequestTypeDef,
     UpdateRuntimeConfigurationOutputTypeDef,
+    CreateFleetInputRequestTypeDef,
+    UpdateRuntimeConfigurationInputRequestTypeDef,
+    DescribeScalingPoliciesOutputTypeDef,
     DescribeVpcPeeringConnectionsOutputTypeDef,
     DescribeGameSessionDetailsOutputTypeDef,
     DescribeMatchmakingOutputTypeDef,
     StartMatchBackfillOutputTypeDef,
     StartMatchmakingOutputTypeDef,
 )
```

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/__init__.py` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/__init__.pyi` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/__main__.py` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GameLift 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.GameLift 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift\nOther"
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

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/client.py` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/client.pyi` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/literals.py` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AcceptanceTypeType",
     "BackfillModeType",
     "BalancingStrategyType",
     "BuildStatusType",
     "CertificateTypeType",
     "ComparisonOperatorTypeType",
@@ -88,15 +87,14 @@
     "GameLiftServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AcceptanceTypeType = Literal["ACCEPT", "REJECT"]
 BackfillModeType = Literal["AUTOMATIC", "MANUAL"]
 BalancingStrategyType = Literal["ON_DEMAND_ONLY", "SPOT_ONLY", "SPOT_PREFERRED"]
 BuildStatusType = Literal["FAILED", "INITIALIZED", "READY"]
 CertificateTypeType = Literal["DISABLED", "GENERATED"]
 ComparisonOperatorTypeType = Literal[
     "GreaterThanOrEqualToThreshold",
@@ -557,14 +555,15 @@
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
@@ -643,26 +642,28 @@
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

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/literals.pyi` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/literals.py`

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
     "AcceptanceTypeType",
     "BackfillModeType",
     "BalancingStrategyType",
     "BuildStatusType",
     "CertificateTypeType",
     "ComparisonOperatorTypeType",
@@ -87,14 +88,15 @@
     "GameLiftServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AcceptanceTypeType = Literal["ACCEPT", "REJECT"]
 BackfillModeType = Literal["AUTOMATIC", "MANUAL"]
 BalancingStrategyType = Literal["ON_DEMAND_ONLY", "SPOT_ONLY", "SPOT_PREFERRED"]
 BuildStatusType = Literal["FAILED", "INITIALIZED", "READY"]
 CertificateTypeType = Literal["DISABLED", "GENERATED"]
 ComparisonOperatorTypeType = Literal[
     "GreaterThanOrEqualToThreshold",
@@ -555,14 +557,15 @@
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
@@ -641,26 +644,28 @@
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

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/paginator.py` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/paginator.pyi` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/type_defs.py` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,25 +65,30 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptMatchInputRequestTypeDef",
-    "RoutingStrategyTypeDef",
+    "RoutingStrategyOutputTypeDef",
+    "AnywhereConfigurationOutputTypeDef",
     "AnywhereConfigurationTypeDef",
+    "AttributeValueOutputTypeDef",
     "AttributeValueTypeDef",
     "AwsCredentialsTypeDef",
     "BuildTypeDef",
+    "CertificateConfigurationOutputTypeDef",
     "CertificateConfigurationTypeDef",
     "ClaimFilterOptionTypeDef",
     "GameServerTypeDef",
     "ComputeTypeDef",
+    "RoutingStrategyTypeDef",
     "TagTypeDef",
     "S3LocationTypeDef",
+    "S3LocationOutputTypeDef",
     "IpPermissionTypeDef",
     "LocationConfigurationTypeDef",
     "ResourceCreationLimitPolicyTypeDef",
     "LocationStateTypeDef",
     "InstanceDefinitionTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "GamePropertyTypeDef",
@@ -127,14 +132,15 @@
     "DescribeFleetEventsInputRequestTypeDef",
     "EventTypeDef",
     "DescribeFleetLocationAttributesInputRequestTypeDef",
     "DescribeFleetLocationCapacityInputRequestTypeDef",
     "DescribeFleetLocationUtilizationInputRequestTypeDef",
     "FleetUtilizationTypeDef",
     "DescribeFleetPortSettingsInputRequestTypeDef",
+    "IpPermissionOutputTypeDef",
     "DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef",
     "DescribeFleetUtilizationInputRequestTypeDef",
     "DescribeGameServerGroupInputRequestTypeDef",
     "DescribeGameServerInputRequestTypeDef",
     "DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef",
     "DescribeGameServerInstancesInputRequestTypeDef",
     "GameServerInstanceTypeDef",
@@ -159,18 +165,25 @@
     "DescribeScalingPoliciesInputDescribeScalingPoliciesPaginateTypeDef",
     "DescribeScalingPoliciesInputRequestTypeDef",
     "DescribeScriptInputRequestTypeDef",
     "DescribeVpcPeeringConnectionsInputRequestTypeDef",
     "DesiredPlayerSessionTypeDef",
     "EC2InstanceCountsTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "FilterConfigurationOutputTypeDef",
+    "ResourceCreationLimitPolicyOutputTypeDef",
+    "GamePropertyOutputTypeDef",
     "TargetTrackingConfigurationTypeDef",
+    "InstanceDefinitionOutputTypeDef",
     "MatchedPlayerSessionTypeDef",
     "PlacedPlayerSessionTypeDef",
-    "PlayerLatencyTypeDef",
+    "PlayerLatencyOutputTypeDef",
+    "GameSessionQueueDestinationOutputTypeDef",
+    "PlayerLatencyPolicyOutputTypeDef",
+    "PriorityConfigurationOutputTypeDef",
     "GetComputeAccessInputRequestTypeDef",
     "GetComputeAuthTokenInputRequestTypeDef",
     "GetComputeAuthTokenOutputTypeDef",
     "GetGameSessionLogUrlInputRequestTypeDef",
     "GetGameSessionLogUrlOutputTypeDef",
     "GetInstanceAccessInputRequestTypeDef",
     "InstanceCredentialsTypeDef",
@@ -188,25 +201,29 @@
     "ListGameServersInputListGameServersPaginateTypeDef",
     "ListGameServersInputRequestTypeDef",
     "ListLocationsInputListLocationsPaginateTypeDef",
     "ListLocationsInputRequestTypeDef",
     "ListScriptsInputListScriptsPaginateTypeDef",
     "ListScriptsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
+    "PlayerLatencyTypeDef",
     "TargetConfigurationTypeDef",
     "PutScalingPolicyOutputTypeDef",
     "RegisterComputeInputRequestTypeDef",
     "RegisterGameServerInputRequestTypeDef",
     "RequestUploadCredentialsInputRequestTypeDef",
     "ResolveAliasInputRequestTypeDef",
     "ResolveAliasOutputTypeDef",
     "ResponseMetadataTypeDef",
     "ResumeGameServerGroupInputRequestTypeDef",
+    "ServerProcessOutputTypeDef",
     "ServerProcessTypeDef",
+    "TargetConfigurationOutputTypeDef",
     "SearchGameSessionsInputRequestTypeDef",
     "SearchGameSessionsInputSearchGameSessionsPaginateTypeDef",
     "StartFleetActionsInputRequestTypeDef",
     "StartFleetActionsOutputTypeDef",
     "StopFleetActionsInputRequestTypeDef",
     "StopFleetActionsOutputTypeDef",
     "StopGameSessionPlacementInputRequestTypeDef",
@@ -220,127 +237,129 @@
     "UpdateFleetPortSettingsOutputTypeDef",
     "UpdateGameServerInputRequestTypeDef",
     "UpdateGameSessionInputRequestTypeDef",
     "ValidateMatchmakingRuleSetInputRequestTypeDef",
     "ValidateMatchmakingRuleSetOutputTypeDef",
     "VpcPeeringConnectionStatusTypeDef",
     "AliasTypeDef",
-    "UpdateAliasInputRequestTypeDef",
+    "PlayerOutputTypeDef",
     "PlayerTypeDef",
     "GetComputeAccessOutputTypeDef",
     "DescribeBuildOutputTypeDef",
     "ListBuildsOutputTypeDef",
     "UpdateBuildOutputTypeDef",
     "ClaimGameServerInputRequestTypeDef",
     "ClaimGameServerOutputTypeDef",
     "DescribeGameServerOutputTypeDef",
     "ListGameServersOutputTypeDef",
     "RegisterGameServerOutputTypeDef",
     "UpdateGameServerOutputTypeDef",
     "DescribeComputeOutputTypeDef",
     "ListComputeOutputTypeDef",
     "RegisterComputeOutputTypeDef",
+    "UpdateAliasInputRequestTypeDef",
     "CreateAliasInputRequestTypeDef",
     "CreateLocationInputRequestTypeDef",
     "CreateMatchmakingRuleSetInputRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateBuildInputRequestTypeDef",
-    "CreateBuildOutputTypeDef",
     "CreateScriptInputRequestTypeDef",
+    "UpdateScriptInputRequestTypeDef",
+    "CreateBuildOutputTypeDef",
     "RequestUploadCredentialsOutputTypeDef",
     "ScriptTypeDef",
-    "UpdateScriptInputRequestTypeDef",
-    "DescribeFleetPortSettingsOutputTypeDef",
     "UpdateFleetPortSettingsInputRequestTypeDef",
     "CreateFleetLocationsInputRequestTypeDef",
-    "FleetAttributesTypeDef",
     "UpdateFleetAttributesInputRequestTypeDef",
     "CreateFleetLocationsOutputTypeDef",
     "DeleteFleetLocationsOutputTypeDef",
     "LocationAttributesTypeDef",
-    "GameServerGroupTypeDef",
     "UpdateGameServerGroupInputRequestTypeDef",
     "CreateGameSessionInputRequestTypeDef",
     "CreateMatchmakingConfigurationInputRequestTypeDef",
-    "GameSessionTypeDef",
-    "MatchmakingConfigurationTypeDef",
     "UpdateMatchmakingConfigurationInputRequestTypeDef",
     "CreateGameSessionQueueInputRequestTypeDef",
-    "GameSessionQueueTypeDef",
     "UpdateGameSessionQueueInputRequestTypeDef",
     "CreateLocationOutputTypeDef",
     "ListLocationsOutputTypeDef",
     "CreateMatchmakingRuleSetOutputTypeDef",
     "DescribeMatchmakingRuleSetsOutputTypeDef",
     "CreatePlayerSessionOutputTypeDef",
     "CreatePlayerSessionsOutputTypeDef",
     "DescribePlayerSessionsOutputTypeDef",
     "CreateVpcPeeringAuthorizationOutputTypeDef",
     "DescribeVpcPeeringAuthorizationsOutputTypeDef",
     "DescribeEC2InstanceLimitsOutputTypeDef",
     "DescribeFleetEventsOutputTypeDef",
     "DescribeFleetLocationUtilizationOutputTypeDef",
     "DescribeFleetUtilizationOutputTypeDef",
+    "DescribeFleetPortSettingsOutputTypeDef",
     "DescribeGameServerInstancesOutputTypeDef",
     "DescribeInstancesOutputTypeDef",
     "FleetCapacityTypeDef",
+    "FleetAttributesTypeDef",
+    "GameSessionTypeDef",
+    "MatchmakingConfigurationTypeDef",
     "GameServerGroupAutoScalingPolicyTypeDef",
+    "GameServerGroupTypeDef",
     "GameSessionConnectionInfoTypeDef",
     "GameSessionPlacementTypeDef",
-    "StartGameSessionPlacementInputRequestTypeDef",
+    "GameSessionQueueTypeDef",
     "InstanceAccessTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartGameSessionPlacementInputRequestTypeDef",
     "PutScalingPolicyInputRequestTypeDef",
-    "ScalingPolicyTypeDef",
+    "RuntimeConfigurationOutputTypeDef",
     "RuntimeConfigurationTypeDef",
+    "ScalingPolicyTypeDef",
     "VpcPeeringConnectionTypeDef",
     "CreateAliasOutputTypeDef",
     "DescribeAliasOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
     "StartMatchBackfillInputRequestTypeDef",
     "StartMatchmakingInputRequestTypeDef",
     "CreateScriptOutputTypeDef",
     "DescribeScriptOutputTypeDef",
     "ListScriptsOutputTypeDef",
     "UpdateScriptOutputTypeDef",
+    "DescribeFleetLocationAttributesOutputTypeDef",
+    "DescribeFleetCapacityOutputTypeDef",
+    "DescribeFleetLocationCapacityOutputTypeDef",
     "CreateFleetOutputTypeDef",
     "DescribeFleetAttributesOutputTypeDef",
-    "DescribeFleetLocationAttributesOutputTypeDef",
-    "CreateGameServerGroupOutputTypeDef",
-    "DeleteGameServerGroupOutputTypeDef",
-    "DescribeGameServerGroupOutputTypeDef",
-    "ListGameServerGroupsOutputTypeDef",
-    "ResumeGameServerGroupOutputTypeDef",
-    "SuspendGameServerGroupOutputTypeDef",
-    "UpdateGameServerGroupOutputTypeDef",
     "CreateGameSessionOutputTypeDef",
     "DescribeGameSessionsOutputTypeDef",
     "GameSessionDetailTypeDef",
     "SearchGameSessionsOutputTypeDef",
     "UpdateGameSessionOutputTypeDef",
     "CreateMatchmakingConfigurationOutputTypeDef",
     "DescribeMatchmakingConfigurationsOutputTypeDef",
     "UpdateMatchmakingConfigurationOutputTypeDef",
-    "CreateGameSessionQueueOutputTypeDef",
-    "DescribeGameSessionQueuesOutputTypeDef",
-    "UpdateGameSessionQueueOutputTypeDef",
-    "DescribeFleetCapacityOutputTypeDef",
-    "DescribeFleetLocationCapacityOutputTypeDef",
     "CreateGameServerGroupInputRequestTypeDef",
+    "CreateGameServerGroupOutputTypeDef",
+    "DeleteGameServerGroupOutputTypeDef",
+    "DescribeGameServerGroupOutputTypeDef",
+    "ListGameServerGroupsOutputTypeDef",
+    "ResumeGameServerGroupOutputTypeDef",
+    "SuspendGameServerGroupOutputTypeDef",
+    "UpdateGameServerGroupOutputTypeDef",
     "MatchmakingTicketTypeDef",
     "DescribeGameSessionPlacementOutputTypeDef",
     "StartGameSessionPlacementOutputTypeDef",
     "StopGameSessionPlacementOutputTypeDef",
+    "CreateGameSessionQueueOutputTypeDef",
+    "DescribeGameSessionQueuesOutputTypeDef",
+    "UpdateGameSessionQueueOutputTypeDef",
     "GetInstanceAccessOutputTypeDef",
-    "DescribeScalingPoliciesOutputTypeDef",
-    "CreateFleetInputRequestTypeDef",
     "DescribeRuntimeConfigurationOutputTypeDef",
-    "UpdateRuntimeConfigurationInputRequestTypeDef",
     "UpdateRuntimeConfigurationOutputTypeDef",
+    "CreateFleetInputRequestTypeDef",
+    "UpdateRuntimeConfigurationInputRequestTypeDef",
+    "DescribeScalingPoliciesOutputTypeDef",
     "DescribeVpcPeeringConnectionsOutputTypeDef",
     "DescribeGameSessionDetailsOutputTypeDef",
     "DescribeMatchmakingOutputTypeDef",
     "StartMatchBackfillOutputTypeDef",
     "StartMatchmakingOutputTypeDef",
 )
 
@@ -349,42 +368,60 @@
     {
         "TicketId": str,
         "PlayerIds": Sequence[str],
         "AcceptanceType": AcceptanceTypeType,
     },
 )
 
-RoutingStrategyTypeDef = TypedDict(
-    "RoutingStrategyTypeDef",
+RoutingStrategyOutputTypeDef = TypedDict(
+    "RoutingStrategyOutputTypeDef",
     {
         "Type": RoutingStrategyTypeType,
         "FleetId": str,
         "Message": str,
     },
     total=False,
 )
 
+AnywhereConfigurationOutputTypeDef = TypedDict(
+    "AnywhereConfigurationOutputTypeDef",
+    {
+        "Cost": str,
+    },
+)
+
 AnywhereConfigurationTypeDef = TypedDict(
     "AnywhereConfigurationTypeDef",
     {
         "Cost": str,
     },
 )
 
-AttributeValueTypeDef = TypedDict(
-    "AttributeValueTypeDef",
+AttributeValueOutputTypeDef = TypedDict(
+    "AttributeValueOutputTypeDef",
     {
         "S": str,
         "N": float,
         "SL": List[str],
         "SDM": Dict[str, float],
     },
     total=False,
 )
 
+AttributeValueTypeDef = TypedDict(
+    "AttributeValueTypeDef",
+    {
+        "S": str,
+        "N": float,
+        "SL": Sequence[str],
+        "SDM": Mapping[str, float],
+    },
+    total=False,
+)
+
 AwsCredentialsTypeDef = TypedDict(
     "AwsCredentialsTypeDef",
     {
         "AccessKeyId": str,
         "SecretAccessKey": str,
         "SessionToken": str,
     },
@@ -403,14 +440,21 @@
         "OperatingSystem": OperatingSystemType,
         "CreationTime": datetime,
         "ServerSdkVersion": str,
     },
     total=False,
 )
 
+CertificateConfigurationOutputTypeDef = TypedDict(
+    "CertificateConfigurationOutputTypeDef",
+    {
+        "CertificateType": CertificateTypeType,
+    },
+)
+
 CertificateConfigurationTypeDef = TypedDict(
     "CertificateConfigurationTypeDef",
     {
         "CertificateType": CertificateTypeType,
     },
 )
 
@@ -455,14 +499,24 @@
         "OperatingSystem": OperatingSystemType,
         "Type": EC2InstanceTypeType,
         "GameLiftServiceSdkEndpoint": str,
     },
     total=False,
 )
 
+RoutingStrategyTypeDef = TypedDict(
+    "RoutingStrategyTypeDef",
+    {
+        "Type": RoutingStrategyTypeType,
+        "FleetId": str,
+        "Message": str,
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
@@ -474,14 +528,25 @@
         "Key": str,
         "RoleArn": str,
         "ObjectVersion": str,
     },
     total=False,
 )
 
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+        "RoleArn": str,
+        "ObjectVersion": str,
+    },
+    total=False,
+)
+
 IpPermissionTypeDef = TypedDict(
     "IpPermissionTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
         "IpRange": str,
         "Protocol": IpProtocolType,
@@ -1050,14 +1115,24 @@
 class DescribeFleetPortSettingsInputRequestTypeDef(
     _RequiredDescribeFleetPortSettingsInputRequestTypeDef,
     _OptionalDescribeFleetPortSettingsInputRequestTypeDef,
 ):
     pass
 
 
+IpPermissionOutputTypeDef = TypedDict(
+    "IpPermissionOutputTypeDef",
+    {
+        "FromPort": int,
+        "ToPort": int,
+        "IpRange": str,
+        "Protocol": IpProtocolType,
+    },
+)
+
 DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef = TypedDict(
     "DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef",
     {
         "FleetIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1460,21 +1535,67 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FilterConfigurationOutputTypeDef = TypedDict(
+    "FilterConfigurationOutputTypeDef",
+    {
+        "AllowedLocations": List[str],
+    },
+    total=False,
+)
+
+ResourceCreationLimitPolicyOutputTypeDef = TypedDict(
+    "ResourceCreationLimitPolicyOutputTypeDef",
+    {
+        "NewGameSessionsPerCreator": int,
+        "PolicyPeriodInMinutes": int,
+    },
+    total=False,
+)
+
+GamePropertyOutputTypeDef = TypedDict(
+    "GamePropertyOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 TargetTrackingConfigurationTypeDef = TypedDict(
     "TargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 
+_RequiredInstanceDefinitionOutputTypeDef = TypedDict(
+    "_RequiredInstanceDefinitionOutputTypeDef",
+    {
+        "InstanceType": GameServerGroupInstanceTypeType,
+    },
+)
+_OptionalInstanceDefinitionOutputTypeDef = TypedDict(
+    "_OptionalInstanceDefinitionOutputTypeDef",
+    {
+        "WeightedCapacity": str,
+    },
+    total=False,
+)
+
+
+class InstanceDefinitionOutputTypeDef(
+    _RequiredInstanceDefinitionOutputTypeDef, _OptionalInstanceDefinitionOutputTypeDef
+):
+    pass
+
+
 MatchedPlayerSessionTypeDef = TypedDict(
     "MatchedPlayerSessionTypeDef",
     {
         "PlayerId": str,
         "PlayerSessionId": str,
     },
     total=False,
@@ -1485,24 +1606,50 @@
     {
         "PlayerId": str,
         "PlayerSessionId": str,
     },
     total=False,
 )
 
-PlayerLatencyTypeDef = TypedDict(
-    "PlayerLatencyTypeDef",
+PlayerLatencyOutputTypeDef = TypedDict(
+    "PlayerLatencyOutputTypeDef",
     {
         "PlayerId": str,
         "RegionIdentifier": str,
         "LatencyInMilliseconds": float,
     },
     total=False,
 )
 
+GameSessionQueueDestinationOutputTypeDef = TypedDict(
+    "GameSessionQueueDestinationOutputTypeDef",
+    {
+        "DestinationArn": str,
+    },
+    total=False,
+)
+
+PlayerLatencyPolicyOutputTypeDef = TypedDict(
+    "PlayerLatencyPolicyOutputTypeDef",
+    {
+        "MaximumIndividualPlayerLatencyMilliseconds": int,
+        "PolicyDurationSeconds": int,
+    },
+    total=False,
+)
+
+PriorityConfigurationOutputTypeDef = TypedDict(
+    "PriorityConfigurationOutputTypeDef",
+    {
+        "PriorityOrder": List[PriorityTypeType],
+        "LocationOrder": List[str],
+    },
+    total=False,
+)
+
 GetComputeAccessInputRequestTypeDef = TypedDict(
     "GetComputeAccessInputRequestTypeDef",
     {
         "FleetId": str,
         "ComputeName": str,
     },
 )
@@ -1778,24 +1925,42 @@
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
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PlayerLatencyTypeDef = TypedDict(
+    "PlayerLatencyTypeDef",
+    {
+        "PlayerId": str,
+        "RegionIdentifier": str,
+        "LatencyInMilliseconds": float,
+    },
+    total=False,
+)
+
 TargetConfigurationTypeDef = TypedDict(
     "TargetConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 
@@ -1894,14 +2059,36 @@
     "ResumeGameServerGroupInputRequestTypeDef",
     {
         "GameServerGroupName": str,
         "ResumeActions": Sequence[Literal["REPLACE_INSTANCE_TYPES"]],
     },
 )
 
+_RequiredServerProcessOutputTypeDef = TypedDict(
+    "_RequiredServerProcessOutputTypeDef",
+    {
+        "LaunchPath": str,
+        "ConcurrentExecutions": int,
+    },
+)
+_OptionalServerProcessOutputTypeDef = TypedDict(
+    "_OptionalServerProcessOutputTypeDef",
+    {
+        "Parameters": str,
+    },
+    total=False,
+)
+
+
+class ServerProcessOutputTypeDef(
+    _RequiredServerProcessOutputTypeDef, _OptionalServerProcessOutputTypeDef
+):
+    pass
+
+
 _RequiredServerProcessTypeDef = TypedDict(
     "_RequiredServerProcessTypeDef",
     {
         "LaunchPath": str,
         "ConcurrentExecutions": int,
     },
 )
@@ -1914,14 +2101,21 @@
 )
 
 
 class ServerProcessTypeDef(_RequiredServerProcessTypeDef, _OptionalServerProcessTypeDef):
     pass
 
 
+TargetConfigurationOutputTypeDef = TypedDict(
+    "TargetConfigurationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+
 SearchGameSessionsInputRequestTypeDef = TypedDict(
     "SearchGameSessionsInputRequestTypeDef",
     {
         "FleetId": str,
         "AliasId": str,
         "Location": str,
         "FilterExpression": str,
@@ -2186,51 +2380,39 @@
 AliasTypeDef = TypedDict(
     "AliasTypeDef",
     {
         "AliasId": str,
         "Name": str,
         "AliasArn": str,
         "Description": str,
-        "RoutingStrategy": RoutingStrategyTypeDef,
+        "RoutingStrategy": RoutingStrategyOutputTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
-_RequiredUpdateAliasInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateAliasInputRequestTypeDef",
+PlayerOutputTypeDef = TypedDict(
+    "PlayerOutputTypeDef",
     {
-        "AliasId": str,
-    },
-)
-_OptionalUpdateAliasInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateAliasInputRequestTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "RoutingStrategy": RoutingStrategyTypeDef,
+        "PlayerId": str,
+        "PlayerAttributes": Dict[str, AttributeValueOutputTypeDef],
+        "Team": str,
+        "LatencyInMs": Dict[str, int],
     },
     total=False,
 )
 
-
-class UpdateAliasInputRequestTypeDef(
-    _RequiredUpdateAliasInputRequestTypeDef, _OptionalUpdateAliasInputRequestTypeDef
-):
-    pass
-
-
 PlayerTypeDef = TypedDict(
     "PlayerTypeDef",
     {
         "PlayerId": str,
-        "PlayerAttributes": Dict[str, AttributeValueTypeDef],
+        "PlayerAttributes": Mapping[str, AttributeValueTypeDef],
         "Team": str,
-        "LatencyInMs": Dict[str, int],
+        "LatencyInMs": Mapping[str, int],
     },
     total=False,
 )
 
 GetComputeAccessOutputTypeDef = TypedDict(
     "GetComputeAccessOutputTypeDef",
     {
@@ -2353,14 +2535,37 @@
     "RegisterComputeOutputTypeDef",
     {
         "Compute": ComputeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredUpdateAliasInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateAliasInputRequestTypeDef",
+    {
+        "AliasId": str,
+    },
+)
+_OptionalUpdateAliasInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateAliasInputRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "RoutingStrategy": RoutingStrategyTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateAliasInputRequestTypeDef(
+    _RequiredUpdateAliasInputRequestTypeDef, _OptionalUpdateAliasInputRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateAliasInputRequestTypeDef = TypedDict(
     "_RequiredCreateAliasInputRequestTypeDef",
     {
         "Name": str,
         "RoutingStrategy": RoutingStrategyTypeDef,
     },
 )
@@ -2420,22 +2625,14 @@
 class CreateMatchmakingRuleSetInputRequestTypeDef(
     _RequiredCreateMatchmakingRuleSetInputRequestTypeDef,
     _OptionalCreateMatchmakingRuleSetInputRequestTypeDef,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -2449,59 +2646,26 @@
         "OperatingSystem": OperatingSystemType,
         "Tags": Sequence[TagTypeDef],
         "ServerSdkVersion": str,
     },
     total=False,
 )
 
-CreateBuildOutputTypeDef = TypedDict(
-    "CreateBuildOutputTypeDef",
-    {
-        "Build": BuildTypeDef,
-        "UploadCredentials": AwsCredentialsTypeDef,
-        "StorageLocation": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateScriptInputRequestTypeDef = TypedDict(
     "CreateScriptInputRequestTypeDef",
     {
         "Name": str,
         "Version": str,
         "StorageLocation": S3LocationTypeDef,
         "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-RequestUploadCredentialsOutputTypeDef = TypedDict(
-    "RequestUploadCredentialsOutputTypeDef",
-    {
-        "UploadCredentials": AwsCredentialsTypeDef,
-        "StorageLocation": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ScriptTypeDef = TypedDict(
-    "ScriptTypeDef",
-    {
-        "ScriptId": str,
-        "ScriptArn": str,
-        "Name": str,
-        "Version": str,
-        "SizeOnDisk": int,
-        "CreationTime": datetime,
-        "StorageLocation": S3LocationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateScriptInputRequestTypeDef = TypedDict(
     "_RequiredUpdateScriptInputRequestTypeDef",
     {
         "ScriptId": str,
     },
 )
 _OptionalUpdateScriptInputRequestTypeDef = TypedDict(
@@ -2518,26 +2682,47 @@
 
 class UpdateScriptInputRequestTypeDef(
     _RequiredUpdateScriptInputRequestTypeDef, _OptionalUpdateScriptInputRequestTypeDef
 ):
     pass
 
 
-DescribeFleetPortSettingsOutputTypeDef = TypedDict(
-    "DescribeFleetPortSettingsOutputTypeDef",
+CreateBuildOutputTypeDef = TypedDict(
+    "CreateBuildOutputTypeDef",
     {
-        "FleetId": str,
-        "FleetArn": str,
-        "InboundPermissions": List[IpPermissionTypeDef],
-        "UpdateStatus": Literal["PENDING_UPDATE"],
-        "Location": str,
+        "Build": BuildTypeDef,
+        "UploadCredentials": AwsCredentialsTypeDef,
+        "StorageLocation": S3LocationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RequestUploadCredentialsOutputTypeDef = TypedDict(
+    "RequestUploadCredentialsOutputTypeDef",
+    {
+        "UploadCredentials": AwsCredentialsTypeDef,
+        "StorageLocation": S3LocationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ScriptTypeDef = TypedDict(
+    "ScriptTypeDef",
+    {
+        "ScriptId": str,
+        "ScriptArn": str,
+        "Name": str,
+        "Version": str,
+        "SizeOnDisk": int,
+        "CreationTime": datetime,
+        "StorageLocation": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateFleetPortSettingsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetPortSettingsInputRequestTypeDef",
     {
         "FleetId": str,
     },
 )
 _OptionalUpdateFleetPortSettingsInputRequestTypeDef = TypedDict(
@@ -2561,46 +2746,14 @@
     "CreateFleetLocationsInputRequestTypeDef",
     {
         "FleetId": str,
         "Locations": Sequence[LocationConfigurationTypeDef],
     },
 )
 
-FleetAttributesTypeDef = TypedDict(
-    "FleetAttributesTypeDef",
-    {
-        "FleetId": str,
-        "FleetArn": str,
-        "FleetType": FleetTypeType,
-        "InstanceType": EC2InstanceTypeType,
-        "Description": str,
-        "Name": str,
-        "CreationTime": datetime,
-        "TerminationTime": datetime,
-        "Status": FleetStatusType,
-        "BuildId": str,
-        "BuildArn": str,
-        "ScriptId": str,
-        "ScriptArn": str,
-        "ServerLaunchPath": str,
-        "ServerLaunchParameters": str,
-        "LogPaths": List[str],
-        "NewGameSessionProtectionPolicy": ProtectionPolicyType,
-        "OperatingSystem": OperatingSystemType,
-        "ResourceCreationLimitPolicy": ResourceCreationLimitPolicyTypeDef,
-        "MetricGroups": List[str],
-        "StoppedActions": List[Literal["AUTO_SCALING"]],
-        "InstanceRoleArn": str,
-        "CertificateConfiguration": CertificateConfigurationTypeDef,
-        "ComputeType": ComputeTypeType,
-        "AnywhereConfiguration": AnywhereConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateFleetAttributesInputRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetAttributesInputRequestTypeDef",
     {
         "FleetId": str,
     },
 )
 _OptionalUpdateFleetAttributesInputRequestTypeDef = TypedDict(
@@ -2650,33 +2803,14 @@
         "LocationState": LocationStateTypeDef,
         "StoppedActions": List[Literal["AUTO_SCALING"]],
         "UpdateStatus": Literal["PENDING_UPDATE"],
     },
     total=False,
 )
 
-GameServerGroupTypeDef = TypedDict(
-    "GameServerGroupTypeDef",
-    {
-        "GameServerGroupName": str,
-        "GameServerGroupArn": str,
-        "RoleArn": str,
-        "InstanceDefinitions": List[InstanceDefinitionTypeDef],
-        "BalancingStrategy": BalancingStrategyType,
-        "GameServerProtectionPolicy": GameServerProtectionPolicyType,
-        "AutoScalingGroupArn": str,
-        "Status": GameServerGroupStatusType,
-        "StatusReason": str,
-        "SuspendedActions": List[Literal["REPLACE_INSTANCE_TYPES"]],
-        "CreationTime": datetime,
-        "LastUpdatedTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateGameServerGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGameServerGroupInputRequestTypeDef",
     {
         "GameServerGroupName": str,
     },
 )
 _OptionalUpdateGameServerGroupInputRequestTypeDef = TypedDict(
@@ -2758,64 +2892,14 @@
 class CreateMatchmakingConfigurationInputRequestTypeDef(
     _RequiredCreateMatchmakingConfigurationInputRequestTypeDef,
     _OptionalCreateMatchmakingConfigurationInputRequestTypeDef,
 ):
     pass
 
 
-GameSessionTypeDef = TypedDict(
-    "GameSessionTypeDef",
-    {
-        "GameSessionId": str,
-        "Name": str,
-        "FleetId": str,
-        "FleetArn": str,
-        "CreationTime": datetime,
-        "TerminationTime": datetime,
-        "CurrentPlayerSessionCount": int,
-        "MaximumPlayerSessionCount": int,
-        "Status": GameSessionStatusType,
-        "StatusReason": Literal["INTERRUPTED"],
-        "GameProperties": List[GamePropertyTypeDef],
-        "IpAddress": str,
-        "DnsName": str,
-        "Port": int,
-        "PlayerSessionCreationPolicy": PlayerSessionCreationPolicyType,
-        "CreatorId": str,
-        "GameSessionData": str,
-        "MatchmakerData": str,
-        "Location": str,
-    },
-    total=False,
-)
-
-MatchmakingConfigurationTypeDef = TypedDict(
-    "MatchmakingConfigurationTypeDef",
-    {
-        "Name": str,
-        "ConfigurationArn": str,
-        "Description": str,
-        "GameSessionQueueArns": List[str],
-        "RequestTimeoutSeconds": int,
-        "AcceptanceTimeoutSeconds": int,
-        "AcceptanceRequired": bool,
-        "RuleSetName": str,
-        "RuleSetArn": str,
-        "NotificationTarget": str,
-        "AdditionalPlayerCount": int,
-        "CustomEventData": str,
-        "CreationTime": datetime,
-        "GameProperties": List[GamePropertyTypeDef],
-        "GameSessionData": str,
-        "BackfillMode": BackfillModeType,
-        "FlexMatchMode": FlexMatchModeType,
-    },
-    total=False,
-)
-
 _RequiredUpdateMatchmakingConfigurationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMatchmakingConfigurationInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateMatchmakingConfigurationInputRequestTypeDef = TypedDict(
@@ -2871,30 +2955,14 @@
 class CreateGameSessionQueueInputRequestTypeDef(
     _RequiredCreateGameSessionQueueInputRequestTypeDef,
     _OptionalCreateGameSessionQueueInputRequestTypeDef,
 ):
     pass
 
 
-GameSessionQueueTypeDef = TypedDict(
-    "GameSessionQueueTypeDef",
-    {
-        "Name": str,
-        "GameSessionQueueArn": str,
-        "TimeoutInSeconds": int,
-        "PlayerLatencyPolicies": List[PlayerLatencyPolicyTypeDef],
-        "Destinations": List[GameSessionQueueDestinationTypeDef],
-        "FilterConfiguration": FilterConfigurationTypeDef,
-        "PriorityConfiguration": PriorityConfigurationTypeDef,
-        "CustomEventData": str,
-        "NotificationTarget": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateGameSessionQueueInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGameSessionQueueInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateGameSessionQueueInputRequestTypeDef = TypedDict(
@@ -3024,14 +3092,26 @@
     {
         "FleetUtilization": List[FleetUtilizationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeFleetPortSettingsOutputTypeDef = TypedDict(
+    "DescribeFleetPortSettingsOutputTypeDef",
+    {
+        "FleetId": str,
+        "FleetArn": str,
+        "InboundPermissions": List[IpPermissionOutputTypeDef],
+        "UpdateStatus": Literal["PENDING_UPDATE"],
+        "Location": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeGameServerInstancesOutputTypeDef = TypedDict(
     "DescribeGameServerInstancesOutputTypeDef",
     {
         "GameServerInstances": List[GameServerInstanceTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -3054,14 +3134,96 @@
         "InstanceType": EC2InstanceTypeType,
         "InstanceCounts": EC2InstanceCountsTypeDef,
         "Location": str,
     },
     total=False,
 )
 
+FleetAttributesTypeDef = TypedDict(
+    "FleetAttributesTypeDef",
+    {
+        "FleetId": str,
+        "FleetArn": str,
+        "FleetType": FleetTypeType,
+        "InstanceType": EC2InstanceTypeType,
+        "Description": str,
+        "Name": str,
+        "CreationTime": datetime,
+        "TerminationTime": datetime,
+        "Status": FleetStatusType,
+        "BuildId": str,
+        "BuildArn": str,
+        "ScriptId": str,
+        "ScriptArn": str,
+        "ServerLaunchPath": str,
+        "ServerLaunchParameters": str,
+        "LogPaths": List[str],
+        "NewGameSessionProtectionPolicy": ProtectionPolicyType,
+        "OperatingSystem": OperatingSystemType,
+        "ResourceCreationLimitPolicy": ResourceCreationLimitPolicyOutputTypeDef,
+        "MetricGroups": List[str],
+        "StoppedActions": List[Literal["AUTO_SCALING"]],
+        "InstanceRoleArn": str,
+        "CertificateConfiguration": CertificateConfigurationOutputTypeDef,
+        "ComputeType": ComputeTypeType,
+        "AnywhereConfiguration": AnywhereConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+GameSessionTypeDef = TypedDict(
+    "GameSessionTypeDef",
+    {
+        "GameSessionId": str,
+        "Name": str,
+        "FleetId": str,
+        "FleetArn": str,
+        "CreationTime": datetime,
+        "TerminationTime": datetime,
+        "CurrentPlayerSessionCount": int,
+        "MaximumPlayerSessionCount": int,
+        "Status": GameSessionStatusType,
+        "StatusReason": Literal["INTERRUPTED"],
+        "GameProperties": List[GamePropertyOutputTypeDef],
+        "IpAddress": str,
+        "DnsName": str,
+        "Port": int,
+        "PlayerSessionCreationPolicy": PlayerSessionCreationPolicyType,
+        "CreatorId": str,
+        "GameSessionData": str,
+        "MatchmakerData": str,
+        "Location": str,
+    },
+    total=False,
+)
+
+MatchmakingConfigurationTypeDef = TypedDict(
+    "MatchmakingConfigurationTypeDef",
+    {
+        "Name": str,
+        "ConfigurationArn": str,
+        "Description": str,
+        "GameSessionQueueArns": List[str],
+        "RequestTimeoutSeconds": int,
+        "AcceptanceTimeoutSeconds": int,
+        "AcceptanceRequired": bool,
+        "RuleSetName": str,
+        "RuleSetArn": str,
+        "NotificationTarget": str,
+        "AdditionalPlayerCount": int,
+        "CustomEventData": str,
+        "CreationTime": datetime,
+        "GameProperties": List[GamePropertyOutputTypeDef],
+        "GameSessionData": str,
+        "BackfillMode": BackfillModeType,
+        "FlexMatchMode": FlexMatchModeType,
+    },
+    total=False,
+)
+
 _RequiredGameServerGroupAutoScalingPolicyTypeDef = TypedDict(
     "_RequiredGameServerGroupAutoScalingPolicyTypeDef",
     {
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
     },
 )
 _OptionalGameServerGroupAutoScalingPolicyTypeDef = TypedDict(
@@ -3076,14 +3238,33 @@
 class GameServerGroupAutoScalingPolicyTypeDef(
     _RequiredGameServerGroupAutoScalingPolicyTypeDef,
     _OptionalGameServerGroupAutoScalingPolicyTypeDef,
 ):
     pass
 
 
+GameServerGroupTypeDef = TypedDict(
+    "GameServerGroupTypeDef",
+    {
+        "GameServerGroupName": str,
+        "GameServerGroupArn": str,
+        "RoleArn": str,
+        "InstanceDefinitions": List[InstanceDefinitionOutputTypeDef],
+        "BalancingStrategy": BalancingStrategyType,
+        "GameServerProtectionPolicy": GameServerProtectionPolicyType,
+        "AutoScalingGroupArn": str,
+        "Status": GameServerGroupStatusType,
+        "StatusReason": str,
+        "SuspendedActions": List[Literal["REPLACE_INSTANCE_TYPES"]],
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+    },
+    total=False,
+)
+
 GameSessionConnectionInfoTypeDef = TypedDict(
     "GameSessionConnectionInfoTypeDef",
     {
         "GameSessionArn": str,
         "IpAddress": str,
         "DnsName": str,
         "Port": int,
@@ -3094,33 +3275,69 @@
 
 GameSessionPlacementTypeDef = TypedDict(
     "GameSessionPlacementTypeDef",
     {
         "PlacementId": str,
         "GameSessionQueueName": str,
         "Status": GameSessionPlacementStateType,
-        "GameProperties": List[GamePropertyTypeDef],
+        "GameProperties": List[GamePropertyOutputTypeDef],
         "MaximumPlayerSessionCount": int,
         "GameSessionName": str,
         "GameSessionId": str,
         "GameSessionArn": str,
         "GameSessionRegion": str,
-        "PlayerLatencies": List[PlayerLatencyTypeDef],
+        "PlayerLatencies": List[PlayerLatencyOutputTypeDef],
         "StartTime": datetime,
         "EndTime": datetime,
         "IpAddress": str,
         "DnsName": str,
         "Port": int,
         "PlacedPlayerSessions": List[PlacedPlayerSessionTypeDef],
         "GameSessionData": str,
         "MatchmakerData": str,
     },
     total=False,
 )
 
+GameSessionQueueTypeDef = TypedDict(
+    "GameSessionQueueTypeDef",
+    {
+        "Name": str,
+        "GameSessionQueueArn": str,
+        "TimeoutInSeconds": int,
+        "PlayerLatencyPolicies": List[PlayerLatencyPolicyOutputTypeDef],
+        "Destinations": List[GameSessionQueueDestinationOutputTypeDef],
+        "FilterConfiguration": FilterConfigurationOutputTypeDef,
+        "PriorityConfiguration": PriorityConfigurationOutputTypeDef,
+        "CustomEventData": str,
+        "NotificationTarget": str,
+    },
+    total=False,
+)
+
+InstanceAccessTypeDef = TypedDict(
+    "InstanceAccessTypeDef",
+    {
+        "FleetId": str,
+        "InstanceId": str,
+        "IpAddress": str,
+        "OperatingSystem": OperatingSystemType,
+        "Credentials": InstanceCredentialsTypeDef,
+    },
+    total=False,
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartGameSessionPlacementInputRequestTypeDef = TypedDict(
     "_RequiredStartGameSessionPlacementInputRequestTypeDef",
     {
         "PlacementId": str,
         "GameSessionQueueName": str,
         "MaximumPlayerSessionCount": int,
     },
@@ -3141,26 +3358,14 @@
 class StartGameSessionPlacementInputRequestTypeDef(
     _RequiredStartGameSessionPlacementInputRequestTypeDef,
     _OptionalStartGameSessionPlacementInputRequestTypeDef,
 ):
     pass
 
 
-InstanceAccessTypeDef = TypedDict(
-    "InstanceAccessTypeDef",
-    {
-        "FleetId": str,
-        "InstanceId": str,
-        "IpAddress": str,
-        "OperatingSystem": OperatingSystemType,
-        "Credentials": InstanceCredentialsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredPutScalingPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutScalingPolicyInputRequestTypeDef",
     {
         "Name": str,
         "FleetId": str,
         "MetricName": MetricNameType,
     },
@@ -3182,45 +3387,55 @@
 
 class PutScalingPolicyInputRequestTypeDef(
     _RequiredPutScalingPolicyInputRequestTypeDef, _OptionalPutScalingPolicyInputRequestTypeDef
 ):
     pass
 
 
+RuntimeConfigurationOutputTypeDef = TypedDict(
+    "RuntimeConfigurationOutputTypeDef",
+    {
+        "ServerProcesses": List[ServerProcessOutputTypeDef],
+        "MaxConcurrentGameSessionActivations": int,
+        "GameSessionActivationTimeoutSeconds": int,
+    },
+    total=False,
+)
+
+RuntimeConfigurationTypeDef = TypedDict(
+    "RuntimeConfigurationTypeDef",
+    {
+        "ServerProcesses": Sequence[ServerProcessTypeDef],
+        "MaxConcurrentGameSessionActivations": int,
+        "GameSessionActivationTimeoutSeconds": int,
+    },
+    total=False,
+)
+
 ScalingPolicyTypeDef = TypedDict(
     "ScalingPolicyTypeDef",
     {
         "FleetId": str,
         "FleetArn": str,
         "Name": str,
         "Status": ScalingStatusTypeType,
         "ScalingAdjustment": int,
         "ScalingAdjustmentType": ScalingAdjustmentTypeType,
         "ComparisonOperator": ComparisonOperatorTypeType,
         "Threshold": float,
         "EvaluationPeriods": int,
         "MetricName": MetricNameType,
         "PolicyType": PolicyTypeType,
-        "TargetConfiguration": TargetConfigurationTypeDef,
+        "TargetConfiguration": TargetConfigurationOutputTypeDef,
         "UpdateStatus": Literal["PENDING_UPDATE"],
         "Location": str,
     },
     total=False,
 )
 
-RuntimeConfigurationTypeDef = TypedDict(
-    "RuntimeConfigurationTypeDef",
-    {
-        "ServerProcesses": Sequence[ServerProcessTypeDef],
-        "MaxConcurrentGameSessionActivations": int,
-        "GameSessionActivationTimeoutSeconds": int,
-    },
-    total=False,
-)
-
 VpcPeeringConnectionTypeDef = TypedDict(
     "VpcPeeringConnectionTypeDef",
     {
         "FleetId": str,
         "FleetArn": str,
         "IpV4CidrBlock": str,
         "VpcPeeringConnectionId": str,
@@ -3338,96 +3553,56 @@
     "UpdateScriptOutputTypeDef",
     {
         "Script": ScriptTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFleetOutputTypeDef = TypedDict(
-    "CreateFleetOutputTypeDef",
-    {
-        "FleetAttributes": FleetAttributesTypeDef,
-        "LocationStates": List[LocationStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeFleetAttributesOutputTypeDef = TypedDict(
-    "DescribeFleetAttributesOutputTypeDef",
-    {
-        "FleetAttributes": List[FleetAttributesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFleetLocationAttributesOutputTypeDef = TypedDict(
     "DescribeFleetLocationAttributesOutputTypeDef",
     {
         "FleetId": str,
         "FleetArn": str,
         "LocationAttributes": List[LocationAttributesTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateGameServerGroupOutputTypeDef = TypedDict(
-    "CreateGameServerGroupOutputTypeDef",
-    {
-        "GameServerGroup": GameServerGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteGameServerGroupOutputTypeDef = TypedDict(
-    "DeleteGameServerGroupOutputTypeDef",
-    {
-        "GameServerGroup": GameServerGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeGameServerGroupOutputTypeDef = TypedDict(
-    "DescribeGameServerGroupOutputTypeDef",
-    {
-        "GameServerGroup": GameServerGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListGameServerGroupsOutputTypeDef = TypedDict(
-    "ListGameServerGroupsOutputTypeDef",
+DescribeFleetCapacityOutputTypeDef = TypedDict(
+    "DescribeFleetCapacityOutputTypeDef",
     {
-        "GameServerGroups": List[GameServerGroupTypeDef],
+        "FleetCapacity": List[FleetCapacityTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResumeGameServerGroupOutputTypeDef = TypedDict(
-    "ResumeGameServerGroupOutputTypeDef",
+DescribeFleetLocationCapacityOutputTypeDef = TypedDict(
+    "DescribeFleetLocationCapacityOutputTypeDef",
     {
-        "GameServerGroup": GameServerGroupTypeDef,
+        "FleetCapacity": FleetCapacityTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SuspendGameServerGroupOutputTypeDef = TypedDict(
-    "SuspendGameServerGroupOutputTypeDef",
+CreateFleetOutputTypeDef = TypedDict(
+    "CreateFleetOutputTypeDef",
     {
-        "GameServerGroup": GameServerGroupTypeDef,
+        "FleetAttributes": FleetAttributesTypeDef,
+        "LocationStates": List[LocationStateTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateGameServerGroupOutputTypeDef = TypedDict(
-    "UpdateGameServerGroupOutputTypeDef",
+DescribeFleetAttributesOutputTypeDef = TypedDict(
+    "DescribeFleetAttributesOutputTypeDef",
     {
-        "GameServerGroup": GameServerGroupTypeDef,
+        "FleetAttributes": List[FleetAttributesTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateGameSessionOutputTypeDef = TypedDict(
     "CreateGameSessionOutputTypeDef",
     {
@@ -3492,99 +3667,114 @@
     "UpdateMatchmakingConfigurationOutputTypeDef",
     {
         "Configuration": MatchmakingConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateGameSessionQueueOutputTypeDef = TypedDict(
-    "CreateGameSessionQueueOutputTypeDef",
+_RequiredCreateGameServerGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateGameServerGroupInputRequestTypeDef",
     {
-        "GameSessionQueue": GameSessionQueueTypeDef,
+        "GameServerGroupName": str,
+        "RoleArn": str,
+        "MinSize": int,
+        "MaxSize": int,
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
+        "InstanceDefinitions": Sequence[InstanceDefinitionTypeDef],
+    },
+)
+_OptionalCreateGameServerGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateGameServerGroupInputRequestTypeDef",
+    {
+        "AutoScalingPolicy": GameServerGroupAutoScalingPolicyTypeDef,
+        "BalancingStrategy": BalancingStrategyType,
+        "GameServerProtectionPolicy": GameServerProtectionPolicyType,
+        "VpcSubnets": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateGameServerGroupInputRequestTypeDef(
+    _RequiredCreateGameServerGroupInputRequestTypeDef,
+    _OptionalCreateGameServerGroupInputRequestTypeDef,
+):
+    pass
+
+
+CreateGameServerGroupOutputTypeDef = TypedDict(
+    "CreateGameServerGroupOutputTypeDef",
+    {
+        "GameServerGroup": GameServerGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeGameSessionQueuesOutputTypeDef = TypedDict(
-    "DescribeGameSessionQueuesOutputTypeDef",
+DeleteGameServerGroupOutputTypeDef = TypedDict(
+    "DeleteGameServerGroupOutputTypeDef",
     {
-        "GameSessionQueues": List[GameSessionQueueTypeDef],
-        "NextToken": str,
+        "GameServerGroup": GameServerGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateGameSessionQueueOutputTypeDef = TypedDict(
-    "UpdateGameSessionQueueOutputTypeDef",
+DescribeGameServerGroupOutputTypeDef = TypedDict(
+    "DescribeGameServerGroupOutputTypeDef",
     {
-        "GameSessionQueue": GameSessionQueueTypeDef,
+        "GameServerGroup": GameServerGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetCapacityOutputTypeDef = TypedDict(
-    "DescribeFleetCapacityOutputTypeDef",
+ListGameServerGroupsOutputTypeDef = TypedDict(
+    "ListGameServerGroupsOutputTypeDef",
     {
-        "FleetCapacity": List[FleetCapacityTypeDef],
+        "GameServerGroups": List[GameServerGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetLocationCapacityOutputTypeDef = TypedDict(
-    "DescribeFleetLocationCapacityOutputTypeDef",
+ResumeGameServerGroupOutputTypeDef = TypedDict(
+    "ResumeGameServerGroupOutputTypeDef",
     {
-        "FleetCapacity": FleetCapacityTypeDef,
+        "GameServerGroup": GameServerGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateGameServerGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateGameServerGroupInputRequestTypeDef",
+SuspendGameServerGroupOutputTypeDef = TypedDict(
+    "SuspendGameServerGroupOutputTypeDef",
     {
-        "GameServerGroupName": str,
-        "RoleArn": str,
-        "MinSize": int,
-        "MaxSize": int,
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "InstanceDefinitions": Sequence[InstanceDefinitionTypeDef],
+        "GameServerGroup": GameServerGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateGameServerGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateGameServerGroupInputRequestTypeDef",
+
+UpdateGameServerGroupOutputTypeDef = TypedDict(
+    "UpdateGameServerGroupOutputTypeDef",
     {
-        "AutoScalingPolicy": GameServerGroupAutoScalingPolicyTypeDef,
-        "BalancingStrategy": BalancingStrategyType,
-        "GameServerProtectionPolicy": GameServerProtectionPolicyType,
-        "VpcSubnets": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
+        "GameServerGroup": GameServerGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class CreateGameServerGroupInputRequestTypeDef(
-    _RequiredCreateGameServerGroupInputRequestTypeDef,
-    _OptionalCreateGameServerGroupInputRequestTypeDef,
-):
-    pass
-
-
 MatchmakingTicketTypeDef = TypedDict(
     "MatchmakingTicketTypeDef",
     {
         "TicketId": str,
         "ConfigurationName": str,
         "ConfigurationArn": str,
         "Status": MatchmakingConfigurationStatusType,
         "StatusReason": str,
         "StatusMessage": str,
         "StartTime": datetime,
         "EndTime": datetime,
-        "Players": List[PlayerTypeDef],
+        "Players": List[PlayerOutputTypeDef],
         "GameSessionConnectionInfo": GameSessionConnectionInfoTypeDef,
         "EstimatedWaitTime": int,
     },
     total=False,
 )
 
 DescribeGameSessionPlacementOutputTypeDef = TypedDict(
@@ -3607,27 +3797,59 @@
     "StopGameSessionPlacementOutputTypeDef",
     {
         "GameSessionPlacement": GameSessionPlacementTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateGameSessionQueueOutputTypeDef = TypedDict(
+    "CreateGameSessionQueueOutputTypeDef",
+    {
+        "GameSessionQueue": GameSessionQueueTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeGameSessionQueuesOutputTypeDef = TypedDict(
+    "DescribeGameSessionQueuesOutputTypeDef",
+    {
+        "GameSessionQueues": List[GameSessionQueueTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateGameSessionQueueOutputTypeDef = TypedDict(
+    "UpdateGameSessionQueueOutputTypeDef",
+    {
+        "GameSessionQueue": GameSessionQueueTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetInstanceAccessOutputTypeDef = TypedDict(
     "GetInstanceAccessOutputTypeDef",
     {
         "InstanceAccess": InstanceAccessTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeScalingPoliciesOutputTypeDef = TypedDict(
-    "DescribeScalingPoliciesOutputTypeDef",
+DescribeRuntimeConfigurationOutputTypeDef = TypedDict(
+    "DescribeRuntimeConfigurationOutputTypeDef",
     {
-        "ScalingPolicies": List[ScalingPolicyTypeDef],
-        "NextToken": str,
+        "RuntimeConfiguration": RuntimeConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateRuntimeConfigurationOutputTypeDef = TypedDict(
+    "UpdateRuntimeConfigurationOutputTypeDef",
+    {
+        "RuntimeConfiguration": RuntimeConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFleetInputRequestTypeDef = TypedDict(
     "_RequiredCreateFleetInputRequestTypeDef",
     {
@@ -3665,34 +3887,27 @@
 
 class CreateFleetInputRequestTypeDef(
     _RequiredCreateFleetInputRequestTypeDef, _OptionalCreateFleetInputRequestTypeDef
 ):
     pass
 
 
-DescribeRuntimeConfigurationOutputTypeDef = TypedDict(
-    "DescribeRuntimeConfigurationOutputTypeDef",
-    {
-        "RuntimeConfiguration": RuntimeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateRuntimeConfigurationInputRequestTypeDef = TypedDict(
     "UpdateRuntimeConfigurationInputRequestTypeDef",
     {
         "FleetId": str,
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
     },
 )
 
-UpdateRuntimeConfigurationOutputTypeDef = TypedDict(
-    "UpdateRuntimeConfigurationOutputTypeDef",
+DescribeScalingPoliciesOutputTypeDef = TypedDict(
+    "DescribeScalingPoliciesOutputTypeDef",
     {
-        "RuntimeConfiguration": RuntimeConfigurationTypeDef,
+        "ScalingPolicies": List[ScalingPolicyTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVpcPeeringConnectionsOutputTypeDef = TypedDict(
     "DescribeVpcPeeringConnectionsOutputTypeDef",
     {
```

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift/type_defs.pyi` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -64,25 +64,30 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptMatchInputRequestTypeDef",
-    "RoutingStrategyTypeDef",
+    "RoutingStrategyOutputTypeDef",
+    "AnywhereConfigurationOutputTypeDef",
     "AnywhereConfigurationTypeDef",
+    "AttributeValueOutputTypeDef",
     "AttributeValueTypeDef",
     "AwsCredentialsTypeDef",
     "BuildTypeDef",
+    "CertificateConfigurationOutputTypeDef",
     "CertificateConfigurationTypeDef",
     "ClaimFilterOptionTypeDef",
     "GameServerTypeDef",
     "ComputeTypeDef",
+    "RoutingStrategyTypeDef",
     "TagTypeDef",
     "S3LocationTypeDef",
+    "S3LocationOutputTypeDef",
     "IpPermissionTypeDef",
     "LocationConfigurationTypeDef",
     "ResourceCreationLimitPolicyTypeDef",
     "LocationStateTypeDef",
     "InstanceDefinitionTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "GamePropertyTypeDef",
@@ -126,14 +131,15 @@
     "DescribeFleetEventsInputRequestTypeDef",
     "EventTypeDef",
     "DescribeFleetLocationAttributesInputRequestTypeDef",
     "DescribeFleetLocationCapacityInputRequestTypeDef",
     "DescribeFleetLocationUtilizationInputRequestTypeDef",
     "FleetUtilizationTypeDef",
     "DescribeFleetPortSettingsInputRequestTypeDef",
+    "IpPermissionOutputTypeDef",
     "DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef",
     "DescribeFleetUtilizationInputRequestTypeDef",
     "DescribeGameServerGroupInputRequestTypeDef",
     "DescribeGameServerInputRequestTypeDef",
     "DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef",
     "DescribeGameServerInstancesInputRequestTypeDef",
     "GameServerInstanceTypeDef",
@@ -158,18 +164,25 @@
     "DescribeScalingPoliciesInputDescribeScalingPoliciesPaginateTypeDef",
     "DescribeScalingPoliciesInputRequestTypeDef",
     "DescribeScriptInputRequestTypeDef",
     "DescribeVpcPeeringConnectionsInputRequestTypeDef",
     "DesiredPlayerSessionTypeDef",
     "EC2InstanceCountsTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "FilterConfigurationOutputTypeDef",
+    "ResourceCreationLimitPolicyOutputTypeDef",
+    "GamePropertyOutputTypeDef",
     "TargetTrackingConfigurationTypeDef",
+    "InstanceDefinitionOutputTypeDef",
     "MatchedPlayerSessionTypeDef",
     "PlacedPlayerSessionTypeDef",
-    "PlayerLatencyTypeDef",
+    "PlayerLatencyOutputTypeDef",
+    "GameSessionQueueDestinationOutputTypeDef",
+    "PlayerLatencyPolicyOutputTypeDef",
+    "PriorityConfigurationOutputTypeDef",
     "GetComputeAccessInputRequestTypeDef",
     "GetComputeAuthTokenInputRequestTypeDef",
     "GetComputeAuthTokenOutputTypeDef",
     "GetGameSessionLogUrlInputRequestTypeDef",
     "GetGameSessionLogUrlOutputTypeDef",
     "GetInstanceAccessInputRequestTypeDef",
     "InstanceCredentialsTypeDef",
@@ -187,25 +200,29 @@
     "ListGameServersInputListGameServersPaginateTypeDef",
     "ListGameServersInputRequestTypeDef",
     "ListLocationsInputListLocationsPaginateTypeDef",
     "ListLocationsInputRequestTypeDef",
     "ListScriptsInputListScriptsPaginateTypeDef",
     "ListScriptsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
+    "PlayerLatencyTypeDef",
     "TargetConfigurationTypeDef",
     "PutScalingPolicyOutputTypeDef",
     "RegisterComputeInputRequestTypeDef",
     "RegisterGameServerInputRequestTypeDef",
     "RequestUploadCredentialsInputRequestTypeDef",
     "ResolveAliasInputRequestTypeDef",
     "ResolveAliasOutputTypeDef",
     "ResponseMetadataTypeDef",
     "ResumeGameServerGroupInputRequestTypeDef",
+    "ServerProcessOutputTypeDef",
     "ServerProcessTypeDef",
+    "TargetConfigurationOutputTypeDef",
     "SearchGameSessionsInputRequestTypeDef",
     "SearchGameSessionsInputSearchGameSessionsPaginateTypeDef",
     "StartFleetActionsInputRequestTypeDef",
     "StartFleetActionsOutputTypeDef",
     "StopFleetActionsInputRequestTypeDef",
     "StopFleetActionsOutputTypeDef",
     "StopGameSessionPlacementInputRequestTypeDef",
@@ -219,127 +236,129 @@
     "UpdateFleetPortSettingsOutputTypeDef",
     "UpdateGameServerInputRequestTypeDef",
     "UpdateGameSessionInputRequestTypeDef",
     "ValidateMatchmakingRuleSetInputRequestTypeDef",
     "ValidateMatchmakingRuleSetOutputTypeDef",
     "VpcPeeringConnectionStatusTypeDef",
     "AliasTypeDef",
-    "UpdateAliasInputRequestTypeDef",
+    "PlayerOutputTypeDef",
     "PlayerTypeDef",
     "GetComputeAccessOutputTypeDef",
     "DescribeBuildOutputTypeDef",
     "ListBuildsOutputTypeDef",
     "UpdateBuildOutputTypeDef",
     "ClaimGameServerInputRequestTypeDef",
     "ClaimGameServerOutputTypeDef",
     "DescribeGameServerOutputTypeDef",
     "ListGameServersOutputTypeDef",
     "RegisterGameServerOutputTypeDef",
     "UpdateGameServerOutputTypeDef",
     "DescribeComputeOutputTypeDef",
     "ListComputeOutputTypeDef",
     "RegisterComputeOutputTypeDef",
+    "UpdateAliasInputRequestTypeDef",
     "CreateAliasInputRequestTypeDef",
     "CreateLocationInputRequestTypeDef",
     "CreateMatchmakingRuleSetInputRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateBuildInputRequestTypeDef",
-    "CreateBuildOutputTypeDef",
     "CreateScriptInputRequestTypeDef",
+    "UpdateScriptInputRequestTypeDef",
+    "CreateBuildOutputTypeDef",
     "RequestUploadCredentialsOutputTypeDef",
     "ScriptTypeDef",
-    "UpdateScriptInputRequestTypeDef",
-    "DescribeFleetPortSettingsOutputTypeDef",
     "UpdateFleetPortSettingsInputRequestTypeDef",
     "CreateFleetLocationsInputRequestTypeDef",
-    "FleetAttributesTypeDef",
     "UpdateFleetAttributesInputRequestTypeDef",
     "CreateFleetLocationsOutputTypeDef",
     "DeleteFleetLocationsOutputTypeDef",
     "LocationAttributesTypeDef",
-    "GameServerGroupTypeDef",
     "UpdateGameServerGroupInputRequestTypeDef",
     "CreateGameSessionInputRequestTypeDef",
     "CreateMatchmakingConfigurationInputRequestTypeDef",
-    "GameSessionTypeDef",
-    "MatchmakingConfigurationTypeDef",
     "UpdateMatchmakingConfigurationInputRequestTypeDef",
     "CreateGameSessionQueueInputRequestTypeDef",
-    "GameSessionQueueTypeDef",
     "UpdateGameSessionQueueInputRequestTypeDef",
     "CreateLocationOutputTypeDef",
     "ListLocationsOutputTypeDef",
     "CreateMatchmakingRuleSetOutputTypeDef",
     "DescribeMatchmakingRuleSetsOutputTypeDef",
     "CreatePlayerSessionOutputTypeDef",
     "CreatePlayerSessionsOutputTypeDef",
     "DescribePlayerSessionsOutputTypeDef",
     "CreateVpcPeeringAuthorizationOutputTypeDef",
     "DescribeVpcPeeringAuthorizationsOutputTypeDef",
     "DescribeEC2InstanceLimitsOutputTypeDef",
     "DescribeFleetEventsOutputTypeDef",
     "DescribeFleetLocationUtilizationOutputTypeDef",
     "DescribeFleetUtilizationOutputTypeDef",
+    "DescribeFleetPortSettingsOutputTypeDef",
     "DescribeGameServerInstancesOutputTypeDef",
     "DescribeInstancesOutputTypeDef",
     "FleetCapacityTypeDef",
+    "FleetAttributesTypeDef",
+    "GameSessionTypeDef",
+    "MatchmakingConfigurationTypeDef",
     "GameServerGroupAutoScalingPolicyTypeDef",
+    "GameServerGroupTypeDef",
     "GameSessionConnectionInfoTypeDef",
     "GameSessionPlacementTypeDef",
-    "StartGameSessionPlacementInputRequestTypeDef",
+    "GameSessionQueueTypeDef",
     "InstanceAccessTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartGameSessionPlacementInputRequestTypeDef",
     "PutScalingPolicyInputRequestTypeDef",
-    "ScalingPolicyTypeDef",
+    "RuntimeConfigurationOutputTypeDef",
     "RuntimeConfigurationTypeDef",
+    "ScalingPolicyTypeDef",
     "VpcPeeringConnectionTypeDef",
     "CreateAliasOutputTypeDef",
     "DescribeAliasOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
     "StartMatchBackfillInputRequestTypeDef",
     "StartMatchmakingInputRequestTypeDef",
     "CreateScriptOutputTypeDef",
     "DescribeScriptOutputTypeDef",
     "ListScriptsOutputTypeDef",
     "UpdateScriptOutputTypeDef",
+    "DescribeFleetLocationAttributesOutputTypeDef",
+    "DescribeFleetCapacityOutputTypeDef",
+    "DescribeFleetLocationCapacityOutputTypeDef",
     "CreateFleetOutputTypeDef",
     "DescribeFleetAttributesOutputTypeDef",
-    "DescribeFleetLocationAttributesOutputTypeDef",
-    "CreateGameServerGroupOutputTypeDef",
-    "DeleteGameServerGroupOutputTypeDef",
-    "DescribeGameServerGroupOutputTypeDef",
-    "ListGameServerGroupsOutputTypeDef",
-    "ResumeGameServerGroupOutputTypeDef",
-    "SuspendGameServerGroupOutputTypeDef",
-    "UpdateGameServerGroupOutputTypeDef",
     "CreateGameSessionOutputTypeDef",
     "DescribeGameSessionsOutputTypeDef",
     "GameSessionDetailTypeDef",
     "SearchGameSessionsOutputTypeDef",
     "UpdateGameSessionOutputTypeDef",
     "CreateMatchmakingConfigurationOutputTypeDef",
     "DescribeMatchmakingConfigurationsOutputTypeDef",
     "UpdateMatchmakingConfigurationOutputTypeDef",
-    "CreateGameSessionQueueOutputTypeDef",
-    "DescribeGameSessionQueuesOutputTypeDef",
-    "UpdateGameSessionQueueOutputTypeDef",
-    "DescribeFleetCapacityOutputTypeDef",
-    "DescribeFleetLocationCapacityOutputTypeDef",
     "CreateGameServerGroupInputRequestTypeDef",
+    "CreateGameServerGroupOutputTypeDef",
+    "DeleteGameServerGroupOutputTypeDef",
+    "DescribeGameServerGroupOutputTypeDef",
+    "ListGameServerGroupsOutputTypeDef",
+    "ResumeGameServerGroupOutputTypeDef",
+    "SuspendGameServerGroupOutputTypeDef",
+    "UpdateGameServerGroupOutputTypeDef",
     "MatchmakingTicketTypeDef",
     "DescribeGameSessionPlacementOutputTypeDef",
     "StartGameSessionPlacementOutputTypeDef",
     "StopGameSessionPlacementOutputTypeDef",
+    "CreateGameSessionQueueOutputTypeDef",
+    "DescribeGameSessionQueuesOutputTypeDef",
+    "UpdateGameSessionQueueOutputTypeDef",
     "GetInstanceAccessOutputTypeDef",
-    "DescribeScalingPoliciesOutputTypeDef",
-    "CreateFleetInputRequestTypeDef",
     "DescribeRuntimeConfigurationOutputTypeDef",
-    "UpdateRuntimeConfigurationInputRequestTypeDef",
     "UpdateRuntimeConfigurationOutputTypeDef",
+    "CreateFleetInputRequestTypeDef",
+    "UpdateRuntimeConfigurationInputRequestTypeDef",
+    "DescribeScalingPoliciesOutputTypeDef",
     "DescribeVpcPeeringConnectionsOutputTypeDef",
     "DescribeGameSessionDetailsOutputTypeDef",
     "DescribeMatchmakingOutputTypeDef",
     "StartMatchBackfillOutputTypeDef",
     "StartMatchmakingOutputTypeDef",
 )
 
@@ -348,42 +367,60 @@
     {
         "TicketId": str,
         "PlayerIds": Sequence[str],
         "AcceptanceType": AcceptanceTypeType,
     },
 )
 
-RoutingStrategyTypeDef = TypedDict(
-    "RoutingStrategyTypeDef",
+RoutingStrategyOutputTypeDef = TypedDict(
+    "RoutingStrategyOutputTypeDef",
     {
         "Type": RoutingStrategyTypeType,
         "FleetId": str,
         "Message": str,
     },
     total=False,
 )
 
+AnywhereConfigurationOutputTypeDef = TypedDict(
+    "AnywhereConfigurationOutputTypeDef",
+    {
+        "Cost": str,
+    },
+)
+
 AnywhereConfigurationTypeDef = TypedDict(
     "AnywhereConfigurationTypeDef",
     {
         "Cost": str,
     },
 )
 
-AttributeValueTypeDef = TypedDict(
-    "AttributeValueTypeDef",
+AttributeValueOutputTypeDef = TypedDict(
+    "AttributeValueOutputTypeDef",
     {
         "S": str,
         "N": float,
         "SL": List[str],
         "SDM": Dict[str, float],
     },
     total=False,
 )
 
+AttributeValueTypeDef = TypedDict(
+    "AttributeValueTypeDef",
+    {
+        "S": str,
+        "N": float,
+        "SL": Sequence[str],
+        "SDM": Mapping[str, float],
+    },
+    total=False,
+)
+
 AwsCredentialsTypeDef = TypedDict(
     "AwsCredentialsTypeDef",
     {
         "AccessKeyId": str,
         "SecretAccessKey": str,
         "SessionToken": str,
     },
@@ -402,14 +439,21 @@
         "OperatingSystem": OperatingSystemType,
         "CreationTime": datetime,
         "ServerSdkVersion": str,
     },
     total=False,
 )
 
+CertificateConfigurationOutputTypeDef = TypedDict(
+    "CertificateConfigurationOutputTypeDef",
+    {
+        "CertificateType": CertificateTypeType,
+    },
+)
+
 CertificateConfigurationTypeDef = TypedDict(
     "CertificateConfigurationTypeDef",
     {
         "CertificateType": CertificateTypeType,
     },
 )
 
@@ -454,14 +498,24 @@
         "OperatingSystem": OperatingSystemType,
         "Type": EC2InstanceTypeType,
         "GameLiftServiceSdkEndpoint": str,
     },
     total=False,
 )
 
+RoutingStrategyTypeDef = TypedDict(
+    "RoutingStrategyTypeDef",
+    {
+        "Type": RoutingStrategyTypeType,
+        "FleetId": str,
+        "Message": str,
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
@@ -473,14 +527,25 @@
         "Key": str,
         "RoleArn": str,
         "ObjectVersion": str,
     },
     total=False,
 )
 
+S3LocationOutputTypeDef = TypedDict(
+    "S3LocationOutputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+        "RoleArn": str,
+        "ObjectVersion": str,
+    },
+    total=False,
+)
+
 IpPermissionTypeDef = TypedDict(
     "IpPermissionTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
         "IpRange": str,
         "Protocol": IpProtocolType,
@@ -1031,14 +1096,24 @@
 
 class DescribeFleetPortSettingsInputRequestTypeDef(
     _RequiredDescribeFleetPortSettingsInputRequestTypeDef,
     _OptionalDescribeFleetPortSettingsInputRequestTypeDef,
 ):
     pass
 
+IpPermissionOutputTypeDef = TypedDict(
+    "IpPermissionOutputTypeDef",
+    {
+        "FromPort": int,
+        "ToPort": int,
+        "IpRange": str,
+        "Protocol": IpProtocolType,
+    },
+)
+
 DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef = TypedDict(
     "DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef",
     {
         "FleetIds": Sequence[str],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1429,21 +1504,65 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+FilterConfigurationOutputTypeDef = TypedDict(
+    "FilterConfigurationOutputTypeDef",
+    {
+        "AllowedLocations": List[str],
+    },
+    total=False,
+)
+
+ResourceCreationLimitPolicyOutputTypeDef = TypedDict(
+    "ResourceCreationLimitPolicyOutputTypeDef",
+    {
+        "NewGameSessionsPerCreator": int,
+        "PolicyPeriodInMinutes": int,
+    },
+    total=False,
+)
+
+GamePropertyOutputTypeDef = TypedDict(
+    "GamePropertyOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 TargetTrackingConfigurationTypeDef = TypedDict(
     "TargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 
+_RequiredInstanceDefinitionOutputTypeDef = TypedDict(
+    "_RequiredInstanceDefinitionOutputTypeDef",
+    {
+        "InstanceType": GameServerGroupInstanceTypeType,
+    },
+)
+_OptionalInstanceDefinitionOutputTypeDef = TypedDict(
+    "_OptionalInstanceDefinitionOutputTypeDef",
+    {
+        "WeightedCapacity": str,
+    },
+    total=False,
+)
+
+class InstanceDefinitionOutputTypeDef(
+    _RequiredInstanceDefinitionOutputTypeDef, _OptionalInstanceDefinitionOutputTypeDef
+):
+    pass
+
 MatchedPlayerSessionTypeDef = TypedDict(
     "MatchedPlayerSessionTypeDef",
     {
         "PlayerId": str,
         "PlayerSessionId": str,
     },
     total=False,
@@ -1454,24 +1573,50 @@
     {
         "PlayerId": str,
         "PlayerSessionId": str,
     },
     total=False,
 )
 
-PlayerLatencyTypeDef = TypedDict(
-    "PlayerLatencyTypeDef",
+PlayerLatencyOutputTypeDef = TypedDict(
+    "PlayerLatencyOutputTypeDef",
     {
         "PlayerId": str,
         "RegionIdentifier": str,
         "LatencyInMilliseconds": float,
     },
     total=False,
 )
 
+GameSessionQueueDestinationOutputTypeDef = TypedDict(
+    "GameSessionQueueDestinationOutputTypeDef",
+    {
+        "DestinationArn": str,
+    },
+    total=False,
+)
+
+PlayerLatencyPolicyOutputTypeDef = TypedDict(
+    "PlayerLatencyPolicyOutputTypeDef",
+    {
+        "MaximumIndividualPlayerLatencyMilliseconds": int,
+        "PolicyDurationSeconds": int,
+    },
+    total=False,
+)
+
+PriorityConfigurationOutputTypeDef = TypedDict(
+    "PriorityConfigurationOutputTypeDef",
+    {
+        "PriorityOrder": List[PriorityTypeType],
+        "LocationOrder": List[str],
+    },
+    total=False,
+)
+
 GetComputeAccessInputRequestTypeDef = TypedDict(
     "GetComputeAccessInputRequestTypeDef",
     {
         "FleetId": str,
         "ComputeName": str,
     },
 )
@@ -1739,24 +1884,42 @@
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
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+PlayerLatencyTypeDef = TypedDict(
+    "PlayerLatencyTypeDef",
+    {
+        "PlayerId": str,
+        "RegionIdentifier": str,
+        "LatencyInMilliseconds": float,
+    },
+    total=False,
+)
+
 TargetConfigurationTypeDef = TypedDict(
     "TargetConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 
@@ -1851,14 +2014,34 @@
     "ResumeGameServerGroupInputRequestTypeDef",
     {
         "GameServerGroupName": str,
         "ResumeActions": Sequence[Literal["REPLACE_INSTANCE_TYPES"]],
     },
 )
 
+_RequiredServerProcessOutputTypeDef = TypedDict(
+    "_RequiredServerProcessOutputTypeDef",
+    {
+        "LaunchPath": str,
+        "ConcurrentExecutions": int,
+    },
+)
+_OptionalServerProcessOutputTypeDef = TypedDict(
+    "_OptionalServerProcessOutputTypeDef",
+    {
+        "Parameters": str,
+    },
+    total=False,
+)
+
+class ServerProcessOutputTypeDef(
+    _RequiredServerProcessOutputTypeDef, _OptionalServerProcessOutputTypeDef
+):
+    pass
+
 _RequiredServerProcessTypeDef = TypedDict(
     "_RequiredServerProcessTypeDef",
     {
         "LaunchPath": str,
         "ConcurrentExecutions": int,
     },
 )
@@ -1869,14 +2052,21 @@
     },
     total=False,
 )
 
 class ServerProcessTypeDef(_RequiredServerProcessTypeDef, _OptionalServerProcessTypeDef):
     pass
 
+TargetConfigurationOutputTypeDef = TypedDict(
+    "TargetConfigurationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+
 SearchGameSessionsInputRequestTypeDef = TypedDict(
     "SearchGameSessionsInputRequestTypeDef",
     {
         "FleetId": str,
         "AliasId": str,
         "Location": str,
         "FilterExpression": str,
@@ -2129,49 +2319,39 @@
 AliasTypeDef = TypedDict(
     "AliasTypeDef",
     {
         "AliasId": str,
         "Name": str,
         "AliasArn": str,
         "Description": str,
-        "RoutingStrategy": RoutingStrategyTypeDef,
+        "RoutingStrategy": RoutingStrategyOutputTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
-_RequiredUpdateAliasInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateAliasInputRequestTypeDef",
+PlayerOutputTypeDef = TypedDict(
+    "PlayerOutputTypeDef",
     {
-        "AliasId": str,
-    },
-)
-_OptionalUpdateAliasInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateAliasInputRequestTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "RoutingStrategy": RoutingStrategyTypeDef,
+        "PlayerId": str,
+        "PlayerAttributes": Dict[str, AttributeValueOutputTypeDef],
+        "Team": str,
+        "LatencyInMs": Dict[str, int],
     },
     total=False,
 )
 
-class UpdateAliasInputRequestTypeDef(
-    _RequiredUpdateAliasInputRequestTypeDef, _OptionalUpdateAliasInputRequestTypeDef
-):
-    pass
-
 PlayerTypeDef = TypedDict(
     "PlayerTypeDef",
     {
         "PlayerId": str,
-        "PlayerAttributes": Dict[str, AttributeValueTypeDef],
+        "PlayerAttributes": Mapping[str, AttributeValueTypeDef],
         "Team": str,
-        "LatencyInMs": Dict[str, int],
+        "LatencyInMs": Mapping[str, int],
     },
     total=False,
 )
 
 GetComputeAccessOutputTypeDef = TypedDict(
     "GetComputeAccessOutputTypeDef",
     {
@@ -2292,14 +2472,35 @@
     "RegisterComputeOutputTypeDef",
     {
         "Compute": ComputeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredUpdateAliasInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateAliasInputRequestTypeDef",
+    {
+        "AliasId": str,
+    },
+)
+_OptionalUpdateAliasInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateAliasInputRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "RoutingStrategy": RoutingStrategyTypeDef,
+    },
+    total=False,
+)
+
+class UpdateAliasInputRequestTypeDef(
+    _RequiredUpdateAliasInputRequestTypeDef, _OptionalUpdateAliasInputRequestTypeDef
+):
+    pass
+
 _RequiredCreateAliasInputRequestTypeDef = TypedDict(
     "_RequiredCreateAliasInputRequestTypeDef",
     {
         "Name": str,
         "RoutingStrategy": RoutingStrategyTypeDef,
     },
 )
@@ -2353,22 +2554,14 @@
 
 class CreateMatchmakingRuleSetInputRequestTypeDef(
     _RequiredCreateMatchmakingRuleSetInputRequestTypeDef,
     _OptionalCreateMatchmakingRuleSetInputRequestTypeDef,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -2382,59 +2575,26 @@
         "OperatingSystem": OperatingSystemType,
         "Tags": Sequence[TagTypeDef],
         "ServerSdkVersion": str,
     },
     total=False,
 )
 
-CreateBuildOutputTypeDef = TypedDict(
-    "CreateBuildOutputTypeDef",
-    {
-        "Build": BuildTypeDef,
-        "UploadCredentials": AwsCredentialsTypeDef,
-        "StorageLocation": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateScriptInputRequestTypeDef = TypedDict(
     "CreateScriptInputRequestTypeDef",
     {
         "Name": str,
         "Version": str,
         "StorageLocation": S3LocationTypeDef,
         "ZipFile": Union[str, bytes, IO[Any], StreamingBody],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-RequestUploadCredentialsOutputTypeDef = TypedDict(
-    "RequestUploadCredentialsOutputTypeDef",
-    {
-        "UploadCredentials": AwsCredentialsTypeDef,
-        "StorageLocation": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ScriptTypeDef = TypedDict(
-    "ScriptTypeDef",
-    {
-        "ScriptId": str,
-        "ScriptArn": str,
-        "Name": str,
-        "Version": str,
-        "SizeOnDisk": int,
-        "CreationTime": datetime,
-        "StorageLocation": S3LocationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateScriptInputRequestTypeDef = TypedDict(
     "_RequiredUpdateScriptInputRequestTypeDef",
     {
         "ScriptId": str,
     },
 )
 _OptionalUpdateScriptInputRequestTypeDef = TypedDict(
@@ -2449,26 +2609,47 @@
 )
 
 class UpdateScriptInputRequestTypeDef(
     _RequiredUpdateScriptInputRequestTypeDef, _OptionalUpdateScriptInputRequestTypeDef
 ):
     pass
 
-DescribeFleetPortSettingsOutputTypeDef = TypedDict(
-    "DescribeFleetPortSettingsOutputTypeDef",
+CreateBuildOutputTypeDef = TypedDict(
+    "CreateBuildOutputTypeDef",
     {
-        "FleetId": str,
-        "FleetArn": str,
-        "InboundPermissions": List[IpPermissionTypeDef],
-        "UpdateStatus": Literal["PENDING_UPDATE"],
-        "Location": str,
+        "Build": BuildTypeDef,
+        "UploadCredentials": AwsCredentialsTypeDef,
+        "StorageLocation": S3LocationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RequestUploadCredentialsOutputTypeDef = TypedDict(
+    "RequestUploadCredentialsOutputTypeDef",
+    {
+        "UploadCredentials": AwsCredentialsTypeDef,
+        "StorageLocation": S3LocationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ScriptTypeDef = TypedDict(
+    "ScriptTypeDef",
+    {
+        "ScriptId": str,
+        "ScriptArn": str,
+        "Name": str,
+        "Version": str,
+        "SizeOnDisk": int,
+        "CreationTime": datetime,
+        "StorageLocation": S3LocationOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateFleetPortSettingsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetPortSettingsInputRequestTypeDef",
     {
         "FleetId": str,
     },
 )
 _OptionalUpdateFleetPortSettingsInputRequestTypeDef = TypedDict(
@@ -2490,46 +2671,14 @@
     "CreateFleetLocationsInputRequestTypeDef",
     {
         "FleetId": str,
         "Locations": Sequence[LocationConfigurationTypeDef],
     },
 )
 
-FleetAttributesTypeDef = TypedDict(
-    "FleetAttributesTypeDef",
-    {
-        "FleetId": str,
-        "FleetArn": str,
-        "FleetType": FleetTypeType,
-        "InstanceType": EC2InstanceTypeType,
-        "Description": str,
-        "Name": str,
-        "CreationTime": datetime,
-        "TerminationTime": datetime,
-        "Status": FleetStatusType,
-        "BuildId": str,
-        "BuildArn": str,
-        "ScriptId": str,
-        "ScriptArn": str,
-        "ServerLaunchPath": str,
-        "ServerLaunchParameters": str,
-        "LogPaths": List[str],
-        "NewGameSessionProtectionPolicy": ProtectionPolicyType,
-        "OperatingSystem": OperatingSystemType,
-        "ResourceCreationLimitPolicy": ResourceCreationLimitPolicyTypeDef,
-        "MetricGroups": List[str],
-        "StoppedActions": List[Literal["AUTO_SCALING"]],
-        "InstanceRoleArn": str,
-        "CertificateConfiguration": CertificateConfigurationTypeDef,
-        "ComputeType": ComputeTypeType,
-        "AnywhereConfiguration": AnywhereConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateFleetAttributesInputRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetAttributesInputRequestTypeDef",
     {
         "FleetId": str,
     },
 )
 _OptionalUpdateFleetAttributesInputRequestTypeDef = TypedDict(
@@ -2577,33 +2726,14 @@
         "LocationState": LocationStateTypeDef,
         "StoppedActions": List[Literal["AUTO_SCALING"]],
         "UpdateStatus": Literal["PENDING_UPDATE"],
     },
     total=False,
 )
 
-GameServerGroupTypeDef = TypedDict(
-    "GameServerGroupTypeDef",
-    {
-        "GameServerGroupName": str,
-        "GameServerGroupArn": str,
-        "RoleArn": str,
-        "InstanceDefinitions": List[InstanceDefinitionTypeDef],
-        "BalancingStrategy": BalancingStrategyType,
-        "GameServerProtectionPolicy": GameServerProtectionPolicyType,
-        "AutoScalingGroupArn": str,
-        "Status": GameServerGroupStatusType,
-        "StatusReason": str,
-        "SuspendedActions": List[Literal["REPLACE_INSTANCE_TYPES"]],
-        "CreationTime": datetime,
-        "LastUpdatedTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateGameServerGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGameServerGroupInputRequestTypeDef",
     {
         "GameServerGroupName": str,
     },
 )
 _OptionalUpdateGameServerGroupInputRequestTypeDef = TypedDict(
@@ -2679,64 +2809,14 @@
 
 class CreateMatchmakingConfigurationInputRequestTypeDef(
     _RequiredCreateMatchmakingConfigurationInputRequestTypeDef,
     _OptionalCreateMatchmakingConfigurationInputRequestTypeDef,
 ):
     pass
 
-GameSessionTypeDef = TypedDict(
-    "GameSessionTypeDef",
-    {
-        "GameSessionId": str,
-        "Name": str,
-        "FleetId": str,
-        "FleetArn": str,
-        "CreationTime": datetime,
-        "TerminationTime": datetime,
-        "CurrentPlayerSessionCount": int,
-        "MaximumPlayerSessionCount": int,
-        "Status": GameSessionStatusType,
-        "StatusReason": Literal["INTERRUPTED"],
-        "GameProperties": List[GamePropertyTypeDef],
-        "IpAddress": str,
-        "DnsName": str,
-        "Port": int,
-        "PlayerSessionCreationPolicy": PlayerSessionCreationPolicyType,
-        "CreatorId": str,
-        "GameSessionData": str,
-        "MatchmakerData": str,
-        "Location": str,
-    },
-    total=False,
-)
-
-MatchmakingConfigurationTypeDef = TypedDict(
-    "MatchmakingConfigurationTypeDef",
-    {
-        "Name": str,
-        "ConfigurationArn": str,
-        "Description": str,
-        "GameSessionQueueArns": List[str],
-        "RequestTimeoutSeconds": int,
-        "AcceptanceTimeoutSeconds": int,
-        "AcceptanceRequired": bool,
-        "RuleSetName": str,
-        "RuleSetArn": str,
-        "NotificationTarget": str,
-        "AdditionalPlayerCount": int,
-        "CustomEventData": str,
-        "CreationTime": datetime,
-        "GameProperties": List[GamePropertyTypeDef],
-        "GameSessionData": str,
-        "BackfillMode": BackfillModeType,
-        "FlexMatchMode": FlexMatchModeType,
-    },
-    total=False,
-)
-
 _RequiredUpdateMatchmakingConfigurationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMatchmakingConfigurationInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateMatchmakingConfigurationInputRequestTypeDef = TypedDict(
@@ -2788,30 +2868,14 @@
 
 class CreateGameSessionQueueInputRequestTypeDef(
     _RequiredCreateGameSessionQueueInputRequestTypeDef,
     _OptionalCreateGameSessionQueueInputRequestTypeDef,
 ):
     pass
 
-GameSessionQueueTypeDef = TypedDict(
-    "GameSessionQueueTypeDef",
-    {
-        "Name": str,
-        "GameSessionQueueArn": str,
-        "TimeoutInSeconds": int,
-        "PlayerLatencyPolicies": List[PlayerLatencyPolicyTypeDef],
-        "Destinations": List[GameSessionQueueDestinationTypeDef],
-        "FilterConfiguration": FilterConfigurationTypeDef,
-        "PriorityConfiguration": PriorityConfigurationTypeDef,
-        "CustomEventData": str,
-        "NotificationTarget": str,
-    },
-    total=False,
-)
-
 _RequiredUpdateGameSessionQueueInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGameSessionQueueInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateGameSessionQueueInputRequestTypeDef = TypedDict(
@@ -2939,14 +3003,26 @@
     {
         "FleetUtilization": List[FleetUtilizationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DescribeFleetPortSettingsOutputTypeDef = TypedDict(
+    "DescribeFleetPortSettingsOutputTypeDef",
+    {
+        "FleetId": str,
+        "FleetArn": str,
+        "InboundPermissions": List[IpPermissionOutputTypeDef],
+        "UpdateStatus": Literal["PENDING_UPDATE"],
+        "Location": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeGameServerInstancesOutputTypeDef = TypedDict(
     "DescribeGameServerInstancesOutputTypeDef",
     {
         "GameServerInstances": List[GameServerInstanceTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2969,14 +3045,96 @@
         "InstanceType": EC2InstanceTypeType,
         "InstanceCounts": EC2InstanceCountsTypeDef,
         "Location": str,
     },
     total=False,
 )
 
+FleetAttributesTypeDef = TypedDict(
+    "FleetAttributesTypeDef",
+    {
+        "FleetId": str,
+        "FleetArn": str,
+        "FleetType": FleetTypeType,
+        "InstanceType": EC2InstanceTypeType,
+        "Description": str,
+        "Name": str,
+        "CreationTime": datetime,
+        "TerminationTime": datetime,
+        "Status": FleetStatusType,
+        "BuildId": str,
+        "BuildArn": str,
+        "ScriptId": str,
+        "ScriptArn": str,
+        "ServerLaunchPath": str,
+        "ServerLaunchParameters": str,
+        "LogPaths": List[str],
+        "NewGameSessionProtectionPolicy": ProtectionPolicyType,
+        "OperatingSystem": OperatingSystemType,
+        "ResourceCreationLimitPolicy": ResourceCreationLimitPolicyOutputTypeDef,
+        "MetricGroups": List[str],
+        "StoppedActions": List[Literal["AUTO_SCALING"]],
+        "InstanceRoleArn": str,
+        "CertificateConfiguration": CertificateConfigurationOutputTypeDef,
+        "ComputeType": ComputeTypeType,
+        "AnywhereConfiguration": AnywhereConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+GameSessionTypeDef = TypedDict(
+    "GameSessionTypeDef",
+    {
+        "GameSessionId": str,
+        "Name": str,
+        "FleetId": str,
+        "FleetArn": str,
+        "CreationTime": datetime,
+        "TerminationTime": datetime,
+        "CurrentPlayerSessionCount": int,
+        "MaximumPlayerSessionCount": int,
+        "Status": GameSessionStatusType,
+        "StatusReason": Literal["INTERRUPTED"],
+        "GameProperties": List[GamePropertyOutputTypeDef],
+        "IpAddress": str,
+        "DnsName": str,
+        "Port": int,
+        "PlayerSessionCreationPolicy": PlayerSessionCreationPolicyType,
+        "CreatorId": str,
+        "GameSessionData": str,
+        "MatchmakerData": str,
+        "Location": str,
+    },
+    total=False,
+)
+
+MatchmakingConfigurationTypeDef = TypedDict(
+    "MatchmakingConfigurationTypeDef",
+    {
+        "Name": str,
+        "ConfigurationArn": str,
+        "Description": str,
+        "GameSessionQueueArns": List[str],
+        "RequestTimeoutSeconds": int,
+        "AcceptanceTimeoutSeconds": int,
+        "AcceptanceRequired": bool,
+        "RuleSetName": str,
+        "RuleSetArn": str,
+        "NotificationTarget": str,
+        "AdditionalPlayerCount": int,
+        "CustomEventData": str,
+        "CreationTime": datetime,
+        "GameProperties": List[GamePropertyOutputTypeDef],
+        "GameSessionData": str,
+        "BackfillMode": BackfillModeType,
+        "FlexMatchMode": FlexMatchModeType,
+    },
+    total=False,
+)
+
 _RequiredGameServerGroupAutoScalingPolicyTypeDef = TypedDict(
     "_RequiredGameServerGroupAutoScalingPolicyTypeDef",
     {
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
     },
 )
 _OptionalGameServerGroupAutoScalingPolicyTypeDef = TypedDict(
@@ -2989,14 +3147,33 @@
 
 class GameServerGroupAutoScalingPolicyTypeDef(
     _RequiredGameServerGroupAutoScalingPolicyTypeDef,
     _OptionalGameServerGroupAutoScalingPolicyTypeDef,
 ):
     pass
 
+GameServerGroupTypeDef = TypedDict(
+    "GameServerGroupTypeDef",
+    {
+        "GameServerGroupName": str,
+        "GameServerGroupArn": str,
+        "RoleArn": str,
+        "InstanceDefinitions": List[InstanceDefinitionOutputTypeDef],
+        "BalancingStrategy": BalancingStrategyType,
+        "GameServerProtectionPolicy": GameServerProtectionPolicyType,
+        "AutoScalingGroupArn": str,
+        "Status": GameServerGroupStatusType,
+        "StatusReason": str,
+        "SuspendedActions": List[Literal["REPLACE_INSTANCE_TYPES"]],
+        "CreationTime": datetime,
+        "LastUpdatedTime": datetime,
+    },
+    total=False,
+)
+
 GameSessionConnectionInfoTypeDef = TypedDict(
     "GameSessionConnectionInfoTypeDef",
     {
         "GameSessionArn": str,
         "IpAddress": str,
         "DnsName": str,
         "Port": int,
@@ -3007,33 +3184,69 @@
 
 GameSessionPlacementTypeDef = TypedDict(
     "GameSessionPlacementTypeDef",
     {
         "PlacementId": str,
         "GameSessionQueueName": str,
         "Status": GameSessionPlacementStateType,
-        "GameProperties": List[GamePropertyTypeDef],
+        "GameProperties": List[GamePropertyOutputTypeDef],
         "MaximumPlayerSessionCount": int,
         "GameSessionName": str,
         "GameSessionId": str,
         "GameSessionArn": str,
         "GameSessionRegion": str,
-        "PlayerLatencies": List[PlayerLatencyTypeDef],
+        "PlayerLatencies": List[PlayerLatencyOutputTypeDef],
         "StartTime": datetime,
         "EndTime": datetime,
         "IpAddress": str,
         "DnsName": str,
         "Port": int,
         "PlacedPlayerSessions": List[PlacedPlayerSessionTypeDef],
         "GameSessionData": str,
         "MatchmakerData": str,
     },
     total=False,
 )
 
+GameSessionQueueTypeDef = TypedDict(
+    "GameSessionQueueTypeDef",
+    {
+        "Name": str,
+        "GameSessionQueueArn": str,
+        "TimeoutInSeconds": int,
+        "PlayerLatencyPolicies": List[PlayerLatencyPolicyOutputTypeDef],
+        "Destinations": List[GameSessionQueueDestinationOutputTypeDef],
+        "FilterConfiguration": FilterConfigurationOutputTypeDef,
+        "PriorityConfiguration": PriorityConfigurationOutputTypeDef,
+        "CustomEventData": str,
+        "NotificationTarget": str,
+    },
+    total=False,
+)
+
+InstanceAccessTypeDef = TypedDict(
+    "InstanceAccessTypeDef",
+    {
+        "FleetId": str,
+        "InstanceId": str,
+        "IpAddress": str,
+        "OperatingSystem": OperatingSystemType,
+        "Credentials": InstanceCredentialsTypeDef,
+    },
+    total=False,
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredStartGameSessionPlacementInputRequestTypeDef = TypedDict(
     "_RequiredStartGameSessionPlacementInputRequestTypeDef",
     {
         "PlacementId": str,
         "GameSessionQueueName": str,
         "MaximumPlayerSessionCount": int,
     },
@@ -3052,26 +3265,14 @@
 
 class StartGameSessionPlacementInputRequestTypeDef(
     _RequiredStartGameSessionPlacementInputRequestTypeDef,
     _OptionalStartGameSessionPlacementInputRequestTypeDef,
 ):
     pass
 
-InstanceAccessTypeDef = TypedDict(
-    "InstanceAccessTypeDef",
-    {
-        "FleetId": str,
-        "InstanceId": str,
-        "IpAddress": str,
-        "OperatingSystem": OperatingSystemType,
-        "Credentials": InstanceCredentialsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredPutScalingPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutScalingPolicyInputRequestTypeDef",
     {
         "Name": str,
         "FleetId": str,
         "MetricName": MetricNameType,
     },
@@ -3091,45 +3292,55 @@
 )
 
 class PutScalingPolicyInputRequestTypeDef(
     _RequiredPutScalingPolicyInputRequestTypeDef, _OptionalPutScalingPolicyInputRequestTypeDef
 ):
     pass
 
+RuntimeConfigurationOutputTypeDef = TypedDict(
+    "RuntimeConfigurationOutputTypeDef",
+    {
+        "ServerProcesses": List[ServerProcessOutputTypeDef],
+        "MaxConcurrentGameSessionActivations": int,
+        "GameSessionActivationTimeoutSeconds": int,
+    },
+    total=False,
+)
+
+RuntimeConfigurationTypeDef = TypedDict(
+    "RuntimeConfigurationTypeDef",
+    {
+        "ServerProcesses": Sequence[ServerProcessTypeDef],
+        "MaxConcurrentGameSessionActivations": int,
+        "GameSessionActivationTimeoutSeconds": int,
+    },
+    total=False,
+)
+
 ScalingPolicyTypeDef = TypedDict(
     "ScalingPolicyTypeDef",
     {
         "FleetId": str,
         "FleetArn": str,
         "Name": str,
         "Status": ScalingStatusTypeType,
         "ScalingAdjustment": int,
         "ScalingAdjustmentType": ScalingAdjustmentTypeType,
         "ComparisonOperator": ComparisonOperatorTypeType,
         "Threshold": float,
         "EvaluationPeriods": int,
         "MetricName": MetricNameType,
         "PolicyType": PolicyTypeType,
-        "TargetConfiguration": TargetConfigurationTypeDef,
+        "TargetConfiguration": TargetConfigurationOutputTypeDef,
         "UpdateStatus": Literal["PENDING_UPDATE"],
         "Location": str,
     },
     total=False,
 )
 
-RuntimeConfigurationTypeDef = TypedDict(
-    "RuntimeConfigurationTypeDef",
-    {
-        "ServerProcesses": Sequence[ServerProcessTypeDef],
-        "MaxConcurrentGameSessionActivations": int,
-        "GameSessionActivationTimeoutSeconds": int,
-    },
-    total=False,
-)
-
 VpcPeeringConnectionTypeDef = TypedDict(
     "VpcPeeringConnectionTypeDef",
     {
         "FleetId": str,
         "FleetArn": str,
         "IpV4CidrBlock": str,
         "VpcPeeringConnectionId": str,
@@ -3243,96 +3454,56 @@
     "UpdateScriptOutputTypeDef",
     {
         "Script": ScriptTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFleetOutputTypeDef = TypedDict(
-    "CreateFleetOutputTypeDef",
-    {
-        "FleetAttributes": FleetAttributesTypeDef,
-        "LocationStates": List[LocationStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeFleetAttributesOutputTypeDef = TypedDict(
-    "DescribeFleetAttributesOutputTypeDef",
-    {
-        "FleetAttributes": List[FleetAttributesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFleetLocationAttributesOutputTypeDef = TypedDict(
     "DescribeFleetLocationAttributesOutputTypeDef",
     {
         "FleetId": str,
         "FleetArn": str,
         "LocationAttributes": List[LocationAttributesTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateGameServerGroupOutputTypeDef = TypedDict(
-    "CreateGameServerGroupOutputTypeDef",
-    {
-        "GameServerGroup": GameServerGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteGameServerGroupOutputTypeDef = TypedDict(
-    "DeleteGameServerGroupOutputTypeDef",
-    {
-        "GameServerGroup": GameServerGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeGameServerGroupOutputTypeDef = TypedDict(
-    "DescribeGameServerGroupOutputTypeDef",
-    {
-        "GameServerGroup": GameServerGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListGameServerGroupsOutputTypeDef = TypedDict(
-    "ListGameServerGroupsOutputTypeDef",
+DescribeFleetCapacityOutputTypeDef = TypedDict(
+    "DescribeFleetCapacityOutputTypeDef",
     {
-        "GameServerGroups": List[GameServerGroupTypeDef],
+        "FleetCapacity": List[FleetCapacityTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResumeGameServerGroupOutputTypeDef = TypedDict(
-    "ResumeGameServerGroupOutputTypeDef",
+DescribeFleetLocationCapacityOutputTypeDef = TypedDict(
+    "DescribeFleetLocationCapacityOutputTypeDef",
     {
-        "GameServerGroup": GameServerGroupTypeDef,
+        "FleetCapacity": FleetCapacityTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SuspendGameServerGroupOutputTypeDef = TypedDict(
-    "SuspendGameServerGroupOutputTypeDef",
+CreateFleetOutputTypeDef = TypedDict(
+    "CreateFleetOutputTypeDef",
     {
-        "GameServerGroup": GameServerGroupTypeDef,
+        "FleetAttributes": FleetAttributesTypeDef,
+        "LocationStates": List[LocationStateTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateGameServerGroupOutputTypeDef = TypedDict(
-    "UpdateGameServerGroupOutputTypeDef",
+DescribeFleetAttributesOutputTypeDef = TypedDict(
+    "DescribeFleetAttributesOutputTypeDef",
     {
-        "GameServerGroup": GameServerGroupTypeDef,
+        "FleetAttributes": List[FleetAttributesTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateGameSessionOutputTypeDef = TypedDict(
     "CreateGameSessionOutputTypeDef",
     {
@@ -3397,97 +3568,112 @@
     "UpdateMatchmakingConfigurationOutputTypeDef",
     {
         "Configuration": MatchmakingConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateGameSessionQueueOutputTypeDef = TypedDict(
-    "CreateGameSessionQueueOutputTypeDef",
+_RequiredCreateGameServerGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateGameServerGroupInputRequestTypeDef",
     {
-        "GameSessionQueue": GameSessionQueueTypeDef,
+        "GameServerGroupName": str,
+        "RoleArn": str,
+        "MinSize": int,
+        "MaxSize": int,
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
+        "InstanceDefinitions": Sequence[InstanceDefinitionTypeDef],
+    },
+)
+_OptionalCreateGameServerGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateGameServerGroupInputRequestTypeDef",
+    {
+        "AutoScalingPolicy": GameServerGroupAutoScalingPolicyTypeDef,
+        "BalancingStrategy": BalancingStrategyType,
+        "GameServerProtectionPolicy": GameServerProtectionPolicyType,
+        "VpcSubnets": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateGameServerGroupInputRequestTypeDef(
+    _RequiredCreateGameServerGroupInputRequestTypeDef,
+    _OptionalCreateGameServerGroupInputRequestTypeDef,
+):
+    pass
+
+CreateGameServerGroupOutputTypeDef = TypedDict(
+    "CreateGameServerGroupOutputTypeDef",
+    {
+        "GameServerGroup": GameServerGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeGameSessionQueuesOutputTypeDef = TypedDict(
-    "DescribeGameSessionQueuesOutputTypeDef",
+DeleteGameServerGroupOutputTypeDef = TypedDict(
+    "DeleteGameServerGroupOutputTypeDef",
     {
-        "GameSessionQueues": List[GameSessionQueueTypeDef],
-        "NextToken": str,
+        "GameServerGroup": GameServerGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateGameSessionQueueOutputTypeDef = TypedDict(
-    "UpdateGameSessionQueueOutputTypeDef",
+DescribeGameServerGroupOutputTypeDef = TypedDict(
+    "DescribeGameServerGroupOutputTypeDef",
     {
-        "GameSessionQueue": GameSessionQueueTypeDef,
+        "GameServerGroup": GameServerGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetCapacityOutputTypeDef = TypedDict(
-    "DescribeFleetCapacityOutputTypeDef",
+ListGameServerGroupsOutputTypeDef = TypedDict(
+    "ListGameServerGroupsOutputTypeDef",
     {
-        "FleetCapacity": List[FleetCapacityTypeDef],
+        "GameServerGroups": List[GameServerGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeFleetLocationCapacityOutputTypeDef = TypedDict(
-    "DescribeFleetLocationCapacityOutputTypeDef",
+ResumeGameServerGroupOutputTypeDef = TypedDict(
+    "ResumeGameServerGroupOutputTypeDef",
     {
-        "FleetCapacity": FleetCapacityTypeDef,
+        "GameServerGroup": GameServerGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateGameServerGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateGameServerGroupInputRequestTypeDef",
+SuspendGameServerGroupOutputTypeDef = TypedDict(
+    "SuspendGameServerGroupOutputTypeDef",
     {
-        "GameServerGroupName": str,
-        "RoleArn": str,
-        "MinSize": int,
-        "MaxSize": int,
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "InstanceDefinitions": Sequence[InstanceDefinitionTypeDef],
+        "GameServerGroup": GameServerGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalCreateGameServerGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateGameServerGroupInputRequestTypeDef",
+
+UpdateGameServerGroupOutputTypeDef = TypedDict(
+    "UpdateGameServerGroupOutputTypeDef",
     {
-        "AutoScalingPolicy": GameServerGroupAutoScalingPolicyTypeDef,
-        "BalancingStrategy": BalancingStrategyType,
-        "GameServerProtectionPolicy": GameServerProtectionPolicyType,
-        "VpcSubnets": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
+        "GameServerGroup": GameServerGroupTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class CreateGameServerGroupInputRequestTypeDef(
-    _RequiredCreateGameServerGroupInputRequestTypeDef,
-    _OptionalCreateGameServerGroupInputRequestTypeDef,
-):
-    pass
-
 MatchmakingTicketTypeDef = TypedDict(
     "MatchmakingTicketTypeDef",
     {
         "TicketId": str,
         "ConfigurationName": str,
         "ConfigurationArn": str,
         "Status": MatchmakingConfigurationStatusType,
         "StatusReason": str,
         "StatusMessage": str,
         "StartTime": datetime,
         "EndTime": datetime,
-        "Players": List[PlayerTypeDef],
+        "Players": List[PlayerOutputTypeDef],
         "GameSessionConnectionInfo": GameSessionConnectionInfoTypeDef,
         "EstimatedWaitTime": int,
     },
     total=False,
 )
 
 DescribeGameSessionPlacementOutputTypeDef = TypedDict(
@@ -3510,27 +3696,59 @@
     "StopGameSessionPlacementOutputTypeDef",
     {
         "GameSessionPlacement": GameSessionPlacementTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateGameSessionQueueOutputTypeDef = TypedDict(
+    "CreateGameSessionQueueOutputTypeDef",
+    {
+        "GameSessionQueue": GameSessionQueueTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeGameSessionQueuesOutputTypeDef = TypedDict(
+    "DescribeGameSessionQueuesOutputTypeDef",
+    {
+        "GameSessionQueues": List[GameSessionQueueTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateGameSessionQueueOutputTypeDef = TypedDict(
+    "UpdateGameSessionQueueOutputTypeDef",
+    {
+        "GameSessionQueue": GameSessionQueueTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetInstanceAccessOutputTypeDef = TypedDict(
     "GetInstanceAccessOutputTypeDef",
     {
         "InstanceAccess": InstanceAccessTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeScalingPoliciesOutputTypeDef = TypedDict(
-    "DescribeScalingPoliciesOutputTypeDef",
+DescribeRuntimeConfigurationOutputTypeDef = TypedDict(
+    "DescribeRuntimeConfigurationOutputTypeDef",
     {
-        "ScalingPolicies": List[ScalingPolicyTypeDef],
-        "NextToken": str,
+        "RuntimeConfiguration": RuntimeConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateRuntimeConfigurationOutputTypeDef = TypedDict(
+    "UpdateRuntimeConfigurationOutputTypeDef",
+    {
+        "RuntimeConfiguration": RuntimeConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateFleetInputRequestTypeDef = TypedDict(
     "_RequiredCreateFleetInputRequestTypeDef",
     {
@@ -3566,34 +3784,27 @@
 )
 
 class CreateFleetInputRequestTypeDef(
     _RequiredCreateFleetInputRequestTypeDef, _OptionalCreateFleetInputRequestTypeDef
 ):
     pass
 
-DescribeRuntimeConfigurationOutputTypeDef = TypedDict(
-    "DescribeRuntimeConfigurationOutputTypeDef",
-    {
-        "RuntimeConfiguration": RuntimeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateRuntimeConfigurationInputRequestTypeDef = TypedDict(
     "UpdateRuntimeConfigurationInputRequestTypeDef",
     {
         "FleetId": str,
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
     },
 )
 
-UpdateRuntimeConfigurationOutputTypeDef = TypedDict(
-    "UpdateRuntimeConfigurationOutputTypeDef",
+DescribeScalingPoliciesOutputTypeDef = TypedDict(
+    "DescribeScalingPoliciesOutputTypeDef",
     {
-        "RuntimeConfiguration": RuntimeConfigurationTypeDef,
+        "ScalingPolicies": List[ScalingPolicyTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeVpcPeeringConnectionsOutputTypeDef = TypedDict(
     "DescribeVpcPeeringConnectionsOutputTypeDef",
     {
```

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift.egg-info/PKG-INFO` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamelift
-Version: 1.28.0
-Summary: Type annotations for boto3.GameLift 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.GameLift 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-gamelift"></a>
 
 # mypy-boto3-gamelift
 
 [![PyPI - mypy-boto3-gamelift](https://img.shields.io/pypi/v/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-gamelift?color=blue)](https://pypistats.org/packages/mypy-boto3-gamelift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamelift)](https://pepy.tech/project/mypy-boto3-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameLift 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[boto3.GameLift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
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
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -457,25 +457,30 @@
 
 `mypy_boto3_gamelift.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_gamelift.type_defs import (
     AcceptMatchInputRequestTypeDef,
-    RoutingStrategyTypeDef,
+    RoutingStrategyOutputTypeDef,
+    AnywhereConfigurationOutputTypeDef,
     AnywhereConfigurationTypeDef,
+    AttributeValueOutputTypeDef,
     AttributeValueTypeDef,
     AwsCredentialsTypeDef,
     BuildTypeDef,
+    CertificateConfigurationOutputTypeDef,
     CertificateConfigurationTypeDef,
     ClaimFilterOptionTypeDef,
     GameServerTypeDef,
     ComputeTypeDef,
+    RoutingStrategyTypeDef,
     TagTypeDef,
     S3LocationTypeDef,
+    S3LocationOutputTypeDef,
     IpPermissionTypeDef,
     LocationConfigurationTypeDef,
     ResourceCreationLimitPolicyTypeDef,
     LocationStateTypeDef,
     InstanceDefinitionTypeDef,
     LaunchTemplateSpecificationTypeDef,
     GamePropertyTypeDef,
@@ -519,14 +524,15 @@
     DescribeFleetEventsInputRequestTypeDef,
     EventTypeDef,
     DescribeFleetLocationAttributesInputRequestTypeDef,
     DescribeFleetLocationCapacityInputRequestTypeDef,
     DescribeFleetLocationUtilizationInputRequestTypeDef,
     FleetUtilizationTypeDef,
     DescribeFleetPortSettingsInputRequestTypeDef,
+    IpPermissionOutputTypeDef,
     DescribeFleetUtilizationInputDescribeFleetUtilizationPaginateTypeDef,
     DescribeFleetUtilizationInputRequestTypeDef,
     DescribeGameServerGroupInputRequestTypeDef,
     DescribeGameServerInputRequestTypeDef,
     DescribeGameServerInstancesInputDescribeGameServerInstancesPaginateTypeDef,
     DescribeGameServerInstancesInputRequestTypeDef,
     GameServerInstanceTypeDef,
@@ -551,18 +557,25 @@
     DescribeScalingPoliciesInputDescribeScalingPoliciesPaginateTypeDef,
     DescribeScalingPoliciesInputRequestTypeDef,
     DescribeScriptInputRequestTypeDef,
     DescribeVpcPeeringConnectionsInputRequestTypeDef,
     DesiredPlayerSessionTypeDef,
     EC2InstanceCountsTypeDef,
     EmptyResponseMetadataTypeDef,
+    FilterConfigurationOutputTypeDef,
+    ResourceCreationLimitPolicyOutputTypeDef,
+    GamePropertyOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
+    InstanceDefinitionOutputTypeDef,
     MatchedPlayerSessionTypeDef,
     PlacedPlayerSessionTypeDef,
-    PlayerLatencyTypeDef,
+    PlayerLatencyOutputTypeDef,
+    GameSessionQueueDestinationOutputTypeDef,
+    PlayerLatencyPolicyOutputTypeDef,
+    PriorityConfigurationOutputTypeDef,
     GetComputeAccessInputRequestTypeDef,
     GetComputeAuthTokenInputRequestTypeDef,
     GetComputeAuthTokenOutputTypeDef,
     GetGameSessionLogUrlInputRequestTypeDef,
     GetGameSessionLogUrlOutputTypeDef,
     GetInstanceAccessInputRequestTypeDef,
     InstanceCredentialsTypeDef,
@@ -580,25 +593,29 @@
     ListGameServersInputListGameServersPaginateTypeDef,
     ListGameServersInputRequestTypeDef,
     ListLocationsInputListLocationsPaginateTypeDef,
     ListLocationsInputRequestTypeDef,
     ListScriptsInputListScriptsPaginateTypeDef,
     ListScriptsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
+    PlayerLatencyTypeDef,
     TargetConfigurationTypeDef,
     PutScalingPolicyOutputTypeDef,
     RegisterComputeInputRequestTypeDef,
     RegisterGameServerInputRequestTypeDef,
     RequestUploadCredentialsInputRequestTypeDef,
     ResolveAliasInputRequestTypeDef,
     ResolveAliasOutputTypeDef,
     ResponseMetadataTypeDef,
     ResumeGameServerGroupInputRequestTypeDef,
+    ServerProcessOutputTypeDef,
     ServerProcessTypeDef,
+    TargetConfigurationOutputTypeDef,
     SearchGameSessionsInputRequestTypeDef,
     SearchGameSessionsInputSearchGameSessionsPaginateTypeDef,
     StartFleetActionsInputRequestTypeDef,
     StartFleetActionsOutputTypeDef,
     StopFleetActionsInputRequestTypeDef,
     StopFleetActionsOutputTypeDef,
     StopGameSessionPlacementInputRequestTypeDef,
@@ -612,127 +629,129 @@
     UpdateFleetPortSettingsOutputTypeDef,
     UpdateGameServerInputRequestTypeDef,
     UpdateGameSessionInputRequestTypeDef,
     ValidateMatchmakingRuleSetInputRequestTypeDef,
     ValidateMatchmakingRuleSetOutputTypeDef,
     VpcPeeringConnectionStatusTypeDef,
     AliasTypeDef,
-    UpdateAliasInputRequestTypeDef,
+    PlayerOutputTypeDef,
     PlayerTypeDef,
     GetComputeAccessOutputTypeDef,
     DescribeBuildOutputTypeDef,
     ListBuildsOutputTypeDef,
     UpdateBuildOutputTypeDef,
     ClaimGameServerInputRequestTypeDef,
     ClaimGameServerOutputTypeDef,
     DescribeGameServerOutputTypeDef,
     ListGameServersOutputTypeDef,
     RegisterGameServerOutputTypeDef,
     UpdateGameServerOutputTypeDef,
     DescribeComputeOutputTypeDef,
     ListComputeOutputTypeDef,
     RegisterComputeOutputTypeDef,
+    UpdateAliasInputRequestTypeDef,
     CreateAliasInputRequestTypeDef,
     CreateLocationInputRequestTypeDef,
     CreateMatchmakingRuleSetInputRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateBuildInputRequestTypeDef,
-    CreateBuildOutputTypeDef,
     CreateScriptInputRequestTypeDef,
+    UpdateScriptInputRequestTypeDef,
+    CreateBuildOutputTypeDef,
     RequestUploadCredentialsOutputTypeDef,
     ScriptTypeDef,
-    UpdateScriptInputRequestTypeDef,
-    DescribeFleetPortSettingsOutputTypeDef,
     UpdateFleetPortSettingsInputRequestTypeDef,
     CreateFleetLocationsInputRequestTypeDef,
-    FleetAttributesTypeDef,
     UpdateFleetAttributesInputRequestTypeDef,
     CreateFleetLocationsOutputTypeDef,
     DeleteFleetLocationsOutputTypeDef,
     LocationAttributesTypeDef,
-    GameServerGroupTypeDef,
     UpdateGameServerGroupInputRequestTypeDef,
     CreateGameSessionInputRequestTypeDef,
     CreateMatchmakingConfigurationInputRequestTypeDef,
-    GameSessionTypeDef,
-    MatchmakingConfigurationTypeDef,
     UpdateMatchmakingConfigurationInputRequestTypeDef,
     CreateGameSessionQueueInputRequestTypeDef,
-    GameSessionQueueTypeDef,
     UpdateGameSessionQueueInputRequestTypeDef,
     CreateLocationOutputTypeDef,
     ListLocationsOutputTypeDef,
     CreateMatchmakingRuleSetOutputTypeDef,
     DescribeMatchmakingRuleSetsOutputTypeDef,
     CreatePlayerSessionOutputTypeDef,
     CreatePlayerSessionsOutputTypeDef,
     DescribePlayerSessionsOutputTypeDef,
     CreateVpcPeeringAuthorizationOutputTypeDef,
     DescribeVpcPeeringAuthorizationsOutputTypeDef,
     DescribeEC2InstanceLimitsOutputTypeDef,
     DescribeFleetEventsOutputTypeDef,
     DescribeFleetLocationUtilizationOutputTypeDef,
     DescribeFleetUtilizationOutputTypeDef,
+    DescribeFleetPortSettingsOutputTypeDef,
     DescribeGameServerInstancesOutputTypeDef,
     DescribeInstancesOutputTypeDef,
     FleetCapacityTypeDef,
+    FleetAttributesTypeDef,
+    GameSessionTypeDef,
+    MatchmakingConfigurationTypeDef,
     GameServerGroupAutoScalingPolicyTypeDef,
+    GameServerGroupTypeDef,
     GameSessionConnectionInfoTypeDef,
     GameSessionPlacementTypeDef,
-    StartGameSessionPlacementInputRequestTypeDef,
+    GameSessionQueueTypeDef,
     InstanceAccessTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartGameSessionPlacementInputRequestTypeDef,
     PutScalingPolicyInputRequestTypeDef,
-    ScalingPolicyTypeDef,
+    RuntimeConfigurationOutputTypeDef,
     RuntimeConfigurationTypeDef,
+    ScalingPolicyTypeDef,
     VpcPeeringConnectionTypeDef,
     CreateAliasOutputTypeDef,
     DescribeAliasOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
     StartMatchBackfillInputRequestTypeDef,
     StartMatchmakingInputRequestTypeDef,
     CreateScriptOutputTypeDef,
     DescribeScriptOutputTypeDef,
     ListScriptsOutputTypeDef,
     UpdateScriptOutputTypeDef,
+    DescribeFleetLocationAttributesOutputTypeDef,
+    DescribeFleetCapacityOutputTypeDef,
+    DescribeFleetLocationCapacityOutputTypeDef,
     CreateFleetOutputTypeDef,
     DescribeFleetAttributesOutputTypeDef,
-    DescribeFleetLocationAttributesOutputTypeDef,
-    CreateGameServerGroupOutputTypeDef,
-    DeleteGameServerGroupOutputTypeDef,
-    DescribeGameServerGroupOutputTypeDef,
-    ListGameServerGroupsOutputTypeDef,
-    ResumeGameServerGroupOutputTypeDef,
-    SuspendGameServerGroupOutputTypeDef,
-    UpdateGameServerGroupOutputTypeDef,
     CreateGameSessionOutputTypeDef,
     DescribeGameSessionsOutputTypeDef,
     GameSessionDetailTypeDef,
     SearchGameSessionsOutputTypeDef,
     UpdateGameSessionOutputTypeDef,
     CreateMatchmakingConfigurationOutputTypeDef,
     DescribeMatchmakingConfigurationsOutputTypeDef,
     UpdateMatchmakingConfigurationOutputTypeDef,
-    CreateGameSessionQueueOutputTypeDef,
-    DescribeGameSessionQueuesOutputTypeDef,
-    UpdateGameSessionQueueOutputTypeDef,
-    DescribeFleetCapacityOutputTypeDef,
-    DescribeFleetLocationCapacityOutputTypeDef,
     CreateGameServerGroupInputRequestTypeDef,
+    CreateGameServerGroupOutputTypeDef,
+    DeleteGameServerGroupOutputTypeDef,
+    DescribeGameServerGroupOutputTypeDef,
+    ListGameServerGroupsOutputTypeDef,
+    ResumeGameServerGroupOutputTypeDef,
+    SuspendGameServerGroupOutputTypeDef,
+    UpdateGameServerGroupOutputTypeDef,
     MatchmakingTicketTypeDef,
     DescribeGameSessionPlacementOutputTypeDef,
     StartGameSessionPlacementOutputTypeDef,
     StopGameSessionPlacementOutputTypeDef,
+    CreateGameSessionQueueOutputTypeDef,
+    DescribeGameSessionQueuesOutputTypeDef,
+    UpdateGameSessionQueueOutputTypeDef,
     GetInstanceAccessOutputTypeDef,
-    DescribeScalingPoliciesOutputTypeDef,
-    CreateFleetInputRequestTypeDef,
     DescribeRuntimeConfigurationOutputTypeDef,
-    UpdateRuntimeConfigurationInputRequestTypeDef,
     UpdateRuntimeConfigurationOutputTypeDef,
+    CreateFleetInputRequestTypeDef,
+    UpdateRuntimeConfigurationInputRequestTypeDef,
+    DescribeScalingPoliciesOutputTypeDef,
     DescribeVpcPeeringConnectionsOutputTypeDef,
     DescribeGameSessionDetailsOutputTypeDef,
     DescribeMatchmakingOutputTypeDef,
     StartMatchBackfillOutputTypeDef,
     StartMatchmakingOutputTypeDef,
 )
```

### Comparing `mypy-boto3-gamelift-1.28.0/mypy_boto3_gamelift.egg-info/SOURCES.txt` & `mypy-boto3-gamelift-1.28.12/mypy_boto3_gamelift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.28.0/setup.py` & `mypy-boto3-gamelift-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-gamelift",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_gamelift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GameLift 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.GameLift 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

