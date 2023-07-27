# Comparing `tmp/sqlx-batis-0.0.9.tar.gz` & `tmp/sqlx-batis-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.0.9.tar", last modified: Wed Jul 26 08:39:15 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.1.0.tar", last modified: Thu Jul 27 11:31:34 2023, max compression
```

## Comparing `sqlx-batis-0.0.9.tar` & `sqlx-batis-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/
--rw-rw-rw-   0        0        0     3373 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2892 2023-07-26 08:34:15.000000 sqlx-batis-0.0.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-26 08:38:48.000000 sqlx-batis-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlbatis/
--rw-rw-rw-   0        0        0      782 2023-07-26 05:51:44.000000 sqlx-batis-0.0.9/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     6894 2023-07-26 08:13:40.000000 sqlx-batis-0.0.9/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6234 2023-07-26 04:35:24.000000 sqlx-batis-0.0.9/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     1391 2023-07-26 08:20:25.000000 sqlx-batis-0.0.9/sqlbatis/engin.py
--rw-rw-rw-   0        0        0     2324 2023-07-26 05:27:34.000000 sqlx-batis-0.0.9/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    34936 2023-07-26 06:54:32.000000 sqlx-batis-0.0.9/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.0.9/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.0.9/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     4939 2023-07-26 06:52:58.000000 sqlx-batis-0.0.9/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1646 2023-07-26 05:39:42.000000 sqlx-batis-0.0.9/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.0.9/sqlbatis/support.py
--rw-rw-rw-   0        0        0      779 2023-07-26 07:56:33.000000 sqlx-batis-0.0.9/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3373 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      464 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/
+-rw-rw-rw-   0        0        0     3373 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2892 2023-07-26 08:34:15.000000 sqlx-batis-0.1.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-27 11:30:05.000000 sqlx-batis-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlbatis/
+-rw-rw-rw-   0        0        0      834 2023-07-26 14:53:18.000000 sqlx-batis-0.1.0/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     8669 2023-07-27 04:44:35.000000 sqlx-batis-0.1.0/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6449 2023-07-27 04:44:35.000000 sqlx-batis-0.1.0/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     4377 2023-07-27 04:39:23.000000 sqlx-batis-0.1.0/sqlbatis/engin.py
+-rw-rw-rw-   0        0        0     3836 2023-07-27 03:54:22.000000 sqlx-batis-0.1.0/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    38924 2023-07-27 04:44:35.000000 sqlx-batis-0.1.0/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.0/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.0/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5238 2023-07-27 04:44:35.000000 sqlx-batis-0.1.0/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.0/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.0/sqlbatis/support.py
+-rw-rw-rw-   0        0        0      603 2023-07-27 11:30:50.000000 sqlx-batis-0.1.0/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3373 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      464 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 11:31:34.000000 sqlx-batis-0.1.0/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.0.9/PKG-INFO` & `sqlx-batis-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.0.9
+Version: 0.1.0
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `sqlx-batis-0.0.9/README.rst` & `sqlx-batis-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.9/setup.py` & `sqlx-batis-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlbatis'],
     description="sqlx-batis is a sql executor for Python like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.2.0',
+        'sqlx-exec>=1.2.2',
     ],
-    version='0.0.9',
+    version='0.1.0',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.0.9/sqlbatis/constant.py` & `sqlx-batis-0.1.0/sqlbatis/constant.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from sqlexec.constant import MYSQL, POSTGRESQL
+
 LIMIT_1 = 1
 
 NO_LIMIT = 0
 
 CACHE_SIZE = 256
 
 MYSQL_SELECT_KEY = "SELECT LAST_INSERT_ID()"
@@ -14,7 +16,8 @@
 
 DYNAMIC_REGEX = '{%|{{|}}|%}'
 
 DEFAULT_KEY_FIELD = 'id'
 
 KEY, SELECT_KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY = '__key__', '__select_key__', '__table__', '__update_by__', '__update_time__',\
     '__del_flag__', '__key_strategy__'
+
```

### Comparing `sqlx-batis-0.0.9/sqlbatis/db.py` & `sqlx-batis-0.1.0/sqlbatis/db.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,30 @@
-from . import sql_support
-from .log_support import sql_log, do_sql_log
+from . import sql_support, Engin, DBError
+from .log_support import sql_log, do_sql_log, save_log, do_page_log, page_log
 
 # Don't remove. Import for not repetitive implementation
-from sqlexec import insert, save, save_sql, batch_insert, batch_execute, execute as supper_execute, get as supper_get, query_one as supper_query_one,\
+from sqlexec import insert, save as save_select_key, save_sql, batch_insert, batch_execute, execute as supper_execute, get as supper_get, query_one as supper_query_one,\
     query as supper_query, select as supper_select, select_one as supper_select_one
 
 
-# ----------------------------------------------------------Update function------------------------------------------------------------------
+def save(table: str, **kwargs):
+    """
+    Insert data into table, return primary key.
+    :param table: table
+    :param kwargs:
+    :return: Primary key
+    """
+    save_log(table, **kwargs)
+    try:
+        select_key = Engin.get_select_key_intf(table=table)
+    except NotImplementedError:
+        raise DBError(f"Expect 'select_key' but not. you may should use 'save_select_key' func with 'select_key'.")
+    return save_select_key(select_key, table, **kwargs)
+
+
 def execute(sql: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO user(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
     """
     sql_log('execute', sql, *args, **kwargs)
@@ -104,53 +118,76 @@
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     return supper_query(sql, *args)
 
 
+def do_select(sql: str, *args):
+    """
+    execute select SQL and return unique result or list results(tuple).
+    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+    """
+    return supper_select(sql, *args)
+
+
 def do_query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_query_one', sql, *args)
     sql, args = sql_support.limit_one_sql_args(sql, *args)
     return supper_query_one(sql, *args)
 
 
-def do_select(sql: str, *args):
-    """
-    execute select SQL and return unique result or list results(tuple).
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-    """
-    return supper_select(sql, *args)
-
-
 def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_select_one', sql, *args)
     sql, args = sql_support.limit_one_sql_args(sql, *args)
     return supper_select_one(sql, *args)
 
 
-# def do_query_page(sql: str, page_num=1, page_size=10, *args):
-#     """
-#     Execute select SQL and return list results(dict).
-#     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-#     """
-#     do_page_log('select_page', sql.strip(), page_num, page_size, args)
-#     sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
-#     return supper_query(sql, *args)
-
-
-# def do_select_page(sql: str, page_num=1, page_size=10, *args):
-#     """
-#     Execute select SQL and return list results(dict).
-#     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-#     """
-#     do_page_log('do_select_page', sql.strip(), page_num, page_size, args)
-#     sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
-#     return supper_select(sql, *args)
+# ----------------------------------------------------------Page function------------------------------------------------------------------
+def query_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
+    """
+    Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
+    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+         SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+    """
+    page_log('query_page', sql, page_num, page_size, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
+    return do_query_page(sql, page_num, page_size, *args)
+
+
+def select_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
+    """
+    Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
+    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+         SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+    """
+    page_log('select_page', sql, page_num, page_size, *args, **kwargs)
+    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
+    return do_select_page(sql, page_num, page_size, *args)
+
+
+def do_query_page(sql: str, page_num=1, page_size=10, *args):
+    """
+    Execute select SQL and return list results(dict).
+    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+    """
+    do_page_log('select_page', sql.strip(), page_num, page_size, args)
+    sql, args = Engin.get_page_sql_args_intf(sql, page_num, page_size, *args)
+    return supper_query(sql, *args)
+
+
+def do_select_page(sql: str, page_num=1, page_size=10, *args):
+    """
+    Execute select SQL and return list results(dict).
+    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+    """
+    do_page_log('do_select_page', sql.strip(), page_num, page_size, args)
+    sql, args = Engin.get_page_sql_args_intf(sql, page_num, page_size, *args)
+    return supper_select(sql, *args)
```

### Comparing `sqlx-batis-0.0.9/sqlbatis/dbx.py` & `sqlx-batis-0.1.0/sqlbatis/dbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from .sql_support import get_batch_args
-from . import Engin, sql_holder as holder
-from .log_support import logger, sql_id_log
+from . import Engin, DBError, sql_holder as holder
+from .log_support import logger, sql_id_log, page_sql_id_log
 
 # Don't remove. Import for not repetitive implementation
-from .db import(do_execute, insert, save_sql, batch_insert, batch_execute as db_batch_execute, do_get, do_query, do_query_one, do_select, do_select_one)
+from .db import(do_execute, insert, save_sql, batch_insert, batch_execute as db_batch_execute, do_get, do_query, do_query_one, do_select, \
+                do_select_one, do_select_page, do_query_page)
 
 
 def save(sql_id: str, *args, **kwargs):
     """
     Execute insert SQL, return primary key.
     :return: Primary key
     """
     sql_id_log('dbx.save', sql_id, *args, **kwargs)
     sql_model = holder.get_sql_model(sql_id)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
     select_key = sql_model.select_key
     if not select_key:
-        select_key = Engin.get_select_key()
+        try:
+            select_key = Engin.get_select_key_intf(sql=sql)
+        except NotImplementedError:
+            raise DBError(f"Expect 'select_key' but not. you can set it in mapper file with 'selectKey'.")
     return save_sql(select_key, sql, *args)
 
 
 def execute(sql_id: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
@@ -102,28 +106,28 @@
          SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_id_log('select_one', sql_id, *args, **kwargs)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
-# def query_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
-#     """
-#     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-#     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-#          SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-#     """
-#     page_sql_id_log('query_page', sql_id, page_num, page_size, *args, **kwargs)
-#     sql, args = holder.get_sql(sql_id, *args, **kwargs)
-#     return do_query_page(sql, page_num, page_size, *args)
-
-
-# def select_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
-#     """
-#     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-#     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-#          SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-#     """
-#     page_sql_id_log('select_page', sql_id, page_num, page_size, *args, **kwargs)
-#     sql, args = holder.get_sql(sql_id, *args, **kwargs)
-#     return do_select_page(sql, page_num, page_size, *args)
+def query_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
+    """
+    Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
+    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+         SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+    """
+    page_sql_id_log('query_page', sql_id, page_num, page_size, *args, **kwargs)
+    sql, args = holder.get_sql(sql_id, *args, **kwargs)
+    return do_query_page(sql, page_num, page_size, *args)
+
+
+def select_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
+    """
+    Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
+    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+         SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+    """
+    page_sql_id_log('select_page', sql_id, page_num, page_size, *args, **kwargs)
+    sql, args = holder.get_sql(sql_id, *args, **kwargs)
+    return do_select_page(sql, page_num, page_size, *args)
```

### Comparing `sqlx-batis-0.0.9/sqlbatis/log_support.py` & `sqlx-batis-0.1.0/sqlbatis/log_support.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,38 @@
 from sqlexec.log_support import logger
 
+
+def save_log(table, **kwargs):
+    logger.debug("Exec func 'pgsqlx.db.save' \n\t Table: '%s', kwargs: %s" % (table, kwargs))
+
+
 def sql_log(function: str, sql: str, *args, **kwargs):
     logger.debug("Exec func 'sqlbatis.db.%s' \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (function, sql.strip(), args, kwargs))
 
+
 def do_sql_log(function: str, sql: str, *args):
     logger.debug("Exec func 'sqlbatis.db.%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
 
+
+def do_page_log(function: str, sql: str, page_num, page_size, *args):
+    logger.debug(
+        "Exec func 'sqlbatis.db.%s', page_num: %d, page_size: %d \n\t sql: %s \n\t args: %s" % (function, page_num, page_size, sql.strip(), args))
+
+
+def page_log(function: str, sql: str, page_num, page_size, *args, **kwargs):
+    logger.debug("Exec func 'sqlbatis.db.%s', page_num: %d, page_size: %d \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (
+                 function, page_num, page_size, sql.strip(), args, kwargs))
+
+
+def page_sql_id_log(function: str, sql_id: str, page_num, page_size, *args, **kwargs):
+    logger.debug("Exec func 'sqlbatis.dbx.%s', page_num: %d, page_size: %d, sql_id: %s, args: %s, kwargs: %s" % (function, page_num, page_size, sql_id, args, kwargs))
+
+
 def sql_id_log(function: str, sql_id: str, *args, **kwargs):
-    logger.debug("Exec func 'sqlbatis.%s', sql_id: %s, args: %s, kwargs: %s" % (function, sql_id.strip(), args, kwargs))
+    logger.debug("Exec func 'sqlbatis.dbx.%s', sql_id: %s, args: %s, kwargs: %s" % (function, sql_id.strip(), args, kwargs))
 
 
 def orm_insert_log(function, class_name, **kwargs):
     logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
 
 
 def orm_delete_by_id_log(function, class_name, _id, update_by):
@@ -24,15 +45,15 @@
 
 def orm_inst_log(function, class_name):
     logger.debug("Exec func 'sqlbatis.orm.Model.%s', Class: '%s'" % (function, class_name))
 
 
 def orm_logical_delete_by_ids_log(function, class_name, ids, update_by, batch_size):
     logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
-    function, class_name, ids, update_by, batch_size))
+        function, class_name, ids, update_by, batch_size))
 
 
 def orm_count_log(function, class_name, **kwargs):
     logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
 
 
 def orm_find_log(function, class_name, *fields, **kwargs):
@@ -41,7 +62,17 @@
 
 def orm_find_by_id_log(function, class_name, _id, *fields):
     logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, fields: %s" % (function, class_name, _id, fields))
 
 
 def orm_find_by_ids_log(function, class_name, ids, *fields):
     logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', ids: %s, fields: %s" % (function, class_name, ids, fields))
+
+
+def orm_page_log(function, page_num, page_size, class_name, *fields, **kwargs):
+    logger.debug("Exec func 'pgsqlx.orm.Model.%s', page_num: %d, page_size: %d \n\t Class: '%s', fields: %s, kwargs: %s" % (
+        function, page_num, page_size, class_name, fields, kwargs))
+
+
+def orm_by_page_log(function, page_num, page_size, class_name, where, *args, **kwargs):
+    logger.debug("Exec func 'sqlx-batis.orm.Model.%s', page_num: %d, page_size: %d \n\t Class: '%s', where: %s, args: %s, kwargs: %s" % (
+        function, page_num, page_size, class_name, where, args, kwargs))
```

### Comparing `sqlx-batis-0.0.9/sqlbatis/orm.py` & `sqlx-batis-0.1.0/sqlbatis/orm.py`

 * *Files 4% similar despite different names*

```diff
@@ -205,16 +205,19 @@
         if key_strategy == KeyStrategy.SNOWFLAKE:
             kwargs[key] = get_snowflake_id()
             db.insert(table, **kwargs)
             return kwargs[key]
         else:
             select_key = cls._get_select_key()
             if not select_key:
-                select_key = Engin.get_select_key(table=table)
-            return db.save(select_key, table, **kwargs)
+                try:
+                    select_key = Engin.get_select_key_intf(table=table, key=key)
+                except NotImplementedError:
+                    raise DBError(f"Expect 'select_key' but not. you can set it in model class with '__select_key__'.")
+            return db.save_select_key(select_key, table, **kwargs)
 
     @classmethod
     def create(cls, **kwargs):
         """
         person = Person.create(name='张三', age=20)
         :return: Instance object
         """
@@ -595,14 +598,88 @@
 
         key, table = cls._get_key_and_table()
         where = 'WHERE {} in ({})'.format(key, ','.join(['?' for _ in range(ids_size)]))
         sql = select_sql(table, where, ids_size, *fields)
         return db.do_select(sql, *ids, ids_size)
 
     @classmethod
+    def find_page(cls, page_num=1, page_size=10, *fields, **kwargs):
+        """
+        Return list(object) or empty list if no result.
+        persons = Person.find_page(1, 10, 'name', 'age', name='张三', age=55)
+        :param page_num: page number
+        :param page_size: page size
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        result = cls.query_page(page_num, page_size, *fields, **kwargs)
+        return [cls.to_obj(**d) for d in result]
+
+    @classmethod
+    def find_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
+        """
+        Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
+        rows = Person.find_by_page(1, 10, 'where name=?', '李四')
+        """
+        log_support.orm_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        return [cls.to_obj(**d) for d in cls.query_page_by(page_num, page_size, where, *args, **kwargs)]
+
+    @classmethod
+    def query_page(cls, page_num=1, page_size=10, *fields, **kwargs):
+        """
+        Return list(dict) or empty list if no result.
+        persons = Person.query_page(1, 10, 'id', 'name', 'age', name='张三', age=55)
+        :param page_num: page number
+        :param page_size: page size
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        table = cls._get_table()
+        where, args, _ = get_where_arg_limit(**kwargs)
+        sql = select_sql(table, where, NO_LIMIT, *fields)
+        return db.do_query_page(sql, page_num, page_size, *args)
+
+    @classmethod
+    def query_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
+        """
+        Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
+        rows = Person.query_by_page(1, 10, 'where name=?', '李四')
+        """
+        log_support.orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        sql = cls._where_sql(where)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return db.do_query_page(sql, page_num, page_size, *args)
+
+    @classmethod
+    def select_page(cls, page_num=1, page_size=10, *fields, **kwargs):
+        """
+        Return list(dict) or empty list if no result.
+        rows = Person.select_page('id', 'name', 'age', name='张三', age=55)
+        :param page_num: page number
+        :param page_size: page size
+        :param fields: Default select all fields if not set
+        """
+        log_support.orm_page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
+        table = cls._get_table()
+        where, args, _ = get_where_arg_limit(**kwargs)
+        sql = select_sql(table, where, NO_LIMIT, *fields)
+        return db.do_select_page(sql, page_num, page_size, *args)
+
+    @classmethod
+    def select_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
+        """
+        Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
+        rows = Person.select_by_page(1, 10, 'where name=?', '李四')
+        """
+        log_support.orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
+        sql = cls._where_sql(where)
+        sql, args = simple_sql(sql, *args, **kwargs)
+        return db.do_select_page(sql, page_num, page_size, *args)
+
+    @classmethod
     def to_obj(cls, **kwargs):
         model = cls.__new__(cls)
         model.__dict__.update(**kwargs)
         return model
 
     def _get_kv(self, ignored_none: bool, key: None, *fields):
         if fields:
@@ -740,15 +817,15 @@
 
 
 # ----------------------------------------------------------Private function------------------------------------------------------------------
 def select_sql(table: str, where: str, limit: Union[int, Tuple[int], List[int]], *fields):
     if fields:
         fields = ','.join([col if '(' in col else '{}'.format(col) for col in fields])
     else:
-        fields = Engin.get_table_columns(table)
+        fields = Engin.get_table_columns_intf(table)
 
     if limit:
         if isinstance(limit, int):
             return 'SELECT {} FROM {} {} LIMIT ?'.format(fields, table, where)
         elif (isinstance(limit, Tuple) or isinstance(limit, List)) and len(limit) == 2:
             return 'SELECT {} FROM {} {} LIMIT ? OFFSET ?'.format(fields, table, where)
         else:
```

### Comparing `sqlx-batis-0.0.9/sqlbatis/snowflake.py` & `sqlx-batis-0.1.0/sqlbatis/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.9/sqlbatis/sql_holder.py` & `sqlx-batis-0.1.0/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.9/sqlbatis/sql_mapper.py` & `sqlx-batis-0.1.0/sqlbatis/sql_mapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sqlexec
 import functools
 from .engin import Engin
-from .support import SqlAction
 from .log_support import logger
+from .support import SqlAction, DBError
 from .sql_support import simple_sql, get_named_sql_args
 from .sql_holder import get_sql_model, do_get_sql, build_sql_id
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
 def mapper(namespace: str = None, sql_id: str = None, batch=False, return_key=False, select_key=None):
@@ -16,31 +16,35 @@
         def _wrapper(*args, **kwargs):
             param_names = func.__code__.co_varnames
             full_sql_id, func_name = before(func, namespace, sql_id, *args, **kwargs)
             sql_model = get_sql_model(full_sql_id)
             exec_func = get_exec_func(func, sql_model.action, batch)
             if return_key:
                 use_select_key = select_key
-                use_sql, args = do_get_sql(sql_model,  batch, param_names, *args, **kwargs)
+                use_sql, args = do_get_sql(sql_model, batch, param_names, *args, **kwargs)
                 if use_select_key is None:
                     use_select_key = sql_model.select_key
                     if use_select_key is None:
-                        use_select_key = Engin.get_select_key(sql=use_sql)
-                assert use_select_key, "'selectKey' should not be None in sql_id: '{}'".format(full_sql_id)
+                        try:
+                            use_select_key = Engin.get_select_key_intf(sql=use_sql)
+                        except NotImplementedError:
+                            return DBError(
+                                f"Expect 'select_key' but not. you can set it in mapper file with 'selectKey', or @mapper with 'select_key'")
                 return sqlexec.save_sql(use_select_key, use_sql, *args)
             if batch:
                 if kwargs:
                     logger.warning("Batch exec sql better use like '{}(args)' or '{}(*args)' then '{}(args=args)'".format(func_name, func_name, func_name))
                     args = list(kwargs.values())[0]
                 use_sql, _ = do_get_sql(sql_model, batch, param_names, *args)
             else:
                 use_sql, args = do_get_sql(sql_model, batch, param_names, *args, **kwargs)
             return exec_func(use_sql, *args)
 
         return _wrapper
+
     return _decorator
 
 
 def sql(value: str, batch=False, return_key=False, select_key=None):
     def _decorator(func):
         @functools.wraps(func)
         def _wrapper(*args, **kwargs):
@@ -50,16 +54,18 @@
                 if batch:
                     if kwargs:
                         args = list(kwargs.values())[0]
                     return sqlexec.batch_execute(use_sql, *args)
                 if return_key:
                     use_select_key = select_key
                     if use_select_key is None:
-                        use_select_key = Engin.get_select_key(sql=use_sql)
-                    assert use_select_key, "'select_key' should not be None in func '{}' at file: '{}' line {}.".format(func.__name__, func.__code__.co_filename, func.__code__.co_firstlineno)
+                        try:
+                            use_select_key = Engin.get_select_key_intf(sql=use_sql)
+                        except NotImplementedError:
+                            return DBError(f"Expect 'select_key' but not in func '{func.__name__}' at file: '{func.__code__.co_filename}', line {func.__code__.co_firstlineno}. you can set it @sql with 'select_key'")
                     assert SqlAction.INSERT.value in low_sql, 'Only insert sql can return primary key.'
                     if kwargs:
                         use_sql, args = get_named_sql_args(use_sql, **kwargs)
                     return sqlexec.save_sql(use_select_key, use_sql, *args)
 
                 if kwargs:
                     use_sql, args = get_named_sql_args(use_sql, **kwargs)
@@ -68,14 +74,15 @@
                 select_func = get_select_func(func)
                 use_sql, args = simple_sql(use_sql, *args, **kwargs)
                 return select_func(use_sql, *args)
             else:
                 return ValueError("Invalid sql: {}.".format(sql))
 
         return _wrapper
+
     return _decorator
 
 
 def get_exec_func(func, action, batch):
     if action == SqlAction.SELECT.value:
         return get_select_func(func)
     elif batch:
```

### Comparing `sqlx-batis-0.0.9/sqlbatis/sql_support.py` & `sqlx-batis-0.1.0/sqlbatis/sql_support.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,19 @@
     if sql_type == 0:
         return sql, args
     if sql_type == 1:
         sql = Template(sql).render(**kwargs)
     return get_named_sql_args(sql, **kwargs)
 
 
+def get_page_start(page_num: int, page_size: int):
+    assert page_num >= 1 and page_size >= 1, "'page_name' and 'page_size' should be higher or equal to 1"
+    return (page_num - 1) * page_size
+
+
 def limit_one_sql_args(sql: str, *args):
     if require_limit(sql):
         return '{} LIMIT ?'.format(sql), [*args, LIMIT_1]
     return sql, args
 
 
 def is_dynamic_sql(sql: str):
```

### Comparing `sqlx-batis-0.0.9/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.1.0/sqlx_batis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.0.9
+Version: 0.1.0
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

