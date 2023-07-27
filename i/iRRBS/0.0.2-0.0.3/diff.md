# Comparing `tmp/iRRBS-0.0.2.tar.gz` & `tmp/iRRBS-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iRRBS-0.0.2.tar", last modified: Thu Jul 27 15:10:15 2023, max compression
+gzip compressed data, was "iRRBS-0.0.3.tar", last modified: Thu Jul 27 15:20:51 2023, max compression
```

## Comparing `iRRBS-0.0.2.tar` & `iRRBS-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 15:10:15.260765 iRRBS-0.0.2/
--rw-rw-r--   0 abel      (1000) abel      (1000)      101 2023-07-27 14:53:04.000000 iRRBS-0.0.2/CHANGELOG.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)     1069 2023-07-27 14:53:04.000000 iRRBS-0.0.2/LICENSE
--rw-rw-r--   0 abel      (1000) abel      (1000)       26 2023-07-27 14:53:04.000000 iRRBS-0.0.2/MANIFEST.in
--rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 15:10:15.260765 iRRBS-0.0.2/PKG-INFO
--rw-rw-r--   0 abel      (1000) abel      (1000)      952 2023-07-27 14:53:04.000000 iRRBS-0.0.2/README.md
--rw-rw-r--   0 abel      (1000) abel      (1000)       77 2023-07-27 14:53:04.000000 iRRBS-0.0.2/__init__.py
-drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 15:10:15.260765 iRRBS-0.0.2/iRRBS.egg-info/
--rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 15:10:15.000000 iRRBS-0.0.2/iRRBS.egg-info/PKG-INFO
--rw-rw-r--   0 abel      (1000) abel      (1000)      261 2023-07-27 15:10:15.000000 iRRBS-0.0.2/iRRBS.egg-info/SOURCES.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)        1 2023-07-27 15:10:15.000000 iRRBS-0.0.2/iRRBS.egg-info/dependency_links.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)       17 2023-07-27 15:10:15.000000 iRRBS-0.0.2/iRRBS.egg-info/requires.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)        1 2023-07-27 15:10:15.000000 iRRBS-0.0.2/iRRBS.egg-info/top_level.txt
--rw-rw-r--   0 abel      (1000) abel      (1000)     7349 2023-07-27 14:53:04.000000 iRRBS-0.0.2/irrbs_pipeline.py
--rw-rw-r--   0 abel      (1000) abel      (1000)     1075 2023-07-27 14:53:04.000000 iRRBS-0.0.2/run_irrbs.py
--rw-rw-r--   0 abel      (1000) abel      (1000)       79 2023-07-27 15:10:15.264765 iRRBS-0.0.2/setup.cfg
--rw-rw-r--   0 abel      (1000) abel      (1000)      806 2023-07-27 15:10:10.000000 iRRBS-0.0.2/setup.py
--rw-rw-r--   0 abel      (1000) abel      (1000)      458 2023-07-27 14:53:04.000000 iRRBS-0.0.2/suppress.py
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 15:20:51.292693 iRRBS-0.0.3/
+-rw-rw-r--   0 abel      (1000) abel      (1000)      101 2023-07-27 14:53:04.000000 iRRBS-0.0.3/CHANGELOG.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1069 2023-07-27 14:53:04.000000 iRRBS-0.0.3/LICENSE
+-rw-rw-r--   0 abel      (1000) abel      (1000)       26 2023-07-27 14:53:04.000000 iRRBS-0.0.3/MANIFEST.in
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 15:20:51.292693 iRRBS-0.0.3/PKG-INFO
+-rw-rw-r--   0 abel      (1000) abel      (1000)      952 2023-07-27 14:53:04.000000 iRRBS-0.0.3/README.md
+-rw-rw-r--   0 abel      (1000) abel      (1000)       79 2023-07-27 15:15:36.000000 iRRBS-0.0.3/__init__.py
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2023-07-27 15:20:51.292693 iRRBS-0.0.3/iRRBS.egg-info/
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1525 2023-07-27 15:20:51.000000 iRRBS-0.0.3/iRRBS.egg-info/PKG-INFO
+-rw-rw-r--   0 abel      (1000) abel      (1000)      261 2023-07-27 15:20:51.000000 iRRBS-0.0.3/iRRBS.egg-info/SOURCES.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)        1 2023-07-27 15:20:51.000000 iRRBS-0.0.3/iRRBS.egg-info/dependency_links.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)       17 2023-07-27 15:20:51.000000 iRRBS-0.0.3/iRRBS.egg-info/requires.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)        1 2023-07-27 15:20:51.000000 iRRBS-0.0.3/iRRBS.egg-info/top_level.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)     7349 2023-07-27 14:53:04.000000 iRRBS-0.0.3/irrbs_pipeline.py
+-rw-rw-r--   0 abel      (1000) abel      (1000)     1075 2023-07-27 14:53:04.000000 iRRBS-0.0.3/run_irrbs.py
+-rw-rw-r--   0 abel      (1000) abel      (1000)       79 2023-07-27 15:20:51.292693 iRRBS-0.0.3/setup.cfg
+-rw-rw-r--   0 abel      (1000) abel      (1000)      806 2023-07-27 15:20:47.000000 iRRBS-0.0.3/setup.py
+-rw-rw-r--   0 abel      (1000) abel      (1000)      458 2023-07-27 14:53:04.000000 iRRBS-0.0.3/suppress.py
```

### Comparing `iRRBS-0.0.2/LICENSE` & `iRRBS-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.2/PKG-INFO` & `iRRBS-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: iRRBS
-Version: 0.0.2
+Version: 0.0.3
 Summary: RRBS tool for deleting artificial cytosins
 Home-page: https://github.com/fothia/iRRBS
 Author: Abel Fothi
 Author-email: fothi.abel@gmail.com
 License: MIT
-Download-URL: https://github.com/fothia/iRRBS/archive/refs/tags/0.0.2.tar.gz
+Download-URL: https://github.com/fothia/iRRBS/archive/refs/tags/0.0.3.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `iRRBS-0.0.2/README.md` & `iRRBS-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.2/iRRBS.egg-info/PKG-INFO` & `iRRBS-0.0.3/iRRBS.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: iRRBS
-Version: 0.0.2
+Version: 0.0.3
 Summary: RRBS tool for deleting artificial cytosins
 Home-page: https://github.com/fothia/iRRBS
 Author: Abel Fothi
 Author-email: fothi.abel@gmail.com
 License: MIT
-Download-URL: https://github.com/fothia/iRRBS/archive/refs/tags/0.0.2.tar.gz
+Download-URL: https://github.com/fothia/iRRBS/archive/refs/tags/0.0.3.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `iRRBS-0.0.2/irrbs_pipeline.py` & `iRRBS-0.0.3/irrbs_pipeline.py`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.2/run_irrbs.py` & `iRRBS-0.0.3/run_irrbs.py`

 * *Files identical despite different names*

### Comparing `iRRBS-0.0.2/setup.py` & `iRRBS-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 'Intended Audience :: Science/Research',
 'Operating System :: Unix',
 'License :: OSI Approved :: MIT License',
 'Programming Language :: Python :: 3',
 ]
 setup(
 name = 'iRRBS',
-version = '0.0.2',
+version = '0.0.3',
 description = 'RRBS tool for deleting artificial cytosins',
 long_description = (this_directory / "README.md").read_text(),
 url = 'https://github.com/fothia/iRRBS',
-download_url = 'https://github.com/fothia/iRRBS/archive/refs/tags/0.0.2.tar.gz',
+download_url = 'https://github.com/fothia/iRRBS/archive/refs/tags/0.0.3.tar.gz',
 author = 'Abel Fothi',
 author_email = 'fothi.abel@gmail.com',
 license = 'MIT',
 classifiers = classifiers,
 keywords = '',
 install_requires = [
           'pysam',
```

