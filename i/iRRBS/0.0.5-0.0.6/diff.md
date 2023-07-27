# Comparing `tmp/iRRBS-0.0.5.tar.gz` & `tmp/iRRBS-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iRRBS-0.0.5.tar", last modified: Thu Jul 27 16:00:18 2023, max compression
+gzip compressed data, was "iRRBS-0.0.6.tar", last modified: Thu Jul 27 16:34:10 2023, max compression
```

## Comparing `iRRBS-0.0.5.tar` & `iRRBS-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 16:00:18.706588 iRRBS-0.0.5/
--rw-rw-r--   0 abel      (1000) abel      (1000)      101 2023-07-27 14:53:04.000000 iRRBS-0.0.5/CHANGELOG.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)     1069 2023-07-27 14:53:04.000000 iRRBS-0.0.5/LICENSE
--rw-rw-r--   0 abel      (1000) abel      (1000)       26 2023-07-27 14:53:04.000000 iRRBS-0.0.5/MANIFEST.in
--rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 16:00:18.706588 iRRBS-0.0.5/PKG-INFO
--rw-rw-r--   0 abel      (1000) abel      (1000)      952 2023-07-27 14:53:04.000000 iRRBS-0.0.5/README.md
--rw-rw-r--   0 abel      (1000) abel      (1000)       79 2023-07-27 15:15:36.000000 iRRBS-0.0.5/__init__.py
-drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 16:00:18.706588 iRRBS-0.0.5/iRRBS.egg-info/
--rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 16:00:18.000000 iRRBS-0.0.5/iRRBS.egg-info/PKG-INFO
--rw-rw-r--   0 abel      (1000) abel      (1000)      261 2023-07-27 16:00:18.000000 iRRBS-0.0.5/iRRBS.egg-info/SOURCES.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)        1 2023-07-27 16:00:18.000000 iRRBS-0.0.5/iRRBS.egg-info/dependency_links.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)       17 2023-07-27 16:00:18.000000 iRRBS-0.0.5/iRRBS.egg-info/requires.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)        1 2023-07-27 16:00:18.000000 iRRBS-0.0.5/iRRBS.egg-info/top_level.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)     7349 2023-07-27 14:53:04.000000 iRRBS-0.0.5/irrbs_pipeline.py
--rw-rw-r--   0 abel      (1000) abel      (1000)     1306 2023-07-27 15:59:26.000000 iRRBS-0.0.5/run_irrbs.py
--rw-rw-r--   0 abel      (1000) abel      (1000)       79 2023-07-27 16:00:18.706588 iRRBS-0.0.5/setup.cfg
--rw-rw-r--   0 abel      (1000) abel      (1000)      806 2023-07-27 16:00:03.000000 iRRBS-0.0.5/setup.py
--rw-rw-r--   0 abel      (1000) abel      (1000)      458 2023-07-27 14:53:04.000000 iRRBS-0.0.5/suppress.py
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 16:34:10.650750 iRRBS-0.0.6/
+-rw-rw-r--   0 abel      (1000) abel      (1000)      101 2023-07-27 14:53:04.000000 iRRBS-0.0.6/CHANGELOG.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1069 2023-07-27 14:53:04.000000 iRRBS-0.0.6/LICENSE
+-rw-rw-r--   0 abel      (1000) abel      (1000)       26 2023-07-27 14:53:04.000000 iRRBS-0.0.6/MANIFEST.in
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 16:34:10.650750 iRRBS-0.0.6/PKG-INFO
+-rw-rw-r--   0 abel      (1000) abel      (1000)      952 2023-07-27 14:53:04.000000 iRRBS-0.0.6/README.md
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 16:34:10.650750 iRRBS-0.0.6/iRRBS/
+-rw-rw-r--   0 abel      (1000) abel      (1000)       79 2023-07-27 15:15:36.000000 iRRBS-0.0.6/iRRBS/__init__.py
+-rw-rw-r--   0 abel      (1000) abel      (1000)     7349 2023-07-27 14:53:04.000000 iRRBS-0.0.6/iRRBS/irrbs_pipeline.py
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1306 2023-07-27 15:59:26.000000 iRRBS-0.0.6/iRRBS/run_irrbs.py
+-rw-rw-r--   0 abel      (1000) abel      (1000)      458 2023-07-27 14:53:04.000000 iRRBS-0.0.6/iRRBS/suppress.py
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 16:34:10.650750 iRRBS-0.0.6/iRRBS.egg-info/
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 16:34:10.000000 iRRBS-0.0.6/iRRBS.egg-info/PKG-INFO
+-rw-rw-r--   0 abel      (1000) abel      (1000)      285 2023-07-27 16:34:10.000000 iRRBS-0.0.6/iRRBS.egg-info/SOURCES.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)        1 2023-07-27 16:34:10.000000 iRRBS-0.0.6/iRRBS.egg-info/dependency_links.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)       17 2023-07-27 16:34:10.000000 iRRBS-0.0.6/iRRBS.egg-info/requires.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)        6 2023-07-27 16:34:10.000000 iRRBS-0.0.6/iRRBS.egg-info/top_level.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)       79 2023-07-27 16:34:10.650750 iRRBS-0.0.6/setup.cfg
+-rw-rw-r--   0 abel      (1000) abel      (1000)      828 2023-07-27 16:30:14.000000 iRRBS-0.0.6/setup.py
```

### Comparing `iRRBS-0.0.5/LICENSE` & `iRRBS-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.5/PKG-INFO` & `iRRBS-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: iRRBS
-Version: 0.0.5
+Version: 0.0.6
 Summary: RRBS tool for deleting artificial cytosins
 Home-page: https://github.com/fothia/iRRBS
 Author: Abel Fothi
 Author-email: fothi.abel@gmail.com
 License: MIT
-Download-URL: https://github.com/fothia/iRRBS/archive/refs/tags/0.0.5.tar.gz
+Download-URL: https://github.com/fothia/iRRBS/archive/refs/tags/0.0.6.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `iRRBS-0.0.5/README.md` & `iRRBS-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.5/iRRBS.egg-info/PKG-INFO` & `iRRBS-0.0.6/iRRBS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: iRRBS
-Version: 0.0.5
+Version: 0.0.6
 Summary: RRBS tool for deleting artificial cytosins
 Home-page: https://github.com/fothia/iRRBS
 Author: Abel Fothi
 Author-email: fothi.abel@gmail.com
 License: MIT
-Download-URL: https://github.com/fothia/iRRBS/archive/refs/tags/0.0.5.tar.gz
+Download-URL: https://github.com/fothia/iRRBS/archive/refs/tags/0.0.6.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `iRRBS-0.0.5/irrbs_pipeline.py` & `iRRBS-0.0.6/iRRBS/irrbs_pipeline.py`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.5/run_irrbs.py` & `iRRBS-0.0.6/iRRBS/run_irrbs.py`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.5/setup.py` & `iRRBS-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 'Intended Audience :: Science/Research',
 'Operating System :: Unix',
 'License :: OSI Approved :: MIT License',
 'Programming Language :: Python :: 3',
 ]
 setup(
 name = 'iRRBS',
-version = '0.0.5',
+packages = ['iRRBS'],
+version = '0.0.6',
 description = 'RRBS tool for deleting artificial cytosins',
 long_description = (this_directory / "README.md").read_text(),
 url = 'https://github.com/fothia/iRRBS',
-download_url = 'https://github.com/fothia/iRRBS/archive/refs/tags/0.0.5.tar.gz',
+download_url = 'https://github.com/fothia/iRRBS/archive/refs/tags/0.0.6.tar.gz',
 author = 'Abel Fothi',
 author_email = 'fothi.abel@gmail.com',
 license = 'MIT',
 classifiers = classifiers,
 keywords = '',
 install_requires = [
           'pysam',
```

