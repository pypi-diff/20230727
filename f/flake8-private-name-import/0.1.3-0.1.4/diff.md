# Comparing `tmp/flake8_private_name_import-0.1.3.tar.gz` & `tmp/flake8_private_name_import-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8_private_name_import-0.1.3.tar", last modified: Wed Jul 26 18:57:01 2023, max compression
+gzip compressed data, was "dist/flake8_private_name_import-0.1.4.tar", last modified: Thu Jul 27 21:13:02 2023, max compression
```

## Comparing `flake8_private_name_import-0.1.3.tar` & `flake8_private_name_import-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/
--rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/PKG-INFO
--rw-rw-r--   0 rows      (1000) rows      (1000)       81 2023-07-25 20:19:44.000000 flake8_private_name_import-0.1.3/README.md
-drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/
--rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/PKG-INFO
--rw-rw-r--   0 rows      (1000) rows      (1000)      399 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/SOURCES.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/dependency_links.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)       63 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/entry_points.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/not-zip-safe
--rw-rw-r--   0 rows      (1000) rows      (1000)       29 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/requires.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)       27 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/top_level.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)     1827 2023-07-26 18:56:58.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.py
--rw-rw-r--   0 rows      (1000) rows      (1000)       38 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/setup.cfg
--rw-rw-r--   0 rows      (1000) rows      (1000)     1779 2023-07-26 18:56:58.000000 flake8_private_name_import-0.1.3/setup.py
+drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-27 21:13:02.000000 flake8_private_name_import-0.1.4/
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-27 21:13:02.000000 flake8_private_name_import-0.1.4/PKG-INFO
+-rw-rw-r--   0 rows      (1000) rows      (1000)      647 2023-07-27 21:08:22.000000 flake8_private_name_import-0.1.4/README.md
+drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-27 21:13:02.000000 flake8_private_name_import-0.1.4/flake8_private_name_import.egg-info/
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-27 21:13:01.000000 flake8_private_name_import-0.1.4/flake8_private_name_import.egg-info/PKG-INFO
+-rw-rw-r--   0 rows      (1000) rows      (1000)      399 2023-07-27 21:13:02.000000 flake8_private_name_import-0.1.4/flake8_private_name_import.egg-info/SOURCES.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-27 21:13:01.000000 flake8_private_name_import-0.1.4/flake8_private_name_import.egg-info/dependency_links.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)       62 2023-07-27 21:13:01.000000 flake8_private_name_import-0.1.4/flake8_private_name_import.egg-info/entry_points.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-27 21:13:01.000000 flake8_private_name_import-0.1.4/flake8_private_name_import.egg-info/not-zip-safe
+-rw-rw-r--   0 rows      (1000) rows      (1000)       29 2023-07-27 21:13:01.000000 flake8_private_name_import-0.1.4/flake8_private_name_import.egg-info/requires.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)       27 2023-07-27 21:13:01.000000 flake8_private_name_import-0.1.4/flake8_private_name_import.egg-info/top_level.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)     4187 2023-07-27 21:12:13.000000 flake8_private_name_import-0.1.4/flake8_private_name_import.py
+-rw-rw-r--   0 rows      (1000) rows      (1000)       38 2023-07-27 21:13:02.000000 flake8_private_name_import-0.1.4/setup.cfg
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1778 2023-07-27 21:08:22.000000 flake8_private_name_import-0.1.4/setup.py
```

### Comparing `flake8_private_name_import-0.1.3/PKG-INFO` & `flake8_private_name_import-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8_private_name_import
-Version: 0.1.3
+Version: 0.1.4
 Summary: flake8 plugin that reports imports of private names
 Home-page: https://github.com/rows-s/flake8_private_name_import
 Author: Vladimir Marmuz
 Author-email: vladimir.rows@gmail.com
 License: MIT
 Description: flake8 plugin that reports imports of private names
 Keywords: python pep8 flake8 private import
```

### Comparing `flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/PKG-INFO` & `flake8_private_name_import-0.1.4/flake8_private_name_import.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-private-name-import
-Version: 0.1.3
+Version: 0.1.4
 Summary: flake8 plugin that reports imports of private names
 Home-page: https://github.com/rows-s/flake8_private_name_import
 Author: Vladimir Marmuz
 Author-email: vladimir.rows@gmail.com
 License: MIT
 Description: flake8 plugin that reports imports of private names
 Keywords: python pep8 flake8 private import
```

### Comparing `flake8_private_name_import-0.1.3/setup.py` & `flake8_private_name_import-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='flake8_private_name_import',
-    version='0.1.3',
+    version='0.1.4',
     description="flake8 plugin that reports imports of private names",
     long_description="flake8 plugin that reports imports of private names",
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Framework :: Flake8',
@@ -39,11 +39,11 @@
     extras_require={
         'test': [
             'pytest',
         ],
     },
     entry_points={
         'flake8.extension': [
-            'PNI001 = flake8_private_name_import:Plugin',
+            'PNI00 = flake8_private_name_import:Plugin',
         ],
     },
 )
```

