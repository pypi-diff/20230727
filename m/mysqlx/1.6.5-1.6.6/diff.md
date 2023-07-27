# Comparing `tmp/mysqlx-1.6.5.tar.gz` & `tmp/mysqlx-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.6.5.tar", last modified: Wed Jul 26 08:41:02 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.6.6.tar", last modified: Thu Jul 27 11:35:26 2023, max compression
```

## Comparing `mysqlx-1.6.5.tar` & `mysqlx-1.6.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:41:02.000000 mysqlx-1.6.5/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx/
--rw-rw-rw-   0        0        0     2726 2023-07-26 07:18:22.000000 mysqlx-1.6.5/mysqlx/db.py
--rw-rw-rw-   0        0        0     1897 2023-07-26 07:24:54.000000 mysqlx-1.6.5/mysqlx/dbx.py
--rw-rw-rw-   0        0        0      763 2023-07-26 07:58:39.000000 mysqlx-1.6.5/mysqlx/engin.py
--rw-rw-rw-   0        0        0     1704 2023-07-26 07:24:54.000000 mysqlx-1.6.5/mysqlx/log_support.py
--rw-rw-rw-   0        0        0     9895 2023-07-26 07:32:28.000000 mysqlx-1.6.5/mysqlx/orm.py
--rw-rw-rw-   0        0        0      339 2023-07-26 07:19:23.000000 mysqlx-1.6.5/mysqlx/sql_support.py
--rw-rw-rw-   0        0        0      641 2023-07-26 08:02:46.000000 mysqlx-1.6.5/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4511 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      317 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4511 2023-07-26 08:41:02.000000 mysqlx-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     4007 2023-07-25 08:23:23.000000 mysqlx-1.6.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-26 08:41:02.000000 mysqlx-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-07-26 08:40:53.000000 mysqlx-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:35:26.000000 mysqlx-1.6.6/
+drwxrwxrwx   0        0        0        0 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx/
+-rw-rw-rw-   0        0        0      663 2023-07-27 04:34:07.000000 mysqlx-1.6.6/mysqlx/db.py
+-rw-rw-rw-   0        0        0      570 2023-07-27 04:34:07.000000 mysqlx-1.6.6/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0      761 2023-07-26 15:03:13.000000 mysqlx-1.6.6/mysqlx/engin.py
+-rw-rw-rw-   0        0        0      414 2023-07-27 04:35:53.000000 mysqlx-1.6.6/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0     6082 2023-07-27 04:32:45.000000 mysqlx-1.6.6/mysqlx/orm.py
+-rw-rw-rw-   0        0        0      339 2023-07-26 07:19:23.000000 mysqlx-1.6.6/mysqlx/sql_support.py
+-rw-rw-rw-   0        0        0      488 2023-07-27 11:33:28.000000 mysqlx-1.6.6/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4511 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      317 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 11:35:26.000000 mysqlx-1.6.6/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4511 2023-07-27 11:35:26.000000 mysqlx-1.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4007 2023-07-25 08:23:23.000000 mysqlx-1.6.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:35:26.000000 mysqlx-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-07-27 11:33:59.000000 mysqlx-1.6.6/setup.py
```

### Comparing `mysqlx-1.6.5/mysqlx/engin.py` & `mysqlx-1.6.6/mysqlx/engin.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,17 @@
         super().__init__(engin)
 
     @classmethod
     def init(cls, name='MySQL'):
         super().init(name)
 
     @staticmethod
-    def _create_insert_sql(table: str, cols: Sequence[str]):
+    def create_insert_sql(table: str, cols: Sequence[str]):
         columns, placeholders = zip(*[('`{}`'.format(col), '?') for col in cols])
         return 'INSERT INTO `{}`({}) VALUES({})'.format(table, ','.join(columns), ','.join(placeholders))
 
     @staticmethod
-    def _page_sql_args(require_limit, sql: str, start, page_size, *args):
+    def page_sql_args(require_limit, sql: str, start, page_size, *args):
         if require_limit(sql):
             sql = '{} LIMIT ?, ?'.format(sql)
         args = [*args, start, page_size]
         return sql, args
```

### Comparing `mysqlx-1.6.5/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.6.6/mysqlx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.6.5
+Version: 1.6.6
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.6.5/PKG-INFO` & `mysqlx-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.6.5
+Version: 1.6.6
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.6.5/README.rst` & `mysqlx-1.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.5/setup.py` & `mysqlx-1.6.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     name='mysqlx',
     packages=['mysqlx'],
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # 'Jinja2>=2.7.0',
-        'sqlx-batis>=0.0.9',
+        'sqlx-batis>=0.1.0',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.6.5',
+    version='1.6.6',
     url='https://gitee.com/summry/mysqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

