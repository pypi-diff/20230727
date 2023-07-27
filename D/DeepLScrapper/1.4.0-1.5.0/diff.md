# Comparing `tmp/DeepLScrapper-1.4.0.tar.gz` & `tmp/DeepLScrapper-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLScrapper-1.4.0.tar", last modified: Thu Jul 27 21:07:19 2023, max compression
+gzip compressed data, was "DeepLScrapper-1.5.0.tar", last modified: Thu Jul 27 21:24:32 2023, max compression
```

## Comparing `DeepLScrapper-1.4.0.tar` & `DeepLScrapper-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:07:19.762053 DeepLScrapper-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:07:19.758053 DeepLScrapper-1.4.0/DeepLScrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-27 21:07:19.000000 DeepLScrapper-1.4.0/DeepLScrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 21:07:19.000000 DeepLScrapper-1.4.0/DeepLScrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:07:19.000000 DeepLScrapper-1.4.0/DeepLScrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 21:07:19.000000 DeepLScrapper-1.4.0/DeepLScrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:07:19.000000 DeepLScrapper-1.4.0/DeepLScrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 21:07:11.000000 DeepLScrapper-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-27 21:07:19.762053 DeepLScrapper-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-27 21:07:11.000000 DeepLScrapper-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:07:19.762053 DeepLScrapper-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 21:07:11.000000 DeepLScrapper-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:24:32.267079 DeepLScrapper-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:24:32.263079 DeepLScrapper-1.5.0/DeepLScrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 21:24:25.000000 DeepLScrapper-1.5.0/DeepLScrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-27 21:24:25.000000 DeepLScrapper-1.5.0/DeepLScrapper/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:24:32.267079 DeepLScrapper-1.5.0/DeepLScrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-27 21:24:32.000000 DeepLScrapper-1.5.0/DeepLScrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 21:24:32.000000 DeepLScrapper-1.5.0/DeepLScrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:24:32.000000 DeepLScrapper-1.5.0/DeepLScrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 21:24:32.000000 DeepLScrapper-1.5.0/DeepLScrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 21:24:32.000000 DeepLScrapper-1.5.0/DeepLScrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 21:24:25.000000 DeepLScrapper-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-27 21:24:32.267079 DeepLScrapper-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-27 21:24:25.000000 DeepLScrapper-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:24:32.267079 DeepLScrapper-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 21:24:25.000000 DeepLScrapper-1.5.0/setup.py
```

### Comparing `DeepLScrapper-1.4.0/DeepLScrapper.egg-info/PKG-INFO` & `DeepLScrapper-1.5.0/DeepLScrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepLScrapper
-Version: 1.4.0
+Version: 1.5.0
 Summary: An unofficial Python library for translating text using DeepL
 Author: Olger Chotza
 Author-email: olgerdev@icloud.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `DeepLScrapper-1.4.0/LICENSE` & `DeepLScrapper-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepLScrapper-1.4.0/PKG-INFO` & `DeepLScrapper-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepLScrapper
-Version: 1.4.0
+Version: 1.5.0
 Summary: An unofficial Python library for translating text using DeepL
 Author: Olger Chotza
 Author-email: olgerdev@icloud.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `DeepLScrapper-1.4.0/README.md` & `DeepLScrapper-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `DeepLScrapper-1.4.0/setup.py` & `DeepLScrapper-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DeepLScrapper',
-    version='1.4.0',
+    version='1.5.0',
     description='An unofficial Python library for translating text using DeepL',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Olger Chotza',
     author_email='olgerdev@icloud.com',
     packages=find_packages(),
     install_requires=[
```

