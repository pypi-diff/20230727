# Comparing `tmp/gpcal-0.9.5.3.tar.gz` & `tmp/gpcal-0.9.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpcal-0.9.5.3.tar", last modified: Wed Jul 26 07:12:03 2023, max compression
+gzip compressed data, was "gpcal-0.9.5.4.tar", last modified: Thu Jul 27 07:15:04 2023, max compression
```

## Comparing `gpcal-0.9.5.3.tar` & `gpcal-0.9.5.4.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 07:12:03.000000 gpcal-0.9.5.3/
--rw-rw-r--   0 jpark     (1000) jpark     (1000)      701 2023-07-26 07:12:03.000000 gpcal-0.9.5.3/PKG-INFO
--rw-r--r--   0 jpark     (1000) jpark     (1000)       62 2023-03-20 13:01:37.000000 gpcal-0.9.5.3/setup.cfg
--rw-r--r--   0 jpark     (1000) jpark     (1000)     1653 2023-07-26 07:11:35.000000 gpcal-0.9.5.3/setup.py
-drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 07:12:03.000000 gpcal-0.9.5.3/gpcal/
--rw-r--r--   0 jpark     (1000) jpark     (1000)      155 2023-07-26 07:11:13.000000 gpcal-0.9.5.3/gpcal/__init__.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    25243 2023-07-26 07:10:31.000000 gpcal-0.9.5.3/gpcal/synthetic.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)     1256 2023-07-26 06:24:04.000000 gpcal-0.9.5.3/gpcal/cleanhelpers.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    36407 2023-07-26 07:10:24.000000 gpcal-0.9.5.3/gpcal/polsolver.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    67694 2023-07-26 07:10:43.000000 gpcal-0.9.5.3/gpcal/timecal.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)    15099 2023-07-26 06:24:04.000000 gpcal-0.9.5.3/gpcal/aipsutil.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)    27022 2023-07-26 07:10:07.000000 gpcal-0.9.5.3/gpcal/obshelpers.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    66424 2023-07-26 07:09:50.000000 gpcal-0.9.5.3/gpcal/channelcal.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)   193500 2023-07-26 07:09:35.000000 gpcal-0.9.5.3/gpcal/gpcal.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    19944 2023-07-26 07:10:14.000000 gpcal-0.9.5.3/gpcal/plothelpers.py
+drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-27 07:15:04.460218 gpcal-0.9.5.4/
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)      662 2023-07-27 07:15:04.460218 gpcal-0.9.5.4/PKG-INFO
+-rw-r--r--   0 jpark     (1000) jpark     (1000)     2991 2023-03-20 13:01:37.000000 gpcal-0.9.5.4/README.rst
+drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-27 07:15:04.460218 gpcal-0.9.5.4/gpcal/
+-rw-r--r--   0 jpark     (1000) jpark     (1000)      155 2023-07-26 07:11:13.000000 gpcal-0.9.5.4/gpcal/__init__.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)    15099 2023-07-26 06:24:04.000000 gpcal-0.9.5.4/gpcal/aipsutil.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    66424 2023-07-26 07:09:50.000000 gpcal-0.9.5.4/gpcal/channelcal.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)     1256 2023-07-26 06:24:04.000000 gpcal-0.9.5.4/gpcal/cleanhelpers.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)   193500 2023-07-26 07:09:35.000000 gpcal-0.9.5.4/gpcal/gpcal.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)    27022 2023-07-26 07:10:07.000000 gpcal-0.9.5.4/gpcal/obshelpers.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    19944 2023-07-26 07:10:14.000000 gpcal-0.9.5.4/gpcal/plothelpers.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    36407 2023-07-26 07:10:24.000000 gpcal-0.9.5.4/gpcal/polsolver.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    25243 2023-07-26 07:10:31.000000 gpcal-0.9.5.4/gpcal/synthetic.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    67694 2023-07-26 07:10:43.000000 gpcal-0.9.5.4/gpcal/timecal.py
+drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-27 07:15:04.460218 gpcal-0.9.5.4/gpcal.egg-info/
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)      662 2023-07-27 07:15:04.000000 gpcal-0.9.5.4/gpcal.egg-info/PKG-INFO
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)      362 2023-07-27 07:15:04.000000 gpcal-0.9.5.4/gpcal.egg-info/SOURCES.txt
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)        1 2023-07-27 07:15:04.000000 gpcal-0.9.5.4/gpcal.egg-info/dependency_links.txt
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)       38 2023-07-27 07:15:04.000000 gpcal-0.9.5.4/gpcal.egg-info/requires.txt
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)        6 2023-07-27 07:15:04.000000 gpcal-0.9.5.4/gpcal.egg-info/top_level.txt
+-rw-r--r--   0 jpark     (1000) jpark     (1000)       79 2023-07-27 07:15:04.460218 gpcal-0.9.5.4/setup.cfg
+-rw-r--r--   0 jpark     (1000) jpark     (1000)     1653 2023-07-27 07:14:22.000000 gpcal-0.9.5.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gpcal-0.9.5.3/PKG-INFO` & `gpcal-0.9.5.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: gpcal
-Version: 0.9.5.3
+Version: 0.9.5.4
 Summary: A generalized instrumental polarization calibration pipeline for VLBI data
 Home-page: https://github.com/jhparkastro/gpcal
+Download-URL: https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz
 Author: Jongho Park
 Author-email: jpark@asiaa.sinica.edu.tw
 License: gpl-2.0
-Download-URL: https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz
-Description: UNKNOWN
 Keywords: VLBI,polarimetry,astronomy,calibration
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `gpcal-0.9.5.3/setup.py` & `gpcal-0.9.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'gpcal',         # How you named your package folder (MyLib)
   packages = ['gpcal'],   # Chose the same as "name"
-  version = '0.9.5.3',      # Start with a small number and increase it with every change you make
+  version = '0.9.5.4',      # Start with a small number and increase it with every change you make
   license='gpl-2.0',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A generalized instrumental polarization calibration pipeline for VLBI data',   # Give a short description about your library
   author = 'Jongho Park',                   # Type in your name
   author_email = 'jpark@asiaa.sinica.edu.tw',      # Type in your E-Mail
   url = 'https://github.com/jhparkastro/gpcal',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz',    # I explain this later on
   keywords = ['VLBI', 'polarimetry', 'astronomy', 'calibration'],   # Keywords that define your package best
```

### Comparing `gpcal-0.9.5.3/gpcal/synthetic.py` & `gpcal-0.9.5.4/gpcal/synthetic.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.3/gpcal/cleanhelpers.py` & `gpcal-0.9.5.4/gpcal/cleanhelpers.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.3/gpcal/polsolver.py` & `gpcal-0.9.5.4/gpcal/polsolver.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.3/gpcal/timecal.py` & `gpcal-0.9.5.4/gpcal/timecal.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.3/gpcal/aipsutil.py` & `gpcal-0.9.5.4/gpcal/aipsutil.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.3/gpcal/obshelpers.py` & `gpcal-0.9.5.4/gpcal/obshelpers.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.3/gpcal/channelcal.py` & `gpcal-0.9.5.4/gpcal/channelcal.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.3/gpcal/gpcal.py` & `gpcal-0.9.5.4/gpcal/gpcal.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.3/gpcal/plothelpers.py` & `gpcal-0.9.5.4/gpcal/plothelpers.py`

 * *Files identical despite different names*

