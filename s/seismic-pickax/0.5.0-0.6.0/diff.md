# Comparing `tmp/seismic-pickax-0.5.0.tar.gz` & `tmp/seismic-pickax-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismic-pickax-0.5.0.tar", last modified: Fri Mar  3 16:48:10 2023, max compression
+gzip compressed data, was "seismic-pickax-0.6.0.tar", last modified: Thu Jul 27 20:12:20 2023, max compression
```

## Comparing `seismic-pickax-0.5.0.tar` & `seismic-pickax-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 crotwell   (502) staff       (20)        0 2023-03-03 16:48:10.277845 seismic-pickax-0.5.0/
--rw-r--r--   0 crotwell   (502) staff       (20)    26526 2022-11-15 17:59:53.000000 seismic-pickax-0.5.0/LICENSE
--rw-r--r--   0 crotwell   (502) staff       (20)     5506 2023-03-03 16:48:10.277688 seismic-pickax-0.5.0/PKG-INFO
--rw-r--r--   0 crotwell   (502) staff       (20)     4867 2023-02-21 21:05:01.000000 seismic-pickax-0.5.0/README.md
--rw-r--r--   0 crotwell   (502) staff       (20)     1103 2023-03-03 16:47:16.000000 seismic-pickax-0.5.0/pyproject.toml
--rw-r--r--   0 crotwell   (502) staff       (20)       38 2023-03-03 16:48:10.277889 seismic-pickax-0.5.0/setup.cfg
-drwxr-xr-x   0 crotwell   (502) staff       (20)        0 2023-03-03 16:48:10.272725 seismic-pickax-0.5.0/src/
-drwxr-xr-x   0 crotwell   (502) staff       (20)        0 2023-03-03 16:48:10.276019 seismic-pickax-0.5.0/src/pickax/
--rw-r--r--   0 crotwell   (502) staff       (20)     1567 2023-03-03 02:23:35.000000 seismic-pickax-0.5.0/src/pickax/__init__.py
--rw-r--r--   0 crotwell   (502) staff       (20)     1332 2023-02-20 15:00:07.000000 seismic-pickax-0.5.0/src/pickax/areautil.py
--rw-r--r--   0 crotwell   (502) staff       (20)     3039 2023-01-06 20:03:03.000000 seismic-pickax-0.5.0/src/pickax/blit_manager.py
--rw-r--r--   0 crotwell   (502) staff       (20)     2717 2023-02-13 21:59:07.000000 seismic-pickax-0.5.0/src/pickax/dataset.py
--rw-r--r--   0 crotwell   (502) staff       (20)     1274 2023-02-09 22:27:24.000000 seismic-pickax-0.5.0/src/pickax/dumppicks.py
--rw-r--r--   0 crotwell   (502) staff       (20)     4443 2023-02-27 17:50:19.000000 seismic-pickax-0.5.0/src/pickax/eqtransform.py
--rw-r--r--   0 crotwell   (502) staff       (20)     4349 2023-03-03 13:27:09.000000 seismic-pickax-0.5.0/src/pickax/exportreal.py
--rw-r--r--   0 crotwell   (502) staff       (20)     4555 2023-02-23 20:55:25.000000 seismic-pickax-0.5.0/src/pickax/flag.py
--rw-r--r--   0 crotwell   (502) staff       (20)     1387 2023-03-03 15:58:32.000000 seismic-pickax-0.5.0/src/pickax/help.py
--rw-r--r--   0 crotwell   (502) staff       (20)     5755 2023-03-02 17:50:47.000000 seismic-pickax-0.5.0/src/pickax/hypoinverse.py
--rw-r--r--   0 crotwell   (502) staff       (20)     1673 2023-02-17 01:27:53.000000 seismic-pickax-0.5.0/src/pickax/mergepicks.py
--rw-r--r--   0 crotwell   (502) staff       (20)    10316 2023-03-02 22:12:43.000000 seismic-pickax-0.5.0/src/pickax/pick_util.py
--rw-r--r--   0 crotwell   (502) staff       (20)    13566 2023-03-03 16:38:30.000000 seismic-pickax-0.5.0/src/pickax/pickax.py
--rw-r--r--   0 crotwell   (502) staff       (20)     3896 2023-03-03 16:12:49.000000 seismic-pickax-0.5.0/src/pickax/pickax_config.py
--rw-r--r--   0 crotwell   (502) staff       (20)     2342 2023-03-03 15:20:59.000000 seismic-pickax-0.5.0/src/pickax/pickax_main.py
--rw-r--r--   0 crotwell   (502) staff       (20)     4413 2023-02-27 16:52:51.000000 seismic-pickax-0.5.0/src/pickax/quake_iterator.py
--rw-r--r--   0 crotwell   (502) staff       (20)     7488 2023-02-25 01:27:45.000000 seismic-pickax-0.5.0/src/pickax/seismogram_iterator.py
--rw-r--r--   0 crotwell   (502) staff       (20)    13295 2023-03-03 16:34:42.000000 seismic-pickax-0.5.0/src/pickax/seismograph.py
--rw-r--r--   0 crotwell   (502) staff       (20)     2766 2023-03-02 20:07:25.000000 seismic-pickax-0.5.0/src/pickax/station_iterator.py
--rw-r--r--   0 crotwell   (502) staff       (20)     1039 2023-01-19 20:06:47.000000 seismic-pickax-0.5.0/src/pickax/traveltime.py
--rw-r--r--   0 crotwell   (502) staff       (20)     2656 2023-02-27 15:37:36.000000 seismic-pickax-0.5.0/src/pickax/usgspicks.py
--rw-r--r--   0 crotwell   (502) staff       (20)       48 2023-03-03 16:47:04.000000 seismic-pickax-0.5.0/src/pickax/version.py
-drwxr-xr-x   0 crotwell   (502) staff       (20)        0 2023-03-03 16:48:10.277487 seismic-pickax-0.5.0/src/seismic_pickax.egg-info/
--rw-r--r--   0 crotwell   (502) staff       (20)     5506 2023-03-03 16:48:10.000000 seismic-pickax-0.5.0/src/seismic_pickax.egg-info/PKG-INFO
--rw-r--r--   0 crotwell   (502) staff       (20)      835 2023-03-03 16:48:10.000000 seismic-pickax-0.5.0/src/seismic_pickax.egg-info/SOURCES.txt
--rw-r--r--   0 crotwell   (502) staff       (20)        1 2023-03-03 16:48:10.000000 seismic-pickax-0.5.0/src/seismic_pickax.egg-info/dependency_links.txt
--rw-r--r--   0 crotwell   (502) staff       (20)      268 2023-03-03 16:48:10.000000 seismic-pickax-0.5.0/src/seismic_pickax.egg-info/entry_points.txt
--rw-r--r--   0 crotwell   (502) staff       (20)       22 2023-03-03 16:48:10.000000 seismic-pickax-0.5.0/src/seismic_pickax.egg-info/requires.txt
--rw-r--r--   0 crotwell   (502) staff       (20)        7 2023-03-03 16:48:10.000000 seismic-pickax-0.5.0/src/seismic_pickax.egg-info/top_level.txt
+drwxr-xr-x   0 crotwell   (502) staff       (20)        0 2023-07-27 20:12:20.459189 seismic-pickax-0.6.0/
+-rw-r--r--   0 crotwell   (502) staff       (20)    26526 2023-02-21 20:55:05.000000 seismic-pickax-0.6.0/LICENSE
+-rw-r--r--   0 crotwell   (502) staff       (20)     5617 2023-07-27 20:12:20.459069 seismic-pickax-0.6.0/PKG-INFO
+-rw-r--r--   0 crotwell   (502) staff       (20)     4978 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/README.md
+-rw-r--r--   0 crotwell   (502) staff       (20)     1199 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/pyproject.toml
+-rw-r--r--   0 crotwell   (502) staff       (20)       38 2023-07-27 20:12:20.459221 seismic-pickax-0.6.0/setup.cfg
+drwxr-xr-x   0 crotwell   (502) staff       (20)        0 2023-07-27 20:12:20.454275 seismic-pickax-0.6.0/src/
+drwxr-xr-x   0 crotwell   (502) staff       (20)        0 2023-07-27 20:12:20.458250 seismic-pickax-0.6.0/src/pickax/
+-rw-r--r--   0 crotwell   (502) staff       (20)     1625 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/__init__.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     1332 2023-02-21 20:58:39.000000 seismic-pickax-0.6.0/src/pickax/areautil.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     3039 2023-02-21 20:55:05.000000 seismic-pickax-0.6.0/src/pickax/blit_manager.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     5508 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/distaz.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     1357 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/dumppicks.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     4443 2023-07-27 20:06:19.000000 seismic-pickax-0.6.0/src/pickax/eqtransform.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     4735 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/exportdistaz.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     4463 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/exportreal.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     6639 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/exportvelest.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     4555 2023-02-21 20:58:39.000000 seismic-pickax-0.6.0/src/pickax/flag.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     1614 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/help.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     5755 2023-07-27 20:06:19.000000 seismic-pickax-0.6.0/src/pickax/hypoinverse.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     1673 2023-02-21 20:58:39.000000 seismic-pickax-0.6.0/src/pickax/mergepicks.py
+-rw-r--r--   0 crotwell   (502) staff       (20)    13512 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/pick_util.py
+-rw-r--r--   0 crotwell   (502) staff       (20)    15696 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/pickax.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     4033 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/pickax_config.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     2580 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/pickax_main.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     5859 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/quake_iterator.py
+-rw-r--r--   0 crotwell   (502) staff       (20)    11355 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/seismogram_iterator.py
+-rw-r--r--   0 crotwell   (502) staff       (20)    13552 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/seismograph.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     5166 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/station_iterator.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     1039 2023-02-21 20:55:05.000000 seismic-pickax-0.6.0/src/pickax/traveltime.py
+-rw-r--r--   0 crotwell   (502) staff       (20)     2656 2023-07-27 20:06:19.000000 seismic-pickax-0.6.0/src/pickax/usgspicks.py
+-rw-r--r--   0 crotwell   (502) staff       (20)       48 2023-07-27 20:11:03.000000 seismic-pickax-0.6.0/src/pickax/version.py
+drwxr-xr-x   0 crotwell   (502) staff       (20)        0 2023-07-27 20:12:20.458898 seismic-pickax-0.6.0/src/seismic_pickax.egg-info/
+-rw-r--r--   0 crotwell   (502) staff       (20)     5617 2023-07-27 20:12:20.000000 seismic-pickax-0.6.0/src/seismic_pickax.egg-info/PKG-INFO
+-rw-r--r--   0 crotwell   (502) staff       (20)      888 2023-07-27 20:12:20.000000 seismic-pickax-0.6.0/src/seismic_pickax.egg-info/SOURCES.txt
+-rw-r--r--   0 crotwell   (502) staff       (20)        1 2023-07-27 20:12:20.000000 seismic-pickax-0.6.0/src/seismic_pickax.egg-info/dependency_links.txt
+-rw-r--r--   0 crotwell   (502) staff       (20)      348 2023-07-27 20:12:20.000000 seismic-pickax-0.6.0/src/seismic_pickax.egg-info/entry_points.txt
+-rw-r--r--   0 crotwell   (502) staff       (20)       22 2023-07-27 20:12:20.000000 seismic-pickax-0.6.0/src/seismic_pickax.egg-info/requires.txt
+-rw-r--r--   0 crotwell   (502) staff       (20)        7 2023-07-27 20:12:20.000000 seismic-pickax-0.6.0/src/seismic_pickax.egg-info/top_level.txt
```

### Comparing `seismic-pickax-0.5.0/LICENSE` & `seismic-pickax-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seismic-pickax-0.5.0/PKG-INFO` & `seismic-pickax-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-pickax
-Version: 0.5.0
+Version: 0.6.0
 Summary: Seismic phase picker.
 Author-email: Philip Crotwell <crotwell@seis.sc.edu>
 Project-URL: Homepage, https://github.com/crotwell/pickax
 Project-URL: Bug Tracker, https://github.com/crotwell/pickax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -64,14 +64,16 @@
 - X: Zoom back out, double time displayed
 - z: Return to original autozoom
 - w: Shift seismogram to left (west)
 - e: Shift seismogram to right (east)
 - t: Print current time, amplitude at mouse position
 - v: Go to next data
 - r: Go to previous data
+- V: Skip forward to next quake
+- R: Skip backward to previous quake
 - q: Quit
 - h: Display this help, but you knew that, right?
 
 Picks are draggable with the mouse.
 
 # Configuration
 
@@ -104,33 +106,33 @@
 If a stream is returned, that becomes
 the current displayed stream, but if None is returned, then it assumes
 the original was modified in place.
 
 # Finish function
 
 The finish function is called whenever the user quits, goes to next or previous,
-ie `q`, `v` or `r`. It is called with four arguments, first is the QuakeML
+ie `q`, `V`, `v`, `R` or `r`. It is called with four arguments, first is the QuakeML
 Event, which contains picks, including both new picks and any existing picks.
 Second is the current stream, useful to get the channel. Third is the command,
-one of "quit", "next", or "prev" and the last is pickax itself.
+one of "quit", "next", "next_quake", "prev" or "prev_quake" and the last is pickax itself.
 
 For next and prev, you generally will call
 `pickax.update_data()` passing in a new stream and optionally
 quake and inventory if they have changed.
 
 # Title
 
 The main window can fave an additional title string, generated by titleFn. The
 default is origin time, lat/lon depth and magnitude of the event. The titleFn
 takes 3 arguments, quake, inventory and stream, similar to the update_data function.
 
 # utilities
 
 - usgspicks: reload event from USGS by id to load picks as default
-query doesn not include. Likely only works if host is USGS server.
+query does not include picks. Likely only works if host is USGS server.
 
 - mergepicks: merge picks from one or more QuakeML files into another, optionally limiting to author
 
 - dumppicks: print picks from one or more QuakeML files
 
 # build hints
```

### Comparing `seismic-pickax-0.5.0/README.md` & `seismic-pickax-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 - X: Zoom back out, double time displayed
 - z: Return to original autozoom
 - w: Shift seismogram to left (west)
 - e: Shift seismogram to right (east)
 - t: Print current time, amplitude at mouse position
 - v: Go to next data
 - r: Go to previous data
+- V: Skip forward to next quake
+- R: Skip backward to previous quake
 - q: Quit
 - h: Display this help, but you knew that, right?
 
 Picks are draggable with the mouse.
 
 # Configuration
 
@@ -88,33 +90,33 @@
 If a stream is returned, that becomes
 the current displayed stream, but if None is returned, then it assumes
 the original was modified in place.
 
 # Finish function
 
 The finish function is called whenever the user quits, goes to next or previous,
-ie `q`, `v` or `r`. It is called with four arguments, first is the QuakeML
+ie `q`, `V`, `v`, `R` or `r`. It is called with four arguments, first is the QuakeML
 Event, which contains picks, including both new picks and any existing picks.
 Second is the current stream, useful to get the channel. Third is the command,
-one of "quit", "next", or "prev" and the last is pickax itself.
+one of "quit", "next", "next_quake", "prev" or "prev_quake" and the last is pickax itself.
 
 For next and prev, you generally will call
 `pickax.update_data()` passing in a new stream and optionally
 quake and inventory if they have changed.
 
 # Title
 
 The main window can fave an additional title string, generated by titleFn. The
 default is origin time, lat/lon depth and magnitude of the event. The titleFn
 takes 3 arguments, quake, inventory and stream, similar to the update_data function.
 
 # utilities
 
 - usgspicks: reload event from USGS by id to load picks as default
-query doesn not include. Likely only works if host is USGS server.
+query does not include picks. Likely only works if host is USGS server.
 
 - mergepicks: merge picks from one or more QuakeML files into another, optionally limiting to author
 
 - dumppicks: print picks from one or more QuakeML files
 
 # build hints
```

### Comparing `seismic-pickax-0.5.0/pyproject.toml` & `seismic-pickax-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seismic-pickax"
-version = "0.5.0"  # also in version.py
+version = "0.6.0"  # also in version.py
 authors = [
   { name="Philip Crotwell", email="crotwell@seis.sc.edu" },
 ]
 description = "Seismic phase picker."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -31,7 +31,9 @@
     "pickax" = "pickax.pickax_main:main"
     "usgspicks" = "pickax.usgspicks:main"
     "mergepicks" = "pickax.mergepicks:main"
     "dumppicks" = "pickax.dumppicks:main"
     "eqtranspicks" = "pickax.eqtransform:main"
     "hypoinverse" = "pickax.hypoinverse:main"
     "exportreal" = "pickax.exportreal:main"
+    "exportvelest" = "pickax.exportvelest:main"
+    "exportdistaz" = "pickax.exportdistaz:main"
```

### Comparing `seismic-pickax-0.5.0/src/pickax/__init__.py` & `seismic-pickax-0.6.0/src/pickax/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,20 +21,22 @@
     CachedPicksQuakeItr
     )
 from .station_iterator import (
     StationIterator,
     StationXMLIterator,
     FDSNStationIterator,
     StationXMLFileIterator,
+    StationXMLDirectoryIterator
     )
 from .seismogram_iterator import (
     SeismogramIterator,
     FDSNSeismogramIterator,
     ThreeAtATime,
     CacheSeismogramIterator,
+    MDLSeismogramIterator
     )
 from .hypoinverse import format_hypoinverse
 from .eqtransform import read_eqt_csv
 from .traveltime import TravelTimeCalc
 from .version import __version__
 
 version = __version__
```

### Comparing `seismic-pickax-0.5.0/src/pickax/areautil.py` & `seismic-pickax-0.6.0/src/pickax/areautil.py`

 * *Files identical despite different names*

### Comparing `seismic-pickax-0.5.0/src/pickax/blit_manager.py` & `seismic-pickax-0.6.0/src/pickax/blit_manager.py`

 * *Files identical despite different names*

### Comparing `seismic-pickax-0.5.0/src/pickax/dumppicks.py` & `seismic-pickax-0.6.0/src/pickax/dumppicks.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,12 +35,14 @@
         print()
         print(qmlfile)
         print("---------------------------")
         in_catalog = read_events(Path(qmlfile))
         for in_quake in in_catalog:
             print(in_quake.short_str())
             for pick in in_quake.picks:
-                if args.author is None or pick.creation_info.author == args.author:
+                if args.author is None \
+                or pick.creation_info.author == args.author \
+                or pick.creation_info.agency_id == args.author:
                     print(f"    {pick_to_string(pick, in_quake)}")
 
 if __name__ == "__main__":
     main()
```

### Comparing `seismic-pickax-0.5.0/src/pickax/eqtransform.py` & `seismic-pickax-0.6.0/src/pickax/eqtransform.py`

 * *Files identical despite different names*

### Comparing `seismic-pickax-0.5.0/src/pickax/exportreal.py` & `seismic-pickax-0.6.0/src/pickax/exportreal.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,16 +85,18 @@
     outdir = Path(".")
     if args.dir is not None:
         outdir = Path(args.dir)
         if not outdir.exists():
             outdir.mkdir(parents=True, exist_ok=True)
     if args.staxml:
         inv = read_inventory(args.staxml)
-        lines = format_hypoinverse(inv)
-        outfile = Path(outdir / f"{args.staxml}.sta")
+        lines = format_real(inv)
+
+        in_path = Path(args.staxml)
+        outfile = Path(outdir / f"{in_path.stem}.sta")
         with open(outfile, "w") as f:
             for l in lines:
                 f.write(f"{l}\n")
     if args.quakeml:
         quakemlPath = Path(args.quakeml)
         if quakemlPath.exists():
             catalog_file = Path(args.quakeml)
@@ -106,14 +108,16 @@
             return
         catalog = read_events(args.quakeml)
         outfile = Path(outdir / f"{quakemlPath.stem}.phs")
         with open(outfile, "w") as phsfile:
             for idx, quake in enumerate(catalog):
                 phsfile.write(f"{qml_to_phs_header(quake, idx+1)}\n")
                 for pick in quake.picks:
+                    if pick.phase_hint == "pick":
+                        continue
                     if args.authors is None or len(args.authors) == 0 \
                             or pick.creation_info.author in args.authors \
                             or pick.creation_info.agency_id in args.authors:
                         phsfile.write(f"{pick_to_phs(pick, quake)}\n")
         if args.invws:
             inv = inventory_for_catalog_picks(catalog, args.authors)
             outfile = Path(outdir / f"pick_channels.staxml")
```

### Comparing `seismic-pickax-0.5.0/src/pickax/flag.py` & `seismic-pickax-0.6.0/src/pickax/flag.py`

 * *Files identical despite different names*

### Comparing `seismic-pickax-0.5.0/src/pickax/hypoinverse.py` & `seismic-pickax-0.6.0/src/pickax/hypoinverse.py`

 * *Files identical despite different names*

### Comparing `seismic-pickax-0.5.0/src/pickax/mergepicks.py` & `seismic-pickax-0.6.0/src/pickax/mergepicks.py`

 * *Files identical despite different names*

### Comparing `seismic-pickax-0.5.0/src/pickax/pick_util.py` & `seismic-pickax-0.6.0/src/pickax/pick_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -159,16 +159,15 @@
             if p.time == catp.time and \
                 p.creation_info is not None and \
                 catp.creation_info is not None and \
                 p.creation_info.author == catp.creation_info.author:
                 found = True
                 break
         if not found:
-            to_add.append(p)
-    out_qmlevent.picks = out_qmlevent.picks + to_add
+            out_qmlevent.picks.append(p)
     for p in to_add:
         arr = arrival_for_pick(p, qmlevent)
         if arr is not None:
             # ?? what origin to add too
             out_qmlevent.preferred_origin().arrivals.append(arr)
         amp = amplitude_for_pick(p, qmlevent)
         if amp is not None:
@@ -184,15 +183,15 @@
         if extractEventId(q) == id:
             found_quake = True
             merge_picks_to_quake(qmlevent, q, author=author)
             break
     if not found_quake:
         clean_quake = qmlevent.copy()
         if author is not None:
-            clean_quake.picks = filter(lambda p: p.creation_info.agency_id == author or p.creation_info.author == author, clean_quake.picks)
+            clean_quake.picks = list(filter(lambda p: p.creation_info.agency_id == author or p.creation_info.author == author, clean_quake.picks))
         catalog.append(clean_quake)
     return catalog
 
 
 def UNKNOWN_PUBLIC_ID():
     length = 8
     letters = string.ascii_lowercase
@@ -249,11 +248,89 @@
 
 def inventory_for_catalog_picks(catalog, window=600, client=None, host="IRIS", debug=False):
     wid_list = []
     for qmlevent in catalog:
         otime = qmlevent.preferred_origin().time
         for pick in qmlevent.picks:
             wid = pick.waveform_id
-            wid_list.append((wid.network_code, wid.station_code, wid.location_code, wid.channel_code, otime, (otime+600)))
+            if wid.network_code is None or \
+                wid.station_code is None or \
+                wid.location_code is None or \
+                wid.channel_code is None:
+                print(f"None in Waveform_Id: {wid.network_code}, {wid.station_code}, {wid.location_code}, {wid.channel_code} for pick on {otime}")
+            else:
+                wid_list.append((wid.network_code, wid.station_code, wid.location_code, wid.channel_code, otime, (otime+600)))
     if client is None:
         client = Client(host, _discover_services=False, debug=debug)
     return client.get_stations_bulk(wid_list, level="channel", )
+
+def station_for_pick(pick, inventory):
+    wid = pick.waveform_id
+    if wid.network_code is None or wid.station_code is None:
+        return None
+    for n in inventory.networks:
+        if n.code == wid.network_code:
+            for s in n.stations:
+                if s.code == wid.station_code:
+                    return s
+    return None
+
+DEF_INST_LIST = ["H", "N"]
+
+def picks_by_author(pick_list, author):
+    return [pick for pick in pick_list if \
+                pick.creation_info.author == author \
+                or pick.creation_info.agency_id == author]
+
+def best_pick_at_station(pick_list, p_s, station_id, quake,
+                         author_list=[],
+                         inst_list=DEF_INST_LIST,
+                         check_unique=False):
+    all_picks = []
+    for pick in pick_list:
+        a = arrival_for_pick(pick, quake)
+        pname = a.phase if a is not None and a.phase is not None else pick.phase_hint
+        if pname == p_s:
+            all_picks.append(pick)
+    all_picks = [p for p in all_picks if \
+                 station_id == f"{p.waveform_id.network_code}.{p.waveform_id.station_code}"]
+    if len(author_list) != 0:
+        for au in author_list:
+            au_picks = picks_by_author(all_picks, au)
+            if len(au_picks) > 0:
+                pick = best_instrument_pick(au_picks,
+                                            station_id,
+                                            inst_list=DEF_INST_LIST,
+                                            check_unique=check_unique)
+                if pick is not None:
+                    return pick
+        # didn't find by author, so none?
+        return None
+    else:
+        return best_instrument_pick(all_picks,
+                                    station_id,
+                                    inst_list=DEF_INST_LIST,
+                                    check_unique=check_unique)
+
+def best_instrument_pick(pick_list,
+                         station_id,
+                         inst_list=DEF_INST_LIST,
+                         check_unique=False):
+    """
+    Finds pick on best (first in list) instrument code.
+    """
+    all_picks = [p for p in pick_list if \
+         station_id == f"{p.waveform_id.network_code}.{p.waveform_id.station_code}"]
+    for inst in inst_list:
+        inst_picks = [pick for pick in all_picks if pick.waveform_id.channel_code[1] == inst]
+        if len(inst_picks) == 0:
+            pass
+        elif check_unique and len(inst_picks)>1:
+            raise Exception(f"More than one pick satisfies criteria for {station_id} on {inst}: {len(inst_picks)}")
+        else:
+            return inst_picks[0]
+    if len(all_picks) == 0:
+        return None
+    elif check_unique and len(all_picks)>1:
+        raise Exception(f"More than one pick satisfies criteria for {station_id}: {len(all_picks)}")
+    else:
+        return all_picks[0]
```

### Comparing `seismic-pickax-0.5.0/src/pickax/pickax.py` & `seismic-pickax-0.6.0/src/pickax/pickax.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,23 +216,70 @@
             self.fig.canvas.draw_idle()
         elif self.config.keymap[event.key] == "AMP_MODE":
             self.config.toggle_amplitude_mode()
             if self.config.amplitude_mode == GLOBAL_AMP:
                 gl_min, gl_max = self.calc_global_amp()
                 for sg in self.seismographList:
                     sg.set_ylim(gl_min, gl_max)
+            else:
+                for sg in self.seismographList:
+                    sg.unset_ylim()
             for sg in self.seismographList:
-                sg.refresh_display()
+                sg.draw()
             self.fig.canvas.draw_idle()
         elif self.config.keymap[event.key] =="GO_QUIT":
             self.do_finish("quit")
         elif self.config.keymap[event.key]  == "GO_NEXT":
             self.do_finish("next")
         elif self.config.keymap[event.key]  == "GO_PREV":
             self.do_finish("prev")
+        elif self.config.keymap[event.key]  == "GO_NEXT_QUAKE":
+            if self.config.seismogram_itr is not None:
+                sta_itr = self.config.seismogram_itr.station_iterator()
+                if sta_itr is not None:
+                    sta_itr.ending()
+            self.do_finish("next")
+        elif self.config.keymap[event.key]  == "GO_PREV_QUAKE":
+            if self.config.seismogram_itr is not None:
+                sta_itr = self.config.seismogram_itr.station_iterator()
+                if sta_itr is not None:
+                    sta_itr.beginning()
+                quake_itr = self.config.seismogram_itr.quake_iterator()
+                if quake_itr is not None:
+                    quake_itr.prev()
+            self.do_finish("prev")
+        elif self.config.keymap[event.key]  == "LIST_QUAKES":
+            all = None
+            if self.config.seismogram_itr is not None:
+                quake_itr = self.config.seismogram_itr.quake_iterator()
+                if quake_itr is not None:
+                    all = quake_itr.all()
+            if all is not None:
+                for q in all:
+                    o = q.preferred_origin()
+                    m = q.preferred_magnitude()
+                    mstr = "    "
+                    if m is not None:
+                        mstr = f"{m.mag}{m.magnitude_type}"
+                    print(f"{o.time} {mstr} ({o.latitude}/{o.longitude})".strip())
+            else:
+                print("Iterator does not allow access to all quakes")
+
+        elif self.config.keymap[event.key]  == "LIST_STATIONS":
+            all = None
+            if self.config.seismogram_itr is not None:
+                sta_itr = self.config.seismogram_itr.station_iterator()
+                if sta_itr is not None:
+                    all = sta_itr.all_stations()
+            if all is not None:
+                for s in all:
+                    print(f"{s.code} ({s.latitude}/{s.longitude})")
+            else:
+                print("Iterator does not allow access to all stations")
+
         elif self.config.keymap[event.key]  == "PICK_GENERIC":
             if event.inaxes is not None:
                 self.do_pick(event)
             self.fig.canvas.draw_idle()
         elif self.config.keymap[event.key]  == "PICK_P":
             if event.inaxes is not None:
                 self.do_pick(event, phase="P")
```

### Comparing `seismic-pickax-0.5.0/src/pickax/pickax_config.py` & `seismic-pickax-0.6.0/src/pickax/pickax_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     'X': "ZOOM_OUT",
     'z': "ZOOM_ORIG",
     'w': "WEST",
     'e': "EAST",
     't': "CURR_MOUSE",
     'v': "GO_NEXT",
     'r': "GO_PREV",
+    'V': "GO_NEXT_QUAKE",
+    'R': "GO_PREV_QUAKE",
+    '*': "LIST_QUAKES",
+    '^': "LIST_STATIONS",
     'q': "GO_QUIT",
     'h': "HELP",
 }
 
 TRACE_AMP = "TRACE_AMP"
 WINDOW_AMP = "WINDOW_AMP"
 GLOBAL_AMP = "GLOBAL_AMP"
@@ -44,14 +48,15 @@
         self._keymap = {}
         self.debug = False
         self.verbose = False
         self.scroll_factor = 8
         self.author_colors = {}
         self.titleFn = default_titleFn
         self.finishFn = None
+        self.seismogram_itr = None
         self.creation_info = None
         self.resource_prefix="smi:pickax"
         self.filters = []
         self.phase_list = []
         self._model =  None
         self.amplitude_mode = TRACE_AMP
         self.figsize=(10,8)
```

### Comparing `seismic-pickax-0.5.0/src/pickax/pickax_main.py` & `seismic-pickax-0.6.0/src/pickax/pickax_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from IPython import embed;
 from IPython.core.getipython import get_ipython
 from .pickax import PickAx
 from .version import __version__
+
+import logging
 import obspy
 from obspy.core.event.base import CreationInfo
 import IPython
 import sys
 import os
 
+import faulthandler
+faulthandler.enable()
+
 from traitlets.config import Config
 
 import argparse
 
 
 def do_parseargs():
     parser = argparse.ArgumentParser(
@@ -35,26 +40,31 @@
         required=False,
         help="Seismogram file, loaded at startup",
     )
     return parser.parse_args()
 
 def main():
     print("Hi PickAx!")
+    print(f"Version: {__version__}")
     print("'h' in the display window will show key help.")
     args = do_parseargs()
     if args.version:
         print(__version__)
         return
+    if args.verbose:
+        logging.basicConfig(level=logging.DEBUG)
 
     c = Config()
     c.InteractiveShellApp.exec_lines = [
         'import math',
         'from obspy.core.event.base import CreationInfo',
         'import obspy',
         'from pickax import PickAx',
+        'import matplotlib',
+        'print(matplotlib.get_backend())',
         'import matplotlib.pyplot as plt',
         "plt.rcParams['toolbar'] = 'None'",
         "plt.rcParams['keymap.fullscreen'].remove('f')",
     ]
     if args.loader:
         if not os.path.exists(args.loader):
             print(f"File {args.loader} does not seem to exist, cowardly quitting...")
```

### Comparing `seismic-pickax-0.5.0/src/pickax/quake_iterator.py` & `seismic-pickax-0.6.0/src/pickax/quake_iterator.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         return None
     @abstractmethod
     def prev(self):
         return None
     @abstractmethod
     def beginning(self):
         pass
+    def all(self):
+        return None
 
 class QuakeMLFileIterator(QuakeIterator):
     def __init__(self, file):
         self.quakes = read_events(file)
         self.batch_idx = -1
     def next(self):
         self.batch_idx += 1
@@ -41,14 +43,55 @@
         self.batch_idx -= 1
         if self.batch_idx < 0:
             self.batch_idx = -1
             return None
         return self.quakes[self.batch_idx]
     def beginning(self):
         self.batch_idx = -1
+    def all(self):
+        return self.quakes
+
+
+class QuakeMLDirectoryIterator(QuakeIterator):
+    """
+    Looks for QuakeML files like *.qml and iterates the quakes in
+    each file.
+    """
+    def __init__(self, dir, pattern="**/*.qml"):
+        self.root_dir = Path(dir)
+        self.pattern = pattern
+        self.qmlfiles = list(root_dir.glob(pattern))
+
+        self.quakes = Catalog()
+        self.q_to_dir = dict()
+        for file in self.qmlfiles:
+            dir_quakes = read_events(file)
+            self.quakes.extend(dir_quakes)
+            for q in dir_quakes:
+                self.q_to_dir[q.resource_id] = file
+        self.batch_idx = -1
+    def next(self):
+        self.batch_idx += 1
+        if self.batch_idx >= len(self.quakes):
+            #self.next_batch()
+            return None
+        quake = self.quakes[self.batch_idx]
+        return quake
+    def prev(self):
+        self.batch_idx -= 1
+        if self.batch_idx < 0:
+            self.batch_idx = -1
+            return None
+        return self.quakes[self.batch_idx]
+    def beginning(self):
+        self.batch_idx = -1
+    def all(self):
+        return self.quakes
+    def quakedir(self, quake):
+        return self.q_to_dir[quake.resource_id]
 
 class FDSNQuakeIterator(QuakeIterator):
     def __init__(self, query_params, days_step=30, dc_name="USGS", debug=False):
         self.debug = debug
         self.dc_name = dc_name
         self._client = None
         self.query_params = dict(query_params)
@@ -60,14 +103,15 @@
         self.batch_idx = -1
     @property
     def client(self):
         if self._client is None:
             self._client = Client(self.dc_name, _discover_services=False, debug=self.debug)
         return self._client
     def next_batch(self):
+        # careful if implement batching, as all() will be wrong in that case?
         try:
             return self.client.get_events(**self.query_params)
         except FDSNNoDataException:
             # return empty catalog instaed of exception
             return Catalog([])
     def next_batch_step(self):
         t1 = self.__curr_end
@@ -99,14 +143,16 @@
         self.batch_idx -= 1
         if self.batch_idx < 0:
             self.batch_idx = -1
             return None
         return self.quakes[self.batch_idx]
     def beginning(self):
         self.batch_idx = -1
+    def all(self):
+        return self.quakes
 
 class CachedPicksQuakeItr(QuakeIterator):
     def __init__(self, quake_itr, cachedir='by_eventid'):
         self.quake_itr = quake_itr
         self.quakes = self.quake_itr.quakes
         self.cachedir = Path(cachedir)
         self.bad_file_chars_pat = re.compile(r'[\s:\(\)/]+')
@@ -125,7 +171,9 @@
         eid = extractEventId(quake)
         qfile = f"eventid_{re.sub(self.bad_file_chars_pat, '_', eid)}.qml"
         qpath=  Path(self.cachedir / qfile)
         if qpath.exists():
             pick_quake = read_events(qpath)[0]
             merge_picks_to_quake(pick_quake, quake)
         return quake
+    def all(self):
+        return self.quake_itr.all()
```

### Comparing `seismic-pickax-0.5.0/src/pickax/seismogram_iterator.py` & `seismic-pickax-0.6.0/src/pickax/seismogram_iterator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,102 @@
 from abc import ABC, abstractmethod
 from collections import deque
+from obspy.core.stream import read as obspyread
 from obspy.clients.fdsn import Client
 from obspy.taup import TauPyModel
 from obspy.geodetics import locations2degrees
-from obspy.clients.fdsn.header import FDSNNoDataException
+from obspy.clients.fdsn.header import FDSNNoDataException, FDSNBadRequestException
 from obspy import Stream
+from pathlib import Path
+from .station_iterator import channel_from_sac, StationXMLDirectoryIterator
+from .quake_iterator import QuakeMLFileIterator
 
 
 class SeismogramIterator(ABC):
+    """
+    Seismogram iterator that can move to next or previous.
+    Optionally, may provide access to station and quake iterators, if used
+    internally.
+    """
     def __init__(self):
         self.__empty__ = None, None, None, []
     @abstractmethod
     def next(self):
         return self.__empty__
     @abstractmethod
     def prev(self):
         return self.__empty__
+    def quake_iterator(self):
+        return None
+    def station_iterator(self):
+        return None
+
+class MDLSeismogramIterator(SeismogramIterator):
+    """
+    Seismogram iterator over a obspy mass downloader directory.
+    """
+    def __init__(self, mdl_dir, mseed_storage = "waveforms", stationxml_storage = "stations", quakeml="*.qml"):
+        self.__empty__ = None, None, None, []
+        self.mdl_dir = Path(mdl_dir)
+        self.mseed_dir = Path(self.mdl_dir, mseed_storage)
+        quakeml_list = list(self.mdl_dir.glob(quakeml))
+        if len(quakeml_list) != 1:
+            print(f"expected one quakeml file but found {len(quakeml_list)} in {mdl_dir} for {quakeml}")
+        self.quakeml = quakeml_list[0]
+        self.quake_itr = QuakeMLFileIterator(self.quakeml)
+        self.curr_quake = self.quake_itr.next()
+        self.station_itr = StationXMLDirectoryIterator(self.mdl_dir, f"{stationxml_storage}/*.xml")
+        self.idx = -1
+
+    def next(self):
+        if self.curr_quake is None:
+            return self.__empty__
+        net, sta = self.station_itr.next()
+        if sta is None:
+            quake = self.quake_itr.next()
+            if quake is None:
+                return self.__empty__
+            self.curr_quake = quake
+            self.station_itr.beginning()
+            net, sta = self.station_itr.next()
+        if sta is None or self.curr_quake is None:
+            return self.__empty__
+        return self.__load_seismograms__(net, sta, self.curr_quake)
+    def prev(self):
+        if self.curr_quake is None:
+            return self.__empty__
+        net, sta = self.station_itr.prev()
+        if sta is None:
+            self.curr_quake = self.quake_itr.prev()
+            self.station_itr.ending()
+            net, sta = self.station_itr.prev()
+            if self.curr_quake is None:
+                return self.__empty__
+
+        if sta is None or self.curr_quake is None:
+            return self.__empty__
+        return self.__load_seismograms__(net, sta, self.curr_quake)
+    def quake_iterator(self):
+        return self.quake_itr
+    def station_iterator(self):
+        return self.station_itr
+    def __load_seismograms__(self, net, sta, quake, query_params={}):
+        print(f"search in {self.mseed_dir} for {net.code}.{sta.code}.*__*__*.mseed")
+        mseed_list = list(self.mseed_dir.glob(f"{net.code}.{sta.code}.*__*__*.mseed"))
+        waveforms = Stream()
+        for mseedfile in mseed_list:
+            st = obspyread(mseedfile, format="MSEED")
+            if st is not None:
+                waveforms += st
+        return net, sta, quake, waveforms
+    def quake_iterator(self):
+        return self.quake_itr
+    def station_iterator(self):
+        return self.station_itr
+
 
 class CacheSeismogramIterator(SeismogramIterator):
     """
     Very simple cache, remembers prev, curr and next data
     for up to size items
     """
     def __init__(self, sub_itr, size=10):
@@ -40,14 +117,18 @@
         if self.__curr_data__ is not None:
             self.__next_cache__.append(self.__curr_data__)
         if len(self.__prev_cache__) > 0:
             self.__curr_data__ = self.__prev_cache__.pop()
         else:
             self.__curr_data__ = self.sub_itr.prev()
         return self.__curr_data__
+    def quake_iterator(self):
+        return self.sub_itr.quake_iterator()
+    def station_iterator(self):
+        return self.sub_itr.station_iterator()
 
 
 class FDSNSeismogramIterator(SeismogramIterator):
     def __init__(self,
                  quake_itr,
                  station_itr,
                  dc_name="IRIS",
@@ -91,46 +172,57 @@
             net, sta = self.station_itr.prev()
             if self.curr_quake is None:
                 return self.__empty__
 
         if sta is None or self.curr_quake is None:
             return self.__empty__
         return self.__load_seismograms__(net, sta, self.curr_quake, self.query_params)
+    def quake_iterator(self):
+        return self.quake_itr
+    def station_iterator(self):
+        return self.station_itr
     def __load_seismograms__(self, net, sta, quake, query_params={}):
         if len(sta.channels) == 0:
             return []
         client = Client(self.dc_name, _discover_services=False, debug=self.debug, timeout=self.timeout)
         origin = quake.preferred_origin()
         if origin is None:
             return self.__empty__
         dist_deg = locations2degrees(sta.latitude, sta.longitude, origin.latitude, origin.longitude)
         s_time = origin.time + self.start_offset
         if self.start_phases != "origin":
-            arrivals = model.get_travel_times(source_depth_in_km=origin.depth/1000,
+            arrivals = self.taup_model.get_travel_times(source_depth_in_km=origin.depth/1000,
                                       distance_in_degree=dist_deg,
                                       phase_list=self.start_phases.split(","))
             if len(arrivals) == 0:
                 return self.__empty__
             s_time = s_time + arrivals[0].time
         e_time = origin.time + self.end_offset
         if self.end_phases != "origin":
-            arrivals = model.get_travel_times(source_depth_in_km=origin.depth/1000,
+            arrivals = self.taup_model.get_travel_times(source_depth_in_km=origin.depth/1000,
                                       distance_in_degree=dist_deg,
                                       phase_list=self.end_phases.split(","))
             if len(arrivals) == 0:
                 return self.__empty__
             e_time = e_time + arrivals[0].time
         locs = set()
         chans = set()
         for c in sta.channels:
             locs.add(c.location_code)
             chans.add(c.code)
+
         waveforms = None
         try:
-            waveforms = client.get_waveforms(net.code, sta.code, ",".join(locs), ",".join(chans), s_time, e_time)
+            locstr = ",".join(locs)
+            chanstr = ",".join(chans)
+            if e_time > s_time:
+                waveforms = client.get_waveforms(net.code, sta.code, locstr, chanstr, s_time, e_time)
+            else:
+                print(f"WARN: start time for request after end time, skipping: {net.code} {sta.code} {locstr} {chanstr} {s_time} {e_time}")
+                waveforms = Stream()
         except FDSNNoDataException:
             waveforms = Stream()
         return net, sta, quake, waveforms
 
 class ThreeAtATime(SeismogramIterator):
     """
     Iterates over a sub-SeismogramIterator grouping the resulting seismograms
@@ -181,7 +273,11 @@
         # load next batch
         self.split_3c(*self.sub_itr.prev())
         self.sub_idx = len(self.sub_waveforms)-1
         if self.sub_idx >= 0:
             return self.cur_net, self.cur_sta, self.cur_quake, self.sub_waveforms[self.sub_idx]
         else:
             return self.cur_net, self.cur_sta, self.cur_quake, []
+    def quake_iterator(self):
+        return self.sub_itr.quake_iterator()
+    def station_iterator(self):
+        return self.sub_itr.station_iterator()
```

### Comparing `seismic-pickax-0.5.0/src/pickax/seismograph.py` & `seismic-pickax-0.6.0/src/pickax/seismograph.py`

 * *Files 6% similar despite different names*

```diff
@@ -254,30 +254,38 @@
         self.ylim = None
         self.ax.set_ylim(auto=True)
         self.refresh_display()
     def set_ylim(self, min_amp, max_amp):
         self.ylim = (min_amp, max_amp)
         self.ax.set_ylim(*self.ylim)
         self.refresh_display()
+    def set_xlim(self, start, end):
+        self.xlim = (start, end)
+        self.ax.set_xlim(*self.xlim)
+        self.refresh_display()
+    def unset_xlim(self):
+        self.xlim = None
+        self.ax.set_xlim(auto=True)
+        self.refresh_display()
     def refresh_display(self):
         self.clear_flags()
         self.clear_trace()
         self.draw_stream()
         self.draw_all_flags()
     def unset_zoom(self):
         self._prev_zoom_time = None
         self.unset_zoom_bound()
     def do_zoom(self, event):
         # event.key=="x":
         if self._prev_zoom_time is not None:
             self.unset_zoom_bound()
             if event.xdata > self._prev_zoom_time:
-                self.ax.set_xlim(left=self._prev_zoom_time, right=event.xdata)
+                self.set_xlim(self._prev_zoom_time, event.xdata)
             else:
-                self.ax.set_xlim(left=event.xdata, right=self._prev_zoom_time)
+                self.set_xlim(event.xdata, self._prev_zoom_time)
             self.zoom_amp()
             self._prev_zoom_time = None
         else:
             self._prev_zoom_time = event.xdata
             xmin, xmax, ymin, ymax = self.ax.axis()
             mean = (ymin+ymax)/2
             hw = 0.9*(ymax-ymin)/2
@@ -286,20 +294,21 @@
             color = "black"
             (ln,) = self.ax.plot(x,y,color=color, lw=1)
             self.set_zoom_bound(ln)
 
     def do_zoom_out(self):
         xmin, xmax, ymin, ymax = self.ax.axis()
         xwidth = xmax - xmin
-        self.ax.set_xlim(xmin-xwidth/2, xmax+xwidth/2)
+        self.set_xlim(xmin-xwidth/2, xmax+xwidth/2)
         self.zoom_amp()
         self.unset_zoom_bound()
     def do_zoom_original(self):
-        self.ax.set_xlim(auto=True)
-        self.ax.set_ylim(auto=True)
+        self.unset_xlim()
+        if self.config.amplitude_mode == TRACE_AMP:
+            self.unset_ylim()
         self.unset_zoom_bound()
         self.clear_flags()
         self.clear_trace()
         self.draw_stream()
         self.draw_all_flags()
     def set_zoom_bound(self, art):
         self._zoom_bounds = [art]
@@ -310,15 +319,15 @@
 
     def mouse_time_amp(self, event):
         offset = event.xdata
         time = self.start + offset
         amp = event.ydata
         return time, amp, offset
     def update_xlim(self, xmin, xmax):
-        self.ax.set_xlim(xmin, xmax)
+        self.set_xlim(xmin, xmax)
         self.zoom_amp()
     def list_channels(self):
         """
         Lists the channel codes for all traces in the stream, removing duplicates.
         Usually all traces will be from a single channel.
         """
         chans = ""
```

### Comparing `seismic-pickax-0.5.0/src/pickax/traveltime.py` & `seismic-pickax-0.6.0/src/pickax/traveltime.py`

 * *Files identical despite different names*

### Comparing `seismic-pickax-0.5.0/src/pickax/usgspicks.py` & `seismic-pickax-0.6.0/src/pickax/usgspicks.py`

 * *Files identical despite different names*

### Comparing `seismic-pickax-0.5.0/src/seismic_pickax.egg-info/PKG-INFO` & `seismic-pickax-0.6.0/src/seismic_pickax.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-pickax
-Version: 0.5.0
+Version: 0.6.0
 Summary: Seismic phase picker.
 Author-email: Philip Crotwell <crotwell@seis.sc.edu>
 Project-URL: Homepage, https://github.com/crotwell/pickax
 Project-URL: Bug Tracker, https://github.com/crotwell/pickax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -64,14 +64,16 @@
 - X: Zoom back out, double time displayed
 - z: Return to original autozoom
 - w: Shift seismogram to left (west)
 - e: Shift seismogram to right (east)
 - t: Print current time, amplitude at mouse position
 - v: Go to next data
 - r: Go to previous data
+- V: Skip forward to next quake
+- R: Skip backward to previous quake
 - q: Quit
 - h: Display this help, but you knew that, right?
 
 Picks are draggable with the mouse.
 
 # Configuration
 
@@ -104,33 +106,33 @@
 If a stream is returned, that becomes
 the current displayed stream, but if None is returned, then it assumes
 the original was modified in place.
 
 # Finish function
 
 The finish function is called whenever the user quits, goes to next or previous,
-ie `q`, `v` or `r`. It is called with four arguments, first is the QuakeML
+ie `q`, `V`, `v`, `R` or `r`. It is called with four arguments, first is the QuakeML
 Event, which contains picks, including both new picks and any existing picks.
 Second is the current stream, useful to get the channel. Third is the command,
-one of "quit", "next", or "prev" and the last is pickax itself.
+one of "quit", "next", "next_quake", "prev" or "prev_quake" and the last is pickax itself.
 
 For next and prev, you generally will call
 `pickax.update_data()` passing in a new stream and optionally
 quake and inventory if they have changed.
 
 # Title
 
 The main window can fave an additional title string, generated by titleFn. The
 default is origin time, lat/lon depth and magnitude of the event. The titleFn
 takes 3 arguments, quake, inventory and stream, similar to the update_data function.
 
 # utilities
 
 - usgspicks: reload event from USGS by id to load picks as default
-query doesn not include. Likely only works if host is USGS server.
+query does not include picks. Likely only works if host is USGS server.
 
 - mergepicks: merge picks from one or more QuakeML files into another, optionally limiting to author
 
 - dumppicks: print picks from one or more QuakeML files
 
 # build hints
```

### Comparing `seismic-pickax-0.5.0/src/seismic_pickax.egg-info/SOURCES.txt` & `seismic-pickax-0.6.0/src/seismic_pickax.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 README.md
 pyproject.toml
 src/pickax/__init__.py
 src/pickax/areautil.py
 src/pickax/blit_manager.py
-src/pickax/dataset.py
+src/pickax/distaz.py
 src/pickax/dumppicks.py
 src/pickax/eqtransform.py
+src/pickax/exportdistaz.py
 src/pickax/exportreal.py
+src/pickax/exportvelest.py
 src/pickax/flag.py
 src/pickax/help.py
 src/pickax/hypoinverse.py
 src/pickax/mergepicks.py
 src/pickax/pick_util.py
 src/pickax/pickax.py
 src/pickax/pickax_config.py
```

