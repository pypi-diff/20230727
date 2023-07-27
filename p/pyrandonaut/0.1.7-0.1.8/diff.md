# Comparing `tmp/pyrandonaut-0.1.7.tar.gz` & `tmp/pyrandonaut-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrandonaut-0.1.7.tar", last modified: Thu Jul 27 04:53:04 2023, max compression
+gzip compressed data, was "pyrandonaut-0.1.8.tar", max compression
```

## Comparing `pyrandonaut-0.1.7.tar` & `pyrandonaut-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,5 @@
-drwx------   0 aesthese   (501) staff       (20)        0 2023-07-27 04:53:04.552708 pyrandonaut-0.1.7/
--rw-------   0 aesthese   (501) staff       (20)    35149 2023-07-27 03:48:57.000000 pyrandonaut-0.1.7/LICENSE
--rw-------   0 aesthese   (501) staff       (20)     7070 2023-07-27 04:53:04.552386 pyrandonaut-0.1.7/PKG-INFO
--rw-------   0 aesthese   (501) staff       (20)     6313 2023-07-27 03:49:58.000000 pyrandonaut-0.1.7/README.md
-drwx------   0 aesthese   (501) staff       (20)        0 2023-07-27 04:53:04.549298 pyrandonaut-0.1.7/pyrandonaut/
--rw-------   0 aesthese   (501) staff       (20)     7378 2023-07-27 04:48:00.000000 pyrandonaut-0.1.7/pyrandonaut/__init__.py
-drwx------   0 aesthese   (501) staff       (20)        0 2023-07-27 04:53:04.551955 pyrandonaut-0.1.7/pyrandonaut.egg-info/
--rw-------   0 aesthese   (501) staff       (20)     7070 2023-07-27 04:53:04.000000 pyrandonaut-0.1.7/pyrandonaut.egg-info/PKG-INFO
--rw-------   0 aesthese   (501) staff       (20)      224 2023-07-27 04:53:04.000000 pyrandonaut-0.1.7/pyrandonaut.egg-info/SOURCES.txt
--rw-------   0 aesthese   (501) staff       (20)        1 2023-07-27 04:53:04.000000 pyrandonaut-0.1.7/pyrandonaut.egg-info/dependency_links.txt
--rw-------   0 aesthese   (501) staff       (20)       84 2023-07-27 04:53:04.000000 pyrandonaut-0.1.7/pyrandonaut.egg-info/requires.txt
--rw-------   0 aesthese   (501) staff       (20)       12 2023-07-27 04:53:04.000000 pyrandonaut-0.1.7/pyrandonaut.egg-info/top_level.txt
--rw-------   0 aesthese   (501) staff       (20)       38 2023-07-27 04:53:04.552809 pyrandonaut-0.1.7/setup.cfg
--rw-------   0 aesthese   (501) staff       (20)     1579 2023-07-27 04:53:02.000000 pyrandonaut-0.1.7/setup.py
+-rw-r--r--   0        0        0    35149 2023-07-27 03:48:57.914723 pyrandonaut-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1100 2023-07-27 07:06:01.632882 pyrandonaut-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7397 2023-07-27 06:53:52.184754 pyrandonaut-0.1.8/pyrandonaut/__init__.py
+-rw-r--r--   0        0        0      840 2023-07-27 07:06:11.828038 pyrandonaut-0.1.8/setup.py
+-rw-r--r--   0        0        0     1068 2023-07-27 07:06:11.828647 pyrandonaut-0.1.8/PKG-INFO
```

### Comparing `pyrandonaut-0.1.7/LICENSE` & `pyrandonaut-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrandonaut-0.1.7/pyrandonaut/__init__.py` & `pyrandonaut-0.1.8/pyrandonaut/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 import numpy as np
 import pandas as pd
 import randonautentropy
 from scipy import stats
 
 __author__ = 'openrandonaut'
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 class Error(Exception):
     """Base class for other exceptions"""
 
 
 class DivisionError(Error):
     """Raised when number of requested point isn't divisible by 1024"""
@@ -218,11 +218,12 @@
     if args.points % 1024 != 0:
         parser.error("Argument POINTS must be divisible by 1024")
 
     coordinate = get_coordinate(args.latitude, args.longitude, args.radius, args.points)
 
     if not args.verbose:
         print(f"{coordinate[0]}, {coordinate[1]}")
-
+    
+    sys.exit()
 
 if __name__ == "__main__":
     main()
```

