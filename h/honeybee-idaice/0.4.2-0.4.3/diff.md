# Comparing `tmp/honeybee-idaice-0.4.2.tar.gz` & `tmp/honeybee-idaice-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.4.2.tar", last modified: Tue Jun 27 15:55:12 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.4.3.tar", last modified: Thu Jul 27 18:22:09 2023, max compression
```

## Comparing `honeybee-idaice-0.4.2.tar` & `honeybee-idaice-0.4.3.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/bldgbody.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/face.py
--rw-r--r--   0 runner    (1001) docker     (123)    27969 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/shade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 15:55:12.000000 honeybee-idaice-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-27 15:53:47.000000 honeybee-idaice-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/bldgbody.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/shade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20568 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 18:22:09.000000 honeybee-idaice-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-27 18:21:03.000000 honeybee-idaice-0.4.3/setup.py
```

### Comparing `honeybee-idaice-0.4.2/LICENSE` & `honeybee-idaice-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.2/PKG-INFO` & `honeybee-idaice-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.4.2
+Version: 0.4.3
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.4.2/README.md` & `honeybee-idaice-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice/archive.py` & `honeybee-idaice-0.4.3/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice/bldgbody.py` & `honeybee-idaice-0.4.3/honeybee_idaice/bldgbody.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,66 @@
 """A module for functions related to IDM building-bodies."""
 from typing import List
 from ladybug_geometry.bounding import bounding_box
 from ladybug_geometry.geometry3d import Plane, LineSegment3D, Face3D, Point3D
 
+from honeybee.model import Model
 from honeybee.room import Room
 from honeybee.facetype import Floor, RoofCeiling
 
-from .geometry_utils import get_floor_boundary, grouped_horizontal_boundary
-
-
-def _section_to_idm_protected(rooms: List[Room]):
+# constant used by IDA-ICE to determine if a geometry element is exterior
+# geometries within this distance of the building body are considered exterior
+IDA_ICE_BUILDING_BODY_TOL = 0.5  # units are meters
+
+# constant used to group rooms into stories by their floor elevations
+# the value is meant to be lower than the height of any room in the model
+# but not so low that a single step down yields a new Story
+MAX_FLOOR_ELEVATION_DIFFERENCE = 0.2  # units are meters of vertical distance
+
+
+def _section_to_idm_protected(rooms: List[Room], tolerance: float):
+    """Create an IDM building section for a group of non-extruded Rooms.
+
+    Args:
+        rooms: A list of Honeybee Rooms.
+        tolerance: The maximum difference between X, Y, and Z values at which point
+            vertices are considered distinct from one another.
+    """
     if not rooms:
         return ''
     XY_PLANE = Plane()
     sections = []
     for room in rooms:
-        room_section = []
-        try:
-            boundary = grouped_horizontal_boundary([room], min_separation=0)
-            bv = list(boundary.boundary)
-            holes = boundary.holes
-        except Exception:
-            bv, _ = get_floor_boundary(room)
-            holes = None
+        room_section = []  # list of IDM strings to be collected
 
-        if not holes:
-            contours = [bv]
-        else:
-            contours = [bv] + [list(h) for h in holes]
+        # get the horizontal boundary around the Room geometry
+        h_bound = room.horizontal_boundary(match_walls=False, tolerance=tolerance)
+        h_bound = h_bound.remove_colinear_vertices(tolerance)
+        contours = [list(h_bound.boundary)]
+        if h_bound.has_holes:
+            contours.extend([list(h) for h in h_bound.holes])
 
+        # convert the vertices of the boundary into an IDM string
         vc = sum(len(c) for c in contours)
         contours_formatted = ' '.join(str(len(c)) for c in contours)
 
         idm_vertices = ' '.join(f'({v.x} {v.y})' for vv in contours for v in vv)
 
-        min_pt, max_pt = bounding_box(room.geometry)
+        min_pt, max_pt = room.geometry.min, room.geometry.max
 
         header = f'((CE-SECTION :N "{room.display_name}_SEC" :T BUILDING-SECTION)\n' \
             ' (:PAR :N PROTECTED_SHAPE :V :TRUE)\n' \
             f' (:PAR :N NCORN :V {vc})\n' \
             f' (:PAR :N CORNERS :DIM ({vc} 2) :V #2A({idm_vertices}))\n' \
             f' (:PAR :N CONTOURS :V ({contours_formatted}))\n' \
             f' (:PAR :N HEIGHT :V {max_pt.z - min_pt.z})\n' \
             f' (:PAR :N BOTTOM :V {min_pt.z})'
         room_section.append(header)
+
+        # loop through the room faces and add the geometries
         wall_count = 0
         floor_count = 0
         for face in room.faces:
             if isinstance(face.type, Floor):
                 type_ = 'CRAWL-FACE'
                 index = -2000 - floor_count
                 floor_count += 1
@@ -87,46 +100,46 @@
                     f'  (:PAR :N CORNERS :DIM ({vc} 3) :V #2A({vertices_idm}))\n' \
                     f'  (:PAR :N CONTOURS :V ({contours_formatted}))\n' \
                     f'  (:PAR :N SLOPE :V {face.altitude + 90})\n' \
                     '  ((FACE :N GROUND-FACE)\n' \
                     '   (:PAR :N NCORN :V 0)\n' \
                     '   (:PAR :N CORNERS :DIM (0 3))))'
 
-            if type_ == 'WALL-FACE' and min_pt.z < -0.1:
+            if type_ == 'WALL-FACE' and min_pt.z < -tolerance:  # below ground geometry
                 # intersect the edges with the XY plane to create two separate segments
                 geometry = face.geometry
                 lines = geometry.intersect_plane(XY_PLANE)
                 if not lines:
                     room_section.append(body)
                     continue
                 # calculate the top and the bottom segments
                 line = lines[0]
                 pt_1 = line.p1
                 pt_2 = line.p2
                 vertices = list(geometry.upper_right_counter_clockwise_vertices)
                 top_part = [vertices[0]]
                 for vc, v in enumerate(vertices[1:]):
                     line = LineSegment3D.from_end_points(top_part[-1], v)
-                    if line.distance_to_point(pt_1) < 0.001:
+                    if line.distance_to_point(pt_1) < tolerance:
                         top_part.extend([pt_1, pt_2])
                         bottom_part = [pt_2, pt_1]
                         other_point = pt_2
                         break
-                    elif line.distance_to_point(pt_2) < 0.001:
+                    elif line.distance_to_point(pt_2) < tolerance:
                         top_part.extend([pt_2, pt_1])
                         bottom_part = [pt_1, pt_2]
                         other_point = pt_1
                         break
                     top_part.append(v)
 
                 vertices_rev = list(reversed(vertices))[:-1]
                 top_part_2 = [vertices[0]]
                 for c, v in enumerate(vertices_rev):
                     line = LineSegment3D.from_end_points(top_part_2[-1], v)
-                    if line.distance_to_point(other_point) < 0.001:
+                    if line.distance_to_point(other_point) < tolerance:
                         indx = -(c + 1)
                         if indx == -1:
                             top_part = top_part + vertices[indx:-1]
                             bottom_part = bottom_part + vertices[vc + 1:]
                         else:
                             top_part = top_part + vertices[indx + 1:]
                             bottom_part = bottom_part + vertices[vc + 1:indx + 1]
@@ -149,65 +162,89 @@
 
         sections.append('\n'.join(room_section) + ')')
 
     return '\n'.join(sections)
 
 
 def _section_to_idm_extruded(
-    extruded_rooms: List[Room], name: str, max_int_wall_thickness: float = 0.45,
-    height_tolerance: float = 0.5,
-        ):
-    """Create an IDM building section for a group of extruded rooms."""
+    extruded_rooms: List[Room], name: str, max_int_wall_thickness: float,
+    tolerance: float
+):
+    """Create an IDM building section for a group of extruded rooms.
+
+    The input rooms should all be at the same floor height and a part of the
+    same story.
+
+    Args:
+        extruded_rooms: A list of Honeybee Rooms that are all extruded.
+        name: text string to be used as a base name for the section.
+        max_int_wall_thickness: Maximum thickness of the interior wall in meters.
+            Gaps between Rooms that are less than this distance will be grouped
+            into the same building section.
+        tolerance: The maximum difference between X, Y, and Z values at which point
+            vertices are considered distinct from one another.
+    """
     if not extruded_rooms:
         return ''
+
+    # group the rooms according to their floor-to-ceiling heights
     groups = {}
     for room in extruded_rooms:
-        _, max_pt = bounding_box(room.geometry)
+        max_pt = room.geometry.max
         for z in groups:
-            if abs(max_pt.z - z) <= height_tolerance:
+            if abs(max_pt.z - z) <= IDA_ICE_BUILDING_BODY_TOL:
                 groups[z].append(room)
                 break
         else:
             groups[max_pt.z] = [room]
 
+    # convert each group of rooms to a separate building section
     sections = []
     for group_count, rooms in enumerate(groups.values()):
+        # get the bounding box around the rooms
         geometry = [room.geometry for room in rooms]
         min_pt, max_pt = bounding_box(geometry)
         height = max_pt.z
         bottom = min_pt.z
+
+        # compute the grouped horizontal boundary around the rooms
+        fail_msg = 'Failed to calculate the horizontal boundary for level containing ' \
+            f'{rooms[0].display_name}. Will use a bounding box for this floor. In ' \
+            'most cases this is because the input value for maximum wall thickness ' \
+            'is not appropriate for the input model. The current input is ' \
+            f'{max_int_wall_thickness}. For models where the walls between the rooms ' \
+            'are touching this value should be set to 0.\n'
+
         try:
-            boundaries = grouped_horizontal_boundary(
-                rooms, min_separation=max_int_wall_thickness
+            boundaries = Room.grouped_horizontal_boundary(
+                rooms, min_separation=max_int_wall_thickness, tolerance=tolerance
             )
         except Exception as e:
-            print(
-                'Failed to calculate the horizontal boundary for level containing '
-                f'{rooms[0].display_name}. Will use a bounding box for this floor.\n'
-                f'{str(e)}'
-            )
+            print(fail_msg + str(e))
             boundaries = []
 
-        # use bounding box instead as a fallback
+        # if the grouped horizontal boundary failed, use the bounding box as a fallback
         bb_boundaries = [
             Face3D([
                 Point3D(min_pt.x, min_pt.y, bottom), Point3D(max_pt.x, min_pt.y, bottom),
                 Point3D(max_pt.x, max_pt.y, bottom), Point3D(min_pt.x, max_pt.y, bottom)
             ])
         ]
-
-        if not boundaries:
+        if not boundaries:  # the max_int_wall_thickness is likely too large
             boundaries = bb_boundaries
-        else:
-            rooms_area = sum(room.floor_area for room in rooms)
-            boundary_area = sum(b.area for b in boundaries)
-            if abs(1 - (rooms_area / boundary_area)) > 0.2:
-                # the boundary is incorrect
-                boundaries = bb_boundaries
+            print(fail_msg)
+        else:  # make sure that grouped_horizontal_boundary is not self-intersecting
+            for bnd in boundaries:
+                if bnd.is_self_intersecting:
+                    # there were likely overlapping Room boundaries causing failure
+                    boundaries = bb_boundaries
+                    print(fail_msg)
+                    break
 
+        # convert the boundaries into building section strings
         for count, boundary in enumerate(boundaries):
             sec_name = f'{name}_{group_count}_{count}_SEC'
             bv = list(boundary.boundary)
             holes = boundary.holes
             if not holes:
                 contours = [bv]
                 vc = len(bv)
@@ -282,29 +319,41 @@
                 '   (:PAR :N NCORN :V 0)\n' \
                 '   (:PAR :N CORNERS :DIM (0 3) :V #2A()))))'
             sections.append(footer)
 
     return '\n'.join(sections)
 
 
-def section_to_idm(rooms: List[Room], max_int_wall_thickness: float):
-    """Create an IDA-ICE building body for rooms."""
+def section_to_idm(model: Model, max_int_wall_thickness: float):
+    """Create an IDA-ICE building body for a Honeybee Model.
+
+    Args:
+        model: A honeybee model.
+        max_int_wall_thickness: Maximum thickness of the interior wall in meters.
+            Gaps between Rooms that are less than this distance will be grouped
+            into the same building section.
+    """
+    # separate the rooms by floor heights and extruded properties
+    rooms = model.rooms
     sections = []
-    grouped_rooms, floor_heights = Room.group_by_floor_height(rooms, min_difference=0.2)
+    grouped_rooms, floor_heights = \
+        Room.group_by_floor_height(rooms, min_difference=MAX_FLOOR_ELEVATION_DIFFERENCE)
     no_ext_rooms = []
     for grouped_room, height in zip(grouped_rooms, floor_heights):
         ext_rooms = []
         for room in grouped_room:
             if not room.user_data['_idm_is_extruded']:
                 no_ext_rooms.append(room)
             else:
                 ext_rooms.append(room)
+        # generate the bodies for the extruded rooms
         if ext_rooms:
             section = _section_to_idm_extruded(
                 ext_rooms, f'Level_{round(height, 2)}',
-                max_int_wall_thickness=max_int_wall_thickness
+                max_int_wall_thickness=max_int_wall_thickness, tolerance=model.tolerance
             )
             sections.append(section)
 
-    sections_protected = _section_to_idm_protected(no_ext_rooms)
+    # add any non-extruded rooms to the result
+    sections_protected = _section_to_idm_protected(no_ext_rooms, model.tolerance)
     sections.append(sections_protected)
     return '\n'.join(sections) + '\n'
```

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice/shade.py` & `honeybee-idaice-0.4.3/honeybee_idaice/shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.4.3/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.4.3/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.4.3/honeybee_idaice/templates/building.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.4.3/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.4.3/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.4.3/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice/writer.py` & `honeybee-idaice-0.4.3/honeybee_idaice/writer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,158 @@
 """Write an idm file from a HBJSON file."""
+import math
 import pathlib
 import shutil
 from typing import List, Tuple
 
-from honeybee.model import Model, Room, Face
+from ladybug_geometry.bounding import bounding_box
+from ladybug_geometry.geometry2d import Point2D, Polygon2D
+from ladybug_geometry.geometry3d import Point3D, Face3D
+from honeybee.model import Model, Room
 from honeybee.facetype import RoofCeiling, Wall, Floor
-from ladybug_geometry.geometry3d import Point3D
 
 from .archive import zip_folder_to_idm
-from .geometry_utils import get_floor_boundary, get_ceiling_boundary, prepare_apertures
-from .bldgbody import section_to_idm
+from .bldgbody import section_to_idm, MAX_FLOOR_ELEVATION_DIFFERENCE
 from .shade import shades_to_idm
-from .face import face_to_idm, opening_to_idm
+from .face import face_to_idm, opening_to_idm, face_reference_plane
 
 
-def ceilings_to_idm(faces: List[Face], origin: Point3D):
-    """Translate a collection of ceilings face to an IDM ENCLOSING-ELEMENT."""
+def ceilings_to_idm(room: Room, origin: Point3D, tolerance: float,
+                    angle_tolerance: float = 1.0):
+    """Translate the ceilings of a Room to an IDM ENCLOSING-ELEMENT.
+
+    Args:
+        room: A honeybee Room.
+        origin: A Point3D for the origin of the parent Room.
+        tolerance: The minimum difference between x, y, and z coordinate
+            values at which points are considered distinct.
+        angle_tolerance: The max angle in degrees that Face normal can differ
+            from the World Z before the Face is treated as being in the
+            World XY plane. (Default: 1).
+    """
     index = -1000
 
+    # if there's only one ceiling, just translate it
+    faces = room.roof_ceilings
     if len(faces) == 1:
-        return face_to_idm(faces[0], origin, index)
+        return face_to_idm(faces[0], origin, index, angle_tolerance)
 
-    vertices, z_range = get_ceiling_boundary(faces)
-    if z_range[1] - z_range[0] <= 0.01:
+    # check to see the vertical range across the ceilings
+    min_pt, max_pt = bounding_box([face.geometry for face in faces])
+    if max_pt.z - min_pt.z <= tolerance:
         # all the ceilings are the same height
-        return '\n'.join(face_to_idm(face, origin, index) for face in faces)
+        return '\n'.join(
+            face_to_idm(face, origin, index, angle_tolerance) for face in faces
+        )
 
-    # TODO: add support for ceiling parts with holes
+    # get the boundary around all of the ceiling parts
+    horiz_boundary = room.horizontal_boundary(tolerance=tolerance)
+    if horiz_boundary.normal.z <= 0:  # ensure upward-facing Face3D
+        horiz_boundary = horiz_boundary.flip()
+    # insert the vertices of the ceiling elements into the horizontal boundary
+    ceil_pts = [pt for f in faces for pt in f.geometry.boundary]
+    ceil_pts_2d = [Point2D(v[0], v[1]) for v in ceil_pts]
+    st_poly = Polygon2D([Point2D(v.x, v.y) for v in horiz_boundary.boundary])
+    st_poly = st_poly.remove_colinear_vertices(tolerance)
+    polygon_update = []
+    for pt in ceil_pts_2d:
+        for v in st_poly.vertices:  # check if pt is already included
+            if pt.is_equivalent(v, tolerance):
+                break
+        else:
+            values = [seg.distance_to_point(pt) for seg in st_poly.segments]
+            if min(values) < tolerance:
+                index_min = min(range(len(values)), key=values.__getitem__)
+                polygon_update.append((index_min, pt))
+    if polygon_update:
+        st_poly = Polygon2D._insert_updates_in_order(st_poly, polygon_update)
+    vertices = [Point3D(pt.x, pt.y, max_pt.z) for pt in st_poly]
+    full_bound = Face3D(vertices, plane=horiz_boundary.plane)
+    vertices = full_bound.lower_left_counter_clockwise_vertices
+
+    # translate the boundary vertices into an enclosing element
     vertices_idm = ' '.join((
         f'({v.x - origin.x} {v.y - origin.y} {v.z - origin.z})' for v in vertices
     ))
     count = len(vertices)
     ceiling = \
         f'((ENCLOSING-ELEMENT :N CEILING_{faces[0].identifier} :T CEILING :INDEX -1000)\n' \
         ' ((AGGREGATE :N GEOMETRY)\n' \
         f'  (:PAR :N CORNERS :DIM ({count} 3) :SP ({count} 3) :V #2A({vertices_idm})))'
-
     ceiling_idm = [ceiling]
 
+    # write each of the ceiling faces to IDM
     for fc, face in enumerate(faces):
         name = f'{face.identifier}_{fc}'
         holes = face.geometry.holes or []
         contours = [list(face.geometry.boundary)] + [list(h) for h in holes]
         vc = sum(len(c) for c in contours)
         contours_formatted = ' '.join(str(len(c)) for c in contours)
         vertices_idm = ' '.join(
             f'({v.x - origin.x} {v.y - origin.y} {v.z - origin.z})'
             for vv in contours for v in vv
         )
 
         # add apertures
+        ref_plane = face_reference_plane(face, angle_tolerance) \
+            if face.has_sub_faces else None
         windows = ['']
         for aperture in face.apertures:
-            windows.append(opening_to_idm(aperture))
+            windows.append(opening_to_idm(aperture, ref_plane))
 
         windows = ''.join(windows)
 
         cp = f' ((ENCLOSING-ELEMENT :N "{name}" :T CEILING-PART :INDEX {-1001 - fc})\n' \
             '  ((AGGREGATE :N GEOMETRY)\n' \
             f'   (:PAR :N CORNERS :DIM ({vc} 3) :SP ({vc} 3) :V #2A({vertices_idm}))\n' \
             f'   (:PAR :N CONTOURS :V ({contours_formatted}))\n' \
             f'   (:PAR :N SLOPE :V {face.altitude + 90})){windows})'
         ceiling_idm.append(cp)
 
     return '\n'.join(ceiling_idm) + ')'
 
 
-def room_to_idm(room: Room):
-    """Translate a Honeybee Room to an IDM Zone."""
+def room_to_idm(room: Room, tolerance: float, angle_tolerance: float = 1.0):
+    """Translate a Honeybee Room to an IDM Zone.
+
+    Args:
+        room: A honeybee Room.
+        tolerance: The minimum difference between x, y, and z coordinate
+            values at which points are considered distinct.
+        angle_tolerance: The max angle in degrees that Face normal can differ
+            from the World Z before the Face is treated as being in the
+            World XY plane. (Default: 1).
+    """
     room_idm = []
 
-    # find floor boundary and llc for origin
-    vertices, pole = get_floor_boundary(room)
-    origin = vertices[0]
+    # find horizontal boundary around the Room
+    horiz_boundary: Face3D = \
+        room.horizontal_boundary(match_walls=True, tolerance=tolerance)
+    holes = horiz_boundary.holes or []
+    contours = [list(horiz_boundary.boundary)] + [list(h) for h in holes]
+    if holes:
+        contours_formatted = ' '.join(str(len(c)) for c in contours)
+    else:
+        contours_formatted = ''
+
+    # create a flatten list for vertices
+    vertices = [v for vl in contours for v in vl]
+
+    if horiz_boundary.normal.z <= 0:  # ensure upward-facing Face3D
+        horiz_boundary = horiz_boundary.flip()
+    if horiz_boundary.has_holes:  # remove any holes from the result
+        horiz_boundary = Face3D(horiz_boundary.boundary, plane=horiz_boundary.plane)
+
+    # get the lower-left corner and a point for the center
+    ordered_vertices = horiz_boundary.lower_left_counter_clockwise_vertices
+    origin = ordered_vertices[0]
+    if horiz_boundary.is_convex:
+        pole = horiz_boundary.center
+    else:  # use a 1 cm tolerance for pole that will not be time consuming to compute
+        pole = horiz_boundary.pole_of_inaccessibility(0.01)
 
     # relative coordinates of the pole
     rp = pole - origin
     # arbitrary x and y size for lighting fixtures
     lighting_x = 0.5
     lighting_y = 0.5
     min_x = rp.x - lighting_x / 2
@@ -104,20 +180,22 @@
 
     if not room.user_data['_idm_is_extruded']:
         geometry = '((AGGREGATE :N GEOMETRY :X NIL)\n' \
             ' (:PAR :N PROTECTED_SHAPE :V :TRUE)\n' \
             f' (:PAR :N ORIGIN :V #({origin.x} {origin.y}))\n' \
             f' (:PAR :N NCORN :V {count})\n' \
             f' (:PAR :N CORNERS :DIM ({count} 2) :V #2A({vertices_idm}))\n' \
+            f' (:PAR :N CONTOURS :V ({contours_formatted}))\n' \
             f' (:PAR :N FLOOR_HEIGHT_FROM_GROUND :V {elevation}))'
     else:
         geometry = '((AGGREGATE :N GEOMETRY :X NIL)\n' \
             f' (:PAR :N ORIGIN :V #({origin.x} {origin.y}))\n' \
             f' (:PAR :N NCORN :V {count})\n' \
             f' (:PAR :N CORNERS :DIM ({count} 2) :V #2A({vertices_idm}))\n' \
+            f' (:PAR :N CONTOURS :V ({contours_formatted}))\n' \
             f' (:PAR :N CEILING-HEIGHT :V {room.user_data["_idm_flr_ceil_height"]})\n' \
             f' (:PAR :N FLOOR_HEIGHT_FROM_GROUND :V {elevation}))'
 
     room_idm.append(geometry)
 
     walls, ceilings, floors = deconstruct_room(room)
     # write faces
@@ -129,22 +207,28 @@
         index = vertices.index(sorted_vertices[0]) + 1
         if index in used_index:
             # this is a vertical segment of a wall with the same starting point.
             # use a new index and hope it doesn't have an aperture
             index = last_index
             last_index += 1
         used_index.append(index)
-        face_idm = face_to_idm(wall, origin=origin, index=index)
+        face_idm = face_to_idm(
+            wall, origin=origin, index=index, angle_tolerance=angle_tolerance
+        )
         room_idm.append(face_idm)
 
     for count, floor in enumerate(floors):
-        face_idm = face_to_idm(floor, origin=origin, index=-(2000 + count))
+        face_idm = face_to_idm(
+            floor, origin=origin, index=-(2000 + count), angle_tolerance=angle_tolerance
+        )
         room_idm.append(face_idm)
 
-    ceiling_idm = ceilings_to_idm(ceilings, origin=origin)
+    ceiling_idm = ceilings_to_idm(
+        room, origin=origin, tolerance=tolerance, angle_tolerance=angle_tolerance
+    )
     room_idm.append(ceiling_idm)
 
     return '\n'.join(room_idm)
 
 
 def deconstruct_room(room: Room):
     """Deconstruct a room into walls, ceilings and floors."""
@@ -160,98 +244,105 @@
         else:
             # TODO: support air boundaries
             walls.append(face)
 
     return walls, ceilings, floors
 
 
-def _is_room_extruded(room: Room) -> Tuple:
-    """Check if the room geometry is an extrusion in Z direction."""
+def _is_room_extruded(room: Room, angle_tolerance: float) -> Tuple:
+    """Check if the room geometry is an extrusion in Z direction.
+
+    Args:
+        room: A honeybee Room.
+        angle_tolerance: The max angle difference in degrees that the normals of
+            Faces are allowed to differ from vertical/horizontal for the Room
+            to not be considered extruded.
+    """
     f_h = 0
     c_h = 0
     for face in room.faces:
         type_ = face.type
         if isinstance(type_, Wall):
-            if abs(face.altitude) > 5:
+            if abs(face.altitude) > angle_tolerance:
                 return False, -1
         elif isinstance(type_, RoofCeiling):
-            if abs(90 - face.altitude) > 5:
+            if abs(90 - face.altitude) > angle_tolerance:
                 return False, -1
             c_h = face.vertices[0].z
         elif isinstance(type_, Floor):
-            if abs(face.altitude + 90) > 5:
+            if abs(face.altitude + 90) > angle_tolerance:
                 return False, -1
             f_h = face.vertices[0].z
 
     return True, round(c_h - f_h, 2)
 
 
-def prepare_model(model: Model) -> Model:
-    """This function prepares the model for translation to IDM.
+def prepare_model(model: Model, max_int_wall_thickness: float = 0.45) -> Model:
+    """Perform a number of model edits to prepare it for translation to IDM.
 
-    * Ensures the model is meters
-    * Check room display names and ensures they are unique
+    * Check room display names and ensure they are unique
     * Mark rooms as extruded and non-extruded
     * Mark doors and apertures in the model to avoid writing duplicated doors and
       apertures
 
+    Args:
+        model: A honeybee model.
+        max_int_wall_thickness: Maximum thickness of the interior wall in meters.
+            This will be used to identify adjacent interior doors and apertures
+            in the model to ensure that only one version of the geometry
+            is written to IDA-ICE. (Default: 0.45).
     """
-    model.convert_to_units(units='Meters')
-
-    try:
-        model.remove_degenerate_geometry()
-    except ValueError as e:
-        # most likely an error with the units. It may or may not become a problem
-        # for IDA-ICE so let's continue the process.
-        print(str(e))
-
-    for face in model.faces:
-        if face.apertures:
-            face._apertures = prepare_apertures(face.apertures)
-
+    # difference in normal angles that make apertures/doors adjacent
+    min_ang = math.pi - math.radians(model.angle_tolerance)
+    # ensure unique room names for each story and make a note of adjacencies
     room_names = {}
-    grouped_rooms, _ = Room.group_by_floor_height(model.rooms, min_difference=0.2)
-    door_adj_tol = 0.75  # assuming the door centers are not closer than this distance
+    grouped_rooms, _ = Room.group_by_floor_height(
+        model.rooms, min_difference=MAX_FLOOR_ELEVATION_DIFFERENCE)
     door_tracker = []
     aperture_tracker = []
     for grouped_room in grouped_rooms:
         for room in grouped_room:
             # check the display name and change it if it is not unique
             room.display_name = \
                 room.display_name.replace('/', '-').replace('\\', '-').replace('\n', ' ')
             if room.display_name in room_names:
                 original_name = room.display_name
                 room.display_name = \
                     f'{room.display_name}_{room_names[original_name]}'
                 room_names[original_name] += 1
             else:
                 room_names[room.display_name] = 1
-            is_extruded, floor_to_ceiling_height = _is_room_extruded(room)
+            # add markers for whether the Room is extruded or not
+            is_extruded, floor_to_ceiling_height = \
+                _is_room_extruded(room, model.angle_tolerance)
             room.user_data = {
                 '_idm_is_extruded': is_extruded,
                 '_idm_flr_ceil_height': floor_to_ceiling_height
             }
+            # add markers so adjacent interior Apertures and Doors are not duplicated
             for face in room.faces:
                 for door in face.doors:
                     center = door.geometry.center
-                    for pt in door_tracker:
-                        if pt.distance_to_point(center) <= door_adj_tol:
+                    normal = door.geometry.normal
+                    for data in door_tracker:
+                        c, n = data
+                        if c.distance_to_point(center) <= max_int_wall_thickness \
+                                and n.angle(normal) > min_ang:
                             door.user_data = {'_idm_ignore': True}
                             break
-                    door_tracker.append(center)
+                    door_tracker.append((center, normal))
                 for aperture in face.apertures:
                     center = aperture.geometry.center
                     normal = aperture.geometry.normal
                     for data in aperture_tracker:
                         c, n = data
-                        if c.distance_to_point(center) <= door_adj_tol \
-                                and abs(n.angle(normal) - 3.14159) < 0.1:
+                        if c.distance_to_point(center) <= max_int_wall_thickness \
+                                and n.angle(normal) > min_ang:
                             aperture.user_data = {'_idm_ignore': True}
                     aperture_tracker.append((center, normal))
-    return model
 
 
 def prepare_folder(bldg_name: str, out_folder: str) -> List[pathlib.Path]:
     """Prepare folders for IDM file."""
     base_folder = pathlib.Path(out_folder)
     model_folder = base_folder.joinpath(bldg_name)
     if model_folder.exists():
@@ -261,33 +352,68 @@
     bldg_folder = model_folder.joinpath(f'{bldg_name}')
     bldg_folder.mkdir(parents=True, exist_ok=True)
     bldg_file = model_folder.joinpath(f'{bldg_name}.idm')
 
     return base_folder, model_folder, bldg_folder, bldg_file
 
 
-def model_to_idm(model: Model, out_folder: pathlib.Path, name: str = None,
-                 max_int_wall_thickness: int = 0.45, debug: bool = False):
+def model_to_idm(
+        model: Model, out_folder: pathlib.Path, name: str = None,
+        max_int_wall_thickness: float = 0.40, max_adjacent_sub_face_dist: float = 0.40,
+        max_frame_thickness: float = 0.1, debug: bool = False):
     """Translate a Honeybee model to an IDM file.
 
     Args:
         model: A honeybee model.
         out_folder: Output folder for idm file.
         name: Output IDM file name.
         max_int_wall_thickness: Maximum thickness of the interior wall in meters. IDA-ICE
             expects the input model to have a gap between the rooms that represents
-            the wall thickness. For models where the walls are touching each other use
-            the values of 0.
+            the wall thickness. This value must be smaller than the smallest Room
+            that is expected in resulting IDA-ICE model and it should never be greater
+            than 0.5 in order to avoid creating invalid building bodies for IDA-ICE.
+            For models where the walls are touching each other, use a value
+            of 0. (Default: 0.40).
+        max_adjacent_sub_face_dist: The maximum distance in meters between interior
+            Apertures and Doors at which they are considered adjacent. This is used to
+            ensure that only one interior Aperture of an adjacent pair is written into
+            the IDM. This value should typically be around the max_int_wall_thickness
+            and should ideally not be thicker than 0.5. But it may be undesirable to
+            set this to zero (like some cases of max_int_wall_thickness),
+            particularly when the adjacent interior geometries are not matching
+            one another. (Default: 0.40).
+        max_frame_thickness: Maximum thickness of the window frame in meters.
+            This will be used to join any non-rectangular Apertures together in
+            an attempt to better rectangularize them for IDM. (Default: 0.1).
         debug: Set to True to not to delete the IDM folder before zipping it into a
             single file.
     """
+    # check for the presence of rooms
     if not model.rooms:
-        raise ValueError('The input model should at least have one room.')
+        raise ValueError(
+            'The model must have at least have one room to translate to IDM.')
 
-    model = prepare_model(model)
+    # duplicate model to avoid mutating it as we edit it for export
+    # otherwise, we'll loose the original model if we want to do anything after export
+    model = model.duplicate()
+
+    # scale the model if the units are not meters
+    if model.units != 'Meters':
+        model.convert_to_units('Meters')
+    # remove degenerate geometry within the model tolerance
+    model.remove_degenerate_geometry()
+    # convert all apertures to be rectangular, using the model tolerances
+    ap_dist = max_frame_thickness if max_frame_thickness > model.tolerance \
+        else model.tolerance
+    model.rectangularize_apertures(max_separation=ap_dist, resolve_adjacency=False)
+
+    # edit the model display_names and add user_data to help with the translation
+    adj_dist = max_adjacent_sub_face_dist \
+        if max_adjacent_sub_face_dist > model.tolerance else model.tolerance
+    prepare_model(model, adj_dist)
 
     # make sure names don't have subfolder or extension
     original_name = name or model.display_name
     name = pathlib.Path(original_name).stem
     bldg_name = name or model.display_name
 
     base_folder, model_folder, bldg_folder, bldg_file = \
@@ -304,15 +430,15 @@
         # add template values
         bldg_template = templates_folder.joinpath('building.idm')
         for line in bldg_template.open('r'):
             bldg.write(line)
 
         # create a building sections/bodies for the building
         sections = section_to_idm(
-            model.rooms, max_int_wall_thickness=max_int_wall_thickness
+            model, max_int_wall_thickness=max_int_wall_thickness
         )
         bldg.write(sections)
 
         # add reference to rooms as zones
         for room in model.rooms:
             bldg.write(f'((CE-ZONE :N "{room.display_name}" :T ZONE))\n')
 
@@ -335,15 +461,15 @@
     template_room = templates_folder.joinpath('room.idm')
     for room in model.rooms:
         room_name = room.display_name
         room_file = bldg_folder.joinpath(f'{room_name}.idm')
         with template_room.open('r') as inf, room_file.open('w') as rm:
             for line in inf:
                 rm.write(f'{line.rstrip()}\n')
-            geometry = room_to_idm(room)
+            geometry = room_to_idm(room, model.tolerance, model.angle_tolerance)
             rm.write(geometry)
             footer = f'\n;[end of {bldg_name}\\{room_name}.idm]\n'
             rm.write(footer)
 
     if not original_name.endswith('.idm'):
         original_name = f'{original_name}.idm'
     idm_file = base_folder.joinpath(original_name)
```

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.4.3/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.4.3/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.4.2
+Version: 0.4.3
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.4.2/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.4.3/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 setup.py
 honeybee_idaice/__init__.py
 honeybee_idaice/__main__.py
 honeybee_idaice/_extend_honeybee.py
 honeybee_idaice/archive.py
 honeybee_idaice/bldgbody.py
 honeybee_idaice/face.py
-honeybee_idaice/geometry_utils.py
 honeybee_idaice/shade.py
 honeybee_idaice/writer.py
 honeybee_idaice/writer_obj.py
 honeybee_idaice.egg-info/PKG-INFO
 honeybee_idaice.egg-info/SOURCES.txt
 honeybee_idaice.egg-info/dependency_links.txt
 honeybee_idaice.egg-info/entry_points.txt
```

### Comparing `honeybee-idaice-0.4.2/setup.py` & `honeybee-idaice-0.4.3/setup.py`

 * *Files identical despite different names*

