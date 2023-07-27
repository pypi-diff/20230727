# Comparing `tmp/permetrics-1.3.3.tar.gz` & `tmp/permetrics-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\permetrics-1.3.3.tar", last modified: Wed Apr  5 11:25:09 2023, max compression
+gzip compressed data, was "dist\permetrics-1.4.0.tar", last modified: Thu Jul 27 02:16:17 2023, max compression
```

## Comparing `permetrics-1.3.3.tar` & `permetrics-1.4.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 11:25:09.607675 permetrics-1.3.3/
--rw-rw-rw-   0        0        0     5823 2023-04-05 11:22:40.000000 permetrics-1.3.3/ChangeLog.md
--rw-rw-rw-   0        0        0    11346 2019-12-06 02:04:06.000000 permetrics-1.3.3/LICENSE
--rw-rw-rw-   0        0        0       77 2022-03-25 11:44:18.000000 permetrics-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0    16950 2023-04-05 11:25:09.607675 permetrics-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    13401 2023-04-05 11:22:40.000000 permetrics-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 11:25:09.542907 permetrics-1.3.3/assets/
--rw-rw-rw-   0        0        0      399 2022-05-23 03:13:19.000000 permetrics-1.3.3/assets/__init__.py
--rw-rw-rw-   0        0        0     1445 2022-04-02 11:00:24.000000 permetrics-1.3.3/assets/check_kld.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:25:09.565974 permetrics-1.3.3/assets/class/
--rw-rw-rw-   0        0        0     7472 2022-05-18 14:02:24.000000 permetrics-1.3.3/assets/class/BC_01_breast_cancer.py
--rw-rw-rw-   0        0        0      953 2022-05-18 08:35:29.000000 permetrics-1.3.3/assets/class/BC_01_coronary_heart_disease.py
--rw-rw-rw-   0        0        0      399 2022-05-23 03:13:09.000000 permetrics-1.3.3/assets/class/__init__.py
--rw-rw-rw-   0        0        0     2609 2022-05-19 15:28:37.000000 permetrics-1.3.3/assets/class/example.py
--rw-rw-rw-   0        0        0     1019 2022-05-18 01:19:52.000000 permetrics-1.3.3/assets/class/fruits_lover_edition.py
--rw-rw-rw-   0        0        0     2960 2022-04-08 11:46:49.000000 permetrics-1.3.3/assets/example.py
--rw-rw-rw-   0        0        0     1280 2022-03-03 13:18:19.000000 permetrics-1.3.3/assets/ga_exam.py
--rw-rw-rw-   0        0        0     1854 2022-03-25 11:44:18.000000 permetrics-1.3.3/assets/test.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:25:09.574487 permetrics-1.3.3/permetrics/
--rw-rw-rw-   0        0        0     1396 2023-04-05 11:22:40.000000 permetrics-1.3.3/permetrics/__init__.py
--rw-rw-rw-   0        0        0    35187 2023-04-05 11:22:40.000000 permetrics-1.3.3/permetrics/classification.py
--rw-rw-rw-   0        0        0     5095 2022-10-02 08:46:37.000000 permetrics-1.3.3/permetrics/evaluator.py
--rw-rw-rw-   0        0        0    93856 2023-04-05 11:22:40.000000 permetrics-1.3.3/permetrics/regression.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:25:09.606104 permetrics-1.3.3/permetrics/utils/
--rw-rw-rw-   0        0        0      399 2022-05-23 04:40:57.000000 permetrics-1.3.3/permetrics/utils/__init__.py
--rw-rw-rw-   0        0        0    11331 2023-04-05 11:22:40.000000 permetrics-1.3.3/permetrics/utils/classifier_util.py
--rw-rw-rw-   0        0        0     7237 2023-04-05 11:22:40.000000 permetrics-1.3.3/permetrics/utils/data_util.py
--rw-rw-rw-   0        0        0     3025 2023-01-06 05:47:02.000000 permetrics-1.3.3/permetrics/utils/regressor_util.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:25:09.595138 permetrics-1.3.3/permetrics.egg-info/
--rw-rw-rw-   0        0        0    16950 2023-04-05 11:25:09.000000 permetrics-1.3.3/permetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      708 2023-04-05 11:25:09.000000 permetrics-1.3.3/permetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 11:25:09.000000 permetrics-1.3.3/permetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-05 11:25:09.000000 permetrics-1.3.3/permetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-05 11:25:09.000000 permetrics-1.3.3/permetrics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 11:25:09.607675 permetrics-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1872 2023-04-05 11:22:40.000000 permetrics-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:16:17.638870 permetrics-1.4.0/
+-rw-rw-rw-   0        0        0     7065 2023-07-27 02:15:50.000000 permetrics-1.4.0/ChangeLog.md
+-rw-rw-rw-   0        0        0    11346 2019-12-06 02:04:06.000000 permetrics-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0       38 2023-07-27 02:15:50.000000 permetrics-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    17802 2023-07-27 02:16:17.638870 permetrics-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14077 2023-07-27 02:15:50.000000 permetrics-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 02:16:17.550759 permetrics-1.4.0/assets/
+-rw-rw-rw-   0        0        0      399 2022-05-23 03:13:19.000000 permetrics-1.4.0/assets/__init__.py
+-rw-rw-rw-   0        0        0     1445 2022-04-02 11:00:24.000000 permetrics-1.4.0/assets/check_kld.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:16:17.574753 permetrics-1.4.0/assets/class/
+-rw-rw-rw-   0        0        0     7472 2022-05-18 14:02:24.000000 permetrics-1.4.0/assets/class/BC_01_breast_cancer.py
+-rw-rw-rw-   0        0        0      953 2022-05-18 08:35:29.000000 permetrics-1.4.0/assets/class/BC_01_coronary_heart_disease.py
+-rw-rw-rw-   0        0        0      399 2022-05-23 03:13:09.000000 permetrics-1.4.0/assets/class/__init__.py
+-rw-rw-rw-   0        0        0     2609 2022-05-19 15:28:37.000000 permetrics-1.4.0/assets/class/example.py
+-rw-rw-rw-   0        0        0     1019 2022-05-18 01:19:52.000000 permetrics-1.4.0/assets/class/fruits_lover_edition.py
+-rw-rw-rw-   0        0        0     2960 2022-04-08 11:46:49.000000 permetrics-1.4.0/assets/example.py
+-rw-rw-rw-   0        0        0     1280 2022-03-03 13:18:19.000000 permetrics-1.4.0/assets/ga_exam.py
+-rw-rw-rw-   0        0        0     1854 2022-03-25 11:44:18.000000 permetrics-1.4.0/assets/test.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:16:17.602968 permetrics-1.4.0/permetrics/
+-rw-rw-rw-   0        0        0     1987 2023-07-27 02:15:50.000000 permetrics-1.4.0/permetrics/__init__.py
+-rw-rw-rw-   0        0        0    35187 2023-07-25 04:34:31.000000 permetrics-1.4.0/permetrics/classification.py
+-rw-rw-rw-   0        0        0    48718 2023-07-27 02:15:50.000000 permetrics-1.4.0/permetrics/clustering.py
+-rw-rw-rw-   0        0        0     5095 2022-10-02 08:46:37.000000 permetrics-1.4.0/permetrics/evaluator.py
+-rw-rw-rw-   0        0        0    93856 2023-07-25 04:34:31.000000 permetrics-1.4.0/permetrics/regression.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:16:17.637875 permetrics-1.4.0/permetrics/utils/
+-rw-rw-rw-   0        0        0      399 2022-05-23 04:40:57.000000 permetrics-1.4.0/permetrics/utils/__init__.py
+-rw-rw-rw-   0        0        0    10317 2023-07-27 02:15:50.000000 permetrics-1.4.0/permetrics/utils/classifier_util.py
+-rw-rw-rw-   0        0        0     6186 2023-07-27 02:15:50.000000 permetrics-1.4.0/permetrics/utils/cluster_util.py
+-rw-rw-rw-   0        0        0     9460 2023-07-27 02:15:50.000000 permetrics-1.4.0/permetrics/utils/data_util.py
+-rw-rw-rw-   0        0        0      959 2023-07-27 02:15:50.000000 permetrics-1.4.0/permetrics/utils/encoder.py
+-rw-rw-rw-   0        0        0     3025 2023-07-25 04:34:31.000000 permetrics-1.4.0/permetrics/utils/regressor_util.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:16:17.623911 permetrics-1.4.0/permetrics.egg-info/
+-rw-rw-rw-   0        0        0    17802 2023-07-27 02:16:17.000000 permetrics-1.4.0/permetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      794 2023-07-27 02:16:17.000000 permetrics-1.4.0/permetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 02:16:17.000000 permetrics-1.4.0/permetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-27 02:16:17.000000 permetrics-1.4.0/permetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-27 02:16:17.000000 permetrics-1.4.0/permetrics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 02:16:17.639867 permetrics-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2117 2023-07-27 02:15:50.000000 permetrics-1.4.0/setup.py
```

### Comparing `permetrics-1.3.3/ChangeLog.md` & `permetrics-1.4.0/ChangeLog.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,48 @@
+# Version 1.4.0
+
++ Add ClusteringMetric:
+  + Add internal metrics (Need X features and y_pred)
+    + ball_hall_index (BHI)
+    + calinski_harabasz_index (CHI)
+    + xie_beni_index (XBI)
+    + banfeld_raftery_index (BRI)
+    + davies_bouldin_index (DBI)
+    + det_ratio_index (DRI)
+    + dunn_index (DI)
+    + ksq_detw_index (KDI)
+    + log_det_ratio_index (LDRI)
+    + log_ss_ratio_index (LSRI)
+    + silhouette_index (SI)
+  + Add external metrics (Need y_true and y_pred)
+    + mutual_info_score (MIS)
+    + normalized_mutual_info_score (NMIS)
+    + rand_score (RaS)
+    + fowlkes_mallows_score (FMS)
+    + homogeneity_score (HS)
+    + completeness_score (CS)
+    + v_measure_score (VMS)
+    + precision_score (PrS)
+    + recall_score (ReS)
+    + f_measure_score (FmS)
+    + czekanowski_dice_score (CDS)
+    + hubert_gamma_score (HGS)
+    + jaccard_score (JS)
+    + kulczynski_score (KS)
+    + mc_nemar_score (MNS)
+    + phi_score (PhS)
+    + rogers_tanimoto_score (RTS)
+    + russel_rao_score (RRS)
+    + sokal_sneath1_score (SS1S)
+    + sokal_sneath2_score (SS2S)
++ Add examples for ClusteringMetric
++ Add LabelEncoder class 
+
+---------------------------------------------------------------------
+
 # Version 1.3.3
 
 ### Update
 
 Update ClassificationMetric:
 + Rename confusion_matrix() in util file
 + Support binary and multi-class classification with one-hot-encoder format
```

### Comparing `permetrics-1.3.3/LICENSE` & `permetrics-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/PKG-INFO` & `permetrics-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: permetrics
-Version: 1.3.3
+Version: 1.4.0
 Summary: PerMetrics: A framework of PERformance METRICS for machine learning models
 Home-page: https://github.com/thieu1995/permetrics
 Author: Nguyen Van Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: MIT
 Download-URL: https://github.com/thieu1995/permetrics/archive/v1.3.3.zip
 Description: 
         <p align="center"><img src=".github/img/logo2.png" alt="PERMETRICS" title="PERMETRICS"/></p>
         
         
         
-        [![GitHub release](https://img.shields.io/badge/release-1.3.3-yellow.svg)](https://github.com/thieu1995/permetrics/releases)
+        [![GitHub release](https://img.shields.io/badge/release-1.4.0-yellow.svg)](https://github.com/thieu1995/permetrics/releases)
         [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/permetrics) 
         [![PyPI version](https://badge.fury.io/py/permetrics.svg)](https://badge.fury.io/py/permetrics)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/permetrics.svg)
         ![PyPI - Status](https://img.shields.io/pypi/status/permetrics.svg)
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/permetrics.svg)
         [![Downloads](https://pepy.tech/badge/permetrics)](https://pepy.tech/project/permetrics)
         ![GitHub Release Date](https://img.shields.io/github/release-date/thieu1995/permetrics.svg)
@@ -25,15 +25,15 @@
         [![DOI](https://zenodo.org/badge/280617738.svg)](https://zenodo.org/badge/latestdoi/280617738)
         [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
         
         
         PerMetrics is a python library for performance metrics of machine learning models. We aim to implement all performance metrics for problems such as regression, classification, clustering, ... problems. Helping users in all field access metrics as fast as possible
         
         * **Free software:** Apache License, Version 2.0
-        * **Total metrics**: 63 (47 regression metrics, 16 classification metrics)
+        * **Total metrics**: 94 (47 regression metrics, 16 classification metrics, 31 clustering metrics)
         * **Documentation:** https://permetrics.readthedocs.io/en/latest/
         * **Python versions:** 3.6.x, 3.7.x, 3.8.x, 3.9.x, 3.10.x
         * **Dependencies:** numpy
         
         
         # Notification
         
@@ -47,15 +47,15 @@
         
         
         # Installation
         
         ### Install with pip
         Install the [current PyPI release](https://pypi.python.org/pypi/permetrics):
         ```sh 
-        $ pip install permetrics==1.3.3
+        $ pip install permetrics==1.4.0
         ```
         
         Or install the development version from GitHub:
         
         ```bash
         pip install git+https://github.com/thieu1995/permetrics
         ```
@@ -85,40 +85,39 @@
         The [documentation](https://permetrics.readthedocs.io/) includes more detailed installation instructions and explanations.
         
         
         ### Example with Regression metrics
         
         
         ```python
-        from numpy import array
-        from permetrics.regression import RegressionMetric
+        import numpy as np
+        from permetrics import RegressionMetric
         
         ## For 1-D array
-        y_true = array([3, -0.5, 2, 7])
-        y_pred = array([2.5, 0.0, 2, 8])
+        y_true = [3, -0.5, 2, 7]
+        y_pred = [2.5, 0.0, 2, 8]
         
         evaluator = RegressionMetric(y_true, y_pred, decimal=5)
         print(evaluator.RMSE())
         print(evaluator.MSE())
         
         ## For > 1-D array
-        y_true = array([[0.5, 1], [-1, 1], [7, -6]])
-        y_pred = array([[0, 2], [-1, 2], [8, -5]])
+        y_true = np.array([[0.5, 1], [-1, 1], [7, -6]])
+        y_pred = np.array([[0, 2], [-1, 2], [8, -5]])
         
         evaluator = RegressionMetric(y_true, y_pred, decimal=5)
         print(evaluator.RMSE(multi_output="raw_values", decimal=5))
         print(evaluator.MAE(multi_output="raw_values", decimal=5))
         ```
         
         
         ### Example with Classification metrics
         
         ```python
-        from numpy import array
-        from permetrics.classification import ClassificationMetric
+        from permetrics import ClassificationMetric
         
         ## For integer labels or categorical labels
         y_true = [0, 1, 0, 0, 1, 0]
         y_pred = [0, 1, 0, 0, 0, 1]
         
         # y_true = ["cat", "ant", "cat", "cat", "ant", "bird", "bird", "bird"]
         # y_pred = ["ant", "ant", "cat", "cat", "ant", "cat", "bird", "ant"]
@@ -130,14 +129,37 @@
         print(evaluator.f1_score())
         print(evaluator.F1S(average="micro"))
         print(evaluator.f1s(average="macro"))
         print(evaluator.f1s(average="weighted"))
         
         ```
         
+        ### Example with Clustering metrics
+        
+        ```python
+        import numpy as np
+        from permetrics import ClusteringMetric
+        
+        # generate sample data
+        X = np.random.uniform(-1, 10, size=(500, 7))        # 500 examples, 7 features
+        y_true = np.random.randint(0, 4, size=500)          # 4 clusters
+        y_pred = np.random.randint(0, 4, size=500)
+        
+        evaluator = ClusteringMetric(y_true=y_true, y_pred=y_pred, X=X, decimal=5)
+        
+        ## Call specific function inside object, each function has 2 names (fullname and short name)
+        ##    + Internal metrics: Need X and y_pred and has suffix as index
+        ##    + External metrics: Need y_true and y_pred and has suffix as score
+        
+        print(evaluator.ball_hall_index())
+        print(evaluator.BHI())
+        ```
+        
+        
+        
         ### Get helps (questions, problems)
         
         * Official source code repo: https://github.com/thieu1995/permetrics
         * Official document: https://permetrics.readthedocs.io/
         * Download releases: https://pypi.org/project/permetrics/
         * Issue tracker: https://github.com/thieu1995/permetrics/issues
         * Notable changes log: https://github.com/thieu1995/permetrics/blob/master/ChangeLog.md
```

### Comparing `permetrics-1.3.3/README.md` & `permetrics-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 <p align="center"><img src=".github/img/logo2.png" alt="PERMETRICS" title="PERMETRICS"/></p>
 
 
 
-[![GitHub release](https://img.shields.io/badge/release-1.3.3-yellow.svg)](https://github.com/thieu1995/permetrics/releases)
+[![GitHub release](https://img.shields.io/badge/release-1.4.0-yellow.svg)](https://github.com/thieu1995/permetrics/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/permetrics) 
 [![PyPI version](https://badge.fury.io/py/permetrics.svg)](https://badge.fury.io/py/permetrics)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/permetrics.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/permetrics.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/permetrics.svg)
 [![Downloads](https://pepy.tech/badge/permetrics)](https://pepy.tech/project/permetrics)
 ![GitHub Release Date](https://img.shields.io/github/release-date/thieu1995/permetrics.svg)
@@ -16,15 +16,15 @@
 [![DOI](https://zenodo.org/badge/280617738.svg)](https://zenodo.org/badge/latestdoi/280617738)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 
 PerMetrics is a python library for performance metrics of machine learning models. We aim to implement all performance metrics for problems such as regression, classification, clustering, ... problems. Helping users in all field access metrics as fast as possible
 
 * **Free software:** Apache License, Version 2.0
-* **Total metrics**: 63 (47 regression metrics, 16 classification metrics)
+* **Total metrics**: 94 (47 regression metrics, 16 classification metrics, 31 clustering metrics)
 * **Documentation:** https://permetrics.readthedocs.io/en/latest/
 * **Python versions:** 3.6.x, 3.7.x, 3.8.x, 3.9.x, 3.10.x
 * **Dependencies:** numpy
 
 
 # Notification
 
@@ -38,15 +38,15 @@
 
 
 # Installation
 
 ### Install with pip
 Install the [current PyPI release](https://pypi.python.org/pypi/permetrics):
 ```sh 
-$ pip install permetrics==1.3.3
+$ pip install permetrics==1.4.0
 ```
 
 Or install the development version from GitHub:
 
 ```bash
 pip install git+https://github.com/thieu1995/permetrics
 ```
@@ -76,40 +76,39 @@
 The [documentation](https://permetrics.readthedocs.io/) includes more detailed installation instructions and explanations.
 
 
 ### Example with Regression metrics
 
 
 ```python
-from numpy import array
-from permetrics.regression import RegressionMetric
+import numpy as np
+from permetrics import RegressionMetric
 
 ## For 1-D array
-y_true = array([3, -0.5, 2, 7])
-y_pred = array([2.5, 0.0, 2, 8])
+y_true = [3, -0.5, 2, 7]
+y_pred = [2.5, 0.0, 2, 8]
 
 evaluator = RegressionMetric(y_true, y_pred, decimal=5)
 print(evaluator.RMSE())
 print(evaluator.MSE())
 
 ## For > 1-D array
-y_true = array([[0.5, 1], [-1, 1], [7, -6]])
-y_pred = array([[0, 2], [-1, 2], [8, -5]])
+y_true = np.array([[0.5, 1], [-1, 1], [7, -6]])
+y_pred = np.array([[0, 2], [-1, 2], [8, -5]])
 
 evaluator = RegressionMetric(y_true, y_pred, decimal=5)
 print(evaluator.RMSE(multi_output="raw_values", decimal=5))
 print(evaluator.MAE(multi_output="raw_values", decimal=5))
 ```
 
 
 ### Example with Classification metrics
 
 ```python
-from numpy import array
-from permetrics.classification import ClassificationMetric
+from permetrics import ClassificationMetric
 
 ## For integer labels or categorical labels
 y_true = [0, 1, 0, 0, 1, 0]
 y_pred = [0, 1, 0, 0, 0, 1]
 
 # y_true = ["cat", "ant", "cat", "cat", "ant", "bird", "bird", "bird"]
 # y_pred = ["ant", "ant", "cat", "cat", "ant", "cat", "bird", "ant"]
@@ -121,14 +120,37 @@
 print(evaluator.f1_score())
 print(evaluator.F1S(average="micro"))
 print(evaluator.f1s(average="macro"))
 print(evaluator.f1s(average="weighted"))
 
 ```
 
+### Example with Clustering metrics
+
+```python
+import numpy as np
+from permetrics import ClusteringMetric
+
+# generate sample data
+X = np.random.uniform(-1, 10, size=(500, 7))        # 500 examples, 7 features
+y_true = np.random.randint(0, 4, size=500)          # 4 clusters
+y_pred = np.random.randint(0, 4, size=500)
+
+evaluator = ClusteringMetric(y_true=y_true, y_pred=y_pred, X=X, decimal=5)
+
+## Call specific function inside object, each function has 2 names (fullname and short name)
+##    + Internal metrics: Need X and y_pred and has suffix as index
+##    + External metrics: Need y_true and y_pred and has suffix as score
+
+print(evaluator.ball_hall_index())
+print(evaluator.BHI())
+```
+
+
+
 ### Get helps (questions, problems)
 
 * Official source code repo: https://github.com/thieu1995/permetrics
 * Official document: https://permetrics.readthedocs.io/
 * Download releases: https://pypi.org/project/permetrics/
 * Issue tracker: https://github.com/thieu1995/permetrics/issues
 * Notable changes log: https://github.com/thieu1995/permetrics/blob/master/ChangeLog.md
```

### Comparing `permetrics-1.3.3/assets/check_kld.py` & `permetrics-1.4.0/assets/check_kld.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/assets/class/BC_01_breast_cancer.py` & `permetrics-1.4.0/assets/class/BC_01_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/assets/class/BC_01_coronary_heart_disease.py` & `permetrics-1.4.0/assets/class/BC_01_coronary_heart_disease.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/assets/class/example.py` & `permetrics-1.4.0/assets/class/example.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/assets/class/fruits_lover_edition.py` & `permetrics-1.4.0/assets/class/fruits_lover_edition.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/assets/example.py` & `permetrics-1.4.0/assets/example.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/assets/ga_exam.py` & `permetrics-1.4.0/assets/ga_exam.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/assets/test.py` & `permetrics-1.4.0/assets/test.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/permetrics/classification.py` & `permetrics-1.4.0/permetrics/classification.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/permetrics/evaluator.py` & `permetrics-1.4.0/permetrics/evaluator.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/permetrics/regression.py` & `permetrics-1.4.0/permetrics/regression.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/permetrics/utils/classifier_util.py` & `permetrics-1.4.0/permetrics/utils/classifier_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -210,45 +210,7 @@
 
     # Compute the Gini index
     sum_true = cumsum_true.sum()
     sum_pred = cumsum_pred.sum()
     n = len(y_true)
     gini = 1 - (2 * (cumsum_true.dot(y_pred_sorted)) / (sum_true * sum_pred + n * y_pred_sorted.sum()))
     return gini
-
-
-class LabelEncoder:
-    def __init__(self):
-        self.classes_ = None
-        self.encoded_classes_ = None
-
-    def fit(self, y):
-        self.classes_, indices = np.unique(y, return_inverse=True)
-        self.encoded_classes_ = np.arange(len(self.classes_))
-        return self
-
-    def transform(self, y):
-        return np.searchsorted(self.classes_, y)
-
-    def inverse_transform(self, y):
-        return self.classes_[y]
-
-    def fit_transform(self, y):
-        self.fit(y)
-        return self.transform(y)
-
-
-# class LabelEncoder:
-#     def __init__(self):
-#         self.classes_ = None
-#         self.encoded_classes_ = None
-#
-#     def fit(self, y):
-#         self.classes_ = list(set(y))
-#         self.encoded_classes_ = {c: i for i, c in enumerate(self.classes_)}
-#         return self
-#
-#     def transform(self, y):
-#         return [self.encoded_classes_[c] for c in y]
-#
-#     def inverse_transform(self, y):
-#         return [self.classes_[i] for i in y]
```

### Comparing `permetrics-1.3.3/permetrics/utils/data_util.py` & `permetrics-1.4.0/permetrics/utils/data_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Created by "Thieu" at 12:12, 19/05/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 import copy as cp
+from permetrics.utils.encoder import LabelEncoder
 
 
 def format_regression_data_type(y_true, y_pred):
     if isinstance(y_true, (list, tuple, np.ndarray)) and isinstance(y_pred, (list, tuple, np.ndarray)):
         ## Remove all dimensions of size 1
         y_true, y_pred = np.squeeze(np.asarray(y_true, dtype='float64')), np.squeeze(np.asarray(y_pred, dtype='float64'))
         if y_true.ndim == y_pred.ndim:
@@ -149,7 +150,55 @@
             if len(np.unique(y_true)) <= 2:
                 raise TypeError("y_score must have shape (n_examples, n_labels) in case of multi-classification problem")
             else:
                 if np.issubdtype(y_true.dtype, np.number):
                     return y_true, y_score, not binary, "number"
                 else:
                     return y_true, y_score, not binary, "string"
+
+
+def is_consecutive_and_start_zero(vector):
+    if sorted(vector) == list(range(min(vector), max(vector) + 1)):
+        if 0 in vector:
+            return True
+    return False
+
+
+def format_external_clustering_data(y_true: np.ndarray, y_pred: np.ndarray):
+    """
+    Need both of y_true and y_pred to format
+    """
+    if not (isinstance(y_true, (list, tuple, np.ndarray)) and isinstance(y_pred, (list, tuple, np.ndarray))):
+        raise TypeError("To calculate external clustering metrics, y_true and y_pred must be lists, tuples or numpy arrays.")
+    else:
+        ## Remove all dimensions of size 1
+        y_true, y_pred = np.squeeze(np.asarray(y_true)), np.squeeze(np.asarray(y_pred))
+        if not (y_true.ndim == y_pred.ndim):
+            raise TypeError("To calculate external clustering metrics, y_true and y_pred must have the same number of dimensions.")
+        else:
+            if y_true.ndim == 1:
+                if np.issubdtype(y_true.dtype, np.number):
+                    if is_consecutive_and_start_zero(y_true):
+                        return y_true, y_pred, None
+                le = LabelEncoder()
+                y_true = le.fit_transform(y_true)
+                y_pred = le.transform(y_pred)
+                return y_true, y_pred, le
+            else:
+                raise TypeError("To calculate clustering metrics, y_true and y_pred must be a 1-D vector.")
+
+
+def format_internal_clustering_data(labels: np.ndarray):
+    if not (isinstance(labels, (list, tuple, np.ndarray))):
+        raise TypeError("To calculate internal clustering metrics, labels must be lists, tuples or numpy arrays.")
+    else:
+        ## Remove all dimensions of size 1
+        labels = np.squeeze(np.asarray(labels))
+        if labels.ndim == 1:
+            if np.issubdtype(labels.dtype, np.number):
+                if is_consecutive_and_start_zero(labels):
+                    return labels, None
+            le = LabelEncoder()
+            labels = le.fit_transform(labels)
+            return labels, le
+        else:
+            raise TypeError("To calculate clustering metrics, labels must be a 1-D vector.")
```

### Comparing `permetrics-1.3.3/permetrics/utils/regressor_util.py` & `permetrics-1.4.0/permetrics/utils/regressor_util.py`

 * *Files identical despite different names*

### Comparing `permetrics-1.3.3/permetrics.egg-info/PKG-INFO` & `permetrics-1.4.0/permetrics.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: permetrics
-Version: 1.3.3
+Version: 1.4.0
 Summary: PerMetrics: A framework of PERformance METRICS for machine learning models
 Home-page: https://github.com/thieu1995/permetrics
 Author: Nguyen Van Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: MIT
 Download-URL: https://github.com/thieu1995/permetrics/archive/v1.3.3.zip
 Description: 
         <p align="center"><img src=".github/img/logo2.png" alt="PERMETRICS" title="PERMETRICS"/></p>
         
         
         
-        [![GitHub release](https://img.shields.io/badge/release-1.3.3-yellow.svg)](https://github.com/thieu1995/permetrics/releases)
+        [![GitHub release](https://img.shields.io/badge/release-1.4.0-yellow.svg)](https://github.com/thieu1995/permetrics/releases)
         [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/permetrics) 
         [![PyPI version](https://badge.fury.io/py/permetrics.svg)](https://badge.fury.io/py/permetrics)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/permetrics.svg)
         ![PyPI - Status](https://img.shields.io/pypi/status/permetrics.svg)
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/permetrics.svg)
         [![Downloads](https://pepy.tech/badge/permetrics)](https://pepy.tech/project/permetrics)
         ![GitHub Release Date](https://img.shields.io/github/release-date/thieu1995/permetrics.svg)
@@ -25,15 +25,15 @@
         [![DOI](https://zenodo.org/badge/280617738.svg)](https://zenodo.org/badge/latestdoi/280617738)
         [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
         
         
         PerMetrics is a python library for performance metrics of machine learning models. We aim to implement all performance metrics for problems such as regression, classification, clustering, ... problems. Helping users in all field access metrics as fast as possible
         
         * **Free software:** Apache License, Version 2.0
-        * **Total metrics**: 63 (47 regression metrics, 16 classification metrics)
+        * **Total metrics**: 94 (47 regression metrics, 16 classification metrics, 31 clustering metrics)
         * **Documentation:** https://permetrics.readthedocs.io/en/latest/
         * **Python versions:** 3.6.x, 3.7.x, 3.8.x, 3.9.x, 3.10.x
         * **Dependencies:** numpy
         
         
         # Notification
         
@@ -47,15 +47,15 @@
         
         
         # Installation
         
         ### Install with pip
         Install the [current PyPI release](https://pypi.python.org/pypi/permetrics):
         ```sh 
-        $ pip install permetrics==1.3.3
+        $ pip install permetrics==1.4.0
         ```
         
         Or install the development version from GitHub:
         
         ```bash
         pip install git+https://github.com/thieu1995/permetrics
         ```
@@ -85,40 +85,39 @@
         The [documentation](https://permetrics.readthedocs.io/) includes more detailed installation instructions and explanations.
         
         
         ### Example with Regression metrics
         
         
         ```python
-        from numpy import array
-        from permetrics.regression import RegressionMetric
+        import numpy as np
+        from permetrics import RegressionMetric
         
         ## For 1-D array
-        y_true = array([3, -0.5, 2, 7])
-        y_pred = array([2.5, 0.0, 2, 8])
+        y_true = [3, -0.5, 2, 7]
+        y_pred = [2.5, 0.0, 2, 8]
         
         evaluator = RegressionMetric(y_true, y_pred, decimal=5)
         print(evaluator.RMSE())
         print(evaluator.MSE())
         
         ## For > 1-D array
-        y_true = array([[0.5, 1], [-1, 1], [7, -6]])
-        y_pred = array([[0, 2], [-1, 2], [8, -5]])
+        y_true = np.array([[0.5, 1], [-1, 1], [7, -6]])
+        y_pred = np.array([[0, 2], [-1, 2], [8, -5]])
         
         evaluator = RegressionMetric(y_true, y_pred, decimal=5)
         print(evaluator.RMSE(multi_output="raw_values", decimal=5))
         print(evaluator.MAE(multi_output="raw_values", decimal=5))
         ```
         
         
         ### Example with Classification metrics
         
         ```python
-        from numpy import array
-        from permetrics.classification import ClassificationMetric
+        from permetrics import ClassificationMetric
         
         ## For integer labels or categorical labels
         y_true = [0, 1, 0, 0, 1, 0]
         y_pred = [0, 1, 0, 0, 0, 1]
         
         # y_true = ["cat", "ant", "cat", "cat", "ant", "bird", "bird", "bird"]
         # y_pred = ["ant", "ant", "cat", "cat", "ant", "cat", "bird", "ant"]
@@ -130,14 +129,37 @@
         print(evaluator.f1_score())
         print(evaluator.F1S(average="micro"))
         print(evaluator.f1s(average="macro"))
         print(evaluator.f1s(average="weighted"))
         
         ```
         
+        ### Example with Clustering metrics
+        
+        ```python
+        import numpy as np
+        from permetrics import ClusteringMetric
+        
+        # generate sample data
+        X = np.random.uniform(-1, 10, size=(500, 7))        # 500 examples, 7 features
+        y_true = np.random.randint(0, 4, size=500)          # 4 clusters
+        y_pred = np.random.randint(0, 4, size=500)
+        
+        evaluator = ClusteringMetric(y_true=y_true, y_pred=y_pred, X=X, decimal=5)
+        
+        ## Call specific function inside object, each function has 2 names (fullname and short name)
+        ##    + Internal metrics: Need X and y_pred and has suffix as index
+        ##    + External metrics: Need y_true and y_pred and has suffix as score
+        
+        print(evaluator.ball_hall_index())
+        print(evaluator.BHI())
+        ```
+        
+        
+        
         ### Get helps (questions, problems)
         
         * Official source code repo: https://github.com/thieu1995/permetrics
         * Official document: https://permetrics.readthedocs.io/
         * Download releases: https://pypi.org/project/permetrics/
         * Issue tracker: https://github.com/thieu1995/permetrics/issues
         * Notable changes log: https://github.com/thieu1995/permetrics/blob/master/ChangeLog.md
```

### Comparing `permetrics-1.3.3/permetrics.egg-info/SOURCES.txt` & `permetrics-1.4.0/permetrics.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -11,18 +11,21 @@
 assets/class/BC_01_breast_cancer.py
 assets/class/BC_01_coronary_heart_disease.py
 assets/class/__init__.py
 assets/class/example.py
 assets/class/fruits_lover_edition.py
 permetrics/__init__.py
 permetrics/classification.py
+permetrics/clustering.py
 permetrics/evaluator.py
 permetrics/regression.py
 permetrics.egg-info/PKG-INFO
 permetrics.egg-info/SOURCES.txt
 permetrics.egg-info/dependency_links.txt
 permetrics.egg-info/requires.txt
 permetrics.egg-info/top_level.txt
 permetrics/utils/__init__.py
 permetrics/utils/classifier_util.py
+permetrics/utils/cluster_util.py
 permetrics/utils/data_util.py
+permetrics/utils/encoder.py
 permetrics/utils/regressor_util.py
```

### Comparing `permetrics-1.3.3/setup.py` & `permetrics-1.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+#!/usr/bin/env python
+# Created by "Thieu" at 13:24, 27/02/2022 ----------%
+#       Email: nguyenthieu2102@gmail.com            %
+#       Github: https://github.com/thieu1995        %
+# --------------------------------------------------%
+
 from setuptools import setup, find_packages
 
 
 def readme():
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="permetrics",
-    version="1.3.3",
+    version="1.4.0",
     author="Nguyen Van Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="PerMetrics: A framework of PERformance METRICS for machine learning models",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/thieu1995/permetrics",
     download_url="https://github.com/thieu1995/permetrics/archive/v1.3.3.zip",
```

