# Comparing `tmp/gyoza-0.0.6.tar.gz` & `tmp/gyoza-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyoza-0.0.6.tar", last modified: Thu Jul 27 14:26:36 2023, max compression
+gzip compressed data, was "gyoza-0.0.7.tar", last modified: Thu Jul 27 14:52:30 2023, max compression
```

## Comparing `gyoza-0.0.6.tar` & `gyoza-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:26:36.483126 gyoza-0.0.6/
--rwxrwxrwx   0 timdick    (501) staff       (20)     1091 2023-06-02 09:45:10.000000 gyoza-0.0.6/LICENSE
--rw-r--r--   0 timdick    (501) staff       (20)     3007 2023-07-27 14:26:36.482730 gyoza-0.0.6/PKG-INFO
--rwxr-xr-x   0 timdick    (501) staff       (20)     2620 2023-07-27 14:15:49.000000 gyoza-0.0.6/README.md
--rwxr-xr-x   0 timdick    (501) staff       (20)      797 2023-07-27 14:23:46.000000 gyoza-0.0.6/pyproject.toml
--rw-r--r--   0 timdick    (501) staff       (20)       38 2023-07-27 14:26:36.483271 gyoza-0.0.6/setup.cfg
--rwxrwxrwx   0 timdick    (501) staff       (20)      173 2023-06-15 09:02:13.000000 gyoza-0.0.6/setup.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:26:36.474596 gyoza-0.0.6/src/
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:26:36.476491 gyoza-0.0.6/src/gyoza/
--rw-r--r--   0 timdick    (501) staff       (20)        0 2023-06-07 09:58:20.000000 gyoza-0.0.6/src/gyoza/__init__.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:26:36.480899 gyoza-0.0.6/src/gyoza/modelling/
--rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 11:33:16.000000 gyoza-0.0.6/src/gyoza/modelling/__init__.py
--rw-r--r--   0 timdick    (501) staff       (20)    13578 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/modelling/data_iterators.py
--rwxr-xr-x   0 timdick    (501) staff       (20)    42532 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/modelling/flow_layers.py
--rw-r--r--   0 timdick    (501) staff       (20)    12575 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/modelling/losses.py
--rw-r--r--   0 timdick    (501) staff       (20)     9161 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/modelling/masks.py
--rw-r--r--   0 timdick    (501) staff       (20)     3173 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/modelling/standard_layers.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:26:36.482136 gyoza-0.0.6/src/gyoza/utilities/
--rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 12:24:09.000000 gyoza-0.0.6/src/gyoza/utilities/__init__.py
--rwxr-xr-x   0 timdick    (501) staff       (20)    11781 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/utilities/math.py
--rw-r--r--   0 timdick    (501) staff       (20)     3987 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/utilities/tensors.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:26:36.478001 gyoza-0.0.6/src/gyoza.egg-info/
--rwxrwxrwx   0 timdick    (501) staff       (20)     3007 2023-07-27 14:26:36.000000 gyoza-0.0.6/src/gyoza.egg-info/PKG-INFO
--rwxrwxrwx   0 timdick    (501) staff       (20)      521 2023-07-27 14:26:36.000000 gyoza-0.0.6/src/gyoza.egg-info/SOURCES.txt
--rwxrwxrwx   0 timdick    (501) staff       (20)        1 2023-07-27 14:26:36.000000 gyoza-0.0.6/src/gyoza.egg-info/dependency_links.txt
--rwxrwxrwx   0 timdick    (501) staff       (20)       98 2023-07-27 14:26:36.000000 gyoza-0.0.6/src/gyoza.egg-info/requires.txt
--rwxrwxrwx   0 timdick    (501) staff       (20)        6 2023-07-27 14:26:36.000000 gyoza-0.0.6/src/gyoza.egg-info/top_level.txt
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:52:30.326175 gyoza-0.0.7/
+-rwxrwxrwx   0 timdick    (501) staff       (20)     1091 2023-06-02 09:45:10.000000 gyoza-0.0.7/LICENSE
+-rw-r--r--   0 timdick    (501) staff       (20)     2995 2023-07-27 14:52:30.325736 gyoza-0.0.7/PKG-INFO
+-rwxr-xr-x   0 timdick    (501) staff       (20)     2608 2023-07-27 14:35:24.000000 gyoza-0.0.7/README.md
+-rwxr-xr-x   0 timdick    (501) staff       (20)      797 2023-07-27 14:50:16.000000 gyoza-0.0.7/pyproject.toml
+-rw-r--r--   0 timdick    (501) staff       (20)       38 2023-07-27 14:52:30.326308 gyoza-0.0.7/setup.cfg
+-rwxrwxrwx   0 timdick    (501) staff       (20)      173 2023-06-15 09:02:13.000000 gyoza-0.0.7/setup.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:52:30.314569 gyoza-0.0.7/src/
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:52:30.316404 gyoza-0.0.7/src/gyoza/
+-rw-r--r--   0 timdick    (501) staff       (20)        0 2023-06-07 09:58:20.000000 gyoza-0.0.7/src/gyoza/__init__.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:52:30.322547 gyoza-0.0.7/src/gyoza/modelling/
+-rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 11:33:16.000000 gyoza-0.0.7/src/gyoza/modelling/__init__.py
+-rw-r--r--   0 timdick    (501) staff       (20)    13578 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/modelling/data_iterators.py
+-rwxr-xr-x   0 timdick    (501) staff       (20)    42532 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/modelling/flow_layers.py
+-rw-r--r--   0 timdick    (501) staff       (20)    12575 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/modelling/losses.py
+-rw-r--r--   0 timdick    (501) staff       (20)     9161 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/modelling/masks.py
+-rw-r--r--   0 timdick    (501) staff       (20)     3173 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/modelling/standard_layers.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:52:30.324920 gyoza-0.0.7/src/gyoza/utilities/
+-rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 12:24:09.000000 gyoza-0.0.7/src/gyoza/utilities/__init__.py
+-rwxr-xr-x   0 timdick    (501) staff       (20)    11781 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/utilities/math.py
+-rw-r--r--   0 timdick    (501) staff       (20)     3987 2023-07-27 14:11:22.000000 gyoza-0.0.7/src/gyoza/utilities/tensors.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:52:30.317880 gyoza-0.0.7/src/gyoza.egg-info/
+-rwxrwxrwx   0 timdick    (501) staff       (20)     2995 2023-07-27 14:52:30.000000 gyoza-0.0.7/src/gyoza.egg-info/PKG-INFO
+-rwxrwxrwx   0 timdick    (501) staff       (20)      521 2023-07-27 14:52:30.000000 gyoza-0.0.7/src/gyoza.egg-info/SOURCES.txt
+-rwxrwxrwx   0 timdick    (501) staff       (20)        1 2023-07-27 14:52:30.000000 gyoza-0.0.7/src/gyoza.egg-info/dependency_links.txt
+-rwxrwxrwx   0 timdick    (501) staff       (20)       98 2023-07-27 14:52:30.000000 gyoza-0.0.7/src/gyoza.egg-info/requires.txt
+-rwxrwxrwx   0 timdick    (501) staff       (20)        6 2023-07-27 14:52:30.000000 gyoza-0.0.7/src/gyoza.egg-info/top_level.txt
```

### Comparing `gyoza-0.0.6/LICENSE` & `gyoza-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.6/PKG-INFO` & `gyoza-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyoza
-Version: 0.0.6
+Version: 0.0.7
 Author-email: Tim Dick <timdi@icloud.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -17,15 +17,15 @@
 ## Download
 As this package is distributed via [PyPI](https://pypi.org/project/gyoza/) it can be installed using:
 ```
 pip install gyoza
 ```
 
 ## Documentation
-Detailed documentation can be found on the companion website of [read-the-docs](https://gyoza.readthedocs.io/en/latest/modules.html)
+Detailed documentation can be found on the companion website of [read-the-docs](https://gyoza.readthedocs.io/en/latest/)
 
 ## Development
 Developers can access the package via [GitHub](https://github.com/TimHenry1995/gyoza)
 
 ## Tutorial
 Tutorials can be found in the [tutorials](https://github.com/TimHenry1995/gyoza/tree/main/tutorials) folder of this repository.
```

### Comparing `gyoza-0.0.6/README.md` & `gyoza-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Download
 As this package is distributed via [PyPI](https://pypi.org/project/gyoza/) it can be installed using:
 ```
 pip install gyoza
 ```
 
 ## Documentation
-Detailed documentation can be found on the companion website of [read-the-docs](https://gyoza.readthedocs.io/en/latest/modules.html)
+Detailed documentation can be found on the companion website of [read-the-docs](https://gyoza.readthedocs.io/en/latest/)
 
 ## Development
 Developers can access the package via [GitHub](https://github.com/TimHenry1995/gyoza)
 
 ## Tutorial
 Tutorials can be found in the [tutorials](https://github.com/TimHenry1995/gyoza/tree/main/tutorials) folder of this repository.
```

### Comparing `gyoza-0.0.6/pyproject.toml` & `gyoza-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "gyoza"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Tim Dick", email="timdi@icloud.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `gyoza-0.0.6/src/gyoza/modelling/data_iterators.py` & `gyoza-0.0.7/src/gyoza/modelling/data_iterators.py`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.6/src/gyoza/modelling/flow_layers.py` & `gyoza-0.0.7/src/gyoza/modelling/flow_layers.py`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.6/src/gyoza/modelling/losses.py` & `gyoza-0.0.7/src/gyoza/modelling/losses.py`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.6/src/gyoza/modelling/masks.py` & `gyoza-0.0.7/src/gyoza/modelling/masks.py`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.6/src/gyoza/modelling/standard_layers.py` & `gyoza-0.0.7/src/gyoza/modelling/standard_layers.py`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.6/src/gyoza/utilities/math.py` & `gyoza-0.0.7/src/gyoza/utilities/math.py`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.6/src/gyoza/utilities/tensors.py` & `gyoza-0.0.7/src/gyoza/utilities/tensors.py`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.6/src/gyoza.egg-info/PKG-INFO` & `gyoza-0.0.7/src/gyoza.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyoza
-Version: 0.0.6
+Version: 0.0.7
 Author-email: Tim Dick <timdi@icloud.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -17,15 +17,15 @@
 ## Download
 As this package is distributed via [PyPI](https://pypi.org/project/gyoza/) it can be installed using:
 ```
 pip install gyoza
 ```
 
 ## Documentation
-Detailed documentation can be found on the companion website of [read-the-docs](https://gyoza.readthedocs.io/en/latest/modules.html)
+Detailed documentation can be found on the companion website of [read-the-docs](https://gyoza.readthedocs.io/en/latest/)
 
 ## Development
 Developers can access the package via [GitHub](https://github.com/TimHenry1995/gyoza)
 
 ## Tutorial
 Tutorials can be found in the [tutorials](https://github.com/TimHenry1995/gyoza/tree/main/tutorials) folder of this repository.
```

### Comparing `gyoza-0.0.6/src/gyoza.egg-info/SOURCES.txt` & `gyoza-0.0.7/src/gyoza.egg-info/SOURCES.txt`

 * *Files identical despite different names*

