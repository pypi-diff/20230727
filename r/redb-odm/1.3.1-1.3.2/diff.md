# Comparing `tmp/redb-odm-1.3.1.tar.gz` & `tmp/redb-odm-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redb-odm-1.3.1.tar", last modified: Sun Jul  9 04:17:53 2023, max compression
+gzip compressed data, was "redb-odm-1.3.2.tar", last modified: Thu Jul 27 21:28:08 2023, max compression
```

## Comparing `redb-odm-1.3.1.tar` & `redb-odm-1.3.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 04:17:53.265205 redb-odm-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-09 04:17:37.000000 redb-odm-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-09 04:17:53.265205 redb-odm-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 04:17:37.000000 redb-odm-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 04:17:53.253205 redb-odm-1.3.1/redb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 04:17:53.257205 redb-odm-1.3.1/redb/behaviors/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/behaviors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/behaviors/i_remember.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/behaviors/soft_deletion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 04:17:53.257205 redb-odm-1.3.1/redb/core/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17117 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/core/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/core/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/core/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 04:17:53.261205 redb-odm-1.3.1/redb/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/interface/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/interface/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/interface/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/interface/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/interface/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/interface/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 04:17:53.261205 redb-odm-1.3.1/redb/json_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/json_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/json_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/json_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/json_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 04:17:53.261205 redb-odm-1.3.1/redb/migo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/migo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/migo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/migo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/migo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 04:17:53.261205 redb-odm-1.3.1/redb/mongo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/mongo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/mongo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/mongo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-09 04:17:37.000000 redb-odm-1.3.1/redb/mongo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 04:17:53.265205 redb-odm-1.3.1/redb_odm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-09 04:17:53.000000 redb-odm-1.3.1/redb_odm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-09 04:17:53.000000 redb-odm-1.3.1/redb_odm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 04:17:53.000000 redb-odm-1.3.1/redb_odm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-09 04:17:53.000000 redb-odm-1.3.1/redb_odm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 04:17:53.000000 redb-odm-1.3.1/redb_odm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 04:17:37.000000 redb-odm-1.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-09 04:17:37.000000 redb-odm-1.3.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-09 04:17:37.000000 redb-odm-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 04:17:53.265205 redb-odm-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-09 04:17:37.000000 redb-odm-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 04:17:53.265205 redb-odm-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-09 04:17:37.000000 redb-odm-1.3.1/tests/test_bson_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-09 04:17:37.000000 redb-odm-1.3.1/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-09 04:17:37.000000 redb-odm-1.3.1/tests/test_i_remember.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-09 04:17:37.000000 redb-odm-1.3.1/tests/test_json_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-07-09 04:17:37.000000 redb-odm-1.3.1/tests/test_mongo_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-09 04:17:37.000000 redb-odm-1.3.1/tests/test_return_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-09 04:17:37.000000 redb-odm-1.3.1/tests/test_soft_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-09 04:17:37.000000 redb-odm-1.3.1/tests/test_unique_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.120695 redb-odm-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 21:27:52.000000 redb-odm-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-27 21:28:08.120695 redb-odm-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 21:27:52.000000 redb-odm-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.112695 redb-odm-1.3.2/redb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/behaviors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/behaviors/i_remember.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/behaviors/soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17117 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb/json_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/json_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/json_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/json_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/json_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb/migo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/migo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/migo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/migo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/migo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb/mongo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/mongo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/mongo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/mongo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/mongo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb_odm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-27 21:28:08.000000 redb-odm-1.3.2/redb_odm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-27 21:28:08.000000 redb-odm-1.3.2/redb_odm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:28:08.000000 redb-odm-1.3.2/redb_odm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-27 21:28:08.000000 redb-odm-1.3.2/redb_odm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 21:28:08.000000 redb-odm-1.3.2/redb_odm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 21:27:52.000000 redb-odm-1.3.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 21:27:52.000000 redb-odm-1.3.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 21:27:52.000000 redb-odm-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:28:08.120695 redb-odm-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-27 21:27:52.000000 redb-odm-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.120695 redb-odm-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_bson_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_i_remember.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_json_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_mongo_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_return_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_soft_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_unique_constraints.py
```

### Comparing `redb-odm-1.3.1/redb/behaviors/i_remember.py` & `redb-odm-1.3.2/redb/behaviors/i_remember.py`

 * *Files 8% similar despite different names*

```diff
@@ -176,38 +176,49 @@
         filter: DocumentData,
         update: DocumentData,
         upsert: bool = False,
         operator: str | None = "$set",
         allow_new_fields: bool = False,
         user_info: Any = None,
     ) -> UpdateOneResult:
+        # TODO: this desperately needs a transaction
+        assert not upsert and operator == "$set" and not allow_new_fields
+        # TODO: fix these missing behaviors or raise appropriate errors
         original_doc = super().find_one(filter=filter)
         new_history = cls._build_history_from_ref(user_info, original_doc)
-        update_result = cls.update_one(
-            filter={"_id": original_doc.id},
-            update=update,
-            upsert=upsert,
-            operator=operator,
-            allow_new_fields=allow_new_fields,
-        )
         cls._historical_insert_one(new_history)
+        original_obj = original_doc.dict()
+        original_obj.pop("_id")
+        if isinstance(update, dict):
+            new_obj = original_obj | update
+        else:
+            new_obj = original_obj | update.dict()
+        new_doc = cls(**new_obj)
+        cls.delete_one(filter=filter)
+        cls.insert_one(new_doc)
+        update_result = UpdateOneResult(matched_count=1, modified_count=1, upserted_id=None)
         return update_result
 
     @classmethod
     def historical_replace_one(
         cls, filter: DocumentData, replacement: DocumentData, user_info: Any = None
     ) -> ReplaceOneResult:
+        # TODO: wrap in ACID transaction
         original_doc = super().find_one(filter=filter)
         new_history = cls._build_history_from_ref(user_info, original_doc)
-        replace_result = cls.replace_one(
-            filter={"_id": original_doc.id},
-            replacement=replacement,
-        )
         cls._historical_insert_one(new_history)
-        return replace_result
+        if isinstance(replacement, dict):
+            new_obj = replacement
+        else:
+            new_obj = replacement.dict()
+        new_obj.pop("_id", "")
+        cls.delete_one(filter=filter)
+        new_doc = cls(**new_obj)
+        new_doc.insert()
+        return ReplaceOneResult(matched_count=1, modified_count=1, upserted_id=None)
 
     @classmethod
     def historical_delete_one(
         cls,
         filter: DocumentData,
         user_info: Any = None,
     ) -> DeleteOneResult:
@@ -221,15 +232,15 @@
     def _build_history_from_ref(
         cls,
         user_info: Any,
         referenced_doc: "IRememberDoc",
     ) -> Dict:
         history_filter = {"ref_id": referenced_doc.id}
         try:
-            histories = cls.historical_find_many(filter=history_filter, fields=["version"], limit=1)
+            histories = cls.historical_find_many(filter=history_filter, fields=["version"], limit=1, sort=SortColumn(name="version", direction=Direction.DESCENDING))
             history = histories[0]
             version = history["version"] + 1  # type: ignore
         except (DocumentNotFound, IndexError):
             version = 1
 
         new_history = referenced_doc.dict(
             ignored_history_fields=False,
```

### Comparing `redb-odm-1.3.1/redb/behaviors/soft_deletion.py` & `redb-odm-1.3.2/redb/behaviors/soft_deletion.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/core/base.py` & `redb-odm-1.3.2/redb/core/base.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/core/document.py` & `redb-odm-1.3.2/redb/core/document.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/core/transaction.py` & `redb-odm-1.3.2/redb/core/transaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import contextlib
 from datetime import datetime
 from typing import Any, ContextManager, Dict, Sequence, Type, TypeVar, overload
 
 import pytz
 from pymongo.errors import DuplicateKeyError
-from redb.behaviors import IRememberDoc
 
+from redb.behaviors import IRememberDoc
 from redb.core.document import (
     Document,
     DocumentData,
     IncludeColumns,
     OptionalDocumentData,
     SortColumns,
     _format_document_data,
@@ -17,14 +17,15 @@
     _format_index,
     _format_sort,
     _get_return_cls,
     _optimize_filter,
     _raise_if_updating_hashable,
     _validate_fields,
 )
+from redb.core.instance import RedB
 from redb.interface.collection import (
     BulkWriteResult,
     Collection,
     DeleteManyResult,
     DeleteOneResult,
     InsertManyResult,
     InsertOneResult,
@@ -37,27 +38,91 @@
     CONFIG_TYPE,
     JSONConfig,
     MigoConfig,
     MongoConfig,
     check_config,
 )
 from redb.interface.errors import UniqueConstraintViolation
+from redb.mongo_system import MongoClient
 
 T = TypeVar("T", bound=Document)
 
 
 class CollectionWrapper:
-    def __init__(self, collection: Collection, history_collection: Collection, collection_class: T) -> None:
+    def __init__(
+        self,
+        collection: Collection,
+        history_collection: Collection,
+        collection_class: T,
+    ) -> None:
         self.__collection = collection
         self.__history_collection = history_collection
         self.__collection_class = collection_class
 
     def _get_driver_collection(self) -> Any:
         return self.__collection._get_driver_collection()
 
+    def switch_db(self, db_name: str) -> "CollectionWrapper":
+        collection_name = self.__collection_class.collection_name()
+
+        client = self.__collection.database.client  # type: ignore
+        db = client.get_database(db_name)
+        collection = db.get_collection(collection_name)
+
+        self.__collection = collection
+
+        return self
+
+    def switch_client(
+        self,
+        config: MongoConfig | dict | None = None,
+        alias: str | None = None,
+    ) -> "CollectionWrapper":
+        collection_name = self.__collection_class.collection_name()
+
+        client = RedB.add_client(config=config, alias=alias)
+
+        old_db_name = self.__collection.database.name  # type: ignore
+        try:
+            db = client.get_database(old_db_name)
+        except:
+            db = client.get_default_database()
+
+        collection = db.get_collection(collection_name)
+
+        self.__collection = collection
+        return self
+
+    def switch(
+        self,
+        db: str | None = None,
+        config: MongoConfig | dict | None = None,
+        alias: str | None = None,
+    ) -> "CollectionWrapper":
+        collection_name = self.__collection_class.collection_name()
+        database_name = self.__collection.database.name  # type: ignore
+
+        if config is not None or alias is not None:
+            client = RedB.add_client(config=config, alias=alias)
+        else:
+            client = self.__collection.database.client  # type: ignore
+
+        if db is not None:
+            _db = client.get_database(db)
+        else:
+            try:
+                _db = client.get_database(database_name)
+            except:
+                _db = client.get_default_database()
+
+        collection = _db.get_collection(collection_name)
+
+        self.__collection = collection
+        return self
+
     def create_indexes(self) -> None:
         indexes = self.__collection_class.get_indexes()
         for index in indexes:
             index = _format_index(index)
             self.__collection.create_index(index)
 
     def find_one(
@@ -136,16 +201,16 @@
         try:
             return self.__collection.insert_one(
                 cls=self.__collection_class,
                 data=data,
             )
         except DuplicateKeyError as e:
             raise UniqueConstraintViolation(dup_keys=e.details["keyValue"])
-        
-    def _historical_insert_one(self,data: DocumentData) -> InsertOneResult:
+
+    def _historical_insert_one(self, data: DocumentData) -> InsertOneResult:
         if self.__history_collection is None:
             raise ValueError("Base class does not inherit from IRememberDoc")
 
         data = _format_document_data(data)
         try:
             return self.__history_collection.insert_one(
                 cls=self.__collection_class,
@@ -247,17 +312,19 @@
         upsert: bool = False,
         operator: str | None = "$set",
         allow_new_fields: bool = False,
         user_info: Any = None,
     ) -> UpdateOneResult:
         if self.__history_collection is None:
             raise ValueError("Base class does not inherit from IRememberDoc")
-        
+
         original_doc = self.find_one(filter=filter)
-        new_history = self.__collection_class._build_history_from_ref(user_info, original_doc)
+        new_history = self.__collection_class._build_history_from_ref(
+            user_info, original_doc
+        )
         update_result = self.update_one(
             filter={"_id": original_doc.id},
             update=update,
             upsert=upsert,
             operator=operator,
             allow_new_fields=allow_new_fields,
         )
@@ -300,25 +367,27 @@
 
     def delete_one(self, filter: DocumentData) -> DeleteOneResult:
         filter = _format_document_data(filter)
         return self.__collection.delete_one(
             cls=self.__collection_class,
             filter=filter,
         )
-    
+
     def historical_delete_one(
         self,
         filter: DocumentData,
         user_info: Any = None,
     ) -> DeleteOneResult:
         if self.__history_collection is None:
             raise ValueError("Base class does not inherit from IRememberDoc")
-        
+
         original_doc = self.find_one(filter=filter)
-        new_history = self.__collection_class._build_history_from_ref(user_info, original_doc)
+        new_history = self.__collection_class._build_history_from_ref(
+            user_info, original_doc
+        )
         delete_result = self.delete_one(filter={"_id": original_doc.id})
         self._historical_insert_one(new_history)
         return delete_result
 
     def delete_many(self, filter: DocumentData) -> DeleteManyResult:
         filter = _format_document_data(filter)
         return self.__collection.delete_many(
@@ -365,34 +434,37 @@
         collection = database.get_collection(collection)
     else:
         collection_name = collection.collection_name()
         driver_history_collection = None
         if issubclass(collection, IRememberDoc):
             history_collection_name = collection.history_collection_name()
             driver_history_collection = database.get_collection(history_collection_name)
-        
+
         driver_collection = database.get_collection(collection_name)
-        collection = CollectionWrapper(driver_collection, driver_history_collection, collection)
+        collection = CollectionWrapper(
+            driver_collection, driver_history_collection, collection
+        )
 
     yield collection
 
     if new_client:
         client.close()
 
 
 def get_client(backend: str | None, config: CONFIG_TYPE):
     if backend == "json" or (backend is None and check_config(config, JSONConfig)):
         from redb.json_system import JSONClient
 
         return True, JSONClient(config)
 
     elif backend == "mongo" or (backend is None and check_config(config, MongoConfig)):
-        from redb.mongo_system import MongoClient
+        from redb.core.instance import RedB
 
-        return True, MongoClient(config)
+        client = RedB.add_client(config)
+        return True, client
 
     elif backend == "migo" and (backend is None and check_config(config, MigoConfig)):
         from redb.migo_system import MigoClient
 
         return True, MigoClient(config)
 
     else:
```

### Comparing `redb-odm-1.3.1/redb/core/utils.py` & `redb-odm-1.3.2/redb/core/utils.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/interface/client.py` & `redb-odm-1.3.2/redb/interface/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/interface/collection.py` & `redb-odm-1.3.2/redb/interface/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/interface/configs.py` & `redb-odm-1.3.2/redb/interface/configs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/interface/database.py` & `redb-odm-1.3.2/redb/interface/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/interface/errors.py` & `redb-odm-1.3.2/redb/interface/errors.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/interface/fields.py` & `redb-odm-1.3.2/redb/interface/fields.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/interface/results.py` & `redb-odm-1.3.2/redb/interface/results.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/json_system/client.py` & `redb-odm-1.3.2/redb/json_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/json_system/collection.py` & `redb-odm-1.3.2/redb/json_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/json_system/database.py` & `redb-odm-1.3.2/redb/json_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/migo_system/client.py` & `redb-odm-1.3.2/redb/migo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/migo_system/collection.py` & `redb-odm-1.3.2/redb/migo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/migo_system/database.py` & `redb-odm-1.3.2/redb/migo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/mongo_system/client.py` & `redb-odm-1.3.2/redb/mongo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/mongo_system/collection.py` & `redb-odm-1.3.2/redb/mongo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb/mongo_system/database.py` & `redb-odm-1.3.2/redb/mongo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/redb_odm.egg-info/SOURCES.txt` & `redb-odm-1.3.2/redb_odm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/setup.py` & `redb-odm-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/tests/test_bson_objs.py` & `redb-odm-1.3.2/tests/test_bson_objs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/tests/test_hashing.py` & `redb-odm-1.3.2/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/tests/test_i_remember.py` & `redb-odm-1.3.2/tests/test_i_remember.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     name: str
     breed: str = "Domestic Shorthair"
     created_by: str
     retired_by: Optional[str] = None
 
     @classmethod
     def get_hashable_fields(cls) -> list[ClassField]:
-        return [cls.name]  # type: ignore
+        return [cls.name, cls.breed]  # type: ignore
 
     @classmethod
     def collection_name(cls) -> str:
         return "cats"
 
 
 @pytest.fixture(scope="module", autouse=True)
@@ -86,14 +86,34 @@
     assert len(hist_cats) == 1
     hist_cat = hist_cats[0]
     assert hist_cat["version"] == 1
     assert hist_cat["created_by"] == creator_email
     assert hist_cat["retired_by"] == user_email
 
 
+def test_historical_version_incrementing(db: Database, fluffy_cat: Cat):
+    obj = fluffy_cat
+    obj.insert()
+    Cat.historical_delete_one({"_id": obj.id}, user_info="user1@email.com")
+    Cat(**obj.dict(exclude={"created_at"})).insert()
+    Cat.historical_delete_one({"_id": obj.id}, user_info="user2@email.com")
+    hist_cats = list(db["cats-history"].find({"name": fluffy_cat.name}, sort=[("version", -1)]))
+    assert len(hist_cats) == 2
+    hist_cat = hist_cats[0]
+    assert hist_cat["version"] == 2
+    assert hist_cat["retired_by"] == "user2@email.com"
+    Cat(**obj.dict(exclude={"created_at"})).insert()
+    Cat.historical_delete_one({"_id": obj.id}, user_info="user3@email.com")
+    hist_cats = list(db["cats-history"].find({"name": fluffy_cat.name}, sort=[("version", -1)]))
+    assert len(hist_cats) == 3
+    hist_cat = hist_cats[0]
+    assert hist_cat["version"] == 3
+    assert hist_cat["retired_by"] == "user3@email.com"
+
+
 @pytest.mark.order(after="test_historical_delete_one")
 def test_historical_find_one(user_email, pony_cat: Cat):
     pony_cat.insert()
     del_res = Cat.historical_delete_one({"_id": pony_cat.id}, user_info=user_email)
     assert del_res.deleted_count
     history = Cat.historical_find_one(filter={"name": pony_cat.name})
     assert history.version == 1
@@ -136,14 +156,15 @@
     assert hist_cat["created_by"] == creator_email
     assert hist_cat["retired_by"] == user_email
     assert hist_cat["breed"] == fluffy_cat.breed
     cats = list(db["cats"].find({"name": fluffy_cat.name}))
     assert len(cats) == 1
     cat = cats[0]
     assert cat["breed"] == "American Bobtail"
+    assert cat["_id"] != fluffy_cat.id
 
 
 def test_historical_replace_one(db: Database, creator_email: str, user_email: str, fluffy_cat: Cat):
     fluffy_cat.insert()
     old_cat_id = fluffy_cat.id
     replaced_result = Cat.historical_replace_one(
         {"name": fluffy_cat.name}, {**fluffy_cat.dict(), "breed": "American Bobtail"}, user_info=user_email
@@ -157,7 +178,8 @@
     assert hist_cat["created_by"] == creator_email
     assert hist_cat["retired_by"] == user_email
     assert hist_cat["breed"] == fluffy_cat.breed
     cats = list(db["cats"].find({"name": fluffy_cat.name}))
     assert len(cats) == 1
     cat = cats[0]
     assert cat["breed"] == "American Bobtail"
+    assert cat["_id"] != fluffy_cat.id
```

### Comparing `redb-odm-1.3.1/tests/test_json_client.py` & `redb-odm-1.3.2/tests/test_json_client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/tests/test_mongo_system.py` & `redb-odm-1.3.2/tests/test_mongo_system.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/tests/test_return_cls.py` & `redb-odm-1.3.2/tests/test_return_cls.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/tests/test_soft_deletion.py` & `redb-odm-1.3.2/tests/test_soft_deletion.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.1/tests/test_unique_constraints.py` & `redb-odm-1.3.2/tests/test_unique_constraints.py`

 * *Files identical despite different names*

