# Comparing `tmp/wyoming_faster_whisper-1.0.0.tar.gz` & `tmp/wyoming_faster_whisper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyoming_faster_whisper-1.0.0.tar", last modified: Thu Jul 27 16:40:34 2023, max compression
+gzip compressed data, was "wyoming_faster_whisper-1.0.1.tar", last modified: Thu Jul 27 16:55:50 2023, max compression
```

## Comparing `wyoming_faster_whisper-1.0.0.tar` & `wyoming_faster_whisper-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-27 16:40:34.217911 wyoming_faster_whisper-1.0.0/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.0/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-07-27 16:40:34.217911 wyoming_faster_whisper-1.0.0/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       56 2023-07-27 16:07:23.000000 wyoming_faster_whisper-1.0.0/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-27 16:40:34.217911 wyoming_faster_whisper-1.0.0/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1225 2023-07-27 16:05:58.000000 wyoming_faster_whisper-1.0.0/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-27 16:40:34.217911 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/__init__.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4171 2023-07-27 16:37:23.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/const.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4593 2023-05-09 19:37:24.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/download.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-27 16:40:34.217911 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/faster_whisper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       37 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/faster_whisper/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5809 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/faster_whisper/feature_extractor.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12038 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/faster_whisper/transcribe.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-09 19:37:36.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/file_hash.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2608 2023-07-27 16:37:58.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/handler.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-27 16:40:34.217911 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-07-27 16:40:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      634 2023-07-27 16:40:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-27 16:40:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       55 2023-07-27 16:40:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-07-27 16:40:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/top_level.txt
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-27 16:55:50.715005 wyoming_faster_whisper-1.0.1/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.1/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-07-27 16:55:50.715005 wyoming_faster_whisper-1.0.1/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       56 2023-07-27 16:07:23.000000 wyoming_faster_whisper-1.0.1/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-27 16:55:50.715005 wyoming_faster_whisper-1.0.1/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1225 2023-07-27 16:55:11.000000 wyoming_faster_whisper-1.0.1/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-27 16:55:50.715005 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/__init__.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4021 2023-07-27 16:55:32.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/const.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4593 2023-05-09 19:37:24.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/download.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-27 16:55:50.715005 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/faster_whisper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       37 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/faster_whisper/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5809 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/faster_whisper/feature_extractor.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12038 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/faster_whisper/transcribe.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-09 19:37:36.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/file_hash.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2608 2023-07-27 16:37:58.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/handler.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-27 16:55:50.715005 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-07-27 16:55:50.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      634 2023-07-27 16:55:50.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-27 16:55:50.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       55 2023-07-27 16:55:50.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-07-27 16:55:50.000000 wyoming_faster_whisper-1.0.1/wyoming_faster_whisper.egg-info/top_level.txt
```

### Comparing `wyoming_faster_whisper-1.0.0/PKG-INFO` & `wyoming_faster_whisper-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyoming_faster_whisper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wyoming Server for Faster Whisper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Keywords: rhasspy wyoming whisper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wyoming_faster_whisper-1.0.0/setup.py` & `wyoming_faster_whisper-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     with open(requirements_path, "r", encoding="utf-8") as requirements_file:
         requirements = requirements_file.read().splitlines()
 
 # -----------------------------------------------------------------------------
 
 setup(
     name="wyoming_faster_whisper",
-    version="1.0.0",
+    version="1.0.1",
     description="Wyoming Server for Faster Whisper",
     url="http://github.com/rhasspy/rhasspy3",
     author="Michael Hansen",
     author_email="mike@rhasspy.org",
     license="MIT",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

### Comparing `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/__main__.py` & `wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,20 +73,15 @@
         if model_dir is not None:
             break
 
     if model_dir is None:
         _LOGGER.info("Downloading %s to %s", model, args.download_dir)
         model_dir = download_model(model, args.download_dir)
 
-    if args.language and (args.language != "auto"):
-        _LOGGER.debug("Language: %s", args.language)
-        languages = [args.language]
-    else:
-        languages = WHISPER_LANGUAGES
-
+    if args.language == "auto":
         # Whisper does not understand "auto"
         args.language = None
 
     wyoming_info = Info(
         asr=[
             AsrProgram(
                 name="faster-whisper",
@@ -101,15 +96,15 @@
                         name=model.value,
                         description=model.value,
                         attribution=Attribution(
                             name="rhasspy",
                             url="https://github.com/rhasspy/models/",
                         ),
                         installed=True,
-                        languages=languages,
+                        languages=WHISPER_LANGUAGES,
                     )
                 ],
             )
         ],
     )
 
     # Load converted faster-whisper model
```

### Comparing `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/const.py` & `wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/const.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/download.py` & `wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/download.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/faster_whisper/feature_extractor.py` & `wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/faster_whisper/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/faster_whisper/transcribe.py` & `wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/faster_whisper/transcribe.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/file_hash.py` & `wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/file_hash.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/handler.py` & `wyoming_faster_whisper-1.0.1/wyoming_faster_whisper/handler.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/PKG-INFO` & `wyoming_faster_whisper-1.0.1/wyoming_faster_whisper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyoming-faster-whisper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wyoming Server for Faster Whisper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Keywords: rhasspy wyoming whisper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/SOURCES.txt` & `wyoming_faster_whisper-1.0.1/wyoming_faster_whisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

