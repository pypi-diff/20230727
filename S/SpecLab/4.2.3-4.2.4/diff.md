# Comparing `tmp/SpecLab-4.2.3.tar.gz` & `tmp/SpecLab-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpecLab-4.2.3.tar", last modified: Thu Jul 13 16:16:06 2023, max compression
+gzip compressed data, was "SpecLab-4.2.4.tar", last modified: Wed Jul 26 22:37:49 2023, max compression
```

## Comparing `SpecLab-4.2.3.tar` & `SpecLab-4.2.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5663 2023-07-13 16:16:06.864657 SpecLab-4.2.3/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5409 2023-07-13 16:13:13.000000 SpecLab-4.2.3/README.md
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/aux/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/aux/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/aux/param_files/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/aux/param_files/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/aux/param_files/imXam_param.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/aux/param_files/imXam_param.default.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/aux/param_files/imXam_param_ARCES.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    36736 2023-07-12 15:12:23.000000 SpecLab-4.2.3/SpecLab/aux/pyqtgraph_modifications.tar.gz
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/cfg/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2186 2023-07-13 16:12:45.000000 SpecLab-4.2.3/SpecLab/cfg/SpecLab_config.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/cfg/epar_imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/doc/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1020 2023-07-13 16:11:49.000000 SpecLab-4.2.3/SpecLab/doc/CHANGELOG.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1509 2023-07-13 16:11:31.000000 SpecLab-4.2.3/SpecLab/doc/KNOWN_ISSUES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/doc/LICENSE.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5409 2023-07-13 16:10:48.000000 SpecLab-4.2.3/SpecLab/doc/README.md
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/doc/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/gen/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53081 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/gen/SpecLabFunctions.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/gen/__init__.py
--rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/gen/globals.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/gen/myfunc.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/imXam/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/imXam/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    49863 2023-07-13 16:00:58.000000 SpecLab-4.2.3/SpecLab/imXam/imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab.egg-info/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5663 2023-07-13 16:16:06.000000 SpecLab-4.2.3/SpecLab.egg-info/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      760 2023-07-13 16:16:06.000000 SpecLab-4.2.3/SpecLab.egg-info/SOURCES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        1 2023-07-13 16:16:06.000000 SpecLab-4.2.3/SpecLab.egg-info/dependency_links.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      138 2023-07-13 16:16:06.000000 SpecLab-4.2.3/SpecLab.egg-info/requires.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        8 2023-07-13 16:16:06.000000 SpecLab-4.2.3/SpecLab.egg-info/top_level.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)       38 2023-07-13 16:16:06.864657 SpecLab-4.2.3/setup.cfg
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1299 2023-07-13 16:13:05.000000 SpecLab-4.2.3/setup.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-26 22:37:49.274435 SpecLab-4.2.4/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5663 2023-07-26 22:37:49.274435 SpecLab-4.2.4/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5409 2023-07-26 22:37:12.000000 SpecLab-4.2.4/README.md
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-26 22:37:49.270435 SpecLab-4.2.4/SpecLab/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-26 22:37:49.270435 SpecLab-4.2.4/SpecLab/aux/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/aux/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-26 22:37:49.270435 SpecLab-4.2.4/SpecLab/aux/param_files/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/aux/param_files/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/aux/param_files/imXam_param.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/aux/param_files/imXam_param.default.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/aux/param_files/imXam_param_ARCES.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    36736 2023-07-12 15:12:23.000000 SpecLab-4.2.4/SpecLab/aux/pyqtgraph_modifications.tar.gz
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-26 22:37:49.270435 SpecLab-4.2.4/SpecLab/cfg/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2186 2023-07-13 16:12:45.000000 SpecLab-4.2.4/SpecLab/cfg/SpecLab_config.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/cfg/epar_imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-26 22:37:49.270435 SpecLab-4.2.4/SpecLab/doc/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1020 2023-07-13 16:11:49.000000 SpecLab-4.2.4/SpecLab/doc/CHANGELOG.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1509 2023-07-13 16:11:31.000000 SpecLab-4.2.4/SpecLab/doc/KNOWN_ISSUES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/doc/LICENSE.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5409 2023-07-26 22:37:08.000000 SpecLab-4.2.4/SpecLab/doc/README.md
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/doc/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-26 22:37:49.274435 SpecLab-4.2.4/SpecLab/gen/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53081 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/gen/SpecLabFunctions.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/gen/__init__.py
+-rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/gen/globals.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/gen/myfunc.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-26 22:37:49.274435 SpecLab-4.2.4/SpecLab/imXam/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.4/SpecLab/imXam/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    46395 2023-07-26 22:35:41.000000 SpecLab-4.2.4/SpecLab/imXam/imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-26 22:37:49.270435 SpecLab-4.2.4/SpecLab.egg-info/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5663 2023-07-26 22:37:49.000000 SpecLab-4.2.4/SpecLab.egg-info/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      760 2023-07-26 22:37:49.000000 SpecLab-4.2.4/SpecLab.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        1 2023-07-26 22:37:49.000000 SpecLab-4.2.4/SpecLab.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      138 2023-07-26 22:37:49.000000 SpecLab-4.2.4/SpecLab.egg-info/requires.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        8 2023-07-26 22:37:49.000000 SpecLab-4.2.4/SpecLab.egg-info/top_level.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)       38 2023-07-26 22:37:49.274435 SpecLab-4.2.4/setup.cfg
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1299 2023-07-26 22:36:08.000000 SpecLab-4.2.4/setup.py
```

### Comparing `SpecLab-4.2.3/PKG-INFO` & `SpecLab-4.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: SpecLab
-Version: 4.2.3
+Version: 4.2.4
 Summary: IRAF imexam+DS9 alternative for Python
 Home-page: http://pypi.python.org/pypi/SpecLab/
 Author: A. F. Kowalski
 Author-email: adam.f.kowalski@colorado.edu
 Description-Content-Type: text/markdown
 
-# imXam:  v4.2.3 (Latest)
+# imXam:  v4.2.4 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
 This uses [PyQtGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically below.  
 A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
 to your site-packages/pyqtgraph/ by running the config below.  The installation below will install PyQt6 (6.5.1).
 
-author: Adam F Kowalski (July 13, 2023)
+author: Adam F Kowalski (July 26, 2023)
 
 ## Installing imXam 
 
 ### Step 1
 
 From terminal (if you want to install to your current conda environment; if not, go to Step 2):
```

### Comparing `SpecLab-4.2.3/README.md` & `SpecLab-4.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# imXam:  v4.2.3 (Latest)
+# imXam:  v4.2.4 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
 This uses [PyQtGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically below.  
 A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
 to your site-packages/pyqtgraph/ by running the config below.  The installation below will install PyQt6 (6.5.1).
 
-author: Adam F Kowalski (July 13, 2023)
+author: Adam F Kowalski (July 26, 2023)
 
 ## Installing imXam 
 
 ### Step 1
 
 From terminal (if you want to install to your current conda environment; if not, go to Step 2):
```

### Comparing `SpecLab-4.2.3/SpecLab/aux/param_files/imXam_param.dat` & `SpecLab-4.2.4/SpecLab/aux/param_files/imXam_param.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.3/SpecLab/aux/param_files/imXam_param.default.dat` & `SpecLab-4.2.4/SpecLab/aux/param_files/imXam_param.default.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.3/SpecLab/aux/param_files/imXam_param_ARCES.dat` & `SpecLab-4.2.4/SpecLab/aux/param_files/imXam_param_ARCES.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.3/SpecLab/aux/pyqtgraph_modifications.tar.gz` & `SpecLab-4.2.4/SpecLab/aux/pyqtgraph_modifications.tar.gz`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.3/SpecLab/cfg/SpecLab_config.py` & `SpecLab-4.2.4/SpecLab/cfg/SpecLab_config.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.3/SpecLab/doc/CHANGELOG.txt` & `SpecLab-4.2.4/SpecLab/doc/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.3/SpecLab/doc/KNOWN_ISSUES.txt` & `SpecLab-4.2.4/SpecLab/doc/KNOWN_ISSUES.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.3/SpecLab/doc/LICENSE.txt` & `SpecLab-4.2.4/SpecLab/doc/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.3/SpecLab/doc/README.md` & `SpecLab-4.2.4/SpecLab/doc/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# imXam:  v4.2.3 (Latest)
+# imXam:  v4.2.4 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
 This uses [PyQtGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically below.  
 A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
 to your site-packages/pyqtgraph/ by running the config below.  The installation below will install PyQt6 (6.5.1).
 
-author: Adam F Kowalski (July 13, 2023)
+author: Adam F Kowalski (July 26, 2023)
 
 ## Installing imXam 
 
 ### Step 1
 
 From terminal (if you want to install to your current conda environment; if not, go to Step 2):
```

### Comparing `SpecLab-4.2.3/SpecLab/gen/SpecLabFunctions.py` & `SpecLab-4.2.4/SpecLab/gen/SpecLabFunctions.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.3/SpecLab/gen/globals.py` & `SpecLab-4.2.4/SpecLab/gen/globals.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.3/SpecLab/gen/myfunc.py` & `SpecLab-4.2.4/SpecLab/gen/myfunc.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.3/SpecLab/imXam/imXam.py` & `SpecLab-4.2.4/SpecLab/imXam/imXam.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     z2_zscale = imclean[midpoint] + (coeffsz[0] / 1.0) * (npoints - midpoint)
     return z1_zscale, z2_zscale
 
 
 
 print('======================================================')
 print('======================================================')
-print('imXam: v4.2.3 (July 13, 2023)')
+print('imXam: v4.2.4 (July 26, 2023)')
 print(' To shut down gui, type q in display window, type h for interactive commands, use middle mouse wheel to zoom in and out')
 print(' You may have to click on image display with left mouse button in order to use interactive commands')
 print(' To get a list of command-line options, type imXam.py -h from a terminal.')
 print('======================================================')
 print('imXam.py located in ',your_site_packages_location[0]+'/SpecLab/imXam/')
 print(' and .../anaconda3/envs/<your_env_name>/bin/')
 print('Default param files located in ',your_site_packages_location[0]+'/SpecLab/aux/param_files/')
@@ -107,16 +107,14 @@
 parser = ArgumentParser(formatter_class=RawTextHelpFormatter)
 
 parser.add_argument("-f", "--file", dest="filename", help="FITS file name to examine")
 parser.add_argument("-z1", "--z1", dest="z1", help="lower ADU value for display. Default is using IRAFs zscale algorithm.")
 parser.add_argument("-z2", "--z2", dest="z2", help="upper ADU value for display. Default is using IRAFs zscale algorithm.")
 parser.add_argument("-b", "--bias", dest="biasname", help="Bias (or Dark) filename to subtract (or any other fits image you want to subtract).  Can click ROI to set a rectangle for a quick aperture sum (with no background subtraction).")
 parser.add_argument("-dispax", "--dispax", dest="dispaxis", help="Dispersion axis:  1 for along x (e.g., DIS), 2 for along y (e.g., KOSMOS) ",default='1')
-parser.add_argument("-hcut", "--horizcut", dest="hcut", help="Method for horizontal cuts (simple,interp) shown in lower left window. Default is simple. ",default='simple')
-parser.add_argument("-vcut", "--vertcut", dest="vcut", help="Method for vertical cuts (simple,interp) shown in lower right window. Default is simple.",default='simple')
 parser.add_argument("-ext", "--extension", dest="uextension", help="Extension number of multi-extension FITS file. Default is 0.", default='0')
 parser.add_argument("-repl", "--replace", dest="replace", help="Replace NaN, -Inf, and Inf values of array with value specified after -repl.  Must be > -999 or doesn't replace.", default=-9999.)
 parser.add_argument("-irisras", "--iris_lvl2", dest="lvl2", help='IRIS Level 2 spec raster;  the integer after -irasras will be the image to plot starting from 0')
 parser.add_argument("-cube", "--datacube", dest="cube", help='data dube FITS file with time (or another quantity such as wavelength) along one of the dimensions;  time (or wavelength) dimension is the one that is the 0th dimension [nt, ny, nx] if reading in with astropy.io.fits.getdata;  the integer after -cube will be the extension starting from 0 to plot')
 parser.add_argument("-scube", "--sdatacube", dest="scube", help='3rd axis image to subtract of data cube; default is last index',default=-1)
 parser.add_argument("-tlim1", "--tlim1", dest="tlim1", help='starting index of cube to plot ',default=0)
 parser.add_argument("-tlim2", "--tlim2", dest="tlim2", help='ending index of cube to plot',default=-1)
@@ -320,68 +318,18 @@
 
 
 # lower left window
 def update():
     global data, imv1
     imv2 = pg.PlotWidget()
     l.addWidget(imv2, 3,0,1,2)
-    d2 = roi.getArraySlice(data, imv1.imageItem, axes=(0,1), returnSlice=False)
-    a = d2[0]
-    x1= a[0][0]  # x-coordinate
-    x2 = a[0][1]  # y-coordinate
-    y1 = a[1][0]
-    y2 = a[1][1]
-
-    x22 = x2
-    x11 = x1
-    y11 = y1
-    y22 = y2
-    if x2 < x1:
-        x11=x2
-        x22=x1
-        y11=y2
-        y22=y1
-    if y2 < y1:
-        y11=y2
-        y22=y1
-        x11=x2
-        x22=x1
-
-    nx = x22-x11+1
-    ny = y22-y11+1
-    nvec = (nx**2 + ny**2)**0.5
-    yarr = np.linspace(y11, y22, int(round(nvec)))
-    m = (x22-x11) /(y22-y11)
-    b = x22 - m*y22
-    xarr = m * yarr + b
-    dx = x22-x11
-    dy = y22-y11
-    xx = np.linspace(1,data.shape[0],data.shape[0])
-    yy = np.linspace(1,data.shape[1],data.shape[1])
-    myfunc = RegularGridInterpolator((xx,yy), data)
-    nn=0
-    vec=[0.]
-    while nn < len(yarr):
-        xarr[nn] = np.rint(xarr[nn])
-        if dy > dx:  # vertical cuts
-            if xarr[nn] < data.shape[0]-1 and yarr[nn] < data.shape[1] - 1:
-                val = data[int(xarr[nn]),int(yarr[nn])].tolist()
-                vec = np.append(vec, val)
-        if dx > dy:   #horizontal cuts
-            if xarr[nn] > 1 and  xarr[nn] < data.shape[0]-1 and yarr[nn] < data.shape[1] - 1:
-                if args.hcut == 'simple':
-                    val = data[int(xarr[nn]),int(yarr[nn])].tolist()
-                if args.hcut == 'interp':
-                    val = myfunc((xarr[nn],yarr[nn]))   ##-- this uses the interpolation function (it's slow)
-                vec = np.append(vec, val)
-        nn=nn+1
-    if len(vec) > 2:
-        imv2.plot(vec[1:,])
-       # imv2.plotItem.getAxis('left').setPen(color=(0, 0, 0), width=0.8) #.setStyle(tickTextColor= 'b')
-      #  graphWidget.plotItem.getAxis('bottom').setPen(color=(0, 0, 0), width=0.8) #.setStyle(tickTextColor= 'b')
+    HORIZSLICE =  roi.getArrayRegion(data, imv1.imageItem, axes=(0,1))
+ 
+    if len(HORIZSLICE) > 2:
+        imv2.plot(HORIZSLICE)
         imv2.setLabel('left', 'Counts / Pix')
         imv2.setLabel('bottom', 'Pix along slice')
 
 
         
 roi.sigRegionChanged.connect(update)
 
@@ -1055,66 +1003,17 @@
 update()
 
 # lower right window
 def update_2():
     global data, imv1
     imv3 = pg.PlotWidget()
     l.addWidget(imv3, 3,2,1,2)
-    d3 = roi_v.getArraySlice(data, imv1.imageItem, axes=(0,1), returnSlice=False)
-    a = d3[0]
-    x1= a[0][0]  # x-coordinate
-    x2 = a[0][1]  # y-coordinate
-    y1 = a[1][0]
-    y2 = a[1][1]
-
-    x22 = x2
-    x11 = x1
-    y11 = y1
-    y22 = y2
-    if x2 < x1:
-        x11=x2
-        x22=x1
-        y11=y2
-        y22=y1
-    if y2 < y1:
-        y11=y2
-        y22=y1
-        x11=x2
-        x22=x1
-
-    nx = x22-x11+1
-    ny = y22-y11+1
-    nvec = (nx**2 + ny**2)**0.5
-    yarr = np.linspace(y11, y22, int(round(nvec)))
-    m = (x22-x11) /(y22-y11)
-    b = x22 - m*y22
-    xarr = m * yarr + b
-    dx = x22-x11
-    dy = y22-y11
-    xx = np.linspace(1,data.shape[0],data.shape[0])
-    yy = np.linspace(1,data.shape[1],data.shape[1])
-    myfunc = RegularGridInterpolator((xx,yy), data)
-    nn=0
-    vec=[0.]
-    while nn < len(yarr):
-        xarr[nn] = np.rint(xarr[nn])
-        if dy > dx:  # vertical cuts
-            if xarr[nn] < data.shape[0]-1 and yarr[nn] < data.shape[1] - 1:
-                if args.vcut == 'simple':
-                    val = data[int(xarr[nn]),int(yarr[nn])].tolist()
-                if args.vcut == 'interp':
-                    val = myfunc((xarr[nn],yarr[nn]))   ##-- this uses the interpolation function (it's slow)
-                vec = np.append(vec, val)
-        if dx > dy:   #horizontal cuts
-            if xarr[nn] < data.shape[0]-1 and yarr[nn] < data.shape[1] - 1:
-                val = data[int(xarr[nn]),int(yarr[nn])].tolist()
-                vec = np.append(vec, val)
-        nn=nn+1
-    if len(vec) > 2:
-        imv3.plot(vec[1:,])
+    VERTSLICE = roi_v.getArrayRegion(data, imv1.imageItem, axes=(0,1))
+    if len(VERTSLICE) > 2:
+        imv3.plot(VERTSLICE)
         imv3.setLabel('left', 'Counts / Pix')
         imv3.setLabel('bottom', 'Pix along slice')
 
 
 roi_v.sigRegionChanged.connect(update_2)
 
 update_2()
```

### Comparing `SpecLab-4.2.3/SpecLab.egg-info/PKG-INFO` & `SpecLab-4.2.4/SpecLab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: SpecLab
-Version: 4.2.3
+Version: 4.2.4
 Summary: IRAF imexam+DS9 alternative for Python
 Home-page: http://pypi.python.org/pypi/SpecLab/
 Author: A. F. Kowalski
 Author-email: adam.f.kowalski@colorado.edu
 Description-Content-Type: text/markdown
 
-# imXam:  v4.2.3 (Latest)
+# imXam:  v4.2.4 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
 This uses [PyQtGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically below.  
 A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
 to your site-packages/pyqtgraph/ by running the config below.  The installation below will install PyQt6 (6.5.1).
 
-author: Adam F Kowalski (July 13, 2023)
+author: Adam F Kowalski (July 26, 2023)
 
 ## Installing imXam 
 
 ### Step 1
 
 From terminal (if you want to install to your current conda environment; if not, go to Step 2):
```

### Comparing `SpecLab-4.2.3/SpecLab.egg-info/SOURCES.txt` & `SpecLab-4.2.4/SpecLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.3/setup.py` & `SpecLab-4.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from pathlib import Path
 
 setup(
     name='SpecLab',
-    version='4.2.3',
+    version='4.2.4',
     author='A. F. Kowalski',
     author_email='adam.f.kowalski@colorado.edu',
     packages=['SpecLab','SpecLab.aux','SpecLab.aux.param_files','SpecLab.imXam','SpecLab.doc','SpecLab.gen',],
     package_data = {'':['*.tar.gz', '*.txt', '*.dat', '*.md', '*.rst'],},
    # include_package_data=True,
    # package_dir={"": ""},
     scripts=['SpecLab/cfg/SpecLab_config.py','SpecLab/imXam/imXam.py','SpecLab/cfg/epar_imXam.py',],
```

