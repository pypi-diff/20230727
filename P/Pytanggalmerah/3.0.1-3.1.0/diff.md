# Comparing `tmp/Pytanggalmerah-3.0.1.tar.gz` & `tmp/Pytanggalmerah-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pytanggalmerah-3.0.1.tar", last modified: Tue May 30 16:54:04 2023, max compression
+gzip compressed data, was "Pytanggalmerah-3.1.0.tar", last modified: Thu Jul 27 16:27:28 2023, max compression
```

## Comparing `Pytanggalmerah-3.0.1.tar` & `Pytanggalmerah-3.1.0.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:54:04.011742 Pytanggalmerah-3.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-05-30 16:53:53.000000 Pytanggalmerah-3.0.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1837 2023-05-30 16:54:04.011742 Pytanggalmerah-3.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:54:04.010742 Pytanggalmerah-3.0.1/Pytanggalmerah.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1837 2023-05-30 16:54:03.000000 Pytanggalmerah-3.0.1/Pytanggalmerah.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-30 16:54:03.000000 Pytanggalmerah-3.0.1/Pytanggalmerah.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 16:54:03.000000 Pytanggalmerah-3.0.1/Pytanggalmerah.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-30 16:54:03.000000 Pytanggalmerah-3.0.1/Pytanggalmerah.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-30 16:54:03.000000 Pytanggalmerah-3.0.1/Pytanggalmerah.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1481 2023-05-30 16:53:53.000000 Pytanggalmerah-3.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-05-30 16:53:53.000000 Pytanggalmerah-3.0.1/harilibur
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:54:04.011742 Pytanggalmerah-3.0.1/pytanggalmerah/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-05-30 16:54:03.000000 Pytanggalmerah-3.0.1/pytanggalmerah/TanggalMerah.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-05-30 16:54:03.000000 Pytanggalmerah-3.0.1/pytanggalmerah/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-05-30 16:54:03.000000 Pytanggalmerah-3.0.1/pytanggalmerah/myrequests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 16:54:04.011742 Pytanggalmerah-3.0.1/pytanggalmerahcache/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 16:53:53.000000 Pytanggalmerah-3.0.1/pytanggalmerahcache/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 16:54:04.011742 Pytanggalmerah-3.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-05-30 16:54:03.000000 Pytanggalmerah-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:27:28.707803 Pytanggalmerah-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-27 16:27:03.000000 Pytanggalmerah-3.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-27 16:27:28.707803 Pytanggalmerah-3.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:27:28.707803 Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-27 16:27:28.000000 Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-27 16:27:28.000000 Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:27:28.000000 Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 16:27:28.000000 Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 16:27:28.000000 Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-27 16:27:03.000000 Pytanggalmerah-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-27 16:27:03.000000 Pytanggalmerah-3.1.0/harilibur
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:27:28.707803 Pytanggalmerah-3.1.0/pytanggalmerah/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-27 16:27:19.000000 Pytanggalmerah-3.1.0/pytanggalmerah/TanggalMerah.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-27 16:27:03.000000 Pytanggalmerah-3.1.0/pytanggalmerah/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-27 16:27:03.000000 Pytanggalmerah-3.1.0/pytanggalmerah/myrequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 16:27:28.711803 Pytanggalmerah-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-27 16:27:19.000000 Pytanggalmerah-3.1.0/setup.py
```

### Comparing `Pytanggalmerah-3.0.1/LICENSE.txt` & `Pytanggalmerah-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Pytanggalmerah-3.0.1/PKG-INFO` & `Pytanggalmerah-3.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: Pytanggalmerah
-Version: 3.0.1
+Version: 3.1.0
 Summary: python module to check indonesia holiday calendar (include sunday)
 Home-page: https://github.com/guangrei/pytanggalmerah
 Author: guangrei
 Author-email: myawn@pm.me
 License: MIT
 Keywords: holiday indonesia calendar sunday
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-[![Build Status](https://travis-ci.org/guangrei/pytanggalmerah.svg?branch=master)](https://travis-ci.org/guangrei/pytanggalmerah)
+[![status workflow test](https://github.com/guangrei/pytanggalmerah/actions/workflows/python-app.yml/badge.svg)](https://github.com/guangrei/pytanggalmerah/actions) [![status workflow build](https://github.com/guangrei/pytanggalmerah/actions/workflows/release_to_pypi.yml/badge.svg)](https://github.com/guangrei/pytanggalmerah/actions)
+
+
+[![Downloads](https://static.pepy.tech/badge/pytanggalmerah)](https://pepy.tech/project/pytanggalmerah) [![Downloads](https://static.pepy.tech/badge/pytanggalmerah/month)](https://pepy.tech/project/pytanggalmerah) [![Downloads](https://static.pepy.tech/badge/pytanggalmerah/week)](https://pepy.tech/project/pytanggalmerah)
 
 **Pytanggalmerah** adalah module python untuk mengecek tanggal merah berdasarkan hari minggu dan hari libur nasional.
 
 ### installasi
 
 ```
 pip install pytanggalmerah
@@ -31,15 +34,15 @@
 t.is_sunday() # mengecek apakah hari minggu, return booelan.
 t.get_event() # mendapatkan event, return list.
 
 ```
  **mengecek specific tanggal tertentu** 
 
 ``` python
-t.set_date(2019, 02, 05)
+t.set_date("2019", "02", "05")
 t.check()
 ```
  **mengatur zona waktu** 
 
 secara default zona waktu pytanggalmerah adalah Asia/Jakarta tapi bisa diubah, seperti
 
 ``` python
@@ -47,15 +50,15 @@
 t.check()
 ```
  **menggunakan lewat terminal**
 
 
 ```
 $ harilibur # check harilibur
-$ harilibur 2023 04 15 # check harilibur dengan spesifikasi
+$ harilibur 2022 04 15 # check harilibur dengan spesifikasi
 $ TIMEZSET = "Asia/Makasar" harilibur # mengecek harilibur dengan spesifikasi timezone
 
 ```
 
 > harilibur command hanya mengecek tanggal merah dan tidak termasuk hari minggu.
 ### sumber data
```

### Comparing `Pytanggalmerah-3.0.1/Pytanggalmerah.egg-info/PKG-INFO` & `Pytanggalmerah-3.1.0/Pytanggalmerah.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: Pytanggalmerah
-Version: 3.0.1
+Version: 3.1.0
 Summary: python module to check indonesia holiday calendar (include sunday)
 Home-page: https://github.com/guangrei/pytanggalmerah
 Author: guangrei
 Author-email: myawn@pm.me
 License: MIT
 Keywords: holiday indonesia calendar sunday
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-[![Build Status](https://travis-ci.org/guangrei/pytanggalmerah.svg?branch=master)](https://travis-ci.org/guangrei/pytanggalmerah)
+[![status workflow test](https://github.com/guangrei/pytanggalmerah/actions/workflows/python-app.yml/badge.svg)](https://github.com/guangrei/pytanggalmerah/actions) [![status workflow build](https://github.com/guangrei/pytanggalmerah/actions/workflows/release_to_pypi.yml/badge.svg)](https://github.com/guangrei/pytanggalmerah/actions)
+
+
+[![Downloads](https://static.pepy.tech/badge/pytanggalmerah)](https://pepy.tech/project/pytanggalmerah) [![Downloads](https://static.pepy.tech/badge/pytanggalmerah/month)](https://pepy.tech/project/pytanggalmerah) [![Downloads](https://static.pepy.tech/badge/pytanggalmerah/week)](https://pepy.tech/project/pytanggalmerah)
 
 **Pytanggalmerah** adalah module python untuk mengecek tanggal merah berdasarkan hari minggu dan hari libur nasional.
 
 ### installasi
 
 ```
 pip install pytanggalmerah
@@ -31,15 +34,15 @@
 t.is_sunday() # mengecek apakah hari minggu, return booelan.
 t.get_event() # mendapatkan event, return list.
 
 ```
  **mengecek specific tanggal tertentu** 
 
 ``` python
-t.set_date(2019, 02, 05)
+t.set_date("2019", "02", "05")
 t.check()
 ```
  **mengatur zona waktu** 
 
 secara default zona waktu pytanggalmerah adalah Asia/Jakarta tapi bisa diubah, seperti
 
 ``` python
@@ -47,15 +50,15 @@
 t.check()
 ```
  **menggunakan lewat terminal**
 
 
 ```
 $ harilibur # check harilibur
-$ harilibur 2023 04 15 # check harilibur dengan spesifikasi
+$ harilibur 2022 04 15 # check harilibur dengan spesifikasi
 $ TIMEZSET = "Asia/Makasar" harilibur # mengecek harilibur dengan spesifikasi timezone
 
 ```
 
 > harilibur command hanya mengecek tanggal merah dan tidak termasuk hari minggu.
 ### sumber data
```

### Comparing `Pytanggalmerah-3.0.1/README.md` & `Pytanggalmerah-3.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-[![Build Status](https://travis-ci.org/guangrei/pytanggalmerah.svg?branch=master)](https://travis-ci.org/guangrei/pytanggalmerah)
+[![status workflow test](https://github.com/guangrei/pytanggalmerah/actions/workflows/python-app.yml/badge.svg)](https://github.com/guangrei/pytanggalmerah/actions) [![status workflow build](https://github.com/guangrei/pytanggalmerah/actions/workflows/release_to_pypi.yml/badge.svg)](https://github.com/guangrei/pytanggalmerah/actions)
+
+
+[![Downloads](https://static.pepy.tech/badge/pytanggalmerah)](https://pepy.tech/project/pytanggalmerah) [![Downloads](https://static.pepy.tech/badge/pytanggalmerah/month)](https://pepy.tech/project/pytanggalmerah) [![Downloads](https://static.pepy.tech/badge/pytanggalmerah/week)](https://pepy.tech/project/pytanggalmerah)
 
 **Pytanggalmerah** adalah module python untuk mengecek tanggal merah berdasarkan hari minggu dan hari libur nasional.
 
 ### installasi
 
 ```
 pip install pytanggalmerah
@@ -19,15 +22,15 @@
 t.is_sunday() # mengecek apakah hari minggu, return booelan.
 t.get_event() # mendapatkan event, return list.
 
 ```
  **mengecek specific tanggal tertentu** 
 
 ``` python
-t.set_date(2019, 02, 05)
+t.set_date("2019", "02", "05")
 t.check()
 ```
  **mengatur zona waktu** 
 
 secara default zona waktu pytanggalmerah adalah Asia/Jakarta tapi bisa diubah, seperti
 
 ``` python
@@ -35,16 +38,16 @@
 t.check()
 ```
  **menggunakan lewat terminal**
 
 
 ```
 $ harilibur # check harilibur
-$ harilibur 2023 04 15 # check harilibur dengan spesifikasi
+$ harilibur 2022 04 15 # check harilibur dengan spesifikasi
 $ TIMEZSET = "Asia/Makasar" harilibur # mengecek harilibur dengan spesifikasi timezone
 
 ```
 
 > harilibur command hanya mengecek tanggal merah dan tidak termasuk hari minggu.
 ### sumber data
 
-**pytanggalmerah** menggunakan data yang bersumber dari google calendar, data yang telah lampau mungkin tidak tersedia & data yang sekarang masih bisa direvisi.
+**pytanggalmerah** menggunakan data yang bersumber dari google calendar, data yang telah lampau mungkin tidak tersedia & data yang sekarang masih bisa direvisi.
```

### Comparing `Pytanggalmerah-3.0.1/pytanggalmerah/TanggalMerah.py` & `Pytanggalmerah-3.1.0/pytanggalmerah/TanggalMerah.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime
 from pytz import timezone
 from .myrequests import MyRequests
 import json
+import os
+
+
+in_cache_path = os.path.abspath(os.path.dirname(__file__)) + "/cache/"
 
 
 class TanggalMerah:
     def __init__(self, cache_path=None, cache_time=600):
         self.event = set([])
         self.date = datetime.now(timezone("Asia/Jakarta"))
-        req = MyRequests("https://raw.githubusercontent.com/guangrei/APIHariLibur_V2/main/calendar.min.json",
-                         cache_path=cache_path, cache_time=cache_time)
+        req = MyRequests("https://raw.githubusercontent.com/guangrei/APIHariLibur_V2/main/holidays.json",
+                         cache_path=in_cache_path, cache_time=cache_time)
         self.data = json.loads(req.response)
 
     # end __init_()
 
     def set_timezone(self, tz):
         self.date = datetime.now(timezone(tz))
         return self.date
@@ -35,16 +39,16 @@
         else:
             return False
 
     # end is_sunday()
 
     def is_holiday(self):
         d = self.date.strftime("%Y-%m-%d")
-        if d in self.data and self.data[d]['holiday']:
-            self.event.add(" | ".join(self.data[d]['summary']))
+        if d in self.data:
+            self.event.add(self.data[d]['summary'])
             return True
         else:
             return False
 
     # end is_holiday()
 
     def set_date(self, y, m, d):
```

### Comparing `Pytanggalmerah-3.0.1/pytanggalmerah/myrequests.py` & `Pytanggalmerah-3.1.0/pytanggalmerah/myrequests.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # -*- coding: utf-8 -*-
 import requests
 from zcache import Cache
 from urllib import parse
-import pytanggalmerahcache
 import os
 
 
 class MyRequests(object):
     def __init__(self, url, cache_time, cache_path=None):
 
         u_en = parse.quote_plus(url)  # url encode
-        if cache_path is None:
-            cache_path = os.path.abspath(
-                os.path.dirname(pytanggalmerahcache.__file__))
         cache = Cache(path=cache_path)
         if cache.has(u_en):
             self.response = cache.get(u_en)
             self.is_loaded_from_cache = True
         else:
             r = self.makeRequest(url)
             if r != False:
```

### Comparing `Pytanggalmerah-3.0.1/setup.py` & `Pytanggalmerah-3.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 ]
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='Pytanggalmerah',
-    version='3.0.1',
-    packages=['pytanggalmerah', 'pytanggalmerahcache'],
+    version='3.1.0',
+    packages=['pytanggalmerah'],
     scripts=["harilibur"],
     license='MIT',
     author="guangrei",
     author_email="myawn@pm.me",
     description="python module to check indonesia holiday calendar (include sunday)",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

