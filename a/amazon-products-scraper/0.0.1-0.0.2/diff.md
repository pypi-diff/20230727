# Comparing `tmp/amazon_products_scraper-0.0.1.tar.gz` & `tmp/amazon_products_scraper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_products_scraper-0.0.1.tar", last modified: Thu Jul 27 09:18:07 2023, max compression
+gzip compressed data, was "dist/amazon_products_scraper-0.0.2.tar", last modified: Thu Jul 27 09:21:55 2023, max compression
```

## Comparing `amazon_products_scraper-0.0.1.tar` & `amazon_products_scraper-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:18:07.837921 amazon_products_scraper-0.0.1/
--rw-r--r--   0 finn       (501) staff       (20)     4230 2023-07-27 09:18:07.838123 amazon_products_scraper-0.0.1/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     1599 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.1/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:18:07.835577 amazon_products_scraper-0.0.1/amazon_products_scraper.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     4230 2023-07-27 09:18:07.000000 amazon_products_scraper-0.0.1/amazon_products_scraper.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      437 2023-07-27 09:18:07.000000 amazon_products_scraper-0.0.1/amazon_products_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:18:07.000000 amazon_products_scraper-0.0.1/amazon_products_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)       79 2023-07-27 09:18:07.000000 amazon_products_scraper-0.0.1/amazon_products_scraper.egg-info/entry_points.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.1/amazon_products_scraper.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 09:18:07.000000 amazon_products_scraper-0.0.1/amazon_products_scraper.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 09:18:07.000000 amazon_products_scraper-0.0.1/amazon_products_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:18:07.837316 amazon_products_scraper-0.0.1/amazon_scraper/
--rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.1/amazon_scraper/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     5856 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.1/amazon_scraper/scraper.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.1/amazon_scraper/version.py
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 09:18:07.838573 amazon_products_scraper-0.0.1/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2751 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.1/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:21:55.400839 amazon_products_scraper-0.0.2/
+-rw-r--r--   0 finn       (501) staff       (20)     4230 2023-07-27 09:21:55.401249 amazon_products_scraper-0.0.2/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     1599 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.2/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:21:55.396217 amazon_products_scraper-0.0.2/amazon_products_scraper.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     4230 2023-07-27 09:21:55.000000 amazon_products_scraper-0.0.2/amazon_products_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      437 2023-07-27 09:21:55.000000 amazon_products_scraper-0.0.2/amazon_products_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:21:55.000000 amazon_products_scraper-0.0.2/amazon_products_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)       70 2023-07-27 09:21:55.000000 amazon_products_scraper-0.0.2/amazon_products_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.2/amazon_products_scraper.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 09:21:55.000000 amazon_products_scraper-0.0.2/amazon_products_scraper.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 09:21:55.000000 amazon_products_scraper-0.0.2/amazon_products_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:21:55.399758 amazon_products_scraper-0.0.2/amazon_scraper/
+-rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.2/amazon_scraper/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     5856 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.2/amazon_scraper/scraper.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 09:20:05.000000 amazon_products_scraper-0.0.2/amazon_scraper/version.py
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 09:21:55.402255 amazon_products_scraper-0.0.2/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2742 2023-07-27 09:21:31.000000 amazon_products_scraper-0.0.2/setup.py
```

### Comparing `amazon_products_scraper-0.0.1/PKG-INFO` & `amazon_products_scraper-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_products_scraper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
```

### Comparing `amazon_products_scraper-0.0.1/README.md` & `amazon_products_scraper-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `amazon_products_scraper-0.0.1/amazon_products_scraper.egg-info/PKG-INFO` & `amazon_products_scraper-0.0.2/amazon_products_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-products-scraper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
```

### Comparing `amazon_products_scraper-0.0.1/amazon_scraper/scraper.py` & `amazon_products_scraper-0.0.2/amazon_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `amazon_products_scraper-0.0.1/setup.py` & `amazon_products_scraper-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "amazon_products_scraper"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 REQUIRES = ["beautifulsoup4", "requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
@@ -32,15 +32,15 @@
     packages=find_packages(),
     include_package_data=True,
     install_requires=REQUIRES,
     zip_safe=False,
     python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*",
     entry_points={
         'console_scripts': [
-            'amazon_scraper = amazon_products_scraper.AmazonScraper:main',
+            'amazon_scraper = amazon_scraper.AmazonScraper:main',
         ],
     },
     project_urls={
         "Bug Tracker": "https://github.com/0xnu/amazonproducts/issues",
         "Changes": "https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md",
         "Documentation": "https://github.com/0xnu/amazonproducts/blob/main/README.md",
         "Source Code": "https://github.com/0xnu/amazonproducts",
```

