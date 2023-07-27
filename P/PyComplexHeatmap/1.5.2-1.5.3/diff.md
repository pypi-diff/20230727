# Comparing `tmp/PyComplexHeatmap-1.5.2.tar.gz` & `tmp/PyComplexHeatmap-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.5.2.tar", last modified: Tue Jul 11 17:11:53 2023, max compression
+gzip compressed data, was "PyComplexHeatmap-1.5.3.tar", last modified: Thu Jul 27 19:11:42 2023, max compression
```

## Comparing `PyComplexHeatmap-1.5.2.tar` & `PyComplexHeatmap-1.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-07-11 17:11:53.108732 PyComplexHeatmap-1.5.2/
--rw-r--r--   0 wding      (503) staff       (20)     1067 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.2/LICENSE
--rw-r--r--   0 wding      (503) staff       (20)      105 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.2/MANIFEST.in
--rw-r--r--   0 wding      (503) staff       (20)    11925 2023-07-11 17:11:53.108010 PyComplexHeatmap-1.5.2/PKG-INFO
-drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-07-11 17:11:53.104495 PyComplexHeatmap-1.5.2/PyComplexHeatmap/
--rw-r--r--   0 wding      (503) staff       (20)      387 2023-07-11 17:10:14.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/__init__.py
--rw-r--r--   0 wding      (503) staff       (20)    66678 2023-07-11 17:05:35.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/annotations.py
--rw-r--r--   0 wding      (503) staff       (20)    75906 2023-07-10 17:29:22.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 wding      (503) staff       (20)     5430 2023-05-15 19:27:29.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/colors.py
--rw-r--r--   0 wding      (503) staff       (20)    21257 2023-06-09 16:20:57.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 wding      (503) staff       (20)     6766 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/example.py
--rw-r--r--   0 wding      (503) staff       (20)    17872 2023-06-09 16:23:11.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 wding      (503) staff       (20)     6788 2023-06-09 16:21:38.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/tools.py
--rw-r--r--   0 wding      (503) staff       (20)    28838 2023-07-11 17:10:03.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-07-11 17:11:53.107260 PyComplexHeatmap-1.5.2/PyComplexHeatmap.egg-info/
--rw-r--r--   0 wding      (503) staff       (20)    11925 2023-07-11 17:11:52.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 wding      (503) staff       (20)      473 2023-07-11 17:11:52.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 wding      (503) staff       (20)        1 2023-07-11 17:11:52.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 wding      (503) staff       (20)       17 2023-07-11 17:11:52.000000 PyComplexHeatmap-1.5.2/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 wding      (503) staff       (20)    11316 2023-06-19 21:12:13.000000 PyComplexHeatmap-1.5.2/README.md
--rw-r--r--   0 wding      (503) staff       (20)      686 2023-07-11 17:08:37.000000 PyComplexHeatmap-1.5.2/pyproject.toml
--rw-r--r--   0 wding      (503) staff       (20)       38 2023-07-11 17:11:53.108937 PyComplexHeatmap-1.5.2/setup.cfg
--rw-r--r--   0 wding      (503) staff       (20)     1044 2023-07-11 17:09:17.000000 PyComplexHeatmap-1.5.2/setup.py
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-07-27 19:11:42.175579 PyComplexHeatmap-1.5.3/
+-rw-r--r--   0 wding      (503) staff       (20)     1067 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.3/LICENSE
+-rw-r--r--   0 wding      (503) staff       (20)      105 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.3/MANIFEST.in
+-rw-r--r--   0 wding      (503) staff       (20)    13319 2023-07-27 19:11:42.174853 PyComplexHeatmap-1.5.3/PKG-INFO
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-07-27 19:11:42.170840 PyComplexHeatmap-1.5.3/PyComplexHeatmap/
+-rw-r--r--   0 wding      (503) staff       (20)      387 2023-07-27 18:48:17.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 wding      (503) staff       (20)    66601 2023-07-27 18:27:59.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 wding      (503) staff       (20)    76487 2023-07-27 18:26:56.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 wding      (503) staff       (20)     5430 2023-05-15 19:27:29.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap/colors.py
+-rw-r--r--   0 wding      (503) staff       (20)    21260 2023-07-27 18:29:22.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 wding      (503) staff       (20)     6766 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap/example.py
+-rw-r--r--   0 wding      (503) staff       (20)    17875 2023-07-27 18:29:51.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 wding      (503) staff       (20)     6815 2023-07-27 18:30:56.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap/tools.py
+-rw-r--r--   0 wding      (503) staff       (20)    29002 2023-07-27 18:28:27.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-07-27 19:11:42.173927 PyComplexHeatmap-1.5.3/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 wding      (503) staff       (20)    13319 2023-07-27 19:11:41.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 wding      (503) staff       (20)      473 2023-07-27 19:11:42.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 wding      (503) staff       (20)        1 2023-07-27 19:11:41.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 wding      (503) staff       (20)       17 2023-07-27 19:11:41.000000 PyComplexHeatmap-1.5.3/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 wding      (503) staff       (20)    11294 2023-07-27 19:08:55.000000 PyComplexHeatmap-1.5.3/README.md
+-rw-r--r--   0 wding      (503) staff       (20)      876 2023-07-27 19:02:25.000000 PyComplexHeatmap-1.5.3/pyproject.toml
+-rw-r--r--   0 wding      (503) staff       (20)       38 2023-07-27 19:11:42.175777 PyComplexHeatmap-1.5.3/setup.cfg
+-rw-r--r--   0 wding      (503) staff       (20)     1044 2023-07-27 18:48:46.000000 PyComplexHeatmap-1.5.3/setup.py
```

### Comparing `PyComplexHeatmap-1.5.2/LICENSE` & `PyComplexHeatmap-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.5.2/PKG-INFO` & `PyComplexHeatmap-1.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: PyComplexHeatmap
-Version: 1.5.2
-Summary: A python package to plot complex heatmap
-Home-page: https://github.com/DingWB/PyComplexHeatmap
-Author: Wubin Ding
-Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
-Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
-Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyComplexHeatmap [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=total&units=international_system&left_color=blue&right_color=black&left_text=Downloads)](https://pepy.tech/project/pycomplexheatmap) [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=month&units=international_system&left_color=green&right_color=orange&left_text=Last%20Month)](https://pepy.tech/project/pycomplexheatmap) [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=week&units=international_system&left_color=red&right_color=brightgreen&left_text=This%20week)](https://pepy.tech/project/pycomplexheatmap)
 PyComplexHeatmap is a Python package to plot complex heatmap (clustermap). Please click [here](https://dingwb.github.io/PyComplexHeatmap) for documentation.
 
 ## Documentation:
 ----------------------
 [https://dingwb.github.io/PyComplexHeatmap](https://dingwb.github.io/PyComplexHeatmap)
 <br><br>
@@ -29,21 +13,21 @@
 <br>
 [wiki/Parameters](../../wiki/Parameters/)
 <br>
 [wiki/Features](../../wiki/Features/)
 
 ## Dependencies:
 ----------------------
-- matplotlib>=3.4.3
+- matplotlib>=3.3.1
 - numpy
 - pandas
 - scipy
 - fastcluster
 ```
-pip install --ignore-install matplotlib==3.5.1 numpy==1.20.3 pandas==1.4.1
+pip install --ignore-install matplotlib numpy pandas
 pip install seaborn #only needed when call functions in tools.py
 ```
 
 ## Citation
 Ding, W., Goldberg, D. and Zhou, W. (2023), PyComplexHeatmap: A Python package to visualize multimodal genomics data. iMeta e115. https://doi.org/10.1002/imt2.115
 <br>
 **DOI**: 10.1002/imt2.115
```

### Comparing `PyComplexHeatmap-1.5.2/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.5.3/PyComplexHeatmap/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import matplotlib
 import matplotlib.pylab as plt
 from .utils import mm2inch
 from .utils import (
     _calculate_luminance,
     cluster_labels,
     plot_legend_list,
-    define_cmap
+    define_cmap,
+    get_colormap
 )
 from .clustermap import plot_heatmap,heatmap
 # -----------------------------------------------------------------------------
 class AnnotationBase():
     """
     Base class for annotation objects.
 
@@ -149,32 +150,32 @@
                 self.cmap = 'jet'
             else:
                 raise TypeError("Can not assign cmap for column %s, please specify cmap" % col)
         elif type(cmap) == str:
             self.cmap = cmap
         else:
             raise TypeError("Unknow data type for cmap!")
-        if plt.colormaps.get(self.cmap).N == 256:  # then heatmap will automatically calculate vmin and vmax
+        if get_colormap(self.cmap).N == 256:  # then heatmap will automatically calculate vmin and vmax
             try:
                 self.plot_kws.setdefault('vmax', np.nanmax(self.df.values))
                 self.plot_kws.setdefault('vmin', np.nanmin(self.df.values))
             except:
                 pass
 
     def _calculate_colors(self):  # add self.color_dict (each col is a dict)
         self.color_dict = {}
         col = self.df.columns.tolist()[0]
-        if plt.colormaps.get(self.cmap).N < 256 or self.df.dtypes[col] == object:
+        if get_colormap(self.cmap).N < 256 or self.df.dtypes[col] == object:
             cc_list = self.df[col].value_counts().index.tolist()  # sorted by value counts
             self.df[col] = self.df[col].map({v: cc_list.index(v) for v in cc_list})
             for v in cc_list:
-                color = plt.colormaps.get(self.cmap)(cc_list.index(v))
+                color = get_colormap(self.cmap)(cc_list.index(v))
                 self.color_dict[v] = color  # matplotlib.colors.to_hex(color)
         else:  # float
-            self.color_dict = {v: plt.colormaps.get(self.cmap)(v) for v in self.df[col].values}
+            self.color_dict = {v: get_colormap(self.cmap)(v) for v in self.df[col].values}
         self.colors = None
 
     def _check_colors(self, colors):
         if isinstance(colors, str):
             colors = {label: colors for label in self.df.iloc[:, 0].unique()}
         if isinstance(colors, list):
             assert len(colors) == self.df.iloc[:, 0].nunique()
@@ -188,15 +189,15 @@
 
     def _calculate_cmap(self):
         self.color_dict = self.colors
         col = self.df.columns.tolist()[0]
         cc_list = list(self.color_dict.keys())  # column values
         self.df[col] = self.df[col].map({v: cc_list.index(v) for v in cc_list})
         self.cmap = matplotlib.colors.ListedColormap([self.color_dict[k] for k in cc_list])
-        self.plot_kws.setdefault('vmax', plt.colormaps.get(self.cmap).N-1)
+        self.plot_kws.setdefault('vmax', get_colormap(self.cmap).N-1)
         self.plot_kws.setdefault('vmin', 0)
 
     def _type_specific_params(self):
         pass
 
     def reorder(self, idx):  # Before plotting, df needs to be reordered according to the new clustered order.
         """
@@ -252,22 +253,22 @@
         self.text_kws.setdefault('zorder', 16)
         self.text_kws.setdefault('ha', 'center')
         self.text_kws.setdefault('va', 'center')
 
     def _calculate_colors(self):  # add self.color_dict (each col is a dict)
         self.color_dict = {}
         col = self.df.columns.tolist()[0]
-        if plt.colormaps.get(self.cmap).N < 256:
+        if get_colormap(self.cmap).N < 256:
             cc_list = self.df[col].value_counts().index.tolist()  # sorted by value counts
             for v in cc_list:
-                color = plt.colormaps.get(self.cmap)(cc_list.index(v))
+                color = get_colormap(self.cmap)(cc_list.index(v))
                 self.color_dict[v] = color  # matplotlib.colors.to_hex(color)
         else:  # float
             cc_list = None
-            self.color_dict = {v: plt.colormaps.get(self.cmap)(v) for v in self.df[col].values}
+            self.color_dict = {v: get_colormap(self.cmap)(v) for v in self.df[col].values}
         self.cc_list = cc_list
         self.colors = None
 
     def _calculate_cmap(self):
         self.color_dict = self.colors
         col = self.df.columns.tolist()[0]
         cc_list = list(self.color_dict.keys())  # column values
@@ -275,18 +276,18 @@
         self.cmap = matplotlib.colors.ListedColormap([self.color_dict[k] for k in cc_list])
 
     def plot(self, ax=None, axis=1, subplot_spec=None, label_kws={},
              ticklabels_kws={}):  # add self.gs,self.fig,self.ax,self.axes
         if hasattr(self.cmap,'N'):
             vmax=self.cmap.N-1
         elif type(self.cmap)==str:
-            vmax=plt.colormaps.get(self.cmap).N-1
+            vmax=get_colormap(self.cmap).N-1
         else:
             vmax=len(self.color_dict)-1
-        self.plot_kws.setdefault('vmax',vmax)  # plt.colormaps.get(self.cmap).N
+        self.plot_kws.setdefault('vmax',vmax)  # get_colormap(self.cmap).N
         self.plot_kws.setdefault('vmin', 0)
         if self.cc_list:
             mat = self.plot_data.iloc[:, 0].map({v: self.cc_list.index(v) for v in self.cc_list}).values
         else:
             mat = self.plot_data.values
         matrix = mat.reshape(1, -1) if axis == 1 else mat.reshape(-1, 1)
         # print(matrix)
@@ -412,21 +413,21 @@
         # self.plot_kws.setdefault('transform_rotates_text', False)
         self.plot_kws.setdefault('arrowprops', arrowprops)
         self.plot_kws.setdefault('rotation_mode', 'anchor')
 
     def _calculate_colors(self):  # add self.color_dict (each col is a dict)
         self.color_dict = {}
         col = self.df.columns.tolist()[0]
-        if plt.colormaps.get(self.cmap).N < 256 or self.df.dtypes[col] == object:
+        if get_colormap(self.cmap).N < 256 or self.df.dtypes[col] == object:
             cc_list = self.df[col].value_counts().index.tolist()  # sorted by value counts
             for v in cc_list:
-                color = plt.colormaps.get(self.cmap)(cc_list.index(v))
+                color = get_colormap(self.cmap)(cc_list.index(v))
                 self.color_dict[v] = color  # matplotlib.colors.to_hex(color)
         else:  # float
-            self.color_dict = {v: plt.colormaps.get(self.cmap)(v) for v in self.df[col].values}
+            self.color_dict = {v: get_colormap(self.cmap)(v) for v in self.df[col].values}
         self.colors = None
 
     def _calculate_cmap(self):
         self.color_dict = self.colors
         col = self.df.columns.tolist()[0]
         cc_list = list(self.color_dict.keys())  # column values
         self.cmap = matplotlib.colors.ListedColormap([self.color_dict[k] for k in cc_list])
@@ -594,15 +595,15 @@
         gap = self.df.max().max() - self.df.min().min()
         self.ylim = [self.df.min().min() - 0.02 * gap, self.df.max().max() + 0.02 * gap]
 
     def plot(self, ax=None, axis=1, subplot_spec=None, label_kws={},
              ticklabels_kws={}):  # add self.gs,self.fig,self.ax,self.axes
         fig = ax.figure
         if self.colors is None:  # calculate colors based on cmap
-            colors = [plt.colormaps.get(self.cmap)(self.plot_data.loc[sampleID].mean()) for sampleID in
+            colors = [get_colormap(self.cmap)(self.plot_data.loc[sampleID].mean()) for sampleID in
                       self.plot_data.index.values]
         else:
             colors = [self.colors] * self.plot_data.shape[0]  # self.colors is a string
         # print(self.plot_kws)
         plot_kws = self.plot_kws.copy()
         edgecolor = plot_kws.pop('edgecolor')
         mlinecolor = plot_kws.pop('medianlinecolor')
@@ -659,33 +660,33 @@
             if self.ncols == 1:
                 self.cmap = 'jet'
             else:
                 self.cmap = 'Set1'
         # print(cmap,self.cmap)
         else:
             self.cmap = cmap
-        if self.ncols >= 2 and plt.colormaps.get(self.cmap).N >= 256:
+        if self.ncols >= 2 and get_colormap(self.cmap).N >= 256:
             raise TypeError("cmap for stacked barplot should not be continuous, you should try: Set1, Dark2 and so on.")
 
     def _calculate_colors(self):  # add self.color_dict (each col is a dict)
         col_list = self.df.columns.tolist()
         self.color_dict = {}
         if len(col_list) >= 2:  # more than two columns, colored by columns names
-            self.colors = [plt.colormaps.get(self.cmap)(col_list.index(v)) for v in self.df.columns]
+            self.colors = [get_colormap(self.cmap)(col_list.index(v)) for v in self.df.columns]
             for v, color in zip(col_list, self.colors):
                 self.color_dict[v] = color
         else:  # only one column, colored by cols[0] values (float)
             # vmax, vmin = np.nanmax(self.df[col_list[0]].values), np.nanmin(self.df[col_list[0]].values)
             # delta = vmax - vmin
             # values = self.df[col_list[0]].fillna(np.nan).unique()
             self.cmap,normalize=define_cmap(self.df[col_list[0]].fillna(np.nan).values,
                                             vmin=None, vmax=None, cmap=self.cmap,
                                             center=None, robust=False,
                           na_col='white')
-            # self.colors = {v: matplotlib.colors.rgb2hex(plt.colormaps.get(self.cmap)((v - vmin) / delta)) for v in values}
+            # self.colors = {v: matplotlib.colors.rgb2hex(get_colormap(self.cmap)((v - vmin) / delta)) for v in values}
             self.colors = lambda v:matplotlib.colors.rgb2hex(self.cmap(normalize(v))) #a function
             self.color_dict = None
 
     def _check_colors(self, colors):
         if not isinstance(colors, (list, str)):
             raise TypeError("colors must be list of string for barplot if provided !")
         if type(colors) == str:
@@ -726,15 +727,15 @@
         if grid:
             ax.grid(linestyle='--', zorder=-10)
         # bar_ct = ax.bar(x=list(range(1, self.nrows + 1,1)),
         #                 height=self.plot_data.values,**self.plot_kws)
         if type(self.colors) == list:
             colors = self.colors
         else: #dict
-            #bad_value_color = matplotlib.colors.rgb2hex(plt.colormaps.get(self.cmap).get_bad())
+            #bad_value_color = matplotlib.colors.rgb2hex(get_colormap(self.cmap).get_bad())
             # colors = [[self.colors.get(v, bad_value_color) for v in self.plot_data.iloc[:, 0].values]]
             colors = [[self.colors(v) for v in self.plot_data.iloc[:, 0].values]]
         base_coordinates = [0] * self.plot_data.shape[0]
         for col, color in zip(self.plot_data.columns, colors):
             if axis == 1:
                 ax.set_xticks(ticks=np.arange(0.5, self.nrows, 1))
                 ax.bar(x=np.arange(0.5, self.nrows, 1), height=self.plot_data[col].values,
@@ -1211,15 +1212,15 @@
         for annotation in self.annotations:
             if not annotation.legend:
                 continue
             legend_kws = annotation.legend_kws.copy()
             # print(annotation.cmap,annotation)
             if (annotation.cmap is None) or \
                 (hasattr(annotation.cmap,'N') and annotation.cmap.N < 256) or \
-                (type(annotation.cmap) ==str and plt.colormaps.get(annotation.cmap).N < 256):
+                (type(annotation.cmap) ==str and get_colormap(annotation.cmap).N < 256):
                 color_dict = annotation.color_dict
                 if color_dict is None:
                     continue
                 self.legend_list.append(
                     [annotation.color_dict, annotation.label, legend_kws, len(annotation.color_dict),'color_dict'])
             else:
                 if annotation.df.shape[1] == 1:
```

### Comparing `PyComplexHeatmap-1.5.2/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.5.3/PyComplexHeatmap/clustermap.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     despine,
     _draw_figure,
     axis_ticklabels_overlap,
     _skip_ticks,
     _auto_ticks,
     _index_to_label,
     _index_to_ticklabels,
-    plot_legend_list
+    plot_legend_list,
+    get_colormap
 )
 # =============================================================================
 class heatmapPlotter:
     def __init__(self, data=None, vmin=None, vmax=None, cmap='bwr', center=None,
                  robust=True, annot=None, fmt='.2g',
                  annot_kws=None, cbar=True, cbar_kws=None,
                  xlabel=None, ylabel=None,
@@ -131,27 +132,27 @@
                 vmax = np.nanmax(calc_data)
         self.vmin, self.vmax = vmin, vmax
 
         # Choose default colormaps if not provided
         if cmap is None:
             if center is None:
                 try:
-                    self.cmap = plt.colormaps.get('turbo').copy()
+                    self.cmap = get_colormap('turbo').copy()
                 except:
-                    self.cmap = plt.colormaps.get('turbo')
+                    self.cmap = get_colormap('turbo')
             else:
                 try:
-                    self.cmap = plt.colormaps.get('exp1').copy()
+                    self.cmap = get_colormap('exp1').copy()
                 except:
-                    self.cmap = plt.colormaps.get('exp1')
+                    self.cmap = get_colormap('exp1')
         elif isinstance(cmap, str):
             try:
-                self.cmap = plt.colormaps.get(cmap).copy()
+                self.cmap = get_colormap(cmap).copy()
             except:
-                self.cmap = plt.colormaps.get(cmap)
+                self.cmap = get_colormap(cmap)
         elif isinstance(cmap, list):
             self.cmap = matplotlib.colors.ListedColormap(cmap)
         else:
             self.cmap = cmap
 
         self.cmap.set_bad(color=self.na_col)  # set the color for NaN values
         # Recenter a divergent colormap
@@ -447,17 +448,17 @@
             vmax = np.nanpercentile(calc_data, 98)
         else:
             vmax = np.nanmax(calc_data)
 
     # Choose default colormaps if not provided
     if isinstance(cmap, str):
         try:
-            cmap = plt.colormaps.get(cmap).copy()
+            cmap = get_colormap(cmap).copy()
         except:
-            cmap = plt.colormaps.get(cmap)
+            cmap = get_colormap(cmap)
 
     cmap.set_bad(color=na_col)  # set the color for NaN values
     # Recenter a divergent colormap
     if center is not None:
         # bad = cmap(np.ma.masked_invalid([np.nan]))[0]  # set the first color as the na_color
         under = cmap(-np.inf)
         over = cmap(np.inf)
@@ -1237,15 +1238,15 @@
                 ax1.set_axis_off()
                 self.ax_row_dendrogram_axes.append(ax1)
 
             try:
                 if rcmap is None:
                     colors = ['black'] * len(self.dendrogram_rows)
                 else:
-                    colors = [plt.colormaps.get(rcmap)(i) for i in range(len(self.dendrogram_rows))]
+                    colors = [get_colormap(rcmap)(i) for i in range(len(self.dendrogram_rows))]
                 for ax_row_dendrogram, dendrogram_row, color in zip(self.ax_row_dendrogram_axes, self.dendrogram_rows,
                                                                     colors):
                     if dendrogram_row is None:
                         continue
                     tree_kws['colors'] = [color] * len(dendrogram_row.dendrogram['ivl'])
                     dendrogram_row.plot(ax=ax_row_dendrogram, tree_kws=tree_kws)
             except:
@@ -1266,15 +1267,15 @@
                 ax1.set_axis_off()
                 self.ax_col_dendrogram_axes.append(ax1)
 
             try:
                 if ccmap is None:
                     colors = ['black'] * len(self.dendrogram_cols)
                 else:
-                    colors = [plt.colormaps.get(ccmap)(i) for i in range(len(self.dendrogram_cols))]
+                    colors = [get_colormap(ccmap)(i) for i in range(len(self.dendrogram_cols))]
                 for ax_col_dendrogram, dendrogram_col, color in zip(self.ax_col_dendrogram_axes, self.dendrogram_cols,
                                                                     colors):
                     if dendrogram_col is None:
                         continue
                     tree_kws['colors'] = [color] * len(dendrogram_col.dendrogram['ivl'])
                     dendrogram_col.plot(ax=ax_col_dendrogram, tree_kws=tree_kws)
             except:
@@ -1505,15 +1506,15 @@
         matplotlib.figure.Figure.set_figwidth(fig, width)  # convert mm to inches
 
     def post_processing(self):
         pass
 # =============================================================================
 def composite(cmlist=None, main=0, ax=None, axis=1, row_gap=15, col_gap=15,
               legend_side='right', legend_gap=5, legend_y=0.8, legend_hpad=None,
-              legend_width=None):
+              legend_width=None, width_ratios=None, height_ratios=None):
     """
     Assemble multiple ClusterMapPlotter objects vertically or horizontally together.
 
     Parameters
     ----------
     cmlist: list
         a list of ClusterMapPlotter (with plot=False).
@@ -1524,14 +1525,20 @@
         of cmlist.
     row/col_gap: float
         the row or columns gap between subplots, unit is mm [15].
     legend_side: str
         right,left [right].
     legend_gap: float
         row gap between two legends, unit is mm.
+    legend_width: float
+        default is None, will be estimated automatically
+    width_ratios: list
+        a list of width, values can be either float or int.
+    height_ratios: list
+        a list of height, values can be either float or int.
 
     Returns
     -------
     tuple:
         ax,legend_axes
 
     """
@@ -1539,22 +1546,22 @@
         ax = plt.gca()
     n = len(cmlist)
     wspace, hspace = 0, 0
     if axis == 1:  # horizontally
         wspace = col_gap * mm2inch * ax.figure.dpi / (ax.get_window_extent().width / n)
         nrows = 1
         ncols = n
-        width_ratios = [cm.data2d.shape[1] for cm in cmlist]
+        width_ratios = [cm.data2d.shape[1] for cm in cmlist] if width_ratios is None else width_ratios
         height_ratios = None
     else:  # vertically
         hspace = row_gap * mm2inch * ax.figure.dpi / (ax.get_window_extent().height / n)
         nrows = n
         ncols = 1
         width_ratios = None
-        height_ratios = [cm.data2d.shape[0] for cm in cmlist]
+        height_ratios = [cm.data2d.shape[0] for cm in cmlist] if height_ratios is None else height_ratios
     gs = ax.figure.add_gridspec(nrows, ncols, width_ratios=width_ratios,
                                 height_ratios=height_ratios,
                                 wspace=wspace, hspace=hspace)
     axes = []
     for i, cm in enumerate(cmlist):
         sharex = axes[0] if axis == 0 and i > 0 else None
         sharey = axes[0] if axis == 1 and i > 0 else None
@@ -1569,15 +1576,21 @@
     legend_list = cm_1.legend_list
     legend_names = [L[1] for L in legend_list]
     label_max_width = ax.figure.get_window_extent().width * cm_1.label_max_width / cm_1.ax.figure.get_window_extent().width
     for i, cm in enumerate(cmlist):
         if i == main:
             continue
         gs1 = gs[i, 0] if axis == 0 else gs[0, i]
-        cm.plot(ax=axes[i], subplot_spec=gs1, row_order=cm_1.row_order, col_order=cm_1.col_order)
+        if axis==1: #composite horizontally, have the same row order
+            col_order=None
+            row_order=cm_1.row_order
+        else: # vertically, have the same col order
+            row_order=None
+            col_order=cm_1.col_order
+        cm.plot(ax=axes[i], subplot_spec=gs1, row_order=row_order, col_order=col_order)
         for L in cm.legend_list:
             if L[1] not in legend_names:
                 legend_names.append(L[1])
                 legend_list.append(L)
         w = ax.figure.get_window_extent().width * cm.label_max_width / cm.ax.figure.get_window_extent().width
         if w > label_max_width:
             label_max_width = w
```

### Comparing `PyComplexHeatmap-1.5.2/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.5.3/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.5.2/PyComplexHeatmap/dotHeatmap.py` & `PyComplexHeatmap-1.5.3/PyComplexHeatmap/dotHeatmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # !/usr/bin/env python3
 import os, sys
 import pandas as pd
 import numpy as np
 import matplotlib
 import matplotlib.pylab as plt
-from .utils import mm2inch,plot_legend_list,despine
+from .utils import mm2inch,plot_legend_list,despine,get_colormap
 from .clustermap import ClusterMapPlotter
 from matplotlib.ticker import MultipleLocator, FormatStrFormatter
 # =============================================================================
 def scale(values,vmin=None,vmax=None):
     if vmin is None:
         vmin=np.nanmin(values)
     if vmax is None:
@@ -130,15 +130,15 @@
         kwargs.setdefault('cmap', cmap)
         c_ready = True
     elif not hue is None and isinstance(cmap,str):
         color_dict = {} #keys are categorical values from hue, values are colors.
         if colors is None:  #using cmap
             col_list = df['Hue'].value_counts().index.tolist()
             for c in col_list:
-                color_dict[c] = matplotlib.colors.to_hex(plt.colormaps.get(cmap)(col_list.index(c)))
+                color_dict[c] = matplotlib.colors.to_hex(get_colormap(cmap)(col_list.index(c)))
         elif type(colors) == dict:
             color_dict = colors
         elif type(colors) == str:
             col_list = df['Hue'].value_counts().index.tolist()
             for c in col_list:
                 color_dict[c] = colors
         else:
@@ -400,15 +400,15 @@
                     self.label_max_width = annotation.label_max_width
         if self.legend:
             if isinstance(self.cmap,str) and not self.hue is None and self.c is None:  #
                 color_dict = {}
                 col_list = self.kwargs['hue'].unstack().value_counts().index.tolist()
                 # print(col_list,self.kwargs['hue'])
                 for c in col_list:
-                    color_dict[c] = matplotlib.colors.to_hex(plt.colormaps.get(self.cmap)(col_list.index(c)))
+                    color_dict[c] = matplotlib.colors.to_hex(get_colormap(self.cmap)(col_list.index(c)))
                 self.legend_list.append([color_dict, self.hue, self.color_legend_kws, len(color_dict), 'color_dict'])
             cmap=self.cmap
             c=self.kwargs.get('c',None)
             cmap_legend_kws=self.cmap_legend_kws.copy()
             cmap_legend_kws['vmax'] = self.v_vmax
             cmap_legend_kws['vmin'] = self.v_vmin
             if not cmap is None and type(cmap) == str and not c is None and type(c)!=str:
```

### Comparing `PyComplexHeatmap-1.5.2/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.5.3/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.5.2/PyComplexHeatmap/oncoPrint.py` & `PyComplexHeatmap-1.5.3/PyComplexHeatmap/oncoPrint.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # !/usr/bin/env python3
 import os, sys
 import pandas as pd
 import numpy as np
 from scipy.cluster import hierarchy
 import matplotlib
 import matplotlib.pylab as plt
-from .utils import _draw_figure,mm2inch,plot_legend_list,despine,_index_to_ticklabels
+from .utils import _draw_figure,mm2inch,plot_legend_list,despine,_index_to_ticklabels,get_colormap
 from .clustermap import ClusterMapPlotter
 from .annotations import HeatmapAnnotation, anno_barplot
 from matplotlib.ticker import MultipleLocator, FormatStrFormatter
 # =============================================================================
 def oncoprint(data,ax=None,colors=None, cmap='Set1',nvar=None,
               aspect=None,bgcolor='whitesmoke',row_gap=1,
               xticklabels_kws=None,subplot_spec=None,
@@ -44,15 +44,15 @@
     """
     if ax is None:
         ax = plt.gca()
     nrows, ncols = data.shape
     if nvar is None:
         nvar=data.iloc[:,0].apply(lambda x:len(x)).max()
     if colors is None:
-        colors=[plt.colormaps.get(cmap)(i) for i in range(nvar)]
+        colors=[get_colormap(cmap)(i) for i in range(nvar)]
     plot_kws.setdefault('width',0.7)
     plot_kws.setdefault('align', 'center')
     rowticklabels=_index_to_ticklabels(data.index)
     colticklabels=_index_to_ticklabels(data.columns)
     ax.set_ylim(0, nrows)
     y_locater = list(np.arange(0.5, nrows, 1))
     ax.yaxis.set_major_locator(plt.FixedLocator(y_locater))
@@ -175,15 +175,15 @@
         if self.remove_empty_cols:
             data2d=data2d.loc[:,df_sum.sum(axis=0)>0]
         row_vc = data2d.apply(lambda x: x.apply(np.array).sum(), axis=1)
         self.row_vc = pd.DataFrame(row_vc.tolist(), index=row_vc.index.tolist(), columns=self.values)
         self.col_vc = data2d.apply(lambda x: x.apply(np.array).sum(), axis=0).T
         self.col_vc.columns=self.values
         if self.colors is None:
-            self.colors = [plt.colormaps.get(self.cmap)(i) for i in range(len(self.values))]
+            self.colors = [get_colormap(self.cmap)(i) for i in range(len(self.values))]
         self.color_dict = {}
         for label, color in zip(self.values, self.colors):
             self.color_dict[label] = color
         return data2d
 
     def _reorder_rows(self):
         if self.verbose >= 1:
```

### Comparing `PyComplexHeatmap-1.5.2/PyComplexHeatmap/tools.py` & `PyComplexHeatmap-1.5.3/PyComplexHeatmap/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # !/usr/bin/env python3
 import os, sys
 import pandas as pd
 import matplotlib
 import matplotlib.pylab as plt
 import seaborn as sns
 import numpy as np
+from .utils import get_colormap
 
 def tbarplot(df=None,x=None,y=None,hue=None,hue_order=None,palette='Set1',figsize=(4,6),
              outname='test.pdf',title=''):
     """
     Plot barplot with text on the top of bar.
 
     Parameters
@@ -79,15 +80,15 @@
 
     Returns
     -------
 
     """
     if not hue is None:
         hue_order=df[hue].unique().tolist() if hue_order is None else hue_order
-        color_dict={h:plt.colormaps.get(cmap)(hue_order.index(h)) for h in hue_order}
+        color_dict={h:get_colormap(cmap)(hue_order.index(h)) for h in hue_order}
     else:
         color_dict=None
         hue_order=None
     N=list(range(1,df.shape[0]+1))
     s_min = np.nanmin(df[size].values)
     delta_s = np.nanmax(df[size].values) - s_min
     fig, ax = plt.subplots(figsize=figsize)
```

### Comparing `PyComplexHeatmap-1.5.2/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.5.3/PyComplexHeatmap/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,20 @@
         'savefig.bbox': 'tight',
         'savefig.dpi':300,
         'savefig.pad_inches': 0.05
     }
     
     rcParams.update(D)
 # =============================================================================
+def get_colormap(cmap):
+    try:
+        return plt.colormaps.get(cmap) # matplotlib >= 3.5.1?
+    except:
+        return plt.get_cmap(cmap) # matplotlib <=3.4.3?
+
 def _check_mask(data, mask):
     """
 
     Ensure that data and mask are compatible and add missing values and infinite values.
     Values will be plotted for cells where ``mask`` is ``False``.
     ``data`` is expected to be a DataFrame; ``mask`` can be an array or
     a DataFrame.
```

### Comparing `PyComplexHeatmap-1.5.2/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.5.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,41 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.5.2
+Version: 1.5.3
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2022 Wubin Ding
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
+Project-URL: repository, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
+Project-URL: documentation, https://dingwb.github.io/PyComplexHeatmap
+Keywords: ComplexHeatmap,heatmap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -29,21 +54,21 @@
 <br>
 [wiki/Parameters](../../wiki/Parameters/)
 <br>
 [wiki/Features](../../wiki/Features/)
 
 ## Dependencies:
 ----------------------
-- matplotlib>=3.4.3
+- matplotlib>=3.3.1
 - numpy
 - pandas
 - scipy
 - fastcluster
 ```
-pip install --ignore-install matplotlib==3.5.1 numpy==1.20.3 pandas==1.4.1
+pip install --ignore-install matplotlib numpy pandas
 pip install seaborn #only needed when call functions in tools.py
 ```
 
 ## Citation
 Ding, W., Goldberg, D. and Zhou, W. (2023), PyComplexHeatmap: A Python package to visualize multimodal genomics data. iMeta e115. https://doi.org/10.1002/imt2.115
 <br>
 **DOI**: 10.1002/imt2.115
```

### Comparing `PyComplexHeatmap-1.5.2/README.md` & `PyComplexHeatmap-1.5.3/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,48 @@
+Metadata-Version: 2.1
+Name: PyComplexHeatmap
+Version: 1.5.3
+Summary: A python package to plot complex heatmap
+Home-page: https://github.com/DingWB/PyComplexHeatmap
+Author: Wubin Ding
+Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2022 Wubin Ding
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
+Project-URL: repository, https://github.com/DingWB/PyComplexHeatmap
+Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
+Project-URL: documentation, https://dingwb.github.io/PyComplexHeatmap
+Keywords: ComplexHeatmap,heatmap
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyComplexHeatmap [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=total&units=international_system&left_color=blue&right_color=black&left_text=Downloads)](https://pepy.tech/project/pycomplexheatmap) [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=month&units=international_system&left_color=green&right_color=orange&left_text=Last%20Month)](https://pepy.tech/project/pycomplexheatmap) [![Downloads](https://static.pepy.tech/personalized-badge/pycomplexheatmap?period=week&units=international_system&left_color=red&right_color=brightgreen&left_text=This%20week)](https://pepy.tech/project/pycomplexheatmap)
 PyComplexHeatmap is a Python package to plot complex heatmap (clustermap). Please click [here](https://dingwb.github.io/PyComplexHeatmap) for documentation.
 
 ## Documentation:
 ----------------------
 [https://dingwb.github.io/PyComplexHeatmap](https://dingwb.github.io/PyComplexHeatmap)
 <br><br>
@@ -13,21 +54,21 @@
 <br>
 [wiki/Parameters](../../wiki/Parameters/)
 <br>
 [wiki/Features](../../wiki/Features/)
 
 ## Dependencies:
 ----------------------
-- matplotlib>=3.4.3
+- matplotlib>=3.3.1
 - numpy
 - pandas
 - scipy
 - fastcluster
 ```
-pip install --ignore-install matplotlib==3.5.1 numpy==1.20.3 pandas==1.4.1
+pip install --ignore-install matplotlib numpy pandas
 pip install seaborn #only needed when call functions in tools.py
 ```
 
 ## Citation
 Ding, W., Goldberg, D. and Zhou, W. (2023), PyComplexHeatmap: A Python package to visualize multimodal genomics data. iMeta e115. https://doi.org/10.1002/imt2.115
 <br>
 **DOI**: 10.1002/imt2.115
```

### Comparing `PyComplexHeatmap-1.5.2/pyproject.toml` & `PyComplexHeatmap-1.5.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [build-system]
-requires = ["setuptools>=61.0","matplotlib>=3.5.1","numpy>=1.20.3","pandas>=1.3.5", "scipy","fastcluster"]
+requires = ["setuptools>=61.0","matplotlib>=3.3.1","numpy","pandas>=1.3.5", "scipy","fastcluster","seaborn"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyComplexHeatmap"
-version = "1.5.2"
+version = "1.5.3"
 authors = [
   { name="Wubin Ding", email="ding.wu.bin.gm@gmail.com" },
 ]
 description = "A python package to plot complex heatmap"
+keywords = ["ComplexHeatmap", "heatmap"]
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+license = {file = "LICENSE"}
 
 [project.urls]
 "Homepage" = "https://github.com/DingWB/PyComplexHeatmap"
+repository = "https://github.com/DingWB/PyComplexHeatmap"
 "Bug Tracker" = "https://github.com/DingWB/PyComplexHeatmap/issues"
+documentation = "https://dingwb.github.io/PyComplexHeatmap"
```

### Comparing `PyComplexHeatmap-1.5.2/setup.py` & `PyComplexHeatmap-1.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 # print(long_description)
 
 #release new version
 setup(
    name='PyComplexHeatmap',
-   version='1.5.2',
+   version='1.5.3',
    description='A Python package to plot complex heatmap',
    # long_description="#PyComplexHeatmap\n##Documentation:https://dingwb.github.io/PyComplexHeatmap/build/html/index.html",
    # long_description_content_type='text/markdown',
    author='Wubin Ding',
    author_email='ding.wu.bin.gm@gmail.com',
    url="https://github.com/DingWB/PyComplexHeatmap",
    packages=['PyComplexHeatmap'], #src
```

