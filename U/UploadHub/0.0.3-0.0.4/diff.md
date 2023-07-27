# Comparing `tmp/UploadHub-0.0.3.tar.gz` & `tmp/UploadHub-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UploadHub-0.0.3.tar", last modified: Thu Jul 27 01:40:26 2023, max compression
+gzip compressed data, was "UploadHub-0.0.4.tar", last modified: Thu Jul 27 01:45:15 2023, max compression
```

## Comparing `UploadHub-0.0.3.tar` & `UploadHub-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 01:40:25.999223 UploadHub-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:02.000000 UploadHub-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      516 2023-07-27 01:40:25.996220 UploadHub-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-18 18:43:42.000000 UploadHub-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 01:40:25.954217 UploadHub-0.0.3/UploadHub/
--rw-rw-rw-   0        0        0        0 2023-07-23 05:01:02.000000 UploadHub-0.0.3/UploadHub/__init__.py
--rw-rw-rw-   0        0        0      704 2023-07-23 05:09:33.000000 UploadHub-0.0.3/UploadHub/__main__.py
--rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:06.000000 UploadHub-0.0.3/UploadHub/license.py
--rw-rw-rw-   0        0        0     9815 2023-07-23 05:09:52.000000 UploadHub-0.0.3/UploadHub/new.py
--rw-rw-rw-   0        0        0      651 2023-07-19 04:20:31.000000 UploadHub-0.0.3/UploadHub/setup.py
--rw-rw-rw-   0        0        0     8234 2023-07-23 05:09:49.000000 UploadHub-0.0.3/UploadHub/upload.py
--rw-rw-rw-   0        0        0     2345 2023-07-27 01:39:15.000000 UploadHub-0.0.3/UploadHub/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:40:25.992220 UploadHub-0.0.3/UploadHub.egg-info/
--rw-rw-rw-   0        0        0      516 2023-07-27 01:40:25.000000 UploadHub-0.0.3/UploadHub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-07-27 01:40:25.000000 UploadHub-0.0.3/UploadHub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 01:40:25.000000 UploadHub-0.0.3/UploadHub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-27 01:40:25.000000 UploadHub-0.0.3/UploadHub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 01:40:25.000000 UploadHub-0.0.3/UploadHub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 01:40:25.999223 UploadHub-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      883 2023-07-27 01:40:13.000000 UploadHub-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:45:15.405163 UploadHub-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:02.000000 UploadHub-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      516 2023-07-27 01:45:15.404183 UploadHub-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-18 18:43:42.000000 UploadHub-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 01:45:15.354145 UploadHub-0.0.4/UploadHub/
+-rw-rw-rw-   0        0        0        0 2023-07-23 05:01:02.000000 UploadHub-0.0.4/UploadHub/__init__.py
+-rw-rw-rw-   0        0        0      704 2023-07-23 05:09:33.000000 UploadHub-0.0.4/UploadHub/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:45:15.401168 UploadHub-0.0.4/UploadHub/data/
+-rw-rw-rw-   0        0        0      112 2023-07-23 04:18:02.000000 UploadHub-0.0.4/UploadHub/data/config.json
+-rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:06.000000 UploadHub-0.0.4/UploadHub/license.py
+-rw-rw-rw-   0        0        0     9815 2023-07-23 05:09:52.000000 UploadHub-0.0.4/UploadHub/new.py
+-rw-rw-rw-   0        0        0      651 2023-07-19 04:20:31.000000 UploadHub-0.0.4/UploadHub/setup.py
+-rw-rw-rw-   0        0        0     8234 2023-07-23 05:09:49.000000 UploadHub-0.0.4/UploadHub/upload.py
+-rw-rw-rw-   0        0        0     2345 2023-07-27 01:39:15.000000 UploadHub-0.0.4/UploadHub/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:45:15.391151 UploadHub-0.0.4/UploadHub.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-27 01:45:15.000000 UploadHub-0.0.4/UploadHub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-27 01:45:15.000000 UploadHub-0.0.4/UploadHub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 01:45:15.000000 UploadHub-0.0.4/UploadHub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-27 01:45:15.000000 UploadHub-0.0.4/UploadHub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 01:45:15.000000 UploadHub-0.0.4/UploadHub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 01:45:15.406163 UploadHub-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-07-27 01:45:13.000000 UploadHub-0.0.4/setup.py
```

### Comparing `UploadHub-0.0.3/LICENSE` & `UploadHub-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.3/PKG-INFO` & `UploadHub-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UploadHub
-Version: 0.0.3
+Version: 0.0.4
 Summary: PYPI and GitHub package uploader.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `UploadHub-0.0.3/UploadHub/__main__.py` & `UploadHub-0.0.4/UploadHub/__main__.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.3/UploadHub/license.py` & `UploadHub-0.0.4/UploadHub/license.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.3/UploadHub/new.py` & `UploadHub-0.0.4/UploadHub/new.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.3/UploadHub/setup.py` & `UploadHub-0.0.4/UploadHub/setup.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.3/UploadHub/upload.py` & `UploadHub-0.0.4/UploadHub/upload.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.3/UploadHub/utils.py` & `UploadHub-0.0.4/UploadHub/utils.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.3/UploadHub.egg-info/PKG-INFO` & `UploadHub-0.0.4/UploadHub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UploadHub
-Version: 0.0.3
+Version: 0.0.4
 Summary: PYPI and GitHub package uploader.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

