# Comparing `tmp/ccsf-1.0.3.tar.gz` & `tmp/ccsf-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccsf-1.0.3.tar", last modified: Wed Jul 26 23:37:27 2023, max compression
+gzip compressed data, was "ccsf-1.0.4.tar", last modified: Wed Jul 26 23:57:48 2023, max compression
```

## Comparing `ccsf-1.0.3.tar` & `ccsf-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:37:27.488936 ccsf-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-26 23:35:58.000000 ccsf-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 23:35:58.000000 ccsf-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-26 23:37:27.484936 ccsf-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-26 23:35:58.000000 ccsf-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:37:27.484936 ccsf-1.0.3/ccsf/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 23:35:58.000000 ccsf-1.0.3/ccsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-07-26 23:35:58.000000 ccsf-1.0.3/ccsf/ccsf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:37:27.484936 ccsf-1.0.3/ccsf/class_discriminative_opt/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 23:35:58.000000 ccsf-1.0.3/ccsf/class_discriminative_opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-26 23:35:58.000000 ccsf-1.0.3/ccsf/class_discriminative_opt/class_discriminative_opt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:37:27.484936 ccsf-1.0.3/ccsf/group_centroid_opt/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 23:35:58.000000 ccsf-1.0.3/ccsf/group_centroid_opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-26 23:35:58.000000 ccsf-1.0.3/ccsf/group_centroid_opt/group_centroid_opt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:37:27.484936 ccsf-1.0.3/ccsf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-26 23:37:27.000000 ccsf-1.0.3/ccsf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-26 23:37:27.000000 ccsf-1.0.3/ccsf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:37:27.000000 ccsf-1.0.3/ccsf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-26 23:37:27.000000 ccsf-1.0.3/ccsf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 23:37:27.000000 ccsf-1.0.3/ccsf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-26 23:35:58.000000 ccsf-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:37:27.488936 ccsf-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 23:35:58.000000 ccsf-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:57:48.041032 ccsf-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-26 23:56:30.000000 ccsf-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 23:56:30.000000 ccsf-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-26 23:57:48.041032 ccsf-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-26 23:56:30.000000 ccsf-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:57:48.037032 ccsf-1.0.4/ccsf/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 23:56:30.000000 ccsf-1.0.4/ccsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-07-26 23:56:30.000000 ccsf-1.0.4/ccsf/ccsf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:57:48.037032 ccsf-1.0.4/ccsf/class_discriminative_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 23:56:30.000000 ccsf-1.0.4/ccsf/class_discriminative_opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-26 23:56:30.000000 ccsf-1.0.4/ccsf/class_discriminative_opt/class_discriminative_opt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:57:48.041032 ccsf-1.0.4/ccsf/group_centroid_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 23:56:30.000000 ccsf-1.0.4/ccsf/group_centroid_opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-26 23:56:30.000000 ccsf-1.0.4/ccsf/group_centroid_opt/group_centroid_opt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:57:48.037032 ccsf-1.0.4/ccsf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-07-26 23:57:47.000000 ccsf-1.0.4/ccsf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-26 23:57:48.000000 ccsf-1.0.4/ccsf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:57:47.000000 ccsf-1.0.4/ccsf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-26 23:57:47.000000 ccsf-1.0.4/ccsf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 23:57:47.000000 ccsf-1.0.4/ccsf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-26 23:56:30.000000 ccsf-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:57:48.041032 ccsf-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 23:56:30.000000 ccsf-1.0.4/setup.py
```

### Comparing `ccsf-1.0.3/LICENSE` & `ccsf-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.3/PKG-INFO` & `ccsf-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccsf
-Version: 1.0.3
+Version: 1.0.4
 Summary: Leveraging cell-cell similarity from gene expression data for high-performance spatial and temporal cellular mappings.
 Home-page: https://github.com/xinglab-ai/ccsf
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -82,15 +82,19 @@
                    delim_whitespace=False)
 label = pd.read_csv('tcga_label.csv', header=None,
                          delim_whitespace=False).to_numpy()
 
 data= data.to_numpy()
 feed_data = {'data': data}
 manifolder = CCSF(random_state=rngState)
+n = 2000
+sampleix = random.sample(range(data.shape[0]), int(n))
+dataSampled = data[sampleix]
 metric, numClass = manifolder.metric_learning(dataSampled, verbose=False)
+dataSampled = stats.zscore(dataSampled, axis=0, ddof=1)
 num_comp= np.array([numClass-1]) # The number of CDM components to be used
 # to compute the cMAP
 manifolder = CCSF(n_clusters=numClass, num_comp=num_comp,metric=metric)
 embedding_CMAP = manifolder.cMap(data=feed_data)
 embedding = embedding_CMAP[0]
 plt.figure()
 plt.title('cMAP visualization ')
@@ -144,15 +148,15 @@
 
 embedding = embedding_CPHATE[0]
 plt.figure()
 plt.title('cPHATE for 32 CCIF components ')
 plt.scatter(embedding[:,0],embedding[:,1],c=label.T,s=0.5)
 plt.xlabel("cPHATE1")
 plt.ylabel("cPHATE2")
-plt.show() 
+plt.show()
 ```
 
 ### Example 4 - Spatial mapping by CCSF
 
 ```python
 # Import all the necessary Python packages
 from ccsf import CCSF
```

### Comparing `ccsf-1.0.3/README.md` & `ccsf-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,19 @@
                    delim_whitespace=False)
 label = pd.read_csv('tcga_label.csv', header=None,
                          delim_whitespace=False).to_numpy()
 
 data= data.to_numpy()
 feed_data = {'data': data}
 manifolder = CCSF(random_state=rngState)
+n = 2000
+sampleix = random.sample(range(data.shape[0]), int(n))
+dataSampled = data[sampleix]
 metric, numClass = manifolder.metric_learning(dataSampled, verbose=False)
+dataSampled = stats.zscore(dataSampled, axis=0, ddof=1)
 num_comp= np.array([numClass-1]) # The number of CDM components to be used
 # to compute the cMAP
 manifolder = CCSF(n_clusters=numClass, num_comp=num_comp,metric=metric)
 embedding_CMAP = manifolder.cMap(data=feed_data)
 embedding = embedding_CMAP[0]
 plt.figure()
 plt.title('cMAP visualization ')
@@ -131,15 +135,15 @@
 
 embedding = embedding_CPHATE[0]
 plt.figure()
 plt.title('cPHATE for 32 CCIF components ')
 plt.scatter(embedding[:,0],embedding[:,1],c=label.T,s=0.5)
 plt.xlabel("cPHATE1")
 plt.ylabel("cPHATE2")
-plt.show() 
+plt.show()
 ```
 
 ### Example 4 - Spatial mapping by CCSF
 
 ```python
 # Import all the necessary Python packages
 from ccsf import CCSF
```

### Comparing `ccsf-1.0.3/ccsf/ccsf.py` & `ccsf-1.0.4/ccsf/ccsf.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.3/ccsf/class_discriminative_opt/class_discriminative_opt.py` & `ccsf-1.0.4/ccsf/class_discriminative_opt/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.3/ccsf/group_centroid_opt/group_centroid_opt.py` & `ccsf-1.0.4/ccsf/group_centroid_opt/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.3/ccsf.egg-info/PKG-INFO` & `ccsf-1.0.4/ccsf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccsf
-Version: 1.0.3
+Version: 1.0.4
 Summary: Leveraging cell-cell similarity from gene expression data for high-performance spatial and temporal cellular mappings.
 Home-page: https://github.com/xinglab-ai/ccsf
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -82,15 +82,19 @@
                    delim_whitespace=False)
 label = pd.read_csv('tcga_label.csv', header=None,
                          delim_whitespace=False).to_numpy()
 
 data= data.to_numpy()
 feed_data = {'data': data}
 manifolder = CCSF(random_state=rngState)
+n = 2000
+sampleix = random.sample(range(data.shape[0]), int(n))
+dataSampled = data[sampleix]
 metric, numClass = manifolder.metric_learning(dataSampled, verbose=False)
+dataSampled = stats.zscore(dataSampled, axis=0, ddof=1)
 num_comp= np.array([numClass-1]) # The number of CDM components to be used
 # to compute the cMAP
 manifolder = CCSF(n_clusters=numClass, num_comp=num_comp,metric=metric)
 embedding_CMAP = manifolder.cMap(data=feed_data)
 embedding = embedding_CMAP[0]
 plt.figure()
 plt.title('cMAP visualization ')
@@ -144,15 +148,15 @@
 
 embedding = embedding_CPHATE[0]
 plt.figure()
 plt.title('cPHATE for 32 CCIF components ')
 plt.scatter(embedding[:,0],embedding[:,1],c=label.T,s=0.5)
 plt.xlabel("cPHATE1")
 plt.ylabel("cPHATE2")
-plt.show() 
+plt.show()
 ```
 
 ### Example 4 - Spatial mapping by CCSF
 
 ```python
 # Import all the necessary Python packages
 from ccsf import CCSF
```

### Comparing `ccsf-1.0.3/setup.py` & `ccsf-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ccsf",
-    version="1.0.3",
+    version="1.0.4",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Leveraging cell-cell similarity from gene expression data for high-performance spatial and temporal cellular mappings.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/ccsf",
     classifiers=[
```

