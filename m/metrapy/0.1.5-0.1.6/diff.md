# Comparing `tmp/metrapy-0.1.5.tar.gz` & `tmp/metrapy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metrapy-0.1.5.tar", last modified: Thu Jul 27 16:55:33 2023, max compression
+gzip compressed data, was "metrapy-0.1.6.tar", last modified: Thu Jul 27 17:19:53 2023, max compression
```

## Comparing `metrapy-0.1.5.tar` & `metrapy-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 16:55:33.217841 metrapy-0.1.5/
--rw-rw-rw-   0        0        0     2670 2023-07-27 16:55:33.217841 metrapy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2347 2023-07-19 20:01:09.000000 metrapy-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 16:55:33.144976 metrapy-0.1.5/metrapy/
--rw-rw-rw-   0        0        0        0 2023-07-25 03:44:41.000000 metrapy-0.1.5/metrapy/__init__.py
--rw-rw-rw-   0        0        0    13885 2023-07-27 16:52:55.000000 metrapy-0.1.5/metrapy/connector.py
--rw-rw-rw-   0        0        0      205 2023-07-19 19:33:58.000000 metrapy-0.1.5/metrapy/defaults.py
--rw-rw-rw-   0        0        0     2414 2023-07-19 19:32:18.000000 metrapy-0.1.5/metrapy/maps.py
--rw-rw-rw-   0        0        0     1877 2023-07-19 19:33:47.000000 metrapy-0.1.5/metrapy/sync.py
--rw-rw-rw-   0        0        0      654 2023-07-27 16:54:45.000000 metrapy-0.1.5/metrapy/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:55:33.209529 metrapy-0.1.5/metrapy.egg-info/
--rw-rw-rw-   0        0        0     2670 2023-07-27 16:55:32.000000 metrapy-0.1.5/metrapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-07-27 16:55:32.000000 metrapy-0.1.5/metrapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 16:55:32.000000 metrapy-0.1.5/metrapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-27 16:55:32.000000 metrapy-0.1.5/metrapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-27 16:55:32.000000 metrapy-0.1.5/metrapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 16:55:33.217841 metrapy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-07-27 16:55:15.000000 metrapy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:19:53.175578 metrapy-0.1.6/
+-rw-rw-rw-   0        0        0     2670 2023-07-27 17:19:53.175578 metrapy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2347 2023-07-19 20:01:09.000000 metrapy-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 17:19:53.113062 metrapy-0.1.6/metrapy/
+-rw-rw-rw-   0        0        0        0 2023-07-25 03:44:41.000000 metrapy-0.1.6/metrapy/__init__.py
+-rw-rw-rw-   0        0        0    13885 2023-07-27 16:52:55.000000 metrapy-0.1.6/metrapy/connector.py
+-rw-rw-rw-   0        0        0      205 2023-07-19 19:33:58.000000 metrapy-0.1.6/metrapy/defaults.py
+-rw-rw-rw-   0        0        0     2414 2023-07-19 19:32:18.000000 metrapy-0.1.6/metrapy/maps.py
+-rw-rw-rw-   0        0        0     1877 2023-07-19 19:33:47.000000 metrapy-0.1.6/metrapy/sync.py
+-rw-rw-rw-   0        0        0      594 2023-07-27 17:18:37.000000 metrapy-0.1.6/metrapy/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:19:53.175578 metrapy-0.1.6/metrapy.egg-info/
+-rw-rw-rw-   0        0        0     2670 2023-07-27 17:19:52.000000 metrapy-0.1.6/metrapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-07-27 17:19:52.000000 metrapy-0.1.6/metrapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 17:19:52.000000 metrapy-0.1.6/metrapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-27 17:19:52.000000 metrapy-0.1.6/metrapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-27 17:19:52.000000 metrapy-0.1.6/metrapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 17:19:53.175578 metrapy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-07-27 17:19:14.000000 metrapy-0.1.6/setup.py
```

### Comparing `metrapy-0.1.5/PKG-INFO` & `metrapy-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrapy
-Version: 0.1.5
+Version: 0.1.6
 Summary: batteries included wrapper utility for MetaTrader5's python integration
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `metrapy-0.1.5/README.md` & `metrapy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.5/metrapy/connector.py` & `metrapy-0.1.6/metrapy/connector.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.5/metrapy/maps.py` & `metrapy-0.1.6/metrapy/maps.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.5/metrapy/sync.py` & `metrapy-0.1.6/metrapy/sync.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.5/metrapy.egg-info/PKG-INFO` & `metrapy-0.1.6/metrapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrapy
-Version: 0.1.5
+Version: 0.1.6
 Summary: batteries included wrapper utility for MetaTrader5's python integration
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `metrapy-0.1.5/setup.py` & `metrapy-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="metrapy",  # This is the name of the package
-    version="0.1.5",  # The initial release version
+    version="0.1.6",  # The initial release version
     author="pavittarx",  # Full name of the author
     description="batteries included wrapper utility for MetaTrader5's python integration",
     long_description=long_description,  # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),  # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

