# Comparing `tmp/mypy-boto3-elasticache-1.28.0.tar.gz` & `tmp/mypy-boto3-elasticache-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elasticache-1.28.0.tar", last modified: Thu Jul  6 20:59:30 2023, max compression
+gzip compressed data, was "mypy-boto3-elasticache-1.28.12.tar", last modified: Thu Jul 27 05:34:38 2023, max compression
```

## Comparing `mypy-boto3-elasticache-1.28.0.tar` & `mypy-boto3-elasticache-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:30.666293 mypy-boto3-elasticache-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:11.000000 mypy-boto3-elasticache-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27271 2023-07-06 20:59:30.666293 mypy-boto3-elasticache-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25770 2023-07-06 20:40:11.000000 mypy-boto3-elasticache-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:30.666293 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-06 20:40:11.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-06 20:40:11.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-06 20:40:11.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68059 2023-07-06 20:40:13.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    67966 2023-07-06 20:40:13.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-07-06 20:40:14.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14175 2023-07-06 20:40:14.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22718 2023-07-06 20:40:14.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22699 2023-07-06 20:40:14.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:11.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86384 2023-07-06 20:40:16.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86317 2023-07-06 20:40:15.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:11.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-06 20:40:14.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-06 20:40:14.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:30.666293 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27271 2023-07-06 20:59:30.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-06 20:59:30.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:30.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:30.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:30.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 20:59:30.000000 mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:30.666293 mypy-boto3-elasticache-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-06 20:40:11.000000 mypy-boto3-elasticache-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.536520 mypy-boto3-elasticache-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-07-27 05:34:38.532520 mypy-boto3-elasticache-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25958 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.532520 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68059 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67966 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22718 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22699 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    87751 2023-07-27 05:21:47.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87684 2023-07-27 05:21:45.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-27 05:21:44.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.532520 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-07-27 05:34:38.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-27 05:34:38.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:38.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:38.000000 mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:38.536520 mypy-boto3-elasticache-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:21:43.000000 mypy-boto3-elasticache-1.28.12/setup.py
```

### Comparing `mypy-boto3-elasticache-1.28.0/LICENSE` & `mypy-boto3-elasticache-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.0/PKG-INFO` & `mypy-boto3-elasticache-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.28.0
-Summary: Type annotations for boto3.ElastiCache 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ElastiCache 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-elasticache"></a>
 
 # mypy-boto3-elasticache
 
 [![PyPI - mypy-boto3-elasticache](https://img.shields.io/pypi/v/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticache?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticache)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticache)](https://pepy.tech/project/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -485,14 +485,15 @@
     CacheEngineVersionTypeDef,
     CacheNodeTypeSpecificValueTypeDef,
     CacheNodeUpdateStatusTypeDef,
     ParameterTypeDef,
     CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
+    CloudWatchLogsDestinationDetailsOutputTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
     NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
@@ -534,14 +535,15 @@
     DescribeServiceUpdatesMessageRequestTypeDef,
     DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
     TimeRangeFilterTypeDef,
     DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
+    KinesisFirehoseDestinationDetailsOutputTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
     GlobalReplicationGroupInfoTypeDef,
@@ -549,117 +551,120 @@
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
     PaginatorConfigTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
     SlotMigrationTypeDef,
     ResponseMetadataTypeDef,
     RevokeCacheSecurityGroupIngressMessageRequestTypeDef,
     ServiceUpdateTypeDef,
     SubnetOutpostTypeDef,
+    TagOutputTypeDef,
     TestFailoverMessageRequestTypeDef,
     UnprocessedUpdateActionTypeDef,
     UserGroupPendingChangesTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
-    TagListMessageTypeDef,
     CreateUserMessageRequestTypeDef,
     ModifyUserMessageRequestTypeDef,
     UserResponseMetadataTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
     CacheSecurityGroupTypeDef,
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
-    NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
     DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
     DescribeUpdateActionsMessageRequestTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
+    DestinationDetailsOutputTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
+    NodeSnapshotTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
+    TagListMessageTypeDef,
     UpdateActionResultsMessageTypeDef,
     UserGroupResponseMetadataTypeDef,
     UserGroupTypeDef,
     DescribeUsersResultTypeDef,
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
-    SnapshotTypeDef,
-    LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
+    LogDeliveryConfigurationRequestTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
+    SnapshotTypeDef,
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
-    CopySnapshotResultTypeDef,
-    CreateSnapshotResultTypeDef,
-    DeleteSnapshotResultTypeDef,
-    DescribeSnapshotsListMessageTypeDef,
+    PendingModifiedValuesTypeDef,
+    ReplicationGroupPendingModifiedValuesTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
-    PendingModifiedValuesTypeDef,
-    ReplicationGroupPendingModifiedValuesTypeDef,
+    CopySnapshotResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     CacheClusterTypeDef,
     ReplicationGroupTypeDef,
     CacheClusterMessageTypeDef,
```

### Comparing `mypy-boto3-elasticache-1.28.0/README.md` & `mypy-boto3-elasticache-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-elasticache"></a>
 
 # mypy-boto3-elasticache
 
 [![PyPI - mypy-boto3-elasticache](https://img.shields.io/pypi/v/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticache?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticache)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticache)](https://pepy.tech/project/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -453,14 +453,15 @@
     CacheEngineVersionTypeDef,
     CacheNodeTypeSpecificValueTypeDef,
     CacheNodeUpdateStatusTypeDef,
     ParameterTypeDef,
     CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
+    CloudWatchLogsDestinationDetailsOutputTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
     NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
@@ -502,14 +503,15 @@
     DescribeServiceUpdatesMessageRequestTypeDef,
     DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
     TimeRangeFilterTypeDef,
     DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
+    KinesisFirehoseDestinationDetailsOutputTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
     GlobalReplicationGroupInfoTypeDef,
@@ -517,117 +519,120 @@
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
     PaginatorConfigTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
     SlotMigrationTypeDef,
     ResponseMetadataTypeDef,
     RevokeCacheSecurityGroupIngressMessageRequestTypeDef,
     ServiceUpdateTypeDef,
     SubnetOutpostTypeDef,
+    TagOutputTypeDef,
     TestFailoverMessageRequestTypeDef,
     UnprocessedUpdateActionTypeDef,
     UserGroupPendingChangesTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
-    TagListMessageTypeDef,
     CreateUserMessageRequestTypeDef,
     ModifyUserMessageRequestTypeDef,
     UserResponseMetadataTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
     CacheSecurityGroupTypeDef,
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
-    NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
     DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
     DescribeUpdateActionsMessageRequestTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
+    DestinationDetailsOutputTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
+    NodeSnapshotTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
+    TagListMessageTypeDef,
     UpdateActionResultsMessageTypeDef,
     UserGroupResponseMetadataTypeDef,
     UserGroupTypeDef,
     DescribeUsersResultTypeDef,
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
-    SnapshotTypeDef,
-    LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
+    LogDeliveryConfigurationRequestTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
+    SnapshotTypeDef,
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
-    CopySnapshotResultTypeDef,
-    CreateSnapshotResultTypeDef,
-    DeleteSnapshotResultTypeDef,
-    DescribeSnapshotsListMessageTypeDef,
+    PendingModifiedValuesTypeDef,
+    ReplicationGroupPendingModifiedValuesTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
-    PendingModifiedValuesTypeDef,
-    ReplicationGroupPendingModifiedValuesTypeDef,
+    CopySnapshotResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     CacheClusterTypeDef,
     ReplicationGroupTypeDef,
     CacheClusterMessageTypeDef,
```

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/__init__.py` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/__init__.pyi` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/__main__.py` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElastiCache 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ElastiCache 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache\nOther"
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

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/client.py` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/client.pyi` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/literals.py` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,14 +265,15 @@
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
@@ -351,26 +352,28 @@
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

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/literals.pyi` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -263,14 +263,15 @@
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
@@ -349,26 +350,28 @@
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

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/paginator.py` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/paginator.pyi` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/type_defs.py` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     "CacheEngineVersionTypeDef",
     "CacheNodeTypeSpecificValueTypeDef",
     "CacheNodeUpdateStatusTypeDef",
     "ParameterTypeDef",
     "CacheParameterGroupNameMessageTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
+    "CloudWatchLogsDestinationDetailsOutputTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
     "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
@@ -120,14 +121,15 @@
     "DescribeServiceUpdatesMessageRequestTypeDef",
     "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsMessageRequestTypeDef",
     "TimeRangeFilterTypeDef",
     "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
     "DescribeUserGroupsMessageRequestTypeDef",
     "FilterTypeDef",
+    "KinesisFirehoseDestinationDetailsOutputTypeDef",
     "KinesisFirehoseDestinationDetailsTypeDef",
     "DisassociateGlobalReplicationGroupMessageRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EventTypeDef",
     "FailoverGlobalReplicationGroupMessageRequestTypeDef",
     "GlobalNodeGroupTypeDef",
     "GlobalReplicationGroupInfoTypeDef",
@@ -135,117 +137,120 @@
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
+    "NodeGroupConfigurationOutputTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
     "PaginatorConfigTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
     "SlotMigrationTypeDef",
     "ResponseMetadataTypeDef",
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     "ServiceUpdateTypeDef",
     "SubnetOutpostTypeDef",
+    "TagOutputTypeDef",
     "TestFailoverMessageRequestTypeDef",
     "UnprocessedUpdateActionTypeDef",
     "UserGroupPendingChangesTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopySnapshotMessageRequestTypeDef",
     "CreateCacheParameterGroupMessageRequestTypeDef",
     "CreateCacheSecurityGroupMessageRequestTypeDef",
     "CreateCacheSubnetGroupMessageRequestTypeDef",
     "CreateSnapshotMessageRequestTypeDef",
     "CreateUserGroupMessageRequestTypeDef",
     "PurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
-    "TagListMessageTypeDef",
     "CreateUserMessageRequestTypeDef",
     "ModifyUserMessageRequestTypeDef",
     "UserResponseMetadataTypeDef",
     "UserTypeDef",
     "CacheNodeTypeDef",
     "NodeGroupMemberTypeDef",
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
     "CacheSecurityGroupTypeDef",
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
-    "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     "DescribeUpdateActionsMessageRequestTypeDef",
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     "DescribeUsersMessageRequestTypeDef",
+    "DestinationDetailsOutputTypeDef",
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
+    "NodeSnapshotTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
+    "TagListMessageTypeDef",
     "UpdateActionResultsMessageTypeDef",
     "UserGroupResponseMetadataTypeDef",
     "UserGroupTypeDef",
     "DescribeUsersResultTypeDef",
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
-    "SnapshotTypeDef",
-    "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
+    "LogDeliveryConfigurationRequestTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "DeleteGlobalReplicationGroupResultTypeDef",
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "ModifyGlobalReplicationGroupResultTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
+    "SnapshotTypeDef",
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
-    "CopySnapshotResultTypeDef",
-    "CreateSnapshotResultTypeDef",
-    "DeleteSnapshotResultTypeDef",
-    "DescribeSnapshotsListMessageTypeDef",
+    "PendingModifiedValuesTypeDef",
+    "ReplicationGroupPendingModifiedValuesTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
-    "PendingModifiedValuesTypeDef",
-    "ReplicationGroupPendingModifiedValuesTypeDef",
+    "CopySnapshotResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
     "ModifyCacheSubnetGroupResultTypeDef",
     "CacheClusterTypeDef",
     "ReplicationGroupTypeDef",
     "CacheClusterMessageTypeDef",
@@ -488,14 +493,22 @@
         "Status": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+CloudWatchLogsDestinationDetailsOutputTypeDef = TypedDict(
+    "CloudWatchLogsDestinationDetailsOutputTypeDef",
+    {
+        "LogGroup": str,
+    },
+    total=False,
+)
+
 CloudWatchLogsDestinationDetailsTypeDef = TypedDict(
     "CloudWatchLogsDestinationDetailsTypeDef",
     {
         "LogGroup": str,
     },
     total=False,
 )
@@ -568,17 +581,17 @@
 NodeGroupConfigurationTypeDef = TypedDict(
     "NodeGroupConfigurationTypeDef",
     {
         "NodeGroupId": str,
         "Slots": str,
         "ReplicaCount": int,
         "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": List[str],
+        "ReplicaAvailabilityZones": Sequence[str],
         "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": List[str],
+        "ReplicaOutpostArns": Sequence[str],
     },
     total=False,
 )
 
 CustomerNodeEndpointTypeDef = TypedDict(
     "CustomerNodeEndpointTypeDef",
     {
@@ -1117,14 +1130,22 @@
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
+KinesisFirehoseDestinationDetailsOutputTypeDef = TypedDict(
+    "KinesisFirehoseDestinationDetailsOutputTypeDef",
+    {
+        "DeliveryStream": str,
+    },
+    total=False,
+)
+
 KinesisFirehoseDestinationDetailsTypeDef = TypedDict(
     "KinesisFirehoseDestinationDetailsTypeDef",
     {
         "DeliveryStream": str,
     },
     total=False,
 )
@@ -1297,14 +1318,28 @@
 
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
 
+NodeGroupConfigurationOutputTypeDef = TypedDict(
+    "NodeGroupConfigurationOutputTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": List[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": List[str],
+    },
+    total=False,
+)
+
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1431,14 +1466,23 @@
     "SubnetOutpostTypeDef",
     {
         "SubnetOutpostArn": str,
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 TestFailoverMessageRequestTypeDef = TypedDict(
     "TestFailoverMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "NodeGroupId": str,
     },
 )
@@ -1634,22 +1678,14 @@
 class PurchaseReservedCacheNodesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
 ):
     pass
 
 
-TagListMessageTypeDef = TypedDict(
-    "TagListMessageTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserMessageRequestTypeDef = TypedDict(
     "_RequiredCreateUserMessageRequestTypeDef",
     {
         "UserId": str,
         "UserName": str,
         "Engine": str,
         "AccessString": str,
@@ -1857,28 +1893,14 @@
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
 
-NodeSnapshotTypeDef = TypedDict(
-    "NodeSnapshotTypeDef",
-    {
-        "CacheClusterId": str,
-        "NodeGroupId": str,
-        "CacheNodeId": str,
-        "NodeGroupConfiguration": NodeGroupConfigurationTypeDef,
-        "CacheSize": str,
-        "CacheNodeCreateTime": datetime,
-        "SnapshotCreateTime": datetime,
-    },
-    total=False,
-)
-
 StartMigrationMessageRequestTypeDef = TypedDict(
     "StartMigrationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
     },
 )
@@ -1983,14 +2005,23 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DestinationDetailsOutputTypeDef = TypedDict(
+    "DestinationDetailsOutputTypeDef",
+    {
+        "CloudWatchLogsDetails": CloudWatchLogsDestinationDetailsOutputTypeDef,
+        "KinesisFirehoseDetails": KinesisFirehoseDestinationDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationDetailsTypeDef = TypedDict(
     "DestinationDetailsTypeDef",
     {
         "CloudWatchLogsDetails": CloudWatchLogsDestinationDetailsTypeDef,
         "KinesisFirehoseDetails": KinesisFirehoseDestinationDetailsTypeDef,
     },
     total=False,
@@ -2087,14 +2118,28 @@
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
 )
 
+NodeSnapshotTypeDef = TypedDict(
+    "NodeSnapshotTypeDef",
+    {
+        "CacheClusterId": str,
+        "NodeGroupId": str,
+        "CacheNodeId": str,
+        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
+        "CacheSize": str,
+        "CacheNodeCreateTime": datetime,
+        "SnapshotCreateTime": datetime,
+    },
+    total=False,
+)
+
 NodeGroupUpdateStatusTypeDef = TypedDict(
     "NodeGroupUpdateStatusTypeDef",
     {
         "NodeGroupId": str,
         "NodeGroupMemberUpdateStatus": List[NodeGroupMemberUpdateStatusTypeDef],
     },
     total=False,
@@ -2159,14 +2204,22 @@
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetOutpost": SubnetOutpostTypeDef,
         "SupportedNetworkTypes": List[NetworkTypeType],
     },
     total=False,
 )
 
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateActionResultsMessageTypeDef = TypedDict(
     "UpdateActionResultsMessageTypeDef",
     {
         "ProcessedUpdateActions": List[ProcessedUpdateActionTypeDef],
         "UnprocessedUpdateActions": List[UnprocessedUpdateActionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2274,81 +2327,46 @@
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
-    {
-        "SnapshotName": str,
-        "ReplicationGroupId": str,
-        "ReplicationGroupDescription": str,
-        "CacheClusterId": str,
-        "SnapshotStatus": str,
-        "SnapshotSource": str,
-        "CacheNodeType": str,
-        "Engine": str,
-        "EngineVersion": str,
-        "NumCacheNodes": int,
-        "PreferredAvailabilityZone": str,
-        "PreferredOutpostArn": str,
-        "CacheClusterCreateTime": datetime,
-        "PreferredMaintenanceWindow": str,
-        "TopicArn": str,
-        "Port": int,
-        "CacheParameterGroupName": str,
-        "CacheSubnetGroupName": str,
-        "VpcId": str,
-        "AutoMinorVersionUpgrade": bool,
-        "SnapshotRetentionLimit": int,
-        "SnapshotWindow": str,
-        "NumNodeGroups": int,
-        "AutomaticFailover": AutomaticFailoverStatusType,
-        "NodeSnapshots": List[NodeSnapshotTypeDef],
-        "KmsKeyId": str,
-        "ARN": str,
-        "DataTiering": DataTieringStatusType,
-    },
-    total=False,
-)
-
-LogDeliveryConfigurationRequestTypeDef = TypedDict(
-    "LogDeliveryConfigurationRequestTypeDef",
+LogDeliveryConfigurationTypeDef = TypedDict(
+    "LogDeliveryConfigurationTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
-        "DestinationDetails": DestinationDetailsTypeDef,
+        "DestinationDetails": DestinationDetailsOutputTypeDef,
         "LogFormat": LogFormatType,
-        "Enabled": bool,
+        "Status": LogDeliveryConfigurationStatusType,
+        "Message": str,
     },
     total=False,
 )
 
-LogDeliveryConfigurationTypeDef = TypedDict(
-    "LogDeliveryConfigurationTypeDef",
+PendingLogDeliveryConfigurationTypeDef = TypedDict(
+    "PendingLogDeliveryConfigurationTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
-        "DestinationDetails": DestinationDetailsTypeDef,
+        "DestinationDetails": DestinationDetailsOutputTypeDef,
         "LogFormat": LogFormatType,
-        "Status": LogDeliveryConfigurationStatusType,
-        "Message": str,
     },
     total=False,
 )
 
-PendingLogDeliveryConfigurationTypeDef = TypedDict(
-    "PendingLogDeliveryConfigurationTypeDef",
+LogDeliveryConfigurationRequestTypeDef = TypedDict(
+    "LogDeliveryConfigurationRequestTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
         "DestinationDetails": DestinationDetailsTypeDef,
         "LogFormat": LogFormatType,
+        "Enabled": bool,
     },
     total=False,
 )
 
 CreateGlobalReplicationGroupResultTypeDef = TypedDict(
     "CreateGlobalReplicationGroupResultTypeDef",
     {
@@ -2442,14 +2460,49 @@
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotName": str,
+        "ReplicationGroupId": str,
+        "ReplicationGroupDescription": str,
+        "CacheClusterId": str,
+        "SnapshotStatus": str,
+        "SnapshotSource": str,
+        "CacheNodeType": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "NumCacheNodes": int,
+        "PreferredAvailabilityZone": str,
+        "PreferredOutpostArn": str,
+        "CacheClusterCreateTime": datetime,
+        "PreferredMaintenanceWindow": str,
+        "TopicArn": str,
+        "Port": int,
+        "CacheParameterGroupName": str,
+        "CacheSubnetGroupName": str,
+        "VpcId": str,
+        "AutoMinorVersionUpgrade": bool,
+        "SnapshotRetentionLimit": int,
+        "SnapshotWindow": str,
+        "NumNodeGroups": int,
+        "AutomaticFailover": AutomaticFailoverStatusType,
+        "NodeSnapshots": List[NodeSnapshotTypeDef],
+        "KmsKeyId": str,
+        "ARN": str,
+        "DataTiering": DataTieringStatusType,
+    },
+    total=False,
+)
+
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2522,45 +2575,43 @@
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CopySnapshotResultTypeDef = TypedDict(
-    "CopySnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
+PendingModifiedValuesTypeDef = TypedDict(
+    "PendingModifiedValuesTypeDef",
     {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NumCacheNodes": int,
+        "CacheNodeIdsToRemove": List[str],
+        "EngineVersion": str,
+        "CacheNodeType": str,
+        "AuthTokenStatus": AuthTokenUpdateStatusType,
+        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
     },
+    total=False,
 )
 
-DescribeSnapshotsListMessageTypeDef = TypedDict(
-    "DescribeSnapshotsListMessageTypeDef",
+ReplicationGroupPendingModifiedValuesTypeDef = TypedDict(
+    "ReplicationGroupPendingModifiedValuesTypeDef",
     {
-        "Marker": str,
-        "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PrimaryClusterId": str,
+        "AutomaticFailoverStatus": PendingAutomaticFailoverStatusType,
+        "Resharding": ReshardingStatusTypeDef,
+        "AuthTokenStatus": AuthTokenUpdateStatusType,
+        "UserGroups": UserGroupsUpdateStatusTypeDef,
+        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ClusterMode": ClusterModeType,
     },
+    total=False,
 )
 
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
@@ -2753,43 +2804,45 @@
 class ModifyReplicationGroupMessageRequestTypeDef(
     _RequiredModifyReplicationGroupMessageRequestTypeDef,
     _OptionalModifyReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
-PendingModifiedValuesTypeDef = TypedDict(
-    "PendingModifiedValuesTypeDef",
+CopySnapshotResultTypeDef = TypedDict(
+    "CopySnapshotResultTypeDef",
     {
-        "NumCacheNodes": int,
-        "CacheNodeIdsToRemove": List[str],
-        "EngineVersion": str,
-        "CacheNodeType": str,
-        "AuthTokenStatus": AuthTokenUpdateStatusType,
-        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ReplicationGroupPendingModifiedValuesTypeDef = TypedDict(
-    "ReplicationGroupPendingModifiedValuesTypeDef",
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
     {
-        "PrimaryClusterId": str,
-        "AutomaticFailoverStatus": PendingAutomaticFailoverStatusType,
-        "Resharding": ReshardingStatusTypeDef,
-        "AuthTokenStatus": AuthTokenUpdateStatusType,
-        "UserGroups": UserGroupsUpdateStatusTypeDef,
-        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
-        "ClusterMode": ClusterModeType,
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeSnapshotsListMessageTypeDef = TypedDict(
+    "DescribeSnapshotsListMessageTypeDef",
+    {
+        "Marker": str,
+        "Snapshots": List[SnapshotTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
```

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/type_defs.pyi` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     "CacheEngineVersionTypeDef",
     "CacheNodeTypeSpecificValueTypeDef",
     "CacheNodeUpdateStatusTypeDef",
     "ParameterTypeDef",
     "CacheParameterGroupNameMessageTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
+    "CloudWatchLogsDestinationDetailsOutputTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
     "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
@@ -119,14 +120,15 @@
     "DescribeServiceUpdatesMessageRequestTypeDef",
     "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsMessageRequestTypeDef",
     "TimeRangeFilterTypeDef",
     "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
     "DescribeUserGroupsMessageRequestTypeDef",
     "FilterTypeDef",
+    "KinesisFirehoseDestinationDetailsOutputTypeDef",
     "KinesisFirehoseDestinationDetailsTypeDef",
     "DisassociateGlobalReplicationGroupMessageRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EventTypeDef",
     "FailoverGlobalReplicationGroupMessageRequestTypeDef",
     "GlobalNodeGroupTypeDef",
     "GlobalReplicationGroupInfoTypeDef",
@@ -134,117 +136,120 @@
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
+    "NodeGroupConfigurationOutputTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
     "PaginatorConfigTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
     "SlotMigrationTypeDef",
     "ResponseMetadataTypeDef",
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     "ServiceUpdateTypeDef",
     "SubnetOutpostTypeDef",
+    "TagOutputTypeDef",
     "TestFailoverMessageRequestTypeDef",
     "UnprocessedUpdateActionTypeDef",
     "UserGroupPendingChangesTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopySnapshotMessageRequestTypeDef",
     "CreateCacheParameterGroupMessageRequestTypeDef",
     "CreateCacheSecurityGroupMessageRequestTypeDef",
     "CreateCacheSubnetGroupMessageRequestTypeDef",
     "CreateSnapshotMessageRequestTypeDef",
     "CreateUserGroupMessageRequestTypeDef",
     "PurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
-    "TagListMessageTypeDef",
     "CreateUserMessageRequestTypeDef",
     "ModifyUserMessageRequestTypeDef",
     "UserResponseMetadataTypeDef",
     "UserTypeDef",
     "CacheNodeTypeDef",
     "NodeGroupMemberTypeDef",
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
     "CacheSecurityGroupTypeDef",
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
-    "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
     "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     "DescribeUpdateActionsMessageRequestTypeDef",
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     "DescribeUsersMessageRequestTypeDef",
+    "DestinationDetailsOutputTypeDef",
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
+    "NodeSnapshotTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
+    "TagListMessageTypeDef",
     "UpdateActionResultsMessageTypeDef",
     "UserGroupResponseMetadataTypeDef",
     "UserGroupTypeDef",
     "DescribeUsersResultTypeDef",
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
-    "SnapshotTypeDef",
-    "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
+    "LogDeliveryConfigurationRequestTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "DeleteGlobalReplicationGroupResultTypeDef",
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "ModifyGlobalReplicationGroupResultTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
+    "SnapshotTypeDef",
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
-    "CopySnapshotResultTypeDef",
-    "CreateSnapshotResultTypeDef",
-    "DeleteSnapshotResultTypeDef",
-    "DescribeSnapshotsListMessageTypeDef",
+    "PendingModifiedValuesTypeDef",
+    "ReplicationGroupPendingModifiedValuesTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
-    "PendingModifiedValuesTypeDef",
-    "ReplicationGroupPendingModifiedValuesTypeDef",
+    "CopySnapshotResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
     "ModifyCacheSubnetGroupResultTypeDef",
     "CacheClusterTypeDef",
     "ReplicationGroupTypeDef",
     "CacheClusterMessageTypeDef",
@@ -483,14 +488,22 @@
         "Status": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+CloudWatchLogsDestinationDetailsOutputTypeDef = TypedDict(
+    "CloudWatchLogsDestinationDetailsOutputTypeDef",
+    {
+        "LogGroup": str,
+    },
+    total=False,
+)
+
 CloudWatchLogsDestinationDetailsTypeDef = TypedDict(
     "CloudWatchLogsDestinationDetailsTypeDef",
     {
         "LogGroup": str,
     },
     total=False,
 )
@@ -557,17 +570,17 @@
 NodeGroupConfigurationTypeDef = TypedDict(
     "NodeGroupConfigurationTypeDef",
     {
         "NodeGroupId": str,
         "Slots": str,
         "ReplicaCount": int,
         "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": List[str],
+        "ReplicaAvailabilityZones": Sequence[str],
         "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": List[str],
+        "ReplicaOutpostArns": Sequence[str],
     },
     total=False,
 )
 
 CustomerNodeEndpointTypeDef = TypedDict(
     "CustomerNodeEndpointTypeDef",
     {
@@ -1092,14 +1105,22 @@
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
+KinesisFirehoseDestinationDetailsOutputTypeDef = TypedDict(
+    "KinesisFirehoseDestinationDetailsOutputTypeDef",
+    {
+        "DeliveryStream": str,
+    },
+    total=False,
+)
+
 KinesisFirehoseDestinationDetailsTypeDef = TypedDict(
     "KinesisFirehoseDestinationDetailsTypeDef",
     {
         "DeliveryStream": str,
     },
     total=False,
 )
@@ -1266,14 +1287,28 @@
 )
 
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
+NodeGroupConfigurationOutputTypeDef = TypedDict(
+    "NodeGroupConfigurationOutputTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": List[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": List[str],
+    },
+    total=False,
+)
+
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1400,14 +1435,23 @@
     "SubnetOutpostTypeDef",
     {
         "SubnetOutpostArn": str,
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 TestFailoverMessageRequestTypeDef = TypedDict(
     "TestFailoverMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "NodeGroupId": str,
     },
 )
@@ -1589,22 +1633,14 @@
 
 class PurchaseReservedCacheNodesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
 ):
     pass
 
-TagListMessageTypeDef = TypedDict(
-    "TagListMessageTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserMessageRequestTypeDef = TypedDict(
     "_RequiredCreateUserMessageRequestTypeDef",
     {
         "UserId": str,
         "UserName": str,
         "Engine": str,
         "AccessString": str,
@@ -1804,28 +1840,14 @@
 
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
-NodeSnapshotTypeDef = TypedDict(
-    "NodeSnapshotTypeDef",
-    {
-        "CacheClusterId": str,
-        "NodeGroupId": str,
-        "CacheNodeId": str,
-        "NodeGroupConfiguration": NodeGroupConfigurationTypeDef,
-        "CacheSize": str,
-        "CacheNodeCreateTime": datetime,
-        "SnapshotCreateTime": datetime,
-    },
-    total=False,
-)
-
 StartMigrationMessageRequestTypeDef = TypedDict(
     "StartMigrationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
     },
 )
@@ -1930,14 +1952,23 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+DestinationDetailsOutputTypeDef = TypedDict(
+    "DestinationDetailsOutputTypeDef",
+    {
+        "CloudWatchLogsDetails": CloudWatchLogsDestinationDetailsOutputTypeDef,
+        "KinesisFirehoseDetails": KinesisFirehoseDestinationDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationDetailsTypeDef = TypedDict(
     "DestinationDetailsTypeDef",
     {
         "CloudWatchLogsDetails": CloudWatchLogsDestinationDetailsTypeDef,
         "KinesisFirehoseDetails": KinesisFirehoseDestinationDetailsTypeDef,
     },
     total=False,
@@ -2030,14 +2061,28 @@
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
 )
 
+NodeSnapshotTypeDef = TypedDict(
+    "NodeSnapshotTypeDef",
+    {
+        "CacheClusterId": str,
+        "NodeGroupId": str,
+        "CacheNodeId": str,
+        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
+        "CacheSize": str,
+        "CacheNodeCreateTime": datetime,
+        "SnapshotCreateTime": datetime,
+    },
+    total=False,
+)
+
 NodeGroupUpdateStatusTypeDef = TypedDict(
     "NodeGroupUpdateStatusTypeDef",
     {
         "NodeGroupId": str,
         "NodeGroupMemberUpdateStatus": List[NodeGroupMemberUpdateStatusTypeDef],
     },
     total=False,
@@ -2102,14 +2147,22 @@
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetOutpost": SubnetOutpostTypeDef,
         "SupportedNetworkTypes": List[NetworkTypeType],
     },
     total=False,
 )
 
+TagListMessageTypeDef = TypedDict(
+    "TagListMessageTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateActionResultsMessageTypeDef = TypedDict(
     "UpdateActionResultsMessageTypeDef",
     {
         "ProcessedUpdateActions": List[ProcessedUpdateActionTypeDef],
         "UnprocessedUpdateActions": List[UnprocessedUpdateActionTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2217,81 +2270,46 @@
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
-    {
-        "SnapshotName": str,
-        "ReplicationGroupId": str,
-        "ReplicationGroupDescription": str,
-        "CacheClusterId": str,
-        "SnapshotStatus": str,
-        "SnapshotSource": str,
-        "CacheNodeType": str,
-        "Engine": str,
-        "EngineVersion": str,
-        "NumCacheNodes": int,
-        "PreferredAvailabilityZone": str,
-        "PreferredOutpostArn": str,
-        "CacheClusterCreateTime": datetime,
-        "PreferredMaintenanceWindow": str,
-        "TopicArn": str,
-        "Port": int,
-        "CacheParameterGroupName": str,
-        "CacheSubnetGroupName": str,
-        "VpcId": str,
-        "AutoMinorVersionUpgrade": bool,
-        "SnapshotRetentionLimit": int,
-        "SnapshotWindow": str,
-        "NumNodeGroups": int,
-        "AutomaticFailover": AutomaticFailoverStatusType,
-        "NodeSnapshots": List[NodeSnapshotTypeDef],
-        "KmsKeyId": str,
-        "ARN": str,
-        "DataTiering": DataTieringStatusType,
-    },
-    total=False,
-)
-
-LogDeliveryConfigurationRequestTypeDef = TypedDict(
-    "LogDeliveryConfigurationRequestTypeDef",
+LogDeliveryConfigurationTypeDef = TypedDict(
+    "LogDeliveryConfigurationTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
-        "DestinationDetails": DestinationDetailsTypeDef,
+        "DestinationDetails": DestinationDetailsOutputTypeDef,
         "LogFormat": LogFormatType,
-        "Enabled": bool,
+        "Status": LogDeliveryConfigurationStatusType,
+        "Message": str,
     },
     total=False,
 )
 
-LogDeliveryConfigurationTypeDef = TypedDict(
-    "LogDeliveryConfigurationTypeDef",
+PendingLogDeliveryConfigurationTypeDef = TypedDict(
+    "PendingLogDeliveryConfigurationTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
-        "DestinationDetails": DestinationDetailsTypeDef,
+        "DestinationDetails": DestinationDetailsOutputTypeDef,
         "LogFormat": LogFormatType,
-        "Status": LogDeliveryConfigurationStatusType,
-        "Message": str,
     },
     total=False,
 )
 
-PendingLogDeliveryConfigurationTypeDef = TypedDict(
-    "PendingLogDeliveryConfigurationTypeDef",
+LogDeliveryConfigurationRequestTypeDef = TypedDict(
+    "LogDeliveryConfigurationRequestTypeDef",
     {
         "LogType": LogTypeType,
         "DestinationType": DestinationTypeType,
         "DestinationDetails": DestinationDetailsTypeDef,
         "LogFormat": LogFormatType,
+        "Enabled": bool,
     },
     total=False,
 )
 
 CreateGlobalReplicationGroupResultTypeDef = TypedDict(
     "CreateGlobalReplicationGroupResultTypeDef",
     {
@@ -2383,14 +2401,49 @@
 
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotName": str,
+        "ReplicationGroupId": str,
+        "ReplicationGroupDescription": str,
+        "CacheClusterId": str,
+        "SnapshotStatus": str,
+        "SnapshotSource": str,
+        "CacheNodeType": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "NumCacheNodes": int,
+        "PreferredAvailabilityZone": str,
+        "PreferredOutpostArn": str,
+        "CacheClusterCreateTime": datetime,
+        "PreferredMaintenanceWindow": str,
+        "TopicArn": str,
+        "Port": int,
+        "CacheParameterGroupName": str,
+        "CacheSubnetGroupName": str,
+        "VpcId": str,
+        "AutoMinorVersionUpgrade": bool,
+        "SnapshotRetentionLimit": int,
+        "SnapshotWindow": str,
+        "NumNodeGroups": int,
+        "AutomaticFailover": AutomaticFailoverStatusType,
+        "NodeSnapshots": List[NodeSnapshotTypeDef],
+        "KmsKeyId": str,
+        "ARN": str,
+        "DataTiering": DataTieringStatusType,
+    },
+    total=False,
+)
+
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2463,45 +2516,43 @@
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CopySnapshotResultTypeDef = TypedDict(
-    "CopySnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
+PendingModifiedValuesTypeDef = TypedDict(
+    "PendingModifiedValuesTypeDef",
     {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "NumCacheNodes": int,
+        "CacheNodeIdsToRemove": List[str],
+        "EngineVersion": str,
+        "CacheNodeType": str,
+        "AuthTokenStatus": AuthTokenUpdateStatusType,
+        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
     },
+    total=False,
 )
 
-DescribeSnapshotsListMessageTypeDef = TypedDict(
-    "DescribeSnapshotsListMessageTypeDef",
+ReplicationGroupPendingModifiedValuesTypeDef = TypedDict(
+    "ReplicationGroupPendingModifiedValuesTypeDef",
     {
-        "Marker": str,
-        "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PrimaryClusterId": str,
+        "AutomaticFailoverStatus": PendingAutomaticFailoverStatusType,
+        "Resharding": ReshardingStatusTypeDef,
+        "AuthTokenStatus": AuthTokenUpdateStatusType,
+        "UserGroups": UserGroupsUpdateStatusTypeDef,
+        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
+        "TransitEncryptionEnabled": bool,
+        "TransitEncryptionMode": TransitEncryptionModeType,
+        "ClusterMode": ClusterModeType,
     },
+    total=False,
 )
 
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
     },
@@ -2686,43 +2737,45 @@
 
 class ModifyReplicationGroupMessageRequestTypeDef(
     _RequiredModifyReplicationGroupMessageRequestTypeDef,
     _OptionalModifyReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-PendingModifiedValuesTypeDef = TypedDict(
-    "PendingModifiedValuesTypeDef",
+CopySnapshotResultTypeDef = TypedDict(
+    "CopySnapshotResultTypeDef",
     {
-        "NumCacheNodes": int,
-        "CacheNodeIdsToRemove": List[str],
-        "EngineVersion": str,
-        "CacheNodeType": str,
-        "AuthTokenStatus": AuthTokenUpdateStatusType,
-        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-ReplicationGroupPendingModifiedValuesTypeDef = TypedDict(
-    "ReplicationGroupPendingModifiedValuesTypeDef",
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
     {
-        "PrimaryClusterId": str,
-        "AutomaticFailoverStatus": PendingAutomaticFailoverStatusType,
-        "Resharding": ReshardingStatusTypeDef,
-        "AuthTokenStatus": AuthTokenUpdateStatusType,
-        "UserGroups": UserGroupsUpdateStatusTypeDef,
-        "LogDeliveryConfigurations": List[PendingLogDeliveryConfigurationTypeDef],
-        "TransitEncryptionEnabled": bool,
-        "TransitEncryptionMode": TransitEncryptionModeType,
-        "ClusterMode": ClusterModeType,
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeSnapshotsListMessageTypeDef = TypedDict(
+    "DescribeSnapshotsListMessageTypeDef",
+    {
+        "Marker": str,
+        "Snapshots": List[SnapshotTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
```

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/waiter.py` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache/waiter.pyi` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache.egg-info/PKG-INFO` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elasticache
-Version: 1.28.0
-Summary: Type annotations for boto3.ElastiCache 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ElastiCache 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-elasticache"></a>
 
 # mypy-boto3-elasticache
 
 [![PyPI - mypy-boto3-elasticache](https://img.shields.io/pypi/v/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elasticache.svg?color=blue)](https://pypi.org/project/mypy-boto3-elasticache)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-elasticache?color=blue)](https://pypistats.org/packages/mypy-boto3-elasticache)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elasticache)](https://pepy.tech/project/mypy-boto3-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElastiCache 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
+[boto3.ElastiCache 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [mypy-boto3-elasticache docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elasticache/).
 
 See how it helps to find and fix potential bugs:
 
@@ -485,14 +485,15 @@
     CacheEngineVersionTypeDef,
     CacheNodeTypeSpecificValueTypeDef,
     CacheNodeUpdateStatusTypeDef,
     ParameterTypeDef,
     CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
+    CloudWatchLogsDestinationDetailsOutputTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
     NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
@@ -534,14 +535,15 @@
     DescribeServiceUpdatesMessageRequestTypeDef,
     DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
     TimeRangeFilterTypeDef,
     DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
+    KinesisFirehoseDestinationDetailsOutputTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
     GlobalReplicationGroupInfoTypeDef,
@@ -549,117 +551,120 @@
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
     PaginatorConfigTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
     SlotMigrationTypeDef,
     ResponseMetadataTypeDef,
     RevokeCacheSecurityGroupIngressMessageRequestTypeDef,
     ServiceUpdateTypeDef,
     SubnetOutpostTypeDef,
+    TagOutputTypeDef,
     TestFailoverMessageRequestTypeDef,
     UnprocessedUpdateActionTypeDef,
     UserGroupPendingChangesTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
-    TagListMessageTypeDef,
     CreateUserMessageRequestTypeDef,
     ModifyUserMessageRequestTypeDef,
     UserResponseMetadataTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
     CacheSecurityGroupTypeDef,
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
-    NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
     DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
     DescribeUpdateActionsMessageRequestTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
+    DestinationDetailsOutputTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
+    NodeSnapshotTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
+    TagListMessageTypeDef,
     UpdateActionResultsMessageTypeDef,
     UserGroupResponseMetadataTypeDef,
     UserGroupTypeDef,
     DescribeUsersResultTypeDef,
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
-    SnapshotTypeDef,
-    LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
+    LogDeliveryConfigurationRequestTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
+    SnapshotTypeDef,
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
-    CopySnapshotResultTypeDef,
-    CreateSnapshotResultTypeDef,
-    DeleteSnapshotResultTypeDef,
-    DescribeSnapshotsListMessageTypeDef,
+    PendingModifiedValuesTypeDef,
+    ReplicationGroupPendingModifiedValuesTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
-    PendingModifiedValuesTypeDef,
-    ReplicationGroupPendingModifiedValuesTypeDef,
+    CopySnapshotResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     CacheClusterTypeDef,
     ReplicationGroupTypeDef,
     CacheClusterMessageTypeDef,
```

### Comparing `mypy-boto3-elasticache-1.28.0/mypy_boto3_elasticache.egg-info/SOURCES.txt` & `mypy-boto3-elasticache-1.28.12/mypy_boto3_elasticache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elasticache-1.28.0/setup.py` & `mypy-boto3-elasticache-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elasticache",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_elasticache"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElastiCache 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ElastiCache 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

