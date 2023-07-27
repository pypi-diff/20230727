# Comparing `tmp/catencfamily-0.0.87.tar.gz` & `tmp/catencfamily-0.0.88.tar.gz`

## Comparing `catencfamily-0.0.87.tar` & `catencfamily-0.0.88.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.87/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    89962 2020-02-02 00:00:00.000000 catencfamily-0.0.87/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    45237 2020-02-02 00:00:00.000000 catencfamily-0.0.87/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.87/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.87/README.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.87/pyproject.toml
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.87/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.88/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    90098 2020-02-02 00:00:00.000000 catencfamily-0.0.88/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    45499 2020-02-02 00:00:00.000000 catencfamily-0.0.88/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.88/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.88/README.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.88/pyproject.toml
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.88/PKG-INFO
```

### Comparing `catencfamily-0.0.87/src/catencfamily/encoders.py` & `catencfamily-0.0.88/src/catencfamily/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 7th July, 2023
+# 26th July, 2023
 """
 References:
 Coding standard:
     https://gist.github.com/nateGeorge/5455d2c57fb33c1ae04706f2dc4fee01
     
 Developing sklearn estimators:
     https://scikit-learn.org/stable/developers/develop.html 
@@ -1299,14 +1299,15 @@
         -----
     
         The method locates communities in the unipartite network
         and also calculates two community related measures: density and
         avg_embeddedness. It returns 3-dictionaries. The first dict indicates 
         which node falls in which community. The other two dictionaries 
         contain node-wise community characteristics.
+        Ref: https://cdlib.readthedocs.io/en/latest/reference/cd_algorithms/algs/cdlib.algorithms.leiden.html#cdlib-algorithms-leiden
         
         Parameters
         ----------
         network: Graph object
         colToProject: string; A column name. Bottom column 
         intermediaryCol: string; A column name. Top column
```

### Comparing `catencfamily-0.0.87/src/catencfamily/utils.py` & `catencfamily-0.0.88/src/catencfamily/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-# 5th July, 2023
+# 27th July, 2023
 
 ## Utility functions
 
 
 import pandas as pd
 import numpy as np
 from scipy.stats import kurtosis
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import StandardScaler
 from sklearn.datasets import make_classification
 from sklearn.cluster import KMeans
 from sklearn.mixture import GaussianMixture
 from sklearn.feature_selection import  mutual_info_classif
 import networkx as nx
+# added 27th July, 2023
+from cdlib import algorithms
 import itertools
 import pickle
 import pathlib
 import string
 import matplotlib.pyplot as plt
 import seaborn as sns
 from pathlib import Path
@@ -1031,16 +1033,21 @@
     colors = colorList
     pos = nx.spring_layout(G, k)
     
     if algo == nx.community.girvan_newman:
         lst_b = algo(G)
         lst_b = tuple(sorted(c) for c in next(lst_b))
         lst_b = [frozenset(i) for i in lst_b ]
-    else:
+    # Changed on 27th July, 2023    
+    if algo ==  algorithms.leiden:
         lst_b = algo(G)
+        lst_b = tuple(sorted(c) for c in next(lst_b))
+        lst_b = [frozenset(i) for i in lst_b ]
+    else:
+        lst_b = algo(G)    
 
     
     color_map_b = {}
     keys = G.nodes()
     values = "black"
     for i in keys:
             color_map_b[i] = values
```

### Comparing `catencfamily-0.0.87/LICENSE` & `catencfamily-0.0.88/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.87/README.md` & `catencfamily-0.0.88/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.87/pyproject.toml` & `catencfamily-0.0.88/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.87"
+version = "0.0.88"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.87/PKG-INFO` & `catencfamily-0.0.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.87
+Version: 0.0.88
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

