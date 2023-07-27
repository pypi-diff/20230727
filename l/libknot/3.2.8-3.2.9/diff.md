# Comparing `tmp/libknot-3.2.8.tar.gz` & `tmp/libknot-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libknot-3.2.8.tar", last modified: Mon Jun 26 05:51:49 2023, max compression
+gzip compressed data, was "libknot-3.2.9.tar", last modified: Thu Jul 27 05:55:18 2023, max compression
```

## Comparing `libknot-3.2.8.tar` & `libknot-3.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-06-26 05:51:49.971862 libknot-3.2.8/
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4876 2023-06-26 05:51:49.971862 libknot-3.2.8/PKG-INFO
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4140 2023-06-26 05:51:16.000000 libknot-3.2.8/README.md
-drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-06-26 05:51:49.971862 libknot-3.2.8/libknot/
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     2457 2023-06-26 05:51:37.000000 libknot-3.2.8/libknot/__init__.py
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)    10988 2022-10-03 08:30:42.000000 libknot-3.2.8/libknot/control.py
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     2862 2023-06-26 05:51:16.000000 libknot-3.2.8/libknot/dname.py
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     9802 2023-02-02 10:28:39.000000 libknot-3.2.8/libknot/probe.py
-drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-06-26 05:51:49.971862 libknot-3.2.8/libknot.egg-info/
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4876 2023-06-26 05:51:49.000000 libknot-3.2.8/libknot.egg-info/PKG-INFO
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)      215 2023-06-26 05:51:49.000000 libknot-3.2.8/libknot.egg-info/SOURCES.txt
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)        1 2023-06-26 05:51:49.000000 libknot-3.2.8/libknot.egg-info/dependency_links.txt
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)        8 2023-06-26 05:51:49.000000 libknot-3.2.8/libknot.egg-info/top_level.txt
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)       38 2023-06-26 05:51:49.971862 libknot-3.2.8/setup.cfg
--rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     1004 2023-06-26 05:51:37.000000 libknot-3.2.8/setup.py
+drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-07-27 05:55:18.704540 libknot-3.2.9/
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4876 2023-07-27 05:55:18.704540 libknot-3.2.9/PKG-INFO
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4140 2023-06-26 05:51:16.000000 libknot-3.2.9/README.md
+drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-07-27 05:55:18.704540 libknot-3.2.9/libknot/
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     2457 2023-07-27 05:54:40.000000 libknot-3.2.9/libknot/__init__.py
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)    10988 2022-10-03 08:30:42.000000 libknot-3.2.9/libknot/control.py
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     2862 2023-06-26 05:51:16.000000 libknot-3.2.9/libknot/dname.py
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     9802 2023-02-02 10:28:39.000000 libknot-3.2.9/libknot/probe.py
+drwxrwxr-x   0 dsalzman  (1000) dsalzman  (1000)        0 2023-07-27 05:55:18.704540 libknot-3.2.9/libknot.egg-info/
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     4876 2023-07-27 05:55:18.000000 libknot-3.2.9/libknot.egg-info/PKG-INFO
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)      215 2023-07-27 05:55:18.000000 libknot-3.2.9/libknot.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)        1 2023-07-27 05:55:18.000000 libknot-3.2.9/libknot.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)        8 2023-07-27 05:55:18.000000 libknot-3.2.9/libknot.egg-info/top_level.txt
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)       38 2023-07-27 05:55:18.704540 libknot-3.2.9/setup.cfg
+-rw-rw-r--   0 dsalzman  (1000) dsalzman  (1000)     1004 2023-07-27 05:54:40.000000 libknot-3.2.9/setup.py
```

### Comparing `libknot-3.2.8/PKG-INFO` & `libknot-3.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libknot
-Version: 3.2.8
+Version: 3.2.9
 Summary: Python bindings for libknot
 Home-page: https://gitlab.nic.cz/knot/knot-dns
 Author: Daniel Salzman
 Author-email: daniel.salzman@nic.cz
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `libknot-3.2.8/README.md` & `libknot-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `libknot-3.2.8/libknot/__init__.py` & `libknot-3.2.9/libknot/__init__.py`

 * *Files identical despite different names*

### Comparing `libknot-3.2.8/libknot/control.py` & `libknot-3.2.9/libknot/control.py`

 * *Files identical despite different names*

### Comparing `libknot-3.2.8/libknot/dname.py` & `libknot-3.2.9/libknot/dname.py`

 * *Files identical despite different names*

### Comparing `libknot-3.2.8/libknot/probe.py` & `libknot-3.2.9/libknot/probe.py`

 * *Files identical despite different names*

### Comparing `libknot-3.2.8/libknot.egg-info/PKG-INFO` & `libknot-3.2.9/libknot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libknot
-Version: 3.2.8
+Version: 3.2.9
 Summary: Python bindings for libknot
 Home-page: https://gitlab.nic.cz/knot/knot-dns
 Author: Daniel Salzman
 Author-email: daniel.salzman@nic.cz
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `libknot-3.2.8/setup.py` & `libknot-3.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 p = pathlib.Path("README.md")
 if p.exists():
     long_description = p.read_text()
 
 setuptools.setup(
     name='libknot',
-    version='3.2.8',
+    version='3.2.9',
     description='Python bindings for libknot',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Daniel Salzman',
     author_email='daniel.salzman@nic.cz',
     url='https://gitlab.nic.cz/knot/knot-dns',
     license='GPL-3.0',
```

