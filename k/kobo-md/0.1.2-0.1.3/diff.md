# Comparing `tmp/kobo-md-0.1.2.tar.gz` & `tmp/kobo-md-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kobo-md-0.1.2.tar", last modified: Thu Jul 27 04:15:29 2023, max compression
+gzip compressed data, was "kobo-md-0.1.3.tar", last modified: Thu Jul 27 08:02:25 2023, max compression
```

## Comparing `kobo-md-0.1.2.tar` & `kobo-md-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 04:15:29.056157 kobo-md-0.1.2/
--rw-r--r--   0 dwall      (501) staff       (20)     1086 2023-07-26 20:39:20.000000 kobo-md-0.1.2/LICENSE.txt
--rw-r--r--   0 dwall      (501) staff       (20)       46 2023-07-26 08:15:21.000000 kobo-md-0.1.2/MANIFEST.in
--rw-r--r--   0 dwall      (501) staff       (20)      760 2023-07-27 04:15:29.056210 kobo-md-0.1.2/PKG-INFO
--rw-r--r--   0 dwall      (501) staff       (20)      561 2023-07-26 21:02:59.000000 kobo-md-0.1.2/README.md
--rw-r--r--   0 dwall      (501) staff       (20)      106 2023-07-27 04:15:29.056389 kobo-md-0.1.2/setup.cfg
--rw-r--r--   0 dwall      (501) staff       (20)      820 2023-07-27 04:15:13.000000 kobo-md-0.1.2/setup.py
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 04:15:29.052292 kobo-md-0.1.2/src/
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 04:15:29.054271 kobo-md-0.1.2/src/kobo/
--rw-r--r--   0 dwall      (501) staff       (20)       42 2023-07-26 20:33:16.000000 kobo-md-0.1.2/src/kobo/__init__.py
--rw-r--r--   0 dwall      (501) staff       (20)     1770 2023-07-26 08:44:52.000000 kobo-md-0.1.2/src/kobo/__main__.py
--rw-r--r--   0 dwall      (501) staff       (20)      791 2023-07-26 08:48:12.000000 kobo-md-0.1.2/src/kobo/helper.py
--rw-r--r--   0 dwall      (501) staff       (20)     6274 2023-07-26 20:33:36.000000 kobo-md-0.1.2/src/kobo/parser.py
--rw-r--r--   0 dwall      (501) staff       (20)      344 2023-07-26 07:12:37.000000 kobo-md-0.1.2/src/kobo/redirects.py
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 04:15:29.052230 kobo-md-0.1.2/src/kobo/resources/
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 04:15:29.054476 kobo-md-0.1.2/src/kobo/resources/content/
--rw-r--r--   0 dwall      (501) staff       (20)       94 2023-07-26 08:39:44.000000 kobo-md-0.1.2/src/kobo/resources/content/index.md
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 04:15:29.052172 kobo-md-0.1.2/src/kobo/resources/static/
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 04:15:29.054863 kobo-md-0.1.2/src/kobo/resources/static/css/
--rw-r--r--   0 dwall      (501) staff       (20)     2527 2023-07-26 07:01:14.000000 kobo-md-0.1.2/src/kobo/resources/static/css/grid.css
--rw-r--r--   0 dwall      (501) staff       (20)      608 2023-07-26 07:01:14.000000 kobo-md-0.1.2/src/kobo/resources/static/css/main.css
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 04:15:29.055479 kobo-md-0.1.2/src/kobo/resources/templates/
--rw-r--r--   0 dwall      (501) staff       (20)      296 2023-07-26 07:01:18.000000 kobo-md-0.1.2/src/kobo/resources/templates/404.html
--rw-r--r--   0 dwall      (501) staff       (20)      383 2023-07-26 07:01:18.000000 kobo-md-0.1.2/src/kobo/resources/templates/index-list.html
--rw-r--r--   0 dwall      (501) staff       (20)      381 2023-07-26 07:01:18.000000 kobo-md-0.1.2/src/kobo/resources/templates/index.html
--rw-r--r--   0 dwall      (501) staff       (20)      375 2023-07-26 07:01:18.000000 kobo-md-0.1.2/src/kobo/resources/templates/page.html
--rw-r--r--   0 dwall      (501) staff       (20)     2534 2023-07-26 07:39:13.000000 kobo-md-0.1.2/src/kobo/server.py
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 04:15:29.056022 kobo-md-0.1.2/src/kobo_md.egg-info/
--rw-r--r--   0 dwall      (501) staff       (20)      760 2023-07-27 04:15:29.000000 kobo-md-0.1.2/src/kobo_md.egg-info/PKG-INFO
--rw-r--r--   0 dwall      (501) staff       (20)      623 2023-07-27 04:15:29.000000 kobo-md-0.1.2/src/kobo_md.egg-info/SOURCES.txt
--rw-r--r--   0 dwall      (501) staff       (20)        1 2023-07-27 04:15:29.000000 kobo-md-0.1.2/src/kobo_md.egg-info/dependency_links.txt
--rw-r--r--   0 dwall      (501) staff       (20)       34 2023-07-27 04:15:29.000000 kobo-md-0.1.2/src/kobo_md.egg-info/requires.txt
--rw-r--r--   0 dwall      (501) staff       (20)        5 2023-07-27 04:15:29.000000 kobo-md-0.1.2/src/kobo_md.egg-info/top_level.txt
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.393062 kobo-md-0.1.3/
+-rw-r--r--   0 dwall      (501) staff       (20)     1086 2023-07-26 20:39:20.000000 kobo-md-0.1.3/LICENSE.txt
+-rw-r--r--   0 dwall      (501) staff       (20)       46 2023-07-27 04:51:30.000000 kobo-md-0.1.3/MANIFEST.in
+-rw-r--r--   0 dwall      (501) staff       (20)      760 2023-07-27 08:02:25.393109 kobo-md-0.1.3/PKG-INFO
+-rw-r--r--   0 dwall      (501) staff       (20)      561 2023-07-26 21:02:59.000000 kobo-md-0.1.3/README.md
+-rw-r--r--   0 dwall      (501) staff       (20)      106 2023-07-27 08:02:25.393273 kobo-md-0.1.3/setup.cfg
+-rw-r--r--   0 dwall      (501) staff       (20)      820 2023-07-27 08:02:05.000000 kobo-md-0.1.3/setup.py
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.389144 kobo-md-0.1.3/src/
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.391086 kobo-md-0.1.3/src/kobo/
+-rw-r--r--   0 dwall      (501) staff       (20)       42 2023-07-27 05:04:42.000000 kobo-md-0.1.3/src/kobo/__init__.py
+-rw-r--r--   0 dwall      (501) staff       (20)     1770 2023-07-26 08:44:52.000000 kobo-md-0.1.3/src/kobo/__main__.py
+-rw-r--r--   0 dwall      (501) staff       (20)      791 2023-07-26 08:48:12.000000 kobo-md-0.1.3/src/kobo/helper.py
+-rw-r--r--   0 dwall      (501) staff       (20)     6378 2023-07-27 08:01:33.000000 kobo-md-0.1.3/src/kobo/parser.py
+-rw-r--r--   0 dwall      (501) staff       (20)      344 2023-07-26 07:12:37.000000 kobo-md-0.1.3/src/kobo/redirects.py
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.389080 kobo-md-0.1.3/src/kobo/resources/
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.391313 kobo-md-0.1.3/src/kobo/resources/content/
+-rw-r--r--   0 dwall      (501) staff       (20)       94 2023-07-26 08:39:44.000000 kobo-md-0.1.3/src/kobo/resources/content/index.md
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.389016 kobo-md-0.1.3/src/kobo/resources/static/
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.391726 kobo-md-0.1.3/src/kobo/resources/static/css/
+-rw-r--r--   0 dwall      (501) staff       (20)     2527 2023-07-26 07:01:14.000000 kobo-md-0.1.3/src/kobo/resources/static/css/grid.css
+-rw-r--r--   0 dwall      (501) staff       (20)      608 2023-07-26 07:01:14.000000 kobo-md-0.1.3/src/kobo/resources/static/css/main.css
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.392454 kobo-md-0.1.3/src/kobo/resources/templates/
+-rw-r--r--   0 dwall      (501) staff       (20)      296 2023-07-26 07:01:18.000000 kobo-md-0.1.3/src/kobo/resources/templates/404.html
+-rw-r--r--   0 dwall      (501) staff       (20)      383 2023-07-26 07:01:18.000000 kobo-md-0.1.3/src/kobo/resources/templates/index-list.html
+-rw-r--r--   0 dwall      (501) staff       (20)      381 2023-07-26 07:01:18.000000 kobo-md-0.1.3/src/kobo/resources/templates/index.html
+-rw-r--r--   0 dwall      (501) staff       (20)      375 2023-07-26 07:01:18.000000 kobo-md-0.1.3/src/kobo/resources/templates/page.html
+-rw-r--r--   0 dwall      (501) staff       (20)     2534 2023-07-26 07:39:13.000000 kobo-md-0.1.3/src/kobo/server.py
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.392977 kobo-md-0.1.3/src/kobo_md.egg-info/
+-rw-r--r--   0 dwall      (501) staff       (20)      760 2023-07-27 08:02:25.000000 kobo-md-0.1.3/src/kobo_md.egg-info/PKG-INFO
+-rw-r--r--   0 dwall      (501) staff       (20)      623 2023-07-27 08:02:25.000000 kobo-md-0.1.3/src/kobo_md.egg-info/SOURCES.txt
+-rw-r--r--   0 dwall      (501) staff       (20)        1 2023-07-27 08:02:25.000000 kobo-md-0.1.3/src/kobo_md.egg-info/dependency_links.txt
+-rw-r--r--   0 dwall      (501) staff       (20)       34 2023-07-27 08:02:25.000000 kobo-md-0.1.3/src/kobo_md.egg-info/requires.txt
+-rw-r--r--   0 dwall      (501) staff       (20)        5 2023-07-27 08:02:25.000000 kobo-md-0.1.3/src/kobo_md.egg-info/top_level.txt
```

### Comparing `kobo-md-0.1.2/LICENSE.txt` & `kobo-md-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.2/PKG-INFO` & `kobo-md-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kobo-md
-Version: 0.1.2
+Version: 0.1.3
 Summary: Markdown Compiler + Server
 Author: Dylan Wallace
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Kobo
```

### Comparing `kobo-md-0.1.2/README.md` & `kobo-md-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.2/setup.py` & `kobo-md-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 import setuptools
 import os
 import sys
 import pathlib
```

### Comparing `kobo-md-0.1.2/src/kobo/__main__.py` & `kobo-md-0.1.3/src/kobo/__main__.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.2/src/kobo/helper.py` & `kobo-md-0.1.3/src/kobo/helper.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.2/src/kobo/parser.py` & `kobo-md-0.1.3/src/kobo/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,16 @@
                 html_path = os.path.join(root, file).replace('.md', '.html')
 
                 if not route:
                     if file == 'index.md': # index -> parent dir should be the endpoint
                         route = os.path.relpath(root, contents_path)
                         if route == '.':
                             route = '/'
+                        elif not route.startswith('/'):
+                            route = '/' + route
                     else:
                         relpath = os.path.relpath(os.path.join(root, file), contents_path) #gets the "effective path"
                         route = '/' + relpath[:-3] # strip off the .md at the end
                 if not template:
                     if file == 'index.md':
                         template = 'index.html'
                     else:
```

### Comparing `kobo-md-0.1.2/src/kobo/resources/static/css/grid.css` & `kobo-md-0.1.3/src/kobo/resources/static/css/grid.css`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.2/src/kobo/resources/static/css/main.css` & `kobo-md-0.1.3/src/kobo/resources/static/css/main.css`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.2/src/kobo/server.py` & `kobo-md-0.1.3/src/kobo/server.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.2/src/kobo_md.egg-info/PKG-INFO` & `kobo-md-0.1.3/src/kobo_md.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kobo-md
-Version: 0.1.2
+Version: 0.1.3
 Summary: Markdown Compiler + Server
 Author: Dylan Wallace
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Kobo
```

### Comparing `kobo-md-0.1.2/src/kobo_md.egg-info/SOURCES.txt` & `kobo-md-0.1.3/src/kobo_md.egg-info/SOURCES.txt`

 * *Files identical despite different names*

