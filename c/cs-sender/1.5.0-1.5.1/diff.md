# Comparing `tmp/cs_sender-1.5.0.tar.gz` & `tmp/cs_sender-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cs_sender-1.5.0.tar", last modified: Thu Nov 17 13:30:39 2022, max compression
+gzip compressed data, was "dist/cs_sender-1.5.1.tar", last modified: Thu Jul 27 02:54:37 2023, max compression
```

## Comparing `cs_sender-1.5.0.tar` & `cs_sender-1.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2022-11-17 13:30:39.000000 cs_sender-1.5.0/
--rw-r--r--   0 arron      (502) staff       (20)     1262 2022-11-17 13:30:39.000000 cs_sender-1.5.0/PKG-INFO
--rw-r--r--   0 arron      (502) staff       (20)      343 2022-11-17 09:13:02.000000 cs_sender-1.5.0/README.md
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2022-11-17 13:30:39.000000 cs_sender-1.5.0/cs_sender/
--rw-r--r--   0 arron      (502) staff       (20)      118 2022-09-23 03:20:16.000000 cs_sender-1.5.0/cs_sender/__init__.py
--rw-r--r--   0 arron      (502) staff       (20)     2806 2022-11-16 06:03:28.000000 cs_sender-1.5.0/cs_sender/api.py
--rw-r--r--   0 arron      (502) staff       (20)      989 2022-09-27 05:48:18.000000 cs_sender-1.5.0/cs_sender/core.py
--rw-r--r--   0 arron      (502) staff       (20)     2372 2022-11-16 06:07:30.000000 cs_sender-1.5.0/cs_sender/extension.py
--rw-r--r--   0 arron      (502) staff       (20)     5365 2022-10-03 13:29:22.000000 cs_sender-1.5.0/cs_sender/log.py
--rw-r--r--   0 arron      (502) staff       (20)      718 2022-11-16 06:12:32.000000 cs_sender-1.5.0/cs_sender/monitor.py
--rw-r--r--   0 arron      (502) staff       (20)     2845 2022-09-19 10:57:11.000000 cs_sender-1.5.0/cs_sender/stats.py
-drwxr-xr-x   0 arron      (502) staff       (20)        0 2022-11-17 13:30:39.000000 cs_sender-1.5.0/cs_sender.egg-info/
--rw-r--r--   0 arron      (502) staff       (20)     1262 2022-11-17 13:30:39.000000 cs_sender-1.5.0/cs_sender.egg-info/PKG-INFO
--rw-r--r--   0 arron      (502) staff       (20)      319 2022-11-17 13:30:39.000000 cs_sender-1.5.0/cs_sender.egg-info/SOURCES.txt
--rw-r--r--   0 arron      (502) staff       (20)        1 2022-11-17 13:30:39.000000 cs_sender-1.5.0/cs_sender.egg-info/dependency_links.txt
--rw-r--r--   0 arron      (502) staff       (20)       16 2022-11-17 13:30:39.000000 cs_sender-1.5.0/cs_sender.egg-info/requires.txt
--rw-r--r--   0 arron      (502) staff       (20)       10 2022-11-17 13:30:39.000000 cs_sender-1.5.0/cs_sender.egg-info/top_level.txt
--rw-r--r--   0 arron      (502) staff       (20)       38 2022-11-17 13:30:39.000000 cs_sender-1.5.0/setup.cfg
--rw-r--r--   0 arron      (502) staff       (20)     1343 2022-11-17 09:12:10.000000 cs_sender-1.5.0/setup.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-27 02:54:37.000000 cs_sender-1.5.1/
+-rw-r--r--   0 arron      (502) staff       (20)     1438 2023-07-27 02:54:37.000000 cs_sender-1.5.1/PKG-INFO
+-rw-r--r--   0 arron      (502) staff       (20)      343 2022-11-17 09:13:02.000000 cs_sender-1.5.1/README.md
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-27 02:54:37.000000 cs_sender-1.5.1/cs_sender/
+-rw-r--r--   0 arron      (502) staff       (20)      118 2022-09-23 03:20:16.000000 cs_sender-1.5.1/cs_sender/__init__.py
+-rw-r--r--   0 arron      (502) staff       (20)     2875 2023-07-27 02:54:24.000000 cs_sender-1.5.1/cs_sender/api.py
+-rw-r--r--   0 arron      (502) staff       (20)      989 2022-09-27 05:48:18.000000 cs_sender-1.5.1/cs_sender/core.py
+-rw-r--r--   0 arron      (502) staff       (20)     2372 2022-11-16 06:07:30.000000 cs_sender-1.5.1/cs_sender/extension.py
+-rw-r--r--   0 arron      (502) staff       (20)     5365 2022-10-03 13:29:22.000000 cs_sender-1.5.1/cs_sender/log.py
+-rw-r--r--   0 arron      (502) staff       (20)      718 2022-11-16 06:12:32.000000 cs_sender-1.5.1/cs_sender/monitor.py
+-rw-r--r--   0 arron      (502) staff       (20)     2845 2022-09-19 10:57:11.000000 cs_sender-1.5.1/cs_sender/stats.py
+drwxr-xr-x   0 arron      (502) staff       (20)        0 2023-07-27 02:54:37.000000 cs_sender-1.5.1/cs_sender.egg-info/
+-rw-r--r--   0 arron      (502) staff       (20)     1438 2023-07-27 02:54:37.000000 cs_sender-1.5.1/cs_sender.egg-info/PKG-INFO
+-rw-r--r--   0 arron      (502) staff       (20)      319 2023-07-27 02:54:37.000000 cs_sender-1.5.1/cs_sender.egg-info/SOURCES.txt
+-rw-r--r--   0 arron      (502) staff       (20)        1 2023-07-27 02:54:37.000000 cs_sender-1.5.1/cs_sender.egg-info/dependency_links.txt
+-rw-r--r--   0 arron      (502) staff       (20)       16 2023-07-27 02:54:37.000000 cs_sender-1.5.1/cs_sender.egg-info/requires.txt
+-rw-r--r--   0 arron      (502) staff       (20)       10 2023-07-27 02:54:37.000000 cs_sender-1.5.1/cs_sender.egg-info/top_level.txt
+-rw-r--r--   0 arron      (502) staff       (20)       38 2023-07-27 02:54:37.000000 cs_sender-1.5.1/setup.cfg
+-rw-r--r--   0 arron      (502) staff       (20)     1343 2023-07-27 02:54:33.000000 cs_sender-1.5.1/setup.py
```

### Comparing `cs_sender-1.5.0/cs_sender/api.py` & `cs_sender-1.5.1/cs_sender/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     @cs_api
     def add_monitor_rule(self, host, project, spider, jobid):
         d = {
             "spider_host": host,
             "spider_project": project,
             "spider_name": spider,
             "spider_job_id": jobid,
+            "description": self._settings.get('CS_DESCRIPTION', ''),
             "monitor_freq": self._settings.get('CS_MONITOR_FREQ', 300),
             "errlog_rate_limit": self._settings.get('CS_ERRLOG_RATE_LIMIT', 0.005),
             "memory_use_limit": self._settings.get('CS_MEMORY_USE_LIMIT', 500)
         }
         response = requests.post(self._monitor_rule_end_point, headers=self.headers, json=d)
         logger.info(f'Add monitor rule, {response.text}')
```

### Comparing `cs_sender-1.5.0/cs_sender/core.py` & `cs_sender-1.5.1/cs_sender/core.py`

 * *Files identical despite different names*

### Comparing `cs_sender-1.5.0/cs_sender/extension.py` & `cs_sender-1.5.1/cs_sender/extension.py`

 * *Files identical despite different names*

### Comparing `cs_sender-1.5.0/cs_sender/log.py` & `cs_sender-1.5.1/cs_sender/log.py`

 * *Files identical despite different names*

### Comparing `cs_sender-1.5.0/cs_sender/monitor.py` & `cs_sender-1.5.1/cs_sender/monitor.py`

 * *Files identical despite different names*

### Comparing `cs_sender-1.5.0/cs_sender/stats.py` & `cs_sender-1.5.1/cs_sender/stats.py`

 * *Files identical despite different names*

### Comparing `cs_sender-1.5.0/setup.py` & `cs_sender-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # !/usr/bin/env python
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='cs_sender',
-    version='V1.5.0',
+    version='V1.5.1',
     description=(
         'scrapy extension for spider monitor web framework cralwer-studio'
     ),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='liuxianglong',
     author_email='liu_xianglong@live.com',
```

