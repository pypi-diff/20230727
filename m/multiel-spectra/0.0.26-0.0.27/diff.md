# Comparing `tmp/multiel_spectra-0.0.26.tar.gz` & `tmp/multiel_spectra-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiel_spectra-0.0.26.tar", last modified: Thu Jul 27 10:49:44 2023, max compression
+gzip compressed data, was "multiel_spectra-0.0.27.tar", last modified: Thu Jul 27 11:37:33 2023, max compression
```

## Comparing `multiel_spectra-0.0.26.tar` & `multiel_spectra-0.0.27.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 10:49:43.982496 multiel_spectra-0.0.26/
--rw-rw-rw-   0        0        0      352 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-07-27 10:49:43.921180 multiel_spectra-0.0.26/.github/
-drwxrwxrwx   0        0        0        0 2023-07-27 10:49:43.989853 multiel_spectra-0.0.26/.github/workflows/
--rw-rw-rw-   0        0        0      667 2023-06-13 15:56:38.000000 multiel_spectra-0.0.26/.github/workflows/release.yml
--rw-rw-rw-   0        0        0      613 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/.github/workflows/test.yml
--rw-rw-rw-   0        0        0     2173 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/.gitignore
-drwxrwxrwx   0        0        0        0 2023-07-27 10:49:43.993917 multiel_spectra-0.0.26/.vscode/
--rw-rw-rw-   0        0        0      187 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/.vscode/settings.json
--rw-rw-rw-   0        0        0     1100 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/LICENSE
--rw-rw-rw-   0        0        0      175 2023-06-19 12:44:52.000000 multiel_spectra-0.0.26/MANIFEST.in
--rw-rw-rw-   0        0        0     8263 2023-07-27 10:49:44.042986 multiel_spectra-0.0.26/PKG-INFO
--rw-rw-rw-   0        0        0     7031 2023-06-20 13:25:46.000000 multiel_spectra-0.0.26/README.md
--rw-rw-rw-   0        0        0      101 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/pyproject.toml
--rw-rw-rw-   0        0        0      126 2023-07-27 10:49:44.051008 multiel_spectra-0.0.26/setup.cfg
--rw-rw-rw-   0        0        0     2632 2023-06-19 16:14:52.000000 multiel_spectra-0.0.26/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:49:43.928383 multiel_spectra-0.0.26/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 10:49:44.010402 multiel_spectra-0.0.26/src/multiel_spectra/
--rw-rw-rw-   0        0        0       58 2023-07-27 10:49:36.000000 multiel_spectra-0.0.26/src/multiel_spectra/__init__.py
--rw-rw-rw-   0        0        0      311 2023-06-14 14:06:06.000000 multiel_spectra-0.0.26/src/multiel_spectra/install_skbeam.py
--rw-rw-rw-   0        0        0      231 2023-06-13 15:27:34.000000 multiel_spectra-0.0.26/src/multiel_spectra/install_spekpy.py
--rw-rw-rw-   0        0        0    75340 2023-07-27 10:39:13.000000 multiel_spectra-0.0.26/src/multiel_spectra/multiel_spectra.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:49:44.035097 multiel_spectra-0.0.26/src/multiel_spectra.egg-info/
--rw-rw-rw-   0        0        0     8263 2023-07-27 10:49:42.000000 multiel_spectra-0.0.26/src/multiel_spectra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      596 2023-07-27 10:49:43.000000 multiel_spectra-0.0.26/src/multiel_spectra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       58 2023-07-27 10:49:42.000000 multiel_spectra-0.0.26/src/multiel_spectra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-07-27 10:49:42.000000 multiel_spectra-0.0.26/src/multiel_spectra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-27 10:49:42.000000 multiel_spectra-0.0.26/src/multiel_spectra.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-27 10:49:44.042986 multiel_spectra-0.0.26/tests/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/tests/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-06-19 13:58:38.000000 multiel_spectra-0.0.26/tests/test_module1.py
--rw-rw-rw-   0        0        0      295 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/tox.ini
--rw-rw-rw-   0        0        0       33 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/vscode.env
+drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.815337 multiel_spectra-0.0.27/
+-rw-rw-rw-   0        0        0      352 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.774103 multiel_spectra-0.0.27/.github/
+drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.825063 multiel_spectra-0.0.27/.github/workflows/
+-rw-rw-rw-   0        0        0      667 2023-06-13 15:56:38.000000 multiel_spectra-0.0.27/.github/workflows/release.yml
+-rw-rw-rw-   0        0        0      613 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0     2173 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.826145 multiel_spectra-0.0.27/.vscode/
+-rw-rw-rw-   0        0        0      187 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1100 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/LICENSE
+-rw-rw-rw-   0        0        0      175 2023-06-19 12:44:52.000000 multiel_spectra-0.0.27/MANIFEST.in
+-rw-rw-rw-   0        0        0     8263 2023-07-27 11:37:33.865654 multiel_spectra-0.0.27/PKG-INFO
+-rw-rw-rw-   0        0        0     7031 2023-06-20 13:25:46.000000 multiel_spectra-0.0.27/README.md
+-rw-rw-rw-   0        0        0      101 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/pyproject.toml
+-rw-rw-rw-   0        0        0      126 2023-07-27 11:37:33.869423 multiel_spectra-0.0.27/setup.cfg
+-rw-rw-rw-   0        0        0     2632 2023-06-19 16:14:52.000000 multiel_spectra-0.0.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.780610 multiel_spectra-0.0.27/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.835640 multiel_spectra-0.0.27/src/multiel_spectra/
+-rw-rw-rw-   0        0        0       58 2023-07-27 11:36:49.000000 multiel_spectra-0.0.27/src/multiel_spectra/__init__.py
+-rw-rw-rw-   0        0        0      311 2023-06-14 14:06:06.000000 multiel_spectra-0.0.27/src/multiel_spectra/install_skbeam.py
+-rw-rw-rw-   0        0        0      231 2023-06-13 15:27:34.000000 multiel_spectra-0.0.27/src/multiel_spectra/install_spekpy.py
+-rw-rw-rw-   0        0        0    75386 2023-07-27 11:36:27.000000 multiel_spectra-0.0.27/src/multiel_spectra/multiel_spectra.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.860988 multiel_spectra-0.0.27/src/multiel_spectra.egg-info/
+-rw-rw-rw-   0        0        0     8263 2023-07-27 11:37:33.000000 multiel_spectra-0.0.27/src/multiel_spectra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2023-07-27 11:37:33.000000 multiel_spectra-0.0.27/src/multiel_spectra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       58 2023-07-27 11:37:33.000000 multiel_spectra-0.0.27/src/multiel_spectra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-07-27 11:37:33.000000 multiel_spectra-0.0.27/src/multiel_spectra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-27 11:37:33.000000 multiel_spectra-0.0.27/src/multiel_spectra.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 11:37:33.864956 multiel_spectra-0.0.27/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/tests/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-06-19 13:58:38.000000 multiel_spectra-0.0.27/tests/test_module1.py
+-rw-rw-rw-   0        0        0      295 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/tox.ini
+-rw-rw-rw-   0        0        0       33 2023-06-13 15:09:48.000000 multiel_spectra-0.0.27/vscode.env
```

### Comparing `multiel_spectra-0.0.26/.github/workflows/release.yml` & `multiel_spectra-0.0.27/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.26/.github/workflows/test.yml` & `multiel_spectra-0.0.27/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.26/.gitignore` & `multiel_spectra-0.0.27/.gitignore`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.26/LICENSE` & `multiel_spectra-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.26/PKG-INFO` & `multiel_spectra-0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiel_spectra
-Version: 0.0.26
+Version: 0.0.27
 Summary: Multi-Element Fluorescence Xray Spectra Generator
 Home-page: https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Author: Fernando Garcia-Avello 
 Author-email: fgarciaa@fi.infn.it
 Project-URL: Documentation, https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Project-URL: Bug Reports, https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Project-URL: Source Code, https://github.com/Fernandogarciagoatcoder/multiel_spectra
```

### Comparing `multiel_spectra-0.0.26/README.md` & `multiel_spectra-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.26/setup.py` & `multiel_spectra-0.0.27/setup.py`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.26/src/multiel_spectra/multiel_spectra.py` & `multiel_spectra-0.0.27/src/multiel_spectra/multiel_spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -601,15 +601,16 @@
         # Add vertical lines with associated tooltips
         p.segment(x0='xs', y0='y0', x1='xs', y1='ys', line_color="green", source=source)
         hover = HoverTool(tooltips=[("Text", "@names")], renderers=[p.renderers[-1]])
         p.add_tools(hover)
 
         # Show the plot
         show(p)
-
+    if decal == False: 
+        params = None
     return final_d, params
 
 # def plot_spectra(spec, c):
 #     return 
 
 #### VERSION NUEVA
```

### Comparing `multiel_spectra-0.0.26/src/multiel_spectra.egg-info/PKG-INFO` & `multiel_spectra-0.0.27/src/multiel_spectra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiel-spectra
-Version: 0.0.26
+Version: 0.0.27
 Summary: Multi-Element Fluorescence Xray Spectra Generator
 Home-page: https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Author: Fernando Garcia-Avello 
 Author-email: fgarciaa@fi.infn.it
 Project-URL: Documentation, https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Project-URL: Bug Reports, https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Project-URL: Source Code, https://github.com/Fernandogarciagoatcoder/multiel_spectra
```

### Comparing `multiel_spectra-0.0.26/src/multiel_spectra.egg-info/SOURCES.txt` & `multiel_spectra-0.0.27/src/multiel_spectra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.26/tests/test_module1.py` & `multiel_spectra-0.0.27/tests/test_module1.py`

 * *Files identical despite different names*

