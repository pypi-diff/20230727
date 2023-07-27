# Comparing `tmp/cdcs-0.2.1.tar.gz` & `tmp/cdcs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\lmh1\Documents\Python-packages\pycdcs\dist\.tmp-a56yut9a\cdcs-0.2.1.tar", last modified: Fri Mar 24 18:39:05 2023, max compression
+gzip compressed data, was "C:\Users\lmh1\Documents\Python-packages\pycdcs\dist\.tmp-2p1qn8nc\cdcs-0.2.2.tar", last modified: Thu Jul 27 14:26:45 2023, max compression
```

## Comparing `cdcs-0.2.1.tar` & `cdcs-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 18:39:05.000000 cdcs-0.2.1/
--rw-rw-rw-   0        0        0     2776 2019-07-10 17:30:09.000000 cdcs-0.2.1/LICENSE.TXT
--rw-rw-rw-   0        0        0     2583 2023-03-24 18:39:05.000000 cdcs-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1776 2023-01-25 20:27:28.000000 cdcs-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-24 18:39:05.000000 cdcs-0.2.1/cdcs/
-drwxrwxrwx   0        0        0        0 2023-03-24 18:39:05.000000 cdcs-0.2.1/cdcs/CDCS/
--rw-rw-rw-   0        0        0     5811 2023-03-24 16:59:19.000000 cdcs-0.2.1/cdcs/CDCS/__init__.py
--rw-rw-rw-   0        0        0    10931 2022-07-27 10:57:44.000000 cdcs-0.2.1/cdcs/CDCS/_blob.py
--rw-rw-rw-   0        0        0     4957 2022-07-20 17:25:54.000000 cdcs-0.2.1/cdcs/CDCS/_pid_xpath.py
--rw-rw-rw-   0        0        0    13469 2022-12-06 16:24:16.000000 cdcs-0.2.1/cdcs/CDCS/_query.py
--rw-rw-rw-   0        0        0    23617 2023-01-20 16:05:56.000000 cdcs-0.2.1/cdcs/CDCS/_record.py
--rw-rw-rw-   0        0        0    26279 2023-01-25 19:18:42.000000 cdcs-0.2.1/cdcs/CDCS/_template.py
--rw-rw-rw-   0        0        0     1696 2022-03-01 22:03:10.000000 cdcs-0.2.1/cdcs/CDCS/_workspace.py
--rw-rw-rw-   0        0        0    10628 2023-01-24 19:26:21.000000 cdcs-0.2.1/cdcs/CDCS/_xslt.py
--rw-rw-rw-   0        0        0    14641 2022-03-01 22:03:10.000000 cdcs-0.2.1/cdcs/RestClient.py
--rw-rw-rw-   0        0        0        5 2023-03-24 18:28:52.000000 cdcs-0.2.1/cdcs/VERSION
--rw-rw-rw-   0        0        0      493 2022-07-26 19:03:38.000000 cdcs-0.2.1/cdcs/__init__.py
--rw-rw-rw-   0        0        0     1041 2023-03-24 16:58:09.000000 cdcs-0.2.1/cdcs/aslist.py
--rw-rw-rw-   0        0        0      607 2022-07-26 19:26:46.000000 cdcs-0.2.1/cdcs/date_parser.py
-drwxrwxrwx   0        0        0        0 2023-03-24 18:39:05.000000 cdcs-0.2.1/cdcs.egg-info/
--rw-rw-rw-   0        0        0     2583 2023-03-24 18:39:05.000000 cdcs-0.2.1/cdcs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2023-03-24 18:39:05.000000 cdcs-0.2.1/cdcs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 18:39:05.000000 cdcs-0.2.1/cdcs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-12-17 16:24:01.000000 cdcs-0.2.1/cdcs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       29 2023-03-24 18:39:05.000000 cdcs-0.2.1/cdcs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-24 18:39:05.000000 cdcs-0.2.1/cdcs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-02-03 20:26:52.000000 cdcs-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-24 18:39:05.000000 cdcs-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1521 2023-01-19 20:42:07.000000 cdcs-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:26:45.000000 cdcs-0.2.2/
+-rw-rw-rw-   0        0        0     2776 2019-07-10 17:30:09.000000 cdcs-0.2.2/LICENSE.TXT
+-rw-rw-rw-   0        0        0     2584 2023-07-27 14:26:45.000000 cdcs-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1776 2023-01-25 20:27:28.000000 cdcs-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs/
+drwxrwxrwx   0        0        0        0 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs/CDCS/
+-rw-rw-rw-   0        0        0     5811 2023-03-24 16:59:19.000000 cdcs-0.2.2/cdcs/CDCS/__init__.py
+-rw-rw-rw-   0        0        0    10931 2022-07-27 10:57:44.000000 cdcs-0.2.2/cdcs/CDCS/_blob.py
+-rw-rw-rw-   0        0        0     4957 2022-07-20 17:25:54.000000 cdcs-0.2.2/cdcs/CDCS/_pid_xpath.py
+-rw-rw-rw-   0        0        0    13469 2022-12-06 16:24:16.000000 cdcs-0.2.2/cdcs/CDCS/_query.py
+-rw-rw-rw-   0        0        0    23612 2023-07-26 14:08:04.000000 cdcs-0.2.2/cdcs/CDCS/_record.py
+-rw-rw-rw-   0        0        0    26279 2023-01-25 19:18:42.000000 cdcs-0.2.2/cdcs/CDCS/_template.py
+-rw-rw-rw-   0        0        0     1696 2022-03-01 22:03:10.000000 cdcs-0.2.2/cdcs/CDCS/_workspace.py
+-rw-rw-rw-   0        0        0    10628 2023-01-24 19:26:21.000000 cdcs-0.2.2/cdcs/CDCS/_xslt.py
+-rw-rw-rw-   0        0        0    14641 2022-03-01 22:03:10.000000 cdcs-0.2.2/cdcs/RestClient.py
+-rw-rw-rw-   0        0        0        5 2023-07-26 14:08:04.000000 cdcs-0.2.2/cdcs/VERSION
+-rw-rw-rw-   0        0        0      959 2023-07-26 14:08:04.000000 cdcs-0.2.2/cdcs/__init__.py
+-rw-rw-rw-   0        0        0     1041 2023-03-24 16:58:09.000000 cdcs-0.2.2/cdcs/aslist.py
+-rw-rw-rw-   0        0        0      607 2022-07-26 19:26:46.000000 cdcs-0.2.2/cdcs/date_parser.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs.egg-info/
+-rw-rw-rw-   0        0        0     2584 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-12-17 16:24:01.000000 cdcs-0.2.2/cdcs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       29 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-27 14:26:45.000000 cdcs-0.2.2/cdcs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-02-03 20:26:52.000000 cdcs-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 14:26:45.000000 cdcs-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1522 2023-07-26 14:08:04.000000 cdcs-0.2.2/setup.py
```

### Comparing `cdcs-0.2.1/LICENSE.TXT` & `cdcs-0.2.2/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `cdcs-0.2.1/PKG-INFO` & `cdcs-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cdcs
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python API client for performing REST calls to configurable data curation system (CDCS) databases
 Home-page: https://github.com/usnistgov/pycdcs
 Author: Lucas Hale
 Author-email: lucas.hale@nist.gov
 Keywords: CDCS,database,rest API,configurable data curation system
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: LICENSE.TXT
 
 # Python CDCS REST API client
 
 This is a base Python package for accessing instances of the NIST Configurable Data Curation System (CDCS) databases, versions 2.X.X and 3.X.X.  It defines a Python CDCS class that streamlines REST calls to a database by
```

### Comparing `cdcs-0.2.1/README.md` & `cdcs-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cdcs-0.2.1/cdcs/CDCS/__init__.py` & `cdcs-0.2.2/cdcs/CDCS/__init__.py`

 * *Files identical despite different names*

### Comparing `cdcs-0.2.1/cdcs/CDCS/_blob.py` & `cdcs-0.2.2/cdcs/CDCS/_blob.py`

 * *Files identical despite different names*

### Comparing `cdcs-0.2.1/cdcs/CDCS/_pid_xpath.py` & `cdcs-0.2.2/cdcs/CDCS/_pid_xpath.py`

 * *Files identical despite different names*

### Comparing `cdcs-0.2.1/cdcs/CDCS/_query.py` & `cdcs-0.2.2/cdcs/CDCS/_query.py`

 * *Files identical despite different names*

### Comparing `cdcs-0.2.1/cdcs/CDCS/_record.py` & `cdcs-0.2.2/cdcs/CDCS/_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Standard library imports
 from pathlib import Path
 from typing import Optional, Union
 
 from tqdm import tqdm
 
-from IPython.core.display import display, HTML
+from IPython.display import display, HTML
 
 # https://pandas.pydata.org/
 import pandas as pd
 
 from .. import aslist, date_parser
 
 record_keys = ['id', 'template', 'workspace', 'user_id', 'title', 'xml_content',
```

### Comparing `cdcs-0.2.1/cdcs/CDCS/_template.py` & `cdcs-0.2.2/cdcs/CDCS/_template.py`

 * *Files identical despite different names*

### Comparing `cdcs-0.2.1/cdcs/CDCS/_workspace.py` & `cdcs-0.2.2/cdcs/CDCS/_workspace.py`

 * *Files identical despite different names*

### Comparing `cdcs-0.2.1/cdcs/CDCS/_xslt.py` & `cdcs-0.2.2/cdcs/CDCS/_xslt.py`

 * *Files identical despite different names*

### Comparing `cdcs-0.2.1/cdcs/RestClient.py` & `cdcs-0.2.2/cdcs/RestClient.py`

 * *Files identical despite different names*

### Comparing `cdcs-0.2.1/cdcs/aslist.py` & `cdcs-0.2.2/cdcs/aslist.py`

 * *Files identical despite different names*

### Comparing `cdcs-0.2.1/cdcs/date_parser.py` & `cdcs-0.2.2/cdcs/date_parser.py`

 * *Files identical despite different names*

### Comparing `cdcs-0.2.1/cdcs.egg-info/PKG-INFO` & `cdcs-0.2.2/cdcs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cdcs
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python API client for performing REST calls to configurable data curation system (CDCS) databases
 Home-page: https://github.com/usnistgov/pycdcs
 Author: Lucas Hale
 Author-email: lucas.hale@nist.gov
 Keywords: CDCS,database,rest API,configurable data curation system
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: LICENSE.TXT
 
 # Python CDCS REST API client
 
 This is a base Python package for accessing instances of the NIST Configurable Data Curation System (CDCS) databases, versions 2.X.X and 3.X.X.  It defines a Python CDCS class that streamlines REST calls to a database by
```

### Comparing `cdcs-0.2.1/setup.py` & `cdcs-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,19 @@
       version = getversion(),
       description = 'Python API client for performing REST calls to configurable data curation system (CDCS) databases',
       long_description = getreadme(),
       classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Natural Language :: English',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Physics'
       ],
       keywords = [
         'CDCS', 
         'database', 
         'rest API', 
         'configurable data curation system',
```

