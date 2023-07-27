# Comparing `tmp/DeepLScrapper-1.3.0.tar.gz` & `tmp/DeepLScrapper-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLScrapper-1.3.0.tar", last modified: Thu Jul 27 20:46:52 2023, max compression
+gzip compressed data, was "DeepLScrapper-1.4.0.tar", last modified: Thu Jul 27 21:07:19 2023, max compression
```

## Comparing `DeepLScrapper-1.3.0.tar` & `DeepLScrapper-1.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:46:52.189229 DeepLScrapper-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:46:52.185229 DeepLScrapper-1.3.0/DeepLScrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-27 20:46:52.000000 DeepLScrapper-1.3.0/DeepLScrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 20:46:52.000000 DeepLScrapper-1.3.0/DeepLScrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:46:52.000000 DeepLScrapper-1.3.0/DeepLScrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 20:46:52.000000 DeepLScrapper-1.3.0/DeepLScrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:46:52.000000 DeepLScrapper-1.3.0/DeepLScrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 20:46:41.000000 DeepLScrapper-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-27 20:46:52.185229 DeepLScrapper-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-27 20:46:41.000000 DeepLScrapper-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:46:52.189229 DeepLScrapper-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 20:46:41.000000 DeepLScrapper-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:07:19.762053 DeepLScrapper-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:07:19.758053 DeepLScrapper-1.4.0/DeepLScrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-27 21:07:19.000000 DeepLScrapper-1.4.0/DeepLScrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 21:07:19.000000 DeepLScrapper-1.4.0/DeepLScrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:07:19.000000 DeepLScrapper-1.4.0/DeepLScrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 21:07:19.000000 DeepLScrapper-1.4.0/DeepLScrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:07:19.000000 DeepLScrapper-1.4.0/DeepLScrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 21:07:11.000000 DeepLScrapper-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-27 21:07:19.762053 DeepLScrapper-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-27 21:07:11.000000 DeepLScrapper-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:07:19.762053 DeepLScrapper-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 21:07:11.000000 DeepLScrapper-1.4.0/setup.py
```

### Comparing `DeepLScrapper-1.3.0/DeepLScrapper.egg-info/PKG-INFO` & `DeepLScrapper-1.4.0/DeepLScrapper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepLScrapper
-Version: 1.3.0
+Version: 1.4.0
 Summary: An unofficial Python library for translating text using DeepL
 Author: Olger Chotza
 Author-email: olgerdev@icloud.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -97,14 +97,21 @@
 ```
 
 ## Dependencies
 
 - Selenium
 - BeautifulSoup4
 
+## Version History
+
+- 1.4.0
+    - Fixed issue with using the library in a multithreading environment
+- 1.3.0
+    - Initial release
+
 ## License
 
 This project is licensed under the MIT License.
 
 ## Disclaimer
 
 This project is not affiliated, associated, authorized, endorsed by, or in any way officially connected with DeepL, or any of its subsidiaries or its affiliates. The official DeepL website can be found at https://www.deepl.com/.
```

### Comparing `DeepLScrapper-1.3.0/LICENSE` & `DeepLScrapper-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepLScrapper-1.3.0/PKG-INFO` & `DeepLScrapper-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepLScrapper
-Version: 1.3.0
+Version: 1.4.0
 Summary: An unofficial Python library for translating text using DeepL
 Author: Olger Chotza
 Author-email: olgerdev@icloud.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -97,14 +97,21 @@
 ```
 
 ## Dependencies
 
 - Selenium
 - BeautifulSoup4
 
+## Version History
+
+- 1.4.0
+    - Fixed issue with using the library in a multithreading environment
+- 1.3.0
+    - Initial release
+
 ## License
 
 This project is licensed under the MIT License.
 
 ## Disclaimer
 
 This project is not affiliated, associated, authorized, endorsed by, or in any way officially connected with DeepL, or any of its subsidiaries or its affiliates. The official DeepL website can be found at https://www.deepl.com/.
```

### Comparing `DeepLScrapper-1.3.0/README.md` & `DeepLScrapper-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,21 @@
 ```
 
 ## Dependencies
 
 - Selenium
 - BeautifulSoup4
 
+## Version History
+
+- 1.4.0
+    - Fixed issue with using the library in a multithreading environment
+- 1.3.0
+    - Initial release
+
 ## License
 
 This project is licensed under the MIT License.
 
 ## Disclaimer
 
 This project is not affiliated, associated, authorized, endorsed by, or in any way officially connected with DeepL, or any of its subsidiaries or its affiliates. The official DeepL website can be found at https://www.deepl.com/.
```

### Comparing `DeepLScrapper-1.3.0/setup.py` & `DeepLScrapper-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DeepLScrapper',
-    version='1.3.0',
+    version='1.4.0',
     description='An unofficial Python library for translating text using DeepL',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Olger Chotza',
     author_email='olgerdev@icloud.com',
     packages=find_packages(),
     install_requires=[
```

