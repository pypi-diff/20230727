# Comparing `tmp/httpconcurrent-0.1.0.tar.gz` & `tmp/httpconcurrent-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpconcurrent-0.1.0.tar", last modified: Wed Jul 26 20:30:47 2023, max compression
+gzip compressed data, was "httpconcurrent-0.2.0.tar", last modified: Thu Jul 27 09:47:30 2023, max compression
```

## Comparing `httpconcurrent-0.1.0.tar` & `httpconcurrent-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 20:30:47.489712 httpconcurrent-0.1.0/
--rw-rw-rw-   0        0        0      840 2023-07-26 20:30:47.488712 httpconcurrent-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 20:30:47.487711 httpconcurrent-0.1.0/httpconcurrent.egg-info/
--rw-rw-rw-   0        0        0      840 2023-07-26 20:30:47.000000 httpconcurrent-0.1.0/httpconcurrent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-07-26 20:30:47.000000 httpconcurrent-0.1.0/httpconcurrent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 20:30:47.000000 httpconcurrent-0.1.0/httpconcurrent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-07-26 20:30:47.000000 httpconcurrent-0.1.0/httpconcurrent.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 20:30:47.000000 httpconcurrent-0.1.0/httpconcurrent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 20:30:47.489712 httpconcurrent-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1115 2023-07-26 20:27:21.000000 httpconcurrent-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:47:30.616983 httpconcurrent-0.2.0/
+-rw-rw-rw-   0        0        0      840 2023-07-27 09:47:30.616983 httpconcurrent-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 09:47:30.604628 httpconcurrent-0.2.0/httpconcurrent/
+-rw-rw-rw-   0        0        0       42 2023-07-27 09:46:33.000000 httpconcurrent-0.2.0/httpconcurrent/__init__.py
+-rw-rw-rw-   0        0        0    20487 2023-07-26 17:35:31.000000 httpconcurrent-0.2.0/httpconcurrent/httpconcurrent.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:47:30.615514 httpconcurrent-0.2.0/httpconcurrent.egg-info/
+-rw-rw-rw-   0        0        0      840 2023-07-27 09:47:30.000000 httpconcurrent-0.2.0/httpconcurrent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-07-27 09:47:30.000000 httpconcurrent-0.2.0/httpconcurrent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 09:47:30.000000 httpconcurrent-0.2.0/httpconcurrent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-27 09:47:30.000000 httpconcurrent-0.2.0/httpconcurrent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-27 09:47:30.000000 httpconcurrent-0.2.0/httpconcurrent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 09:47:30.616983 httpconcurrent-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1115 2023-07-27 09:47:24.000000 httpconcurrent-0.2.0/setup.py
```

### Comparing `httpconcurrent-0.1.0/PKG-INFO` & `httpconcurrent-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpconcurrent
-Version: 0.1.0
+Version: 0.2.0
 Summary: HTTP Concurrent: A Python library for handling HTTP requests and managing threads.
 Home-page: UNKNOWN
 Author: Mattew
 Author-email: mattewrak@hotmail.com
 License: UNKNOWN
 Description: The package simplifies making HTTP requests, managing concurrent threads, and performing various network-related tasks with ease.
 Keywords: httpconcurrent,http requests,thread management,concurrent requests,network tasks
```

### Comparing `httpconcurrent-0.1.0/httpconcurrent.egg-info/PKG-INFO` & `httpconcurrent-0.2.0/httpconcurrent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpconcurrent
-Version: 0.1.0
+Version: 0.2.0
 Summary: HTTP Concurrent: A Python library for handling HTTP requests and managing threads.
 Home-page: UNKNOWN
 Author: Mattew
 Author-email: mattewrak@hotmail.com
 License: UNKNOWN
 Description: The package simplifies making HTTP requests, managing concurrent threads, and performing various network-related tasks with ease.
 Keywords: httpconcurrent,http requests,thread management,concurrent requests,network tasks
```

### Comparing `httpconcurrent-0.1.0/setup.py` & `httpconcurrent-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='httpconcurrent',
-    version='0.1.0',
+    version='0.2.0',
     description='HTTP Concurrent: A Python library for handling HTTP requests and managing threads.',
     long_description='The package simplifies making HTTP requests, managing concurrent threads, and performing various network-related tasks with ease.',
     long_description_content_type='text/markdown',
     author='Mattew',
     author_email='mattewrak@hotmail.com',
     packages=find_packages(),
     install_requires=[
```

