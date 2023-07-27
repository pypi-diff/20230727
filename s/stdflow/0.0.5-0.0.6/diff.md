# Comparing `tmp/stdflow-0.0.5.tar.gz` & `tmp/stdflow-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdflow-0.0.5.tar", last modified: Wed Jul 26 02:02:42 2023, max compression
+gzip compressed data, was "stdflow-0.0.6.tar", last modified: Thu Jul 27 03:03:43 2023, max compression
```

## Comparing `stdflow-0.0.5.tar` & `stdflow-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:02:42.891794 stdflow-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-26 02:02:26.000000 stdflow-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-26 02:02:42.891794 stdflow-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-26 02:02:26.000000 stdflow-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-26 02:02:26.000000 stdflow-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 02:02:42.891794 stdflow-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:02:42.891794 stdflow-0.0.5/stdflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-26 02:02:42.000000 stdflow-0.0.5/stdflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-26 02:02:42.000000 stdflow-0.0.5/stdflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 02:02:42.000000 stdflow-0.0.5/stdflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-26 02:02:42.000000 stdflow-0.0.5/stdflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 02:02:42.000000 stdflow-0.0.5/stdflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:03:43.808923 stdflow-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 03:03:32.000000 stdflow-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-27 03:03:43.808923 stdflow-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-27 03:03:32.000000 stdflow-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-27 03:03:32.000000 stdflow-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 03:03:43.808923 stdflow-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:03:43.808923 stdflow-0.0.6/stdflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-27 03:03:43.000000 stdflow-0.0.6/stdflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-27 03:03:43.000000 stdflow-0.0.6/stdflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:03:43.000000 stdflow-0.0.6/stdflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-27 03:03:43.000000 stdflow-0.0.6/stdflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 03:03:43.000000 stdflow-0.0.6/stdflow.egg-info/top_level.txt
```

### Comparing `stdflow-0.0.5/LICENSE` & `stdflow-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.5/pyproject.toml` & `stdflow-0.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -3,36 +3,44 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ["stdflow"]
 
 [project]
 name = "stdflow"
-version = "0.0.5"
+version = "0.0.6"
 description = "[alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output."
 readme = "README.md"
 authors = [
     { name = "Cyprien Ricque", email = "ricque.cyprien@gmail.com" },
 ]
 keywords = ["data science", "data", "flow", "data flow"]
-requires-python = ">=3.9"
+requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     'License :: OSI Approved :: MIT License',
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
-    "pandas~=2.0.3",
-    "datetime~=5.2",
-    "python-box[all]~=7.0",
+    # Python 3.9
+    "pandas>=2.0.0; python_version>='3.9'",
+
+    # Python 3.7
+    "typing-extensions>=4.7.1; python_version<'3.8'",
+    "pandas~=1.3.5; python_version<'3.8'",
+
+    # Any
     "openpyxl~=3.1.2",
-    "python-box~=7.0.1"
+    "python-box[all]~=7.0",
 ]
 
 
+
 [tool.isort]
 profile = "black"
 
 [tool.black]
 line-length = 100
 target-version = ['py39']
```

