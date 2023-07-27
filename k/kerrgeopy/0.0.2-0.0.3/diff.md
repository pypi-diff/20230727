# Comparing `tmp/kerrgeopy-0.0.2.tar.gz` & `tmp/kerrgeopy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerrgeopy-0.0.2.tar", last modified: Thu Jul 27 19:51:30 2023, max compression
+gzip compressed data, was "kerrgeopy-0.0.3.tar", last modified: Thu Jul 27 20:07:58 2023, max compression
```

## Comparing `kerrgeopy-0.0.2.tar` & `kerrgeopy-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 spark59    (502) staff       (20)        0 2023-07-27 19:51:30.730636 kerrgeopy-0.0.2/
--rw-r--r--   0 spark59    (502) staff       (20)    35149 2023-06-20 15:00:03.000000 kerrgeopy-0.0.2/LICENSE
--rw-r--r--   0 spark59    (502) staff       (20)      381 2023-07-27 19:51:30.730514 kerrgeopy-0.0.2/PKG-INFO
--rw-r--r--   0 spark59    (502) staff       (20)     7097 2023-07-27 15:12:37.000000 kerrgeopy-0.0.2/README.md
-drwxr-xr-x   0 spark59    (502) staff       (20)        0 2023-07-27 19:51:30.728875 kerrgeopy-0.0.2/kerrgeopy/
--rw-r--r--   0 spark59    (502) staff       (20)      278 2023-07-27 19:15:12.000000 kerrgeopy-0.0.2/kerrgeopy/__init__.py
--rw-r--r--   0 spark59    (502) staff       (20)     9245 2023-07-27 19:21:00.000000 kerrgeopy-0.0.2/kerrgeopy/bound_orbit.py
--rw-r--r--   0 spark59    (502) staff       (20)     5938 2023-07-27 18:56:14.000000 kerrgeopy-0.0.2/kerrgeopy/bound_solutions.py
--rw-r--r--   0 spark59    (502) staff       (20)    15012 2023-07-27 14:56:42.000000 kerrgeopy-0.0.2/kerrgeopy/constants_of_motion.py
--rw-r--r--   0 spark59    (502) staff       (20)    11298 2023-07-27 18:56:15.000000 kerrgeopy-0.0.2/kerrgeopy/frequencies.py
--rw-r--r--   0 spark59    (502) staff       (20)    11913 2023-07-27 18:56:18.000000 kerrgeopy-0.0.2/kerrgeopy/frequencies_from_constants.py
--rw-r--r--   0 spark59    (502) staff       (20)    12854 2023-07-27 18:41:44.000000 kerrgeopy-0.0.2/kerrgeopy/orbit.py
--rw-r--r--   0 spark59    (502) staff       (20)     4859 2023-07-27 19:16:57.000000 kerrgeopy-0.0.2/kerrgeopy/plunging_orbit.py
--rw-r--r--   0 spark59    (502) staff       (20)    10504 2023-07-27 14:52:10.000000 kerrgeopy-0.0.2/kerrgeopy/plunging_solutions.py
--rw-r--r--   0 spark59    (502) staff       (20)     4986 2023-07-27 18:56:21.000000 kerrgeopy-0.0.2/kerrgeopy/spacetime.py
--rw-r--r--   0 spark59    (502) staff       (20)     5438 2023-07-27 18:52:33.000000 kerrgeopy-0.0.2/kerrgeopy/units.py
-drwxr-xr-x   0 spark59    (502) staff       (20)        0 2023-07-27 19:51:30.729610 kerrgeopy-0.0.2/kerrgeopy.egg-info/
--rw-r--r--   0 spark59    (502) staff       (20)      381 2023-07-27 19:51:30.000000 kerrgeopy-0.0.2/kerrgeopy.egg-info/PKG-INFO
--rw-r--r--   0 spark59    (502) staff       (20)      603 2023-07-27 19:51:30.000000 kerrgeopy-0.0.2/kerrgeopy.egg-info/SOURCES.txt
--rw-r--r--   0 spark59    (502) staff       (20)        1 2023-07-27 19:51:30.000000 kerrgeopy-0.0.2/kerrgeopy.egg-info/dependency_links.txt
--rw-r--r--   0 spark59    (502) staff       (20)       28 2023-07-27 19:51:30.000000 kerrgeopy-0.0.2/kerrgeopy.egg-info/requires.txt
--rw-r--r--   0 spark59    (502) staff       (20)       16 2023-07-27 19:51:30.000000 kerrgeopy-0.0.2/kerrgeopy.egg-info/top_level.txt
--rw-r--r--   0 spark59    (502) staff       (20)       38 2023-07-27 19:51:30.730724 kerrgeopy-0.0.2/setup.cfg
--rw-r--r--   0 spark59    (502) staff       (20)      541 2023-07-27 19:51:14.000000 kerrgeopy-0.0.2/setup.py
-drwxr-xr-x   0 spark59    (502) staff       (20)        0 2023-07-27 19:51:30.730332 kerrgeopy-0.0.2/tests/
--rw-r--r--   0 spark59    (502) staff       (20)        0 2023-06-22 15:13:03.000000 kerrgeopy-0.0.2/tests/__init__.py
--rw-r--r--   0 spark59    (502) staff       (20)     1739 2023-07-27 18:37:01.000000 kerrgeopy-0.0.2/tests/test_bound_solutions.py
--rw-r--r--   0 spark59    (502) staff       (20)     2455 2023-07-27 18:56:14.000000 kerrgeopy-0.0.2/tests/test_constants.py
--rw-r--r--   0 spark59    (502) staff       (20)     2456 2023-07-27 18:35:04.000000 kerrgeopy-0.0.2/tests/test_frequencies.py
--rw-r--r--   0 spark59    (502) staff       (20)     1944 2023-07-27 19:13:43.000000 kerrgeopy-0.0.2/tests/test_orbit.py
+drwxr-xr-x   0 spark59    (502) staff       (20)        0 2023-07-27 20:07:58.788828 kerrgeopy-0.0.3/
+-rw-r--r--   0 spark59    (502) staff       (20)    35149 2023-06-20 15:00:03.000000 kerrgeopy-0.0.3/LICENSE
+-rw-r--r--   0 spark59    (502) staff       (20)      381 2023-07-27 20:07:58.788691 kerrgeopy-0.0.3/PKG-INFO
+-rw-r--r--   0 spark59    (502) staff       (20)     7097 2023-07-27 15:12:37.000000 kerrgeopy-0.0.3/README.md
+drwxr-xr-x   0 spark59    (502) staff       (20)        0 2023-07-27 20:07:58.786376 kerrgeopy-0.0.3/kerrgeopy/
+-rw-r--r--   0 spark59    (502) staff       (20)      278 2023-07-27 19:15:12.000000 kerrgeopy-0.0.3/kerrgeopy/__init__.py
+-rw-r--r--   0 spark59    (502) staff       (20)     9245 2023-07-27 19:21:00.000000 kerrgeopy-0.0.3/kerrgeopy/bound_orbit.py
+-rw-r--r--   0 spark59    (502) staff       (20)     5938 2023-07-27 18:56:14.000000 kerrgeopy-0.0.3/kerrgeopy/bound_solutions.py
+-rw-r--r--   0 spark59    (502) staff       (20)    15012 2023-07-27 14:56:42.000000 kerrgeopy-0.0.3/kerrgeopy/constants_of_motion.py
+-rw-r--r--   0 spark59    (502) staff       (20)    11298 2023-07-27 18:56:15.000000 kerrgeopy-0.0.3/kerrgeopy/frequencies.py
+-rw-r--r--   0 spark59    (502) staff       (20)    11913 2023-07-27 18:56:18.000000 kerrgeopy-0.0.3/kerrgeopy/frequencies_from_constants.py
+-rw-r--r--   0 spark59    (502) staff       (20)    12854 2023-07-27 18:41:44.000000 kerrgeopy-0.0.3/kerrgeopy/orbit.py
+-rw-r--r--   0 spark59    (502) staff       (20)     4859 2023-07-27 19:16:57.000000 kerrgeopy-0.0.3/kerrgeopy/plunging_orbit.py
+-rw-r--r--   0 spark59    (502) staff       (20)    10504 2023-07-27 14:52:10.000000 kerrgeopy-0.0.3/kerrgeopy/plunging_solutions.py
+-rw-r--r--   0 spark59    (502) staff       (20)     4986 2023-07-27 18:56:21.000000 kerrgeopy-0.0.3/kerrgeopy/spacetime.py
+-rw-r--r--   0 spark59    (502) staff       (20)     5438 2023-07-27 18:52:33.000000 kerrgeopy-0.0.3/kerrgeopy/units.py
+drwxr-xr-x   0 spark59    (502) staff       (20)        0 2023-07-27 20:07:58.787313 kerrgeopy-0.0.3/kerrgeopy.egg-info/
+-rw-r--r--   0 spark59    (502) staff       (20)      381 2023-07-27 20:07:58.000000 kerrgeopy-0.0.3/kerrgeopy.egg-info/PKG-INFO
+-rw-r--r--   0 spark59    (502) staff       (20)      603 2023-07-27 20:07:58.000000 kerrgeopy-0.0.3/kerrgeopy.egg-info/SOURCES.txt
+-rw-r--r--   0 spark59    (502) staff       (20)        1 2023-07-27 20:07:58.000000 kerrgeopy-0.0.3/kerrgeopy.egg-info/dependency_links.txt
+-rw-r--r--   0 spark59    (502) staff       (20)       33 2023-07-27 20:07:58.000000 kerrgeopy-0.0.3/kerrgeopy.egg-info/requires.txt
+-rw-r--r--   0 spark59    (502) staff       (20)       16 2023-07-27 20:07:58.000000 kerrgeopy-0.0.3/kerrgeopy.egg-info/top_level.txt
+-rw-r--r--   0 spark59    (502) staff       (20)       38 2023-07-27 20:07:58.788870 kerrgeopy-0.0.3/setup.cfg
+-rw-r--r--   0 spark59    (502) staff       (20)      546 2023-07-27 20:06:00.000000 kerrgeopy-0.0.3/setup.py
+drwxr-xr-x   0 spark59    (502) staff       (20)        0 2023-07-27 20:07:58.788373 kerrgeopy-0.0.3/tests/
+-rw-r--r--   0 spark59    (502) staff       (20)        0 2023-06-22 15:13:03.000000 kerrgeopy-0.0.3/tests/__init__.py
+-rw-r--r--   0 spark59    (502) staff       (20)     1739 2023-07-27 18:37:01.000000 kerrgeopy-0.0.3/tests/test_bound_solutions.py
+-rw-r--r--   0 spark59    (502) staff       (20)     2455 2023-07-27 18:56:14.000000 kerrgeopy-0.0.3/tests/test_constants.py
+-rw-r--r--   0 spark59    (502) staff       (20)     2456 2023-07-27 18:35:04.000000 kerrgeopy-0.0.3/tests/test_frequencies.py
+-rw-r--r--   0 spark59    (502) staff       (20)     1944 2023-07-27 19:13:43.000000 kerrgeopy-0.0.3/tests/test_orbit.py
```

### Comparing `kerrgeopy-0.0.2/LICENSE` & `kerrgeopy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/README.md` & `kerrgeopy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/kerrgeopy/bound_orbit.py` & `kerrgeopy-0.0.3/kerrgeopy/bound_orbit.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/kerrgeopy/bound_solutions.py` & `kerrgeopy-0.0.3/kerrgeopy/bound_solutions.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/kerrgeopy/constants_of_motion.py` & `kerrgeopy-0.0.3/kerrgeopy/constants_of_motion.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/kerrgeopy/frequencies.py` & `kerrgeopy-0.0.3/kerrgeopy/frequencies.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/kerrgeopy/frequencies_from_constants.py` & `kerrgeopy-0.0.3/kerrgeopy/frequencies_from_constants.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/kerrgeopy/orbit.py` & `kerrgeopy-0.0.3/kerrgeopy/orbit.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/kerrgeopy/plunging_orbit.py` & `kerrgeopy-0.0.3/kerrgeopy/plunging_orbit.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/kerrgeopy/plunging_solutions.py` & `kerrgeopy-0.0.3/kerrgeopy/plunging_solutions.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/kerrgeopy/spacetime.py` & `kerrgeopy-0.0.3/kerrgeopy/spacetime.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/kerrgeopy/units.py` & `kerrgeopy-0.0.3/kerrgeopy/units.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/kerrgeopy.egg-info/SOURCES.txt` & `kerrgeopy-0.0.3/kerrgeopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/setup.py` & `kerrgeopy-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 import setuptools
 
 setup(
     name="kerrgeopy",
-    version="0.0.2",
+    version="0.0.3",
     author="Seyong Park",
     description="Library for computing bound and plunging geodesics in Kerr spacetime",
     url="https://github.com/syp2001/KerrGeoPy",
     packages=setuptools.find_packages(),
     classifiers=(
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Natural Language :: English",
     ),
-    install_requires=["scipy>=1.8","numpy","matplotlib"]
+    install_requires=["scipy>=1.8","numpy","matplotlib>=3.3"]
 )
```

### Comparing `kerrgeopy-0.0.2/tests/test_bound_solutions.py` & `kerrgeopy-0.0.3/tests/test_bound_solutions.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/tests/test_constants.py` & `kerrgeopy-0.0.3/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/tests/test_frequencies.py` & `kerrgeopy-0.0.3/tests/test_frequencies.py`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.0.2/tests/test_orbit.py` & `kerrgeopy-0.0.3/tests/test_orbit.py`

 * *Files identical despite different names*

