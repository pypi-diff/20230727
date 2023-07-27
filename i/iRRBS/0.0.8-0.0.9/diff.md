# Comparing `tmp/iRRBS-0.0.8.tar.gz` & `tmp/iRRBS-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iRRBS-0.0.8.tar", last modified: Thu Jul 27 20:46:35 2023, max compression
+gzip compressed data, was "iRRBS-0.0.9.tar", last modified: Thu Jul 27 20:59:11 2023, max compression
```

## Comparing `iRRBS-0.0.8.tar` & `iRRBS-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 20:46:35.491357 iRRBS-0.0.8/
--rw-rw-r--   0 abel      (1000) abel      (1000)      101 2023-07-27 14:53:04.000000 iRRBS-0.0.8/CHANGELOG.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)     1069 2023-07-27 14:53:04.000000 iRRBS-0.0.8/LICENSE
--rw-rw-r--   0 abel      (1000) abel      (1000)       26 2023-07-27 14:53:04.000000 iRRBS-0.0.8/MANIFEST.in
--rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 20:46:35.491357 iRRBS-0.0.8/PKG-INFO
--rw-rw-r--   0 abel      (1000) abel      (1000)      952 2023-07-27 14:53:04.000000 iRRBS-0.0.8/README.md
-drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 20:46:35.491357 iRRBS-0.0.8/iRRBS/
--rw-rw-r--   0 abel      (1000) abel      (1000)      102 2023-07-27 20:45:09.000000 iRRBS-0.0.8/iRRBS/__init__.py
--rw-rw-r--   0 abel      (1000) abel      (1000)     7349 2023-07-27 14:53:04.000000 iRRBS-0.0.8/iRRBS/irrbs_pipeline.py
--rw-rw-r--   0 abel      (1000) abel      (1000)     1088 2023-07-27 20:30:37.000000 iRRBS-0.0.8/iRRBS/run_irrbs.py
--rw-rw-r--   0 abel      (1000) abel      (1000)      458 2023-07-27 14:53:04.000000 iRRBS-0.0.8/iRRBS/suppress.py
-drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 20:46:35.491357 iRRBS-0.0.8/iRRBS.egg-info/
--rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 20:46:35.000000 iRRBS-0.0.8/iRRBS.egg-info/PKG-INFO
--rw-rw-r--   0 abel      (1000) abel      (1000)      285 2023-07-27 20:46:35.000000 iRRBS-0.0.8/iRRBS.egg-info/SOURCES.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)        1 2023-07-27 20:46:35.000000 iRRBS-0.0.8/iRRBS.egg-info/dependency_links.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)       17 2023-07-27 20:46:35.000000 iRRBS-0.0.8/iRRBS.egg-info/requires.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)        6 2023-07-27 20:46:35.000000 iRRBS-0.0.8/iRRBS.egg-info/top_level.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)       79 2023-07-27 20:46:35.491357 iRRBS-0.0.8/setup.cfg
--rw-rw-r--   0 abel      (1000) abel      (1000)      828 2023-07-27 20:46:03.000000 iRRBS-0.0.8/setup.py
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 20:59:11.204566 iRRBS-0.0.9/
+-rw-rw-r--   0 abel      (1000) abel      (1000)      101 2023-07-27 14:53:04.000000 iRRBS-0.0.9/CHANGELOG.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1069 2023-07-27 14:53:04.000000 iRRBS-0.0.9/LICENSE
+-rw-rw-r--   0 abel      (1000) abel      (1000)       26 2023-07-27 14:53:04.000000 iRRBS-0.0.9/MANIFEST.in
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 20:59:11.204566 iRRBS-0.0.9/PKG-INFO
+-rw-rw-r--   0 abel      (1000) abel      (1000)      952 2023-07-27 14:53:04.000000 iRRBS-0.0.9/README.md
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 20:59:11.200566 iRRBS-0.0.9/iRRBS/
+-rw-rw-r--   0 abel      (1000) abel      (1000)      112 2023-07-27 20:58:51.000000 iRRBS-0.0.9/iRRBS/__init__.py
+-rw-rw-r--   0 abel      (1000) abel      (1000)     7349 2023-07-27 14:53:04.000000 iRRBS-0.0.9/iRRBS/irrbs_pipeline.py
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1088 2023-07-27 20:30:37.000000 iRRBS-0.0.9/iRRBS/run_irrbs.py
+-rw-rw-r--   0 abel      (1000) abel      (1000)      458 2023-07-27 14:53:04.000000 iRRBS-0.0.9/iRRBS/suppress.py
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 20:59:11.204566 iRRBS-0.0.9/iRRBS.egg-info/
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 20:59:11.000000 iRRBS-0.0.9/iRRBS.egg-info/PKG-INFO
+-rw-rw-r--   0 abel      (1000) abel      (1000)      285 2023-07-27 20:59:11.000000 iRRBS-0.0.9/iRRBS.egg-info/SOURCES.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)        1 2023-07-27 20:59:11.000000 iRRBS-0.0.9/iRRBS.egg-info/dependency_links.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)       17 2023-07-27 20:59:11.000000 iRRBS-0.0.9/iRRBS.egg-info/requires.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)        6 2023-07-27 20:59:11.000000 iRRBS-0.0.9/iRRBS.egg-info/top_level.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)       79 2023-07-27 20:59:11.204566 iRRBS-0.0.9/setup.cfg
+-rw-rw-r--   0 abel      (1000) abel      (1000)      828 2023-07-27 20:58:56.000000 iRRBS-0.0.9/setup.py
```

### Comparing `iRRBS-0.0.8/LICENSE` & `iRRBS-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.8/PKG-INFO` & `iRRBS-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iRRBS
-Version: 0.0.8
+Version: 0.0.9
 Summary: RRBS tool for deleting artificial cytosins
 Home-page: https://github.com/fothia/iRRBS
 Author: Abel Fothi
 Author-email: fothi.abel@gmail.com
 License: MIT
 Download-URL: https://github.com/fothia/iRRBS/archive/refs/tags/0.0.6.tar.gz
 Platform: UNKNOWN
```

### Comparing `iRRBS-0.0.8/README.md` & `iRRBS-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.8/iRRBS/irrbs_pipeline.py` & `iRRBS-0.0.9/iRRBS/irrbs_pipeline.py`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.8/iRRBS/run_irrbs.py` & `iRRBS-0.0.9/iRRBS/run_irrbs.py`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.8/iRRBS.egg-info/PKG-INFO` & `iRRBS-0.0.9/iRRBS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iRRBS
-Version: 0.0.8
+Version: 0.0.9
 Summary: RRBS tool for deleting artificial cytosins
 Home-page: https://github.com/fothia/iRRBS
 Author: Abel Fothi
 Author-email: fothi.abel@gmail.com
 License: MIT
 Download-URL: https://github.com/fothia/iRRBS/archive/refs/tags/0.0.6.tar.gz
 Platform: UNKNOWN
```

### Comparing `iRRBS-0.0.8/setup.py` & `iRRBS-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 'Operating System :: Unix',
 'License :: OSI Approved :: MIT License',
 'Programming Language :: Python :: 3',
 ]
 setup(
 name = 'iRRBS',
 packages = ['iRRBS'],
-version = '0.0.8',
+version = '0.0.9',
 description = 'RRBS tool for deleting artificial cytosins',
 long_description = (this_directory / "README.md").read_text(),
 url = 'https://github.com/fothia/iRRBS',
 download_url = 'https://github.com/fothia/iRRBS/archive/refs/tags/0.0.6.tar.gz',
 author = 'Abel Fothi',
 author_email = 'fothi.abel@gmail.com',
 license = 'MIT',
```

