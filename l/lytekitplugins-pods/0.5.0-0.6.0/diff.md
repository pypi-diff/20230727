# Comparing `tmp/lytekitplugins-pods-0.5.0.tar.gz` & `tmp/lytekitplugins-pods-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytekitplugins-pods-0.5.0.tar", last modified: Thu Jul 27 18:48:22 2023, max compression
+gzip compressed data, was "lytekitplugins-pods-0.6.0.tar", last modified: Thu Jul 27 19:15:11 2023, max compression
```

## Comparing `lytekitplugins-pods-0.5.0.tar` & `lytekitplugins-pods-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 18:48:22.401434 lytekitplugins-pods-0.5.0/
--rw-r--r--   0 aidan      (501) staff       (20)      890 2023-07-27 18:48:22.400859 lytekitplugins-pods-0.5.0/PKG-INFO
--rw-r--r--   0 aidan      (501) staff       (20)      727 2022-10-03 21:59:15.000000 lytekitplugins-pods-0.5.0/README.md
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 18:48:22.397171 lytekitplugins-pods-0.5.0/flytekitplugins/
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 18:48:22.398314 lytekitplugins-pods-0.5.0/flytekitplugins/pod/
--rw-r--r--   0 aidan      (501) staff       (20)      216 2022-10-03 21:59:15.000000 lytekitplugins-pods-0.5.0/flytekitplugins/pod/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     5608 2023-07-27 18:36:35.000000 lytekitplugins-pods-0.5.0/flytekitplugins/pod/task.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 18:48:22.400274 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/
--rw-r--r--   0 aidan      (501) staff       (20)      890 2023-07-27 18:48:22.000000 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/PKG-INFO
--rw-r--r--   0 aidan      (501) staff       (20)      344 2023-07-27 18:48:22.000000 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/SOURCES.txt
--rw-r--r--   0 aidan      (501) staff       (20)        1 2023-07-27 18:48:22.000000 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/dependency_links.txt
--rw-r--r--   0 aidan      (501) staff       (20)       16 2023-07-27 18:48:22.000000 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/namespace_packages.txt
--rw-r--r--   0 aidan      (501) staff       (20)       35 2023-07-27 18:48:22.000000 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/requires.txt
--rw-r--r--   0 aidan      (501) staff       (20)       16 2023-07-27 18:48:22.000000 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/top_level.txt
--rw-r--r--   0 aidan      (501) staff       (20)       38 2023-07-27 18:48:22.401566 lytekitplugins-pods-0.5.0/setup.cfg
--rw-r--r--   0 aidan      (501) staff       (20)     1200 2023-07-27 18:48:14.000000 lytekitplugins-pods-0.5.0/setup.py
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 19:15:11.114151 lytekitplugins-pods-0.6.0/
+-rw-r--r--   0 aidan      (501) staff       (20)      890 2023-07-27 19:15:11.113739 lytekitplugins-pods-0.6.0/PKG-INFO
+-rw-r--r--   0 aidan      (501) staff       (20)      727 2022-10-03 21:59:15.000000 lytekitplugins-pods-0.6.0/README.md
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 19:15:11.110719 lytekitplugins-pods-0.6.0/flytekitplugins/
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 19:15:11.111597 lytekitplugins-pods-0.6.0/flytekitplugins/pod/
+-rw-r--r--   0 aidan      (501) staff       (20)      216 2022-10-03 21:59:15.000000 lytekitplugins-pods-0.6.0/flytekitplugins/pod/__init__.py
+-rw-r--r--   0 aidan      (501) staff       (20)     5608 2023-07-27 18:36:35.000000 lytekitplugins-pods-0.6.0/flytekitplugins/pod/task.py
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 19:15:11.113258 lytekitplugins-pods-0.6.0/lytekitplugins_pods.egg-info/
+-rw-r--r--   0 aidan      (501) staff       (20)      890 2023-07-27 19:15:11.000000 lytekitplugins-pods-0.6.0/lytekitplugins_pods.egg-info/PKG-INFO
+-rw-r--r--   0 aidan      (501) staff       (20)      344 2023-07-27 19:15:11.000000 lytekitplugins-pods-0.6.0/lytekitplugins_pods.egg-info/SOURCES.txt
+-rw-r--r--   0 aidan      (501) staff       (20)        1 2023-07-27 19:15:11.000000 lytekitplugins-pods-0.6.0/lytekitplugins_pods.egg-info/dependency_links.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       16 2023-07-27 19:15:11.000000 lytekitplugins-pods-0.6.0/lytekitplugins_pods.egg-info/namespace_packages.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       35 2023-07-27 19:15:11.000000 lytekitplugins-pods-0.6.0/lytekitplugins_pods.egg-info/requires.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       16 2023-07-27 19:15:11.000000 lytekitplugins-pods-0.6.0/lytekitplugins_pods.egg-info/top_level.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       38 2023-07-27 19:15:11.114295 lytekitplugins-pods-0.6.0/setup.cfg
+-rw-r--r--   0 aidan      (501) staff       (20)     1200 2023-07-27 19:15:08.000000 lytekitplugins-pods-0.6.0/setup.py
```

### Comparing `lytekitplugins-pods-0.5.0/PKG-INFO` & `lytekitplugins-pods-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytekitplugins-pods
-Version: 0.5.0
+Version: 0.6.0
 Summary: Flytekit plugin to support K8s Pod tasks
 Home-page: UNKNOWN
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lytekitplugins-pods-0.5.0/README.md` & `lytekitplugins-pods-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `lytekitplugins-pods-0.5.0/flytekitplugins/pod/task.py` & `lytekitplugins-pods-0.6.0/flytekitplugins/pod/task.py`

 * *Files identical despite different names*

### Comparing `lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/PKG-INFO` & `lytekitplugins-pods-0.6.0/lytekitplugins_pods.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytekitplugins-pods
-Version: 0.5.0
+Version: 0.6.0
 Summary: Flytekit plugin to support K8s Pod tasks
 Home-page: UNKNOWN
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lytekitplugins-pods-0.5.0/setup.py` & `lytekitplugins-pods-0.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 PLUGIN_NAME = "pod"
 
 microlib_name = "lytekitplugins-pods"
 
 plugin_requires = [
     "kubernetes>=12.0.1",
-    "lytekit==0.15.0"
+    "lytekit==0.15.1"
 ]
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Flytekit plugin to support K8s Pod tasks",
```

