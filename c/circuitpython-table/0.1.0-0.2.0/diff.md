# Comparing `tmp/circuitpython-table-0.1.0.tar.gz` & `tmp/circuitpython-table-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-table-0.1.0.tar", last modified: Sat Jul 22 20:27:57 2023, max compression
+gzip compressed data, was "circuitpython-table-0.2.0.tar", last modified: Thu Jul 27 13:21:40 2023, max compression
```

## Comparing `circuitpython-table-0.1.0.tar` & `circuitpython-table-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:27:57.103355 circuitpython-table-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:27:57.099355 circuitpython-table-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:27:57.099355 circuitpython-table-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-22 20:27:57.103355 circuitpython-table-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:27:57.103355 circuitpython-table-0.1.0/circuitpython_table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-22 20:27:57.000000 circuitpython-table-0.1.0/circuitpython_table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-22 20:27:57.000000 circuitpython-table-0.1.0/circuitpython_table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:27:57.000000 circuitpython-table-0.1.0/circuitpython_table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-22 20:27:57.000000 circuitpython-table-0.1.0/circuitpython_table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 20:27:57.000000 circuitpython-table-0.1.0/circuitpython_table.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:27:57.103355 circuitpython-table-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:27:57.103355 circuitpython-table-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:27:57.103355 circuitpython-table-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-22 20:27:47.000000 circuitpython-table-0.1.0/examples/table_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-22 20:27:47.000000 circuitpython-table-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-22 20:27:35.000000 circuitpython-table-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:27:57.103355 circuitpython-table-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-22 20:27:47.000000 circuitpython-table-0.1.0/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:21:40.213177 circuitpython-table-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:21:40.209177 circuitpython-table-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:21:40.209177 circuitpython-table-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-27 13:21:40.213177 circuitpython-table-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:21:40.213177 circuitpython-table-0.2.0/circuitpython_table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-27 13:21:40.000000 circuitpython-table-0.2.0/circuitpython_table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-27 13:21:40.000000 circuitpython-table-0.2.0/circuitpython_table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:21:40.000000 circuitpython-table-0.2.0/circuitpython_table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-27 13:21:40.000000 circuitpython-table-0.2.0/circuitpython_table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 13:21:40.000000 circuitpython-table-0.2.0/circuitpython_table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:21:40.213177 circuitpython-table-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:21:40.213177 circuitpython-table-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:21:40.213177 circuitpython-table-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-27 13:21:31.000000 circuitpython-table-0.2.0/examples/table_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-27 13:21:31.000000 circuitpython-table-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-27 13:21:18.000000 circuitpython-table-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:21:40.213177 circuitpython-table-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-07-27 13:21:31.000000 circuitpython-table-0.2.0/table.py
```

### Comparing `circuitpython-table-0.1.0/.github/workflows/build.yml` & `circuitpython-table-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-table-0.1.0/.github/workflows/release_gh.yml` & `circuitpython-table-0.2.0/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-table-0.1.0/.pre-commit-config.yaml` & `circuitpython-table-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-table-0.1.0/.pylintrc` & `circuitpython-table-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-table-0.1.0/LICENSE` & `circuitpython-table-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-table-0.1.0/PKG-INFO` & `circuitpython-table-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-table
-Version: 0.1.0
+Version: 0.2.0
 Summary: CircuitPython Library to creat tables
 Author-email: JDM <xxx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_TABLE
 Keywords: sensor,blinka,circuitpython,micropython,table,table,cells,rows
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-table-0.1.0/README.rst` & `circuitpython-table-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-table-0.1.0/circuitpython_table.egg-info/PKG-INFO` & `circuitpython-table-0.2.0/circuitpython_table.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-table
-Version: 0.1.0
+Version: 0.2.0
 Summary: CircuitPython Library to creat tables
 Author-email: JDM <xxx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_TABLE
 Keywords: sensor,blinka,circuitpython,micropython,table,table,cells,rows
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-table-0.1.0/circuitpython_table.egg-info/SOURCES.txt` & `circuitpython-table-0.2.0/circuitpython_table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-table-0.1.0/docs/_static/Logo.png` & `circuitpython-table-0.2.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-table-0.1.0/docs/_static/favicon.ico` & `circuitpython-table-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-table-0.1.0/docs/conf.py` & `circuitpython-table-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-table-0.1.0/pyproject.toml` & `circuitpython-table-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-table"
 description = "CircuitPython Library to creat tables"
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_TABLE"}
 keywords = [
     "sensor",
```

### Comparing `circuitpython-table-0.1.0/table.py` & `circuitpython-table-0.2.0/table.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,66 +15,70 @@
 
 import displayio
 from bitmaptools import draw_line
 from adafruit_bitmap_font import bitmap_font
 from adafruit_display_text import bitmap_label
 
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_TABLE.git"
 
 
 class Table(displayio.Group):
     """
     Create a table with the given parameters.
 
     :param int originx: The x origin of the table.
     :param int originy: The y origin of the table.
     :param int width: The width of the table.
     :param int height: The height of the table.
     :param list table: The table to be displayed.
     :param str font_file: The font file to be used.
-    :param int color: Line color. Defaults to 0xFFFFFF. White.
+    :param int color: Line color. Defaults to 0xFFFFFF
+    :param int text_color: Text color. Defaults to 0x123456
 
     """
 
     def __init__(
         self,
-        originx,
-        originy,
-        width=480,
-        height=320,
+        originx: int,
+        originy: int,
+        width: int = 200,
+        height: int = 200,
         structure: list = None,
         table: list = None,
         font_file=None,
-        color: int = 0xFFFFFF,
+        border_color: int = 0xFFFFFF,
+        text_color: int = 0x123456,
     ) -> None:
-        super().__init__(x=0, y=0, scale=1)
+        super().__init__(x=originx, y=originy, scale=1)
+        self._padding = 3
+        self._plotbitmap = displayio.Bitmap(
+            width + 2 * self._padding, height + 2 * self._padding, 10
+        )
         self._table = table
+        self._text_color = text_color
 
-        self._plotbitmap = displayio.Bitmap(width, height, 20)
-
-        self._colum_size = [originx]
-        self._row_size = [originy]
+        self._colum_size = [0]
+        self._row_size = [0]
         self._font_to_use = bitmap_font.load_font(font_file)
-        width, height, _, self._dy = self._font_to_use.get_bounding_box()
+        widtht, heightt, _, self._dy = self._font_to_use.get_bounding_box()
 
-        self._origin_x = originx
-        self._origin_y = originy
-        self._padding = 3
+        self._origin_x = 0
+        self._origin_y = 0
 
         self._get_structure(structure)
 
-        self._width = width
-        self._height = height
+        self._width = widtht
+        self._height = heightt
 
-        plot_palette = displayio.Palette(20)
+        plot_palette = displayio.Palette(10)
         plot_palette.make_transparent(0)
-        plot_palette[1] = color
-        plot_palette[2] = 0xFF0000
+        plot_palette[1] = 0xFFFFFF
+        plot_palette[2] = border_color
         plot_palette[3] = 0x00FF00
         plot_palette[4] = 0x0000FF
         plot_palette[5] = 0xFFFF00
         plot_palette[6] = 0x00FFFF
         plot_palette[7] = 0x123456
         plot_palette[8] = 0x654321
         plot_palette[9] = 0x000000
@@ -93,18 +97,24 @@
         """
         texth = bitmap_label.Label(self._font_to_use, text="-")
         textv = bitmap_label.Label(self._font_to_use, text="|")
         distanceh = 0
         distancev = 0
 
         for row in structure:
+            if len(structure[0]) == 1:
+                self._colum_size.append(
+                    self._origin_x + distanceh + len(row[0]) * texth.width
+                )
+                break
             for element in row:
-                start = self._origin_x + distanceh + len(element * texth.width)
+                start = self._origin_x + distanceh + len(element) * texth.width
+
                 self._colum_size.append(start)
-                distanceh = distanceh + len(element * texth.width)
+                distanceh = distanceh + len(element) * texth.width
 
         for row in self._table:
             start = self._origin_y + distancev + textv.height
             self._row_size.append(start)
             distancev = distancev + textv.height
 
     def create_borders(self, color_index=2):
@@ -113,37 +123,50 @@
 
 
         """
 
         for distance in self._colum_size:
             draw_line(
                 self._plotbitmap,
-                distance - self._padding,
-                self._origin_y + self._dy - self._padding,
-                distance - self._padding,
-                self._row_size[-1] + self._dy - self._padding,
+                distance,
+                self._origin_y,
+                distance,
+                self._row_size[-1],
                 color_index,
             )
 
         for distance in self._row_size:
             draw_line(
                 self._plotbitmap,
-                self._origin_x - self._padding,
-                distance + self._dy - self._padding,
-                self._colum_size[-1] - self._padding,
-                distance + self._dy - self._padding,
+                self._origin_x,
+                distance,
+                self._colum_size[-1],
+                distance,
                 color_index,
             )
 
     def create_label_objects(self):
         """
         Create label objects
         """
 
-        for j, row in enumerate(self._table):
-            if len(row) > 1:
-                for i, cell_text in enumerate(row):
-                    text = bitmap_label.Label(self._font_to_use, text=cell_text)
-                    text.x = self._colum_size[i]
-                    text.y = self._row_size[j]
+        if len(self._colum_size) == 2:
+            for j, row in enumerate(self._table):
+                text = bitmap_label.Label(
+                    self._font_to_use, text=row, color=self._text_color
+                )
+                text.x = self._colum_size[0] + self._padding
+                text.y = self._row_size[j] + self._padding - self._dy
+
+                self.append(text)
+
+        else:
+            for j, row in enumerate(self._table):
+                if len(row) > 1:
+                    for i, cell_text in enumerate(row):
+                        text = bitmap_label.Label(
+                            self._font_to_use, text=cell_text, color=self._text_color
+                        )
+                        text.x = self._colum_size[i] + self._padding
+                        text.y = self._row_size[j] + self._padding - self._dy
 
                     self.append(text)
```

