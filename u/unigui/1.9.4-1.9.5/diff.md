# Comparing `tmp/unigui-1.9.4.tar.gz` & `tmp/unigui-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.9.4.tar", last modified: Wed Jul 26 16:10:40 2023, max compression
+gzip compressed data, was "dist/unigui-1.9.5.tar", last modified: Thu Jul 27 17:34:48 2023, max compression
```

## Comparing `unigui-1.9.4.tar` & `unigui-1.9.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     5250 2023-07-26 02:29:57.000000 unigui-1.9.4/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3558 2023-07-26 08:55:15.000000 unigui-1.9.4/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)     4299 2023-07-25 09:16:10.000000 unigui-1.9.4/unigui/tables.py
--rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.4/unigui/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)     7362 2023-07-26 09:52:46.000000 unigui-1.9.4/unigui/autotest.py
--rw-r--r--   0 george    (1000) george    (1000)     2623 2023-07-24 13:07:39.000000 unigui-1.9.4/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     5565 2023-07-24 17:13:07.000000 unigui-1.9.4/unigui/reloader.py
--rw-rw-r--   0 george    (1000) george    (1000)     8713 2023-07-26 09:11:50.000000 unigui-1.9.4/unigui/users.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/css/vendor.f747ec02.css
--rw-rw-r--   0 george    (1000) george    (1000)     2750 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/css/750.ca964e27.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)  1436034 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/js/vendor.5659ce27.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/js/app.df555111.js
--rw-rw-r--   0 george    (1000) george    (1000)    48813 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/js/750.4831ed09.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.4/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      642 2023-07-26 16:04:11.000000 unigui-1.9.4/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19239 2023-07-26 16:10:40.000000 unigui-1.9.4/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-26 16:10:40.000000 unigui-1.9.4/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18934 2023-07-17 14:52:22.000000 unigui-1.9.4/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.4/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       63 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19239 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.4/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1258 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     5250 2023-07-26 02:29:57.000000 unigui-1.9.5/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3531 2023-07-26 16:18:00.000000 unigui-1.9.5/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4299 2023-07-25 09:16:10.000000 unigui-1.9.5/unigui/tables.py
+-rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.5/unigui/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7370 2023-07-26 17:26:22.000000 unigui-1.9.5/unigui/autotest.py
+-rw-r--r--   0 george    (1000) george    (1000)     2642 2023-07-26 17:28:06.000000 unigui-1.9.5/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5573 2023-07-26 17:26:38.000000 unigui-1.9.5/unigui/reloader.py
+-rw-rw-r--   0 george    (1000) george    (1000)     8713 2023-07-26 09:11:50.000000 unigui-1.9.5/unigui/users.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)     2750 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/css/982.c7dd083b.css
+-rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/css/vendor.f747ec02.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)  1436034 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/js/vendor.5659ce27.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)    49159 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/js/982.872ac96a.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/js/app.6805317c.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-27 17:29:44.000000 unigui-1.9.5/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.5/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      642 2023-07-27 17:33:52.000000 unigui-1.9.5/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    18810 2023-07-27 17:34:48.000000 unigui-1.9.5/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-27 17:34:48.000000 unigui-1.9.5/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18505 2023-07-27 09:01:10.000000 unigui-1.9.5/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.5/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       63 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    18810 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.5/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1258 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-27 17:34:48.000000 unigui-1.9.5/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.9.4/unigui/guielements.py` & `unigui-1.9.5/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/server.py` & `unigui-1.9.5/unigui/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from aiohttp import web, WSMsgType
 from .users import *
 from pathlib import Path
 from .reloader import empty_app 
 from .autotest import recorder, jsonString, run_tests
 from config import port, upload_dir
-from .utils import app_dir
 import traceback
 
 async def post_handler(request):
     reader = await request.multipart()
     field = await reader.next()   
     filename = upload_path(field.filename)      
     size = 0
```

### Comparing `unigui-1.9.4/unigui/tables.py` & `unigui-1.9.5/unigui/tables.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/autotest.py` & `unigui-1.9.5/unigui/autotest.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 def button_clicked(_,__):
     test_name.value = ''
     test_name.complete = smart_complete(os.listdir(testdir))
     return Dialog('Create autotest..', ask_create_test, test_name, rewrite)
 
 def create_test(fname):
-    fname = f'{testdir}/{fname}'    
+    fname = f'{testdir}{divpath}{fname}'    
     if os.path.exists(fname) and not rewrite.value:
         return Warning(f'Test file {fname} already exists!')              
     
     button.mode = 'red'   
     button.tooltip = 'Stop test recording'
     button.changed = recorder.stop_recording
     recorder.start(fname)
```

### Comparing `unigui-1.9.4/unigui/utils.py` & `unigui-1.9.5/unigui/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os, jsonpickle, json, platform, requests
 
 blocks_dir = 'blocks'        
 screens_dir =  'screens'        
 UpdateScreen = True
 
+divpath = '\\' if platform.system() == 'Windows' else '/'
 libpath = os.path.dirname(os.path.realpath(__file__))
-webpath = libpath + '/web' 
+webpath = f'{libpath}{divpath}web' 
 app_dir = os.getcwd()
-divpath = '\\' if platform.system() == 'Windows' else '/'
 
 try:
     import config
 except:
     with open('config.py', 'w') as f:        
         f.write("""port = 8000 
 upload_dir = 'web'
@@ -45,15 +45,15 @@
     for a in arr:
         if isinstance(a, list):
             yield from flatten(*a)
         else:
             yield a
     
 def cache_url(url):
-    "cache url file in upload_dir snd returns local file"""
+    """cache url file in upload_dir and returns the local file name"""
     fname = url2filename(url)   
     fname = upload_path(fname)
     response = requests.get(url)
     if response.status_code != 200:
         return None
     file = open(fname, "wb")
     file.write(response.content)
```

### Comparing `unigui-1.9.4/unigui/reloader.py` & `unigui-1.9.5/unigui/reloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         def on_deleted(self, event):            
             if not event.is_directory and User.last_user:
                 user = User.last_user            
                 arr = event.src_path.split(divpath) 
                 name = arr[-1]
                 dir = arr[-2]  
                 if name.endswith('.py') and dir == 'screens':
-                    delfile = f'{dir}/{name}'
+                    delfile = f'{dir}{divpath}{name}'
                     for i, s in enumerate(user.screens):
                         if s.__file__ == delfile:
                             user.screens.remove(s)
                             if user.screen_module is s:
                                 if user.screens:                                                                        
                                     fname = user.screens[0].__file__.split(divpath)[-1]
                                     module = reload(fname)
```

### Comparing `unigui-1.9.4/unigui/users.py` & `unigui-1.9.5/unigui/users.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/favicon.ico` & `unigui-1.9.5/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/css/vendor.f747ec02.css` & `unigui-1.9.5/unigui/web/css/vendor.f747ec02.css`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/css/750.ca964e27.css` & `unigui-1.9.5/unigui/web/css/982.c7dd083b.css`

 * *Files 18% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-thumb-hover:#2176d2;--scrollbar-thumb-dark:#2176d2;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.chart-container[data-v-12be25e8]{height:400px;width:400px}body[data-v-5682537f]{display:flex;justify-content:center}.custom-caption[data-v-5682537f]{padding:5px!important}.web-camera-container[data-v-5682537f]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-5682537f]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-5682537f]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-5682537f]{opacity:1}.web-camera-container .camera-shoot[data-v-5682537f]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-5682537f]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-5682537f]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-5682537f]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-5682537f]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-5682537f]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-5682537f]{animation:preload-5682537f 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-5682537f]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-5682537f]:nth-child(3){animation-delay:.4s}@keyframes preload-5682537f{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.q-tab__label{font-size:16px;font-weight:700}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-thumb-hover:#2176d2;--scrollbar-thumb-dark:#2176d2;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.chart-container[data-v-12be25e8]{height:400px;width:400px}body[data-v-206674a7]{display:flex;justify-content:center}.custom-caption[data-v-206674a7]{padding:5px!important}.web-camera-container[data-v-206674a7]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-206674a7]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-206674a7]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-206674a7]{opacity:1}.web-camera-container .camera-shoot[data-v-206674a7]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-206674a7]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-206674a7]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-206674a7]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-206674a7]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-206674a7]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-206674a7]{animation:preload-206674a7 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-206674a7]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-206674a7]:nth-child(3){animation-delay:.4s}@keyframes preload-206674a7{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.q-tab__label{font-size:16px;font-weight:700}
```

### Comparing `unigui-1.9.4/unigui/web/icons/favicon-96x96.png` & `unigui-1.9.5/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/icons/favicon-16x16.png` & `unigui-1.9.5/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/icons/favicon-32x32.png` & `unigui-1.9.5/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/icons/favicon-128x128.png` & `unigui-1.9.5/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `unigui-1.9.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.9.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.9.5/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.9.5/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.9.5/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/js/vendor.5659ce27.js` & `unigui-1.9.5/unigui/web/js/vendor.5659ce27.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/js/430.591e9a73.js` & `unigui-1.9.5/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/js/app.df555111.js` & `unigui-1.9.5/unigui/web/js/app.6805317c.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(750)]).then(r.bind(r, 8750)),
+                        component: () => Promise.all([r.e(736), r.e(982)]).then(r.bind(r, 9982)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -164,24 +164,24 @@
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, o) => (r.f[o](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
             430: "591e9a73",
-            750: "4831ed09"
+            982: "872ac96a"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
             736: "f747ec02",
-            750: "ca964e27"
+            982: "c7dd083b"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -264,15 +264,15 @@
                 e(o, l, n, a)
             })),
             n = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                750: 1
+                982: 1
             };
             n[e] ? t.push(n[e]) : 0 !== n[e] && r[e] && t.push(n[e] = o(e).then((() => {
                 n[e] = 0
             }), (t => {
                 throw delete n[e], t
             })))
         }
```

### Comparing `unigui-1.9.4/unigui/web/js/750.4831ed09.js` & `unigui-1.9.5/unigui/web/js/982.872ac96a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [750], {
-        8750: (e, t, a) => {
+    [982], {
+        9982: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => sa
             });
             var s = a(3673),
                 l = a(2323);
             const i = (0, s._)("div", {
                     class: "q-pa-md"
@@ -15,16 +15,16 @@
                 }, null, -1);
 
             function o(e, t, a, o, d, r) {
                 const c = (0, s.up)("q-item-label"),
                     h = (0, s.up)("element"),
                     u = (0, s.up)("q-tab"),
                     p = (0, s.up)("q-tabs"),
-                    m = (0, s.up)("q-space"),
-                    g = (0, s.up)("q-tooltip"),
+                    g = (0, s.up)("q-space"),
+                    m = (0, s.up)("q-tooltip"),
                     f = (0, s.up)("q-btn"),
                     y = (0, s.up)("q-toolbar"),
                     w = (0, s.up)("q-header"),
                     b = (0, s.up)("zone"),
                     k = (0, s.up)("q-page"),
                     v = (0, s.up)("q-page-container"),
                     x = (0, s.up)("q-layout");
@@ -74,22 +74,22 @@
                                     class: "justify-center text-white shadow-2",
                                     "no-caps": "",
                                     name: t.name,
                                     label: t.name,
                                     onClick: a => e.tabclick(t.name)
                                 }, null, 8, ["name", "label", "onClick"]))])))), 256))])),
                                 _: 1
-                            }, 8, ["modelValue"]), (0, s.Wm)(m), (0, s.Wm)(f, {
+                            }, 8, ["modelValue"]), (0, s.Wm)(g), (0, s.Wm)(f, {
                                 "no-caps": "",
                                 dense: "",
                                 round: "",
                                 icon: e.Dark.isActive ? "light_mode" : "dark_mode",
                                 onClick: e.switchTheme
                             }, {
-                                default: (0, s.w5)((() => [(0, s.Wm)(g, {
+                                default: (0, s.w5)((() => [(0, s.Wm)(m, {
                                     class: "text-body2"
                                 }, {
                                     default: (0, s.w5)((() => [(0, s.Uk)("Dark/Light mode")])),
                                     _: 1
                                 })])),
                                 _: 1
                             }, 8, ["icon", "onClick"])])),
@@ -144,48 +144,48 @@
             }
             a(71);
             var r = a(698),
                 c = a(8603);
             let h = null,
                 u = {};
             var p;
-            let m = !0;
-            const g = ["graph", "docviewer", "linechart", "block"];
-            const f = window.location.host,
-                y = `${window.location.protocol}//${f}`,
-                w = !1;
+            const g = !1;
+            let m = g;
+            const f = ["graph", "docviewer", "linechart", "block"];
+            const y = window.location.host,
+                w = `${window.location.protocol}//${y}`;
             let b = {},
                 k = {},
                 v = {};
 
             function C(e) {
-                p = new WebSocket(w ? "ws://localhost:8000/ws" : `ws://${f}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
-                    m && console.log("incoming message", t.data), e.processMessage(JSON.parse(t.data))
+                p = new WebSocket(g ? "ws://localhost:8000/ws" : `ws://${y}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
+                    m && console.log("incoming message", t.data), h.designCycle = 0, e.processMessage(JSON.parse(t.data))
                 }, p.onerror = t => e.error(t), p.onclose = t => {
                     t.wasClean ? e.info("Connection was finished by the server.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, m && console.info("close code : " + t.code + " reason: " + t.reason)
                 }, h = e
             }
 
             function _(e) {
-                console.log("sended", e), p.send(JSON.stringify(e))
+                m && console.log("sended", e), p.send(JSON.stringify(e))
             }
             let q = 0,
                 A = !0;
 
             function D(e) {
                 A = e, e || (v = {})
             }
 
             function S(e) {
                 if (A) {
                     let t = v[e.fullname];
                     if (t) return t.styleSize;
                     A = !1
                 }
-                return ""
+                return null
             }
 
             function j(e, t, a, s = "complete") {
                 let l = ++q,
                     i = [e.pdata.name, e.data.name, s, t, l];
                 _(i), u[l] = a
             }
@@ -194,56 +194,66 @@
                 b = {}, v = k, A = !0, k = {}
             }
 
             function Z(e, t) {
                 Object.assign(e.data, t), e.updated = t.value, e.value = t.value
             }
 
-            function M(e) {
+            function $(e) {
                 for (let t of e) {
                     let e = t.path;
                     if (e.length > 1) {
                         e.reverse();
                         let a = e.join("@"),
                             s = k[a];
                         Z(s, t.data)
                     } else {
                         let a = b[e[0]];
                         Object.assign(a.data, t.data)
                     }
                 }
             }
 
-            function $(e) {
+            function M(e) {
                 "string" == typeof e.value ? h.error(e.value) : u[e.id](e.value), delete u[e.id]
             }
 
             function W(e) {
                 let t = [];
                 for (let s of e) s instanceof Array ? t.push(s) : t.push([s]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
             function V(e = !1) {
-                for (let [t, a] of Object.entries(k)) !a.expanding || e && !g.includes(a.type) || (a.styleSize = "");
-                (0, s.Y3)((() => {
-                    requestAnimationFrame((() => {
+                for (let t of Object.values(k))
+                    if (t.expanding && (!e || f.includes(t.type))) {
+                        t.has_recalc = !0;
+                        let e = t.$el;
+                        if (e.getBoundingClientRect) {
+                            let e = t.$el.getBoundingClientRect();
+                            window.innerHeight < e.top + e.height && (t.styleSize = "")
+                        }
+                    }(0, s.Y3)((() => {
                         requestAnimationFrame((() => {
-                            K(document.documentElement.scrollWidth > window.innerWidth)
+                            requestAnimationFrame((() => {
+                                requestAnimationFrame((() => {
+                                    K(document.documentElement.scrollWidth > window.innerWidth)
+                                }))
+                            }))
                         }))
                     }))
-                }))
             }
-            let E = (0, c.debounce)(V, 200);
+            let E = (0, c.debounce)(V, 100);
 
             function K(e) {
-                m && console.log("------------------recalc design");
-                const t = Q(e),
-                    a = H(e);
+                if (m && console.log(`------------------recalc design ${h.designCycle}`), h.designCycle >= 3) return;
+                h.designCycle++;
+                const t = H(e),
+                    a = Q(e);
                 for (let [s, l] of Object.entries(t)) {
                     let t = k[s],
                         i = a[s];
                     const [n, o] = i || [0, 1];
                     let d, r = t.geom(),
                         c = r.el,
                         h = t.pdata ? t.pdata.name : t.name,
@@ -258,24 +268,24 @@
                             }
                         } else if (e.name == t.data.name) {
                         d = t;
                         break
                     }
                     let p = n;
                     p /= o;
-                    let m = e || g.includes(t.type);
-                    if (m || "" == t.styleSize) {
-                        let e = m ? `width:${Math.ceil(c.clientWidth+p)}px` : "",
-                            a = s.startsWith("_scroll@") ? r.inner.clientHeight : c.clientHeight;
-                        a < 0 && (a = 20), t.styleSize = `height: ${a+l}px; ${e}`
-                    }
+                    let g = e || f.includes(t.type) || t.has_recalc,
+                        m = g ? `width:${Math.ceil(c.clientWidth+p)}px` : "",
+                        y = s.startsWith("_scroll@") ? r.inner.clientHeight : c.clientHeight;
+                    y < 0 && (y = 20);
+                    let w = `height: ${y+l}px; ${m}`;
+                    w != t.styleSize && (t.styleSize = w), t.has_recalc = !1
                 }
             }
 
-            function Q(e) {
+            function H(e) {
                 const t = h.screen.blocks;
                 let a = window.innerHeight;
                 a += 14;
                 let s = {},
                     l = new Map,
                     i = {};
                 for (let [d, r] of Object.entries(b)) i[r.name] = r.$el.getBoundingClientRect().height;
@@ -338,15 +348,15 @@
                 }
                 let o = Array.from(l.entries());
                 o.sort(((e, t) => e[0] in s || e[1] in s ? -1 : 1));
                 for (let [d, r] of o) r in s ? s[d] = s[r] : s[r] = s[d];
                 return s
             }
 
-            function H(e) {
+            function Q(e) {
                 let t = null;
                 const a = t ? [t] : h.screen.blocks;
                 let s = window.innerWidth - 15,
                     l = [],
                     i = {};
                 for (let d of a)
                     if (0 == l.length)
@@ -371,15 +381,15 @@
                     let t = Array.isArray(d) ? d[d.length - 1] : d,
                         a = b[t.name].$el.getBoundingClientRect().right;
                     t = Array.isArray(d) ? d[0] : d;
                     let l = b[t.name].$el.getBoundingClientRect().left,
                         i = s - a + l - 10;
                     const r = [];
                     for (let [s, n] of Object.entries(k))
-                        if (n.expanding_width && (n.fullname.startsWith("_scroll@") || e || g.includes(n.type))) {
+                        if (n.expanding_width && (n.fullname.startsWith("_scroll@") || e || f.includes(n.type))) {
                             let e = s.split("@")[1];
                             if (d.find((t => t.name == e))) {
                                 let e = !0,
                                     t = n.geom().left;
                                 for (let [a, s] of r.entries())
                                     if (s !== n && s.geom().left == t) {
                                         s.geom().scrollWidth < n.geom().scrollWidth ? (r[a] = n, o.set(s.fullname, n.fullname)) : o.set(n.fullname, s.fullname), e = !1;
@@ -440,27 +450,27 @@
                         type: String,
                         default: ""
                     }
                 }
             });
             var U = a(4260),
                 N = a(3414),
-                T = a(2035),
-                F = a(4554),
+                F = a(2035),
+                T = a(4554),
                 P = a(2350),
-                I = a(7518),
-                R = a.n(I);
+                R = a(7518),
+                I = a.n(R);
             const L = (0, U.Z)(O, [
                     ["render", d]
                 ]),
                 B = L;
-            R()(O, "components", {
+            I()(O, "components", {
                 QItem: N.Z,
-                QItemSection: T.Z,
-                QIcon: F.Z,
+                QItemSection: F.Z,
+                QIcon: T.Z,
                 QItemLabel: P.Z
             });
             const Y = {
                     key: 0,
                     class: "row q-col-gutter-xs q-py-xs"
                 },
                 X = {
@@ -568,15 +578,15 @@
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"]))], 8, se)))), 256))])),
                     _: 1
                 }, 8, ["style"])
             }
             var ne = a(8880);
-            const oe = e => ((0, s.dD)("data-v-5682537f"), e = e(), (0, s.Cn)(), e),
+            const oe = e => ((0, s.dD)("data-v-206674a7"), e = e(), (0, s.Cn)(), e),
                 de = {
                     key: 4,
                     class: "{'bg-blue-grey-9': Dark.isActive}"
                 },
                 re = ["width", "height"],
                 ce = ["src"],
                 he = {
@@ -585,18 +595,18 @@
                 },
                 ue = {
                     class: "camera-button"
                 },
                 pe = {
                     key: 0
                 },
-                me = {
+                ge = {
                     key: 1
                 },
-                ge = {
+                me = {
                     class: "camera-loading"
                 },
                 fe = oe((() => (0, s._)("ul", {
                     class: "loader-circle"
                 }, [(0, s._)("li"), (0, s._)("li"), (0, s._)("li")], -1))),
                 ye = [fe],
                 we = ["height"],
@@ -617,16 +627,16 @@
             function _e(e, t, a, i, n, o) {
                 const d = (0, s.up)("q-icon"),
                     r = (0, s.up)("q-img"),
                     c = (0, s.up)("q-badge"),
                     h = (0, s.up)("q-select"),
                     u = (0, s.up)("q-checkbox"),
                     p = (0, s.up)("q-toggle"),
-                    m = (0, s.up)("q-btn"),
-                    g = (0, s.up)("q-btn-toggle"),
+                    g = (0, s.up)("q-btn"),
+                    m = (0, s.up)("q-btn-toggle"),
                     f = (0, s.up)("utable"),
                     y = (0, s.up)("linechart"),
                     w = (0, s.up)("q-input"),
                     b = (0, s.up)("q-tree"),
                     k = (0, s.up)("q-scroll-area"),
                     v = (0, s.up)("q-separator"),
                     x = (0, s.up)("q-uploader"),
@@ -688,22 +698,22 @@
                 }, null, 8, ["modelValue", "label"])) : "switch" == e.type ? ((0, s.wg)(), (0, s.j4)(p, {
                     key: 3,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[3] || (t[3] = t => e.value = t),
                     color: "primary",
                     label: e.nameLabel,
                     "left-label": ""
-                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, s.wg)(), (0, s.iD)("div", de, [e.showname ? ((0, s.wg)(), (0, s.j4)(m, {
+                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, s.wg)(), (0, s.iD)("div", de, [e.showname ? ((0, s.wg)(), (0, s.j4)(g, {
                     key: 0,
                     ripple: !1,
                     color: "indigo-10",
                     disable: "",
                     label: e.name,
                     "no-caps": ""
-                }, null, 8, ["label"])) : (0, s.kq)("", !0), (0, s.Wm)(g, {
+                }, null, 8, ["label"])) : (0, s.kq)("", !0), (0, s.Wm)(m, {
                     modelValue: e.value,
                     "onUpdate:modelValue": t[4] || (t[4] = t => e.value = t),
                     class: (0, l.C_)({
                         "bg-blue-grey-9": e.Dark.isActive
                     }),
                     "no-caps": "",
                     options: e.data.options.map((e => ({
@@ -836,15 +846,15 @@
                 }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, s.wg)(), (0, s.iD)("div", he, [(0, s._)("div", ue, [(0, s._)("button", {
                     class: (0, l.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", me, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", pe, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", ge, ye, 512), [
+                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", ge, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", pe, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", me, ye, 512), [
                     [ne.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, s.wy)(((0, s.wg)(), (0, s.iD)("div", {
                     key: 0,
                     class: (0, l.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, s._)("div", {
@@ -867,18 +877,18 @@
                     [ne.F8, e.isPhotoTaken]
                 ])], 2)), [
                     [ne.F8, !e.isLoading]
                 ]) : (0, s.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, s.wg)(), (0, s.iD)("div", ke, [(0, s._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[12] || (t[12] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, xe)])) : (0, s.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("div", Ce, [(0, s.Wm)(m, {
+                }, xe)])) : (0, s.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("div", Ce, [(0, s.Wm)(g, {
                     onClick: e.downloadImage,
                     label: "Send"
-                }, null, 8, ["onClick"])])) : (0, s.kq)("", !0)])) : "" != e.showname ? ((0, s.wg)(), (0, s.j4)(m, {
+                }, null, 8, ["onClick"])])) : (0, s.kq)("", !0)])) : "" != e.showname ? ((0, s.wg)(), (0, s.j4)(g, {
                     key: 18,
                     "no-caps": "",
                     class: (0, l.C_)({
                         "bg-blue-grey-9": e.Dark.isActive
                     }),
                     label: e.name,
                     icon: e.data.icon,
@@ -888,15 +898,15 @@
                         key: 0,
                         class: "text-body2"
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["class", "label", "icon", "onClick"])) : e.data.mode ? ((0, s.wg)(), (0, s.j4)(m, {
+                }, 8, ["class", "label", "icon", "onClick"])) : e.data.mode ? ((0, s.wg)(), (0, s.j4)(g, {
                     key: 20,
                     "no-caps": "",
                     dense: "",
                     round: "",
                     class: (0, l.C_)({
                         "bg-grey-9": e.Dark.isActive
                     }),
@@ -908,15 +918,15 @@
                         key: 0,
                         class: "text-body2"
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["class", "onClick"])) : ((0, s.wg)(), (0, s.j4)(m, {
+                }, 8, ["class", "onClick"])) : ((0, s.wg)(), (0, s.j4)(g, {
                     key: 19,
                     "no-caps": "",
                     dense: "",
                     round: "",
                     class: (0, l.C_)({
                         "bg-grey-9": e.Dark.isActive
                     }),
@@ -944,16 +954,16 @@
             function Se(e, t, a, i, n, o) {
                 const d = (0, s.up)("q-icon"),
                     r = (0, s.up)("q-tooltip"),
                     c = (0, s.up)("q-input"),
                     h = (0, s.up)("q-btn"),
                     u = (0, s.up)("q-th"),
                     p = (0, s.up)("q-tr"),
-                    m = (0, s.up)("q-checkbox"),
-                    g = (0, s.up)("q-select"),
+                    g = (0, s.up)("q-checkbox"),
+                    m = (0, s.up)("q-select"),
                     f = (0, s.up)("q-td"),
                     y = (0, s.up)("q-table");
                 return (0, s.wg)(), (0, s.j4)(y, {
                     "virtual-scroll": "",
                     dense: e.data.dense,
                     style: (0, l.j5)(e.styleSize),
                     flat: "",
@@ -1147,21 +1157,21 @@
                         props: t,
                         onClick: e => t.selected = !t.selected
                     }, {
                         default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.columns, ((a, i) => ((0, s.wg)(), (0, s.j4)(f, {
                             key: a.name,
                             props: t
                         }, {
-                            default: (0, s.w5)((() => ["boolean" == typeof t.row[a.name] ? ((0, s.wg)(), (0, s.j4)(m, {
+                            default: (0, s.w5)((() => ["boolean" == typeof t.row[a.name] ? ((0, s.wg)(), (0, s.j4)(g, {
                                 key: 0,
                                 modelValue: t.row[a.name],
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, s => e.change_switcher(t.row, a.name, i)],
                                 dense: "",
                                 disable: !e.editMode
-                            }, null, 8, ["modelValue", "onUpdate:modelValue", "disable"])) : e.editMode && "complete" in e.data && i == e.cedit && e.redit == t.row.iiid ? ((0, s.wg)(), (0, s.j4)(g, {
+                            }, null, 8, ["modelValue", "onUpdate:modelValue", "disable"])) : e.editMode && "complete" in e.data && i == e.cedit && e.redit == t.row.iiid ? ((0, s.wg)(), (0, s.j4)(m, {
                                 key: 1,
                                 dense: "",
                                 "model-value": t.row[a.name],
                                 "use-input": "",
                                 "hide-selected": "",
                                 "fill-input": "",
                                 autofocus: "",
@@ -1193,15 +1203,15 @@
             }
             var je = a(1959),
                 ze = a(9058);
 
             function Ze(e, t) {
                 return e.length === t.length && e.every(((e, a) => t[a] && e.iiid == t[a].iiid))
             }
-            const Me = (0, s.aZ)({
+            const $e = (0, s.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
                     } = (0, je.BK)(e);
                     let l = (0, s.Fl)((() => {
@@ -1407,52 +1417,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var $e = a(9267),
+            var Me = a(9267),
                 We = a(4842),
                 Ve = a(8870),
                 Ee = a(2165),
                 Ke = a(8186),
-                Qe = a(2414),
-                He = a(3884),
+                He = a(2414),
+                Qe = a(3884),
                 Oe = a(5735),
                 Ue = a(7208);
-            const Ne = (0, U.Z)(Me, [
+            const Ne = (0, U.Z)($e, [
                     ["render", Se]
                 ]),
-                Te = Ne;
-            R()(Me, "components", {
-                QTable: $e.Z,
+                Fe = Ne;
+            I()($e, "components", {
+                QTable: Me.Z,
                 QInput: We.Z,
-                QIcon: F.Z,
+                QIcon: T.Z,
                 QTooltip: Ve.Z,
                 QBtn: Ee.Z,
                 QTr: Ke.Z,
-                QTh: Qe.Z,
-                QTd: He.Z,
+                QTh: He.Z,
+                QTd: Qe.Z,
                 QCheckbox: Oe.Z,
                 QSelect: Ue.Z
             });
-            const Fe = ["nodes", "edges"];
+            const Te = ["nodes", "edges"];
 
             function Pe(e, t, a, i, n, o) {
                 return (0, s.wg)(), (0, s.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, l.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Fe)
+                }, null, 12, Te)
             }
-            var Ie = a(2393),
-                Re = a.n(Ie);
-            const Le = Re().stylesheet().selector("node").css({
+            var Re = a(2393),
+                Ie = a.n(Re);
+            const Le = Ie().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4",
                     "font-size": "14px"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555",
                     "font-size": "14px"
@@ -1513,15 +1523,15 @@
                         }
                     },
                     beforeUnmount() {
                         window.removeEventListener("keydown", this.handleKeyDown), window.removeEventListener("keyup", this.handleKeyUp)
                     },
                     mounted() {
                         window.addEventListener("keydown", this.handleKeyDown), window.addEventListener("keyup", this.handleKeyUp);
-                        let e = Re()({
+                        let e = Ie()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1805,34 +1815,34 @@
                             this.$refs.chart.setOption(this.options), this.$refs.chart.chart.on("click", (e => alert("!")))
                         }
                     },
                     mounted() {
                         this.calcSeries()
                     }
                 },
-                mt = (0, U.Z)(pt, [
+                gt = (0, U.Z)(pt, [
                     ["render", et],
                     ["__scopeId", "data-v-12be25e8"]
                 ]),
-                gt = mt;
+                mt = gt;
 
             function ft(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
-                a.open("POST", y, !0), a.onload = function() {
+                a.open("POST", w, !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
             const yt = (0, s.aZ)({
                 name: "element",
                 components: {
-                    utable: Te,
+                    utable: Fe,
                     cgraph: Je,
-                    linechart: gt
+                    linechart: mt
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
@@ -1927,16 +1937,17 @@
                 mounted() {
                     k[this.fullname] = this, this.data.focus && this.$refs.inputRef.$el.focus()
                 },
                 data() {
                     return {
                         Dark: ze.Z,
                         value: this.data.value,
-                        styleSize: h.visibility ? S(this) : "",
-                        host_path: y,
+                        styleSize: h.visibility ? S(this) : null,
+                        has_recalc: !0,
+                        host_path: w,
                         options: [],
                         expandedKeys: [],
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
@@ -2060,25 +2071,25 @@
                 xt = a(1232),
                 Ct = a(5551),
                 _t = a(5869),
                 qt = a(1745),
                 At = a(8430);
             const Dt = (0, U.Z)(yt, [
                     ["render", _e],
-                    ["__scopeId", "data-v-5682537f"]
+                    ["__scopeId", "data-v-206674a7"]
                 ]),
                 St = Dt;
 
             function jt(e) {
                 let t = e.type;
                 return "tree" == t || "table" == t || "list" == t || "docviewer" == t || "graph" == t || "linechart" == t
             }
-            R()(yt, "components", {
+            I()(yt, "components", {
                 QImg: wt.Z,
-                QIcon: F.Z,
+                QIcon: T.Z,
                 QSelect: Ue.Z,
                 QBadge: bt.Z,
                 QCheckbox: Oe.Z,
                 QToggle: kt.Z,
                 QBtn: Ee.Z,
                 QBtnToggle: vt.Z,
                 QInput: We.Z,
@@ -2182,18 +2193,18 @@
                 watch: {
                     data(e) {
                         m && console.log("data update", this.name), b[this.name] = this, this.expanding && (this.styleSize = h.visibility ? S(this) : "", k[this.fullname] = this)
                     }
                 }
             });
             var Zt = a(151);
-            const Mt = (0, U.Z)(zt, [
+            const $t = (0, U.Z)(zt, [
                     ["render", ie]
                 ]),
-                $t = Mt;
+                Mt = $t;
 
             function Wt() {
                 console.log();
                 let e = A && k.size == v.size;
                 if (e)
                     for (let [t, a] of Object.entries(k))
                         if (!v[t]) {
@@ -2203,23 +2214,23 @@
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
                             h.visible(!0)
                         }))
                     }))
                 })))
             }
-            R()(zt, "components", {
+            I()(zt, "components", {
                 QCard: Zt.Z,
-                QIcon: F.Z,
+                QIcon: T.Z,
                 QScrollArea: xt.Z
             });
             const Vt = (0, s.aZ)({
                     name: "zone",
                     components: {
-                        block: $t
+                        block: Mt
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, s.Y3)((() => {
                             requestAnimationFrame((() => {
@@ -2228,19 +2239,19 @@
                         }))
                     }
                 }),
                 Et = (0, U.Z)(Vt, [
                     ["render", J]
                 ]),
                 Kt = Et,
-                Qt = {
+                Ht = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function Ht(e, t, a, i, n, o) {
+            function Qt(e, t, a, i, n, o) {
                 const d = (0, s.up)("block"),
                     r = (0, s.up)("q-item-label"),
                     c = (0, s.up)("q-space"),
                     h = (0, s.up)("q-btn"),
                     u = (0, s.up)("q-card"),
                     p = (0, s.up)("q-dialog");
                 return (0, s.wg)(), (0, s.j4)(p, {
@@ -2257,15 +2268,15 @@
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, s.kq)("", !0), (0, s.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, s._)("div", Qt, [(0, s.Wm)(c), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(a.buttons, (e => ((0, s.wg)(), (0, s.j4)(h, {
+                        }), (0, s._)("div", Ht, [(0, s.Wm)(c), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(a.buttons, (e => ((0, s.wg)(), (0, s.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => o.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
@@ -2274,15 +2285,15 @@
             }
             const Ot = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: $t
+                    block: Mt
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
@@ -2303,31 +2314,31 @@
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
             var Ut = a(5926),
                 Nt = a(2025);
-            const Tt = (0, U.Z)(Ot, [
-                    ["render", Ht]
+            const Ft = (0, U.Z)(Ot, [
+                    ["render", Qt]
                 ]),
-                Ft = Tt;
-            R()(Ot, "components", {
+                Tt = Ft;
+            I()(Ot, "components", {
                 QDialog: Ut.Z,
                 QCard: Zt.Z,
                 QItemLabel: P.Z,
                 QSpace: Nt.Z,
                 QBtn: Ee.Z
             });
             var Pt = a(589);
-            let It = "theme";
+            let Rt = "theme";
             try {
-                ze.Z.set(Pt.Z.getItem(It))
+                ze.Z.set(Pt.Z.getItem(Rt))
             } catch (la) {}
-            let Rt = null;
+            let It = null;
             const Lt = (0, s.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         Dark: ze.Z,
                         menu: [],
@@ -2336,15 +2347,16 @@
                             name: "toolbar"
                         },
                         localServer: !0,
                         statusConnect: !1,
                         screen: {
                             blocks: []
                         },
-                        visibility: !1
+                        visibility: !0,
+                        designCycle: 0
                     }
                 },
                 components: {
                     menubar: B,
                     zone: Kt,
                     element: St
                 },
@@ -2352,35 +2364,35 @@
                     C(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
                 methods: {
                     switchTheme() {
-                        ze.Z.set(!ze.Z.isActive), Pt.Z.set(It, ze.Z.isActive)
+                        ze.Z.set(!ze.Z.isActive), Pt.Z.set(Rt, ze.Z.isActive)
                     },
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
                         _(["root", e])
                     },
                     visible(e) {
-                        this.$refs.page.$el.style.visibility = e ? "" : "hidden", this.visibility = e
+                        this.visibility != e && (this.$refs.page.$el.style.visibility = e ? "" : "hidden", this.visibility = e)
                     },
                     onResize(e) {
-                        m && console.log("window has been resized", window.innerHeight, window.innerWidth), E()
+                        m && console.log("window has been resized", window.innerHeight, window.innerWidth), this.designCycle = 0, E()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Ft
+                                component: Tt
                             },
                             {
                                 height: a,
                                 ...s
                             } = e;
                         s.width = 750;
                         let l = {
@@ -2399,25 +2411,25 @@
                         let a = t,
                             s = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == Rt ? (s = {
+                        "progress" == t ? null == It ? (s = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, Rt = this.$q.notify(s)) : null == e ? (Rt(), Rt = null) : (s = {
+                        }, It = this.$q.notify(s)) : null == e ? (It(), It = null) : (s = {
                             caption: e
-                        }, Rt(s)) : ("error" == t && s.type, this.$q.notify(s))
+                        }, It(s)) : ("error" == t && s.type, this.$q.notify(s))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
@@ -2430,26 +2442,26 @@
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Ft, t.componentProps = {
+                            t.component = Tt, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
-                        } else if ("answer" == e.type) $(e);
+                        } else if ("answer" == e.type) M(e);
                         else {
                             let t = e.updates && e.updates.length;
-                            t && M(e.updates);
+                            t && $(e.updates);
                             let a = !1;
                             ["error", "progress", "warning", "info"].includes(e.type) && (this.notify(e.value, e.type), a = !0), a || t || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        Rt && "progress" != e.type && this.notify(null, "progress")
+                        It && "progress" != e.type && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize);
                     const e = new ResizeObserver((e => {
                         let t = document.documentElement.scrollWidth > window.innerWidth || document.documentElement.scrollHeight > window.innerHeight;
                         t && V(!0)
@@ -2465,15 +2477,15 @@
                 Jt = a(3269),
                 ea = a(2652),
                 ta = a(4379);
             const aa = (0, U.Z)(Lt, [
                     ["render", o]
                 ]),
                 sa = aa;
-            R()(Lt, "components", {
+            I()(Lt, "components", {
                 QLayout: Bt.Z,
                 QHeader: Yt.Z,
                 QToolbar: Xt.Z,
                 QBtn: Ee.Z,
                 QItemLabel: P.Z,
                 QTabs: Gt.Z,
                 QTab: Jt.Z,
```

### Comparing `unigui-1.9.4/unigui/web/js/193.283445be.js` & `unigui-1.9.5/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/unigui/web/index.html` & `unigui-1.9.5/unigui/web/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.5659ce27.js></script><script defer src=js/app.df555111.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.5659ce27.js></script><script defer src=js/app.6805317c.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.9.4/LICENSE` & `unigui-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.9.4/setup.py` & `unigui-1.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.9.4',      
+      version='1.9.5',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.9.4/PKG-INFO` & `unigui-1.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.4
+Version: 1.9.5
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -201,21 +201,14 @@
 ### Load to server Button ###
 Special button provides file loading from user device or computer to the Unigui server.
 ```
 UploadButton('Load', handler_when_loading_finish, icon='photo_library')
 ```
 handler_when_loading_finish(button_, the_loaded_file_filename) where the_loaded_file_filename is a file name in upload server folder. This folder name is defined in config.py .
 
-### Camera Button ###
-Special button provides to make a photo on the user mobile device. 
-```
-CameraButton('Make a photo', handler_when_shooting_finish, icon='camera_alt')
-```
-handler_when_loading_finish(button_, name_of_loaded_file) where name_of_loaded_file is the made photo name in the server folder. This folder name is defined in config.py .
-
 ### Edit and Text field. ###
 ```
 Edit('Some field', '') #for string value
 Edit('Number field', 0.9, type = 'number') #changed handler will get a number
 ```
 If set edit = false it will be readonly field or text label.
 ```
@@ -411,10 +404,9 @@
 print(isinstance(user, Hello_user))
 ```
 
 More info about User class methods you can find in user.py in the souce dir.
 
 Examples are in tests folder.
 
-Unigui protocol messages from/to server you can see in a browser console (F12).
```

### Comparing `unigui-1.9.4/README.md` & `unigui-1.9.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -189,21 +189,14 @@
 ### Load to server Button ###
 Special button provides file loading from user device or computer to the Unigui server.
 ```
 UploadButton('Load', handler_when_loading_finish, icon='photo_library')
 ```
 handler_when_loading_finish(button_, the_loaded_file_filename) where the_loaded_file_filename is a file name in upload server folder. This folder name is defined in config.py .
 
-### Camera Button ###
-Special button provides to make a photo on the user mobile device. 
-```
-CameraButton('Make a photo', handler_when_shooting_finish, icon='camera_alt')
-```
-handler_when_loading_finish(button_, name_of_loaded_file) where name_of_loaded_file is the made photo name in the server folder. This folder name is defined in config.py .
-
 ### Edit and Text field. ###
 ```
 Edit('Some field', '') #for string value
 Edit('Number field', 0.9, type = 'number') #changed handler will get a number
 ```
 If set edit = false it will be readonly field or text label.
 ```
@@ -399,8 +392,7 @@
 print(isinstance(user, Hello_user))
 ```
 
 More info about User class methods you can find in user.py in the souce dir.
 
 Examples are in tests folder.
 
-Unigui protocol messages from/to server you can see in a browser console (F12).
```

### Comparing `unigui-1.9.4/unigui.egg-info/PKG-INFO` & `unigui-1.9.5/unigui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.4
+Version: 1.9.5
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -201,21 +201,14 @@
 ### Load to server Button ###
 Special button provides file loading from user device or computer to the Unigui server.
 ```
 UploadButton('Load', handler_when_loading_finish, icon='photo_library')
 ```
 handler_when_loading_finish(button_, the_loaded_file_filename) where the_loaded_file_filename is a file name in upload server folder. This folder name is defined in config.py .
 
-### Camera Button ###
-Special button provides to make a photo on the user mobile device. 
-```
-CameraButton('Make a photo', handler_when_shooting_finish, icon='camera_alt')
-```
-handler_when_loading_finish(button_, name_of_loaded_file) where name_of_loaded_file is the made photo name in the server folder. This folder name is defined in config.py .
-
 ### Edit and Text field. ###
 ```
 Edit('Some field', '') #for string value
 Edit('Number field', 0.9, type = 'number') #changed handler will get a number
 ```
 If set edit = false it will be readonly field or text label.
 ```
@@ -411,10 +404,9 @@
 print(isinstance(user, Hello_user))
 ```
 
 More info about User class methods you can find in user.py in the souce dir.
 
 Examples are in tests folder.
 
-Unigui protocol messages from/to server you can see in a browser console (F12).
```

### Comparing `unigui-1.9.4/unigui.egg-info/SOURCES.txt` & `unigui-1.9.5/unigui.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/750.ca964e27.css
+unigui/web/css/982.c7dd083b.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.f747ec02.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -31,10 +31,10 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/750.4831ed09.js
-unigui/web/js/app.df555111.js
+unigui/web/js/982.872ac96a.js
+unigui/web/js/app.6805317c.js
 unigui/web/js/vendor.5659ce27.js
```

