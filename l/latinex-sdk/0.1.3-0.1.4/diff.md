# Comparing `tmp/latinex_sdk-0.1.3.tar.gz` & `tmp/latinex_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latinex_sdk-0.1.3.tar", last modified: Thu Jul 27 00:28:04 2023, max compression
+gzip compressed data, was "latinex_sdk-0.1.4.tar", last modified: Thu Jul 27 00:34:08 2023, max compression
```

## Comparing `latinex_sdk-0.1.3.tar` & `latinex_sdk-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:28:04.460811 latinex_sdk-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 00:27:55.000000 latinex_sdk-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-27 00:28:04.460811 latinex_sdk-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-27 00:27:55.000000 latinex_sdk-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:28:04.460811 latinex_sdk-0.1.3/latinex-sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 00:27:55.000000 latinex_sdk-0.1.3/latinex-sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-27 00:27:55.000000 latinex_sdk-0.1.3/latinex-sdk/generic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:28:04.460811 latinex_sdk-0.1.3/latinex_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-27 00:28:04.000000 latinex_sdk-0.1.3/latinex_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 00:28:04.000000 latinex_sdk-0.1.3/latinex_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:28:04.000000 latinex_sdk-0.1.3/latinex_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 00:28:04.000000 latinex_sdk-0.1.3/latinex_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 00:28:04.000000 latinex_sdk-0.1.3/latinex_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:28:04.460811 latinex_sdk-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-27 00:27:55.000000 latinex_sdk-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:34:08.874193 latinex_sdk-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 00:33:58.000000 latinex_sdk-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-27 00:34:08.874193 latinex_sdk-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-27 00:33:58.000000 latinex_sdk-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:34:08.874193 latinex_sdk-0.1.4/latinex_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 00:33:58.000000 latinex_sdk-0.1.4/latinex_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-27 00:33:58.000000 latinex_sdk-0.1.4/latinex_sdk/generic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:34:08.874193 latinex_sdk-0.1.4/latinex_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-27 00:34:08.000000 latinex_sdk-0.1.4/latinex_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 00:34:08.000000 latinex_sdk-0.1.4/latinex_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:34:08.000000 latinex_sdk-0.1.4/latinex_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 00:34:08.000000 latinex_sdk-0.1.4/latinex_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 00:34:08.000000 latinex_sdk-0.1.4/latinex_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:34:08.874193 latinex_sdk-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-27 00:33:58.000000 latinex_sdk-0.1.4/setup.py
```

### Comparing `latinex_sdk-0.1.3/LICENSE` & `latinex_sdk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `latinex_sdk-0.1.3/PKG-INFO` & `latinex_sdk-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latinex_sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Software Development Kit for Latinex (https://www.latinexbolsa.com)
 Author: Blasser Analytica (Rodolfo Blasser)
 Author-email: <rodolfoblasser@gmail.com>
 Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `latinex_sdk-0.1.3/README.md` & `latinex_sdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `latinex_sdk-0.1.3/latinex-sdk/generic_utils.py` & `latinex_sdk-0.1.4/latinex_sdk/generic_utils.py`

 * *Files identical despite different names*

### Comparing `latinex_sdk-0.1.3/latinex_sdk.egg-info/PKG-INFO` & `latinex_sdk-0.1.4/latinex_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latinex-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Software Development Kit for Latinex (https://www.latinexbolsa.com)
 Author: Blasser Analytica (Rodolfo Blasser)
 Author-email: <rodolfoblasser@gmail.com>
 Keywords: python,panama,finance,stocks,fixed income,data,api,market data,latinex
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `latinex_sdk-0.1.3/setup.py` & `latinex_sdk-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'Software Development Kit for Latinex (https://www.latinexbolsa.com)'
 LONG_DESCRIPTION = 'This SKD facilitates the use of the Latinex REST API, it allows the user to register (getting an API Key) and to fetch data in a friction-less manner'
 
 # Setting up
 setup(
     name="latinex_sdk",
     version=VERSION,
```

