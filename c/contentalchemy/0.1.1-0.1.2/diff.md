# Comparing `tmp/contentalchemy-0.1.1.tar.gz` & `tmp/contentalchemy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contentalchemy-0.1.1.tar", max compression
+gzip compressed data, was "contentalchemy-0.1.2.tar", max compression
```

## Comparing `contentalchemy-0.1.1.tar` & `contentalchemy-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-07-27 02:40:10.435321 contentalchemy-0.1.1/README.md
--rw-r--r--   0        0        0      122 2023-07-27 03:11:50.724271 contentalchemy-0.1.1/contentalchemy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 03:13:04.336291 contentalchemy-0.1.1/contentalchemy/images/__init__.py
--rw-r--r--   0        0        0      175 2023-07-27 04:45:27.477854 contentalchemy-0.1.1/contentalchemy/images/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-07-27 03:14:18.966030 contentalchemy-0.1.1/contentalchemy/images/sync_api/__init__.py
--rw-r--r--   0        0        0      184 2023-07-27 04:45:27.477854 contentalchemy-0.1.1/contentalchemy/images/sync_api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2182 2023-07-27 04:45:27.477854 contentalchemy-0.1.1/contentalchemy/images/sync_api/__pycache__/snapper.cpython-310.pyc
--rw-r--r--   0        0        0     2064 2023-07-27 04:05:29.541928 contentalchemy-0.1.1/contentalchemy/images/sync_api/snapper.py
--rwxr-xr-x   0        0        0    16864 2023-07-26 18:41:09.439633 contentalchemy-0.1.1/contentalchemy/images/sync_api/snapshot_template.html
--rw-r--r--   0        0        0      333 2023-07-27 05:38:37.178646 contentalchemy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 contentalchemy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-27 02:40:10.435321 contentalchemy-0.1.2/README.md
+-rw-r--r--   0        0        0      279 2023-07-27 06:01:38.764204 contentalchemy-0.1.2/contentalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 03:13:04.336291 contentalchemy-0.1.2/contentalchemy/images/__init__.py
+-rw-r--r--   0        0        0      175 2023-07-27 04:45:27.477854 contentalchemy-0.1.2/contentalchemy/images/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-07-27 03:14:18.966030 contentalchemy-0.1.2/contentalchemy/images/sync_api/__init__.py
+-rw-r--r--   0        0        0      184 2023-07-27 04:45:27.477854 contentalchemy-0.1.2/contentalchemy/images/sync_api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2182 2023-07-27 04:45:27.477854 contentalchemy-0.1.2/contentalchemy/images/sync_api/__pycache__/snapper.cpython-310.pyc
+-rw-r--r--   0        0        0     2064 2023-07-27 04:05:29.541928 contentalchemy-0.1.2/contentalchemy/images/sync_api/snapper.py
+-rwxr-xr-x   0        0        0    16864 2023-07-26 18:41:09.439633 contentalchemy-0.1.2/contentalchemy/images/sync_api/snapshot_template.html
+-rw-r--r--   0        0        0      333 2023-07-27 06:02:04.726859 contentalchemy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 contentalchemy-0.1.2/PKG-INFO
```

### Comparing `contentalchemy-0.1.1/contentalchemy/images/sync_api/__pycache__/snapper.cpython-310.pyc` & `contentalchemy-0.1.2/contentalchemy/images/sync_api/__pycache__/snapper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `contentalchemy-0.1.1/contentalchemy/images/sync_api/snapper.py` & `contentalchemy-0.1.2/contentalchemy/images/sync_api/snapper.py`

 * *Files identical despite different names*

### Comparing `contentalchemy-0.1.1/contentalchemy/images/sync_api/snapshot_template.html` & `contentalchemy-0.1.2/contentalchemy/images/sync_api/snapshot_template.html`

 * *Files identical despite different names*

### Comparing `contentalchemy-0.1.1/PKG-INFO` & `contentalchemy-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contentalchemy
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: nguyenthanhquang152
 Author-email: nguyenthanhquang.cse@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

