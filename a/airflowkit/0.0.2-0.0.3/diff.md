# Comparing `tmp/airflowkit-0.0.2.tar.gz` & `tmp/airflowkit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflowkit-0.0.2.tar", last modified: Thu Jul 27 08:30:22 2023, max compression
+gzip compressed data, was "airflowkit-0.0.3.tar", last modified: Thu Jul 27 09:42:56 2023, max compression
```

## Comparing `airflowkit-0.0.2.tar` & `airflowkit-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.874514 airflowkit-0.0.2/
--rw-r--r--   0 marc       (501) staff       (20)      394 2023-07-27 08:28:41.000000 airflowkit-0.0.2/CHANGELOG.md
--rw-r--r--   0 marc       (501) staff       (20)     1069 2023-03-25 13:22:59.000000 airflowkit-0.0.2/LICENSE
--rw-r--r--   0 marc       (501) staff       (20)       21 2023-03-25 13:22:59.000000 airflowkit-0.0.2/MANIFEST.in
--rw-r--r--   0 marc       (501) staff       (20)      460 2023-07-27 08:30:22.874354 airflowkit-0.0.2/PKG-INFO
--rw-r--r--   0 marc       (501) staff       (20)      142 2023-03-25 13:25:40.000000 airflowkit-0.0.2/README.md
--rw-r--r--   0 marc       (501) staff       (20)       38 2023-07-27 08:30:22.874559 airflowkit-0.0.2/setup.cfg
--rw-r--r--   0 marc       (501) staff       (20)     1043 2023-03-25 14:29:52.000000 airflowkit-0.0.2/setup.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.870630 airflowkit-0.0.2/src/
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.871650 airflowkit-0.0.2/src/airflowkit/
--rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:33:15.000000 airflowkit-0.0.2/src/airflowkit/__init__.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.872748 airflowkit-0.0.2/src/airflowkit/sensors/
--rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:27:19.000000 airflowkit-0.0.2/src/airflowkit/sensors/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)     4536 2023-07-27 08:27:10.000000 airflowkit-0.0.2/src/airflowkit/sensors/gcs_any_objects_existence_async_sensor.py
--rw-r--r--   0 marc       (501) staff       (20)     4501 2023-07-27 08:17:47.000000 airflowkit-0.0.2/src/airflowkit/sensors/gcs_objects_existence_async_sensor.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.873428 airflowkit-0.0.2/src/airflowkit/triggers/
--rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:27:19.000000 airflowkit-0.0.2/src/airflowkit/triggers/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)     3625 2023-07-27 08:26:10.000000 airflowkit-0.0.2/src/airflowkit/triggers/gcs_any_blobs_trigger.py
--rw-r--r--   0 marc       (501) staff       (20)     3567 2023-03-25 13:47:24.000000 airflowkit-0.0.2/src/airflowkit/triggers/gcs_blobs_trigger.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.872180 airflowkit-0.0.2/src/airflowkit.egg-info/
--rw-r--r--   0 marc       (501) staff       (20)      460 2023-07-27 08:30:22.000000 airflowkit-0.0.2/src/airflowkit.egg-info/PKG-INFO
--rw-r--r--   0 marc       (501) staff       (20)      580 2023-07-27 08:30:22.000000 airflowkit-0.0.2/src/airflowkit.egg-info/SOURCES.txt
--rw-r--r--   0 marc       (501) staff       (20)        1 2023-07-27 08:30:22.000000 airflowkit-0.0.2/src/airflowkit.egg-info/dependency_links.txt
--rw-r--r--   0 marc       (501) staff       (20)       62 2023-07-27 08:30:22.000000 airflowkit-0.0.2/src/airflowkit.egg-info/requires.txt
--rw-r--r--   0 marc       (501) staff       (20)       11 2023-07-27 08:30:22.000000 airflowkit-0.0.2/src/airflowkit.egg-info/top_level.txt
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.873668 airflowkit-0.0.2/tests/
--rw-r--r--   0 marc       (501) staff       (20)      215 2023-03-25 13:47:24.000000 airflowkit-0.0.2/tests/test_imports.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.475052 airflowkit-0.0.3/
+-rw-r--r--   0 marc       (501) staff       (20)      458 2023-07-27 09:42:03.000000 airflowkit-0.0.3/CHANGELOG.md
+-rw-r--r--   0 marc       (501) staff       (20)     1069 2023-03-25 13:22:59.000000 airflowkit-0.0.3/LICENSE
+-rw-r--r--   0 marc       (501) staff       (20)       21 2023-03-25 13:22:59.000000 airflowkit-0.0.3/MANIFEST.in
+-rw-r--r--   0 marc       (501) staff       (20)      460 2023-07-27 09:42:56.474911 airflowkit-0.0.3/PKG-INFO
+-rw-r--r--   0 marc       (501) staff       (20)      142 2023-03-25 13:25:40.000000 airflowkit-0.0.3/README.md
+-rw-r--r--   0 marc       (501) staff       (20)       38 2023-07-27 09:42:56.475094 airflowkit-0.0.3/setup.cfg
+-rw-r--r--   0 marc       (501) staff       (20)     1043 2023-07-27 09:41:18.000000 airflowkit-0.0.3/setup.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.472218 airflowkit-0.0.3/src/
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.473331 airflowkit-0.0.3/src/airflowkit/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:33:15.000000 airflowkit-0.0.3/src/airflowkit/__init__.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.474316 airflowkit-0.0.3/src/airflowkit/sensors/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:27:19.000000 airflowkit-0.0.3/src/airflowkit/sensors/__init__.py
+-rw-r--r--   0 marc       (501) staff       (20)     4536 2023-07-27 08:27:10.000000 airflowkit-0.0.3/src/airflowkit/sensors/gcs_any_objects_existence_async_sensor.py
+-rw-r--r--   0 marc       (501) staff       (20)     4501 2023-07-27 08:17:47.000000 airflowkit-0.0.3/src/airflowkit/sensors/gcs_objects_existence_async_sensor.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.474641 airflowkit-0.0.3/src/airflowkit/triggers/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:27:19.000000 airflowkit-0.0.3/src/airflowkit/triggers/__init__.py
+-rw-r--r--   0 marc       (501) staff       (20)     3625 2023-07-27 08:26:10.000000 airflowkit-0.0.3/src/airflowkit/triggers/gcs_any_blobs_trigger.py
+-rw-r--r--   0 marc       (501) staff       (20)     3566 2023-07-27 09:28:44.000000 airflowkit-0.0.3/src/airflowkit/triggers/gcs_blobs_trigger.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.473947 airflowkit-0.0.3/src/airflowkit.egg-info/
+-rw-r--r--   0 marc       (501) staff       (20)      460 2023-07-27 09:42:56.000000 airflowkit-0.0.3/src/airflowkit.egg-info/PKG-INFO
+-rw-r--r--   0 marc       (501) staff       (20)      580 2023-07-27 09:42:56.000000 airflowkit-0.0.3/src/airflowkit.egg-info/SOURCES.txt
+-rw-r--r--   0 marc       (501) staff       (20)        1 2023-07-27 09:42:56.000000 airflowkit-0.0.3/src/airflowkit.egg-info/dependency_links.txt
+-rw-r--r--   0 marc       (501) staff       (20)       62 2023-07-27 09:42:56.000000 airflowkit-0.0.3/src/airflowkit.egg-info/requires.txt
+-rw-r--r--   0 marc       (501) staff       (20)       11 2023-07-27 09:42:56.000000 airflowkit-0.0.3/src/airflowkit.egg-info/top_level.txt
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 09:42:56.474753 airflowkit-0.0.3/tests/
+-rw-r--r--   0 marc       (501) staff       (20)      215 2023-03-25 13:47:24.000000 airflowkit-0.0.3/tests/test_imports.py
```

### Comparing `airflowkit-0.0.2/LICENSE` & `airflowkit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `airflowkit-0.0.2/setup.py` & `airflowkit-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,14 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         # "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8, <3.9",
     install_requires=[
-        "apache-airflow[google]>=2.4.3",
+        "apache-airflow[google]>=2.5.3",
         "apache-airflow-providers-google",
     ],
     package_dir={'': 'src'},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     include_package_data=True,
 )
```

### Comparing `airflowkit-0.0.2/src/airflowkit/sensors/gcs_any_objects_existence_async_sensor.py` & `airflowkit-0.0.3/src/airflowkit/sensors/gcs_any_objects_existence_async_sensor.py`

 * *Files identical despite different names*

### Comparing `airflowkit-0.0.2/src/airflowkit/sensors/gcs_objects_existence_async_sensor.py` & `airflowkit-0.0.3/src/airflowkit/sensors/gcs_objects_existence_async_sensor.py`

 * *Files identical despite different names*

### Comparing `airflowkit-0.0.2/src/airflowkit/triggers/gcs_any_blobs_trigger.py` & `airflowkit-0.0.3/src/airflowkit/triggers/gcs_any_blobs_trigger.py`

 * *Files identical despite different names*

### Comparing `airflowkit-0.0.2/src/airflowkit/triggers/gcs_blobs_trigger.py` & `airflowkit-0.0.3/src/airflowkit/triggers/gcs_blobs_trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from airflow.providers.google.cloud.hooks.gcs import GCSAsyncHook
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
 class GCSBlobsTrigger(BaseTrigger):
     """
-    A trigger that fires and it finds the requested files or folders present in the given bucket.
+    A trigger that fires if it finds the requested files or folders present in the given bucket.
 
     :param bucket: the bucket in the google cloud storage where the objects are residing.
     :param objects_names: list of files or folders present in the bucket
     :param google_cloud_conn_id: reference to the Google Connection
     :param poke_interval: polling period in seconds to check for file/folder
     """
```

### Comparing `airflowkit-0.0.2/src/airflowkit.egg-info/SOURCES.txt` & `airflowkit-0.0.3/src/airflowkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

