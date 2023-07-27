# Comparing `tmp/picaso-3.1.1.tar.gz` & `tmp/picaso-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picaso-3.1.1.tar", last modified: Sun Jul 16 21:41:48 2023, max compression
+gzip compressed data, was "picaso-3.1.2.tar", last modified: Thu Jul 27 06:06:42 2023, max compression
```

## Comparing `picaso-3.1.1.tar` & `picaso-3.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-07-16 21:41:48.145520 picaso-3.1.1/
--rw-r--r--   0 nbatalh1   (503) staff       (20)    35141 2019-11-21 19:50:22.000000 picaso-3.1.1/LICENSE
--rw-r--r--   0 nbatalh1   (503) staff       (20)      736 2023-07-16 21:41:48.145635 picaso-3.1.1/PKG-INFO
--rw-r--r--   0 nbatalh1   (503) staff       (20)     9222 2023-03-24 18:45:38.000000 picaso-3.1.1/README.md
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-07-16 21:41:48.142881 picaso-3.1.1/picaso/
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)      188 2020-08-18 18:11:20.000000 picaso-3.1.1/picaso/__init__.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    41567 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/analyze.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    28434 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/atmsetup.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    16419 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/build_3d_input.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    10326 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/cia_interpolate.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)    50616 2023-03-24 18:45:38.000000 picaso-3.1.1/picaso/climate.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    21239 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/deq_chem.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     5996 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/disco.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)   123112 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/elements.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)   169414 2023-03-24 18:45:38.000000 picaso-3.1.1/picaso/fluxes.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     1751 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/io_utils.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)   288719 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/justdoit.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    80150 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/justplotit.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    65867 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/opacity_factory.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)   118894 2023-07-16 21:34:43.000000 picaso-3.1.1/picaso/optics.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    28193 2022-08-19 21:57:10.000000 picaso-3.1.1/picaso/phasecurves.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    14066 2020-02-07 23:44:16.000000 picaso-3.1.1/picaso/rayleigh.py
--rw-r--r--   0 nbatalh1   (503) staff       (20)     4174 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/references.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2993 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/run_opa_factory.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)    10516 2023-03-24 18:45:38.000000 picaso-3.1.1/picaso/test.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2481 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/test_optics.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     4880 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/vulcan.py
--rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2523 2022-10-25 17:12:52.000000 picaso-3.1.1/picaso/wavelength.py
-drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-07-16 21:41:48.145268 picaso-3.1.1/picaso.egg-info/
--rw-r--r--   0 nbatalh1   (503) staff       (20)      736 2023-07-16 21:41:47.000000 picaso-3.1.1/picaso.egg-info/PKG-INFO
--rw-r--r--   0 nbatalh1   (503) staff       (20)      675 2023-07-16 21:41:47.000000 picaso-3.1.1/picaso.egg-info/SOURCES.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2023-07-16 21:41:47.000000 picaso-3.1.1/picaso.egg-info/dependency_links.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2019-11-21 21:13:50.000000 picaso-3.1.1/picaso.egg-info/not-zip-safe
--rw-r--r--   0 nbatalh1   (503) staff       (20)      158 2023-07-16 21:41:47.000000 picaso-3.1.1/picaso.egg-info/requires.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)        7 2023-07-16 21:41:47.000000 picaso-3.1.1/picaso.egg-info/top_level.txt
--rw-r--r--   0 nbatalh1   (503) staff       (20)      767 2023-07-16 21:41:48.146178 picaso-3.1.1/setup.cfg
--rw-r--r--   0 nbatalh1   (503) staff       (20)     3216 2023-07-16 21:34:56.000000 picaso-3.1.1/setup.py
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-07-27 06:06:42.631588 picaso-3.1.2/
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    35141 2019-11-21 19:50:22.000000 picaso-3.1.2/LICENSE
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      717 2023-07-27 06:06:42.631832 picaso-3.1.2/PKG-INFO
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     9222 2023-03-24 18:45:38.000000 picaso-3.1.2/README.md
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-07-27 06:06:42.625367 picaso-3.1.2/picaso/
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)      188 2020-08-18 18:11:20.000000 picaso-3.1.2/picaso/__init__.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    41398 2023-07-27 06:00:56.000000 picaso-3.1.2/picaso/analyze.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    28553 2023-07-27 06:05:57.000000 picaso-3.1.2/picaso/atmsetup.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    16419 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/build_3d_input.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    10326 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/cia_interpolate.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)    50616 2023-03-24 18:45:38.000000 picaso-3.1.2/picaso/climate.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    21239 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/deq_chem.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     5996 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/disco.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)   123112 2023-07-26 21:49:17.000000 picaso-3.1.2/picaso/elements.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)   169414 2023-03-24 18:45:38.000000 picaso-3.1.2/picaso/fluxes.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     1751 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/io_utils.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)   288719 2023-07-26 21:49:17.000000 picaso-3.1.2/picaso/justdoit.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    80150 2023-07-26 21:49:17.000000 picaso-3.1.2/picaso/justplotit.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    65867 2023-07-17 22:26:27.000000 picaso-3.1.2/picaso/opacity_factory.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)   118894 2023-07-26 21:49:17.000000 picaso-3.1.2/picaso/optics.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    28193 2022-08-19 21:57:10.000000 picaso-3.1.2/picaso/phasecurves.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    14066 2020-02-07 23:44:16.000000 picaso-3.1.2/picaso/rayleigh.py
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     4174 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/references.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2993 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/run_opa_factory.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)    10516 2023-03-24 18:45:38.000000 picaso-3.1.2/picaso/test.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2481 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/test_optics.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     4880 2022-10-25 17:12:52.000000 picaso-3.1.2/picaso/vulcan.py
+-rwxr-xr-x   0 nbatalh1   (503) staff       (20)     2577 2023-07-26 21:49:25.000000 picaso-3.1.2/picaso/wavelength.py
+drwxr-xr-x   0 nbatalh1   (503) staff       (20)        0 2023-07-27 06:06:42.631126 picaso-3.1.2/picaso.egg-info/
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      717 2023-07-27 06:06:42.000000 picaso-3.1.2/picaso.egg-info/PKG-INFO
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      675 2023-07-27 06:06:42.000000 picaso-3.1.2/picaso.egg-info/SOURCES.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2023-07-27 06:06:42.000000 picaso-3.1.2/picaso.egg-info/dependency_links.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)        1 2019-11-21 21:13:50.000000 picaso-3.1.2/picaso.egg-info/not-zip-safe
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      158 2023-07-27 06:06:42.000000 picaso-3.1.2/picaso.egg-info/requires.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)        7 2023-07-27 06:06:42.000000 picaso-3.1.2/picaso.egg-info/top_level.txt
+-rw-r--r--   0 nbatalh1   (503) staff       (20)      767 2023-07-27 06:06:42.633452 picaso-3.1.2/setup.cfg
+-rw-r--r--   0 nbatalh1   (503) staff       (20)     3216 2023-07-27 06:04:34.000000 picaso-3.1.2/setup.py
```

### Comparing `picaso-3.1.1/LICENSE` & `picaso-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/PKG-INFO` & `picaso-3.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: picaso
-Version: 3.1.1
+Version: 3.1.2
 Summary: planetary intesity code for atmospheric scattering observations
 Home-page: https://natashabatalha.github.io/picaso
+Download-URL: https://github.com/natashabatalha/picaso
 Author: Natasha E. Batalha
 Author-email: natasha.e.batalha@gmail.com
 License: GPL-3.0
-Download-URL: https://github.com/natashabatalha/picaso
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
 README.md
-
```

### Comparing `picaso-3.1.1/README.md` & `picaso-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/analyze.py` & `picaso-3.1.2/picaso/analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,15 +362,14 @@
         plt.rcParams['lines.markersize'] = 3
         plt.rcParams['lines.markeredgewidth'] = 0
         
         cmap = plt.cm.magma
         #cmap.set_bad('k',1.)
         
         plt.rcParams['image.cmap'] = 'magma'                   # Colormap.
-        plt.rcParams['image.interpolation'] = None
         plt.rcParams['image.origin'] = 'lower'
         plt.rcParams['font.family'] = 'sans-serif'
         plt.rcParams['font.serif'] = 'DejaVu Sans'
         plt.rcParams['mathtext.fontset'] = 'stixsans'
         #plt.rcParams['axes.prop_cycle'] = \
         #plt.cycler(color=["tomato", "dodgerblue", "gold", 'forestgreen', 'mediumorchid', 'lightblue'])
         plt.rcParams['figure.dpi'] = 300
@@ -511,15 +510,14 @@
                 plt.rcParams['lines.markersize'] = 3
                 plt.rcParams['lines.markeredgewidth'] = 0
 
                 cmap = plt.cm.magma
                 #cmap.set_bad('k',1.)
 
                 plt.rcParams['image.cmap'] = 'magma'                   # Colormap.
-                plt.rcParams['image.interpolation'] = None
                 plt.rcParams['image.origin'] = 'lower'
                 plt.rcParams['font.family'] = 'sans-serif'
                 plt.rcParams['font.serif'] = 'DejaVu Sans'
                 plt.rcParams['mathtext.fontset'] = 'stixsans'
                 #plt.rcParams['axes.prop_cycle'] = \
                 #color = plt.cycler()
                 colors=["xkcd:salmon", "dodgerblue", "sandybrown", 'cadetblue', 'orchid', 'lightblue']
@@ -851,15 +849,14 @@
                 plt.rcParams['lines.markersize'] = 3
                 plt.rcParams['lines.markeredgewidth'] = 0
 
                 cmap = plt.cm.get_cmap('tab20b', len(gas_names))
                 #cmap.set_bad('k',1.)
 
                 plt.rcParams['image.cmap'] = 'magma'                   # Colormap.
-                plt.rcParams['image.interpolation'] = None
                 plt.rcParams['image.origin'] = 'lower'
                 plt.rcParams['font.family'] = 'serif'
                 plt.rcParams['font.serif'] = 'DejaVu Sans'
                 plt.rcParams['mathtext.fontset'] = 'stixsans'
                 plt.rcParams['axes.prop_cycle'] = \
                 plt.cycler(color=["xkcd:salmon", "dodgerblue", "sandybrown", 'cadetblue', 'orchid', 'lightblue'])
                 plt.rcParams['figure.dpi'] = 300
```

### Comparing `picaso-3.1.1/picaso/atmsetup.py` & `picaso-3.1.2/picaso/atmsetup.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,22 +489,25 @@
 
             #read in the file that was supplied         
             cld_input = self.input['clouds']['profile'] 
             
             #then reshape and regrid inputs to be a nice matrix that is nlayer by nwave
             #total extinction optical depth 
             opd = np.reshape(cld_input['opd'].values, (self.c.nlayer,self.c.input_npts_wave))
+            opd = opd.astype(np.float64)
             if regrid: opd = regrid_cld(opd, self.input_wno, wno)
             self.layer['cloud'] = {'opd': opd}
             #cloud assymetry parameter
             g0 = np.reshape(cld_input['g0'].values, (self.c.nlayer,self.c.input_npts_wave))
+            g0 = g0.astype(np.float64)
             if regrid: g0 = regrid_cld(g0, self.input_wno, wno)
             self.layer['cloud']['g0'] = g0
             #cloud single scattering albedo 
             w0 = np.reshape(cld_input['w0'].values, (self.c.nlayer,self.c.input_npts_wave))
+            w0 = w0.astype(np.float64)
             if regrid: w0 = regrid_cld(w0, self.input_wno, wno)
             self.layer['cloud']['w0'] = w0  
 
         #if no filepath was given and nothing was given for g0/w0, then assume the run is cloud free and give zeros for all thi stuff         
         elif (isinstance(self.input['clouds']['profile'] , type(None)) and (self.dimension=='1d')):
 
             zeros = np.zeros((self.c.nlayer,self.c.output_npts_wave))
```

### Comparing `picaso-3.1.1/picaso/build_3d_input.py` & `picaso-3.1.2/picaso/build_3d_input.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/cia_interpolate.py` & `picaso-3.1.2/picaso/cia_interpolate.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/climate.py` & `picaso-3.1.2/picaso/climate.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/deq_chem.py` & `picaso-3.1.2/picaso/deq_chem.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/disco.py` & `picaso-3.1.2/picaso/disco.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/elements.py` & `picaso-3.1.2/picaso/elements.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/fluxes.py` & `picaso-3.1.2/picaso/fluxes.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/io_utils.py` & `picaso-3.1.2/picaso/io_utils.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/justdoit.py` & `picaso-3.1.2/picaso/justdoit.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/justplotit.py` & `picaso-3.1.2/picaso/justplotit.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/opacity_factory.py` & `picaso-3.1.2/picaso/opacity_factory.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/optics.py` & `picaso-3.1.2/picaso/optics.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/phasecurves.py` & `picaso-3.1.2/picaso/phasecurves.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/rayleigh.py` & `picaso-3.1.2/picaso/rayleigh.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/references.py` & `picaso-3.1.2/picaso/references.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/run_opa_factory.py` & `picaso-3.1.2/picaso/run_opa_factory.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/test.py` & `picaso-3.1.2/picaso/test.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/test_optics.py` & `picaso-3.1.2/picaso/test_optics.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/vulcan.py` & `picaso-3.1.2/picaso/vulcan.py`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/picaso/wavelength.py` & `picaso-3.1.2/picaso/wavelength.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,11 +61,11 @@
 	Returns
 	-------
 	matrix 
 		matrix that has been reinterpolated to new wave number grid 
 	"""
 	new = np.zeros((matrix.shape[0],len(new_wno)))
 	for i in range(matrix.shape[0]): 
-		new[i, :] = np.interp(new_wno, old_wno, matrix[i,:])
+		new[i, :] = np.interp(new_wno.astype('float64'), old_wno.astype('float64'), matrix[i,:].astype('float64'))
 		#f = sci.interp1d(old_wno, matrix[i,:],kind='cubic')
 		#new[i, :] = f(new_wno)
 	return new
```

### Comparing `picaso-3.1.1/picaso.egg-info/PKG-INFO` & `picaso-3.1.2/picaso.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: picaso
-Version: 3.1.1
+Version: 3.1.2
 Summary: planetary intesity code for atmospheric scattering observations
 Home-page: https://natashabatalha.github.io/picaso
+Download-URL: https://github.com/natashabatalha/picaso
 Author: Natasha E. Batalha
 Author-email: natasha.e.batalha@gmail.com
 License: GPL-3.0
-Download-URL: https://github.com/natashabatalha/picaso
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
 README.md
-
```

### Comparing `picaso-3.1.1/picaso.egg-info/SOURCES.txt` & `picaso-3.1.2/picaso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/setup.cfg` & `picaso-3.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `picaso-3.1.1/setup.py` & `picaso-3.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 # from the setup.cfg file.
 #
 # use_2to3 and zip_safe are common options support by setuptools; these can
 # also be placed in the setup.cfg, as will be demonstrated in a future update
 # to this sample package.
 setup(
     name='picaso', 
-    version = '3.1.1',
+    version = '3.1.2',
     description = 'planetary intesity code for atmospheric scattering observations',
     long_description = 'README.md',
     author = 'Natasha E. Batalha',
     author_email = 'natasha.e.batalha@gmail.com',
     url = 'https://natashabatalha.github.io/picaso',
     license = 'GPL-3.0',
     download_url = 'https://github.com/natashabatalha/picaso',
```

