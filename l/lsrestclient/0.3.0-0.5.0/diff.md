# Comparing `tmp/lsrestclient-0.3.0.tar.gz` & `tmp/lsrestclient-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsrestclient-0.3.0.tar", max compression
+gzip compressed data, was "lsrestclient-0.5.0.tar", max compression
```

## Comparing `lsrestclient-0.3.0.tar` & `lsrestclient-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.649481 lsrestclient-0.3.0/README.md
--rw-r--r--   0        0        0     3463 2023-07-27 13:55:03.321953 lsrestclient-0.3.0/lsrestclient/__init__.py
--rw-r--r--   0        0        0      212 2023-07-27 13:55:03.321953 lsrestclient-0.3.0/lsrestclient/exceptions.py
--rw-r--r--   0        0        0      706 2023-07-27 13:55:33.098831 lsrestclient-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6672 1970-01-01 00:00:00.000000 lsrestclient-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.649481 lsrestclient-0.5.0/README.md
+-rw-r--r--   0        0        0       72 2023-07-27 14:36:50.038756 lsrestclient-0.5.0/lsrestclient/__init__.py
+-rw-r--r--   0        0        0     8704 2023-07-27 14:36:50.038756 lsrestclient-0.5.0/lsrestclient/client.py
+-rw-r--r--   0        0        0      588 2023-07-27 14:36:50.038756 lsrestclient-0.5.0/lsrestclient/exceptions.py
+-rw-r--r--   0        0        0     1088 2023-07-27 14:36:50.038756 lsrestclient-0.5.0/lsrestclient/response.py
+-rw-r--r--   0        0        0      706 2023-07-27 14:37:11.566388 lsrestclient-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6672 1970-01-01 00:00:00.000000 lsrestclient-0.5.0/PKG-INFO
```

### Comparing `lsrestclient-0.3.0/README.md` & `lsrestclient-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lsrestclient-0.3.0/pyproject.toml` & `lsrestclient-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lsrestclient"
-version = "0.3.0"
+version = "0.5.0"
 description = "REST Api Client"
 authors = ["mba <bartel@electronic-shop.lu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
```

### Comparing `lsrestclient-0.3.0/PKG-INFO` & `lsrestclient-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsrestclient
-Version: 0.3.0
+Version: 0.5.0
 Summary: REST Api Client
 Author: mba
 Author-email: bartel@electronic-shop.lu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

