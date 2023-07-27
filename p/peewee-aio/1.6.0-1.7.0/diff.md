# Comparing `tmp/peewee_aio-1.6.0.tar.gz` & `tmp/peewee_aio-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_aio-1.6.0.tar", max compression
+gzip compressed data, was "peewee_aio-1.7.0.tar", max compression
```

## Comparing `peewee_aio-1.6.0.tar` & `peewee_aio-1.7.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     4681 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/README.md
--rw-r--r--   0        0        0      132 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/__init__.py
--rw-r--r--   0        0        0     1210 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/databases.py
--rw-r--r--   0        0        0    17336 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/fields.py
--rw-r--r--   0        0        0    15918 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/manager.py
--rw-r--r--   0        0        0    17014 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/model.py
--rw-r--r--   0        0        0        0 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/py.typed
--rw-r--r--   0        0        0      268 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/peewee_aio/types.py
--rw-r--r--   0        0        0     2622 2023-07-07 14:13:53.716803 peewee_aio-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 peewee_aio-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     4681 2023-07-27 07:02:17.179262 peewee_aio-1.7.0/README.md
+-rw-r--r--   0        0        0      132 2023-07-27 07:02:17.179262 peewee_aio-1.7.0/peewee_aio/__init__.py
+-rw-r--r--   0        0        0     1210 2023-07-27 07:02:17.179262 peewee_aio-1.7.0/peewee_aio/databases.py
+-rw-r--r--   0        0        0    17336 2023-07-27 07:02:17.179262 peewee_aio-1.7.0/peewee_aio/fields.py
+-rw-r--r--   0        0        0    15918 2023-07-27 07:02:17.179262 peewee_aio-1.7.0/peewee_aio/manager.py
+-rw-r--r--   0        0        0    17014 2023-07-27 07:02:17.179262 peewee_aio-1.7.0/peewee_aio/model.py
+-rw-r--r--   0        0        0        0 2023-07-27 07:02:17.179262 peewee_aio-1.7.0/peewee_aio/py.typed
+-rw-r--r--   0        0        0      268 2023-07-27 07:02:17.179262 peewee_aio-1.7.0/peewee_aio/types.py
+-rw-r--r--   0        0        0      842 2023-07-27 07:02:17.179262 peewee_aio-1.7.0/peewee_aio/utils.py
+-rw-r--r--   0        0        0     2622 2023-07-27 07:02:17.179262 peewee_aio-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 peewee_aio-1.7.0/PKG-INFO
```

### Comparing `peewee_aio-1.6.0/README.md` & `peewee_aio-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.6.0/peewee_aio/databases.py` & `peewee_aio-1.7.0/peewee_aio/databases.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.6.0/peewee_aio/fields.py` & `peewee_aio-1.7.0/peewee_aio/fields.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.6.0/peewee_aio/manager.py` & `peewee_aio-1.7.0/peewee_aio/manager.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.6.0/peewee_aio/model.py` & `peewee_aio-1.7.0/peewee_aio/model.py`

 * *Files identical despite different names*

### Comparing `peewee_aio-1.6.0/pyproject.toml` & `peewee_aio-1.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-aio"
-version = "1.6.0"
+version = "1.7.0"
 description = "Async support for Peewee ORM"
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/klen/peewee-aio"
 repository = "https://github.com/klen/peewee-aio"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["peewee", "asyncio", "trio", "orm"]
```

### Comparing `peewee_aio-1.6.0/PKG-INFO` & `peewee_aio-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-aio
-Version: 1.6.0
+Version: 1.7.0
 Summary: Async support for Peewee ORM
 Home-page: https://github.com/klen/peewee-aio
 License: MIT
 Keywords: peewee,asyncio,trio,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

