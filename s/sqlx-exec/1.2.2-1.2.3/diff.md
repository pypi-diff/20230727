# Comparing `tmp/sqlx-exec-1.2.2.tar.gz` & `tmp/sqlx-exec-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.2.2.tar", last modified: Thu Jul 27 11:28:24 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.2.3.tar", last modified: Thu Jul 27 11:29:36 2023, max compression
```

## Comparing `sqlx-exec-1.2.2.tar` & `sqlx-exec-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:28:24.000000 sqlx-exec-1.2.2/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     2770 2023-07-27 11:28:24.000000 sqlx-exec-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2261 2023-07-26 08:32:11.000000 sqlx-exec-1.2.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-27 11:28:24.000000 sqlx-exec-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1161 2023-07-27 11:28:15.000000 sqlx-exec-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:28:24.000000 sqlx-exec-1.2.2/sqlexec/
--rw-rw-rw-   0        0        0      350 2023-07-27 11:09:15.000000 sqlx-exec-1.2.2/sqlexec/constant.py
--rw-rw-rw-   0        0        0     1446 2023-07-27 04:42:17.000000 sqlx-exec-1.2.2/sqlexec/engin.py
--rw-rw-rw-   0        0        0    10206 2023-07-27 11:18:24.000000 sqlx-exec-1.2.2/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1246 2023-07-27 11:21:29.000000 sqlx-exec-1.2.2/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.2.2/sqlexec/log_support.py
--rw-rw-rw-   0        0        0      833 2023-07-25 17:51:41.000000 sqlx-exec-1.2.2/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1134 2023-07-26 14:36:38.000000 sqlx-exec-1.2.2/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.2.2/sqlexec/support.py
--rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.2.2/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:28:24.000000 sqlx-exec-1.2.2/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-27 11:28:24.000000 sqlx-exec-1.2.2/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 13:22:36.000000 sqlx-exec-1.2.2/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2770 2023-07-27 11:28:24.000000 sqlx-exec-1.2.2/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-07-27 11:28:24.000000 sqlx-exec-1.2.2/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 11:28:24.000000 sqlx-exec-1.2.2/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2740 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2232 2023-07-27 11:29:33.000000 sqlx-exec-1.2.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-07-27 11:29:33.000000 sqlx-exec-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/sqlexec/
+-rw-rw-rw-   0        0        0      350 2023-07-27 11:09:15.000000 sqlx-exec-1.2.3/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     1446 2023-07-27 04:42:17.000000 sqlx-exec-1.2.3/sqlexec/engin.py
+-rw-rw-rw-   0        0        0    10206 2023-07-27 11:18:24.000000 sqlx-exec-1.2.3/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1246 2023-07-27 11:21:29.000000 sqlx-exec-1.2.3/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.2.3/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0      833 2023-07-25 17:51:41.000000 sqlx-exec-1.2.3/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1134 2023-07-26 14:36:38.000000 sqlx-exec-1.2.3/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.2.3/sqlexec/support.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.2.3/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 13:22:36.000000 sqlx-exec-1.2.3/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2740 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 11:29:36.000000 sqlx-exec-1.2.3/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.2.2/LICENSE` & `sqlx-exec-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.2/PKG-INFO` & `sqlx-exec-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.2.2
+Version: 1.2.3
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -14,15 +14,14 @@
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
-   from sqlexec import Engin
 
    if __name__ == '__main__':
        sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
```

### Comparing `sqlx-exec-1.2.2/README.rst` & `sqlx-exec-1.2.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
-   from sqlexec import Engin
 
    if __name__ == '__main__':
        sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
```

### Comparing `sqlx-exec-1.2.2/setup.py` & `sqlx-exec-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.2',
+    version='1.2.3',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.2.2/sqlexec/engin.py` & `sqlx-exec-1.2.3/sqlexec/engin.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.2/sqlexec/exec.py` & `sqlx-exec-1.2.3/sqlexec/exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.2/sqlexec/init_import.py` & `sqlx-exec-1.2.3/sqlexec/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.2/sqlexec/log_support.py` & `sqlx-exec-1.2.3/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.2/sqlexec/pooling.py` & `sqlx-exec-1.2.3/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.2/sqlexec/sql_support.py` & `sqlx-exec-1.2.3/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.2/sqlexec/support.py` & `sqlx-exec-1.2.3/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.2/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.2.3/sqlx_exec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.2.2
+Version: 1.2.3
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -14,15 +14,14 @@
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
-   from sqlexec import Engin
 
    if __name__ == '__main__':
        sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
```

