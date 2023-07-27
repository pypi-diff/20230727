# Comparing `tmp/scraper_util_avliu-0.1.0.tar.gz` & `tmp/scraper_util_avliu-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scraper_util_avliu-0.1.0.tar", last modified: Thu Jul 27 16:03:39 2023, max compression
+gzip compressed data, was "scraper_util_avliu-0.1.1.tar", last modified: Thu Jul 27 16:07:26 2023, max compression
```

## Comparing `scraper_util_avliu-0.1.0.tar` & `scraper_util_avliu-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:03:39.244171 scraper_util_avliu-0.1.0/
--rw-r--r--   0 avliu      (504) staff       (20)        5 2023-06-20 08:37:43.000000 scraper_util_avliu-0.1.0/LICENSE
--rw-r--r--   0 avliu      (504) staff       (20)       84 2023-07-27 16:03:39.243984 scraper_util_avliu-0.1.0/PKG-INFO
--rw-r--r--   0 avliu      (504) staff       (20)      228 2023-07-27 15:54:00.000000 scraper_util_avliu-0.1.0/README.md
--rw-r--r--   0 avliu      (504) staff       (20)      269 2023-07-27 16:03:32.000000 scraper_util_avliu-0.1.0/pyproject.toml
--rw-r--r--   0 avliu      (504) staff       (20)       38 2023-07-27 16:03:39.244228 scraper_util_avliu-0.1.0/setup.cfg
-drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:03:39.241094 scraper_util_avliu-0.1.0/src/
-drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:03:39.242775 scraper_util_avliu-0.1.0/src/scraper_util_avliu/
--rw-r--r--   0 avliu      (504) staff       (20)        1 2023-06-20 08:37:43.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu/__init__.py
--rw-r--r--   0 avliu      (504) staff       (20)       36 2023-07-27 16:01:51.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu/example.py
--rw-r--r--   0 avliu      (504) staff       (20)     3246 2023-07-27 15:36:17.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu/util.py
-drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:03:39.243755 scraper_util_avliu-0.1.0/src/scraper_util_avliu.egg-info/
--rw-r--r--   0 avliu      (504) staff       (20)       84 2023-07-27 16:03:39.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu.egg-info/PKG-INFO
--rw-r--r--   0 avliu      (504) staff       (20)      361 2023-07-27 16:03:39.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu.egg-info/SOURCES.txt
--rw-r--r--   0 avliu      (504) staff       (20)        1 2023-07-27 16:03:39.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu.egg-info/dependency_links.txt
--rw-r--r--   0 avliu      (504) staff       (20)       72 2023-07-27 16:03:39.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu.egg-info/requires.txt
--rw-r--r--   0 avliu      (504) staff       (20)       19 2023-07-27 16:03:39.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu.egg-info/top_level.txt
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:07:26.781619 scraper_util_avliu-0.1.1/
+-rw-r--r--   0 avliu      (504) staff       (20)        5 2023-06-20 08:37:43.000000 scraper_util_avliu-0.1.1/LICENSE
+-rw-r--r--   0 avliu      (504) staff       (20)       84 2023-07-27 16:07:26.781140 scraper_util_avliu-0.1.1/PKG-INFO
+-rw-r--r--   0 avliu      (504) staff       (20)      228 2023-07-27 15:54:00.000000 scraper_util_avliu-0.1.1/README.md
+-rw-r--r--   0 avliu      (504) staff       (20)      269 2023-07-27 16:07:17.000000 scraper_util_avliu-0.1.1/pyproject.toml
+-rw-r--r--   0 avliu      (504) staff       (20)       38 2023-07-27 16:07:26.781741 scraper_util_avliu-0.1.1/setup.cfg
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:07:26.775346 scraper_util_avliu-0.1.1/src/
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:07:26.778013 scraper_util_avliu-0.1.1/src/scraper_util_avliu/
+-rw-r--r--   0 avliu      (504) staff       (20)        1 2023-06-20 08:37:43.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu/__init__.py
+-rw-r--r--   0 avliu      (504) staff       (20)       36 2023-07-27 16:01:51.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu/example.py
+-rw-r--r--   0 avliu      (504) staff       (20)     3243 2023-07-27 16:07:04.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu/util.py
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:07:26.780551 scraper_util_avliu-0.1.1/src/scraper_util_avliu.egg-info/
+-rw-r--r--   0 avliu      (504) staff       (20)       84 2023-07-27 16:07:26.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu.egg-info/PKG-INFO
+-rw-r--r--   0 avliu      (504) staff       (20)      361 2023-07-27 16:07:26.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu.egg-info/SOURCES.txt
+-rw-r--r--   0 avliu      (504) staff       (20)        1 2023-07-27 16:07:26.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu.egg-info/dependency_links.txt
+-rw-r--r--   0 avliu      (504) staff       (20)       72 2023-07-27 16:07:26.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu.egg-info/requires.txt
+-rw-r--r--   0 avliu      (504) staff       (20)       19 2023-07-27 16:07:26.000000 scraper_util_avliu-0.1.1/src/scraper_util_avliu.egg-info/top_level.txt
```

### Comparing `scraper_util_avliu-0.1.0/src/scraper_util_avliu/util.py` & `scraper_util_avliu-0.1.1/src/scraper_util_avliu/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import mysql.connector
 import os
 
 
 def get_selenium_driver(undetected=False):
 
     print(os.getcwd())
-    adblock_filepath = 'util/lib/adblock.crx'
+    adblock_filepath = './lib/adblock.crx'
 
     if undetected:
         chrome_options = uc.ChromeOptions()
         chrome_options.add_argument('--mute-audio')
         chrome_options.add_extension(adblock_filepath)
         driver = uc.Chrome(options=chrome_options)
```

