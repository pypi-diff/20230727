# Comparing `tmp/mypy-boto3-neptune-1.28.0.tar.gz` & `tmp/mypy-boto3-neptune-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-neptune-1.28.0.tar", last modified: Thu Jul  6 21:00:11 2023, max compression
+gzip compressed data, was "mypy-boto3-neptune-1.28.12.tar", last modified: Thu Jul 27 05:35:04 2023, max compression
```

## Comparing `mypy-boto3-neptune-1.28.0.tar` & `mypy-boto3-neptune-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.866379 mypy-boto3-neptune-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25543 2023-07-06 21:00:11.866379 mypy-boto3-neptune-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24058 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.866379 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67621 2023-07-06 20:48:05.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    67527 2023-07-06 20:48:05.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-07-06 20:48:06.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-07-06 20:48:06.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-07-06 20:48:05.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-07-06 20:48:05.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    84576 2023-07-06 20:48:08.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    84499 2023-07-06 20:48:07.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-06 20:48:05.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-06 20:48:05.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.866379 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25543 2023-07-06 21:00:11.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 21:00:11.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:11.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:11.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:11.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 21:00:11.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:11.866379 mypy-boto3-neptune-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.944427 mypy-boto3-neptune-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25580 2023-07-27 05:35:04.944427 mypy-boto3-neptune-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.944427 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67621 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67527 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-07-27 05:26:53.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-27 05:26:53.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-07-27 05:26:53.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-07-27 05:26:53.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    85182 2023-07-27 05:26:54.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85105 2023-07-27 05:26:54.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-27 05:26:53.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-27 05:26:53.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.944427 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25580 2023-07-27 05:35:04.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 05:35:04.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:04.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:35:04.000000 mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:04.944427 mypy-boto3-neptune-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:26:52.000000 mypy-boto3-neptune-1.28.12/setup.py
```

### Comparing `mypy-boto3-neptune-1.28.0/LICENSE` & `mypy-boto3-neptune-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.0/PKG-INFO` & `mypy-boto3-neptune-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-neptune
-Version: 1.28.0
-Summary: Type annotations for boto3.Neptune 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Neptune 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-neptune"></a>
 
 # mypy-boto3-neptune
 
 [![PyPI - mypy-boto3-neptune](https://img.shields.io/pypi/v/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-neptune?color=blue)](https://pypistats.org/packages/mypy-boto3-neptune)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-neptune)](https://pepy.tech/project/mypy-boto3-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Neptune 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[boto3.Neptune 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [mypy-boto3-neptune docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/).
 
 See how it helps to find and fix potential bugs:
 
@@ -439,15 +439,15 @@
     DBParameterGroupTypeDef,
     CreateDBClusterEndpointOutputTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterEndpointTypeDef,
     DBClusterMemberTypeDef,
     DBClusterOptionGroupStatusTypeDef,
-    ParameterTypeDef,
+    ParameterOutputTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     ServerlessV2ScalingConfigurationInfoTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     TimezoneTypeDef,
     UpgradeTargetTypeDef,
@@ -479,14 +479,15 @@
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     FailoverGlobalClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ModifyDBClusterEndpointMessageRequestTypeDef,
     ModifyDBClusterEndpointOutputTypeDef,
+    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
     PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PromoteReadReplicaDBClusterMessageRequestTypeDef,
@@ -495,14 +496,15 @@
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveRoleFromDBClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
+    TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     DeleteEventSubscriptionResultTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
@@ -512,15 +514,14 @@
     CreateDBClusterEndpointMessageRequestTypeDef,
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBParameterGroupMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
-    TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ClusterPendingModifiedValuesTypeDef,
     PendingModifiedValuesTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
@@ -536,18 +537,14 @@
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
     RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ModifyDBParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBEngineVersionTypeDef,
     DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
     DescribeDBClusterEndpointsMessageRequestTypeDef,
     DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
     DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
@@ -580,16 +577,21 @@
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ModifyDBParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBParameterGroupMessageRequestTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
+    TagListMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
     DBClusterTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
```

### Comparing `mypy-boto3-neptune-1.28.0/README.md` & `mypy-boto3-neptune-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-neptune"></a>
 
 # mypy-boto3-neptune
 
 [![PyPI - mypy-boto3-neptune](https://img.shields.io/pypi/v/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-neptune?color=blue)](https://pypistats.org/packages/mypy-boto3-neptune)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-neptune)](https://pepy.tech/project/mypy-boto3-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Neptune 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[boto3.Neptune 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [mypy-boto3-neptune docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,15 +407,15 @@
     DBParameterGroupTypeDef,
     CreateDBClusterEndpointOutputTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterEndpointTypeDef,
     DBClusterMemberTypeDef,
     DBClusterOptionGroupStatusTypeDef,
-    ParameterTypeDef,
+    ParameterOutputTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     ServerlessV2ScalingConfigurationInfoTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     TimezoneTypeDef,
     UpgradeTargetTypeDef,
@@ -447,14 +447,15 @@
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     FailoverGlobalClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ModifyDBClusterEndpointMessageRequestTypeDef,
     ModifyDBClusterEndpointOutputTypeDef,
+    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
     PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PromoteReadReplicaDBClusterMessageRequestTypeDef,
@@ -463,14 +464,15 @@
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveRoleFromDBClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
+    TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     DeleteEventSubscriptionResultTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
@@ -480,15 +482,14 @@
     CreateDBClusterEndpointMessageRequestTypeDef,
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBParameterGroupMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
-    TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ClusterPendingModifiedValuesTypeDef,
     PendingModifiedValuesTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
@@ -504,18 +505,14 @@
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
     RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ModifyDBParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBEngineVersionTypeDef,
     DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
     DescribeDBClusterEndpointsMessageRequestTypeDef,
     DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
     DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
@@ -548,16 +545,21 @@
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ModifyDBParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBParameterGroupMessageRequestTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
+    TagListMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
     DBClusterTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
```

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/__init__.py` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/__init__.pyi` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/__main__.py` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Neptune 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Neptune 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune\nOther"
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

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/client.py` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/client.pyi` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/literals.py` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/literals.py`

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

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/literals.pyi` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,15 @@
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
@@ -276,26 +277,28 @@
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

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/paginator.py` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/paginator.pyi` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/type_defs.py` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "DBParameterGroupTypeDef",
     "CreateDBClusterEndpointOutputTypeDef",
     "ServerlessV2ScalingConfigurationTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
-    "ParameterTypeDef",
+    "ParameterOutputTypeDef",
     "DBClusterParameterGroupNameMessageTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "ServerlessV2ScalingConfigurationInfoTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "TimezoneTypeDef",
     "UpgradeTargetTypeDef",
@@ -78,14 +78,15 @@
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "FailoverGlobalClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
     "ModifyDBClusterEndpointMessageRequestTypeDef",
     "ModifyDBClusterEndpointOutputTypeDef",
+    "ParameterTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
@@ -94,14 +95,15 @@
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveRoleFromDBClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "ResponseMetadataTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
+    "TagOutputTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
     "EventSubscriptionsMessageTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
@@ -111,15 +113,14 @@
     "CreateDBClusterEndpointMessageRequestTypeDef",
     "CreateDBClusterParameterGroupMessageRequestTypeDef",
     "CreateDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBInstanceMessageRequestTypeDef",
     "CreateDBParameterGroupMessageRequestTypeDef",
     "CreateDBSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
-    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionTypeDef",
     "SubnetTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
     "ClusterPendingModifiedValuesTypeDef",
     "PendingModifiedValuesTypeDef",
     "CopyDBClusterParameterGroupResultTypeDef",
     "CreateDBClusterParameterGroupResultTypeDef",
@@ -135,18 +136,14 @@
     "ModifyDBClusterMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
     "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBEngineVersionTypeDef",
     "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
@@ -179,16 +176,21 @@
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBParameterGroupMessageRequestTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "ValidStorageOptionsTypeDef",
+    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
     "DBClusterTypeDef",
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
@@ -459,16 +461,16 @@
     {
         "DBClusterOptionGroupName": str,
         "Status": str,
     },
     total=False,
 )
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "ApplyType": str,
         "DataType": str,
@@ -875,14 +877,31 @@
         "StaticMembers": List[str],
         "ExcludedMembers": List[str],
         "DBClusterEndpointArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
+    {
+        "ParameterName": str,
+        "ParameterValue": str,
+        "Description": str,
+        "Source": str,
+        "ApplyType": str,
+        "DataType": str,
+        "AllowedValues": str,
+        "IsModifiable": bool,
+        "MinimumEngineVersion": str,
+        "ApplyMethod": ApplyMethodType,
+    },
+    total=False,
+)
+
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -1105,14 +1124,23 @@
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
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
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1447,22 +1475,14 @@
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
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
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
@@ -1838,101 +1858,39 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DBParameterGroupDetailsTypeDef = TypedDict(
     "DBParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterTypeDef],
-    },
-    total=False,
-)
-
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-)
-
-ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-)
-
-_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-    total=False,
-)
-
-
-class ResetDBClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
-
-
-_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-    },
-)
-_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
     },
     total=False,
 )
 
-
-class ResetDBParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBParameterGroupMessageRequestTypeDef,
-):
-    pass
-
-
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
     total=False,
@@ -2529,14 +2487,76 @@
         "StorageEncrypted": bool,
         "DeletionProtection": bool,
         "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
     },
     total=False,
 )
 
+ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+    total=False,
+)
+
+
+class ResetDBClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+
+_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+    },
+)
+_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+    total=False,
+)
+
+
+class ResetDBParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
     total=False,
@@ -2549,14 +2569,22 @@
         "StorageSize": List[RangeTypeDef],
         "ProvisionedIops": List[RangeTypeDef],
         "IopsToStorageRatio": List[DoubleRangeTypeDef],
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
 OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
     "OrderableDBInstanceOptionsMessageTypeDef",
     {
         "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/type_defs.pyi` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "DBParameterGroupTypeDef",
     "CreateDBClusterEndpointOutputTypeDef",
     "ServerlessV2ScalingConfigurationTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
-    "ParameterTypeDef",
+    "ParameterOutputTypeDef",
     "DBClusterParameterGroupNameMessageTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "ServerlessV2ScalingConfigurationInfoTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "TimezoneTypeDef",
     "UpgradeTargetTypeDef",
@@ -77,14 +77,15 @@
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "FailoverGlobalClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
     "ModifyDBClusterEndpointMessageRequestTypeDef",
     "ModifyDBClusterEndpointOutputTypeDef",
+    "ParameterTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
     "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
@@ -93,14 +94,15 @@
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveRoleFromDBClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "ResponseMetadataTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
+    "TagOutputTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
     "EventSubscriptionsMessageTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
@@ -110,15 +112,14 @@
     "CreateDBClusterEndpointMessageRequestTypeDef",
     "CreateDBClusterParameterGroupMessageRequestTypeDef",
     "CreateDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBInstanceMessageRequestTypeDef",
     "CreateDBParameterGroupMessageRequestTypeDef",
     "CreateDBSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
-    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionTypeDef",
     "SubnetTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
     "ClusterPendingModifiedValuesTypeDef",
     "PendingModifiedValuesTypeDef",
     "CopyDBClusterParameterGroupResultTypeDef",
     "CreateDBClusterParameterGroupResultTypeDef",
@@ -134,18 +135,14 @@
     "ModifyDBClusterMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
     "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    "ResetDBClusterParameterGroupMessageRequestTypeDef",
-    "ResetDBParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBEngineVersionTypeDef",
     "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
@@ -178,16 +175,21 @@
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    "ResetDBClusterParameterGroupMessageRequestTypeDef",
+    "ResetDBParameterGroupMessageRequestTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "ValidStorageOptionsTypeDef",
+    "TagListMessageTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
     "DBClusterTypeDef",
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
@@ -454,16 +456,16 @@
     {
         "DBClusterOptionGroupName": str,
         "Status": str,
     },
     total=False,
 )
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "ApplyType": str,
         "DataType": str,
@@ -864,14 +866,31 @@
         "StaticMembers": List[str],
         "ExcludedMembers": List[str],
         "DBClusterEndpointArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
+    {
+        "ParameterName": str,
+        "ParameterValue": str,
+        "Description": str,
+        "Source": str,
+        "ApplyType": str,
+        "DataType": str,
+        "AllowedValues": str,
+        "IsModifiable": bool,
+        "MinimumEngineVersion": str,
+        "ApplyMethod": ApplyMethodType,
+    },
+    total=False,
+)
+
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -1082,14 +1101,23 @@
 StopDBClusterMessageRequestTypeDef = TypedDict(
     "StopDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
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
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1404,22 +1432,14 @@
 
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
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
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
@@ -1785,97 +1805,39 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DBParameterGroupDetailsTypeDef = TypedDict(
     "DBParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterTypeDef],
-    },
-    total=False,
-)
-
-ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-)
-
-ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-)
-
-_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-    total=False,
-)
-
-class ResetDBClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
-
-_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "DBParameterGroupName": str,
-    },
-)
-_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
+        "Parameters": List[ParameterOutputTypeDef],
     },
     total=False,
 )
 
-class ResetDBParameterGroupMessageRequestTypeDef(
-    _RequiredResetDBParameterGroupMessageRequestTypeDef,
-    _OptionalResetDBParameterGroupMessageRequestTypeDef,
-):
-    pass
-
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
     total=False,
@@ -2452,14 +2414,72 @@
         "StorageEncrypted": bool,
         "DeletionProtection": bool,
         "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
     },
     total=False,
 )
 
+ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+ModifyDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+)
+
+_RequiredResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalResetDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBClusterParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+    total=False,
+)
+
+class ResetDBClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
+
+_RequiredResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "DBParameterGroupName": str,
+    },
+)
+_OptionalResetDBParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetDBParameterGroupMessageRequestTypeDef",
+    {
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
+    },
+    total=False,
+)
+
+class ResetDBParameterGroupMessageRequestTypeDef(
+    _RequiredResetDBParameterGroupMessageRequestTypeDef,
+    _OptionalResetDBParameterGroupMessageRequestTypeDef,
+):
+    pass
+
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
     total=False,
@@ -2472,14 +2492,22 @@
         "StorageSize": List[RangeTypeDef],
         "ProvisionedIops": List[RangeTypeDef],
         "IopsToStorageRatio": List[DoubleRangeTypeDef],
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
 OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
     "OrderableDBInstanceOptionsMessageTypeDef",
     {
         "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/waiter.py` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/waiter.pyi` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/PKG-INFO` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-neptune
-Version: 1.28.0
-Summary: Type annotations for boto3.Neptune 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Neptune 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-neptune"></a>
 
 # mypy-boto3-neptune
 
 [![PyPI - mypy-boto3-neptune](https://img.shields.io/pypi/v/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-neptune?color=blue)](https://pypistats.org/packages/mypy-boto3-neptune)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-neptune)](https://pepy.tech/project/mypy-boto3-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Neptune 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[boto3.Neptune 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [mypy-boto3-neptune docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/).
 
 See how it helps to find and fix potential bugs:
 
@@ -439,15 +439,15 @@
     DBParameterGroupTypeDef,
     CreateDBClusterEndpointOutputTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterEndpointTypeDef,
     DBClusterMemberTypeDef,
     DBClusterOptionGroupStatusTypeDef,
-    ParameterTypeDef,
+    ParameterOutputTypeDef,
     DBClusterParameterGroupNameMessageTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     ServerlessV2ScalingConfigurationInfoTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     TimezoneTypeDef,
     UpgradeTargetTypeDef,
@@ -479,14 +479,15 @@
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     FailoverGlobalClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ModifyDBClusterEndpointMessageRequestTypeDef,
     ModifyDBClusterEndpointOutputTypeDef,
+    ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
     PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PromoteReadReplicaDBClusterMessageRequestTypeDef,
@@ -495,14 +496,15 @@
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveRoleFromDBClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
+    TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     DeleteEventSubscriptionResultTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
@@ -512,15 +514,14 @@
     CreateDBClusterEndpointMessageRequestTypeDef,
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBParameterGroupMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
-    TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ClusterPendingModifiedValuesTypeDef,
     PendingModifiedValuesTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
@@ -536,18 +537,14 @@
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
     RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
-    ModifyDBClusterParameterGroupMessageRequestTypeDef,
-    ModifyDBParameterGroupMessageRequestTypeDef,
-    ResetDBClusterParameterGroupMessageRequestTypeDef,
-    ResetDBParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBEngineVersionTypeDef,
     DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
     DescribeDBClusterEndpointsMessageRequestTypeDef,
     DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
     DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
@@ -580,16 +577,21 @@
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
+    ModifyDBClusterParameterGroupMessageRequestTypeDef,
+    ModifyDBParameterGroupMessageRequestTypeDef,
+    ResetDBClusterParameterGroupMessageRequestTypeDef,
+    ResetDBParameterGroupMessageRequestTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
+    TagListMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
     DBClusterTypeDef,
     DescribeEngineDefaultClusterParametersResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
     DescribeDBClusterSnapshotAttributesResultTypeDef,
     ModifyDBClusterSnapshotAttributeResultTypeDef,
```

### Comparing `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/SOURCES.txt` & `mypy-boto3-neptune-1.28.12/mypy_boto3_neptune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.28.0/setup.py` & `mypy-boto3-neptune-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-neptune",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_neptune"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Neptune 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Neptune 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

