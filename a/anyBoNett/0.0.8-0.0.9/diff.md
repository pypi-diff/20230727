# Comparing `tmp/anyBoNett-0.0.8.tar.gz` & `tmp/anyBoNett-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyBoNett-0.0.8.tar", last modified: Thu Jul 20 22:16:18 2023, max compression
+gzip compressed data, was "anyBoNett-0.0.9.tar", last modified: Thu Jul 27 01:06:50 2023, max compression
```

## Comparing `anyBoNett-0.0.8.tar` & `anyBoNett-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 22:16:18.125024 anyBoNett-0.0.8/
--rw-rw-rw-   0        0        0     1094 2023-07-20 01:37:41.000000 anyBoNett-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3817 2023-07-20 22:16:18.122403 anyBoNett-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3531 2023-07-20 22:10:51.000000 anyBoNett-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 22:16:18.118491 anyBoNett-0.0.8/anyBoNett.egg-info/
--rw-rw-rw-   0        0        0     3817 2023-07-20 22:16:17.000000 anyBoNett-0.0.8/anyBoNett.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-07-20 22:16:17.000000 anyBoNett-0.0.8/anyBoNett.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 22:16:17.000000 anyBoNett-0.0.8/anyBoNett.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-20 22:16:17.000000 anyBoNett-0.0.8/anyBoNett.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-20 22:16:17.000000 anyBoNett-0.0.8/anyBoNett.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 22:16:18.121039 anyBoNett-0.0.8/anybonett/
--rw-rw-rw-   0        0        0     3132 2023-07-20 22:12:01.000000 anyBoNett-0.0.8/anybonett/NET.py
--rw-rw-rw-   0        0        0       42 2023-07-20 22:16:18.125024 anyBoNett-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      493 2023-07-20 22:15:52.000000 anyBoNett-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:06:50.180250 anyBoNett-0.0.9/
+-rw-rw-rw-   0        0        0     1094 2023-07-20 01:37:41.000000 anyBoNett-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3817 2023-07-27 01:06:50.180250 anyBoNett-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3531 2023-07-20 22:10:51.000000 anyBoNett-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 01:06:50.164253 anyBoNett-0.0.9/anyBoNett.egg-info/
+-rw-rw-rw-   0        0        0     3817 2023-07-27 01:06:49.000000 anyBoNett-0.0.9/anyBoNett.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-07-27 01:06:50.000000 anyBoNett-0.0.9/anyBoNett.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 01:06:49.000000 anyBoNett-0.0.9/anyBoNett.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-27 01:06:49.000000 anyBoNett-0.0.9/anyBoNett.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 01:06:49.000000 anyBoNett-0.0.9/anyBoNett.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 01:06:50.172257 anyBoNett-0.0.9/anybonett/
+-rw-rw-rw-   0        0        0     3132 2023-07-20 22:12:01.000000 anyBoNett-0.0.9/anybonett/NET.py
+-rw-rw-rw-   0        0        0       42 2023-07-27 01:06:50.180250 anyBoNett-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      509 2023-07-27 01:06:36.000000 anyBoNett-0.0.9/setup.py
```

### Comparing `anyBoNett-0.0.8/LICENSE` & `anyBoNett-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anyBoNett-0.0.8/PKG-INFO` & `anyBoNett-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyBoNett
-Version: 0.0.8
+Version: 0.0.9
 Summary: uma biblioteca pra facilitar pesquisas
 Author: AnyBoLIB
 Author-email: bidjorys@gmail.com
 License: MIT License
 Keywords: ytl,anybonett,net,anybonet,
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `anyBoNett-0.0.8/README.md` & `anyBoNett-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `anyBoNett-0.0.8/anyBoNett.egg-info/PKG-INFO` & `anyBoNett-0.0.9/anyBoNett.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyBoNett
-Version: 0.0.8
+Version: 0.0.9
 Summary: uma biblioteca pra facilitar pesquisas
 Author: AnyBoLIB
 Author-email: bidjorys@gmail.com
 License: MIT License
 Keywords: ytl,anybonett,net,anybonet,
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `anyBoNett-0.0.8/anybonett/NET.py` & `anyBoNett-0.0.9/anybonett/NET.py`

 * *Files identical despite different names*

