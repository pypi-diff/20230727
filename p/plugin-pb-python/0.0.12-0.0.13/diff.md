# Comparing `tmp/plugin-pb-python-0.0.12.tar.gz` & `tmp/plugin-pb-python-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugin-pb-python-0.0.12.tar", last modified: Thu Jul 27 08:37:42 2023, max compression
+gzip compressed data, was "plugin-pb-python-0.0.13.tar", last modified: Thu Jul 27 12:09:49 2023, max compression
```

## Comparing `plugin-pb-python-0.0.12.tar` & `plugin-pb-python-0.0.13.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:42.462197 plugin-pb-python-0.0.12/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-27 08:37:42.462197 plugin-pb-python-0.0.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:42.458197 plugin-pb-python-0.0.12/cloudquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:42.458197 plugin-pb-python-0.0.12/cloudquery/discovery_v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/discovery_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/discovery_v1/discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/discovery_v1/discovery_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/discovery_v1/discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/discovery_v1/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:42.462197 plugin-pb-python-0.0.12/cloudquery/plugin_v3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/plugin_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/plugin_v3/plugin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/plugin_v3/plugin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/plugin_v3/plugin_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/plugin_v3/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:42.462197 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 08:37:42.462197 plugin-pb-python-0.0.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:09:49.148550 plugin-pb-python-0.0.13/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-27 12:09:49.148550 plugin-pb-python-0.0.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:09:49.144550 plugin-pb-python-0.0.13/cloudquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:09:49.144550 plugin-pb-python-0.0.13/cloudquery/discovery_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/cloudquery/discovery_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/cloudquery/discovery_v1/discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/cloudquery/discovery_v1/discovery_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/cloudquery/discovery_v1/discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/cloudquery/discovery_v1/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:09:49.148550 plugin-pb-python-0.0.13/cloudquery/plugin_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/cloudquery/plugin_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/cloudquery/plugin_v3/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/cloudquery/plugin_v3/plugin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/cloudquery/plugin_v3/plugin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/cloudquery/plugin_v3/plugin_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/cloudquery/plugin_v3/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:09:49.148550 plugin-pb-python-0.0.13/plugin_pb_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-27 12:09:49.000000 plugin-pb-python-0.0.13/plugin_pb_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-27 12:09:49.000000 plugin-pb-python-0.0.13/plugin_pb_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:09:49.000000 plugin-pb-python-0.0.13/plugin_pb_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 12:09:49.000000 plugin-pb-python-0.0.13/plugin_pb_python.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:09:48.000000 plugin-pb-python-0.0.13/plugin_pb_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 12:09:49.000000 plugin-pb-python-0.0.13/plugin_pb_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 12:09:49.000000 plugin-pb-python-0.0.13/plugin_pb_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 12:09:49.148550 plugin-pb-python-0.0.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-27 12:09:32.000000 plugin-pb-python-0.0.13/setup.py
```

### Comparing `plugin-pb-python-0.0.12/LICENSE` & `plugin-pb-python-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.12/PKG-INFO` & `plugin-pb-python-0.0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugin-pb-python
-Version: 0.0.12
+Version: 0.0.13
 Summary: CloudQuery Plugin client and server library
 Home-page: https://github.com/cloudquery/plugin-pb-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `plugin-pb-python-0.0.12/README.md` & `plugin-pb-python-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.12/cloudquery/discovery_v1/discovery_pb2.py` & `plugin-pb-python-0.0.13/cloudquery/discovery_v1/discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.12/cloudquery/discovery_v1/discovery_pb2.pyi` & `plugin-pb-python-0.0.13/cloudquery/discovery_v1/discovery_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.12/cloudquery/discovery_v1/discovery_pb2_grpc.py` & `plugin-pb-python-0.0.13/cloudquery/discovery_v1/discovery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.12/cloudquery/plugin_v3/plugin_pb2.py` & `plugin-pb-python-0.0.13/cloudquery/plugin_v3/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.12/cloudquery/plugin_v3/plugin_pb2.pyi` & `plugin-pb-python-0.0.13/cloudquery/plugin_v3/plugin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.12/cloudquery/plugin_v3/plugin_pb2_grpc.py` & `plugin-pb-python-0.0.13/cloudquery/plugin_v3/plugin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.12/plugin_pb_python.egg-info/PKG-INFO` & `plugin-pb-python-0.0.13/plugin_pb_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugin-pb-python
-Version: 0.0.12
+Version: 0.0.13
 Summary: CloudQuery Plugin client and server library
 Home-page: https://github.com/cloudquery/plugin-pb-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `plugin-pb-python-0.0.12/plugin_pb_python.egg-info/SOURCES.txt` & `plugin-pb-python-0.0.13/plugin_pb_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 cloudquery/discovery_v1/__init__.py
 cloudquery/discovery_v1/discovery_pb2.py
 cloudquery/discovery_v1/discovery_pb2.pyi
 cloudquery/discovery_v1/discovery_pb2_grpc.py
 cloudquery/discovery_v1/py.typed
 cloudquery/plugin_v3/__init__.py
+cloudquery/plugin_v3/arrow.py
 cloudquery/plugin_v3/plugin_pb2.py
 cloudquery/plugin_v3/plugin_pb2.pyi
 cloudquery/plugin_v3/plugin_pb2_grpc.py
 cloudquery/plugin_v3/py.typed
 plugin_pb_python.egg-info/PKG-INFO
 plugin_pb_python.egg-info/SOURCES.txt
 plugin_pb_python.egg-info/dependency_links.txt
```

### Comparing `plugin-pb-python-0.0.12/setup.py` & `plugin-pb-python-0.0.13/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 description = "CloudQuery Plugin client and server library"
 
 dependencies = [
     "grpcio >= 1.56.0",
     "grpcio-tools >= 1.56.0",
     "protobuf >= 4.23.4",
+    "pyarrow >= 12.0.1"
 ]
 url = "https://github.com/cloudquery/plugin-pb-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 long_description = """
 Python Low Level Client for CloudQuery Plugin
@@ -32,15 +33,15 @@
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("cloudquery")
 ]
 setuptools.setup(
     name=name,
-    version="0.0.12",
+    version="0.0.13",
     description=description,
     long_description=long_description,
     author="CloudQuery LTD",
     author_email="pypi-packages@cloudquery.io",
     license="MPL-2.0",
     url=url,
     classifiers=[
```

