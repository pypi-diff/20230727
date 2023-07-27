# Comparing `tmp/ntscraper-0.1.5.tar.gz` & `tmp/ntscraper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntscraper-0.1.5.tar", last modified: Wed Jul 12 09:58:27 2023, max compression
+gzip compressed data, was "ntscraper-0.1.6.tar", last modified: Thu Jul 27 18:07:55 2023, max compression
```

## Comparing `ntscraper-0.1.5.tar` & `ntscraper-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 09:58:27.341008 ntscraper-0.1.5/
--rw-rw-rw-   0        0        0     1091 2023-01-15 20:51:11.000000 ntscraper-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     3497 2023-07-12 09:58:27.333025 ntscraper-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2571 2023-07-12 09:48:40.000000 ntscraper-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 09:58:27.300998 ntscraper-0.1.5/ntscraper/
--rw-rw-rw-   0        0        0       26 2023-07-12 09:21:01.000000 ntscraper-0.1.5/ntscraper/__init__.py
--rw-rw-rw-   0        0        0    27718 2023-07-12 09:46:56.000000 ntscraper-0.1.5/ntscraper/nitter.py
-drwxrwxrwx   0        0        0        0 2023-07-12 09:58:27.333025 ntscraper-0.1.5/ntscraper.egg-info/
--rw-rw-rw-   0        0        0     3497 2023-07-12 09:58:26.000000 ntscraper-0.1.5/ntscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-12 09:58:27.000000 ntscraper-0.1.5/ntscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 09:58:26.000000 ntscraper-0.1.5/ntscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-12 09:58:26.000000 ntscraper-0.1.5/ntscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 09:58:27.000000 ntscraper-0.1.5/ntscraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 09:58:27.341008 ntscraper-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-07-12 09:48:05.000000 ntscraper-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 18:07:55.964204 ntscraper-0.1.6/
+-rw-rw-rw-   0        0        0     1091 2023-01-15 20:51:11.000000 ntscraper-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     3439 2023-07-27 18:07:55.964204 ntscraper-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2513 2023-07-27 18:07:45.000000 ntscraper-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 18:07:55.908185 ntscraper-0.1.6/ntscraper/
+-rw-rw-rw-   0        0        0       26 2023-07-12 10:00:30.000000 ntscraper-0.1.6/ntscraper/__init__.py
+-rw-rw-rw-   0        0        0    27712 2023-07-27 18:05:03.000000 ntscraper-0.1.6/ntscraper/nitter.py
+drwxrwxrwx   0        0        0        0 2023-07-27 18:07:55.964204 ntscraper-0.1.6/ntscraper.egg-info/
+-rw-rw-rw-   0        0        0     3439 2023-07-27 18:07:55.000000 ntscraper-0.1.6/ntscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-27 18:07:55.000000 ntscraper-0.1.6/ntscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 18:07:55.000000 ntscraper-0.1.6/ntscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-27 18:07:55.000000 ntscraper-0.1.6/ntscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 18:07:55.000000 ntscraper-0.1.6/ntscraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 18:07:55.964204 ntscraper-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2023-07-27 18:05:32.000000 ntscraper-0.1.6/setup.py
```

### Comparing `ntscraper-0.1.5/LICENSE.txt` & `ntscraper-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ntscraper-0.1.5/PKG-INFO` & `ntscraper-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntscraper
-Version: 0.1.5
+Version: 0.1.6
 Summary: Unofficial library to scrape Twitter profiles and posts from Nitter instances
 Author: Lorenzo Bocchi
 Author-email: lorenzobocchi99@yahoo.com
 License: MIT
 Project-URL: Homepage, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Source, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Documentation, https://github.com/bocchilorenzo/ntscraper
@@ -96,12 +96,12 @@
 random_instance = scraper.get_random_instance()
 ```
 
 Returns a random Nitter instance.
 
 ## Note
 
-Unfortunately, at the moment searching for tweets either via 'term' or 'hashtag' doesn't work because Twitter removed the ability to search without being registered, and as consequence Nitter's search is broken. You can still scrape user profiles.
+Some Nitter instances may not work properly due to recent changes on Twitter's side. If you have trouble scraping with a certain instance, try changing it and check if the problem persists.
 
 ## To do list
 
 - [ ] Add scraping of individual posts with comments
```

### Comparing `ntscraper-0.1.5/README.md` & `ntscraper-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -74,12 +74,12 @@
 random_instance = scraper.get_random_instance()
 ```
 
 Returns a random Nitter instance.
 
 ## Note
 
-Unfortunately, at the moment searching for tweets either via 'term' or 'hashtag' doesn't work because Twitter removed the ability to search without being registered, and as consequence Nitter's search is broken. You can still scrape user profiles.
+Some Nitter instances may not work properly due to recent changes on Twitter's side. If you have trouble scraping with a certain instance, try changing it and check if the problem persists.
 
 ## To do list
 
 - [ ] Add scraping of individual posts with comments
```

### Comparing `ntscraper-0.1.5/ntscraper/nitter.py` & `ntscraper-0.1.6/ntscraper/nitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def __is_instance_encrypted(self, instance):
         """
         Check if the instance uses encrypted media
 
         :param instance: Nitter instance
         :return: True if encrypted, False otherwise
         """
-        instance_new, soup = self.__get_page("/Twitter", instance)
+        instance_new, soup = self.__get_page("/x", instance)
 
         if (
             soup.find("a", class_="profile-card-avatar").find("img")
             and "/enc/"
             in soup.find("a", class_="profile-card-avatar").find("img")["src"]
         ):
             return True
```

### Comparing `ntscraper-0.1.5/ntscraper.egg-info/PKG-INFO` & `ntscraper-0.1.6/ntscraper.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntscraper
-Version: 0.1.5
+Version: 0.1.6
 Summary: Unofficial library to scrape Twitter profiles and posts from Nitter instances
 Author: Lorenzo Bocchi
 Author-email: lorenzobocchi99@yahoo.com
 License: MIT
 Project-URL: Homepage, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Source, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Documentation, https://github.com/bocchilorenzo/ntscraper
@@ -96,12 +96,12 @@
 random_instance = scraper.get_random_instance()
 ```
 
 Returns a random Nitter instance.
 
 ## Note
 
-Unfortunately, at the moment searching for tweets either via 'term' or 'hashtag' doesn't work because Twitter removed the ability to search without being registered, and as consequence Nitter's search is broken. You can still scrape user profiles.
+Some Nitter instances may not work properly due to recent changes on Twitter's side. If you have trouble scraping with a certain instance, try changing it and check if the problem persists.
 
 ## To do list
 
 - [ ] Add scraping of individual posts with comments
```

### Comparing `ntscraper-0.1.5/setup.py` & `ntscraper-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="ntscraper",
-    version="0.1.5",
+    version="0.1.6",
     description="Unofficial library to scrape Twitter profiles and posts from Nitter instances",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         'Homepage': 'https://github.com/bocchilorenzo/ntscraper',
         'Source': 'https://github.com/bocchilorenzo/ntscraper',
         'Documentation': 'https://github.com/bocchilorenzo/ntscraper'
```

