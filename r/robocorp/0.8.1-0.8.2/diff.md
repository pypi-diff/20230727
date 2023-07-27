# Comparing `tmp/robocorp-0.8.1.tar.gz` & `tmp/robocorp-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp-0.8.1.tar", max compression
+gzip compressed data, was "robocorp-0.8.2.tar", max compression
```

## Comparing `robocorp-0.8.1.tar` & `robocorp-0.8.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      599 2023-07-18 11:54:37.083345 robocorp-0.8.1/README.md
--rw-r--r--   0        0        0      776 2023-07-18 11:54:37.083345 robocorp-0.8.1/pyproject.toml
--rw-r--r--   0        0        0       78 2023-07-18 11:54:37.087345 robocorp-0.8.1/src/robocorp/_meta/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 11:54:37.087345 robocorp-0.8.1/src/robocorp/_meta/py.typed
--rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 robocorp-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      599 2023-07-27 17:21:53.983795 robocorp-0.8.2/README.md
+-rw-r--r--   0        0        0      776 2023-07-27 17:21:53.983795 robocorp-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-27 17:21:53.983795 robocorp-0.8.2/src/robocorp/_meta/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 17:21:53.983795 robocorp-0.8.2/src/robocorp/_meta/py.typed
+-rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 robocorp-0.8.2/PKG-INFO
```

### Comparing `robocorp-0.8.1/README.md` & `robocorp-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `robocorp-0.8.1/PKG-INFO` & `robocorp-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: robocorp
-Version: 0.8.1
+Version: 0.8.2
 Summary: Robocorp core libraries for Python automation
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Ossi Rajuvaara
 Author-email: ossi@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: robocorp-log (==2.3.0)
-Requires-Dist: robocorp-storage (==0.3.1)
-Requires-Dist: robocorp-tasks (==2.1.2)
+Requires-Dist: robocorp-log (==2.5.0)
+Requires-Dist: robocorp-storage (==0.3.2)
+Requires-Dist: robocorp-tasks (==2.1.3)
 Requires-Dist: robocorp-vault (==1.2.0)
 Requires-Dist: robocorp-workitems (==1.2.1)
 Project-URL: Repository, https://github.com/robocorp/robo/
 Description-Content-Type: text/markdown
 
 # robocorp (metapackage)
```

