# Comparing `tmp/minlog-0.2.0.tar.gz` & `tmp/minlog-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minlog-0.2.0.tar", max compression
+gzip compressed data, was "minlog-0.3.0.tar", max compression
```

## Comparing `minlog-0.2.0.tar` & `minlog-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0       26 2023-06-07 18:56:59.420529 minlog-0.2.0/README.md
--rw-r--r--   0        0        0     1718 2023-06-07 18:55:13.390059 minlog-0.2.0/minlog/__init__.py
--rw-r--r--   0        0        0      297 2023-07-27 02:20:10.373316 minlog-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 minlog-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       26 2023-06-07 18:56:59.420529 minlog-0.3.0/README.md
+-rw-r--r--   0        0        0     4869 2023-07-27 05:55:47.270050 minlog-0.3.0/minlog/__init__.py
+-rw-r--r--   0        0        0      523 2023-07-27 05:52:40.500198 minlog-0.3.0/minlog/_test.py
+-rw-r--r--   0        0        0      297 2023-07-27 05:36:03.383457 minlog-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 minlog-0.3.0/PKG-INFO
```

### Comparing `minlog-0.2.0/PKG-INFO` & `minlog-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minlog
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: redthing1
 Author-email: redthing1@alt.icu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

