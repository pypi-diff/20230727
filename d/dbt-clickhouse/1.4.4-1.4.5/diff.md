# Comparing `tmp/dbt-clickhouse-1.4.4.tar.gz` & `tmp/dbt-clickhouse-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickhouse-1.4.4.tar", last modified: Wed Jul 19 23:40:40 2023, max compression
+gzip compressed data, was "dbt-clickhouse-1.4.5.tar", last modified: Thu Jul 27 11:54:54 2023, max compression
```

## Comparing `dbt-clickhouse-1.4.4.tar` & `dbt-clickhouse-1.4.5.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:40.439318 dbt-clickhouse-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-19 23:40:40.439318 dbt-clickhouse-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:40.435318 dbt-clickhouse-1.4.4/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:40.431318 dbt-clickhouse-1.4.4/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:40.435318 dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/dbclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    15208 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/nativeclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:40.435318 dbt-clickhouse-1.4.4/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:40.435318 dbt-clickhouse-1.4.4/dbt/include/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:40.435318 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:40.435318 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:40.439318 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/distributed_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/s3.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/view.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/persist_docs.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:40.439318 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/schema_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/schema_tests/relationships.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:40.439318 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/utils/utils.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:40:40.439318 dbt-clickhouse-1.4.4/dbt_clickhouse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-19 23:40:40.000000 dbt-clickhouse-1.4.4/dbt_clickhouse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-19 23:40:40.000000 dbt-clickhouse-1.4.4/dbt_clickhouse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 23:40:40.000000 dbt-clickhouse-1.4.4/dbt_clickhouse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-19 23:40:40.000000 dbt-clickhouse-1.4.4/dbt_clickhouse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-19 23:40:40.000000 dbt-clickhouse-1.4.4/dbt_clickhouse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 23:40:40.439318 dbt-clickhouse-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-19 23:40:37.000000 dbt-clickhouse-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:54.881857 dbt-clickhouse-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-07-27 11:54:54.881857 dbt-clickhouse-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17848 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:54.877857 dbt-clickhouse-1.4.5/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:54.877857 dbt-clickhouse-1.4.5/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:54.881857 dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/dbclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15208 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/nativeclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:54.877857 dbt-clickhouse-1.4.5/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:54.881857 dbt-clickhouse-1.4.5/dbt/include/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:54.881857 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:54.881857 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:54.881857 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/distributed_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/distributed_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/s3.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/persist_docs.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:54.881857 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/schema_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/schema_tests/relationships.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:54.881857 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/utils/utils.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:54:54.881857 dbt-clickhouse-1.4.5/dbt_clickhouse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-07-27 11:54:54.000000 dbt-clickhouse-1.4.5/dbt_clickhouse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-27 11:54:54.000000 dbt-clickhouse-1.4.5/dbt_clickhouse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:54:54.000000 dbt-clickhouse-1.4.5/dbt_clickhouse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 11:54:54.000000 dbt-clickhouse-1.4.5/dbt_clickhouse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 11:54:54.000000 dbt-clickhouse-1.4.5/dbt_clickhouse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:54:54.881857 dbt-clickhouse-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-27 11:54:51.000000 dbt-clickhouse-1.4.5/setup.py
```

### Comparing `dbt-clickhouse-1.4.4/LICENSE` & `dbt-clickhouse-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/PKG-INFO` & `dbt-clickhouse-1.4.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: dbt-clickhouse
-Version: 1.4.4
-Summary: The Clickhouse plugin for dbt (data build tool)
-Home-page: https://github.com/ClickHouse/dbt-clickhouse
-Author: ClickHouse Inc.
-Author-email: guy@clickhouse.com
-License: MIT
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <img src="https://raw.githubusercontent.com/ClickHouse/dbt-clickhouse/master/etc/chdbt.png" alt="clickhouse dbt logo" width="300"/>
 </p>
 
 # dbt-clickhouse
 
 This plugin ports [dbt](https://getdbt.com) functionality to [Clickhouse](https://clickhouse.tech/).
@@ -48,14 +25,16 @@
 - [x] Seeds
 - [x] Sources
 - [x] Docs generate
 - [x] Tests
 - [x] Snapshots
 - [x] Most dbt-utils macros (now included in dbt-core)  
 - [x] Ephemeral materialization
+- [x] Distributed table materialization (experimental)
+- [x] Distributed incremental materialization (experimental)
 
 # Usage Notes
 
 ## Database
 
 The dbt model relation identifier `database.schema.table` is not compatible with Clickhouse because Clickhouse does not support a `schema`.
 So we use a simplified approach `schema.table`, where `schema` is the Clickhouse database. Using the `default` database is not recommended.
@@ -84,14 +63,15 @@
       retries: [1] # Number of times to retry a "retriable" database exception (such as a 503 'Service Unavailable' error)
       compression: [<empty string>] Use gzip compression if truthy (http), or compression type for a native connection
       connect_timeout: [10] # Timeout in seconds to establish a connection to ClickHouse
       send_receive_timeout: [300] # Timeout in seconds to receive data from the ClickHouse server
       cluster_mode: [False] # Use specific settings designed to improve operation on Replicated databases (recommended for ClickHouse Cloud)
       use_lw_deletes: [False] Use the strategy `delete+insert` as the default incremental strategy.
       check_exchange: [True] # Validate that clickhouse support the atomic EXCHANGE TABLES command.  (Not needed for most ClickHouse versions)
+      local_suffix [local] # Table suffix of local tables on shards for distributed materializations 
       custom_settings: [{}] # A dicitonary/mapping of custom ClickHouse settings for the connection - default is empty.
       
       # Native (clickhouse-driver) connection settings
       sync_request_timeout: [5] Timeout for server ping
       compress_block_size: [1048576] Compression block size if compression is enabled
       
 ```
@@ -172,14 +152,115 @@
 | structure             | The column structure of the data in bucket, as a list of name/datatype pairs, such as `['id UInt32', 'date DateTime', 'value String']`  If not provided ClickHouse will infer the structure. |
 | aws_access_key_id     | The S3 access key id.                                                                                                                                                                        |
 | aws_secret_access_key | The S3 secrete key.                                                                                                                                                                          |
 | compression           | The compression method used with the S3 objects.  If not provided ClickHouse will attempt to determine compression based on the file name.                                                   |
 
 See the [S3 test file](https://github.com/ClickHouse/dbt-clickhouse/blob/main/tests/integration/adapter/test_s3.py) for examples of how to use this macro.
 
+# Distributed materializations
+
+Note:  Distributed materializations experimental and are not currently included in the automated test suite.
+
+WARNING: 
+
+To use distributed materializations correctly you should set **insert_distributed_sync** = 1 (or use as prehook) in order to have correct data while SELECT queries. Otherwise, downstream operations could produce invalid results
+if the distributed insert has not completed before additional updates are executed.
+
+## Distributed table materialization
+
+Distributed table created with following steps:
+1. Creates temp view with sql query to get right structure
+2. Create empty local tables based on view 
+3. Create distributed table based on local tables. 
+4. Data inserts into distributed table, so it is distributed across shards without duplicating.
+
+### Distributed table model example
+```sql
+{{
+    config(
+        materialized='distributed_table',
+        order_by='id, created_at',
+        sharding_key='cityHash64(id)',
+        engine='ReplacingMergeTree'
+    )
+}}
+
+select id, created_at, item from {{ source('db', 'table') }}
+```
+
+### Generated migrations
+
+```sql
+CREATE TABLE db.table_local on cluster cluster
+(
+    `id` UInt64,
+    `created_at` DateTime,
+    `item` String
+)
+ENGINE = ReplacingMergeTree
+ORDER BY (id, created_at)
+SETTINGS index_granularity = 8192;
+
+
+CREATE TABLE db.table on cluster cluster
+(
+    `id` UInt64,
+    `created_at` DateTime,
+    `item` String
+)
+ENGINE = Distributed('cluster', 'db', 'table_local', cityHash64(id));
+```
+
+## Distributed incremental materialization
+
+Incremental model based on the same idea as distributed table, the main difficulty is to process all incremental strategies correctly.
+
+1. _The Append Strategy_ just insert data into distributed table.
+2. _The Delete+Insert_ Strategy creates distributed temp table to work with all data on every shard.
+3. _The Default (Legacy) Strategy_ creates distributed temp and intermediate tables for the same reason.
+
+Only shard tables are replacing, because distributed table does not keep data. 
+The distributed table reloads only when the full_refresh mode is enabled or the table structure may have changed.
+
+### Distributed incremental model example
+```sql
+{{
+    config(
+        materialized='distributed_incremental',
+        engine='MergeTree',
+        incremental_strategy='append',
+        unique_key='id,created_at'
+    )
+}}
+
+select id, created_at, item from {{ source('db', 'table') }}
+```
+
+### Generated migrations
+
+```sql
+CREATE TABLE db.table_local on cluster cluster
+(
+    `id` UInt64,
+    `created_at` DateTime,
+    `item` String
+)
+ENGINE = MergeTree
+SETTINGS index_granularity = 8192;
+
+
+CREATE TABLE db.table on cluster cluster
+(
+    `id` UInt64,
+    `created_at` DateTime,
+    `item` String
+)
+ENGINE = Distributed('cluster', 'db', 'table_local', cityHash64(id));
+```
+
 # Running Tests
 
 This adapter passes all of dbt basic tests as presented in dbt's official docs: https://docs.getdbt.com/docs/contributing/testing-a-new-adapter#testing-your-adapter.
 Use `pytest tests` to run tests.
 
 You can customize the test environment via environment variables. We recommend doing so with the pytest `pytest-dotenv` plugin combined with root level `test.env`
 configuration file (this file should not be checked into git).  The following environment variables are recognized:
```

### Comparing `dbt-clickhouse-1.4.4/README.md` & `dbt-clickhouse-1.4.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: dbt-clickhouse
+Version: 1.4.5
+Summary: The Clickhouse plugin for dbt (data build tool)
+Home-page: https://github.com/ClickHouse/dbt-clickhouse
+Author: ClickHouse Inc.
+Author-email: guy@clickhouse.com
+License: MIT
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <img src="https://raw.githubusercontent.com/ClickHouse/dbt-clickhouse/master/etc/chdbt.png" alt="clickhouse dbt logo" width="300"/>
 </p>
 
 # dbt-clickhouse
 
 This plugin ports [dbt](https://getdbt.com) functionality to [Clickhouse](https://clickhouse.tech/).
@@ -25,14 +48,16 @@
 - [x] Seeds
 - [x] Sources
 - [x] Docs generate
 - [x] Tests
 - [x] Snapshots
 - [x] Most dbt-utils macros (now included in dbt-core)  
 - [x] Ephemeral materialization
+- [x] Distributed table materialization (experimental)
+- [x] Distributed incremental materialization (experimental)
 
 # Usage Notes
 
 ## Database
 
 The dbt model relation identifier `database.schema.table` is not compatible with Clickhouse because Clickhouse does not support a `schema`.
 So we use a simplified approach `schema.table`, where `schema` is the Clickhouse database. Using the `default` database is not recommended.
@@ -61,14 +86,15 @@
       retries: [1] # Number of times to retry a "retriable" database exception (such as a 503 'Service Unavailable' error)
       compression: [<empty string>] Use gzip compression if truthy (http), or compression type for a native connection
       connect_timeout: [10] # Timeout in seconds to establish a connection to ClickHouse
       send_receive_timeout: [300] # Timeout in seconds to receive data from the ClickHouse server
       cluster_mode: [False] # Use specific settings designed to improve operation on Replicated databases (recommended for ClickHouse Cloud)
       use_lw_deletes: [False] Use the strategy `delete+insert` as the default incremental strategy.
       check_exchange: [True] # Validate that clickhouse support the atomic EXCHANGE TABLES command.  (Not needed for most ClickHouse versions)
+      local_suffix [local] # Table suffix of local tables on shards for distributed materializations 
       custom_settings: [{}] # A dicitonary/mapping of custom ClickHouse settings for the connection - default is empty.
       
       # Native (clickhouse-driver) connection settings
       sync_request_timeout: [5] Timeout for server ping
       compress_block_size: [1048576] Compression block size if compression is enabled
       
 ```
@@ -149,14 +175,115 @@
 | structure             | The column structure of the data in bucket, as a list of name/datatype pairs, such as `['id UInt32', 'date DateTime', 'value String']`  If not provided ClickHouse will infer the structure. |
 | aws_access_key_id     | The S3 access key id.                                                                                                                                                                        |
 | aws_secret_access_key | The S3 secrete key.                                                                                                                                                                          |
 | compression           | The compression method used with the S3 objects.  If not provided ClickHouse will attempt to determine compression based on the file name.                                                   |
 
 See the [S3 test file](https://github.com/ClickHouse/dbt-clickhouse/blob/main/tests/integration/adapter/test_s3.py) for examples of how to use this macro.
 
+# Distributed materializations
+
+Note:  Distributed materializations experimental and are not currently included in the automated test suite.
+
+WARNING: 
+
+To use distributed materializations correctly you should set **insert_distributed_sync** = 1 (or use as prehook) in order to have correct data while SELECT queries. Otherwise, downstream operations could produce invalid results
+if the distributed insert has not completed before additional updates are executed.
+
+## Distributed table materialization
+
+Distributed table created with following steps:
+1. Creates temp view with sql query to get right structure
+2. Create empty local tables based on view 
+3. Create distributed table based on local tables. 
+4. Data inserts into distributed table, so it is distributed across shards without duplicating.
+
+### Distributed table model example
+```sql
+{{
+    config(
+        materialized='distributed_table',
+        order_by='id, created_at',
+        sharding_key='cityHash64(id)',
+        engine='ReplacingMergeTree'
+    )
+}}
+
+select id, created_at, item from {{ source('db', 'table') }}
+```
+
+### Generated migrations
+
+```sql
+CREATE TABLE db.table_local on cluster cluster
+(
+    `id` UInt64,
+    `created_at` DateTime,
+    `item` String
+)
+ENGINE = ReplacingMergeTree
+ORDER BY (id, created_at)
+SETTINGS index_granularity = 8192;
+
+
+CREATE TABLE db.table on cluster cluster
+(
+    `id` UInt64,
+    `created_at` DateTime,
+    `item` String
+)
+ENGINE = Distributed('cluster', 'db', 'table_local', cityHash64(id));
+```
+
+## Distributed incremental materialization
+
+Incremental model based on the same idea as distributed table, the main difficulty is to process all incremental strategies correctly.
+
+1. _The Append Strategy_ just insert data into distributed table.
+2. _The Delete+Insert_ Strategy creates distributed temp table to work with all data on every shard.
+3. _The Default (Legacy) Strategy_ creates distributed temp and intermediate tables for the same reason.
+
+Only shard tables are replacing, because distributed table does not keep data. 
+The distributed table reloads only when the full_refresh mode is enabled or the table structure may have changed.
+
+### Distributed incremental model example
+```sql
+{{
+    config(
+        materialized='distributed_incremental',
+        engine='MergeTree',
+        incremental_strategy='append',
+        unique_key='id,created_at'
+    )
+}}
+
+select id, created_at, item from {{ source('db', 'table') }}
+```
+
+### Generated migrations
+
+```sql
+CREATE TABLE db.table_local on cluster cluster
+(
+    `id` UInt64,
+    `created_at` DateTime,
+    `item` String
+)
+ENGINE = MergeTree
+SETTINGS index_granularity = 8192;
+
+
+CREATE TABLE db.table on cluster cluster
+(
+    `id` UInt64,
+    `created_at` DateTime,
+    `item` String
+)
+ENGINE = Distributed('cluster', 'db', 'table_local', cityHash64(id));
+```
+
 # Running Tests
 
 This adapter passes all of dbt basic tests as presented in dbt's official docs: https://docs.getdbt.com/docs/contributing/testing-a-new-adapter#testing-your-adapter.
 Use `pytest tests` to run tests.
 
 You can customize the test environment via environment variables. We recommend doing so with the pytest `pytest-dotenv` plugin combined with root level `test.env`
 configuration file (this file should not be checked into git).  The following environment variables are recognized:
```

### Comparing `dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/__init__.py` & `dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/column.py` & `dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/column.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/connections.py` & `dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/credentials.py` & `dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/dbclient.py` & `dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/dbclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/httpclient.py` & `dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/httpclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/impl.py` & `dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/nativeclient.py` & `dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/nativeclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/adapters/clickhouse/relation.py` & `dbt-clickhouse-1.4.5/dbt/adapters/clickhouse/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/adapters/apply_grants.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/adapters/relation.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/adapters.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/catalog.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/distributed_table.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/distributed_table.sql`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 {% materialization distributed_table, adapter='clickhouse' %}
+  {% set insert_distributed_sync = run_query("SELECT value FROM system.settings WHERE name = 'insert_distributed_sync'")[0][0] %}
+  {% if insert_distributed_sync != '1' %}
+     {% do exceptions.raise_compiler_error('To use distributed materialization setting insert_distributed_sync should be set to 1') %}
+  {% endif %}
+
   {%- set local_suffix = adapter.get_clickhouse_local_suffix() -%}
 
   {%- set existing_relation = load_cached_relation(this) -%}
   {%- set target_relation = this.incorporate(type='table') -%}
 
   {% set existing_relation_local = existing_relation.incorporate(path={"identifier": model['name'] + local_suffix}) if existing_relation is not none else none %}
   {% set target_relation_local = target_relation.incorporate(path={"identifier": model['name'] + local_suffix}) if target_relation is not none else none %}
@@ -33,16 +38,15 @@
   {% call statement('main') %}
     {{ create_view_as(view_relation, sql) }}
   {% endcall %}
 
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   {% if backup_relation is none %}
-    {% do run_query(create_empty_table_from_relation(target_relation_local, view_relation)) or '' %}
-    {% do run_query(create_distributed_table(target_relation, target_relation_local)) or '' %}
+    {{ create_distributed_local_table(target_relation, target_relation_local, view_relation) }}
   {% elif existing_relation.can_exchange %}
     -- We can do an atomic exchange, so no need for an intermediate
     {% call statement('main') -%}
       {% do run_query(create_empty_table_from_relation(backup_relation, view_relation)) or '' %}
     {%- endcall %}
     {% do exchange_tables_atomic(backup_relation, existing_relation) %}
   {% else %}
@@ -62,15 +66,20 @@
   {{ drop_relation_if_exists(backup_relation) }}
   {{ run_hooks(post_hooks, inside_transaction=False) }}
   {{ return({'relations': [target_relation]}) }}
 
 {% endmaterialization %}
 
 {% macro create_distributed_table(relation, local_relation) %}
-   {%- set cluster = adapter.get_clickhouse_cluster_name()[1:-1] -%}
+    {%- set cluster = adapter.get_clickhouse_cluster_name() -%}
+   {% if cluster is none %}
+        {% do exceptions.raise_compiler_error('Cluster name should be defined for using distributed materializations, current is None') %}
+    {% endif %}
+
+   {%- set cluster = cluster[1:-1] -%}
    {%- set sharding = config.get('sharding_key') -%}
 
     CREATE TABLE {{ relation }} {{ on_cluster_clause() }} AS {{ local_relation }}
     ENGINE = Distributed('{{ cluster}}', '{{ relation.schema }}', '{{ local_relation.name }}'
     {% if sharding is not none %}
         , {{ sharding }}
     {% endif %}
@@ -94,7 +103,17 @@
 
   {{ engine_clause() }}
   {{ order_cols(label="order by") }}
   {{ primary_key_clause(label="primary key") }}
   {{ partition_cols(label="partition by") }}
   {{ adapter.get_model_settings(model) }}
 {%- endmacro %}
+
+{% macro create_distributed_local_table(distributed_relation, shard_relation, structure_relation, sql_query=none) -%}
+  {{ drop_relation_if_exists(shard_relation) }}
+  {{ drop_relation_if_exists(distributed_relation) }}
+  {% do run_query(create_empty_table_from_relation(shard_relation, structure_relation)) or '' %}
+  {% do run_query(create_distributed_table(distributed_relation, shard_relation)) or '' %}
+  {% if sql_query is not none %}
+    {% do run_query(clickhouse__insert_into(distributed_relation, sql_query)) or '' %}
+  {% endif %}
+{%- endmacro %}
```

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/incremental.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/incremental.sql`

 * *Files 11% similar despite different names*

```diff
@@ -130,74 +130,105 @@
     {% endif %}
 
     {% do sync_column_schemas(on_schema_change, target_relation, schema_changes_dict) %}
 
 {% endmacro %}
 
 
-{% macro clickhouse__incremental_legacy(existing_relation, intermediate_relation, on_schema_change, unique_key) %}
-    -- First create a temporary table for all of the new data
+{% macro clickhouse__incremental_legacy(existing_relation, intermediate_relation, on_schema_change, unique_key, is_distributed=False) %}
     {% set new_data_relation = existing_relation.incorporate(path={"identifier": model['name'] + '__dbt_new_data'}) %}
     {{ drop_relation_if_exists(new_data_relation) }}
-    {% call statement('create_new_data_temp') %}
+    {%- set distributed_new_data_relation = existing_relation.incorporate(path={"identifier": model['name'] + '__dbt_distributed_new_data'}) -%}
+
+    {%- set inserted_relation = intermediate_relation -%}
+    {%- set inserting_relation = new_data_relation -%}
+
+    -- First create a temporary table for all of the new data
+    {% if is_distributed %}
+      -- Need to use distributed table to have data on all shards
+      {%- set inserting_relation = distributed_new_data_relation -%}
+      {{ create_distributed_local_table(distributed_new_data_relation, new_data_relation, existing_relation, sql) }}
+    {% else %}
+      {% call statement('create_new_data_temp') %}
         {{ get_create_table_as_sql(False, new_data_relation, sql) }}
-    {% endcall %}
+      {% endcall %}
+    {% endif %}
 
     -- Next create another temporary table that will eventually be used to replace the existing table.  We can't
     -- use the table just created in the previous step because we don't want to override any updated rows with
     -- old rows when we insert the old data
-    {% call statement('main') %}
-       create table {{ intermediate_relation }} as {{ new_data_relation }}
-    {% endcall %}
+    {% if is_distributed %}
+      {%- set distributed_intermediate_relation = make_intermediate_relation(existing_relation) -%}
+      {%- set inserted_relation = distributed_intermediate_relation -%}
+      {{ create_distributed_local_table(distributed_intermediate_relation, intermediate_relation, existing_relation) }}
+    {% else %}
+      {% call statement('main') %}
+          create table {{ intermediate_relation }} as {{ new_data_relation }} {{ on_cluster_clause() }}
+      {% endcall %}
+    {% endif %}
 
     -- Insert all the existing rows into the new temporary table, ignoring any rows that have keys in the "new data"
     -- table.
     {%- set dest_columns = adapter.get_columns_in_relation(existing_relation) -%}
     {%- set dest_cols_csv = dest_columns | map(attribute='quoted') | join(', ') -%}
     {% call statement('insert_existing_data') %}
-        insert into {{ intermediate_relation }} ({{ dest_cols_csv }})
+        insert into {{ inserted_relation }} ({{ dest_cols_csv }})
         select {{ dest_cols_csv }}
         from {{ existing_relation }}
           where ({{ unique_key }}) not in (
             select {{ unique_key }}
-            from {{ new_data_relation }}
+            from {{ inserting_relation }}
           )
        {{ adapter.get_model_settings(model) }}
     {% endcall %}
 
     -- Insert all of the new data into the temporary table
     {% call statement('insert_new_data') %}
-     insert into {{ intermediate_relation }} ({{ dest_cols_csv }})
+     insert into {{ inserted_relation }} ({{ dest_cols_csv }})
         select {{ dest_cols_csv }}
-        from {{ new_data_relation }}
+        from {{ inserting_relation }}
       {{ adapter.get_model_settings(model) }}
     {% endcall %}
 
     {% do adapter.drop_relation(new_data_relation) %}
+    {{ drop_relation_if_exists(distributed_new_data_relation) }}
+    {{ drop_relation_if_exists(distributed_intermediate_relation) }}
 
 {% endmacro %}
 
 
-{% macro clickhouse__incremental_delete_insert(existing_relation, unique_key, incremental_predicates) %}
+{% macro clickhouse__incremental_delete_insert(existing_relation, unique_key, incremental_predicates, is_distributed=False) %}
     {% set new_data_relation = existing_relation.incorporate(path={"identifier": model['name']
        + '__dbt_new_data_' + invocation_id.replace('-', '_')}) %}
     {{ drop_relation_if_exists(new_data_relation) }}
-    {% call statement('main') %}
+    {%- set distributed_new_data_relation = existing_relation.incorporate(path={"identifier": model['name'] + '__dbt_distributed_new_data'}) -%}
+
+    {%- set inserting_relation = new_data_relation -%}
+
+    {% if is_distributed %}
+      -- Need to use distributed table to have data on all shards
+      {%- set inserting_relation = distributed_new_data_relation -%}
+      {{ create_distributed_local_table(distributed_new_data_relation, new_data_relation, existing_relation, sql) }}
+    {% else %}
+      {% call statement('main') %}
         {{ get_create_table_as_sql(False, new_data_relation, sql) }}
-    {% endcall %}
+      {% endcall %}
+    {% endif %}
+
     {% call statement('delete_existing_data') %}
       delete from {{ existing_relation }} where ({{ unique_key }}) in (select {{ unique_key }}
-                                          from {{ new_data_relation }})
+                                          from {{ inserting_relation }})
       {%- if incremental_predicates %}
         {% for predicate in incremental_predicates %}
             and {{ predicate }}
         {% endfor %}
       {%- endif -%};
     {% endcall %}
 
     {%- set dest_columns = adapter.get_columns_in_relation(existing_relation) -%}
     {%- set dest_cols_csv = dest_columns | map(attribute='quoted') | join(', ') -%}
     {% call statement('insert_new_data') %}
-        insert into {{ existing_relation}} select {{ dest_cols_csv}} from {{ new_data_relation }}
+        insert into {{ existing_relation }} select {{ dest_cols_csv }} from {{ inserting_relation }}
     {% endcall %}
     {% do adapter.drop_relation(new_data_relation) %}
+    {{ drop_relation_if_exists(distributed_new_data_relation) }}
 {% endmacro %}
```

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/s3.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/s3.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/seed.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/snapshot.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/table.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/materializations/view.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/persist_docs.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt/include/clickhouse/macros/utils/utils.sql` & `dbt-clickhouse-1.4.5/dbt/include/clickhouse/macros/utils/utils.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.4.4/dbt_clickhouse.egg-info/PKG-INFO` & `dbt-clickhouse-1.4.5/dbt_clickhouse.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickhouse
-Version: 1.4.4
+Version: 1.4.5
 Summary: The Clickhouse plugin for dbt (data build tool)
 Home-page: https://github.com/ClickHouse/dbt-clickhouse
 Author: ClickHouse Inc.
 Author-email: guy@clickhouse.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,16 @@
 - [x] Seeds
 - [x] Sources
 - [x] Docs generate
 - [x] Tests
 - [x] Snapshots
 - [x] Most dbt-utils macros (now included in dbt-core)  
 - [x] Ephemeral materialization
+- [x] Distributed table materialization (experimental)
+- [x] Distributed incremental materialization (experimental)
 
 # Usage Notes
 
 ## Database
 
 The dbt model relation identifier `database.schema.table` is not compatible with Clickhouse because Clickhouse does not support a `schema`.
 So we use a simplified approach `schema.table`, where `schema` is the Clickhouse database. Using the `default` database is not recommended.
@@ -84,14 +86,15 @@
       retries: [1] # Number of times to retry a "retriable" database exception (such as a 503 'Service Unavailable' error)
       compression: [<empty string>] Use gzip compression if truthy (http), or compression type for a native connection
       connect_timeout: [10] # Timeout in seconds to establish a connection to ClickHouse
       send_receive_timeout: [300] # Timeout in seconds to receive data from the ClickHouse server
       cluster_mode: [False] # Use specific settings designed to improve operation on Replicated databases (recommended for ClickHouse Cloud)
       use_lw_deletes: [False] Use the strategy `delete+insert` as the default incremental strategy.
       check_exchange: [True] # Validate that clickhouse support the atomic EXCHANGE TABLES command.  (Not needed for most ClickHouse versions)
+      local_suffix [local] # Table suffix of local tables on shards for distributed materializations 
       custom_settings: [{}] # A dicitonary/mapping of custom ClickHouse settings for the connection - default is empty.
       
       # Native (clickhouse-driver) connection settings
       sync_request_timeout: [5] Timeout for server ping
       compress_block_size: [1048576] Compression block size if compression is enabled
       
 ```
@@ -172,14 +175,115 @@
 | structure             | The column structure of the data in bucket, as a list of name/datatype pairs, such as `['id UInt32', 'date DateTime', 'value String']`  If not provided ClickHouse will infer the structure. |
 | aws_access_key_id     | The S3 access key id.                                                                                                                                                                        |
 | aws_secret_access_key | The S3 secrete key.                                                                                                                                                                          |
 | compression           | The compression method used with the S3 objects.  If not provided ClickHouse will attempt to determine compression based on the file name.                                                   |
 
 See the [S3 test file](https://github.com/ClickHouse/dbt-clickhouse/blob/main/tests/integration/adapter/test_s3.py) for examples of how to use this macro.
 
+# Distributed materializations
+
+Note:  Distributed materializations experimental and are not currently included in the automated test suite.
+
+WARNING: 
+
+To use distributed materializations correctly you should set **insert_distributed_sync** = 1 (or use as prehook) in order to have correct data while SELECT queries. Otherwise, downstream operations could produce invalid results
+if the distributed insert has not completed before additional updates are executed.
+
+## Distributed table materialization
+
+Distributed table created with following steps:
+1. Creates temp view with sql query to get right structure
+2. Create empty local tables based on view 
+3. Create distributed table based on local tables. 
+4. Data inserts into distributed table, so it is distributed across shards without duplicating.
+
+### Distributed table model example
+```sql
+{{
+    config(
+        materialized='distributed_table',
+        order_by='id, created_at',
+        sharding_key='cityHash64(id)',
+        engine='ReplacingMergeTree'
+    )
+}}
+
+select id, created_at, item from {{ source('db', 'table') }}
+```
+
+### Generated migrations
+
+```sql
+CREATE TABLE db.table_local on cluster cluster
+(
+    `id` UInt64,
+    `created_at` DateTime,
+    `item` String
+)
+ENGINE = ReplacingMergeTree
+ORDER BY (id, created_at)
+SETTINGS index_granularity = 8192;
+
+
+CREATE TABLE db.table on cluster cluster
+(
+    `id` UInt64,
+    `created_at` DateTime,
+    `item` String
+)
+ENGINE = Distributed('cluster', 'db', 'table_local', cityHash64(id));
+```
+
+## Distributed incremental materialization
+
+Incremental model based on the same idea as distributed table, the main difficulty is to process all incremental strategies correctly.
+
+1. _The Append Strategy_ just insert data into distributed table.
+2. _The Delete+Insert_ Strategy creates distributed temp table to work with all data on every shard.
+3. _The Default (Legacy) Strategy_ creates distributed temp and intermediate tables for the same reason.
+
+Only shard tables are replacing, because distributed table does not keep data. 
+The distributed table reloads only when the full_refresh mode is enabled or the table structure may have changed.
+
+### Distributed incremental model example
+```sql
+{{
+    config(
+        materialized='distributed_incremental',
+        engine='MergeTree',
+        incremental_strategy='append',
+        unique_key='id,created_at'
+    )
+}}
+
+select id, created_at, item from {{ source('db', 'table') }}
+```
+
+### Generated migrations
+
+```sql
+CREATE TABLE db.table_local on cluster cluster
+(
+    `id` UInt64,
+    `created_at` DateTime,
+    `item` String
+)
+ENGINE = MergeTree
+SETTINGS index_granularity = 8192;
+
+
+CREATE TABLE db.table on cluster cluster
+(
+    `id` UInt64,
+    `created_at` DateTime,
+    `item` String
+)
+ENGINE = Distributed('cluster', 'db', 'table_local', cityHash64(id));
+```
+
 # Running Tests
 
 This adapter passes all of dbt basic tests as presented in dbt's official docs: https://docs.getdbt.com/docs/contributing/testing-a-new-adapter#testing-your-adapter.
 Use `pytest tests` to run tests.
 
 You can customize the test environment via environment variables. We recommend doing so with the pytest `pytest-dotenv` plugin combined with root level `test.env`
 configuration file (this file should not be checked into git).  The following environment variables are recognized:
```

### Comparing `dbt-clickhouse-1.4.4/dbt_clickhouse.egg-info/SOURCES.txt` & `dbt-clickhouse-1.4.5/dbt_clickhouse.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 dbt/include/clickhouse/__init__.py
 dbt/include/clickhouse/dbt_project.yml
 dbt/include/clickhouse/macros/adapters.sql
 dbt/include/clickhouse/macros/catalog.sql
 dbt/include/clickhouse/macros/persist_docs.sql
 dbt/include/clickhouse/macros/adapters/apply_grants.sql
 dbt/include/clickhouse/macros/adapters/relation.sql
+dbt/include/clickhouse/macros/materializations/distributed_incremental.sql
 dbt/include/clickhouse/macros/materializations/distributed_table.sql
 dbt/include/clickhouse/macros/materializations/incremental.sql
 dbt/include/clickhouse/macros/materializations/s3.sql
 dbt/include/clickhouse/macros/materializations/seed.sql
 dbt/include/clickhouse/macros/materializations/snapshot.sql
 dbt/include/clickhouse/macros/materializations/table.sql
 dbt/include/clickhouse/macros/materializations/view.sql
```

### Comparing `dbt-clickhouse-1.4.4/setup.py` & `dbt-clickhouse-1.4.5/setup.py`

 * *Files identical despite different names*

