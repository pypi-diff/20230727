# Comparing `tmp/milho_multi_sqlite3_manager-0.3.0.tar.gz` & `tmp/milho_multi_sqlite3_manager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milho_multi_sqlite3_manager-0.3.0.tar", max compression
+gzip compressed data, was "milho_multi_sqlite3_manager-0.4.0.tar", max compression
```

## Comparing `milho_multi_sqlite3_manager-0.3.0.tar` & `milho_multi_sqlite3_manager-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0       78 2023-07-01 18:48:26.038198 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/__init__.py
--rw-r--r--   0        0        0       35 2023-07-11 01:06:13.985060 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/file_manager/__init__.py
--rw-r--r--   0        0        0     2348 2023-07-11 02:04:32.602447 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/file_manager/file_manager.py
--rw-r--r--   0        0        0       41 2023-07-11 01:05:11.426535 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/sqlite3_manager/__init__.py
--rw-r--r--   0        0        0     9847 2023-07-11 01:52:34.227736 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/sqlite3_manager/sqlite3_manager.py
--rw-r--r--   0        0        0     6479 2023-07-11 02:03:43.934491 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/sqlite3_manager/sqlite3_manager_test.py
--rw-r--r--   0        0        0        0 2023-06-16 03:42:12.550884 milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/tests/__init__.py
--rw-r--r--   0        0        0      453 2023-07-11 02:12:24.012409 milho_multi_sqlite3_manager-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1185 2023-06-25 17:47:20.995550 milho_multi_sqlite3_manager-0.3.0/README.md
--rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 milho_multi_sqlite3_manager-0.3.0/setup.py
--rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 milho_multi_sqlite3_manager-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      118 2023-07-27 17:45:17.705146 milho_multi_sqlite3_manager-0.4.0/multisqlite3manager/__init__.py
+-rw-r--r--   0        0        0      269 2023-07-27 17:44:58.188107 milho_multi_sqlite3_manager-0.4.0/multisqlite3manager/file_manager/__init__.py
+-rw-r--r--   0        0        0     2348 2023-07-11 02:04:32.602447 milho_multi_sqlite3_manager-0.4.0/multisqlite3manager/file_manager/file_manager.py
+-rw-r--r--   0        0        0      356 2023-07-27 17:39:29.510169 milho_multi_sqlite3_manager-0.4.0/multisqlite3manager/sqlite3_manager/__init__.py
+-rw-r--r--   0        0        0     9847 2023-07-11 17:41:43.230958 milho_multi_sqlite3_manager-0.4.0/multisqlite3manager/sqlite3_manager/sqlite3_manager.py
+-rw-r--r--   0        0        0     6479 2023-07-11 02:03:43.934491 milho_multi_sqlite3_manager-0.4.0/multisqlite3manager/sqlite3_manager/sqlite3_manager_test.py
+-rw-r--r--   0        0        0      453 2023-07-27 17:57:53.261477 milho_multi_sqlite3_manager-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1185 2023-06-25 17:47:20.995550 milho_multi_sqlite3_manager-0.4.0/README.md
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 milho_multi_sqlite3_manager-0.4.0/setup.py
+-rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 milho_multi_sqlite3_manager-0.4.0/PKG-INFO
```

### Comparing `milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/file_manager/file_manager.py` & `milho_multi_sqlite3_manager-0.4.0/multisqlite3manager/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/sqlite3_manager/sqlite3_manager.py` & `milho_multi_sqlite3_manager-0.4.0/multisqlite3manager/sqlite3_manager/sqlite3_manager.py`

 * *Files identical despite different names*

### Comparing `milho_multi_sqlite3_manager-0.3.0/multisqlite3manager/sqlite3_manager/sqlite3_manager_test.py` & `milho_multi_sqlite3_manager-0.4.0/multisqlite3manager/sqlite3_manager/sqlite3_manager_test.py`

 * *Files identical despite different names*

### Comparing `milho_multi_sqlite3_manager-0.3.0/README.md` & `milho_multi_sqlite3_manager-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `milho_multi_sqlite3_manager-0.3.0/setup.py` & `milho_multi_sqlite3_manager-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['multisqlite3manager',
  'multisqlite3manager.file_manager',
- 'multisqlite3manager.sqlite3_manager',
- 'multisqlite3manager.tests']
+ 'multisqlite3manager.sqlite3_manager']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pandas>=2.0.2,<3.0.0', 'sqlalchemy>=2.0.16,<3.0.0', 'sqlglot>=16.3.1,<17.0.0']
 
 setup_kwargs = {
     'name': 'milho-multi-sqlite3-manager',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': '',
     'long_description': '# milho-multi-sqlite3-manager\n\n## Description\n\nThe idea is to have an environment with multiple SQLITE3 files, aiming at ease of access and use.\nThe inspiration for creating this module came from the ease of working with Spark in BigData environments where, generally, everything is integrated, without the need to make several explicit connections in the code.\n\nIf you want an integrated environment on your machine, create an environment variable called "MULTISQLITE3MANAGER_FOLDER_PATH" with the directory of your folder. You will need to make sure that all files in this folder are SQLITE3 databases.\n\nWhen "to_dataframe" is used, the result is a Pandas DataFrame. The query is previously parsed to map all the databases used in the SQL. Then the module create a sqlalchemy connection and attach that databases to the connection. After that, the query is executed and the result is a Pandas DataFrame. \n\n## Code Samples\n\n```python\n\nfrom multisqlite3manager import print_databases, print_tables, to_dataframe\n\nprint_databases()\nprint_tables("DB_NAME")\n\ndf = to_dataframe("SELECT * FROM db_1.tMisto")\ndf2 = to_dataframe("SELECT * FROM db_2_copy.tMisto")\n\n```\n',
     'author': 'Guilherme S. Magalhães',
     'author_email': '40049979+Guisilcol@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `milho_multi_sqlite3_manager-0.3.0/PKG-INFO` & `milho_multi_sqlite3_manager-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milho-multi-sqlite3-manager
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: Guilherme S. Magalhães
 Author-email: 40049979+Guisilcol@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

