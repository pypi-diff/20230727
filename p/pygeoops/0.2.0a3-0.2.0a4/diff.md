# Comparing `tmp/pygeoops-0.2.0a3.tar.gz` & `tmp/pygeoops-0.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoops-0.2.0a3.tar", last modified: Wed Jul 26 15:14:18 2023, max compression
+gzip compressed data, was "pygeoops-0.2.0a4.tar", last modified: Thu Jul 27 01:41:15 2023, max compression
```

## Comparing `pygeoops-0.2.0a3.tar` & `pygeoops-0.2.0a4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:14:18.818250 pygeoops-0.2.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-26 15:14:18.818250 pygeoops-0.2.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:14:18.814250 pygeoops-0.2.0a3/pygeoops/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_simplify_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_simplify_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_view_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:14:18.818250 pygeoops-0.2.0a3/pygeoops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-26 15:14:18.000000 pygeoops-0.2.0a3/pygeoops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-26 15:14:18.000000 pygeoops-0.2.0a3/pygeoops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:14:18.000000 pygeoops-0.2.0a3/pygeoops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-26 15:14:18.000000 pygeoops-0.2.0a3/pygeoops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 15:14:18.000000 pygeoops-0.2.0a3/pygeoops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-26 15:14:18.818250 pygeoops-0.2.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:14:18.818250 pygeoops-0.2.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_simplify_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_simplify_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_view_angles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:41:15.755622 pygeoops-0.2.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-27 01:41:15.755622 pygeoops-0.2.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:41:15.751622 pygeoops-0.2.0a4/pygeoops/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_simplify_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_simplify_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/_view_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pygeoops/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:41:15.751622 pygeoops-0.2.0a4/pygeoops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-27 01:41:15.000000 pygeoops-0.2.0a4/pygeoops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-27 01:41:15.000000 pygeoops-0.2.0a4/pygeoops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 01:41:15.000000 pygeoops-0.2.0a4/pygeoops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 01:41:15.000000 pygeoops-0.2.0a4/pygeoops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 01:41:15.000000 pygeoops-0.2.0a4/pygeoops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-27 01:41:15.755622 pygeoops-0.2.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:41:15.755622 pygeoops-0.2.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_simplify_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_simplify_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-27 01:41:05.000000 pygeoops-0.2.0a4/tests/test_view_angles.py
```

### Comparing `pygeoops-0.2.0a3/LICENSE.txt` & `pygeoops-0.2.0a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/PKG-INFO` & `pygeoops-0.2.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoops
-Version: 0.2.0a3
+Version: 0.2.0a4
 Summary: Library with some less common or extended spatial functions
 Author-email: Pieter Roggemans <pieter.roggemans@gmail.com>
 Project-URL: Homepage, https://github.com/pygeoops/pygeoops
 Project-URL: Bug Tracker, https://github.com/pygeoops/pygeoops/issues
 Keywords: GIS,cartography,pandas,shapely,geopandas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pygeoops-0.2.0a3/README.md` & `pygeoops-0.2.0a4/README.md`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/pygeoops/_centerline.py` & `pygeoops-0.2.0a4/pygeoops/_centerline.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/pygeoops/_general.py` & `pygeoops-0.2.0a4/pygeoops/_general.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/pygeoops/_grid.py` & `pygeoops-0.2.0a4/pygeoops/_grid.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/pygeoops/_simplify.py` & `pygeoops-0.2.0a4/pygeoops/_simplify.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,18 +207,22 @@
         tolerance=tolerance,
         algorithm=algorithm,
         lookahead=lookahead,
         simplify_lookahead_points=simplify_lookahead_points,
         keep_points_on=keep_points_on,
     )
 
-    # If topology needs to be preserved, keep original ring if simplify results is
-    # None or not enough points
-    if preserve_topology and (exterior_simpl is None or len(exterior_simpl) < 3):
-        exterior_simpl = polygon.exterior.coords
+    # If simplify result is None or not enough points
+    if exterior_simpl is None or len(exterior_simpl) < 3:
+        if preserve_topology:
+            # If topology needs to be preserved, keep original ring
+            exterior_simpl = polygon.exterior.coords
+        else:
+            # No use to continue... result is None polygon
+            return None
 
     # Now simplify interior rings
     interiors_simpl = []
     for interior in polygon.interiors:
         interior_simpl = simplify_coords(
             coords=interior.coords,
             tolerance=tolerance,
@@ -270,20 +274,23 @@
         tolerance=tolerance,
         algorithm=algorithm,
         lookahead=lookahead,
         simplify_lookahead_points=simplify_lookahead_points,
         keep_points_on=keep_points_on,
     )
 
-    # If preserve_topology is True and the result is no line anymore, return
-    # original line
-    if preserve_topology and (coords_simpl is None or len(coords_simpl) < 2):
-        return linestring
-    else:
-        return shapely.LineString(coords_simpl)
+    # If the result is no line anymore
+    if coords_simpl is None or len(coords_simpl) < 2:
+        if preserve_topology:
+            # If preserve_topology is True, return original line
+            return linestring
+        else:
+            return None
+
+    return shapely.LineString(coords_simpl)
 
 
 def simplify_coords(
     coords: Union[np.ndarray, shapely.coords.CoordinateSequence],
     tolerance: float,
     algorithm: str,
     lookahead: int,
@@ -292,14 +299,16 @@
 ) -> np.ndarray:
     if isinstance(coords, shapely.coords.CoordinateSequence):
         coords = np.asarray(coords)
     # Determine the indexes of the coordinates to keep after simplification
     if algorithm == "rdp":
         coords_simplify_idx = simplification.simplify_coords_idx(coords, tolerance)
     elif algorithm == "vw":
+        # The simplification library also has a topology preserving variant of vw, but
+        # it doesn't support returning indexes, so is not used.
         coords_simplify_idx = simplification.simplify_coords_vw_idx(coords, tolerance)
     elif algorithm in ["lang", "lang+"]:
         coords_simplify_idx = simplify_lang.simplify_coords_lang_idx(
             coords=coords,
             tolerance=tolerance,
             lookahead=lookahead,
             simplify_lookahead_points=simplify_lookahead_points,
```

### Comparing `pygeoops-0.2.0a3/pygeoops/_simplify_lang.py` & `pygeoops-0.2.0a4/pygeoops/_simplify_lang.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/pygeoops/_simplify_topo.py` & `pygeoops-0.2.0a4/pygeoops/_simplify_topo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Module containing utilities regarding operations on geoseries.
 """
 
 import logging
 from typing import Optional, Union
+import warnings
 
 from geopandas import GeoSeries
 import numpy as np
 from numpy.typing import NDArray
 import shapely
 from shapely.geometry.base import BaseGeometry
 import topojson
@@ -70,15 +71,20 @@
     # -----------------
     # If the input is no Geoseries or list, convert it to a list as the topojson library
     # seems to like that best.
     geometries = geometry
     if not isinstance(geometry, (GeoSeries, list)):
         geometries = geometry.tolist()
 
-    topo = topojson.Topology(data=geometries, prequantize=False)
+    with warnings.catch_warnings():
+        message = "invalid value encountered in cast.*"
+        warnings.filterwarnings(
+            action="ignore", category=RuntimeWarning, message=message
+        )
+        topo = topojson.Topology(data=geometries, prequantize=False)
 
     # Simplify all arcs/vectors/boundaries of the topologies
     # ------------------------------------------------------
     topolines = shapely.MultiLineString(topo.output["arcs"])
     topolines_simpl = pygeoops.simplify(
         geometry=topolines,
         tolerance=tolerance,
@@ -86,15 +92,15 @@
         lookahead=lookahead,
         keep_points_on=keep_points_on,
         preserve_topology=True,
     )
     assert topolines_simpl is not None
 
     # Copy the results of the simplified lines back to the topology arcs
-    if algorithm == "lang":
+    if algorithm in ["lang", "lang+"]:
         # For LANG, a simple copy is OK
         assert isinstance(topolines_simpl, shapely.MultiLineString)
         topo.output["arcs"] = [list(geom.coords) for geom in topolines_simpl.geoms]
     else:
         # For rdp, only overwrite the lines that have a valid result
         for index in range(len(topo.output["arcs"])):
             # If the result of the simplify is a point, keep original
@@ -130,26 +136,18 @@
         )
     except Exception:
         # Geometry or GeometryCollection don't have a primitive type, so exception is
         # thrown. In this case all geometry types are OK, so don't filter the result.
         primitive_types_orig = None
 
     if primitive_types_orig is not None and len(primitive_types_orig) == 1:
-        # If output contains different types, extract only the desired type.
-        geometry_types_simpl = topo_simpl_gdf.geometry.geom_type.unique()
-        primitive_types_simpl = list(
-            {GeometryType(type).to_primitivetype.name for type in geometry_types_simpl}
+        # Extract only the desired type from simplified output
+        topo_simpl_gdf.geometry = pygeoops.collection_extract(
+            topo_simpl_gdf.geometry, PrimitiveType(primitive_types_orig[0])
         )
-        if (
-            len(primitive_types_simpl) > 1
-            or primitive_types_orig[0] != primitive_types_simpl[0]
-        ):
-            topo_simpl_gdf.geometry = pygeoops.collection_extract(
-                topo_simpl_gdf.geometry.array, PrimitiveType(primitive_types_orig[0])
-            )
 
     # Return result in the appropriate type
     # -------------------------------------
     if isinstance(geometry, GeoSeries):
         return topo_simpl_gdf.geometry
     else:
         return topo_simpl_gdf.geometry.array.to_numpy()
```

### Comparing `pygeoops-0.2.0a3/pygeoops/_types.py` & `pygeoops-0.2.0a4/pygeoops/_types.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/pygeoops/_view_angles.py` & `pygeoops-0.2.0a4/pygeoops/_view_angles.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/pygeoops.egg-info/PKG-INFO` & `pygeoops-0.2.0a4/pygeoops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoops
-Version: 0.2.0a3
+Version: 0.2.0a4
 Summary: Library with some less common or extended spatial functions
 Author-email: Pieter Roggemans <pieter.roggemans@gmail.com>
 Project-URL: Homepage, https://github.com/pygeoops/pygeoops
 Project-URL: Bug Tracker, https://github.com/pygeoops/pygeoops/issues
 Keywords: GIS,cartography,pandas,shapely,geopandas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pygeoops-0.2.0a3/pygeoops.egg-info/SOURCES.txt` & `pygeoops-0.2.0a4/pygeoops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/pyproject.toml` & `pygeoops-0.2.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoops"
-version = "0.2.0a3"
+version = "0.2.0a4"
 authors = [
   { name="Pieter Roggemans", email="pieter.roggemans@gmail.com" },
 ]
 description = "Library with some less common or extended spatial functions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pygeoops-0.2.0a3/tests/test_centerline.py` & `pygeoops-0.2.0a4/tests/test_centerline.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/tests/test_general.py` & `pygeoops-0.2.0a4/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/tests/test_grid.py` & `pygeoops-0.2.0a4/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/tests/test_helper.py` & `pygeoops-0.2.0a4/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/tests/test_simplify.py` & `pygeoops-0.2.0a4/tests/test_simplify.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,17 @@
             geometry=shapely.LineString([(0, 0), (10, 10), (20, 20)]),
             tolerance=1,
             preserve_topology=False,
             preserve_common_boundaries=True,
         )
 
 
-@pytest.mark.parametrize("algorithm, tolerance", [("lang", 2), ("rdp", 2), ("vw", 15)])
+@pytest.mark.parametrize(
+    "algorithm, tolerance", [("lang", 2), ("lang+", 2), ("rdp", 2), ("vw", 15)]
+)
 def test_simplify_keep_points_on(tmp_path, algorithm, tolerance):
     # Skip test if simplification is not available
     if algorithm != "lang":
         _ = pytest.importorskip("simplification")
 
     # Prepare test data
     poly_input = shapely.Polygon(
@@ -318,33 +320,35 @@
     assert result is None
 
     # Test simplify on None geometry list
     result = pygeoops.simplify([None], 1)
     assert result == [None]
 
 
-def test_simplify_preservetopology_lang():
+@pytest.mark.parametrize(
+    "algorithm, tolerance", [("lang", 10), ("lang+", 10), ("vw", 50)]
+)
+def test_simplify_preservetopology(algorithm, tolerance):
     # Test Polygon lookahead -1
     poly = shapely.Polygon(
         shell=[(0, 0), (0, 10), (1, 10), (10, 10), (10, 0), (0, 0)],
         holes=[[(2, 2), (2, 8), (8, 8), (8, 2), (2, 2)]],
     )
+
     # If preserve_topology True, the original polygon is returned
     geom_simplified = pygeoops.simplify(
         geometry=poly,
-        algorithm="lang",
-        tolerance=10,
+        algorithm=algorithm,
+        tolerance=tolerance,
         preserve_topology=True,
-        lookahead=-1,
     )
     assert isinstance(geom_simplified, shapely.Polygon)
     assert poly.equals(geom_simplified) is True
 
     # If preserve_topology False, the polygon becomes None
     geom_simplified = pygeoops.simplify(
         geometry=poly,
-        algorithm="lang",
-        tolerance=10,
+        algorithm=algorithm,
+        tolerance=tolerance,
         preserve_topology=False,
-        lookahead=-1,
     )
     assert geom_simplified is None
```

### Comparing `pygeoops-0.2.0a3/tests/test_simplify_lang.py` & `pygeoops-0.2.0a4/tests/test_simplify_lang.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/tests/test_simplify_topo.py` & `pygeoops-0.2.0a4/tests/test_simplify_topo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import warnings
 import geopandas as gpd
 import numpy as np
 import pytest
 import shapely
 
 from pygeoops import _simplify_topo as simplify_topo
 import test_helper
 
 
-@pytest.mark.parametrize("algorithm", ["rdp", "lang"])
+@pytest.mark.parametrize("algorithm", ["rdp", "lang", "lang+"])
 def test_simplify_topo(algorithm):
     # Skip test if algorithm != "lang" and simplification is not available
     if algorithm != "lang":
         _ = pytest.importorskip("simplification")
 
     # Prepare test data
     poly1 = shapely.Polygon([(10, 10), (0, 10), (0, 0), (10, 0), (10, 10)])
@@ -53,14 +54,43 @@
     # poly 1 can't be simplified and stays the same.
     assert result[0] == input[0]
     # Due to the ~ common boundary between poly1 and poly2, a point (10, 0) is added
     # to poly2. Simplification removes (11,0), so poly2 ends up the same as poly1.
     assert result[0] == result[2]
 
 
+def test_simplify_topo_warning_on_cast():
+    """
+    Test handling of following warning in simplify_topo:
+        topojson/core/dedup.py:107:
+        RuntimeWarning: invalid value encountered in cast
+        data["bookkeeping_shared_arcs"] = array_bk_sarcs.astype(np.int64).tolist()
+    """
+    # Prepare test data
+    poly1 = shapely.Polygon([(0, 0), (10, 0), (10, 10), (0, 10), (0, 0)])
+    poly2 = shapely.Polygon([(10, 0), (20, 0), (20, 10), (10, 10), (10, 0)])
+    poly3 = shapely.Polygon([(20, 0), (30, 0), (30, 10), (20, 10), (20, 0)])
+    input = [poly1, poly2, poly3]
+
+    # Test
+    with warnings.catch_warnings():
+        message = "invalid value encountered in cast.*"
+        warnings.filterwarnings(
+            action="error", category=RuntimeWarning, message=message
+        )
+        result = simplify_topo.simplify_topo(input, tolerance=1, algorithm="lang")
+
+    # Check result
+    assert result is not None
+    assert isinstance(result, np.ndarray)
+    assert len(result) == len(input)
+    assert result[0].normalize() == input[0].normalize()
+    assert result[1].normalize() == input[1].normalize()
+
+
 def test_simplify_topo_ducktype_ndarray():
     """
     Test returning a GeoSeries when input is a GeoSeries + make sure the indexes from
     the input GeoSeries are retained!
     """
     # Prepare test data
     poly1 = shapely.Polygon([(10, 10), (0, 10), (0, 0), (10, 0), (10, 10)])
@@ -164,7 +194,47 @@
     for idx, geom_result in enumerate(result):
         if idx == 0:
             assert geom_result == shapely.Polygon(
                 [(10, 10), (0, 10), (0, 0), (10, 0), (10, 10)]
             )
         elif idx == 1:
             assert geom_result is None
+
+
+def test_simplify_topo_result_GeometryCollection(tmp_path):
+    """
+    Test with Polygons as input where an island in a polygon collapses to a lines
+    because of the simplification, resulting in a GeometryCollection.
+    In this case the line is removed from the GeometryCollection so the output only
+    contains Polygons.
+    This tests a specific case because GeometryCollection doesn't have a primitive type.
+    """
+    # Prepare test data
+    # Polygon with a narrow triangle as a hole
+    poly_narrow_hole = shapely.Polygon(
+        shell=[(10, 10), (0, 10), (0, 0), (10, 0), (10, 10)],
+        holes=[[(5, 5), (1, 5), (1, 4), (5, 5)]],
+    )
+    # Standard polygon
+    poly = shapely.Polygon([(30, 10), (20, 10), (20, 0), (30, 0), (30, 10)])
+    input = [poly_narrow_hole, poly]
+    output_path = tmp_path / f"{__name__}_input.png"
+    test_helper.plot([poly_narrow_hole, poly], output_path)
+
+    # Test
+    result = simplify_topo.simplify_topo(input, tolerance=1, algorithm="lang")
+
+    output_path = tmp_path / f"{__name__}_result.png"
+    test_helper.plot(result, output_path)
+
+    # Check result
+    assert result is not None
+    assert isinstance(result, np.ndarray)
+    assert len(result) == len(input)
+    for idx, geom_result in enumerate(result):
+        if idx == 0:
+            assert (
+                geom_result.normalize()
+                == shapely.Polygon(poly_narrow_hole.exterior).normalize()
+            )
+        elif idx == 1:
+            assert geom_result.normalize() == poly.normalize()
```

### Comparing `pygeoops-0.2.0a3/tests/test_types.py` & `pygeoops-0.2.0a4/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a3/tests/test_view_angles.py` & `pygeoops-0.2.0a4/tests/test_view_angles.py`

 * *Files identical despite different names*

