# Comparing `tmp/amazon_scrape-0.0.8.tar.gz` & `tmp/amazon_scrape-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_scrape-0.0.8.tar", last modified: Thu Jul 27 14:11:42 2023, max compression
+gzip compressed data, was "dist/amazon_scrape-0.0.9.tar", last modified: Thu Jul 27 14:14:48 2023, max compression
```

## Comparing `amazon_scrape-0.0.8.tar` & `amazon_scrape-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:11:42.179571 amazon_scrape-0.0.8/
--rw-r--r--   0 finn       (501) staff       (20)     4928 2023-07-27 14:11:42.179817 amazon_scrape-0.0.8/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2242 2023-07-27 14:10:57.000000 amazon_scrape-0.0.8/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:11:42.177038 amazon_scrape-0.0.8/amazon_scrape.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     4928 2023-07-27 14:11:42.000000 amazon_scrape-0.0.8/amazon_scrape.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-27 14:11:42.000000 amazon_scrape-0.0.8/amazon_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 14:11:42.000000 amazon_scrape-0.0.8/amazon_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-27 14:11:42.000000 amazon_scrape-0.0.8/amazon_scrape.egg-info/entry_points.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 13:53:21.000000 amazon_scrape-0.0.8/amazon_scrape.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 14:11:42.000000 amazon_scrape-0.0.8/amazon_scrape.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 14:11:42.000000 amazon_scrape-0.0.8/amazon_scrape.egg-info/top_level.txt
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:11:42.178860 amazon_scrape-0.0.8/amazon_scraper/
--rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 13:52:23.000000 amazon_scrape-0.0.8/amazon_scraper/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     6832 2023-07-27 13:52:23.000000 amazon_scrape-0.0.8/amazon_scraper/scraper.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 14:11:29.000000 amazon_scrape-0.0.8/amazon_scraper/version.py
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 14:11:42.180427 amazon_scrape-0.0.8/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2726 2023-07-27 14:11:29.000000 amazon_scrape-0.0.8/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:14:48.885316 amazon_scrape-0.0.9/
+-rw-r--r--   0 finn       (501) staff       (20)     4966 2023-07-27 14:14:48.885519 amazon_scrape-0.0.9/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2242 2023-07-27 14:10:57.000000 amazon_scrape-0.0.9/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:14:48.883479 amazon_scrape-0.0.9/amazon_scrape.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     4966 2023-07-27 14:14:48.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-27 14:14:48.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 14:14:48.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-27 14:14:48.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/entry_points.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 13:53:21.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 14:14:48.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 14:14:48.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/top_level.txt
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:14:48.884919 amazon_scrape-0.0.9/amazon_scraper/
+-rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 13:52:23.000000 amazon_scrape-0.0.9/amazon_scraper/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     6832 2023-07-27 13:52:23.000000 amazon_scrape-0.0.9/amazon_scraper/scraper.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 14:14:45.000000 amazon_scrape-0.0.9/amazon_scraper/version.py
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 14:14:48.885964 amazon_scrape-0.0.9/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2764 2023-07-27 14:14:45.000000 amazon_scrape-0.0.9/setup.py
```

### Comparing `amazon_scrape-0.0.8/PKG-INFO` & `amazon_scrape-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: amazon_scrape
-Version: 0.0.8
-Summary: Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
+Version: 0.0.9
+Summary: Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, Rating Count, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/0xnu/amazonproducts/blob/main/README.md
```

### Comparing `amazon_scrape-0.0.8/README.md` & `amazon_scrape-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `amazon_scrape-0.0.8/amazon_scrape.egg-info/PKG-INFO` & `amazon_scrape-0.0.9/amazon_scrape.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: amazon-scrape
-Version: 0.0.8
-Summary: Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
+Version: 0.0.9
+Summary: Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, Rating Count, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/0xnu/amazonproducts/blob/main/README.md
```

### Comparing `amazon_scrape-0.0.8/amazon_scraper/scraper.py` & `amazon_scrape-0.0.9/amazon_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `amazon_scrape-0.0.8/setup.py` & `amazon_scrape-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "amazon_scrape"
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 REQUIRES = ["beautifulsoup4", "requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
@@ -19,15 +19,15 @@
     macros.append(('PLATFORM_BSD', '1'))
 elif 'linux' in sys.platform:
     macros.append(('_GNU_SOURCE', ''))
 
 setup(
     name=NAME,
     version=VERSION,
-    description="Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.",
+    description="Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, Rating Count, and Price.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Finbarrs Oketunji",
     author_email="f@finbarrs.eu",
     url="https://finbarrs.eu",
     packages=find_packages(),
     include_package_data=True,
```

