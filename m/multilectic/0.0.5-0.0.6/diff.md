# Comparing `tmp/multilectic-0.0.5.tar.gz` & `tmp/multilectic-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multilectic-0.0.5.tar", last modified: Thu Jul 27 01:03:11 2023, max compression
+gzip compressed data, was "multilectic-0.0.6.tar", last modified: Thu Jul 27 11:43:01 2023, max compression
```

## Comparing `multilectic-0.0.5.tar` & `multilectic-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-27 01:03:11.908185 multilectic-0.0.5/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2023-07-24 11:57:34.000000 multilectic-0.0.5/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      615 2023-07-27 01:03:11.908185 multilectic-0.0.5/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       67 2023-07-26 18:58:44.000000 multilectic-0.0.5/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      629 2023-07-27 01:01:40.000000 multilectic-0.0.5/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-27 01:03:11.908185 multilectic-0.0.5/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-27 01:03:11.908185 multilectic-0.0.5/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-27 01:03:11.908185 multilectic-0.0.5/src/multilectic/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      253 2023-07-26 18:58:44.000000 multilectic-0.0.5/src/multilectic/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2023-07-27 01:00:48.000000 multilectic-0.0.5/src/multilectic/positions.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-27 01:03:11.908185 multilectic-0.0.5/src/multilectic.egg-info/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      615 2023-07-27 01:03:11.000000 multilectic-0.0.5/src/multilectic.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      269 2023-07-27 01:03:11.000000 multilectic-0.0.5/src/multilectic.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-27 01:03:11.000000 multilectic-0.0.5/src/multilectic.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       12 2023-07-27 01:03:11.000000 multilectic-0.0.5/src/multilectic.egg-info/top_level.txt
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-27 01:03:11.908185 multilectic-0.0.5/tests/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      261 2023-07-26 18:32:54.000000 multilectic-0.0.5/tests/test_positions.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-27 11:43:01.202950 multilectic-0.0.6/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2023-07-24 11:57:34.000000 multilectic-0.0.6/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      615 2023-07-27 11:43:01.202950 multilectic-0.0.6/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       67 2023-07-26 18:58:44.000000 multilectic-0.0.6/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      629 2023-07-27 11:41:17.000000 multilectic-0.0.6/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-27 11:43:01.202950 multilectic-0.0.6/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-27 11:43:01.198950 multilectic-0.0.6/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-27 11:43:01.202950 multilectic-0.0.6/src/multilectic/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      253 2023-07-26 18:58:44.000000 multilectic-0.0.6/src/multilectic/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1071 2023-07-27 11:41:17.000000 multilectic-0.0.6/src/multilectic/positions.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-27 11:43:01.202950 multilectic-0.0.6/src/multilectic.egg-info/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      615 2023-07-27 11:43:01.000000 multilectic-0.0.6/src/multilectic.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      269 2023-07-27 11:43:01.000000 multilectic-0.0.6/src/multilectic.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-27 11:43:01.000000 multilectic-0.0.6/src/multilectic.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       12 2023-07-27 11:43:01.000000 multilectic-0.0.6/src/multilectic.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-27 11:43:01.202950 multilectic-0.0.6/tests/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      261 2023-07-26 18:32:54.000000 multilectic-0.0.6/tests/test_positions.py
```

### Comparing `multilectic-0.0.5/LICENSE` & `multilectic-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `multilectic-0.0.5/PKG-INFO` & `multilectic-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilectic
-Version: 0.0.5
+Version: 0.0.6
 Summary: The multilogue philosophy with more than two 'truths'
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilectic/multilectic
 Project-URL: Bug Tracker, https://github.com/multilectic/multilectic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multilectic-0.0.5/pyproject.toml` & `multilectic-0.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "multilectic"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "The multilogue philosophy with more than two 'truths'"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `multilectic-0.0.5/src/multilectic/positions.py` & `multilectic-0.0.6/src/multilectic/positions.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 This source code is licensed under the license found in the
 LICENSE file in the root directory of this source tree.
 """
 from typing import List, Dict
 
 
 class Position(object):
-    """ A position in a multilogue discussion. """
+    """ A current position in a multilogue discussion. """
 
     thesis: str                 = ""
     antithesis: str             = ""
     facts: List[str]            = []
     presuppositions: List[str]  = []
-
-    conversation: List[Dict]    = []  # The course of conversation, sequence of statements.
+    assumptions: List[str]      = []
 
     def __init__(self, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
             super(Position, self).__init__()
 
     def __call__(self, *args, **kwargs):
@@ -29,9 +28,10 @@
         return self
 
     def __repr__(self):
         return f"""Position   
             Thesis:  {self.thesis}, 
             Antithesis: {self.thesis},
             Facts: {self.facts},
-            Presuppositions: {self.presuppositions}
+            Presuppositions: {self.presuppositions},
+            Assumptions: {self.assumptions}
             """
```

### Comparing `multilectic-0.0.5/src/multilectic.egg-info/PKG-INFO` & `multilectic-0.0.6/src/multilectic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilectic
-Version: 0.0.5
+Version: 0.0.6
 Summary: The multilogue philosophy with more than two 'truths'
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilectic/multilectic
 Project-URL: Bug Tracker, https://github.com/multilectic/multilectic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

