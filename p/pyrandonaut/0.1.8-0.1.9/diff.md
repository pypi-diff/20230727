# Comparing `tmp/pyrandonaut-0.1.8.tar.gz` & `tmp/pyrandonaut-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrandonaut-0.1.8.tar", max compression
+gzip compressed data, was "pyrandonaut-0.1.9.tar", max compression
```

## Comparing `pyrandonaut-0.1.8.tar` & `pyrandonaut-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-07-27 03:48:57.914723 pyrandonaut-0.1.8/LICENSE
--rw-r--r--   0        0        0     1100 2023-07-27 07:06:01.632882 pyrandonaut-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7397 2023-07-27 06:53:52.184754 pyrandonaut-0.1.8/pyrandonaut/__init__.py
--rw-r--r--   0        0        0      840 2023-07-27 07:06:11.828038 pyrandonaut-0.1.8/setup.py
--rw-r--r--   0        0        0     1068 2023-07-27 07:06:11.828647 pyrandonaut-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-27 03:48:57.914723 pyrandonaut-0.1.9/LICENSE
+-rw-r--r--   0        0        0     6313 2023-07-27 03:49:58.238521 pyrandonaut-0.1.9/README.md
+-rw-r--r--   0        0        0     1121 2023-07-27 07:12:06.853575 pyrandonaut-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     7397 2023-07-27 07:10:22.462612 pyrandonaut-0.1.9/pyrandonaut/__init__.py
+-rw-r--r--   0        0        0     7356 2023-07-27 07:12:22.451366 pyrandonaut-0.1.9/setup.py
+-rw-r--r--   0        0        0     7423 2023-07-27 07:12:22.451818 pyrandonaut-0.1.9/PKG-INFO
```

### Comparing `pyrandonaut-0.1.8/LICENSE` & `pyrandonaut-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrandonaut-0.1.8/pyproject.toml` & `pyrandonaut-0.1.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "pyrandonaut"
-version = "0.1.8"
+version = "0.1.9"
 description = "Open-source quantum random coordinate generation for randonauts <3"
 authors = ["alicemandragora <openrandonaut@riseup.net>"]
 license = "GPLv3"
+readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     'Topic :: System :: Installation/Setup',
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

### Comparing `pyrandonaut-0.1.8/pyrandonaut/__init__.py` & `pyrandonaut-0.1.9/pyrandonaut/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 import numpy as np
 import pandas as pd
 import randonautentropy
 from scipy import stats
 
 __author__ = 'openrandonaut'
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 class Error(Exception):
     """Base class for other exceptions"""
 
 
 class DivisionError(Error):
     """Raised when number of requested point isn't divisible by 1024"""
```

