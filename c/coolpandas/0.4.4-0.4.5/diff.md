# Comparing `tmp/coolpandas-0.4.4.tar.gz` & `tmp/coolpandas-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolpandas-0.4.4.tar", last modified: Thu Jul 13 15:05:31 2023, max compression
+gzip compressed data, was "coolpandas-0.4.5.tar", last modified: Thu Jul 27 16:12:07 2023, max compression
```

## Comparing `coolpandas-0.4.4.tar` & `coolpandas-0.4.5.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.852748 coolpandas-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 15:05:08.000000 coolpandas-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-13 15:05:31.852748 coolpandas-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-13 15:05:08.000000 coolpandas-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.844748 coolpandas-0.4.4/coolpandas/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.848748 coolpandas-0.4.4/coolpandas/connect/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/connect/redshift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.848748 coolpandas-0.4.4/coolpandas/eda/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/features_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/geo_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/random_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/value_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.848748 coolpandas-0.4.4/coolpandas/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/evaluate/confusion_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.848748 coolpandas-0.4.4/coolpandas/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/distplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/geoplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/lineplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/mapplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.848748 coolpandas-0.4.4/coolpandas/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/stats/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/stats/ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.852748 coolpandas-0.4.4/coolpandas/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/transform/bin.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/transform/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/transform/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/transform/outliers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.852748 coolpandas-0.4.4/coolpandas/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/utils/random_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.848748 coolpandas-0.4.4/coolpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-13 15:05:31.000000 coolpandas-0.4.4/coolpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 15:05:31.000000 coolpandas-0.4.4/coolpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:05:31.000000 coolpandas-0.4.4/coolpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 15:05:31.000000 coolpandas-0.4.4/coolpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 15:05:31.000000 coolpandas-0.4.4/coolpandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-13 15:05:08.000000 coolpandas-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:05:31.852748 coolpandas-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.076561 coolpandas-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 16:11:46.000000 coolpandas-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-27 16:12:07.076561 coolpandas-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-27 16:11:46.000000 coolpandas-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.068561 coolpandas-0.4.5/coolpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.068561 coolpandas-0.4.5/coolpandas/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/connect/redshift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.072561 coolpandas-0.4.5/coolpandas/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/features_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/geo_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/value_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.072561 coolpandas-0.4.5/coolpandas/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/evaluate/confusion_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.076561 coolpandas-0.4.5/coolpandas/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/distplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/geoplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/mapplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.076561 coolpandas-0.4.5/coolpandas/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/stats/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/stats/ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.076561 coolpandas-0.4.5/coolpandas/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/transform/bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/transform/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/transform/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/transform/outliers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.076561 coolpandas-0.4.5/coolpandas/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/utils/random_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.068561 coolpandas-0.4.5/coolpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-27 16:12:07.000000 coolpandas-0.4.5/coolpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-27 16:12:07.000000 coolpandas-0.4.5/coolpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:12:07.000000 coolpandas-0.4.5/coolpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-27 16:12:07.000000 coolpandas-0.4.5/coolpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 16:12:07.000000 coolpandas-0.4.5/coolpandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-27 16:11:46.000000 coolpandas-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 16:12:07.076561 coolpandas-0.4.5/setup.cfg
```

### Comparing `coolpandas-0.4.4/LICENSE` & `coolpandas-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/PKG-INFO` & `coolpandas-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.4.4/README.md` & `coolpandas-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/connect/redshift.py` & `coolpandas-0.4.5/coolpandas/connect/redshift.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/eda/__init__.py` & `coolpandas-0.4.5/coolpandas/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/eda/correlation.py` & `coolpandas-0.4.5/coolpandas/eda/correlation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 
 import numpy as np
 import pandas as pd
 
-from coolpandas.plot import mapplot
+from coolpandas.plot import confusion_matrix
 
 
 def get_correlation(
     data_frame: pd.DataFrame, method: str = "pearson", plot: bool = True, **kwargs
 ) -> pd.DataFrame:
     """Get the correlations of a DataFrame.
 
@@ -20,14 +20,10 @@
     Returns:
         pd.DataFrame: Correlations.
     """
     correlation_matrix: pd.DataFrame = data_frame.corr(method=method)
     truncate: callable = lambda x: math.trunc(100 * x) / 100
     correlation_matrix = correlation_matrix.applymap(truncate)
     if plot:
-        mask = np.triu(np.ones_like(correlation_matrix, dtype=bool))
-        mapplot(
-            correlation_matrix.mask(mask),
-            title=f"{method.capitalize()} correlation map",
-            **kwargs,
-        ).show()
+        fig = confusion_matrix(data_frame, **kwargs)
+        fig.show()
     return correlation_matrix
```

### Comparing `coolpandas-0.4.4/coolpandas/eda/distribution.py` & `coolpandas-0.4.5/coolpandas/eda/distribution.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/eda/duplicates.py` & `coolpandas-0.4.5/coolpandas/eda/duplicates.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     return duplicated_data_frame
 
 
 def duplicated_columns(
     data_frame: pd.DataFrame, display_summary: bool = True, drop: bool = False
 ) -> pd.DataFrame:
     """Get duplicated columns in a DataFrame and drop them if specified.
+
     Args:
         data_frame (pd.DataFrame): DataFrame to get duplicated columns.
         display_summary (bool, optional): Whether to display summary. Defaults to True.
         drop (bool, optional): Whether to drop duplicated columns. Defaults to True.
+
     Returns:
         pd.DataFrame: Duplicated columns.
     """
-    # uniques, indexes = np.unique(data_frame, return_index=True, axis=1)
-    # return pd.DataFrame(uniq, index=data_frame.index, columns=data_frame.columns[~indexes])
     duplicates: pd.Series = data_frame.apply(lambda x: x.duplicated(), axis=1).all()
     duplicated_data_frame: pd.DataFrame = data_frame[duplicates[duplicates].index]
     if display_summary:
         print(f"Number of duplicated columns: {duplicated_data_frame.shape[1]}")
     if drop:
         data_frame.drop(columns=duplicated_data_frame.columns, inplace=True)
     if display_summary and drop:
```

### Comparing `coolpandas-0.4.4/coolpandas/eda/features_type.py` & `coolpandas-0.4.5/coolpandas/eda/features_type.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/eda/geo_distance.py` & `coolpandas-0.4.5/coolpandas/eda/geo_distance.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/eda/missing_values.py` & `coolpandas-0.4.5/coolpandas/eda/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/eda/shape.py` & `coolpandas-0.4.5/coolpandas/eda/shape.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,10 +18,12 @@
     summary["rows_number"], summary["columns_number"] = data_frame.shape
     summary["columns_name"] = data_frame.columns.tolist()
     summary["columns_type"] = data_frame.dtypes.tolist()
     if display_summary:
         display(data_frame.head())
         print(f"Number of rows: {summary.get('rows_number')}")
         print(f"Number of columns: {summary.get('columns_number')}")
-        print(f"Columns name: {summary['columns_name']}")
-        print(f"Columns type: {summary['columns_type']}")
+        columns_info: list[tuple[str, str]] = list(
+            zip(summary["columns_name"], summary["columns_type"])
+        )
+        print(f"Columns: {columns_info}")
     return summary
```

### Comparing `coolpandas-0.4.4/coolpandas/eda/summary.py` & `coolpandas-0.4.5/coolpandas/eda/summary.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/eda/value_counts.py` & `coolpandas-0.4.5/coolpandas/eda/value_counts.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/evaluate/confusion_matrix.py` & `coolpandas-0.4.5/coolpandas/evaluate/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/plot/barplot.py` & `coolpandas-0.4.5/coolpandas/plot/barplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .style import custom_template, format_title
 
 
 def barplot(
     data_frame: pd.DataFrame,
     x_axis: str,
     y_axis: str,
-    title: str,
+    title: str = "",
     subtitle: str | None = None,
     **kwargs,
 ) -> go.Figure:
     """Create a bar plot.
 
     Args:
         data_frame (pd.DataFrame): DataFrame to plot.
```

### Comparing `coolpandas-0.4.4/coolpandas/plot/boxplot.py` & `coolpandas-0.4.5/coolpandas/plot/boxplot.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .style import custom_template, format_title
 
 
 def boxplot(
     data_frame: pd.DataFrame,
     x_axis: str,
     y_axis: str,
-    title: str,
+    title: str = "",
     subtitle: str | None = None,
     outliers: bool = True,
     **kwargs,
 ) -> go.Figure:
     """Create a box plot.
 
     Args:
```

### Comparing `coolpandas-0.4.4/coolpandas/plot/distplot.py` & `coolpandas-0.4.5/coolpandas/plot/distplot.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from .style import custom_template, format_title
 
 
 def distplot(
     data_frame: pd.DataFrame,
     x_axis: str,
-    y_axis: str,
-    title: str,
+    y_axis: str | None = None,
+    title: str = "",
     subtitle: str | None = None,
     **kwargs,
 ) -> go.Figure:
     """Create a bar plot.
 
     Args:
         data_frame (pd.DataFrame): DataFrame to plot.
```

### Comparing `coolpandas-0.4.4/coolpandas/plot/geoplot.py` & `coolpandas-0.4.5/coolpandas/plot/geoplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .style import custom_template, format_title
 
 
 def geoplot(
     data_frame: pd.DataFrame,
     lat: str,
     lon: str,
-    title: str,
+    title: str = "",
     subtitle: str | None = None,
     **kwargs,
 ) -> go.Figure:
     """Create a map plot based on latitude and longitude of DataFrame passed columns.
 
     Args:
         data_frame (pd.DataFrame): DataFrame to plot.
```

### Comparing `coolpandas-0.4.4/coolpandas/plot/lineplot.py` & `coolpandas-0.4.5/coolpandas/plot/lineplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .style import custom_template, format_title
 
 
 def lineplot(
     data_frame: pd.DataFrame,
     x_axis: str,
     y_axis: str,
-    title: str,
+    title: str = "",
     subtitle: str | None = None,
     **kwargs,
 ) -> go.Figure:
     """Create a bar plot.
 
     Args:
         data_frame (pd.DataFrame): DataFrame to plot.
```

### Comparing `coolpandas-0.4.4/coolpandas/plot/mapplot.py` & `coolpandas-0.4.5/coolpandas/plot/mapplot.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import plotly.graph_objects as go
 
 from .style import custom_template, format_title
 
 
 def mapplot(
     matrix: pd.DataFrame,
-    title: str,
+    title: str = "",
     subtitle: str | None = None,
     width: int = 1000,
     height: int = 1000,
     **kwargs,
 ) -> go.Figure:
     """Create a correlation map.
```

### Comparing `coolpandas-0.4.4/coolpandas/plot/scatterplot.py` & `coolpandas-0.4.5/coolpandas/plot/scatterplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .style import custom_template, format_title
 
 
 def scatterplot(
     data_frame: pd.DataFrame,
     x_axis: str,
     y_axis: str,
-    title: str,
+    title: str = "",
     subtitle: str | None = None,
     **kwargs,
 ) -> go.Figure:
     """Create a scatter plot.
 
     Args:
         data_frame (pd.DataFrame): DataFrame to plot.
```

### Comparing `coolpandas-0.4.4/coolpandas/plot/style.py` & `coolpandas-0.4.5/coolpandas/plot/style.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/stats/effect.py` & `coolpandas-0.4.5/coolpandas/stats/effect.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/stats/ttest.py` & `coolpandas-0.4.5/coolpandas/stats/ttest.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/transform/bin.py` & `coolpandas-0.4.5/coolpandas/transform/bin.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/transform/missing_values.py` & `coolpandas-0.4.5/coolpandas/transform/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.4/coolpandas/transform/outliers.py` & `coolpandas-0.4.5/coolpandas/transform/outliers.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,45 +2,51 @@
 import pandas as pd
 
 
 def iqr_outliers(
     data_frame: pd.DataFrame,
     column: str,
     threshold: float = 1.5,
+    transform_outliers: bool = False,
     create_outlier_column: bool = False,
     lower_bound: float | None = None,
     upper_bound: float | None = None,
 ) -> pd.DataFrame:
     """Transform outliers using the interquartile range method. If the lower_bound and upper_bound are not provided, they will be calculated using the threshold.
 
     Args:
         data_frame (pd.DataFrame): DataFrame to get outliers from.
         column (str): Column to get outliers from.
         threshold (float, optional): Threshold to use. Defaults to 1.5.
+        transform_outliers (bool, optional): Whether to transform outliers.
         create_outlier_column (bool, optional): Whether to create a column with
         outliers. Defaults to False.
         lower_bound (float, optional): Lower bound to use. Defaults to None.
         upper_bound (float, optional): Upper bound to use. Defaults to None.
 
     Returns:
         pd.DataFrame: DataFrame with outliers.
+        float: Lower bound.
+        float: Upper bound.
     """
     if lower_bound is None or upper_bound is None:
         quartile_1: float = data_frame[column].quantile(0.25)
         quartile_3: float = data_frame[column].quantile(0.75)
         iqr: float = quartile_3 - quartile_1
-    if lower_bound is None:
-        lower_bound: float = quartile_1 - (threshold * iqr)
-    if upper_bound is None:
-        upper_bound: float = quartile_3 + (threshold * iqr)
+    if lower_bound is None or upper_bound is None:
+        if lower_bound is None:
+            lower_bound: float = quartile_1 - (threshold * iqr)
+        if upper_bound is None:
+            upper_bound: float = quartile_3 + (threshold * iqr)
     if create_outlier_column:
         data_frame[f"{column}_outlier"] = data_frame[column].apply(
             lambda x: 1 if x < lower_bound or x > upper_bound else 0
         )
-    data_frame[column] = data_frame[column].apply(
-        lambda x: lower_bound
-        if x < lower_bound
-        else x
-        if x < upper_bound
-        else upper_bound
-    )
-    return data_frame
+    if transform_outliers:
+        data_frame[column] = data_frame[column].apply(
+            lambda x: lower_bound
+            if x < lower_bound
+            else x
+            if x < upper_bound
+            else upper_bound
+        )
+    return data_frame, lower_bound, upper_bound
```

### Comparing `coolpandas-0.4.4/coolpandas.egg-info/PKG-INFO` & `coolpandas-0.4.5/coolpandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.4.4/coolpandas.egg-info/SOURCES.txt` & `coolpandas-0.4.5/coolpandas.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 coolpandas/eda/summary.py
 coolpandas/eda/value_counts.py
 coolpandas/evaluate/__init__.py
 coolpandas/evaluate/confusion_matrix.py
 coolpandas/plot/__init__.py
 coolpandas/plot/barplot.py
 coolpandas/plot/boxplot.py
+coolpandas/plot/confusion_matrix.py
 coolpandas/plot/distplot.py
 coolpandas/plot/geoplot.py
 coolpandas/plot/lineplot.py
 coolpandas/plot/mapplot.py
 coolpandas/plot/scatterplot.py
 coolpandas/plot/style.py
 coolpandas/stats/__init__.py
```

### Comparing `coolpandas-0.4.4/pyproject.toml` & `coolpandas-0.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coolpandas"
-version = "0.4.4"
+version = "0.4.5"
 authors = [
   { name="Avel Docquin", email="adocquin@outlook.com" },
   ]
 description = "A Python package for Exploratory Data Analysis."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

