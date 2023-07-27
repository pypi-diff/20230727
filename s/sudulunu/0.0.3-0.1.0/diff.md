# Comparing `tmp/sudulunu-0.0.3.tar.gz` & `tmp/sudulunu-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sudulunu-0.0.3.tar", last modified: Mon Nov 28 04:01:32 2022, max compression
+gzip compressed data, was "sudulunu-0.1.0.tar", last modified: Thu Jul 27 04:48:54 2023, max compression
```

## Comparing `sudulunu-0.0.3.tar` & `sudulunu-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)        0 2022-11-28 04:01:32.994517 sudulunu-0.0.3/
--rw-r--r--   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)     1070 2022-11-28 02:40:35.000000 sudulunu-0.0.3/LICENSE
--rw-r--r--   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)      742 2022-11-28 04:01:32.994051 sudulunu-0.0.3/PKG-INFO
--rw-r--r--   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)      172 2022-11-28 02:57:07.000000 sudulunu-0.0.3/README.md
--rw-r--r--   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)      598 2022-11-28 04:01:24.000000 sudulunu-0.0.3/pyproject.toml
--rw-r--r--   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)       38 2022-11-28 04:01:32.994632 sudulunu-0.0.3/setup.cfg
--rw-r--r--   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)      802 2022-11-28 04:00:35.000000 sudulunu-0.0.3/setup.py
-drwxr-xr-x   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)        0 2022-11-28 04:01:32.988967 sudulunu-0.0.3/src/
-drwxr-xr-x   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)        0 2022-11-28 04:01:32.991262 sudulunu-0.0.3/src/sudulunu/
--rw-r--r--   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)        0 2022-11-28 02:44:25.000000 sudulunu-0.0.3/src/sudulunu/__init__.py
--rw-r--r--   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)     2446 2022-11-28 04:00:25.000000 sudulunu-0.0.3/src/sudulunu/helpers.py
-drwxr-xr-x   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)        0 2022-11-28 04:01:32.993454 sudulunu-0.0.3/src/sudulunu.egg-info/
--rw-r--r--   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)      742 2022-11-28 04:01:32.000000 sudulunu-0.0.3/src/sudulunu.egg-info/PKG-INFO
--rw-r--r--   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)      234 2022-11-28 04:01:32.000000 sudulunu-0.0.3/src/sudulunu.egg-info/SOURCES.txt
--rw-r--r--   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)        1 2022-11-28 04:01:32.000000 sudulunu-0.0.3/src/sudulunu.egg-info/dependency_links.txt
--rw-r--r--   0 josh_nicholas (2085374771) GNM\WG COM Australia Operations (1987631478)        9 2022-11-28 04:01:32.000000 sudulunu-0.0.3/src/sudulunu.egg-info/top_level.txt
+drwxr-xr-x   0 josh_nicholas   (503) staff       (20)        0 2023-07-27 04:48:54.865392 sudulunu-0.1.0/
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)     1070 2023-07-27 04:33:12.000000 sudulunu-0.1.0/LICENSE
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)      741 2023-07-27 04:48:54.865202 sudulunu-0.1.0/PKG-INFO
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)      172 2023-07-27 04:33:12.000000 sudulunu-0.1.0/README.md
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)      621 2023-07-27 04:47:23.000000 sudulunu-0.1.0/pyproject.toml
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)       38 2023-07-27 04:48:54.865457 sudulunu-0.1.0/setup.cfg
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)      802 2023-07-27 04:47:39.000000 sudulunu-0.1.0/setup.py
+drwxr-xr-x   0 josh_nicholas   (503) staff       (20)        0 2023-07-27 04:48:54.861766 sudulunu-0.1.0/src/
+drwxr-xr-x   0 josh_nicholas   (503) staff       (20)        0 2023-07-27 04:48:54.863471 sudulunu-0.1.0/src/sudulunu/
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)        0 2023-07-27 04:33:12.000000 sudulunu-0.1.0/src/sudulunu/__init__.py
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)     2826 2023-07-27 04:48:27.000000 sudulunu-0.1.0/src/sudulunu/helpers.py
+drwxr-xr-x   0 josh_nicholas   (503) staff       (20)        0 2023-07-27 04:48:54.864522 sudulunu-0.1.0/src/sudulunu.egg-info/
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)      741 2023-07-27 04:48:54.000000 sudulunu-0.1.0/src/sudulunu.egg-info/PKG-INFO
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)      256 2023-07-27 04:48:54.000000 sudulunu-0.1.0/src/sudulunu.egg-info/SOURCES.txt
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)        1 2023-07-27 04:48:54.000000 sudulunu-0.1.0/src/sudulunu.egg-info/dependency_links.txt
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)        9 2023-07-27 04:48:54.000000 sudulunu-0.1.0/src/sudulunu.egg-info/top_level.txt
+drwxr-xr-x   0 josh_nicholas   (503) staff       (20)        0 2023-07-27 04:48:54.864922 sudulunu-0.1.0/tests/
+-rw-r--r--   0 josh_nicholas   (503) staff       (20)      211 2023-07-27 04:33:12.000000 sudulunu-0.1.0/tests/test_helpers.py
```

### Comparing `sudulunu-0.0.3/LICENSE` & `sudulunu-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sudulunu-0.0.3/PKG-INFO` & `sudulunu-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sudulunu
-Version: 0.0.3
+Version: 0.1.0
 Summary: A package with some helper scripts
 Home-page: https://github.com/joshnicholas/sudulunu
 Author: Josh Nicholas
 Author-email: Josh <josh@thambi.li>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/joshnicholas/sudulunu
+Project-URL: Bug Tracker, https://github.com/joshnicholas/sudulunu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sudulunu-0.0.3/pyproject.toml` & `sudulunu-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pyproject.toml
 
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
+requires = ["setuptools>=61.0.0", "wheel", 'pandas', 'fuzzywuzzy']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sudulunu"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="Josh", email="josh@thambi.li" },
 ]
 description = "A package with some helper scripts"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+"Homepage" = "https://github.com/joshnicholas/sudulunu"
+"Bug Tracker" = "https://github.com/joshnicholas/sudulunu"
```

### Comparing `sudulunu-0.0.3/setup.py` & `sudulunu-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "sudulunu",
-    version = "0.0.3",
+    version = "0.1.0",
     author = "Josh Nicholas",
     author_email = "josh@thambi.li",
     description = "A package with some helper scripts",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/joshnicholas/sudulunu",
     project_urls = {
```

### Comparing `sudulunu-0.0.3/src/sudulunu/helpers.py` & `sudulunu-0.1.0/src/sudulunu/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 import os
 import pandas as pd
 import time 
 import random 
 from fuzzywuzzy import fuzz
 from fuzzywuzzy import process
 
+
+def rc(listo, to_remove = False):
+
+    exclude = ['.DS_Store']
+    if to_remove:
+        exclude.extend(to_remove)
+
+    ## Remove strings in list if string contains something from exclude
+    inter = [s for s in listo if not any(x in s for x in exclude)]
+
+    return inter
+
 def pp(frame):
   inter = frame.copy()
 
   print(inter)
   print(inter.columns.tolist())
 
 
@@ -119,8 +131,9 @@
 
 		if len(result) > 0:
 				result = result[0]
 				dicto[word] = result[0]
 
 	return dicto 
 
-
+# python3 -m pip install --user --upgrade setuptools wheel
+# python3 -m pip install --user --upgrade twine
```

### Comparing `sudulunu-0.0.3/src/sudulunu.egg-info/PKG-INFO` & `sudulunu-0.1.0/src/sudulunu.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sudulunu
-Version: 0.0.3
+Version: 0.1.0
 Summary: A package with some helper scripts
 Home-page: https://github.com/joshnicholas/sudulunu
 Author: Josh Nicholas
 Author-email: Josh <josh@thambi.li>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/joshnicholas/sudulunu
+Project-URL: Bug Tracker, https://github.com/joshnicholas/sudulunu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

