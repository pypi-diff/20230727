# Comparing `tmp/datarefiner_client-0.0.1.tar.gz` & `tmp/datarefiner_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarefiner_client-0.0.1.tar", max compression
+gzip compressed data, was "datarefiner_client-0.0.2.tar", max compression
```

## Comparing `datarefiner_client-0.0.1.tar` & `datarefiner_client-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      192 2023-07-19 15:02:22.128663 datarefiner_client-0.0.1/README.md
--rw-r--r--   0        0        0      112 2023-07-19 14:08:06.395364 datarefiner_client-0.0.1/datarefiner_client/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 11:21:29.796050 datarefiner_client-0.0.1/datarefiner_client/api/__init__.py
--rw-r--r--   0        0        0      808 2023-07-19 14:18:24.527446 datarefiner_client-0.0.1/datarefiner_client/api/entities.py
--rw-r--r--   0        0        0     3296 2023-07-21 14:18:21.973807 datarefiner_client-0.0.1/datarefiner_client/api/supervised_labels.py
--rw-r--r--   0        0        0     1543 2023-07-24 11:53:38.465589 datarefiner_client-0.0.1/datarefiner_client/api/uploads.py
--rw-r--r--   0        0        0     4403 2023-07-25 13:16:50.415403 datarefiner_client-0.0.1/datarefiner_client/client.py
--rw-r--r--   0        0        0     1277 2023-07-24 11:25:22.677009 datarefiner_client-0.0.1/datarefiner_client/dataframe_uploader.py
--rw-r--r--   0        0        0      387 2023-07-24 11:05:07.712720 datarefiner_client-0.0.1/datarefiner_client/exceptions.py
--rw-r--r--   0        0        0      287 2023-07-25 13:15:37.886662 datarefiner_client-0.0.1/datarefiner_client/settings.py
--rw-r--r--   0        0        0      840 2023-07-24 12:03:37.993082 datarefiner_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 datarefiner_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      907 2023-07-27 12:11:45.113217 datarefiner_client-0.0.2/README.md
+-rw-r--r--   0        0        0      112 2023-07-27 12:42:30.245165 datarefiner_client-0.0.2/datarefiner_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 11:21:29.796050 datarefiner_client-0.0.2/datarefiner_client/api/__init__.py
+-rw-r--r--   0        0        0      808 2023-07-19 14:18:24.527446 datarefiner_client-0.0.2/datarefiner_client/api/entities.py
+-rw-r--r--   0        0        0     3296 2023-07-21 14:18:21.973807 datarefiner_client-0.0.2/datarefiner_client/api/supervised_labels.py
+-rw-r--r--   0        0        0     1543 2023-07-24 11:53:38.465589 datarefiner_client-0.0.2/datarefiner_client/api/uploads.py
+-rw-r--r--   0        0        0     4403 2023-07-25 13:16:50.415403 datarefiner_client-0.0.2/datarefiner_client/client.py
+-rw-r--r--   0        0        0     1277 2023-07-24 11:25:22.677009 datarefiner_client-0.0.2/datarefiner_client/dataframe_uploader.py
+-rw-r--r--   0        0        0      387 2023-07-24 11:05:07.712720 datarefiner_client-0.0.2/datarefiner_client/exceptions.py
+-rw-r--r--   0        0        0      287 2023-07-25 13:15:37.886662 datarefiner_client-0.0.2/datarefiner_client/settings.py
+-rw-r--r--   0        0        0      981 2023-07-27 12:42:22.593016 datarefiner_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1535 1970-01-01 00:00:00.000000 datarefiner_client-0.0.2/PKG-INFO
```

### Comparing `datarefiner_client-0.0.1/datarefiner_client/api/entities.py` & `datarefiner_client-0.0.2/datarefiner_client/api/entities.py`

 * *Files identical despite different names*

### Comparing `datarefiner_client-0.0.1/datarefiner_client/api/supervised_labels.py` & `datarefiner_client-0.0.2/datarefiner_client/api/supervised_labels.py`

 * *Files identical despite different names*

### Comparing `datarefiner_client-0.0.1/datarefiner_client/api/uploads.py` & `datarefiner_client-0.0.2/datarefiner_client/api/uploads.py`

 * *Files identical despite different names*

### Comparing `datarefiner_client-0.0.1/datarefiner_client/client.py` & `datarefiner_client-0.0.2/datarefiner_client/client.py`

 * *Files identical despite different names*

### Comparing `datarefiner_client-0.0.1/datarefiner_client/dataframe_uploader.py` & `datarefiner_client-0.0.2/datarefiner_client/dataframe_uploader.py`

 * *Files identical despite different names*

### Comparing `datarefiner_client-0.0.1/pyproject.toml` & `datarefiner_client-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datarefiner-client"
-version = "0.0.1"
+version = "0.0.2"
 description = "API client for Datarefiner"
 authors = ["Datarefiner <admin@datarefiner.com>"]
 readme = "README.md"
 packages = [{include = "datarefiner_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -26,12 +26,18 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = ["."]
 addopts = ["-v", "-ra", "--cov=."]
 
 [tool.semantic_release]
-branch = "main"
-version_variable = "datarefiner_client/__init__.py:__version__"
+version_variable = [
+    "datarefiner_client/__init__.py:__version__",
+    "pyproject.toml:version"
+]
+branch = "master"
+upload_to_pypi = true
+upload_to_release = false
+build_command = "pip install poetry && poetry build"
 
 [tool.black]
 line-length = 120
```

