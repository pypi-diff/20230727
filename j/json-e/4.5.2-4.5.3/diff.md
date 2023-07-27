# Comparing `tmp/json-e-4.5.2.tar.gz` & `tmp/json-e-4.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-e-4.5.2.tar", last modified: Mon Apr 10 12:17:08 2023, max compression
+gzip compressed data, was "json-e-4.5.3.tar", last modified: Thu Jul 27 02:28:58 2023, max compression
```

## Comparing `json-e-4.5.2.tar` & `json-e-4.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 dustin    (1002) dustin    (1002)        0 2023-04-10 12:17:08.048677 json-e-4.5.2/
--rw-rw-r--   0 dustin    (1002) dustin    (1002)       65 2021-12-03 22:39:01.000000 json-e-4.5.2/MANIFEST.in
--rw-rw-r--   0 dustin    (1002) dustin    (1002)      471 2023-04-10 12:17:08.048677 json-e-4.5.2/PKG-INFO
-drwxrwxr-x   0 dustin    (1002) dustin    (1002)        0 2023-04-10 12:17:08.044677 json-e-4.5.2/json_e.egg-info/
--rw-rw-r--   0 dustin    (1002) dustin    (1002)      471 2023-04-10 12:17:07.000000 json-e-4.5.2/json_e.egg-info/PKG-INFO
--rw-rw-r--   0 dustin    (1002) dustin    (1002)      310 2023-04-10 12:17:07.000000 json-e-4.5.2/json_e.egg-info/SOURCES.txt
--rw-rw-r--   0 dustin    (1002) dustin    (1002)        1 2023-04-10 12:17:07.000000 json-e-4.5.2/json_e.egg-info/dependency_links.txt
--rw-rw-r--   0 dustin    (1002) dustin    (1002)       21 2023-04-10 12:17:07.000000 json-e-4.5.2/json_e.egg-info/requires.txt
--rw-rw-r--   0 dustin    (1002) dustin    (1002)        6 2023-04-10 12:17:07.000000 json-e-4.5.2/json_e.egg-info/top_level.txt
-drwxrwxr-x   0 dustin    (1002) dustin    (1002)        0 2023-04-10 12:17:08.048677 json-e-4.5.2/jsone/
--rw-rw-r--   0 dustin    (1002) dustin    (1002)     1135 2021-12-03 22:39:01.000000 json-e-4.5.2/jsone/AST.py
--rw-rw-r--   0 dustin    (1002) dustin    (1002)      936 2021-12-03 22:39:01.000000 json-e-4.5.2/jsone/__init__.py
--rw-rw-r--   0 dustin    (1002) dustin    (1002)     4922 2021-12-03 22:39:01.000000 json-e-4.5.2/jsone/builtins.py
--rw-rw-r--   0 dustin    (1002) dustin    (1002)     7623 2021-12-03 22:39:01.000000 json-e-4.5.2/jsone/interpreter.py
--rw-rw-r--   0 dustin    (1002) dustin    (1002)     9405 2022-12-25 18:43:58.000000 json-e-4.5.2/jsone/parser.py
--rw-rw-r--   0 dustin    (1002) dustin    (1002)    14545 2022-12-25 18:43:58.000000 json-e-4.5.2/jsone/render.py
--rw-rw-r--   0 dustin    (1002) dustin    (1002)     3560 2021-12-03 22:39:01.000000 json-e-4.5.2/jsone/shared.py
--rw-rw-r--   0 dustin    (1002) dustin    (1002)      793 2021-12-03 22:39:01.000000 json-e-4.5.2/jsone/six.py
--rw-rw-r--   0 dustin    (1002) dustin    (1002)       81 2023-04-10 12:17:08.048677 json-e-4.5.2/setup.cfg
--rw-rw-r--   0 dustin    (1002) dustin    (1002)      659 2023-04-10 12:16:14.000000 json-e-4.5.2/setup.py
+drwxrwxr-x   0 dustin    (1002) dustin    (1002)        0 2023-07-27 02:28:58.861176 json-e-4.5.3/
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)       65 2023-07-27 02:21:18.000000 json-e-4.5.3/MANIFEST.in
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)      471 2023-07-27 02:28:58.861176 json-e-4.5.3/PKG-INFO
+drwxrwxr-x   0 dustin    (1002) dustin    (1002)        0 2023-07-27 02:28:58.857176 json-e-4.5.3/json_e.egg-info/
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)      471 2023-07-27 02:28:58.000000 json-e-4.5.3/json_e.egg-info/PKG-INFO
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)      310 2023-07-27 02:28:58.000000 json-e-4.5.3/json_e.egg-info/SOURCES.txt
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)        1 2023-07-27 02:28:58.000000 json-e-4.5.3/json_e.egg-info/dependency_links.txt
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)       21 2023-07-27 02:28:58.000000 json-e-4.5.3/json_e.egg-info/requires.txt
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)        6 2023-07-27 02:28:58.000000 json-e-4.5.3/json_e.egg-info/top_level.txt
+drwxrwxr-x   0 dustin    (1002) dustin    (1002)        0 2023-07-27 02:28:58.861176 json-e-4.5.3/jsone/
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)     1135 2023-07-27 02:21:18.000000 json-e-4.5.3/jsone/AST.py
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)      936 2023-07-27 02:21:18.000000 json-e-4.5.3/jsone/__init__.py
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)     4922 2023-07-27 02:21:18.000000 json-e-4.5.3/jsone/builtins.py
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)     7623 2023-07-27 02:21:18.000000 json-e-4.5.3/jsone/interpreter.py
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)     9405 2023-07-27 02:21:18.000000 json-e-4.5.3/jsone/parser.py
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)    14545 2023-07-27 02:21:18.000000 json-e-4.5.3/jsone/render.py
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)     3560 2023-07-27 02:21:18.000000 json-e-4.5.3/jsone/shared.py
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)      793 2023-07-27 02:21:18.000000 json-e-4.5.3/jsone/six.py
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)       81 2023-07-27 02:28:58.861176 json-e-4.5.3/setup.cfg
+-rw-rw-r--   0 dustin    (1002) dustin    (1002)      659 2023-07-27 02:27:49.000000 json-e-4.5.3/setup.py
```

### Comparing `json-e-4.5.2/jsone/AST.py` & `json-e-4.5.3/jsone/AST.py`

 * *Files identical despite different names*

### Comparing `json-e-4.5.2/jsone/__init__.py` & `json-e-4.5.3/jsone/__init__.py`

 * *Files identical despite different names*

### Comparing `json-e-4.5.2/jsone/builtins.py` & `json-e-4.5.3/jsone/builtins.py`

 * *Files identical despite different names*

### Comparing `json-e-4.5.2/jsone/interpreter.py` & `json-e-4.5.3/jsone/interpreter.py`

 * *Files identical despite different names*

### Comparing `json-e-4.5.2/jsone/parser.py` & `json-e-4.5.3/jsone/parser.py`

 * *Files identical despite different names*

### Comparing `json-e-4.5.2/jsone/render.py` & `json-e-4.5.3/jsone/render.py`

 * *Files identical despite different names*

### Comparing `json-e-4.5.2/jsone/shared.py` & `json-e-4.5.3/jsone/shared.py`

 * *Files identical despite different names*

### Comparing `json-e-4.5.2/jsone/six.py` & `json-e-4.5.3/jsone/six.py`

 * *Files identical despite different names*

### Comparing `json-e-4.5.2/setup.py` & `json-e-4.5.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import os
 from setuptools import setup, find_packages
 
-version = "4.5.2"
+version = "4.5.3"
 
 description='A data-structure parameterization system written for embedding context in JSON objects'
 
 long_description = '''\
 {description}.
 
 See https://json-e.js.org for usage information.
```

