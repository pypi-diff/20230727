# Comparing `tmp/cq23-2.4.1.tar.gz` & `tmp/cq23-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-2.4.1.tar", last modified: Sat Jul 22 16:05:20 2023, max compression
+gzip compressed data, was "cq23-2.5.0.tar", last modified: Thu Jul 27 14:16:04 2023, max compression
```

## Comparing `cq23-2.4.1.tar` & `cq23-2.5.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-22 16:05:20.246125 cq23-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-22 16:05:10.000000 cq23-2.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-22 16:05:10.000000 cq23-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-22 16:05:20.246125 cq23-2.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.242124 cq23-2.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.242124 cq23-2.4.1/src/cq23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/src/cq23/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/src/cq23/build_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/build_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/build_image/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/build_image/docker_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/src/cq23/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/src/cq23/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/src/cq23/client_logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/client_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/client_logs/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/src/cq23/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/src/cq23/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/src/cq23/replay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/replay/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/src/cq23/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/src/cq23/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/web_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/src/cq23/web_server/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/web_server/files/loading_screen.html
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/web_server/flask_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.246125 cq23-2.4.1/src/cq23/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-22 16:05:10.000000 cq23-2.4.1/src/cq23/zip/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 16:05:20.242124 cq23-2.4.1/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-22 16:05:20.000000 cq23-2.4.1/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-22 16:05:20.000000 cq23-2.4.1/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 16:05:20.000000 cq23-2.4.1/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-22 16:05:20.000000 cq23-2.4.1/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-22 16:05:20.000000 cq23-2.4.1/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-22 16:05:20.000000 cq23-2.4.1/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-27 14:16:04.235471 cq23-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-27 14:15:56.000000 cq23-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 14:15:56.000000 cq23-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-27 14:16:04.235471 cq23-2.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.231471 cq23-2.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.231471 cq23-2.5.0/src/cq23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.231471 cq23-2.5.0/src/cq23/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.231471 cq23-2.5.0/src/cq23/build_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/build_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/build_image/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/build_image/docker_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/client_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/client_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/client_logs/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/replay/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/web_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/web_server/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/web_server/files/loading_screen.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.235471 cq23-2.5.0/src/cq23/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-27 14:15:56.000000 cq23-2.5.0/src/cq23/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:16:04.231471 cq23-2.5.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-27 14:16:04.000000 cq23-2.5.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-27 14:16:04.000000 cq23-2.5.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:16:04.000000 cq23-2.5.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-27 14:16:04.000000 cq23-2.5.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-27 14:16:04.000000 cq23-2.5.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-27 14:16:04.000000 cq23-2.5.0/src/cq23.egg-info/top_level.txt
```

### Comparing `cq23-2.4.1/PKG-INFO` & `cq23-2.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 2.4.1
+Version: 2.5.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-2.4.1/setup.cfg` & `cq23-2.5.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 2.4.1
+version = 2.5.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-2.4.1/src/cq23/admin/aws.py` & `cq23-2.5.0/src/cq23/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/admin/builder.py` & `cq23-2.5.0/src/cq23/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/admin/worker.py` & `cq23-2.5.0/src/cq23/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/build_image/command.py` & `cq23-2.5.0/src/cq23/build_image/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/build_image/docker_tools.py` & `cq23-2.5.0/src/cq23/build_image/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/check/command.py` & `cq23-2.5.0/src/cq23/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/cleanup/command.py` & `cq23-2.5.0/src/cq23/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/client_logs/command.py` & `cq23-2.5.0/src/cq23/client_logs/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/main/command.py` & `cq23-2.5.0/src/cq23/main/command.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 
 from .utils import restore_cwd
 
 
 def help_message():
     message = (
         "Available commands:\n\n"
+        + "> cq23 help\n"
         + "> cq23 new <language> <bot name>\n"
         + "> cq23 build <name>\n"
         + "> cq23 run\n"
         + "> cq23 run map=<map name>\n"
         + "> cq23 run home=<home bot name> away=<away bot name>\n"
         + "> cq23 replay\n"
         + "> cq23 zip\n"
         + "> cq23 check\n"
         + "> cq23 logs <client name>\n"
         + "> cq23 cleanup\n\n"
         + "If you need help with the competition, post a message in Discord or email us at info@codequest.club."
+        + " \t\t\t PXU8V6"
     )
     print(message)
 
 
 @restore_cwd
 def route_command():
     command_args = sys.argv[1:]
```

### Comparing `cq23-2.4.1/src/cq23/main/utils.py` & `cq23-2.5.0/src/cq23/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/new_client/command.py` & `cq23-2.5.0/src/cq23/new_client/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/replay/command.py` & `cq23-2.5.0/src/cq23/replay/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/run_game/command.py` & `cq23-2.5.0/src/cq23/run_game/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
     if not os.path.exists(game_files_dir):
         os.makedirs(game_files_dir)
     os.chdir(game_files_dir)
     game_files_abs_path = os.getcwd()
 
     clone_or_pull_repository(gcs_repo, gcs_folder_name)
+    print("KH73TU")
     docker_tools.pull_latest_game_server()
     run_gcs(
         gcs_folder_name,
         home_image,
         away_image,
         extract_arg_from_command_args("map", args),
     )
```

### Comparing `cq23-2.4.1/src/cq23/run_game/docker_tools.py` & `cq23-2.5.0/src/cq23/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/run_game/gcs.py` & `cq23-2.5.0/src/cq23/run_game/gcs.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/web_server/files/loading_screen.html` & `cq23-2.5.0/src/cq23/web_server/files/loading_screen.html`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/web_server/flask_api.py` & `cq23-2.5.0/src/cq23/web_server/flask_api.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23/zip/command.py` & `cq23-2.5.0/src/cq23/zip/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.4.1/src/cq23.egg-info/PKG-INFO` & `cq23-2.5.0/src/cq23.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 2.4.1
+Version: 2.5.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-2.4.1/src/cq23.egg-info/SOURCES.txt` & `cq23-2.5.0/src/cq23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

