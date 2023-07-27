# Comparing `tmp/simple_pygame-0.0.6.tar.gz` & `tmp/simple_pygame-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_pygame-0.0.6.tar", last modified: Wed Jun 28 14:18:20 2023, max compression
+gzip compressed data, was "simple_pygame-0.0.7.tar", last modified: Thu Jul 27 10:05:24 2023, max compression
```

## Comparing `simple_pygame-0.0.6.tar` & `simple_pygame-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 14:18:20.456643 simple_pygame-0.0.6/
--rw-rw-rw-   0        0        0     1087 2023-02-13 12:51:16.000000 simple_pygame-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1416 2023-06-28 14:18:20.456643 simple_pygame-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      897 2023-06-28 14:16:32.000000 simple_pygame-0.0.6/README.md
--rw-rw-rw-   0        0        0      602 2023-06-28 14:16:13.000000 simple_pygame-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 14:18:20.456643 simple_pygame-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-28 14:18:20.425395 simple_pygame-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-28 14:18:20.425395 simple_pygame-0.0.6/src/simple_pygame/
--rw-rw-rw-   0        0        0     1689 2023-06-28 14:11:02.000000 simple_pygame-0.0.6/src/simple_pygame/__init__.py
--rw-rw-rw-   0        0        0      319 2023-06-28 14:11:01.000000 simple_pygame-0.0.6/src/simple_pygame/constants.py
--rw-rw-rw-   0        0        0     1169 2023-06-28 14:10:59.000000 simple_pygame-0.0.6/src/simple_pygame/mixer.py
--rw-rw-rw-   0        0        0    37405 2023-06-28 14:16:43.000000 simple_pygame-0.0.6/src/simple_pygame/music.py
--rw-rw-rw-   0        0        0     3230 2023-06-28 14:10:51.000000 simple_pygame-0.0.6/src/simple_pygame/transform.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:18:20.441019 simple_pygame-0.0.6/src/simple_pygame.egg-info/
--rw-rw-rw-   0        0        0     1416 2023-06-28 14:18:20.000000 simple_pygame-0.0.6/src/simple_pygame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-06-28 14:18:20.000000 simple_pygame-0.0.6/src/simple_pygame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 14:18:20.000000 simple_pygame-0.0.6/src/simple_pygame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-28 14:18:20.000000 simple_pygame-0.0.6/src/simple_pygame.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 10:05:24.280054 simple_pygame-0.0.7/
+-rw-rw-rw-   0        0        0     1087 2023-07-27 10:04:19.000000 simple_pygame-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1416 2023-07-27 10:05:24.280054 simple_pygame-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      897 2023-07-27 10:04:06.000000 simple_pygame-0.0.7/README.md
+-rw-rw-rw-   0        0        0      602 2023-07-27 09:48:51.000000 simple_pygame-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 10:05:24.280054 simple_pygame-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 10:05:24.233177 simple_pygame-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 10:05:24.248802 simple_pygame-0.0.7/src/simple_pygame/
+-rw-rw-rw-   0        0        0     2288 2023-07-27 09:42:00.000000 simple_pygame-0.0.7/src/simple_pygame/__init__.py
+-rw-rw-rw-   0        0        0    41629 2023-07-27 09:30:48.000000 simple_pygame-0.0.7/src/simple_pygame/audio.py
+-rw-rw-rw-   0        0        0      321 2023-07-27 09:31:53.000000 simple_pygame-0.0.7/src/simple_pygame/constants.py
+-rw-rw-rw-   0        0        0     1660 2023-07-27 09:40:47.000000 simple_pygame-0.0.7/src/simple_pygame/mixer.py
+-rw-rw-rw-   0        0        0     3304 2023-07-27 10:03:54.000000 simple_pygame-0.0.7/src/simple_pygame/transform.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:05:24.280054 simple_pygame-0.0.7/src/simple_pygame.egg-info/
+-rw-rw-rw-   0        0        0     1416 2023-07-27 10:05:24.000000 simple_pygame-0.0.7/src/simple_pygame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-07-27 10:05:24.000000 simple_pygame-0.0.7/src/simple_pygame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 10:05:24.000000 simple_pygame-0.0.7/src/simple_pygame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-27 10:05:24.000000 simple_pygame-0.0.7/src/simple_pygame.egg-info/top_level.txt
```

### Comparing `simple_pygame-0.0.6/LICENSE` & `simple_pygame-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_pygame-0.0.6/PKG-INFO` & `simple_pygame-0.0.7/src/simple_pygame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simple_pygame
-Version: 0.0.6
+Name: simple-pygame
+Version: 0.0.7
 Summary: A Python library that provides many features using Pygame and other libraries.
 Author: YoutuberTom
 Project-URL: Source, https://github.com/YoutuberTom/Simple_Pygame
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,16 +26,16 @@
 
     Python >= 3.7.0
 
 ## Python libraries:
 
 | Library | Version |
 |:--------|:--------|
-|pygame   |>= 2.0.0 |
-|pyaudio  |>= 0.2.11|
+|pygame   |>= 1.9.4 |
+|pyaudio  |>= 0.2.12|
 
 ## Other requirements:
 
 - ffmpeg.
 
 - ffprobe (optional).
```

### Comparing `simple_pygame-0.0.6/README.md` & `simple_pygame-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
     Python >= 3.7.0
 
 ## Python libraries:
 
 | Library | Version |
 |:--------|:--------|
-|pygame   |>= 2.0.0 |
-|pyaudio  |>= 0.2.11|
+|pygame   |>= 1.9.4 |
+|pyaudio  |>= 0.2.12|
 
 ## Other requirements:
 
 - ffmpeg.
 
 - ffprobe (optional).
```

### Comparing `simple_pygame-0.0.6/pyproject.toml` & `simple_pygame-0.0.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple_pygame"
-version = "0.0.6"
+version = "0.0.7"
 description = "A Python library that provides many features using Pygame and other libraries."
 readme = "README.md"
 requires-python = ">= 3.7"
 authors = [
     {name = "YoutuberTom"}
 ]
 classifiers = [
```

### Comparing `simple_pygame-0.0.6/src/simple_pygame/__init__.py` & `simple_pygame-0.0.7/src/simple_pygame/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 """
 Simple Pygame is a Python library that provides many features using Pygame and other libraries. It can help you create multimedia programs much easier and cleaner.
 """
 import gc
+from typing import Iterable
 from .constants import __version__
 from .constants import *
 from . import mixer
 
-_init = False
-
-def get_init() -> bool:
-    """
-    Return `True` if Simple Pygame is currently initialized, otherwise `False`.
+def init(modules: Iterable = []) -> tuple:
     """
-    return _init
+    Import/Initialize Simple Pygame modules and return successfully imported/initialized modules.
 
-def init() -> tuple:
-    """
-    Import/Initialize all Simple Pygame modules and return successfully imported/initialized modules.
+    Parameters
+    ----------
+
+    modules (optional): Specifies which modules to import/initialize. If it's empty, import/initialize all Simple Pygame modules.
     """
-    global _init
+    try:
+        modules_len = len(modules)
+        iter(modules)
+    except TypeError:
+        raise TypeError("Modules is not iterable.") from None
 
-    if get_init():
-        return ()
-    _init = True
-    
     successfully_imported = []
 
-    mixer_successfully_imported = mixer.init()
-    if mixer_successfully_imported:
-        successfully_imported.append(MixerModule)
-    
-    try:
-        global transform
-        from . import transform
-        successfully_imported.append(TransformModule)
-    except ImportError:
-        pass
-
-    if len(successfully_imported) == 0:
-        _init = False
-    
+    if modules_len == 0 or MixerModule in modules:
+        mixer_successfully_imported = mixer.init()
+        if mixer_successfully_imported:
+            successfully_imported.append(MixerModule)
+
+    if modules_len == 0 or TransformModule in modules:
+        try:
+            global transform
+            from . import transform
+            successfully_imported.append(TransformModule)
+        except ImportError:
+            pass
+
     return (*successfully_imported,)
 
-def quit() -> tuple:
+def quit(modules: Iterable = []) -> tuple:
     """
-    Quit/Uninitialize all Simple Pygame modules and return successfully quit/uninitialized modules.
-    """
-    global _init
+    Quit/Uninitialize Simple Pygame modules and return successfully quit/uninitialized modules.
 
-    if not get_init():
-        return ()
-    _init = False
+    Parameters
+    ----------
 
-    successfully_quit = []
+    modules (optional): Specifies which modules to quit/uninitialize. If it's empty, quit/uninitialize all Simple Pygame modules.
+    """
+    try:
+        modules_len = len(modules)
+        iter(modules)
+    except TypeError:
+        raise TypeError("Modules is not iterable.") from None
 
-    mixer_successfully_quit = mixer.quit()
-    if mixer_successfully_quit:
-        successfully_quit.append(MixerModule)
+    successfully_quit = []
 
-    try:
-        global transform
-        del transform
-        successfully_quit.append(TransformModule)
-    except NameError:
-        pass
+    if modules_len == 0 or MixerModule in modules:
+        mixer_successfully_quit = mixer.quit()
+        if mixer_successfully_quit:
+            successfully_quit.append(MixerModule)
+
+    if modules_len == 0 or TransformModule in modules:
+        try:
+            global transform
+            del transform
+            successfully_quit.append(TransformModule)
+        except NameError:
+            pass
 
     gc.collect()
     return (*successfully_quit,)
```

### Comparing `simple_pygame-0.0.6/src/simple_pygame/transform.py` & `simple_pygame-0.0.7/src/simple_pygame/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,33 +25,31 @@
 
     rect (optional): The Rect defining the area that should be filled. If the value is `None`, the entire Surface will be filled.
 
     special_flags (optional): Additional flags to customize the fill behavior.
     """
     if rect == None:
         surface.fill(color, special_flags = special_flags)
-
         return rect
 
     try:
-        rect = pygame.Rect(rect)
+        rect = pygame.Rect(rect) if type(rect) != pygame.Rect else rect
     except TypeError:
         raise ValueError("Invalid rect style object.") from None
 
     if rect.x < 0:
         rect.width, rect.x = max(0, rect.width + rect.x), 0
     if rect.y < 0:
         rect.height, rect.y = max(0, rect.height + rect.y), 0
 
     surface_size = surface.get_size()
     rect.width = min(max(0, rect.width), surface_size[0])
     rect.height = min(max(0, rect.height), surface_size[1])
 
     surface.fill(color, rect, special_flags)
-
     return rect
 
 def reverse_fill(surface: pygame.Surface, color: Union[pygame.Color, tuple, list], rect: pygame.Rect, special_flags: int = 0) -> pygame.Surface:
     """
     Fill the area outside the specified Rect on the given Surface with a solid color.
 
     Parameters
@@ -62,15 +60,15 @@
     color: The color to fill the Surface with.
 
     rect: The Rect defining the area that should not be filled.
 
     special_flags (optional): Additional flags to customize the fill behavior.
     """
     try:
-        rect = pygame.Rect(rect)
+        rect = pygame.Rect(rect) if type(rect) != pygame.Rect else rect
     except TypeError:
         raise ValueError("Invalid rect style object.") from None
 
     if rect.x < 0:
         rect.width, rect.x = max(0, rect.width + rect.x), 0
     if rect.y < 0:
         rect.height, rect.y = max(0, rect.height + rect.y), 0
```

### Comparing `simple_pygame-0.0.6/src/simple_pygame.egg-info/PKG-INFO` & `simple_pygame-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simple-pygame
-Version: 0.0.6
+Name: simple_pygame
+Version: 0.0.7
 Summary: A Python library that provides many features using Pygame and other libraries.
 Author: YoutuberTom
 Project-URL: Source, https://github.com/YoutuberTom/Simple_Pygame
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,16 +26,16 @@
 
     Python >= 3.7.0
 
 ## Python libraries:
 
 | Library | Version |
 |:--------|:--------|
-|pygame   |>= 2.0.0 |
-|pyaudio  |>= 0.2.11|
+|pygame   |>= 1.9.4 |
+|pyaudio  |>= 0.2.12|
 
 ## Other requirements:
 
 - ffmpeg.
 
 - ffprobe (optional).
```

