# Comparing `tmp/kobo-md-0.1.3.tar.gz` & `tmp/kobo-md-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kobo-md-0.1.3.tar", last modified: Thu Jul 27 08:02:25 2023, max compression
+gzip compressed data, was "kobo-md-0.1.4.tar", last modified: Thu Jul 27 09:18:52 2023, max compression
```

## Comparing `kobo-md-0.1.3.tar` & `kobo-md-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.393062 kobo-md-0.1.3/
--rw-r--r--   0 dwall      (501) staff       (20)     1086 2023-07-26 20:39:20.000000 kobo-md-0.1.3/LICENSE.txt
--rw-r--r--   0 dwall      (501) staff       (20)       46 2023-07-27 04:51:30.000000 kobo-md-0.1.3/MANIFEST.in
--rw-r--r--   0 dwall      (501) staff       (20)      760 2023-07-27 08:02:25.393109 kobo-md-0.1.3/PKG-INFO
--rw-r--r--   0 dwall      (501) staff       (20)      561 2023-07-26 21:02:59.000000 kobo-md-0.1.3/README.md
--rw-r--r--   0 dwall      (501) staff       (20)      106 2023-07-27 08:02:25.393273 kobo-md-0.1.3/setup.cfg
--rw-r--r--   0 dwall      (501) staff       (20)      820 2023-07-27 08:02:05.000000 kobo-md-0.1.3/setup.py
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.389144 kobo-md-0.1.3/src/
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.391086 kobo-md-0.1.3/src/kobo/
--rw-r--r--   0 dwall      (501) staff       (20)       42 2023-07-27 05:04:42.000000 kobo-md-0.1.3/src/kobo/__init__.py
--rw-r--r--   0 dwall      (501) staff       (20)     1770 2023-07-26 08:44:52.000000 kobo-md-0.1.3/src/kobo/__main__.py
--rw-r--r--   0 dwall      (501) staff       (20)      791 2023-07-26 08:48:12.000000 kobo-md-0.1.3/src/kobo/helper.py
--rw-r--r--   0 dwall      (501) staff       (20)     6378 2023-07-27 08:01:33.000000 kobo-md-0.1.3/src/kobo/parser.py
--rw-r--r--   0 dwall      (501) staff       (20)      344 2023-07-26 07:12:37.000000 kobo-md-0.1.3/src/kobo/redirects.py
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.389080 kobo-md-0.1.3/src/kobo/resources/
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.391313 kobo-md-0.1.3/src/kobo/resources/content/
--rw-r--r--   0 dwall      (501) staff       (20)       94 2023-07-26 08:39:44.000000 kobo-md-0.1.3/src/kobo/resources/content/index.md
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.389016 kobo-md-0.1.3/src/kobo/resources/static/
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.391726 kobo-md-0.1.3/src/kobo/resources/static/css/
--rw-r--r--   0 dwall      (501) staff       (20)     2527 2023-07-26 07:01:14.000000 kobo-md-0.1.3/src/kobo/resources/static/css/grid.css
--rw-r--r--   0 dwall      (501) staff       (20)      608 2023-07-26 07:01:14.000000 kobo-md-0.1.3/src/kobo/resources/static/css/main.css
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.392454 kobo-md-0.1.3/src/kobo/resources/templates/
--rw-r--r--   0 dwall      (501) staff       (20)      296 2023-07-26 07:01:18.000000 kobo-md-0.1.3/src/kobo/resources/templates/404.html
--rw-r--r--   0 dwall      (501) staff       (20)      383 2023-07-26 07:01:18.000000 kobo-md-0.1.3/src/kobo/resources/templates/index-list.html
--rw-r--r--   0 dwall      (501) staff       (20)      381 2023-07-26 07:01:18.000000 kobo-md-0.1.3/src/kobo/resources/templates/index.html
--rw-r--r--   0 dwall      (501) staff       (20)      375 2023-07-26 07:01:18.000000 kobo-md-0.1.3/src/kobo/resources/templates/page.html
--rw-r--r--   0 dwall      (501) staff       (20)     2534 2023-07-26 07:39:13.000000 kobo-md-0.1.3/src/kobo/server.py
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 08:02:25.392977 kobo-md-0.1.3/src/kobo_md.egg-info/
--rw-r--r--   0 dwall      (501) staff       (20)      760 2023-07-27 08:02:25.000000 kobo-md-0.1.3/src/kobo_md.egg-info/PKG-INFO
--rw-r--r--   0 dwall      (501) staff       (20)      623 2023-07-27 08:02:25.000000 kobo-md-0.1.3/src/kobo_md.egg-info/SOURCES.txt
--rw-r--r--   0 dwall      (501) staff       (20)        1 2023-07-27 08:02:25.000000 kobo-md-0.1.3/src/kobo_md.egg-info/dependency_links.txt
--rw-r--r--   0 dwall      (501) staff       (20)       34 2023-07-27 08:02:25.000000 kobo-md-0.1.3/src/kobo_md.egg-info/requires.txt
--rw-r--r--   0 dwall      (501) staff       (20)        5 2023-07-27 08:02:25.000000 kobo-md-0.1.3/src/kobo_md.egg-info/top_level.txt
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 09:18:52.749080 kobo-md-0.1.4/
+-rw-r--r--   0 dwall      (501) staff       (20)     1086 2023-07-26 20:39:20.000000 kobo-md-0.1.4/LICENSE.txt
+-rw-r--r--   0 dwall      (501) staff       (20)       46 2023-07-27 04:51:30.000000 kobo-md-0.1.4/MANIFEST.in
+-rw-r--r--   0 dwall      (501) staff       (20)      759 2023-07-27 09:18:52.749225 kobo-md-0.1.4/PKG-INFO
+-rw-r--r--   0 dwall      (501) staff       (20)      560 2023-07-27 09:18:45.000000 kobo-md-0.1.4/README.md
+-rw-r--r--   0 dwall      (501) staff       (20)      106 2023-07-27 09:18:52.749481 kobo-md-0.1.4/setup.cfg
+-rw-r--r--   0 dwall      (501) staff       (20)      820 2023-07-27 09:18:45.000000 kobo-md-0.1.4/setup.py
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 09:18:52.744572 kobo-md-0.1.4/src/
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 09:18:52.746441 kobo-md-0.1.4/src/kobo/
+-rw-r--r--   0 dwall      (501) staff       (20)       42 2023-07-27 05:04:42.000000 kobo-md-0.1.4/src/kobo/__init__.py
+-rw-r--r--   0 dwall      (501) staff       (20)     1780 2023-07-27 09:18:45.000000 kobo-md-0.1.4/src/kobo/__main__.py
+-rw-r--r--   0 dwall      (501) staff       (20)      791 2023-07-26 08:48:12.000000 kobo-md-0.1.4/src/kobo/helper.py
+-rw-r--r--   0 dwall      (501) staff       (20)     6378 2023-07-27 08:01:33.000000 kobo-md-0.1.4/src/kobo/parser.py
+-rw-r--r--   0 dwall      (501) staff       (20)      344 2023-07-26 07:12:37.000000 kobo-md-0.1.4/src/kobo/redirects.py
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 09:18:52.744518 kobo-md-0.1.4/src/kobo/resources/
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 09:18:52.746713 kobo-md-0.1.4/src/kobo/resources/content/
+-rw-r--r--   0 dwall      (501) staff       (20)       94 2023-07-26 08:39:44.000000 kobo-md-0.1.4/src/kobo/resources/content/index.md
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 09:18:52.744464 kobo-md-0.1.4/src/kobo/resources/static/
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 09:18:52.747125 kobo-md-0.1.4/src/kobo/resources/static/css/
+-rw-r--r--   0 dwall      (501) staff       (20)     2527 2023-07-26 07:01:14.000000 kobo-md-0.1.4/src/kobo/resources/static/css/grid.css
+-rw-r--r--   0 dwall      (501) staff       (20)      608 2023-07-26 07:01:14.000000 kobo-md-0.1.4/src/kobo/resources/static/css/main.css
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 09:18:52.747934 kobo-md-0.1.4/src/kobo/resources/templates/
+-rw-r--r--   0 dwall      (501) staff       (20)      296 2023-07-26 07:01:18.000000 kobo-md-0.1.4/src/kobo/resources/templates/404.html
+-rw-r--r--   0 dwall      (501) staff       (20)      383 2023-07-26 07:01:18.000000 kobo-md-0.1.4/src/kobo/resources/templates/index-list.html
+-rw-r--r--   0 dwall      (501) staff       (20)      381 2023-07-26 07:01:18.000000 kobo-md-0.1.4/src/kobo/resources/templates/index.html
+-rw-r--r--   0 dwall      (501) staff       (20)      375 2023-07-26 07:01:18.000000 kobo-md-0.1.4/src/kobo/resources/templates/page.html
+-rw-r--r--   0 dwall      (501) staff       (20)     2534 2023-07-27 09:18:45.000000 kobo-md-0.1.4/src/kobo/server.py
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-27 09:18:52.748962 kobo-md-0.1.4/src/kobo_md.egg-info/
+-rw-r--r--   0 dwall      (501) staff       (20)      759 2023-07-27 09:18:52.000000 kobo-md-0.1.4/src/kobo_md.egg-info/PKG-INFO
+-rw-r--r--   0 dwall      (501) staff       (20)      623 2023-07-27 09:18:52.000000 kobo-md-0.1.4/src/kobo_md.egg-info/SOURCES.txt
+-rw-r--r--   0 dwall      (501) staff       (20)        1 2023-07-27 09:18:52.000000 kobo-md-0.1.4/src/kobo_md.egg-info/dependency_links.txt
+-rw-r--r--   0 dwall      (501) staff       (20)       34 2023-07-27 09:18:52.000000 kobo-md-0.1.4/src/kobo_md.egg-info/requires.txt
+-rw-r--r--   0 dwall      (501) staff       (20)        5 2023-07-27 09:18:52.000000 kobo-md-0.1.4/src/kobo_md.egg-info/top_level.txt
```

### Comparing `kobo-md-0.1.3/LICENSE.txt` & `kobo-md-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.3/PKG-INFO` & `kobo-md-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kobo-md
-Version: 0.1.3
+Version: 0.1.4
 Summary: Markdown Compiler + Server
 Author: Dylan Wallace
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Kobo
@@ -12,14 +12,14 @@
 
 # Features
 - Built with Flask
 - Native support for markdown using katex
 - No customization -> forced to use the best web theme you've ever seen
 
 # Installation
-1. Run `python3 -m pip install katex-md`
+1. Run `python3 -m pip install kobo-md`
 2. Install katex via `npm install katex`
 
 # Usage
 - To start a new project, simply enter the target directory and run `python3 -m katex new`.
 - To run the server, run `python3 -m katex server` from the project directory.
 - To compile markdown files into html snippets, run `python3 -m katex compile`.
```

### Comparing `kobo-md-0.1.3/README.md` & `kobo-md-0.1.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 
 # Features
 - Built with Flask
 - Native support for markdown using katex
 - No customization -> forced to use the best web theme you've ever seen
 
 # Installation
-1. Run `python3 -m pip install katex-md`
+1. Run `python3 -m pip install kobo-md`
 2. Install katex via `npm install katex`
 
 # Usage
 - To start a new project, simply enter the target directory and run `python3 -m katex new`.
 - To run the server, run `python3 -m katex server` from the project directory.
 - To compile markdown files into html snippets, run `python3 -m katex compile`.
```

### Comparing `kobo-md-0.1.3/setup.py` & `kobo-md-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 
 import setuptools
 import os
 import sys
 import pathlib
```

### Comparing `kobo-md-0.1.3/src/kobo/__main__.py` & `kobo-md-0.1.4/src/kobo/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from . import server
 
 # Global vars
 
 CWD = Path.cwd()
 CONTENT_PATH, TEMPLATES_PATH, STATIC_PATH, REDIRECTS_PATH, FROZEN_PATH = helper.gen_paths(CWD)
 INTERNAL_TEMPLATES_PATH = Path(__file__).parent / 'resources' / 'templates'
-INTERNAL_STATIC_PATH = Path(__file__).parent / 'resources' / 'templates'
+INTERNAL_STATIC_PATH = Path(__file__).parent / 'resources' / 'static'
 INTERNAL_CONTENT_PATH = Path(__file__).parent / 'resources' / 'content'
 
 # Parser setup
 
 argparser = argparse.ArgumentParser(
     prog='kobo'
 )
@@ -42,11 +42,13 @@
     server_app = server.create_server(CWD, **kwargs)
     if not args.gunicorn:
         port = args.port if args.port else 8000
         server_app.run('0.0.0.0', port=port)
     else:
         pass #TODO Implement running gunicorn
 
+    exit(0)
+
 if args.command == 'compile':
     parser.parse_tree_save(CONTENT_PATH, FROZEN_PATH)
     print('Saved routes to `%s`' % str(FROZEN_PATH))
     exit(0)
```

### Comparing `kobo-md-0.1.3/src/kobo/helper.py` & `kobo-md-0.1.4/src/kobo/helper.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.3/src/kobo/parser.py` & `kobo-md-0.1.4/src/kobo/parser.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.3/src/kobo/resources/static/css/grid.css` & `kobo-md-0.1.4/src/kobo/resources/static/css/grid.css`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.3/src/kobo/resources/static/css/main.css` & `kobo-md-0.1.4/src/kobo/resources/static/css/main.css`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.3/src/kobo/server.py` & `kobo-md-0.1.4/src/kobo/server.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1.3/src/kobo_md.egg-info/PKG-INFO` & `kobo-md-0.1.4/src/kobo_md.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kobo-md
-Version: 0.1.3
+Version: 0.1.4
 Summary: Markdown Compiler + Server
 Author: Dylan Wallace
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Kobo
@@ -12,14 +12,14 @@
 
 # Features
 - Built with Flask
 - Native support for markdown using katex
 - No customization -> forced to use the best web theme you've ever seen
 
 # Installation
-1. Run `python3 -m pip install katex-md`
+1. Run `python3 -m pip install kobo-md`
 2. Install katex via `npm install katex`
 
 # Usage
 - To start a new project, simply enter the target directory and run `python3 -m katex new`.
 - To run the server, run `python3 -m katex server` from the project directory.
 - To compile markdown files into html snippets, run `python3 -m katex compile`.
```

### Comparing `kobo-md-0.1.3/src/kobo_md.egg-info/SOURCES.txt` & `kobo-md-0.1.4/src/kobo_md.egg-info/SOURCES.txt`

 * *Files identical despite different names*

