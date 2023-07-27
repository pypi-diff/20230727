# Comparing `tmp/amazon_scrape-0.0.3.tar.gz` & `tmp/amazon_scrape-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_scrape-0.0.3.tar", last modified: Thu Jul 27 09:49:59 2023, max compression
+gzip compressed data, was "dist/amazon_scrape-0.0.4.tar", last modified: Thu Jul 27 10:15:08 2023, max compression
```

## Comparing `amazon_scrape-0.0.3.tar` & `amazon_scrape-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:49:59.423415 amazon_scrape-0.0.3/
--rw-r--r--   0 finn       (501) staff       (20)     4164 2023-07-27 09:49:59.423815 amazon_scrape-0.0.3/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     1543 2023-07-27 09:49:01.000000 amazon_scrape-0.0.3/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:49:59.418537 amazon_scrape-0.0.3/amazon_scrape.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     4164 2023-07-27 09:49:59.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-27 09:49:59.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:49:59.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-27 09:49:59.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/entry_points.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:43:05.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 09:49:59.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 09:49:59.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/top_level.txt
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:49:59.422122 amazon_scrape-0.0.3/amazon_scraper/
--rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 09:15:43.000000 amazon_scrape-0.0.3/amazon_scraper/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     5856 2023-07-27 09:15:43.000000 amazon_scrape-0.0.3/amazon_scraper/scraper.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 09:48:22.000000 amazon_scrape-0.0.3/amazon_scraper/version.py
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 09:49:59.424879 amazon_scrape-0.0.3/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2726 2023-07-27 09:48:22.000000 amazon_scrape-0.0.3/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 10:15:08.274536 amazon_scrape-0.0.4/
+-rw-r--r--   0 finn       (501) staff       (20)     4134 2023-07-27 10:15:08.275013 amazon_scrape-0.0.4/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     1543 2023-07-27 10:12:58.000000 amazon_scrape-0.0.4/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 10:15:08.267935 amazon_scrape-0.0.4/amazon_scrape.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     4134 2023-07-27 10:15:08.000000 amazon_scrape-0.0.4/amazon_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-27 10:15:08.000000 amazon_scrape-0.0.4/amazon_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 10:15:08.000000 amazon_scrape-0.0.4/amazon_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-27 10:15:08.000000 amazon_scrape-0.0.4/amazon_scrape.egg-info/entry_points.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 10:13:49.000000 amazon_scrape-0.0.4/amazon_scrape.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 10:15:08.000000 amazon_scrape-0.0.4/amazon_scrape.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 10:15:08.000000 amazon_scrape-0.0.4/amazon_scrape.egg-info/top_level.txt
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 10:15:08.273508 amazon_scrape-0.0.4/amazon_scraper/
+-rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 10:12:58.000000 amazon_scrape-0.0.4/amazon_scraper/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     5856 2023-07-27 10:12:58.000000 amazon_scrape-0.0.4/amazon_scraper/scraper.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 10:12:58.000000 amazon_scrape-0.0.4/amazon_scraper/version.py
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 10:15:08.276533 amazon_scrape-0.0.4/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2726 2023-07-27 10:12:58.000000 amazon_scrape-0.0.4/setup.py
```

### Comparing `amazon_scrape-0.0.3/PKG-INFO` & `amazon_scrape-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: amazon_scrape
-Version: 0.0.3
+Version: 0.0.4
 Summary: Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/0xnu/amazonproducts/blob/main/README.md
 Project-URL: Source Code, https://github.com/0xnu/amazonproducts
 Description: Amazon Products Scraper
         =======================
         
-        .. image:: https://badge.fury.io/py/amazon_products_scraper.svg
-            :target: https://badge.fury.io/py/amazon_products_scraper
-            :alt: amazon_products_scraper Python Package Version
+        .. image:: https://badge.fury.io/py/amazon-scrape.svg
+            :target: https://badge.fury.io/py/amazon-scrape
+            :alt: amazon-scrape Python Package Version
         
         Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
         
         Requirements
         ------------
         
         Python 2.7 and later.
```

### Comparing `amazon_scrape-0.0.3/README.md` & `amazon_scrape-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `amazon_scrape-0.0.3/amazon_scrape.egg-info/PKG-INFO` & `amazon_scrape-0.0.4/amazon_scrape.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: amazon-scrape
-Version: 0.0.3
+Version: 0.0.4
 Summary: Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/0xnu/amazonproducts/blob/main/README.md
 Project-URL: Source Code, https://github.com/0xnu/amazonproducts
 Description: Amazon Products Scraper
         =======================
         
-        .. image:: https://badge.fury.io/py/amazon_products_scraper.svg
-            :target: https://badge.fury.io/py/amazon_products_scraper
-            :alt: amazon_products_scraper Python Package Version
+        .. image:: https://badge.fury.io/py/amazon-scrape.svg
+            :target: https://badge.fury.io/py/amazon-scrape
+            :alt: amazon-scrape Python Package Version
         
         Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
         
         Requirements
         ------------
         
         Python 2.7 and later.
```

### Comparing `amazon_scrape-0.0.3/amazon_scraper/scraper.py` & `amazon_scrape-0.0.4/amazon_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `amazon_scrape-0.0.3/setup.py` & `amazon_scrape-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "amazon_scrape"
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 REQUIRES = ["beautifulsoup4", "requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

