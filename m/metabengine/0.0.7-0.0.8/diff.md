# Comparing `tmp/metabengine-0.0.7.tar.gz` & `tmp/metabengine-0.0.8.tar.gz`

## Comparing `metabengine-0.0.7.tar` & `metabengine-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 metabengine-0.0.7/src/metabengine/__init__.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 metabengine-0.0.7/src/metabengine/alignment.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 metabengine-0.0.7/src/metabengine/ann_feat_quality.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 metabengine-0.0.7/src/metabengine/calculate_mass.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 metabengine-0.0.7/src/metabengine/feature_grouping.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 metabengine-0.0.7/src/metabengine/msms.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 metabengine-0.0.7/src/metabengine/params.py
--rw-r--r--   0        0        0    13699 2020-02-02 00:00:00.000000 metabengine-0.0.7/src/metabengine/peak_detect.py
--rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 metabengine-0.0.7/src/metabengine/raw_data_utils.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 metabengine-0.0.7/src/metabengine/targeted_search.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 metabengine-0.0.7/src/metabengine/visual.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 metabengine-0.0.7/LICENSE
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 metabengine-0.0.7/README.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 metabengine-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 metabengine-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 metabengine-0.0.8/src/metabengine/__init__.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 metabengine-0.0.8/src/metabengine/alignment.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 metabengine-0.0.8/src/metabengine/ann_feat_quality.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 metabengine-0.0.8/src/metabengine/calculate_mass.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 metabengine-0.0.8/src/metabengine/feature_grouping.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 metabengine-0.0.8/src/metabengine/msms.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 metabengine-0.0.8/src/metabengine/params.py
+-rw-r--r--   0        0        0    13699 2020-02-02 00:00:00.000000 metabengine-0.0.8/src/metabengine/peak_detect.py
+-rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 metabengine-0.0.8/src/metabengine/raw_data_utils.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 metabengine-0.0.8/src/metabengine/targeted_search.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 metabengine-0.0.8/src/metabengine/visual.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 metabengine-0.0.8/LICENSE
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 metabengine-0.0.8/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 metabengine-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 metabengine-0.0.8/PKG-INFO
```

### Comparing `metabengine-0.0.7/src/metabengine/__init__.py` & `metabengine-0.0.8/src/metabengine/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,8 +42,20 @@
         print('Running alignment on: ', file_name)
         alignement(feature_list, d, cross_file_params)
     
     # choose the best MS2 for each feature
     for feat in feature_list:
         feat.choose_best_ms2()
     
-    return feature_list
+    return feature_list
+
+
+def read_raw_file_to_obj(file_name, estimate_param=False):
+    d = raw.MSData()
+    params = Params()
+    d.read_raw_data(file_name, params)
+
+    if estimate_param:
+        params.estimate_params(d)
+        d.params = params
+    
+    return d
```

### Comparing `metabengine-0.0.7/src/metabengine/alignment.py` & `metabengine-0.0.8/src/metabengine/alignment.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.7/src/metabengine/ann_feat_quality.py` & `metabengine-0.0.8/src/metabengine/ann_feat_quality.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.7/src/metabengine/calculate_mass.py` & `metabengine-0.0.8/src/metabengine/calculate_mass.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.7/src/metabengine/feature_grouping.py` & `metabengine-0.0.8/src/metabengine/feature_grouping.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.7/src/metabengine/msms.py` & `metabengine-0.0.8/src/metabengine/msms.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.7/src/metabengine/params.py` & `metabengine-0.0.8/src/metabengine/params.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.7/src/metabengine/peak_detect.py` & `metabengine-0.0.8/src/metabengine/peak_detect.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.7/src/metabengine/raw_data_utils.py` & `metabengine-0.0.8/src/metabengine/raw_data_utils.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.7/src/metabengine/targeted_search.py` & `metabengine-0.0.8/src/metabengine/targeted_search.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.7/LICENSE` & `metabengine-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.7/pyproject.toml` & `metabengine-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metabengine"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 maintainers = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 description = "Data preprocessing for mass spectrometry-based metabolomics data"
```

### Comparing `metabengine-0.0.7/PKG-INFO` & `metabengine-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabengine
-Version: 0.0.7
+Version: 0.0.8
 Summary: Data preprocessing for mass spectrometry-based metabolomics data
 Project-URL: Homepage, https://github.com/Waddlessss/metabengine
 Author-email: Huaxu Yu <yhxchem@outlook.com>
 Maintainer-email: Huaxu Yu <yhxchem@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

