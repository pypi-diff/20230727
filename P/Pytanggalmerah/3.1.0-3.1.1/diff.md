# Comparing `tmp/Pytanggalmerah-3.1.0.tar.gz` & `tmp/Pytanggalmerah-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pytanggalmerah-3.1.0.tar", last modified: Thu Jul 27 16:27:28 2023, max compression
+gzip compressed data, was "Pytanggalmerah-3.1.1.tar", last modified: Thu Jul 27 17:27:02 2023, max compression
```

## Comparing `Pytanggalmerah-3.1.0.tar` & `Pytanggalmerah-3.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:27:28.707803 Pytanggalmerah-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-27 16:27:03.000000 Pytanggalmerah-3.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-27 16:27:28.707803 Pytanggalmerah-3.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:27:28.707803 Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-27 16:27:28.000000 Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-27 16:27:28.000000 Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:27:28.000000 Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 16:27:28.000000 Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 16:27:28.000000 Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-27 16:27:03.000000 Pytanggalmerah-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-27 16:27:03.000000 Pytanggalmerah-3.1.0/harilibur
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:27:28.707803 Pytanggalmerah-3.1.0/pytanggalmerah/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-27 16:27:19.000000 Pytanggalmerah-3.1.0/pytanggalmerah/TanggalMerah.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-27 16:27:03.000000 Pytanggalmerah-3.1.0/pytanggalmerah/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-27 16:27:03.000000 Pytanggalmerah-3.1.0/pytanggalmerah/myrequests.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 16:27:28.711803 Pytanggalmerah-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-27 16:27:19.000000 Pytanggalmerah-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:27:02.842887 Pytanggalmerah-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-27 17:26:43.000000 Pytanggalmerah-3.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-27 17:27:02.842887 Pytanggalmerah-3.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:27:02.842887 Pytanggalmerah-3.1.1/Pytanggalmerah.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-27 17:27:02.000000 Pytanggalmerah-3.1.1/Pytanggalmerah.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-27 17:27:02.000000 Pytanggalmerah-3.1.1/Pytanggalmerah.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:27:02.000000 Pytanggalmerah-3.1.1/Pytanggalmerah.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 17:27:02.000000 Pytanggalmerah-3.1.1/Pytanggalmerah.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 17:27:02.000000 Pytanggalmerah-3.1.1/Pytanggalmerah.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-27 17:26:43.000000 Pytanggalmerah-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-27 17:26:43.000000 Pytanggalmerah-3.1.1/harilibur
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:27:02.842887 Pytanggalmerah-3.1.1/pytanggalmerah/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-27 17:26:55.000000 Pytanggalmerah-3.1.1/pytanggalmerah/TanggalMerah.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-27 17:26:43.000000 Pytanggalmerah-3.1.1/pytanggalmerah/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-27 17:26:43.000000 Pytanggalmerah-3.1.1/pytanggalmerah/myrequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:27:02.842887 Pytanggalmerah-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-27 17:26:55.000000 Pytanggalmerah-3.1.1/setup.py
```

### Comparing `Pytanggalmerah-3.1.0/LICENSE.txt` & `Pytanggalmerah-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Pytanggalmerah-3.1.0/PKG-INFO` & `Pytanggalmerah-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytanggalmerah
-Version: 3.1.0
+Version: 3.1.1
 Summary: python module to check indonesia holiday calendar (include sunday)
 Home-page: https://github.com/guangrei/pytanggalmerah
 Author: guangrei
 Author-email: myawn@pm.me
 License: MIT
 Keywords: holiday indonesia calendar sunday
 Description-Content-Type: text/markdown
```

### Comparing `Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/PKG-INFO` & `Pytanggalmerah-3.1.1/Pytanggalmerah.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pytanggalmerah
-Version: 3.1.0
+Version: 3.1.1
 Summary: python module to check indonesia holiday calendar (include sunday)
 Home-page: https://github.com/guangrei/pytanggalmerah
 Author: guangrei
 Author-email: myawn@pm.me
 License: MIT
 Keywords: holiday indonesia calendar sunday
 Description-Content-Type: text/markdown
```

### Comparing `Pytanggalmerah-3.1.0/README.md` & `Pytanggalmerah-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Pytanggalmerah-3.1.0/pytanggalmerah/TanggalMerah.py` & `Pytanggalmerah-3.1.1/pytanggalmerah/TanggalMerah.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 from pytz import timezone
 from .myrequests import MyRequests
 import json
 import os
 
 
-in_cache_path = os.path.abspath(os.path.dirname(__file__)) + "/cache/"
+in_cache_path = os.path.abspath(os.path.dirname(__file__))
 
 
 class TanggalMerah:
     def __init__(self, cache_path=None, cache_time=600):
         self.event = set([])
         self.date = datetime.now(timezone("Asia/Jakarta"))
         req = MyRequests("https://raw.githubusercontent.com/guangrei/APIHariLibur_V2/main/holidays.json",
```

### Comparing `Pytanggalmerah-3.1.0/pytanggalmerah/myrequests.py` & `Pytanggalmerah-3.1.1/pytanggalmerah/myrequests.py`

 * *Files identical despite different names*

### Comparing `Pytanggalmerah-3.1.0/setup.py` & `Pytanggalmerah-3.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='Pytanggalmerah',
-    version='3.1.0',
+    version='3.1.1',
     packages=['pytanggalmerah'],
     scripts=["harilibur"],
     license='MIT',
     author="guangrei",
     author_email="myawn@pm.me",
     description="python module to check indonesia holiday calendar (include sunday)",
     long_description=long_description,
```

