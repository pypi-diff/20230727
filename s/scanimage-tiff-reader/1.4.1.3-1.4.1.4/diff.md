# Comparing `tmp/scanimage-tiff-reader-1.4.1.3.tar.gz` & `tmp/scanimage-tiff-reader-1.4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Gitlab\scanimagetiffreader-python\dist\.tmp-i325r66q\scanimage-tiff-reader-1.4.1.3.tar", last modified: Tue May 30 14:58:52 2023, max compression
+gzip compressed data, was "C:\git\scanimagetiffreader-python\dist\.tmp-bygh1w3z\scanimage-tiff-reader-1.4.1.4.tar", last modified: Thu Jul 27 21:19:41 2023, max compression
```

## Comparing `scanimage-tiff-reader-1.4.1.3.tar` & `scanimage-tiff-reader-1.4.1.4.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/
--rw-rw-rw-   0        0        0      570 2023-05-16 20:53:57.000000 scanimage-tiff-reader-1.4.1.3/LICENSE
--rw-rw-rw-   0        0        0      119 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3779 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2076 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/README.rst
--rw-rw-rw-   0        0        0     1330 2023-05-19 19:23:47.000000 scanimage-tiff-reader-1.4.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/setup.cfg
--rw-rw-rw-   0        0        0       69 2023-05-19 18:45:13.000000 scanimage-tiff-reader-1.4.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/
--rw-rw-rw-   0        0        0    13401 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/
--rw-rw-rw-   0        0        0      708 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/
-drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/
--rw-rw-rw-   0        0        0   379788 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/libScanImageTiffReaderAPI.so
-drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/
-drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/
--rw-rw-rw-   0        0        0  2409728 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/libScanImageTiffReaderAPI.so
-drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/
-drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/
--rw-rw-rw-   0        0        0   538112 2023-05-10 16:52:16.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/ScanImageTiffReaderAPI.dll
--rw-rw-rw-   0        0        0      919 2023-05-10 16:52:17.000000 scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/
--rw-rw-rw-   0        0        0     3779 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      767 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-30 14:58:52.000000 scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/
+-rw-rw-rw-   0        0        0      570 2023-07-27 21:08:29.000000 scanimage-tiff-reader-1.4.1.4/LICENSE
+-rw-rw-rw-   0        0        0      119 2023-07-27 21:08:29.000000 scanimage-tiff-reader-1.4.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3779 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2076 2023-07-27 21:08:29.000000 scanimage-tiff-reader-1.4.1.4/README.rst
+-rw-rw-rw-   0        0        0     1330 2023-07-27 21:12:30.000000 scanimage-tiff-reader-1.4.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/setup.cfg
+-rw-rw-rw-   0        0        0       69 2023-07-27 21:08:29.000000 scanimage-tiff-reader-1.4.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/
+-rw-rw-rw-   0        0        0    13401 2023-07-27 21:08:29.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/
+-rw-rw-rw-   0        0        0      708 2023-07-27 21:08:29.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/
+-rw-rw-rw-   0        0        0   379788 2023-07-27 21:08:29.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/libScanImageTiffReaderAPI.so
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin-arm64/
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin-arm64/lib/
+-rw-rw-rw-   0        0        0   645241 2023-07-27 21:08:29.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin-arm64/lib/libScanImageTiffReaderAPI.so
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/
+-rw-rw-rw-   0        0        0  2409728 2023-07-27 21:08:29.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/libScanImageTiffReaderAPI.so
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/
+-rw-rw-rw-   0        0        0   538112 2023-07-27 21:08:29.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/ScanImageTiffReaderAPI.dll
+-rw-rw-rw-   0        0        0     1190 2023-07-27 21:08:29.000000 scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/scanimage_tiff_reader.egg-info/
+-rw-rw-rw-   0        0        0     3779 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/scanimage_tiff_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      872 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/scanimage_tiff_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/scanimage_tiff_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/scanimage_tiff_reader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/scanimage_tiff_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-27 21:19:41.000000 scanimage-tiff-reader-1.4.1.4/src/scanimage_tiff_reader.egg-info/top_level.txt
```

### Comparing `scanimage-tiff-reader-1.4.1.3/LICENSE` & `scanimage-tiff-reader-1.4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1.3/PKG-INFO` & `scanimage-tiff-reader-1.4.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanimage-tiff-reader
-Version: 1.4.1.3
+Version: 1.4.1.4
 Summary: A fast (big)tiff reader that provides access to ScanImage-specific metadata.
 Author: Nathan Clack
 Maintainer-email: Lawrence Niu <lawrence@mbfbioscience.com>, Nelson Downs <nelson@mbfbioscience.com>, MBF Support <support@mbfbioscience.com>
 License: Copyright (C) 2023 MBF Bioscience
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `scanimage-tiff-reader-1.4.1.3/README.rst` & `scanimage-tiff-reader-1.4.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1.3/pyproject.toml` & `scanimage-tiff-reader-1.4.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scanimage-tiff-reader"
-version = "1.4.1.3"
+version = "1.4.1.4"
 description = "A fast (big)tiff reader that provides access to ScanImage-specific metadata."
 readme = "README.rst"
 license = {file = "LICENSE"}
 authors = [
     {name = "Nathan Clack"},
 ]
 requires-python = ">=3.7"
```

### Comparing `scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/__init__.py` & `scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/__init__.py`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/README.md` & `scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/README.md`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/libScanImageTiffReaderAPI.so` & `scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/libScanImageTiffReaderAPI.so`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/libScanImageTiffReaderAPI.so` & `scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/libScanImageTiffReaderAPI.so`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/ScanImageTiffReaderAPI.dll` & `scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/ScanImageTiffReaderAPI.dll`

 * *Files identical despite different names*

### Comparing `scanimage-tiff-reader-1.4.1.3/src/ScanImageTiffReader/external/__init__.py` & `scanimage-tiff-reader-1.4.1.4/src/ScanImageTiffReader/external/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """ Defines paths to binary resource derived with provenance external to this
 code.  This is also used in `setup.py`.
 """
 
 _registry={
-    'Windows': {'location':'ScanImageTiffReader-1.4.1-win64',  'name':"ScanImageTiffReaderAPI.dll"},      
-    'Darwin' : {'location':'ScanImageTiffReader-1.4.1-Darwin', 'name':"libScanImageTiffReaderAPI.so"},         
-    'Linux'  : {'location':'ScanImageTiffReader-1.4.1-Linux',  'name':"libScanImageTiffReaderAPI.so"},     
+    'Windows'      : {'location':'ScanImageTiffReader-1.4.1-win64',  'name':"ScanImageTiffReaderAPI.dll"},
+    'Darwin'       : {'location':'ScanImageTiffReader-1.4.1-Darwin', 'name':"libScanImageTiffReaderAPI.so"},
+    'Darwin-arm64' : {'location':'ScanImageTiffReader-1.4.1-Darwin-arm64', 'name':"libScanImageTiffReaderAPI.so"},
+    'Linux'        : {'location':'ScanImageTiffReader-1.4.1-Linux',  'name':"libScanImageTiffReaderAPI.so"},
 }
 
 def resource_path():
     """ Returns an absolute path to a shared library with the ScanImageTiffReaderAPI.
     """
     from os.path import (abspath,join,dirname)
     import platform
     # Lookup based on platform string.
     # If the platform string isn't matched, we'll use Linux as a fallback.
-    info=_registry.get(platform.system(),_registry['Linux'])
+    if platform.system() == 'Darwin' and platform.machine() == 'arm64':
+        # Apple Silicon
+        info=_registry.get('Darwin-arm64')
+    else:
+        info=_registry.get(platform.system(),_registry['Linux'])
     return join(dirname(abspath(__file__)),info["location"],'lib',info["name"])
```

### Comparing `scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/PKG-INFO` & `scanimage-tiff-reader-1.4.1.4/src/scanimage_tiff_reader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanimage-tiff-reader
-Version: 1.4.1.3
+Version: 1.4.1.4
 Summary: A fast (big)tiff reader that provides access to ScanImage-specific metadata.
 Author: Nathan Clack
 Maintainer-email: Lawrence Niu <lawrence@mbfbioscience.com>, Nelson Downs <nelson@mbfbioscience.com>, MBF Support <support@mbfbioscience.com>
 License: Copyright (C) 2023 MBF Bioscience
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `scanimage-tiff-reader-1.4.1.3/src/scanimage_tiff_reader.egg-info/SOURCES.txt` & `scanimage-tiff-reader-1.4.1.4/src/scanimage_tiff_reader.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.py
 src/ScanImageTiffReader/__init__.py
 src/ScanImageTiffReader/external/README.md
 src/ScanImageTiffReader/external/__init__.py
+src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin-arm64/lib/libScanImageTiffReaderAPI.so
 src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Darwin/lib/libScanImageTiffReaderAPI.so
 src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-Linux/lib/libScanImageTiffReaderAPI.so
 src/ScanImageTiffReader/external/ScanImageTiffReader-1.4.1-win64/lib/ScanImageTiffReaderAPI.dll
 src/scanimage_tiff_reader.egg-info/PKG-INFO
 src/scanimage_tiff_reader.egg-info/SOURCES.txt
 src/scanimage_tiff_reader.egg-info/dependency_links.txt
 src/scanimage_tiff_reader.egg-info/entry_points.txt
```

