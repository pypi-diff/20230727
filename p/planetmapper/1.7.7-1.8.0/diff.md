# Comparing `tmp/planetmapper-1.7.7.tar.gz` & `tmp/planetmapper-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.7.7.tar", last modified: Mon Jul 10 15:58:57 2023, max compression
+gzip compressed data, was "planetmapper-1.8.0.tar", last modified: Thu Jul 27 08:48:10 2023, max compression
```

## Comparing `planetmapper-1.7.7.tar` & `planetmapper-1.8.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:58:57.960238 planetmapper-1.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-10 15:58:45.000000 planetmapper-1.7.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-10 15:58:57.960238 planetmapper-1.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-10 15:58:45.000000 planetmapper-1.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:58:57.956238 planetmapper-1.7.7/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    81538 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (123)   112443 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:58:57.960238 planetmapper-1.7.7/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/data/ring_aliases.json
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   119046 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    46648 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-07-10 15:58:45.000000 planetmapper-1.7.7/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:58:57.956238 planetmapper-1.7.7/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-10 15:58:57.000000 planetmapper-1.7.7/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-10 15:58:57.000000 planetmapper-1.7.7/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:58:57.000000 planetmapper-1.7.7/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 15:58:57.000000 planetmapper-1.7.7/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 15:58:57.000000 planetmapper-1.7.7/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 15:58:57.000000 planetmapper-1.7.7/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-10 15:58:45.000000 planetmapper-1.7.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:58:57.960238 planetmapper-1.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-10 15:58:45.000000 planetmapper-1.7.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:58:57.960238 planetmapper-1.7.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    35990 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    41788 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    29465 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-10 15:58:45.000000 planetmapper-1.7.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:48:10.325588 planetmapper-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 08:47:55.000000 planetmapper-1.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-27 08:48:10.325588 planetmapper-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-27 08:47:55.000000 planetmapper-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:48:10.321588 planetmapper-1.8.0/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88165 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122224 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:48:10.321588 planetmapper-1.8.0/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/data/ring_aliases.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119118 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52908 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-07-27 08:47:55.000000 planetmapper-1.8.0/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:48:10.321588 planetmapper-1.8.0/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-27 08:48:10.000000 planetmapper-1.8.0/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-27 08:48:10.000000 planetmapper-1.8.0/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:48:10.000000 planetmapper-1.8.0/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 08:48:10.000000 planetmapper-1.8.0/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 08:48:10.000000 planetmapper-1.8.0/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 08:48:10.000000 planetmapper-1.8.0/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-27 08:47:55.000000 planetmapper-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 08:48:10.325588 planetmapper-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-27 08:47:55.000000 planetmapper-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:48:10.325588 planetmapper-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-07-27 08:47:55.000000 planetmapper-1.8.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-27 08:47:55.000000 planetmapper-1.8.0/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44067 2023-07-27 08:47:55.000000 planetmapper-1.8.0/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54197 2023-07-27 08:47:55.000000 planetmapper-1.8.0/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-27 08:47:55.000000 planetmapper-1.8.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-27 08:47:55.000000 planetmapper-1.8.0/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 08:47:55.000000 planetmapper-1.8.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-27 08:47:55.000000 planetmapper-1.8.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-27 08:47:55.000000 planetmapper-1.8.0/tests/test_kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-07-27 08:47:55.000000 planetmapper-1.8.0/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-27 08:47:55.000000 planetmapper-1.8.0/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-27 08:47:55.000000 planetmapper-1.8.0/tests/test_utils.py
```

### Comparing `planetmapper-1.7.7/LICENSE.txt` & `planetmapper-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/PKG-INFO` & `planetmapper-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.7
+Version: 1.8.0
 Summary: PlanetMapper: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
```

### Comparing `planetmapper-1.7.7/README.md` & `planetmapper-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/planetmapper/__init__.py` & `planetmapper-1.8.0/planetmapper/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/planetmapper/base.py` & `planetmapper-1.8.0/planetmapper/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import functools
 import glob
+import math
 import numbers
 import os
 from collections.abc import Iterable
 from pathlib import Path
 from typing import (
     Any,
     Callable,
@@ -644,14 +645,21 @@
             observer_frame=self.observer_frame,
         )
 
     def _obsvec2radec_radians(self, obsvec: np.ndarray) -> tuple[float, float]:
         """
         Transform rectangular vector in observer frame to observer ra/dec coordinates.
         """
+        if not (
+            math.isfinite(obsvec[0])
+            and math.isfinite(obsvec[1])
+            and math.isfinite(obsvec[2])
+        ):
+            # ^ profiling suggests this is the fastest NaN check
+            return np.nan, np.nan
         _, ra, dec = spice.recrad(obsvec)
         return ra, dec
 
 
 def load_kernels(*paths, clear_before: bool = False) -> list[str]:
     """
     Load spice kernels defined by patterns.
```

### Comparing `planetmapper-1.7.7/planetmapper/basic_body.py` & `planetmapper-1.8.0/planetmapper/basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/planetmapper/body.py` & `planetmapper-1.8.0/planetmapper/body.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 except ImportError:
     from typing_extensions import Unpack
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
+import math
+
 import matplotlib.patheffects as path_effects
 import matplotlib.pyplot as plt
 import matplotlib.transforms
 import numpy as np
 import spiceypy as spice
 from matplotlib.axes import Axes
 from spiceypy.utils.exceptions import (
     NotFoundError,
     SpiceBODIESNOTDISTINCT,
+    SpiceINVALIDTARGET,
     SpiceKERNELVARNOTFOUND,
     SpiceSPKINSUFFDATA,
 )
 
 from . import data_loader, utils
 from .base import BodyBase, Numeric
 from .basic_body import BasicBody
@@ -192,14 +195,16 @@
         """Method used to calculate surface intercepts in SPICE."""
         self.et: float
         """Ephemeris time of the observation corresponding to `utc`."""
         self.dtm: datetime.datetime
         """Python timezone aware datetime of the observation corresponding to `utc`."""
         self.target_body_id: int
         """SPICE numeric ID of the target body."""
+        self.radii: np.ndarray
+        """Array of radii of the target body along the x, y and z axes in km."""
         self.r_eq: float
         """Equatorial radius of the target body in km."""
         self.r_polar: float
         """Polar radius of the target body in km."""
         self.flattening: float
         """Flattening of target body, calculated as `(r_eq - r_polar) / r_eq`."""
         self.prograde: bool
@@ -229,14 +234,18 @@
         """Equatorial angular diameter of the target in arcseconds."""
         self.subpoint_distance: float
         """Distance from the observer to the sub-observer point on the target."""
         self.subpoint_lon: float
         """Longitude of the sub-observer point on the target."""
         self.subpoint_lat: float
         """Latitude of the sub-observer point on the target."""
+        self.subsol_lon: float
+        """Longitude of the sub-solar point on the target."""
+        self.subsol_lat: float
+        """Latitude of the sub-solar point on the target."""
         self.named_ring_data: dict[str, list[float]]
         """
         Dictionary of ring radii for the target from :func:`data_loader.get_ring_radii`.
 
         The dictionary keys are the names of the rings, and values are list of ring 
         radii in km. If the length of this list is 2, then the values give the inner and 
         outer radii of the ring respectively. Otherwise, the length should be 1, meaning
@@ -347,14 +356,30 @@
         self._subpoint_obsvec = self._rayvec2obsvec(
             self._subpoint_rayvec, self._subpoint_et
         )
         self._subpoint_ra, self._subpoint_dec = self._radian_pair2degrees(
             *self._obsvec2radec_radians(self._subpoint_obsvec)
         )
 
+        # Find sub solar point
+        try:
+            self._subsol_targvec, self._subsol_et, self._subsol_rayvec = spice.subslr(
+                self._subpoint_method_encoded,  # type: ignore
+                self._target_encoded,  # type: ignore
+                self.et,
+                self._target_frame_encoded,  # type: ignore
+                self._aberration_correction_encoded,  # type: ignore
+                self._observer_encoded,  # type: ignore
+            )
+            self.subsol_lon, self.subsol_lat = self.targvec2lonlat(self._subsol_targvec)
+        except SpiceINVALIDTARGET:
+            # If the target is the sun, then there is no sub-solar point
+            self.subsol_lon = np.nan
+            self.subsol_lat = np.nan
+
         # Set up equatorial plane (for ring calculations)
         targvec_north_pole = self.lonlat2targvec(0, 90)
         obsvec_north_pole = self._targvec2obsvec(targvec_north_pole)
         self._ring_plane = spice.nvp2pl(
             obsvec_north_pole - self._target_obsvec,
             self._target_obsvec,
         )
@@ -617,14 +642,16 @@
     # Coordinate transformations target -> observer direction
     def _lonlat2targvec_radians(
         self, lon: float, lat: float, alt: float = 0
     ) -> np.ndarray:
         """
         Transform lon/lat coordinates on body to rectangular vector in target frame.
         """
+        if not (math.isfinite(lon) and math.isfinite(lat) and math.isfinite(alt)):
+            return np.array([np.nan, np.nan, np.nan])
         return spice.pgrrec(
             self._target_encoded,  # type: ignore
             lon,
             lat,
             alt,  # type: ignore
             self.r_eq,
             self.flattening,
@@ -674,14 +701,16 @@
             et,
             self.et,
         )
         return np.matmul(px, rayvec)
 
     # Coordinate transformations observer -> target direction
     def _radec2obsvec_norm_radians(self, ra: float, dec: float) -> np.ndarray:
+        if not (math.isfinite(ra) and math.isfinite(dec)):
+            return np.array([np.nan, np.nan, np.nan])
         return spice.radrec(1, ra, dec)
 
     def _obsvec2targvec(self, obsvec: np.ndarray) -> np.ndarray:
         """
         Transform rectangular vector in observer frame to rectangular vector in target
         frame.
 
@@ -727,14 +756,21 @@
             self._observer_encoded,
             self._observer_frame_encoded,
             obsvec_norm,
         )
         return spoint
 
     def _targvec2lonlat_radians(self, targvec: np.ndarray) -> tuple[float, float]:
+        if not (
+            math.isfinite(targvec[0])
+            and math.isfinite(targvec[1])
+            and math.isfinite(targvec[2])
+        ):
+            # ^ profiling suggests this is the fastest NaN check
+            return np.nan, np.nan
         lon, lat, alt = spice.recpgr(
             self._target_encoded,  # type: ignore
             targvec,
             self.r_eq,
             self.flattening,
         )
         return lon, lat
@@ -1036,14 +1072,21 @@
             transform = transform + ax.transData
         return transform
 
     # General
     def _illumf_from_targvec_radians(
         self, targvec: np.ndarray
     ) -> tuple[float, float, float, bool, bool]:
+        if not (
+            math.isfinite(targvec[0])
+            and math.isfinite(targvec[1])
+            and math.isfinite(targvec[2])
+        ):
+            # ^ profiling suggests this is the fastest NaN check
+            return np.nan, np.nan, np.nan, False, False
         trgepc, srfvec, phase, incdnc, emissn, visibl, lit = spice.illumf(
             self._surface_method_encoded,  # type: ignore
             self._target_encoded,  # type: ignore
             self._illumination_source_encoded,  # type: ignore
             self.et,
             self._target_frame_encoded,  # type: ignore
             self._aberration_correction_encoded,  # type: ignore
@@ -1120,14 +1163,73 @@
                 ra_night[idx] = np.nan
                 dec_night[idx] = np.nan
             else:
                 ra_day[idx] = np.nan
                 dec_day[idx] = np.nan
         return ra_day, dec_day, ra_night, dec_night
 
+    def limb_coordinates_from_radec(
+        self, ra: float, dec: float
+    ) -> tuple[float, float, float]:
+        """
+        Calculate the coordinates relative to the target body's limb for a point in the
+        sky.
+
+        The coordinates are calculated for the point on the ray (as defined by RA/Dec)
+        which is closest to the target body's limb.
+
+        Args:
+            ra: Right ascension of point in the sky of the observer.
+            dec: Declination of point in the sky of the observer.
+
+        Returns:
+            `(lon, lat, dist)` tuple of coordinates relative to the target body's limb.
+            `lon` and `lat` give the planetographic longitude and latitude of the point
+            on the limb closest to the point defined by `ra` and `dec`. `dist` gives the
+            distance from the point defined by `ra` and `dec` to the target's limb.
+            Positive values of `dist` mean that the point is above the limb and negative
+            values mean that the point is below the limb (i.e. on the target body's
+            disc).
+        """
+        coords = self._limb_coordinates_from_obsvec(
+            self._radec2obsvec_norm_radians(*self._degree_pair2radians(ra, dec))
+        )
+        return coords
+
+    def _limb_coordinates_from_obsvec(
+        self, obsvec_norm: np.ndarray
+    ) -> tuple[float, float, float]:
+        if not (
+            math.isfinite(obsvec_norm[0])
+            and math.isfinite(obsvec_norm[1])
+            and math.isfinite(obsvec_norm[2])
+        ):
+            return np.nan, np.nan, np.nan
+
+        # Get the point on the RA/Dec ray (defined be obsvec_norm) that is closest to
+        # the centre of the target body.
+        nearpoint_obsvec, nearpoint_dist = spice.nplnpt(
+            np.array([0, 0, 0]),  # centre of observer
+            obsvec_norm,  # direction vector from observer to POI
+            self._target_obsvec,  # reference point at centre of target body
+        )
+
+        # Get the point on the surface of the target body that is closest to the
+        # nearpoint.
+        surface_targvec = spice.surfpt(
+            np.array([0, 0, 0]),
+            self._obsvec2targvec(nearpoint_obsvec),
+            self.radii[0],
+            self.radii[1],
+            self.radii[2],
+        )
+        lon, lat = self.targvec2lonlat(surface_targvec)
+        dist = nearpoint_dist - self.vector_magnitude(surface_targvec)
+        return lon, lat, dist
+
     # Visibility
     def _test_if_targvec_visible(self, targvec: np.ndarray) -> bool:
         phase, incdnc, emissn, visibl, lit = self._illumf_from_targvec_radians(targvec)
         return visibl
 
     def test_if_lonlat_visible(self, lon: float, lat: float) -> bool:
         """
@@ -1300,14 +1402,67 @@
         azimuth_radians = self._azimuth_angle_from_gie_radians(
             *self._illumination_angles_from_targvec_radians(
                 self.lonlat2targvec(lon, lat)
             )
         )
         return np.rad2deg(azimuth_radians)
 
+    def _lst_from_lon(
+        self, lon: float
+    ) -> tuple[int | float, int | float, int | float, str, str]:
+        if not math.isfinite(lon):
+            return np.nan, np.nan, np.nan, '', ''
+        return spice.et2lst(
+            self.et - self.target_light_time,
+            self.target_body_id,
+            np.deg2rad(lon),
+            'planetographic',
+        )
+
+    def local_solar_time_from_lon(self, lon: float) -> float:
+        """
+        Calculate the numerical local solar time for a longitude on the target body. For
+        example, `0.0` corresponds to midnight and `12.5` corresponds to 12:30pm.
+
+        See also :func:`local_solar_time_string_from_lon`.
+
+        .. note::
+
+            A 'local hour' of solar time is a defined as 1/24th of the solar day on the
+            target body, so will not correspond to a 'normal' hour as measured by a
+            clock. See
+            `the SPICE documentation <https://naif.jpl.nasa.gov/pub/naif/toolkit_docs/C/cspice/et2lst_c.html>`__
+            for more details.
+
+        Args:
+            lon: Longitude of point on target body.
+
+        Returns:
+            Numerical local solar time in 'local hours'.
+        """
+        hr, mn, sc, time, ampm = self._lst_from_lon(lon)
+        return hr + mn / 60 + sc / 3600
+
+    def local_solar_time_string_from_lon(self, lon: float) -> str:
+        """
+        Local solar time string representation for a longitude on the target body. For
+        example, `'00:00:00'` corresponds to midnight and `'12:30:00'` corresponds to
+        12:30pm.
+
+        See :func:`local_solar_time_from_lon` for more details.
+
+        Args:
+            lon: Longitude of point on target body.
+
+        Returns:
+            String representation of local solar time.
+        """
+        hr, mn, sc, time, ampm = self._lst_from_lon(lon)
+        return time
+
     def terminator_radec(
         self,
         npts: int = 360,
         only_visible: bool = True,
         close_loop: bool = True,
         method: str = 'UMBRAL/TANGENT/ELLIPSOID',
         corloc: str = 'ELLIPSOID TERMINATOR',
@@ -1370,14 +1525,20 @@
         """
         return self._test_if_targvec_illuminated(self.lonlat2targvec(lon, lat))
 
     # Rings
     def _ring_coordinates_from_obsvec(
         self, obsvec: np.ndarray, only_visible: bool = True
     ) -> tuple[float, float, float]:
+        if not (
+            math.isfinite(obsvec[0])
+            and math.isfinite(obsvec[1])
+            and math.isfinite(obsvec[2])
+        ):
+            return np.nan, np.nan, np.nan
         nxpts, intercept_obsvec = spice.inrypl(
             np.array([0, 0, 0]), obsvec, self._ring_plane
         )
         if nxpts != 1:
             return np.nan, np.nan, np.nan
         targvec = self._obsvec2targvec(intercept_obsvec)
         lon, lat, alt = spice.recpgr(
@@ -1653,14 +1814,20 @@
             Distance of the point in km.
         """
         position, velocity, lt = self._state_from_targvec(self.lonlat2targvec(lon, lat))
         return lt * self.speed_of_light()
 
     # Planetographic <-> planetocentric
     def _targvec2lonlat_centric(self, targvec: np.ndarray) -> tuple[float, float]:
+        if not (
+            math.isfinite(targvec[0])
+            and math.isfinite(targvec[1])
+            and math.isfinite(targvec[2])
+        ):
+            return np.nan, np.nan
         radius, lon_centric, lat_centric = spice.reclat(targvec)
         return self._radian_pair2degrees(lon_centric, lat_centric)
 
     def graphic2centric_lonlat(self, lon: float, lat: float) -> tuple[float, float]:
         """
         Convert planetographic longitude/latitude to planetocentric.
 
@@ -1682,22 +1849,24 @@
         Args:
             lon_centric: Planetocentric longitude.
             lat_centric: Planetographic latitude.
 
         Returns:
             `(lon, lat)` tuple of planetographic coordinates.
         """
-        targvec = spice.latsrf(
+        if not (math.isfinite(lon_centric) and math.isfinite(lat_centric)):
+            return np.nan, np.nan
+        targvecs = spice.latsrf(
             self._surface_method_encoded,  # type: ignore
             self._target_encoded,  # type: ignore
             self.et,
             self._target_frame_encoded,  # type: ignore
             [[np.deg2rad(lon_centric), np.deg2rad(lat_centric)]],
         )
-        return self.targvec2lonlat(targvec[0])
+        return self.targvec2lonlat(targvecs[0])
 
     # Other
     def north_pole_angle(self) -> float:
         """
         Calculate the angle of the north pole of the target body relative to the
         positive declination direction.
```

### Comparing `planetmapper-1.7.7/planetmapper/body_xy.py` & `planetmapper-1.8.0/planetmapper/body_xy.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     lon: float
     lat: float
     size: int
     lon_coords: np.ndarray
     lat_coords: np.ndarray
     projection_x_coords: np.ndarray
     projection_y_coords: np.ndarray | None
+    xlim: tuple[float, float] | None
+    ylim: tuple[float, float] | None
 
 
 class _BackplaneMapGetter(Protocol):
     def __call__(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         ...
 
 
@@ -70,20 +72,18 @@
     Args:
         name: Short name identifying the backplane. This is used as the `EXTNAME` for
             the backplane when saving FITS files in :func:`Observation.save`.
         description: More detailed description of the backplane (e.g. including units).
         get_img: Function which takes no arguments returns a numpy array containing a
             backplane image when called. This should generally be a method such as
             :func:`BodyXY.get_lon_img`.
-        get_map: Function returns a numpy array containing a cylindrical map of
-            backplane values when called. This should take a single `float` argument,
-            `degree_interval` which defines the interval in degrees between the
-            longitude/latitude points in the mapped output. `degree_interval` should be
-            optional with a default value of 1. This function should generally be a
-            method such as :func:`BodyXY.get_lon_map`.
+        get_map: Function returns a numpy array containing a map of backplane values
+            when called. This should take map projection keyword arguments, as described
+            in :func:`BodyXY.generate_map_coordinates`. This function should generally
+            be a method such as :func:`BodyXY.get_lon_map`.
     """
 
     name: str
     description: str
     get_img: Callable[[], np.ndarray]
     get_map: _BackplaneMapGetter
 
@@ -681,15 +681,15 @@
 
         Returns:
             `(nx, ny)` tuple containing the number of pixels in the x and y dimension of
             the image respectively
         """
         return (self._nx, self._ny)
 
-    def set_disc_method(self, method: str):
+    def set_disc_method(self, method: str) -> None:
         """
         Record the method used to find the coordinates of the target body's disc. This
         recorded method can then be used when metadata is saved, such as in
         :func:`Observation.save`.
 
         `set_disc_method` is called automatically by functions which find the disc, such
         as :func:`set_x0` and :func:`Observation.centre_disc`, so does not normally need
@@ -1154,15 +1154,15 @@
         projection = map_kw_used['projection']
 
         ax.set_aspect(1, adjustable=aspect_adjustable)
 
         lon_ticks = np.arange(0, 360.0001, grid_interval)
         lat_ticks = np.arange(-90, 90.0001, grid_interval)
 
-        if projection == 'azimuthal':
+        if projection in {'azimuthal', 'azimuthal equal area'}:
             # Run separately for either side of equator to reduce issues for azimuthal
             # where the grid lines overplot each other. We still can get issues for e.g.
             # lat=45, but this fixes the most common cases of lat=0,90,-90 and it's a
             # relatively minor cosmetic bug so is probably more-or-less fine as-is.
             npts = 360
             lats_to_plot = [np.linspace(-90, 0, npts), np.linspace(0, 90, npts)]
         else:
@@ -1203,15 +1203,15 @@
             # Elipse boundary - https://math.stackexchange.com/questions/91132
             x0 = 1
             b = self.r_polar / self.r_eq
             theta = np.radians(map_kw_used['lat'])
             y0 = np.sqrt((np.sin(theta)) ** 2 + b**2 * (np.cos(theta)) ** 2)
             t = np.linspace(0, -2 * np.pi, 100)
             boundary = (x0 * np.cos(t), y0 * np.sin(t))
-        elif projection == 'azimuthal':
+        elif projection in {'azimuthal', 'azimuthal equal area'}:
             # Circular boundary
             x0 = y0 = 1
             t = np.linspace(0, -2 * np.pi, 100)
             boundary = (x0 * np.cos(t), y0 * np.sin(t))
 
         if boundary:
             ax.plot(*boundary, **kwargs['map_boundary'])
@@ -1240,15 +1240,15 @@
                     [f'{x:.0f}°' if x % 90 == 0 else '' for x in lon_ticks]
                 )
 
                 ax.set_yticks(lat_ticks)
                 ax.set_yticklabels(
                     [f'{y:.0f}°' if y % 90 == 0 else '' for y in lat_ticks]
                 )
-            elif projection in {'orthographic', 'azimuthal'}:
+            elif projection in {'orthographic', 'azimuthal', 'azimuthal equal area'}:
                 ax.set_xticks([])
                 ax.set_yticks([])
 
         if add_title:
             ax.set_title(self.get_description(multiline=True))
         return ax
 
@@ -1470,16 +1470,15 @@
         ny = yy.shape[0]
 
         def plot_fn(ax: Axes):
             self.plot_map_wireframe(
                 ax=ax,
                 add_axis_labels=False,
                 add_title=False,
-                **(plot_kwargs or {})
-                | dict(common_formatting=dict(color='k')),  # type:ignore
+                **(plot_kwargs or {}) | dict(common_formatting=dict(color='k')),
                 **map_kwargs,
             )
             # Add dx/dy to the limits to ensure the wireframe covers all of each pixel
             # as the xx and yy coordinates only give the centre of each pixel
             dx = abs(xx[0][1] - xx[0][0]) / 2
             ax.set_xlim(np.nanmin(xx) - dx, np.nanmax(xx) + dx)
             dy = abs(yy[1][0] - yy[0][0]) / 2
@@ -1720,14 +1719,16 @@
         lon: float = 0,
         lat: float = 0,
         size: int = 100,
         lon_coords: np.ndarray | tuple | None = None,
         lat_coords: np.ndarray | tuple | None = None,
         projection_x_coords: np.ndarray | tuple | None = None,
         projection_y_coords: np.ndarray | tuple | None = None,
+        xlim: tuple[float, float] | None = None,
+        ylim: tuple[float, float] | None = None,
     ) -> tuple[
         np.ndarray,
         np.ndarray,
         np.ndarray,
         np.ndarray,
         pyproj.Transformer,
         dict[str, Any],
@@ -1744,14 +1745,17 @@
           points. This is the default map projection.
         - `'orthographic'`: orthographic projection where the central longitude and
           latitude can be customized with the `lon` and `lat` arguments. The size of the
           map can be controlled with the `size` argument.
         - `'azimuthal'`: azimuthal equidistant projection where the central longitude
           and latitude can be customized with the `lon` and `lat` arguments. The size of
           the map can be controlled with the `size` argument.
+        - `'azimuthal equal area'`: Lambert azimuthal equal area projection where the
+          central longitude and latitude can be customized with the `lon` and `lat`
+          arguments. The size of the map can be controlled with the `size` argument.
         - `'manual'`: manually specify the longitude and latitude coordinates to use
           for each point on the map with the `lon_coords` and `lat_coords` arguments.
 
         Projections can also be specified by passing a pyproj projection string to the
         `projection` argument. If you are manually specifying a projection, you must
         also specify `projection_x_coords` and `projection_y_coords` to provide the x
         and y coordinates to project the data to. See
@@ -1765,132 +1769,181 @@
             :func:`map_img`.
 
         Usage examples: ::
 
             # Generate default rectangular map for emission backplane
             body.get_backplane_map('EMISSION')
 
-            # Generate default rectangular map at lower resolution
-            body.get_backplane_map('EMISSION', degree_interval=10)
+            # Generate default rectangular map at lower resolution and only covering
+            # the northern hemisphere
+            body.get_backplane_map('EMISSION', degree_interval=10, ylim=(0, np.inf))
 
             # Generate orthographic map of northern hemisphere
             body.get_backplane_map('EMISSION', projection='orthographic', lat=90)
 
             # Plot orthographic map of southern hemisphere with higher resolution
             body.plot_backplane_map(
                 'EMISSION', projection='orthographic', lat=-90, size=500
                 )
 
-            # Get azimuthal map projection of image, centred on specific coordinate
+            # Get azimuthal equidistant map projection of image, centred on specific
+            # coordinate
             body.map_img(img, projection='azimuthal', lon=45, lat=30)
 
         Args:
             projection: String describing map projection to use (see list of supported
                 projections above).
             degree_interval: Degree interval for `'rectangular` projection.
-            lon: Central longitude of `'orthographic'` and `'azimuthal'` projections.
-            lat: Central latitude of `'orthographic'` and `'azimuthal'` projections.
-            size: Pixel size (width and height) of generated `'orthographic'` and
-                `'azimuthal'` projections.
+            lon: Central longitude of `'orthographic'`, `'azimuthal'` and `'azimuthal
+                equal area'` projections.
+            lat: Central latitude of `'orthographic'`, `'azimuthal'` and `'azimuthal
+                equal area'` projections.
+            size: Pixel size (width and height) of generated `'orthographic'`,
+                `'azimuthal'` and `'azimuthal equal area'` projections.
             lon_coords: Longitude coordinates to use for `'manual'` projection. This
                 must be a tuple (e.g. use `lon_coords=tuple(np.linspace(0, 360, 100))`)
                 - this allows mapping arguments and outputs to be cached).
             lat_coords: Latitude coordinates to use for `'manual'` projection. This
                 must be a tuple.
             projection_x_coords: Projected x coordinates to use with a pyproj projection
                 string. This must be a tuple.
             projection_y_coords: Projected x coordinates to use with a pyproj projection
                 string. This must be a tuple.
+            xlim: Tuple of `(x_min, x_max)` limits in the projected x coordinates of
+                the map. If `None`, the default, then the no limits are applied (i.e.
+                the entire globe will be mapped). If `xlim` is provided, it should be a
+                tuple of two floats specifying the minimum and maximum x coordinates to
+                project the map to. For example, to only plot the western hemisphere,
+                you can use use `xlim=(0, 180)` in a rectangular projection. Note that
+                these limits are expressed in the projected coordinates of the map.
+                Setting the limits can be useful to speed up the performance of mapping
+                when only a subset of the map is needed (such as for observations with
+                limited spatial extent). If you only want to set one limit, then you can
+                pass infinity e.g. `xlim=(315, np.inf)` to only set the minimum limit.
+                The limits are implemented using
+                `x_to_keep = (x >= min(xlim)) & (x <= max(xlim))`, so the ordering of
+                the limits does not matter. Note that the limit calculations assume that
+                the data is on a rectangular grid (i.e. all rows have the same x
+                coordinates and all columns have the same y coordinates), so may produce
+                unexpected results if a custom projection is used.
+            ylim: Tuple of `(y_min, y_max)` limits in the projected y coordinates of
+                the map. If `None`, the default, then the no limits are applied. See
+                `xlim` for more details.
 
         Returns:
             `(lons, lats, xx, yy, transformer, info)` tuple where `lons` and `lats` are
             the longitude and latitude coordinates of the map, `xx` and `yy` are the
             projected coordinates of the map, `transformer` is a `pyproj.Transformer`
             object that can be used to transform between the two coordinate systems, and
             `info` is a dictionary containing the arguments used to build the map (e.g.
-            for the default case this is
-            `{'projection': 'rectangular', 'degree_interval': 1}`).
+            for the default case this would be `{'projection': 'rectangular',
+            'degree_interval': 1, 'xlim': None, 'ylim': None}`).
         """
         info: dict[str, Any]  # Explicitly declare type of info to make pyright happy
         if projection == 'rectangular':
-            lon_coords = np.arange(degree_interval / 2, 360, degree_interval)
+            lons = np.arange(degree_interval / 2, 360, degree_interval)
             if self.positive_longitude_direction == 'W':
-                lon_coords = lon_coords[::-1]
-            lat_coords = np.arange(-90 + degree_interval / 2, 90, degree_interval)
-            lon_coords, lat_coords = np.meshgrid(lon_coords, lat_coords)
+                lons = lons[::-1]
+            lats = np.arange(-90 + degree_interval / 2, 90, degree_interval)
+            lons, lats = np.meshgrid(lons, lats)
+            xx, yy = lons, lats
+            transformer = self._get_pyproj_transformer()
             info = dict(projection=projection, degree_interval=degree_interval)
-            return (
-                lon_coords,
-                lat_coords,
-                lon_coords,
-                lat_coords,
-                self._get_pyproj_transformer(),
-                info,
-            )
         elif projection == 'manual':
-            if lon_coords is None or lat_coords is None:
-                raise ValueError('lons and lats must be provided for manual projection')
-            lon_coords = np.asarray(lon_coords)
-            lat_coords = np.asarray(lat_coords)
-            if lon_coords.ndim != lat_coords.ndim:
+            lons = lon_coords
+            lats = lat_coords
+            if lons is None or lats is None:
+                raise ValueError(
+                    'lon_coords and lat_coords must be provided for manual projection'
+                )
+            lons = np.asarray(lons)
+            lats = np.asarray(lats)
+            if lons.ndim != lats.ndim:
                 raise ValueError(
                     'lon_coords and lat_coords must have the same number of dimensions'
                 )
-            if lon_coords.ndim == 1:
-                lon_coords, lat_coords = np.meshgrid(lon_coords, lat_coords)
-            if lon_coords.ndim != 2:
+            if lons.ndim == 1:
+                lons, lats = np.meshgrid(lons, lats)
+            if lons.ndim != 2:
                 raise ValueError('lon_coords and lat_coords must be 1D or 2D arrays')
-            if lon_coords.shape != lat_coords.shape:
+            if lons.shape != lats.shape:
                 raise ValueError('lon_coords and lat_coords must have the same shape')
+            xx, yy = lons, lats
+            transformer = self._get_pyproj_transformer()
             info = dict(projection=projection)
-            return (
-                lon_coords,
-                lat_coords,
-                lon_coords,
-                lat_coords,
-                self._get_pyproj_transformer(),
-                info,
-            )
         elif projection == 'orthographic':
             b = self.r_polar / self.r_eq
             proj = '+proj=ortho +a={a} +b={b} +lon_0={lon_0} +lat_0={lat_0} +y_0={y_0} +type=crs'.format(
                 a=1,
                 b=b,
                 lon_0=lon,
                 lat_0=lat,
                 y_0=(b - 1) * np.sin(np.radians(lat * 2)),
             )
             lim = max(1, b) * 1.01
-            info = dict(projection=projection, lon=lon, lat=lat, size=size)
-            return (
-                *self._get_pyproj_map_coords(proj, np.linspace(-lim, lim, size)),
-                info,
+            lons, lats, xx, yy, transformer = self._get_pyproj_map_coords(
+                proj, np.linspace(-lim, lim, size)
             )
+            info = dict(projection=projection, lon=lon, lat=lat, size=size)
         elif projection == 'azimuthal':
             proj = '+proj=aeqd +R={a} +lon_0={lon_0} +lat_0={lat_0} +type=crs'.format(
                 a=1 / np.pi,
                 lon_0=lon,
                 lat_0=lat,
             )
             lim = 1.01
+            lons, lats, xx, yy, transformer = self._get_pyproj_map_coords(
+                proj, np.linspace(-lim, lim, size)
+            )
             info = dict(projection=projection, lon=lon, lat=lat, size=size)
-            return (
-                *self._get_pyproj_map_coords(proj, np.linspace(-lim, lim, size)),
-                info,
+        elif projection == 'azimuthal equal area':
+            proj = '+proj=laea +R={a} +lon_0={lon_0} +lat_0={lat_0} +type=crs'.format(
+                a=1 / 2,
+                lon_0=lon,
+                lat_0=lat,
+            )
+            lim = 1.01
+            lons, lats, xx, yy, transformer = self._get_pyproj_map_coords(
+                proj, np.linspace(-lim, lim, size)
             )
+            info = dict(projection=projection, lon=lon, lat=lat, size=size)
         else:
             if projection_x_coords is None:
                 raise ValueError('x coords must be provided')
-            info = dict(projection=projection)
-            return (
-                *self._get_pyproj_map_coords(
-                    projection, projection_x_coords, projection_y_coords
-                ),
-                info,
+            lons, lats, xx, yy, transformer = self._get_pyproj_map_coords(
+                projection, projection_x_coords, projection_y_coords
             )
+            info = dict(
+                projection=projection,
+                projection_x_coords=projection_x_coords,
+                projection_y_coords=projection_y_coords,
+            )
+
+        info['xlim'] = xlim
+        info['ylim'] = ylim
+        if xlim is not None:
+            x_arr = xx[0]
+            x_to_keep = (x_arr >= min(xlim)) & (x_arr <= max(xlim))
+            xx = xx[:, x_to_keep]
+            yy = yy[:, x_to_keep]
+            lons = lons[:, x_to_keep]
+            lats = lats[:, x_to_keep]
+        if ylim is not None:
+            y_arr = yy[:, 0]
+            y_to_keep = (y_arr >= min(ylim)) & (y_arr <= max(ylim))
+            xx = xx[y_to_keep, :]
+            yy = yy[y_to_keep, :]
+            lons = lons[y_to_keep, :]
+            lats = lats[y_to_keep, :]
+
+        # Standardise invalid lon/lat points (e.g. inf -> nan)
+        lons[~np.isfinite(lons)] = np.nan
+        lats[~np.isfinite(lats)] = np.nan
+
+        return lons, lats, xx, yy, transformer, info
 
     def _get_pyproj_map_coords(
         self,
         projection: str,
         xx: np.ndarray | tuple,
         yy: np.ndarray | tuple | None = None,
     ) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, pyproj.Transformer]:
@@ -2035,14 +2088,32 @@
             targvec = targvec_map[a, b]
             if math.isnan(targvec[0]):
                 # only check if first element nan for efficiency
                 continue
             yield a, b, targvec_map[a, b]
 
     @_cache_clearable_result
+    def _get_obsvec_norm_img(self) -> np.ndarray:
+        out = self._make_empty_img(3)
+        ra_img = self.get_ra_img()
+        dec_img = self.get_dec_img()
+        for y, x in self._iterate_image(out.shape):
+            out[y, x] = self._radec2obsvec_norm_radians(
+                *self._degree_pair2radians(ra_img[y, x], dec_img[y, x])
+            )
+        return out
+
+    @_cache_stable_result
+    def _get_obsvec_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
+        out = self._make_empty_map(3, **map_kwargs)
+        for a, b, targvec in self._enumerate_targvec_map(**map_kwargs):
+            out[a, b] = self._targvec2obsvec(targvec)
+        return out
+
+    @_cache_clearable_result
     @progress_decorator
     def _get_lonlat_img(self) -> np.ndarray:
         out = self._make_empty_img(2)
         for y, x, targvec in self._enumerate_targvec_img(progress=True):
             out[y, x] = self._targvec2lonlat_radians(targvec)
         return np.rad2deg(out)
 
@@ -2068,15 +2139,15 @@
 
     def get_lon_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of planetographic longitude values.
+            Array containing map of planetographic longitude values.
         """
         return self._get_lonlat_map(**map_kwargs)[:, :, 0]
 
     def get_lat_img(self) -> np.ndarray:
         """
         See also :func:`get_backplane_img`.
 
@@ -2088,15 +2159,15 @@
 
     def get_lat_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of planetographic latitude values.
+            Array containing map of planetographic latitude values.
         """
         return self._get_lonlat_map(**map_kwargs)[:, :, 1]
 
     @_cache_clearable_result
     @progress_decorator
     def _get_lonlat_centric_img(self) -> np.ndarray:
         out = self._make_empty_img(2)
@@ -2124,15 +2195,15 @@
 
     def get_lon_centric_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of planetocentric longitude values.
+            Array containing map of planetocentric longitude values.
         """
         return self._get_lonlat_centric_map(**map_kwargs)[:, :, 0]
 
     def get_lat_centric_img(self) -> np.ndarray:
         """
         See also :func:`get_backplane_img`.
 
@@ -2144,15 +2215,15 @@
 
     def get_lat_centric_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of planetocentric latitude values.
+            Array containing map of planetocentric latitude values.
         """
         return self._get_lonlat_centric_map(**map_kwargs)[:, :, 1]
 
     @_cache_clearable_result
     @progress_decorator
     def _get_radec_img(self) -> np.ndarray:
         out = self._make_empty_img(2)
@@ -2161,17 +2232,19 @@
         return np.rad2deg(out)
 
     @_cache_stable_result
     @progress_decorator
     def _get_radec_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         out = self._make_empty_map(2, **map_kwargs)
         visible = self._get_illumf_map(**map_kwargs)[:, :, 4]
+        obsvec_map = self._get_obsvec_map(**map_kwargs)
         for a, b, targvec in self._enumerate_targvec_map(progress=True, **map_kwargs):
+            # use targvec iterator to ensure don't have NaNs
             if visible[a, b]:
-                out[a, b] = self._obsvec2radec_radians(self._targvec2obsvec(targvec))
+                out[a, b] = self._obsvec2radec_radians(obsvec_map[a, b])
         return np.rad2deg(out)
 
     def get_ra_img(self) -> np.ndarray:
         """
         See also :func:`get_backplane_img`.
 
         Returns:
@@ -2181,16 +2254,16 @@
 
     def get_ra_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of right ascension values as viewed by the
-            observer. Locations which are not visible have a value of NaN.
+            Array containing map of right ascension values as viewed by the observer.
+            Locations which are not visible have a value of NaN.
         """
         return self._get_radec_map(**map_kwargs)[:, :, 0]
 
     def get_dec_img(self) -> np.ndarray:
         """
         See also :func:`get_backplane_img`.
 
@@ -2201,16 +2274,16 @@
 
     def get_dec_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of declination values as viewed by the
-            observer. Locations which are not visible have a value of NaN.
+            Array containing map of declination values as viewed by the observer.
+            Locations which are not visible have a value of NaN.
         """
         return self._get_radec_map(**map_kwargs)[:, :, 1]
 
     @_cache_clearable_result
     @progress_decorator
     def _get_xy_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         out = self._make_empty_map(2, **map_kwargs)
@@ -2237,17 +2310,17 @@
 
     def get_x_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the x pixel coordinates each location
-            corresponds to in the observation. Locations which are not visible or are
-            not in the image frame have a value of NaN.
+            Array containing map of the x pixel coordinates each location corresponds to
+            in the observation. Locations which are not visible or are not in the image
+            frame have a value of NaN.
         """
         return self._get_xy_map(**map_kwargs)[:, :, 0]
 
     def get_y_img(self) -> np.ndarray:
         """
         See also :func:`get_backplane_img`.
 
@@ -2261,17 +2334,17 @@
 
     def get_y_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the y pixel coordinates each location
-            corresponds to in the observation. Locations which are not visible or are
-            not in the image frame have a value of NaN.
+            Array containing map of the y pixel coordinates each location corresponds to
+            in the observation. Locations which are not visible or are not in the image
+            frame have a value of NaN.
         """
         return self._get_xy_map(**map_kwargs)[:, :, 1]
 
     @_cache_clearable_result
     def _get_km_xy_img(self) -> np.ndarray:
         out = self._make_empty_img(2)
         radec_img = self._get_radec_img()
@@ -2301,17 +2374,16 @@
 
     def get_km_x_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the distance in target plane in km in
-            the East-West direction. Locations which are not visible have a value of
-            NaN.
+            Array containing map of the distance in target plane in km in the East-West
+            direction. Locations which are not visible have a value of NaN.
         """
         return self._get_km_xy_map(**map_kwargs)[:, :, 0]
 
     def get_km_y_img(self) -> np.ndarray:
         """
         See also :func:`get_backplane_img`.
 
@@ -2323,17 +2395,16 @@
 
     def get_km_y_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the distance in target plane in km in
-            the North-South direction. Locations which are not visible have a value of
-            NaN.
+            Array containing map of the distance in target plane in km in the
+            North-South direction. Locations which are not visible have a value of NaN.
         """
         return self._get_km_xy_map(**map_kwargs)[:, :, 1]
 
     @_cache_clearable_result
     @progress_decorator
     def _get_illumination_gie_img(self) -> np.ndarray:
         out = self._make_empty_img(3)
@@ -2361,16 +2432,16 @@
 
     def get_phase_angle_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the phase angle value at each point on
-            the target's surface.
+            Array containing map of the phase angle value at each point on the target's
+            surface.
         """
         return self._get_illumf_map(**map_kwargs)[:, :, 0]
 
     def get_incidence_angle_img(self) -> np.ndarray:
         """
         See also :func:`get_backplane_img`.
 
@@ -2382,16 +2453,16 @@
 
     def get_incidence_angle_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the incidence angle value at each point
-            on the target's surface.
+            Array containing map of the incidence angle value at each point on the
+            target's surface.
         """
         return self._get_illumf_map(**map_kwargs)[:, :, 1]
 
     def get_emission_angle_img(self) -> np.ndarray:
         """
         See also :func:`get_backplane_img`.
 
@@ -2403,16 +2474,16 @@
 
     def get_emission_angle_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the emission angle value at each point
-            on the target's surface.
+            Array containing map of the emission angle value at each point on the
+            target's surface.
         """
         return self._get_illumf_map(**map_kwargs)[:, :, 2]
 
     @_cache_clearable_result
     def get_azimuth_angle_img(self) -> np.ndarray:
         """
         See also :func:`get_backplane_img`.
@@ -2435,30 +2506,68 @@
     @_cache_stable_result
     def get_azimuth_angle_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the azimuth angle value at each point
-            on the target's surface.
+            Array containing map of the azimuth angle value at each point on the
+            target's surface.
         """
         phase_radians = np.deg2rad(self._get_illumf_map(**map_kwargs)[:, :, 0])
         incidence_radians = np.deg2rad(self._get_illumf_map(**map_kwargs)[:, :, 1])
         emission_radians = np.deg2rad(self._get_illumf_map(**map_kwargs)[:, :, 2])
         with warnings.catch_warnings():
             warnings.filterwarnings('ignore', 'divide by zero encountered in')
             warnings.filterwarnings('ignore', 'invalid value encountered in')
             azimuth_radians = self._azimuth_angle_from_gie_radians(
                 phase_radians, incidence_radians, emission_radians
             )
         return np.rad2deg(azimuth_radians)
 
     @_cache_clearable_result
     @progress_decorator
+    def get_local_solar_time_img(self) -> np.ndarray:
+        """
+        See also :func:`get_backplane_img`.
+
+        Returns:
+            Array containing the local solar time value of each pixel in the image, as
+            calculated by :func:`Body.local_solar_time_from_lon`. Points off the disc
+            have a value of NaN.
+        """
+        lon_img = self.get_lon_img()
+        out = self._make_empty_img()
+        for y, x in self._iterate_image(out.shape, progress=True):
+            lon = lon_img[y, x]
+            if not math.isnan(lon):
+                out[y, x] = self.local_solar_time_from_lon(lon)
+        return out
+
+    @_cache_stable_result
+    @progress_decorator
+    def get_local_solar_time_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
+        """
+        See :func:`generate_map_coordinates` for accepted arguments. See also
+        :func:`get_backplane_map`.
+
+        Returns:
+            Array containing map of the local solar time at each point on the target's
+            surface, as calculated by :func:`Body.local_solar_time_from_lon`.
+        """
+        lon_map = self.get_lon_map(**map_kwargs)
+        out = self._make_empty_map(**map_kwargs)
+        for a, b in self._iterate_image(out.shape, progress=True):
+            lon = lon_map[a, b]
+            if math.isfinite(lon):
+                out[a, b] = self.local_solar_time_from_lon(lon)
+        return out
+
+    @_cache_clearable_result
+    @progress_decorator
     def _get_state_imgs(self) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
         position_img = self._make_empty_img(3)
         velocity_img = self._make_empty_img(3)
         lt_img = self._make_empty_img()
         for y, x, targvec in self._enumerate_targvec_img(progress=True):
             (
                 position_img[y, x],
@@ -2496,16 +2605,16 @@
 
     def get_distance_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the observer-target distance in km of
-            each point on the target's surface.
+            Array containing map of the observer-target distance in km of each point on
+            the target's surface.
         """
         position_map, velocity_map, lt_map = self._get_state_maps(**map_kwargs)
         return lt_map * self.speed_of_light()
 
     @_cache_clearable_result
     @progress_decorator
     def get_radial_velocity_img(self) -> np.ndarray:
@@ -2529,16 +2638,16 @@
     @progress_decorator
     def get_radial_velocity_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the observer-target radial velocity in
-            km/s of each point on the target's surface.
+            Array containing map of the observer-target radial velocity in km/s of each
+            point on the target's surface.
         """
         out = self._make_empty_map(**map_kwargs)
         position_map, velocity_map, lt_map = self._get_state_maps(**map_kwargs)
         for a, b, targvec in self._enumerate_targvec_map(progress=True, **map_kwargs):
             out[a, b] = self._radial_velocity_from_state(
                 position_map[a, b], velocity_map[a, b]
             )
@@ -2557,35 +2666,122 @@
 
     def get_doppler_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the doppler factor of each point on the
-            target's surface. This is calculated using
-            :func:`SpiceBase.calculate_doppler_factor` on velocities from
-            :func:`get_radial_velocity_map`.
+            Array containing map of the doppler factor of each point on the target's
+            surface. This is calculated using :func:`SpiceBase.calculate_doppler_factor`
+            on velocities from :func:`get_radial_velocity_map`.
         """
         return self.calculate_doppler_factor(self.get_radial_velocity_map(**map_kwargs))
 
     @_cache_clearable_result
     @progress_decorator
+    def _get_limb_coordinate_imgs(self) -> np.ndarray:
+        out = self._make_empty_img(3)
+        obsvec_img = self._get_obsvec_norm_img()
+        for y, x in self._iterate_image(out.shape, progress=True):
+            obsvec = obsvec_img[y, x]
+            out[y, x] = self._limb_coordinates_from_obsvec(obsvec)
+        return out
+
+    @_cache_stable_result
+    @progress_decorator
+    def _get_limb_coordinate_maps(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
+        out = self._make_empty_map(3, **map_kwargs)
+        visible = self._get_illumf_map(**map_kwargs)[:, :, 4]
+        obsvec_map = self._get_obsvec_map(**map_kwargs)
+        for a, b, targvec in self._enumerate_targvec_map(progress=True, **map_kwargs):
+            if visible[a, b]:
+                out[a, b] = self._limb_coordinates_from_obsvec(obsvec_map[a, b])
+        return out
+
+    def get_limb_lon_img(self) -> np.ndarray:
+        """
+        See also :func:`get_backplane_img`.
+
+        Returns:
+            Array containing the planetographic longitude of the point on the target's
+            limb that is closest to each pixel. See
+            :func:`Body.limb_coordinates_from_radec` for more detail.
+        """
+        return self._get_limb_coordinate_imgs()[:, :, 0]
+
+    def get_limb_lon_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
+        """
+        See :func:`generate_map_coordinates` for accepted arguments. See also
+        :func:`get_backplane_map`.
+
+        Returns:
+            Array containing map of the planetographic longitude of the point on the
+            target's limb that is closest to each point on the target's surface (for the
+            observer). See :func:`Body.limb_coordinates_from_radec` for more detail.
+        """
+        return self._get_limb_coordinate_maps(**map_kwargs)[:, :, 0]
+
+    def get_limb_lat_img(self) -> np.ndarray:
+        """
+        See also :func:`get_backplane_img`.
+
+        Returns:
+            Array containing the planetographic latitude of the point on the target's
+            limb that is closest to each pixel. See
+            :func:`Body.limb_coordinates_from_radec` for more detail.
+        """
+        return self._get_limb_coordinate_imgs()[:, :, 1]
+
+    def get_limb_lat_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
+        """
+        See :func:`generate_map_coordinates` for accepted arguments. See also
+        :func:`get_backplane_map`.
+
+        Returns:
+            Array containing map of the planetographic latitude of the point on the
+            target's limb that is closest to each point on the target's surface (for the
+            observer). See :func:`Body.limb_coordinates_from_radec` for more detail.
+        """
+        return self._get_limb_coordinate_maps(**map_kwargs)[:, :, 1]
+
+    def get_limb_distance_img(self) -> np.ndarray:
+        """
+        See also :func:`get_backplane_img`.
+
+        Returns:
+            Array containing the distance in km above the target's limb for each pixel.
+            See :func:`Body.limb_coordinates_from_radec` for more detail.
+        """
+        return self._get_limb_coordinate_imgs()[:, :, 2]
+
+    def get_limb_distance_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
+        """
+        See :func:`generate_map_coordinates` for accepted arguments. See also
+        :func:`get_backplane_map`.
+
+        Returns:
+            Array containing map of the distance in km above the target's limb for each
+            point on the target's surface (for the observer). See
+            :func:`Body.limb_coordinates_from_radec` for more detail.
+        """
+        return self._get_limb_coordinate_maps(**map_kwargs)[:, :, 2]
+
+    @_cache_clearable_result
+    @progress_decorator
     def _get_ring_plane_coordinate_imgs(
         self,
     ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
         radius_img = self._make_empty_img()
         long_img = self._make_empty_img()
         dist_img = self._make_empty_img()
 
-        ra_img = self.get_ra_img()
-        dec_img = self.get_dec_img()
+        obsvec_img = self._get_obsvec_norm_img()
         for y, x in self._iterate_image(radius_img.shape, progress=True):
-            radius, long, dist = self.ring_plane_coordinates(
-                ra_img[y, x], dec_img[y, x], only_visible=False
+            radius, long, dist = self._ring_coordinates_from_obsvec(
+                obsvec_img[y, x], only_visible=False
             )
             radius_img[y, x] = radius
             long_img[y, x] = long
             dist_img[y, x] = dist
 
         hidden_img = dist_img > self.get_distance_img()
         radius_img[hidden_img] = np.nan
@@ -2599,20 +2795,19 @@
         self, **map_kwargs: Unpack[_MapKwargs]
     ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
         radius_map = self._make_empty_map(**map_kwargs)
         long_map = self._make_empty_map(**map_kwargs)
         dist_map = self._make_empty_map(**map_kwargs)
 
         visible = self._get_illumf_map(**map_kwargs)[:, :, 4]
-        ra_map = self.get_ra_map(**map_kwargs)
-        dec_map = self.get_dec_map(**map_kwargs)
+        obsvec_map = self._get_obsvec_map(**map_kwargs)
         for a, b, targvec in self._enumerate_targvec_map(progress=True, **map_kwargs):
             if visible[a, b]:
-                radius, long, dist = self.ring_plane_coordinates(
-                    ra_map[a, b], dec_map[a, b], only_visible=False
+                radius, long, dist = self._ring_coordinates_from_obsvec(
+                    obsvec_map[a, b], only_visible=False
                 )
                 radius_map[a, b] = radius
                 long_map[a, b] = long
                 dist_map[a, b] = dist
 
         hidden_map = dist_map > self.get_distance_map(**map_kwargs)
         radius_map[hidden_map] = np.nan
@@ -2633,18 +2828,18 @@
 
     def get_ring_plane_radius_map(self, **map_kwargs: Unpack[_MapKwargs]) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the ring plane radius in km obscuring
-            each point on the target's surface, calculated using
-            :func:`Body.ring_plane_coordinates`. Points where the target body is
-            unobscured by the ring plane have a value of NaN.
+            Array containing map of the ring plane radius in km obscuring each point on
+            the target's surface, calculated using :func:`Body.ring_plane_coordinates`.
+            Points where the target body is unobscured by the ring plane have a value of
+            NaN.
         """
         return self._get_ring_plane_coordinate_maps(**map_kwargs)[0]
 
     def get_ring_plane_longitude_img(self) -> np.ndarray:
         """
         See also :func:`get_backplane_img`.
 
@@ -2659,16 +2854,16 @@
         self, **map_kwargs: Unpack[_MapKwargs]
     ) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the ring plane planetographic longitude
-            in degrees obscuring each point on the target's surface, calculated using
+            Array containing map of the ring plane planetographic longitude in degrees
+            obscuring each point on the target's surface, calculated using
             :func:`Body.ring_plane_coordinates`. Points where the target body is
             unobscured by the ring plane have a value of NaN.
         """
         return self._get_ring_plane_coordinate_maps(**map_kwargs)[1]
 
     def get_ring_plane_distance_img(self) -> np.ndarray:
         """
@@ -2685,17 +2880,17 @@
         self, **map_kwargs: Unpack[_MapKwargs]
     ) -> np.ndarray:
         """
         See :func:`generate_map_coordinates` for accepted arguments. See also
         :func:`get_backplane_map`.
 
         Returns:
-            Array containing cylindrical map of the ring plane distance from the
-            observer in km obscuring each point on the target's surface, calculated
-            using  :func:`Body.ring_plane_coordinates`. Points where the target body is
+            Array containing map of the ring plane distance from the observer in km
+            obscuring each point on the target's surface, calculated using
+            :func:`Body.ring_plane_coordinates`. Points where the target body is
             unobscured by the ring plane have a value of NaN.
         """
         return self._get_ring_plane_coordinate_maps(**map_kwargs)[2]
 
     # Default backplane registration
     def _register_default_backplanes(self) -> None:
         self.register_backplane(
@@ -2781,14 +2976,20 @@
         self.register_backplane(
             'AZIMUTH',
             'Azimuth angle [deg]',
             self.get_azimuth_angle_img,
             self.get_azimuth_angle_map,
         )
         self.register_backplane(
+            'LOCAL-SOLAR-TIME',
+            'Local solar time [local hours]',
+            self.get_local_solar_time_img,
+            self.get_local_solar_time_map,
+        )
+        self.register_backplane(
             'DISTANCE',
             'Distance to observer [km]',
             self.get_distance_img,
             self.get_distance_map,
         )
         self.register_backplane(
             'RADIAL-VELOCITY',
@@ -2799,14 +3000,32 @@
         self.register_backplane(
             'DOPPLER',
             'Doppler factor, sqrt((1 + v/c)/(1 - v/c)) where v is radial velocity',
             self.get_doppler_img,
             self.get_doppler_map,
         )
         self.register_backplane(
+            'LIMB-DISTANCE',
+            'Distance above limb [km]',
+            self.get_limb_distance_img,
+            self.get_limb_distance_map,
+        )
+        self.register_backplane(
+            'LIMB-LON-GRAPHIC',
+            'Planetographic longitude of closest point on the limb [deg]',
+            self.get_limb_lon_img,
+            self.get_limb_lon_map,
+        )
+        self.register_backplane(
+            'LIMB-LAT-GRAPHIC',
+            'Planetographic latitude of closest point on the limb [deg]',
+            self.get_limb_lat_img,
+            self.get_limb_lat_map,
+        )
+        self.register_backplane(
             'RING-RADIUS',
             'Equatorial (ring) plane radius [km]',
             self.get_ring_plane_radius_img,
             self.get_ring_plane_radius_map,
         )
         self.register_backplane(
             'RING-LON-GRAPHIC',
```

### Comparing `planetmapper-1.7.7/planetmapper/data/rings.json` & `planetmapper-1.8.0/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/planetmapper/data_loader.py` & `planetmapper-1.8.0/planetmapper/data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/planetmapper/gui.py` & `planetmapper-1.8.0/planetmapper/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 LINESTYLES = ('solid', 'dashed', 'dotted', 'dashdot')
 MARKERS = ('x', '+', 'o', '.', '*', 'v', '^', '<', '>', ',', 'D', 'd', '|', '_')
 GRID_INTERVALS = ('10', '30', '45', '90')
 CMAPS = ('gray', 'viridis', 'plasma', 'inferno', 'magma', 'cividis')
 LIMIT_TYPES = ('absolute', 'percentile')
 
 MAP_INTERPOLATIONS = ('nearest', 'linear', 'quadratic', 'cubic')
-MAP_PROJECTIONS = ('rectangular', 'orthographic', 'azimuthal')
+MAP_PROJECTIONS = ('rectangular', 'orthographic', 'azimuthal', 'azimuthal equal area')
 
 DEFAULT_HINT = ''
 
 
 # Deal with X11 font bug by replacing high codepoint chars with ASCII equivalents.
 # This seems to prevent the use of fonts which cause the X_OpenFont error which
 # XQuartz was producing when trying to run planetmapper over SSH on mac. This is a bit
@@ -2030,15 +2030,17 @@
         map_enabled = bool(self.save_map.get())
         projection_type = self.map_projection.get()
         self.toggle(map_enabled, self.map_widgets)
         self.toggle(
             map_enabled and projection_type in {'rectangular'}, self.map_rect_widgets
         )
         self.toggle(
-            map_enabled and projection_type in {'orthographic', 'azimuthal'},
+            map_enabled
+            and projection_type
+            in {'orthographic', 'azimuthal', 'azimuthal equal area'},
             self.map_ortho_widgets,
         )
 
     def toggle(self, enabled: bool, widgets: list[tk.Widget]) -> None:
         for widget in widgets:
             if enabled:
                 if isinstance(widget, ttk.Combobox):
```

### Comparing `planetmapper-1.7.7/planetmapper/kernel_downloader.py` & `planetmapper-1.8.0/planetmapper/kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/planetmapper/observation.py` & `planetmapper-1.8.0/planetmapper/observation.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import photutils.aperture
 import PIL.Image
 import scipy.ndimage
 from astropy.io import fits
 from astropy.utils.exceptions import AstropyWarning
 
 from . import common, utils
-from .base import _cache_clearable_result
+from .base import _cache_clearable_result, _cache_stable_result
 from .body_xy import BodyXY, Unpack, _MapKwargs
 from .progress import SaveMapProgressHookCLI, SaveNavProgressHookCLI, progress_decorator
 
 T = TypeVar('T')
 S = TypeVar('S')
 P = ParamSpec('P')
 
@@ -314,14 +314,15 @@
 
     def _get_wcs_from_header(self, suppress_warnings: bool = False) -> astropy.wcs.WCS:
         with warnings.catch_warnings():
             if suppress_warnings:
                 warnings.simplefilter('ignore', category=AstropyWarning)
             return astropy.wcs.WCS(self.header).celestial
 
+    @_cache_stable_result
     def _get_disc_params_from_wcs(
         self,
         suppress_warnings: bool = False,
         validate: bool = True,
         use_header_offsets: bool = True,
     ) -> tuple[float, float, float, float]:
         wcs = self._get_wcs_from_header(suppress_warnings=suppress_warnings)
@@ -373,16 +374,16 @@
         Set disc parameters using WCS information in the observation's FITS header.
 
         See also :func:`rotation_from_wcs` and :func:`plate_scale_from_wcs`.
 
         .. note::
 
             There may be very slight differences between the coordinates converted
-            directly from the WCS information, and the coordinates converted by
-            PlanetMapper
+            directly from the WCS information and the coordinates converted by
+            PlanetMapper.
 
         Args:
             suppress_warnings: Hide warnings produced by astropy when calculating WCS
                 conversions.
             validate: Run checks to ensure the WCS conversion has appropriate RA/Dec
                 coordinate dimensions.
             use_header_offsets: If present, use the `HIERARCH NAV RA_OFFSET` and
@@ -450,14 +451,146 @@
             ValueError: if no WCS information is found in the FITS header, or validation
                 fails.
         """
         x0, y0, r0, rotation = self._get_disc_params_from_wcs(*args, **kwargs)
         self.set_r0(r0)
         self.set_disc_method('wcs_plate_scale')
 
+    def get_wcs_offset(self, *args, **kwargs) -> tuple[float, float, float, float]:
+        """
+        .. warning ::
+
+            This is a beta feature and the API may change in future.
+
+        Get the difference between the current disc parameters and the disc parameters
+        calculated from the WCS information in the observation's FITS header.
+
+        For example, this function can be used to retrieve the cumulative offset after
+        adjusting the disc position: ::
+
+            # Initialise disc with parameters from WCS
+            observation.disc_from_wcs()
+
+            # Adjust the disc position
+            observation.adjust_disc_params(1, 2, 3, 4)
+            observation.adjust_disc_params(dx=0.1)
+
+            # Retrieve the cumulative offset
+            print(observation.get_wcs_offset())  # (1.1, 2.0, 3.0, 4.0)
+
+        Similarly, this function can be used to retrieve the offset after running the
+        GUI to fit the disc: ::
+
+            observation.run_gui()
+            print(observation.get_wcs_offset())
+
+        See also :func:`get_wcs_arcsec_offset`.
+
+        Args:
+            *args, **kwargs: See :func:`disc_from_wcs` for additional arguments.
+
+        Returns:
+            `(dx, dy, dr, drotation)` tuple containing the differences in disc
+            parameters between the current disc parameters (i.e. those returned by
+            :func:`BodyXY.get_disc_params`) and the disc parameters calculated from
+            the WCS information in the observation's FITS header. `dx` and `dy` give the
+            difference in the disc centre position in pixels, `dr` gives the difference
+            in the disc radius in pixels, and `drotation` gives the difference in the
+            rotation angle in degrees.
+
+        Raises:
+            ValueError: if no WCS information is found in the FITS header, or validation
+                fails.
+        """
+        x0_wcs, y0_wcs, r0_wcs, rotation_wcs = self._get_disc_params_from_wcs(
+            *args, **kwargs
+        )
+        dx = self.get_x0() - x0_wcs
+        dy = self.get_y0() - y0_wcs
+        dr = self.get_r0() - r0_wcs
+        drotation = (self.get_rotation() - rotation_wcs) % 360
+        return dx, dy, dr, drotation
+
+    def get_wcs_arcsec_offset(
+        self, *args, check_is_position_offset_only: bool = True, **kwargs
+    ) -> tuple[float, float]:
+        """
+        .. warning ::
+
+            This is a beta feature and the API may change in future.
+
+        Get the offset in RA/Dec celestial coordinates between the current disc location
+        and the disc location calculated from the WCS information in the observation's
+        FITS header.
+
+        For example, this function can be used to retrieve the cumulative offset after
+        adjusting the disc position: ::
+
+            # Initialise disc with parameters from WCS
+            observation.disc_from_wcs()
+
+            # Adjust the disc position
+            observation.add_arcsec_offset(10, 10)
+            observation.add_arcsec_offset(dra_arcsec=1.23)
+
+            # Retrieve the cumulative offset
+            print(observation.get_wcs_arcsec_offset())  # (11.23, 10.0)
+
+        Similarly, this function can be used to retrieve the offset after running the
+        GUI to fit the disc: ::
+
+            observation.run_gui()
+            print(observation.get_wcs_arcsec_offset())
+
+        The RA/Dec offsets returned by this function are generally only meaningful if
+        the disc location `(x0, y0)` is the only difference between the current disc
+        parameters and those derived from the WCS. Therefore, by default this function
+        checks that the `dr` and `drotation` values returned by :func:`get_wcs_offset`
+        are sufficiently small to be considered a position offset only, and raises a
+        `ValueError` if this is not the case. This check can be disabled by setting
+        `check_is_position_offset_only` to `False`.
+
+        See also :func:`get_wcs_offset`.
+
+        Args:
+            *args, **kwargs: See :func:`disc_from_wcs` for additional arguments.
+            check_is_position_offset_only: If `True` (the default), check that the
+                `dr` and `drotation` values returned by :func:`get_wcs_offset` are
+                sufficiently small to be considered a position offset only. If this is
+                `False`, then the `dr` and `drotation` values are not checked.
+
+        Returns:
+            `(dra_arcsec, ddec_arcsec)` tuple containing the offsets in arcseconds in
+            the RA and Dec celestial coordinates between the current disc location (i.e.
+            those returned by :func:`BodyXY.get_disc_params`) and the disc location
+            calculated from the WCS information in the observation's FITS header.
+
+        Raises:
+            ValueError: if no WCS information is found in the FITS header, or validation
+                fails. A ValueError is also raised if `check_is_position_offset_only`
+                is `True` and the `dr` or `drotation` values returned by
+                :func:`get_wcs_offset` are not sufficiently small.
+        """
+        dx, dy, dr, drotation = self.get_wcs_offset(*args, **kwargs)
+        if check_is_position_offset_only:
+            if abs(dr) > 1e-3:
+                raise ValueError(
+                    f'r0 is different between WCS and observation (dr={dr})'
+                )
+            if abs((drotation + 180) % 360 - 180) > 1e-3:
+                # ^ modulo operation makes 359 -> -1 so -ve drotation works properly
+                raise ValueError(
+                    f'rotation is different between WCS and observation (drotation={drotation})'
+                )
+        ra0, dec0 = self.xy2radec(0, 0)
+        ra1, dec1 = self.xy2radec(dx, dy)
+        dra_arcsec = (ra1 - ra0) * 3600
+        ddec_arcsec = (dec1 - dec0) * 3600
+        return dra_arcsec, ddec_arcsec
+
     def _get_img_for_fitting(self) -> np.ndarray:
         img = np.nansum(self.data, axis=0)
         mask_img = np.isnan(img)
         img[mask_img] = np.nanmin(img)  # Mask nan values for com calculation etc.
         return img
 
     def fit_disc_position(self) -> None:
@@ -711,14 +844,26 @@
         self.append_to_header(
             'SUBPOINT LON',
             self.subpoint_lon,
             '[degrees] Sub-observer pgr longitude.',
             header=header,
         )
         self.append_to_header(
+            'SUBSOL LAT',
+            self.subsol_lat,
+            '[degrees] Sub-solar pgr latitude.',
+            header=header,
+        )
+        self.append_to_header(
+            'SUBSOL LON',
+            self.subsol_lon,
+            '[degrees] Sub-solar pgr longitude.',
+            header=header,
+        )
+        self.append_to_header(
             'LON-DIRECTION',
             self.positive_longitude_direction,
             'Positive pgr longitude direction.',
             header=header,
         )
         self.append_to_header(
             'NP-ANGLE',
```

### Comparing `planetmapper-1.7.7/planetmapper/progress.py` & `planetmapper-1.8.0/planetmapper/progress.py`

 * *Files 7% similar despite different names*

```diff
@@ -153,16 +153,18 @@
         super().__init__(*args, **kwargs)
         self.weights: dict[str, float] = {
             'BodyXY._get_targvec_img': 100,
             'BodyXY._get_lonlat_img': 50,
             'BodyXY._get_radec_img': 5,
             'BodyXY._get_lonlat_centric_img': 5,
             'BodyXY._get_illumination_gie_img': 50,
+            'BodyXY.get_local_solar_time_img': 5,
             'BodyXY._get_state_imgs': 30,
             'BodyXY.get_radial_velocity_img': 5,
+            'BodyXY._get_limb_coordinate_imgs': 20,
             'BodyXY._get_ring_coordinate_imgs': 50,
             'Observation.save_observation': 100,
         }
         self.default_key = 'Observation.save_observation'
 
     def get_description(self) -> str:
         return 'Saving observation'
@@ -176,16 +178,18 @@
         self.weights: dict[str, float] = {
             'Observation._get_mapped_data': n_wavelengths * 5,
             'BodyXY._get_targvec_map': 10,
             'BodyXY._get_illumf_map': 5,
             'BodyXY._get_radec_map': 10,
             'BodyXY._get_xy_map': 10,
             # 'BodyXY._get_lonlat_map': 10,
+            'BodyXY.get_local_solar_time_map': 5,
             'BodyXY._get_lonlat_centric_map': 5,
             'BodyXY._get_state_maps': 5,
+            'BodyXY._get_limb_coordinate_maps': 10,
             'BodyXY._get_ring_coordinate_maps': 10,
             'Observation.save_mapped_observation': 20,
         }
         self.default_key = 'Observation.save_mapped_observation'
 
     def get_description(self) -> str:
         return 'Saving map'
```

### Comparing `planetmapper-1.7.7/planetmapper/utils.py` & `planetmapper-1.8.0/planetmapper/utils.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.8.0/planetmapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.7.7
+Version: 1.8.0
 Summary: PlanetMapper: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 License: MIT
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
```

### Comparing `planetmapper-1.7.7/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.8.0/planetmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/pyproject.toml` & `planetmapper-1.8.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.black]
 skip-string-normalization = true
 exclude = ""
 # Manually set exclude="" to prevent black using .gitignore due
 # to black not parsing trailing slashes in .gitignore correctly
 # https://github.com/psf/black/issues/3694
-extend_exclude = "typings"
+extend_exclude = "python-type-stubs"
 
 
 [tool.isort]
 profile = "black"
-extend_skip = ["typings"]
+extend_skip = ["python-type-stubs"]
 
 
 [tool.coverage.run]
 branch = true
 include = ["planetmapper/*.py"]
 omit = ["planetmapper/gui.py"]
 
@@ -48,13 +48,14 @@
 
 [tool.pylint.miscellaneous]
 notes=["FIXME", "XXX"] # Allow TODO comments, but not FIXME or XXX
 
 
 [tool.pyright]
 include = ["planetmapper/*.py", "setup.py"]
+stubPath = "python-type-stubs/stubs"
 reportPropertyTypeMismatch = true
 reportConstantRedefinition = true
 reportIncompatibleMethodOverride = true
 reportIncompatibleVariableOverride = true
 reportUnnecessaryComparison = true
 reportUnnecessaryContains = true
```

### Comparing `planetmapper-1.7.7/setup.py` & `planetmapper-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/tests/test_base.py` & `planetmapper-1.8.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/tests/test_basic_body.py` & `planetmapper-1.8.0/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/tests/test_body.py` & `planetmapper-1.8.0/tests/test_body.py`

 * *Files 18% similar despite different names*

```diff
@@ -81,14 +81,16 @@
         self.assertAlmostEqual(self.body.target_distance, 819638074.3312353)
         self.assertAlmostEqual(self.body.target_ra, 196.37198562427025)
         self.assertAlmostEqual(self.body.target_dec, -5.565793847134351)
         self.assertAlmostEqual(self.body.target_diameter_arcsec, 35.98242703657337)
         self.assertAlmostEqual(self.body.subpoint_distance, 819566594.28005)
         self.assertAlmostEqual(self.body.subpoint_lon, 153.12585514751467)
         self.assertAlmostEqual(self.body.subpoint_lat, -3.0886644594385193)
+        self.assertAlmostEqual(self.body.subsol_lon, 163.44768812575543)
+        self.assertAlmostEqual(self.body.subsol_lat, -2.7185371707509427)
         self.assertEqual(
             self.body.named_ring_data,
             {
                 'Halo': [89400.0, 123000.0],
                 'Main Ring': [123000.0, 128940.0],
                 'Amalthea Ring': [128940.0, 181350.0],
                 'Thebe Ring': [181350.0, 221900.0],
@@ -100,14 +102,20 @@
         self.assertEqual(self.body.coordinates_of_interest_radec, [])
         self.assertEqual(self.body.other_bodies_of_interest, [])
 
         moon = Body('moon', '2005-01-01')
         self.assertEqual(moon.positive_longitude_direction, 'E')
         self.assertTrue(moon.prograde)
 
+        sun = Body('sun', '2005-01-01')
+        self.assertEqual(sun.positive_longitude_direction, 'E')
+        self.assertTrue(sun.prograde)
+        self.assertTrue(np.isnan(sun.subsol_lon))
+        self.assertTrue(np.isnan(sun.subsol_lat))
+
     def test_repr(self):
         self.assertEqual(
             repr(self.body),
             "Body('JUPITER', '2005-01-01T00:00:00.000000', observer='HST')",
         )
 
     def test_eq(self):
@@ -368,18 +376,24 @@
         self.assertEqual(self.body.ring_radii, set())
 
     def test_lonlat2radec(self):
         pairs = [
             [(0, 90), (196.37390490466322, -5.561534444253404)],
             [(0, 0), (196.36982789576643, -5.565060944053696)],
             [(123.456, -56.789), (196.3691609381441, -5.5685956879058764)],
+            [(np.nan, np.nan), (np.nan, np.nan)],
+            [(np.nan, 0), (np.nan, np.nan)],
+            [(0, np.nan), (np.nan, np.nan)],
+            [(np.inf, np.inf), (np.nan, np.nan)],
         ]
         for lonlat, radec in pairs:
             with self.subTest(lonlat):
-                self.assertTrue(np.allclose(self.body.lonlat2radec(*lonlat), radec))
+                self.assertTrue(
+                    np.allclose(self.body.lonlat2radec(*lonlat), radec, equal_nan=True)
+                )
 
     def test_radec2lonlat(self):
         self.assertTrue(
             np.array_equal(
                 self.body.radec2lonlat(0, 0), (np.nan, np.nan), equal_nan=True
             )
         )
@@ -392,66 +406,97 @@
                 (153.1235185909613, -3.0887371238645795),
             ],
             [(196.372, -5.566), (154.24480750302573, -5.475831082435726)],
             [
                 (196.3742715121965, -5.561743939677709),
                 (180.00086055026196, 80.00042229835671),
             ],
+            [(np.nan, np.nan), (np.nan, np.nan)],
+            [(np.nan, 0), (np.nan, np.nan)],
+            [(0, np.nan), (np.nan, np.nan)],
+            [(np.inf, np.inf), (np.nan, np.nan)],
         ]
         for radec, lonlat in pairs:
             with self.subTest(radec):
                 self.assertTrue(
                     np.allclose(
                         self.body.radec2lonlat(*radec),
                         lonlat,
+                        equal_nan=True,
                     )
                 )
-                self.assertTrue(
-                    np.allclose(
-                        self.body.lonlat2radec(*lonlat),
-                        radec,
+                if all(np.isfinite(x) for x in radec):
+                    self.assertTrue(
+                        np.allclose(
+                            self.body.lonlat2radec(*lonlat), radec, equal_nan=True
+                        )
                     )
-                )
 
     def test_lonlat2targvec(self):
         pairs = [
             ((0, 0), np.array([71492.0, -0.0, 0.0])),
             ((360, 0), np.array([[71492.0, -0.0, 0.0]])),
             ((123, 45), np.array([-28439.90450754, -43793.6125254, 45662.45633365])),
             (
                 (-80, -12.3456789),
                 np.array([[12162.32647743, 68975.98103572, -13405.21131042]]),
             ),
+            [(np.nan, np.nan), np.array([np.nan, np.nan, np.nan])],
+            [(np.nan, 0), np.array([np.nan, np.nan, np.nan])],
+            [(0, np.nan), np.array([np.nan, np.nan, np.nan])],
+            [(np.inf, np.inf), np.array([np.nan, np.nan, np.nan])],
         ]
         for (lon, lat), targvec in pairs:
             with self.subTest((lon, lat)):
                 self.assertTrue(
-                    np.allclose(self.body.lonlat2targvec(lon, lat), targvec)
+                    np.allclose(
+                        self.body.lonlat2targvec(lon, lat), targvec, equal_nan=True
+                    )
                 )
 
     def test_targvec2lonlat(self):
         pairs = [
             (np.array([0, 0, 0]), (0.0, 90.0)),
             (np.array([1, 2, 3]), (296.565051177078, 89.98665551067639)),
             (np.array([-9876, 543210, 0]), (268.9584308375042, 0.0)),
+            (np.array([np.nan, np.nan, np.nan]), (np.nan, np.nan)),
+            (np.array([np.nan, 0, 0]), (np.nan, np.nan)),
+            (np.array([0, np.nan, 0]), (np.nan, np.nan)),
+            (np.array([0, 0, np.nan]), (np.nan, np.nan)),
+            (np.array([np.inf, np.inf, np.inf]), (np.nan, np.nan)),
         ]
         for targvec, lonlat in pairs:
             with self.subTest(targvec):
-                self.assertTrue(np.allclose(self.body.targvec2lonlat(targvec), lonlat))
+                self.assertTrue(
+                    np.allclose(
+                        self.body.targvec2lonlat(targvec), lonlat, equal_nan=True
+                    )
+                )
 
     def test_km_radec(self):
         pairs = [
             [(0, 0), (196.37198562427025, -5.565793847134351)],
             [(99999, 99999), (196.36846760253624, -5.556548919202668)],
         ]
         for km, radec in pairs:
             with self.subTest(km):
                 self.assertTrue(np.allclose(self.body.km2radec(*km), radec))
                 self.assertTrue(np.allclose(self.body.radec2km(*radec), km, atol=1e-3))
 
+        inputs = [
+            (np.nan, np.nan),
+            (np.nan, 0),
+            (0, np.nan),
+            (np.inf, np.inf),
+        ]
+        for a in inputs:
+            with self.subTest(a):
+                self.assertTrue(all(not np.isfinite(x) for x in self.body.km2radec(*a)))
+                self.assertTrue(all(not np.isfinite(x) for x in self.body.radec2km(*a)))
+
     def test_km_lonlat(self):
         pairs = [
             [(0, 0), (153.1235185909613, -3.0887371238645795)],
             [(123, 456.789), (153.02550380815194, -2.6701272595645387)],
             [(-500, -200), (153.52449023101565, -3.2726499274177465)],
             [(5000, 50001), (147.49451214685632, 47.45177666020315)],
         ]
@@ -464,14 +509,29 @@
 
         self.assertTrue(
             np.array_equal(
                 self.body.km2lonlat(100000000, 0), (np.nan, np.nan), equal_nan=True
             )
         )
 
+        inputs = [
+            (np.nan, np.nan),
+            (np.nan, 0),
+            (0, np.nan),
+            (np.inf, np.inf),
+        ]
+        for a in inputs:
+            with self.subTest(a):
+                self.assertTrue(
+                    all(not np.isfinite(x) for x in self.body.km2lonlat(*a))
+                )
+                self.assertTrue(
+                    all(not np.isfinite(x) for x in self.body.lonlat2km(*a))
+                )
+
     def test_limbradec(self):
         self.assertTrue(
             np.allclose(
                 self.body.limb_radec(npts=10),
                 (
                     np.array(
                         [
@@ -538,14 +598,60 @@
                     array([nan, nan, nan, 196.36782109, 196.36828846, nan]),
                     array([nan, nan, nan, -5.56817191, -5.56246245, nan]),
                 ),
                 equal_nan=True,
             )
         )
 
+    def test_limb_coordinates_from_radec(self):
+        args: list[tuple[tuple[float, float], tuple[float, float, float]]] = [
+            ((0, 0), (82.72145635455739, -7.331180721378409, 243226446.365406)),
+            (
+                (196.3719829300016, -5.565779946690757),
+                (67.23274105785333, 58.34599234749429, -68089.8880967631),
+            ),
+            (
+                (196.372, -5.566),
+                (248.13985326986065, -64.83923990338549, -64857.80811442864),
+            ),
+            ((196.3, -5.5), (64.1290135632679, 20.79992677586983, 1320579.9259661217)),
+            ((np.nan, np.nan), (np.nan, np.nan, np.nan)),
+            ((np.nan, 0), (np.nan, np.nan, np.nan)),
+            ((0, np.nan), (np.nan, np.nan, np.nan)),
+            ((np.inf, np.inf), (np.nan, np.nan, np.nan)),
+        ]
+        for (ra, dec), (lon_expected, lat_expected, dist_expected) in args:
+            with self.subTest(ra=ra, dec=dec):
+                lon, lat, dist = self.body.limb_coordinates_from_radec(ra, dec)
+                self.assertTrue(
+                    np.allclose(lon, lon_expected, rtol=1e-5, equal_nan=True)
+                )
+                self.assertTrue(
+                    np.allclose(lat, lat_expected, rtol=1e-5, equal_nan=True)
+                )
+                self.assertTrue(
+                    np.allclose(dist, dist_expected, rtol=1e-5, equal_nan=True)
+                )
+
+    def test_if_lonlat_visible(self):
+        pairs: list[tuple[tuple[float, float], bool]] = [
+            ((0, 0), False),
+            ((180, 12), True),
+            ((50, -80), True),
+            ((np.nan, np.nan), False),
+            ((np.nan, 0), False),
+            ((0, np.nan), False),
+            ((np.inf, np.inf), False),
+        ]
+        for lonlat, visible in pairs:
+            with self.subTest(lonlat=lonlat):
+                self.assertEqual(
+                    self.body.test_if_lonlat_visible(*lonlat), visible, lonlat
+                )
+
     def test_other_body_los_intercept(self):
         utc = '2005-01-01 04:00:00'
         jupiter = planetmapper.Body('Jupiter', utc)
 
         intercepts: list[tuple[str, str | None, bool]] = [
             ('thebe', 'hidden', False),
             ('metis', 'transit', True),
@@ -575,34 +681,70 @@
         self.assertEqual(body.test_if_other_body_visible('amalthea'), True)
 
         body = planetmapper.Body('Jupiter', '2005-01-01 06:34:05')
         self.assertEqual(body.other_body_los_intercept('amalthea'), 'part transit')
         self.assertEqual(body.test_if_other_body_visible('amalthea'), True)
 
     def test_illimination_angles_from_lonlat(self):
-        self.assertTrue(
-            np.allclose(
-                self.body.illumination_angles_from_lonlat(0, 0),
-                (10.31594976458697, 163.2795134457034, 152.99822832991876),
-            )
-        )
-        self.assertTrue(
-            np.allclose(
-                self.body.illumination_angles_from_lonlat(123.456, -78.9),
+        args: list[tuple[tuple[float, float], tuple[float, float, float]]] = [
+            ((0, 0), (10.31594976458697, 163.2795134457034, 152.99822832991876)),
+            (
+                (123.456, -78.9),
                 (10.316968817304499, 79.16351827229181, 77.68583738495468),
-            )
-        )
+            ),
+            ((np.nan, np.nan), (np.nan, np.nan, np.nan)),
+            ((np.nan, 0), (np.nan, np.nan, np.nan)),
+            ((0, np.nan), (np.nan, np.nan, np.nan)),
+            ((np.inf, np.inf), (np.nan, np.nan, np.nan)),
+        ]
+
+        for lonlat, angles in args:
+            with self.subTest(lonlat=lonlat):
+                self.assertTrue(
+                    np.allclose(
+                        self.body.illumination_angles_from_lonlat(*lonlat),
+                        angles,
+                        equal_nan=True,
+                    )
+                )
 
     def test_azimuth_angle_from_lonlat(self):
-        self.assertAlmostEqual(
-            self.body.azimuth_angle_from_lonlat(0, 0), 177.66817822757469
-        )
-        self.assertAlmostEqual(
-            self.body.azimuth_angle_from_lonlat(123.456, -78.9), 169.57651996164563
-        )
+        args: list[tuple[tuple[float, float], float]] = [
+            ((0, 0), 177.66817822757469),
+            ((123.456, -78.9), 169.57651996164563),
+            ((np.nan, np.nan), np.nan),
+            ((np.nan, 0), np.nan),
+            ((0, np.nan), np.nan),
+            ((np.inf, np.inf), np.nan),
+        ]
+        for lonlat, angle in args:
+            with self.subTest(lonlat=lonlat):
+                self.assertTrue(
+                    np.allclose(
+                        self.body.azimuth_angle_from_lonlat(*lonlat),
+                        angle,
+                        equal_nan=True,
+                    )
+                )
+
+    def test_local_solar_time(self):
+        args: list[tuple[float, float, str]] = [
+            (0, 22.89638888888889, '22:53:47'),
+            (-90, 4.896388888888889, '04:53:47'),
+            (123.456, 14.666111111111112, '14:39:58'),
+            (999.999, 4.229722222222223, '04:13:47'),
+            (np.nan, np.nan, ''),
+            (np.inf, np.nan, ''),
+        ]
+        for lon, lst_expected, s_expected in args:
+            with self.subTest(lon=lon):
+                lst = self.body.local_solar_time_from_lon(lon)
+                s = self.body.local_solar_time_string_from_lon(lon)
+                self.assertTrue(np.isclose(lst, lst_expected, equal_nan=True))
+                self.assertEqual(s, s_expected)
 
     def test_terminator_radec(self):
         self.assertTrue(
             np.allclose(
                 self.body.terminator_radec(npts=5),
                 (
                     array([nan, nan, nan, 196.36784184, 196.36838618, nan]),
@@ -619,63 +761,61 @@
             )
         )
 
     def test_if_lonlat_illuminated(self):
         pairs: list[tuple[tuple[float, float], bool]] = [
             ((0, 0), False),
             ((180, 12), True),
+            ((50, -80), False),
+            ((np.nan, np.nan), False),
+            ((np.nan, 0), False),
+            ((0, np.nan), False),
+            ((np.inf, np.inf), False),
         ]
         for (lon, lat), illuminated in pairs:
             with self.subTest(lon=lon, lat=lat):
                 self.assertEqual(
                     self.body.test_if_lonlat_illuminated(lon, lat), illuminated
                 )
 
     def test_ring_plane_coordinates(self):
-        self.assertTrue(
-            np.allclose(
-                self.body.ring_plane_coordinates(0, 0),
-                (nan, nan, nan),
-                equal_nan=True,
-            ),
-        )
-        self.assertTrue(
-            np.allclose(
-                self.body.ring_plane_coordinates(
-                    196.37198562427025, -5.565793847134351
-                ),
-                (nan, nan, nan),
-                equal_nan=True,
-            ),
-        )
-        self.assertTrue(
-            np.allclose(
-                self.body.ring_plane_coordinates(
-                    196.37347182693253, -5.561472466522512
-                ),
+        args: list[tuple[tuple[float, float, bool], tuple[float, float, float]]] = [
+            ((0, 0, True), (nan, nan, nan)),
+            ((196.37198562427025, -5.565793847134351, True), (nan, nan, nan)),
+            (
+                (196.37347182693253, -5.561472466522512, True),
                 (1377914.753652832, 152.91772706249577, 818261707.8278764),
-                equal_nan=True,
             ),
-        )
-        self.assertTrue(
-            np.allclose(
-                self.body.ring_plane_coordinates(196.3696997398314, -5.569843641306982),
-                (nan, nan, nan),
-                equal_nan=True,
-            ),
-        )
-        self.assertTrue(
-            np.allclose(
-                self.body.ring_plane_coordinates(
-                    196.37198562427025, -5.565793847134351, only_visible=False
-                ),
+            ((196.3696997398314, -5.569843641306982, True), (nan, nan, nan)),
+            (
+                (196.37198562427025, -5.565793847134351, False),
                 (4638.105239104683, 156.0690984698183, 819638074.3312378),
-                equal_nan=True,
             ),
-        )
+            (
+                (196.3, -5.5, True),
+                (9305877.091704229, 145.3644753085151, 810435703.2382222),
+            ),
+            ((np.nan, np.nan, True), (np.nan, np.nan, np.nan)),
+            ((np.nan, 0, True), (np.nan, np.nan, np.nan)),
+            ((0, np.nan, True), (np.nan, np.nan, np.nan)),
+            ((np.inf, np.inf, True), (np.nan, np.nan, np.nan)),
+        ]
+        for (lon, lat, only_visible), coords in args:
+            with self.subTest(lon=lon, lat=lat, only_visible=only_visible):
+                self.assertTrue(
+                    np.allclose(
+                        self.body.ring_plane_coordinates(
+                            lon, lat, only_visible=only_visible
+                        ),
+                        coords,
+                        equal_nan=True,
+                    ),
+                )
+
+        # test default args
         self.assertTrue(
             np.allclose(
                 self.body.ring_plane_coordinates(196.3, -5.5),
                 (9305877.091704229, 145.3644753085151, 810435703.2382222),
                 equal_nan=True,
             ),
         )
@@ -697,14 +837,21 @@
                 (
                     array([196.36825958, 196.37571178, 196.36825958]),
                     array([-5.56452821, -5.56705935, -5.56452821]),
                 ),
                 equal_nan=True,
             )
         )
+        self.assertTrue(
+            np.allclose(
+                self.body.ring_radec(np.nan, npts=2, only_visible=False),
+                (array([nan, nan]), array([nan, nan])),
+                equal_nan=True,
+            )
+        )
 
     def test_visible_lonlat_grid_radec(self):
         self.assertTrue(
             np.allclose(
                 self.body.visible_lonlat_grid_radec(interval=45, npts=5),
                 [
                     (
@@ -787,20 +934,46 @@
                     ),
                 ],
                 equal_nan=True,
             )
         )
 
     def test_radial_velocity_from_lonlat(self):
-        self.assertAlmostEqual(
-            self.body.radial_velocity_from_lonlat(0, 0), -20.796924908179438
-        )
+        args: list[tuple[tuple[float, float], float]] = [
+            ((0, 0), -20.796924908179438),
+            ((np.nan, np.nan), np.nan),
+            ((np.nan, 0), np.nan),
+            ((0, np.nan), np.nan),
+            ((np.inf, np.inf), np.nan),
+        ]
+        for lonlat, x in args:
+            with self.subTest(lonlat=lonlat):
+                self.assertTrue(
+                    np.allclose(
+                        self.body.radial_velocity_from_lonlat(*lonlat),
+                        x,
+                        equal_nan=True,
+                    )
+                )
 
     def test_distance_from_lonalt(self):
-        self.assertAlmostEqual(self.body.distance_from_lonlat(0, 0), 819701772.0279644)
+        args: list[tuple[tuple[float, float], float]] = [
+            ((0, 0), 819701772.0279644),
+            ((np.nan, np.nan), np.nan),
+            ((np.nan, 0), np.nan),
+            ((0, np.nan), np.nan),
+            ((np.inf, np.inf), np.nan),
+        ]
+        for lonlat, x in args:
+            with self.subTest(lonlat=lonlat):
+                self.assertTrue(
+                    np.allclose(
+                        self.body.distance_from_lonlat(*lonlat), x, equal_nan=True
+                    )
+                )
 
     def test_graphic_centric_lonlat(self):
         pairs = [
             [(0, 0), (0, 0)],
             [(0, 90), (0, 90)],
             [(0, -90), (0, -90)],
             [(90, 0), (-90, 0)],
@@ -811,14 +984,29 @@
                 self.assertTrue(
                     np.allclose(self.body.graphic2centric_lonlat(*graphic), centric)
                 )
                 self.assertTrue(
                     np.allclose(self.body.centric2graphic_lonlat(*centric), graphic)
                 )
 
+        pairs = [
+            ((np.nan, np.nan), (np.nan, np.nan)),
+            ((np.nan, 0), (np.nan, np.nan)),
+            ((0, np.nan), (np.nan, np.nan)),
+            ((np.inf, np.inf), (np.nan, np.nan)),
+        ]
+        for a, b in pairs:
+            with self.subTest(a):
+                self.assertTrue(
+                    np.allclose(self.body.graphic2centric_lonlat(*a), b, equal_nan=True)
+                )
+                self.assertTrue(
+                    np.allclose(self.body.centric2graphic_lonlat(*a), b, equal_nan=True)
+                )
+
     def test_north_pole_angle(self):
         self.assertAlmostEqual(self.body.north_pole_angle(), -24.256254044782136)
 
     def test_get_description(self):
         self.assertEqual(
             self.body.get_description(),
             'JUPITER (599)\nfrom HST\nat 2005-01-01 00:00 UTC',
```

### Comparing `planetmapper-1.7.7/tests/test_body_xy.py` & `planetmapper-1.8.0/tests/test_body_xy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import unittest
 from unittest.mock import MagicMock, patch
 
 import common_testing
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.collections import QuadMesh
-from numpy import array, nan
+from numpy import array, inf, nan
 
 import planetmapper
 import planetmapper.base
 import planetmapper.progress
 from planetmapper import BodyXY
 from planetmapper.body_xy import Backplane, BackplaneNotFoundError
+from planetmapper.body_xy import _MapKwargs as MapKwargs
 
 
 class TestFunctions(unittest.TestCase):
     def test_make_backplane_documentation_str(self):
         self.assertIsInstance(
             planetmapper.body_xy._make_backplane_documentation_str(), str
         )
@@ -270,14 +271,29 @@
                     )
                     if not any(np.isnan(lonlat)):
                         self.assertTrue(
                             np.allclose(body.lonlat2xy(*lonlat), xy, equal_nan=True)
                         )
                     self.assertTrue(np.allclose(body.km2xy(*km), xy, equal_nan=True))
 
+        args = [
+            (np.nan, np.nan),
+            (np.nan, 0),
+            (0, np.nan),
+            (np.inf, np.inf),
+        ]
+        for a in args:
+            with self.subTest(a):
+                self.assertTrue(not all(np.isfinite(self.body.xy2radec(*a))))
+                self.assertTrue(not all(np.isfinite(self.body.xy2lonlat(*a))))
+                self.assertTrue(not all(np.isfinite(self.body.xy2km(*a))))
+                self.assertTrue(not all(np.isfinite(self.body.radec2xy(*a))))
+                self.assertTrue(not all(np.isfinite(self.body.lonlat2xy(*a))))
+                self.assertTrue(not all(np.isfinite(self.body.km2xy(*a))))
+
     def test_set_disc_params(self):
         x0, y0, r0, rotation = [1.1, 2.2, 3.3, 4.4]
         self.body.set_disc_params(x0, y0, r0, rotation)
         self.assertEqual(self.body.get_x0(), x0)
         self.assertEqual(self.body.get_y0(), y0)
         self.assertEqual(self.body.get_r0(), r0)
         self.assertAlmostEqual(self.body.get_rotation(), rotation)
@@ -578,14 +594,27 @@
         self.assertEqual(len(ax.get_images()), 0)
         self.assertEqual(len(ax.get_children()), 30)
         plt.close(fig)
 
         fig, ax = plt.subplots()
         self.body.plot_map_wireframe(
             ax=ax,
+            projection='azimuthal equal area',
+            lat=-90,
+            label_poles=False,
+            grid_interval=45,
+        )
+        self.assertEqual(len(ax.get_lines()), 20)
+        self.assertEqual(len(ax.get_images()), 0)
+        self.assertEqual(len(ax.get_children()), 30)
+        plt.close(fig)
+
+        fig, ax = plt.subplots()
+        self.body.plot_map_wireframe(
+            ax=ax,
             projection='manual',
             lon_coords=np.linspace(-180, 180, 5),
             lat_coords=np.linspace(0, 90, 3),
         )
         self.assertEqual(len(ax.get_lines()), 17)
         self.assertEqual(len(ax.get_images()), 0)
         self.assertEqual(len(ax.get_children()), 29)
@@ -771,21 +800,286 @@
         )
         output_b = self.body.generate_map_coordinates(
             '+proj=ortho +R=1 +type=crs',
             projection_x_coords=np.array([0, 0.25, 0.5]),
             projection_y_coords=np.array([0, 0.25, 0.5]),
         )
         for idx, (a, b) in enumerate(zip(output_a, output_b)):
+            if idx == 5:
+                # info dict with projection_y_coords = None
+                self.assertEqual(a['projection_y_coords'], None)  # type: ignore
+                a['projection_y_coords'] = b['projection_y_coords']  # type: ignore
+            with self.subTest(idx=idx):
+                self.assertEqual(type(a), type(b))
+                if isinstance(a, np.ndarray):
+                    self.assertTrue(np.array_equal(a, b))  # type: ignore
+                else:
+                    self.assertEqual(a, b)
+
+        # Test limits
+        output_a = self.body.generate_map_coordinates(degree_interval=30)
+        output_b = self.body.generate_map_coordinates(
+            degree_interval=30, xlim=None, ylim=None
+        )
+        for idx, (a, b) in enumerate(zip(output_a, output_b)):
             with self.subTest(idx=idx):
                 self.assertEqual(type(a), type(b))
                 if isinstance(a, np.ndarray):
                     self.assertTrue(np.array_equal(a, b))
                 else:
                     self.assertEqual(a, b)
 
+        args: list[
+            tuple[
+                tuple[float, float] | None,
+                tuple[float, float] | None,
+                np.ndarray,
+                np.ndarray,
+            ]
+        ] = [
+            (
+                None,
+                None,
+                array([[315.0, 225.0, 135.0, 45.0], [315.0, 225.0, 135.0, 45.0]]),
+                array([[-45.0, -45.0, -45.0, -45.0], [45.0, 45.0, 45.0, 45.0]]),
+            ),
+            (
+                (-np.inf, np.inf),
+                (-np.inf, np.inf),
+                array([[315.0, 225.0, 135.0, 45.0], [315.0, 225.0, 135.0, 45.0]]),
+                array([[-45.0, -45.0, -45.0, -45.0], [45.0, 45.0, 45.0, 45.0]]),
+            ),
+            (
+                (135, -np.inf),
+                (45, np.inf),
+                array([[135.0, 45.0]]),
+                array([[45.0, 45.0]]),
+            ),
+            (
+                (100, 300),
+                (-50, 50),
+                array([[225.0, 135.0], [225.0, 135.0]]),
+                array([[-45.0, -45.0], [45.0, 45.0]]),
+            ),
+            (
+                (300, 100),
+                (50, -50),
+                array([[225.0, 135.0], [225.0, 135.0]]),
+                array([[-45.0, -45.0], [45.0, 45.0]]),
+            ),
+        ]
+        for xlim, ylim, lons_expected, lats_expected in args:
+            with self.subTest(xlim=xlim, ylim=ylim):
+                (
+                    lons,
+                    lats,
+                    xx,
+                    yy,
+                    transformer,
+                    info,
+                ) = self.body.generate_map_coordinates(
+                    degree_interval=90, xlim=xlim, ylim=ylim
+                )
+                self.assertTrue(
+                    np.array_equal(lons, lons_expected),
+                    msg=f'{lons} <> {lons_expected}',
+                )
+                self.assertTrue(np.array_equal(lats, lats_expected))
+                self.assertTrue(np.array_equal(xx, lons_expected))
+                self.assertTrue(np.array_equal(yy, lats_expected))
+                self.assertEqual(info['xlim'], xlim)
+                self.assertEqual(info['ylim'], ylim)
+
+        # Test reference
+        args: list[tuple[MapKwargs, np.ndarray, np.ndarray, np.ndarray, np.ndarray]] = [
+            (
+                MapKwargs(degree_interval=123),
+                array([[307.5, 184.5, 61.5]]),
+                array([[-28.5, -28.5, -28.5]]),
+                array([[307.5, 184.5, 61.5]]),
+                array([[-28.5, -28.5, -28.5]]),
+            ),
+            (
+                MapKwargs(projection='orthographic', size=3),
+                array([[nan, nan, nan], [nan, 0.0, nan], [nan, nan, nan]]),
+                array([[nan, nan, nan], [nan, 0.0, nan], [nan, nan, nan]]),
+                array([[-1.01, 0.0, 1.01], [-1.01, 0.0, 1.01], [-1.01, 0.0, 1.01]]),
+                array([[-1.01, -1.01, -1.01], [0.0, 0.0, 0.0], [1.01, 1.01, 1.01]]),
+            ),
+            (
+                MapKwargs(projection='orthographic', size=3, lon=123.456, lat=-2),
+                array([[nan, nan, nan], [nan, 123.456, nan], [nan, nan, nan]]),
+                array([[nan, nan, nan], [nan, -2.29643357, nan], [nan, nan, nan]]),
+                array([[-1.01, 0.0, 1.01], [-1.01, 0.0, 1.01], [-1.01, 0.0, 1.01]]),
+                array([[-1.01, -1.01, -1.01], [0.0, 0.0, 0.0], [1.01, 1.01, 1.01]]),
+            ),
+            (
+                MapKwargs(projection='azimuthal', size=4),
+                array(
+                    [
+                        [nan, nan, nan, nan],
+                        [nan, -83.93213465, 83.93213465, nan],
+                        [nan, -83.93213465, 83.93213465, nan],
+                        [nan, nan, nan, nan],
+                    ]
+                ),
+                array(
+                    [
+                        [nan, nan, nan, nan],
+                        [nan, -44.83904649, -44.83904649, nan],
+                        [nan, 44.83904649, 44.83904649, nan],
+                        [nan, nan, nan, nan],
+                    ]
+                ),
+                array(
+                    [
+                        [-1.01, -0.33666667, 0.33666667, 1.01],
+                        [-1.01, -0.33666667, 0.33666667, 1.01],
+                        [-1.01, -0.33666667, 0.33666667, 1.01],
+                        [-1.01, -0.33666667, 0.33666667, 1.01],
+                    ]
+                ),
+                array(
+                    [
+                        [-1.01, -1.01, -1.01, -1.01],
+                        [-0.33666667, -0.33666667, -0.33666667, -0.33666667],
+                        [0.33666667, 0.33666667, 0.33666667, 0.33666667],
+                        [1.01, 1.01, 1.01, 1.01],
+                    ]
+                ),
+            ),
+            (
+                MapKwargs(projection='azimuthal', size=4, lat=90, lon=123.456),
+                array(
+                    [
+                        [nan, nan, nan, nan],
+                        [nan, 78.456, 168.456, nan],
+                        [nan, -11.544, -101.544, nan],
+                        [nan, nan, nan, nan],
+                    ]
+                ),
+                array(
+                    [
+                        [nan, nan, nan, nan],
+                        [nan, 4.29865812, 4.29865812, nan],
+                        [nan, 4.29865812, 4.29865812, nan],
+                        [nan, nan, nan, nan],
+                    ]
+                ),
+                array(
+                    [
+                        [-1.01, -0.33666667, 0.33666667, 1.01],
+                        [-1.01, -0.33666667, 0.33666667, 1.01],
+                        [-1.01, -0.33666667, 0.33666667, 1.01],
+                        [-1.01, -0.33666667, 0.33666667, 1.01],
+                    ]
+                ),
+                array(
+                    [
+                        [-1.01, -1.01, -1.01, -1.01],
+                        [-0.33666667, -0.33666667, -0.33666667, -0.33666667],
+                        [0.33666667, 0.33666667, 0.33666667, 0.33666667],
+                        [1.01, 1.01, 1.01, 1.01],
+                    ]
+                ),
+            ),
+            (
+                MapKwargs(projection='azimuthal equal area', size=5),
+                array(
+                    [
+                        [nan, nan, nan, nan, nan],
+                        [nan, -91.6285626, 0.0, 91.6285626, nan],
+                        [nan, -60.66270473, 0.0, 60.66270473, nan],
+                        [nan, -91.6285626, 0.0, 91.6285626, nan],
+                        [nan, nan, nan, nan, nan],
+                    ]
+                ),
+                array(
+                    [
+                        [nan, nan, nan, nan, nan],
+                        [nan, -44.98842597, -60.66270473, -44.98842597, nan],
+                        [nan, 0.0, 0.0, 0.0, nan],
+                        [nan, 44.98842597, 60.66270473, 44.98842597, nan],
+                        [nan, nan, nan, nan, nan],
+                    ]
+                ),
+                array(
+                    [
+                        [-1.01, -0.505, 0.0, 0.505, 1.01],
+                        [-1.01, -0.505, 0.0, 0.505, 1.01],
+                        [-1.01, -0.505, 0.0, 0.505, 1.01],
+                        [-1.01, -0.505, 0.0, 0.505, 1.01],
+                        [-1.01, -0.505, 0.0, 0.505, 1.01],
+                    ]
+                ),
+                array(
+                    [
+                        [-1.01, -1.01, -1.01, -1.01, -1.01],
+                        [-0.505, -0.505, -0.505, -0.505, -0.505],
+                        [0.0, 0.0, 0.0, 0.0, 0.0],
+                        [0.505, 0.505, 0.505, 0.505, 0.505],
+                        [1.01, 1.01, 1.01, 1.01, 1.01],
+                    ]
+                ),
+            ),
+            (
+                MapKwargs(projection='azimuthal equal area', size=5, lat=-12, lon=34),
+                array(
+                    [
+                        [nan, nan, nan, nan, nan],
+                        [nan, -69.26373836, 34.0, 137.26373836, nan],
+                        [nan, -27.20027738, 34.0, 95.20027738, nan],
+                        [nan, -45.79039062, 34.0, 113.79039062, nan],
+                        [nan, nan, nan, nan, nan],
+                    ]
+                ),
+                array(
+                    [
+                        [nan, nan, nan, nan, nan],
+                        [nan, -43.4196019, -72.66270473, -43.4196019, nan],
+                        [nan, -5.84665238, -12.0, -5.84665238, nan],
+                        [nan, 44.08255341, 48.66270473, 44.08255341, nan],
+                        [nan, nan, nan, nan, nan],
+                    ]
+                ),
+                array(
+                    [
+                        [-1.01, -0.505, 0.0, 0.505, 1.01],
+                        [-1.01, -0.505, 0.0, 0.505, 1.01],
+                        [-1.01, -0.505, 0.0, 0.505, 1.01],
+                        [-1.01, -0.505, 0.0, 0.505, 1.01],
+                        [-1.01, -0.505, 0.0, 0.505, 1.01],
+                    ]
+                ),
+                array(
+                    [
+                        [-1.01, -1.01, -1.01, -1.01, -1.01],
+                        [-0.505, -0.505, -0.505, -0.505, -0.505],
+                        [0.0, 0.0, 0.0, 0.0, 0.0],
+                        [0.505, 0.505, 0.505, 0.505, 0.505],
+                        [1.01, 1.01, 1.01, 1.01, 1.01],
+                    ]
+                ),
+            ),
+        ]
+        for kwargs, lons_expected, lats_expected, xx_expected, yy_expected in args:
+            with self.subTest(kwargs=kwargs):
+                (
+                    lons,
+                    lats,
+                    xx,
+                    yy,
+                    transformer,
+                    info,
+                ) = self.body.generate_map_coordinates(**kwargs)
+                self.assertTrue(np.allclose(lons, lons_expected, equal_nan=True))
+                self.assertTrue(np.allclose(lats, lats_expected, equal_nan=True))
+                self.assertTrue(np.allclose(xx, xx_expected))
+                self.assertTrue(np.allclose(yy, yy_expected))
+
     def test_standardise_backplane_name(self):
         self.assertEqual(self.body.standardise_backplane_name('EMISSION'), 'EMISSION')
         self.assertEqual(self.body.standardise_backplane_name(' EMISSION '), 'EMISSION')
         self.assertEqual(self.body.standardise_backplane_name('emission'), 'EMISSION')
         self.assertEqual(self.body.standardise_backplane_name('EmIsSiOn'), 'EMISSION')
 
     def test_register_backplane(self):
@@ -832,17 +1126,21 @@
             'PIXEL-Y: Observation y pixel coordinate [pixels]',
             'KM-X: East-West distance in target plane [km]',
             'KM-Y: North-South distance in target plane [km]',
             'PHASE: Phase angle [deg]',
             'INCIDENCE: Incidence angle [deg]',
             'EMISSION: Emission angle [deg]',
             'AZIMUTH: Azimuth angle [deg]',
+            'LOCAL-SOLAR-TIME: Local solar time [local hours]',
             'DISTANCE: Distance to observer [km]',
             'RADIAL-VELOCITY: Radial velocity away from observer [km/s]',
             'DOPPLER: Doppler factor, sqrt((1 + v/c)/(1 - v/c)) where v is radial velocity',
+            'LIMB-DISTANCE: Distance above limb [km]',
+            'LIMB-LON-GRAPHIC: Planetographic longitude of closest point on the limb [deg]',
+            'LIMB-LAT-GRAPHIC: Planetographic latitude of closest point on the limb [deg]',
             'RING-RADIUS: Equatorial (ring) plane radius [km]',
             'RING-LON-GRAPHIC: Equatorial (ring) plane planetographic longitude [deg]',
             'RING-DISTANCE: Equatorial (ring) plane distance to observer [km]',
         ]
         self.assertEqual(
             self.body.backplane_summary_string(),
             '\n'.join(lines),
```

### Comparing `planetmapper-1.7.7/tests/test_common.py` & `planetmapper-1.8.0/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/tests/test_data_loader.py` & `planetmapper-1.8.0/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/tests/test_init.py` & `planetmapper-1.8.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/tests/test_kernel_downloader.py` & `planetmapper-1.8.0/tests/test_kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/tests/test_observation.py` & `planetmapper-1.8.0/tests/test_observation.py`

 * *Files 4% similar despite different names*

```diff
@@ -465,14 +465,76 @@
             with self.assertWarns(AstropyWarning):
                 obs.disc_from_wcs(validate=False, suppress_warnings=False)
 
         with warnings.catch_warnings():
             warnings.simplefilter('error')
             obs.position_from_wcs(validate=False, suppress_warnings=True)
 
+    def test_wcs_offset(self):
+        with self.assertRaises(ValueError):
+            self.observation.get_wcs_offset(suppress_warnings=True)
+        with self.assertRaises(ValueError):
+            self.observation.get_wcs_arcsec_offset(suppress_warnings=True)
+
+        x0 = 198.87871682168858
+        y0 = -31.89770255438151
+        r0 = 164.4473594677842
+        rotation = 260.32237572846986
+
+        path = os.path.join(common_testing.DATA_PATH, 'inputs', 'wcs.fits')
+        obs = Observation(path)
+
+        obs.disc_from_wcs(suppress_warnings=True)
+        self.assertTrue(
+            np.allclose(obs.get_disc_params(), (x0, y0, r0, rotation), atol=0.2)
+        )
+
+        adjustment = (1.23, -4.56, 7.89, 10.11)
+        obs.adjust_disc_params(*adjustment)
+        self.assertTrue(
+            np.allclose(obs.get_wcs_offset(suppress_warnings=True), adjustment),
+            msg=f'{obs.get_wcs_offset(suppress_warnings=True)} != {adjustment}',
+        )
+        obs.adjust_disc_params(dx=10)
+        adjustment = (1.23 + 10, -4.56, 7.89, 10.11)
+        self.assertTrue(
+            np.allclose(obs.get_wcs_offset(suppress_warnings=True), adjustment)
+        )
+
+        obs.disc_from_wcs(suppress_warnings=True)
+        obs.add_arcsec_offset(1, 2.5)
+        self.assertTrue(
+            np.allclose(obs.get_wcs_arcsec_offset(suppress_warnings=True), (1, 2.5))
+        )
+        obs.add_arcsec_offset(10)
+        self.assertTrue(
+            np.allclose(obs.get_wcs_arcsec_offset(suppress_warnings=True), (11, 2.5))
+        )
+
+        obs.disc_from_wcs(suppress_warnings=True)
+        obs.adjust_disc_params(dr=10)
+        with self.assertRaises(ValueError):
+            obs.get_wcs_arcsec_offset(suppress_warnings=True)
+        obs.get_wcs_arcsec_offset(
+            suppress_warnings=True, check_is_position_offset_only=False
+        )
+
+        obs.disc_from_wcs(suppress_warnings=True)
+        obs.adjust_disc_params(drotation=123)
+        with self.assertRaises(ValueError):
+            obs.get_wcs_arcsec_offset(suppress_warnings=True)
+        obs.get_wcs_arcsec_offset(
+            suppress_warnings=True, check_is_position_offset_only=False
+        )
+
+        # check don't get wraparound errors for small -ve drotation
+        obs.disc_from_wcs(suppress_warnings=True)
+        obs.adjust_disc_params(drotation=-1e-6)
+        obs.get_wcs_arcsec_offset(suppress_warnings=True)
+
     def test_fit_disc(self):
         data = np.ones((5, 10, 8))
         data[:, 3:5, 2:4] = 10
         obs = Observation(
             data=data,
             target='Jupiter',
             observer='hst',
@@ -693,18 +755,25 @@
         with fits.open(path) as hdul, fits.open(path_ref) as hdul_ref:
             if skip_wireframe:
                 hdul_ref = fits.HDUList(
                     [hdu for hdu in hdul_ref if hdu.name != 'WIREFRAME']
                 )
             with self.subTest('Number of backplanes', filename=filename):
                 self.assertEqual(len(hdul), len(hdul_ref))
-            for hdu, hdu_ref in zip(hdul, hdul_ref):
-                self.assertEqual(hdu.name, hdu_ref.name)
-                extname = hdu.name
-                with self.subTest(filename=filename, extname=extname):
+
+            with self.subTest('Backplane names', filename=filename):
+                self.assertEqual(
+                    set(hdu.name for hdu in hdul),
+                    set(hdu.name for hdu in hdul_ref),
+                )
+
+            for hdu_ref in hdul_ref:
+                extname = hdu_ref.name
+                hdu = hdul[extname]
+                with self.subTest('HDU data', filename=filename, extname=extname):
                     data = hdu.data
                     data_ref = hdu_ref.data
                     self.assertEqual(data.shape, data_ref.shape)
 
                     # Significantly increase tolerance for wireframe as it is generated
                     # from a Matplotlib plot, so is sensitive to the OS/environment
                     # (e.g. fonts available), and is only a cosmetic backplane anyway
@@ -713,27 +782,29 @@
                     atol = 64 if extname == 'WIREFRAME' else 1e-8  # 1e-8 is the default
                     self.assertTrue(
                         np.allclose(data, data_ref, atol=atol, equal_nan=True)
                     )
 
                 header = hdu.header
                 header_ref = hdu_ref.header
-                with self.subTest(filename=filename, extname=extname):
+                with self.subTest('HDU header', filename=filename, extname=extname):
                     self.assertEqual(set(header.keys()), set(header_ref.keys()))
 
                 keys_to_skip = {'*DATE*', '*VERSION*'}
                 for key in header.keys():
                     if any(
                         fnmatch.fnmatch(key.casefold(), pattern.casefold())
                         for pattern in keys_to_skip
                     ):
                         continue
                     value = header[key]
                     value_ref = header_ref[key]
-                    with self.subTest(filename=filename, extname=extname, key=key):
+                    with self.subTest(
+                        'HDU keader key', filename=filename, extname=extname, key=key
+                    ):
                         if isinstance(value, float):
                             self.assertAlmostEqual(value, value_ref)
                         else:
                             self.assertEqual(value, value_ref)
 
     @patch('planetmapper.gui.GUI.run')
     def test_run_gui(self, mock_run: MagicMock):
```

### Comparing `planetmapper-1.7.7/tests/test_progress.py` & `planetmapper-1.8.0/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.7.7/tests/test_utils.py` & `planetmapper-1.8.0/tests/test_utils.py`

 * *Files identical despite different names*

