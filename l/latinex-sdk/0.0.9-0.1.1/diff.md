# Comparing `tmp/latinex-sdk-0.0.9.tar.gz` & `tmp/latinex-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latinex-sdk-0.0.9.tar", last modified: Wed Jul 26 23:20:53 2023, max compression
+gzip compressed data, was "latinex-sdk-0.1.1.tar", last modified: Wed Jul 26 23:52:55 2023, max compression
```

## Comparing `latinex-sdk-0.0.9.tar` & `latinex-sdk-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:20:53.124433 latinex-sdk-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 23:20:42.000000 latinex-sdk-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-26 23:20:53.124433 latinex-sdk-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-26 23:20:42.000000 latinex-sdk-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:20:53.120433 latinex-sdk-0.0.9/latinex-sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-26 23:20:42.000000 latinex-sdk-0.0.9/latinex-sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-26 23:20:42.000000 latinex-sdk-0.0.9/latinex-sdk/generic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:20:53.124433 latinex-sdk-0.0.9/latinex_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-26 23:20:53.000000 latinex-sdk-0.0.9/latinex_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-26 23:20:53.000000 latinex-sdk-0.0.9/latinex_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:20:53.000000 latinex-sdk-0.0.9/latinex_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 23:20:53.000000 latinex-sdk-0.0.9/latinex_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 23:20:53.000000 latinex-sdk-0.0.9/latinex_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:20:53.124433 latinex-sdk-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-26 23:20:42.000000 latinex-sdk-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:55.755653 latinex-sdk-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 23:52:44.000000 latinex-sdk-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-26 23:52:55.755653 latinex-sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-26 23:52:44.000000 latinex-sdk-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:55.755653 latinex-sdk-0.1.1/latinex-sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-26 23:52:44.000000 latinex-sdk-0.1.1/latinex-sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-26 23:52:44.000000 latinex-sdk-0.1.1/latinex-sdk/generic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:55.755653 latinex-sdk-0.1.1/latinex_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-26 23:52:55.000000 latinex-sdk-0.1.1/latinex_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-26 23:52:55.000000 latinex-sdk-0.1.1/latinex_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:52:55.000000 latinex-sdk-0.1.1/latinex_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 23:52:55.000000 latinex-sdk-0.1.1/latinex_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 23:52:55.000000 latinex-sdk-0.1.1/latinex_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:52:55.755653 latinex-sdk-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-26 23:52:44.000000 latinex-sdk-0.1.1/setup.py
```

### Comparing `latinex-sdk-0.0.9/LICENSE` & `latinex-sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `latinex-sdk-0.0.9/PKG-INFO` & `latinex-sdk-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latinex-sdk
-Version: 0.0.9
+Version: 0.1.1
 Summary: Software Development Kit for Latinex (https://www.latinexbolsa.com)
 Author: Blasser Analytica (Rodolfo Blasser)
 Author-email: <rodolfoblasser@gmail.com>
 Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `latinex-sdk-0.0.9/README.md` & `latinex-sdk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `latinex-sdk-0.0.9/latinex-sdk/generic_utils.py` & `latinex-sdk-0.1.1/latinex-sdk/generic_utils.py`

 * *Files identical despite different names*

### Comparing `latinex-sdk-0.0.9/latinex_sdk.egg-info/PKG-INFO` & `latinex-sdk-0.1.1/latinex_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latinex-sdk
-Version: 0.0.9
+Version: 0.1.1
 Summary: Software Development Kit for Latinex (https://www.latinexbolsa.com)
 Author: Blasser Analytica (Rodolfo Blasser)
 Author-email: <rodolfoblasser@gmail.com>
 Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `latinex-sdk-0.0.9/setup.py` & `latinex-sdk-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.9'
+VERSION = '0.1.1'
 DESCRIPTION = 'Software Development Kit for Latinex (https://www.latinexbolsa.com)'
 LONG_DESCRIPTION = 'This SKD facilitates the use of the Latinex REST API, it allows the user to register (getting an API Key) and to fetch data in a friction-less manner'
 
 # Setting up
 setup(
     name="latinex-sdk",
     version=VERSION,
```

