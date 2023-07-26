# Comparing `tmp/ccsf-1.0.0.tar.gz` & `tmp/ccsf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccsf-1.0.0.tar", last modified: Wed Jul 26 22:12:08 2023, max compression
+gzip compressed data, was "ccsf-1.0.1.tar", last modified: Wed Jul 26 23:12:16 2023, max compression
```

## Comparing `ccsf-1.0.0.tar` & `ccsf-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:12:08.626875 ccsf-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-26 22:11:02.000000 ccsf-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 22:11:02.000000 ccsf-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-26 22:12:08.626875 ccsf-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-26 22:11:02.000000 ccsf-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:12:08.626875 ccsf-1.0.0/ccsf/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/ccsf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:12:08.626875 ccsf-1.0.0/ccsf/class_discriminative_opt/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/class_discriminative_opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/class_discriminative_opt/class_discriminative_opt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:12:08.626875 ccsf-1.0.0/ccsf/group_centroid_opt/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/group_centroid_opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/group_centroid_opt/group_centroid_opt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:12:08.626875 ccsf-1.0.0/ccsf/novosparc/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/novosparc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:12:08.626875 ccsf-1.0.0/ccsf/novosparc/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/novosparc/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/novosparc/geometry/_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:12:08.626875 ccsf-1.0.0/ccsf/novosparc/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/novosparc/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/novosparc/plotting/_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:12:08.626875 ccsf-1.0.0/ccsf/novosparc/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/novosparc/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/novosparc/preprocessing/_preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:12:08.626875 ccsf-1.0.0/ccsf/novosparc/reconstruction/
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/novosparc/reconstruction/_GWadjusted.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/novosparc/reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-26 22:11:02.000000 ccsf-1.0.0/ccsf/novosparc/reconstruction/_reconstruction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:12:08.626875 ccsf-1.0.0/ccsf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-26 22:12:08.000000 ccsf-1.0.0/ccsf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-26 22:12:08.000000 ccsf-1.0.0/ccsf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:12:08.000000 ccsf-1.0.0/ccsf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 22:12:08.000000 ccsf-1.0.0/ccsf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 22:12:08.000000 ccsf-1.0.0/ccsf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-26 22:11:02.000000 ccsf-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:12:08.626875 ccsf-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 22:11:02.000000 ccsf-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:12:16.724700 ccsf-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-26 23:11:09.000000 ccsf-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 23:11:09.000000 ccsf-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-26 23:12:16.724700 ccsf-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-26 23:11:09.000000 ccsf-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:12:16.720700 ccsf-1.0.1/ccsf/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/ccsf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:12:16.724700 ccsf-1.0.1/ccsf/class_discriminative_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/class_discriminative_opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/class_discriminative_opt/class_discriminative_opt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:12:16.724700 ccsf-1.0.1/ccsf/group_centroid_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/group_centroid_opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/group_centroid_opt/group_centroid_opt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:12:16.724700 ccsf-1.0.1/ccsf/novosparc/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/novosparc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:12:16.724700 ccsf-1.0.1/ccsf/novosparc/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/novosparc/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/novosparc/geometry/_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:12:16.724700 ccsf-1.0.1/ccsf/novosparc/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/novosparc/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/novosparc/plotting/_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:12:16.724700 ccsf-1.0.1/ccsf/novosparc/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/novosparc/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/novosparc/preprocessing/_preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:12:16.724700 ccsf-1.0.1/ccsf/novosparc/reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/novosparc/reconstruction/_GWadjusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/novosparc/reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-26 23:11:09.000000 ccsf-1.0.1/ccsf/novosparc/reconstruction/_reconstruction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:12:16.724700 ccsf-1.0.1/ccsf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-26 23:12:16.000000 ccsf-1.0.1/ccsf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-26 23:12:16.000000 ccsf-1.0.1/ccsf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:12:16.000000 ccsf-1.0.1/ccsf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-26 23:12:16.000000 ccsf-1.0.1/ccsf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 23:12:16.000000 ccsf-1.0.1/ccsf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-26 23:11:09.000000 ccsf-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:12:16.724700 ccsf-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 23:11:09.000000 ccsf-1.0.1/setup.py
```

### Comparing `ccsf-1.0.0/LICENSE` & `ccsf-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.0/ccsf/ccsf.py` & `ccsf-1.0.1/ccsf/ccsf.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.0/ccsf/class_discriminative_opt/class_discriminative_opt.py` & `ccsf-1.0.1/ccsf/class_discriminative_opt/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.0/ccsf/group_centroid_opt/group_centroid_opt.py` & `ccsf-1.0.1/ccsf/group_centroid_opt/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.0/ccsf/novosparc/geometry/_geometry.py` & `ccsf-1.0.1/ccsf/novosparc/geometry/_geometry.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.0/ccsf/novosparc/plotting/_plotting.py` & `ccsf-1.0.1/ccsf/novosparc/plotting/_plotting.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.0/ccsf/novosparc/preprocessing/_preprocessing.py` & `ccsf-1.0.1/ccsf/novosparc/preprocessing/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.0/ccsf/novosparc/reconstruction/_GWadjusted.py` & `ccsf-1.0.1/ccsf/novosparc/reconstruction/_GWadjusted.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.0/ccsf/novosparc/reconstruction/_reconstruction.py` & `ccsf-1.0.1/ccsf/novosparc/reconstruction/_reconstruction.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.0/ccsf.egg-info/SOURCES.txt` & `ccsf-1.0.1/ccsf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.0/setup.py` & `ccsf-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ccsf",
-    version="1.0.0",
+    version="1.0.1",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Leveraging cell-cell similarity from gene expression data for high-performance spatial and temporal cellular mappings.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/ccsf",
     classifiers=[
```

