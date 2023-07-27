# Comparing `tmp/lytekitplugins-pods-0.4.0.tar.gz` & `tmp/lytekitplugins-pods-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytekitplugins-pods-0.4.0.tar", last modified: Sat Oct 15 19:47:21 2022, max compression
+gzip compressed data, was "lytekitplugins-pods-0.5.0.tar", last modified: Thu Jul 27 18:48:22 2023, max compression
```

## Comparing `lytekitplugins-pods-0.4.0.tar` & `lytekitplugins-pods-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-15 19:47:21.076002 lytekitplugins-pods-0.4.0/
--rw-r--r--   0 ayush      (504) staff       (20)      843 2022-10-15 19:47:21.075700 lytekitplugins-pods-0.4.0/PKG-INFO
--rw-r--r--   0 ayush      (504) staff       (20)      727 2022-06-07 01:08:15.000000 lytekitplugins-pods-0.4.0/README.md
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-15 19:47:21.071833 lytekitplugins-pods-0.4.0/flytekitplugins/
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-15 19:47:21.073321 lytekitplugins-pods-0.4.0/flytekitplugins/pod/
--rw-r--r--   0 ayush      (504) staff       (20)      216 2022-06-07 01:08:15.000000 lytekitplugins-pods-0.4.0/flytekitplugins/pod/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)     5644 2022-10-15 19:45:52.000000 lytekitplugins-pods-0.4.0/flytekitplugins/pod/task.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2022-10-15 19:47:21.075121 lytekitplugins-pods-0.4.0/lytekitplugins_pods.egg-info/
--rw-r--r--   0 ayush      (504) staff       (20)      843 2022-10-15 19:47:21.000000 lytekitplugins-pods-0.4.0/lytekitplugins_pods.egg-info/PKG-INFO
--rw-r--r--   0 ayush      (504) staff       (20)      344 2022-10-15 19:47:21.000000 lytekitplugins-pods-0.4.0/lytekitplugins_pods.egg-info/SOURCES.txt
--rw-r--r--   0 ayush      (504) staff       (20)        1 2022-10-15 19:47:21.000000 lytekitplugins-pods-0.4.0/lytekitplugins_pods.egg-info/dependency_links.txt
--rw-r--r--   0 ayush      (504) staff       (20)       16 2022-10-15 19:47:21.000000 lytekitplugins-pods-0.4.0/lytekitplugins_pods.egg-info/namespace_packages.txt
--rw-r--r--   0 ayush      (504) staff       (20)       34 2022-10-15 19:47:21.000000 lytekitplugins-pods-0.4.0/lytekitplugins_pods.egg-info/requires.txt
--rw-r--r--   0 ayush      (504) staff       (20)       16 2022-10-15 19:47:21.000000 lytekitplugins-pods-0.4.0/lytekitplugins_pods.egg-info/top_level.txt
--rw-r--r--   0 ayush      (504) staff       (20)       38 2022-10-15 19:47:21.076128 lytekitplugins-pods-0.4.0/setup.cfg
--rw-r--r--   0 ayush      (504) staff       (20)     1200 2022-10-15 19:47:06.000000 lytekitplugins-pods-0.4.0/setup.py
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 18:48:22.401434 lytekitplugins-pods-0.5.0/
+-rw-r--r--   0 aidan      (501) staff       (20)      890 2023-07-27 18:48:22.400859 lytekitplugins-pods-0.5.0/PKG-INFO
+-rw-r--r--   0 aidan      (501) staff       (20)      727 2022-10-03 21:59:15.000000 lytekitplugins-pods-0.5.0/README.md
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 18:48:22.397171 lytekitplugins-pods-0.5.0/flytekitplugins/
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 18:48:22.398314 lytekitplugins-pods-0.5.0/flytekitplugins/pod/
+-rw-r--r--   0 aidan      (501) staff       (20)      216 2022-10-03 21:59:15.000000 lytekitplugins-pods-0.5.0/flytekitplugins/pod/__init__.py
+-rw-r--r--   0 aidan      (501) staff       (20)     5608 2023-07-27 18:36:35.000000 lytekitplugins-pods-0.5.0/flytekitplugins/pod/task.py
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 18:48:22.400274 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/
+-rw-r--r--   0 aidan      (501) staff       (20)      890 2023-07-27 18:48:22.000000 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/PKG-INFO
+-rw-r--r--   0 aidan      (501) staff       (20)      344 2023-07-27 18:48:22.000000 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/SOURCES.txt
+-rw-r--r--   0 aidan      (501) staff       (20)        1 2023-07-27 18:48:22.000000 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/dependency_links.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       16 2023-07-27 18:48:22.000000 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/namespace_packages.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       35 2023-07-27 18:48:22.000000 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/requires.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       16 2023-07-27 18:48:22.000000 lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/top_level.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       38 2023-07-27 18:48:22.401566 lytekitplugins-pods-0.5.0/setup.cfg
+-rw-r--r--   0 aidan      (501) staff       (20)     1200 2023-07-27 18:48:14.000000 lytekitplugins-pods-0.5.0/setup.py
```

### Comparing `lytekitplugins-pods-0.4.0/PKG-INFO` & `lytekitplugins-pods-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: lytekitplugins-pods
-Version: 0.4.0
+Version: 0.5.0
 Summary: Flytekit plugin to support K8s Pod tasks
+Home-page: UNKNOWN
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
+
+UNKNOWN
+
```

### Comparing `lytekitplugins-pods-0.4.0/README.md` & `lytekitplugins-pods-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lytekitplugins-pods-0.4.0/flytekitplugins/pod/task.py` & `lytekitplugins-pods-0.5.0/flytekitplugins/pod/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from kubernetes.client import ApiClient
 from kubernetes.client.models import V1Container, V1EnvVar, V1PodSpec, V1ResourceRequirements
 
 from flytekit import FlyteContext, PythonFunctionTask
 from flytekit.configuration import SerializationSettings
 from flytekit.exceptions import user as _user_exceptions
 from flytekit.extend import Promise, TaskPlugins
-from flytekit.loggers import logger
 from flytekit.models import task as _task_models
 
 _PRIMARY_CONTAINER_NAME_FIELD = "primary_container_name"
 
 
 def _sanitize_resource_name(resource: _task_models.Resources.ResourceEntry) -> str:
     return _core_task.Resources.ResourceName.Name(resource.name).lower().replace("_", "-")
```

### Comparing `lytekitplugins-pods-0.4.0/lytekitplugins_pods.egg-info/PKG-INFO` & `lytekitplugins-pods-0.5.0/lytekitplugins_pods.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: lytekitplugins-pods
-Version: 0.4.0
+Version: 0.5.0
 Summary: Flytekit plugin to support K8s Pod tasks
+Home-page: UNKNOWN
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
+
+UNKNOWN
+
```

### Comparing `lytekitplugins-pods-0.4.0/setup.py` & `lytekitplugins-pods-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 PLUGIN_NAME = "pod"
 
 microlib_name = "lytekitplugins-pods"
 
 plugin_requires = [
-    "lytekit>=0.2.2",
     "kubernetes>=12.0.1",
+    "lytekit==0.15.0"
 ]
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Flytekit plugin to support K8s Pod tasks",
```

