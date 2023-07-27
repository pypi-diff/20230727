# Comparing `tmp/mcemtools-0.8.0.tar.gz` & `tmp/mcemtools-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.8.0.tar", last modified: Wed Jul 19 12:55:35 2023, max compression
+gzip compressed data, was "mcemtools-0.8.1.tar", last modified: Thu Jul 27 13:34:58 2023, max compression
```

## Comparing `mcemtools-0.8.0.tar` & `mcemtools-0.8.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:35.405779 mcemtools-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-19 12:55:24.000000 mcemtools-0.8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-19 12:55:24.000000 mcemtools-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-19 12:55:24.000000 mcemtools-0.8.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-19 12:55:24.000000 mcemtools-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-19 12:55:24.000000 mcemtools-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-19 12:55:35.405779 mcemtools-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-19 12:55:24.000000 mcemtools-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:35.405779 mcemtools-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-19 12:55:24.000000 mcemtools-0.8.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:35.405779 mcemtools-0.8.0/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-19 12:55:24.000000 mcemtools-0.8.0/mcemtools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:35.405779 mcemtools-0.8.0/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 12:55:35.000000 mcemtools-0.8.0/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-19 12:55:24.000000 mcemtools-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-19 12:55:35.405779 mcemtools-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-19 12:55:24.000000 mcemtools-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:55:35.405779 mcemtools-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-19 12:55:24.000000 mcemtools-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-19 12:55:24.000000 mcemtools-0.8.0/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-19 12:55:24.000000 mcemtools-0.8.0/tests/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-19 12:55:24.000000 mcemtools-0.8.0/tests/test_mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-19 12:55:24.000000 mcemtools-0.8.0/tests/test_tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-19 12:55:24.000000 mcemtools-0.8.0/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:58.850114 mcemtools-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-27 13:34:46.000000 mcemtools-0.8.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-27 13:34:46.000000 mcemtools-0.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-27 13:34:46.000000 mcemtools-0.8.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-27 13:34:46.000000 mcemtools-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-27 13:34:46.000000 mcemtools-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-27 13:34:58.850114 mcemtools-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-27 13:34:46.000000 mcemtools-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:58.846114 mcemtools-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:58.846114 mcemtools-0.8.1/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:58.846114 mcemtools-0.8.1/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 13:34:46.000000 mcemtools-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-27 13:34:58.850114 mcemtools-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-27 13:34:46.000000 mcemtools-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:58.850114 mcemtools-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-27 13:34:46.000000 mcemtools-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-27 13:34:46.000000 mcemtools-0.8.1/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-27 13:34:46.000000 mcemtools-0.8.1/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-27 13:34:46.000000 mcemtools-0.8.1/tests/test_mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-27 13:34:46.000000 mcemtools-0.8.1/tests/test_tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-27 13:34:46.000000 mcemtools-0.8.1/tests/test_transforms.py
```

### Comparing `mcemtools-0.8.0/CONTRIBUTING.rst` & `mcemtools-0.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/LICENSE` & `mcemtools-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/PKG-INFO` & `mcemtools-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.8.0
+Version: 0.8.1
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -104,7 +104,11 @@
 * markimage bug is fixed
 
 0.8.0 (2023-07-19)
 ------------------
 * markimage bug is fixed really as US version of centre is center.
 * napari based GUI is added to mcemtools.
 * bianary files can be read too.
+
+0.8.1 (2023-07-27)
+------------------
+* viewer_4D is a lot more concise and bug free.
```

### Comparing `mcemtools-0.8.0/README.rst` & `mcemtools-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/docs/Makefile` & `mcemtools-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/docs/conf.py` & `mcemtools-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/docs/installation.rst` & `mcemtools-0.8.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/docs/make.bat` & `mcemtools-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/mcemtools/__init__.py` & `mcemtools-0.8.1/mcemtools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for mcemtools."""
 
 __author__ = """Alireza Sadri"""
 __email__ = 'Alireza.Sadri@monash.edu'
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 
 from .analysis import pyMSSE, cross_correlation_4D, SymmSTEM
 from .analysis import centre_of_mass_4D, sum_4D
 
 from .masking import annular_mask, image_by_windows, markimage, mask2D_to_4D
 
 from .tensor_svd import svd_fit, svd_eval
```

### Comparing `mcemtools-0.8.0/mcemtools/analysis.py` & `mcemtools-0.8.1/mcemtools/analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,28 @@
             est_std = cumsums[n_inliers] ** 0.5
             est_done = True
     if (not est_done):
         est_std = cumsums[-1] ** 0.5
         n_inliers = fitting_errors.shape[0]
     return (est_std, n_inliers, adjacencies, res_sq_sortinds)
 
+def swirl_and_sum(img):
+    _img = np.zeros(img.shape, dtype = img.dtype)
+    _img[1:-1, 1:-1] = \
+          img[ :-2,  :-2] \
+        + img[ :-2, 1:-1] \
+        + img[ :-2, 2:  ] \
+        + img[1:-1,  :-2] \
+        + img[1:-1, 1:-1] \
+        + img[1:-1, 2:  ] \
+        + img[2:  ,  :-2] \
+        + img[2:  , 1:-1] \
+        + img[2:  , 2:  ]
+    return _img
+    
 def sum_4D(data4D, mask4D = None):
     """ Annular virtual detector
             Given a 4D dataset, n_x x n_y x n_r x n_c.
             the output is the marginalized images over the n_x, n_y or n_r,n_c
         
         :param data4D:
             data in 4 dimension real_x x real_y x k_r x k_c
```

### Comparing `mcemtools-0.8.0/mcemtools/masking.py` & `mcemtools-0.8.1/mcemtools/masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/mcemtools/tensor_svd.py` & `mcemtools-0.8.1/mcemtools/tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/mcemtools/transforms.py` & `mcemtools-0.8.1/mcemtools/transforms.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.8.1/mcemtools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.8.0
+Version: 0.8.1
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -104,7 +104,11 @@
 * markimage bug is fixed
 
 0.8.0 (2023-07-19)
 ------------------
 * markimage bug is fixed really as US version of centre is center.
 * napari based GUI is added to mcemtools.
 * bianary files can be read too.
+
+0.8.1 (2023-07-27)
+------------------
+* viewer_4D is a lot more concise and bug free.
```

### Comparing `mcemtools-0.8.0/mcemtools.egg-info/SOURCES.txt` & `mcemtools-0.8.1/mcemtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/setup.py` & `mcemtools-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
```

### Comparing `mcemtools-0.8.0/tests/test_analysis.py` & `mcemtools-0.8.1/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/tests/test_masking.py` & `mcemtools-0.8.1/tests/test_masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/tests/test_mcemtools.py` & `mcemtools-0.8.1/tests/test_mcemtools.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/tests/test_tensor_svd.py` & `mcemtools-0.8.1/tests/test_tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.0/tests/test_transforms.py` & `mcemtools-0.8.1/tests/test_transforms.py`

 * *Files identical despite different names*

