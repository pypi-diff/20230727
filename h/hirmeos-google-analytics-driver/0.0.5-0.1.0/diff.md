# Comparing `tmp/hirmeos-google-analytics-driver-0.0.5.tar.gz` & `tmp/hirmeos-google-analytics-driver-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hirmeos-google-analytics-driver-0.0.5.tar", last modified: Fri Aug  7 21:10:02 2020, max compression
+gzip compressed data, was "dist/hirmeos-google-analytics-driver-0.1.0.tar", last modified: Thu Aug 13 10:29:50 2020, max compression
```

## Comparing `hirmeos-google-analytics-driver-0.0.5.tar` & `hirmeos-google-analytics-driver-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2020-08-07 21:10:02.000000 hirmeos-google-analytics-driver-0.0.5/
--rw-r--r--   0 rowan     (1000) rowan     (1000)     1752 2020-08-07 21:10:02.000000 hirmeos-google-analytics-driver-0.0.5/PKG-INFO
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2020-08-07 21:10:02.000000 hirmeos-google-analytics-driver-0.0.5/google_analytics_driver/
--rw-r--r--   0 rowan     (1000) rowan     (1000)      161 2019-11-21 11:10:25.000000 hirmeos-google-analytics-driver-0.0.5/google_analytics_driver/__init__.py
--rw-r--r--   0 rowan     (1000) rowan     (1000)     2625 2020-08-07 18:40:47.000000 hirmeos-google-analytics-driver-0.0.5/google_analytics_driver/clients.py
--rw-r--r--   0 rowan     (1000) rowan     (1000)     1649 2019-11-25 11:13:59.000000 hirmeos-google-analytics-driver-0.0.5/google_analytics_driver/logic.py
--rw-r--r--   0 rowan     (1000) rowan     (1000)        0 2019-11-20 12:48:37.000000 hirmeos-google-analytics-driver-0.0.5/google_analytics_driver/resolve.py
--rw-r--r--   0 rowan     (1000) rowan     (1000)     3397 2020-08-07 21:06:20.000000 hirmeos-google-analytics-driver-0.0.5/google_analytics_driver/retrieve.py
--rw-r--r--   0 rowan     (1000) rowan     (1000)     1928 2020-06-11 12:52:19.000000 hirmeos-google-analytics-driver-0.0.5/google_analytics_driver/service.py
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2020-08-07 21:10:02.000000 hirmeos-google-analytics-driver-0.0.5/hirmeos_google_analytics_driver.egg-info/
--rw-r--r--   0 rowan     (1000) rowan     (1000)     1752 2020-08-07 21:10:02.000000 hirmeos-google-analytics-driver-0.0.5/hirmeos_google_analytics_driver.egg-info/PKG-INFO
--rw-r--r--   0 rowan     (1000) rowan     (1000)      492 2020-08-07 21:10:02.000000 hirmeos-google-analytics-driver-0.0.5/hirmeos_google_analytics_driver.egg-info/SOURCES.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)        1 2020-08-07 21:10:02.000000 hirmeos-google-analytics-driver-0.0.5/hirmeos_google_analytics_driver.egg-info/dependency_links.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)       99 2020-08-07 21:10:02.000000 hirmeos-google-analytics-driver-0.0.5/hirmeos_google_analytics_driver.egg-info/requires.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)       24 2020-08-07 21:10:02.000000 hirmeos-google-analytics-driver-0.0.5/hirmeos_google_analytics_driver.egg-info/top_level.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)       38 2020-08-07 21:10:02.000000 hirmeos-google-analytics-driver-0.0.5/setup.cfg
--rw-r--r--   0 rowan     (1000) rowan     (1000)      873 2020-08-07 21:09:47.000000 hirmeos-google-analytics-driver-0.0.5/setup.py
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2020-08-13 10:29:50.000000 hirmeos-google-analytics-driver-0.1.0/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     2312 2020-08-13 10:29:50.000000 hirmeos-google-analytics-driver-0.1.0/PKG-INFO
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2020-08-13 10:29:50.000000 hirmeos-google-analytics-driver-0.1.0/google_analytics_driver/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      161 2019-11-21 11:10:25.000000 hirmeos-google-analytics-driver-0.1.0/google_analytics_driver/__init__.py
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     2625 2020-08-13 09:54:05.000000 hirmeos-google-analytics-driver-0.1.0/google_analytics_driver/clients.py
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     1695 2020-08-13 09:55:27.000000 hirmeos-google-analytics-driver-0.1.0/google_analytics_driver/logic.py
+-rw-r--r--   0 rowan     (1000) rowan     (1000)        0 2019-11-20 12:48:37.000000 hirmeos-google-analytics-driver-0.1.0/google_analytics_driver/resolve.py
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     3810 2020-08-13 09:49:50.000000 hirmeos-google-analytics-driver-0.1.0/google_analytics_driver/retrieve.py
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     1928 2020-06-11 12:52:19.000000 hirmeos-google-analytics-driver-0.1.0/google_analytics_driver/service.py
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2020-08-13 10:29:50.000000 hirmeos-google-analytics-driver-0.1.0/hirmeos_google_analytics_driver.egg-info/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)     2312 2020-08-13 10:29:50.000000 hirmeos-google-analytics-driver-0.1.0/hirmeos_google_analytics_driver.egg-info/PKG-INFO
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      492 2020-08-13 10:29:50.000000 hirmeos-google-analytics-driver-0.1.0/hirmeos_google_analytics_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)        1 2020-08-13 10:29:50.000000 hirmeos-google-analytics-driver-0.1.0/hirmeos_google_analytics_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       99 2020-08-13 10:29:50.000000 hirmeos-google-analytics-driver-0.1.0/hirmeos_google_analytics_driver.egg-info/requires.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       24 2020-08-13 10:29:50.000000 hirmeos-google-analytics-driver-0.1.0/hirmeos_google_analytics_driver.egg-info/top_level.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       38 2020-08-13 10:29:50.000000 hirmeos-google-analytics-driver-0.1.0/setup.cfg
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      873 2020-08-13 10:29:08.000000 hirmeos-google-analytics-driver-0.1.0/setup.py
```

### Comparing `hirmeos-google-analytics-driver-0.0.5/PKG-INFO` & `hirmeos-google-analytics-driver-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hirmeos-google-analytics-driver
-Version: 0.0.5
+Version: 0.1.0
 Summary: Functions required by google_analytics_driver
 Home-page: https://github.com/hirmeos/google_analytics_driver
 Author: Rowan Hatherley
 Author-email: rowan.hatherley@ubiquitypress.com
 License: UNKNOWN
 Description: Hirmeos google-analytics-driver Python library
         ==============================================
@@ -27,14 +27,26 @@
         
         Note: We are still in the early stages of this package so there will likely be
         many breaking changes as we go along.
         
         Release Notes:
         ==============
         
+        [0.1.0] - 2020-08-13
+        --------------------
+        Changed
+        .......
+         - Allow additional columns to be specified when generating GA row data.
+         - Allow identifier-type to be specified when resolving GA report so the driver
+           can match non-URL identifiers for events.
+         - Kwargs: `prefix`, `regexes` have been made optional as these are only used
+           for path/URL identifiers.
+         - Driver will attempt to order the columns in the GA row data to prevent
+           mismatching of fields.
+        
         [0.0.4] - 2020-06-11
         --------------------
         Changed
         .......
          - Turn off cache_discovery when running the build() command, which breaks
            services using oauth2client >= 4.0.0 or google-auth.
```

### Comparing `hirmeos-google-analytics-driver-0.0.5/google_analytics_driver/clients.py` & `hirmeos-google-analytics-driver-0.1.0/google_analytics_driver/clients.py`

 * *Files identical despite different names*

### Comparing `hirmeos-google-analytics-driver-0.0.5/google_analytics_driver/logic.py` & `hirmeos-google-analytics-driver-0.1.0/google_analytics_driver/logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,8 +59,8 @@
         row (list): Values from a row in the GA report.
 
     Returns:
         list: Values from a row in the GA report.
     """
     if len(row) == 2:
         row = ['/'] + row
-    return row
+    return row[:3]  # in case additional dimensions are used
```

### Comparing `hirmeos-google-analytics-driver-0.0.5/google_analytics_driver/retrieve.py` & `hirmeos-google-analytics-driver-0.1.0/google_analytics_driver/retrieve.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 def identify_columns(
         header_row,
-        identifier_name='',
+        identifier_name=None,
         country_code_name='ga:countryIsoCode',
         value_name=None,  # Value assumed to be last
         **extra_columns
 ):
-    """Optional call: Get index of relevant columns in each GA row.
+    """Find indices of relevant GA columns followed by remaining columns.
 
     Args:
         header_row (list): Column headers for the GA rows
         identifier_name (str): Name of GA dimension for the identifier.
         country_code_name (str): Name of GA dimension for the country.
         value_name (str): Name of GA dimension for the value.
 
     Returns:
         tuple: indexes of identifier, country and value in each GA row.
+
+    Used to reorder columns for downstream processing if more than 3 columns
+    are present in GA row data.
     """
-    value_index = header_row.index(value_name) if value_name else -1
+    total_columns = len(header_row)
+
+    if total_columns <= 3:  # try not to break previous implementations.
+        return list(range(total_columns))
 
-    return [
-        header_row.index(identifier_name),
+    all_indices = set(range(total_columns))
+
+    relevant_indices = [
+        header_row.index(identifier_name) if identifier_name else 0,
         header_row.index(country_code_name),
-        value_index,
+        header_row.index(value_name) if value_name else total_columns - 1,
     ] + [header_row.index(column) for column in extra_columns]
 
+    remaining_indices = list(all_indices - set(relevant_indices))
+
+    return relevant_indices + remaining_indices
+
 
 def generate_row_data(results, headers=None):
     """Yield headers and data from a Google Analytics report.
 
     Args:
         results (dict): Google Analytics statistics results.
         headers (dict): GA columns for identifier, country and value.
 
     Yields:
         list: CSV-style headers and data from the report.
     """
+    if not headers:
+        headers = {}
+
     report = results.get("reports")[0]
     column_header = report.get('columnHeader', {})
 
     metric_headers = column_header.get(
         'metricHeader', {}
     ).get('metricHeaderEntries', [])
 
     headers_row = column_header.get('dimensions', []).copy()
     headers_row.extend(header.get("name") for header in metric_headers)
 
-    header_indices = [i for i in range(len(headers_row))]
-
-    if headers:
-        header_indices = identify_columns(headers_row, **headers)
-        headers_row = [headers_row[i] for i in header_indices]
+    header_indices = identify_columns(headers_row, **headers)
+    headers_row = [headers_row[i] for i in header_indices]
 
     yield headers_row
 
     for row in report.get('data', {}).get('rows', []):
         full_row = row['dimensions'] + row['metrics'][0]['values']
         full_row = [full_row[i] for i in header_indices]
         yield full_row
```

### Comparing `hirmeos-google-analytics-driver-0.0.5/google_analytics_driver/service.py` & `hirmeos-google-analytics-driver-0.1.0/google_analytics_driver/service.py`

 * *Files identical despite different names*

### Comparing `hirmeos-google-analytics-driver-0.0.5/hirmeos_google_analytics_driver.egg-info/PKG-INFO` & `hirmeos-google-analytics-driver-0.1.0/hirmeos_google_analytics_driver.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hirmeos-google-analytics-driver
-Version: 0.0.5
+Version: 0.1.0
 Summary: Functions required by google_analytics_driver
 Home-page: https://github.com/hirmeos/google_analytics_driver
 Author: Rowan Hatherley
 Author-email: rowan.hatherley@ubiquitypress.com
 License: UNKNOWN
 Description: Hirmeos google-analytics-driver Python library
         ==============================================
@@ -27,14 +27,26 @@
         
         Note: We are still in the early stages of this package so there will likely be
         many breaking changes as we go along.
         
         Release Notes:
         ==============
         
+        [0.1.0] - 2020-08-13
+        --------------------
+        Changed
+        .......
+         - Allow additional columns to be specified when generating GA row data.
+         - Allow identifier-type to be specified when resolving GA report so the driver
+           can match non-URL identifiers for events.
+         - Kwargs: `prefix`, `regexes` have been made optional as these are only used
+           for path/URL identifiers.
+         - Driver will attempt to order the columns in the GA row data to prevent
+           mismatching of fields.
+        
         [0.0.4] - 2020-06-11
         --------------------
         Changed
         .......
          - Turn off cache_discovery when running the build() command, which breaks
            services using oauth2client >= 4.0.0 or google-auth.
```

### Comparing `hirmeos-google-analytics-driver-0.0.5/setup.py` & `hirmeos-google-analytics-driver-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'google-api-python-client>=1.7.11',
     'google-auth>=1.6.3',
 ]
 
 
 setup(
     name='hirmeos-google-analytics-driver',
-    version='0.0.5',
+    version='0.1.0',
     author='Rowan Hatherley',
     author_email='rowan.hatherley@ubiquitypress.com',
     description='Functions required by google_analytics_driver',
     install_requires=requirements,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/hirmeos/google_analytics_driver',
```

