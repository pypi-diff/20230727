# Comparing `tmp/pheno-utils-0.3.7.6.tar.gz` & `tmp/pheno-utils-0.3.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.7.6.tar", last modified: Wed Jul 26 08:40:52 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.7.7.tar", last modified: Thu Jul 27 12:53:44 2023, max compression
```

## Comparing `pheno-utils-0.3.7.6.tar` & `pheno-utils-0.3.7.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:40:52.841837 pheno-utils-0.3.7.6/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2361 2023-07-26 08:40:52.840707 pheno-utils-0.3.7.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1583 2023-07-26 07:07:45.000000 pheno-utils-0.3.7.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:40:52.787822 pheno-utils-0.3.7.6/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      344 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19064 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16533 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)    11559 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     4638 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/config.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7781 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    20116 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)    13188 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:40:52.831999 pheno-utils-0.3.7.6/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2361 2023-07-26 08:40:52.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-26 08:40:52.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 08:40:52.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-26 08:40:52.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-26 08:40:52.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 08:40:52.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      944 2023-07-26 08:40:26.000000 pheno-utils-0.3.7.6/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 08:40:52.842455 pheno-utils-0.3.7.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3842 2023-07-26 08:31:51.000000 pheno-utils-0.3.7.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:53:44.210536 pheno-utils-0.3.7.7/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-07-27 12:53:44.209557 pheno-utils-0.3.7.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1583 2023-07-26 07:07:45.000000 pheno-utils-0.3.7.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:53:44.158715 pheno-utils-0.3.7.7/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19064 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    11559 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     4638 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7781 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20118 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:53:44.203677 pheno-utils-0.3.7.7/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-07-27 12:53:43.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-27 12:53:43.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 12:53:43.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-27 12:53:43.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-27 12:53:43.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-27 12:53:43.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      944 2023-07-27 12:50:42.000000 pheno-utils-0.3.7.7/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 12:53:44.211037 pheno-utils-0.3.7.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-07-26 08:46:36.000000 pheno-utils-0.3.7.7/setup.py
```

### Comparing `pheno-utils-0.3.7.6/LICENSE` & `pheno-utils-0.3.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/PKG-INFO` & `pheno-utils-0.3.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.7.6
+Version: 0.3.7.7
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.7.6/README.md` & `pheno-utils-0.3.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils/_modidx.py` & `pheno-utils-0.3.7.7/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.7.7/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.7.7/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils/basic_plots.py` & `pheno-utils-0.3.7.7/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.7.7/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.7.7/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.7.7/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils/config.py` & `pheno-utils-0.3.7.7/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils/dates_plots.py` & `pheno-utils-0.3.7.7/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.7.7/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils/meta_loader.py` & `pheno-utils-0.3.7.7/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.7.7/pheno_utils/pheno_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,28 +367,29 @@
 
     def __load_dataframes__(self) -> None:
         """
         Load all tables in the dataset dictionary.
         """
         self.dfs = {}
         self.fields = set()
-        for relative_location in self.dict['relative_location'].dropna().unique():
-            # parquet_name = relative_location.split(os.sep)[-1]
-            parquet_name = os.sep.join(relative_location.split(os.sep)[2:])
+        for relative_location in self.dict['relative_location'].dropna().unique(): 
+            parquet_name = relative_location.split(os.sep)[-1]
+            internal_location = os.sep.join(relative_location.split(os.sep)[1:])
+            
             
             if any([pattern in relative_location for pattern in self.skip_dfs]):
                 print(f'Skipping {relative_location}')
                 continue
-            df = self.__load_one_dataframe__(parquet_name)
+            df = self.__load_one_dataframe__(internal_location)
             if df is None:
                 continue
-            table_name = parquet_name.split('.')[0].split(os.sep)[-1]
+            table_name = parquet_name.split('.')[0]
             self.dfs[table_name] = df
             if not df.index.is_unique:
-                print('Warning: index is not unique for', parquet_name)
+                print('Warning: index is not unique for', table_name)
             self.fields |= set(self.dfs[table_name].columns.tolist())
         self.fields = sorted(list(self.fields))
 
     def __load_one_dataframe__(self, relative_location: str) -> pd.DataFrame:
         """
         Load one dataframe.
```

### Comparing `pheno-utils-0.3.7.6/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.7.7/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.7.7/pheno_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.7.6
+Version: 0.3.7.7
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.7.6/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.7.7/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.6/settings.ini` & `pheno-utils-0.3.7.7/settings.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pheno-utils
 lib_name = pheno-utils
-version = 0.3.7.6
+version = 0.3.7.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pheno_utils
 nbs_path = nbs
 recursive = True
```

