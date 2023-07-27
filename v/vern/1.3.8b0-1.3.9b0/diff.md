# Comparing `tmp/vern-1.3.8b0.tar.gz` & `tmp/vern-1.3.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vern-1.3.8b0.tar", last modified: Tue Feb  7 07:10:02 2023, max compression
+gzip compressed data, was "vern-1.3.9b0.tar", last modified: Tue Feb  7 07:36:06 2023, max compression
```

## Comparing `vern-1.3.8b0.tar` & `vern-1.3.9b0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:10:02.332798 vern-1.3.8b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-07 07:09:51.000000 vern-1.3.8b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-07 07:09:51.000000 vern-1.3.8b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-02-07 07:10:02.332798 vern-1.3.8b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-02-07 07:09:51.000000 vern-1.3.8b0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-07 07:09:51.000000 vern-1.3.8b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 07:10:02.332798 vern-1.3.8b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-02-07 07:09:51.000000 vern-1.3.8b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:10:02.332798 vern-1.3.8b0/vern/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-02-07 07:09:51.000000 vern-1.3.8b0/vern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-02-07 07:09:51.000000 vern-1.3.8b0/vern/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-02-07 07:09:51.000000 vern-1.3.8b0/vern/parse_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-02-07 07:09:51.000000 vern-1.3.8b0/vern/parse_autocad.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-07 07:09:51.000000 vern-1.3.8b0/vern/parse_mat.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-07 07:09:51.000000 vern-1.3.8b0/vern/parse_oscilloscope_electrical.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-07 07:09:51.000000 vern-1.3.8b0/vern/parse_oscilloscope_optical_left.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-02-07 07:09:51.000000 vern-1.3.8b0/vern/parse_oscilloscope_optical_left_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-07 07:09:51.000000 vern-1.3.8b0/vern/parse_oscilloscope_optical_right.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-02-07 07:09:51.000000 vern-1.3.8b0/vern/parse_profilometer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-07 07:09:51.000000 vern-1.3.8b0/vern/parse_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-07 07:09:51.000000 vern-1.3.8b0/vern/parse_vsm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:10:02.332798 vern-1.3.8b0/vern.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-02-07 07:10:02.000000 vern-1.3.8b0/vern.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-02-07 07:10:02.000000 vern-1.3.8b0/vern.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 07:10:02.000000 vern-1.3.8b0/vern.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-07 07:10:02.000000 vern-1.3.8b0/vern.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-07 07:10:02.000000 vern-1.3.8b0/vern.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-07 07:10:02.000000 vern-1.3.8b0/vern.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:36:06.489922 vern-1.3.9b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-07 07:35:50.000000 vern-1.3.9b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-07 07:35:50.000000 vern-1.3.9b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-02-07 07:36:06.489922 vern-1.3.9b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-02-07 07:35:50.000000 vern-1.3.9b0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-07 07:35:50.000000 vern-1.3.9b0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 07:36:06.489922 vern-1.3.9b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-02-07 07:35:50.000000 vern-1.3.9b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:36:06.485922 vern-1.3.9b0/vern/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-02-07 07:35:50.000000 vern-1.3.9b0/vern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-02-07 07:35:50.000000 vern-1.3.9b0/vern/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-02-07 07:35:50.000000 vern-1.3.9b0/vern/parse_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-02-07 07:35:50.000000 vern-1.3.9b0/vern/parse_autocad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-07 07:35:50.000000 vern-1.3.9b0/vern/parse_mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-07 07:35:50.000000 vern-1.3.9b0/vern/parse_oscilloscope_electrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-07 07:35:50.000000 vern-1.3.9b0/vern/parse_oscilloscope_optical_left.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-02-07 07:35:50.000000 vern-1.3.9b0/vern/parse_oscilloscope_optical_left_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-07 07:35:50.000000 vern-1.3.9b0/vern/parse_oscilloscope_optical_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-02-07 07:35:50.000000 vern-1.3.9b0/vern/parse_profilometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-07 07:35:50.000000 vern-1.3.9b0/vern/parse_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-07 07:35:50.000000 vern-1.3.9b0/vern/parse_vsm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 07:36:06.489922 vern-1.3.9b0/vern.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-02-07 07:36:06.000000 vern-1.3.9b0/vern.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-02-07 07:36:06.000000 vern-1.3.9b0/vern.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 07:36:06.000000 vern-1.3.9b0/vern.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-07 07:36:06.000000 vern-1.3.9b0/vern.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-07 07:36:06.000000 vern-1.3.9b0/vern.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-07 07:36:06.000000 vern-1.3.9b0/vern.egg-info/top_level.txt
```

### Comparing `vern-1.3.8b0/LICENSE` & `vern-1.3.9b0/LICENSE`

 * *Files identical despite different names*

### Comparing `vern-1.3.8b0/PKG-INFO` & `vern-1.3.9b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vern
-Version: 1.3.8b0
+Version: 1.3.9b0
 Summary: templated auto processing/visualization of measured data
 Home-page: http://github.com/BoronSpoon/vern
 Author: boronspoon
 Author-email: rayanticlimactic@gmail.com
 License: MIT License
 Keywords: matplotlib,research,plot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vern-1.3.8b0/README.rst` & `vern-1.3.9b0/README.rst`

 * *Files identical despite different names*

### Comparing `vern-1.3.8b0/setup.py` & `vern-1.3.9b0/setup.py`

 * *Files identical despite different names*

### Comparing `vern-1.3.8b0/vern/misc.py` & `vern-1.3.9b0/vern/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,17 +86,17 @@
                 self.df.plot(kind="line", x=keys[0], y="fit_y", legend=None, ax=self.ax, style="-")
                 self.ax.text(xmin, ymax, f"{params[0]:.3f}x+{params[1]:.3f}, r2={r2:.3f}", horizontalalignment="left", verticalalignment="top")
             else:
                 self.df.plot(kind="line", x=keys[0], y=keys[1], legend=None, ax=self.ax)
             self.ax.set(ylabel=keys[1])
         else:
             if self.linear_regression:
-                self.df.scatter(x=keys[0], ax=self.ax, fit_reg=True, subplots=self.subplots, layout=(self.subplot_x,self.subplot_y), sharex=True, sharey=True)
+                self.df.scatter(x=keys[0], ax=self.ax, fit_reg=True, subplots=self.subplots, layout=(self.subplot_x,self.subplot_y), sharex=True, sharey=True, xlabel=keys[0].split("\t")[0], ylabel=keys[0].split("\t")[1])
             else:
-                self.df.plot(kind="line", x=keys[0], ax=self.ax, subplots=self.subplots, layout=(self.subplot_x,self.subplot_y), sharex=True, sharey=True)
+                self.df.plot(kind="line", x=keys[0], ax=self.ax, subplots=self.subplots, layout=(self.subplot_x,self.subplot_y), sharex=True, sharey=True, xlabel=keys[0].split("\t")[0], ylabel=keys[0].split("\t")[1])
             self.ax.set(xlabel=keys[0].split("\t")[0])
             self.ax.set(ylabel=keys[0].split("\t")[1])
         plt.savefig(plot_path, bbox_inches="tight")
  
     def on_xlims_change(self, event_ax):
         self.xlim = event_ax.get_xlim()
     def on_ylims_change(self, event_ax):
```

### Comparing `vern-1.3.8b0/vern/parse_all.py` & `vern-1.3.9b0/vern/parse_all.py`

 * *Files identical despite different names*

### Comparing `vern-1.3.8b0/vern/parse_autocad.py` & `vern-1.3.9b0/vern/parse_autocad.py`

 * *Files identical despite different names*

### Comparing `vern-1.3.8b0/vern/parse_oscilloscope_electrical.py` & `vern-1.3.9b0/vern/parse_oscilloscope_electrical.py`

 * *Files identical despite different names*

### Comparing `vern-1.3.8b0/vern/parse_oscilloscope_optical_left.py` & `vern-1.3.9b0/vern/parse_oscilloscope_optical_left.py`

 * *Files identical despite different names*

### Comparing `vern-1.3.8b0/vern/parse_oscilloscope_optical_left_xy.py` & `vern-1.3.9b0/vern/parse_oscilloscope_optical_left_xy.py`

 * *Files identical despite different names*

### Comparing `vern-1.3.8b0/vern/parse_oscilloscope_optical_right.py` & `vern-1.3.9b0/vern/parse_oscilloscope_optical_right.py`

 * *Files identical despite different names*

### Comparing `vern-1.3.8b0/vern/parse_profilometer.py` & `vern-1.3.9b0/vern/parse_profilometer.py`

 * *Files identical despite different names*

### Comparing `vern-1.3.8b0/vern/parse_tabular.py` & `vern-1.3.9b0/vern/parse_tabular.py`

 * *Files identical despite different names*

### Comparing `vern-1.3.8b0/vern/parse_vsm.py` & `vern-1.3.9b0/vern/parse_vsm.py`

 * *Files identical despite different names*

### Comparing `vern-1.3.8b0/vern.egg-info/PKG-INFO` & `vern-1.3.9b0/vern.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vern
-Version: 1.3.8b0
+Version: 1.3.9b0
 Summary: templated auto processing/visualization of measured data
 Home-page: http://github.com/BoronSpoon/vern
 Author: boronspoon
 Author-email: rayanticlimactic@gmail.com
 License: MIT License
 Keywords: matplotlib,research,plot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vern-1.3.8b0/vern.egg-info/SOURCES.txt` & `vern-1.3.9b0/vern.egg-info/SOURCES.txt`

 * *Files identical despite different names*

