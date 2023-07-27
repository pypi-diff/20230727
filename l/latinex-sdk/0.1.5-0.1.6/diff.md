# Comparing `tmp/latinex_sdk-0.1.5.tar.gz` & `tmp/latinex_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latinex_sdk-0.1.5.tar", last modified: Thu Jul 27 00:41:29 2023, max compression
+gzip compressed data, was "latinex_sdk-0.1.6.tar", last modified: Thu Jul 27 00:46:32 2023, max compression
```

## Comparing `latinex_sdk-0.1.5.tar` & `latinex_sdk-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:41:29.940515 latinex_sdk-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 00:41:19.000000 latinex_sdk-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-27 00:41:29.940515 latinex_sdk-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-27 00:41:19.000000 latinex_sdk-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:41:29.936515 latinex_sdk-0.1.5/latinex_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 00:41:19.000000 latinex_sdk-0.1.5/latinex_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-27 00:41:19.000000 latinex_sdk-0.1.5/latinex_sdk/generic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:41:29.940515 latinex_sdk-0.1.5/latinex_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-27 00:41:29.000000 latinex_sdk-0.1.5/latinex_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 00:41:29.000000 latinex_sdk-0.1.5/latinex_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:41:29.000000 latinex_sdk-0.1.5/latinex_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 00:41:29.000000 latinex_sdk-0.1.5/latinex_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 00:41:29.000000 latinex_sdk-0.1.5/latinex_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:41:29.940515 latinex_sdk-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-27 00:41:19.000000 latinex_sdk-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:46:32.448604 latinex_sdk-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 00:46:19.000000 latinex_sdk-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-27 00:46:32.448604 latinex_sdk-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-27 00:46:19.000000 latinex_sdk-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:46:32.444604 latinex_sdk-0.1.6/latinex_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 00:46:19.000000 latinex_sdk-0.1.6/latinex_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-27 00:46:19.000000 latinex_sdk-0.1.6/latinex_sdk/generic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:46:32.448604 latinex_sdk-0.1.6/latinex_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-27 00:46:32.000000 latinex_sdk-0.1.6/latinex_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 00:46:32.000000 latinex_sdk-0.1.6/latinex_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:46:32.000000 latinex_sdk-0.1.6/latinex_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 00:46:32.000000 latinex_sdk-0.1.6/latinex_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 00:46:32.000000 latinex_sdk-0.1.6/latinex_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:46:32.448604 latinex_sdk-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-27 00:46:19.000000 latinex_sdk-0.1.6/setup.py
```

### Comparing `latinex_sdk-0.1.5/LICENSE` & `latinex_sdk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `latinex_sdk-0.1.5/PKG-INFO` & `latinex_sdk-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latinex_sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Software Development Kit for Latinex (https://www.latinexbolsa.com)
 Author: Blasser Analytica (Rodolfo Blasser)
 Author-email: <rodolfoblasser@gmail.com>
 Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `latinex_sdk-0.1.5/README.md` & `latinex_sdk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `latinex_sdk-0.1.5/latinex_sdk.egg-info/PKG-INFO` & `latinex_sdk-0.1.6/latinex_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latinex-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Software Development Kit for Latinex (https://www.latinexbolsa.com)
 Author: Blasser Analytica (Rodolfo Blasser)
 Author-email: <rodolfoblasser@gmail.com>
 Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `latinex_sdk-0.1.5/setup.py` & `latinex_sdk-0.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'Software Development Kit for Latinex (https://www.latinexbolsa.com)'
 LONG_DESCRIPTION = 'This SKD facilitates the use of the Latinex REST API, it allows the user to register (getting an API Key) and to fetch data in a friction-less manner'
 
 # Setting up
 setup(
     name="latinex_sdk",
     version=VERSION,
```

