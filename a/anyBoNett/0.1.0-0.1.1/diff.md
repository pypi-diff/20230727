# Comparing `tmp/anyBoNett-0.1.0.tar.gz` & `tmp/anyBoNett-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyBoNett-0.1.0.tar", last modified: Thu Jul 27 01:11:48 2023, max compression
+gzip compressed data, was "anyBoNett-0.1.1.tar", last modified: Thu Jul 27 01:13:04 2023, max compression
```

## Comparing `anyBoNett-0.1.0.tar` & `anyBoNett-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 01:11:48.355968 anyBoNett-0.1.0/
--rw-rw-rw-   0        0        0     1094 2023-07-20 01:37:41.000000 anyBoNett-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3817 2023-07-27 01:11:48.355968 anyBoNett-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3531 2023-07-20 22:10:51.000000 anyBoNett-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 01:11:48.347960 anyBoNett-0.1.0/anyBoNett.egg-info/
--rw-rw-rw-   0        0        0     3817 2023-07-27 01:11:48.000000 anyBoNett-0.1.0/anyBoNett.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-07-27 01:11:48.000000 anyBoNett-0.1.0/anyBoNett.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 01:11:48.000000 anyBoNett-0.1.0/anyBoNett.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-27 01:11:48.000000 anyBoNett-0.1.0/anyBoNett.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 01:11:48.000000 anyBoNett-0.1.0/anyBoNett.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-27 01:11:48.347960 anyBoNett-0.1.0/anybonett/
--rw-rw-rw-   0        0        0     3138 2023-07-27 01:11:09.000000 anyBoNett-0.1.0/anybonett/NET.py
--rw-rw-rw-   0        0        0       42 2023-07-27 01:11:48.355968 anyBoNett-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      506 2023-07-27 01:11:31.000000 anyBoNett-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:13:04.717272 anyBoNett-0.1.1/
+-rw-rw-rw-   0        0        0     1094 2023-07-20 01:37:41.000000 anyBoNett-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3817 2023-07-27 01:13:04.715944 anyBoNett-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3531 2023-07-20 22:10:51.000000 anyBoNett-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 01:13:04.706169 anyBoNett-0.1.1/anyBoNett.egg-info/
+-rw-rw-rw-   0        0        0     3817 2023-07-27 01:13:04.000000 anyBoNett-0.1.1/anyBoNett.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-07-27 01:13:04.000000 anyBoNett-0.1.1/anyBoNett.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 01:13:04.000000 anyBoNett-0.1.1/anyBoNett.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-27 01:13:04.000000 anyBoNett-0.1.1/anyBoNett.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 01:13:04.000000 anyBoNett-0.1.1/anyBoNett.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 01:13:04.706169 anyBoNett-0.1.1/anybonett/
+-rw-rw-rw-   0        0        0     3107 2023-07-27 01:12:33.000000 anyBoNett-0.1.1/anybonett/NET.py
+-rw-rw-rw-   0        0        0       42 2023-07-27 01:13:04.717272 anyBoNett-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      506 2023-07-27 01:12:43.000000 anyBoNett-0.1.1/setup.py
```

### Comparing `anyBoNett-0.1.0/LICENSE` & `anyBoNett-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anyBoNett-0.1.0/PKG-INFO` & `anyBoNett-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyBoNett
-Version: 0.1.0
+Version: 0.1.1
 Summary: uma biblioteca pra facilitar pesquisas
 Author: AnyBoLIB
 Author-email: bidjorys@gmail.com
 License: MIT License
 Keywords: ytl,anybonett,net,anybonet,
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `anyBoNett-0.1.0/README.md` & `anyBoNett-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `anyBoNett-0.1.0/anyBoNett.egg-info/PKG-INFO` & `anyBoNett-0.1.1/anyBoNett.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyBoNett
-Version: 0.1.0
+Version: 0.1.1
 Summary: uma biblioteca pra facilitar pesquisas
 Author: AnyBoLIB
 Author-email: bidjorys@gmail.com
 License: MIT License
 Keywords: ytl,anybonett,net,anybonet,
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `anyBoNett-0.1.0/anybonett/NET.py` & `anyBoNett-0.1.1/anybonett/NET.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import webbrowser
 import wikipedia
 import requests
-from googlesearch import search
+
 
 def search_youtube(input):
     try:
         url = f"https://www.youtube.com/results?search_query={input}"
         s = webbrowser.open(url)
         return
     except Exception as e:
```

