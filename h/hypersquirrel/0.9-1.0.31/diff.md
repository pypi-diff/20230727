# Comparing `tmp/hypersquirrel-0.9.tar.gz` & `tmp/hypersquirrel-1.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypersquirrel-0.9.tar", last modified: Thu Nov 18 00:15:36 2021, max compression
+gzip compressed data, was "hypersquirrel-1.0.31.tar", last modified: Thu Jul 27 16:46:33 2023, max compression
```

## Comparing `hypersquirrel-0.9.tar` & `hypersquirrel-1.0.31.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.771202 hypersquirrel-0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-11-18 00:15:26.000000 hypersquirrel-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      730 2021-11-18 00:15:36.771202 hypersquirrel-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      381 2021-11-18 00:15:26.000000 hypersquirrel-0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.767202 hypersquirrel-0.9/hypersquirrel/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.767202 hypersquirrel-0.9/hypersquirrel/scraper/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/buondua.py
--rw-r--r--   0 runner    (1001) docker     (121)      861 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/cosplayporntube.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/drts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/ehen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/fseg.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/googleimagesearch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1942 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/hcos.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/hnlg.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/lgbb.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/nh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/nlgs.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/opendir.py
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/reddit.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/sb.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/sbgx.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/v2ph.py
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/vg.py
--rw-r--r--   0 runner    (1001) docker     (121)      850 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/xh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/xv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraper/youtubeapi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3185 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/scraperfactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.767202 hypersquirrel-0.9/hypersquirrel/watchlist/
--rw-r--r--   0 runner    (1001) docker     (121)      833 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.771202 hypersquirrel-0.9/hypersquirrel/watchlist/decorator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/decorator/maxitems.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.771202 hypersquirrel-0.9/hypersquirrel/watchlist/validator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/validator/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/validator/paged.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2021-11-18 00:15:26.000000 hypersquirrel-0.9/hypersquirrel/watchlist/validatorfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 00:15:36.767202 hypersquirrel-0.9/hypersquirrel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      730 2021-11-18 00:15:36.000000 hypersquirrel-0.9/hypersquirrel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-11-18 00:15:36.000000 hypersquirrel-0.9/hypersquirrel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 00:15:36.000000 hypersquirrel-0.9/hypersquirrel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-11-18 00:15:36.000000 hypersquirrel-0.9/hypersquirrel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-11-18 00:15:36.000000 hypersquirrel-0.9/hypersquirrel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-18 00:15:36.771202 hypersquirrel-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      609 2021-11-18 00:15:27.000000 hypersquirrel-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:33.286415 hypersquirrel-1.0.31/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-27 16:46:33.286415 hypersquirrel-1.0.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:33.282415 hypersquirrel-1.0.31/hypersquirrel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:33.282415 hypersquirrel-1.0.31/hypersquirrel/literalinterpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/literalinterpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/literalinterpreter/ehen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/literalinterpreter/instagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/literalinterpreter/ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/literalinterpreterfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:33.286415 hypersquirrel-1.0.31/hypersquirrel/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/buondua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/cosplayporntube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/drts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/ehen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/fseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/googleimagesearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/hcos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/hellp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/hnlg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/lgbb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/nh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/nlgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/opendir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/sb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/sbgx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/v2ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/vg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/xh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/xv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/youtubeapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraperfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:33.282415 hypersquirrel-1.0.31/hypersquirrel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-27 16:46:33.000000 hypersquirrel-1.0.31/hypersquirrel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-27 16:46:33.000000 hypersquirrel-1.0.31/hypersquirrel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:46:33.000000 hypersquirrel-1.0.31/hypersquirrel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 16:46:33.000000 hypersquirrel-1.0.31/hypersquirrel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 16:46:33.000000 hypersquirrel-1.0.31/hypersquirrel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 16:46:33.286415 hypersquirrel-1.0.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-27 16:46:17.000000 hypersquirrel-1.0.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:33.286415 hypersquirrel-1.0.31/ytdlwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/ytdlwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/ytdlwrapper/ytdlpscrape.py
```

### Comparing `hypersquirrel-0.9/LICENSE` & `hypersquirrel-1.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/PKG-INFO` & `hypersquirrel-1.0.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypersquirrel
-Version: 0.9
+Version: 1.0.31
 Summary: Scrapes posts from various websites
 Home-page: UNKNOWN
 Author: vka
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/buondua.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/buondua.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/cosplayporntube.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/cosplayporntube.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/drts.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/drts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generator
+from typing import Iterator
 
 from commmons import head, md5
 from lxml.html import HtmlElement
 
 from hypersquirrel.util import html_from_url_with_headers
 
 
@@ -35,11 +35,11 @@
         if "gallery" in source_url:
             yield {
                 **file,
                 "sourceurl": f"vpr://{source_url}"
             }
 
 
-def scrape_drts(url: str) -> Generator[dict, None, None]:
+def scrape_drts(url: str) -> Iterator[dict]:
     root = html_from_url_with_headers(url)
     yield from vids(root)
     yield from pics(root)
```

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/ehen.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/ehen.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/fseg.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/fseg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/hcos.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/hcos.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/hnlg.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/hnlg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/lgbb.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/lgbb.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/nlgs.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/nlgs.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/sbgx.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/sbgx.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/vg.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/vg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/xh.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/xh.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/hypersquirrel/scraper/xv.py` & `hypersquirrel-1.0.31/hypersquirrel/scraper/xv.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-0.9/hypersquirrel/scraperfactory.py` & `hypersquirrel-1.0.31/hypersquirrel/scraperfactory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-from typing import Callable, Generator
+from typing import Callable, Iterator
 
+from .core import Watchlist
 from .scraper import youtubeapi
 from .scraper.buondua import scrape_buondua
 from .scraper.cosplayporntube import scrape_cpt
 from .scraper.drts import scrape_drts
 from .scraper.ehen import scrape_ehen
 from .scraper.fseg import scrape as scrape_fseg_html
 from .scraper.googleimagesearch import scrape_gimg
 from .scraper.hcos import scrape_hcos
 from .scraper.hnlg import scrape_hnlg
 from .scraper.lgbb import scrape_lgbb
 from .scraper.nh import scrape as scrape_nh_html
 from .scraper.nlgs import scrape_uulg, scrape_nlgs, scrape_lgcx
 from .scraper.opendir import scrape as scrape_opendir
-from .scraper.reddit import scrape_subreddit
+from .scraper.reddit import scrape_reddit_rss, scrape_reddit_json
 from .scraper.sb import scrape as scrape_sb_html
 from .scraper.sbgx import scrape_sbgx
 from .scraper.v2ph import scrape_v2ph
 from .scraper.vg import scrape_vipergirls as scrape_vg_html
 from .scraper.xh import scrape as scrape_xh_html
 from .scraper.xv import scrape as scrape_xv_html
-from .watchlist import Watchlist
+from .scraper.hellp import scrape as scrape_hellp
 
 
 class WatchlistScraperFactory:
     def __init__(self):
         self.registry = list()
 
     def register_scraper(self, predicate: Callable[[Watchlist], bool],
-                         scraper: Callable[[str], Generator[dict, None, None]]):
+                         scraper: Callable[[str], Iterator[dict]]):
         self.registry.append((predicate, scraper,))
 
     def get_scraper(self, watchlist: Watchlist):
         for registry_pair in self.registry:
             condition = registry_pair[0]
             scraper = registry_pair[1]
             if condition(watchlist):
@@ -47,15 +48,16 @@
 register_scraper = _wsf.register_scraper
 
 register_scraper(lambda w: "pornhub.com" in w.url, scrape_nh_html)
 register_scraper(lambda w: "vipergirls" in w.url, scrape_vg_html)
 register_scraper(lambda w: "xhamster" in w.url, scrape_xh_html)
 register_scraper(lambda w: "xvideos.com" in w.url, scrape_xv_html)
 register_scraper(lambda w: "spankbang.com" in w.url, scrape_sb_html)
-register_scraper(lambda w: "reddit" in w.url, scrape_subreddit)
+register_scraper(lambda w: "reddit" in w.url and "json?feed" in w.url, scrape_reddit_json)
+register_scraper(lambda w: "reddit" in w.url, scrape_reddit_rss)
 register_scraper(lambda w: "v2ph" in w.url, scrape_v2ph)
 register_scraper(lambda w: "hentai-cosplays" in w.url, scrape_hcos)
 register_scraper(lambda w: "buondua" in w.url, scrape_buondua)
 register_scraper(lambda w: "e-hentai" in w.url, scrape_ehen)
 register_scraper(lambda w: "cosplayporntube" in w.url, scrape_cpt)
 register_scraper(lambda w: "egirls" in w.url, scrape_fseg_html)
 register_scraper(lambda w: "nlegs" in w.url, scrape_nlgs)
@@ -64,10 +66,9 @@
 register_scraper(lambda w: "legbabe" in w.url, scrape_lgbb)
 register_scraper(lambda w: "leg.cx" in w.url, scrape_lgcx)
 register_scraper(lambda w: "superbeautygirlx" in w.url, scrape_sbgx)
 register_scraper(lambda w: "porn-images-xxx" in w.url, scrape_hcos)
 register_scraper(lambda w: "hentai-img" in w.url, scrape_hcos)
 register_scraper(lambda w: "google" in w.url, scrape_gimg)
 register_scraper(lambda w: "dirtyship" in w.url, scrape_drts)
-
-if youtubeapi.APIKEY:
-    register_scraper(lambda w: "youtube" in w.url, youtubeapi.scrape_youtubeapi)
+register_scraper(lambda w: "hellporno" in w.url, scrape_hellp)
+register_scraper(lambda w: "youtube" in w.url, youtubeapi.scrape_youtubeapi)
```

### Comparing `hypersquirrel-0.9/hypersquirrel.egg-info/PKG-INFO` & `hypersquirrel-1.0.31/hypersquirrel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypersquirrel
-Version: 0.9
+Version: 1.0.31
 Summary: Scrapes posts from various websites
 Home-page: UNKNOWN
 Author: vka
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `hypersquirrel-0.9/hypersquirrel.egg-info/SOURCES.txt` & `hypersquirrel-1.0.31/hypersquirrel.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 LICENSE
 README.md
 setup.py
 hypersquirrel/__init__.py
 hypersquirrel/__main__.py
+hypersquirrel/core.py
 hypersquirrel/entry.py
+hypersquirrel/literalinterpreterfactory.py
 hypersquirrel/scraperfactory.py
 hypersquirrel/util.py
 hypersquirrel.egg-info/PKG-INFO
 hypersquirrel.egg-info/SOURCES.txt
 hypersquirrel.egg-info/dependency_links.txt
 hypersquirrel.egg-info/requires.txt
 hypersquirrel.egg-info/top_level.txt
+hypersquirrel/literalinterpreter/__init__.py
+hypersquirrel/literalinterpreter/ehen.py
+hypersquirrel/literalinterpreter/instagram.py
+hypersquirrel/literalinterpreter/ph.py
 hypersquirrel/scraper/__init__.py
 hypersquirrel/scraper/buondua.py
 hypersquirrel/scraper/cosplayporntube.py
 hypersquirrel/scraper/drts.py
 hypersquirrel/scraper/ehen.py
 hypersquirrel/scraper/fseg.py
 hypersquirrel/scraper/googleimagesearch.py
 hypersquirrel/scraper/hcos.py
+hypersquirrel/scraper/hellp.py
 hypersquirrel/scraper/hnlg.py
 hypersquirrel/scraper/lgbb.py
 hypersquirrel/scraper/nh.py
 hypersquirrel/scraper/nlgs.py
 hypersquirrel/scraper/opendir.py
 hypersquirrel/scraper/reddit.py
 hypersquirrel/scraper/sb.py
 hypersquirrel/scraper/sbgx.py
 hypersquirrel/scraper/v2ph.py
 hypersquirrel/scraper/vg.py
 hypersquirrel/scraper/xh.py
 hypersquirrel/scraper/xv.py
 hypersquirrel/scraper/youtubeapi.py
-hypersquirrel/watchlist/__init__.py
-hypersquirrel/watchlist/validatorfactory.py
-hypersquirrel/watchlist/decorator/__init__.py
-hypersquirrel/watchlist/decorator/maxitems.py
-hypersquirrel/watchlist/validator/__init__.py
-hypersquirrel/watchlist/validator/base.py
-hypersquirrel/watchlist/validator/paged.py
+ytdlwrapper/__init__.py
+ytdlwrapper/ytdlpscrape.py
```

### Comparing `hypersquirrel-0.9/setup.py` & `hypersquirrel-1.0.31/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hypersquirrel",
-    version="0.9",
+    version="v1.0.31",
     author="vka",
     description="Scrapes posts from various websites",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=("test",)),
     classifiers=[
         "Programming Language :: Python :: 3",
```

