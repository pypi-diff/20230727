# Comparing `tmp/scmomat-0.2.0.tar.gz` & `tmp/scmomat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmomat-0.2.0.tar", last modified: Wed Jan 11 03:21:18 2023, max compression
+gzip compressed data, was "scmomat-0.2.1.tar", last modified: Thu Jul 27 18:47:06 2023, max compression
```

## Comparing `scmomat-0.2.0.tar` & `scmomat-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-sr-x   0 zzhang834 (1059113) gtperson  (2626)        0 2023-01-11 03:21:18.342761 scmomat-0.2.0/
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)     1066 2023-01-11 03:18:23.000000 scmomat-0.2.0/LICENSE
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)       25 2023-01-11 03:18:23.000000 scmomat-0.2.0/MANIFEST.in
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)     7829 2023-01-11 03:21:18.342761 scmomat-0.2.0/PKG-INFO
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)     7008 2023-01-11 03:18:23.000000 scmomat-0.2.0/README.md
-drwxr-sr-x   0 zzhang834 (1059113) gtperson  (2626)        0 2023-01-11 03:21:18.342761 scmomat-0.2.0/scmomat/
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)      188 2023-01-11 03:18:24.000000 scmomat-0.2.0/scmomat/__init__.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)       62 2023-01-11 03:18:24.000000 scmomat-0.2.0/scmomat/__version__.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    21371 2023-01-11 03:18:24.000000 scmomat-0.2.0/scmomat/bmk.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    33204 2023-01-11 03:18:24.000000 scmomat-0.2.0/scmomat/model.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)   120615 2023-01-11 03:18:24.000000 scmomat-0.2.0/scmomat/umap_batch.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    33572 2023-01-11 03:18:24.000000 scmomat-0.2.0/scmomat/utils.py
-drwxr-sr-x   0 zzhang834 (1059113) gtperson  (2626)        0 2023-01-11 03:21:18.342761 scmomat-0.2.0/scmomat.egg-info/
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)     7829 2023-01-11 03:21:17.000000 scmomat-0.2.0/scmomat.egg-info/PKG-INFO
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)      639 2023-01-11 03:21:18.000000 scmomat-0.2.0/scmomat.egg-info/SOURCES.txt
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)        1 2023-01-11 03:21:17.000000 scmomat-0.2.0/scmomat.egg-info/dependency_links.txt
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)      129 2023-01-11 03:21:18.000000 scmomat-0.2.0/scmomat.egg-info/requires.txt
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)        8 2023-01-11 03:21:18.000000 scmomat-0.2.0/scmomat.egg-info/top_level.txt
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)       38 2023-01-11 03:21:18.342761 scmomat-0.2.0/setup.cfg
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)     4117 2023-01-11 03:18:24.000000 scmomat-0.2.0/setup.py
-drwxr-sr-x   0 zzhang834 (1059113) gtperson  (2626)        0 2023-01-11 03:21:18.342761 scmomat-0.2.0/test/
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    50946 2023-01-11 03:18:24.000000 scmomat-0.2.0/test/test_bmmc_healthy.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    14250 2023-01-11 03:18:24.000000 scmomat-0.2.0/test/test_hyperparams.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    20900 2023-01-11 03:18:24.000000 scmomat-0.2.0/test/test_marker_detection.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    48633 2023-01-11 03:18:24.000000 scmomat-0.2.0/test/test_mop_5batches.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    27229 2023-01-11 03:18:24.000000 scmomat-0.2.0/test/test_pancreas.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    73157 2023-01-11 03:18:24.000000 scmomat-0.2.0/test/test_pbmc.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    36300 2023-01-11 03:18:24.000000 scmomat-0.2.0/test/test_simulated_2modalities.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    36689 2023-01-11 03:18:24.000000 scmomat-0.2.0/test/test_simulated_3modalities.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    34257 2023-01-11 03:18:24.000000 scmomat-0.2.0/test/test_simulated_imbalanced.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    17211 2023-01-11 03:18:24.000000 scmomat-0.2.0/test/test_simulated_nopseudo.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    37474 2023-01-11 03:18:24.000000 scmomat-0.2.0/test/test_spleen.py
--rw-r--r--   0 zzhang834 (1059113) gtperson  (2626)    46027 2023-01-11 03:18:24.000000 scmomat-0.2.0/test/test_spleen_subsample.py
+drwxr-sr-x   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        0 2023-07-27 18:47:06.393109 scmomat-0.2.1/
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     1066 2023-02-21 22:18:42.000000 scmomat-0.2.1/LICENSE
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)       25 2023-02-21 22:18:42.000000 scmomat-0.2.1/MANIFEST.in
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     7829 2023-07-27 18:47:06.392109 scmomat-0.2.1/PKG-INFO
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     7008 2023-02-21 22:18:42.000000 scmomat-0.2.1/README.md
+drwxr-sr-x   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        0 2023-07-27 18:47:06.344108 scmomat-0.2.1/scmomat/
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)      188 2023-02-21 22:21:48.000000 scmomat-0.2.1/scmomat/__init__.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)       62 2023-02-21 22:21:48.000000 scmomat-0.2.1/scmomat/__version__.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    21371 2023-02-21 22:21:48.000000 scmomat-0.2.1/scmomat/bmk.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    33204 2023-02-21 22:21:48.000000 scmomat-0.2.1/scmomat/model.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)   120615 2023-02-21 22:21:48.000000 scmomat-0.2.1/scmomat/umap_batch.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    33574 2023-07-27 18:11:22.000000 scmomat-0.2.1/scmomat/utils.py
+drwxr-sr-x   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        0 2023-07-27 18:47:06.357109 scmomat-0.2.1/scmomat.egg-info/
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     7829 2023-07-27 18:47:06.000000 scmomat-0.2.1/scmomat.egg-info/PKG-INFO
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)      639 2023-07-27 18:47:06.000000 scmomat-0.2.1/scmomat.egg-info/SOURCES.txt
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        1 2023-07-27 18:47:06.000000 scmomat-0.2.1/scmomat.egg-info/dependency_links.txt
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)      129 2023-07-27 18:47:06.000000 scmomat-0.2.1/scmomat.egg-info/requires.txt
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        8 2023-07-27 18:47:06.000000 scmomat-0.2.1/scmomat.egg-info/top_level.txt
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)       38 2023-07-27 18:47:06.394109 scmomat-0.2.1/setup.cfg
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)     4117 2023-07-27 18:45:30.000000 scmomat-0.2.1/setup.py
+drwxr-sr-x   0 zzhang834 (1059113) coc-xzhanglab-access (372345)        0 2023-07-27 18:47:06.389109 scmomat-0.2.1/test/
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    50946 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_bmmc_healthy.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    14250 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_hyperparams.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    20900 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_marker_detection.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    48633 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_mop_5batches.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    27229 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_pancreas.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    73157 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_pbmc.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    36300 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_simulated_2modalities.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    36689 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_simulated_3modalities.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    34257 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_simulated_imbalanced.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    17211 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_simulated_nopseudo.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    37474 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_spleen.py
+-rw-r--r--   0 zzhang834 (1059113) coc-xzhanglab-access (372345)    46027 2023-02-21 22:18:42.000000 scmomat-0.2.1/test/test_spleen_subsample.py
```

### Comparing `scmomat-0.2.0/LICENSE` & `scmomat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/PKG-INFO` & `scmomat-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmomat
-Version: 0.2.0
+Version: 0.2.1
 Summary: scmomat: a single-cell multi-omics mosaic integration method
 Home-page: https://github.com/PeterZZQ/scMoMaT
 Author: Ziqi Zhang
 Author-email: zhangziqibuaa@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `scmomat-0.2.0/README.md` & `scmomat-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/scmomat/bmk.py` & `scmomat-0.2.1/scmomat/bmk.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/scmomat/model.py` & `scmomat-0.2.1/scmomat/model.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/scmomat/umap_batch.py` & `scmomat-0.2.1/scmomat/umap_batch.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/scmomat/utils.py` & `scmomat-0.2.1/scmomat/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     -------------
         counts: count matrix
         modality: modality that the matrix belong to, can be ``ATAC'', ``RNA'', ``protein''
         log: log transform the data or not
     """
     if modality == "ATAC":
         # make binary, maximum is 1
-        counts = (counts > 0).astype(np.float) 
+        counts = (counts > 0).astype(np.float64) 
         # # normalize according to library size
         # counts = counts / np.sum(counts, axis = 1)[:,None]
         # counts = counts/np.max(counts)
 
     # elif modality == "interaction":
     #     # gene by region matrix
     #     counts = counts/(np.sum(counts, axis = 1)[:,None] + 1e-6)
```

### Comparing `scmomat-0.2.0/scmomat.egg-info/PKG-INFO` & `scmomat-0.2.1/scmomat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmomat
-Version: 0.2.0
+Version: 0.2.1
 Summary: scmomat: a single-cell multi-omics mosaic integration method
 Home-page: https://github.com/PeterZZQ/scMoMaT
 Author: Ziqi Zhang
 Author-email: zhangziqibuaa@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `scmomat-0.2.0/scmomat.egg-info/SOURCES.txt` & `scmomat-0.2.1/scmomat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/setup.py` & `scmomat-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'scmomat'
 DESCRIPTION = 'scmomat: a single-cell multi-omics mosaic integration method'
 URL = 'https://github.com/PeterZZQ/scMoMaT'
 EMAIL = 'zhangziqibuaa@gmail.com'
 AUTHOR = 'Ziqi Zhang'
 REQUIRES_PYTHON = '>=3.8.10'
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'torch>=1.11.0',
     'numpy>=1.19.5',
     'pandas>=1.4.0',
     'scipy>=1.7.3',
```

### Comparing `scmomat-0.2.0/test/test_bmmc_healthy.py` & `scmomat-0.2.1/test/test_bmmc_healthy.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/test/test_hyperparams.py` & `scmomat-0.2.1/test/test_hyperparams.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/test/test_marker_detection.py` & `scmomat-0.2.1/test/test_marker_detection.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/test/test_mop_5batches.py` & `scmomat-0.2.1/test/test_mop_5batches.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/test/test_pancreas.py` & `scmomat-0.2.1/test/test_pancreas.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/test/test_pbmc.py` & `scmomat-0.2.1/test/test_pbmc.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/test/test_simulated_2modalities.py` & `scmomat-0.2.1/test/test_simulated_2modalities.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/test/test_simulated_3modalities.py` & `scmomat-0.2.1/test/test_simulated_3modalities.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/test/test_simulated_imbalanced.py` & `scmomat-0.2.1/test/test_simulated_imbalanced.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/test/test_simulated_nopseudo.py` & `scmomat-0.2.1/test/test_simulated_nopseudo.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/test/test_spleen.py` & `scmomat-0.2.1/test/test_spleen.py`

 * *Files identical despite different names*

### Comparing `scmomat-0.2.0/test/test_spleen_subsample.py` & `scmomat-0.2.1/test/test_spleen_subsample.py`

 * *Files identical despite different names*

