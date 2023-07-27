# Comparing `tmp/iRRBS-0.0.6.tar.gz` & `tmp/iRRBS-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iRRBS-0.0.6.tar", last modified: Thu Jul 27 16:34:10 2023, max compression
+gzip compressed data, was "iRRBS-0.0.7.tar", last modified: Thu Jul 27 20:31:17 2023, max compression
```

## Comparing `iRRBS-0.0.6.tar` & `iRRBS-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 16:34:10.650750 iRRBS-0.0.6/
--rw-rw-r--   0 abel      (1000) abel      (1000)      101 2023-07-27 14:53:04.000000 iRRBS-0.0.6/CHANGELOG.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)     1069 2023-07-27 14:53:04.000000 iRRBS-0.0.6/LICENSE
--rw-rw-r--   0 abel      (1000) abel      (1000)       26 2023-07-27 14:53:04.000000 iRRBS-0.0.6/MANIFEST.in
--rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 16:34:10.650750 iRRBS-0.0.6/PKG-INFO
--rw-rw-r--   0 abel      (1000) abel      (1000)      952 2023-07-27 14:53:04.000000 iRRBS-0.0.6/README.md
-drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 16:34:10.650750 iRRBS-0.0.6/iRRBS/
--rw-rw-r--   0 abel      (1000) abel      (1000)       79 2023-07-27 15:15:36.000000 iRRBS-0.0.6/iRRBS/__init__.py
--rw-rw-r--   0 abel      (1000) abel      (1000)     7349 2023-07-27 14:53:04.000000 iRRBS-0.0.6/iRRBS/irrbs_pipeline.py
--rw-rw-r--   0 abel      (1000) abel      (1000)     1306 2023-07-27 15:59:26.000000 iRRBS-0.0.6/iRRBS/run_irrbs.py
--rw-rw-r--   0 abel      (1000) abel      (1000)      458 2023-07-27 14:53:04.000000 iRRBS-0.0.6/iRRBS/suppress.py
-drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 16:34:10.650750 iRRBS-0.0.6/iRRBS.egg-info/
--rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 16:34:10.000000 iRRBS-0.0.6/iRRBS.egg-info/PKG-INFO
--rw-rw-r--   0 abel      (1000) abel      (1000)      285 2023-07-27 16:34:10.000000 iRRBS-0.0.6/iRRBS.egg-info/SOURCES.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)        1 2023-07-27 16:34:10.000000 iRRBS-0.0.6/iRRBS.egg-info/dependency_links.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)       17 2023-07-27 16:34:10.000000 iRRBS-0.0.6/iRRBS.egg-info/requires.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)        6 2023-07-27 16:34:10.000000 iRRBS-0.0.6/iRRBS.egg-info/top_level.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)       79 2023-07-27 16:34:10.650750 iRRBS-0.0.6/setup.cfg
--rw-rw-r--   0 abel      (1000) abel      (1000)      828 2023-07-27 16:30:14.000000 iRRBS-0.0.6/setup.py
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 20:31:17.943039 iRRBS-0.0.7/
+-rw-rw-r--   0 abel      (1000) abel      (1000)      101 2023-07-27 14:53:04.000000 iRRBS-0.0.7/CHANGELOG.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1069 2023-07-27 14:53:04.000000 iRRBS-0.0.7/LICENSE
+-rw-rw-r--   0 abel      (1000) abel      (1000)       26 2023-07-27 14:53:04.000000 iRRBS-0.0.7/MANIFEST.in
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 20:31:17.943039 iRRBS-0.0.7/PKG-INFO
+-rw-rw-r--   0 abel      (1000) abel      (1000)      952 2023-07-27 14:53:04.000000 iRRBS-0.0.7/README.md
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 20:31:17.939039 iRRBS-0.0.7/iRRBS/
+-rw-rw-r--   0 abel      (1000) abel      (1000)      107 2023-07-27 20:30:29.000000 iRRBS-0.0.7/iRRBS/__init__.py
+-rw-rw-r--   0 abel      (1000) abel      (1000)     7349 2023-07-27 14:53:04.000000 iRRBS-0.0.7/iRRBS/irrbs_pipeline.py
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1088 2023-07-27 20:30:37.000000 iRRBS-0.0.7/iRRBS/run_irrbs.py
+-rw-rw-r--   0 abel      (1000) abel      (1000)      458 2023-07-27 14:53:04.000000 iRRBS-0.0.7/iRRBS/suppress.py
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 20:31:17.939039 iRRBS-0.0.7/iRRBS.egg-info/
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 20:31:17.000000 iRRBS-0.0.7/iRRBS.egg-info/PKG-INFO
+-rw-rw-r--   0 abel      (1000) abel      (1000)      285 2023-07-27 20:31:17.000000 iRRBS-0.0.7/iRRBS.egg-info/SOURCES.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)        1 2023-07-27 20:31:17.000000 iRRBS-0.0.7/iRRBS.egg-info/dependency_links.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)       17 2023-07-27 20:31:17.000000 iRRBS-0.0.7/iRRBS.egg-info/requires.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)        6 2023-07-27 20:31:17.000000 iRRBS-0.0.7/iRRBS.egg-info/top_level.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)       79 2023-07-27 20:31:17.943039 iRRBS-0.0.7/setup.cfg
+-rw-rw-r--   0 abel      (1000) abel      (1000)      828 2023-07-27 20:31:13.000000 iRRBS-0.0.7/setup.py
```

### Comparing `iRRBS-0.0.6/LICENSE` & `iRRBS-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.6/PKG-INFO` & `iRRBS-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iRRBS
-Version: 0.0.6
+Version: 0.0.7
 Summary: RRBS tool for deleting artificial cytosins
 Home-page: https://github.com/fothia/iRRBS
 Author: Abel Fothi
 Author-email: fothi.abel@gmail.com
 License: MIT
 Download-URL: https://github.com/fothia/iRRBS/archive/refs/tags/0.0.6.tar.gz
 Platform: UNKNOWN
```

### Comparing `iRRBS-0.0.6/README.md` & `iRRBS-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.6/iRRBS/irrbs_pipeline.py` & `iRRBS-0.0.7/iRRBS/irrbs_pipeline.py`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.6/iRRBS/run_irrbs.py` & `iRRBS-0.0.7/iRRBS/run_irrbs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 import argparse
-import sys
-import os
 from iRRBS.irrbs_pipeline import IPipeline 
 from iRRBS.suppress import Suppress
 
 
-# Get the parent directory of the current script (run_irrbs.py)
-parent_dir = os.path.dirname(os.path.abspath(__file__))
-
-# Add the parent directory to the Python path
-sys.path.append(parent_dir)
-
-
 def main():
     parser = argparse.ArgumentParser(description='iRRBS pipeline')
     parser.add_argument('-i', '--infile', help='Input BAM file', required=True)
     parser.add_argument('-c', '--chromsizes', help='Chromosome sizes file', required=True)
     parser.add_argument('-g', '--genome', help='Genome file', required=True)
     parser.add_argument('-o', '--outfile', help='Output BAM file', required=True)
     args = parser.parse_args()
```

### Comparing `iRRBS-0.0.6/iRRBS.egg-info/PKG-INFO` & `iRRBS-0.0.7/iRRBS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iRRBS
-Version: 0.0.6
+Version: 0.0.7
 Summary: RRBS tool for deleting artificial cytosins
 Home-page: https://github.com/fothia/iRRBS
 Author: Abel Fothi
 Author-email: fothi.abel@gmail.com
 License: MIT
 Download-URL: https://github.com/fothia/iRRBS/archive/refs/tags/0.0.6.tar.gz
 Platform: UNKNOWN
```

### Comparing `iRRBS-0.0.6/setup.py` & `iRRBS-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 'Operating System :: Unix',
 'License :: OSI Approved :: MIT License',
 'Programming Language :: Python :: 3',
 ]
 setup(
 name = 'iRRBS',
 packages = ['iRRBS'],
-version = '0.0.6',
+version = '0.0.7',
 description = 'RRBS tool for deleting artificial cytosins',
 long_description = (this_directory / "README.md").read_text(),
 url = 'https://github.com/fothia/iRRBS',
 download_url = 'https://github.com/fothia/iRRBS/archive/refs/tags/0.0.6.tar.gz',
 author = 'Abel Fothi',
 author_email = 'fothi.abel@gmail.com',
 license = 'MIT',
```

