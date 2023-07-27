# Comparing `tmp/consulate-fork-0.7.0.tar.gz` & `tmp/consulate-fork-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consulate-fork-0.7.0.tar", last modified: Wed Jul 26 12:41:47 2023, max compression
+gzip compressed data, was "consulate-fork-0.7.1.tar", last modified: Thu Jul 27 07:56:46 2023, max compression
```

## Comparing `consulate-fork-0.7.0.tar` & `consulate-fork-0.7.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 bogdan.c   (501) staff       (20)        0 2023-07-26 12:41:47.770892 consulate-fork-0.7.0/
--rw-r--r--   0 bogdan.c   (501) staff       (20)     1523 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/LICENSE
--rw-r--r--   0 bogdan.c   (501) staff       (20)       34 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/MANIFEST.in
--rw-r--r--   0 bogdan.c   (501) staff       (20)     1283 2023-07-26 12:41:47.770956 consulate-fork-0.7.0/PKG-INFO
--rw-r--r--   0 bogdan.c   (501) staff       (20)     6734 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/README.rst
-drwxr-xr-x   0 bogdan.c   (501) staff       (20)        0 2023-07-26 12:41:47.767203 consulate-fork-0.7.0/consulate/
--rw-r--r--   0 bogdan.c   (501) staff       (20)      826 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/__init__.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     4195 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/adapters.py
-drwxr-xr-x   0 bogdan.c   (501) staff       (20)        0 2023-07-26 12:41:47.769208 consulate-fork-0.7.0/consulate/api/
--rw-r--r--   0 bogdan.c   (501) staff       (20)      587 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/api/__init__.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)    15840 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/api/acl.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)    15305 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/api/agent.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     6008 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/api/base.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     6410 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/api/catalog.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     1767 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/api/coordinate.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     1735 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/api/event.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     1930 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/api/health.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)    12546 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/api/kv.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     3032 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/api/lock.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     3909 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/api/session.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)      672 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/api/status.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)    22008 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/cli.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     6603 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/client.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     1117 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/exceptions.py
-drwxr-xr-x   0 bogdan.c   (501) staff       (20)        0 2023-07-26 12:41:47.769846 consulate-fork-0.7.0/consulate/models/
--rw-r--r--   0 bogdan.c   (501) staff       (20)       43 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/models/__init__.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     4121 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/models/acl.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     6921 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/models/agent.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     5423 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/models/base.py
--rw-r--r--   0 bogdan.c   (501) staff       (20)     3088 2023-07-26 10:34:51.000000 consulate-fork-0.7.0/consulate/utils.py
-drwxr-xr-x   0 bogdan.c   (501) staff       (20)        0 2023-07-26 12:41:47.770689 consulate-fork-0.7.0/consulate_fork.egg-info/
--rw-r--r--   0 bogdan.c   (501) staff       (20)     1283 2023-07-26 12:41:47.000000 consulate-fork-0.7.0/consulate_fork.egg-info/PKG-INFO
--rw-r--r--   0 bogdan.c   (501) staff       (20)      823 2023-07-26 12:41:47.000000 consulate-fork-0.7.0/consulate_fork.egg-info/SOURCES.txt
--rw-r--r--   0 bogdan.c   (501) staff       (20)        1 2023-07-26 12:41:47.000000 consulate-fork-0.7.0/consulate_fork.egg-info/dependency_links.txt
--rw-r--r--   0 bogdan.c   (501) staff       (20)       49 2023-07-26 12:41:47.000000 consulate-fork-0.7.0/consulate_fork.egg-info/entry_points.txt
--rw-r--r--   0 bogdan.c   (501) staff       (20)      305 2023-07-26 12:41:47.000000 consulate-fork-0.7.0/consulate_fork.egg-info/requires.txt
--rw-r--r--   0 bogdan.c   (501) staff       (20)       10 2023-07-26 12:41:47.000000 consulate-fork-0.7.0/consulate_fork.egg-info/top_level.txt
--rw-r--r--   0 bogdan.c   (501) staff       (20)        1 2023-07-26 12:11:02.000000 consulate-fork-0.7.0/consulate_fork.egg-info/zip-safe
--rw-r--r--   0 bogdan.c   (501) staff       (20)      332 2023-07-26 12:41:47.771211 consulate-fork-0.7.0/setup.cfg
--rw-r--r--   0 bogdan.c   (501) staff       (20)     2375 2023-07-26 10:44:32.000000 consulate-fork-0.7.0/setup.py
+drwxr-xr-x   0 bogdan.c   (501) staff       (20)        0 2023-07-27 07:56:46.191240 consulate-fork-0.7.1/
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     1523 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/LICENSE
+-rw-r--r--   0 bogdan.c   (501) staff       (20)       34 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/MANIFEST.in
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     1236 2023-07-27 07:56:46.191396 consulate-fork-0.7.1/PKG-INFO
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     6734 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/README.rst
+drwxr-xr-x   0 bogdan.c   (501) staff       (20)        0 2023-07-27 07:56:46.183578 consulate-fork-0.7.1/consulate/
+-rw-r--r--   0 bogdan.c   (501) staff       (20)      826 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/__init__.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     4195 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/adapters.py
+drwxr-xr-x   0 bogdan.c   (501) staff       (20)        0 2023-07-27 07:56:46.187546 consulate-fork-0.7.1/consulate/api/
+-rw-r--r--   0 bogdan.c   (501) staff       (20)      587 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/api/__init__.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)    15840 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/api/acl.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)    15305 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/api/agent.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     6008 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/api/base.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     6410 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/api/catalog.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     1767 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/api/coordinate.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     1735 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/api/event.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     1930 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/api/health.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)    12546 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/api/kv.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     3032 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/api/lock.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     3909 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/api/session.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)      672 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/api/status.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)    22008 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/cli.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     6603 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/client.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     1117 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/exceptions.py
+drwxr-xr-x   0 bogdan.c   (501) staff       (20)        0 2023-07-27 07:56:46.188718 consulate-fork-0.7.1/consulate/models/
+-rw-r--r--   0 bogdan.c   (501) staff       (20)       43 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/models/__init__.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     4121 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/models/acl.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     6921 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/models/agent.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     5423 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/models/base.py
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     3088 2023-07-26 10:34:51.000000 consulate-fork-0.7.1/consulate/utils.py
+drwxr-xr-x   0 bogdan.c   (501) staff       (20)        0 2023-07-27 07:56:46.191037 consulate-fork-0.7.1/consulate_fork.egg-info/
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     1236 2023-07-27 07:56:46.000000 consulate-fork-0.7.1/consulate_fork.egg-info/PKG-INFO
+-rw-r--r--   0 bogdan.c   (501) staff       (20)      823 2023-07-27 07:56:46.000000 consulate-fork-0.7.1/consulate_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 bogdan.c   (501) staff       (20)        1 2023-07-27 07:56:46.000000 consulate-fork-0.7.1/consulate_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 bogdan.c   (501) staff       (20)       49 2023-07-27 07:56:46.000000 consulate-fork-0.7.1/consulate_fork.egg-info/entry_points.txt
+-rw-r--r--   0 bogdan.c   (501) staff       (20)      305 2023-07-27 07:56:46.000000 consulate-fork-0.7.1/consulate_fork.egg-info/requires.txt
+-rw-r--r--   0 bogdan.c   (501) staff       (20)       10 2023-07-27 07:56:46.000000 consulate-fork-0.7.1/consulate_fork.egg-info/top_level.txt
+-rw-r--r--   0 bogdan.c   (501) staff       (20)        1 2023-07-27 07:56:46.000000 consulate-fork-0.7.1/consulate_fork.egg-info/zip-safe
+-rw-r--r--   0 bogdan.c   (501) staff       (20)      332 2023-07-27 07:56:46.192042 consulate-fork-0.7.1/setup.cfg
+-rw-r--r--   0 bogdan.c   (501) staff       (20)     2329 2023-07-27 07:51:32.000000 consulate-fork-0.7.1/setup.py
```

### Comparing `consulate-fork-0.7.0/LICENSE` & `consulate-fork-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/PKG-INFO` & `consulate-fork-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: consulate-fork
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Client library and command line application for the Consul. Fork of Consulate package
 Home-page: https://consulate.readthedocs.org
 Author: Gavin M. Roy
 Author-email: gavinr@aweber.com
 Maintainer: Bogdan Tselobanov
 Maintainer-email: azerot966@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Clustering
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: unixsocket
```

### Comparing `consulate-fork-0.7.0/README.rst` & `consulate-fork-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/__init__.py` & `consulate-fork-0.7.1/consulate/__init__.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/adapters.py` & `consulate-fork-0.7.1/consulate/adapters.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/api/__init__.py` & `consulate-fork-0.7.1/consulate/api/__init__.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/api/acl.py` & `consulate-fork-0.7.1/consulate/api/acl.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/api/agent.py` & `consulate-fork-0.7.1/consulate/api/agent.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/api/base.py` & `consulate-fork-0.7.1/consulate/api/base.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/api/catalog.py` & `consulate-fork-0.7.1/consulate/api/catalog.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/api/coordinate.py` & `consulate-fork-0.7.1/consulate/api/coordinate.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/api/event.py` & `consulate-fork-0.7.1/consulate/api/event.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/api/health.py` & `consulate-fork-0.7.1/consulate/api/health.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/api/kv.py` & `consulate-fork-0.7.1/consulate/api/kv.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/api/lock.py` & `consulate-fork-0.7.1/consulate/api/lock.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/api/session.py` & `consulate-fork-0.7.1/consulate/api/session.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/api/status.py` & `consulate-fork-0.7.1/consulate/api/status.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/cli.py` & `consulate-fork-0.7.1/consulate/cli.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/client.py` & `consulate-fork-0.7.1/consulate/client.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/exceptions.py` & `consulate-fork-0.7.1/consulate/exceptions.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/models/acl.py` & `consulate-fork-0.7.1/consulate/models/acl.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/models/agent.py` & `consulate-fork-0.7.1/consulate/models/agent.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/models/base.py` & `consulate-fork-0.7.1/consulate/models/base.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate/utils.py` & `consulate-fork-0.7.1/consulate/utils.py`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/consulate_fork.egg-info/PKG-INFO` & `consulate-fork-0.7.1/consulate_fork.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: consulate-fork
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Client library and command line application for the Consul. Fork of Consulate package
 Home-page: https://consulate.readthedocs.org
 Author: Gavin M. Roy
 Author-email: gavinr@aweber.com
 Maintainer: Bogdan Tselobanov
 Maintainer-email: azerot966@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Clustering
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: unixsocket
```

### Comparing `consulate-fork-0.7.0/consulate_fork.egg-info/SOURCES.txt` & `consulate-fork-0.7.1/consulate_fork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `consulate-fork-0.7.0/setup.py` & `consulate-fork-0.7.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 __author__ = "Gavin M. Roy"
 __email__ = "gavinr@aweber.com"
 
 __maintainer__ = "Bogdan Tselobanov"
 __maintainer_email__ = "azerot966@gmail.com"
 
@@ -53,21 +53,20 @@
     packages=["consulate", "consulate.api", "consulate.models"],
     entry_points=dict(console_scripts=["consulate=consulate.cli:main"]),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: System :: Systems Administration",
         "Topic :: System :: Clustering",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Software Development :: Libraries",
     ],
```

