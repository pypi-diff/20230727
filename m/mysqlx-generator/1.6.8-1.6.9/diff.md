# Comparing `tmp/mysqlx-generator-1.6.8.tar.gz` & `tmp/mysqlx-generator-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-generator-1.6.8.tar", last modified: Wed Jul 26 09:11:55 2023, max compression
+gzip compressed data, was "dist\mysqlx-generator-1.6.9.tar", last modified: Thu Jul 27 11:36:07 2023, max compression
```

## Comparing `mysqlx-generator-1.6.8.tar` & `mysqlx-generator-1.6.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx/
--rw-rw-rw-   0        0        0     6196 2023-07-26 08:02:46.000000 mysqlx-generator-1.6.8/mysqlx/generator.py
--rw-rw-rw-   0        0        0     1802 2023-07-24 02:58:28.000000 mysqlx-generator-1.6.8/mysqlx/generator.tpl
--rw-rw-rw-   0        0        0      641 2023-07-26 08:02:46.000000 mysqlx-generator-1.6.8/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2826 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      317 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2826 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     2358 2023-07-24 01:17:21.000000 mysqlx-generator-1.6.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-07-26 09:11:49.000000 mysqlx-generator-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:36:07.000000 mysqlx-generator-1.6.9/
+drwxrwxrwx   0        0        0        0 2023-07-27 11:36:07.000000 mysqlx-generator-1.6.9/mysqlx/
+-rw-rw-rw-   0        0        0     5941 2023-07-27 11:34:47.000000 mysqlx-generator-1.6.9/mysqlx/generator.py
+-rw-rw-rw-   0        0        0     1802 2023-07-24 02:58:28.000000 mysqlx-generator-1.6.9/mysqlx/generator.tpl
+-rw-rw-rw-   0        0        0      488 2023-07-27 11:33:28.000000 mysqlx-generator-1.6.9/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:36:07.000000 mysqlx-generator-1.6.9/mysqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:36:07.000000 mysqlx-generator-1.6.9/mysqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-27 11:36:07.000000 mysqlx-generator-1.6.9/mysqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2826 2023-07-27 11:36:07.000000 mysqlx-generator-1.6.9/mysqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-27 11:36:07.000000 mysqlx-generator-1.6.9/mysqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      317 2023-07-27 11:36:07.000000 mysqlx-generator-1.6.9/mysqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 11:36:07.000000 mysqlx-generator-1.6.9/mysqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2826 2023-07-27 11:36:07.000000 mysqlx-generator-1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2358 2023-07-24 01:17:21.000000 mysqlx-generator-1.6.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:36:07.000000 mysqlx-generator-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2023-07-27 11:35:54.000000 mysqlx-generator-1.6.9/setup.py
```

### Comparing `mysqlx-generator-1.6.8/mysqlx/generator.py` & `mysqlx-generator-1.6.9/mysqlx/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     comma1 = ','
     comma2 = '，'
     sql = '''
     SELECT column_name, data_type, character_maximum_length, NUMERIC_precision, NUMERIC_scale, column_key FROM information_schema.columns
      WHERE table_schema = (SELECT DATABASE()) AND table_name = ? 
     '''
 
-    def __init__(self, user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=0, show_sql=False, use_unicode=True, **kwargs):
+    def __init__(self, **kwargs):
         MySqlEngin.init()
-        init_db(user=user, password=password, database=database, host=host, port=port, pool_size=pool_size, show_sql=show_sql, use_unicode=use_unicode, **kwargs)
+        init_db(**kwargs)
 
     def generate_with_schema(self, schema: str = None, path: str = None, *args, **kwargs):
         if schema:
             db.execute('use %s' % schema)
         tables = db.select('show tables')
         tables = [table[0] for table in tables]
         self.generate_with_tables(tables=tables, path=path, *args, **kwargs)
```

### Comparing `mysqlx-generator-1.6.8/mysqlx/generator.tpl` & `mysqlx-generator-1.6.9/mysqlx/generator.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.6.8/mysqlx_generator.egg-info/PKG-INFO` & `mysqlx-generator-1.6.9/mysqlx_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.6.8
+Version: 1.6.9
 Summary: mysqlx-generator is a model code generator from tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-generator-1.6.8/PKG-INFO` & `mysqlx-generator-1.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.6.8
+Version: 1.6.9
 Summary: mysqlx-generator is a model code generator from tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-generator-1.6.8/README.rst` & `mysqlx-generator-1.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.6.8/setup.py` & `mysqlx-generator-1.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     packages=['mysqlx'],
     description="mysqlx-generator is a model code generator from tables for MySqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'mysqlx>=1.6.5',
     ],
-    version='1.6.8',
+    version='1.6.9',
     url='https://gitee.com/summry/mysqlx/blob/master/generator.md',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['MySQL', 'mysqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

