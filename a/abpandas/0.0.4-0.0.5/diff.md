# Comparing `tmp/abpandas-0.0.4.tar.gz` & `tmp/abpandas-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abpandas-0.0.4.tar", last modified: Thu Jul 27 14:00:43 2023, max compression
+gzip compressed data, was "abpandas-0.0.5.tar", last modified: Thu Jul 27 14:16:56 2023, max compression
```

## Comparing `abpandas-0.0.4.tar` & `abpandas-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 14:00:43.387643 abpandas-0.0.4/
--rw-rw-rw-   0        0        0      894 2023-07-27 14:00:43.383484 abpandas-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 14:00:43.325852 abpandas-0.0.4/abpandas/
--rw-rw-rw-   0        0        0       85 2023-07-26 18:33:02.000000 abpandas-0.0.4/abpandas/__init__.py
--rw-rw-rw-   0        0        0      739 2023-07-27 10:03:57.000000 abpandas-0.0.4/abpandas/agent.py
--rw-rw-rw-   0        0        0     7724 2023-07-27 13:59:28.000000 abpandas-0.0.4/abpandas/model.py
--rw-rw-rw-   0        0        0     1859 2023-07-27 13:59:49.000000 abpandas-0.0.4/abpandas/space.py
-drwxrwxrwx   0        0        0        0 2023-07-27 14:00:43.380523 abpandas-0.0.4/abpandas.egg-info/
--rw-rw-rw-   0        0        0      894 2023-07-27 14:00:43.000000 abpandas-0.0.4/abpandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-07-27 14:00:43.000000 abpandas-0.0.4/abpandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 14:00:43.000000 abpandas-0.0.4/abpandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-27 14:00:43.000000 abpandas-0.0.4/abpandas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-27 14:00:43.000000 abpandas-0.0.4/abpandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 14:00:43.388641 abpandas-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1466 2023-07-27 14:00:34.000000 abpandas-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:16:56.860983 abpandas-0.0.5/
+-rw-rw-rw-   0        0        0      894 2023-07-27 14:16:56.857963 abpandas-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 14:16:56.812739 abpandas-0.0.5/abpandas/
+-rw-rw-rw-   0        0        0       85 2023-07-26 18:33:02.000000 abpandas-0.0.5/abpandas/__init__.py
+-rw-rw-rw-   0        0        0      739 2023-07-27 14:16:22.000000 abpandas-0.0.5/abpandas/agent.py
+-rw-rw-rw-   0        0        0     7767 2023-07-27 14:16:20.000000 abpandas-0.0.5/abpandas/model.py
+-rw-rw-rw-   0        0        0     1859 2023-07-27 14:16:17.000000 abpandas-0.0.5/abpandas/space.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:16:56.853829 abpandas-0.0.5/abpandas.egg-info/
+-rw-rw-rw-   0        0        0      894 2023-07-27 14:16:56.000000 abpandas-0.0.5/abpandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-07-27 14:16:56.000000 abpandas-0.0.5/abpandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 14:16:56.000000 abpandas-0.0.5/abpandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-27 14:16:56.000000 abpandas-0.0.5/abpandas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 14:16:56.000000 abpandas-0.0.5/abpandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 14:16:56.861983 abpandas-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1466 2023-07-27 14:16:28.000000 abpandas-0.0.5/setup.py
```

### Comparing `abpandas-0.0.4/PKG-INFO` & `abpandas-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abpandas
-Version: 0.0.4
+Version: 0.0.5
 Summary: Agent Based Pandas tool (ABPandas)
 Author: Yahya Gamal
 Author-email: <abpandas.yg@outlook.com>
 Keywords: python,Agent Based Model,Spatial,Pandas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
```

### Comparing `abpandas-0.0.4/abpandas/agent.py` & `abpandas-0.0.5/abpandas/agent.py`

 * *Files identical despite different names*

### Comparing `abpandas-0.0.4/abpandas/model.py` & `abpandas-0.0.5/abpandas/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,13 +224,12 @@
         
         Returns
         -------
         int
             index of the polygon in the abpandas.space geodataframe
         """
         try:
-            temp_index = self.space[self.space['i'] == i][self.space['j'] == j].index[0]
-            return temp_index
+            temp_index_a = self.space[self.space['i'] == i]
+            temp_index_b = temp_index_a[temp_index_a['j'] == j]
+            return temp_index_b.index[0]
         except:
             print("Error: invalid i or j")
-
-
```

### Comparing `abpandas-0.0.4/abpandas/space.py` & `abpandas-0.0.5/abpandas/space.py`

 * *Files identical despite different names*

### Comparing `abpandas-0.0.4/abpandas.egg-info/PKG-INFO` & `abpandas-0.0.5/abpandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abpandas
-Version: 0.0.4
+Version: 0.0.5
 Summary: Agent Based Pandas tool (ABPandas)
 Author: Yahya Gamal
 Author-email: <abpandas.yg@outlook.com>
 Keywords: python,Agent Based Model,Spatial,Pandas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
```

### Comparing `abpandas-0.0.4/setup.py` & `abpandas-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'Agent Based Pandas tool (ABPandas)'
 LONG_DESCRIPTION = 'An Agent Based Modelling (ABM) package that can generate grid spatial shape files or work with predefined shape files.\nThe package focuses on simplicity by assigning Agents to spatial Polygons instead of assigning x and y locations for each agents.\nThis makes it useful in situations where granual movement of agents in space is not necessary (e.g. residentail location models)'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="abpandas",
```

