# Comparing `tmp/pyPPG-1.0.1.tar.gz` & `tmp/pyPPG-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPPG-1.0.1.tar", last modified: Thu Jul 27 15:20:00 2023, max compression
+gzip compressed data, was "pyPPG-1.0.2.tar", last modified: Thu Jul 27 15:38:56 2023, max compression
```

## Comparing `pyPPG-1.0.1.tar` & `pyPPG-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 15:20:00.987187 pyPPG-1.0.1/
--rw-rw-rw-   0        0        0      105 2023-05-03 11:40:28.000000 pyPPG-1.0.1/AUTHORS.rst
--rw-rw-rw-   0        0        0    35972 2023-07-18 09:12:28.000000 pyPPG-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      619 2023-07-27 15:20:00.987187 pyPPG-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3415 2023-07-27 14:35:58.000000 pyPPG-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 15:20:00.970239 pyPPG-1.0.1/pyPPG/
--rw-rw-rw-   0        0        0     3194 2023-07-26 11:45:26.000000 pyPPG-1.0.1/pyPPG/Biomarkers.py
--rw-rw-rw-   0        0        0     9372 2023-07-27 08:33:09.000000 pyPPG-1.0.1/pyPPG/DataHandling.py
--rw-rw-rw-   0        0        0     2145 2023-07-27 09:19:15.000000 pyPPG-1.0.1/pyPPG/EXAMPLE.py
--rw-rw-rw-   0        0        0    49759 2023-07-27 08:52:59.000000 pyPPG-1.0.1/pyPPG/FiducialPoints.py
--rw-rw-rw-   0        0        0     1845 2023-07-27 08:06:54.000000 pyPPG-1.0.1/pyPPG/Preprocessing.py
--rw-rw-rw-   0        0        0     1906 2023-07-26 12:38:04.000000 pyPPG-1.0.1/pyPPG/Statistics.py
--rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.1/pyPPG/__init__.py
--rw-rw-rw-   0        0        0     4945 2023-07-23 15:56:13.000000 pyPPG-1.0.1/pyPPG/ppgSQI.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:20:00.986465 pyPPG-1.0.1/pyPPG/ppg_bm/
--rw-rw-rw-   0        0        0        0 2023-07-21 19:27:04.000000 pyPPG-1.0.1/pyPPG/ppg_bm/__init__.py
--rw-rw-rw-   0        0        0    49194 2023-07-26 11:16:42.000000 pyPPG-1.0.1/pyPPG/ppg_bm/get_biomarkers.py
--rw-rw-rw-   0        0        0     4754 2023-07-23 15:47:56.000000 pyPPG-1.0.1/pyPPG/ppg_bm/get_bm_derivs_ratios.py
--rw-rw-rw-   0        0        0     3230 2023-07-23 15:47:56.000000 pyPPG-1.0.1/pyPPG/ppg_bm/get_bm_ppg_derivs.py
--rw-rw-rw-   0        0        0     6086 2023-07-23 15:49:12.000000 pyPPG-1.0.1/pyPPG/ppg_bm/get_bm_ppg_sig.py
--rw-rw-rw-   0        0        0     4313 2023-07-23 15:47:56.000000 pyPPG-1.0.1/pyPPG/ppg_bm/get_bm_sig_ratios.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:20:00.970239 pyPPG-1.0.1/pyPPG.egg-info/
--rw-rw-rw-   0        0        0      619 2023-07-27 15:20:00.000000 pyPPG-1.0.1/pyPPG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-07-27 15:20:00.000000 pyPPG-1.0.1/pyPPG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 15:20:00.000000 pyPPG-1.0.1/pyPPG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 15:20:00.000000 pyPPG-1.0.1/pyPPG.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-27 15:20:00.000000 pyPPG-1.0.1/pyPPG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      190 2023-07-27 13:48:40.000000 pyPPG-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 15:20:00.987187 pyPPG-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-07-27 15:10:13.000000 pyPPG-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:38:56.005346 pyPPG-1.0.2/
+-rw-rw-rw-   0        0        0      105 2023-05-03 11:40:28.000000 pyPPG-1.0.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0    35972 2023-07-18 09:12:28.000000 pyPPG-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      619 2023-07-27 15:38:56.005346 pyPPG-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3415 2023-07-27 14:35:58.000000 pyPPG-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 15:38:55.989700 pyPPG-1.0.2/pyPPG/
+-rw-rw-rw-   0        0        0     3194 2023-07-26 11:45:26.000000 pyPPG-1.0.2/pyPPG/Biomarkers.py
+-rw-rw-rw-   0        0        0     9372 2023-07-27 08:33:09.000000 pyPPG-1.0.2/pyPPG/DataHandling.py
+-rw-rw-rw-   0        0        0     2145 2023-07-27 09:19:15.000000 pyPPG-1.0.2/pyPPG/EXAMPLE.py
+-rw-rw-rw-   0        0        0    49759 2023-07-27 08:52:59.000000 pyPPG-1.0.2/pyPPG/FiducialPoints.py
+-rw-rw-rw-   0        0        0     1845 2023-07-27 08:06:54.000000 pyPPG-1.0.2/pyPPG/Preprocessing.py
+-rw-rw-rw-   0        0        0     1906 2023-07-26 12:38:04.000000 pyPPG-1.0.2/pyPPG/Statistics.py
+-rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.2/pyPPG/__init__.py
+-rw-rw-rw-   0        0        0     4945 2023-07-23 15:56:13.000000 pyPPG-1.0.2/pyPPG/ppgSQI.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:38:56.005346 pyPPG-1.0.2/pyPPG/ppg_bm/
+-rw-rw-rw-   0        0        0        0 2023-07-21 19:27:04.000000 pyPPG-1.0.2/pyPPG/ppg_bm/__init__.py
+-rw-rw-rw-   0        0        0    49194 2023-07-26 11:16:42.000000 pyPPG-1.0.2/pyPPG/ppg_bm/get_biomarkers.py
+-rw-rw-rw-   0        0        0     4754 2023-07-23 15:47:56.000000 pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_derivs_ratios.py
+-rw-rw-rw-   0        0        0     3230 2023-07-23 15:47:56.000000 pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_ppg_derivs.py
+-rw-rw-rw-   0        0        0     6086 2023-07-23 15:49:12.000000 pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_ppg_sig.py
+-rw-rw-rw-   0        0        0     4313 2023-07-23 15:47:56.000000 pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_sig_ratios.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:38:56.005346 pyPPG-1.0.2/pyPPG.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-07-27 15:38:55.000000 pyPPG-1.0.2/pyPPG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-07-27 15:38:55.000000 pyPPG-1.0.2/pyPPG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 15:38:55.000000 pyPPG-1.0.2/pyPPG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 15:38:55.000000 pyPPG-1.0.2/pyPPG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-27 15:38:55.000000 pyPPG-1.0.2/pyPPG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-07-27 13:48:40.000000 pyPPG-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 15:38:56.005346 pyPPG-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-07-27 15:38:28.000000 pyPPG-1.0.2/setup.py
```

### Comparing `pyPPG-1.0.1/LICENSE.txt` & `pyPPG-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/PKG-INFO` & `pyPPG-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPPG
-Version: 1.0.1
+Version: 1.0.2
 Summary: pyPPG: a python toolbox for PPG morphological analysis.
 Home-page: https://github.com/godamartonaron/GODA_pyPPG
 Author: Marton A. Goda, PhD
 Author-email: marton.goda@campus.technion.ac.il
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `pyPPG-1.0.1/README.md` & `pyPPG-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG/Biomarkers.py` & `pyPPG-1.0.2/pyPPG/Biomarkers.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG/DataHandling.py` & `pyPPG-1.0.2/pyPPG/DataHandling.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG/EXAMPLE.py` & `pyPPG-1.0.2/pyPPG/EXAMPLE.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG/FiducialPoints.py` & `pyPPG-1.0.2/pyPPG/FiducialPoints.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG/Preprocessing.py` & `pyPPG-1.0.2/pyPPG/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG/Statistics.py` & `pyPPG-1.0.2/pyPPG/Statistics.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG/ppgSQI.py` & `pyPPG-1.0.2/pyPPG/ppgSQI.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG/ppg_bm/get_biomarkers.py` & `pyPPG-1.0.2/pyPPG/ppg_bm/get_biomarkers.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG/ppg_bm/get_bm_derivs_ratios.py` & `pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_derivs_ratios.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG/ppg_bm/get_bm_ppg_derivs.py` & `pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_ppg_derivs.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG/ppg_bm/get_bm_ppg_sig.py` & `pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_ppg_sig.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG/ppg_bm/get_bm_sig_ratios.py` & `pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_sig_ratios.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/pyPPG.egg-info/PKG-INFO` & `pyPPG-1.0.2/pyPPG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPPG
-Version: 1.0.1
+Version: 1.0.2
 Summary: pyPPG: a python toolbox for PPG morphological analysis.
 Home-page: https://github.com/godamartonaron/GODA_pyPPG
 Author: Marton A. Goda, PhD
 Author-email: marton.goda@campus.technion.ac.il
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `pyPPG-1.0.1/pyPPG.egg-info/SOURCES.txt` & `pyPPG-1.0.2/pyPPG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.1/setup.py` & `pyPPG-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyPPG',
-    version='1.0.1',
+    version='1.0.2',
     description='pyPPG: a python toolbox for PPG morphological analysis.',
     author='Marton A. Goda, PhD',
     author_email="marton.goda@campus.technion.ac.il",
     long_description=0,
     long_description_content_type="text/markdown",
     url="https://github.com/godamartonaron/GODA_pyPPG",
     project_urls={"Bug Tracker": "https://github.com/pypa/sampleproject/issues",},
```

