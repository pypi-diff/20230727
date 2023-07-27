# Comparing `tmp/filelistener-1.0.3.tar.gz` & `tmp/filelistener-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filelistener-1.0.3.tar", last modified: Thu Jul 27 05:11:17 2023, max compression
+gzip compressed data, was "filelistener-1.0.4.tar", last modified: Thu Jul 27 05:18:31 2023, max compression
```

## Comparing `filelistener-1.0.3.tar` & `filelistener-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:11:17.906144 filelistener-1.0.3/
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:11:17.891856 filelistener-1.0.3/Content/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     8054 2023-07-27 05:02:56.000000 filelistener-1.0.3/Content/duplicate_content.py
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:11:17.895515 filelistener-1.0.3/Content/modules/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:10:47.000000 filelistener-1.0.3/Content/modules/__init__.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     1453 2023-07-27 05:09:32.000000 filelistener-1.0.3/Content/modules/duplicate_zip_files.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-27 05:11:17.903031 filelistener-1.0.3/PKG-INFO
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      500 2023-07-27 05:06:29.000000 filelistener-1.0.3/README.md
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:11:17.901993 filelistener-1.0.3/filelistener.egg-info/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-27 05:11:17.000000 filelistener-1.0.3/filelistener.egg-info/PKG-INFO
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      332 2023-07-27 05:11:17.000000 filelistener-1.0.3/filelistener.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        1 2023-07-27 05:11:17.000000 filelistener-1.0.3/filelistener.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       58 2023-07-27 05:11:17.000000 filelistener-1.0.3/filelistener.egg-info/entry_points.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        9 2023-07-27 05:11:17.000000 filelistener-1.0.3/filelistener.egg-info/requires.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        1 2023-07-27 05:11:17.000000 filelistener-1.0.3/filelistener.egg-info/top_level.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       38 2023-07-27 05:11:17.906459 filelistener-1.0.3/setup.cfg
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      496 2023-07-27 05:10:41.000000 filelistener-1.0.3/setup.py
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:18:31.969475 filelistener-1.0.4/
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:18:31.955230 filelistener-1.0.4/Content/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:15:38.000000 filelistener-1.0.4/Content/__init__.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     8054 2023-07-27 05:17:00.000000 filelistener-1.0.4/Content/duplicate_content.py
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:18:31.957521 filelistener-1.0.4/Content/modules/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:10:47.000000 filelistener-1.0.4/Content/modules/__init__.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     1453 2023-07-27 05:09:32.000000 filelistener-1.0.4/Content/modules/duplicate_zip_files.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-27 05:18:31.968565 filelistener-1.0.4/PKG-INFO
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      500 2023-07-27 05:06:29.000000 filelistener-1.0.4/README.md
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:18:31.966530 filelistener-1.0.4/filelistener.egg-info/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-27 05:18:31.000000 filelistener-1.0.4/filelistener.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      352 2023-07-27 05:18:31.000000 filelistener-1.0.4/filelistener.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        1 2023-07-27 05:18:31.000000 filelistener-1.0.4/filelistener.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       58 2023-07-27 05:18:31.000000 filelistener-1.0.4/filelistener.egg-info/entry_points.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        9 2023-07-27 05:18:31.000000 filelistener-1.0.4/filelistener.egg-info/requires.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        8 2023-07-27 05:18:31.000000 filelistener-1.0.4/filelistener.egg-info/top_level.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       38 2023-07-27 05:18:31.969721 filelistener-1.0.4/setup.cfg
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      496 2023-07-27 05:18:17.000000 filelistener-1.0.4/setup.py
```

### Comparing `filelistener-1.0.3/Content/duplicate_content.py` & `filelistener-1.0.4/Content/duplicate_content.py`

 * *Files identical despite different names*

### Comparing `filelistener-1.0.3/Content/modules/duplicate_zip_files.py` & `filelistener-1.0.4/Content/modules/duplicate_zip_files.py`

 * *Files identical despite different names*

