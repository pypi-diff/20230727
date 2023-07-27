# Comparing `tmp/cdsutils-1.6.0.tar.gz` & `tmp/cdsutils-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdsutils-1.6.0.tar", last modified: Mon Oct 10 20:43:14 2022, max compression
+gzip compressed data, was "cdsutils-1.6.1.tar", last modified: Thu Jul 27 17:00:51 2023, max compression
```

## Comparing `cdsutils-1.6.0.tar` & `cdsutils-1.6.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2022-10-10 20:43:14.614459 cdsutils-1.6.0/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       49 2022-06-09 21:18:15.000000 cdsutils-1.6.0/.gitignore
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1936 2022-06-09 21:18:15.000000 cdsutils-1.6.0/.gitlab-ci.yml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1727 2018-01-27 01:16:19.000000 cdsutils-1.6.0/COPYING
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    35068 2015-09-03 04:54:56.000000 cdsutils-1.6.0/COPYING-GPL-3
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       74 2020-05-07 21:27:25.000000 cdsutils-1.6.0/MANIFEST.in
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      876 2022-10-10 20:43:14.610459 cdsutils-1.6.0/PKG-INFO
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      126 2018-01-27 01:16:19.000000 cdsutils-1.6.0/README.md
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2022-10-10 20:43:14.610459 cdsutils-1.6.0/cdsutils/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1159 2022-10-10 20:39:07.000000 cdsutils-1.6.0/cdsutils/__init__.py
--rwxr-xr-x   0 jrollins  (1000) jrollins  (1000)     1716 2022-10-10 20:39:07.000000 cdsutils-1.6.0/cdsutils/__main__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1352 2022-06-09 21:18:15.000000 cdsutils-1.6.0/cdsutils/_util.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      176 2022-10-10 20:43:14.000000 cdsutils-1.6.0/cdsutils/_version.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     4537 2022-10-10 20:37:01.000000 cdsutils-1.6.0/cdsutils/audio.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     5357 2020-07-22 18:54:23.000000 cdsutils-1.6.0/cdsutils/avg.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      157 2020-05-07 21:27:25.000000 cdsutils-1.6.0/cdsutils/errors.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     8377 2020-05-07 21:27:25.000000 cdsutils-1.6.0/cdsutils/feutils.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    11027 2020-05-07 21:27:25.000000 cdsutils-1.6.0/cdsutils/fft.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     3114 2022-06-09 21:18:15.000000 cdsutils-1.6.0/cdsutils/getdata.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     4077 2020-05-07 21:27:25.000000 cdsutils-1.6.0/cdsutils/gnuradio_blocks.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    10374 2022-10-10 20:39:07.000000 cdsutils-1.6.0/cdsutils/matrix.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     3479 2022-06-09 21:18:15.000000 cdsutils-1.6.0/cdsutils/nds.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1249 2021-04-07 16:55:27.000000 cdsutils-1.6.0/cdsutils/plot.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      870 2020-05-07 21:27:25.000000 cdsutils-1.6.0/cdsutils/read.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     5177 2020-10-16 16:14:45.000000 cdsutils-1.6.0/cdsutils/read_filter.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     6694 2020-05-07 21:27:25.000000 cdsutils-1.6.0/cdsutils/servo.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    10528 2022-10-10 20:39:07.000000 cdsutils-1.6.0/cdsutils/sfm.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     7648 2020-05-07 21:27:25.000000 cdsutils-1.6.0/cdsutils/step.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1718 2020-05-07 21:27:25.000000 cdsutils-1.6.0/cdsutils/switch.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     6128 2022-10-10 20:39:07.000000 cdsutils-1.6.0/cdsutils/tests.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     6956 2020-05-07 21:27:25.000000 cdsutils-1.6.0/cdsutils/trigservo.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     4809 2020-05-07 21:27:25.000000 cdsutils-1.6.0/cdsutils/water.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      745 2020-05-07 21:27:25.000000 cdsutils-1.6.0/cdsutils/write.py
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2022-10-10 20:43:14.610459 cdsutils-1.6.0/cdsutils.egg-info/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      876 2022-10-10 20:43:14.000000 cdsutils-1.6.0/cdsutils.egg-info/PKG-INFO
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      729 2022-10-10 20:43:14.000000 cdsutils-1.6.0/cdsutils.egg-info/SOURCES.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)        1 2022-10-10 20:43:14.000000 cdsutils-1.6.0/cdsutils.egg-info/dependency_links.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       52 2022-10-10 20:43:14.000000 cdsutils-1.6.0/cdsutils.egg-info/entry_points.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       49 2022-10-10 20:43:14.000000 cdsutils-1.6.0/cdsutils.egg-info/requires.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)        9 2022-10-10 20:43:14.000000 cdsutils-1.6.0/cdsutils.egg-info/top_level.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       38 2022-10-10 20:43:14.614459 cdsutils-1.6.0/setup.cfg
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1311 2022-10-10 20:39:07.000000 cdsutils-1.6.0/setup.py
+drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2023-07-27 17:00:51.624441 cdsutils-1.6.1/
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)       49 2022-06-09 21:18:15.000000 cdsutils-1.6.1/.gitignore
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1492 2023-07-27 00:15:01.000000 cdsutils-1.6.1/.gitlab-ci.yml
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1727 2018-01-27 01:16:19.000000 cdsutils-1.6.1/COPYING
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)    35068 2015-09-03 04:54:56.000000 cdsutils-1.6.1/COPYING-GPL-3
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)       74 2020-05-07 21:27:25.000000 cdsutils-1.6.1/MANIFEST.in
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      876 2023-07-27 17:00:51.624441 cdsutils-1.6.1/PKG-INFO
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      126 2018-01-27 01:16:19.000000 cdsutils-1.6.1/README.md
+drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2023-07-27 17:00:51.620441 cdsutils-1.6.1/cdsutils/
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1159 2022-10-10 20:39:07.000000 cdsutils-1.6.1/cdsutils/__init__.py
+-rwxr-xr-x   0 jrollins  (1000) jrollins  (1000)     1716 2022-10-10 20:39:07.000000 cdsutils-1.6.1/cdsutils/__main__.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1352 2022-06-09 21:18:15.000000 cdsutils-1.6.1/cdsutils/_util.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      160 2023-07-27 17:00:51.000000 cdsutils-1.6.1/cdsutils/_version.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     4537 2022-10-10 20:37:01.000000 cdsutils-1.6.1/cdsutils/audio.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     5357 2020-07-22 18:54:23.000000 cdsutils-1.6.1/cdsutils/avg.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      157 2020-05-07 21:27:25.000000 cdsutils-1.6.1/cdsutils/errors.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     8377 2020-05-07 21:27:25.000000 cdsutils-1.6.1/cdsutils/feutils.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)    11027 2020-05-07 21:27:25.000000 cdsutils-1.6.1/cdsutils/fft.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     3114 2022-06-09 21:18:15.000000 cdsutils-1.6.1/cdsutils/getdata.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     4077 2020-05-07 21:27:25.000000 cdsutils-1.6.1/cdsutils/gnuradio_blocks.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)    10374 2022-10-10 20:39:07.000000 cdsutils-1.6.1/cdsutils/matrix.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     3479 2022-06-09 21:18:15.000000 cdsutils-1.6.1/cdsutils/nds.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1249 2021-04-07 16:55:27.000000 cdsutils-1.6.1/cdsutils/plot.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      870 2020-05-07 21:27:25.000000 cdsutils-1.6.1/cdsutils/read.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     5177 2020-10-16 16:14:45.000000 cdsutils-1.6.1/cdsutils/read_filter.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     6694 2020-05-07 21:27:25.000000 cdsutils-1.6.1/cdsutils/servo.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)    10528 2022-10-10 20:39:07.000000 cdsutils-1.6.1/cdsutils/sfm.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     7648 2020-05-07 21:27:25.000000 cdsutils-1.6.1/cdsutils/step.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1718 2020-05-07 21:27:25.000000 cdsutils-1.6.1/cdsutils/switch.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     6092 2023-07-26 19:25:31.000000 cdsutils-1.6.1/cdsutils/test_commands.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     6956 2020-05-07 21:27:25.000000 cdsutils-1.6.1/cdsutils/trigservo.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     4809 2020-05-07 21:27:25.000000 cdsutils-1.6.1/cdsutils/water.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      745 2020-05-07 21:27:25.000000 cdsutils-1.6.1/cdsutils/write.py
+drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2023-07-27 17:00:51.624441 cdsutils-1.6.1/cdsutils.egg-info/
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      876 2023-07-27 17:00:51.000000 cdsutils-1.6.1/cdsutils.egg-info/PKG-INFO
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      737 2023-07-27 17:00:51.000000 cdsutils-1.6.1/cdsutils.egg-info/SOURCES.txt
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)        1 2023-07-27 17:00:51.000000 cdsutils-1.6.1/cdsutils.egg-info/dependency_links.txt
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)       52 2023-07-27 17:00:51.000000 cdsutils-1.6.1/cdsutils.egg-info/entry_points.txt
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)       30 2023-07-27 17:00:51.000000 cdsutils-1.6.1/cdsutils.egg-info/requires.txt
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)        9 2023-07-27 17:00:51.000000 cdsutils-1.6.1/cdsutils.egg-info/top_level.txt
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)       38 2023-07-27 17:00:51.624441 cdsutils-1.6.1/setup.cfg
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1305 2023-07-26 23:17:59.000000 cdsutils-1.6.1/setup.py
```

### Comparing `cdsutils-1.6.0/COPYING` & `cdsutils-1.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/COPYING-GPL-3` & `cdsutils-1.6.1/COPYING-GPL-3`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/PKG-INFO` & `cdsutils-1.6.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdsutils
-Version: 1.6.0
+Version: 1.6.1
 Summary: Advanced LIGO CDS python utilities
 Home-page: https://git.ligo.org/cds/cdsutils
 Author: Jameson Graef Rollins
 Author-email: jameson.rollins@ligo.org
 License: GPL-3.0-or-later
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `cdsutils-1.6.0/cdsutils/__init__.py` & `cdsutils-1.6.1/cdsutils/__init__.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/__main__.py` & `cdsutils-1.6.1/cdsutils/__main__.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/_util.py` & `cdsutils-1.6.1/cdsutils/_util.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/audio.py` & `cdsutils-1.6.1/cdsutils/audio.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/avg.py` & `cdsutils-1.6.1/cdsutils/avg.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/feutils.py` & `cdsutils-1.6.1/cdsutils/feutils.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/fft.py` & `cdsutils-1.6.1/cdsutils/fft.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/getdata.py` & `cdsutils-1.6.1/cdsutils/getdata.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/gnuradio_blocks.py` & `cdsutils-1.6.1/cdsutils/gnuradio_blocks.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/matrix.py` & `cdsutils-1.6.1/cdsutils/matrix.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/nds.py` & `cdsutils-1.6.1/cdsutils/nds.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/plot.py` & `cdsutils-1.6.1/cdsutils/plot.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/read.py` & `cdsutils-1.6.1/cdsutils/read.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/read_filter.py` & `cdsutils-1.6.1/cdsutils/read_filter.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/servo.py` & `cdsutils-1.6.1/cdsutils/servo.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/sfm.py` & `cdsutils-1.6.1/cdsutils/sfm.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/step.py` & `cdsutils-1.6.1/cdsutils/step.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/switch.py` & `cdsutils-1.6.1/cdsutils/switch.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/tests.py` & `cdsutils-1.6.1/cdsutils/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import unittest
 import os
 import time
 import multiprocessing
-from collections import defaultdict
 
 from ezca import Ezca
 from ezca.emulators import const as emu_const
 from ezca.emulators.ligofilter import start_emulator
 
 from .step import Step, step
 from .servo import Servo, servo
```

### Comparing `cdsutils-1.6.0/cdsutils/trigservo.py` & `cdsutils-1.6.1/cdsutils/trigservo.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/water.py` & `cdsutils-1.6.1/cdsutils/water.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils/write.py` & `cdsutils-1.6.1/cdsutils/write.py`

 * *Files identical despite different names*

### Comparing `cdsutils-1.6.0/cdsutils.egg-info/PKG-INFO` & `cdsutils-1.6.1/cdsutils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdsutils
-Version: 1.6.0
+Version: 1.6.1
 Summary: Advanced LIGO CDS python utilities
 Home-page: https://git.ligo.org/cds/cdsutils
 Author: Jameson Graef Rollins
 Author-email: jameson.rollins@ligo.org
 License: GPL-3.0-or-later
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `cdsutils-1.6.0/cdsutils.egg-info/SOURCES.txt` & `cdsutils-1.6.1/cdsutils.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 cdsutils/plot.py
 cdsutils/read.py
 cdsutils/read_filter.py
 cdsutils/servo.py
 cdsutils/sfm.py
 cdsutils/step.py
 cdsutils/switch.py
-cdsutils/tests.py
+cdsutils/test_commands.py
 cdsutils/trigservo.py
 cdsutils/water.py
 cdsutils/write.py
 cdsutils.egg-info/PKG-INFO
 cdsutils.egg-info/SOURCES.txt
 cdsutils.egg-info/dependency_links.txt
 cdsutils.egg-info/entry_points.txt
```

### Comparing `cdsutils-1.6.0/setup.py` & `cdsutils-1.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,18 +32,18 @@
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
 
     install_requires=[
         'gpstime',
-        'nds2-client',
+        #'nds2-client',
         'matplotlib',
         'numpy',
-        'python-ezca',
+        'ezca',
     ],
 
     packages=[
         'cdsutils',
     ],
 
     entry_points={
```

