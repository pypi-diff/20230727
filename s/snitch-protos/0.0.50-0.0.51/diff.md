# Comparing `tmp/snitch-protos-0.0.50.tar.gz` & `tmp/snitch-protos-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snitch-protos-0.0.50.tar", last modified: Wed Jul 26 22:55:28 2023, max compression
+gzip compressed data, was "snitch-protos-0.0.51.tar", last modified: Thu Jul 27 15:57:00 2023, max compression
```

## Comparing `snitch-protos-0.0.50.tar` & `snitch-protos-0.0.51.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:28.782901 snitch-protos-0.0.50/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 22:55:28.782901 snitch-protos-0.0.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 22:54:54.000000 snitch-protos-0.0.50/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:55:28.782901 snitch-protos-0.0.50/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-26 22:55:28.000000 snitch-protos-0.0.50/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:28.778901 snitch-protos-0.0.50/snitch_protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 22:54:54.000000 snitch-protos-0.0.50/snitch_protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:28.782901 snitch-protos-0.0.50/snitch_protos/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    32523 2023-07-26 22:54:54.000000 snitch-protos-0.0.50/snitch_protos/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:28.782901 snitch-protos-0.0.50/snitch_protos/protos/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-26 22:54:54.000000 snitch-protos-0.0.50/snitch_protos/protos/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:28.782901 snitch-protos-0.0.50/snitch_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 22:55:28.000000 snitch-protos-0.0.50/snitch_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-26 22:55:28.000000 snitch-protos-0.0.50/snitch_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:55:28.000000 snitch-protos-0.0.50/snitch_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 22:55:28.000000 snitch-protos-0.0.50/snitch_protos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:57:00.096790 snitch-protos-0.0.51/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 15:57:00.096790 snitch-protos-0.0.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-27 15:56:29.000000 snitch-protos-0.0.51/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 15:57:00.096790 snitch-protos-0.0.51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-27 15:56:59.000000 snitch-protos-0.0.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:57:00.096790 snitch-protos-0.0.51/snitch_protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:29.000000 snitch-protos-0.0.51/snitch_protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:57:00.096790 snitch-protos-0.0.51/snitch_protos/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    32523 2023-07-27 15:56:29.000000 snitch-protos-0.0.51/snitch_protos/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:57:00.096790 snitch-protos-0.0.51/snitch_protos/protos/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-27 15:56:29.000000 snitch-protos-0.0.51/snitch_protos/protos/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:57:00.096790 snitch-protos-0.0.51/snitch_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 15:57:00.000000 snitch-protos-0.0.51/snitch_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 15:57:00.000000 snitch-protos-0.0.51/snitch_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:57:00.000000 snitch-protos-0.0.51/snitch_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 15:57:00.000000 snitch-protos-0.0.51/snitch_protos.egg-info/top_level.txt
```

### Comparing `snitch-protos-0.0.50/PKG-INFO` & `snitch-protos-0.0.51/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.50
+Version: 0.0.51
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `snitch-protos-0.0.50/setup.py` & `snitch-protos-0.0.51/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='snitch-protos',
-    version='0.0.50',
+    version='0.0.51',
     description='Protobuf python package for Streamdal.com Snitch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/streamdal/snitch-protos',
     author='Streamdal.com',
     author_email='engineering@streamdal.com',
     license='MIT',
```

### Comparing `snitch-protos-0.0.50/snitch_protos/protos/__init__.py` & `snitch-protos-0.0.51/snitch_protos/protos/__init__.py`

 * *Files identical despite different names*

### Comparing `snitch-protos-0.0.50/snitch_protos/protos/steps/__init__.py` & `snitch-protos-0.0.51/snitch_protos/protos/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `snitch-protos-0.0.50/snitch_protos.egg-info/PKG-INFO` & `snitch-protos-0.0.51/snitch_protos.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.50
+Version: 0.0.51
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

