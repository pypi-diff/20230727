# Comparing `tmp/dcekit-2.9.0.tar.gz` & `tmp/dcekit-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcekit-2.9.0.tar", last modified: Tue Aug  9 02:56:54 2022, max compression
+gzip compressed data, was "dcekit-2.9.1.tar", last modified: Thu Aug 11 10:06:27 2022, max compression
```

## Comparing `dcekit-2.9.0.tar` & `dcekit-2.9.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2022-08-09 02:56:54.525413 dcekit-2.9.0/
--rw-rw-rw-   0        0        0     1093 2022-03-21 01:15:05.000000 dcekit-2.9.0/LICENSE
--rw-rw-rw-   0        0        0     1093 2022-03-21 01:15:05.000000 dcekit-2.9.0/LICENSE.txt
--rw-rw-rw-   0        0        0       87 2022-03-21 01:15:05.000000 dcekit-2.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1656 2022-08-09 02:56:54.524127 dcekit-2.9.0/PKG-INFO
--rw-rw-rw-   0        0        0      123 2022-03-21 01:15:05.000000 dcekit-2.9.0/README.md
-drwxrwxrwx   0        0        0        0 2022-08-09 02:56:54.140255 dcekit-2.9.0/dcekit/
--rw-rw-rw-   0        0        0       74 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-09 02:56:54.226598 dcekit-2.9.0/dcekit/design_of_exmeriments/
--rw-rw-rw-   0        0        0      134 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/design_of_exmeriments/__init__.py
--rw-rw-rw-   0        0        0     4020 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/design_of_exmeriments/bayesian_optimization.py
-drwxrwxrwx   0        0        0        0 2022-08-09 02:56:54.271267 dcekit-2.9.0/dcekit/generative_model/
--rw-rw-rw-   0        0        0      146 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/generative_model/__init__.py
--rw-rw-rw-   0        0        0    46019 2022-08-02 03:48:23.000000 dcekit-2.9.0/dcekit/generative_model/gmr.py
--rw-rw-rw-   0        0        0    63419 2022-07-17 05:00:52.000000 dcekit-2.9.0/dcekit/generative_model/gtm.py
--rw-rw-rw-   0        0        0    46832 2022-08-02 03:48:23.000000 dcekit-2.9.0/dcekit/generative_model/vbgmr.py
-drwxrwxrwx   0        0        0        0 2022-08-09 02:56:54.312853 dcekit-2.9.0/dcekit/just_in_time/
--rw-rw-rw-   0        0        0      130 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/just_in_time/__init__.py
--rw-rw-rw-   0        0        0     4702 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/just_in_time/jitpls.py
--rw-rw-rw-   0        0        0     4358 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/just_in_time/lwpls.py
-drwxrwxrwx   0        0        0        0 2022-08-09 02:56:54.370163 dcekit-2.9.0/dcekit/learning/
--rw-rw-rw-   0        0        0      376 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/learning/__init__.py
--rw-rw-rw-   0        0        0    19543 2022-06-24 22:52:42.000000 dcekit-2.9.0/dcekit/learning/ensemble_learning.py
--rw-rw-rw-   0        0        0     8351 2022-06-24 22:52:42.000000 dcekit-2.9.0/dcekit/learning/semi_supervised_learning.py
--rw-rw-rw-   0        0        0     5206 2022-06-24 22:52:42.000000 dcekit-2.9.0/dcekit/learning/transfer_learning.py
-drwxrwxrwx   0        0        0        0 2022-08-09 02:56:54.413773 dcekit-2.9.0/dcekit/optimization/
--rw-rw-rw-   0        0        0      265 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/optimization/__init__.py
--rw-rw-rw-   0        0        0     6363 2022-05-09 03:10:26.000000 dcekit-2.9.0/dcekit/optimization/fast_opt_svr_hyperparams.py
--rw-rw-rw-   0        0        0     2193 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/optimization/iot.py
-drwxrwxrwx   0        0        0        0 2022-08-09 02:56:54.445548 dcekit-2.9.0/dcekit/sampling/
--rw-rw-rw-   0        0        0      118 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/sampling/__init__.py
--rw-rw-rw-   0        0        0     2594 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/sampling/kennard_stone.py
-drwxrwxrwx   0        0        0        0 2022-08-09 02:56:54.484487 dcekit-2.9.0/dcekit/validation/
--rw-rw-rw-   0        0        0      594 2022-08-09 02:44:45.000000 dcekit-2.9.0/dcekit/validation/__init__.py
--rw-rw-rw-   0        0        0     5496 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/validation/applicability_domain.py
--rw-rw-rw-   0        0        0     2618 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/validation/metrics.py
--rw-rw-rw-   0        0        0    23177 2022-08-09 02:44:45.000000 dcekit-2.9.0/dcekit/validation/validation.py
-drwxrwxrwx   0        0        0        0 2022-08-09 02:56:54.521703 dcekit-2.9.0/dcekit/variable_selection/
--rw-rw-rw-   0        0        0      305 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/variable_selection/__init__.py
--rw-rw-rw-   0        0        0     3587 2022-03-21 01:15:05.000000 dcekit-2.9.0/dcekit/variable_selection/basic_variable_selection.py
-drwxrwxrwx   0        0        0        0 2022-08-09 02:56:54.194530 dcekit-2.9.0/dcekit.egg-info/
--rw-rw-rw-   0        0        0     1656 2022-08-09 02:56:53.000000 dcekit-2.9.0/dcekit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1074 2022-08-09 02:56:53.000000 dcekit-2.9.0/dcekit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-09 02:56:53.000000 dcekit-2.9.0/dcekit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2022-08-09 02:56:53.000000 dcekit-2.9.0/dcekit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-08-09 02:56:53.000000 dcekit-2.9.0/dcekit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-09 02:56:54.526435 dcekit-2.9.0/setup.cfg
--rw-rw-rw-   0        0        0      612 2022-08-09 02:44:45.000000 dcekit-2.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-11 10:06:27.212512 dcekit-2.9.1/
+-rw-rw-rw-   0        0        0     1093 2022-03-21 01:15:05.000000 dcekit-2.9.1/LICENSE
+-rw-rw-rw-   0        0        0     1093 2022-03-21 01:15:05.000000 dcekit-2.9.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       87 2022-03-21 01:15:05.000000 dcekit-2.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1656 2022-08-11 10:06:27.211705 dcekit-2.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2022-03-21 01:15:05.000000 dcekit-2.9.1/README.md
+drwxrwxrwx   0        0        0        0 2022-08-11 10:06:26.735282 dcekit-2.9.1/dcekit/
+-rw-rw-rw-   0        0        0       74 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-11 10:06:26.836929 dcekit-2.9.1/dcekit/design_of_exmeriments/
+-rw-rw-rw-   0        0        0      134 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/design_of_exmeriments/__init__.py
+-rw-rw-rw-   0        0        0     4020 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/design_of_exmeriments/bayesian_optimization.py
+drwxrwxrwx   0        0        0        0 2022-08-11 10:06:26.907163 dcekit-2.9.1/dcekit/generative_model/
+-rw-rw-rw-   0        0        0      146 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/generative_model/__init__.py
+-rw-rw-rw-   0        0        0    46019 2022-08-02 03:48:23.000000 dcekit-2.9.1/dcekit/generative_model/gmr.py
+-rw-rw-rw-   0        0        0    63419 2022-07-17 05:00:52.000000 dcekit-2.9.1/dcekit/generative_model/gtm.py
+-rw-rw-rw-   0        0        0    46832 2022-08-02 03:48:23.000000 dcekit-2.9.1/dcekit/generative_model/vbgmr.py
+drwxrwxrwx   0        0        0        0 2022-08-11 10:06:26.959066 dcekit-2.9.1/dcekit/just_in_time/
+-rw-rw-rw-   0        0        0      130 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/just_in_time/__init__.py
+-rw-rw-rw-   0        0        0     4702 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/just_in_time/jitpls.py
+-rw-rw-rw-   0        0        0     4358 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/just_in_time/lwpls.py
+drwxrwxrwx   0        0        0        0 2022-08-11 10:06:27.037294 dcekit-2.9.1/dcekit/learning/
+-rw-rw-rw-   0        0        0      376 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/learning/__init__.py
+-rw-rw-rw-   0        0        0    19543 2022-06-24 22:52:42.000000 dcekit-2.9.1/dcekit/learning/ensemble_learning.py
+-rw-rw-rw-   0        0        0     8351 2022-06-24 22:52:42.000000 dcekit-2.9.1/dcekit/learning/semi_supervised_learning.py
+-rw-rw-rw-   0        0        0     5206 2022-06-24 22:52:42.000000 dcekit-2.9.1/dcekit/learning/transfer_learning.py
+drwxrwxrwx   0        0        0        0 2022-08-11 10:06:27.081683 dcekit-2.9.1/dcekit/optimization/
+-rw-rw-rw-   0        0        0      265 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/optimization/__init__.py
+-rw-rw-rw-   0        0        0     6363 2022-05-09 03:10:26.000000 dcekit-2.9.1/dcekit/optimization/fast_opt_svr_hyperparams.py
+-rw-rw-rw-   0        0        0     2193 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/optimization/iot.py
+drwxrwxrwx   0        0        0        0 2022-08-11 10:06:27.122887 dcekit-2.9.1/dcekit/sampling/
+-rw-rw-rw-   0        0        0      118 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/sampling/__init__.py
+-rw-rw-rw-   0        0        0     2594 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/sampling/kennard_stone.py
+drwxrwxrwx   0        0        0        0 2022-08-11 10:06:27.189108 dcekit-2.9.1/dcekit/validation/
+-rw-rw-rw-   0        0        0      594 2022-08-09 02:44:45.000000 dcekit-2.9.1/dcekit/validation/__init__.py
+-rw-rw-rw-   0        0        0     5496 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/validation/applicability_domain.py
+-rw-rw-rw-   0        0        0     2618 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/validation/metrics.py
+-rw-rw-rw-   0        0        0    23177 2022-08-09 02:44:45.000000 dcekit-2.9.1/dcekit/validation/validation.py
+drwxrwxrwx   0        0        0        0 2022-08-11 10:06:27.209623 dcekit-2.9.1/dcekit/variable_selection/
+-rw-rw-rw-   0        0        0      305 2022-03-21 01:15:05.000000 dcekit-2.9.1/dcekit/variable_selection/__init__.py
+-rw-rw-rw-   0        0        0     3512 2022-08-11 10:04:47.000000 dcekit-2.9.1/dcekit/variable_selection/basic_variable_selection.py
+drwxrwxrwx   0        0        0        0 2022-08-11 10:06:26.805411 dcekit-2.9.1/dcekit.egg-info/
+-rw-rw-rw-   0        0        0     1656 2022-08-11 10:06:25.000000 dcekit-2.9.1/dcekit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1074 2022-08-11 10:06:26.000000 dcekit-2.9.1/dcekit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-11 10:06:25.000000 dcekit-2.9.1/dcekit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2022-08-11 10:06:26.000000 dcekit-2.9.1/dcekit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-08-11 10:06:26.000000 dcekit-2.9.1/dcekit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-08-11 10:06:27.212682 dcekit-2.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      612 2022-08-11 10:04:47.000000 dcekit-2.9.1/setup.py
```

### Comparing `dcekit-2.9.0/LICENSE` & `dcekit-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/LICENSE.txt` & `dcekit-2.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/PKG-INFO` & `dcekit-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcekit
-Version: 2.9.0
+Version: 2.9.1
 Summary: Data Chemical Engineering toolkit
 Home-page: https://github.com/hkaneko1985/dcekit/
 Author: Hiromasa Kaneko
 Author-email: hkaneko226@gmail.com
 License: MIT License
         
         Copyright (c) 2019 Hiromasa Kaneko
```

### Comparing `dcekit-2.9.0/dcekit/design_of_exmeriments/bayesian_optimization.py` & `dcekit-2.9.1/dcekit/design_of_exmeriments/bayesian_optimization.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/generative_model/gmr.py` & `dcekit-2.9.1/dcekit/generative_model/gmr.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/generative_model/gtm.py` & `dcekit-2.9.1/dcekit/generative_model/gtm.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/generative_model/vbgmr.py` & `dcekit-2.9.1/dcekit/generative_model/vbgmr.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/just_in_time/jitpls.py` & `dcekit-2.9.1/dcekit/just_in_time/jitpls.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/just_in_time/lwpls.py` & `dcekit-2.9.1/dcekit/just_in_time/lwpls.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/learning/ensemble_learning.py` & `dcekit-2.9.1/dcekit/learning/ensemble_learning.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/learning/semi_supervised_learning.py` & `dcekit-2.9.1/dcekit/learning/semi_supervised_learning.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/learning/transfer_learning.py` & `dcekit-2.9.1/dcekit/learning/transfer_learning.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/optimization/fast_opt_svr_hyperparams.py` & `dcekit-2.9.1/dcekit/optimization/fast_opt_svr_hyperparams.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/optimization/iot.py` & `dcekit-2.9.1/dcekit/optimization/iot.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/sampling/kennard_stone.py` & `dcekit-2.9.1/dcekit/sampling/kennard_stone.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/validation/__init__.py` & `dcekit-2.9.1/dcekit/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/validation/applicability_domain.py` & `dcekit-2.9.1/dcekit/validation/applicability_domain.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/validation/metrics.py` & `dcekit-2.9.1/dcekit/validation/metrics.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/validation/validation.py` & `dcekit-2.9.1/dcekit/validation/validation.py`

 * *Files identical despite different names*

### Comparing `dcekit-2.9.0/dcekit/variable_selection/basic_variable_selection.py` & `dcekit-2.9.1/dcekit/variable_selection/basic_variable_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,16 +97,14 @@
     cluster_numbers : numpy.array
         cluster number for each variable
     """
     x = pd.DataFrame(x)
     r_in_x = x.corr()
     r_in_x = abs(r_in_x)
     distance_in_x = 1 / r_in_x
-    for i in range(r_in_x.shape[0]):
-        r_in_x.iloc[i, i] = 10 ^ 10
 
     # clustering
     clustering = AgglomerativeClustering(n_clusters=None, affinity='precomputed', compute_full_tree='True',
                                          distance_threshold=1 / threshold_of_r, linkage='complete')
     clustering.fit(distance_in_x)
     cluster_numbers = clustering.labels_
```

### Comparing `dcekit-2.9.0/dcekit.egg-info/PKG-INFO` & `dcekit-2.9.1/dcekit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcekit
-Version: 2.9.0
+Version: 2.9.1
 Summary: Data Chemical Engineering toolkit
 Home-page: https://github.com/hkaneko1985/dcekit/
 Author: Hiromasa Kaneko
 Author-email: hkaneko226@gmail.com
 License: MIT License
         
         Copyright (c) 2019 Hiromasa Kaneko
```

### Comparing `dcekit-2.9.0/dcekit.egg-info/SOURCES.txt` & `dcekit-2.9.1/dcekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

