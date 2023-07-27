# Comparing `tmp/RMK_support-1.0.2.tar.gz` & `tmp/RMK_support-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RMK_support-1.0.2.tar", last modified: Wed Jun 28 14:30:07 2023, max compression
+gzip compressed data, was "RMK_support-1.0.3.tar", last modified: Thu Jul 27 14:02:02 2023, max compression
```

## Comparing `RMK_support-1.0.2.tar` & `RMK_support-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:30:07.501800 RMK_support-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-28 14:29:49.000000 RMK_support-1.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-28 14:30:07.497800 RMK_support-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-28 14:29:49.000000 RMK_support-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:30:07.497800 RMK_support-1.0.2/RMK_support/
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/IO_support.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/amjuel_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/amjuel_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/analysis_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/calculation_tree_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    85448 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/common_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    40282 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/crm_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/dashboard_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/init_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    30956 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/rk_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    71007 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/simple_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/sk_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-28 14:29:49.000000 RMK_support-1.0.2/RMK_support/variable_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:30:07.497800 RMK_support-1.0.2/RMK_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-28 14:30:07.000000 RMK_support-1.0.2/RMK_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-28 14:30:07.000000 RMK_support-1.0.2/RMK_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 14:30:07.000000 RMK_support-1.0.2/RMK_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-28 14:30:07.000000 RMK_support-1.0.2/RMK_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-28 14:30:07.000000 RMK_support-1.0.2/RMK_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 14:30:07.501800 RMK_support-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-28 14:29:50.000000 RMK_support-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:02:02.843718 RMK_support-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-07-27 14:01:49.000000 RMK_support-1.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-27 14:02:02.843718 RMK_support-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-27 14:01:49.000000 RMK_support-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:02:02.839718 RMK_support-1.0.3/RMK_support/
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/IO_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/amjuel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/amjuel_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/analysis_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/calculation_tree_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85465 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/common_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40282 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/crm_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/dashboard_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/init_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30956 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/rk_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71007 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/simple_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/sk_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-27 14:01:49.000000 RMK_support-1.0.3/RMK_support/variable_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:02:02.843718 RMK_support-1.0.3/RMK_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-27 14:02:02.000000 RMK_support-1.0.3/RMK_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-27 14:02:02.000000 RMK_support-1.0.3/RMK_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:02:02.000000 RMK_support-1.0.3/RMK_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 14:02:02.000000 RMK_support-1.0.3/RMK_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 14:02:02.000000 RMK_support-1.0.3/RMK_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:02:02.843718 RMK_support-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-27 14:01:49.000000 RMK_support-1.0.3/setup.py
```

### Comparing `RMK_support-1.0.2/LICENSE.md` & `RMK_support-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/PKG-INFO` & `RMK_support-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RMK_support
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python modules and notebooks used to initialize and analyze ReMKiT1D runs 
 Author: UK Atomic Energy Authority
 Maintainer: Stefan Mijin
 Maintainer-email: stefan.mijin@ukaea.uk
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `RMK_support-1.0.2/README.md` & `RMK_support-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/IO_support.py` & `RMK_support-1.0.3/RMK_support/IO_support.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/amjuel_reader.py` & `RMK_support-1.0.3/RMK_support/amjuel_reader.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/amjuel_support.py` & `RMK_support-1.0.3/RMK_support/amjuel_support.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/analysis_support.py` & `RMK_support-1.0.3/RMK_support/analysis_support.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/calculation_tree_support.py` & `RMK_support-1.0.3/RMK_support/calculation_tree_support.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/common_models.py` & `RMK_support-1.0.3/RMK_support/common_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2507,20 +2507,20 @@
 
     vGrid = wrapper.grid.vGrid
     dv = wrapper.grid.vWidths
     interp = np.zeros(len(dv)).tolist()
 
     vProfile = [1 / (v**2) for v in vGrid]
 
-    drag = vGrid**2 * dv
-    vSum = [
-        0 for i in range(len(drag))
-    ]  # vGrid**2 if exact energy source is required, 0 if exactly no particle source is required (either way the error is negligible)
-    vSum[:-1] = vGrid[1:] ** 2 - vGrid[:-1] ** 2
-    drag = drag / vSum
+    drag = dv * np.ones(len(vGrid))
+    vSum = np.zeros(
+        len(drag)
+    )  # ones if exact energy source is required, 0 if exactly no particle source is required (either way the error is negligible)
+    vSum[:-1] = vGrid[:-1] ** 2 / (vGrid[1:] ** 2 - vGrid[:-1] ** 2)
+    drag = drag * vSum
     normConst = sc.CustomNormConst(multConst=multConst)
 
     newTerm = sc.GeneralMatrixTerm(
         distFunName,
         customNormConst=normConst,
         velocityProfile=vProfile,
         varData=varData,
```

### Comparing `RMK_support-1.0.2/RMK_support/crm_support.py` & `RMK_support-1.0.3/RMK_support/crm_support.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/dashboard_support.py` & `RMK_support-1.0.3/RMK_support/dashboard_support.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/grid.py` & `RMK_support-1.0.3/RMK_support/grid.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/init_templates.py` & `RMK_support-1.0.3/RMK_support/init_templates.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/rk_wrapper.py` & `RMK_support-1.0.3/RMK_support/rk_wrapper.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/simple_containers.py` & `RMK_support-1.0.3/RMK_support/simple_containers.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/sk_normalization.py` & `RMK_support-1.0.3/RMK_support/sk_normalization.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support/variable_container.py` & `RMK_support-1.0.3/RMK_support/variable_container.py`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/RMK_support.egg-info/PKG-INFO` & `RMK_support-1.0.3/RMK_support.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RMK-support
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python modules and notebooks used to initialize and analyze ReMKiT1D runs 
 Author: UK Atomic Energy Authority
 Maintainer: Stefan Mijin
 Maintainer-email: stefan.mijin@ukaea.uk
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `RMK_support-1.0.2/RMK_support.egg-info/SOURCES.txt` & `RMK_support-1.0.3/RMK_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RMK_support-1.0.2/setup.py` & `RMK_support-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages  # type: ignore
 
 setup(
     name="RMK_support",
-    version="1.0.2",
+    version="1.0.3",
     packages=["RMK_support"],
     install_requires=[
         "numpy",
         "xarray",
         "holoviews",
         "panel",
         "matplotlib",
```

