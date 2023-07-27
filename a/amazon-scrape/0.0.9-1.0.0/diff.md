# Comparing `tmp/amazon_scrape-0.0.9.tar.gz` & `tmp/amazon_scrape-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_scrape-0.0.9.tar", last modified: Thu Jul 27 14:14:48 2023, max compression
+gzip compressed data, was "dist/amazon_scrape-1.0.0.tar", last modified: Thu Jul 27 14:25:56 2023, max compression
```

## Comparing `amazon_scrape-0.0.9.tar` & `amazon_scrape-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:14:48.885316 amazon_scrape-0.0.9/
--rw-r--r--   0 finn       (501) staff       (20)     4966 2023-07-27 14:14:48.885519 amazon_scrape-0.0.9/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2242 2023-07-27 14:10:57.000000 amazon_scrape-0.0.9/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:14:48.883479 amazon_scrape-0.0.9/amazon_scrape.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     4966 2023-07-27 14:14:48.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-27 14:14:48.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 14:14:48.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-27 14:14:48.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/entry_points.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 13:53:21.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 14:14:48.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 14:14:48.000000 amazon_scrape-0.0.9/amazon_scrape.egg-info/top_level.txt
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:14:48.884919 amazon_scrape-0.0.9/amazon_scraper/
--rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 13:52:23.000000 amazon_scrape-0.0.9/amazon_scraper/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     6832 2023-07-27 13:52:23.000000 amazon_scrape-0.0.9/amazon_scraper/scraper.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 14:14:45.000000 amazon_scrape-0.0.9/amazon_scraper/version.py
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 14:14:48.885964 amazon_scrape-0.0.9/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2764 2023-07-27 14:14:45.000000 amazon_scrape-0.0.9/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:25:56.425020 amazon_scrape-1.0.0/
+-rw-r--r--   0 finn       (501) staff       (20)     4938 2023-07-27 14:25:56.425214 amazon_scrape-1.0.0/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2228 2023-07-27 14:23:23.000000 amazon_scrape-1.0.0/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:25:56.422584 amazon_scrape-1.0.0/amazon_scrape.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     4938 2023-07-27 14:25:56.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-27 14:25:56.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 14:25:56.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-27 14:25:56.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/entry_points.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 13:53:21.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 14:25:56.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 14:25:56.000000 amazon_scrape-1.0.0/amazon_scrape.egg-info/top_level.txt
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 14:25:56.424541 amazon_scrape-1.0.0/amazon_scraper/
+-rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 13:52:23.000000 amazon_scrape-1.0.0/amazon_scraper/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     6484 2023-07-27 14:22:54.000000 amazon_scrape-1.0.0/amazon_scraper/scraper.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 14:25:52.000000 amazon_scrape-1.0.0/amazon_scraper/version.py
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 14:25:56.425928 amazon_scrape-1.0.0/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2750 2023-07-27 14:25:52.000000 amazon_scrape-1.0.0/setup.py
```

### Comparing `amazon_scrape-0.0.9/PKG-INFO` & `amazon_scrape-1.0.0/amazon_scrape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: amazon_scrape
-Version: 0.0.9
-Summary: Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, Rating Count, and Price.
+Name: amazon-scrape
+Version: 1.0.0
+Summary: Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/0xnu/amazonproducts/blob/main/README.md
@@ -13,15 +13,15 @@
 Description: Amazon Products Scraper
         =======================
         
         .. image:: https://badge.fury.io/py/amazon-scrape.svg
             :target: https://badge.fury.io/py/amazon-scrape
             :alt: amazon-scrape Python Package Version
         
-        Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, Rating Count, and Price.
+        Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.
         
         Requirements
         ------------
         
         Python 2.7 and later.
```

### Comparing `amazon_scrape-0.0.9/README.md` & `amazon_scrape-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Amazon Products Scraper
 
 [![PyPI version](https://badge.fury.io/py/amazon-scrape.svg)](https://badge.fury.io/py/amazon-scrape)
 
-Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, Rating Count, and Price.
+Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.
 
 ## Requirements
 
 Python 2.7 and later.
 
 ## Setup
```

### Comparing `amazon_scrape-0.0.9/amazon_scrape.egg-info/PKG-INFO` & `amazon_scrape-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: amazon-scrape
-Version: 0.0.9
-Summary: Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, Rating Count, and Price.
+Name: amazon_scrape
+Version: 1.0.0
+Summary: Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/0xnu/amazonproducts/blob/main/README.md
@@ -13,15 +13,15 @@
 Description: Amazon Products Scraper
         =======================
         
         .. image:: https://badge.fury.io/py/amazon-scrape.svg
             :target: https://badge.fury.io/py/amazon-scrape
             :alt: amazon-scrape Python Package Version
         
-        Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, Rating Count, and Price.
+        Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.
         
         Requirements
         ------------
         
         Python 2.7 and later.
```

### Comparing `amazon_scrape-0.0.9/amazon_scraper/scraper.py` & `amazon_scrape-1.0.0/amazon_scraper/scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.csv_file = open('amazon_products.csv', 'w', newline='')
         self.json_file = open('amazon_products.json', 'w')
         self.writer = csv.writer(self.csv_file)
         self.json_data = []
         self.locale = locale
 
     def start_scraping(self):
-        self.writer.writerow(["product_name", "product_images", "rating_count", "price", "product_url", "number_of_reviews", "asin"])
+        self.writer.writerow(["product_name", "product_images", "price", "product_url", "number_of_reviews", "asin"])
         for page in range(1, self.pages + 1):
             url = self.url + "&page=" + str(page)
             headers = {"User-Agent": random.choice(self.user_agents)}
             response = requests.get(url, headers=headers)
             soup = BeautifulSoup(response.content, "html.parser")
             products = soup.find_all("div", {"class": "sg-col-inner"})
 
@@ -63,21 +63,14 @@
                 # Product images
                 images = product.find_all("img", {"class": "s-image"})
                 if images is not None:
                     images = [image['src'] for image in images]
                 else:
                     images = []
 
-                # Rating count
-                rating_count = product.find("span", {"class": "a-size-base"})
-                if rating_count is not None:
-                    rating_count = rating_count.text
-                else:
-                    rating_count = ''
-
                 # Price
                 price = product.find("span", {"class": "a-offscreen"})
                 if price is not None:
                     price = price.text
                 else:
                     price = ''
 
@@ -95,21 +88,20 @@
                 else:
                     number_of_reviews = ''
 
                 # ASIN
                 asin = product_url.split("/dp/")[1].split("/")[0] if "/dp/" in product_url else ''
 
                 # Write to CSV
-                self.writer.writerow([name, ", ".join(images), rating_count, price, product_url, number_of_reviews, asin])
+                self.writer.writerow([name, ", ".join(images), price, product_url, number_of_reviews, asin])
 
                 # Add to JSON data
                 self.json_data.append({
                     "product_name": name,
                     "product_images": images,
-                    "rating_count": rating_count,
                     "price": price,
                     "product_url": product_url,
                     "number_of_reviews": number_of_reviews,
                     "asin": asin
                 })
 
         json.dump(self.json_data, self.json_file, indent=4)
```

### Comparing `amazon_scrape-0.0.9/setup.py` & `amazon_scrape-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "amazon_scrape"
-VERSION = "0.0.9"
+VERSION = "1.0.0"
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
-    description="Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, Rating Count, and Price.",
+    description="Scrape Amazon product data such as Product Name, Product Images, Product URL, Number of Reviews, ASIN, and Price.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Finbarrs Oketunji",
     author_email="f@finbarrs.eu",
     url="https://finbarrs.eu",
     packages=find_packages(),
     include_package_data=True,
```

