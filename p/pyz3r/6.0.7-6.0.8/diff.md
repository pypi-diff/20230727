# Comparing `tmp/pyz3r-6.0.7.tar.gz` & `tmp/pyz3r-6.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyz3r-6.0.7.tar", last modified: Sat Mar 11 18:52:12 2023, max compression
+gzip compressed data, was "pyz3r-6.0.8.tar", last modified: Thu Jul 27 16:35:50 2023, max compression
```

## Comparing `pyz3r-6.0.7.tar` & `pyz3r-6.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 18:52:12.396430 pyz3r-6.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-03-11 18:51:55.000000 pyz3r-6.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-03-11 18:52:12.396430 pyz3r-6.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-03-11 18:51:55.000000 pyz3r-6.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 18:52:12.396430 pyz3r-6.0.7/pyz3r/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-11 18:51:55.000000 pyz3r-6.0.7/pyz3r/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-03-11 18:51:55.000000 pyz3r-6.0.7/pyz3r/alttpr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-03-11 18:51:55.000000 pyz3r-6.0.7/pyz3r/customizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-11 18:51:55.000000 pyz3r-6.0.7/pyz3r/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 18:52:12.396430 pyz3r-6.0.7/pyz3r/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 18:51:55.000000 pyz3r-6.0.7/pyz3r/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-03-11 18:51:55.000000 pyz3r-6.0.7/pyz3r/ext/priestmode.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-03-11 18:51:55.000000 pyz3r-6.0.7/pyz3r/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-03-11 18:51:55.000000 pyz3r-6.0.7/pyz3r/mystery.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-03-11 18:51:55.000000 pyz3r-6.0.7/pyz3r/rom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-03-11 18:51:55.000000 pyz3r-6.0.7/pyz3r/sm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-03-11 18:51:55.000000 pyz3r-6.0.7/pyz3r/smvaria.py
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-03-11 18:51:55.000000 pyz3r-6.0.7/pyz3r/spoiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 18:52:12.396430 pyz3r-6.0.7/pyz3r.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-03-11 18:52:12.000000 pyz3r-6.0.7/pyz3r.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-11 18:52:12.000000 pyz3r-6.0.7/pyz3r.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 18:52:12.000000 pyz3r-6.0.7/pyz3r.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-11 18:52:12.000000 pyz3r-6.0.7/pyz3r.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-11 18:52:12.000000 pyz3r-6.0.7/pyz3r.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 18:52:12.396430 pyz3r-6.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-11 18:51:55.000000 pyz3r-6.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:35:50.135294 pyz3r-6.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-27 16:35:36.000000 pyz3r-6.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-07-27 16:35:50.135294 pyz3r-6.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-07-27 16:35:36.000000 pyz3r-6.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:35:50.135294 pyz3r-6.0.8/pyz3r/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-27 16:35:36.000000 pyz3r-6.0.8/pyz3r/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-07-27 16:35:36.000000 pyz3r-6.0.8/pyz3r/alttpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-27 16:35:36.000000 pyz3r-6.0.8/pyz3r/customizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-27 16:35:36.000000 pyz3r-6.0.8/pyz3r/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:35:50.135294 pyz3r-6.0.8/pyz3r/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:35:36.000000 pyz3r-6.0.8/pyz3r/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-07-27 16:35:36.000000 pyz3r-6.0.8/pyz3r/ext/priestmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-27 16:35:36.000000 pyz3r-6.0.8/pyz3r/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-07-27 16:35:36.000000 pyz3r-6.0.8/pyz3r/mystery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-07-27 16:35:36.000000 pyz3r-6.0.8/pyz3r/rom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-27 16:35:36.000000 pyz3r-6.0.8/pyz3r/sm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-27 16:35:36.000000 pyz3r-6.0.8/pyz3r/smvaria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-07-27 16:35:36.000000 pyz3r-6.0.8/pyz3r/spoiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:35:50.135294 pyz3r-6.0.8/pyz3r.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-07-27 16:35:50.000000 pyz3r-6.0.8/pyz3r.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-27 16:35:50.000000 pyz3r-6.0.8/pyz3r.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:35:50.000000 pyz3r-6.0.8/pyz3r.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-27 16:35:50.000000 pyz3r-6.0.8/pyz3r.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 16:35:50.000000 pyz3r-6.0.8/pyz3r.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 16:35:50.135294 pyz3r-6.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-27 16:35:36.000000 pyz3r-6.0.8/setup.py
```

### Comparing `pyz3r-6.0.7/LICENSE` & `pyz3r-6.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyz3r-6.0.7/PKG-INFO` & `pyz3r-6.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyz3r
-Version: 6.0.7
+Version: 6.0.8
 Summary: A python module for interacting with the web API of various randomizers, such as https://alttpr.com or https://samus.link.
 Home-page: https://github.com/tcprescott/pyz3r
 Author: Thomas Prescott
 Author-email: tcprescott@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyz3r-6.0.7/README.md` & `pyz3r-6.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyz3r-6.0.7/pyz3r/alttpr.py` & `pyz3r-6.0.8/pyz3r/alttpr.py`

 * *Files identical despite different names*

### Comparing `pyz3r-6.0.7/pyz3r/customizer.py` & `pyz3r-6.0.8/pyz3r/customizer.py`

 * *Files identical despite different names*

### Comparing `pyz3r-6.0.7/pyz3r/ext/priestmode.py` & `pyz3r-6.0.8/pyz3r/ext/priestmode.py`

 * *Files identical despite different names*

### Comparing `pyz3r-6.0.7/pyz3r/misc.py` & `pyz3r-6.0.8/pyz3r/misc.py`

 * *Files identical despite different names*

### Comparing `pyz3r-6.0.7/pyz3r/mystery.py` & `pyz3r-6.0.8/pyz3r/mystery.py`

 * *Files identical despite different names*

### Comparing `pyz3r-6.0.7/pyz3r/rom.py` & `pyz3r-6.0.8/pyz3r/rom.py`

 * *Files identical despite different names*

### Comparing `pyz3r-6.0.7/pyz3r/sm.py` & `pyz3r-6.0.8/pyz3r/sm.py`

 * *Files identical despite different names*

### Comparing `pyz3r-6.0.7/pyz3r/spoiler.py` & `pyz3r-6.0.8/pyz3r/spoiler.py`

 * *Files identical despite different names*

### Comparing `pyz3r-6.0.7/pyz3r.egg-info/PKG-INFO` & `pyz3r-6.0.8/pyz3r.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyz3r
-Version: 6.0.7
+Version: 6.0.8
 Summary: A python module for interacting with the web API of various randomizers, such as https://alttpr.com or https://samus.link.
 Home-page: https://github.com/tcprescott/pyz3r
 Author: Thomas Prescott
 Author-email: tcprescott@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyz3r-6.0.7/setup.py` & `pyz3r-6.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="pyz3r",
-    version="6.0.7",
+    version="6.0.8",
     author="Thomas Prescott",
     author_email="tcprescott@gmail.com",
     description="A python module for interacting with the web API of various randomizers, such as https://alttpr.com or https://samus.link.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/tcprescott/pyz3r",
     packages=find_packages(),
```

