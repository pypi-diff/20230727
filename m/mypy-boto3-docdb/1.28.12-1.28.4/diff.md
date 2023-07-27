# Comparing `tmp/mypy-boto3-docdb-1.28.12.tar.gz` & `tmp/mypy-boto3-docdb-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-docdb-1.28.12.tar", last modified: Thu Jul 27 05:34:35 2023, max compression
+gzip compressed data, was "mypy-boto3-docdb-1.28.4.tar", last modified: Tue Jul 18 01:01:42 2023, max compression
```

## Comparing `mypy-boto3-docdb-1.28.12.tar` & `mypy-boto3-docdb-1.28.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.872529 mypy-boto3-docdb-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22678 2023-07-27 05:34:35.868529 mypy-boto3-docdb-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21199 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.864529 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51205 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51130 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-07-27 05:20:26.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17415 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17400 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61193 2023-07-27 05:20:27.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    61140 2023-07-27 05:20:27.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.868529 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22678 2023-07-27 05:34:35.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-27 05:34:35.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:35.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:34:35.000000 mypy-boto3-docdb-1.28.12/mypy_boto3_docdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:35.872529 mypy-boto3-docdb-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:20:25.000000 mypy-boto3-docdb-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22691 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21214 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51205 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51130 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17389 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60559 2023-07-18 01:00:30.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60506 2023-07-18 01:00:29.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-18 01:00:28.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22691 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 01:01:41.000000 mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:42.001310 mypy-boto3-docdb-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-18 01:00:27.000000 mypy-boto3-docdb-1.28.4/setup.py
```

### Comparing `mypy-boto3-docdb-1.28.12/LICENSE` & `mypy-boto3-docdb-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.12/PKG-INFO` & `mypy-boto3-docdb-1.28.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb
-Version: 1.28.12
-Summary: Type annotations for boto3.DocDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.4
+Summary: Type annotations for boto3.DocDB 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb)](https://pepy.tech/project/mypy-boto3-docdb)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,66 +408,66 @@
 `mypy_boto3_docdb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_docdb.type_defs import (
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     CertificateTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterMemberTypeDef,
     ParameterOutputTypeDef,
-    DBClusterParameterGroupNameMessageTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     EndpointTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     PendingMaintenanceActionTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
     TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
+    DBClusterParameterGroupNameMessageTypeDef,
     DeleteEventSubscriptionResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopyDBClusterParameterGroupMessageRequestTypeDef,
     CopyDBClusterSnapshotMessageRequestTypeDef,
     CreateDBClusterMessageRequestTypeDef,
@@ -490,43 +490,43 @@
     DBClusterSnapshotMessageTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBClusterTypeDef,
     DBEngineVersionTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
-    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
-    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
-    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
-    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
-    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
-    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBInstancesMessageRequestTypeDef,
-    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
-    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
-    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
+    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
+    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
+    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
+    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
+    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
+    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
+    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
     ModifyDBClusterParameterGroupMessageRequestTypeDef,
     ResetDBClusterParameterGroupMessageRequestTypeDef,
```

### Comparing `mypy-boto3-docdb-1.28.12/README.md` & `mypy-boto3-docdb-1.28.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb)](https://pepy.tech/project/mypy-boto3-docdb)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -376,66 +376,66 @@
 `mypy_boto3_docdb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_docdb.type_defs import (
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     CertificateTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterMemberTypeDef,
     ParameterOutputTypeDef,
-    DBClusterParameterGroupNameMessageTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     EndpointTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     PendingMaintenanceActionTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
     TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
+    DBClusterParameterGroupNameMessageTypeDef,
     DeleteEventSubscriptionResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopyDBClusterParameterGroupMessageRequestTypeDef,
     CopyDBClusterSnapshotMessageRequestTypeDef,
     CreateDBClusterMessageRequestTypeDef,
@@ -458,43 +458,43 @@
     DBClusterSnapshotMessageTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBClusterTypeDef,
     DBEngineVersionTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
-    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
-    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
-    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
-    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
-    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
-    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBInstancesMessageRequestTypeDef,
-    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
-    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
-    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
+    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
+    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
+    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
+    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
+    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
+    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
+    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
     ModifyDBClusterParameterGroupMessageRequestTypeDef,
     ResetDBClusterParameterGroupMessageRequestTypeDef,
```

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/__init__.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/__init__.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/__main__.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DocDB 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.DocDB 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/client.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/client.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/literals.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -273,28 +272,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
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
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/literals.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -271,28 +270,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
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
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/paginator.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     """
 
     def paginate(
         self,
         *,
         CertificateIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describecertificatespaginator)
         """
 
 
@@ -120,15 +120,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbclusterparametergroupspaginator)
         """
 
 
@@ -140,15 +140,15 @@
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbclusterparameterspaginator)
         """
 
 
@@ -163,15 +163,15 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbclustersnapshotspaginator)
         """
 
 
@@ -182,15 +182,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbclusterspaginator)
         """
 
 
@@ -206,15 +206,15 @@
         Engine: str = ...,
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbengineversionspaginator)
         """
 
 
@@ -225,15 +225,15 @@
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbinstancespaginator)
         """
 
 
@@ -244,15 +244,15 @@
     """
 
     def paginate(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbsubnetgroupspaginator)
         """
 
 
@@ -263,15 +263,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -287,15 +287,15 @@
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describeeventspaginator)
         """
 
 
@@ -306,15 +306,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeGlobalClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describeglobalclusterspaginator)
         """
 
 
@@ -329,15 +329,15 @@
         *,
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[OrderableDBInstanceOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
 
@@ -348,13 +348,13 @@
     """
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[PendingMaintenanceActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describependingmaintenanceactionspaginator)
         """
```

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/paginator.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     """
 
     def paginate(
         self,
         *,
         CertificateIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[CertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describecertificatespaginator)
         """
 
 class DescribeDBClusterParameterGroupsPaginator(Paginator):
@@ -116,15 +116,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbclusterparametergroupspaginator)
         """
 
 class DescribeDBClusterParametersPaginator(Paginator):
@@ -135,15 +135,15 @@
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbclusterparameterspaginator)
         """
 
 class DescribeDBClusterSnapshotsPaginator(Paginator):
@@ -157,15 +157,15 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbclustersnapshotspaginator)
         """
 
 class DescribeDBClustersPaginator(Paginator):
@@ -175,15 +175,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbclusterspaginator)
         """
 
 class DescribeDBEngineVersionsPaginator(Paginator):
@@ -198,15 +198,15 @@
         Engine: str = ...,
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBEngineVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbengineversionspaginator)
         """
 
 class DescribeDBInstancesPaginator(Paginator):
@@ -216,15 +216,15 @@
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbinstancespaginator)
         """
 
 class DescribeDBSubnetGroupsPaginator(Paginator):
@@ -234,15 +234,15 @@
     """
 
     def paginate(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DBSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describedbsubnetgroupspaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(Paginator):
@@ -252,15 +252,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEventSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(Paginator):
@@ -275,15 +275,15 @@
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describeeventspaginator)
         """
 
 class DescribeGlobalClustersPaginator(Paginator):
@@ -293,15 +293,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeGlobalClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describeglobalclusterspaginator)
         """
 
 class DescribeOrderableDBInstanceOptionsPaginator(Paginator):
@@ -315,15 +315,15 @@
         *,
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[OrderableDBInstanceOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
 class DescribePendingMaintenanceActionsPaginator(Paginator):
@@ -333,13 +333,13 @@
     """
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[PendingMaintenanceActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/paginators/#describependingmaintenanceactionspaginator)
         """
```

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/type_defs.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,66 +22,66 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "CertificateTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "DBClusterParameterGroupTypeDef",
     "DBClusterSnapshotTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterMemberTypeDef",
     "ParameterOutputTypeDef",
-    "DBClusterParameterGroupNameMessageTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "EndpointTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     "DeleteDBClusterSnapshotMessageRequestTypeDef",
     "DeleteDBInstanceMessageRequestTypeDef",
     "DeleteDBSubnetGroupMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteGlobalClusterMessageRequestTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
     "ParameterTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
     "TagOutputTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
+    "DBClusterParameterGroupNameMessageTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopyDBClusterParameterGroupMessageRequestTypeDef",
     "CopyDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBClusterMessageRequestTypeDef",
@@ -104,43 +104,43 @@
     "DBClusterSnapshotMessageTypeDef",
     "DeleteDBClusterSnapshotResultTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBClusterTypeDef",
     "DBEngineVersionTypeDef",
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
-    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
-    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
-    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
-    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
     "DescribeDBClustersMessageRequestTypeDef",
-    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     "DescribeDBEngineVersionsMessageRequestTypeDef",
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     "DescribeDBInstancesMessageRequestTypeDef",
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultClusterParametersMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     "DescribeGlobalClustersMessageRequestTypeDef",
-    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
-    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
+    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
     "ModifyDBClusterParameterGroupMessageRequestTypeDef",
     "ResetDBClusterParameterGroupMessageRequestTypeDef",
@@ -198,15 +198,25 @@
         "SubscriptionCreationTime": str,
         "SourceType": str,
         "SourceIdsList": List[str],
         "EventCategoriesList": List[str],
         "Enabled": bool,
         "EventSubscriptionArn": str,
     },
-    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -224,28 +234,26 @@
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
-    total=False,
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateIdentifier": str,
         "CertificateType": str,
         "Thumbprint": str,
         "ValidFrom": datetime,
         "ValidTill": datetime,
         "CertificateArn": str,
     },
-    total=False,
 )
 
 CloudwatchLogsExportConfigurationTypeDef = TypedDict(
     "CloudwatchLogsExportConfigurationTypeDef",
     {
         "EnableLogTypes": Sequence[str],
         "DisableLogTypes": Sequence[str],
@@ -257,15 +265,14 @@
     "DBClusterParameterGroupTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBClusterParameterGroupArn": str,
     },
-    total=False,
 )
 
 DBClusterSnapshotTypeDef = TypedDict(
     "DBClusterSnapshotTypeDef",
     {
         "AvailabilityZones": List[str],
         "DBClusterSnapshotIdentifier": str,
@@ -281,15 +288,14 @@
         "SnapshotType": str,
         "PercentProgress": int,
         "StorageEncrypted": bool,
         "KmsKeyId": str,
         "DBClusterSnapshotArn": str,
         "SourceDBClusterSnapshotArn": str,
     },
-    total=False,
 )
 
 _RequiredCreateGlobalClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
     },
@@ -319,15 +325,14 @@
     "DBClusterMemberTypeDef",
     {
         "DBInstanceIdentifier": str,
         "IsClusterWriter": bool,
         "DBClusterParameterGroupStatus": str,
         "PromotionTier": int,
     },
-    total=False,
 )
 
 ParameterOutputTypeDef = TypedDict(
     "ParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
@@ -336,83 +341,68 @@
         "ApplyType": str,
         "DataType": str,
         "AllowedValues": str,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ApplyMethod": ApplyMethodType,
     },
-    total=False,
-)
-
-DBClusterParameterGroupNameMessageTypeDef = TypedDict(
-    "DBClusterParameterGroupNameMessageTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 DBClusterRoleTypeDef = TypedDict(
     "DBClusterRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
     },
-    total=False,
 )
 
 DBClusterSnapshotAttributeTypeDef = TypedDict(
     "DBClusterSnapshotAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[str],
     },
-    total=False,
 )
 
 VpcSecurityGroupMembershipTypeDef = TypedDict(
     "VpcSecurityGroupMembershipTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
-    total=False,
 )
 
 UpgradeTargetTypeDef = TypedDict(
     "UpgradeTargetTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "Description": str,
         "AutoUpgrade": bool,
         "IsMajorVersionUpgrade": bool,
     },
-    total=False,
 )
 
 DBInstanceStatusInfoTypeDef = TypedDict(
     "DBInstanceStatusInfoTypeDef",
     {
         "StatusType": str,
         "Normal": bool,
         "Status": str,
         "Message": str,
     },
-    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "Port": int,
         "HostedZoneId": str,
     },
-    total=False,
 )
 
 _RequiredDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
@@ -479,14 +469,24 @@
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 DescribeDBClusterSnapshotAttributesMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
     },
 )
 
@@ -495,41 +495,32 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
-    total=False,
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "EventCategories": List[str],
         "Date": datetime,
         "SourceArn": str,
     },
-    total=False,
 )
 
 FailoverDBClusterMessageRequestTypeDef = TypedDict(
     "FailoverDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "TargetDBInstanceIdentifier": str,
@@ -540,15 +531,14 @@
 GlobalClusterMemberTypeDef = TypedDict(
     "GlobalClusterMemberTypeDef",
     {
         "DBClusterArn": str,
         "Readers": List[str],
         "IsWriter": bool,
     },
-    total=False,
 )
 
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
@@ -685,44 +675,32 @@
 class ModifyGlobalClusterMessageRequestTypeDef(
     _RequiredModifyGlobalClusterMessageRequestTypeDef,
     _OptionalModifyGlobalClusterMessageRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PendingCloudwatchLogsExportsTypeDef = TypedDict(
     "PendingCloudwatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": List[str],
         "LogTypesToDisable": List[str],
     },
-    total=False,
 )
 
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 _RequiredRebootDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredRebootDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
@@ -762,25 +740,14 @@
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceName": str,
         "TagKeys": Sequence[str],
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
 StartDBClusterMessageRequestTypeDef = TypedDict(
     "StartDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
@@ -793,63 +760,77 @@
 
 TagOutputTypeDef = TypedDict(
     "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
-    total=False,
 )
 
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEventSubscriptionResultTypeDef = TypedDict(
     "CreateEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DBClusterParameterGroupNameMessageTypeDef = TypedDict(
+    "DBClusterParameterGroupNameMessageTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventSubscriptionResultTypeDef = TypedDict(
     "DeleteEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventSubscriptionsMessageTypeDef = TypedDict(
     "EventSubscriptionsMessageTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyEventSubscriptionResultTypeDef = TypedDict(
     "ModifyEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveSourceIdentifierFromSubscriptionResultTypeDef = TypedDict(
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
     {
         "ResourceName": str,
@@ -1148,33 +1129,31 @@
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "Vpc": bool,
     },
-    total=False,
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
-    total=False,
 )
 
 CertificateMessageTypeDef = TypedDict(
     "CertificateMessageTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredModifyDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
@@ -1207,94 +1186,92 @@
     pass
 
 
 CopyDBClusterParameterGroupResultTypeDef = TypedDict(
     "CopyDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterParameterGroupResultTypeDef = TypedDict(
     "CreateDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupsMessageTypeDef = TypedDict(
     "DBClusterParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "DBClusterParameterGroups": List[DBClusterParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDBClusterSnapshotResultTypeDef = TypedDict(
     "CopyDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterSnapshotResultTypeDef = TypedDict(
     "CreateDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterSnapshotMessageTypeDef = TypedDict(
     "DBClusterSnapshotMessageTypeDef",
     {
         "Marker": str,
         "DBClusterSnapshots": List[DBClusterSnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBClusterSnapshotResultTypeDef = TypedDict(
     "DeleteDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
         "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
         "Parameters": List[ParameterOutputTypeDef],
     },
-    total=False,
 )
 
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
-    total=False,
 )
 
 DBClusterTypeDef = TypedDict(
     "DBClusterTypeDef",
     {
         "AvailabilityZones": List[str],
         "BackupRetentionPeriod": int,
@@ -1325,98 +1302,52 @@
         "DBClusterArn": str,
         "AssociatedRoles": List[DBClusterRoleTypeDef],
         "CloneGroupId": str,
         "ClusterCreateTime": datetime,
         "EnabledCloudwatchLogsExports": List[str],
         "DeletionProtection": bool,
     },
-    total=False,
 )
 
 DBEngineVersionTypeDef = TypedDict(
     "DBEngineVersionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "DBEngineDescription": str,
         "DBEngineVersionDescription": str,
         "ValidUpgradeTarget": List[UpgradeTargetTypeDef],
         "ExportableLogTypes": List[str],
         "SupportsLogExportsToCloudwatchLogs": bool,
     },
-    total=False,
-)
-
-DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
-    {
-        "CertificateIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 DescribeCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeCertificatesMessageRequestTypeDef",
     {
         "CertificateIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
-    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
-    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeDBClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDBClusterParametersMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
     },
 )
 _OptionalDescribeDBClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1434,28 +1365,14 @@
 class DescribeDBClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDBClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDBClusterParametersMessageRequestTypeDef,
 ):
     pass
 
 
-DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "DBClusterSnapshotIdentifier": str,
-        "SnapshotType": str,
-        "Filters": Sequence[FilterTypeDef],
-        "IncludeShared": bool,
-        "IncludePublic": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1463,50 +1380,25 @@
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
     },
     total=False,
 )
 
-DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
-    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClustersMessageRequestTypeDef = TypedDict(
     "DescribeDBClustersMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
-    {
-        "Engine": str,
-        "EngineVersion": str,
-        "DBParameterGroupFamily": str,
-        "Filters": Sequence[FilterTypeDef],
-        "DefaultOnly": bool,
-        "ListSupportedCharacterSets": bool,
-        "ListSupportedTimezones": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBEngineVersionsMessageRequestTypeDef = TypedDict(
     "DescribeDBEngineVersionsMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1515,45 +1407,25 @@
         "DefaultOnly": bool,
         "ListSupportedCharacterSets": bool,
         "ListSupportedTimezones": bool,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
-    {
-        "DBInstanceIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBInstancesMessageRequestTypeDef = TypedDict(
     "DescribeDBInstancesMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
-    {
-        "DBSubnetGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -1590,50 +1462,25 @@
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -1642,62 +1489,25 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
-    {
-        "GlobalClusterIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
     "DescribeGlobalClustersMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
-    {
-        "Engine": str,
-    },
-)
-_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
-    {
-        "EngineVersion": str,
-        "DBInstanceClass": str,
-        "LicenseModel": str,
-        "Vpc": bool,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
-    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
-    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     {
         "Engine": str,
     },
 )
 _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
@@ -1718,26 +1528,14 @@
 class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
     _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
 ):
     pass
 
 
-DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
-    TypedDict(
-        "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
-        {
-            "ResourceIdentifier": str,
-            "Filters": Sequence[FilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -1763,14 +1561,191 @@
 class ListTagsForResourceMessageRequestTypeDef(
     _RequiredListTagsForResourceMessageRequestTypeDef,
     _OptionalListTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
 
+DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+    {
+        "CertificateIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
+    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+):
+    pass
+
+
+DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "DBClusterSnapshotIdentifier": str,
+        "SnapshotType": str,
+        "Filters": Sequence[FilterTypeDef],
+        "IncludeShared": bool,
+        "IncludePublic": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
+    {
+        "Engine": str,
+        "EngineVersion": str,
+        "DBParameterGroupFamily": str,
+        "Filters": Sequence[FilterTypeDef],
+        "DefaultOnly": bool,
+        "ListSupportedCharacterSets": bool,
+        "ListSupportedTimezones": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+    {
+        "DBInstanceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
+    {
+        "DBSubnetGroupName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
+    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    {
+        "GlobalClusterIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    {
+        "Engine": str,
+    },
+)
+_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    {
+        "EngineVersion": str,
+        "DBInstanceClass": str,
+        "LicenseModel": str,
+        "Vpc": bool,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
+    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+):
+    pass
+
+
+DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
+    TypedDict(
+        "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
+        {
+            "ResourceIdentifier": str,
+            "Filters": Sequence[FilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
 DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef = TypedDict(
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     {
         "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -1791,24 +1766,24 @@
     total=False,
 )
 
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventsMessageTypeDef = TypedDict(
     "EventsMessageTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalClusterTypeDef = TypedDict(
     "GlobalClusterTypeDef",
     {
         "GlobalClusterIdentifier": str,
@@ -1818,15 +1793,14 @@
         "Engine": str,
         "EngineVersion": str,
         "DatabaseName": str,
         "StorageEncrypted": bool,
         "DeletionProtection": bool,
         "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
     },
-    total=False,
 )
 
 ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "ModifyDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "Parameters": Sequence[ParameterTypeDef],
@@ -1870,225 +1844,222 @@
         "Iops": int,
         "DBInstanceIdentifier": str,
         "StorageType": str,
         "CACertificateIdentifier": str,
         "DBSubnetGroupName": str,
         "PendingCloudwatchLogsExports": PendingCloudwatchLogsExportsTypeDef,
     },
-    total=False,
 )
 
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
-    total=False,
 )
 
 TagListMessageTypeDef = TypedDict(
     "TagListMessageTypeDef",
     {
         "TagList": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
     "OrderableDBInstanceOptionsMessageTypeDef",
     {
         "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBSubnetGroupTypeDef = TypedDict(
     "DBSubnetGroupTypeDef",
     {
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
         "DBSubnetGroupArn": str,
     },
-    total=False,
 )
 
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBClusterSnapshotAttributeResultTypeDef = TypedDict(
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterResultTypeDef = TypedDict(
     "CreateDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterMessageTypeDef = TypedDict(
     "DBClusterMessageTypeDef",
     {
         "Marker": str,
         "DBClusters": List[DBClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBClusterResultTypeDef = TypedDict(
     "DeleteDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverDBClusterResultTypeDef = TypedDict(
     "FailoverDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBClusterResultTypeDef = TypedDict(
     "ModifyDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreDBClusterFromSnapshotResultTypeDef = TypedDict(
     "RestoreDBClusterFromSnapshotResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreDBClusterToPointInTimeResultTypeDef = TypedDict(
     "RestoreDBClusterToPointInTimeResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDBClusterResultTypeDef = TypedDict(
     "StartDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopDBClusterResultTypeDef = TypedDict(
     "StopDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBEngineVersionMessageTypeDef = TypedDict(
     "DBEngineVersionMessageTypeDef",
     {
         "Marker": str,
         "DBEngineVersions": List[DBEngineVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGlobalClusterResultTypeDef = TypedDict(
     "CreateGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGlobalClusterResultTypeDef = TypedDict(
     "DeleteGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalClustersMessageTypeDef = TypedDict(
     "GlobalClustersMessageTypeDef",
     {
         "Marker": str,
         "GlobalClusters": List[GlobalClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyGlobalClusterResultTypeDef = TypedDict(
     "ModifyGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveFromGlobalClusterResultTypeDef = TypedDict(
     "RemoveFromGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PendingMaintenanceActionsMessageTypeDef = TypedDict(
     "PendingMaintenanceActionsMessageTypeDef",
     {
         "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBSubnetGroupResultTypeDef = TypedDict(
     "CreateDBSubnetGroupResultTypeDef",
     {
         "DBSubnetGroup": DBSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBInstanceTypeDef = TypedDict(
     "DBInstanceTypeDef",
     {
         "DBInstanceIdentifier": str,
@@ -2115,67 +2086,66 @@
         "DbiResourceId": str,
         "CACertificateIdentifier": str,
         "CopyTagsToSnapshot": bool,
         "PromotionTier": int,
         "DBInstanceArn": str,
         "EnabledCloudwatchLogsExports": List[str],
     },
-    total=False,
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "DBSubnetGroups": List[DBSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBSubnetGroupResultTypeDef = TypedDict(
     "ModifyDBSubnetGroupResultTypeDef",
     {
         "DBSubnetGroup": DBSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBInstanceResultTypeDef = TypedDict(
     "CreateDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBInstanceMessageTypeDef = TypedDict(
     "DBInstanceMessageTypeDef",
     {
         "Marker": str,
         "DBInstances": List[DBInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBInstanceResultTypeDef = TypedDict(
     "DeleteDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBInstanceResultTypeDef = TypedDict(
     "ModifyDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootDBInstanceResultTypeDef = TypedDict(
     "RebootDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/type_defs.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -21,66 +21,66 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "CertificateTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "DBClusterParameterGroupTypeDef",
     "DBClusterSnapshotTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterMemberTypeDef",
     "ParameterOutputTypeDef",
-    "DBClusterParameterGroupNameMessageTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "EndpointTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     "DeleteDBClusterSnapshotMessageRequestTypeDef",
     "DeleteDBInstanceMessageRequestTypeDef",
     "DeleteDBSubnetGroupMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteGlobalClusterMessageRequestTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
     "ParameterTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
     "TagOutputTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
+    "DBClusterParameterGroupNameMessageTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopyDBClusterParameterGroupMessageRequestTypeDef",
     "CopyDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBClusterMessageRequestTypeDef",
@@ -103,43 +103,43 @@
     "DBClusterSnapshotMessageTypeDef",
     "DeleteDBClusterSnapshotResultTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBClusterTypeDef",
     "DBEngineVersionTypeDef",
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
-    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
-    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
-    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
-    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
     "DescribeDBClustersMessageRequestTypeDef",
-    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     "DescribeDBEngineVersionsMessageRequestTypeDef",
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     "DescribeDBInstancesMessageRequestTypeDef",
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultClusterParametersMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     "DescribeGlobalClustersMessageRequestTypeDef",
-    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
-    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
+    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
     "ModifyDBClusterParameterGroupMessageRequestTypeDef",
     "ResetDBClusterParameterGroupMessageRequestTypeDef",
@@ -197,15 +197,25 @@
         "SubscriptionCreationTime": str,
         "SourceType": str,
         "SourceIdsList": List[str],
         "EventCategoriesList": List[str],
         "Enabled": bool,
         "EventSubscriptionArn": str,
     },
-    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -223,28 +233,26 @@
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
-    total=False,
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateIdentifier": str,
         "CertificateType": str,
         "Thumbprint": str,
         "ValidFrom": datetime,
         "ValidTill": datetime,
         "CertificateArn": str,
     },
-    total=False,
 )
 
 CloudwatchLogsExportConfigurationTypeDef = TypedDict(
     "CloudwatchLogsExportConfigurationTypeDef",
     {
         "EnableLogTypes": Sequence[str],
         "DisableLogTypes": Sequence[str],
@@ -256,15 +264,14 @@
     "DBClusterParameterGroupTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBClusterParameterGroupArn": str,
     },
-    total=False,
 )
 
 DBClusterSnapshotTypeDef = TypedDict(
     "DBClusterSnapshotTypeDef",
     {
         "AvailabilityZones": List[str],
         "DBClusterSnapshotIdentifier": str,
@@ -280,15 +287,14 @@
         "SnapshotType": str,
         "PercentProgress": int,
         "StorageEncrypted": bool,
         "KmsKeyId": str,
         "DBClusterSnapshotArn": str,
         "SourceDBClusterSnapshotArn": str,
     },
-    total=False,
 )
 
 _RequiredCreateGlobalClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
     },
@@ -316,15 +322,14 @@
     "DBClusterMemberTypeDef",
     {
         "DBInstanceIdentifier": str,
         "IsClusterWriter": bool,
         "DBClusterParameterGroupStatus": str,
         "PromotionTier": int,
     },
-    total=False,
 )
 
 ParameterOutputTypeDef = TypedDict(
     "ParameterOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
@@ -333,83 +338,68 @@
         "ApplyType": str,
         "DataType": str,
         "AllowedValues": str,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ApplyMethod": ApplyMethodType,
     },
-    total=False,
-)
-
-DBClusterParameterGroupNameMessageTypeDef = TypedDict(
-    "DBClusterParameterGroupNameMessageTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
 )
 
 DBClusterRoleTypeDef = TypedDict(
     "DBClusterRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
     },
-    total=False,
 )
 
 DBClusterSnapshotAttributeTypeDef = TypedDict(
     "DBClusterSnapshotAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[str],
     },
-    total=False,
 )
 
 VpcSecurityGroupMembershipTypeDef = TypedDict(
     "VpcSecurityGroupMembershipTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
-    total=False,
 )
 
 UpgradeTargetTypeDef = TypedDict(
     "UpgradeTargetTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "Description": str,
         "AutoUpgrade": bool,
         "IsMajorVersionUpgrade": bool,
     },
-    total=False,
 )
 
 DBInstanceStatusInfoTypeDef = TypedDict(
     "DBInstanceStatusInfoTypeDef",
     {
         "StatusType": str,
         "Normal": bool,
         "Status": str,
         "Message": str,
     },
-    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "Port": int,
         "HostedZoneId": str,
     },
-    total=False,
 )
 
 _RequiredDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
@@ -474,14 +464,24 @@
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 DescribeDBClusterSnapshotAttributesMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
     },
 )
 
@@ -490,41 +490,32 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
-    total=False,
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "EventCategories": List[str],
         "Date": datetime,
         "SourceArn": str,
     },
-    total=False,
 )
 
 FailoverDBClusterMessageRequestTypeDef = TypedDict(
     "FailoverDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "TargetDBInstanceIdentifier": str,
@@ -535,15 +526,14 @@
 GlobalClusterMemberTypeDef = TypedDict(
     "GlobalClusterMemberTypeDef",
     {
         "DBClusterArn": str,
         "Readers": List[str],
         "IsWriter": bool,
     },
-    total=False,
 )
 
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
@@ -670,44 +660,32 @@
 
 class ModifyGlobalClusterMessageRequestTypeDef(
     _RequiredModifyGlobalClusterMessageRequestTypeDef,
     _OptionalModifyGlobalClusterMessageRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PendingCloudwatchLogsExportsTypeDef = TypedDict(
     "PendingCloudwatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": List[str],
         "LogTypesToDisable": List[str],
     },
-    total=False,
 )
 
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
         "CurrentApplyDate": datetime,
         "Description": str,
     },
-    total=False,
 )
 
 _RequiredRebootDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredRebootDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
@@ -745,25 +723,14 @@
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceName": str,
         "TagKeys": Sequence[str],
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
 StartDBClusterMessageRequestTypeDef = TypedDict(
     "StartDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
@@ -776,63 +743,77 @@
 
 TagOutputTypeDef = TypedDict(
     "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
-    total=False,
 )
 
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEventSubscriptionResultTypeDef = TypedDict(
     "CreateEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DBClusterParameterGroupNameMessageTypeDef = TypedDict(
+    "DBClusterParameterGroupNameMessageTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventSubscriptionResultTypeDef = TypedDict(
     "DeleteEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventSubscriptionsMessageTypeDef = TypedDict(
     "EventSubscriptionsMessageTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyEventSubscriptionResultTypeDef = TypedDict(
     "ModifyEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveSourceIdentifierFromSubscriptionResultTypeDef = TypedDict(
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
     {
         "ResourceName": str,
@@ -1111,33 +1092,31 @@
         "Engine": str,
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
         "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "Vpc": bool,
     },
-    total=False,
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
-    total=False,
 )
 
 CertificateMessageTypeDef = TypedDict(
     "CertificateMessageTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredModifyDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
@@ -1168,94 +1147,92 @@
 ):
     pass
 
 CopyDBClusterParameterGroupResultTypeDef = TypedDict(
     "CopyDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterParameterGroupResultTypeDef = TypedDict(
     "CreateDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupsMessageTypeDef = TypedDict(
     "DBClusterParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "DBClusterParameterGroups": List[DBClusterParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDBClusterSnapshotResultTypeDef = TypedDict(
     "CopyDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterSnapshotResultTypeDef = TypedDict(
     "CreateDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterSnapshotMessageTypeDef = TypedDict(
     "DBClusterSnapshotMessageTypeDef",
     {
         "Marker": str,
         "DBClusterSnapshots": List[DBClusterSnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBClusterSnapshotResultTypeDef = TypedDict(
     "DeleteDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
         "Parameters": List[ParameterOutputTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
         "Marker": str,
         "Parameters": List[ParameterOutputTypeDef],
     },
-    total=False,
 )
 
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
-    total=False,
 )
 
 DBClusterTypeDef = TypedDict(
     "DBClusterTypeDef",
     {
         "AvailabilityZones": List[str],
         "BackupRetentionPeriod": int,
@@ -1286,96 +1263,52 @@
         "DBClusterArn": str,
         "AssociatedRoles": List[DBClusterRoleTypeDef],
         "CloneGroupId": str,
         "ClusterCreateTime": datetime,
         "EnabledCloudwatchLogsExports": List[str],
         "DeletionProtection": bool,
     },
-    total=False,
 )
 
 DBEngineVersionTypeDef = TypedDict(
     "DBEngineVersionTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "DBEngineDescription": str,
         "DBEngineVersionDescription": str,
         "ValidUpgradeTarget": List[UpgradeTargetTypeDef],
         "ExportableLogTypes": List[str],
         "SupportsLogExportsToCloudwatchLogs": bool,
     },
-    total=False,
-)
-
-DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
-    {
-        "CertificateIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
 )
 
 DescribeCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeCertificatesMessageRequestTypeDef",
     {
         "CertificateIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
-    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
-    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeDBClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDBClusterParametersMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
     },
 )
 _OptionalDescribeDBClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1391,28 +1324,14 @@
 
 class DescribeDBClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDBClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDBClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "DBClusterSnapshotIdentifier": str,
-        "SnapshotType": str,
-        "Filters": Sequence[FilterTypeDef],
-        "IncludeShared": bool,
-        "IncludePublic": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1420,50 +1339,25 @@
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
     },
     total=False,
 )
 
-DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
-    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClustersMessageRequestTypeDef = TypedDict(
     "DescribeDBClustersMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
-    {
-        "Engine": str,
-        "EngineVersion": str,
-        "DBParameterGroupFamily": str,
-        "Filters": Sequence[FilterTypeDef],
-        "DefaultOnly": bool,
-        "ListSupportedCharacterSets": bool,
-        "ListSupportedTimezones": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBEngineVersionsMessageRequestTypeDef = TypedDict(
     "DescribeDBEngineVersionsMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "Filters": Sequence[FilterTypeDef],
@@ -1472,45 +1366,25 @@
         "DefaultOnly": bool,
         "ListSupportedCharacterSets": bool,
         "ListSupportedTimezones": bool,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
-    {
-        "DBInstanceIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBInstancesMessageRequestTypeDef = TypedDict(
     "DescribeDBInstancesMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
-    {
-        "DBSubnetGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -1545,50 +1419,25 @@
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -1597,60 +1446,25 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
-    {
-        "GlobalClusterIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
     "DescribeGlobalClustersMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
-    {
-        "Engine": str,
-    },
-)
-_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
-    {
-        "EngineVersion": str,
-        "DBInstanceClass": str,
-        "LicenseModel": str,
-        "Vpc": bool,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
-    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
-    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     {
         "Engine": str,
     },
 )
 _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
@@ -1669,26 +1483,14 @@
 
 class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
     _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
     _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
 ):
     pass
 
-DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
-    TypedDict(
-        "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
-        {
-            "ResourceIdentifier": str,
-            "Filters": Sequence[FilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
@@ -1712,14 +1514,187 @@
 
 class ListTagsForResourceMessageRequestTypeDef(
     _RequiredListTagsForResourceMessageRequestTypeDef,
     _OptionalListTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
+DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+    {
+        "CertificateIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
+    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+):
+    pass
+
+DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "DBClusterSnapshotIdentifier": str,
+        "SnapshotType": str,
+        "Filters": Sequence[FilterTypeDef],
+        "IncludeShared": bool,
+        "IncludePublic": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
+    {
+        "Engine": str,
+        "EngineVersion": str,
+        "DBParameterGroupFamily": str,
+        "Filters": Sequence[FilterTypeDef],
+        "DefaultOnly": bool,
+        "ListSupportedCharacterSets": bool,
+        "ListSupportedTimezones": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+    {
+        "DBInstanceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
+    {
+        "DBSubnetGroupName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
+    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    {
+        "GlobalClusterIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    {
+        "Engine": str,
+    },
+)
+_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    {
+        "EngineVersion": str,
+        "DBInstanceClass": str,
+        "LicenseModel": str,
+        "Vpc": bool,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
+    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+):
+    pass
+
+DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
+    TypedDict(
+        "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
+        {
+            "ResourceIdentifier": str,
+            "Filters": Sequence[FilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
 DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef = TypedDict(
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     {
         "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -1740,24 +1715,24 @@
     total=False,
 )
 
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventsMessageTypeDef = TypedDict(
     "EventsMessageTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalClusterTypeDef = TypedDict(
     "GlobalClusterTypeDef",
     {
         "GlobalClusterIdentifier": str,
@@ -1767,15 +1742,14 @@
         "Engine": str,
         "EngineVersion": str,
         "DatabaseName": str,
         "StorageEncrypted": bool,
         "DeletionProtection": bool,
         "GlobalClusterMembers": List[GlobalClusterMemberTypeDef],
     },
-    total=False,
 )
 
 ModifyDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "ModifyDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "Parameters": Sequence[ParameterTypeDef],
@@ -1817,225 +1791,222 @@
         "Iops": int,
         "DBInstanceIdentifier": str,
         "StorageType": str,
         "CACertificateIdentifier": str,
         "DBSubnetGroupName": str,
         "PendingCloudwatchLogsExports": PendingCloudwatchLogsExportsTypeDef,
     },
-    total=False,
 )
 
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
-    total=False,
 )
 
 TagListMessageTypeDef = TypedDict(
     "TagListMessageTypeDef",
     {
         "TagList": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
     "OrderableDBInstanceOptionsMessageTypeDef",
     {
         "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBSubnetGroupTypeDef = TypedDict(
     "DBSubnetGroupTypeDef",
     {
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
         "DBSubnetGroupArn": str,
     },
-    total=False,
 )
 
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBClusterSnapshotAttributeResultTypeDef = TypedDict(
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterResultTypeDef = TypedDict(
     "CreateDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterMessageTypeDef = TypedDict(
     "DBClusterMessageTypeDef",
     {
         "Marker": str,
         "DBClusters": List[DBClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBClusterResultTypeDef = TypedDict(
     "DeleteDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverDBClusterResultTypeDef = TypedDict(
     "FailoverDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBClusterResultTypeDef = TypedDict(
     "ModifyDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreDBClusterFromSnapshotResultTypeDef = TypedDict(
     "RestoreDBClusterFromSnapshotResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreDBClusterToPointInTimeResultTypeDef = TypedDict(
     "RestoreDBClusterToPointInTimeResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDBClusterResultTypeDef = TypedDict(
     "StartDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopDBClusterResultTypeDef = TypedDict(
     "StopDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBEngineVersionMessageTypeDef = TypedDict(
     "DBEngineVersionMessageTypeDef",
     {
         "Marker": str,
         "DBEngineVersions": List[DBEngineVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGlobalClusterResultTypeDef = TypedDict(
     "CreateGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGlobalClusterResultTypeDef = TypedDict(
     "DeleteGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalClustersMessageTypeDef = TypedDict(
     "GlobalClustersMessageTypeDef",
     {
         "Marker": str,
         "GlobalClusters": List[GlobalClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyGlobalClusterResultTypeDef = TypedDict(
     "ModifyGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveFromGlobalClusterResultTypeDef = TypedDict(
     "RemoveFromGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PendingMaintenanceActionsMessageTypeDef = TypedDict(
     "PendingMaintenanceActionsMessageTypeDef",
     {
         "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBSubnetGroupResultTypeDef = TypedDict(
     "CreateDBSubnetGroupResultTypeDef",
     {
         "DBSubnetGroup": DBSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBInstanceTypeDef = TypedDict(
     "DBInstanceTypeDef",
     {
         "DBInstanceIdentifier": str,
@@ -2062,67 +2033,66 @@
         "DbiResourceId": str,
         "CACertificateIdentifier": str,
         "CopyTagsToSnapshot": bool,
         "PromotionTier": int,
         "DBInstanceArn": str,
         "EnabledCloudwatchLogsExports": List[str],
     },
-    total=False,
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "DBSubnetGroups": List[DBSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBSubnetGroupResultTypeDef = TypedDict(
     "ModifyDBSubnetGroupResultTypeDef",
     {
         "DBSubnetGroup": DBSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBInstanceResultTypeDef = TypedDict(
     "CreateDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBInstanceMessageTypeDef = TypedDict(
     "DBInstanceMessageTypeDef",
     {
         "Marker": str,
         "DBInstances": List[DBInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBInstanceResultTypeDef = TypedDict(
     "DeleteDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBInstanceResultTypeDef = TypedDict(
     "ModifyDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootDBInstanceResultTypeDef = TypedDict(
     "RebootDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/waiter.py` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb/waiter.pyi` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb.egg-info/PKG-INFO` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb
-Version: 1.28.12
-Summary: Type annotations for boto3.DocDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.4
+Summary: Type annotations for boto3.DocDB 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-docdb"></a>
 
 # mypy-boto3-docdb
 
 [![PyPI - mypy-boto3-docdb](https://img.shields.io/pypi/v/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb)](https://pepy.tech/project/mypy-boto3-docdb)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-docdb?color=blue)](https://pypistats.org/packages/mypy-boto3-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[boto3.DocDB 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-docdb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,66 +408,66 @@
 `mypy_boto3_docdb.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_docdb.type_defs import (
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     CertificateTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterMemberTypeDef,
     ParameterOutputTypeDef,
-    DBClusterParameterGroupNameMessageTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     EndpointTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ParameterTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     PendingMaintenanceActionTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
     TagOutputTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
+    DBClusterParameterGroupNameMessageTypeDef,
     DeleteEventSubscriptionResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopyDBClusterParameterGroupMessageRequestTypeDef,
     CopyDBClusterSnapshotMessageRequestTypeDef,
     CreateDBClusterMessageRequestTypeDef,
@@ -490,43 +490,43 @@
     DBClusterSnapshotMessageTypeDef,
     DeleteDBClusterSnapshotResultTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBClusterTypeDef,
     DBEngineVersionTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
-    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
-    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
-    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
-    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
-    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
-    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBInstancesMessageRequestTypeDef,
-    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
-    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
-    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
+    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
+    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
+    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
+    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
+    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
+    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
+    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
     ModifyDBClusterParameterGroupMessageRequestTypeDef,
     ResetDBClusterParameterGroupMessageRequestTypeDef,
```

### Comparing `mypy-boto3-docdb-1.28.12/mypy_boto3_docdb.egg-info/SOURCES.txt` & `mypy-boto3-docdb-1.28.4/mypy_boto3_docdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-1.28.12/setup.py` & `mypy-boto3-docdb-1.28.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-docdb",
-    version="1.28.12",
+    version="1.28.4",
     packages=["mypy_boto3_docdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DocDB 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.DocDB 1.28.4 service generated with mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

