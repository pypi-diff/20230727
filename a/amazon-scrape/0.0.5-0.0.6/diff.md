# Comparing `tmp/amazon_scrape-0.0.5.tar.gz` & `tmp/amazon_scrape-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amazon_scrape-0.0.5.tar", last modified: Thu Jul 27 11:40:31 2023, max compression
+gzip compressed data, was "dist/amazon_scrape-0.0.6.tar", last modified: Thu Jul 27 13:54:50 2023, max compression
```

## Comparing `amazon_scrape-0.0.5.tar` & `amazon_scrape-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 11:40:31.819908 amazon_scrape-0.0.5/
--rw-r--r--   0 finn       (501) staff       (20)     4890 2023-07-27 11:40:31.820533 amazon_scrape-0.0.5/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2101 2023-07-27 11:39:37.000000 amazon_scrape-0.0.5/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 11:40:31.814813 amazon_scrape-0.0.5/amazon_scrape.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     4890 2023-07-27 11:40:31.000000 amazon_scrape-0.0.5/amazon_scrape.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-27 11:40:31.000000 amazon_scrape-0.0.5/amazon_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 11:40:31.000000 amazon_scrape-0.0.5/amazon_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-27 11:40:31.000000 amazon_scrape-0.0.5/amazon_scrape.egg-info/entry_points.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 11:39:56.000000 amazon_scrape-0.0.5/amazon_scrape.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 11:40:31.000000 amazon_scrape-0.0.5/amazon_scrape.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 11:40:31.000000 amazon_scrape-0.0.5/amazon_scrape.egg-info/top_level.txt
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 11:40:31.818779 amazon_scrape-0.0.5/amazon_scraper/
--rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 11:39:37.000000 amazon_scrape-0.0.5/amazon_scraper/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     5856 2023-07-27 11:39:36.000000 amazon_scrape-0.0.5/amazon_scraper/scraper.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 11:39:37.000000 amazon_scrape-0.0.5/amazon_scraper/version.py
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 11:40:31.821904 amazon_scrape-0.0.5/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2726 2023-07-27 11:39:37.000000 amazon_scrape-0.0.5/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 13:54:50.584991 amazon_scrape-0.0.6/
+-rw-r--r--   0 finn       (501) staff       (20)     4890 2023-07-27 13:54:50.585624 amazon_scrape-0.0.6/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2101 2023-07-27 13:52:23.000000 amazon_scrape-0.0.6/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 13:54:50.575437 amazon_scrape-0.0.6/amazon_scrape.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     4890 2023-07-27 13:54:50.000000 amazon_scrape-0.0.6/amazon_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      367 2023-07-27 13:54:50.000000 amazon_scrape-0.0.6/amazon_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 13:54:50.000000 amazon_scrape-0.0.6/amazon_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)       64 2023-07-27 13:54:50.000000 amazon_scrape-0.0.6/amazon_scrape.egg-info/entry_points.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-07-27 13:53:21.000000 amazon_scrape-0.0.6/amazon_scrape.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)       24 2023-07-27 13:54:50.000000 amazon_scrape-0.0.6/amazon_scrape.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       15 2023-07-27 13:54:50.000000 amazon_scrape-0.0.6/amazon_scrape.egg-info/top_level.txt
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-07-27 13:54:50.583781 amazon_scrape-0.0.6/amazon_scraper/
+-rw-r--r--   0 finn       (501) staff       (20)       48 2023-07-27 13:52:23.000000 amazon_scrape-0.0.6/amazon_scraper/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     6832 2023-07-27 13:52:23.000000 amazon_scrape-0.0.6/amazon_scraper/scraper.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-07-27 13:52:23.000000 amazon_scrape-0.0.6/amazon_scraper/version.py
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-07-27 13:54:50.587496 amazon_scrape-0.0.6/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2726 2023-07-27 13:52:23.000000 amazon_scrape-0.0.6/setup.py
```

### Comparing `amazon_scrape-0.0.5/PKG-INFO` & `amazon_scrape-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_scrape
-Version: 0.0.5
+Version: 0.0.6
 Summary: Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
```

### Comparing `amazon_scrape-0.0.5/README.md` & `amazon_scrape-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `amazon_scrape-0.0.5/amazon_scrape.egg-info/PKG-INFO` & `amazon_scrape-0.0.6/amazon_scrape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-scrape
-Version: 0.0.5
+Version: 0.0.6
 Summary: Scrape Amazon product data such as Product Name, Product Images, Rating Count, and Price.
 Home-page: https://finbarrs.eu
 Author: Finbarrs Oketunji
 Author-email: f@finbarrs.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/0xnu/amazonproducts/issues
 Project-URL: Changes, https://github.com/0xnu/amazonproducts/blob/main/CHANGELOG.md
```

### Comparing `amazon_scrape-0.0.5/amazon_scraper/scraper.py` & `amazon_scrape-0.0.6/amazon_scraper/scraper.py`

 * *Files 19% similar despite different names*

```diff
@@ -37,17 +37,18 @@
             self.url = f"http://api.scraperapi.com?api_key={api_key}&url={url}"
         self.api_key = api_key
         self.pages = pages
         self.csv_file = open('amazon_products.csv', 'w', newline='')
         self.json_file = open('amazon_products.json', 'w')
         self.writer = csv.writer(self.csv_file)
         self.json_data = []
+        self.locale = locale
 
     def start_scraping(self):
-        self.writer.writerow(["product_name", "product_images", "rating_count", "price"])
+        self.writer.writerow(["product_name", "product_images", "rating_count", "price", "product_url", "number_of_reviews", "asin"])
         for page in range(1, self.pages + 1):
             url = self.url + "&page=" + str(page)
             headers = {"User-Agent": random.choice(self.user_agents)}
             response = requests.get(url, headers=headers)
             soup = BeautifulSoup(response.content, "html.parser")
             products = soup.find_all("div", {"class": "sg-col-inner"})
 
@@ -76,23 +77,43 @@
                 # Price
                 price = product.find("span", {"class": "a-offscreen"})
                 if price is not None:
                     price = price.text
                 else:
                     price = ''
 
+                # Product URL
+                product_url = product.find("a", {"class": "a-link-normal"})
+                if product_url is not None:
+                    product_url = f'https://www.amazon.{self.locale}' + product_url['href']
+                else:
+                    product_url = ''
+
+                # Number of reviews
+                number_of_reviews = product.find("span", {"class": "a-size-base"})
+                if number_of_reviews is not None:
+                    number_of_reviews = number_of_reviews.text
+                else:
+                    number_of_reviews = ''
+
+                # ASIN
+                asin = product_url.split("/dp/")[1].split("/")[0] if "/dp/" in product_url else ''
+
                 # Write to CSV
-                self.writer.writerow([name, ", ".join(images), rating_count, price])
+                self.writer.writerow([name, ", ".join(images), rating_count, price, product_url, number_of_reviews, asin])
 
                 # Add to JSON data
                 self.json_data.append({
                     "product_name": name,
                     "product_images": images,
                     "rating_count": rating_count,
-                    "price": price
+                    "price": price,
+                    "product_url": product_url,
+                    "number_of_reviews": number_of_reviews,
+                    "asin": asin
                 })
 
         json.dump(self.json_data, self.json_file, indent=4)
 
     def close_files(self):
         self.csv_file.close()
         self.json_file.close()
```

### Comparing `amazon_scrape-0.0.5/setup.py` & `amazon_scrape-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "amazon_scrape"
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 REQUIRES = ["beautifulsoup4", "requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

