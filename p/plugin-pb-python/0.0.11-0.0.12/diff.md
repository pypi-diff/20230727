# Comparing `tmp/plugin-pb-python-0.0.11.tar.gz` & `tmp/plugin-pb-python-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugin-pb-python-0.0.11.tar", last modified: Fri Jul 21 14:01:48 2023, max compression
+gzip compressed data, was "plugin-pb-python-0.0.12.tar", last modified: Thu Jul 27 08:37:42 2023, max compression
```

## Comparing `plugin-pb-python-0.0.11.tar` & `plugin-pb-python-0.0.12.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:01:48.665773 plugin-pb-python-0.0.11/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-07-21 14:01:34.000000 plugin-pb-python-0.0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-21 14:01:48.665773 plugin-pb-python-0.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 14:01:34.000000 plugin-pb-python-0.0.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:01:48.657772 plugin-pb-python-0.0.11/cloudquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:01:48.661773 plugin-pb-python-0.0.11/cloudquery/plugin_v3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 14:01:34.000000 plugin-pb-python-0.0.11/cloudquery/plugin_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-07-21 14:01:34.000000 plugin-pb-python-0.0.11/cloudquery/plugin_v3/plugin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-21 14:01:34.000000 plugin-pb-python-0.0.11/cloudquery/plugin_v3/plugin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-21 14:01:34.000000 plugin-pb-python-0.0.11/cloudquery/plugin_v3/plugin_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:01:48.665773 plugin-pb-python-0.0.11/plugin_pb_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-21 14:01:48.000000 plugin-pb-python-0.0.11/plugin_pb_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-21 14:01:48.000000 plugin-pb-python-0.0.11/plugin_pb_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:01:48.000000 plugin-pb-python-0.0.11/plugin_pb_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 14:01:48.000000 plugin-pb-python-0.0.11/plugin_pb_python.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:01:48.000000 plugin-pb-python-0.0.11/plugin_pb_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-21 14:01:48.000000 plugin-pb-python-0.0.11/plugin_pb_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 14:01:48.000000 plugin-pb-python-0.0.11/plugin_pb_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 14:01:48.665773 plugin-pb-python-0.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-21 14:01:34.000000 plugin-pb-python-0.0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:42.462197 plugin-pb-python-0.0.12/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-27 08:37:42.462197 plugin-pb-python-0.0.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:42.458197 plugin-pb-python-0.0.12/cloudquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:42.458197 plugin-pb-python-0.0.12/cloudquery/discovery_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/discovery_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/discovery_v1/discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/discovery_v1/discovery_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/discovery_v1/discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/discovery_v1/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:42.462197 plugin-pb-python-0.0.12/cloudquery/plugin_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/plugin_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/plugin_v3/plugin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/plugin_v3/plugin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/plugin_v3/plugin_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/cloudquery/plugin_v3/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:37:42.462197 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 08:37:42.000000 plugin-pb-python-0.0.12/plugin_pb_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 08:37:42.462197 plugin-pb-python-0.0.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-27 08:37:26.000000 plugin-pb-python-0.0.12/setup.py
```

### Comparing `plugin-pb-python-0.0.11/LICENSE` & `plugin-pb-python-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.11/PKG-INFO` & `plugin-pb-python-0.0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugin-pb-python
-Version: 0.0.11
+Version: 0.0.12
 Summary: CloudQuery Plugin client and server library
 Home-page: https://github.com/cloudquery/plugin-pb-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
@@ -24,8 +24,8 @@
 
 Python Low Level Client for CloudQuery Plugin
 ================================================
 
 Overview
 -----------
 
-This is low level gRPC APIs for CloudQuery Plugin. Please see more on [github.com/cloudquery/plugin-pb-pyton](https://github.com/cloudquery/plugin-pb-pyton)
+This is low level gRPC APIs for CloudQuery Plugin. Please see more on [github.com/cloudquery/plugin-pb-python](https://github.com/cloudquery/plugin-pb-python)
```

### Comparing `plugin-pb-python-0.0.11/README.md` & `plugin-pb-python-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.11/cloudquery/plugin_v3/plugin_pb2.py` & `plugin-pb-python-0.0.12/cloudquery/plugin_v3/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.11/cloudquery/plugin_v3/plugin_pb2.pyi` & `plugin-pb-python-0.0.12/cloudquery/plugin_v3/plugin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.11/cloudquery/plugin_v3/plugin_pb2_grpc.py` & `plugin-pb-python-0.0.12/cloudquery/plugin_v3/plugin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `plugin-pb-python-0.0.11/plugin_pb_python.egg-info/PKG-INFO` & `plugin-pb-python-0.0.12/plugin_pb_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugin-pb-python
-Version: 0.0.11
+Version: 0.0.12
 Summary: CloudQuery Plugin client and server library
 Home-page: https://github.com/cloudquery/plugin-pb-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
@@ -24,8 +24,8 @@
 
 Python Low Level Client for CloudQuery Plugin
 ================================================
 
 Overview
 -----------
 
-This is low level gRPC APIs for CloudQuery Plugin. Please see more on [github.com/cloudquery/plugin-pb-pyton](https://github.com/cloudquery/plugin-pb-pyton)
+This is low level gRPC APIs for CloudQuery Plugin. Please see more on [github.com/cloudquery/plugin-pb-python](https://github.com/cloudquery/plugin-pb-python)
```

### Comparing `plugin-pb-python-0.0.11/setup.py` & `plugin-pb-python-0.0.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,25 @@
 long_description = """
 Python Low Level Client for CloudQuery Plugin
 ================================================
 
 Overview
 -----------
 
-This is low level gRPC APIs for CloudQuery Plugin. Please see more on [github.com/cloudquery/plugin-pb-pyton](https://github.com/cloudquery/plugin-pb-pyton)
+This is low level gRPC APIs for CloudQuery Plugin. Please see more on [github.com/cloudquery/plugin-pb-python](https://github.com/cloudquery/plugin-pb-python)
 """
 
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("cloudquery")
 ]
 setuptools.setup(
     name=name,
-    version="0.0.11",
+    version="0.0.12",
     description=description,
     long_description=long_description,
     author="CloudQuery LTD",
     author_email="pypi-packages@cloudquery.io",
     license="MPL-2.0",
     url=url,
     classifiers=[
@@ -60,10 +60,10 @@
     platforms="Posix; MacOS X; Windows",
     packages=packages,
     python_requires=">=3.7",
     namespace_packages=["cloudquery"],
     # namespace_packages=namespaces,
     install_requires=dependencies,
     include_package_data=True,
-    package_data={"cloudquery": ["plugin_v3/py.typed", "plugin_v3/*.pyi"]},
+    package_data={"cloudquery": ["plugin_v3/py.typed", "plugin_v3/*.pyi", "discovery_v1/py.typed", "discovery_v1/*.pyi"]},
     zip_safe=False,
-)
+)
```

