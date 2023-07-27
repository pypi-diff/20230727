# Comparing `tmp/abpandas-0.0.1.tar.gz` & `tmp/abpandas-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abpandas-0.0.1.tar", last modified: Wed Jul 26 22:03:27 2023, max compression
+gzip compressed data, was "abpandas-0.0.2.tar", last modified: Thu Jul 27 08:10:34 2023, max compression
```

## Comparing `abpandas-0.0.1.tar` & `abpandas-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 22:03:27.310027 abpandas-0.0.1/
--rw-rw-rw-   0        0        0      933 2023-07-26 22:03:27.309029 abpandas-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 22:03:27.284099 abpandas-0.0.1/abpandas/
--rw-rw-rw-   0        0        0       85 2023-07-26 18:33:02.000000 abpandas-0.0.1/abpandas/__init__.py
--rw-rw-rw-   0        0        0      739 2023-07-26 16:13:24.000000 abpandas-0.0.1/abpandas/agent.py
--rw-rw-rw-   0        0        0     6698 2023-07-26 18:33:17.000000 abpandas-0.0.1/abpandas/model.py
--rw-rw-rw-   0        0        0     1178 2023-07-26 15:50:02.000000 abpandas-0.0.1/abpandas/space.py
-drwxrwxrwx   0        0        0        0 2023-07-26 22:03:27.307034 abpandas-0.0.1/abpandas.egg-info/
--rw-rw-rw-   0        0        0      933 2023-07-26 22:03:26.000000 abpandas-0.0.1/abpandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-07-26 22:03:27.000000 abpandas-0.0.1/abpandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 22:03:26.000000 abpandas-0.0.1/abpandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-26 22:03:26.000000 abpandas-0.0.1/abpandas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 22:03:26.000000 abpandas-0.0.1/abpandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 22:03:27.310027 abpandas-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1466 2023-07-26 22:03:17.000000 abpandas-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:10:34.915096 abpandas-0.0.2/
+-rw-rw-rw-   0        0        0      894 2023-07-27 08:10:34.899091 abpandas-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 08:10:34.787092 abpandas-0.0.2/abpandas/
+-rw-rw-rw-   0        0        0       85 2023-07-26 18:33:02.000000 abpandas-0.0.2/abpandas/__init__.py
+-rw-rw-rw-   0        0        0      739 2023-07-26 16:13:24.000000 abpandas-0.0.2/abpandas/agent.py
+-rw-rw-rw-   0        0        0     6698 2023-07-26 18:33:17.000000 abpandas-0.0.2/abpandas/model.py
+-rw-rw-rw-   0        0        0     1178 2023-07-26 15:50:02.000000 abpandas-0.0.2/abpandas/space.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:10:34.892095 abpandas-0.0.2/abpandas.egg-info/
+-rw-rw-rw-   0        0        0      894 2023-07-27 08:10:31.000000 abpandas-0.0.2/abpandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-07-27 08:10:34.000000 abpandas-0.0.2/abpandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 08:10:31.000000 abpandas-0.0.2/abpandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-27 08:10:32.000000 abpandas-0.0.2/abpandas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 08:10:33.000000 abpandas-0.0.2/abpandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 08:10:34.916094 abpandas-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1466 2023-07-27 08:09:34.000000 abpandas-0.0.2/setup.py
```

### Comparing `abpandas-0.0.1/PKG-INFO` & `abpandas-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: abpandas
-Version: 0.0.1
+Version: 0.0.2
 Summary: Agent Based Pandas tool (ABPandas)
 Author: Yahya Gamal
 Author-email: <abpandas.yg@outlook.com>
-License: UNKNOWN
 Keywords: python,Agent Based Model,Spatial,Pandas
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 
 An Agent Based Modelling (ABM) package that can generate grid spatial shape files or work with predefined shape files.
 The package focuses on simplicity by assigning Agents to spatial Polygons instead of assigning x and y locations for each agents.
 This makes it useful in situations where granual movement of agents in space is not necessary (e.g. residentail location models)
-
```

### Comparing `abpandas-0.0.1/abpandas/agent.py` & `abpandas-0.0.2/abpandas/agent.py`

 * *Files identical despite different names*

### Comparing `abpandas-0.0.1/abpandas/model.py` & `abpandas-0.0.2/abpandas/model.py`

 * *Files identical despite different names*

### Comparing `abpandas-0.0.1/abpandas/space.py` & `abpandas-0.0.2/abpandas/space.py`

 * *Files identical despite different names*

### Comparing `abpandas-0.0.1/abpandas.egg-info/PKG-INFO` & `abpandas-0.0.2/abpandas.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: abpandas
-Version: 0.0.1
+Version: 0.0.2
 Summary: Agent Based Pandas tool (ABPandas)
 Author: Yahya Gamal
 Author-email: <abpandas.yg@outlook.com>
-License: UNKNOWN
 Keywords: python,Agent Based Model,Spatial,Pandas
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 
 An Agent Based Modelling (ABM) package that can generate grid spatial shape files or work with predefined shape files.
 The package focuses on simplicity by assigning Agents to spatial Polygons instead of assigning x and y locations for each agents.
 This makes it useful in situations where granual movement of agents in space is not necessary (e.g. residentail location models)
-
```

### Comparing `abpandas-0.0.1/setup.py` & `abpandas-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'Agent Based Pandas tool (ABPandas)'
 LONG_DESCRIPTION = 'An Agent Based Modelling (ABM) package that can generate grid spatial shape files or work with predefined shape files.\nThe package focuses on simplicity by assigning Agents to spatial Polygons instead of assigning x and y locations for each agents.\nThis makes it useful in situations where granual movement of agents in space is not necessary (e.g. residentail location models)'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="abpandas",
```

