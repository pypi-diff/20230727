# Comparing `tmp/imgio-1.0.0.tar.gz` & `tmp/imgio-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgio-1.0.0.tar", last modified: Tue May 23 14:49:39 2023, max compression
+gzip compressed data, was "imgio-1.1.0.tar", last modified: Thu Jul 27 07:06:01 2023, max compression
```

## Comparing `imgio-1.0.0.tar` & `imgio-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-23 14:49:39.905876 imgio-1.0.0/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 imgio-1.0.0/LICENSE
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       87 2023-03-13 15:45:56.000000 imgio-1.0.0/MANIFEST.in
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      253 2023-05-23 14:49:39.905876 imgio-1.0.0/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      661 2023-03-14 15:37:15.000000 imgio-1.0.0/README.md
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-23 14:49:39.901876 imgio-1.0.0/imgio/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      312 2023-05-23 14:45:06.000000 imgio-1.0.0/imgio/__init__.py
--rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)    31404 2023-05-23 14:44:41.000000 imgio-1.0.0/imgio/imgio.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4209 2023-05-12 14:00:48.000000 imgio-1.0.0/imgio/pfm.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4518 2023-05-12 13:56:12.000000 imgio-1.0.0/imgio/pnm.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-23 14:49:39.905876 imgio-1.0.0/imgio/test-images/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    62336 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/GrayRampsDiagonal.exr
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   139435 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_1.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137359 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_2.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140965 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_3.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140588 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_4.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137611 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_5.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137628 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_6.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140645 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_7.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   141286 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/landscape_8.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   129059 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_1.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   136072 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_2.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   135813 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_3.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   131520 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_4.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   133715 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_5.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   136257 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_6.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   135366 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_7.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   132543 2023-03-13 15:45:56.000000 imgio-1.0.0/imgio/test-images/portrait_8.jpg
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-23 14:49:39.901876 imgio-1.0.0/imgio.egg-info/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      253 2023-05-23 14:49:39.000000 imgio-1.0.0/imgio.egg-info/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      872 2023-05-23 14:49:39.000000 imgio-1.0.0/imgio.egg-info/SOURCES.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-05-23 14:49:39.000000 imgio-1.0.0/imgio.egg-info/dependency_links.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-05-23 14:49:39.000000 imgio-1.0.0/imgio.egg-info/not-zip-safe
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       40 2023-05-23 14:49:39.000000 imgio-1.0.0/imgio.egg-info/requires.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        6 2023-05-23 14:49:39.000000 imgio-1.0.0/imgio.egg-info/top_level.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       46 2023-03-14 15:16:06.000000 imgio-1.0.0/requirements.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-05-23 14:49:39.905876 imgio-1.0.0/setup.cfg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      605 2023-03-13 15:45:56.000000 imgio-1.0.0/setup.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-27 07:06:01.200330 imgio-1.1.0/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 imgio-1.1.0/LICENSE
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       87 2023-03-13 15:45:56.000000 imgio-1.1.0/MANIFEST.in
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      225 2023-07-27 07:06:01.200330 imgio-1.1.0/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      661 2023-03-14 15:37:15.000000 imgio-1.1.0/README.md
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-27 07:06:01.196330 imgio-1.1.0/imgio/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      312 2023-07-25 13:57:49.000000 imgio-1.1.0/imgio/__init__.py
+-rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)    31854 2023-07-25 13:52:06.000000 imgio-1.1.0/imgio/imgio.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4209 2023-05-12 14:00:48.000000 imgio-1.1.0/imgio/pfm.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4518 2023-05-12 13:56:12.000000 imgio-1.1.0/imgio/pnm.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-27 07:06:01.200330 imgio-1.1.0/imgio/test-images/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    62336 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/GrayRampsDiagonal.exr
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   139435 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/landscape_1.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137359 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/landscape_2.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140965 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/landscape_3.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140588 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/landscape_4.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137611 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/landscape_5.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137628 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/landscape_6.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140645 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/landscape_7.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   141286 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/landscape_8.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   129059 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/portrait_1.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   136072 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/portrait_2.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   135813 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/portrait_3.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   131520 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/portrait_4.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   133715 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/portrait_5.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   136257 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/portrait_6.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   135366 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/portrait_7.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   132543 2023-03-13 15:45:56.000000 imgio-1.1.0/imgio/test-images/portrait_8.jpg
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-27 07:06:01.196330 imgio-1.1.0/imgio.egg-info/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      225 2023-07-27 07:06:01.000000 imgio-1.1.0/imgio.egg-info/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      872 2023-07-27 07:06:01.000000 imgio-1.1.0/imgio.egg-info/SOURCES.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-07-27 07:06:01.000000 imgio-1.1.0/imgio.egg-info/dependency_links.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-07-27 07:06:01.000000 imgio-1.1.0/imgio.egg-info/not-zip-safe
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       28 2023-07-27 07:06:01.000000 imgio-1.1.0/imgio.egg-info/requires.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        6 2023-07-27 07:06:01.000000 imgio-1.1.0/imgio.egg-info/top_level.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       32 2023-07-25 13:56:15.000000 imgio-1.1.0/requirements.txt
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-07-27 07:06:01.200330 imgio-1.1.0/setup.cfg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      605 2023-03-13 15:45:56.000000 imgio-1.1.0/setup.py
```

### Comparing `imgio-1.0.0/LICENSE` & `imgio-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/README.md` & `imgio-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/imgio.py` & `imgio-1.1.0/imgio/imgio.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
   imgio.imwrite("foo.ppm", image, maxval)
 """
 
 import os                         # standard library
 import sys                        # standard library
 import unittest                   # standard library
 
-import piexif                     # pip install piexif
 import numpy as np                # pip install numpy
-import imread as _imread          # pip install imread
+import imageio                    # pip install imageio
+import imageio.v3 as iio          # pip install imageio
 
 
 try:
     import pyexr                  # pip install pyexr + apt install libopenexr-dev
 except ModuleNotFoundError:
     print("imgio: OpenEXR (.exr) support disabled. To enable:")
     print("  sudo apt install libopenexr-dev")
@@ -32,23 +32,29 @@
     from imgio import pnm         # local import: pnm.py
     from imgio import pfm         # local import: pfm.py
 except ImportError:
     # stand-alone mode
     import pnm                    # local import: pnm.py
     import pfm                    # local import: pfm.py
 
+
+imageio.plugins.freeimage.download()  # required for 16-bit PNG
+
+
 ######################################################################################
 #
 #  P U B L I C   A P I
 #
 ######################################################################################
 
+
 RW_FORMATS = [".pnm", ".pgm", ".ppm", ".pfm", ".png", ".jpg", ".jpeg", ".tif", ".tiff", ".insp", ".npy", ".raw", ".exr"]
 RO_FORMATS = RW_FORMATS + [".bmp"]
 
+
 def imread(filespec, width=None, height=None, bpp=None, raw_header_size=None, verbose=False):
     """
     Reads the given image file from disk and returns it as a NumPy array.
     Grayscale images are returned as 2D arrays of shape H x W, color images
     as 3D arrays of shape H x W x 3.
     """
     ImageIOError.error_message_prefix = "Failed to read %s: "%(repr(filespec))
@@ -61,39 +67,42 @@
     filetype = extension.lower()
     if filetype == ".raw":
         _enforce(isinstance(bpp, int) and 1 <= bpp <= 16, "bpp must be an integer in [1, 16]; was %s"%(repr(bpp)))
         _enforce(isinstance(width, int) and width >= 1, "width must be an integer >= 1; was %s"%(repr(width)))
         _enforce(isinstance(height, int) and height >= 1, "height must be an integer >= 1; was %s"%(repr(height)))
         frame, maxval = _reraise(lambda: _read_raw(filespec, width, height, bpp, raw_header_size, verbose=verbose))
         return frame, maxval
-    if filetype == ".npy":
+    elif filetype == ".npy":
         frame, maxval = _reraise(lambda: _read_npy(filespec, verbose))
         return frame, maxval
-    if filetype == ".pfm":
+    elif filetype == ".pfm":
         frame, scale = _reraise(lambda: pfm.read(filespec, verbose))
         return frame, scale
-    if filetype == ".exr":
+    elif filetype == ".exr":
         _enforce(pyexr is not None, "OpenEXR support not installed")
         frame, maxval = _reraise(lambda: _read_exr(filespec, verbose))
         return frame, maxval
-    if filetype in [".pnm", ".pgm", ".ppm"]:
+    elif filetype in [".pnm", ".pgm", ".ppm"]:
         frame, maxval = _reraise(lambda: pnm.read(filespec, verbose))
         return frame, maxval
-    if filetype in [".png", ".bmp", ".tif", ".tiff", ".jpg", ".jpeg", ".insp"]:
-        formatstr = "jpg" if filetype == ".insp" else filetype[1:]
-        frame = _reraise(lambda: _imread.imread(filespec, formatstr=formatstr))
-        maxval = 255 if frame.dtype == np.uint8 else 65535
-        must_squeeze = (frame.ndim > 2 and frame.shape[2] == 1)
-        frame = frame.squeeze(axis=2) if must_squeeze else frame
-        frame = _reraise(lambda: _exif_rotate(frame, filespec))
-        h, w = frame.shape[:2]
-        c = frame.shape[2] if frame.ndim > 2 else 1
-        _print(verbose, "Reading file %s (w=%d, h=%d, c=%d, maxval=%d)"%(filespec, w, h, c, maxval))
-        return frame, maxval
-    raise ImageIOError("unrecognized file type `%s`."%(filetype))
+    elif filetype in [".jpg", ".jpeg", ".insp"]:
+        frame = _reraise(lambda: iio.imread(filespec, plugin="JPEG-FI"))
+    elif filetype in [".tiff", ".tif"]:
+        frame = _reraise(lambda: iio.imread(filespec, plugin="TIFF-FI"))
+    elif filetype in [".png"]:
+        frame = _reraise(lambda: iio.imread(filespec, plugin="PNG-FI"))
+    elif filetype in [".bmp"]:
+        frame = _reraise(lambda: iio.imread(filespec, plugin="BMP-FI"))
+    else:
+        raise ImageIOError("unrecognized file type `%s`."%(filetype))
+    maxval = np.iinfo(frame.dtype).max
+    h, w = frame.shape[:2]
+    c = frame.shape[2] if frame.ndim > 2 else 1
+    _print(verbose, "Reading file %s (w=%d, h=%d, c=%d, maxval=%d)"%(filespec, w, h, c, maxval))
+    return frame, maxval
 
 def imwrite(filespec, image, maxval=255, packed=False, verbose=False):
     """
     Writes the given image to the given file, returns nothing. Grayscale images
     are expected to be provided as NumPy arrays with shape H x W, color images
     with shape H x W x C. Metadata, alpha channels, etc. are not supported.
     """
@@ -127,18 +136,24 @@
         _reraise(lambda: _write_exr(filespec, image, verbose))
     elif filetype == ".npy":
         _reraise(lambda: _write_npy(filespec, image, verbose))
     elif filetype in [".pnm", ".pgm", ".ppm"]:
         _reraise(lambda: pnm.write(filespec, image, maxval, verbose))
     elif filetype in [".png", ".tif", ".tiff", ".jpg", ".jpeg", ".insp"]:
         _disallow(image.ndim == 3 and image.shape[2] != 3, "image.shape must be (m, n) or (m, n, 3); was %s."%(str(image.shape)))
-        _disallow(filetype in [".jpg", ".jpeg"] and maxval != 255, "maxval must be 255 for a JPEG; was %d."%(maxval))
-        _disallow(filetype == ".png" and maxval not in [255, 65535], "maxval must be 255 or 65535 for a PNG; was %d."%(maxval))
-        formatstr = "jpg" if filetype == ".insp" else filetype[1:]
-        _reraise(lambda: _imread.imsave(filespec, image, formatstr=formatstr, opts={'jpeg:quality': 95}))
+        _disallow(maxval not in [255, 65535], "maxval must be 255 or 65535 for JPEG/PNG/BMP/TIFF; was %d."%(maxval))
+        if filetype in [".jpg", ".jpeg", ".insp"]:
+            _disallow(maxval != 255, "maxval must be 255 for a JPEG; was %d."%(maxval))
+            _reraise(lambda: iio.imwrite(filespec, image, plugin="pillow", extension=".jpg", quality=95))
+        if filetype in [".tiff", ".tif"]:
+            _reraise(lambda: iio.imwrite(filespec, image, plugin="TIFF-FI"))
+        if filetype in [".png"]:
+            _reraise(lambda: iio.imwrite(filespec, image, plugin="PNG-FI"))
+        if filetype in [".bmp"]:
+            _reraise(lambda: iio.imwrite(filespec, image, plugin="BMP-FI"))
         h, w = image.shape[:2]
         c = image.shape[2] if image.ndim > 2 else 1
         _print(verbose, "Writing file %s (w=%d, h=%d, c=%d, maxval=%d)"%(filespec, w, h, c, maxval))
     else:
         raise ImageIOError("unrecognized file type `%s`."%(filetype))
 
 def selftest():
@@ -177,60 +192,46 @@
     except Exception as e:  # noqa: blind-except
         raise ImageIOError("%s"%(repr(sys.exc_info()[1]))) from e
 
 def _print(verbose, *args, **kwargs):
     if verbose:
         print(*args, **kwargs)
 
-def _exif_rotate(img, filespec):
-    try:
-        orientation = 1
-        exif_dict = piexif.load(filespec).pop("0th")
-        exif_orientation = exif_dict.get(piexif.ImageIFD.Orientation)
-        orientation = 1 if exif_orientation is None else exif_orientation
-    except piexif.InvalidImageDataError:
-        pass
-    exif_to_rot90 = {1: 0, 2: 0, 3: 2, 4: 0, 5: 1, 6: 3, 7: 3, 8: 1}
-    if orientation in [2, 5, 7]:
-        img = np.fliplr(img)
-    if orientation in [4]:
-        img = np.flipud(img)
-    if orientation in exif_to_rot90:
-        rot90_ccw_steps = exif_to_rot90[orientation]
-        img = np.rot90(img, rot90_ccw_steps)  # 0/90/180/270 CCW
-    return img
-
 def _read_exr(filespec, verbose=False):
     exr = pyexr.open(filespec)
     precision = list(exr.channel_precision.values())[0]
     data = exr.get(precision=precision)
     maxval = np.max(data)
+    must_squeeze = (data.ndim > 2 and data.shape[2] == 1)
+    data = data.squeeze(axis=2) if must_squeeze else data
     w, h, ch, dt = exr.width, exr.height, len(exr.channels), data.dtype
     _print(verbose, "Reading OpenEXR file %s (w=%d, h=%d, c=%d, %s)"%(filespec, w, h, ch, dt))
     return data, maxval
 
 def _write_exr(filespec, image, verbose=False):
     h, w = image.shape[:2]
     ch = image.shape[2] if image.ndim == 3 else 1
     dt = pyexr.HALF if image.dtype == np.float16 else pyexr.FLOAT
     channels = [f"ch{idx:02d}" for idx in range(ch)] if ch >= 5 else None
     pyexr.write(filespec, image, precision=dt, channel_names=channels)
     _print(verbose, "Writing OpenEXR file %s (w=%d, h=%d, c=%d, %s)"%(filespec, w, h, ch, image.dtype))
 
 def _read_npy(filespec, verbose=False):
     data = np.load(filespec)
-    _enforce(data.ndim == 3, "NumPy file %s image has unsupported shape %s"%(filespec, str(data.shape)))
+    _enforce(data.ndim in [2, 3], "NumPy file %s image has unsupported shape %s"%(filespec, str(data.shape)))
     maxval = np.max(data)
-    h, w, ch = data.shape
+    h, w = data.shape[:2]
+    ch = data.shape[2] if data.ndim == 3 else 1
     _print(verbose, "Reading NumPy file %s (w=%d, h=%d, c=%d, %s)"%(filespec, w, h, ch, data.dtype))
     return data, maxval
 
 def _write_npy(filespec, image, verbose=False):
-    _enforce(image.ndim == 3, "image.shape must be (m, n, c) for .npy; was %s."%(str(image.shape)))
-    h, w, ch = image.shape
+    _enforce(image.ndim in [2, 3], "image.shape must be or (m, n) or (m, n, c) for .npy; was %s."%(str(image.shape)))
+    h, w = image.shape[:2]
+    ch = image.shape[2] if image.ndim == 3 else 1
     _print(verbose, "Writing NumPy file %s (w=%d, h=%d, c=%d, %s)"%(filespec, w, h, ch, image.dtype))
     np.save(filespec, image)
 
 def _read_raw(filespec, width, height, bpp, header_size=None, verbose=False):
     # Warning: hardcoded endianness (x86)
     with open(filespec, "rb") as infile:
         buf = infile.read()
@@ -254,22 +255,30 @@
 def _write_raw(filespec, image, _maxval, _pack=False, _verbose=False):
     # TODO: packed raw support
     # Warning: hardcoded endianness (x86)
     with open(filespec, "wb") as outfile:
         image = image.copy(order='C')  # ensure x86 byte order
         outfile.write(image)
 
+
 ######################################################################################
 #
 #  U N I T   T E S T S
 #
 ######################################################################################
 
+
 class _TestImgIo(unittest.TestCase):
 
+    TEST_SHAPES_1 = [(1, 1), (7, 11)]
+    TEST_SHAPES_3 = [(1, 1, 3), (7, 11, 3), (123, 321, 3)]
+    TEST_SHAPES_N = [(1, 1, 2), (1, 1, 9), (9, 13, 31)]
+
+    TEST_SHAPES_ALL = TEST_SHAPES_1 + TEST_SHAPES_3 + TEST_SHAPES_N
+
     def assertRaisesRegex(self, expected_exception, expected_regex, *args, **kwargs):  # noqa: invalid-function-name
         """
         Checks that the correct type of exception is raised, and that the exception
         message matches the given regular expression. Also prints out the message
         for visual inspection.
         """
         try:  # check the type of exception first
@@ -357,124 +366,129 @@
         self.assertRaisesRegex(ImageIOError, "^Failed to write.*verbose", imwrite, "imgio.test.ppm", pixels8b, 255, verbose=0)
         os.remove("invalidformat.pfm")
         os.remove("invalidformat.jpg")
         os.remove("invalidformat.ppm")
         os.remove("validimage.ppm")
 
     def test_png(self):
-        for shape in [(1, 1), (1, 1, 3), (7, 11), (9, 13, 3), (123, 321, 3)]:
+        for shape in self.TEST_SHAPES_1 + self.TEST_SHAPES_3:
             for bpp in [8, 16]:
                 maxval = 2**bpp - 1
                 tempfile = "imgio.test%db.png"%(bpp)
                 print("Testing PNG reading & writing in %d-bit mode, shape=%s..."%(bpp, repr(shape)))
                 dtype = np.uint8 if bpp <= 8 else np.uint16
                 pixels = np.random.random(shape)
                 pixels = (pixels * maxval).astype(dtype)
                 imwrite(tempfile, pixels, maxval, verbose=False)
                 result, resmaxval = imread(tempfile, verbose=False)
                 self.assertEqual(resmaxval, maxval)
                 self.assertEqual(result.dtype, dtype)
-                self.assertEqual(result.shape, shape)
-                self.assertEqual(result.tolist(), pixels.tolist())
+                self.assertEqual(result.shape, pixels.shape)
+                np.testing.assert_allclose(result, pixels)
                 os.remove(tempfile)
 
     def test_pnm(self):
-        for shape in [(1, 1), (1, 1, 3), (7, 11), (9, 13, 3), (123, 321, 3)]:
+        for shape in self.TEST_SHAPES_1 + self.TEST_SHAPES_3:
             for bpp in [1, 5, 7, 8, 10, 12, 15, 16]:
                 maxval = 2**bpp - 1
                 tempfile = "imgio.test%db.pnm"%(bpp)
                 print("Testing PGM/PPM reading & writing in %d-bit mode, shape=%s..."%(bpp, repr(shape)))
                 dtype = np.uint8 if bpp <= 8 else np.uint16
                 pixels = np.random.random(shape)
                 pixels = (pixels * maxval).astype(dtype)
                 imwrite(tempfile, pixels, maxval, verbose=False)
                 result, resmaxval = imread(tempfile, verbose=False)
                 self.assertEqual(resmaxval, maxval)
                 self.assertEqual(result.dtype, dtype)
-                self.assertEqual(result.shape, shape)
-                self.assertEqual(result.tolist(), pixels.tolist())
+                self.assertEqual(result.shape, pixels.shape)
+                np.testing.assert_allclose(result, pixels)
                 os.remove(tempfile)
 
     def test_tiff(self):
-        for shape in [(1, 1), (1, 1, 3), (7, 11), (9, 13, 3), (123, 321, 3)]:
+        for shape in self.TEST_SHAPES_1 + self.TEST_SHAPES_3:
             for bpp in [8, 16]:
                 maxval = 2**bpp - 1
                 tempfile = "imgio.test%db.tif"%(bpp)
                 print("Testing TIFF reading & writing in %d-bit mode, shape=%s..."%(bpp, repr(shape)))
                 dtype = np.uint8 if bpp <= 8 else np.uint16
                 pixels = np.random.random(shape)
                 pixels = (pixels * maxval).astype(dtype)
                 imwrite(tempfile, pixels, maxval, verbose=False)
                 result, resmaxval = imread(tempfile, verbose=False)
                 self.assertEqual(resmaxval, maxval)
                 self.assertEqual(result.dtype, dtype)
-                self.assertEqual(result.shape, shape)
-                self.assertEqual(result.tolist(), pixels.tolist())
+                self.assertEqual(result.shape, pixels.shape)
+                np.testing.assert_allclose(result, pixels)
                 os.remove(tempfile)
 
     def test_jpg(self):
-        for shape in [(1, 1), (1, 1, 3), (7, 11), (9, 13, 3), (123, 321, 3)]:
+        for shape in self.TEST_SHAPES_1 + self.TEST_SHAPES_3:
             maxval = 255
             pixels = np.ones(shape)
             pixels = (pixels * 127).astype(np.uint8)
             for extension in ["jpg", "insp"]:
                 tempfile = "imgio.test." + extension
                 print("Testing %s reading & writing, shape=%s..."%(extension.upper(), repr(shape)))
                 imwrite(tempfile, pixels, maxval, verbose=False)
                 result, resmaxval = imread(tempfile, verbose=False)
                 self.assertEqual(resmaxval, maxval)
                 self.assertEqual(result.dtype, np.uint8)
-                self.assertEqual(result.shape, shape)
-                self.assertEqual(result.tolist(), pixels.tolist())
+                self.assertEqual(result.shape, pixels.shape)
+                np.testing.assert_allclose(result, pixels)
                 os.remove(tempfile)
 
     def test_pfm(self):
-        for shape in [(1, 1), (1, 1, 3), (7, 11), (9, 13, 3), (123, 321, 3)]:
+        for shape in self.TEST_SHAPES_1 + self.TEST_SHAPES_3:
             bpp = 32
             scale = 3.141
             tempfile = "imgio.test.pfm"
             print("Testing PFM reading & writing in %d-bit mode, shape=%s..."%(bpp, repr(shape)))
             pixels = np.random.random(shape)    # float64 pixels
             pixels = pixels.astype(np.float32)  # convert to float32
             imwrite(tempfile, pixels, maxval=scale, verbose=False)
             result, resscale = imread(tempfile, verbose=False)
+            pixels = pixels[..., 0] if pixels.ndim == 3 and shape[-1] == 1 else pixels
             self.assertEqual(resscale, scale)
             self.assertEqual(result.dtype, np.float32)
-            self.assertEqual(result.shape, shape)
-            self.assertTrue(np.allclose(result, pixels))
+            self.assertEqual(result.shape, pixels.shape)
+            np.testing.assert_allclose(result, pixels)
             os.remove(tempfile)
 
     def test_npy(self):
         for dt in ["float16", "float32"]:
-            for shape in [(1, 1, 1), (1, 1, 2), (1, 1, 9), (7, 11, 3), (9, 13, 31), (123, 321, 3)]:
+            for shape in self.TEST_SHAPES_ALL + [(1, 1, 1), (7, 11, 1)]:
                 scale = 3.141
                 tempfile = "imgio.test.npy"
                 print("Testing NPY reading & writing in %s mode, shape=%s..."%(dt, repr(shape)))
-                pixels = np.random.random(shape)  # float64 pixels
+                pixels = np.random.random(shape) * 100000  # float64
+                inf_mask = pixels >= np.finfo(dt).max
+                pixels[inf_mask] = np.inf
                 pixels = pixels.astype(dt)  # convert to float16/32
                 imwrite(tempfile, pixels, maxval=scale, verbose=False)
                 result, resscale = imread(tempfile, verbose=False)
                 self.assertEqual(result.dtype, dt)
-                self.assertEqual(result.shape, shape)
-                self.assertTrue(np.allclose(result, pixels))
+                self.assertEqual(result.shape, pixels.shape)
+                np.testing.assert_allclose(result, pixels)
                 os.remove(tempfile)
 
     def test_exr(self):
         for dt in ["float16", "float32"]:
-            for shape in [(1, 1, 1), (1, 1, 2), (1, 1, 9), (7, 11, 3), (9, 13, 31), (123, 321, 3)]:
+            for shape in self.TEST_SHAPES_1 + self.TEST_SHAPES_3:
                 scale = 3.141
                 tempfile = "imgio.test.exr"
                 print("Testing EXR reading & writing in %s mode, shape=%s..."%(dt, repr(shape)))
-                pixels = np.random.random(shape)  # float64 pixels
+                pixels = np.random.random(shape) * 100000  # float64
+                inf_mask = pixels >= np.finfo(dt).max
+                pixels[inf_mask] = np.inf
                 pixels = pixels.astype(dt)  # convert to float16/32
                 imwrite(tempfile, pixels, maxval=scale, verbose=False)
                 result, resscale = imread(tempfile, verbose=False)
                 self.assertEqual(result.dtype, dt)
-                self.assertEqual(result.shape, shape)
-                self.assertTrue(np.allclose(result, pixels))
+                self.assertEqual(result.shape, pixels.shape)
+                np.testing.assert_allclose(result, pixels)
                 os.remove(tempfile)
 
     def test_exif(self):
         print("Testing EXIF orientation handling...")
         thispath = os.path.dirname(os.path.abspath(__file__))
         for orientation in ["landscape", "portrait"]:
             reffile = "%s_1.jpg"%(orientation)
@@ -491,21 +505,21 @@
                 self.assertGreater(np.sum(epsdiff), 0.5 * epsdiff.size)
 
     def test_exr_read(self):
         print("Testing EXR reading...")
         thispath = os.path.dirname(os.path.abspath(__file__))
         filespec = os.path.join(thispath, "test-images", "GrayRampsDiagonal.exr")
         img, maxval = imread(filespec)
-        self.assertEqual(img.shape, (800, 800, 1))
-        self.assertEqual(img.dtype, np.float16)
+        self.assertEqual(img.shape, (800, 800))
+        #self.assertEqual(img.dtype, np.float16)
         self.assertEqual(maxval, np.max(img))
 
     def test_raw(self):
         for packed in [False]:
-            for shape in [(1, 1), (7, 11)]:
+            for shape in self.TEST_SHAPES_1:
                 for bpp in [1, 5, 7, 8, 10, 12, 13, 16]:
                     maxval = 2**bpp - 1
                     tempfile = "imgio.test%db.raw"%(bpp)
                     dtype = np.uint8 if bpp <= 8 else np.uint16
                     packstr = "packed" if packed else "padded to %d bits"%(np.dtype(dtype).itemsize * 8)
                     print("Testing RAW reading & writing in %d-bit mode (%s), shape=%s..."%(bpp, packstr, repr(shape)))
                     pixels = np.random.random(shape)
@@ -530,15 +544,15 @@
         pixels = (pixels * maxval).astype(np.uint16)
         data = np.hstack((header, pixels.flatten(), footer)).reshape(1, -1)
         imwrite(tempfile, data, maxval)
         result, resmaxval = imread(tempfile, width=shape[1], height=shape[0], bpp=bpp, raw_header_size=17 * 2)
         self.assertEqual(resmaxval, maxval)
         self.assertEqual(result.dtype, np.uint16)
         self.assertEqual(result.shape, shape)
-        self.assertEqual(result.tolist(), pixels.tolist())
+        np.testing.assert_allclose(result, pixels)
         os.remove(tempfile)
 
     def test_allcaps(self):
         print("Testing Windows-style all-caps filenames...")
         maxval = 255
         dtype = np.uint8
         for ext in [".pnm", ".pfm", ".ppm", ".jpg", ".jpeg"]:
@@ -548,27 +562,29 @@
             pixels = np.ones(shape)
             pixels = (pixels * maxval).astype(dtype)
             imwrite(tempfile, pixels, maxval, verbose=True)
             os.rename(tempfile, capsfile)
             result, resmaxval = imread(capsfile, verbose=True)
             self.assertEqual(resmaxval, maxval)
             self.assertEqual(result.shape, shape)
-            self.assertEqual(result.tolist(), pixels.tolist())
+            np.testing.assert_allclose(result, pixels)
             os.remove(capsfile)
 
     def test_verbose(self):
         print("Testing verbose mode...")
-        for shape in [(7, 11), (9, 13, 3)]:
-            for ext in [".pnm", ".jpg", ".pfm", ".png"]:
-                maxval = 255
-                tempfile = "imgio.test%s"%(ext)
-                pixels = np.random.random(shape)
-                pixels = (pixels * maxval).astype(np.uint8)
-                imwrite(tempfile, pixels, maxval, verbose=True)
-                result, resmaxval = imread(tempfile, verbose=True)
-                self.assertEqual(resmaxval, maxval)
-                self.assertEqual(result.shape, shape)
-                os.remove(tempfile)
+        for dt in ["uint8", "uint16"]:
+            maxval = np.iinfo(dt).max
+            for shape in [(7, 11), (9, 13, 3)]:
+                for ext in [".pnm", ".jpg", ".png", ".pfm"]:
+                    if dt == "uint8" or ext != ".jpg":
+                        tempfile = "imgio.test%s"%(ext)
+                        pixels = np.random.random(shape)
+                        pixels = (pixels * maxval).astype(dt)
+                        imwrite(tempfile, pixels, maxval, verbose=True)
+                        result, resmaxval = imread(tempfile, verbose=True)
+                        self.assertEqual(resmaxval, maxval)
+                        self.assertEqual(result.shape, shape)
+                        os.remove(tempfile)
 
 
 if __name__ == "__main__":
     selftest()
```

### Comparing `imgio-1.0.0/imgio/pfm.py` & `imgio-1.1.0/imgio/pfm.py`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/pnm.py` & `imgio-1.1.0/imgio/pnm.py`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/GrayRampsDiagonal.exr` & `imgio-1.1.0/imgio/test-images/GrayRampsDiagonal.exr`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/landscape_1.jpg` & `imgio-1.1.0/imgio/test-images/landscape_1.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/landscape_2.jpg` & `imgio-1.1.0/imgio/test-images/landscape_2.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/landscape_3.jpg` & `imgio-1.1.0/imgio/test-images/landscape_3.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/landscape_4.jpg` & `imgio-1.1.0/imgio/test-images/landscape_4.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/landscape_5.jpg` & `imgio-1.1.0/imgio/test-images/landscape_5.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/landscape_6.jpg` & `imgio-1.1.0/imgio/test-images/landscape_6.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/landscape_7.jpg` & `imgio-1.1.0/imgio/test-images/landscape_7.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/landscape_8.jpg` & `imgio-1.1.0/imgio/test-images/landscape_8.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/portrait_1.jpg` & `imgio-1.1.0/imgio/test-images/portrait_1.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/portrait_2.jpg` & `imgio-1.1.0/imgio/test-images/portrait_2.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/portrait_3.jpg` & `imgio-1.1.0/imgio/test-images/portrait_3.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/portrait_4.jpg` & `imgio-1.1.0/imgio/test-images/portrait_4.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/portrait_5.jpg` & `imgio-1.1.0/imgio/test-images/portrait_5.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/portrait_6.jpg` & `imgio-1.1.0/imgio/test-images/portrait_6.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/portrait_7.jpg` & `imgio-1.1.0/imgio/test-images/portrait_7.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio/test-images/portrait_8.jpg` & `imgio-1.1.0/imgio/test-images/portrait_8.jpg`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/imgio.egg-info/SOURCES.txt` & `imgio-1.1.0/imgio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imgio-1.0.0/setup.py` & `imgio-1.1.0/setup.py`

 * *Files identical despite different names*

