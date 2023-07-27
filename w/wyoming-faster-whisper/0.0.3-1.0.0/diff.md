# Comparing `tmp/wyoming_faster_whisper-0.0.3.tar.gz` & `tmp/wyoming_faster_whisper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyoming_faster_whisper-0.0.3.tar", last modified: Wed May 10 14:43:47 2023, max compression
+gzip compressed data, was "wyoming_faster_whisper-1.0.0.tar", last modified: Thu Jul 27 16:40:34 2023, max compression
```

## Comparing `wyoming_faster_whisper-0.0.3.tar` & `wyoming_faster_whisper-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-10 14:43:47.145580 wyoming_faster_whisper-0.0.3/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-05-10 14:43:47.145580 wyoming_faster_whisper-0.0.3/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       55 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-05-10 14:43:47.145580 wyoming_faster_whisper-0.0.3/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1225 2023-05-10 14:43:21.000000 wyoming_faster_whisper-0.0.3/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-10 14:43:47.145580 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/__init__.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     3837 2023-05-10 14:42:35.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/const.py
--rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4593 2023-05-09 19:37:24.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/download.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-10 14:43:47.145580 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/faster_whisper/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       37 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/faster_whisper/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5809 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/faster_whisper/feature_extractor.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12038 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/faster_whisper/transcribe.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-09 19:37:36.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/file_hash.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2199 2023-04-21 15:28:34.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/handler.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-10 14:43:47.145580 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-05-10 14:43:47.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      634 2023-05-10 14:43:47.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-10 14:43:47.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       54 2023-05-10 14:43:47.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-05-10 14:43:47.000000 wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/top_level.txt
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-27 16:40:34.217911 wyoming_faster_whisper-1.0.0/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       25 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.0/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-07-27 16:40:34.217911 wyoming_faster_whisper-1.0.0/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       56 2023-07-27 16:07:23.000000 wyoming_faster_whisper-1.0.0/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-07-27 16:40:34.217911 wyoming_faster_whisper-1.0.0/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1225 2023-07-27 16:05:58.000000 wyoming_faster_whisper-1.0.0/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-27 16:40:34.217911 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       41 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/__init__.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4171 2023-07-27 16:37:23.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1015 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/const.py
+-rwxr-xr-x   0 hansenm   (1000) hansenm   (1000)     4593 2023-05-09 19:37:24.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/download.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-27 16:40:34.217911 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/faster_whisper/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       37 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/faster_whisper/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5809 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/faster_whisper/feature_extractor.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12038 2023-04-21 15:28:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/faster_whisper/transcribe.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1107 2023-05-09 19:37:36.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/file_hash.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2608 2023-07-27 16:37:58.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/handler.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-27 16:40:34.217911 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      647 2023-07-27 16:40:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      634 2023-07-27 16:40:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-27 16:40:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       55 2023-07-27 16:40:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-07-27 16:40:34.000000 wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/top_level.txt
```

### Comparing `wyoming_faster_whisper-0.0.3/PKG-INFO` & `wyoming_faster_whisper-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyoming_faster_whisper
-Version: 0.0.3
+Version: 1.0.0
 Summary: Wyoming Server for Faster Whisper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Keywords: rhasspy wyoming whisper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wyoming_faster_whisper-0.0.3/setup.py` & `wyoming_faster_whisper-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     with open(requirements_path, "r", encoding="utf-8") as requirements_file:
         requirements = requirements_file.read().splitlines()
 
 # -----------------------------------------------------------------------------
 
 setup(
     name="wyoming_faster_whisper",
-    version="0.0.3",
+    version="1.0.0",
     description="Wyoming Server for Faster Whisper",
     url="http://github.com/rhasspy/rhasspy3",
     author="Michael Hansen",
     author_email="mike@rhasspy.org",
     license="MIT",
     packages=setuptools.find_packages(),
     install_requires=requirements,
```

### Comparing `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/__main__.py` & `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,51 +19,54 @@
 
 async def main() -> None:
     """Main entry point."""
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--model",
         required=True,
-        choices=list(FasterWhisperModel),
+        choices=list(v.value for v in FasterWhisperModel),
         help="Name of faster-whisper model to use",
     )
     parser.add_argument("--uri", required=True, help="unix:// or tcp://")
     parser.add_argument(
         "--data-dir",
         required=True,
         action="append",
         help="Data directory to check for downloaded models",
     )
     parser.add_argument(
         "--download-dir",
-        required=True,
-        help="Directory to download models into",
+        help="Directory to download models into (default: first data dir)",
     )
     parser.add_argument(
         "--device",
         default="cpu",
         help="Device to use for inference (default: cpu)",
     )
     parser.add_argument(
         "--language",
-        help="Language to set for transcription",
+        help="Default language to set for transcription",
     )
     parser.add_argument(
         "--compute-type",
         default="default",
         help="Compute type (float16, int8, etc.)",
     )
     parser.add_argument(
         "--beam-size",
         type=int,
         default=5,
     )
     parser.add_argument("--debug", action="store_true", help="Log DEBUG messages")
     args = parser.parse_args()
 
+    if not args.download_dir:
+        # Download to first data dir by default
+        args.download_dir = args.data_dir[0]
+
     logging.basicConfig(level=logging.DEBUG if args.debug else logging.INFO)
 
     # Look for model
     model = FasterWhisperModel(args.model)
     model_dir: Optional[Path] = None
     for data_dir in args.data_dir:
         model_dir = find_model(model, data_dir)
@@ -83,22 +86,24 @@
         # Whisper does not understand "auto"
         args.language = None
 
     wyoming_info = Info(
         asr=[
             AsrProgram(
                 name="faster-whisper",
+                description="Faster Whisper transcription with CTranslate2",
                 attribution=Attribution(
                     name="Guillaume Klein",
                     url="https://github.com/guillaumekln/faster-whisper/",
                 ),
                 installed=True,
                 models=[
                     AsrModel(
                         name=model.value,
+                        description=model.value,
                         attribution=Attribution(
                             name="rhasspy",
                             url="https://github.com/rhasspy/models/",
                         ),
                         installed=True,
                         languages=languages,
                     )
@@ -128,8 +133,11 @@
         )
     )
 
 
 # -----------------------------------------------------------------------------
 
 if __name__ == "__main__":
-    asyncio.run(main())
+    try:
+        asyncio.run(main())
+    except KeyboardInterrupt:
+        pass
```

### Comparing `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/const.py` & `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/const.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/download.py` & `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/download.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/faster_whisper/feature_extractor.py` & `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/faster_whisper/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/faster_whisper/transcribe.py` & `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/faster_whisper/transcribe.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/file_hash.py` & `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/file_hash.py`

 * *Files identical despite different names*

### Comparing `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper/handler.py` & `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper/handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Event handler for clients of the server."""
 import argparse
 import asyncio
 import logging
 
-from wyoming.asr import Transcript
+from wyoming.asr import Transcribe, Transcript
 from wyoming.audio import AudioChunk, AudioChunkConverter, AudioStop
 from wyoming.event import Event
 from wyoming.info import Describe, Info
 from wyoming.server import AsyncEventHandler
 
 from .faster_whisper import WhisperModel
 
@@ -34,21 +34,29 @@
         self.model_lock = model_lock
         self.audio = bytes()
         self.audio_converter = AudioChunkConverter(
             rate=16000,
             width=2,
             channels=1,
         )
+        self._language = self.cli_args.language
 
     async def handle_event(self, event: Event) -> bool:
         if Describe.is_type(event.type):
             await self.write_event(self.wyoming_info_event)
             _LOGGER.debug("Sent info")
             return True
 
+        if Transcribe.is_type(event.type):
+            transcribe = Transcribe.from_event(event)
+            if transcribe.language:
+                self._language = transcribe.language
+                _LOGGER.debug("Language set to %s", transcribe.language)
+            return True
+
         if AudioChunk.is_type(event.type):
             if not self.audio:
                 _LOGGER.debug("Receiving audio")
 
             chunk = AudioChunk.from_event(event)
             chunk = self.audio_converter.convert(chunk)
             self.audio += chunk.audio
@@ -57,20 +65,23 @@
 
         if AudioStop.is_type(event.type):
             _LOGGER.debug("Audio stopped")
             async with self.model_lock:
                 segments, _info = self.model.transcribe(
                     self.audio,
                     beam_size=self.cli_args.beam_size,
-                    language=self.cli_args.language,
+                    language=self._language,
                 )
 
             text = " ".join(segment.text for segment in segments)
             _LOGGER.info(text)
 
             await self.write_event(Transcript(text=text).event())
             _LOGGER.debug("Completed request")
 
+            # Reset
             self.audio = bytes()
+            self._language = self.cli_args.language
+
             return False
 
         return True
```

### Comparing `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/PKG-INFO` & `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyoming-faster-whisper
-Version: 0.0.3
+Version: 1.0.0
 Summary: Wyoming Server for Faster Whisper
 Home-page: http://github.com/rhasspy/rhasspy3
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: MIT
 Keywords: rhasspy wyoming whisper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `wyoming_faster_whisper-0.0.3/wyoming_faster_whisper.egg-info/SOURCES.txt` & `wyoming_faster_whisper-1.0.0/wyoming_faster_whisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

