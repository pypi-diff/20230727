# Comparing `tmp/airflowkit-0.0.1.tar.gz` & `tmp/airflowkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflowkit-0.0.1.tar", last modified: Sat Mar 25 14:32:49 2023, max compression
+gzip compressed data, was "airflowkit-0.0.2.tar", last modified: Thu Jul 27 08:30:22 2023, max compression
```

## Comparing `airflowkit-0.0.1.tar` & `airflowkit-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-03-25 14:32:49.673695 airflowkit-0.0.1/
--rw-r--r--   0 marc       (501) staff       (20)      218 2023-03-25 14:32:16.000000 airflowkit-0.0.1/CHANGELOG.md
--rw-r--r--   0 marc       (501) staff       (20)     1069 2023-03-25 13:22:59.000000 airflowkit-0.0.1/LICENSE
--rw-r--r--   0 marc       (501) staff       (20)       21 2023-03-25 13:22:59.000000 airflowkit-0.0.1/MANIFEST.in
--rw-r--r--   0 marc       (501) staff       (20)      460 2023-03-25 14:32:49.673535 airflowkit-0.0.1/PKG-INFO
--rw-r--r--   0 marc       (501) staff       (20)      142 2023-03-25 13:25:40.000000 airflowkit-0.0.1/README.md
--rw-r--r--   0 marc       (501) staff       (20)       38 2023-03-25 14:32:49.673743 airflowkit-0.0.1/setup.cfg
--rw-r--r--   0 marc       (501) staff       (20)     1043 2023-03-25 14:29:52.000000 airflowkit-0.0.1/setup.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-03-25 14:32:49.669053 airflowkit-0.0.1/src/
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-03-25 14:32:49.670139 airflowkit-0.0.1/src/airflowkit/
--rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:33:15.000000 airflowkit-0.0.1/src/airflowkit/__init__.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-03-25 14:32:49.672301 airflowkit-0.0.1/src/airflowkit/sensors/
--rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:27:19.000000 airflowkit-0.0.1/src/airflowkit/sensors/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)     4502 2023-03-25 13:59:23.000000 airflowkit-0.0.1/src/airflowkit/sensors/gcs_objects_existence_async_sensor.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-03-25 14:32:49.672729 airflowkit-0.0.1/src/airflowkit/triggers/
--rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:27:19.000000 airflowkit-0.0.1/src/airflowkit/triggers/__init__.py
--rw-r--r--   0 marc       (501) staff       (20)     3567 2023-03-25 13:47:24.000000 airflowkit-0.0.1/src/airflowkit/triggers/gcs_blobs_trigger.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-03-25 14:32:49.672040 airflowkit-0.0.1/src/airflowkit.egg-info/
--rw-r--r--   0 marc       (501) staff       (20)      460 2023-03-25 14:32:49.000000 airflowkit-0.0.1/src/airflowkit.egg-info/PKG-INFO
--rw-r--r--   0 marc       (501) staff       (20)      466 2023-03-25 14:32:49.000000 airflowkit-0.0.1/src/airflowkit.egg-info/SOURCES.txt
--rw-r--r--   0 marc       (501) staff       (20)        1 2023-03-25 14:32:49.000000 airflowkit-0.0.1/src/airflowkit.egg-info/dependency_links.txt
--rw-r--r--   0 marc       (501) staff       (20)       62 2023-03-25 14:32:49.000000 airflowkit-0.0.1/src/airflowkit.egg-info/requires.txt
--rw-r--r--   0 marc       (501) staff       (20)       11 2023-03-25 14:32:49.000000 airflowkit-0.0.1/src/airflowkit.egg-info/top_level.txt
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-03-25 14:32:49.673144 airflowkit-0.0.1/tests/
--rw-r--r--   0 marc       (501) staff       (20)      215 2023-03-25 13:47:24.000000 airflowkit-0.0.1/tests/test_imports.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.874514 airflowkit-0.0.2/
+-rw-r--r--   0 marc       (501) staff       (20)      394 2023-07-27 08:28:41.000000 airflowkit-0.0.2/CHANGELOG.md
+-rw-r--r--   0 marc       (501) staff       (20)     1069 2023-03-25 13:22:59.000000 airflowkit-0.0.2/LICENSE
+-rw-r--r--   0 marc       (501) staff       (20)       21 2023-03-25 13:22:59.000000 airflowkit-0.0.2/MANIFEST.in
+-rw-r--r--   0 marc       (501) staff       (20)      460 2023-07-27 08:30:22.874354 airflowkit-0.0.2/PKG-INFO
+-rw-r--r--   0 marc       (501) staff       (20)      142 2023-03-25 13:25:40.000000 airflowkit-0.0.2/README.md
+-rw-r--r--   0 marc       (501) staff       (20)       38 2023-07-27 08:30:22.874559 airflowkit-0.0.2/setup.cfg
+-rw-r--r--   0 marc       (501) staff       (20)     1043 2023-03-25 14:29:52.000000 airflowkit-0.0.2/setup.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.870630 airflowkit-0.0.2/src/
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.871650 airflowkit-0.0.2/src/airflowkit/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:33:15.000000 airflowkit-0.0.2/src/airflowkit/__init__.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.872748 airflowkit-0.0.2/src/airflowkit/sensors/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:27:19.000000 airflowkit-0.0.2/src/airflowkit/sensors/__init__.py
+-rw-r--r--   0 marc       (501) staff       (20)     4536 2023-07-27 08:27:10.000000 airflowkit-0.0.2/src/airflowkit/sensors/gcs_any_objects_existence_async_sensor.py
+-rw-r--r--   0 marc       (501) staff       (20)     4501 2023-07-27 08:17:47.000000 airflowkit-0.0.2/src/airflowkit/sensors/gcs_objects_existence_async_sensor.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.873428 airflowkit-0.0.2/src/airflowkit/triggers/
+-rw-r--r--   0 marc       (501) staff       (20)        0 2023-03-25 13:27:19.000000 airflowkit-0.0.2/src/airflowkit/triggers/__init__.py
+-rw-r--r--   0 marc       (501) staff       (20)     3625 2023-07-27 08:26:10.000000 airflowkit-0.0.2/src/airflowkit/triggers/gcs_any_blobs_trigger.py
+-rw-r--r--   0 marc       (501) staff       (20)     3567 2023-03-25 13:47:24.000000 airflowkit-0.0.2/src/airflowkit/triggers/gcs_blobs_trigger.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.872180 airflowkit-0.0.2/src/airflowkit.egg-info/
+-rw-r--r--   0 marc       (501) staff       (20)      460 2023-07-27 08:30:22.000000 airflowkit-0.0.2/src/airflowkit.egg-info/PKG-INFO
+-rw-r--r--   0 marc       (501) staff       (20)      580 2023-07-27 08:30:22.000000 airflowkit-0.0.2/src/airflowkit.egg-info/SOURCES.txt
+-rw-r--r--   0 marc       (501) staff       (20)        1 2023-07-27 08:30:22.000000 airflowkit-0.0.2/src/airflowkit.egg-info/dependency_links.txt
+-rw-r--r--   0 marc       (501) staff       (20)       62 2023-07-27 08:30:22.000000 airflowkit-0.0.2/src/airflowkit.egg-info/requires.txt
+-rw-r--r--   0 marc       (501) staff       (20)       11 2023-07-27 08:30:22.000000 airflowkit-0.0.2/src/airflowkit.egg-info/top_level.txt
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2023-07-27 08:30:22.873668 airflowkit-0.0.2/tests/
+-rw-r--r--   0 marc       (501) staff       (20)      215 2023-03-25 13:47:24.000000 airflowkit-0.0.2/tests/test_imports.py
```

### Comparing `airflowkit-0.0.1/LICENSE` & `airflowkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airflowkit-0.0.1/setup.py` & `airflowkit-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `airflowkit-0.0.1/src/airflowkit/sensors/gcs_objects_existence_async_sensor.py` & `airflowkit-0.0.2/src/airflowkit/sensors/gcs_objects_existence_async_sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class GCSObjectsExistenceAsyncSensor(BaseSensorOperator):
     """
-    Checks for the existence of a file in Google Cloud Storage.
+    Checks for the existence of files in Google Cloud Storage.
 
     :param bucket: The Google Cloud Storage bucket where the object is.
     :param objects: The names of the objects to check in the Google cloud
         storage bucket.
     :param google_cloud_conn_id: The connection ID to use when
         connecting to Google Cloud Storage.
     :param delegate_to: The account to impersonate using domain-wide delegation of authority,
```

### Comparing `airflowkit-0.0.1/src/airflowkit/triggers/gcs_blobs_trigger.py` & `airflowkit-0.0.2/src/airflowkit/triggers/gcs_blobs_trigger.py`

 * *Files identical despite different names*

