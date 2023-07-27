# Comparing `tmp/pymolviz-1.1.1.1.tar.gz` & `tmp/pymolviz-1.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/highgarden/PyMolViz/module/dist/.tmp-br_9jy3d/pymolviz-1.1.1.1.tar", last modified: Wed Jul 26 12:35:40 2023, max compression
+gzip compressed data, was "/home/highgarden/PyMolViz/module/dist/.tmp-p3ferfrx/pymolviz-1.1.2.1.tar", last modified: Thu Jul 27 11:50:25 2023, max compression
```

## Comparing `pymolviz-1.1.1.1.tar` & `pymolviz-1.1.2.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)      266 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/PKG-INFO
-drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/pymolviz/
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     9252 2023-07-24 11:53:42.000000 pymolviz-1.1.1.1/pymolviz/ColorMap.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2423 2023-07-24 13:12:11.000000 pymolviz-1.1.1.1/pymolviz/Displayable.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1842 2023-07-24 11:54:42.000000 pymolviz-1.1.1.1/pymolviz/Group.py
-drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/pymolviz/PyMOLobjects/
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1053 2023-07-24 11:47:59.000000 pymolviz-1.1.1.1/pymolviz/PyMOLobjects/Labels.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)       26 2023-07-20 14:22:32.000000 pymolviz-1.1.1.1/pymolviz/PyMOLobjects/__init__.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2025 2023-07-24 11:54:57.000000 pymolviz-1.1.1.1/pymolviz/Script.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)      237 2023-07-21 15:03:55.000000 pymolviz-1.1.1.1/pymolviz/__init__.py
-drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/pymolviz/meshes/
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2933 2023-07-24 11:46:39.000000 pymolviz-1.1.1.1/pymolviz/meshes/Arrows.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2847 2023-07-24 11:45:15.000000 pymolviz-1.1.1.1/pymolviz/meshes/CGOCollection.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2791 2023-07-24 11:46:21.000000 pymolviz-1.1.1.1/pymolviz/meshes/Lines.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     3180 2023-07-24 11:46:08.000000 pymolviz-1.1.1.1/pymolviz/meshes/Mesh.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1167 2023-07-24 11:47:25.000000 pymolviz-1.1.1.1/pymolviz/meshes/Plane.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     3831 2023-07-24 11:58:38.000000 pymolviz-1.1.1.1/pymolviz/meshes/Points.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1338 2023-07-24 11:47:48.000000 pymolviz-1.1.1.1/pymolviz/meshes/Sphere.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)      195 2023-07-20 14:22:32.000000 pymolviz-1.1.1.1/pymolviz/meshes/__init__.py
-drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/pymolviz/util/
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)       81 2023-07-20 14:22:32.000000 pymolviz-1.1.1.1/pymolviz/util/__init__.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)    15472 2023-07-24 11:12:50.000000 pymolviz-1.1.1.1/pymolviz/util/colors.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     4799 2023-05-12 12:56:34.000000 pymolviz-1.1.1.1/pymolviz/util/geometries.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1727 2023-07-20 14:22:32.000000 pymolviz-1.1.1.1/pymolviz/util/io.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)      711 2023-05-12 08:38:42.000000 pymolviz-1.1.1.1/pymolviz/util/math.py
-drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/pymolviz/volumetric/
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2283 2023-07-26 12:29:19.000000 pymolviz-1.1.1.1/pymolviz/volumetric/ColorRamp.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     5708 2023-07-24 13:06:51.000000 pymolviz-1.1.1.1/pymolviz/volumetric/GridData.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     5679 2023-07-20 14:22:32.000000 pymolviz-1.1.1.1/pymolviz/volumetric/IrregularData.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1104 2023-07-20 14:22:32.000000 pymolviz-1.1.1.1/pymolviz/volumetric/IsoMesh.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2932 2023-07-24 11:49:46.000000 pymolviz-1.1.1.1/pymolviz/volumetric/IsoSurface.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2462 2023-07-24 11:50:16.000000 pymolviz-1.1.1.1/pymolviz/volumetric/IsoVolume.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)     4638 2023-07-26 12:26:26.000000 pymolviz-1.1.1.1/pymolviz/volumetric/Volume.py
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)      228 2023-07-20 14:22:32.000000 pymolviz-1.1.1.1/pymolviz/volumetric/__init__.py
-drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/pymolviz.egg-info/
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)      266 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/pymolviz.egg-info/PKG-INFO
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)      962 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/pymolviz.egg-info/SOURCES.txt
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)        1 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/pymolviz.egg-info/dependency_links.txt
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)        1 2023-07-20 14:30:13.000000 pymolviz-1.1.1.1/pymolviz.egg-info/not-zip-safe
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)       30 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/pymolviz.egg-info/requires.txt
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)        9 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/pymolviz.egg-info/top_level.txt
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)       38 2023-07-26 12:35:40.000000 pymolviz-1.1.1.1/setup.cfg
--rw-r--r--   0 highgarden  (1000) highgarden  (1000)      638 2023-07-26 12:35:00.000000 pymolviz-1.1.1.1/setup.py
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      266 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/PKG-INFO
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/pymolviz/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     9252 2023-07-24 11:53:42.000000 pymolviz-1.1.2.1/pymolviz/ColorMap.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2423 2023-07-24 13:12:11.000000 pymolviz-1.1.2.1/pymolviz/Displayable.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1842 2023-07-24 11:54:42.000000 pymolviz-1.1.2.1/pymolviz/Group.py
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/pymolviz/PyMOLobjects/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1053 2023-07-24 11:47:59.000000 pymolviz-1.1.2.1/pymolviz/PyMOLobjects/Labels.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1667 2023-07-27 11:45:45.000000 pymolviz-1.1.2.1/pymolviz/PyMOLobjects/PseudoAtoms.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)       63 2023-07-27 11:32:07.000000 pymolviz-1.1.2.1/pymolviz/PyMOLobjects/__init__.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2025 2023-07-24 11:54:57.000000 pymolviz-1.1.2.1/pymolviz/Script.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      237 2023-07-21 15:03:55.000000 pymolviz-1.1.2.1/pymolviz/__init__.py
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/pymolviz/meshes/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2933 2023-07-24 11:46:39.000000 pymolviz-1.1.2.1/pymolviz/meshes/Arrows.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2847 2023-07-24 11:45:15.000000 pymolviz-1.1.2.1/pymolviz/meshes/CGOCollection.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2791 2023-07-24 11:46:21.000000 pymolviz-1.1.2.1/pymolviz/meshes/Lines.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     3180 2023-07-24 11:46:08.000000 pymolviz-1.1.2.1/pymolviz/meshes/Mesh.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1167 2023-07-24 11:47:25.000000 pymolviz-1.1.2.1/pymolviz/meshes/Plane.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     4053 2023-07-27 11:46:52.000000 pymolviz-1.1.2.1/pymolviz/meshes/Points.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1338 2023-07-24 11:47:48.000000 pymolviz-1.1.2.1/pymolviz/meshes/Sphere.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      195 2023-07-20 14:22:32.000000 pymolviz-1.1.2.1/pymolviz/meshes/__init__.py
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/pymolviz/util/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)       81 2023-07-20 14:22:32.000000 pymolviz-1.1.2.1/pymolviz/util/__init__.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)    15472 2023-07-24 11:12:50.000000 pymolviz-1.1.2.1/pymolviz/util/colors.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     4799 2023-05-12 12:56:34.000000 pymolviz-1.1.2.1/pymolviz/util/geometries.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1727 2023-07-20 14:22:32.000000 pymolviz-1.1.2.1/pymolviz/util/io.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      711 2023-05-12 08:38:42.000000 pymolviz-1.1.2.1/pymolviz/util/math.py
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/pymolviz/volumetric/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2283 2023-07-26 12:29:19.000000 pymolviz-1.1.2.1/pymolviz/volumetric/ColorRamp.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     5708 2023-07-24 13:06:51.000000 pymolviz-1.1.2.1/pymolviz/volumetric/GridData.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     5679 2023-07-20 14:22:32.000000 pymolviz-1.1.2.1/pymolviz/volumetric/IrregularData.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1104 2023-07-20 14:22:32.000000 pymolviz-1.1.2.1/pymolviz/volumetric/IsoMesh.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2932 2023-07-24 11:49:46.000000 pymolviz-1.1.2.1/pymolviz/volumetric/IsoSurface.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2462 2023-07-24 11:50:16.000000 pymolviz-1.1.2.1/pymolviz/volumetric/IsoVolume.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     4638 2023-07-26 12:26:26.000000 pymolviz-1.1.2.1/pymolviz/volumetric/Volume.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      228 2023-07-20 14:22:32.000000 pymolviz-1.1.2.1/pymolviz/volumetric/__init__.py
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/pymolviz.egg-info/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      266 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/pymolviz.egg-info/PKG-INFO
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      999 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/pymolviz.egg-info/SOURCES.txt
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)        1 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/pymolviz.egg-info/dependency_links.txt
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)        1 2023-07-20 14:30:13.000000 pymolviz-1.1.2.1/pymolviz.egg-info/not-zip-safe
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)       30 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/pymolviz.egg-info/requires.txt
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)        9 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/pymolviz.egg-info/top_level.txt
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)       38 2023-07-27 11:50:25.000000 pymolviz-1.1.2.1/setup.cfg
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      638 2023-07-27 11:49:52.000000 pymolviz-1.1.2.1/setup.py
```

### Comparing `pymolviz-1.1.1.1/pymolviz/ColorMap.py` & `pymolviz-1.1.2.1/pymolviz/ColorMap.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/Displayable.py` & `pymolviz-1.1.2.1/pymolviz/Displayable.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/Group.py` & `pymolviz-1.1.2.1/pymolviz/Group.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/PyMOLobjects/Labels.py` & `pymolviz-1.1.2.1/pymolviz/PyMOLobjects/Labels.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/Script.py` & `pymolviz-1.1.2.1/pymolviz/Script.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/meshes/Arrows.py` & `pymolviz-1.1.2.1/pymolviz/meshes/Arrows.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/meshes/CGOCollection.py` & `pymolviz-1.1.2.1/pymolviz/meshes/CGOCollection.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/meshes/Lines.py` & `pymolviz-1.1.2.1/pymolviz/meshes/Lines.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/meshes/Mesh.py` & `pymolviz-1.1.2.1/pymolviz/meshes/Mesh.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/meshes/Plane.py` & `pymolviz-1.1.2.1/pymolviz/meshes/Plane.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/meshes/Points.py` & `pymolviz-1.1.2.1/pymolviz/meshes/Points.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 import numpy as np
 
 from ..ColorMap import ColorMap
 from ..Displayable import Displayable
+from ..PyMOLobjects.PseudoAtoms import PseudoAtoms
 
 class Points(Displayable):
     """ Class to store points and associated colors which can be displayed as a point cloud.
     
     
     Attributes:
         vertices (array-like): An array-like of vertex positions.
@@ -19,29 +20,34 @@
         colormap: Optional. Defaults to "RdYlBu_r". Name of a colormap or a matplotlib colormap or a pymolviz.ColorMap object. Used to map values to colors.
         render_as (str): Optional. Defaults to "Spheres". How to display the points. Can be "Spheres" or "Dots" or None. If None, the points are not displayed.
         radius (float): Optional. Defaults to .3. Only relevant if render_as is "Spheres". The radius of the spheres.
     """
 
     def __init__(self, vertices, color = "red", name = None, state = 1, transparency = 0, colormap = "RdYlBu_r", render_as = "Spheres", radius = .3, *args, **kwargs) -> None:
         super().__init__(name)
+        self.vertices = np.array(vertices, dtype=float).reshape(-1, 3)
         if type(colormap) != ColorMap:
             self.colormap = ColorMap(color, colormap, state = state, name=f"{self.name}_colormap", *args, **kwargs)
         else:
             self.colormap = colormap
         if "single" in self.colormap._color_type: # colors were not inferred
-            self.color = np.arange(vertices.shape[0]) # color is just the index
+            self.color = np.arange(self.vertices.shape[0]) # color is just the index
         else:
             self.color = np.array(color).flatten()
 
-        self.vertices = np.array(vertices, dtype=float).reshape(-1, 3)
         self.render_as = render_as
         self.radius = radius
         self.state = state
         self.transparency = transparency
 
+
+    def as_pseudoatoms(self) -> PseudoAtoms:
+        return PseudoAtoms(self.vertices, self.color, name = self.name, state = self.state, colormap = self.colormap)
+
+
     def _create_CGO_list(self) -> list:
         """ Creates a CGO list from the mesh information. Points can be displayed as spheres or as points.
 
         Returns:
             List of str: The CGO list.
         """
```

### Comparing `pymolviz-1.1.1.1/pymolviz/meshes/Sphere.py` & `pymolviz-1.1.2.1/pymolviz/meshes/Sphere.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/util/colors.py` & `pymolviz-1.1.2.1/pymolviz/util/colors.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/util/geometries.py` & `pymolviz-1.1.2.1/pymolviz/util/geometries.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/util/io.py` & `pymolviz-1.1.2.1/pymolviz/util/io.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/util/math.py` & `pymolviz-1.1.2.1/pymolviz/util/math.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/volumetric/ColorRamp.py` & `pymolviz-1.1.2.1/pymolviz/volumetric/ColorRamp.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/volumetric/GridData.py` & `pymolviz-1.1.2.1/pymolviz/volumetric/GridData.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/volumetric/IrregularData.py` & `pymolviz-1.1.2.1/pymolviz/volumetric/IrregularData.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/volumetric/IsoMesh.py` & `pymolviz-1.1.2.1/pymolviz/volumetric/IsoMesh.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/volumetric/IsoSurface.py` & `pymolviz-1.1.2.1/pymolviz/volumetric/IsoSurface.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/volumetric/IsoVolume.py` & `pymolviz-1.1.2.1/pymolviz/volumetric/IsoVolume.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz/volumetric/Volume.py` & `pymolviz-1.1.2.1/pymolviz/volumetric/Volume.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1.1.1/pymolviz.egg-info/SOURCES.txt` & `pymolviz-1.1.2.1/pymolviz.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pymolviz.egg-info/PKG-INFO
 pymolviz.egg-info/SOURCES.txt
 pymolviz.egg-info/dependency_links.txt
 pymolviz.egg-info/not-zip-safe
 pymolviz.egg-info/requires.txt
 pymolviz.egg-info/top_level.txt
 pymolviz/PyMOLobjects/Labels.py
+pymolviz/PyMOLobjects/PseudoAtoms.py
 pymolviz/PyMOLobjects/__init__.py
 pymolviz/meshes/Arrows.py
 pymolviz/meshes/CGOCollection.py
 pymolviz/meshes/Lines.py
 pymolviz/meshes/Mesh.py
 pymolviz/meshes/Plane.py
 pymolviz/meshes/Points.py
```

### Comparing `pymolviz-1.1.1.1/setup.py` & `pymolviz-1.1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 setup(name='pymolviz',
-        version='1.1.1.1',
+        version='1.1.2.1',
         description='Library to facilitate creation of PyMOL Vizualizations.',
         url='https://github.com/Finnem/PyMolViz',
         author='Finn Mier',
         license='MIT',
         packages=['pymolviz.meshes', 'pymolviz.PyMOLobjects', 'pymolviz.util', 'pymolviz.volumetric', 'pymolviz'],
         install_requires=[
                 'numpy',
```

