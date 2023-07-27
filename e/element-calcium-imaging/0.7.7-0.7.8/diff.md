# Comparing `tmp/element-calcium-imaging-0.7.7.tar.gz` & `tmp/element-calcium-imaging-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-calcium-imaging-0.7.7.tar", last modified: Mon Jul 24 18:14:23 2023, max compression
+gzip compressed data, was "element-calcium-imaging-0.7.8.tar", last modified: Thu Jul 27 16:31:20 2023, max compression
```

## Comparing `element-calcium-imaging-0.7.7.tar` & `element-calcium-imaging-0.7.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:14:23.297047 element-calcium-imaging-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-07-24 18:14:23.297047 element-calcium-imaging-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:14:23.293047 element-calcium-imaging-0.7.7/element_calcium_imaging/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    66550 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    63748 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/imaging_no_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    74306 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/imaging_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/imaging_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:14:23.297047 element-calcium-imaging-0.7.7/element_calcium_imaging/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/plotting/cell_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/plotting/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    25849 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/element_calcium_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:14:23.297047 element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-07-24 18:14:23.000000 element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-24 18:14:23.000000 element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:14:23.000000 element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 18:14:23.000000 element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 18:14:23.000000 element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:14:23.297047 element-calcium-imaging-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-24 18:14:20.000000 element-calcium-imaging-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:31:20.933898 element-calcium-imaging-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-07-27 16:31:20.933898 element-calcium-imaging-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:31:20.933898 element-calcium-imaging-0.7.8/element_calcium_imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/element_calcium_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/element_calcium_imaging/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66550 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/element_calcium_imaging/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63748 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/element_calcium_imaging/imaging_no_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74306 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/element_calcium_imaging/imaging_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/element_calcium_imaging/imaging_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:31:20.933898 element-calcium-imaging-0.7.8/element_calcium_imaging/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/element_calcium_imaging/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/element_calcium_imaging/plotting/cell_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/element_calcium_imaging/plotting/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/element_calcium_imaging/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/element_calcium_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:31:20.933898 element-calcium-imaging-0.7.8/element_calcium_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-07-27 16:31:20.000000 element-calcium-imaging-0.7.8/element_calcium_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-27 16:31:20.000000 element-calcium-imaging-0.7.8/element_calcium_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:31:20.000000 element-calcium-imaging-0.7.8/element_calcium_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-27 16:31:20.000000 element-calcium-imaging-0.7.8/element_calcium_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 16:31:20.000000 element-calcium-imaging-0.7.8/element_calcium_imaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 16:31:20.933898 element-calcium-imaging-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-27 16:31:17.000000 element-calcium-imaging-0.7.8/setup.py
```

### Comparing `element-calcium-imaging-0.7.7/LICENSE` & `element-calcium-imaging-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.7/PKG-INFO` & `element-calcium-imaging-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-calcium-imaging
-Version: 0.7.7
+Version: 0.7.8
 Summary: Calcium Imaging DataJoint Element
 Home-page: https://github.com/datajoint/element-calcium-imaging
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
```

### Comparing `element-calcium-imaging-0.7.7/README.md` & `element-calcium-imaging-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.7/element_calcium_imaging/analysis.py` & `element-calcium-imaging-0.7.8/element_calcium_imaging/analysis.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.7/element_calcium_imaging/imaging.py` & `element-calcium-imaging-0.7.8/element_calcium_imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.7/element_calcium_imaging/imaging_no_curation.py` & `element-calcium-imaging-0.7.8/element_calcium_imaging/imaging_no_curation.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.7/element_calcium_imaging/imaging_preprocess.py` & `element-calcium-imaging-0.7.8/element_calcium_imaging/imaging_preprocess.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.7/element_calcium_imaging/imaging_report.py` & `element-calcium-imaging-0.7.8/element_calcium_imaging/imaging_report.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.7/element_calcium_imaging/plotting/cell_plot.py` & `element-calcium-imaging-0.7.8/element_calcium_imaging/plotting/cell_plot.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.7/element_calcium_imaging/plotting/widget.py` & `element-calcium-imaging-0.7.8/element_calcium_imaging/plotting/widget.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.7/element_calcium_imaging/scan.py` & `element-calcium-imaging-0.7.8/element_calcium_imaging/scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,18 +513,20 @@
                             field_y=None,
                             field_z=None,
                         )
                         for plane_idx in range(nd2_file.sizes.get("Z", 1))
                     ]
                 )
         elif acq_software == "PrairieView":
-            from element_interface import prairieviewreader
+            from element_interface import prairie_view_loader
 
             scan_filepaths = get_image_files(key, "*.tif")
-            PVScan_info = prairieviewreader.get_pv_metadata(scan_filepaths[0])
+            PVScan_info = prairie_view_loader.get_prairieview_metadata(
+                scan_filepaths[0]
+            )
             self.insert1(
                 dict(
                     key,
                     nfields=PVScan_info["num_fields"],
                     nchannels=PVScan_info["num_channels"],
                     ndepths=PVScan_info["num_planes"],
                     nframes=PVScan_info["num_frames"],
```

### Comparing `element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/PKG-INFO` & `element-calcium-imaging-0.7.8/element_calcium_imaging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-calcium-imaging
-Version: 0.7.7
+Version: 0.7.8
 Summary: Calcium Imaging DataJoint Element
 Home-page: https://github.com/datajoint/element-calcium-imaging
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
```

### Comparing `element-calcium-imaging-0.7.7/element_calcium_imaging.egg-info/SOURCES.txt` & `element-calcium-imaging-0.7.8/element_calcium_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.7/setup.py` & `element-calcium-imaging-0.7.8/setup.py`

 * *Files identical despite different names*

