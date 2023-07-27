# Comparing `tmp/thrift_pyi-0.5.0.tar.gz` & `tmp/thrift_pyi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thrift_pyi-0.5.0.tar", max compression
+gzip compressed data, was "thrift_pyi-0.6.0.tar", max compression
```

## Comparing `thrift_pyi-0.5.0.tar` & `thrift_pyi-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1074 2022-12-12 18:01:58.020030 thrift_pyi-0.5.0/LICENSE
--rw-r--r--   0        0        0     3470 2022-12-12 18:01:58.020030 thrift_pyi-0.5.0/README.rst
--rw-r--r--   0        0        0     1280 2022-12-12 18:01:58.020030 thrift_pyi-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-12 18:01:58.020030 thrift_pyi-0.5.0/src/thriftpyi/__init__.py
--rw-r--r--   0        0        0       92 2022-12-12 18:01:58.020030 thrift_pyi-0.5.0/src/thriftpyi/__main__.py
--rw-r--r--   0        0        0     1091 2022-12-12 18:01:58.020030 thrift_pyi-0.5.0/src/thriftpyi/cli.py
--rw-r--r--   0        0        0      183 2022-12-12 18:01:58.020030 thrift_pyi-0.5.0/src/thriftpyi/compat.py
--rw-r--r--   0        0        0     5064 2022-12-12 18:01:58.024031 thrift_pyi-0.5.0/src/thriftpyi/entities.py
--rw-r--r--   0        0        0      391 2022-12-12 18:01:58.024031 thrift_pyi-0.5.0/src/thriftpyi/files.py
--rw-r--r--   0        0        0     1262 2022-12-12 18:01:58.024031 thrift_pyi-0.5.0/src/thriftpyi/main.py
--rw-r--r--   0        0        0     5101 2022-12-12 18:01:58.024031 thrift_pyi-0.5.0/src/thriftpyi/proxies.py
--rw-r--r--   0        0        0        0 2022-12-12 18:01:58.024031 thrift_pyi-0.5.0/src/thriftpyi/py.typed
--rw-r--r--   0        0        0     2515 2022-12-12 18:01:58.024031 thrift_pyi-0.5.0/src/thriftpyi/stubs.py
--rw-r--r--   0        0        0     2079 2022-12-12 18:01:58.024031 thrift_pyi-0.5.0/src/thriftpyi/utils.py
--rw-r--r--   0        0        0     4606 1970-01-01 00:00:00.000000 thrift_pyi-0.5.0/setup.py
--rw-r--r--   0        0        0     4722 1970-01-01 00:00:00.000000 thrift_pyi-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-27 19:27:39.719424 thrift_pyi-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3470 2023-07-27 19:27:39.719424 thrift_pyi-0.6.0/README.rst
+-rw-r--r--   0        0        0     1280 2023-07-27 19:27:39.723425 thrift_pyi-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 19:27:39.723425 thrift_pyi-0.6.0/src/thriftpyi/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-27 19:27:39.723425 thrift_pyi-0.6.0/src/thriftpyi/__main__.py
+-rw-r--r--   0        0        0     1091 2023-07-27 19:27:39.723425 thrift_pyi-0.6.0/src/thriftpyi/cli.py
+-rw-r--r--   0        0        0      183 2023-07-27 19:27:39.723425 thrift_pyi-0.6.0/src/thriftpyi/compat.py
+-rw-r--r--   0        0        0     5064 2023-07-27 19:27:39.723425 thrift_pyi-0.6.0/src/thriftpyi/entities.py
+-rw-r--r--   0        0        0      391 2023-07-27 19:27:39.723425 thrift_pyi-0.6.0/src/thriftpyi/files.py
+-rw-r--r--   0        0        0     1262 2023-07-27 19:27:39.723425 thrift_pyi-0.6.0/src/thriftpyi/main.py
+-rw-r--r--   0        0        0     5116 2023-07-27 19:27:39.723425 thrift_pyi-0.6.0/src/thriftpyi/proxies.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:27:39.723425 thrift_pyi-0.6.0/src/thriftpyi/py.typed
+-rw-r--r--   0        0        0     2515 2023-07-27 19:27:39.723425 thrift_pyi-0.6.0/src/thriftpyi/stubs.py
+-rw-r--r--   0        0        0     2079 2023-07-27 19:27:39.723425 thrift_pyi-0.6.0/src/thriftpyi/utils.py
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 thrift_pyi-0.6.0/PKG-INFO
```

### Comparing `thrift_pyi-0.5.0/LICENSE` & `thrift_pyi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thrift_pyi-0.5.0/README.rst` & `thrift_pyi-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `thrift_pyi-0.5.0/pyproject.toml` & `thrift_pyi-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thrift-pyi"
-version = "0.5.0"
+version = "0.6.0"
 description = "This is simple `.pyi` stubs generator from thrift interfaces"
 readme = "README.rst"
 repository = "https://github.com/unmade/thrift-pyi"
 authors = ["Aleksei Maslakov <lesha.maslakov@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "thriftpyi", from = "src" },
```

### Comparing `thrift_pyi-0.5.0/src/thriftpyi/cli.py` & `thrift_pyi-0.6.0/src/thriftpyi/cli.py`

 * *Files identical despite different names*

### Comparing `thrift_pyi-0.5.0/src/thriftpyi/entities.py` & `thrift_pyi-0.6.0/src/thriftpyi/entities.py`

 * *Files identical despite different names*

### Comparing `thrift_pyi-0.5.0/src/thriftpyi/main.py` & `thrift_pyi-0.6.0/src/thriftpyi/main.py`

 * *Files identical despite different names*

### Comparing `thrift_pyi-0.5.0/src/thriftpyi/proxies.py` & `thrift_pyi-0.6.0/src/thriftpyi/proxies.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         )
 
         fields = spec.get_fields()
         methods = []
         if fields:
             methods.append(Method(name="__init__", args=fields))
 
-        return ModuleItem(name=texc.__name__, methods=methods)
+        return ModuleItem(name=texc.__name__, methods=methods, fields=fields)
 
     @classmethod
     def _make_service(cls, tservice) -> ModuleItem:
         return ModuleItem(
             name=tservice.__name__,
             methods=[
                 Method(
```

### Comparing `thrift_pyi-0.5.0/src/thriftpyi/stubs.py` & `thrift_pyi-0.6.0/src/thriftpyi/stubs.py`

 * *Files identical despite different names*

### Comparing `thrift_pyi-0.5.0/src/thriftpyi/utils.py` & `thrift_pyi-0.6.0/src/thriftpyi/utils.py`

 * *Files identical despite different names*

### Comparing `thrift_pyi-0.5.0/PKG-INFO` & `thrift_pyi-0.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 Metadata-Version: 2.1
 Name: thrift-pyi
-Version: 0.5.0
+Version: 0.6.0
 Summary: This is simple `.pyi` stubs generator from thrift interfaces
 Home-page: https://github.com/unmade/thrift-pyi
 License: MIT
 Author: Aleksei Maslakov
 Author-email: lesha.maslakov@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Dist: astunparse (>=1.6.3,<2.0.0) ; python_full_version < "3.9.0"
 Requires-Dist: autoflake
 Requires-Dist: black
 Requires-Dist: thriftpy2 (>=0.4.2,<0.5.0)
 Project-URL: Repository, https://github.com/unmade/thrift-pyi
 Description-Content-Type: text/x-rst
```

