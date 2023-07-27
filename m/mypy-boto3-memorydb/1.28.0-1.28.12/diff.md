# Comparing `tmp/mypy-boto3-memorydb-1.28.0.tar.gz` & `tmp/mypy-boto3-memorydb-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-memorydb-1.28.0.tar", last modified: Thu Jul  6 21:00:08 2023, max compression
+gzip compressed data, was "mypy-boto3-memorydb-1.28.12.tar", last modified: Thu Jul 27 05:35:02 2023, max compression
```

## Comparing `mypy-boto3-memorydb-1.28.0.tar` & `mypy-boto3-memorydb-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.102371 mypy-boto3-memorydb-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:30.000000 mypy-boto3-memorydb-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-07-06 21:00:08.102371 mypy-boto3-memorydb-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-07-06 20:47:30.000000 mypy-boto3-memorydb-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.098371 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-06 20:47:30.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-06 20:47:30.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:47:30.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36305 2023-07-06 20:47:31.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36248 2023-07-06 20:47:30.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-07-06 20:47:31.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-07-06 20:47:31.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-07-06 20:47:31.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-07-06 20:47:31.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:30.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41450 2023-07-06 20:47:32.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41415 2023-07-06 20:47:32.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:30.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:08.102371 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-07-06 21:00:07.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 21:00:07.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:07.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:07.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:07.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:07.000000 mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:08.102371 mypy-boto3-memorydb-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:47:30.000000 mypy-boto3-memorydb-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.372436 mypy-boto3-memorydb-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:31.000000 mypy-boto3-memorydb-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19669 2023-07-27 05:35:02.364436 mypy-boto3-memorydb-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18178 2023-07-27 05:26:31.000000 mypy-boto3-memorydb-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.364436 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-27 05:26:31.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-27 05:26:31.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 05:26:31.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36305 2023-07-27 05:26:31.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36248 2023-07-27 05:26:31.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-27 05:26:32.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-27 05:26:32.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-07-27 05:26:31.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-07-27 05:26:31.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:31.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41621 2023-07-27 05:26:32.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-07-27 05:26:32.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:31.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.364436 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19669 2023-07-27 05:35:02.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:35:02.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:02.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:35:02.000000 mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:02.372436 mypy-boto3-memorydb-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:26:31.000000 mypy-boto3-memorydb-1.28.12/setup.py
```

### Comparing `mypy-boto3-memorydb-1.28.0/LICENSE` & `mypy-boto3-memorydb-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.0/PKG-INFO` & `mypy-boto3-memorydb-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-memorydb
-Version: 1.28.0
-Summary: Type annotations for boto3.MemoryDB 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MemoryDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-memorydb"></a>
 
 # mypy-boto3-memorydb
 
 [![PyPI - mypy-boto3-memorydb](https://img.shields.io/pypi/v/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-memorydb?color=blue)](https://pypistats.org/packages/mypy-boto3-memorydb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-memorydb)](https://pepy.tech/project/mypy-boto3-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MemoryDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[boto3.MemoryDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
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
 [mypy-boto3-memorydb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -425,14 +425,15 @@
     DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     FilterTypeDef,
     FailoverShardRequestRequestTypeDef,
     ListAllowedNodeTypeUpdatesRequestRequestTypeDef,
     ListAllowedNodeTypeUpdatesResponseTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RecurringChargeTypeDef,
     ReplicaConfigurationRequestTypeDef,
     ResetParameterGroupRequestRequestTypeDef,
     SlotMigrationTypeDef,
     ResponseMetadataTypeDef,
@@ -450,30 +451,30 @@
     CopySnapshotRequestRequestTypeDef,
     CreateACLRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     PurchaseReservedNodesOfferingRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagResourceResponseTypeDef,
-    UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DeleteParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     ResetParameterGroupResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     DescribeEngineVersionsResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
+    TagResourceResponseTypeDef,
+    UntagResourceResponseTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     ReservedNodeTypeDef,
     ReservedNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     UpdateClusterRequestRequestTypeDef,
     ShardDetailTypeDef,
     CreateACLResponseTypeDef,
```

### Comparing `mypy-boto3-memorydb-1.28.0/README.md` & `mypy-boto3-memorydb-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-memorydb"></a>
 
 # mypy-boto3-memorydb
 
 [![PyPI - mypy-boto3-memorydb](https://img.shields.io/pypi/v/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-memorydb?color=blue)](https://pypistats.org/packages/mypy-boto3-memorydb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-memorydb)](https://pepy.tech/project/mypy-boto3-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MemoryDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[boto3.MemoryDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
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
 [mypy-boto3-memorydb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,14 +393,15 @@
     DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     FilterTypeDef,
     FailoverShardRequestRequestTypeDef,
     ListAllowedNodeTypeUpdatesRequestRequestTypeDef,
     ListAllowedNodeTypeUpdatesResponseTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RecurringChargeTypeDef,
     ReplicaConfigurationRequestTypeDef,
     ResetParameterGroupRequestRequestTypeDef,
     SlotMigrationTypeDef,
     ResponseMetadataTypeDef,
@@ -418,30 +419,30 @@
     CopySnapshotRequestRequestTypeDef,
     CreateACLRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     PurchaseReservedNodesOfferingRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagResourceResponseTypeDef,
-    UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DeleteParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     ResetParameterGroupResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     DescribeEngineVersionsResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
+    TagResourceResponseTypeDef,
+    UntagResourceResponseTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     ReservedNodeTypeDef,
     ReservedNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     UpdateClusterRequestRequestTypeDef,
     ShardDetailTypeDef,
     CreateACLResponseTypeDef,
```

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/__init__.py` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/__init__.pyi` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/__main__.py` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MemoryDB 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.MemoryDB 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB\nOther"
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

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/client.py` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/client.pyi` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/literals.py` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
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
@@ -268,26 +269,28 @@
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

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/literals.pyi` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,15 @@
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
@@ -266,26 +267,28 @@
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

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/paginator.py` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/paginator.pyi` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/type_defs.py` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeSubnetGroupsRequestRequestTypeDef",
     "FilterTypeDef",
     "FailoverShardRequestRequestTypeDef",
     "ListAllowedNodeTypeUpdatesRequestRequestTypeDef",
     "ListAllowedNodeTypeUpdatesResponseTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ParameterNameValueTypeDef",
     "RecurringChargeTypeDef",
     "ReplicaConfigurationRequestTypeDef",
     "ResetParameterGroupRequestRequestTypeDef",
     "SlotMigrationTypeDef",
     "ResponseMetadataTypeDef",
@@ -105,30 +106,30 @@
     "CopySnapshotRequestRequestTypeDef",
     "CreateACLRequestRequestTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "CreateParameterGroupRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateSubnetGroupRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
     "PurchaseReservedNodesOfferingRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagResourceResponseTypeDef",
-    "UntagResourceResponseTypeDef",
     "CreateParameterGroupResponseTypeDef",
     "DeleteParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "ResetParameterGroupResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
     "DescribeEngineVersionsResponseTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeParametersResponseTypeDef",
     "DescribeServiceUpdatesResponseTypeDef",
     "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
+    "TagResourceResponseTypeDef",
+    "UntagResourceResponseTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
     "ReservedNodeTypeDef",
     "ReservedNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "ShardDetailTypeDef",
     "CreateACLResponseTypeDef",
@@ -685,14 +686,23 @@
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1105,22 +1115,14 @@
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPurchaseReservedNodesOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedNodesOfferingRequestRequestTypeDef",
     {
         "ReservedNodesOfferingId": str,
     },
 )
 _OptionalPurchaseReservedNodesOfferingRequestRequestTypeDef = TypedDict(
@@ -1145,30 +1147,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-TagResourceResponseTypeDef = TypedDict(
-    "TagResourceResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UntagResourceResponseTypeDef = TypedDict(
-    "UntagResourceResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateParameterGroupResponseTypeDef = TypedDict(
     "CreateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1259,14 +1245,38 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TagResourceResponseTypeDef = TypedDict(
+    "TagResourceResponseTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UntagResourceResponseTypeDef = TypedDict(
+    "UntagResourceResponseTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateParameterGroupRequestRequestTypeDef = TypedDict(
     "UpdateParameterGroupRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
         "ParameterNameValues": Sequence[ParameterNameValueTypeDef],
     },
 )
```

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb/type_defs.pyi` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeSubnetGroupsRequestRequestTypeDef",
     "FilterTypeDef",
     "FailoverShardRequestRequestTypeDef",
     "ListAllowedNodeTypeUpdatesRequestRequestTypeDef",
     "ListAllowedNodeTypeUpdatesResponseTypeDef",
     "ListTagsRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ParameterNameValueTypeDef",
     "RecurringChargeTypeDef",
     "ReplicaConfigurationRequestTypeDef",
     "ResetParameterGroupRequestRequestTypeDef",
     "SlotMigrationTypeDef",
     "ResponseMetadataTypeDef",
@@ -104,30 +105,30 @@
     "CopySnapshotRequestRequestTypeDef",
     "CreateACLRequestRequestTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "CreateParameterGroupRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateSubnetGroupRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
     "PurchaseReservedNodesOfferingRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TagResourceResponseTypeDef",
-    "UntagResourceResponseTypeDef",
     "CreateParameterGroupResponseTypeDef",
     "DeleteParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "ResetParameterGroupResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
     "DescribeEngineVersionsResponseTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeParametersResponseTypeDef",
     "DescribeServiceUpdatesResponseTypeDef",
     "DescribeUsersRequestDescribeUsersPaginateTypeDef",
     "DescribeUsersRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
+    "TagResourceResponseTypeDef",
+    "UntagResourceResponseTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
     "ReservedNodeTypeDef",
     "ReservedNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "ShardDetailTypeDef",
     "CreateACLResponseTypeDef",
@@ -678,14 +679,23 @@
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
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
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1074,22 +1084,14 @@
 )
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPurchaseReservedNodesOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedNodesOfferingRequestRequestTypeDef",
     {
         "ReservedNodesOfferingId": str,
     },
 )
 _OptionalPurchaseReservedNodesOfferingRequestRequestTypeDef = TypedDict(
@@ -1112,30 +1114,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-TagResourceResponseTypeDef = TypedDict(
-    "TagResourceResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UntagResourceResponseTypeDef = TypedDict(
-    "UntagResourceResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateParameterGroupResponseTypeDef = TypedDict(
     "CreateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1226,14 +1212,38 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TagResourceResponseTypeDef = TypedDict(
+    "TagResourceResponseTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UntagResourceResponseTypeDef = TypedDict(
+    "UntagResourceResponseTypeDef",
+    {
+        "TagList": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateParameterGroupRequestRequestTypeDef = TypedDict(
     "UpdateParameterGroupRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
         "ParameterNameValues": Sequence[ParameterNameValueTypeDef],
     },
 )
```

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb.egg-info/PKG-INFO` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-memorydb
-Version: 1.28.0
-Summary: Type annotations for boto3.MemoryDB 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MemoryDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-memorydb"></a>
 
 # mypy-boto3-memorydb
 
 [![PyPI - mypy-boto3-memorydb](https://img.shields.io/pypi/v/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-memorydb.svg?color=blue)](https://pypi.org/project/mypy-boto3-memorydb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-memorydb?color=blue)](https://pypistats.org/packages/mypy-boto3-memorydb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-memorydb)](https://pepy.tech/project/mypy-boto3-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MemoryDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[boto3.MemoryDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
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
 [mypy-boto3-memorydb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_memorydb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -425,14 +425,15 @@
     DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     FilterTypeDef,
     FailoverShardRequestRequestTypeDef,
     ListAllowedNodeTypeUpdatesRequestRequestTypeDef,
     ListAllowedNodeTypeUpdatesResponseTypeDef,
     ListTagsRequestRequestTypeDef,
+    TagOutputTypeDef,
     PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RecurringChargeTypeDef,
     ReplicaConfigurationRequestTypeDef,
     ResetParameterGroupRequestRequestTypeDef,
     SlotMigrationTypeDef,
     ResponseMetadataTypeDef,
@@ -450,30 +451,30 @@
     CopySnapshotRequestRequestTypeDef,
     CreateACLRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     PurchaseReservedNodesOfferingRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    TagResourceResponseTypeDef,
-    UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DeleteParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     ResetParameterGroupResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
     DescribeEngineVersionsResponseTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeParametersResponseTypeDef,
     DescribeServiceUpdatesResponseTypeDef,
     DescribeUsersRequestDescribeUsersPaginateTypeDef,
     DescribeUsersRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
+    TagResourceResponseTypeDef,
+    UntagResourceResponseTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     ReservedNodeTypeDef,
     ReservedNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     UpdateClusterRequestRequestTypeDef,
     ShardDetailTypeDef,
     CreateACLResponseTypeDef,
```

### Comparing `mypy-boto3-memorydb-1.28.0/mypy_boto3_memorydb.egg-info/SOURCES.txt` & `mypy-boto3-memorydb-1.28.12/mypy_boto3_memorydb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-memorydb-1.28.0/setup.py` & `mypy-boto3-memorydb-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-memorydb",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_memorydb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MemoryDB 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.MemoryDB 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

