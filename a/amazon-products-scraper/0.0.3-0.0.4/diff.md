# Comparing `tmp/amazon_products_scraper-0.0.3.tar.gz` & `tmp/amazon_products_scraper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_products_scraper-0.0.3.tar", last modified: Thu Jul 27 09:27:04 2023, max compression
+gzip compressed data, was "dist/amazon_products_scraper-0.0.4.tar", last modified: Thu Jul 27 09:31:45 2023, max compression
```

## Comparing `amazon_products_scraper-0.0.3.tar` & `amazon_products_scraper-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:27:04.404043 amazon_products_scraper-0.0.3/
--rw-r--r--   0 finn       (501) staff       (20)     4230 2023-07-27 09:27:04.404427 amazon_products_scraper-0.0.3/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     1599 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.3/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:27:04.398838 amazon_products_scraper-0.0.3/amazon_products_scraper.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     4230 2023-07-27 09:27:04.000000 amazon_products_scraper-0.0.3/amazon_products_scraper.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      387 2023-07-27 09:27:04.000000 amazon_products_scraper-0.0.3/amazon_products_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:27:04.000000 amazon_products_scraper-0.0.3/amazon_products_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.3/amazon_products_scraper.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 09:27:04.000000 amazon_products_scraper-0.0.3/amazon_products_scraper.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 09:27:04.000000 amazon_products_scraper-0.0.3/amazon_products_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:27:04.402920 amazon_products_scraper-0.0.3/amazon_scraper/
--rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.3/amazon_scraper/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     5856 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.3/amazon_scraper/scraper.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 09:26:43.000000 amazon_products_scraper-0.0.3/amazon_scraper/version.py
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 09:27:04.405394 amazon_products_scraper-0.0.3/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2605 2023-07-27 09:26:54.000000 amazon_products_scraper-0.0.3/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:31:45.492697 amazon_products_scraper-0.0.4/
+-rw-r--r--   0 finn       (501) staff       (20)     4230 2023-07-27 09:31:45.493022 amazon_products_scraper-0.0.4/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     1599 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.4/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:31:45.489841 amazon_products_scraper-0.0.4/amazon_products_scraper.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     4230 2023-07-27 09:31:45.000000 amazon_products_scraper-0.0.4/amazon_products_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      437 2023-07-27 09:31:45.000000 amazon_products_scraper-0.0.4/amazon_products_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:31:45.000000 amazon_products_scraper-0.0.4/amazon_products_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-27 09:31:45.000000 amazon_products_scraper-0.0.4/amazon_products_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.4/amazon_products_scraper.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 09:31:45.000000 amazon_products_scraper-0.0.4/amazon_products_scraper.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 09:31:45.000000 amazon_products_scraper-0.0.4/amazon_products_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:31:45.491901 amazon_products_scraper-0.0.4/amazon_scraper/
+-rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.4/amazon_scraper/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     5856 2023-07-27 09:15:43.000000 amazon_products_scraper-0.0.4/amazon_scraper/scraper.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 09:28:21.000000 amazon_products_scraper-0.0.4/amazon_scraper/version.py
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 09:31:45.493684 amazon_products_scraper-0.0.4/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2734 2023-07-27 09:31:43.000000 amazon_products_scraper-0.0.4/setup.py
```

### Comparing `amazon_products_scraper-0.0.3/PKG-INFO` & `amazon_products_scraper-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_products_scraper
-Version: 0.0.3
+Version: 0.0.4
 Summary: Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
```

### Comparing `amazon_products_scraper-0.0.3/README.md` & `amazon_products_scraper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `amazon_products_scraper-0.0.3/amazon_products_scraper.egg-info/PKG-INFO` & `amazon_products_scraper-0.0.4/amazon_products_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-products-scraper
-Version: 0.0.3
+Version: 0.0.4
 Summary: Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
```

### Comparing `amazon_products_scraper-0.0.3/amazon_scraper/scraper.py` & `amazon_products_scraper-0.0.4/amazon_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `amazon_products_scraper-0.0.3/setup.py` & `amazon_products_scraper-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "amazon_products_scraper"
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 REQUIRES = ["beautifulsoup4", "requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
@@ -30,14 +30,19 @@
     author_email="f@finbarrs.eu",
     url="https://finbarrs.eu",
     packages=find_packages(),
     include_package_data=True,
     install_requires=REQUIRES,
     zip_safe=False,
     python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*",
+    entry_points={
+        'console_scripts': [
+            'amazon_scraper=amazon_scraper.scraper:main',
+        ],
+    },
     project_urls={
         "Bug Tracker": "https://github.com/0xnu/amazonproducts/issues",
         "Changes": "https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md",
         "Documentation": "https://github.com/0xnu/amazonproducts/blob/main/README.md",
         "Source Code": "https://github.com/0xnu/amazonproducts",
     },
     classifiers=[
```

