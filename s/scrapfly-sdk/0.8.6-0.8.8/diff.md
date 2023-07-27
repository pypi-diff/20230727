# Comparing `tmp/scrapfly-sdk-0.8.6.tar.gz` & `tmp/scrapfly-sdk-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapfly-sdk-0.8.6.tar", last modified: Thu Jun  8 02:08:49 2023, max compression
+gzip compressed data, was "scrapfly-sdk-0.8.8.tar", last modified: Thu Jul 27 12:38:19 2023, max compression
```

## Comparing `scrapfly-sdk-0.8.6.tar` & `scrapfly-sdk-0.8.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-06-08 02:08:49.817298 scrapfly-sdk-0.8.6/
--rw-r--r--   0 johann    (1000) johann    (1000)     1390 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.6/LICENSE
--rw-r--r--   0 johann    (1000) johann    (1000)     2704 2023-06-08 02:08:49.817298 scrapfly-sdk-0.8.6/PKG-INFO
--rw-r--r--   0 johann    (1000) johann    (1000)     1451 2023-02-21 22:10:41.000000 scrapfly-sdk-0.8.6/README.md
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-06-08 02:08:49.813965 scrapfly-sdk-0.8.6/scrapfly/
--rw-r--r--   0 johann    (1000) johann    (1000)     1336 2023-02-24 16:37:40.000000 scrapfly-sdk-0.8.6/scrapfly/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)    16613 2022-06-14 19:45:38.000000 scrapfly-sdk-0.8.6/scrapfly/api_response.py
--rw-r--r--   0 johann    (1000) johann    (1000)    15969 2023-02-21 22:13:29.000000 scrapfly-sdk-0.8.6/scrapfly/client.py
--rw-r--r--   0 johann    (1000) johann    (1000)     7244 2023-06-08 02:00:48.000000 scrapfly-sdk-0.8.6/scrapfly/errors.py
--rw-r--r--   0 johann    (1000) johann    (1000)      653 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.6/scrapfly/frozen_dict.py
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-06-08 02:08:49.813965 scrapfly-sdk-0.8.6/scrapfly/polyfill/
--rw-r--r--   0 johann    (1000) johann    (1000)        0 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.6/scrapfly/polyfill/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)      556 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.6/scrapfly/polyfill/cached_property.py
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-06-08 02:08:49.813965 scrapfly-sdk-0.8.6/scrapfly/reporter/
--rw-r--r--   0 johann    (1000) johann    (1000)      406 2021-12-18 23:00:36.000000 scrapfly-sdk-0.8.6/scrapfly/reporter/ChainReporter.py
--rw-r--r--   0 johann    (1000) johann    (1000)      214 2021-12-18 22:59:57.000000 scrapfly-sdk-0.8.6/scrapfly/reporter/NoopReporter.py
--rw-r--r--   0 johann    (1000) johann    (1000)      944 2021-12-19 00:22:06.000000 scrapfly-sdk-0.8.6/scrapfly/reporter/PrintReporter.py
--rw-r--r--   0 johann    (1000) johann    (1000)     1164 2022-04-30 01:02:19.000000 scrapfly-sdk-0.8.6/scrapfly/reporter/SentryReporter.py
--rw-r--r--   0 johann    (1000) johann    (1000)      792 2021-12-18 22:59:04.000000 scrapfly-sdk-0.8.6/scrapfly/reporter/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)    11339 2023-02-24 16:27:20.000000 scrapfly-sdk-0.8.6/scrapfly/scrape_config.py
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-06-08 02:08:49.813965 scrapfly-sdk-0.8.6/scrapfly/scrapy/
--rw-r--r--   0 johann    (1000) johann    (1000)      473 2022-05-16 00:35:14.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)     4924 2022-05-13 14:57:24.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/downloader.py
--rw-r--r--   0 johann    (1000) johann    (1000)     3163 2023-06-08 02:00:48.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/middleware.py
--rw-r--r--   0 johann    (1000) johann    (1000)     1800 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/pipelines.py
--rw-r--r--   0 johann    (1000) johann    (1000)     1293 2022-04-05 19:53:12.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/request.py
--rw-r--r--   0 johann    (1000) johann    (1000)     3133 2022-04-05 19:58:38.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/response.py
--rw-r--r--   0 johann    (1000) johann    (1000)     8774 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/spider.py
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-06-08 02:08:49.817298 scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/
--rw-r--r--   0 johann    (1000) johann    (1000)     2704 2023-06-08 02:08:49.000000 scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/PKG-INFO
--rw-r--r--   0 johann    (1000) johann    (1000)      784 2023-06-08 02:08:49.000000 scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 johann    (1000) johann    (1000)        1 2023-06-08 02:08:49.000000 scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 johann    (1000) johann    (1000)      390 2023-06-08 02:08:49.000000 scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/requires.txt
--rw-r--r--   0 johann    (1000) johann    (1000)        9 2023-06-08 02:08:49.000000 scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/top_level.txt
--rw-r--r--   0 johann    (1000) johann    (1000)      272 2023-06-08 02:08:49.817298 scrapfly-sdk-0.8.6/setup.cfg
--rw-r--r--   0 johann    (1000) johann    (1000)     3124 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.6/setup.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/
+-rw-r--r--   0 johann    (1000) johann    (1000)     1390 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.8/LICENSE
+-rw-r--r--   0 johann    (1000) johann    (1000)     2727 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/PKG-INFO
+-rw-r--r--   0 johann    (1000) johann    (1000)     1451 2023-02-21 22:10:41.000000 scrapfly-sdk-0.8.8/README.md
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-07-27 12:38:19.311485 scrapfly-sdk-0.8.8/scrapfly/
+-rw-r--r--   0 johann    (1000) johann    (1000)     1336 2023-06-08 02:08:56.000000 scrapfly-sdk-0.8.8/scrapfly/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)    16613 2022-06-14 19:45:38.000000 scrapfly-sdk-0.8.8/scrapfly/api_response.py
+-rw-r--r--   0 johann    (1000) johann    (1000)    15969 2023-02-21 22:13:29.000000 scrapfly-sdk-0.8.8/scrapfly/client.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     7244 2023-06-08 02:00:48.000000 scrapfly-sdk-0.8.8/scrapfly/errors.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      653 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.8/scrapfly/frozen_dict.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/scrapfly/polyfill/
+-rw-r--r--   0 johann    (1000) johann    (1000)        0 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.8/scrapfly/polyfill/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      556 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.8/scrapfly/polyfill/cached_property.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/scrapfly/reporter/
+-rw-r--r--   0 johann    (1000) johann    (1000)      406 2021-12-18 23:00:36.000000 scrapfly-sdk-0.8.8/scrapfly/reporter/ChainReporter.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      214 2021-12-18 22:59:57.000000 scrapfly-sdk-0.8.8/scrapfly/reporter/NoopReporter.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      944 2021-12-19 00:22:06.000000 scrapfly-sdk-0.8.8/scrapfly/reporter/PrintReporter.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     1164 2022-04-30 01:02:19.000000 scrapfly-sdk-0.8.8/scrapfly/reporter/SentryReporter.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      792 2021-12-18 22:59:04.000000 scrapfly-sdk-0.8.8/scrapfly/reporter/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)    11339 2023-02-24 16:27:20.000000 scrapfly-sdk-0.8.8/scrapfly/scrape_config.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/scrapfly/scrapy/
+-rw-r--r--   0 johann    (1000) johann    (1000)      473 2022-05-16 00:35:14.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     4924 2022-05-13 14:57:24.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/downloader.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     3163 2023-06-08 02:00:48.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/middleware.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     1800 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/pipelines.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     1293 2022-04-05 19:53:12.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/request.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     3133 2022-04-05 19:58:38.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/response.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     8774 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.8/scrapfly/scrapy/spider.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/
+-rw-r--r--   0 johann    (1000) johann    (1000)     2727 2023-07-27 12:38:19.000000 scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 johann    (1000) johann    (1000)      784 2023-07-27 12:38:19.000000 scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)        1 2023-07-27 12:38:19.000000 scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)      556 2023-07-27 12:38:19.000000 scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/requires.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)        9 2023-07-27 12:38:19.000000 scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/top_level.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)      272 2023-07-27 12:38:19.314819 scrapfly-sdk-0.8.8/setup.cfg
+-rw-r--r--   0 johann    (1000) johann    (1000)     3323 2023-07-27 12:32:43.000000 scrapfly-sdk-0.8.8/setup.py
```

### Comparing `scrapfly-sdk-0.8.6/LICENSE` & `scrapfly-sdk-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/PKG-INFO` & `scrapfly-sdk-0.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapfly-sdk
-Version: 0.8.6
+Version: 0.8.8
 Summary: Scrapfly SDK for Scrapfly
 Home-page: https://github.com/scrapfly/python-sdk
 Author: Scrapfly
 Author-email: tech@scrapfly.io
 License: BSD
 Project-URL: Company, https://scrapfly.io
 Project-URL: Documentation, https://scrapfly.io/docs
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: develop
+Provides-Extra: deploy
 Provides-Extra: scrapy
 Provides-Extra: parser
 Provides-Extra: speedups
 Provides-Extra: concurrency
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `scrapfly-sdk-0.8.6/README.md` & `scrapfly-sdk-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/__init__.py` & `scrapfly-sdk-0.8.8/scrapfly/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.6'
+__version__ = '0.8.8'
 
 from typing import Tuple
 from .errors import ScrapflyError
 from .errors import ScrapflyAspError
 from .errors import ScrapflyProxyError
 from .errors import ScrapflyScheduleError
 from .errors import ScrapflyScrapeError
```

### Comparing `scrapfly-sdk-0.8.6/scrapfly/api_response.py` & `scrapfly-sdk-0.8.8/scrapfly/api_response.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/client.py` & `scrapfly-sdk-0.8.8/scrapfly/client.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/errors.py` & `scrapfly-sdk-0.8.8/scrapfly/errors.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/frozen_dict.py` & `scrapfly-sdk-0.8.8/scrapfly/frozen_dict.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/polyfill/cached_property.py` & `scrapfly-sdk-0.8.8/scrapfly/polyfill/cached_property.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/reporter/PrintReporter.py` & `scrapfly-sdk-0.8.8/scrapfly/reporter/PrintReporter.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/reporter/SentryReporter.py` & `scrapfly-sdk-0.8.8/scrapfly/reporter/SentryReporter.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/reporter/__init__.py` & `scrapfly-sdk-0.8.8/scrapfly/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/scrape_config.py` & `scrapfly-sdk-0.8.8/scrapfly/scrape_config.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/scrapy/downloader.py` & `scrapfly-sdk-0.8.8/scrapfly/scrapy/downloader.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/scrapy/middleware.py` & `scrapfly-sdk-0.8.8/scrapfly/scrapy/middleware.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/scrapy/pipelines.py` & `scrapfly-sdk-0.8.8/scrapfly/scrapy/pipelines.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/scrapy/request.py` & `scrapfly-sdk-0.8.8/scrapfly/scrapy/request.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/scrapy/response.py` & `scrapfly-sdk-0.8.8/scrapfly/scrapy/response.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly/scrapy/spider.py` & `scrapfly-sdk-0.8.8/scrapfly/scrapy/spider.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/PKG-INFO` & `scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapfly-sdk
-Version: 0.8.6
+Version: 0.8.8
 Summary: Scrapfly SDK for Scrapfly
 Home-page: https://github.com/scrapfly/python-sdk
 Author: Scrapfly
 Author-email: tech@scrapfly.io
 License: BSD
 Project-URL: Company, https://scrapfly.io
 Project-URL: Documentation, https://scrapfly.io/docs
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: develop
+Provides-Extra: deploy
 Provides-Extra: scrapy
 Provides-Extra: parser
 Provides-Extra: speedups
 Provides-Extra: concurrency
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/SOURCES.txt` & `scrapfly-sdk-0.8.8/scrapfly_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.6/setup.py` & `scrapfly-sdk-0.8.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,26 +46,37 @@
         'isort',
         'readme_renderer',
         'twine',
         'setuptools',
         'wheel',
         'pdoc3'
     ],
+    'deploy': [
+        'bumpversion',
+        'isort',
+        'readme_renderer',
+        'twine',
+        'setuptools',
+        'wheel',
+        'pdoc3',
+        'pip',
+        'colorama',
+        'sentry-sdk'
+    ],
     'scrapy': [
         'scrapy>=2.4.0'
     ],
     'parser': [
         'lxml',
         'beautifulsoup4',
         'soupsieve',
         'extruct'
     ],
     'speedups': [
         'brotlipy',
-        'cchardet',
         'msgpack'
     ],
     'concurrency': []
 }
 
 all_deps = set()
 for env, deps in EXTRA_DEPENDENCIES.items():
```

