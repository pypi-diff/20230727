# Comparing `tmp/AcrylicTK-0.0.1.tar.gz` & `tmp/AcrylicTK-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AcrylicTK-0.0.1.tar", last modified: Thu Jul 27 00:57:16 2023, max compression
+gzip compressed data, was "AcrylicTK-0.0.2.tar", last modified: Thu Jul 27 15:43:41 2023, max compression
```

## Comparing `AcrylicTK-0.0.1.tar` & `AcrylicTK-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 00:57:16.694047 AcrylicTK-0.0.1/
--rw-rw-rw-   0        0        0        4 2023-07-25 20:06:15.000000 AcrylicTK-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2905 2023-07-27 00:57:16.694047 AcrylicTK-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2312 2023-07-27 00:02:15.000000 AcrylicTK-0.0.1/README.md
--rw-rw-rw-   0        0        0      103 2023-07-26 23:03:55.000000 AcrylicTK-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-27 00:57:16.664033 AcrylicTK-0.0.1/scr/
-drwxrwxrwx   0        0        0        0 2023-07-27 00:57:16.675031 AcrylicTK-0.0.1/scr/AcrylicTK/
--rw-rw-rw-   0        0        0     4317 2023-07-26 23:54:41.000000 AcrylicTK-0.0.1/scr/AcrylicTK/AcrylicTK.py
--rw-rw-rw-   0        0        0        0 2023-07-25 19:57:23.000000 AcrylicTK-0.0.1/scr/AcrylicTK/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-07-25 19:55:20.000000 AcrylicTK-0.0.1/scr/AcrylicTK/blurWindow.py
-drwxrwxrwx   0        0        0        0 2023-07-27 00:57:16.692066 AcrylicTK-0.0.1/scr/AcrylicTK.egg-info/
--rw-rw-rw-   0        0        0     2905 2023-07-27 00:57:16.000000 AcrylicTK-0.0.1/scr/AcrylicTK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-07-27 00:57:16.000000 AcrylicTK-0.0.1/scr/AcrylicTK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 00:57:16.000000 AcrylicTK-0.0.1/scr/AcrylicTK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 00:57:16.000000 AcrylicTK-0.0.1/scr/AcrylicTK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-07-27 00:57:16.700031 AcrylicTK-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 15:43:41.855146 AcrylicTK-0.0.2/
+-rw-rw-rw-   0        0        0        4 2023-07-25 20:06:15.000000 AcrylicTK-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2905 2023-07-27 15:43:41.855146 AcrylicTK-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2312 2023-07-27 00:02:15.000000 AcrylicTK-0.0.2/README.md
+-rw-rw-rw-   0        0        0      121 2023-07-27 15:43:15.000000 AcrylicTK-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-27 15:43:41.823854 AcrylicTK-0.0.2/scr/
+drwxrwxrwx   0        0        0        0 2023-07-27 15:43:41.839477 AcrylicTK-0.0.2/scr/AcrylicTK/
+-rw-rw-rw-   0        0        0     4317 2023-07-27 15:41:23.000000 AcrylicTK-0.0.2/scr/AcrylicTK/AcrylicTK.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 19:57:23.000000 AcrylicTK-0.0.2/scr/AcrylicTK/__init__.py
+-rw-rw-rw-   0        0        0     6694 2023-07-25 19:55:20.000000 AcrylicTK-0.0.2/scr/AcrylicTK/blurWindow.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:43:41.855146 AcrylicTK-0.0.2/scr/AcrylicTK.egg-info/
+-rw-rw-rw-   0        0        0     2905 2023-07-27 15:43:41.000000 AcrylicTK-0.0.2/scr/AcrylicTK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-07-27 15:43:41.000000 AcrylicTK-0.0.2/scr/AcrylicTK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 15:43:41.000000 AcrylicTK-0.0.2/scr/AcrylicTK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 15:43:41.000000 AcrylicTK-0.0.2/scr/AcrylicTK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-07-27 15:43:41.870728 AcrylicTK-0.0.2/setup.cfg
```

### Comparing `AcrylicTK-0.0.1/PKG-INFO` & `AcrylicTK-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AcrylicTK
-Version: 0.0.1
+Version: 0.0.2
 Summary: Allows acrylic/transparent effect on tkinter
 Home-page: https://github.com
 Author: HumanDev2000
 Author-email: rewor78956@inkiny.com
 Project-URL: Bug Tracker, https://github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `AcrylicTK-0.0.1/README.md` & `AcrylicTK-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `AcrylicTK-0.0.1/scr/AcrylicTK/AcrylicTK.py` & `AcrylicTK-0.0.2/scr/AcrylicTK/AcrylicTK.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from tkinter import *
 from ctypes import windll
-from blurWindow import GlobalBlur
+from BlurWindow import GlobalBlur
 
 AppBG = None
 App = None
 acrylic = '#010101'
 
 
 class transparency:
```

### Comparing `AcrylicTK-0.0.1/scr/AcrylicTK/blurWindow.py` & `AcrylicTK-0.0.2/scr/AcrylicTK/blurWindow.py`

 * *Files identical despite different names*

### Comparing `AcrylicTK-0.0.1/scr/AcrylicTK.egg-info/PKG-INFO` & `AcrylicTK-0.0.2/scr/AcrylicTK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AcrylicTK
-Version: 0.0.1
+Version: 0.0.2
 Summary: Allows acrylic/transparent effect on tkinter
 Home-page: https://github.com
 Author: HumanDev2000
 Author-email: rewor78956@inkiny.com
 Project-URL: Bug Tracker, https://github.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `AcrylicTK-0.0.1/setup.cfg` & `AcrylicTK-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2041 6372 796c 6963 544b 0d0a 7665   = AcrylicTK..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 310d 0a61  rsion = 0.0.1..a
+00000020: 7273 696f 6e20 3d20 302e 302e 320d 0a61  rsion = 0.0.2..a
 00000030: 7574 686f 7220 3d20 4875 6d61 6e44 6576  uthor = HumanDev
 00000040: 3230 3030 0d0a 6175 7468 6f72 5f65 6d61  2000..author_ema
 00000050: 696c 203d 2072 6577 6f72 3738 3935 3640  il = rewor78956@
 00000060: 696e 6b69 6e79 2e63 6f6d 0d0a 6465 7363  inkiny.com..desc
 00000070: 7269 7074 696f 6e20 3d20 416c 6c6f 7773  ription = Allows
 00000080: 2061 6372 796c 6963 2f74 7261 6e73 7061   acrylic/transpa
 00000090: 7265 6e74 2065 6666 6563 7420 6f6e 2074  rent effect on t
```

