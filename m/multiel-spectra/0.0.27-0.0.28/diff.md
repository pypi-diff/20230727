# Comparing `tmp/multiel_spectra-0.0.27.tar.gz` & `tmp/multiel_spectra-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiel_spectra-0.0.27.tar", last modified: Thu Jul 27 11:37:33 2023, max compression
+gzip compressed data, was "multiel_spectra-0.0.28.tar", last modified: Thu Jul 27 11:41:16 2023, max compression
```

## Comparing `multiel_spectra-0.0.27.tar` & `multiel_spectra-0.0.28.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.815337 multiel_spectra-0.0.27/
--rw-rw-rw-   0        0        0      352 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.774103 multiel_spectra-0.0.27/.github/
-drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.825063 multiel_spectra-0.0.27/.github/workflows/
--rw-rw-rw-   0        0        0      667 2023-06-13 15:56:38.000000 multiel_spectra-0.0.27/.github/workflows/release.yml
--rw-rw-rw-   0        0        0      613 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/.github/workflows/test.yml
--rw-rw-rw-   0        0        0     2173 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/.gitignore
-drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.826145 multiel_spectra-0.0.27/.vscode/
--rw-rw-rw-   0        0        0      187 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/.vscode/settings.json
--rw-rw-rw-   0        0        0     1100 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/LICENSE
--rw-rw-rw-   0        0        0      175 2023-06-19 12:44:52.000000 multiel_spectra-0.0.27/MANIFEST.in
--rw-rw-rw-   0        0        0     8263 2023-07-27 11:37:33.865654 multiel_spectra-0.0.27/PKG-INFO
--rw-rw-rw-   0        0        0     7031 2023-06-20 13:25:46.000000 multiel_spectra-0.0.27/README.md
--rw-rw-rw-   0        0        0      101 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/pyproject.toml
--rw-rw-rw-   0        0        0      126 2023-07-27 11:37:33.869423 multiel_spectra-0.0.27/setup.cfg
--rw-rw-rw-   0        0        0     2632 2023-06-19 16:14:52.000000 multiel_spectra-0.0.27/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.780610 multiel_spectra-0.0.27/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.835640 multiel_spectra-0.0.27/src/multiel_spectra/
--rw-rw-rw-   0        0        0       58 2023-07-27 11:36:49.000000 multiel_spectra-0.0.27/src/multiel_spectra/__init__.py
--rw-rw-rw-   0        0        0      311 2023-06-14 14:06:06.000000 multiel_spectra-0.0.27/src/multiel_spectra/install_skbeam.py
--rw-rw-rw-   0        0        0      231 2023-06-13 15:27:34.000000 multiel_spectra-0.0.27/src/multiel_spectra/install_spekpy.py
--rw-rw-rw-   0        0        0    75386 2023-07-27 11:36:27.000000 multiel_spectra-0.0.27/src/multiel_spectra/multiel_spectra.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.860988 multiel_spectra-0.0.27/src/multiel_spectra.egg-info/
--rw-rw-rw-   0        0        0     8263 2023-07-27 11:37:33.000000 multiel_spectra-0.0.27/src/multiel_spectra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      596 2023-07-27 11:37:33.000000 multiel_spectra-0.0.27/src/multiel_spectra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       58 2023-07-27 11:37:33.000000 multiel_spectra-0.0.27/src/multiel_spectra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-07-27 11:37:33.000000 multiel_spectra-0.0.27/src/multiel_spectra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-27 11:37:33.000000 multiel_spectra-0.0.27/src/multiel_spectra.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.864956 multiel_spectra-0.0.27/tests/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/tests/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-06-19 13:58:38.000000 multiel_spectra-0.0.27/tests/test_module1.py
--rw-rw-rw-   0        0        0      295 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/tox.ini
--rw-rw-rw-   0        0        0       33 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/vscode.env
+drwxrwxrwx   0        0        0        0 2023-07-27 11:41:16.691697 multiel_spectra-0.0.28/
+-rw-rw-rw-   0        0        0      352 2023-06-13 15:09:48.000000 multiel_spectra-0.0.28/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-07-27 11:41:16.658004 multiel_spectra-0.0.28/.github/
+drwxrwxrwx   0        0        0        0 2023-07-27 11:41:16.696062 multiel_spectra-0.0.28/.github/workflows/
+-rw-rw-rw-   0        0        0      667 2023-06-13 15:56:38.000000 multiel_spectra-0.0.28/.github/workflows/release.yml
+-rw-rw-rw-   0        0        0      613 2023-06-13 15:09:48.000000 multiel_spectra-0.0.28/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0     2173 2023-06-13 15:09:48.000000 multiel_spectra-0.0.28/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-27 11:41:16.696062 multiel_spectra-0.0.28/.vscode/
+-rw-rw-rw-   0        0        0      187 2023-06-13 15:09:48.000000 multiel_spectra-0.0.28/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1100 2023-06-13 15:09:48.000000 multiel_spectra-0.0.28/LICENSE
+-rw-rw-rw-   0        0        0      175 2023-06-19 12:44:52.000000 multiel_spectra-0.0.28/MANIFEST.in
+-rw-rw-rw-   0        0        0     8263 2023-07-27 11:41:16.769068 multiel_spectra-0.0.28/PKG-INFO
+-rw-rw-rw-   0        0        0     7031 2023-06-20 13:25:46.000000 multiel_spectra-0.0.28/README.md
+-rw-rw-rw-   0        0        0      101 2023-06-13 15:09:48.000000 multiel_spectra-0.0.28/pyproject.toml
+-rw-rw-rw-   0        0        0      126 2023-07-27 11:41:16.769068 multiel_spectra-0.0.28/setup.cfg
+-rw-rw-rw-   0        0        0     2632 2023-06-19 16:14:52.000000 multiel_spectra-0.0.28/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:41:16.661452 multiel_spectra-0.0.28/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 11:41:16.737857 multiel_spectra-0.0.28/src/multiel_spectra/
+-rw-rw-rw-   0        0        0       58 2023-07-27 11:40:59.000000 multiel_spectra-0.0.28/src/multiel_spectra/__init__.py
+-rw-rw-rw-   0        0        0      311 2023-06-14 14:06:06.000000 multiel_spectra-0.0.28/src/multiel_spectra/install_skbeam.py
+-rw-rw-rw-   0        0        0      231 2023-06-13 15:27:34.000000 multiel_spectra-0.0.28/src/multiel_spectra/install_spekpy.py
+-rw-rw-rw-   0        0        0    75357 2023-07-27 11:40:51.000000 multiel_spectra-0.0.28/src/multiel_spectra/multiel_spectra.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:41:16.760251 multiel_spectra-0.0.28/src/multiel_spectra.egg-info/
+-rw-rw-rw-   0        0        0     8263 2023-07-27 11:41:16.000000 multiel_spectra-0.0.28/src/multiel_spectra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2023-07-27 11:41:16.000000 multiel_spectra-0.0.28/src/multiel_spectra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       58 2023-07-27 11:41:16.000000 multiel_spectra-0.0.28/src/multiel_spectra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-07-27 11:41:16.000000 multiel_spectra-0.0.28/src/multiel_spectra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-27 11:41:16.000000 multiel_spectra-0.0.28/src/multiel_spectra.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 11:41:16.769068 multiel_spectra-0.0.28/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:09:48.000000 multiel_spectra-0.0.28/tests/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-06-19 13:58:38.000000 multiel_spectra-0.0.28/tests/test_module1.py
+-rw-rw-rw-   0        0        0      295 2023-06-13 15:09:48.000000 multiel_spectra-0.0.28/tox.ini
+-rw-rw-rw-   0        0        0       33 2023-06-13 15:09:48.000000 multiel_spectra-0.0.28/vscode.env
```

### Comparing `multiel_spectra-0.0.27/.github/workflows/release.yml` & `multiel_spectra-0.0.28/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.27/.github/workflows/test.yml` & `multiel_spectra-0.0.28/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.27/.gitignore` & `multiel_spectra-0.0.28/.gitignore`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.27/LICENSE` & `multiel_spectra-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.27/PKG-INFO` & `multiel_spectra-0.0.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiel_spectra
-Version: 0.0.27
+Version: 0.0.28
 Summary: Multi-Element Fluorescence Xray Spectra Generator
 Home-page: https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Author: Fernando Garcia-Avello 
 Author-email: fgarciaa@fi.infn.it
 Project-URL: Documentation, https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Project-URL: Bug Reports, https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Project-URL: Source Code, https://github.com/Fernandogarciagoatcoder/multiel_spectra
```

### Comparing `multiel_spectra-0.0.27/README.md` & `multiel_spectra-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.27/setup.py` & `multiel_spectra-0.0.28/setup.py`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.27/src/multiel_spectra/multiel_spectra.py` & `multiel_spectra-0.0.28/src/multiel_spectra/multiel_spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,14 +557,15 @@
                - final_d (array): The generated spectrum with various components combined.
                - params (dict): Dictionary containing parameters related to the generated spectrum.
 
     Note: Some functions like multi_trans_gen, escape_peaks, sum_peaks, decalibration, and detector_eff are assumed
           to be defined elsewhere and used in this function.
     """
     spec, peaks, els = multi_trans_gen( a, Prim,brems)
+    params = None
     if escape == True: 
         spec = escape_peaks(spec,peaks, els)[0]
     if sum == True:
         spec = sum_peaks(spec,peaks, els)[0]
     if decal == True: 
         spec, params = decalibration(spec)
     spec = detector_eff(spec, np.arange(0,30,0.05))
@@ -601,16 +602,14 @@
         # Add vertical lines with associated tooltips
         p.segment(x0='xs', y0='y0', x1='xs', y1='ys', line_color="green", source=source)
         hover = HoverTool(tooltips=[("Text", "@names")], renderers=[p.renderers[-1]])
         p.add_tools(hover)
 
         # Show the plot
         show(p)
-    if decal == False: 
-        params = None
     return final_d, params
 
 # def plot_spectra(spec, c):
 #     return 
 
 #### VERSION NUEVA
```

### Comparing `multiel_spectra-0.0.27/src/multiel_spectra.egg-info/PKG-INFO` & `multiel_spectra-0.0.28/src/multiel_spectra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiel-spectra
-Version: 0.0.27
+Version: 0.0.28
 Summary: Multi-Element Fluorescence Xray Spectra Generator
 Home-page: https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Author: Fernando Garcia-Avello 
 Author-email: fgarciaa@fi.infn.it
 Project-URL: Documentation, https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Project-URL: Bug Reports, https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Project-URL: Source Code, https://github.com/Fernandogarciagoatcoder/multiel_spectra
```

### Comparing `multiel_spectra-0.0.27/src/multiel_spectra.egg-info/SOURCES.txt` & `multiel_spectra-0.0.28/src/multiel_spectra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.27/tests/test_module1.py` & `multiel_spectra-0.0.28/tests/test_module1.py`

 * *Files identical despite different names*

