# Comparing `tmp/ccsf-1.0.2.tar.gz` & `tmp/ccsf-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccsf-1.0.2.tar", last modified: Wed Jul 26 23:28:01 2023, max compression
+gzip compressed data, was "ccsf-1.0.3.tar", last modified: Wed Jul 26 23:37:27 2023, max compression
```

## Comparing `ccsf-1.0.2.tar` & `ccsf-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:28:01.585118 ccsf-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-26 23:26:44.000000 ccsf-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 23:26:44.000000 ccsf-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-26 23:28:01.585118 ccsf-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-26 23:26:44.000000 ccsf-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:28:01.585118 ccsf-1.0.2/ccsf/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 23:26:44.000000 ccsf-1.0.2/ccsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-07-26 23:26:44.000000 ccsf-1.0.2/ccsf/ccsf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:28:01.585118 ccsf-1.0.2/ccsf/class_discriminative_opt/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 23:26:44.000000 ccsf-1.0.2/ccsf/class_discriminative_opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-26 23:26:44.000000 ccsf-1.0.2/ccsf/class_discriminative_opt/class_discriminative_opt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:28:01.585118 ccsf-1.0.2/ccsf/group_centroid_opt/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 23:26:44.000000 ccsf-1.0.2/ccsf/group_centroid_opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-26 23:26:44.000000 ccsf-1.0.2/ccsf/group_centroid_opt/group_centroid_opt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:28:01.585118 ccsf-1.0.2/ccsf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-26 23:28:01.000000 ccsf-1.0.2/ccsf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-26 23:28:01.000000 ccsf-1.0.2/ccsf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:28:01.000000 ccsf-1.0.2/ccsf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 23:28:01.000000 ccsf-1.0.2/ccsf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 23:28:01.000000 ccsf-1.0.2/ccsf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-26 23:26:44.000000 ccsf-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:28:01.585118 ccsf-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 23:26:44.000000 ccsf-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:37:27.488936 ccsf-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-26 23:35:58.000000 ccsf-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 23:35:58.000000 ccsf-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-26 23:37:27.484936 ccsf-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-26 23:35:58.000000 ccsf-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:37:27.484936 ccsf-1.0.3/ccsf/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 23:35:58.000000 ccsf-1.0.3/ccsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-07-26 23:35:58.000000 ccsf-1.0.3/ccsf/ccsf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:37:27.484936 ccsf-1.0.3/ccsf/class_discriminative_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 23:35:58.000000 ccsf-1.0.3/ccsf/class_discriminative_opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-26 23:35:58.000000 ccsf-1.0.3/ccsf/class_discriminative_opt/class_discriminative_opt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:37:27.484936 ccsf-1.0.3/ccsf/group_centroid_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 23:35:58.000000 ccsf-1.0.3/ccsf/group_centroid_opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-26 23:35:58.000000 ccsf-1.0.3/ccsf/group_centroid_opt/group_centroid_opt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:37:27.484936 ccsf-1.0.3/ccsf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-26 23:37:27.000000 ccsf-1.0.3/ccsf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-26 23:37:27.000000 ccsf-1.0.3/ccsf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:37:27.000000 ccsf-1.0.3/ccsf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-26 23:37:27.000000 ccsf-1.0.3/ccsf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 23:37:27.000000 ccsf-1.0.3/ccsf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-26 23:35:58.000000 ccsf-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:37:27.488936 ccsf-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 23:35:58.000000 ccsf-1.0.3/setup.py
```

### Comparing `ccsf-1.0.2/LICENSE` & `ccsf-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.2/PKG-INFO` & `ccsf-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccsf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Leveraging cell-cell similarity from gene expression data for high-performance spatial and temporal cellular mappings.
 Home-page: https://github.com/xinglab-ai/ccsf
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ccsf-1.0.2/README.md` & `ccsf-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.2/ccsf/ccsf.py` & `ccsf-1.0.3/ccsf/ccsf.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.2/ccsf/class_discriminative_opt/class_discriminative_opt.py` & `ccsf-1.0.3/ccsf/class_discriminative_opt/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.2/ccsf/group_centroid_opt/group_centroid_opt.py` & `ccsf-1.0.3/ccsf/group_centroid_opt/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `ccsf-1.0.2/ccsf.egg-info/PKG-INFO` & `ccsf-1.0.3/ccsf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccsf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Leveraging cell-cell similarity from gene expression data for high-performance spatial and temporal cellular mappings.
 Home-page: https://github.com/xinglab-ai/ccsf
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ccsf-1.0.2/setup.py` & `ccsf-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ccsf",
-    version="1.0.2",
+    version="1.0.3",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Leveraging cell-cell similarity from gene expression data for high-performance spatial and temporal cellular mappings.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/ccsf",
     classifiers=[
```

