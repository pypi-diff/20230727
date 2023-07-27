# Comparing `tmp/stdflow-0.0.6.tar.gz` & `tmp/stdflow-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdflow-0.0.6.tar", last modified: Thu Jul 27 03:03:43 2023, max compression
+gzip compressed data, was "stdflow-0.0.7.tar", last modified: Thu Jul 27 03:54:28 2023, max compression
```

## Comparing `stdflow-0.0.6.tar` & `stdflow-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:03:43.808923 stdflow-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 03:03:32.000000 stdflow-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-27 03:03:43.808923 stdflow-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-27 03:03:32.000000 stdflow-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-27 03:03:32.000000 stdflow-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 03:03:43.808923 stdflow-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:03:43.808923 stdflow-0.0.6/stdflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-27 03:03:43.000000 stdflow-0.0.6/stdflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-27 03:03:43.000000 stdflow-0.0.6/stdflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:03:43.000000 stdflow-0.0.6/stdflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-27 03:03:43.000000 stdflow-0.0.6/stdflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 03:03:43.000000 stdflow-0.0.6/stdflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:28.677455 stdflow-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 03:54:15.000000 stdflow-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-27 03:54:28.677455 stdflow-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-27 03:54:15.000000 stdflow-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-27 03:54:15.000000 stdflow-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 03:54:28.677455 stdflow-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:28.677455 stdflow-0.0.7/stdflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-27 03:54:28.000000 stdflow-0.0.7/stdflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-27 03:54:28.000000 stdflow-0.0.7/stdflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:54:28.000000 stdflow-0.0.7/stdflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-27 03:54:28.000000 stdflow-0.0.7/stdflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 03:54:28.000000 stdflow-0.0.7/stdflow.egg-info/top_level.txt
```

### Comparing `stdflow-0.0.6/LICENSE` & `stdflow-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.6/PKG-INFO` & `stdflow-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdflow
-Version: 0.0.6
+Version: 0.0.7
 Summary: [alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output.
 Author-email: Cyprien Ricque <ricque.cyprien@gmail.com>
 Keywords: data science,data,flow,data flow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `stdflow-0.0.6/README.md` & `stdflow-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.6/pyproject.toml` & `stdflow-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ["stdflow"]
 
 [project]
 name = "stdflow"
-version = "0.0.6"
+version = "0.0.7"
 description = "[alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output."
 readme = "README.md"
 authors = [
     { name = "Cyprien Ricque", email = "ricque.cyprien@gmail.com" },
 ]
 keywords = ["data science", "data", "flow", "data flow"]
 requires-python = ">=3.7"
```

### Comparing `stdflow-0.0.6/stdflow.egg-info/PKG-INFO` & `stdflow-0.0.7/stdflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdflow
-Version: 0.0.6
+Version: 0.0.7
 Summary: [alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output.
 Author-email: Cyprien Ricque <ricque.cyprien@gmail.com>
 Keywords: data science,data,flow,data flow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

