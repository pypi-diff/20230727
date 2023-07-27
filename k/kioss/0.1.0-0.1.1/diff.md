# Comparing `tmp/kioss-0.1.0.tar.gz` & `tmp/kioss-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.1.0.tar", last modified: Thu Jul 27 15:38:02 2023, max compression
+gzip compressed data, was "kioss-0.1.1.tar", last modified: Thu Jul 27 17:10:58 2023, max compression
```

## Comparing `kioss-0.1.0.tar` & `kioss-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:02.883457 kioss-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 15:37:54.000000 kioss-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-27 15:38:02.879457 kioss-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-27 15:37:54.000000 kioss-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:02.879457 kioss-0.1.0/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 15:37:54.000000 kioss-0.1.0/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-07-27 15:37:54.000000 kioss-0.1.0/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 15:37:54.000000 kioss-0.1.0/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:02.879457 kioss-0.1.0/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-27 15:38:02.000000 kioss-0.1.0/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-27 15:38:02.000000 kioss-0.1.0/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:38:02.000000 kioss-0.1.0/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 15:38:02.000000 kioss-0.1.0/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 15:38:02.883457 kioss-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-27 15:37:54.000000 kioss-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:02.879457 kioss-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-27 15:37:54.000000 kioss-0.1.0/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-27 15:37:54.000000 kioss-0.1.0/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:10:58.027750 kioss-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 17:10:48.000000 kioss-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-27 17:10:58.027750 kioss-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-27 17:10:48.000000 kioss-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:10:58.027750 kioss-0.1.1/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 17:10:48.000000 kioss-0.1.1/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-07-27 17:10:48.000000 kioss-0.1.1/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 17:10:48.000000 kioss-0.1.1/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:10:58.027750 kioss-0.1.1/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-27 17:10:57.000000 kioss-0.1.1/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-27 17:10:58.000000 kioss-0.1.1/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:10:57.000000 kioss-0.1.1/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 17:10:57.000000 kioss-0.1.1/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:10:58.027750 kioss-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-27 17:10:48.000000 kioss-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:10:58.027750 kioss-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-27 17:10:48.000000 kioss-0.1.1/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-27 17:10:48.000000 kioss-0.1.1/test/test_util.py
```

### Comparing `kioss-0.1.0/LICENSE` & `kioss-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.1.0/README.md` & `kioss-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 ## Toy use case:
 
 ```python
 import re
 from kioss import Pipe
 import requests
 
-# detects emails in text and raises if any of them is unreachable
+# detects emails domains in text and raises if any of them is unreachable
 
 
 # A Pipe can be created from any iterator/iterable,
 # it is designed to easily process on the fly the data elements
 # from large files, APIs or databases without requiring large memory or disk.
 # we use a local file for this example:
 with open("/path/to/file.text", "r") as text_file:
     if unreachable_domain_samples := (
-        #this pipe will read the text file line by line
+        # this pipe will read the text file line by line
         Pipe(text_file)
         # split each map on spaces to get iterator on words
         .map(str.split)
         .map(iter)
         # flatten the pipe to make it yield individual words
         .flatten()
         # log the advancement of this step
```

### Comparing `kioss-0.1.0/kioss/pipe.py` & `kioss-0.1.1/kioss/pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         Args:
             n_error_samples (int, optional): The maximum number of error samples to include in the RuntimeError message (default is 8).
         Raises:
             RuntimeError: If any exception is catched during iteration.
         """
         if errors := (
             self.catch(Exception, ignore=False)
-            .log()
+            .log(objects_description="ultimate elements")
             .filter(lambda elem: isinstance(elem, Exception))
             .map(repr)
             .collect(limit=n_error_samples)
         ):
             raise RuntimeError(errors)
```

### Comparing `kioss-0.1.0/test/test_pipe.py` & `kioss-0.1.1/test/test_pipe.py`

 * *Files identical despite different names*

