# Comparing `tmp/pbu-1.1.1.tar.gz` & `tmp/pbu-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbu-1.1.1.tar", last modified: Thu Jul 27 00:29:25 2023, max compression
+gzip compressed data, was "pbu-1.1.2.tar", last modified: Thu Jul 27 00:49:42 2023, max compression
```

## Comparing `pbu-1.1.1.tar` & `pbu-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-27 00:29:25.446626 pbu-1.1.1/
--rw-rw-r--   0 peter     (1000) peter     (1000)    28194 2023-07-27 00:29:25.446626 pbu-1.1.1/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)    22559 2023-04-08 00:03:20.000000 pbu-1.1.1/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-27 00:29:25.445625 pbu-1.1.1/pbu/
--rw-rw-r--   0 peter     (1000) peter     (1000)      846 2023-07-27 00:27:21.000000 pbu-1.1.1/pbu/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1733 2023-07-27 00:25:20.000000 pbu-1.1.1/pbu/app_config.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6264 2023-07-05 06:07:23.000000 pbu-1.1.1/pbu/basic_monitor.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      474 2021-02-28 01:39:36.000000 pbu-1.1.1/pbu/constant_listing.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5668 2023-07-13 00:10:51.000000 pbu-1.1.1/pbu/datascience_util.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3755 2022-04-12 02:57:09.000000 pbu-1.1.1/pbu/date_time.py
--rw-r--r--   0 peter     (1000) peter     (1000)      374 2023-07-05 06:00:07.000000 pbu-1.1.1/pbu/debug_object.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4224 2023-04-07 23:51:49.000000 pbu-1.1.1/pbu/default_options.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1290 2023-07-27 00:27:10.000000 pbu-1.1.1/pbu/files.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8739 2023-07-05 07:15:28.000000 pbu-1.1.1/pbu/json_document.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4757 2021-02-28 01:39:36.000000 pbu-1.1.1/pbu/json_wrapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6937 2022-08-12 05:35:20.000000 pbu-1.1.1/pbu/logger.py
--rw-r--r--   0 peter     (1000) peter     (1000)      304 2023-01-25 00:24:29.000000 pbu-1.1.1/pbu/paging.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1223 2023-04-11 09:50:57.000000 pbu-1.1.1/pbu/performance_logger.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    29256 2022-12-08 01:37:27.000000 pbu-1.1.1/pbu/time_series.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-27 00:29:25.446626 pbu-1.1.1/pbu.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)    28194 2023-07-27 00:29:25.000000 pbu-1.1.1/pbu.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      468 2023-07-27 00:29:25.000000 pbu-1.1.1/pbu.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-27 00:29:25.000000 pbu-1.1.1/pbu.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2021-02-28 02:00:39.000000 pbu-1.1.1/pbu.egg-info/not-zip-safe
--rw-rw-r--   0 peter     (1000) peter     (1000)       35 2023-07-27 00:29:25.000000 pbu-1.1.1/pbu.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        4 2023-07-27 00:29:25.000000 pbu-1.1.1/pbu.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-27 00:29:25.446626 pbu-1.1.1/setup.cfg
--rw-rw-r--   0 peter     (1000) peter     (1000)      704 2023-07-27 00:27:26.000000 pbu-1.1.1/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-27 00:49:42.469335 pbu-1.1.2/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    28194 2023-07-27 00:49:42.469335 pbu-1.1.2/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)    22559 2023-04-08 00:03:20.000000 pbu-1.1.2/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-27 00:49:42.468335 pbu-1.1.2/pbu/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      863 2023-07-27 00:49:05.000000 pbu-1.1.2/pbu/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1733 2023-07-27 00:25:20.000000 pbu-1.1.2/pbu/app_config.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6264 2023-07-05 06:07:23.000000 pbu-1.1.2/pbu/basic_monitor.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      474 2021-02-28 01:39:36.000000 pbu-1.1.2/pbu/constant_listing.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5668 2023-07-13 00:10:51.000000 pbu-1.1.2/pbu/datascience_util.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3755 2022-04-12 02:57:09.000000 pbu-1.1.2/pbu/date_time.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      374 2023-07-05 06:00:07.000000 pbu-1.1.2/pbu/debug_object.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4224 2023-04-07 23:51:49.000000 pbu-1.1.2/pbu/default_options.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2104 2023-07-27 00:48:58.000000 pbu-1.1.2/pbu/files.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8739 2023-07-05 07:15:28.000000 pbu-1.1.2/pbu/json_document.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4757 2021-02-28 01:39:36.000000 pbu-1.1.2/pbu/json_wrapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6937 2022-08-12 05:35:20.000000 pbu-1.1.2/pbu/logger.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      304 2023-01-25 00:24:29.000000 pbu-1.1.2/pbu/paging.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1223 2023-04-11 09:50:57.000000 pbu-1.1.2/pbu/performance_logger.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    29256 2022-12-08 01:37:27.000000 pbu-1.1.2/pbu/time_series.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-27 00:49:42.469335 pbu-1.1.2/pbu.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    28194 2023-07-27 00:49:42.000000 pbu-1.1.2/pbu.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      468 2023-07-27 00:49:42.000000 pbu-1.1.2/pbu.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-27 00:49:42.000000 pbu-1.1.2/pbu.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2021-02-28 02:00:39.000000 pbu-1.1.2/pbu.egg-info/not-zip-safe
+-rw-rw-r--   0 peter     (1000) peter     (1000)       35 2023-07-27 00:49:42.000000 pbu-1.1.2/pbu.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        4 2023-07-27 00:49:42.000000 pbu-1.1.2/pbu.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-27 00:49:42.469335 pbu-1.1.2/setup.cfg
+-rw-rw-r--   0 peter     (1000) peter     (1000)      704 2023-07-27 00:49:10.000000 pbu-1.1.2/setup.py
```

### Comparing `pbu-1.1.1/PKG-INFO` & `pbu-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbu
-Version: 1.1.1
+Version: 1.1.2
 Summary: Basic Utility module for the Python programming language
 Home-page: https://github.com/ilfrich/python-basic-utils
 Author: Peter Ilfrich
 Author-email: das-peter@gmx.de
 License: Apache-2.0
 Description: # Python Basic Utilities `pbu`
```

### Comparing `pbu-1.1.1/README.md` & `pbu-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pbu-1.1.1/pbu/__init__.py` & `pbu-1.1.2/pbu/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 from pbu.default_options import default_options, default_value, list_find_one, list_map_filter, list_join, not_none
 from pbu.constant_listing import ConstantListing
 from pbu.performance_logger import PerformanceLogger
 from pbu.date_time import combine_date_time, to_utc, to_timezone, set_timezone, DATE_FORMAT, DATETIME_FORMAT
 from pbu.datascience_util import weighted_mean, normalise, discretise, compute_linear_function_parameters
 from pbu.app_config import BasicConfig
 from pbu.json_document import JsonDocument, list_to_json, list_from_json
-from pbu.files import write_json, read_json, ensure_directory
+from pbu.files import write_json, read_json, ensure_directory, convert_to_path
 from pbu.debug_object import DebugObject
```

### Comparing `pbu-1.1.1/pbu/app_config.py` & `pbu-1.1.2/pbu/app_config.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.1/pbu/basic_monitor.py` & `pbu-1.1.2/pbu/basic_monitor.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.1/pbu/datascience_util.py` & `pbu-1.1.2/pbu/datascience_util.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.1/pbu/date_time.py` & `pbu-1.1.2/pbu/date_time.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.1/pbu/default_options.py` & `pbu-1.1.2/pbu/default_options.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.1/pbu/json_document.py` & `pbu-1.1.2/pbu/json_document.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.1/pbu/json_wrapper.py` & `pbu-1.1.2/pbu/json_wrapper.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.1/pbu/logger.py` & `pbu-1.1.2/pbu/logger.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.1/pbu/performance_logger.py` & `pbu-1.1.2/pbu/performance_logger.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.1/pbu/time_series.py` & `pbu-1.1.2/pbu/time_series.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.1/pbu.egg-info/PKG-INFO` & `pbu-1.1.2/pbu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbu
-Version: 1.1.1
+Version: 1.1.2
 Summary: Basic Utility module for the Python programming language
 Home-page: https://github.com/ilfrich/python-basic-utils
 Author: Peter Ilfrich
 Author-email: das-peter@gmx.de
 License: Apache-2.0
 Description: # Python Basic Utilities `pbu`
```

### Comparing `pbu-1.1.1/setup.py` & `pbu-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="pbu",
-      version="1.1.1",
+      version="1.1.2",
       description="Basic Utility module for the Python programming language",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/ilfrich/python-basic-utils",
       author="Peter Ilfrich",
       author_email="das-peter@gmx.de",
       license="Apache-2.0",
```

