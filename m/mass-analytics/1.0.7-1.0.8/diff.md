# Comparing `tmp/mass_analytics-1.0.7.tar.gz` & `tmp/mass_analytics-1.0.8.tar.gz`

## Comparing `mass_analytics-1.0.7.tar` & `mass_analytics-1.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/src/mass_analytics/__init__.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/src/mass_analytics/data_frame_util.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/src/mass_analytics/date.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/src/mass_analytics/reader.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/LICENSE.txt
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/README.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 mass_analytics-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mass_analytics-1.0.8/src/mass_analytics/__init__.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 mass_analytics-1.0.8/src/mass_analytics/data_frame_util.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 mass_analytics-1.0.8/src/mass_analytics/date.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 mass_analytics-1.0.8/src/mass_analytics/reader.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 mass_analytics-1.0.8/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 mass_analytics-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 mass_analytics-1.0.8/PKG-INFO
```

### Comparing `mass_analytics-1.0.7/src/mass_analytics/date.py` & `mass_analytics-1.0.8/src/mass_analytics/date.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 def is_date(string):
     """
     Return whether the string can be interpreted as a date.
 
     Parameters:
         string (str): string to check for date
     """
+    
     try:
         if type(string) is not str:
             return False 
         parse(string, fuzzy=False)
         return True
 
     except ValueError:
```

### Comparing `mass_analytics-1.0.7/src/mass_analytics/reader.py` & `mass_analytics-1.0.8/src/mass_analytics/reader.py`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.0.7/LICENSE.txt` & `mass_analytics-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.0.7/README.md` & `mass_analytics-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.0.7/PKG-INFO` & `mass_analytics-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mass_analytics
-Version: 1.0.7
-Summary: A small example package for mass-analytics
+Version: 1.0.8
+Summary: Streamline data preprocessing and enhance analysis with our Powerful Data Preparation Package.
 Author-email: Selim <selim.alouini@mass-analytics.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy==1.25.1
```

