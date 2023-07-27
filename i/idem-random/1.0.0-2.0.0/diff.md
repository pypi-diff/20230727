# Comparing `tmp/idem-random-1.0.0.tar.gz` & `tmp/idem-random-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-random-1.0.0.tar", last modified: Mon Jul 17 15:16:07 2023, max compression
+gzip compressed data, was "idem-random-2.0.0.tar", last modified: Thu Jul 27 01:16:15 2023, max compression
```

## Comparing `idem-random-1.0.0.tar` & `idem-random-2.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/
--rw-r--r--   0 root         (0) root         (0)    11329 2023-07-17 15:15:53.000000 idem-random-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3713 2023-07-17 15:16:07.088203 idem-random-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2912 2023-07-17 15:15:53.000000 idem-random-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/
--rw-r--r--   0 root         (0) root         (0)     1293 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/exec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/exec/random/
--rw-r--r--   0 root         (0) root         (0)     3467 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/exec/random/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/idem_random/
--rw-r--r--   0 root         (0) root         (0)      836 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/idem_random/init.py
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/states/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/states/random/
--rw-r--r--   0 root         (0) root         (0)     4985 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/states/random/id.py
--rw-r--r--   0 root         (0) root         (0)     5571 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/states/random/integer.py
--rw-r--r--   0 root         (0) root         (0)     7290 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/states/random/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/tool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/tool/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random/tool/random/
--rw-r--r--   0 root         (0) root         (0)     1264 2023-07-17 15:15:53.000000 idem-random-1.0.0/idem_random/tool/random/id.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-17 15:16:06.000000 idem-random-1.0.0/idem_random/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 15:16:07.088203 idem-random-1.0.0/idem_random.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3713 2023-07-17 15:16:07.000000 idem-random-1.0.0/idem_random.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      597 2023-07-17 15:16:07.000000 idem-random-1.0.0/idem_random.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 15:16:07.000000 idem-random-1.0.0/idem_random.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-17 15:16:07.000000 idem-random-1.0.0/idem_random.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-17 15:16:07.000000 idem-random-1.0.0/idem_random.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-17 15:16:07.000000 idem-random-1.0.0/idem_random.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 15:16:07.088203 idem-random-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2766 2023-07-17 15:15:53.000000 idem-random-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 01:16:15.348619 idem-random-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11329 2023-07-27 01:16:00.000000 idem-random-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3714 2023-07-27 01:16:15.348619 idem-random-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-27 01:16:00.000000 idem-random-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 01:16:15.344618 idem-random-2.0.0/idem_random/
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-07-27 01:16:00.000000 idem-random-2.0.0/idem_random/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 01:16:15.344618 idem-random-2.0.0/idem_random/exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 01:16:00.000000 idem-random-2.0.0/idem_random/exec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 01:16:15.344618 idem-random-2.0.0/idem_random/exec/random/
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-07-27 01:16:00.000000 idem-random-2.0.0/idem_random/exec/random/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 01:16:15.344618 idem-random-2.0.0/idem_random/idem_random/
+-rw-r--r--   0 root         (0) root         (0)      836 2023-07-27 01:16:00.000000 idem-random-2.0.0/idem_random/idem_random/init.py
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-27 01:16:00.000000 idem-random-2.0.0/idem_random/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 01:16:15.344618 idem-random-2.0.0/idem_random/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 01:16:00.000000 idem-random-2.0.0/idem_random/states/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 01:16:15.344618 idem-random-2.0.0/idem_random/states/random/
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-07-27 01:16:00.000000 idem-random-2.0.0/idem_random/states/random/id.py
+-rw-r--r--   0 root         (0) root         (0)     5571 2023-07-27 01:16:00.000000 idem-random-2.0.0/idem_random/states/random/integer.py
+-rw-r--r--   0 root         (0) root         (0)     7290 2023-07-27 01:16:00.000000 idem-random-2.0.0/idem_random/states/random/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 01:16:15.344618 idem-random-2.0.0/idem_random/tool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 01:16:00.000000 idem-random-2.0.0/idem_random/tool/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 01:16:15.348619 idem-random-2.0.0/idem_random/tool/random/
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-07-27 01:16:00.000000 idem-random-2.0.0/idem_random/tool/random/id.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-27 01:16:14.000000 idem-random-2.0.0/idem_random/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 01:16:15.344618 idem-random-2.0.0/idem_random.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3714 2023-07-27 01:16:15.000000 idem-random-2.0.0/idem_random.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      597 2023-07-27 01:16:15.000000 idem-random-2.0.0/idem_random.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 01:16:15.000000 idem-random-2.0.0/idem_random.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-27 01:16:15.000000 idem-random-2.0.0/idem_random.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-27 01:16:15.000000 idem-random-2.0.0/idem_random.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-27 01:16:15.000000 idem-random-2.0.0/idem_random.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 01:16:15.348619 idem-random-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2767 2023-07-27 01:16:00.000000 idem-random-2.0.0/setup.py
```

### Comparing `idem-random-1.0.0/LICENSE` & `idem-random-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-random-1.0.0/PKG-INFO` & `idem-random-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-random
-Version: 1.0.0
+Version: 2.0.0
 Summary: Idem plugin for providing randomness
 Home-page: UNKNOWN
 Author: 
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===========
 idem-random
 ===========
 
@@ -73,15 +73,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.6+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `idem-random-1.0.0/README.rst` & `idem-random-2.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.6+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `idem-random-1.0.0/idem_random/conf.py` & `idem-random-2.0.0/idem_random/conf.py`

 * *Files identical despite different names*

### Comparing `idem-random-1.0.0/idem_random/exec/random/password.py` & `idem-random-2.0.0/idem_random/exec/random/password.py`

 * *Files identical despite different names*

### Comparing `idem-random-1.0.0/idem_random/idem_random/init.py` & `idem-random-2.0.0/idem_random/idem_random/init.py`

 * *Files identical despite different names*

### Comparing `idem-random-1.0.0/idem_random/states/random/id.py` & `idem-random-2.0.0/idem_random/states/random/id.py`

 * *Files identical despite different names*

### Comparing `idem-random-1.0.0/idem_random/states/random/integer.py` & `idem-random-2.0.0/idem_random/states/random/integer.py`

 * *Files identical despite different names*

### Comparing `idem-random-1.0.0/idem_random/states/random/password.py` & `idem-random-2.0.0/idem_random/states/random/password.py`

 * *Files identical despite different names*

### Comparing `idem-random-1.0.0/idem_random/tool/random/id.py` & `idem-random-2.0.0/idem_random/tool/random/id.py`

 * *Files identical despite different names*

### Comparing `idem-random-1.0.0/idem_random.egg-info/PKG-INFO` & `idem-random-2.0.0/idem_random.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-random
-Version: 1.0.0
+Version: 2.0.0
 Summary: Idem plugin for providing randomness
 Home-page: UNKNOWN
 Author: 
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===========
 idem-random
 ===========
 
@@ -73,15 +73,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.6+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `idem-random-1.0.0/idem_random.egg-info/SOURCES.txt` & `idem-random-2.0.0/idem_random.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-random-1.0.0/setup.py` & `idem-random-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,25 +70,25 @@
     url="",
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
     entry_points={"console_scripts": ["idem-random = idem_random.scripts:start"]},
     cmdclass={"clean": Clean},
 )
```

