# Comparing `tmp/csvm-0.0.1.tar.gz` & `tmp/csvm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvm-0.0.1.tar", last modified: Sat Jun 10 15:48:43 2023, max compression
+gzip compressed data, was "csvm-0.0.2.tar", last modified: Thu Jul 27 00:57:38 2023, max compression
```

## Comparing `csvm-0.0.1.tar` & `csvm-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-10 15:48:43.087058 csvm-0.0.1/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        0 2023-05-19 22:50:04.000000 csvm-0.0.1/LICENSE
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     3634 2023-06-10 15:48:43.087058 csvm-0.0.1/PKG-INFO
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     3440 2023-06-10 15:44:53.000000 csvm-0.0.1/README.md
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      328 2023-06-10 15:47:47.000000 csvm-0.0.1/pyproject.toml
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       38 2023-06-10 15:48:43.087058 csvm-0.0.1/setup.cfg
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-10 15:48:43.087058 csvm-0.0.1/src/
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-10 15:48:43.087058 csvm-0.0.1/src/csvm/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       99 2023-06-06 12:31:16.000000 csvm-0.0.1/src/csvm/__init__.py
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      910 2023-06-05 12:40:49.000000 csvm-0.0.1/src/csvm/models.py
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     3320 2023-06-06 12:30:07.000000 csvm-0.0.1/src/csvm/reader.py
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-10 15:48:43.087058 csvm-0.0.1/src/csvm.egg-info/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     3634 2023-06-10 15:48:43.000000 csvm-0.0.1/src/csvm.egg-info/PKG-INFO
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      240 2023-06-10 15:48:43.000000 csvm-0.0.1/src/csvm.egg-info/SOURCES.txt
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        1 2023-06-10 15:48:43.000000 csvm-0.0.1/src/csvm.egg-info/dependency_links.txt
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        5 2023-06-10 15:48:43.000000 csvm-0.0.1/src/csvm.egg-info/top_level.txt
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-10 15:48:43.087058 csvm-0.0.1/tests/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     2100 2023-06-06 12:26:20.000000 csvm-0.0.1/tests/test_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:57:38.249992 csvm-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 00:57:29.000000 csvm-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-27 00:57:38.249992 csvm-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-27 00:57:29.000000 csvm-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-27 00:57:29.000000 csvm-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:57:38.249992 csvm-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:57:38.245992 csvm-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:57:38.249992 csvm-0.0.2/src/csvm/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-27 00:57:29.000000 csvm-0.0.2/src/csvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-27 00:57:29.000000 csvm-0.0.2/src/csvm/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-27 00:57:29.000000 csvm-0.0.2/src/csvm/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:57:38.249992 csvm-0.0.2/src/csvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-27 00:57:38.000000 csvm-0.0.2/src/csvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-27 00:57:38.000000 csvm-0.0.2/src/csvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:57:38.000000 csvm-0.0.2/src/csvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 00:57:38.000000 csvm-0.0.2/src/csvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-27 00:57:38.000000 csvm-0.0.2/src/csvm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:57:38.249992 csvm-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-27 00:57:29.000000 csvm-0.0.2/tests/test_reader.py
```

### Comparing `csvm-0.0.1/PKG-INFO` & `csvm-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: csvm
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Rafael Sanabria <rafael.d.sanabria@gmail.com>
+License: MIT License
+Project-URL: Repository, https://github.com/rfsan/csvm
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 # CSVM
 
 CSVM is a file format that allows you to save multiple tables, add comments, and include metadata for both tables and columns
 
 ## File format explanation
```

### Comparing `csvm-0.0.1/README.md` & `csvm-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `csvm-0.0.1/src/csvm/models.py` & `csvm-0.0.2/src/csvm/models.py`

 * *Files identical despite different names*

### Comparing `csvm-0.0.1/src/csvm/reader.py` & `csvm-0.0.2/src/csvm/reader.py`

 * *Files identical despite different names*

### Comparing `csvm-0.0.1/src/csvm.egg-info/PKG-INFO` & `csvm-0.0.2/src/csvm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: csvm
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Rafael Sanabria <rafael.d.sanabria@gmail.com>
+License: MIT License
+Project-URL: Repository, https://github.com/rfsan/csvm
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 # CSVM
 
 CSVM is a file format that allows you to save multiple tables, add comments, and include metadata for both tables and columns
 
 ## File format explanation
```

### Comparing `csvm-0.0.1/tests/test_reader.py` & `csvm-0.0.2/tests/test_reader.py`

 * *Files identical despite different names*

