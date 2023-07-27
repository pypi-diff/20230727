# Comparing `tmp/nichord-0.1.7.tar.gz` & `tmp/nichord-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nichord-0.1.7.tar", last modified: Sun Jul 23 22:07:16 2023, max compression
+gzip compressed data, was "nichord-0.1.8.tar", last modified: Thu Jul 27 14:53:22 2023, max compression
```

## Comparing `nichord-0.1.7.tar` & `nichord-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 22:07:16.639710 nichord-0.1.7/
--rw-rw-rw-   0        0        0     1290 2023-07-23 22:07:16.639710 nichord-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    10897 2023-07-23 20:57:39.000000 nichord-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 22:07:16.635708 nichord-0.1.7/nichord/
--rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.1.7/nichord/__init__.py
--rw-rw-rw-   0        0        0    33895 2022-11-13 20:04:28.000000 nichord-0.1.7/nichord/chord.py
--rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.1.7/nichord/combine.py
--rw-rw-rw-   0        0        0      482 2022-05-22 13:31:30.000000 nichord-0.1.7/nichord/convert.py
--rw-rw-rw-   0        0        0     5639 2023-07-23 21:52:21.000000 nichord-0.1.7/nichord/coord_labeler.py
--rw-rw-rw-   0        0        0     5731 2022-11-12 03:52:39.000000 nichord-0.1.7/nichord/glassbrain.py
--rw-rw-rw-   0        0        0     1854 2022-05-16 00:16:25.000000 nichord-0.1.7/nichord/patch_RendererAgg.py
--rw-rw-rw-   0        0        0     8678 2023-07-23 21:52:21.000000 nichord-0.1.7/nichord/peak.py
-drwxrwxrwx   0        0        0        0 2023-07-23 22:07:16.638709 nichord-0.1.7/nichord.egg-info/
--rw-rw-rw-   0        0        0     1290 2023-07-23 22:07:16.000000 nichord-0.1.7/nichord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-07-23 22:07:16.000000 nichord-0.1.7/nichord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 22:07:16.000000 nichord-0.1.7/nichord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-23 22:07:16.000000 nichord-0.1.7/nichord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-23 22:07:16.000000 nichord-0.1.7/nichord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 22:07:16.640709 nichord-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1806 2023-07-23 22:07:09.000000 nichord-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:53:22.699819 nichord-0.1.8/
+-rw-rw-rw-   0        0        0     1290 2023-07-27 14:53:22.698818 nichord-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    10897 2023-07-23 20:57:39.000000 nichord-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 14:53:22.693817 nichord-0.1.8/nichord/
+-rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.1.8/nichord/__init__.py
+-rw-rw-rw-   0        0        0    33895 2022-11-13 20:04:28.000000 nichord-0.1.8/nichord/chord.py
+-rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.1.8/nichord/combine.py
+-rw-rw-rw-   0        0        0      482 2022-05-22 13:31:30.000000 nichord-0.1.8/nichord/convert.py
+-rw-rw-rw-   0        0        0     5639 2023-07-23 21:52:21.000000 nichord-0.1.8/nichord/coord_labeler.py
+-rw-rw-rw-   0        0        0     5731 2022-11-12 03:52:39.000000 nichord-0.1.8/nichord/glassbrain.py
+-rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.1.8/nichord/patch_RendererAgg.py
+-rw-rw-rw-   0        0        0     8678 2023-07-23 21:52:21.000000 nichord-0.1.8/nichord/peak.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:53:22.697818 nichord-0.1.8/nichord.egg-info/
+-rw-rw-rw-   0        0        0     1290 2023-07-27 14:53:22.000000 nichord-0.1.8/nichord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-07-27 14:53:22.000000 nichord-0.1.8/nichord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 14:53:22.000000 nichord-0.1.8/nichord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-27 14:53:22.000000 nichord-0.1.8/nichord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 14:53:22.000000 nichord-0.1.8/nichord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 14:53:22.699819 nichord-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1806 2023-07-27 14:51:12.000000 nichord-0.1.8/setup.py
```

### Comparing `nichord-0.1.7/PKG-INFO` & `nichord-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nichord
-Version: 0.1.7
+Version: 0.1.8
 Summary: Creates chord diagrams for connectivity/graph data
 Home-page: https://github.com/paulcbogdan/NiChord
 Author: paulcbogdan
 Author-email: paulcbogdan@gmail.com
 License: MIT
 Keywords: plotting,fmri,plotting,chord
 Platform: UNKNOWN
```

### Comparing `nichord-0.1.7/README.md` & `nichord-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nichord-0.1.7/nichord/__init__.py` & `nichord-0.1.8/nichord/__init__.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.7/nichord/chord.py` & `nichord-0.1.8/nichord/chord.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.7/nichord/combine.py` & `nichord-0.1.8/nichord/combine.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.7/nichord/coord_labeler.py` & `nichord-0.1.8/nichord/coord_labeler.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.7/nichord/glassbrain.py` & `nichord-0.1.8/nichord/glassbrain.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.7/nichord/patch_RendererAgg.py` & `nichord-0.1.8/nichord/patch_RendererAgg.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,24 @@
         #   I submitted a bug report to matplotlib, along with this solution.
         #   It has not been accepted yet, so for now I am "monkey patching" the
         #   function with this.
 
         if ismath:
             return self.draw_mathtext(gc, x, y, s, prop, angle)
 
+
         flags = backend_agg.get_hinting_flag()
-        font = self._get_agg_font(prop)
+
+        # matplotlib changed the name of one of its functions in version 3.6
+        matplotlib_v36 = callable(getattr(self, '_prepare_font', None))
+        if matplotlib_v36:
+            font = self._prepare_font(prop)
+        else:
+            font = self._get_agg_font(prop)
+
         if font is None:
             return None
         # [comment preserved from the original version of this function]
         # We pass '0' for angle here, since it will be rotated (in raster
         # space) in the following call to draw_text_image).
 
         font.set_text(s, 0, flags=flags)
@@ -39,7 +47,11 @@
         # y = round(y  + yd)
         self._renderer.draw_text_image(font, x, y + 1, angle, gc)
 
 
 def do_monkey_patch() -> None:
     backend_agg.RendererAgg = NeuoChordRenderAgg
 
+
+
+if __name__ == '__main__':
+    do_monkey_patch()
```

### Comparing `nichord-0.1.7/nichord/peak.py` & `nichord-0.1.8/nichord/peak.py`

 * *Files identical despite different names*

### Comparing `nichord-0.1.7/nichord.egg-info/PKG-INFO` & `nichord-0.1.8/nichord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nichord
-Version: 0.1.7
+Version: 0.1.8
 Summary: Creates chord diagrams for connectivity/graph data
 Home-page: https://github.com/paulcbogdan/NiChord
 Author: paulcbogdan
 Author-email: paulcbogdan@gmail.com
 License: MIT
 Keywords: plotting,fmri,plotting,chord
 Platform: UNKNOWN
```

### Comparing `nichord-0.1.7/setup.py` & `nichord-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 'To find out more about the package and see an example, see its [GitHub repo](https://github.com/paulcbogdan/NiChord).'
 
 setup(
     name="nichord",
     description="Creates chord diagrams for connectivity/graph data",
     long_description=desc,
     long_description_content_type="text/markdown",
-    version="v0.1.7",
+    version="v0.1.8",
     packages=["nichord"],
     python_requires=">=3.5",
     url="https://github.com/paulcbogdan/NiChord",
     author="paulcbogdan",
     author_email="paulcbogdan@gmail.com",
     install_requires=["nilearn",
                       "matplotlib",
```

