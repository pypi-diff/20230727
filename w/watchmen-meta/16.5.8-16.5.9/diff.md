# Comparing `tmp/watchmen_meta-16.5.8.tar.gz` & `tmp/watchmen_meta-16.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_meta-16.5.8.tar", max compression
+gzip compressed data, was "watchmen_meta-16.5.9.tar", max compression
```

## Comparing `watchmen_meta-16.5.8.tar` & `watchmen_meta-16.5.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.199630 watchmen_meta-16.5.8/LICENSE
--rw-r--r--   0        0        0     1015 2023-06-08 03:33:39.199630 watchmen_meta-16.5.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.199630 watchmen_meta-16.5.8/src/watchmen_meta/__init__.py
--rw-r--r--   0        0        0      496 2023-06-08 03:33:39.199630 watchmen_meta-16.5.8/src/watchmen_meta/admin/__init__.py
--rw-r--r--   0        0        0     5952 2023-06-08 03:33:39.199630 watchmen_meta-16.5.8/src/watchmen_meta/admin/enumeration_service.py
--rw-r--r--   0        0        0     3925 2023-06-08 03:33:39.199630 watchmen_meta-16.5.8/src/watchmen_meta/admin/pipeline_graphic_service.py
--rw-r--r--   0        0        0     6482 2023-06-08 03:33:39.199630 watchmen_meta-16.5.8/src/watchmen_meta/admin/pipeline_service.py
--rw-r--r--   0        0        0     4502 2023-06-08 03:33:39.199630 watchmen_meta-16.5.8/src/watchmen_meta/admin/space_service.py
--rw-r--r--   0        0        0     6568 2023-06-08 03:33:39.199630 watchmen_meta-16.5.8/src/watchmen_meta/admin/topic_service.py
--rw-r--r--   0        0        0     3740 2023-06-08 03:33:39.199630 watchmen_meta-16.5.8/src/watchmen_meta/admin/topic_snapshot_lock_service.py
--rw-r--r--   0        0        0     4882 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/admin/topic_snapshot_scheduler_service.py
--rw-r--r--   0        0        0     3799 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/admin/user_group_service.py
--rw-r--r--   0        0        0     4658 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/admin/user_service.py
--rw-r--r--   0        0        0      108 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/analysis/__init__.py
--rw-r--r--   0        0        0     3024 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/analysis/pipeline_index_service.py
--rw-r--r--   0        0        0     5553 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/analysis/topic_index_service.py
--rw-r--r--   0        0        0       73 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/auth/__init__.py
--rw-r--r--   0        0        0     2731 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/auth/auth_helper.py
--rw-r--r--   0        0        0      726 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/common/__init__.py
--rw-r--r--   0        0        0       48 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/common/exception.py
--rw-r--r--   0        0        0      418 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/common/last_visit_service.py
--rw-r--r--   0        0        0     6206 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/common/operation_service.py
--rw-r--r--   0        0        0     4540 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/common/package_version_service.py
--rw-r--r--   0        0        0     7833 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/common/settings.py
--rw-r--r--   0        0        0     7488 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/common/storage_service.py
--rw-r--r--   0        0        0     6682 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/common/tuple_service.py
--rw-r--r--   0        0        0     6212 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/common/user_based_tuple_service.py
--rw-r--r--   0        0        0      267 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/console/__init__.py
--rw-r--r--   0        0        0     2289 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/console/connected_space_graphic_service.py
--rw-r--r--   0        0        0     6726 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/console/connected_space_service.py
--rw-r--r--   0        0        0     3570 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/console/dashboard_service.py
--rw-r--r--   0        0        0     5922 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/console/report_service.py
--rw-r--r--   0        0        0     5405 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/console/subject_service.py
--rw-r--r--   0        0        0      158 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/dqc/__init__.py
--rw-r--r--   0        0        0     2929 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/dqc/catalog_service.py
--rw-r--r--   0        0        0     2492 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/dqc/monitor_rule_lock_service.py
--rw-r--r--   0        0        0     4433 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/dqc/monitor_rule_service.py
--rw-r--r--   0        0        0      101 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/gui/__init__.py
--rw-r--r--   0        0        0     3389 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/gui/favorite_service.py
--rw-r--r--   0        0        0     3665 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/gui/last_snapshot_service.py
--rw-r--r--   0        0        0      277 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/system/__init__.py
--rw-r--r--   0        0        0     4389 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/system/data_source_service.py
--rw-r--r--   0        0        0     2718 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/system/external_writer_service.py
--rw-r--r--   0        0        0     1557 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/system/key_store_service.py
--rw-r--r--   0        0        0     3847 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/system/pat_service.py
--rw-r--r--   0        0        0     3076 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/system/plugin_service.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/system/sql_query_performance_service.py
--rw-r--r--   0        0        0     1782 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/system/tenant_service.py
--rw-r--r--   0        0        0        0 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/webhook/__init__.py
--rw-r--r--   0        0        0     3223 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/webhook/event_definition_service.py
--rw-r--r--   0        0        0     2956 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/webhook/notification_definition_service.py
--rw-r--r--   0        0        0     2185 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/webhook/subscription_event_lock_service.py
--rw-r--r--   0        0        0     2976 2023-06-08 03:33:39.203630 watchmen_meta-16.5.8/src/watchmen_meta/webhook/subscription_event_service.py
--rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 watchmen_meta-16.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/LICENSE
+-rw-r--r--   0        0        0     1015 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/__init__.py
+-rw-r--r--   0        0        0      496 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/admin/__init__.py
+-rw-r--r--   0        0        0     5952 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/admin/enumeration_service.py
+-rw-r--r--   0        0        0     3925 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/admin/pipeline_graphic_service.py
+-rw-r--r--   0        0        0     6482 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/admin/pipeline_service.py
+-rw-r--r--   0        0        0     4502 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/admin/space_service.py
+-rw-r--r--   0        0        0     6568 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/admin/topic_service.py
+-rw-r--r--   0        0        0     3740 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/admin/topic_snapshot_lock_service.py
+-rw-r--r--   0        0        0     4882 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/admin/topic_snapshot_scheduler_service.py
+-rw-r--r--   0        0        0     3799 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/admin/user_group_service.py
+-rw-r--r--   0        0        0     4658 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/admin/user_service.py
+-rw-r--r--   0        0        0      108 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/analysis/__init__.py
+-rw-r--r--   0        0        0     3024 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/analysis/pipeline_index_service.py
+-rw-r--r--   0        0        0     5553 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/analysis/topic_index_service.py
+-rw-r--r--   0        0        0       73 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/auth/__init__.py
+-rw-r--r--   0        0        0     2731 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/auth/auth_helper.py
+-rw-r--r--   0        0        0      726 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/common/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/common/exception.py
+-rw-r--r--   0        0        0      418 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/common/last_visit_service.py
+-rw-r--r--   0        0        0     6252 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/common/operation_service.py
+-rw-r--r--   0        0        0     4540 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/common/package_version_service.py
+-rw-r--r--   0        0        0     7835 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/common/settings.py
+-rw-r--r--   0        0        0     7488 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/common/storage_service.py
+-rw-r--r--   0        0        0     6682 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/common/tuple_service.py
+-rw-r--r--   0        0        0     6212 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/common/user_based_tuple_service.py
+-rw-r--r--   0        0        0      267 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/console/__init__.py
+-rw-r--r--   0        0        0     2289 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/console/connected_space_graphic_service.py
+-rw-r--r--   0        0        0     6726 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/console/connected_space_service.py
+-rw-r--r--   0        0        0     3570 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/console/dashboard_service.py
+-rw-r--r--   0        0        0     5922 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/console/report_service.py
+-rw-r--r--   0        0        0     5405 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/console/subject_service.py
+-rw-r--r--   0        0        0      158 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/dqc/__init__.py
+-rw-r--r--   0        0        0     2929 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/dqc/catalog_service.py
+-rw-r--r--   0        0        0     2492 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/dqc/monitor_rule_lock_service.py
+-rw-r--r--   0        0        0     4433 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/dqc/monitor_rule_service.py
+-rw-r--r--   0        0        0      101 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/gui/__init__.py
+-rw-r--r--   0        0        0     3389 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/gui/favorite_service.py
+-rw-r--r--   0        0        0     3665 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/gui/last_snapshot_service.py
+-rw-r--r--   0        0        0      277 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/system/__init__.py
+-rw-r--r--   0        0        0     4389 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/system/data_source_service.py
+-rw-r--r--   0        0        0     2718 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/system/external_writer_service.py
+-rw-r--r--   0        0        0     1557 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/system/key_store_service.py
+-rw-r--r--   0        0        0     3847 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/system/pat_service.py
+-rw-r--r--   0        0        0     3076 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/system/plugin_service.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/system/sql_query_performance_service.py
+-rw-r--r--   0        0        0     1782 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/system/tenant_service.py
+-rw-r--r--   0        0        0        0 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/webhook/__init__.py
+-rw-r--r--   0        0        0     3223 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/webhook/event_definition_service.py
+-rw-r--r--   0        0        0     2956 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/webhook/notification_definition_service.py
+-rw-r--r--   0        0        0     2185 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/webhook/subscription_event_lock_service.py
+-rw-r--r--   0        0        0     2976 2023-06-10 16:48:37.883968 watchmen_meta-16.5.9/src/watchmen_meta/webhook/subscription_event_service.py
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 watchmen_meta-16.5.9/PKG-INFO
```

### Comparing `watchmen_meta-16.5.8/LICENSE` & `watchmen_meta-16.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/pyproject.toml` & `watchmen_meta-16.5.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "watchmen-meta"
-version = "16.5.8"
+version = "16.5.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_meta", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pycryptodome = "^3.14.1"
-watchmen-auth = "16.5.8"
-watchmen-storage = "16.5.8"
-watchmen-storage-mysql = { version = "16.5.8", optional = true }
-watchmen-storage-oracle = { version = "16.5.8", optional = true }
-watchmen-storage-mongodb = { version = "16.5.8", optional = true }
-watchmen-storage-mssql = { version = "16.5.8", optional = true }
-watchmen-storage-postgresql = { version = "16.5.8", optional = true }
+watchmen-auth = "16.5.9"
+watchmen-storage = "16.5.9"
+watchmen-storage-mysql = { version = "16.5.9", optional = true }
+watchmen-storage-oracle = { version = "16.5.9", optional = true }
+watchmen-storage-mongodb = { version = "16.5.9", optional = true }
+watchmen-storage-mssql = { version = "16.5.9", optional = true }
+watchmen-storage-postgresql = { version = "16.5.9", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/admin/enumeration_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/admin/enumeration_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/admin/pipeline_graphic_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/admin/pipeline_graphic_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/admin/pipeline_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/admin/pipeline_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/admin/space_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/admin/space_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/admin/topic_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/admin/topic_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/admin/topic_snapshot_lock_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/admin/topic_snapshot_lock_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/admin/topic_snapshot_scheduler_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/admin/topic_snapshot_scheduler_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/admin/user_group_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/admin/user_group_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/admin/user_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/admin/user_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/analysis/pipeline_index_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/analysis/pipeline_index_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/analysis/topic_index_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/analysis/topic_index_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/auth/auth_helper.py` & `watchmen_meta-16.5.9/src/watchmen_meta/auth/auth_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/common/__init__.py` & `watchmen_meta-16.5.9/src/watchmen_meta/common/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/common/operation_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/common/operation_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	EntityStraightColumn, EntityStraightAggregateColumn, EntityColumnAggregateArithmetic, EntityDeleter, \
 	SnowflakeGenerator, TransactionalStorageSPI
 
 RecordId = TypeVar('RecordId', bound=str)
 
 
 class OperationShaper(EntityShaper):
-	
+
 	def serialize(self, operation: Operation) -> EntityRow:
 		return {
 			'record_id': operation.recordId,
 			'operation_type': operation.operationType,
 			'tuple_type': operation.tupleType,
 			'tuple_key': operation.tupleKey,
 			'tuple_id': operation.tupleId,
@@ -30,15 +30,15 @@
 			'version_num': operation.versionNum,
 			'tenant_id': operation.tenantId,
 			'created_at': operation.createdAt,
 			'created_by': operation.createdBy,
 			'last_modified_at': operation.lastModifiedAt,
 			'last_modified_by': operation.lastModifiedBy
 		}
-	
+
 	def deserialize(self, row: EntityRow) -> Operation:
 		# noinspection PyTypeChecker
 		return Operation(
 			recordId=row.get('record_id'),
 			operationType=row.get('operation_type'),
 			tupleType=row.get('tuple_type'),
 			tupleKey=row.get('tuple_key'),
@@ -67,15 +67,15 @@
 	):
 		super().__init__(storage)
 		self.with_snowflake_generator(snowflake_generator)
 		self.with_principal_service(principal_service)
 
 	def get_entity_name(self) -> EntityName:
 		return OPERATIONS_TABLE
-	
+
 	def get_entity_shaper(self) -> EntityShaper:
 		return OPERATIONS_ENTITY_SHAPER
 
 	# noinspection SpellCheckingInspection
 	def get_storable_id_column_name(self) -> EntityName:
 		return 'record_id'
 
@@ -95,22 +95,23 @@
 	def get_record_ids(self, version_num: str, tuple_type: str):
 		return self.storage.find_straight_values(EntityStraightValuesFinder(
 			name=self.get_entity_name(),
 			shaper=self.get_entity_shaper(),
 			criteria=[
 				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='tuple_type'), right=tuple_type),
 				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='version_num'), right=version_num),
-				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='tenant_id'), right=self.principalService.tenantId)
+				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='tenant_id'),
+				                         right=self.principalService.tenantId)
 			],
 			straightColumns=[EntityStraightAggregateColumn(columnName="record_id",
 			                                               arithmetic=EntityColumnAggregateArithmetic.MAX),
 			                 EntityStraightColumn(columnName="tuple_id")]
 		))
 
-	def get_record_with_create_type(self, version_num: str, tuple_type: str,tuple_id:str):
+	def get_record_with_create_type(self, version_num: str, tuple_type: str, tuple_id: str):
 		return self.storage.find_straight_values(EntityStraightValuesFinder(
 			name=self.get_entity_name(),
 			shaper=self.get_entity_shaper(),
 			criteria=[
 				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='tuple_type'), right=tuple_type),
 				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='version_num'), right=version_num),
 				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='tuple_id'),
@@ -118,18 +119,17 @@
 				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='tenant_id'),
 				                         right=self.principalService.tenantId),
 				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='operation_type'),
 				                         right=OperationType.CREATE),
 
 			],
 			straightColumns=[EntityStraightColumn(columnName="record_id",
-			                                               arithmetic=EntityColumnAggregateArithmetic.MAX)]
+			                                      arithmetic=EntityColumnAggregateArithmetic.MAX)]
 		))
 
-
 	def get_operation_by_id(self, id_: str) -> Optional[Operation]:
 		return self.storage.find_by_id(id_, self.get_entity_id_helper())
 
 	def get_previous_record_id(self, tuple_id: str, version: str) -> Optional[str]:
 		rows = self.storage.find_straight_values(EntityStraightValuesFinder(
 			name=self.get_entity_name(),
 			shaper=self.get_entity_shaper(),
@@ -142,17 +142,18 @@
 				                         operator=EntityCriteriaOperator.NOT_EQUALS,
 				                         right=version),
 			],
 			straightColumns=[EntityStraightAggregateColumn(columnName="record_id",
 			                                               arithmetic=EntityColumnAggregateArithmetic.MAX)]
 		))
 		return rows[0].get("record_id")
-	
+
 	def clean_operations(self, tuple_type: str) -> int:
 		return self.storage.delete(EntityDeleter(
 			name=self.get_entity_name(),
 			shaper=self.get_entity_shaper(),
 			criteria=[
 				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='tuple_type'), right=tuple_type),
-				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='tenant_id'), right=self.principalService.tenantId)
+				EntityCriteriaExpression(left=ColumnNameLiteral(columnName='tenant_id'),
+				                         right=self.principalService.tenantId)
 			]
 		))
```

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/common/package_version_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/common/package_version_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/common/settings.py` & `watchmen_meta-16.5.9/src/watchmen_meta/common/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 		# secrets_dir = '/var/run'
 		env_file = '.env'
 		env_file_encoding = 'utf-8'
 		case_sensitive = True
 
 
 settings = MetaSettings()
-logger.info(f'Meta settings[{settings.dict()}].')
+# logger.info(f'Meta settings[{settings.dict()}].')
 
 
 def ask_super_admin() -> PrincipalService:
 	return PrincipalService(User(
 		userId=settings.SUPER_ADMIN_USER_ID,
 		name=settings.SUPER_ADMIN_USER_NAME,
 		nickname=settings.SUPER_ADMIN_USER_NICKNAME,
```

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/common/storage_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/common/storage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/common/tuple_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/common/tuple_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/common/user_based_tuple_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/common/user_based_tuple_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/console/connected_space_graphic_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/console/connected_space_graphic_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/console/connected_space_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/console/connected_space_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/console/dashboard_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/console/dashboard_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/console/report_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/console/report_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/console/subject_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/console/subject_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/dqc/catalog_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/dqc/catalog_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/dqc/monitor_rule_lock_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/dqc/monitor_rule_lock_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/dqc/monitor_rule_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/dqc/monitor_rule_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/gui/favorite_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/gui/favorite_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/gui/last_snapshot_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/gui/last_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/system/data_source_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/system/data_source_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/system/external_writer_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/system/external_writer_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/system/key_store_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/system/key_store_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/system/pat_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/system/pat_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/system/plugin_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/system/plugin_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/system/tenant_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/system/tenant_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/webhook/event_definition_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/webhook/event_definition_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/webhook/notification_definition_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/webhook/notification_definition_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/webhook/subscription_event_lock_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/webhook/subscription_event_lock_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/src/watchmen_meta/webhook/subscription_event_service.py` & `watchmen_meta-16.5.9/src/watchmen_meta/webhook/subscription_event_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_meta-16.5.8/PKG-INFO` & `watchmen_meta-16.5.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-meta
-Version: 16.5.8
+Version: 16.5.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: mongodb
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: postgresql
 Requires-Dist: pycryptodome (>=3.14.1,<4.0.0)
-Requires-Dist: watchmen-auth (==16.5.8)
-Requires-Dist: watchmen-storage (==16.5.8)
-Requires-Dist: watchmen-storage-mongodb (==16.5.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-postgresql (==16.5.8) ; extra == "postgresql"
+Requires-Dist: watchmen-auth (==16.5.9)
+Requires-Dist: watchmen-storage (==16.5.9)
+Requires-Dist: watchmen-storage-mongodb (==16.5.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-postgresql (==16.5.9) ; extra == "postgresql"
```

