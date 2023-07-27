# Comparing `tmp/nonebot_plugin_makemidi-0.1.8.tar.gz` & `tmp/nonebot_plugin_makemidi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_makemidi-0.1.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_makemidi-0.1.9.tar", max compression
```

## Comparing `nonebot_plugin_makemidi-0.1.8.tar` & `nonebot_plugin_makemidi-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1558 2022-09-30 10:19:42.198519 nonebot_plugin_makemidi-0.1.8/nonebot_plugin_makemidi/__init__.py
--rw-r--r--   0        0        0     5871 2022-09-30 15:05:09.600498 nonebot_plugin_makemidi-0.1.8/nonebot_plugin_makemidi/data_source.py
--rw-r--r--   0        0        0  3208108 2021-07-26 12:38:59.000000 nonebot_plugin_makemidi-0.1.8/nonebot_plugin_makemidi/resources/gm.sf2
--rw-r--r--   0        0        0      693 2022-09-30 15:07:55.589824 nonebot_plugin_makemidi-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      797 2022-09-30 15:07:59.578714 nonebot_plugin_makemidi-0.1.8/setup.py
--rw-r--r--   0        0        0      661 2022-09-30 15:07:59.578714 nonebot_plugin_makemidi-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1558 2022-09-30 10:19:42.198519 nonebot_plugin_makemidi-0.1.9/nonebot_plugin_makemidi/__init__.py
+-rw-r--r--   0        0        0     6308 2022-10-04 00:57:21.311378 nonebot_plugin_makemidi-0.1.9/nonebot_plugin_makemidi/data_source.py
+-rw-r--r--   0        0        0  3208108 2021-07-26 12:38:59.000000 nonebot_plugin_makemidi-0.1.9/nonebot_plugin_makemidi/resources/gm.sf2
+-rw-r--r--   0        0        0      693 2022-10-04 01:01:59.362506 nonebot_plugin_makemidi-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      797 2022-10-04 01:03:27.020049 nonebot_plugin_makemidi-0.1.9/setup.py
+-rw-r--r--   0        0        0      661 2022-10-04 01:03:27.020049 nonebot_plugin_makemidi-0.1.9/PKG-INFO
```

### Comparing `nonebot_plugin_makemidi-0.1.8/nonebot_plugin_makemidi/__init__.py` & `nonebot_plugin_makemidi-0.1.9/nonebot_plugin_makemidi/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_makemidi-0.1.8/nonebot_plugin_makemidi/data_source.py` & `nonebot_plugin_makemidi-0.1.9/nonebot_plugin_makemidi/data_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,26 +71,34 @@
     return note, tone_change
 
 
 def play_note(note, length, track, bpm=120, base_num=0, delay=0, velocity=1.0, channel=0, tone_change=0):
     meta_time = 60 * 60 * 10 / bpm
     major_notes = [0, 2, 2, 1, 2, 2, 2, 1]
     base_note = 60
-    if tone_change == 0:
-        note = base_note + base_num * 12 + sum(major_notes[0:note])
-    elif tone_change > 0:
-        note = base_note + base_num * 12 + sum(major_notes[0:note]) + tone_change
-    elif tone_change < 0:
-        note = base_note + base_num * 12 + sum(major_notes[0:note]) + tone_change
-    track.append(
-        Message('note_on', note=note, velocity=round(64 * velocity),
-                time=round(delay * meta_time), channel=channel))
-    track.append(
-        Message('note_off', note=note, velocity=round(64 * velocity),
-                time=round(meta_time * length), channel=channel))
+    if note != 0 and 1 <= note <= 7:
+        if tone_change == 0:
+            note = base_note + base_num * 12 + sum(major_notes[0:note])
+        elif tone_change > 0:
+            note = base_note + base_num * 12 + sum(major_notes[0:note]) + tone_change
+        elif tone_change < 0:
+            note = base_note + base_num * 12 + sum(major_notes[0:note]) + tone_change
+        track.append(
+            Message('note_on', note=note, velocity=round(64 * velocity),
+                    time=round(delay * meta_time), channel=channel))
+        track.append(
+            Message('note_off', note=note, velocity=round(64 * velocity),
+                    time=round(meta_time * length), channel=channel))
+    elif note == 0:
+        track.append(
+            Message('note_on', note=note, velocity=round(64 * velocity),
+                    time=round(delay * meta_time), channel=channel))
+        track.append(
+            Message('note_off', note=note, velocity=round(64 * velocity),
+                    time=round(meta_time * length), channel=channel))
 
 
 def make_midi(qq, notes, bpm=120, program=0, key_signature='C'):
     if os.path.exists(midi_path):
         pass
     else:
         os.mkdir(midi_path)
@@ -104,18 +112,18 @@
     mid.tracks.append(track)
     tempo = bpm2tempo(bpm)
     track.append(Message('program_change', channel=0, program=program, time=0))
     track.append(MetaMessage('set_tempo', tempo=tempo, time=0))
     track.append(MetaMessage('key_signature', key=key_signature))
     for note in notes:
         if '~' in note:
-            length = 1 + 0.5 * int(str(note).count('~'))
+            length = 1 + int(str(note).count('~'))
             note = note.replace('~', '')
         elif '_' in note:
-            length = 1 - 0.25 * int(str(note).count('_'))
+            length = 1 * 0.5 ** int(str(note).count('_'))
             note = note.replace('_', '')
         else:
             length = 1
         if '#' in note:
             tone_change = 1
             note = note.replace('#', '')
         elif 'b' in note:
```

### Comparing `nonebot_plugin_makemidi-0.1.8/nonebot_plugin_makemidi/resources/gm.sf2` & `nonebot_plugin_makemidi-0.1.9/nonebot_plugin_makemidi/resources/gm.sf2`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_makemidi-0.1.8/pyproject.toml` & `nonebot_plugin_makemidi-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_makemidi"
-version = "0.1.8"
+version = "0.1.9"
 description = "Easy midi maker"
 authors = ["RandomEnch <randomench@foxmail.com>"]
 license = "MIT"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
```

### Comparing `nonebot_plugin_makemidi-0.1.8/setup.py` & `nonebot_plugin_makemidi-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'mido',
  'nonebot-adapter-onebot>=2.0.0-beta.1,<3.0.0',
  'nonebot2>=2.0.0-beta.4,<3.0.0',
  'pydub>=0.25.1,<0.26.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-makemidi',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Easy midi maker',
     'long_description': None,
     'author': 'RandomEnch',
     'author_email': 'randomench@foxmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `nonebot_plugin_makemidi-0.1.8/PKG-INFO` & `nonebot_plugin_makemidi-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-makemidi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Easy midi maker
 License: MIT
 Author: RandomEnch
 Author-email: randomench@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

