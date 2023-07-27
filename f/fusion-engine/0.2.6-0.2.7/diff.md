# Comparing `tmp/fusion-engine-0.2.6.tar.gz` & `tmp/fusion-engine-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-0.2.6.tar", last modified: Wed Jul 26 13:57:49 2023, max compression
+gzip compressed data, was "fusion-engine-0.2.7.tar", last modified: Thu Jul 27 09:21:18 2023, max compression
```

## Comparing `fusion-engine-0.2.6.tar` & `fusion-engine-0.2.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-26 13:57:49.101007 fusion-engine-0.2.6/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-0.2.6/LICENCE.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5290 2023-07-26 13:57:49.100489 fusion-engine-0.2.6/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4027 2023-07-24 21:00:42.000000 fusion-engine-0.2.6/README.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1667 2023-07-24 10:32:49.000000 fusion-engine-0.2.6/pyproject.toml
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       24 2023-07-07 14:54:41.000000 fusion-engine-0.2.6/requirements.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-26 13:57:49.101233 fusion-engine-0.2.6/setup.cfg
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1020 2023-07-24 20:53:33.000000 fusion-engine-0.2.6/setup.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-26 13:57:49.077012 fusion-engine-0.2.6/src/
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-26 13:57:49.084670 fusion-engine-0.2.6/src/fusion_engine.egg-info/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5290 2023-07-26 13:57:49.000000 fusion-engine-0.2.6/src/fusion_engine.egg-info/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      881 2023-07-26 13:57:49.000000 fusion-engine-0.2.6/src/fusion_engine.egg-info/SOURCES.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-26 13:57:49.000000 fusion-engine-0.2.6/src/fusion_engine.egg-info/dependency_links.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       25 2023-07-26 13:57:49.000000 fusion-engine-0.2.6/src/fusion_engine.egg-info/requires.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-07-26 13:57:49.000000 fusion-engine-0.2.6/src/fusion_engine.egg-info/top_level.txt
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-26 13:57:49.085794 fusion-engine-0.2.6/src/fusionengine/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1079 2023-07-26 13:45:36.000000 fusion-engine-0.2.6/src/fusionengine/__init__.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-26 13:57:49.086453 fusion-engine-0.2.6/src/fusionengine/debugfiles/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-0.2.6/src/fusionengine/debugfiles/fe.png
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-26 13:57:49.099449 fusion-engine-0.2.6/src/fusionengine/files/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3974 2023-07-26 13:45:02.000000 fusion-engine-0.2.6/src/fusionengine/files/body.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1694 2023-07-25 14:30:48.000000 fusion-engine-0.2.6/src/fusionengine/files/color.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      458 2023-07-25 14:34:56.000000 fusion-engine-0.2.6/src/fusionengine/files/data.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      162 2023-07-25 14:35:08.000000 fusion-engine-0.2.6/src/fusionengine/files/debug.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2753 2023-07-25 14:31:30.000000 fusion-engine-0.2.6/src/fusionengine/files/draw.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      370 2023-07-25 14:35:37.000000 fusion-engine-0.2.6/src/fusionengine/files/enums.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    10776 2023-07-25 14:36:51.000000 fusion-engine-0.2.6/src/fusionengine/files/event.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      250 2023-07-25 14:37:33.000000 fusion-engine-0.2.6/src/fusionengine/files/exceptions.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      173 2023-07-25 14:37:50.000000 fusion-engine-0.2.6/src/fusionengine/files/fonts.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1073 2023-07-25 14:38:51.000000 fusion-engine-0.2.6/src/fusionengine/files/image.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      557 2023-07-20 10:26:42.000000 fusion-engine-0.2.6/src/fusionengine/files/imports.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-0.2.6/src/fusionengine/files/physics.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      692 2023-07-25 14:40:03.000000 fusion-engine-0.2.6/src/fusionengine/files/shape.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5576 2023-07-25 14:39:35.000000 fusion-engine-0.2.6/src/fusionengine/files/storage.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      929 2023-07-25 14:41:15.000000 fusion-engine-0.2.6/src/fusionengine/files/systems.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4133 2023-07-25 14:43:59.000000 fusion-engine-0.2.6/src/fusionengine/files/ui.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3250 2023-07-25 16:06:47.000000 fusion-engine-0.2.6/src/fusionengine/files/window.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-27 09:21:18.327516 fusion-engine-0.2.7/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-0.2.7/LICENCE.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5290 2023-07-27 09:21:18.326593 fusion-engine-0.2.7/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4027 2023-07-24 21:00:42.000000 fusion-engine-0.2.7/README.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1667 2023-07-24 10:32:49.000000 fusion-engine-0.2.7/pyproject.toml
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       24 2023-07-07 14:54:41.000000 fusion-engine-0.2.7/requirements.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-07-27 09:21:18.327907 fusion-engine-0.2.7/setup.cfg
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1348 2023-07-27 09:19:57.000000 fusion-engine-0.2.7/setup.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-27 09:21:18.301513 fusion-engine-0.2.7/src/
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-27 09:21:18.309527 fusion-engine-0.2.7/src/fusion_engine.egg-info/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5290 2023-07-27 09:21:18.000000 fusion-engine-0.2.7/src/fusion_engine.egg-info/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      881 2023-07-27 09:21:18.000000 fusion-engine-0.2.7/src/fusion_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-07-27 09:21:18.000000 fusion-engine-0.2.7/src/fusion_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       25 2023-07-27 09:21:18.000000 fusion-engine-0.2.7/src/fusion_engine.egg-info/requires.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-07-27 09:21:18.000000 fusion-engine-0.2.7/src/fusion_engine.egg-info/top_level.txt
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-27 09:21:18.310229 fusion-engine-0.2.7/src/fusionengine/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1124 2023-07-27 09:20:57.000000 fusion-engine-0.2.7/src/fusionengine/__init__.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-27 09:21:18.311001 fusion-engine-0.2.7/src/fusionengine/debugfiles/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-0.2.7/src/fusionengine/debugfiles/fe.png
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-07-27 09:21:18.325379 fusion-engine-0.2.7/src/fusionengine/files/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3974 2023-07-26 13:45:02.000000 fusion-engine-0.2.7/src/fusionengine/files/body.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1694 2023-07-25 14:30:48.000000 fusion-engine-0.2.7/src/fusionengine/files/color.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      458 2023-07-25 14:34:56.000000 fusion-engine-0.2.7/src/fusionengine/files/data.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      162 2023-07-25 14:35:08.000000 fusion-engine-0.2.7/src/fusionengine/files/debug.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2753 2023-07-25 14:31:30.000000 fusion-engine-0.2.7/src/fusionengine/files/draw.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      370 2023-07-25 14:35:37.000000 fusion-engine-0.2.7/src/fusionengine/files/enums.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    10776 2023-07-25 14:36:51.000000 fusion-engine-0.2.7/src/fusionengine/files/event.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      250 2023-07-25 14:37:33.000000 fusion-engine-0.2.7/src/fusionengine/files/exceptions.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      173 2023-07-25 14:37:50.000000 fusion-engine-0.2.7/src/fusionengine/files/fonts.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1073 2023-07-25 14:38:51.000000 fusion-engine-0.2.7/src/fusionengine/files/image.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      557 2023-07-20 10:26:42.000000 fusion-engine-0.2.7/src/fusionengine/files/imports.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-0.2.7/src/fusionengine/files/physics.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      692 2023-07-25 14:40:03.000000 fusion-engine-0.2.7/src/fusionengine/files/shape.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5576 2023-07-25 14:39:35.000000 fusion-engine-0.2.7/src/fusionengine/files/storage.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      929 2023-07-25 14:41:15.000000 fusion-engine-0.2.7/src/fusionengine/files/systems.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     4133 2023-07-25 14:43:59.000000 fusion-engine-0.2.7/src/fusionengine/files/ui.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3440 2023-07-27 09:10:08.000000 fusion-engine-0.2.7/src/fusionengine/files/window.py
```

### Comparing `fusion-engine-0.2.6/LICENCE.md` & `fusion-engine-0.2.7/LICENCE.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/PKG-INFO` & `fusion-engine-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.2.6
+Version: 0.2.7
 Summary: A custom open-source game engine on Python and PySDL2, it's written in pure Python! It's easy and fast!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `fusion-engine-0.2.6/README.md` & `fusion-engine-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/pyproject.toml` & `fusion-engine-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusion_engine.egg-info/PKG-INFO` & `fusion-engine-0.2.7/src/fusion_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 0.2.6
+Version: 0.2.7
 Summary: A custom open-source game engine on Python and PySDL2, it's written in pure Python! It's easy and fast!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: LICENSE.md
 Keywords: game,python,gamedev,game-engine,sdl2,game-development,pure-python,sdl2-mixer,sdl2-ttf,sdl2-image,python-game,pysdl2,sdl2-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `fusion-engine-0.2.6/src/fusion_engine.egg-info/SOURCES.txt` & `fusion-engine-0.2.7/src/fusion_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusionengine/__init__.py` & `fusion-engine-0.2.7/src/fusionengine/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 __author__ = "Dimkauzh"
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 import fusionengine.files.systems as sysconfig
 from fusionengine.files.imports import *
 
 class Main:
     def __init__(self):
         """A class that contains all the functions and classes. You need to initialize this class to use the engine.
         """
         sdl2.SDL_Init(sdl2.SDL_INIT_VIDEO)
         self.window = window.Window()
         self.color = color.Colors()
+        self.colortools = color.ColorTools()
         self.event = event.Event()
         self.keys = event.Keys()
         self.draw = draw.Draw()
         self.image = image.Image()
         self.body = body
         self.system = sysconfig.System()
         self.rendereroptions = sysconfig.RendererOptions()
```

### Comparing `fusion-engine-0.2.6/src/fusionengine/debugfiles/fe.png` & `fusion-engine-0.2.7/src/fusionengine/debugfiles/fe.png`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusionengine/files/body.py` & `fusion-engine-0.2.7/src/fusionengine/files/body.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusionengine/files/color.py` & `fusion-engine-0.2.7/src/fusionengine/files/color.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusionengine/files/draw.py` & `fusion-engine-0.2.7/src/fusionengine/files/draw.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusionengine/files/event.py` & `fusion-engine-0.2.7/src/fusionengine/files/event.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusionengine/files/image.py` & `fusion-engine-0.2.7/src/fusionengine/files/image.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusionengine/files/imports.py` & `fusion-engine-0.2.7/src/fusionengine/files/imports.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusionengine/files/shape.py` & `fusion-engine-0.2.7/src/fusionengine/files/shape.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusionengine/files/storage.py` & `fusion-engine-0.2.7/src/fusionengine/files/storage.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusionengine/files/systems.py` & `fusion-engine-0.2.7/src/fusionengine/files/systems.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusionengine/files/ui.py` & `fusion-engine-0.2.7/src/fusionengine/files/ui.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-0.2.6/src/fusionengine/files/window.py` & `fusion-engine-0.2.7/src/fusionengine/files/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import fusionengine.files.systems as sysconfig
 from fusionengine.files.imports import *
 
 class _CustomRenderer:
-    def __init__(self, window: sdl2.SDL_CreateWindow) -> None:
+    def __init__(self, window: sdl2.SDL_CreateWindow, title: str, width: int, height: int) -> None:
         """A class that creates a new custom renderer. (Not for the user)
 
         Args:
             window (sdl2.SDL_CreateWindow): An created sdl2 window
         """        """"""
         self.window = window
+
+        self.title = title
+        self.width = width
+        self.height = height
+        self.size = (self.width, self.height)
+
         self.event = sdl2.SDL_Event()
         self.renderer = sdl2.SDL_CreateRenderer(self.window, -1, sysconfig.RendererOptions().rendererflag)
         sdl2.SDL_SetRenderDrawBlendMode(self.renderer, sdl2.SDL_BLENDMODE_BLEND)
 
 class Window:
     def __init__(self) -> None:
         """A class that contains all the window functions.
@@ -39,15 +45,15 @@
                                        sdl2.SDL_WINDOWPOS_CENTERED,
                                        sdl2.SDL_WINDOWPOS_CENTERED,
                                        width,
                                        height,
                                        sdl2.SDL_WINDOW_SHOWN
                                        )
         self._running = True
-        self.window = _CustomRenderer(self.window_window)
+        self.window = _CustomRenderer(self.window_window, title, width, height)
 
         return self.window
 
     def loop(self, your_loop: callable):
         """A custom decorator function that turns a function into the main loop of the program.
 
         Args:
```

