# Comparing `tmp/pgsqlx-generator-1.6.8.tar.gz` & `tmp/pgsqlx-generator-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-generator-1.6.8.tar", last modified: Wed Jul 26 08:49:57 2023, max compression
+gzip compressed data, was "dist\pgsqlx-generator-1.6.9.tar", last modified: Thu Jul 27 11:40:01 2023, max compression
```

## Comparing `pgsqlx-generator-1.6.8.tar` & `pgsqlx-generator-1.6.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:49:57.000000 pgsqlx-generator-1.6.8/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:49:57.000000 pgsqlx-generator-1.6.8/pgsqlx/
--rw-rw-rw-   0        0        0     6644 2023-07-26 08:47:06.000000 pgsqlx-generator-1.6.8/pgsqlx/generator.py
--rw-rw-rw-   0        0        0     1905 2023-07-24 06:46:00.000000 pgsqlx-generator-1.6.8/pgsqlx/generator.tpl
--rw-rw-rw-   0        0        0      660 2023-07-26 08:45:19.000000 pgsqlx-generator-1.6.8/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:49:57.000000 pgsqlx-generator-1.6.8/pgsqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-26 08:49:57.000000 pgsqlx-generator-1.6.8/pgsqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-26 08:49:57.000000 pgsqlx-generator-1.6.8/pgsqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2868 2023-07-26 08:49:57.000000 pgsqlx-generator-1.6.8/pgsqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-26 08:49:57.000000 pgsqlx-generator-1.6.8/pgsqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      317 2023-07-26 08:49:57.000000 pgsqlx-generator-1.6.8/pgsqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 08:49:57.000000 pgsqlx-generator-1.6.8/pgsqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2868 2023-07-26 08:49:57.000000 pgsqlx-generator-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     2395 2023-07-24 07:34:39.000000 pgsqlx-generator-1.6.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-26 08:49:57.000000 pgsqlx-generator-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1118 2023-07-26 08:49:48.000000 pgsqlx-generator-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:40:01.000000 pgsqlx-generator-1.6.9/
+drwxrwxrwx   0        0        0        0 2023-07-27 11:40:01.000000 pgsqlx-generator-1.6.9/pgsqlx/
+-rw-rw-rw-   0        0        0     6448 2023-07-27 11:38:44.000000 pgsqlx-generator-1.6.9/pgsqlx/generator.py
+-rw-rw-rw-   0        0        0     1905 2023-07-24 06:46:00.000000 pgsqlx-generator-1.6.9/pgsqlx/generator.tpl
+-rw-rw-rw-   0        0        0      508 2023-07-27 11:38:44.000000 pgsqlx-generator-1.6.9/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:40:01.000000 pgsqlx-generator-1.6.9/pgsqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:40:01.000000 pgsqlx-generator-1.6.9/pgsqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-27 11:40:01.000000 pgsqlx-generator-1.6.9/pgsqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2868 2023-07-27 11:40:01.000000 pgsqlx-generator-1.6.9/pgsqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-27 11:40:01.000000 pgsqlx-generator-1.6.9/pgsqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      317 2023-07-27 11:40:01.000000 pgsqlx-generator-1.6.9/pgsqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 11:40:01.000000 pgsqlx-generator-1.6.9/pgsqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2868 2023-07-27 11:40:01.000000 pgsqlx-generator-1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2395 2023-07-24 07:34:39.000000 pgsqlx-generator-1.6.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:40:01.000000 pgsqlx-generator-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1118 2023-07-27 11:39:52.000000 pgsqlx-generator-1.6.9/setup.py
```

### Comparing `pgsqlx-generator-1.6.8/pgsqlx/generator.py` & `pgsqlx-generator-1.6.9/pgsqlx/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     comma2 = '，'
     sql = '''SELECT column_name as "COLUMN_NAME", udt_name as "DATA_TYPE", column_default 
              FROM information_schema.columns WHERE table_schema='public' AND table_name = ?'''
     key_sql = '''SELECT a.attname FROM pg_index i
                  JOIN pg_attribute a ON a.attrelid = i.indrelid AND a.attnum = any(i.indkey)
                  WHERE i.indrelid = ?::regclass AND i.indisprimary LIMIT 1'''
 
-    def __init__(self, user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=0, show_sql=False, use_unicode=True, **kwargs):
+    def __init__(self, pool_size=0, **kwargs):
         PostgresEngin.init()
-        init_db(user=user, password=password, database=database, host=host, port=port, pool_size=pool_size, show_sql=show_sql, **kwargs)
+        init_db(pool_size=pool_size, **kwargs)
 
     def generate_with_schema(self, schema: str = None, path: str = None, *args, **kwargs):
         if schema:
             db.execute('use %s' % schema)
         tables = db.select('show tables')
         tables = [table[0] for table in tables]
         self.generate_with_tables(tables=tables, path=path, *args, **kwargs)
```

### Comparing `pgsqlx-generator-1.6.8/pgsqlx/generator.tpl` & `pgsqlx-generator-1.6.9/pgsqlx/generator.tpl`

 * *Files identical despite different names*

### Comparing `pgsqlx-generator-1.6.8/pgsqlx_generator.egg-info/PKG-INFO` & `pgsqlx-generator-1.6.9/pgsqlx_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx-generator
-Version: 1.6.8
+Version: 1.6.9
 Summary: pgsqlx-generator is a model code generator from tables for PgSqlx.
 Home-page: https://gitee.com/summry/pgsqlx/blob/master/generator.md
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: PostgreSQL,PgSqlx,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-generator-1.6.8/PKG-INFO` & `pgsqlx-generator-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx-generator
-Version: 1.6.8
+Version: 1.6.9
 Summary: pgsqlx-generator is a model code generator from tables for PgSqlx.
 Home-page: https://gitee.com/summry/pgsqlx/blob/master/generator.md
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: PostgreSQL,PgSqlx,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-generator-1.6.8/README.rst` & `pgsqlx-generator-1.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-generator-1.6.8/setup.py` & `pgsqlx-generator-1.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     packages=['pgsqlx'],
     description="pgsqlx-generator is a model code generator from tables for PgSqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'pgsqlx>=1.6.6',
     ],
-    version='1.6.8',
+    version='1.6.9',
     url='https://gitee.com/summry/pgsqlx/blob/master/generator.md',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['PostgreSQL', 'PgSqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

