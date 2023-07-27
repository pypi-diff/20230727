# Comparing `tmp/filelistener-1.0.4.tar.gz` & `tmp/filelistener-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filelistener-1.0.4.tar", last modified: Thu Jul 27 05:18:31 2023, max compression
+gzip compressed data, was "filelistener-1.0.5.tar", last modified: Thu Jul 27 05:20:29 2023, max compression
```

## Comparing `filelistener-1.0.4.tar` & `filelistener-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:18:31.969475 filelistener-1.0.4/
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:18:31.955230 filelistener-1.0.4/Content/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:15:38.000000 filelistener-1.0.4/Content/__init__.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     8054 2023-07-27 05:17:00.000000 filelistener-1.0.4/Content/duplicate_content.py
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:18:31.957521 filelistener-1.0.4/Content/modules/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:10:47.000000 filelistener-1.0.4/Content/modules/__init__.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     1453 2023-07-27 05:09:32.000000 filelistener-1.0.4/Content/modules/duplicate_zip_files.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-27 05:18:31.968565 filelistener-1.0.4/PKG-INFO
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      500 2023-07-27 05:06:29.000000 filelistener-1.0.4/README.md
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:18:31.966530 filelistener-1.0.4/filelistener.egg-info/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-27 05:18:31.000000 filelistener-1.0.4/filelistener.egg-info/PKG-INFO
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      352 2023-07-27 05:18:31.000000 filelistener-1.0.4/filelistener.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        1 2023-07-27 05:18:31.000000 filelistener-1.0.4/filelistener.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       58 2023-07-27 05:18:31.000000 filelistener-1.0.4/filelistener.egg-info/entry_points.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        9 2023-07-27 05:18:31.000000 filelistener-1.0.4/filelistener.egg-info/requires.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        8 2023-07-27 05:18:31.000000 filelistener-1.0.4/filelistener.egg-info/top_level.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       38 2023-07-27 05:18:31.969721 filelistener-1.0.4/setup.cfg
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      496 2023-07-27 05:18:17.000000 filelistener-1.0.4/setup.py
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:20:29.057536 filelistener-1.0.5/
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:20:29.009939 filelistener-1.0.5/Content/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:15:38.000000 filelistener-1.0.5/Content/__init__.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     8062 2023-07-27 05:20:10.000000 filelistener-1.0.5/Content/duplicate_content.py
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:20:29.016118 filelistener-1.0.5/Content/modules/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:10:47.000000 filelistener-1.0.5/Content/modules/__init__.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     1453 2023-07-27 05:09:32.000000 filelistener-1.0.5/Content/modules/duplicate_zip_files.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-27 05:20:29.056204 filelistener-1.0.5/PKG-INFO
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      500 2023-07-27 05:06:29.000000 filelistener-1.0.5/README.md
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:20:29.055128 filelistener-1.0.5/filelistener.egg-info/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-27 05:20:28.000000 filelistener-1.0.5/filelistener.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      352 2023-07-27 05:20:28.000000 filelistener-1.0.5/filelistener.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        1 2023-07-27 05:20:28.000000 filelistener-1.0.5/filelistener.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       58 2023-07-27 05:20:28.000000 filelistener-1.0.5/filelistener.egg-info/entry_points.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        9 2023-07-27 05:20:28.000000 filelistener-1.0.5/filelistener.egg-info/requires.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        8 2023-07-27 05:20:28.000000 filelistener-1.0.5/filelistener.egg-info/top_level.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       38 2023-07-27 05:20:29.057774 filelistener-1.0.5/setup.cfg
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      496 2023-07-27 05:20:25.000000 filelistener-1.0.5/setup.py
```

### Comparing `filelistener-1.0.4/Content/duplicate_content.py` & `filelistener-1.0.5/Content/duplicate_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import argparse
 import platform
 import subprocess
 from collections import defaultdict
-from modules.duplicate_zip_files import check_single_zip_for_duplicates
+from Content.modules.duplicate_zip_files import check_single_zip_for_duplicates
 
 
 def get_file_hash(file_path):
     """Calculate the MD5 hash of a file.
 
     Args:
         file_path (str): The path to the file.
```

### Comparing `filelistener-1.0.4/Content/modules/duplicate_zip_files.py` & `filelistener-1.0.5/Content/modules/duplicate_zip_files.py`

 * *Files identical despite different names*

