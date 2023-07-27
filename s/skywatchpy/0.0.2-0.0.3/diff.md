# Comparing `tmp/skywatchpy-0.0.2.tar.gz` & `tmp/skywatchpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\skywatchpy-0.0.2.tar", last modified: Thu Jul 27 11:49:50 2023, max compression
+gzip compressed data, was "dist\skywatchpy-0.0.3.tar", last modified: Thu Jul 27 11:52:18 2023, max compression
```

## Comparing `skywatchpy-0.0.2.tar` & `skywatchpy-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:49:50.000000 skywatchpy-0.0.2/
--rw-rw-rw-   0        0        0        0 2023-07-27 10:59:13.000000 skywatchpy-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      323 2023-07-27 11:49:50.000000 skywatchpy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        2 2023-07-27 11:12:22.000000 skywatchpy-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-27 11:49:50.000000 skywatchpy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      682 2023-07-27 11:49:19.000000 skywatchpy-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:49:50.000000 skywatchpy-0.0.2/skywatchpy/
--rw-rw-rw-   0        0        0     1440 2023-07-27 10:55:21.000000 skywatchpy-0.0.2/skywatchpy/countries.py
--rw-rw-rw-   0        0        0      327 2023-07-26 17:45:49.000000 skywatchpy-0.0.2/skywatchpy/KEYS.py
--rw-rw-rw-   0        0        0       64 2023-07-26 18:14:10.000000 skywatchpy-0.0.2/skywatchpy/services.py
--rw-rw-rw-   0        0        0        0 2023-07-27 10:54:08.000000 skywatchpy-0.0.2/skywatchpy/test.py
--rw-rw-rw-   0        0        0     3045 2023-07-27 11:44:21.000000 skywatchpy-0.0.2/skywatchpy/weather.py
--rw-rw-rw-   0        0        0       21 2023-07-27 10:59:40.000000 skywatchpy-0.0.2/skywatchpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:49:50.000000 skywatchpy-0.0.2/skywatchpy.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-27 11:49:50.000000 skywatchpy-0.0.2/skywatchpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-27 11:49:50.000000 skywatchpy-0.0.2/skywatchpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      323 2023-07-27 11:49:50.000000 skywatchpy-0.0.2/skywatchpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       23 2023-07-27 11:49:50.000000 skywatchpy-0.0.2/skywatchpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      358 2023-07-27 11:49:50.000000 skywatchpy-0.0.2/skywatchpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2023-07-27 11:49:50.000000 skywatchpy-0.0.2/skywatchpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 11:52:18.000000 skywatchpy-0.0.3/
+-rw-rw-rw-   0        0        0        0 2023-07-27 10:59:13.000000 skywatchpy-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      323 2023-07-27 11:52:18.000000 skywatchpy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2023-07-27 11:12:22.000000 skywatchpy-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:52:18.000000 skywatchpy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      682 2023-07-27 11:52:17.000000 skywatchpy-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:52:18.000000 skywatchpy-0.0.3/skywatchpy/
+-rw-rw-rw-   0        0        0     1440 2023-07-27 10:55:21.000000 skywatchpy-0.0.3/skywatchpy/countries.py
+-rw-rw-rw-   0        0        0      327 2023-07-26 17:45:49.000000 skywatchpy-0.0.3/skywatchpy/KEYS.py
+-rw-rw-rw-   0        0        0        0 2023-07-27 10:54:08.000000 skywatchpy-0.0.3/skywatchpy/test.py
+-rw-rw-rw-   0        0        0     3056 2023-07-27 11:52:11.000000 skywatchpy-0.0.3/skywatchpy/weather.py
+-rw-rw-rw-   0        0        0       21 2023-07-27 10:59:40.000000 skywatchpy-0.0.3/skywatchpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:52:18.000000 skywatchpy-0.0.3/skywatchpy.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:52:18.000000 skywatchpy-0.0.3/skywatchpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-27 11:49:50.000000 skywatchpy-0.0.3/skywatchpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      323 2023-07-27 11:52:18.000000 skywatchpy-0.0.3/skywatchpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2023-07-27 11:52:18.000000 skywatchpy-0.0.3/skywatchpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      335 2023-07-27 11:52:18.000000 skywatchpy-0.0.3/skywatchpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 11:52:18.000000 skywatchpy-0.0.3/skywatchpy.egg-info/top_level.txt
```

### Comparing `skywatchpy-0.0.2/setup.py` & `skywatchpy-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup_args = dict(
     name="skywatchpy",
-    version="0.0.2",
+    version="0.0.3",
     description="",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Abdurakhmon Asatullayev",
     author_email="abduraxmonasatullayev35@gmail.com",
     url='https://github.com/Abduraxmonnn/SkyWatchPy.git',
     license="MIT",
```

### Comparing `skywatchpy-0.0.2/skywatchpy/countries.py` & `skywatchpy-0.0.3/skywatchpy/countries.py`

 * *Files identical despite different names*

### Comparing `skywatchpy-0.0.2/skywatchpy/weather.py` & `skywatchpy-0.0.3/skywatchpy/weather.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Python
 import requests
 
 
 # Project
 from skywatchpy.KEYS import API_KEY, API_URL
-from countries import countries_name
+from skywatchpy.countries import countries_name
 
 
 def change_type_number(number_from_to=None):
     return float if number_from_to is None else number_from_to
 
 
 class Current(object):
```

