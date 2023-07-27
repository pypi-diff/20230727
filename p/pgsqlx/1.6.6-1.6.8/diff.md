# Comparing `tmp/pgsqlx-1.6.6.tar.gz` & `tmp/pgsqlx-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.6.6.tar", last modified: Wed Jul 26 08:49:29 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.6.8.tar", last modified: Thu Jul 27 11:39:37 2023, max compression
```

## Comparing `pgsqlx-1.6.6.tar` & `pgsqlx-1.6.8.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:49:29.000000 pgsqlx-1.6.6/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:49:29.000000 pgsqlx-1.6.6/pgsqlx/
--rw-rw-rw-   0        0        0      156 2023-07-26 07:07:24.000000 pgsqlx-1.6.6/pgsqlx/constant.py
--rw-rw-rw-   0        0        0     3107 2023-07-26 07:17:42.000000 pgsqlx-1.6.6/pgsqlx/db.py
--rw-rw-rw-   0        0        0     2002 2023-07-26 07:26:12.000000 pgsqlx-1.6.6/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0     1532 2023-07-26 07:59:16.000000 pgsqlx-1.6.6/pgsqlx/engin.py
--rw-rw-rw-   0        0        0     1896 2023-07-26 07:25:39.000000 pgsqlx-1.6.6/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0     6066 2023-07-26 07:29:24.000000 pgsqlx-1.6.6/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     3310 2023-07-26 07:10:47.000000 pgsqlx-1.6.6/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0      349 2023-07-26 05:51:44.000000 pgsqlx-1.6.6/pgsqlx/sql_support.py
--rw-rw-rw-   0        0        0      660 2023-07-26 08:45:19.000000 pgsqlx-1.6.6/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:49:29.000000 pgsqlx-1.6.6/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-26 08:49:29.000000 pgsqlx-1.6.6/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-26 08:49:29.000000 pgsqlx-1.6.6/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4612 2023-07-26 08:49:29.000000 pgsqlx-1.6.6/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-26 08:49:29.000000 pgsqlx-1.6.6/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      357 2023-07-26 08:49:29.000000 pgsqlx-1.6.6/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 08:49:29.000000 pgsqlx-1.6.6/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4612 2023-07-26 08:49:29.000000 pgsqlx-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     4096 2023-07-25 08:21:22.000000 pgsqlx-1.6.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-26 08:49:29.000000 pgsqlx-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1237 2023-07-26 08:49:07.000000 pgsqlx-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/
+drwxrwxrwx   0        0        0        0 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx/
+-rw-rw-rw-   0        0        0      156 2023-07-26 07:07:24.000000 pgsqlx-1.6.8/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0     1080 2023-07-27 04:20:30.000000 pgsqlx-1.6.8/pgsqlx/db.py
+-rw-rw-rw-   0        0        0      695 2023-07-27 04:21:57.000000 pgsqlx-1.6.8/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0      544 2023-07-27 04:10:16.000000 pgsqlx-1.6.8/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0     2283 2023-07-27 04:21:57.000000 pgsqlx-1.6.8/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0     3318 2023-07-27 04:21:26.000000 pgsqlx-1.6.8/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0      508 2023-07-27 11:38:44.000000 pgsqlx-1.6.8/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4612 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      319 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4612 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-07-25 08:21:22.000000 pgsqlx-1.6.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:39:37.000000 pgsqlx-1.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2023-07-27 11:39:31.000000 pgsqlx-1.6.8/setup.py
```

### Comparing `pgsqlx-1.6.6/pgsqlx/sql_mapper.py` & `pgsqlx-1.6.8/pgsqlx/sql_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sqlexec
 import functools
 from .log_support import logger
-from .engin import PostgresEngin
 from sqlbatis.support import SqlAction
+from sqlbatis.engin import PostgresEngin
 from sqlbatis.sql_support import simple_sql, get_named_sql_args
 from sqlbatis.sql_holder import get_sql_model, do_get_sql
 from sqlbatis.sql_mapper import get_exec_func, before, get_select_func
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
```

### Comparing `pgsqlx-1.6.6/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.6.8/pgsqlx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.6.6
+Version: 1.6.8
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.6.6/PKG-INFO` & `pgsqlx-1.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.6.6
+Version: 1.6.8
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.6.6/README.rst` & `pgsqlx-1.6.8/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.6/setup.py` & `pgsqlx-1.6.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # 'Jinja2>=2.7.0',
         # 'psycopg2>=2.7.4',
         'sqlx-batis>=0.0.9',
     ],
-    version='1.6.6',
+    version='1.6.8',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

