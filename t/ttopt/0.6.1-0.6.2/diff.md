# Comparing `tmp/ttopt-0.6.1.tar.gz` & `tmp/ttopt-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttopt-0.6.1.tar", last modified: Mon Jul 24 16:18:36 2023, max compression
+gzip compressed data, was "ttopt-0.6.2.tar", last modified: Thu Jul 27 20:14:17 2023, max compression
```

## Comparing `ttopt-0.6.1.tar` & `ttopt-0.6.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-24 16:18:36.342344 ttopt-0.6.1/
--rw-r--r--   0 andrei     (501) staff       (20)     1116 2023-05-20 17:13:27.000000 ttopt-0.6.1/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       63 2023-07-24 14:15:32.000000 ttopt-0.6.1/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     4248 2023-07-24 16:18:36.342559 ttopt-0.6.1/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     3035 2023-07-24 16:17:55.000000 ttopt-0.6.1/README.md
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-24 16:18:36.337483 ttopt-0.6.1/demo/
--rw-r--r--   0 andrei     (501) staff       (20)     2414 2023-07-24 16:07:54.000000 ttopt-0.6.1/demo/base.py
--rw-r--r--   0 andrei     (501) staff       (20)     2509 2023-07-24 16:09:42.000000 ttopt-0.6.1/demo/cache.py
--rw-r--r--   0 andrei     (501) staff       (20)     2645 2023-07-24 16:08:17.000000 ttopt-0.6.1/demo/qtt.py
--rw-r--r--   0 andrei     (501) staff       (20)     2529 2023-07-24 16:09:08.000000 ttopt-0.6.1/demo/qtt_100d.py
--rw-r--r--   0 andrei     (501) staff       (20)     2352 2023-07-24 16:08:38.000000 ttopt-0.6.1/demo/qtt_max.py
--rw-r--r--   0 andrei     (501) staff       (20)     2594 2023-07-24 16:09:58.000000 ttopt-0.6.1/demo/tensor.py
--rw-r--r--   0 andrei     (501) staff       (20)     3134 2023-07-24 16:10:18.000000 ttopt-0.6.1/demo/tensor_init.py
--rw-r--r--   0 andrei     (501) staff       (20)     2484 2023-07-24 16:09:22.000000 ttopt-0.6.1/demo/vect.py
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-24 16:18:36.343571 ttopt-0.6.1/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2412 2023-07-24 14:16:39.000000 ttopt-0.6.1/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-24 16:18:36.339326 ttopt-0.6.1/ttopt/
--rw-r--r--   0 andrei     (501) staff       (20)      178 2023-07-24 16:16:53.000000 ttopt-0.6.1/ttopt/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     5267 2023-07-24 14:11:36.000000 ttopt-0.6.1/ttopt/maxvol.py
--rw-r--r--   0 andrei     (501) staff       (20)    22561 2023-07-24 15:59:59.000000 ttopt-0.6.1/ttopt/ttopt.py
--rw-r--r--   0 andrei     (501) staff       (20)    10763 2023-07-24 16:06:35.000000 ttopt-0.6.1/ttopt/ttopt_raw.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-24 16:18:36.341871 ttopt-0.6.1/ttopt.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     4248 2023-07-24 16:18:36.000000 ttopt-0.6.1/ttopt.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)      384 2023-07-24 16:18:36.000000 ttopt-0.6.1/ttopt.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-24 16:18:36.000000 ttopt-0.6.1/ttopt.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)      163 2023-07-24 16:18:36.000000 ttopt-0.6.1/ttopt.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)        6 2023-07-24 16:18:36.000000 ttopt-0.6.1/ttopt.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 20:14:17.356793 ttopt-0.6.2/
+-rw-r--r--   0 andrei     (501) staff       (20)     1116 2023-05-20 17:13:27.000000 ttopt-0.6.2/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       88 2023-07-27 20:13:30.000000 ttopt-0.6.2/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     4248 2023-07-27 20:14:17.356945 ttopt-0.6.2/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     3035 2023-07-27 20:12:13.000000 ttopt-0.6.2/README.md
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 20:14:17.352802 ttopt-0.6.2/demo/
+-rw-r--r--   0 andrei     (501) staff       (20)     2414 2023-07-24 16:07:54.000000 ttopt-0.6.2/demo/base.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2509 2023-07-24 16:09:42.000000 ttopt-0.6.2/demo/cache.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2645 2023-07-24 16:08:17.000000 ttopt-0.6.2/demo/qtt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2529 2023-07-24 16:09:08.000000 ttopt-0.6.2/demo/qtt_100d.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2352 2023-07-24 16:08:38.000000 ttopt-0.6.2/demo/qtt_max.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2594 2023-07-24 16:09:58.000000 ttopt-0.6.2/demo/tensor.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3134 2023-07-24 16:10:18.000000 ttopt-0.6.2/demo/tensor_init.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2484 2023-07-24 16:09:22.000000 ttopt-0.6.2/demo/vect.py
+-rw-r--r--   0 andrei     (501) staff       (20)      211 2023-07-24 14:42:56.000000 ttopt-0.6.2/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-27 20:14:17.357549 ttopt-0.6.2/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2412 2023-07-24 14:16:39.000000 ttopt-0.6.2/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 20:14:17.354514 ttopt-0.6.2/ttopt/
+-rw-r--r--   0 andrei     (501) staff       (20)      178 2023-07-27 20:12:08.000000 ttopt-0.6.2/ttopt/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5267 2023-07-24 14:11:36.000000 ttopt-0.6.2/ttopt/maxvol.py
+-rw-r--r--   0 andrei     (501) staff       (20)    22560 2023-07-27 20:11:25.000000 ttopt-0.6.2/ttopt/ttopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)    10763 2023-07-27 20:10:53.000000 ttopt-0.6.2/ttopt/ttopt_raw.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-27 20:14:17.356526 ttopt-0.6.2/ttopt.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     4248 2023-07-27 20:14:17.000000 ttopt-0.6.2/ttopt.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)      401 2023-07-27 20:14:17.000000 ttopt-0.6.2/ttopt.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-27 20:14:17.000000 ttopt-0.6.2/ttopt.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      163 2023-07-27 20:14:17.000000 ttopt-0.6.2/ttopt.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        6 2023-07-27 20:14:17.000000 ttopt-0.6.2/ttopt.egg-info/top_level.txt
```

### Comparing `ttopt-0.6.1/LICENSE.txt` & `ttopt-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ttopt-0.6.1/PKG-INFO` & `ttopt-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttopt
-Version: 0.6.1
+Version: 0.6.2
 Summary: Multivariate function optimizer based on the tensor train approach.
 Home-page: https://github.com/AndreiChertkov/ttopt
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 Project-URL: Source, https://github.com/AndreiChertkov/ttopt
 Keywords: function optimization function minimization low-rank representation tensor train format TT-decomposition cross approximation
 Classifier: Development Status :: 4 - Beta
@@ -34,15 +34,15 @@
 > Please, see also our software product [teneva](https://github.com/AndreiChertkov/teneva) which provides a very compact implementation of basic operations in the TT-format.
 
 
 ## Installation
 
 You can install the `ttopt` package for `python >= 3.7` with pip:
 ```bash
-pip install ttopt==0.6.1
+pip install ttopt==0.6.2
 ```
 
 
 ## Examples
 
 The demo-scripts with detailed comments are collected in the folder `demo`:
```

### Comparing `ttopt-0.6.1/README.md` & `ttopt-0.6.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 > Please, see also our software product [teneva](https://github.com/AndreiChertkov/teneva) which provides a very compact implementation of basic operations in the TT-format.
 
 
 ## Installation
 
 You can install the `ttopt` package for `python >= 3.7` with pip:
 ```bash
-pip install ttopt==0.6.1
+pip install ttopt==0.6.2
 ```
 
 
 ## Examples
 
 The demo-scripts with detailed comments are collected in the folder `demo`:
```

### Comparing `ttopt-0.6.1/demo/base.py` & `ttopt-0.6.2/demo/base.py`

 * *Files identical despite different names*

### Comparing `ttopt-0.6.1/demo/cache.py` & `ttopt-0.6.2/demo/cache.py`

 * *Files identical despite different names*

### Comparing `ttopt-0.6.1/demo/qtt.py` & `ttopt-0.6.2/demo/qtt.py`

 * *Files identical despite different names*

### Comparing `ttopt-0.6.1/demo/qtt_100d.py` & `ttopt-0.6.2/demo/qtt_100d.py`

 * *Files identical despite different names*

### Comparing `ttopt-0.6.1/demo/qtt_max.py` & `ttopt-0.6.2/demo/qtt_max.py`

 * *Files identical despite different names*

### Comparing `ttopt-0.6.1/demo/tensor.py` & `ttopt-0.6.2/demo/tensor.py`

 * *Files identical despite different names*

### Comparing `ttopt-0.6.1/demo/tensor_init.py` & `ttopt-0.6.2/demo/tensor_init.py`

 * *Files identical despite different names*

### Comparing `ttopt-0.6.1/demo/vect.py` & `ttopt-0.6.2/demo/vect.py`

 * *Files identical despite different names*

### Comparing `ttopt-0.6.1/setup.py` & `ttopt-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `ttopt-0.6.1/ttopt/maxvol.py` & `ttopt-0.6.2/ttopt/maxvol.py`

 * *Files identical despite different names*

### Comparing `ttopt-0.6.1/ttopt/ttopt.py` & `ttopt-0.6.2/ttopt/ttopt.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,15 @@
             if with_e_x and self.e_x is not None:
                 text += f'e_x={self.e_x:-8.2e} '
             if with_e_y and self.e_y is not None:
                 text += f'e_y={self.e_y:-8.2e} '
 
         return text
 
-    def optimize(self, rank=10, Y0=None, seed=42, fs_opt=1., is_max=False,
+    def optimize(self, rank=4, Y0=None, seed=42, fs_opt=1., is_max=False,
                  add_opt_inner=True, add_opt_outer=False, add_opt_rect=False,
                  add_rnd_inner=False, add_rnd_outer=False, J0=None):
         """Perform the function optimization process by TT-based approach.
 
         Args:
             rank (int): maximum TT-rank.
             Y0 (list of 3D np.ndarrays of float): optional initial tensor in
```

### Comparing `ttopt-0.6.1/ttopt/ttopt_raw.py` & `ttopt-0.6.2/ttopt/ttopt_raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import numpy as np
 
 
 from .maxvol import maxvol
 from .maxvol import maxvol_rect
 
 
-def ttopt(f, n, rank=5, evals=None, Y0=None, seed=42, fs_opt=1.,
+def ttopt(f, n, rank=4, evals=None, Y0=None, seed=42, fs_opt=1.,
           add_opt_inner=True, add_opt_outer=False, add_opt_rect=False,
           add_rnd_inner=False, add_rnd_outer=False, J0=None, is_max=False):
     """Find the optimum element of the implicitly given multidimensional array.
 
     This function computes the minimum or maximum of the implicitly given
     d-dimensional (d >= 2) array (tensor). The adaptive method based on the
     TT-approximation and the cross-maximum-volume principle are used.
```

### Comparing `ttopt-0.6.1/ttopt.egg-info/PKG-INFO` & `ttopt-0.6.2/ttopt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttopt
-Version: 0.6.1
+Version: 0.6.2
 Summary: Multivariate function optimizer based on the tensor train approach.
 Home-page: https://github.com/AndreiChertkov/ttopt
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 Project-URL: Source, https://github.com/AndreiChertkov/ttopt
 Keywords: function optimization function minimization low-rank representation tensor train format TT-decomposition cross approximation
 Classifier: Development Status :: 4 - Beta
@@ -34,15 +34,15 @@
 > Please, see also our software product [teneva](https://github.com/AndreiChertkov/teneva) which provides a very compact implementation of basic operations in the TT-format.
 
 
 ## Installation
 
 You can install the `ttopt` package for `python >= 3.7` with pip:
 ```bash
-pip install ttopt==0.6.1
+pip install ttopt==0.6.2
 ```
 
 
 ## Examples
 
 The demo-scripts with detailed comments are collected in the folder `demo`:
```

