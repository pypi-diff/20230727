# Comparing `tmp/htsexperimentation-0.1.7.tar.gz` & `tmp/htsexperimentation-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htsexperimentation-0.1.7.tar", last modified: Tue Dec 20 10:23:57 2022, max compression
+gzip compressed data, was "htsexperimentation-0.1.8.tar", last modified: Thu Dec 29 21:10:33 2022, max compression
```

## Comparing `htsexperimentation-0.1.7.tar` & `htsexperimentation-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 10:23:57.507358 htsexperimentation-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2022-12-20 10:23:57.503358 htsexperimentation-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 10:23:57.503358 htsexperimentation-0.1.7/htsexperimentation/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 10:23:57.503358 htsexperimentation-0.1.7/htsexperimentation/compute_results/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/compute_results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/compute_results/compute_res_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 10:23:57.503358 htsexperimentation-0.1.7/htsexperimentation/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/helpers/file_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/helpers/helper_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 10:23:57.503358 htsexperimentation-0.1.7/htsexperimentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/tests/test_agg_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/tests/test_agg_results_prison.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/tests/test_calculating_compute_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/tests/test_parse_prison.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/tests/test_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 10:23:57.503358 htsexperimentation-0.1.7/htsexperimentation/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/htsexperimentation/visualization/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 10:23:57.503358 htsexperimentation-0.1.7/htsexperimentation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2022-12-20 10:23:57.000000 htsexperimentation-0.1.7/htsexperimentation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2022-12-20 10:23:57.000000 htsexperimentation-0.1.7/htsexperimentation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 10:23:57.000000 htsexperimentation-0.1.7/htsexperimentation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-20 10:23:57.000000 htsexperimentation-0.1.7/htsexperimentation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-20 10:23:57.000000 htsexperimentation-0.1.7/htsexperimentation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 10:23:57.507358 htsexperimentation-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2022-12-20 10:23:45.000000 htsexperimentation-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:10:33.456978 htsexperimentation-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2022-12-29 21:10:33.456978 htsexperimentation-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:10:33.452978 htsexperimentation-0.1.8/htsexperimentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:10:33.452978 htsexperimentation-0.1.8/htsexperimentation/compute_results/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/compute_results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/compute_results/compute_res_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/compute_results/results_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:10:33.452978 htsexperimentation-0.1.8/htsexperimentation/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/helpers/file_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/helpers/helper_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:10:33.452978 htsexperimentation-0.1.8/htsexperimentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/tests/test_agg_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/tests/test_agg_results_prison.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/tests/test_calculating_compute_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/tests/test_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:10:33.456978 htsexperimentation-0.1.8/htsexperimentation/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/htsexperimentation/visualization/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:10:33.452978 htsexperimentation-0.1.8/htsexperimentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2022-12-29 21:10:33.000000 htsexperimentation-0.1.8/htsexperimentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2022-12-29 21:10:33.000000 htsexperimentation-0.1.8/htsexperimentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 21:10:33.000000 htsexperimentation-0.1.8/htsexperimentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-29 21:10:33.000000 htsexperimentation-0.1.8/htsexperimentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-29 21:10:33.000000 htsexperimentation-0.1.8/htsexperimentation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-29 21:10:33.456978 htsexperimentation-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2022-12-29 21:10:17.000000 htsexperimentation-0.1.8/setup.py
```

### Comparing `htsexperimentation-0.1.7/PKG-INFO` & `htsexperimentation-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htsexperimentation
-Version: 0.1.7
+Version: 0.1.8
 Summary: Hierarchical time series forecasting package to help analyze experiments
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 Keywords: python,time series,hierarchical,forecasting,machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `htsexperimentation-0.1.7/htsexperimentation/compute_results/compute_res_funcs.py` & `htsexperimentation-0.1.8/htsexperimentation/compute_results/compute_res_funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import pandas as pd
 import pickle
 import copy
 import os
 from ..helpers.helper_func import keys_exists
 from ..helpers.file_handlers import parse_file_name
 
-
 def compute_aggreated_results_dict(
-    algorithm, dataset, path="../results_probabilistic", err_metric="mase"
+    algorithm, dataset, path="../results", err_metric="mase"
 ):
     results_dict = {}
     for file in [
         path
-        for path in os.listdir(path)
-        if algorithm in path and dataset in path and "orig" in path
+        for path in os.listdir(f"{path}/{algorithm}")
+        if dataset in path and "orig" in path
     ]:
-        with open(f"{path}/{file}", "rb") as handle:
+        with open(f"{path}/{algorithm}/{file}", "rb") as handle:
             sample, version, transformation = parse_file_name(file, dataset)
             if not keys_exists(results_dict, transformation):
                 results_dict[transformation] = {}
             if not keys_exists(results_dict, transformation, version):
                 results_dict[transformation][version] = {}
             if not keys_exists(results_dict, transformation, version, sample):
                 results_dict[transformation][version][sample] = {}
@@ -79,15 +78,15 @@
     )
 
     return df
 
 
 def agg_res_full_hierarchy(results_dict):
     df = compute_aggregated_results_df(results_dict)
-    df[['value']] = df[['value']].astype('float')
+    df[["value"]] = df[["value"]].astype("float")
     df = df.groupby(["group", "version", "sample", "error"]).mean().reset_index()
     df["group"] = df["group"].str.split("_").str[0]
     df["group"] = df["group"].str.lower()
     df.dropna(inplace=True)
 
     return df
 
@@ -107,15 +106,15 @@
         + "_"
         + df_bottom["group"].str.split("_").str[2]
     )
     return df_bottom.set_index("order").sort_values(by="order")
 
 
 def calculate_computing_time(
-    datasets: list, algorithms: list, path: str = "../results_probabilistic"
+    datasets: list, algorithms: list, path: str = "../results"
 ):
     res = []
     for d in datasets:
         for algo in algorithms:
             res.append(
                 pd.DataFrame(
                     compute_aggreated_results_dict(
@@ -125,15 +124,15 @@
                 )
             )
         df = pd.concat(res)
         pass
 
 
 def calculate_agg_results_all_datasets(
-    datasets: list, algorithms: list, err: str, path: str = "../results_probabilistic"
+    datasets: list, algorithms: list, err: str, path: str = "../results"
 ) -> list:
     """Calculate aggregated results for all datasets with the purpose of plotting
 
     Parameters
     ----------
     :param algorithms: list of algorithms
     :param datasets:  list of datasets
@@ -170,15 +169,15 @@
         df_orig.algorithm = df_orig.algorithm.astype("category")
         df_orig.algorithm.cat.set_categories(sorter, inplace=True)
         df_orig_list.append(df_orig)
 
     return df_orig_list
 
 
-def get_output(dataset, algorithm, transf, path="../results_probabilistic"):
+def get_output(dataset, algorithm, transf, path="../results"):
     for file in [
         path
         for path in os.listdir(path)
         if algorithm in path and dataset in path and "orig" in path and transf in path
     ]:
         with open(f"{path}/{file}", "rb") as handle:
             e = pickle.load(handle)
```

### Comparing `htsexperimentation-0.1.7/htsexperimentation/helpers/helper_func.py` & `htsexperimentation-0.1.8/htsexperimentation/helpers/helper_func.py`

 * *Files identical despite different names*

### Comparing `htsexperimentation-0.1.7/htsexperimentation/tests/test_agg_results.py` & `htsexperimentation-0.1.8/htsexperimentation/tests/test_agg_results.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from ..compute_results.compute_res_funcs import calculate_agg_results_all_datasets
+from ..compute_results.compute_res_funcs import calculate_agg_results_all_datasets, load_aggregate_results_algorithm
 from ..config import RESULTS_PATH
 
 
 class TestModel(unittest.TestCase):
     def setUp(self):
         self.datasets = ["prison", "tourism"]
         self.algorithms = ["gpf", "mint", "standard_gp_pie", "ets_bu", "deepar", "arima_bu"]
@@ -13,8 +13,8 @@
             calculate_agg_results_all_datasets(
                 self.datasets,
                 self.algorithms,
                 "mase",
                 path=RESULTS_PATH,
             )[1].shape
             == (1378, 6),
-        )
+        )
```

### Comparing `htsexperimentation-0.1.7/htsexperimentation/tests/test_agg_results_prison.py` & `htsexperimentation-0.1.8/htsexperimentation/tests/test_agg_results_prison.py`

 * *Files identical despite different names*

### Comparing `htsexperimentation-0.1.7/htsexperimentation/tests/test_calculating_compute_time.py` & `htsexperimentation-0.1.8/htsexperimentation/tests/test_calculating_compute_time.py`

 * *Files identical despite different names*

### Comparing `htsexperimentation-0.1.7/htsexperimentation/tests/test_plots.py` & `htsexperimentation-0.1.8/htsexperimentation/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `htsexperimentation-0.1.7/htsexperimentation/visualization/plotting.py` & `htsexperimentation-0.1.8/htsexperimentation/visualization/plotting.py`

 * *Files identical despite different names*

### Comparing `htsexperimentation-0.1.7/htsexperimentation.egg-info/PKG-INFO` & `htsexperimentation-0.1.8/htsexperimentation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htsexperimentation
-Version: 0.1.7
+Version: 0.1.8
 Summary: Hierarchical time series forecasting package to help analyze experiments
 Author: Luis Roque
 Author-email: <roque0luis@gmail.com>
 Keywords: python,time series,hierarchical,forecasting,machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `htsexperimentation-0.1.7/htsexperimentation.egg-info/SOURCES.txt` & `htsexperimentation-0.1.8/htsexperimentation.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 README.md
 setup.py
 htsexperimentation/__init__.py
-htsexperimentation/config.py
 htsexperimentation.egg-info/PKG-INFO
 htsexperimentation.egg-info/SOURCES.txt
 htsexperimentation.egg-info/dependency_links.txt
 htsexperimentation.egg-info/requires.txt
 htsexperimentation.egg-info/top_level.txt
 htsexperimentation/compute_results/__init__.py
 htsexperimentation/compute_results/compute_res_funcs.py
+htsexperimentation/compute_results/results_handler.py
 htsexperimentation/helpers/__init__.py
 htsexperimentation/helpers/file_handlers.py
 htsexperimentation/helpers/helper_func.py
 htsexperimentation/tests/__init__.py
 htsexperimentation/tests/test_agg_results.py
 htsexperimentation/tests/test_agg_results_prison.py
 htsexperimentation/tests/test_calculating_compute_time.py
-htsexperimentation/tests/test_parse_prison.py
 htsexperimentation/tests/test_plots.py
+htsexperimentation/tests/test_results.py
 htsexperimentation/visualization/__init__.py
 htsexperimentation/visualization/plotting.py
```

### Comparing `htsexperimentation-0.1.7/setup.py` & `htsexperimentation-0.1.8/setup.py`

 * *Files identical despite different names*

