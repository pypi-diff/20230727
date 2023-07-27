# Comparing `tmp/mecord-cli-0.1.92.tar.gz` & `tmp/mecord-cli-0.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecord-cli-0.1.92.tar", last modified: Thu Jul 27 08:04:52 2023, max compression
+gzip compressed data, was "mecord-cli-0.1.93.tar", last modified: Thu Jul 27 08:07:19 2023, max compression
```

## Comparing `mecord-cli-0.1.92.tar` & `mecord-cli-0.1.93.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 08:04:52.460280 mecord-cli-0.1.92/
--rw-rw-rw-   0        0        0     1078 2023-04-19 06:54:05.000000 mecord-cli-0.1.92/LICENSE
--rw-rw-rw-   0        0        0     2364 2023-07-27 08:04:52.459785 mecord-cli-0.1.92/PKG-INFO
--rw-rw-rw-   0        0        0     1942 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 08:04:52.438508 mecord-cli-0.1.92/mecord/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/__init__.py
--rw-rw-rw-   0        0        0    57424 2023-07-03 02:47:14.000000 mecord-cli-0.1.92/mecord/aigc_ext_pb2.py
--rw-rw-rw-   0        0        0    10618 2023-07-27 06:26:10.000000 mecord-cli-0.1.92/mecord/capability_provider.py
--rw-rw-rw-   0        0        0    41642 2023-07-03 02:47:14.000000 mecord-cli-0.1.92/mecord/common_ext_pb2.py
--rw-rw-rw-   0        0        0      176 2023-07-27 08:04:52.000000 mecord-cli-0.1.92/mecord/constant.py
--rw-rw-rw-   0        0        0     1934 2023-07-03 02:47:14.000000 mecord-cli-0.1.92/mecord/main.py
--rw-rw-rw-   0        0        0    10604 2023-07-27 06:29:12.000000 mecord-cli-0.1.92/mecord/mecord_service.py
--rw-rw-rw-   0        0        0    11578 2023-07-27 06:26:10.000000 mecord-cli-0.1.92/mecord/mecord_widget.py
--rw-rw-rw-   0        0        0    10668 2023-07-27 08:04:20.000000 mecord-cli-0.1.92/mecord/progress_monitor.py
-drwxrwxrwx   0        0        0        0 2023-07-27 08:04:52.439996 mecord-cli-0.1.92/mecord/public_tools/
--rw-rw-rw-   0        0        0        0 2023-04-21 11:01:50.000000 mecord-cli-0.1.92/mecord/public_tools/__init__.py
--rw-rw-rw-   0        0        0      302 2023-04-20 10:06:00.000000 mecord-cli-0.1.92/mecord/public_tools/decorator_tools.py
--rw-rw-rw-   0        0        0     3321 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/rpcinput_pb2.py
-drwxrwxrwx   0        0        0        0 2023-07-27 08:04:52.442476 mecord-cli-0.1.92/mecord/script_template/
--rw-rw-rw-   0        0        0        0 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/script_template/__init__.py
--rw-rw-rw-   0        0        0      312 2023-04-21 11:40:09.000000 mecord-cli-0.1.92/mecord/script_template/launch.py
--rw-rw-rw-   0        0        0      915 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/script_template/main.py
--rw-rw-rw-   0        0        0      801 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/script_template/run.py
--rw-rw-rw-   0        0        0     6214 2023-07-27 06:26:10.000000 mecord-cli-0.1.92/mecord/store.py
--rw-rw-rw-   0        0        0     8912 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/uauth_common_pb2.py
--rw-rw-rw-   0        0        0   110273 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/uauth_ext_pb2.py
--rw-rw-rw-   0        0        0     2450 2023-07-27 06:26:10.000000 mecord-cli-0.1.92/mecord/upload.py
--rw-rw-rw-   0        0        0    13069 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/user_status_ext_pb2.py
--rw-rw-rw-   0        0        0    12538 2023-07-27 06:26:10.000000 mecord-cli-0.1.92/mecord/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 08:04:52.446444 mecord-cli-0.1.92/mecord/widget_template/
--rw-rw-rw-   0        0        0     1977 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/widget_template/MekongJS.js.py
--rw-rw-rw-   0        0        0        0 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/widget_template/__init__.py
--rw-rw-rw-   0        0        0      219 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/widget_template/config.json.py
--rw-rw-rw-   0        0        0     1678 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/widget_template/icon.png.py
--rw-rw-rw-   0        0        0      719 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/widget_template/index.html.py
--rw-rw-rw-   0        0        0     9981 2023-07-27 06:26:10.000000 mecord-cli-0.1.92/mecord/xy_pb.py
--rw-rw-rw-   0        0        0     2216 2023-04-19 07:17:07.000000 mecord-cli-0.1.92/mecord/xy_user.py
-drwxrwxrwx   0        0        0        0 2023-07-27 08:04:52.459286 mecord-cli-0.1.92/mecord_cli.egg-info/
--rw-rw-rw-   0        0        0     2364 2023-07-27 08:04:52.000000 mecord-cli-0.1.92/mecord_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1009 2023-07-27 08:04:52.000000 mecord-cli-0.1.92/mecord_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 08:04:52.000000 mecord-cli-0.1.92/mecord_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-27 08:04:52.000000 mecord-cli-0.1.92/mecord_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       78 2023-07-27 08:04:52.000000 mecord-cli-0.1.92/mecord_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-27 08:04:52.000000 mecord-cli-0.1.92/mecord_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 08:04:52.460280 mecord-cli-0.1.92/setup.cfg
--rw-rw-rw-   0        0        0     2525 2023-07-27 08:04:40.000000 mecord-cli-0.1.92/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:07:19.904183 mecord-cli-0.1.93/
+-rw-rw-rw-   0        0        0     1078 2023-04-19 06:54:05.000000 mecord-cli-0.1.93/LICENSE
+-rw-rw-rw-   0        0        0     2364 2023-07-27 08:07:19.903712 mecord-cli-0.1.93/PKG-INFO
+-rw-rw-rw-   0        0        0     1942 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 08:07:19.883847 mecord-cli-0.1.93/mecord/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/__init__.py
+-rw-rw-rw-   0        0        0    57424 2023-07-03 02:47:14.000000 mecord-cli-0.1.93/mecord/aigc_ext_pb2.py
+-rw-rw-rw-   0        0        0    10618 2023-07-27 06:26:10.000000 mecord-cli-0.1.93/mecord/capability_provider.py
+-rw-rw-rw-   0        0        0    41642 2023-07-03 02:47:14.000000 mecord-cli-0.1.93/mecord/common_ext_pb2.py
+-rw-rw-rw-   0        0        0      176 2023-07-27 08:07:19.000000 mecord-cli-0.1.93/mecord/constant.py
+-rw-rw-rw-   0        0        0     1934 2023-07-03 02:47:14.000000 mecord-cli-0.1.93/mecord/main.py
+-rw-rw-rw-   0        0        0    10606 2023-07-27 08:05:46.000000 mecord-cli-0.1.93/mecord/mecord_service.py
+-rw-rw-rw-   0        0        0    11578 2023-07-27 06:26:10.000000 mecord-cli-0.1.93/mecord/mecord_widget.py
+-rw-rw-rw-   0        0        0    10668 2023-07-27 08:04:20.000000 mecord-cli-0.1.93/mecord/progress_monitor.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:07:19.884839 mecord-cli-0.1.93/mecord/public_tools/
+-rw-rw-rw-   0        0        0        0 2023-04-21 11:01:50.000000 mecord-cli-0.1.93/mecord/public_tools/__init__.py
+-rw-rw-rw-   0        0        0      302 2023-04-20 10:06:00.000000 mecord-cli-0.1.93/mecord/public_tools/decorator_tools.py
+-rw-rw-rw-   0        0        0     3321 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/rpcinput_pb2.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:07:19.887319 mecord-cli-0.1.93/mecord/script_template/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/script_template/__init__.py
+-rw-rw-rw-   0        0        0      312 2023-04-21 11:40:09.000000 mecord-cli-0.1.93/mecord/script_template/launch.py
+-rw-rw-rw-   0        0        0      915 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/script_template/main.py
+-rw-rw-rw-   0        0        0      801 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/script_template/run.py
+-rw-rw-rw-   0        0        0     6214 2023-07-27 06:26:10.000000 mecord-cli-0.1.93/mecord/store.py
+-rw-rw-rw-   0        0        0     8912 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/uauth_common_pb2.py
+-rw-rw-rw-   0        0        0   110273 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/uauth_ext_pb2.py
+-rw-rw-rw-   0        0        0     2450 2023-07-27 06:26:10.000000 mecord-cli-0.1.93/mecord/upload.py
+-rw-rw-rw-   0        0        0    13069 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/user_status_ext_pb2.py
+-rw-rw-rw-   0        0        0    12538 2023-07-27 06:26:10.000000 mecord-cli-0.1.93/mecord/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:07:19.890295 mecord-cli-0.1.93/mecord/widget_template/
+-rw-rw-rw-   0        0        0     1977 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/widget_template/MekongJS.js.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/widget_template/__init__.py
+-rw-rw-rw-   0        0        0      219 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/widget_template/config.json.py
+-rw-rw-rw-   0        0        0     1678 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/widget_template/icon.png.py
+-rw-rw-rw-   0        0        0      719 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/widget_template/index.html.py
+-rw-rw-rw-   0        0        0     9981 2023-07-27 06:26:10.000000 mecord-cli-0.1.93/mecord/xy_pb.py
+-rw-rw-rw-   0        0        0     2216 2023-04-19 07:17:07.000000 mecord-cli-0.1.93/mecord/xy_user.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:07:19.902723 mecord-cli-0.1.93/mecord_cli.egg-info/
+-rw-rw-rw-   0        0        0     2364 2023-07-27 08:07:19.000000 mecord-cli-0.1.93/mecord_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1009 2023-07-27 08:07:19.000000 mecord-cli-0.1.93/mecord_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 08:07:19.000000 mecord-cli-0.1.93/mecord_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-27 08:07:19.000000 mecord-cli-0.1.93/mecord_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2023-07-27 08:07:19.000000 mecord-cli-0.1.93/mecord_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-27 08:07:19.000000 mecord-cli-0.1.93/mecord_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 08:07:19.904183 mecord-cli-0.1.93/setup.cfg
+-rw-rw-rw-   0        0        0     2525 2023-07-27 08:05:53.000000 mecord-cli-0.1.93/setup.py
```

### Comparing `mecord-cli-0.1.92/LICENSE` & `mecord-cli-0.1.93/LICENSE`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/PKG-INFO` & `mecord-cli-0.1.93/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecord-cli
-Version: 0.1.92
+Version: 0.1.93
 Summary: mecord tools
 Home-page: https://github.com/mecordofficial
 Author: pengjun
 Author-email: mr_lonely@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mecord-cli-0.1.92/README.md` & `mecord-cli-0.1.93/README.md`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/aigc_ext_pb2.py` & `mecord-cli-0.1.93/mecord/aigc_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/capability_provider.py` & `mecord-cli-0.1.93/mecord/capability_provider.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/common_ext_pb2.py` & `mecord-cli-0.1.93/mecord/common_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/main.py` & `mecord-cli-0.1.93/mecord/main.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/mecord_service.py` & `mecord-cli-0.1.93/mecord/mecord_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pathlib import Path
 from urllib.parse import *
 
 from mecord import store
 from mecord import xy_pb
 from mecord import xy_user 
 from mecord import utils
-from mecord import progress_monitor
+# from mecord import progress_monitor
 
 def process_is_alive(pid: int) -> bool:
     try:
         process = psutil.Process(pid)
         pstatus = process.status()
         if pstatus == psutil.STATUS_RUNNING or pstatus == psutil.STATUS_SLEEPING:
             return True
```

### Comparing `mecord-cli-0.1.92/mecord/mecord_widget.py` & `mecord-cli-0.1.93/mecord/mecord_widget.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/progress_monitor.py` & `mecord-cli-0.1.93/mecord/progress_monitor.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/rpcinput_pb2.py` & `mecord-cli-0.1.93/mecord/rpcinput_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/script_template/main.py` & `mecord-cli-0.1.93/mecord/script_template/main.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/script_template/run.py` & `mecord-cli-0.1.93/mecord/script_template/run.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/store.py` & `mecord-cli-0.1.93/mecord/store.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/uauth_common_pb2.py` & `mecord-cli-0.1.93/mecord/uauth_common_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/uauth_ext_pb2.py` & `mecord-cli-0.1.93/mecord/uauth_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/upload.py` & `mecord-cli-0.1.93/mecord/upload.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/user_status_ext_pb2.py` & `mecord-cli-0.1.93/mecord/user_status_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/utils.py` & `mecord-cli-0.1.93/mecord/utils.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/widget_template/MekongJS.js.py` & `mecord-cli-0.1.93/mecord/widget_template/MekongJS.js.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/widget_template/icon.png.py` & `mecord-cli-0.1.93/mecord/widget_template/icon.png.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/widget_template/index.html.py` & `mecord-cli-0.1.93/mecord/widget_template/index.html.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/xy_pb.py` & `mecord-cli-0.1.93/mecord/xy_pb.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord/xy_user.py` & `mecord-cli-0.1.93/mecord/xy_user.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/mecord_cli.egg-info/PKG-INFO` & `mecord-cli-0.1.93/mecord_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecord-cli
-Version: 0.1.92
+Version: 0.1.93
 Summary: mecord tools
 Home-page: https://github.com/mecordofficial
 Author: pengjun
 Author-email: mr_lonely@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mecord-cli-0.1.92/mecord_cli.egg-info/SOURCES.txt` & `mecord-cli-0.1.93/mecord_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.92/setup.py` & `mecord-cli-0.1.93/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 import subprocess
 import datetime
 
-mecord_version = "0.1.92"
+mecord_version = "0.1.93"
 
 mecord_build_number = int(mecord_version.replace(".",""))
 cur_dir = os.path.dirname(os.path.abspath(__file__))
 constanspy = os.path.join(cur_dir, "mecord", "constant.py")
 try:
     result = subprocess.run("git config user.email", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
     build_user = "Noh"
```

