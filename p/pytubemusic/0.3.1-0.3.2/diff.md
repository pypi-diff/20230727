# Comparing `tmp/pytubemusic-0.3.1.tar.gz` & `tmp/pytubemusic-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubemusic-0.3.1.tar", last modified: Thu Jun 29 05:11:10 2023, max compression
+gzip compressed data, was "pytubemusic-0.3.2.tar", last modified: Thu Jul 27 00:26:34 2023, max compression
```

## Comparing `pytubemusic-0.3.1.tar` & `pytubemusic-0.3.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-29 05:11:10.598577 pytubemusic-0.3.1/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1075 2023-01-01 00:59:16.000000 pytubemusic-0.3.1/LICENSE
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5533 2023-06-29 05:11:10.598448 pytubemusic-0.3.1/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3826 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/README.md
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      858 2023-06-29 05:10:19.000000 pytubemusic-0.3.1/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-05-25 08:59:56.000000 pytubemusic-0.3.1/requirements.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-06-29 05:11:10.598617 pytubemusic-0.3.1/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-29 05:11:10.593527 pytubemusic-0.3.1/src/
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-29 05:11:10.594991 pytubemusic-0.3.1/src/pytubemusic/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-01-01 00:52:45.000000 pytubemusic-0.3.1/src/pytubemusic/__init__.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1721 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/__main__.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2431 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/audio.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3852 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/logutils.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5684 2023-06-29 05:07:56.000000 pytubemusic-0.3.1/src/pytubemusic/track.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3314 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/utils.py
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-29 05:11:10.596103 pytubemusic-0.3.1/src/pytubemusic/validation/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1354 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/__init__.py
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-29 05:11:10.596504 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      769 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/album.schema.json
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-29 05:11:10.597985 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      366 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/album_metadata.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      659 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/cover.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      307 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/end_timestamp.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      749 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/merge.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1455 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/playlist.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      220 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/playlist_url.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      746 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/split.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      311 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/start_timestamp.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      531 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/track.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      369 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/track_metadata.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      228 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/video_url.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      775 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/track.schema.json
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      638 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/src/pytubemusic/validation/schemata/type.schema.json
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-29 05:11:10.595952 pytubemusic-0.3.1/src/pytubemusic.egg-info/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5533 2023-06-29 05:11:10.000000 pytubemusic-0.3.1/src/pytubemusic.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1452 2023-06-29 05:11:10.000000 pytubemusic-0.3.1/src/pytubemusic.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-06-29 05:11:10.000000 pytubemusic-0.3.1/src/pytubemusic.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       53 2023-06-29 05:11:10.000000 pytubemusic-0.3.1/src/pytubemusic.egg-info/entry_points.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-06-29 05:11:10.000000 pytubemusic-0.3.1/src/pytubemusic.egg-info/requires.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       12 2023-06-29 05:11:10.000000 pytubemusic-0.3.1/src/pytubemusic.egg-info/top_level.txt
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-06-29 05:11:10.598271 pytubemusic-0.3.1/tests/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     8993 2023-06-29 04:49:28.000000 pytubemusic-0.3.1/tests/test_schemata.py
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1641 2023-02-14 00:54:23.000000 pytubemusic-0.3.1/tests/test_utils.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-07-27 00:26:34.381534 pytubemusic-0.3.2/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1075 2023-01-01 00:59:16.000000 pytubemusic-0.3.2/LICENSE
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5533 2023-07-27 00:26:34.381387 pytubemusic-0.3.2/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3826 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/README.md
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      858 2023-07-27 00:25:42.000000 pytubemusic-0.3.2/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-05-25 08:59:56.000000 pytubemusic-0.3.2/requirements.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-07-27 00:26:34.381575 pytubemusic-0.3.2/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-07-27 00:26:34.375109 pytubemusic-0.3.2/src/
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-07-27 00:26:34.377300 pytubemusic-0.3.2/src/pytubemusic/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-01-01 00:52:45.000000 pytubemusic-0.3.2/src/pytubemusic/__init__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1721 2023-06-30 04:08:30.000000 pytubemusic-0.3.2/src/pytubemusic/__main__.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2431 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/audio.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3704 2023-06-30 04:08:30.000000 pytubemusic-0.3.2/src/pytubemusic/logutils.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5684 2023-06-29 05:07:56.000000 pytubemusic-0.3.2/src/pytubemusic/track.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     3597 2023-07-27 00:18:34.000000 pytubemusic-0.3.2/src/pytubemusic/utils.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-07-27 00:26:34.378259 pytubemusic-0.3.2/src/pytubemusic/validation/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1354 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/__init__.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-07-27 00:26:34.378839 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      769 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/album.schema.json
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-07-27 00:26:34.380606 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      366 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/album_metadata.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      659 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/cover.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      307 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/end_timestamp.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      749 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/merge.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1455 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/playlist.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      220 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/playlist_url.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      746 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/split.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      311 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/start_timestamp.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      531 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/track.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      369 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/track_metadata.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      228 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/video_url.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      775 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/track.schema.json
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      638 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/src/pytubemusic/validation/schemata/type.schema.json
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-07-27 00:26:34.378125 pytubemusic-0.3.2/src/pytubemusic.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     5533 2023-07-27 00:26:34.000000 pytubemusic-0.3.2/src/pytubemusic.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1452 2023-07-27 00:26:34.000000 pytubemusic-0.3.2/src/pytubemusic.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-07-27 00:26:34.000000 pytubemusic-0.3.2/src/pytubemusic.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       53 2023-07-27 00:26:34.000000 pytubemusic-0.3.2/src/pytubemusic.egg-info/entry_points.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      132 2023-07-27 00:26:34.000000 pytubemusic-0.3.2/src/pytubemusic.egg-info/requires.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       12 2023-07-27 00:26:34.000000 pytubemusic-0.3.2/src/pytubemusic.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-07-27 00:26:34.381002 pytubemusic-0.3.2/tests/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     8993 2023-06-29 04:49:28.000000 pytubemusic-0.3.2/tests/test_schemata.py
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1641 2023-02-14 00:54:23.000000 pytubemusic-0.3.2/tests/test_utils.py
```

### Comparing `pytubemusic-0.3.1/LICENSE` & `pytubemusic-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/PKG-INFO` & `pytubemusic-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubemusic
-Version: 0.3.1
+Version: 0.3.2
 Summary: A cli that may or may not download albums from a certain website
 License: MIT License
         
         Copyright (c) 2023 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pytubemusic-0.3.1/README.md` & `pytubemusic-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/pyproject.toml` & `pytubemusic-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubemusic"
-version = "0.3.1"
+version = "0.3.2"
 description = 'A cli that may or may not download albums from a certain website'
 
 readme = "README.md"
 requires-python = ">=3.11"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `pytubemusic-0.3.1/src/pytubemusic/__main__.py` & `pytubemusic-0.3.2/src/pytubemusic/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from collections.abc import Mapping
 from pathlib import Path
 
 import cowexcept
 from typer import Argument, Option, Typer
 
-from .logutils import log_block, log_call, open_or_panic
+from .logutils import log_block, log_call
 from .track import Track
-from .utils import get_cover
+from .utils import get_cover, open_or_panic
 from .validation import loadf_or_panic
 
 app = Typer(add_completion=False)
 
 logger = logging.getLogger("pytubemusic")
 logger.setLevel(logging.INFO)
 logger.addHandler(logging.StreamHandler())
```

### Comparing `pytubemusic-0.3.1/src/pytubemusic/audio.py` & `pytubemusic-0.3.2/src/pytubemusic/audio.py`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/src/pytubemusic/logutils.py` & `pytubemusic-0.3.2/src/pytubemusic/logutils.py`

 * *Files 12% similar despite different names*

```diff
@@ -109,20 +109,14 @@
 
 def log_message(msg, fmt_args, fmt_kwargs, level):
     if msg is not None:
         msg = indent(msg, " " * _INDENT).format(*fmt_args, **fmt_kwargs)
         logger.log(level, msg)
 
 
-@contextlib.contextmanager
-def open_or_panic(file_name, mode, msg):
-    with (PanicOn(OSError, msg), open(file_name, mode) as f):
-        yield f
-
-
 def log_iter(
         level=logging.INFO,
         on_each: str = None,
         on_enter: str = None,
         on_exit: str = None,
         start: int = 0,
 ):
```

### Comparing `pytubemusic-0.3.1/src/pytubemusic/track.py` & `pytubemusic-0.3.2/src/pytubemusic/track.py`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/src/pytubemusic/utils.py` & `pytubemusic-0.3.2/src/pytubemusic/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import contextlib
 import urllib.request
 from collections.abc import Iterable, Mapping
 from datetime import datetime, timedelta
 from itertools import chain, pairwise
 from pathlib import Path, PurePath
 from tempfile import NamedTemporaryFile
 from typing import Any
 
+from pytubemusic.logutils import PanicOn
+
 __all__ = [
     "to_delta", "to_timestamp", "to_microseconds", "pathify",
     "set_ends", "merge_metadata", "get_cover", "pad", "File", "TrackData",
-    "StrMap",
+    "StrMap", "open_or_panic",
 ]
 
 StrMap = Mapping[str, Any]
 TrackData = Iterable[StrMap]
 
 File = NamedTemporaryFile
 
@@ -87,20 +90,27 @@
         case {"url": url}:
             f = NamedTemporaryFile(suffix='.jpg')
             img = urllib.request.urlopen(url).read()
             f.write(img)
             return f
         case {"file": path}:
             tmp = NamedTemporaryFile(suffix='.jpg')
-            with open(relative_to.parent / path, "rb") as f:
+            msg = f"Cannot find cover file"
+            with open_or_panic(relative_to.parent / path, "rb", msg) as f:
                 tmp.write(f.read())
             return tmp
         case None:
             return None
         case _:
             raise ValueError(f"Unrecognised Cover format: `{cover}`")
 
 
 def pad(tracks, factory, length):
     tracks = list(tracks)
     tracks += [factory() for _ in range(length - len(tracks))]
     return tracks
+
+
+@contextlib.contextmanager
+def open_or_panic(file_name, mode, msg):
+    with (PanicOn(OSError, msg), open(file_name, mode) as f):
+        yield f
```

### Comparing `pytubemusic-0.3.1/src/pytubemusic/validation/__init__.py` & `pytubemusic-0.3.2/src/pytubemusic/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/src/pytubemusic/validation/schemata/album.schema.json` & `pytubemusic-0.3.2/src/pytubemusic/validation/schemata/album.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/cover.schema.json` & `pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/cover.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/merge.schema.json` & `pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/merge.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/playlist.schema.json` & `pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/playlist.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/split.schema.json` & `pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/split.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/src/pytubemusic/validation/schemata/components/track.schema.json` & `pytubemusic-0.3.2/src/pytubemusic/validation/schemata/components/track.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/src/pytubemusic/validation/schemata/track.schema.json` & `pytubemusic-0.3.2/src/pytubemusic/validation/schemata/track.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/src/pytubemusic/validation/schemata/type.schema.json` & `pytubemusic-0.3.2/src/pytubemusic/validation/schemata/type.schema.json`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/src/pytubemusic.egg-info/PKG-INFO` & `pytubemusic-0.3.2/src/pytubemusic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubemusic
-Version: 0.3.1
+Version: 0.3.2
 Summary: A cli that may or may not download albums from a certain website
 License: MIT License
         
         Copyright (c) 2023 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pytubemusic-0.3.1/src/pytubemusic.egg-info/SOURCES.txt` & `pytubemusic-0.3.2/src/pytubemusic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/tests/test_schemata.py` & `pytubemusic-0.3.2/tests/test_schemata.py`

 * *Files identical despite different names*

### Comparing `pytubemusic-0.3.1/tests/test_utils.py` & `pytubemusic-0.3.2/tests/test_utils.py`

 * *Files identical despite different names*

