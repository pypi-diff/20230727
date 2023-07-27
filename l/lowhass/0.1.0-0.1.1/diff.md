# Comparing `tmp/lowhass-0.1.0.tar.gz` & `tmp/lowhass-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lowhass-0.1.0.tar", last modified: Thu Jul 27 19:56:07 2023, max compression
+gzip compressed data, was "lowhass-0.1.1.tar", last modified: Thu Jul 27 20:16:32 2023, max compression
```

## Comparing `lowhass-0.1.0.tar` & `lowhass-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 itec      (1000) itec      (1000)        0 2023-07-27 19:56:07.204992 lowhass-0.1.0/
--rw-r--r--   0 itec      (1000) itec      (1000)     3078 2023-07-27 16:08:28.000000 lowhass-0.1.0/.gitignore
--rw-r--r--   0 itec      (1000) itec      (1000)     1068 2023-07-27 16:08:28.000000 lowhass-0.1.0/LICENSE
--rw-r--r--   0 itec      (1000) itec      (1000)      343 2023-07-27 19:56:07.204992 lowhass-0.1.0/PKG-INFO
--rw-r--r--   0 itec      (1000) itec      (1000)       65 2023-07-27 19:55:35.000000 lowhass-0.1.0/README.md
-drwxr-xr-x   0 itec      (1000) itec      (1000)        0 2023-07-27 19:56:07.201659 lowhass-0.1.0/lowhass/
--rw-r--r--   0 itec      (1000) itec      (1000)      293 2023-07-27 19:52:02.000000 lowhass-0.1.0/lowhass/__init__.py
--rw-r--r--   0 itec      (1000) itec      (1000)     2007 2023-07-27 18:00:21.000000 lowhass-0.1.0/lowhass/rest_client.py
-drwxr-xr-x   0 itec      (1000) itec      (1000)        0 2023-07-27 19:56:07.204992 lowhass-0.1.0/lowhass/typings/
--rw-r--r--   0 itec      (1000) itec      (1000)      113 2023-07-27 17:46:57.000000 lowhass-0.1.0/lowhass/typings/__init__.py
--rw-r--r--   0 itec      (1000) itec      (1000)      754 2023-07-27 17:12:12.000000 lowhass-0.1.0/lowhass/typings/config.py
--rw-r--r--   0 itec      (1000) itec      (1000)      103 2023-07-27 17:18:49.000000 lowhass-0.1.0/lowhass/typings/events.py
--rw-r--r--   0 itec      (1000) itec      (1000)      527 2023-07-27 17:37:22.000000 lowhass-0.1.0/lowhass/typings/service.py
--rw-r--r--   0 itec      (1000) itec      (1000)      259 2023-07-27 17:48:19.000000 lowhass-0.1.0/lowhass/typings/state.py
--rw-r--r--   0 itec      (1000) itec      (1000)       73 2023-07-27 16:24:37.000000 lowhass-0.1.0/lowhass/typings/status.py
--rw-r--r--   0 itec      (1000) itec      (1000)      424 2023-07-27 16:28:45.000000 lowhass-0.1.0/lowhass/util.py
--rw-r--r--   0 itec      (1000) itec      (1000)     3972 2023-07-27 19:42:19.000000 lowhass-0.1.0/lowhass/ws_client.py
-drwxr-xr-x   0 itec      (1000) itec      (1000)        0 2023-07-27 19:56:07.204992 lowhass-0.1.0/lowhass.egg-info/
--rw-r--r--   0 itec      (1000) itec      (1000)      343 2023-07-27 19:56:07.000000 lowhass-0.1.0/lowhass.egg-info/PKG-INFO
--rw-r--r--   0 itec      (1000) itec      (1000)      452 2023-07-27 19:56:07.000000 lowhass-0.1.0/lowhass.egg-info/SOURCES.txt
--rw-r--r--   0 itec      (1000) itec      (1000)        1 2023-07-27 19:56:07.000000 lowhass-0.1.0/lowhass.egg-info/dependency_links.txt
--rw-r--r--   0 itec      (1000) itec      (1000)       29 2023-07-27 19:56:07.000000 lowhass-0.1.0/lowhass.egg-info/requires.txt
--rw-r--r--   0 itec      (1000) itec      (1000)        8 2023-07-27 19:56:07.000000 lowhass-0.1.0/lowhass.egg-info/top_level.txt
--rw-r--r--   0 itec      (1000) itec      (1000)      549 2023-07-27 19:55:41.000000 lowhass-0.1.0/pyproject.toml
--rw-r--r--   0 itec      (1000) itec      (1000)       28 2023-07-27 19:55:54.000000 lowhass-0.1.0/requirements.txt
--rw-r--r--   0 itec      (1000) itec      (1000)       38 2023-07-27 19:56:07.204992 lowhass-0.1.0/setup.cfg
+drwxr-xr-x   0 itec      (1000) itec      (1000)        0 2023-07-27 20:16:32.184784 lowhass-0.1.1/
+-rw-r--r--   0 itec      (1000) itec      (1000)     3078 2023-07-27 16:08:28.000000 lowhass-0.1.1/.gitignore
+-rw-r--r--   0 itec      (1000) itec      (1000)     1068 2023-07-27 16:08:28.000000 lowhass-0.1.1/LICENSE
+-rw-r--r--   0 itec      (1000) itec      (1000)      343 2023-07-27 20:16:32.184784 lowhass-0.1.1/PKG-INFO
+-rw-r--r--   0 itec      (1000) itec      (1000)       65 2023-07-27 19:55:35.000000 lowhass-0.1.1/README.md
+drwxr-xr-x   0 itec      (1000) itec      (1000)        0 2023-07-27 20:16:32.184784 lowhass-0.1.1/lowhass/
+-rw-r--r--   0 itec      (1000) itec      (1000)      316 2023-07-27 20:16:16.000000 lowhass-0.1.1/lowhass/__init__.py
+-rw-r--r--   0 itec      (1000) itec      (1000)     2007 2023-07-27 18:00:21.000000 lowhass-0.1.1/lowhass/rest_client.py
+drwxr-xr-x   0 itec      (1000) itec      (1000)        0 2023-07-27 20:16:32.184784 lowhass-0.1.1/lowhass/typings/
+-rw-r--r--   0 itec      (1000) itec      (1000)      113 2023-07-27 17:46:57.000000 lowhass-0.1.1/lowhass/typings/__init__.py
+-rw-r--r--   0 itec      (1000) itec      (1000)      754 2023-07-27 17:12:12.000000 lowhass-0.1.1/lowhass/typings/config.py
+-rw-r--r--   0 itec      (1000) itec      (1000)      103 2023-07-27 17:18:49.000000 lowhass-0.1.1/lowhass/typings/events.py
+-rw-r--r--   0 itec      (1000) itec      (1000)      527 2023-07-27 17:37:22.000000 lowhass-0.1.1/lowhass/typings/service.py
+-rw-r--r--   0 itec      (1000) itec      (1000)      259 2023-07-27 17:48:19.000000 lowhass-0.1.1/lowhass/typings/state.py
+-rw-r--r--   0 itec      (1000) itec      (1000)       73 2023-07-27 16:24:37.000000 lowhass-0.1.1/lowhass/typings/status.py
+-rw-r--r--   0 itec      (1000) itec      (1000)      424 2023-07-27 16:28:45.000000 lowhass-0.1.1/lowhass/util.py
+-rw-r--r--   0 itec      (1000) itec      (1000)     3972 2023-07-27 19:42:19.000000 lowhass-0.1.1/lowhass/ws_client.py
+drwxr-xr-x   0 itec      (1000) itec      (1000)        0 2023-07-27 20:16:32.184784 lowhass-0.1.1/lowhass.egg-info/
+-rw-r--r--   0 itec      (1000) itec      (1000)      343 2023-07-27 20:16:32.000000 lowhass-0.1.1/lowhass.egg-info/PKG-INFO
+-rw-r--r--   0 itec      (1000) itec      (1000)      452 2023-07-27 20:16:32.000000 lowhass-0.1.1/lowhass.egg-info/SOURCES.txt
+-rw-r--r--   0 itec      (1000) itec      (1000)        1 2023-07-27 20:16:32.000000 lowhass-0.1.1/lowhass.egg-info/dependency_links.txt
+-rw-r--r--   0 itec      (1000) itec      (1000)       29 2023-07-27 20:16:32.000000 lowhass-0.1.1/lowhass.egg-info/requires.txt
+-rw-r--r--   0 itec      (1000) itec      (1000)        8 2023-07-27 20:16:32.000000 lowhass-0.1.1/lowhass.egg-info/top_level.txt
+-rw-r--r--   0 itec      (1000) itec      (1000)      549 2023-07-27 19:55:41.000000 lowhass-0.1.1/pyproject.toml
+-rw-r--r--   0 itec      (1000) itec      (1000)       28 2023-07-27 19:55:54.000000 lowhass-0.1.1/requirements.txt
+-rw-r--r--   0 itec      (1000) itec      (1000)       38 2023-07-27 20:16:32.184784 lowhass-0.1.1/setup.cfg
```

### Comparing `lowhass-0.1.0/.gitignore` & `lowhass-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lowhass-0.1.0/LICENSE` & `lowhass-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lowhass-0.1.0/lowhass/rest_client.py` & `lowhass-0.1.1/lowhass/rest_client.py`

 * *Files identical despite different names*

### Comparing `lowhass-0.1.0/lowhass/typings/config.py` & `lowhass-0.1.1/lowhass/typings/config.py`

 * *Files identical despite different names*

### Comparing `lowhass-0.1.0/lowhass/typings/service.py` & `lowhass-0.1.1/lowhass/typings/service.py`

 * *Files identical despite different names*

### Comparing `lowhass-0.1.0/lowhass/ws_client.py` & `lowhass-0.1.1/lowhass/ws_client.py`

 * *Files identical despite different names*

### Comparing `lowhass-0.1.0/pyproject.toml` & `lowhass-0.1.1/pyproject.toml`

 * *Files identical despite different names*

