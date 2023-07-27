# Comparing `tmp/peewee_aio-1.7.1.tar.gz` & `tmp/peewee_aio-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_aio-1.7.1.tar", max compression
+gzip compressed data, was "peewee_aio-1.7.2.tar", max compression
```

## Comparing `peewee_aio-1.7.1.tar` & `peewee_aio-1.7.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4681 2023-07-27 07:10:25.827578 peewee_aio-1.7.1/README.md
--rw-r--r--   0        0        0      132 2023-07-27 07:10:25.827578 peewee_aio-1.7.1/peewee_aio/__init__.py
--rw-r--r--   0        0        0     1210 2023-07-27 07:10:25.827578 peewee_aio-1.7.1/peewee_aio/databases.py
--rw-r--r--   0        0        0    17336 2023-07-27 07:10:25.827578 peewee_aio-1.7.1/peewee_aio/fields.py
--rw-r--r--   0        0        0    15918 2023-07-27 07:10:25.827578 peewee_aio-1.7.1/peewee_aio/manager.py
--rw-r--r--   0        0        0    17014 2023-07-27 07:10:25.827578 peewee_aio-1.7.1/peewee_aio/model.py
--rw-r--r--   0        0        0        0 2023-07-27 07:10:25.827578 peewee_aio-1.7.1/peewee_aio/py.typed
--rw-r--r--   0        0        0      268 2023-07-27 07:10:25.827578 peewee_aio-1.7.1/peewee_aio/types.py
--rw-r--r--   0        0        0      839 2023-07-27 07:10:25.831578 peewee_aio-1.7.1/peewee_aio/utils.py
--rw-r--r--   0        0        0     2622 2023-07-27 07:10:25.831578 peewee_aio-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 peewee_aio-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     4681 2023-07-27 08:41:05.086637 peewee_aio-1.7.2/README.md
+-rw-r--r--   0        0        0      132 2023-07-27 08:41:05.086637 peewee_aio-1.7.2/peewee_aio/__init__.py
+-rw-r--r--   0        0        0     1210 2023-07-27 08:41:05.086637 peewee_aio-1.7.2/peewee_aio/databases.py
+-rw-r--r--   0        0        0    17336 2023-07-27 08:41:05.086637 peewee_aio-1.7.2/peewee_aio/fields.py
+-rw-r--r--   0        0        0    15918 2023-07-27 08:41:05.086637 peewee_aio-1.7.2/peewee_aio/manager.py
+-rw-r--r--   0        0        0    17014 2023-07-27 08:41:05.086637 peewee_aio-1.7.2/peewee_aio/model.py
+-rw-r--r--   0        0        0        0 2023-07-27 08:41:05.086637 peewee_aio-1.7.2/peewee_aio/py.typed
+-rw-r--r--   0        0        0      268 2023-07-27 08:41:05.086637 peewee_aio-1.7.2/peewee_aio/types.py
+-rw-r--r--   0        0        0      901 2023-07-27 08:41:05.086637 peewee_aio-1.7.2/peewee_aio/utils.py
+-rw-r--r--   0        0        0     2622 2023-07-27 08:41:05.090637 peewee_aio-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 peewee_aio-1.7.2/PKG-INFO
```

### Comparing `peewee_aio-1.7.1/README.md` & `peewee_aio-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.7.1/peewee_aio/databases.py` & `peewee_aio-1.7.2/peewee_aio/databases.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.7.1/peewee_aio/fields.py` & `peewee_aio-1.7.2/peewee_aio/fields.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.7.1/peewee_aio/manager.py` & `peewee_aio-1.7.2/peewee_aio/manager.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.7.1/peewee_aio/model.py` & `peewee_aio-1.7.2/peewee_aio/model.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.7.1/pyproject.toml` & `peewee_aio-1.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-aio"
-version = "1.7.1"
+version = "1.7.2"
 description = "Async support for Peewee ORM"
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/klen/peewee-aio"
 repository = "https://github.com/klen/peewee-aio"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["peewee", "asyncio", "trio", "orm"]
```

### Comparing `peewee_aio-1.7.1/PKG-INFO` & `peewee_aio-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-aio
-Version: 1.7.1
+Version: 1.7.2
 Summary: Async support for Peewee ORM
 Home-page: https://github.com/klen/peewee-aio
 License: MIT
 Keywords: peewee,asyncio,trio,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

