# Comparing `tmp/tdvisu-1.1.8.tar.gz` & `tmp/tdvisu-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdvisu-1.1.8.tar", last modified: Tue May  4 18:30:32 2021, max compression
+gzip compressed data, was "tdvisu-1.1.9.tar", last modified: Thu Jul 27 17:08:59 2023, max compression
```

## Comparing `tdvisu-1.1.8.tar` & `tdvisu-1.1.9.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:30:32.035356 tdvisu-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    20425 2021-05-04 18:30:32.035356 tdvisu-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7998 2021-05-04 18:30:22.000000 tdvisu-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-04 18:30:32.035356 tdvisu-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2021-05-04 18:30:22.000000 tdvisu-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:30:32.031356 tdvisu-1.1.8/tdvisu/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-05-04 18:30:22.000000 tdvisu-1.1.8/tdvisu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22701 2021-05-04 18:30:22.000000 tdvisu-1.1.8/tdvisu/construct_dpdb_visu.py
--rw-r--r--   0 runner    (1001) docker     (121)     9361 2021-05-04 18:30:22.000000 tdvisu-1.1.8/tdvisu/dijkstra.py
--rw-r--r--   0 runner    (1001) docker     (121)     5276 2021-05-04 18:30:22.000000 tdvisu-1.1.8/tdvisu/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    12600 2021-05-04 18:30:22.000000 tdvisu-1.1.8/tdvisu/svgjoin.py
--rw-r--r--   0 runner    (1001) docker     (121)    15534 2021-05-04 18:30:22.000000 tdvisu-1.1.8/tdvisu/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)      193 2021-05-04 18:30:22.000000 tdvisu-1.1.8/tdvisu/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    29090 2021-05-04 18:30:22.000000 tdvisu-1.1.8/tdvisu/visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)     4185 2021-05-04 18:30:22.000000 tdvisu-1.1.8/tdvisu/visualization_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:30:32.035356 tdvisu-1.1.8/tdvisu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    20425 2021-05-04 18:30:31.000000 tdvisu-1.1.8/tdvisu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      549 2021-05-04 18:30:31.000000 tdvisu-1.1.8/tdvisu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 18:30:31.000000 tdvisu-1.1.8/tdvisu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-05-04 18:30:31.000000 tdvisu-1.1.8/tdvisu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-05-04 18:30:31.000000 tdvisu-1.1.8/tdvisu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:30:32.035356 tdvisu-1.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2980 2021-05-04 18:30:22.000000 tdvisu-1.1.8/test/test_bag_creation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6814 2021-05-04 18:30:22.000000 tdvisu-1.1.8/test/test_construct_dpdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     3683 2021-05-04 18:30:22.000000 tdvisu-1.1.8/test/test_dijkstra.py
--rw-r--r--   0 runner    (1001) docker     (121)     5851 2021-05-04 18:30:22.000000 tdvisu-1.1.8/test/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     9172 2021-05-04 18:30:22.000000 tdvisu-1.1.8/test/test_svgjoin.py
--rw-r--r--   0 runner    (1001) docker     (121)     8313 2021-05-04 18:30:22.000000 tdvisu-1.1.8/test/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2021-05-04 18:30:22.000000 tdvisu-1.1.8/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3458 2021-05-04 18:30:22.000000 tdvisu-1.1.8/test/test_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:08:59.518997 tdvisu-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 17:08:47.000000 tdvisu-1.1.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-07-27 17:08:47.000000 tdvisu-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20731 2023-07-27 17:08:59.518997 tdvisu-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-07-27 17:08:47.000000 tdvisu-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:08:59.518997 tdvisu-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-27 17:08:47.000000 tdvisu-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:08:59.514997 tdvisu-1.1.9/tdvisu/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-27 17:08:47.000000 tdvisu-1.1.9/tdvisu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-07-27 17:08:47.000000 tdvisu-1.1.9/tdvisu/construct_dpdb_visu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-07-27 17:08:47.000000 tdvisu-1.1.9/tdvisu/dijkstra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-27 17:08:47.000000 tdvisu-1.1.9/tdvisu/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-07-27 17:08:47.000000 tdvisu-1.1.9/tdvisu/svgjoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-27 17:08:47.000000 tdvisu-1.1.9/tdvisu/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-27 17:08:47.000000 tdvisu-1.1.9/tdvisu/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29090 2023-07-27 17:08:47.000000 tdvisu-1.1.9/tdvisu/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-27 17:08:47.000000 tdvisu-1.1.9/tdvisu/visualization_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:08:59.514997 tdvisu-1.1.9/tdvisu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20731 2023-07-27 17:08:59.000000 tdvisu-1.1.9/tdvisu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-27 17:08:59.000000 tdvisu-1.1.9/tdvisu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:08:59.000000 tdvisu-1.1.9/tdvisu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 17:08:59.000000 tdvisu-1.1.9/tdvisu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 17:08:59.000000 tdvisu-1.1.9/tdvisu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:08:59.518997 tdvisu-1.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-27 17:08:47.000000 tdvisu-1.1.9/test/test_bag_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-27 17:08:47.000000 tdvisu-1.1.9/test/test_construct_dpdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-27 17:08:47.000000 tdvisu-1.1.9/test/test_dijkstra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-27 17:08:47.000000 tdvisu-1.1.9/test/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-07-27 17:08:47.000000 tdvisu-1.1.9/test/test_svgjoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-27 17:08:47.000000 tdvisu-1.1.9/test/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-27 17:08:47.000000 tdvisu-1.1.9/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-27 17:08:47.000000 tdvisu-1.1.9/test/test_visualization.py
```

### Comparing `tdvisu-1.1.8/PKG-INFO` & `tdvisu-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdvisu
-Version: 1.1.8
+Version: 1.1.9
 Summary: Visualizing Dynamic Programming on Tree Decompositions.
 Home-page: https://github.com/VaeterchenFrost/tdvisu
 Author: Martin Röbke
 Author-email: martin.roebke@mailbox.tu-dresden.de
 License: GPLv3
 Description: # TdVisu
         ![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)
@@ -196,15 +196,15 @@
         - On the GitHub page go to: Release, **[Draft a new release](https://github.com/VaeterchenFrost/tdvisu/releases/new )** 
         - Enter v'YOUR VERSION NUMBER' as the tag.
         - Add a **Release Title** (could be just the version)
         - Add some description (like in the CHANGELOG.md)
         - Click on **Publish release** on the bottom
         
         ## Should automatically release to [PyPI](https://pypi.org/project/tdvisu/ )
-        - For details see: [Upload Python Package](https://github.com/VaeterchenFrost/tdvisu/blob/master/.github/workflows/python-app.yml )
+        - For details see: [Upload Python Package](https://github.com/VaeterchenFrost/tdvisu/blob/master/.github/workflows/python-publish.yml )
         
         **Now you are set for the new release :tada:**
         
         ----------
         
         
         # Changelog
@@ -213,14 +213,23 @@
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/ ), and this
         project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html ).
         
         ## [Unreleased]
         - No unreleased changes yet.
         
+        ## [1.1.9] - 2023-07-27
+        
+        ### Added
+        - `python-benedict[xml]` to dependencies
+        ### Changed
+        - Updated requirements.txt
+        - Updated stable-requirements.txt
+        
+        
         ## [1.1.8] - 2021-05-04
         
         ### Changed
         - Updated pyyaml from 5.3.1 to 5.4 [#33]
         - Updated py from 1.9.0 to 1.10.0 [#35]
         - Fixed python-app.yml [#34]
         
@@ -402,15 +411,16 @@
         
         [@VaeterchenFrost]: https://github.com/VaeterchenFrost
         [PyPI]: https://pypi.org/project/tdvisu/
         [mypy]: https://github.com/python/mypy
         [DIRECTORY]: https://github.com/VaeterchenFrost/tdvisu/blob/master/DIRECTORY.md
         [Codecov]: https://codecov.io/gh/VaeterchenFrost/tdvisu
         
-        [Unreleased]: https://github.com/VaeterchenFrost/tdvisu/compare/v1.1.8...master
+        [Unreleased]: https://github.com/VaeterchenFrost/tdvisu/compare/v1.1.9...master
+        [1.1.8]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.9
         [1.1.8]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.8
         [1.1.7]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.7
         [1.1.6]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.6
         [1.1.5]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.5
         [1.1.4]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.4
         [1.1.3]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.3
         [1.1.2]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.2
```

### Comparing `tdvisu-1.1.8/README.md` & `tdvisu-1.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -188,13 +188,13 @@
 - On the GitHub page go to: Release, **[Draft a new release](https://github.com/VaeterchenFrost/tdvisu/releases/new )** 
 - Enter v'YOUR VERSION NUMBER' as the tag.
 - Add a **Release Title** (could be just the version)
 - Add some description (like in the CHANGELOG.md)
 - Click on **Publish release** on the bottom
 
 ## Should automatically release to [PyPI](https://pypi.org/project/tdvisu/ )
-- For details see: [Upload Python Package](https://github.com/VaeterchenFrost/tdvisu/blob/master/.github/workflows/python-app.yml )
+- For details see: [Upload Python Package](https://github.com/VaeterchenFrost/tdvisu/blob/master/.github/workflows/python-publish.yml )
 
 **Now you are set for the new release :tada:**
 
 ----------
```

### Comparing `tdvisu-1.1.8/setup.py` & `tdvisu-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,11 +61,11 @@
       long_description_content_type='text/markdown',
       url="https://github.com/VaeterchenFrost/tdvisu",
       author="Martin Röbke",
       author_email="martin.roebke@mailbox.tu-dresden.de",
       license='GPLv3',
       packages=['tdvisu'],
       platforms='any',
-      install_requires=['graphviz', 'psycopg2', 'python-benedict', 'PyYAML'],
+      install_requires=['graphviz', 'psycopg2', 'python-benedict', 'python-benedict[xml]', 'PyYAML'],
       extras_require={'test': tests_require},
       classifiers=classifiers,
       keywords='graph visualization dynamic-programming msol-solver')
```

### Comparing `tdvisu-1.1.8/tdvisu/construct_dpdb_visu.py` & `tdvisu-1.1.9/tdvisu/construct_dpdb_visu.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/tdvisu/dijkstra.py` & `tdvisu-1.1.9/tdvisu/dijkstra.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/tdvisu/reader.py` & `tdvisu-1.1.9/tdvisu/reader.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/tdvisu/svgjoin.py` & `tdvisu-1.1.9/tdvisu/svgjoin.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/tdvisu/utilities.py` & `tdvisu-1.1.9/tdvisu/utilities.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/tdvisu/visualization.py` & `tdvisu-1.1.9/tdvisu/visualization.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/tdvisu/visualization_data.py` & `tdvisu-1.1.9/tdvisu/visualization_data.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/tdvisu.egg-info/PKG-INFO` & `tdvisu-1.1.9/tdvisu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdvisu
-Version: 1.1.8
+Version: 1.1.9
 Summary: Visualizing Dynamic Programming on Tree Decompositions.
 Home-page: https://github.com/VaeterchenFrost/tdvisu
 Author: Martin Röbke
 Author-email: martin.roebke@mailbox.tu-dresden.de
 License: GPLv3
 Description: # TdVisu
         ![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)
@@ -196,15 +196,15 @@
         - On the GitHub page go to: Release, **[Draft a new release](https://github.com/VaeterchenFrost/tdvisu/releases/new )** 
         - Enter v'YOUR VERSION NUMBER' as the tag.
         - Add a **Release Title** (could be just the version)
         - Add some description (like in the CHANGELOG.md)
         - Click on **Publish release** on the bottom
         
         ## Should automatically release to [PyPI](https://pypi.org/project/tdvisu/ )
-        - For details see: [Upload Python Package](https://github.com/VaeterchenFrost/tdvisu/blob/master/.github/workflows/python-app.yml )
+        - For details see: [Upload Python Package](https://github.com/VaeterchenFrost/tdvisu/blob/master/.github/workflows/python-publish.yml )
         
         **Now you are set for the new release :tada:**
         
         ----------
         
         
         # Changelog
@@ -213,14 +213,23 @@
         
         The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/ ), and this
         project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html ).
         
         ## [Unreleased]
         - No unreleased changes yet.
         
+        ## [1.1.9] - 2023-07-27
+        
+        ### Added
+        - `python-benedict[xml]` to dependencies
+        ### Changed
+        - Updated requirements.txt
+        - Updated stable-requirements.txt
+        
+        
         ## [1.1.8] - 2021-05-04
         
         ### Changed
         - Updated pyyaml from 5.3.1 to 5.4 [#33]
         - Updated py from 1.9.0 to 1.10.0 [#35]
         - Fixed python-app.yml [#34]
         
@@ -402,15 +411,16 @@
         
         [@VaeterchenFrost]: https://github.com/VaeterchenFrost
         [PyPI]: https://pypi.org/project/tdvisu/
         [mypy]: https://github.com/python/mypy
         [DIRECTORY]: https://github.com/VaeterchenFrost/tdvisu/blob/master/DIRECTORY.md
         [Codecov]: https://codecov.io/gh/VaeterchenFrost/tdvisu
         
-        [Unreleased]: https://github.com/VaeterchenFrost/tdvisu/compare/v1.1.8...master
+        [Unreleased]: https://github.com/VaeterchenFrost/tdvisu/compare/v1.1.9...master
+        [1.1.8]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.9
         [1.1.8]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.8
         [1.1.7]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.7
         [1.1.6]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.6
         [1.1.5]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.5
         [1.1.4]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.4
         [1.1.3]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.3
         [1.1.2]: https://github.com/VaeterchenFrost/tdvisu/releases/tag/v1.1.2
```

### Comparing `tdvisu-1.1.8/tdvisu.egg-info/SOURCES.txt` & `tdvisu-1.1.9/tdvisu.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+COPYING
+LICENSE
 README.md
 setup.py
 tdvisu/__init__.py
 tdvisu/construct_dpdb_visu.py
 tdvisu/dijkstra.py
 tdvisu/reader.py
 tdvisu/svgjoin.py
```

### Comparing `tdvisu-1.1.8/test/test_bag_creation.py` & `tdvisu-1.1.9/test/test_bag_creation.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/test/test_construct_dpdb.py` & `tdvisu-1.1.9/test/test_construct_dpdb.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/test/test_dijkstra.py` & `tdvisu-1.1.9/test/test_dijkstra.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/test/test_reader.py` & `tdvisu-1.1.9/test/test_reader.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/test/test_svgjoin.py` & `tdvisu-1.1.9/test/test_svgjoin.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/test/test_utilities.py` & `tdvisu-1.1.9/test/test_utilities.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/test/test_version.py` & `tdvisu-1.1.9/test/test_version.py`

 * *Files identical despite different names*

### Comparing `tdvisu-1.1.8/test/test_visualization.py` & `tdvisu-1.1.9/test/test_visualization.py`

 * *Files identical despite different names*

