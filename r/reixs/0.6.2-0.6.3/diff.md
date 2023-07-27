# Comparing `tmp/reixs-0.6.2.tar.gz` & `tmp/reixs-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reixs-0.6.2.tar", last modified: Thu Jul 13 19:36:47 2023, max compression
+gzip compressed data, was "reixs-0.6.3.tar", last modified: Thu Jul 27 19:15:47 2023, max compression
```

## Comparing `reixs-0.6.2.tar` & `reixs-0.6.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:36:47.430481 reixs-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-13 19:36:34.000000 reixs-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-13 19:36:47.434481 reixs-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-07-13 19:36:34.000000 reixs-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 19:36:34.000000 reixs-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-13 19:36:47.434481 reixs-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:36:47.418481 reixs-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:36:47.430481 reixs-0.6.2/src/reixs/
--rw-r--r--   0 runner    (1001) docker     (123)    58598 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/LoadData.py
--rw-r--r--   0 runner    (1001) docker     (123)    32990 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/ReadData.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/add_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/beamline_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/mca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/rixs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/rsxs_mcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/rsxs_readutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/sca.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/simplemath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/spec_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-07-13 19:36:34.000000 reixs-0.6.2/src/reixs/xeol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:36:47.430481 reixs-0.6.2/src/reixs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-13 19:36:47.000000 reixs-0.6.2/src/reixs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-13 19:36:47.000000 reixs-0.6.2/src/reixs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:36:47.000000 reixs-0.6.2/src/reixs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 19:36:47.000000 reixs-0.6.2/src/reixs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 19:36:47.000000 reixs-0.6.2/src/reixs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:15:47.257766 reixs-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-27 19:15:36.000000 reixs-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-27 19:15:47.257766 reixs-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-07-27 19:15:36.000000 reixs-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-27 19:15:36.000000 reixs-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-27 19:15:47.257766 reixs-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:15:47.253766 reixs-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:15:47.257766 reixs-0.6.3/src/reixs/
+-rw-r--r--   0 runner    (1001) docker     (123)    58598 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/LoadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32990 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/ReadData.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15932 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/add_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/beamline_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/mca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/rixs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/rsxs_mcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/rsxs_readutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/sca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/simplemath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/spec_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-07-27 19:15:36.000000 reixs-0.6.3/src/reixs/xeol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:15:47.257766 reixs-0.6.3/src/reixs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-27 19:15:47.000000 reixs-0.6.3/src/reixs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-27 19:15:47.000000 reixs-0.6.3/src/reixs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:15:47.000000 reixs-0.6.3/src/reixs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 19:15:47.000000 reixs-0.6.3/src/reixs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 19:15:47.000000 reixs-0.6.3/src/reixs.egg-info/top_level.txt
```

### Comparing `reixs-0.6.2/LICENSE` & `reixs-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/PKG-INFO` & `reixs-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.6.2
+Version: 0.6.3
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.6.2/README.md` & `reixs-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/setup.cfg` & `reixs-0.6.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = reixs
-version = 0.6.2
+version = 0.6.3
 author = Patrick Braun
 author_email = patrick.braun@usask.ca
 description = Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pmb399/REIXSAnalysis
 project_urls = 
@@ -24,14 +24,15 @@
 	numpy
 	pandas
 	bokeh>=2.3.3,<3
 	scipy
 	ipywidgets
 	ipyfilechooser
 	h5py
+	shapely
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `reixs-0.6.2/src/reixs/LoadData.py` & `reixs-0.6.3/src/reixs/LoadData.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/ReadData.py` & `reixs-0.6.3/src/reixs/ReadData.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/add_subtract.py` & `reixs-0.6.3/src/reixs/add_subtract.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/beamline_info.py` & `reixs-0.6.3/src/reixs/beamline_info.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/mca.py` & `reixs-0.6.3/src/reixs/mca.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/mesh.py` & `reixs-0.6.3/src/reixs/mesh.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/parser.py` & `reixs-0.6.3/src/reixs/parser.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/rixs_readutil.py` & `reixs-0.6.3/src/reixs/rixs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/rsxs_mcp.py` & `reixs-0.6.3/src/reixs/rsxs_mcp.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/rsxs_readutil.py` & `reixs-0.6.3/src/reixs/rsxs_readutil.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/sca.py` & `reixs-0.6.3/src/reixs/sca.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 from .ReadData import REIXS
 from .edges import EdgeDict
 from .xeol import *
 from .simplemath import apply_offset, grid_data, apply_savgol, bin_data
 import warnings
 import numpy as np
 from .parser import math_stream
+from shapely.geometry import Point, Polygon
 
-
-def loadSCAscans(basedir, file, x_stream, y_stream, *args, norm=True, is_XAS=False, xoffset=None, xcoffset=None, yoffset=None, ycoffset=None, background=None, energyloss=None, grid_x=[None, None, None], savgol=None, binsize=None, legend_items={}):
+def loadSCAscans(basedir, file, x_stream, y_stream, *args, norm=True, is_XAS=False, xoffset=None, xcoffset=None, yoffset=None, ycoffset=None, background=None, energyloss=None, grid_x=[None, None, None], savgol=None, binsize=None, legend_items={}, polygon=None):
     """Internal function to load MCA data
     
         Parameters
         ----------
         See Load1d function.
     """
 
     # Define special streams that are calculated internally
     special_streams = ['TEY', 'TFY', 'PFY', 'iPFY', 'XES', 'rXES', 'specPFY',
-                       'XRF', 'rXRF', 'XEOL', 'rXEOL', 'POY', 'TOY', 'EY', 'Sample', 'Mesh', 'ET', 'rLOSS']  # all special inputs
+                       'XRF', 'rXRF', 'XEOL', 'rXEOL', 'POY', 'TOY', 'EY', 'Sample', 'Mesh', 'ET', 'rLOSS', 'pXES']  # all special inputs
     XAS_streams = ['TEY', 'TFY', 'PFY', 'iPFY', 'specPFY', 'POY',
-                   'TOY', 'rXES', 'rXRF', 'rXEOL', 'ET', 'rLOSS']  # All that are normalized to mesh
+                   'TOY', 'rXES', 'rXRF', 'rXEOL', 'ET', 'rLOSS','pXES']  # All that are normalized to mesh
 
     # Note that the data dict only gets populated locally until the appropriate
     # singular y stream is return -- Assignment of y_stream happens after evaluation
     # of mathemtatical expression
 
     def get_y_data(y_stream, data, arg, background, REIXSObj):
         # Get the y-data stream
@@ -141,14 +141,39 @@
 
                 y_data = np.sum(matrix[idx_min:idx_max,:],axis=0)
 
                 # Store the corresponding new energy loss scale (gridded for even image spacing in eems 2d)
                 data[arg].energy_loss_gridded = energy_transfer
 
                 return y_data
+            
+            elif doesMatchPattern(y_stream, ['pXES']):
+                # This is to integrate over an constant incident energy region -- probes constant intermediate states
+                poly = Polygon(polygon)
+
+                # Utilize 2d EEMs to convert excitation emission map
+                from .mca import loadMCAscans
+                
+                mca = loadMCAscans(basedir, file, 'Mono Energy', 'MCP Energy', 'MCP', arg, norm=norm, xoffset=xoffset, xcoffset=xcoffset, yoffset=yoffset, ycoffset=ycoffset, background=background, grid_x=grid_x)
+                x_data = mca[arg].x_data
+                y_data = mca[arg].y_data
+                detector = mca[arg].detector
+               
+                pXES = list()
+                for x_idx,x in enumerate(x_data):
+                    y_sum = 0
+                    for y_idx,y in enumerate(y_data):
+                        p = Point(x,y)
+                        if poly.contains(p):
+                            y_sum += detector[y_idx,x_idx]
+                    pXES.append(y_sum)
+
+                y_data = np.array(pXES)
+
+                return y_data
 
             # Legacy for RSXS use
             elif y_stream == 'EY':
                 return data[arg].sample_current
 
             # elif y_stream == 'tey':
             #    # spec mnemonic for sample current
```

### Comparing `reixs-0.6.2/src/reixs/simplemath.py` & `reixs-0.6.3/src/reixs/simplemath.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/spec_config.py` & `reixs-0.6.3/src/reixs/spec_config.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/util.py` & `reixs-0.6.3/src/reixs/util.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs/xeol.py` & `reixs-0.6.3/src/reixs/xeol.py`

 * *Files identical despite different names*

### Comparing `reixs-0.6.2/src/reixs.egg-info/PKG-INFO` & `reixs-0.6.3/src/reixs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reixs
-Version: 0.6.2
+Version: 0.6.3
 Summary: Library to analyse, plot, and export data taken at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/pmb399/REIXSAnalysis
 Author: Patrick Braun
 Author-email: patrick.braun@usask.ca
 Project-URL: Bug Tracker, https://github.com/pmb399/REIXSAnalysis
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
```

### Comparing `reixs-0.6.2/src/reixs.egg-info/SOURCES.txt` & `reixs-0.6.3/src/reixs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

