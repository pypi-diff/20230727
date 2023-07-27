# Comparing `tmp/pyhyypapihawkmod-1.1.7b1.tar.gz` & `tmp/pyhyypapihawkmod-1.1.7b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.7b1.tar", last modified: Thu Jul 27 14:24:31 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.7b3.tar", last modified: Thu Jul 27 19:51:18 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.7b1.tar` & `pyhyypapihawkmod-1.1.7b3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 14:24:31.162703 pyhyypapihawkmod-1.1.7b1/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b1/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b1/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-07-27 14:24:31.161700 pyhyypapihawkmod-1.1.7b1/PKG-INFO
--rw-rw-rw-   0        0        0     2169 2023-07-27 13:24:43.000000 pyhyypapihawkmod-1.1.7b1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 14:24:31.148793 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0    11035 2023-07-27 13:25:28.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    29480 2023-07-27 13:26:27.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4026 2023-07-27 13:23:03.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:24:31.159411 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-07-27 14:24:31.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-27 14:24:31.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 14:24:31.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-27 14:24:31.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-27 14:24:31.000000 pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 14:24:31.163199 pyhyypapihawkmod-1.1.7b1/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-27 14:22:54.000000 pyhyypapihawkmod-1.1.7b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:51:17.997477 pyhyypapihawkmod-1.1.7b3/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b3/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b3/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-27 19:51:17.996439 pyhyypapihawkmod-1.1.7b3/PKG-INFO
+-rw-rw-rw-   0        0        0     2265 2023-07-27 19:49:15.000000 pyhyypapihawkmod-1.1.7b3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 19:51:17.985295 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0    11035 2023-07-27 19:49:21.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    29480 2023-07-27 18:48:41.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4026 2023-07-27 14:27:12.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:51:17.994418 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-27 19:51:17.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-27 19:51:17.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 19:51:17.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-27 19:51:17.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-27 19:51:17.000000 pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 19:51:17.997477 pyhyypapihawkmod-1.1.7b3/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-27 19:48:15.000000 pyhyypapihawkmod-1.1.7b3/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.7b1/LICENSE.md` & `pyhyypapihawkmod-1.1.7b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.7b1/PKG-INFO` & `pyhyypapihawkmod-1.1.7b3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.7b1
+Version: 1.1.7b3
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.7b1/README.md` & `pyhyypapihawkmod-1.1.7b3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,20 @@
 ```
 print(json.dumps(client.get_sync_info(),indent=2))
 
 ```
 
 Changelog 
 
+1.1.7b3
+- Revert 1.1.7b2
+
+1.1.7b2
+- Removed one sleep delay for slightly better response
+
 1.1.7b1
 
 - Zones now show openviolated and tampered information from IDS server
 - Added delays between server requests to prevent blocking
 
 1.1.6-b3
 - Zones now show openviolated and tampered information from IDS server
```

### Comparing `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/alarm_info.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.7b1
+Version: 1.1.7b3
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.7b1/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.7b3/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.7b1/setup.py` & `pyhyypapihawkmod-1.1.7b3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.7b1",
+    version="1.1.7b3",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

