# Comparing `tmp/glview-1.5.4.tar.gz` & `tmp/glview-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glview-1.5.4.tar", last modified: Tue Jun 13 14:00:33 2023, max compression
+gzip compressed data, was "glview-1.5.5.tar", last modified: Thu Jul 27 07:16:45 2023, max compression
```

## Comparing `glview-1.5.4.tar` & `glview-1.5.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-06-13 14:00:33.719439 glview-1.5.4/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 glview-1.5.4/LICENSE
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       99 2023-03-13 15:45:56.000000 glview-1.5.4/MANIFEST.in
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      829 2023-06-13 14:00:33.719439 glview-1.5.4/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      380 2023-05-03 12:54:40.000000 glview-1.5.4/README.md
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-06-13 14:00:33.719439 glview-1.5.4/glview/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      332 2023-03-15 12:51:16.000000 glview-1.5.4/glview/__init__.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15417 2023-03-13 15:45:56.000000 glview-1.5.4/glview/argv.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    11756 2023-05-12 14:23:54.000000 glview-1.5.4/glview/glrenderer.py
--rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)     9369 2023-06-13 13:48:47.000000 glview-1.5.4/glview/glview.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     8698 2023-06-13 13:58:46.000000 glview-1.5.4/glview/imageprovider.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      297 2023-05-09 09:52:42.000000 glview-1.5.4/glview/panzoom.vs
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    17722 2023-06-13 13:48:47.000000 glview-1.5.4/glview/pygletui.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     4546 2023-06-13 13:48:47.000000 glview-1.5.4/glview/texture.fs
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-06-13 13:54:28.000000 glview-1.5.4/glview/version.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-06-13 14:00:33.719439 glview-1.5.4/glview.egg-info/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      829 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      431 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/SOURCES.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/dependency_links.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       39 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/entry_points.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      140 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/requires.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/top_level.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-06-13 14:00:33.000000 glview-1.5.4/glview.egg-info/zip-safe
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      175 2023-06-13 13:44:12.000000 glview-1.5.4/requirements.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-06-13 14:00:33.719439 glview-1.5.4/setup.cfg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1200 2023-03-13 15:45:56.000000 glview-1.5.4/setup.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-27 07:16:45.012491 glview-1.5.5/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 glview-1.5.5/LICENSE
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       99 2023-03-13 15:45:56.000000 glview-1.5.5/MANIFEST.in
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      829 2023-07-27 07:16:45.012491 glview-1.5.5/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      380 2023-05-03 12:54:40.000000 glview-1.5.5/README.md
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-27 07:16:45.008491 glview-1.5.5/glview/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      332 2023-07-26 12:23:21.000000 glview-1.5.5/glview/__init__.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15417 2023-03-13 15:45:56.000000 glview-1.5.5/glview/argv.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    11756 2023-05-12 14:23:54.000000 glview-1.5.5/glview/glrenderer.py
+-rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)     9293 2023-06-19 09:07:27.000000 glview-1.5.5/glview/glview.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     8698 2023-06-13 13:58:46.000000 glview-1.5.5/glview/imageprovider.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      297 2023-05-09 09:52:42.000000 glview-1.5.5/glview/panzoom.vs
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    17704 2023-06-22 08:20:42.000000 glview-1.5.5/glview/pygletui.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     4546 2023-06-13 13:48:47.000000 glview-1.5.5/glview/texture.fs
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-07-27 07:14:08.000000 glview-1.5.5/glview/version.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-27 07:16:45.012491 glview-1.5.5/glview.egg-info/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      829 2023-07-27 07:16:44.000000 glview-1.5.5/glview.egg-info/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      431 2023-07-27 07:16:44.000000 glview-1.5.5/glview.egg-info/SOURCES.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-07-27 07:16:44.000000 glview-1.5.5/glview.egg-info/dependency_links.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       39 2023-07-27 07:16:44.000000 glview-1.5.5/glview.egg-info/entry_points.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      126 2023-07-27 07:16:44.000000 glview-1.5.5/glview.egg-info/requires.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-07-27 07:16:44.000000 glview-1.5.5/glview.egg-info/top_level.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-07-27 07:16:44.000000 glview-1.5.5/glview.egg-info/zip-safe
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      161 2023-07-27 07:10:20.000000 glview-1.5.5/requirements.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-07-27 07:16:45.012491 glview-1.5.5/setup.cfg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1200 2023-03-13 15:45:56.000000 glview-1.5.5/setup.py
```

### Comparing `glview-1.5.4/LICENSE` & `glview-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `glview-1.5.4/PKG-INFO` & `glview-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glview
-Version: 1.5.4
+Version: 1.5.5
 Summary: Lightning-fast image viewer with smooth zooming & panning.
 Home-page: http://github.com/toaarnio/glview
 Author: Tomi Aarnio
 Author-email: tomi.p.aarnio@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `glview-1.5.4/glview/argv.py` & `glview-1.5.5/glview/argv.py`

 * *Files identical despite different names*

### Comparing `glview-1.5.4/glview/glrenderer.py` & `glview-1.5.5/glview/glrenderer.py`

 * *Files identical despite different names*

### Comparing `glview-1.5.4/glview/glview.py` & `glview-1.5.5/glview/glview.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,14 @@
         print("    mouse left + move       pan image; synchronized if multiple tiles")
         print("    left / right            pan image; synchronized if multiple tiles")
         print("    PageUp / PageDown       cycle through images on active tile")
         print("    ctrl + left / right     cycle through images on all tiles")
         print("    r                       rotate active tile 90 degrees clockwise")
         print("    s                       split window into 1/2/3/4 tiles")
         print("    1 / 2 / 3 / 4           select active tile for PageUp/PageDown/r")
-        print("    w                       write current tile(s) to a PNG")
         print("    h                       reset zoom/pan/exposure to initial state")
         print("    f                       toggle fullscreen <-> windowed")
         print("    t                       toggle nearest <-> linear filtering")
         print("    g                       toggle sRGB gamma correction on/off")
         print("    n                       toggle exposure normalization on/off")
         print("    e                       slide exposure from -2EV to +2EV & back")
         print("    b                       toggle between HDR/LDR exposure control")
```

### Comparing `glview-1.5.4/glview/imageprovider.py` & `glview-1.5.5/glview/imageprovider.py`

 * *Files identical despite different names*

### Comparing `glview-1.5.4/glview/pygletui.py` & `glview-1.5.5/glview/pygletui.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     def _caption(self):
         fps = pyglet.clock.get_frequency()
         gamut = "off" if not self.gamut_fit else f"p = {self.gamut_pow[0]:.1f}"
         caption = f"glview [{self.ev:+1.2f}EV | gamut fit {gamut} | {fps:.1f} fps]"
         for tileidx in range(self.numtiles):
             imgidx = self.img_per_tile[tileidx]
-            basename = os.path.basename(self.files.filespecs[imgidx])
+            basename = self.files.filespecs[imgidx]
             caption = f"{caption} | {basename} [{imgidx+1}/{self.files.numfiles}]"
         return caption
 
     def _retile(self, numtiles, winsize):
         w, h = winsize
         viewports = {}
         if numtiles == 1:
```

### Comparing `glview-1.5.4/glview/texture.fs` & `glview-1.5.5/glview/texture.fs`

 * *Files identical despite different names*

### Comparing `glview-1.5.4/glview.egg-info/PKG-INFO` & `glview-1.5.5/glview.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glview
-Version: 1.5.4
+Version: 1.5.5
 Summary: Lightning-fast image viewer with smooth zooming & panning.
 Home-page: http://github.com/toaarnio/glview
 Author: Tomi Aarnio
 Author-email: tomi.p.aarnio@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `glview-1.5.4/setup.py` & `glview-1.5.5/setup.py`

 * *Files identical despite different names*

