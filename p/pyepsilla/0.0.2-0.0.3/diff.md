# Comparing `tmp/pyepsilla-0.0.2.tar.gz` & `tmp/pyepsilla-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepsilla-0.0.2.tar", last modified: Mon Jul 24 17:10:53 2023, max compression
+gzip compressed data, was "pyepsilla-0.0.3.tar", last modified: Thu Jul 27 17:13:44 2023, max compression
```

## Comparing `pyepsilla-0.0.2.tar` & `pyepsilla-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-24 17:10:53.893412 pyepsilla-0.0.2/
--rw-r--r--   0 eric       (501) staff       (20)    11357 2023-07-24 16:13:02.000000 pyepsilla-0.0.2/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)        0 2023-07-24 16:17:39.000000 pyepsilla-0.0.2/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-24 17:10:53.893314 pyepsilla-0.0.2/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      357 2023-07-24 17:07:13.000000 pyepsilla-0.0.2/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-24 17:10:53.891817 pyepsilla-0.0.2/pyepsilla/
--rw-r--r--   0 eric       (501) staff       (20)       69 2023-07-24 17:00:28.000000 pyepsilla-0.0.2/pyepsilla/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-24 17:10:53.893121 pyepsilla-0.0.2/pyepsilla/vectordb/
--rw-r--r--   0 eric       (501) staff       (20)       97 2023-07-24 17:05:00.000000 pyepsilla-0.0.2/pyepsilla/vectordb/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      381 2023-07-24 17:04:43.000000 pyepsilla-0.0.2/pyepsilla/vectordb/client.py
--rw-r--r--   0 eric       (501) staff       (20)      142 2023-07-24 17:05:50.000000 pyepsilla-0.0.2/pyepsilla/vectordb/filed.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-24 17:10:53.892438 pyepsilla-0.0.2/pyepsilla.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-24 17:10:53.000000 pyepsilla-0.0.2/pyepsilla.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      312 2023-07-24 17:10:53.000000 pyepsilla-0.0.2/pyepsilla.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-24 17:10:53.000000 pyepsilla-0.0.2/pyepsilla.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       17 2023-07-24 17:10:53.000000 pyepsilla-0.0.2/pyepsilla.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       10 2023-07-24 17:10:53.000000 pyepsilla-0.0.2/pyepsilla.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-24 17:10:53.893446 pyepsilla-0.0.2/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)      546 2023-07-24 17:09:59.000000 pyepsilla-0.0.2/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-27 17:13:44.140181 pyepsilla-0.0.3/
+-rw-r--r--   0 eric       (501) staff       (20)    11357 2023-07-24 16:13:02.000000 pyepsilla-0.0.3/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)        0 2023-07-24 16:17:39.000000 pyepsilla-0.0.3/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-27 17:13:44.140076 pyepsilla-0.0.3/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      357 2023-07-24 17:07:13.000000 pyepsilla-0.0.3/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-27 17:13:44.138213 pyepsilla-0.0.3/pyepsilla/
+-rw-r--r--   0 eric       (501) staff       (20)       69 2023-07-24 17:00:28.000000 pyepsilla-0.0.3/pyepsilla/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     1422 2023-07-27 17:08:27.000000 pyepsilla-0.0.3/pyepsilla/simple_example.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-27 17:13:44.139725 pyepsilla-0.0.3/pyepsilla/vectordb/
+-rw-r--r--   0 eric       (501) staff       (20)      108 2023-07-27 16:02:20.000000 pyepsilla-0.0.3/pyepsilla/vectordb/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     3902 2023-07-27 17:06:13.000000 pyepsilla-0.0.3/pyepsilla/vectordb/client.py
+-rw-r--r--   0 eric       (501) staff       (20)      410 2023-07-27 17:05:39.000000 pyepsilla-0.0.3/pyepsilla/vectordb/field.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-27 17:13:44.139154 pyepsilla-0.0.3/pyepsilla.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)      298 2023-07-27 17:13:44.000000 pyepsilla-0.0.3/pyepsilla.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      340 2023-07-27 17:13:44.000000 pyepsilla-0.0.3/pyepsilla.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-27 17:13:44.000000 pyepsilla-0.0.3/pyepsilla.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       17 2023-07-27 17:13:44.000000 pyepsilla-0.0.3/pyepsilla.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       10 2023-07-27 17:13:44.000000 pyepsilla-0.0.3/pyepsilla.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-07-27 17:13:44.140215 pyepsilla-0.0.3/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)      546 2023-07-27 17:11:49.000000 pyepsilla-0.0.3/setup.py
```

### Comparing `pyepsilla-0.0.2/LICENSE` & `pyepsilla-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.0.2/setup.py` & `pyepsilla-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyepsilla',
-    version= '0.0.2',
+    version= '0.0.3',
     keywords='epsilla',
     author= 'Epsilla Team',
     description='Epsilla Python SDK',
     license='Apache License',
     packages=find_packages(),
     include_package_data=True,
     platforms='any',
```

