# Comparing `tmp/NewsArticlesScraper-0.2.7.tar.gz` & `tmp/NewsArticlesScraper-0.2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\NewsArticlesScraper-0.2.7.tar", last modified: Tue Jul 25 14:49:53 2023, max compression
+gzip compressed data, was "dist\NewsArticlesScraper-0.2.7.1.tar", last modified: Thu Jul 27 04:29:09 2023, max compression
```

## Comparing `NewsArticlesScraper-0.2.7.tar` & `NewsArticlesScraper-0.2.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:49:53.332652 NewsArticlesScraper-0.2.7/
-drwxrwxrwx   0        0        0        0 2023-07-25 14:49:53.274650 NewsArticlesScraper-0.2.7/NewsArticlesScraper/
--rw-rw-rw-   0        0        0    11043 2023-07-25 08:07:58.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper/ArticleUrlSrapers.py
--rw-rw-rw-   0        0        0    14676 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper/Scrapers.py
--rw-rw-rw-   0        0        0       64 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:49:53.328652 NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/
--rw-rw-rw-   0        0        0      648 2023-07-25 14:49:53.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-07-25 14:49:53.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:49:53.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-25 14:49:53.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-25 14:49:53.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2023-07-25 14:49:53.331653 NewsArticlesScraper-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 14:49:53.333653 NewsArticlesScraper-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      996 2023-07-25 14:39:52.000000 NewsArticlesScraper-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 04:29:09.363278 NewsArticlesScraper-0.2.7.1/
+drwxrwxrwx   0        0        0        0 2023-07-27 04:29:09.335364 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper/
+-rw-rw-rw-   0        0        0    11240 2023-07-27 04:28:28.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper/ArticleUrlSrapers.py
+-rw-rw-rw-   0        0        0    14676 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper/Scrapers.py
+-rw-rw-rw-   0        0        0       64 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 04:29:09.360280 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-07-27 04:29:09.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-07-27 04:29:09.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 04:29:09.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-27 04:29:09.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-27 04:29:09.000000 NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      650 2023-07-27 04:29:09.362273 NewsArticlesScraper-0.2.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 04:29:09.363278 NewsArticlesScraper-0.2.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      998 2023-07-27 04:28:28.000000 NewsArticlesScraper-0.2.7.1/setup.py
```

### Comparing `NewsArticlesScraper-0.2.7/NewsArticlesScraper/ArticleUrlSrapers.py` & `NewsArticlesScraper-0.2.7.1/NewsArticlesScraper/ArticleUrlSrapers.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,17 @@
                 if "cn:contentClassification" in result:
                     clasf = result["cn:contentClassification"]
                     if "premium" in clasf:
                         premium = True
                 if not premium:
                     if result["cn:branding"] == "cnbc":
                         if result["cn:type"] not in ["cnbcvideo", "live_story"]:
-                            yield {"url": result["cn:liveURL"], "time": t}
+                            yield {"url": result["cn:liveURL"],
+                                   "time": t,
+                                   "origin": "c"}
 
 
 class NytUrlSpider(scrapy.Spider):
     """Spider to scrape NYT article urls.
 
     """
     name = 'NytUrlSpider'
@@ -190,15 +192,17 @@
             if api_point == "historic":
                 url = article["web_url"]
             else:
                 try:
                     url = article["related_urls"][0]["url"]
                 except (TypeError, IndexError):
                     url = article["url"]
-            yield {"url": url, "time": pub_date}
+            yield {"url": url,
+                   "time": pub_date,
+                   "origin": "n"}
 
 
 class TheGuardianSpider(scrapy.Spider):
     """Spider to scrape The Guardian article urls.
 
     """
     name = 'TheGuardianSpider'
@@ -246,8 +250,10 @@
             yield scrapy.Request(to_request_url, callback=self.parse_api)
 
     @staticmethod
     def parse_api(response):
         data = response.json()["response"]
         articles = data["results"]
         for article in articles:
-            yield {"url": article["webUrl"], "time": ciso8601.parse_datetime(article["webPublicationDate"])}
+            yield {"url": article["webUrl"],
+                   "time": ciso8601.parse_datetime(article["webPublicationDate"]),
+                   "origin": "g"}
```

### Comparing `NewsArticlesScraper-0.2.7/NewsArticlesScraper/Scrapers.py` & `NewsArticlesScraper-0.2.7.1/NewsArticlesScraper/Scrapers.py`

 * *Files identical despite different names*

### Comparing `NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/PKG-INFO` & `NewsArticlesScraper-0.2.7.1/NewsArticlesScraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.7
+Version: 0.2.7.1
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.7/PKG-INFO` & `NewsArticlesScraper-0.2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.7
+Version: 0.2.7.1
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.7/setup.py` & `NewsArticlesScraper-0.2.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.7'
+VERSION = '0.2.7.1'
 DESCRIPTION = 'Scraping news articles'
 LONG_DESCRIPTION = 'A package that allows you to scrape news articles from various news sites via scrapy.'
 
 # Setting up
 setup(
     name="NewsArticlesScraper",
     version=VERSION,
```

