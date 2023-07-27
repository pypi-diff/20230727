# Comparing `tmp/element-interface-0.5.4.tar.gz` & `tmp/element-interface-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-interface-0.5.4.tar", last modified: Thu May 25 18:47:59 2023, max compression
+gzip compressed data, was "element-interface-0.6.0.tar", last modified: Thu Jul 27 15:38:44 2023, max compression
```

## Comparing `element-interface-0.5.4.tar` & `element-interface-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:47:59.071871 element-interface-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 18:47:55.000000 element-interface-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-25 18:47:59.071871 element-interface-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-25 18:47:55.000000 element-interface-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:47:59.071871 element-interface-0.5.4/element_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:47:56.000000 element-interface-0.5.4/element_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-05-25 18:47:56.000000 element-interface-0.5.4/element_interface/caiman_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-25 18:47:56.000000 element-interface-0.5.4/element_interface/dandi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-25 18:47:56.000000 element-interface-0.5.4/element_interface/extract_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-25 18:47:56.000000 element-interface-0.5.4/element_interface/extract_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-05-25 18:47:56.000000 element-interface-0.5.4/element_interface/prairieviewreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-25 18:47:56.000000 element-interface-0.5.4/element_interface/run_caiman.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-25 18:47:56.000000 element-interface-0.5.4/element_interface/scanimage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-25 18:47:56.000000 element-interface-0.5.4/element_interface/suite2p_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-25 18:47:56.000000 element-interface-0.5.4/element_interface/suite2p_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-05-25 18:47:56.000000 element-interface-0.5.4/element_interface/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 18:47:56.000000 element-interface-0.5.4/element_interface/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:47:59.071871 element-interface-0.5.4/element_interface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-25 18:47:58.000000 element-interface-0.5.4/element_interface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-25 18:47:58.000000 element-interface-0.5.4/element_interface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:47:58.000000 element-interface-0.5.4/element_interface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 18:47:58.000000 element-interface-0.5.4/element_interface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 18:47:58.000000 element-interface-0.5.4/element_interface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 18:47:59.071871 element-interface-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 18:47:56.000000 element-interface-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:44.539561 element-interface-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-27 15:38:39.000000 element-interface-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-27 15:38:44.539561 element-interface-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-27 15:38:39.000000 element-interface-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:44.539561 element-interface-0.6.0/element_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/caiman_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/dandi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/extract_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/extract_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/prairie_view_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/run_caiman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/scanimage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/suite2p_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/suite2p_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:44.539561 element-interface-0.6.0/element_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-27 15:38:44.000000 element-interface-0.6.0/element_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-27 15:38:44.000000 element-interface-0.6.0/element_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:38:44.000000 element-interface-0.6.0/element_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 15:38:44.000000 element-interface-0.6.0/element_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 15:38:44.000000 element-interface-0.6.0/element_interface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 15:38:44.539561 element-interface-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-27 15:38:39.000000 element-interface-0.6.0/setup.py
```

### Comparing `element-interface-0.5.4/LICENSE` & `element-interface-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `element-interface-0.5.4/PKG-INFO` & `element-interface-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-interface
-Version: 0.5.4
+Version: 0.6.0
 Summary: Loaders of neurophysiological data into the DataJoint Elements
 Home-page: https://github.com/datajoint/element-interface
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
```

### Comparing `element-interface-0.5.4/README.md` & `element-interface-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `element-interface-0.5.4/element_interface/caiman_loader.py` & `element-interface-0.6.0/element_interface/caiman_loader.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.5.4/element_interface/dandi.py` & `element-interface-0.6.0/element_interface/dandi.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.5.4/element_interface/extract_loader.py` & `element-interface-0.6.0/element_interface/extract_loader.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.5.4/element_interface/extract_trigger.py` & `element-interface-0.6.0/element_interface/extract_trigger.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.5.4/element_interface/prairieviewreader.py` & `element-interface-0.6.0/element_interface/prairie_view_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,163 +1,173 @@
 import pathlib
 import xml.etree.ElementTree as ET
 from datetime import datetime
 
 import numpy as np
 
 
-def get_pv_metadata(pvtiffile: str) -> dict:
-    """Extract metadata for scans generated by PrairieView acquisition software.
+def get_prairieview_metadata(ome_tif_filepath: str) -> dict:
+    """Extract metadata for scans generated by Prairie View acquisition software.
 
-    The PrairieView software generates one .ome.tif imaging file per frame acquired. The
-    metadata for all frames is contained one .xml file. This function locates the .xml
-    file and generates a dictionary necessary to populate the DataJoint ScanInfo and
-    Field tables. PrairieView works with resonance scanners with a single field.
-    PrairieView does not support bidirectional x and y scanning. ROI information is not
-    contained in the .xml file. All images generated using PrairieView have square
-    dimensions(e.g. 512x512).
+    The Prairie View software generates one `.ome.tif` imaging file per frame
+    acquired. The metadata for all frames is contained in one .xml file. This
+    function locates the .xml file and generates a dictionary necessary to
+    populate the DataJoint `ScanInfo` and `Field` tables. Prairie View works
+    with resonance scanners with a single field. Prairie View does not support
+    bidirectional x and y scanning. ROI information is not contained in the
+    `.xml` file. All images generated using Prairie View have square dimensions(e.g. 512x512).
 
     Args:
-        pvtiffile: An absolute path to the .ome.tif image file.
+        ome_tif_filepath: An absolute path to the .ome.tif image file.
 
     Raises:
         FileNotFoundError: No .xml file containing information about the acquired scan
-            was found at path in parent directory at `pvtiffile`.
+            was found at path in parent directory at `ome_tif_filepath`.
 
     Returns:
         metainfo: A dict mapping keys to corresponding metadata values fetched from the
             .xml file.
     """
 
     # May return multiple xml files. Only need one that contains scan metadata.
-    xml_files = pathlib.Path(pvtiffile).parent.glob("*.xml")
+    xml_files_list = pathlib.Path(ome_tif_filepath).parent.glob("*.xml")
 
-    for xml_file in xml_files:
-        tree = ET.parse(xml_file)
-        root = tree.getroot()
-        if root.find(".//Sequence"):
+    for file in xml_files_list:
+        xml_tree = ET.parse(file)
+        xml_file = xml_tree.getroot()
+        if xml_file.find(".//Sequence"):
             break
     else:
         raise FileNotFoundError(
-            f"No PrarieView metadata XML file found at {pvtiffile.parent}"
+            f"No PrarieView metadata .xml file found at {pathlib.Path(ome_tif_filepath).parent}"
         )
 
     bidirectional_scan = False  # Does not support bidirectional
     roi = 0
     n_fields = 1  # Always contains 1 field
-    record_start_time = root.find(".//Sequence/[@cycle='1']").attrib.get("time")
+    recording_start_time = xml_file.find(".//Sequence/[@cycle='1']").attrib.get("time")
 
     # Get all channels and find unique values
     channel_list = [
         int(channel.attrib.get("channel"))
-        for channel in root.iterfind(".//Sequence/Frame/File/[@channel]")
+        for channel in xml_file.iterfind(".//Sequence/Frame/File/[@channel]")
     ]
     n_channels = len(set(channel_list))
-    n_frames = len(root.findall(".//Sequence/Frame"))
+    n_frames = len(xml_file.findall(".//Sequence/Frame"))
     framerate = 1 / float(
-        root.findall('.//PVStateValue/[@key="framePeriod"]')[0].attrib.get("value")
+        xml_file.findall('.//PVStateValue/[@key="framePeriod"]')[0].attrib.get("value")
     )  # rate = 1/framePeriod
 
     usec_per_line = (
         float(
-            root.findall(".//PVStateValue/[@key='scanLinePeriod']")[0].attrib.get(
+            xml_file.findall(".//PVStateValue/[@key='scanLinePeriod']")[0].attrib.get(
                 "value"
             )
         )
         * 1e6
     )  # Convert from seconds to microseconds
 
-    scan_datetime = datetime.strptime(root.attrib.get("date"), "%m/%d/%Y %I:%M:%S %p")
+    scan_datetime = datetime.strptime(
+        xml_file.attrib.get("date"), "%m/%d/%Y %I:%M:%S %p"
+    )
 
-    total_duration = float(
-        root.findall(".//Sequence/Frame")[-1].attrib.get("relativeTime")
+    total_scan_duration = float(
+        xml_file.findall(".//Sequence/Frame")[-1].attrib.get("relativeTime")
     )
 
-    px_height = int(
-        root.findall(".//PVStateValue/[@key='pixelsPerLine']")[0].attrib.get("value")
+    pixel_height = int(
+        xml_file.findall(".//PVStateValue/[@key='pixelsPerLine']")[0].attrib.get(
+            "value"
+        )
     )
     # All PrairieView-acquired images have square dimensions (512 x 512; 1024 x 1024)
-    px_width = px_height
+    pixel_width = pixel_height
 
     um_per_pixel = float(
-        root.find(
+        xml_file.find(
             ".//PVStateValue/[@key='micronsPerPixel']/IndexedValue/[@index='XAxis']"
         ).attrib.get("value")
     )
 
-    um_height = um_width = float(px_height) * um_per_pixel
+    um_height = um_width = float(pixel_height) * um_per_pixel
 
     # x and y coordinate values for the center of the field
     x_field = float(
-        root.find(
+        xml_file.find(
             ".//PVStateValue/[@key='currentScanCenter']/IndexedValue/[@index='XAxis']"
         ).attrib.get("value")
     )
     y_field = float(
-        root.find(
+        xml_file.find(
             ".//PVStateValue/[@key='currentScanCenter']/IndexedValue/[@index='YAxis']"
         ).attrib.get("value")
     )
     if (
-        root.find(
+        xml_file.find(
             ".//Sequence/[@cycle='1']/Frame/PVStateShard/PVStateValue/[@key='positionCurrent']/SubindexedValues/[@index='ZAxis']"
         )
         is None
     ):
-
         z_fields = np.float64(
-            root.find(
+            xml_file.find(
                 ".//PVStateValue/[@key='positionCurrent']/SubindexedValues/[@index='ZAxis']/SubindexedValue"
             ).attrib.get("value")
         )
         n_depths = 1
         assert z_fields.size == n_depths
         bidirection_z = False
 
     else:
+        bidirection_z = (
+            xml_file.find(".//Sequence").attrib.get("bidirectionalZ") == "True"
+        )
 
-        bidirection_z = root.find(".//Sequence").attrib.get("bidirectionalZ") == "True"
-
-        # One "Frame" per depth. Gets number of frames in first sequence
+        # One "Frame" per depth in the .xml file. Gets number of frames in first sequence
         planes = [
             int(plane.attrib.get("index"))
-            for plane in root.findall(".//Sequence/[@cycle='1']/Frame")
+            for plane in xml_file.findall(".//Sequence/[@cycle='1']/Frame")
         ]
         n_depths = len(set(planes))
 
-        z_controllers = root.findall(
+        z_controllers = xml_file.findall(
             ".//Sequence/[@cycle='1']/Frame/[@index='1']/PVStateShard/PVStateValue/[@key='positionCurrent']/SubindexedValues/[@index='ZAxis']/SubindexedValue"
         )
-        if len(z_controllers) > 1:
 
+        # If more than one Z-axis controllers are found, 
+        # check which controller is changing z_field depth. Only 1 controller
+        # must change depths.
+        if len(z_controllers) > 1:
             z_repeats = []
-            for controller in root.findall(
-                ".//Sequence/[@cycle='1']/Frame/[@index='1']/PVStateShard/PVStateValue/[@key='positionCurrent']/SubindexedValues/[@index='ZAxis']/"):
+            for controller in xml_file.findall(
+                ".//Sequence/[@cycle='1']/Frame/[@index='1']/PVStateShard/PVStateValue/[@key='positionCurrent']/SubindexedValues/[@index='ZAxis']/"
+            ):
                 z_repeats.append(
                     [
                         float(z.attrib.get("value"))
-                        for z in root.findall(
+                        for z in xml_file.findall(
                             ".//Sequence/[@cycle='1']/Frame/PVStateShard/PVStateValue/[@key='positionCurrent']/SubindexedValues/[@index='ZAxis']/SubindexedValue/[@subindex='{0}']".format(
                                 controller.attrib.get("subindex")
                             )
                         )
                     ]
                 )
-    
-
-            controller_assert = [not all(z == z_controller[0] for z in z_controller) for z_controller in z_repeats]
-
-            assert sum(controller_assert)==1, "Multiple controllers changing z depth is not supported"
+            controller_assert = [
+                not all(z == z_controller[0] for z in z_controller)
+                for z_controller in z_repeats
+            ]
+            assert (
+                sum(controller_assert) == 1
+            ), "Multiple controllers changing z depth is not supported"
 
             z_fields = z_repeats[controller_assert.index(True)]
-            
+
         else:
             z_fields = [
                 z.attrib.get("value")
-                for z in root.findall(
+                for z in xml_file.findall(
                     ".//Sequence/[@cycle='1']/Frame/PVStateShard/PVStateValue/[@key='positionCurrent']/SubindexedValues/[@index='ZAxis']/SubindexedValue/[@subindex='0']"
                 )
             ]
 
         assert (
             len(z_fields) == n_depths
         ), "Number of z fields does not match number of depths."
@@ -172,19 +182,19 @@
         y_pos=None,
         z_pos=None,
         frame_rate=framerate,
         bidirectional=bidirectional_scan,
         bidirectional_z=bidirection_z,
         scan_datetime=scan_datetime,
         usecs_per_line=usec_per_line,
-        scan_duration=total_duration,
-        height_in_pixels=px_height,
-        width_in_pixels=px_width,
+        scan_duration=total_scan_duration,
+        height_in_pixels=pixel_height,
+        width_in_pixels=pixel_width,
         height_in_um=um_height,
         width_in_um=um_width,
         fieldX=x_field,
         fieldY=y_field,
         fieldZ=z_fields,
-        recording_time=record_start_time,
+        recording_time=recording_start_time,
     )
 
     return metainfo
```

### Comparing `element-interface-0.5.4/element_interface/run_caiman.py` & `element-interface-0.6.0/element_interface/run_caiman.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.5.4/element_interface/scanimage_utils.py` & `element-interface-0.6.0/element_interface/scanimage_utils.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.5.4/element_interface/suite2p_loader.py` & `element-interface-0.6.0/element_interface/suite2p_loader.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.5.4/element_interface/suite2p_trigger.py` & `element-interface-0.6.0/element_interface/suite2p_trigger.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.5.4/element_interface/utils.py` & `element-interface-0.6.0/element_interface/utils.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.5.4/element_interface.egg-info/PKG-INFO` & `element-interface-0.6.0/element_interface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-interface
-Version: 0.5.4
+Version: 0.6.0
 Summary: Loaders of neurophysiological data into the DataJoint Elements
 Home-page: https://github.com/datajoint/element-interface
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
```

### Comparing `element-interface-0.5.4/element_interface.egg-info/SOURCES.txt` & `element-interface-0.6.0/element_interface.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 README.md
 setup.py
 element_interface/__init__.py
 element_interface/caiman_loader.py
 element_interface/dandi.py
 element_interface/extract_loader.py
 element_interface/extract_trigger.py
-element_interface/prairieviewreader.py
+element_interface/prairie_view_loader.py
 element_interface/run_caiman.py
 element_interface/scanimage_utils.py
 element_interface/suite2p_loader.py
 element_interface/suite2p_trigger.py
 element_interface/utils.py
 element_interface/version.py
 element_interface.egg-info/PKG-INFO
```

### Comparing `element-interface-0.5.4/setup.py` & `element-interface-0.6.0/setup.py`

 * *Files identical despite different names*

