# Comparing `tmp/pbu-1.1.0.tar.gz` & `tmp/pbu-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbu-1.1.0.tar", last modified: Wed Jul  5 07:21:23 2023, max compression
+gzip compressed data, was "pbu-1.1.1.tar", last modified: Thu Jul 27 00:29:25 2023, max compression
```

## Comparing `pbu-1.1.0.tar` & `pbu-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-05 07:21:23.030140 pbu-1.1.0/
--rw-rw-r--   0 peter     (1000) peter     (1000)    28194 2023-07-05 07:21:23.030140 pbu-1.1.0/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)    22559 2023-04-08 00:03:20.000000 pbu-1.1.0/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-05 07:21:23.030140 pbu-1.1.0/pbu/
--rw-rw-r--   0 peter     (1000) peter     (1000)      792 2023-07-05 05:55:01.000000 pbu-1.1.0/pbu/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1733 2022-12-08 02:17:54.000000 pbu-1.1.0/pbu/app_config.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6264 2023-07-05 06:07:23.000000 pbu-1.1.0/pbu/basic_monitor.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      474 2021-02-28 01:39:36.000000 pbu-1.1.0/pbu/constant_listing.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4383 2023-04-08 01:50:06.000000 pbu-1.1.0/pbu/datascience_util.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3755 2022-04-12 02:57:09.000000 pbu-1.1.0/pbu/date_time.py
--rw-r--r--   0 peter     (1000) peter     (1000)      374 2023-07-05 06:00:07.000000 pbu-1.1.0/pbu/debug_object.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4224 2023-04-07 23:51:49.000000 pbu-1.1.0/pbu/default_options.py
--rw-r--r--   0 peter     (1000) peter     (1000)      993 2023-04-03 04:48:29.000000 pbu-1.1.0/pbu/files.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8739 2023-07-05 07:15:28.000000 pbu-1.1.0/pbu/json_document.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4757 2021-02-28 01:39:36.000000 pbu-1.1.0/pbu/json_wrapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6937 2022-08-12 05:35:20.000000 pbu-1.1.0/pbu/logger.py
--rw-r--r--   0 peter     (1000) peter     (1000)      304 2023-01-25 00:24:29.000000 pbu-1.1.0/pbu/paging.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1223 2023-04-11 09:50:57.000000 pbu-1.1.0/pbu/performance_logger.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    29256 2022-12-08 01:37:27.000000 pbu-1.1.0/pbu/time_series.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-05 07:21:23.030140 pbu-1.1.0/pbu.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)    28194 2023-07-05 07:21:22.000000 pbu-1.1.0/pbu.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      468 2023-07-05 07:21:22.000000 pbu-1.1.0/pbu.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-05 07:21:22.000000 pbu-1.1.0/pbu.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2021-02-28 02:00:39.000000 pbu-1.1.0/pbu.egg-info/not-zip-safe
--rw-rw-r--   0 peter     (1000) peter     (1000)       35 2023-07-05 07:21:22.000000 pbu-1.1.0/pbu.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        4 2023-07-05 07:21:22.000000 pbu-1.1.0/pbu.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-05 07:21:23.030140 pbu-1.1.0/setup.cfg
--rw-rw-r--   0 peter     (1000) peter     (1000)      704 2023-07-05 07:11:36.000000 pbu-1.1.0/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-27 00:29:25.446626 pbu-1.1.1/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    28194 2023-07-27 00:29:25.446626 pbu-1.1.1/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)    22559 2023-04-08 00:03:20.000000 pbu-1.1.1/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-27 00:29:25.445625 pbu-1.1.1/pbu/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      846 2023-07-27 00:27:21.000000 pbu-1.1.1/pbu/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1733 2023-07-27 00:25:20.000000 pbu-1.1.1/pbu/app_config.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6264 2023-07-05 06:07:23.000000 pbu-1.1.1/pbu/basic_monitor.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      474 2021-02-28 01:39:36.000000 pbu-1.1.1/pbu/constant_listing.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5668 2023-07-13 00:10:51.000000 pbu-1.1.1/pbu/datascience_util.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3755 2022-04-12 02:57:09.000000 pbu-1.1.1/pbu/date_time.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      374 2023-07-05 06:00:07.000000 pbu-1.1.1/pbu/debug_object.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4224 2023-04-07 23:51:49.000000 pbu-1.1.1/pbu/default_options.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1290 2023-07-27 00:27:10.000000 pbu-1.1.1/pbu/files.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8739 2023-07-05 07:15:28.000000 pbu-1.1.1/pbu/json_document.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4757 2021-02-28 01:39:36.000000 pbu-1.1.1/pbu/json_wrapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6937 2022-08-12 05:35:20.000000 pbu-1.1.1/pbu/logger.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      304 2023-01-25 00:24:29.000000 pbu-1.1.1/pbu/paging.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1223 2023-04-11 09:50:57.000000 pbu-1.1.1/pbu/performance_logger.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    29256 2022-12-08 01:37:27.000000 pbu-1.1.1/pbu/time_series.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-27 00:29:25.446626 pbu-1.1.1/pbu.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    28194 2023-07-27 00:29:25.000000 pbu-1.1.1/pbu.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      468 2023-07-27 00:29:25.000000 pbu-1.1.1/pbu.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-27 00:29:25.000000 pbu-1.1.1/pbu.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2021-02-28 02:00:39.000000 pbu-1.1.1/pbu.egg-info/not-zip-safe
+-rw-rw-r--   0 peter     (1000) peter     (1000)       35 2023-07-27 00:29:25.000000 pbu-1.1.1/pbu.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        4 2023-07-27 00:29:25.000000 pbu-1.1.1/pbu.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-27 00:29:25.446626 pbu-1.1.1/setup.cfg
+-rw-rw-r--   0 peter     (1000) peter     (1000)      704 2023-07-27 00:27:26.000000 pbu-1.1.1/setup.py
```

### Comparing `pbu-1.1.0/PKG-INFO` & `pbu-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbu
-Version: 1.1.0
+Version: 1.1.1
 Summary: Basic Utility module for the Python programming language
 Home-page: https://github.com/ilfrich/python-basic-utils
 Author: Peter Ilfrich
 Author-email: das-peter@gmx.de
 License: Apache-2.0
 Description: # Python Basic Utilities `pbu`
```

### Comparing `pbu-1.1.0/README.md` & `pbu-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pbu-1.1.0/pbu/__init__.py` & `pbu-1.1.1/pbu/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 from pbu.time_series import TimeSeries
 from pbu.paging import PagingInformation
 from pbu.basic_monitor import BasicMonitor, JobStatus
 from pbu.default_options import default_options, default_value, list_find_one, list_map_filter, list_join, not_none
 from pbu.constant_listing import ConstantListing
 from pbu.performance_logger import PerformanceLogger
 from pbu.date_time import combine_date_time, to_utc, to_timezone, set_timezone, DATE_FORMAT, DATETIME_FORMAT
-from pbu.datascience_util import weighted_mean, normalise, discretise
+from pbu.datascience_util import weighted_mean, normalise, discretise, compute_linear_function_parameters
 from pbu.app_config import BasicConfig
 from pbu.json_document import JsonDocument, list_to_json, list_from_json
-from pbu.files import write_json, read_json
+from pbu.files import write_json, read_json, ensure_directory
 from pbu.debug_object import DebugObject
```

### Comparing `pbu-1.1.0/pbu/app_config.py` & `pbu-1.1.1/pbu/app_config.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.0/pbu/basic_monitor.py` & `pbu-1.1.1/pbu/basic_monitor.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.0/pbu/datascience_util.py` & `pbu-1.1.1/pbu/datascience_util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Optional
+from typing import List, Union, Optional, Tuple
 from statistics import mean
 
 
 def weighted_mean(values: List[Union[float, int]], weights: List[Union[int, float]] = []) -> Optional[float]:
     """
     This will generate a mean value for the list of provided `values`, where each value is multiplied by the
     corresponding weight in the same position. If there are more `values` than `weights`, remaining values will receive
@@ -64,23 +64,27 @@
 
     if value > max_value and limit is True:
         return 1.0 if inverted is False else 0.0
 
     if max_value == min_value:
         return 0.5
 
-    norm = 0.5  # just in case
+    def _handle_return(norm):
+        return norm if inverted is False else 1.0 - norm  # handle inverted flag
+
     if mid_point is None:
-        norm = (float(value) - float(min_value)) / (float(max_value) - float(min_value))
+        return _handle_return((float(value) - float(min_value)) / (float(max_value) - float(min_value)))
     else:
         if value <= mid_point:
-            norm = ((float(value) - float(min_value)) / (float(mid_point) - float(min_value))) * 0.5
+            # value is below mid-point (return 0 - 0.5)
+            return _handle_return(((float(value) - float(min_value)) / (float(mid_point) - float(min_value))) * 0.5)
         else:
-            norm = (((float(value) - float(mid_point)) / (float(max_value) - float(mid_point))) * 0.5) + 0.5
-    return norm if inverted is False else 1.0 - norm
+            # value is above mid-point (return 0.5 - 1.0)
+            return _handle_return(
+                (((float(value) - float(mid_point)) / (float(max_value) - float(mid_point))) * 0.5) + 0.5)
 
 
 def discretise(value: Union[float, int], precision: Union[float, int] = 1, floor=False,
                ceil=False) -> Union[float, int]:
     """
     This function will round the given value to the nearest multiple of the given precision. There are 2 boolean flags
     available that can force the function to return the lower or upper boundary of a precision interval. If neither is
@@ -96,7 +100,41 @@
     remainder = value % precision
     if ceil is True:
         return value - remainder + precision
     if floor is True:
         return value - remainder
     # mid point is default fallback
     return (value - remainder) + (precision * 0.5)
+
+
+def compute_linear_function_parameters(xy_points: List[tuple]) -> Tuple[float, float, float]:
+    """
+    Computes m and b to minimise the error of all given points to map onto a linear function y = m * x + b.
+    :param xy_points: a list of tuples representing the (x, y) points
+    :return: a tuple with 3 elements containing the parameters m, b and the total (sum) error of all points when
+    comparing against the linear function.
+    """
+    n = len(xy_points)
+
+    # arrays to store all the elements
+    x2 = []  # x squared
+    xy = []  # x * y
+    x = []  # all x-values
+    y = []  # all y-values
+
+    # collect all point data
+    for (x_val, y_val) in xy_points:
+        x2.append(x_val * x_val)
+        xy.append(x_val * y_val)
+        x.append(x_val)
+        y.append(y_val)
+
+    # determine m and b
+    m = ((n * sum(xy)) - (sum(x) * sum(y))) / ((n * sum(x2)) - (sum(x) * sum(x)))
+    b = (sum(y) - (m * sum(x))) / n
+
+    # calculate total error
+    error = 0.0
+    for (x, y) in xy_points:
+        error += abs(y - ((m * x) + b))
+
+    return m, b, error
```

### Comparing `pbu-1.1.0/pbu/date_time.py` & `pbu-1.1.1/pbu/date_time.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.0/pbu/default_options.py` & `pbu-1.1.1/pbu/default_options.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.0/pbu/files.py` & `pbu-1.1.1/pbu/files.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,7 +25,16 @@
     """
     if not os.path.exists(path):
         return None
     fp = open(path)
     data = json.load(fp)
     fp.close()
     return data
+
+
+def ensure_directory(path: str):
+    """
+    Makes sure a certain directory exists. If it doesn't exist, the directory will be created.
+    :param path: a path reference (absolute or relative) to the directory that should exist.
+    """
+    if not os.path.isdir(path):
+        os.makedirs(path)
```

### Comparing `pbu-1.1.0/pbu/json_document.py` & `pbu-1.1.1/pbu/json_document.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.0/pbu/json_wrapper.py` & `pbu-1.1.1/pbu/json_wrapper.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.0/pbu/logger.py` & `pbu-1.1.1/pbu/logger.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.0/pbu/performance_logger.py` & `pbu-1.1.1/pbu/performance_logger.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.0/pbu/time_series.py` & `pbu-1.1.1/pbu/time_series.py`

 * *Files identical despite different names*

### Comparing `pbu-1.1.0/pbu.egg-info/PKG-INFO` & `pbu-1.1.1/pbu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbu
-Version: 1.1.0
+Version: 1.1.1
 Summary: Basic Utility module for the Python programming language
 Home-page: https://github.com/ilfrich/python-basic-utils
 Author: Peter Ilfrich
 Author-email: das-peter@gmx.de
 License: Apache-2.0
 Description: # Python Basic Utilities `pbu`
```

### Comparing `pbu-1.1.0/setup.py` & `pbu-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="pbu",
-      version="1.1.0",
+      version="1.1.1",
       description="Basic Utility module for the Python programming language",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/ilfrich/python-basic-utils",
       author="Peter Ilfrich",
       author_email="das-peter@gmx.de",
       license="Apache-2.0",
```

