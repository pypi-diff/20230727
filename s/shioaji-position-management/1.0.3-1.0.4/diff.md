# Comparing `tmp/shioaji_position_management-1.0.3.tar.gz` & `tmp/shioaji_position_management-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shioaji_position_management-1.0.3.tar", last modified: Mon Jul 24 05:58:17 2023, max compression
+gzip compressed data, was "shioaji_position_management-1.0.4.tar", last modified: Thu Jul 27 14:41:16 2023, max compression
```

## Comparing `shioaji_position_management-1.0.3.tar` & `shioaji_position_management-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-24 05:58:17.733801 shioaji_position_management-1.0.3/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     1067 2023-07-24 05:41:32.000000 shioaji_position_management-1.0.3/LICENSE
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2636 2023-07-24 05:58:17.733801 shioaji_position_management-1.0.3/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2028 2023-07-24 05:58:10.000000 shioaji_position_management-1.0.3/README.md
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-07-24 05:41:50.000000 shioaji_position_management-1.0.3/pyproject.toml
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      771 2023-07-24 05:58:17.733801 shioaji_position_management-1.0.3/setup.cfg
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-24 05:58:17.729801 shioaji_position_management-1.0.3/src/
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-24 05:58:17.733801 shioaji_position_management-1.0.3/src/shioaji_position_management/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       95 2023-07-24 05:41:49.000000 shioaji_position_management-1.0.3/src/shioaji_position_management/__init__.py
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     3112 2023-07-24 05:56:37.000000 shioaji_position_management-1.0.3/src/shioaji_position_management/shioaji_position_management.py
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-24 05:58:17.733801 shioaji_position_management-1.0.3/src/shioaji_position_management.egg-info/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2636 2023-07-24 05:58:17.000000 shioaji_position_management-1.0.3/src/shioaji_position_management.egg-info/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      423 2023-07-24 05:58:17.000000 shioaji_position_management-1.0.3/src/shioaji_position_management.egg-info/SOURCES.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-24 05:58:17.000000 shioaji_position_management-1.0.3/src/shioaji_position_management.egg-info/dependency_links.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       15 2023-07-24 05:58:17.000000 shioaji_position_management-1.0.3/src/shioaji_position_management.egg-info/requires.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       28 2023-07-24 05:58:17.000000 shioaji_position_management-1.0.3/src/shioaji_position_management.egg-info/top_level.txt
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:41:16.959315 shioaji_position_management-1.0.4/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     1067 2023-07-24 05:41:32.000000 shioaji_position_management-1.0.4/LICENSE
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2683 2023-07-27 14:41:16.959315 shioaji_position_management-1.0.4/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2075 2023-07-27 14:40:37.000000 shioaji_position_management-1.0.4/README.md
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-07-24 05:41:50.000000 shioaji_position_management-1.0.4/pyproject.toml
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      771 2023-07-27 14:41:16.963315 shioaji_position_management-1.0.4/setup.cfg
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:41:16.943315 shioaji_position_management-1.0.4/src/
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:41:16.951315 shioaji_position_management-1.0.4/src/shioaji_position_management/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       95 2023-07-24 05:41:49.000000 shioaji_position_management-1.0.4/src/shioaji_position_management/__init__.py
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     3133 2023-07-27 14:40:55.000000 shioaji_position_management-1.0.4/src/shioaji_position_management/shioaji_position_management.py
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-07-27 14:41:16.959315 shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     2683 2023-07-27 14:41:16.000000 shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      423 2023-07-27 14:41:16.000000 shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-07-27 14:41:16.000000 shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       15 2023-07-27 14:41:16.000000 shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/requires.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       28 2023-07-27 14:41:16.000000 shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/top_level.txt
```

### Comparing `shioaji_position_management-1.0.3/LICENSE` & `shioaji_position_management-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shioaji_position_management-1.0.3/PKG-INFO` & `shioaji_position_management-1.0.4/src/shioaji_position_management.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shioaji_position_management
-Version: 1.0.3
+Name: shioaji-position-management
+Version: 1.0.4
 Summary: An Extensions help you trading with Sinopac shioaji
 Home-page: https://github.com/NickLin910221/shioaji_position_management
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Position_Management/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -58,14 +58,15 @@
 ```sh
 pip install shioaji_position_management
 ```
 
 ## Usage
 
 ## Version
+- v1.0.4 (2023/7/27) fix some bugs about order
 - v1.0.3 (2023/7/24) Release & fix some bugs
 - v1.0.2
 - v1.0.1
 - v1.0.0
 
 ## Roadmap
```

### Comparing `shioaji_position_management-1.0.3/README.md` & `shioaji_position_management-1.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 ```sh
 pip install shioaji_position_management
 ```
 
 ## Usage
 
 ## Version
+- v1.0.4 (2023/7/27) fix some bugs about order
 - v1.0.3 (2023/7/24) Release & fix some bugs
 - v1.0.2
 - v1.0.1
 - v1.0.0
 
 ## Roadmap
```

### Comparing `shioaji_position_management-1.0.3/setup.cfg` & `shioaji_position_management-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shioaji_position_management
-version = 1.0.3
+version = 1.0.4
 author = NickLin910221
 author_email = nicklin910221@gmail.com
 description = An Extensions help you trading with Sinopac shioaji
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = shioaji
 url = https://github.com/NickLin910221/shioaji_position_management
```

### Comparing `shioaji_position_management-1.0.3/src/shioaji_position_management/shioaji_position_management.py` & `shioaji_position_management-1.0.4/src/shioaji_position_management/shioaji_position_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from loguru import logger
 import datetime
+import shioaji as sj
 
 class shioaji_position_management:
     __slots__ = ["api", "stock", "future", "option", "ordering", "acc", "logger"]
 
     def __init__(self, api, acc):
         self.api = api
         assert len(api.list_accounts()) > 0
```

### Comparing `shioaji_position_management-1.0.3/src/shioaji_position_management.egg-info/PKG-INFO` & `shioaji_position_management-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shioaji-position-management
-Version: 1.0.3
+Name: shioaji_position_management
+Version: 1.0.4
 Summary: An Extensions help you trading with Sinopac shioaji
 Home-page: https://github.com/NickLin910221/shioaji_position_management
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Position_Management/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -58,14 +58,15 @@
 ```sh
 pip install shioaji_position_management
 ```
 
 ## Usage
 
 ## Version
+- v1.0.4 (2023/7/27) fix some bugs about order
 - v1.0.3 (2023/7/24) Release & fix some bugs
 - v1.0.2
 - v1.0.1
 - v1.0.0
 
 ## Roadmap
```

