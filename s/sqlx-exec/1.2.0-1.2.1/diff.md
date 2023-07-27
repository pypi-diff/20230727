# Comparing `tmp/sqlx-exec-1.2.0.tar.gz` & `tmp/sqlx-exec-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.2.0.tar", last modified: Wed Jul 26 08:38:02 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.2.1.tar", last modified: Thu Jul 27 02:00:27 2023, max compression
```

## Comparing `sqlx-exec-1.2.0.tar` & `sqlx-exec-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:38:02.000000 sqlx-exec-1.2.0/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     2770 2023-07-26 08:38:02.000000 sqlx-exec-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2261 2023-07-26 08:32:11.000000 sqlx-exec-1.2.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-26 08:38:02.000000 sqlx-exec-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1161 2023-07-26 08:37:31.000000 sqlx-exec-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:38:02.000000 sqlx-exec-1.2.0/sqlexec/
--rw-rw-rw-   0        0        0      136 2023-07-26 00:53:39.000000 sqlx-exec-1.2.0/sqlexec/constant.py
--rw-rw-rw-   0        0        0     1410 2023-07-26 08:07:43.000000 sqlx-exec-1.2.0/sqlexec/engin.py
--rw-rw-rw-   0        0        0    11421 2023-07-26 07:55:26.000000 sqlx-exec-1.2.0/sqlexec/exec.py
--rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.2.0/sqlexec/log_support.py
--rw-rw-rw-   0        0        0      833 2023-07-25 17:51:41.000000 sqlx-exec-1.2.0/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1157 2023-07-26 02:18:21.000000 sqlx-exec-1.2.0/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.2.0/sqlexec/support.py
--rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.2.0/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:38:02.000000 sqlx-exec-1.2.0/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-26 08:38:01.000000 sqlx-exec-1.2.0/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 13:22:36.000000 sqlx-exec-1.2.0/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2770 2023-07-26 08:38:01.000000 sqlx-exec-1.2.0/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-07-26 08:38:02.000000 sqlx-exec-1.2.0/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 08:38:01.000000 sqlx-exec-1.2.0/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 02:00:27.000000 sqlx-exec-1.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2770 2023-07-27 02:00:27.000000 sqlx-exec-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2261 2023-07-26 08:32:11.000000 sqlx-exec-1.2.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-27 02:00:27.000000 sqlx-exec-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-07-27 01:59:40.000000 sqlx-exec-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:00:27.000000 sqlx-exec-1.2.1/sqlexec/
+-rw-rw-rw-   0        0        0      268 2023-07-26 15:50:37.000000 sqlx-exec-1.2.1/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     1033 2023-07-26 15:55:33.000000 sqlx-exec-1.2.1/sqlexec/engin.py
+-rw-rw-rw-   0        0        0    11401 2023-07-27 01:58:10.000000 sqlx-exec-1.2.1/sqlexec/exec.py
+-rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.2.1/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0      833 2023-07-25 17:51:41.000000 sqlx-exec-1.2.1/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1134 2023-07-26 14:36:38.000000 sqlx-exec-1.2.1/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.2.1/sqlexec/support.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.2.1/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:00:27.000000 sqlx-exec-1.2.1/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-27 02:00:27.000000 sqlx-exec-1.2.1/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 13:22:36.000000 sqlx-exec-1.2.1/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2770 2023-07-27 02:00:27.000000 sqlx-exec-1.2.1/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-07-27 02:00:27.000000 sqlx-exec-1.2.1/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 02:00:27.000000 sqlx-exec-1.2.1/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.2.0/LICENSE` & `sqlx-exec-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.0/PKG-INFO` & `sqlx-exec-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.2.0
+Version: 1.2.1
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
```

### Comparing `sqlx-exec-1.2.0/README.rst` & `sqlx-exec-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.0/setup.py` & `sqlx-exec-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.0',
+    version='1.2.1',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.2.0/sqlexec/engin.py` & `sqlx-exec-1.2.1/sqlexec/engin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,36 @@
 from typing import Sequence
 from functools import lru_cache
-from .constant import CACHE_SIZE
+from .constant import CACHE_SIZE, UNKNOW
 
 _ENGIN = None
 
 
 class Engin:
-    def __init__(self, name=None):
+    def __init__(self, name=UNKNOW):
         self.name = name
 
     @classmethod
-    def init(cls, name=None):
+    def init(cls, name=UNKNOW):
         global _ENGIN
         if _ENGIN:
-            if name and not _ENGIN.name:
+            if _ENGIN.name == UNKNOW and name != UNKNOW:
                 _ENGIN.name = name
         else:
             _ENGIN = cls(name)
 
     @staticmethod
     def current_engin():
         global _ENGIN
-        return _ENGIN.name
+        if _ENGIN:
+            return _ENGIN.name
+        return None
 
     @classmethod
     @lru_cache(maxsize=CACHE_SIZE)
-    def create_insert_sql(cls, table: str, cols: Sequence[str]):
-        return _ENGIN._create_insert_sql(table, cols)
-
-    @staticmethod
-    def page_sql_args(require_limit, sql: str, start: int, page_size: int, *args):
-        return _ENGIN._page_sql_args(require_limit, sql, start, page_size, *args)
-
-    @staticmethod
-    def get_select_key(*args, **kwargs):
-        return _ENGIN._get_select_key(*args, **kwargs)
-
-    @staticmethod
-    @lru_cache(maxsize=CACHE_SIZE)
-    def get_table_columns(table: str):
-        return _ENGIN._get_table_columns(table)
+    def create_insert_sql_intf(cls, table: str, cols: Sequence[str]):
+        return _ENGIN.create_insert_sql(table, cols)
 
     @staticmethod
-    def _create_insert_sql(table: str, cols: Sequence[str]):
+    def create_insert_sql(table: str, cols: Sequence[str]):
         columns, placeholders = zip(*[('{}'.format(col), '?') for col in cols])
         return 'INSERT INTO {}({}) VALUES({})'.format(table, ', '.join(columns), ','.join(placeholders))
```

### Comparing `sqlx-exec-1.2.0/sqlexec/exec.py` & `sqlx-exec-1.2.1/sqlexec/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 import importlib
 from .engin import Engin
 from . import sql_support
-from .constant import DRIVERS
+from .constant import DRIVERS, MYSQL_CONNECTOR, UNKNOW
 from .log_support import logger, insert_log, save_log, get_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
 
 _DB_CTX = None
 _SHOW_SQL = False
 
 
@@ -21,30 +21,29 @@
     if debug:
         from logging import DEBUG
         logger.setLevel(DEBUG)
 
     if driver:
         if driver not in DRIVERS:
             logger.warning(f"Driver '{driver}' not support now, may be you should adapte it youself.")
-        engin_name = DRIVERS.get(driver)
-        creator = _import(driver, engin_name)
+        engin = DRIVERS.get(driver)
+        creator = _import(driver, engin)
     else:
         current_engin = Engin.current_engin()
-        drivers = dict(filter(lambda x: x[1] == current_engin, DRIVERS.items())) if current_engin else DRIVERS
-        for driver in drivers:
+        drivers = dict(filter(lambda x: x[1] == current_engin, DRIVERS.items())) if current_engin and current_engin != UNKNOW else DRIVERS
+        for driver, engin in drivers.items():
             try:
                 creator = importlib.import_module(driver)
-                engin_name = DRIVERS.get(driver)
                 break
             except ModuleNotFoundError:
                 pass
         if not creator:
-            raise DBError(f"You may forget install driver, now suppor: {list(DRIVERS.keys())}")
+            raise DBError(f"You may forget install driver, now support: {list(DRIVERS.keys())}")
 
-    if 'mysql.connector' == driver:
+    if MYSQL_CONNECTOR == driver:
         prepared = True
         kwargs['pool_size'] = pool_size
 
     if pool_size <= 0 or prepared:
         connect = lambda: creator.connect(**kwargs)
     else:
         from .pooling import pooled_connect
@@ -52,26 +51,26 @@
 
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
         _SHOW_SQL = show_sql
         _DB_CTX = DBCtx(connect=connect, prepared=prepared)
 
-    Engin.init(engin_name)
+    Engin.init(engin)
     if pool_size > 0:
-        logger.info("Inited db engine <%s> of %s with driver: '%s' and pool size: %d." % (hex(id(_DB_CTX)), engin_name, driver, pool_size))
+        logger.info("Inited db engin <%s> of %s with driver: '%s' and pool size: %d." % (hex(id(_DB_CTX)), engin, driver, pool_size))
     else:
-        logger.info("Inited db engine <%s> of %s with driver: '%s'." % (hex(id(_DB_CTX)), engin_name, driver))
+        logger.info("Inited db engin <%s> of %s with driver: '%s'." % (hex(id(_DB_CTX)), engin, driver))
 
-def _import(driver, engin_name):
+def _import(driver, engin):
 
     try:
         return importlib.import_module(driver)
     except ModuleNotFoundError:
-        raise DBError(f"Import {engin_name} driver '{driver}' failed, please sure it was installed or change other driver.")
+        raise DBError(f"Import {engin} driver '{driver}' failed, please sure it was installed or change other driver.")
 
 
 def _del_kwarg(key, kwargs):
     if key in kwargs:
         del kwargs[key]
```

### Comparing `sqlx-exec-1.2.0/sqlexec/log_support.py` & `sqlx-exec-1.2.1/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.0/sqlexec/pooling.py` & `sqlx-exec-1.2.1/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.0/sqlexec/sql_support.py` & `sqlx-exec-1.2.1/sqlexec/sql_support.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import re
 from .engin import Engin
 from typing import Sequence
-from .log_support import logger
 from functools import lru_cache
 from .constant import CACHE_SIZE, NAMED_REGEX
 
 def insert_sql_args(table: str, **kwargs):
     cols, args = zip(*kwargs.items())
-    sql = Engin.create_insert_sql(table, cols)
+    sql = Engin.create_insert_sql_intf(table, cols)
     return sql, args
 
 
 def get_batch_args(*args):
     return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Sequence) else args
 
 
 def batch_insert_sql_args(table: str, *args):
     args = get_batch_args(*args)
     args = [zip(*arg.items()) for arg in args]  # [(cols, args)]
     cols, args = zip(*args)  # (cols), (args)
-    sql = Engin.create_insert_sql(table, cols[0])
+    sql = Engin.create_insert_sql_intf(table, cols[0])
     return sql, args
 
 
 def batch_named_sql_args(sql: str, *args):
     args = get_batch_args(*args)
     args = [get_named_args(sql, **arg) for arg in args]
     sql = get_named_sql(sql)
```

### Comparing `sqlx-exec-1.2.0/sqlexec/support.py` & `sqlx-exec-1.2.1/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.0/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.2.1/sqlx_exec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.2.0
+Version: 1.2.1
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
```

