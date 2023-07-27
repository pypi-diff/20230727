# Comparing `tmp/amazon_scrape-0.0.2.tar.gz` & `tmp/amazon_scrape-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_scrape-0.0.2.tar", last modified: Thu Jul 27 09:45:29 2023, max compression
+gzip compressed data, was "dist/amazon_scrape-0.0.3.tar", last modified: Thu Jul 27 09:49:59 2023, max compression
```

## Comparing `amazon_scrape-0.0.2.tar` & `amazon_scrape-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:45:29.484684 amazon_scrape-0.0.2/
--rw-r--r--   0 finn       (501) staff       (20)     4220 2023-07-27 09:45:29.485253 amazon_scrape-0.0.2/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     1599 2023-07-27 09:15:43.000000 amazon_scrape-0.0.2/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:45:29.480185 amazon_scrape-0.0.2/amazon_scrape.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     4220 2023-07-27 09:45:29.000000 amazon_scrape-0.0.2/amazon_scrape.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-27 09:45:29.000000 amazon_scrape-0.0.2/amazon_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:45:29.000000 amazon_scrape-0.0.2/amazon_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-27 09:45:29.000000 amazon_scrape-0.0.2/amazon_scrape.egg-info/entry_points.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:43:05.000000 amazon_scrape-0.0.2/amazon_scrape.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 09:45:29.000000 amazon_scrape-0.0.2/amazon_scrape.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 09:45:29.000000 amazon_scrape-0.0.2/amazon_scrape.egg-info/top_level.txt
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:45:29.483556 amazon_scrape-0.0.2/amazon_scraper/
--rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 09:15:43.000000 amazon_scrape-0.0.2/amazon_scraper/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     5856 2023-07-27 09:15:43.000000 amazon_scrape-0.0.2/amazon_scraper/scraper.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 09:45:25.000000 amazon_scrape-0.0.2/amazon_scraper/version.py
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 09:45:29.486943 amazon_scrape-0.0.2/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2726 2023-07-27 09:45:25.000000 amazon_scrape-0.0.2/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:49:59.423415 amazon_scrape-0.0.3/
+-rw-r--r--   0 finn       (501) staff       (20)     4164 2023-07-27 09:49:59.423815 amazon_scrape-0.0.3/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     1543 2023-07-27 09:49:01.000000 amazon_scrape-0.0.3/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:49:59.418537 amazon_scrape-0.0.3/amazon_scrape.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     4164 2023-07-27 09:49:59.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-27 09:49:59.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:49:59.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-27 09:49:59.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/entry_points.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 09:43:05.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 09:49:59.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 09:49:59.000000 amazon_scrape-0.0.3/amazon_scrape.egg-info/top_level.txt
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 09:49:59.422122 amazon_scrape-0.0.3/amazon_scraper/
+-rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 09:15:43.000000 amazon_scrape-0.0.3/amazon_scraper/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     5856 2023-07-27 09:15:43.000000 amazon_scrape-0.0.3/amazon_scraper/scraper.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 09:48:22.000000 amazon_scrape-0.0.3/amazon_scraper/version.py
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 09:49:59.424879 amazon_scrape-0.0.3/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2726 2023-07-27 09:48:22.000000 amazon_scrape-0.0.3/setup.py
```

### Comparing `amazon_scrape-0.0.2/PKG-INFO` & `amazon_scrape-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_scrape
-Version: 0.0.2
+Version: 0.0.3
 Summary: Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
@@ -28,39 +28,39 @@
         Setup
         -----
         
         You can install this package by using the pip tool and installing:
         
         .. code-block:: bash
         
-        	$ pip install amazon_products_scraper
+        	$ pip install amazon-scrape
         
         Or:
         
         .. code-block:: bash
         
-        	$ easy_install amazon_products_scraper
+        	$ easy_install amazon-scrape
         
         
         Usage Example
         -------------
         
         .. code-block:: python
         
             ## Specify locale, keywords, API key, and number of pages to scrape
-            amazon_products_scraper --locale com --keywords "laptop" --proxy_api_key "your_api_key" --pages 10
+            amazon_scraper --locale com --keywords "laptop" --proxy_api_key "your_api_key" --pages 10
         
             ## Specify only keywords and API key (will default to "co.uk" locale and 20 pages):
-            amazon_products_scraper --keywords "iphone" --proxy_api_key "your_api_key"
+            amazon_scraper --keywords "iphone" --proxy_api_key "your_api_key"
         
             ## Specify a direct Amazon URL and API key (will default to "co.uk" locale and 20 pages):
-            amazon_products_scraper --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
+            amazon_scraper --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
         
             ## Specify locale and Amazon URL (will default to 20 pages):
-            amazon_products_scraper --locale de --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
+            amazon_scraper --locale de --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
         
         
         Create Scraper API Account
         --------------------------
         
         Sign up for a Scraper API `user account`_.
```

### Comparing `amazon_scrape-0.0.2/README.md` & `amazon_scrape-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 Python 2.7 and later.
 
 ## Setup
 
 You can install this package by using the pip tool and installing:
 
 ```python
-pip install amazon_products_scraper
+pip install amazon-scrape
 ## OR
-easy_install amazon_products_scraper
+easy_install amazon-scrape
 ```
 
 Install from source with:
 
 ```python
 python setup.py install --user
 
 ## or `sudo python setup.py install` to install the package for all users
 ```
 
 ## Usage Example
 
 ```python
 # Specify locale, keywords, API key, and number of pages to scrape
-amazon_products_scraper --locale com --keywords "laptop" --proxy_api_key "your_api_key" --pages 10
+amazon_scraper --locale com --keywords "laptop" --proxy_api_key "your_api_key" --pages 10
 
 ## Specify only keywords and API key (will default to "co.uk" locale and 20 pages):
-amazon_products_scraper --keywords "iphone" --proxy_api_key "your_api_key"
+amazon_scraper --keywords "iphone" --proxy_api_key "your_api_key"
 
 ## Specify a direct Amazon URL and API key (will default to "co.uk" locale and 20 pages):
-amazon_products_scraper --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
+amazon_scraper --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
 
 ## Specify locale and Amazon URL (will default to 20 pages):
-amazon_products_scraper --locale de --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
+amazon_scraper --locale de --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
 ```
 
 ## Create Scraper API Account
 
 Sign up for a Scraper API [user account](https://www.scraperapi.com/?fp_ref=finbarrs11).
```

### Comparing `amazon_scrape-0.0.2/amazon_scrape.egg-info/PKG-INFO` & `amazon_scrape-0.0.3/amazon_scrape.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-scrape
-Version: 0.0.2
+Version: 0.0.3
 Summary: Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
@@ -28,39 +28,39 @@
         Setup
         -----
         
         You can install this package by using the pip tool and installing:
         
         .. code-block:: bash
         
-        	$ pip install amazon_products_scraper
+        	$ pip install amazon-scrape
         
         Or:
         
         .. code-block:: bash
         
-        	$ easy_install amazon_products_scraper
+        	$ easy_install amazon-scrape
         
         
         Usage Example
         -------------
         
         .. code-block:: python
         
             ## Specify locale, keywords, API key, and number of pages to scrape
-            amazon_products_scraper --locale com --keywords "laptop" --proxy_api_key "your_api_key" --pages 10
+            amazon_scraper --locale com --keywords "laptop" --proxy_api_key "your_api_key" --pages 10
         
             ## Specify only keywords and API key (will default to "co.uk" locale and 20 pages):
-            amazon_products_scraper --keywords "iphone" --proxy_api_key "your_api_key"
+            amazon_scraper --keywords "iphone" --proxy_api_key "your_api_key"
         
             ## Specify a direct Amazon URL and API key (will default to "co.uk" locale and 20 pages):
-            amazon_products_scraper --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
+            amazon_scraper --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
         
             ## Specify locale and Amazon URL (will default to 20 pages):
-            amazon_products_scraper --locale de --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
+            amazon_scraper --locale de --url "https://www.amazon.de/s?k=iphone&crid=1OHYY6U6OGCK5&sprefix=ipho%2Caps%2C335&ref=nb_sb_noss_2" --proxy_api_key "your_api_key"
         
         
         Create Scraper API Account
         --------------------------
         
         Sign up for a Scraper API `user account`_.
```

### Comparing `amazon_scrape-0.0.2/amazon_scraper/scraper.py` & `amazon_scrape-0.0.3/amazon_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `amazon_scrape-0.0.2/setup.py` & `amazon_scrape-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "amazon_scrape"
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 REQUIRES = ["beautifulsoup4", "requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

