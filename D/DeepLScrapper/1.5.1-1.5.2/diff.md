# Comparing `tmp/DeepLScrapper-1.5.1.tar.gz` & `tmp/DeepLScrapper-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLScrapper-1.5.1.tar", last modified: Thu Jul 27 21:31:53 2023, max compression
+gzip compressed data, was "DeepLScrapper-1.5.2.tar", last modified: Thu Jul 27 21:47:44 2023, max compression
```

## Comparing `DeepLScrapper-1.5.1.tar` & `DeepLScrapper-1.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:31:53.497217 DeepLScrapper-1.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:31:53.493216 DeepLScrapper-1.5.1/DeepLScrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 21:31:44.000000 DeepLScrapper-1.5.1/DeepLScrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-27 21:31:44.000000 DeepLScrapper-1.5.1/DeepLScrapper/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:31:53.497217 DeepLScrapper-1.5.1/DeepLScrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-27 21:31:53.000000 DeepLScrapper-1.5.1/DeepLScrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 21:31:53.000000 DeepLScrapper-1.5.1/DeepLScrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:31:53.000000 DeepLScrapper-1.5.1/DeepLScrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-27 21:31:53.000000 DeepLScrapper-1.5.1/DeepLScrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 21:31:53.000000 DeepLScrapper-1.5.1/DeepLScrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 21:31:44.000000 DeepLScrapper-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-27 21:31:53.497217 DeepLScrapper-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-27 21:31:44.000000 DeepLScrapper-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:31:53.497217 DeepLScrapper-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-27 21:31:44.000000 DeepLScrapper-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:47:44.706074 DeepLScrapper-1.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:47:44.706074 DeepLScrapper-1.5.2/DeepLScrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 21:47:36.000000 DeepLScrapper-1.5.2/DeepLScrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-27 21:47:36.000000 DeepLScrapper-1.5.2/DeepLScrapper/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:47:44.706074 DeepLScrapper-1.5.2/DeepLScrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-27 21:47:44.000000 DeepLScrapper-1.5.2/DeepLScrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-27 21:47:44.000000 DeepLScrapper-1.5.2/DeepLScrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:47:44.000000 DeepLScrapper-1.5.2/DeepLScrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-27 21:47:44.000000 DeepLScrapper-1.5.2/DeepLScrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 21:47:44.000000 DeepLScrapper-1.5.2/DeepLScrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 21:47:36.000000 DeepLScrapper-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-27 21:47:44.706074 DeepLScrapper-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-27 21:47:36.000000 DeepLScrapper-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:47:44.706074 DeepLScrapper-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-27 21:47:36.000000 DeepLScrapper-1.5.2/setup.py
```

### Comparing `DeepLScrapper-1.5.1/DeepLScrapper/translator.py` & `DeepLScrapper-1.5.2/DeepLScrapper/translator.py`

 * *Files identical despite different names*

### Comparing `DeepLScrapper-1.5.1/DeepLScrapper.egg-info/PKG-INFO` & `DeepLScrapper-1.5.2/DeepLScrapper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepLScrapper
-Version: 1.5.1
+Version: 1.5.2
 Summary: An unofficial Python library for translating text using DeepL
 Author: Olger Chotza
 Author-email: olgerdev@icloud.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -99,18 +99,22 @@
 ## Dependencies
 
 - Selenium
 - BeautifulSoup4
 
 ## Version History
 
-- 1.4.0
-    - Fixed issue with using the library in a multithreading environment
-- 1.3.0
+
+- 1.5.[0-2]
+    - Restructured the project
+    - Fixed the issue to using the library
+    - Updated the documentation regarding the changes
+- 1.[3-5].0
     - Initial release
+    - Fixed issue with using the library in a multithreading environment
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## Disclaimer
```

### Comparing `DeepLScrapper-1.5.1/LICENSE` & `DeepLScrapper-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepLScrapper-1.5.1/PKG-INFO` & `DeepLScrapper-1.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepLScrapper
-Version: 1.5.1
+Version: 1.5.2
 Summary: An unofficial Python library for translating text using DeepL
 Author: Olger Chotza
 Author-email: olgerdev@icloud.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -99,18 +99,22 @@
 ## Dependencies
 
 - Selenium
 - BeautifulSoup4
 
 ## Version History
 
-- 1.4.0
-    - Fixed issue with using the library in a multithreading environment
-- 1.3.0
+
+- 1.5.[0-2]
+    - Restructured the project
+    - Fixed the issue to using the library
+    - Updated the documentation regarding the changes
+- 1.[3-5].0
     - Initial release
+    - Fixed issue with using the library in a multithreading environment
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## Disclaimer
```

### Comparing `DeepLScrapper-1.5.1/README.md` & `DeepLScrapper-1.5.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -82,18 +82,22 @@
 ## Dependencies
 
 - Selenium
 - BeautifulSoup4
 
 ## Version History
 
-- 1.4.0
-    - Fixed issue with using the library in a multithreading environment
-- 1.3.0
+
+- 1.5.[0-2]
+    - Restructured the project
+    - Fixed the issue to using the library
+    - Updated the documentation regarding the changes
+- 1.[3-5].0
     - Initial release
+    - Fixed issue with using the library in a multithreading environment
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## Disclaimer
```

### Comparing `DeepLScrapper-1.5.1/setup.py` & `DeepLScrapper-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DeepLScrapper',
-    version='1.5.1',
+    version='1.5.2',
     description='An unofficial Python library for translating text using DeepL',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Olger Chotza',
     author_email='olgerdev@icloud.com',
     packages=find_packages(),
     install_requires=[
```

