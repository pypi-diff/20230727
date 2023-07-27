# Comparing `tmp/snouty_viewer-0.2.4.tar.gz` & `tmp/snouty_viewer-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snouty_viewer-0.2.4.tar", last modified: Wed Jul 26 21:12:33 2023, max compression
+gzip compressed data, was "snouty_viewer-0.2.5.tar", last modified: Thu Jul 27 00:14:54 2023, max compression
```

## Comparing `snouty_viewer-0.2.4.tar` & `snouty_viewer-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 21:12:33.592950 snouty_viewer-0.2.4/
--rw-rw-rw-   0        0        0     1114 2022-08-03 18:36:50.000000 snouty_viewer-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      101 2022-08-03 18:36:50.000000 snouty_viewer-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6239 2023-07-26 21:12:33.592950 snouty_viewer-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     4954 2023-02-28 00:35:30.000000 snouty_viewer-0.2.4/README.md
--rw-rw-rw-   0        0        0      192 2022-08-03 18:36:50.000000 snouty_viewer-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0     1642 2023-07-26 21:12:33.592950 snouty_viewer-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 21:12:33.452350 snouty_viewer-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 21:12:33.483575 snouty_viewer-0.2.4/src/scripts/
--rw-rw-rw-   0        0        0        0 2023-07-25 21:56:56.000000 snouty_viewer-0.2.4/src/scripts/__init__.py
--rw-rw-rw-   0        0        0     2603 2023-07-26 21:07:56.000000 snouty_viewer-0.2.4/src/scripts/split_positions.py
-drwxrwxrwx   0        0        0        0 2023-07-26 21:12:33.514828 snouty_viewer-0.2.4/src/snouty_viewer/
--rw-rw-rw-   0        0        0      149 2023-03-01 19:34:57.000000 snouty_viewer-0.2.4/src/snouty_viewer/__init__.py
--rw-rw-rw-   0        0        0      357 2023-02-22 23:25:37.000000 snouty_viewer-0.2.4/src/snouty_viewer/_reader.py
-drwxrwxrwx   0        0        0        0 2023-07-26 21:12:33.592950 snouty_viewer-0.2.4/src/snouty_viewer/_tests/
--rw-rw-rw-   0        0        0        0 2022-08-03 18:36:50.000000 snouty_viewer-0.2.4/src/snouty_viewer/_tests/__init__.py
--rw-rw-rw-   0        0        0     8226 2022-08-31 22:44:42.000000 snouty_viewer-0.2.4/src/snouty_viewer/_tests/test_reader.py
--rw-rw-rw-   0        0        0     1286 2022-09-01 00:10:24.000000 snouty_viewer-0.2.4/src/snouty_viewer/_tests/test_widget.py
--rw-rw-rw-   0        0        0     9478 2023-07-26 21:07:44.000000 snouty_viewer-0.2.4/src/snouty_viewer/_widget.py
--rw-rw-rw-   0        0        0     1622 2023-02-28 00:28:17.000000 snouty_viewer-0.2.4/src/snouty_viewer/_writer.py
--rw-rw-rw-   0        0        0     5075 2023-07-26 20:26:02.000000 snouty_viewer-0.2.4/src/snouty_viewer/im_loader.py
--rw-rw-rw-   0        0        0     1408 2023-07-26 21:01:23.000000 snouty_viewer-0.2.4/src/snouty_viewer/napari.yaml
--rw-rw-rw-   0        0        0     6238 2023-07-25 21:54:24.000000 snouty_viewer-0.2.4/src/snouty_viewer/vol_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-26 21:12:33.577324 snouty_viewer-0.2.4/src/snouty_viewer.egg-info/
--rw-rw-rw-   0        0        0     6239 2023-07-26 21:12:33.000000 snouty_viewer-0.2.4/src/snouty_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      684 2023-07-26 21:12:33.000000 snouty_viewer-0.2.4/src/snouty_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 21:12:33.000000 snouty_viewer-0.2.4/src/snouty_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-26 21:12:33.000000 snouty_viewer-0.2.4/src/snouty_viewer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-07-26 21:12:33.000000 snouty_viewer-0.2.4/src/snouty_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-26 21:12:33.000000 snouty_viewer-0.2.4/src/snouty_viewer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 00:14:54.936074 snouty_viewer-0.2.5/
+-rw-rw-rw-   0        0        0     1114 2022-08-03 18:36:50.000000 snouty_viewer-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      101 2022-08-03 18:36:50.000000 snouty_viewer-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6239 2023-07-27 00:14:54.936074 snouty_viewer-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4954 2023-02-28 00:35:30.000000 snouty_viewer-0.2.5/README.md
+-rw-rw-rw-   0        0        0      192 2022-08-03 18:36:50.000000 snouty_viewer-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1642 2023-07-27 00:14:54.951698 snouty_viewer-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 00:14:54.794786 snouty_viewer-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 00:14:54.826037 snouty_viewer-0.2.5/src/scripts/
+-rw-rw-rw-   0        0        0        0 2023-07-25 21:56:56.000000 snouty_viewer-0.2.5/src/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2603 2023-07-26 21:07:56.000000 snouty_viewer-0.2.5/src/scripts/split_positions.py
+drwxrwxrwx   0        0        0        0 2023-07-27 00:14:54.857918 snouty_viewer-0.2.5/src/snouty_viewer/
+-rw-rw-rw-   0        0        0      149 2023-03-01 19:34:57.000000 snouty_viewer-0.2.5/src/snouty_viewer/__init__.py
+-rw-rw-rw-   0        0        0      357 2023-02-22 23:25:37.000000 snouty_viewer-0.2.5/src/snouty_viewer/_reader.py
+drwxrwxrwx   0        0        0        0 2023-07-27 00:14:54.936074 snouty_viewer-0.2.5/src/snouty_viewer/_tests/
+-rw-rw-rw-   0        0        0        0 2022-08-03 18:36:50.000000 snouty_viewer-0.2.5/src/snouty_viewer/_tests/__init__.py
+-rw-rw-rw-   0        0        0     8226 2022-08-31 22:44:42.000000 snouty_viewer-0.2.5/src/snouty_viewer/_tests/test_reader.py
+-rw-rw-rw-   0        0        0     1286 2022-09-01 00:10:24.000000 snouty_viewer-0.2.5/src/snouty_viewer/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    10214 2023-07-27 00:13:11.000000 snouty_viewer-0.2.5/src/snouty_viewer/_widget.py
+-rw-rw-rw-   0        0        0     1622 2023-02-28 00:28:17.000000 snouty_viewer-0.2.5/src/snouty_viewer/_writer.py
+-rw-rw-rw-   0        0        0     5265 2023-07-27 00:12:59.000000 snouty_viewer-0.2.5/src/snouty_viewer/im_loader.py
+-rw-rw-rw-   0        0        0     1408 2023-07-26 21:01:23.000000 snouty_viewer-0.2.5/src/snouty_viewer/napari.yaml
+-rw-rw-rw-   0        0        0     6238 2023-07-25 21:54:24.000000 snouty_viewer-0.2.5/src/snouty_viewer/vol_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-27 00:14:54.920449 snouty_viewer-0.2.5/src/snouty_viewer.egg-info/
+-rw-rw-rw-   0        0        0     6239 2023-07-27 00:14:54.000000 snouty_viewer-0.2.5/src/snouty_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2023-07-27 00:14:54.000000 snouty_viewer-0.2.5/src/snouty_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 00:14:54.000000 snouty_viewer-0.2.5/src/snouty_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-27 00:14:54.000000 snouty_viewer-0.2.5/src/snouty_viewer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-07-27 00:14:54.000000 snouty_viewer-0.2.5/src/snouty_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-27 00:14:54.000000 snouty_viewer-0.2.5/src/snouty_viewer.egg-info/top_level.txt
```

### Comparing `snouty_viewer-0.2.4/LICENSE` & `snouty_viewer-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.4/PKG-INFO` & `snouty_viewer-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snouty_viewer
-Version: 0.2.4
+Version: 0.2.5
 Summary: A plugin to visualize, deskew, and combine Snouty data.
 Home-page: https://github.com/aelefebv/snouty-viewer
 Author: Austin E. Y. T. Lefebvre
 Author-email: austin.e.lefebvre@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aelefebv/snouty-viewer/issues
 Project-URL: Documentation, https://github.com/aelefebv/snouty-viewer#README.md
```

### Comparing `snouty_viewer-0.2.4/README.md` & `snouty_viewer-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.4/setup.cfg` & `snouty_viewer-0.2.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6e6f 7574 795f 7669 6577 6572   = snouty_viewer
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 322e  ..version = 0.2.
-00000030: 340d 0a64 6573 6372 6970 7469 6f6e 203d  4..description =
+00000030: 350d 0a64 6573 6372 6970 7469 6f6e 203d  5..description =
 00000040: 2041 2070 6c75 6769 6e20 746f 2076 6973   A plugin to vis
 00000050: 7561 6c69 7a65 2c20 6465 736b 6577 2c20  ualize, deskew, 
 00000060: 616e 6420 636f 6d62 696e 6520 536e 6f75  and combine Snou
 00000070: 7479 2064 6174 612e 0d0a 6c6f 6e67 5f64  ty data...long_d
 00000080: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000090: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
 000000a0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
```

### Comparing `snouty_viewer-0.2.4/src/scripts/split_positions.py` & `snouty_viewer-0.2.5/src/scripts/split_positions.py`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.4/src/snouty_viewer/_tests/test_reader.py` & `snouty_viewer-0.2.5/src/snouty_viewer/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.4/src/snouty_viewer/_tests/test_widget.py` & `snouty_viewer-0.2.5/src/snouty_viewer/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.4/src/snouty_viewer/_widget.py` & `snouty_viewer-0.2.5/src/snouty_viewer/_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,28 +101,38 @@
     #     ome.images[0].description = description
     #     ome.images[0].pixels.type = dtype
     # note: numpy uses 8 bits as smallest, so 'bit' type does nothing for bool.
     #     ome_xml = ome.to_xml()
     #     tifffile.tiffcomment(path_im, ome_xml)
 
     def _deshear_channel(self, ch_num):
+        # there's probably a more pythonic way to go about this following DRY,
+        # but whatever, it works.
         if self.num_c == 1:
             desheard_ch = self.im_desheared
             for z in range(self.num_z):
                 deshear_shift = int(np.rint(z * self.scan_step_size_px))
                 desheard_ch[
                     :, z, deshear_shift : (deshear_shift + self.num_y), :
                 ] = self.data[:, z, :, :]
         else:
-            desheard_ch = self.im_desheared[:, ch_num, :, :, :]
-            for z in range(self.num_z):
-                deshear_shift = int(np.rint(z * self.scan_step_size_px))
-                desheard_ch[
-                    :, z, deshear_shift : (deshear_shift + self.num_y), :
-                ] = self.data[:, ch_num, z, :, :]
+            if self.num_t > 1:
+                desheard_ch = self.im_desheared[:, ch_num, :, :, :]
+                for z in range(self.num_z):
+                    deshear_shift = int(np.rint(z * self.scan_step_size_px))
+                    desheard_ch[
+                        :, z, deshear_shift : (deshear_shift + self.num_y), :
+                    ] = self.data[:, ch_num, z, :, :]
+            else:
+                desheard_ch = self.im_desheared[ch_num, :, :, :]
+                for z in range(self.num_z):
+                    deshear_shift = int(np.rint(z * self.scan_step_size_px))
+                    desheard_ch[
+                        z, deshear_shift : (deshear_shift + self.num_y), :
+                    ] = self.data[ch_num, z, :, :]
         return desheard_ch
 
     def _display_image(
         self, im, wavelength=0, color="gray", multichannel=False
     ):
         if multichannel:
             self.displayed_images.insert(
@@ -176,16 +186,20 @@
                 color = "bop orange"
             elif wavelength < 700:
                 color = "red"
             else:
                 color = "magenta"
             ch_desheared = self._deshear_channel(ch)
             if self.num_c > 1:
-                self.im_desheared[:, ch, ...] = ch_desheared[:, ...]
-                ch_desheared = ch_desheared[:, ...]
+                if self.num_t > 1:
+                    self.im_desheared[:, ch, ...] = ch_desheared[:, ...]
+                    ch_desheared = ch_desheared[:, ...]
+                else:
+                    self.im_desheared[ch, ...] = ch_desheared[:, ...]
+                    ch_desheared = ch_desheared[:, ...]
             else:
                 self.im_desheared = ch_desheared
             if not batch:
                 self._display_image(ch_desheared, wavelength, color)
 
         if (self.num_c > 1 and not batch) or show_multi:
             self._display_image(self.im_desheared, multichannel=True)
```

### Comparing `snouty_viewer-0.2.4/src/snouty_viewer/_writer.py` & `snouty_viewer-0.2.5/src/snouty_viewer/_writer.py`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.4/src/snouty_viewer/im_loader.py` & `snouty_viewer-0.2.5/src/snouty_viewer/im_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,20 @@
         im_path_info.im_shape,
         im_path_info.metadata,
         save_path,
         im_path_info.im_dtype,
     )
     for ch_num in range(im_path_info.num_channels):
         if im_path_info.num_channels > 1:
-            skewed_memmap[:, ch_num, ...] = load_channel(im_path_info, ch_num)
+            if im_path_info.num_volumes > 1:
+                skewed_memmap[:, ch_num, ...] = load_channel(
+                    im_path_info, ch_num
+                )
+            else:
+                skewed_memmap[ch_num, ...] = load_channel(im_path_info, ch_num)
             # ch_desheared = ch_desheared[:, ...]
         else:
             # self.im_desheared = ch_desheared
             skewed_memmap = load_channel(im_path_info, ch_num)
     px_size = float(im_path_info.metadata["sample_px_um"])
     z_px_size = px_size * float(im_path_info.metadata["voxel_aspect_ratio"])
     scale = (z_px_size, px_size, px_size)
```

### Comparing `snouty_viewer-0.2.4/src/snouty_viewer/napari.yaml` & `snouty_viewer-0.2.5/src/snouty_viewer/napari.yaml`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.4/src/snouty_viewer/vol_loader.py` & `snouty_viewer-0.2.5/src/snouty_viewer/vol_loader.py`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.4/src/snouty_viewer.egg-info/PKG-INFO` & `snouty_viewer-0.2.5/src/snouty_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snouty-viewer
-Version: 0.2.4
+Version: 0.2.5
 Summary: A plugin to visualize, deskew, and combine Snouty data.
 Home-page: https://github.com/aelefebv/snouty-viewer
 Author: Austin E. Y. T. Lefebvre
 Author-email: austin.e.lefebvre@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aelefebv/snouty-viewer/issues
 Project-URL: Documentation, https://github.com/aelefebv/snouty-viewer#README.md
```

### Comparing `snouty_viewer-0.2.4/src/snouty_viewer.egg-info/SOURCES.txt` & `snouty_viewer-0.2.5/src/snouty_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

