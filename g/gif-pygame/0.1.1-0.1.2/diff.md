# Comparing `tmp/gif_pygame-0.1.1.tar.gz` & `tmp/gif_pygame-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gif_pygame-0.1.1.tar", last modified: Wed Jul 26 17:16:15 2023, max compression
+gzip compressed data, was "gif_pygame-0.1.2.tar", last modified: Thu Jul 27 18:29:43 2023, max compression
```

## Comparing `gif_pygame-0.1.1.tar` & `gif_pygame-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:16:15.451869 gif_pygame-0.1.1/
--rw-rw-rw-   0        0        0     1083 2023-03-27 19:37:47.000000 gif_pygame-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     5023 2023-07-26 17:16:15.451869 gif_pygame-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4039 2023-07-26 15:03:01.000000 gif_pygame-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 17:16:15.439414 gif_pygame-0.1.1/gif_pygame/
--rw-rw-rw-   0        0        0       50 2023-03-27 21:16:13.000000 gif_pygame-0.1.1/gif_pygame/__init__.py
--rw-rw-rw-   0        0        0    22554 2023-07-26 14:47:22.000000 gif_pygame-0.1.1/gif_pygame/_pygame_gif.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:16:15.450867 gif_pygame-0.1.1/gif_pygame.egg-info/
--rw-rw-rw-   0        0        0     5023 2023-07-26 17:16:15.000000 gif_pygame-0.1.1/gif_pygame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-07-26 17:16:15.000000 gif_pygame-0.1.1/gif_pygame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:16:15.000000 gif_pygame-0.1.1/gif_pygame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 17:16:15.000000 gif_pygame-0.1.1/gif_pygame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 17:16:15.000000 gif_pygame-0.1.1/gif_pygame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 17:16:15.452870 gif_pygame-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1281 2023-07-26 17:15:33.000000 gif_pygame-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 18:29:43.240625 gif_pygame-0.1.2/
+-rw-rw-rw-   0        0        0     1083 2023-03-27 19:37:47.000000 gif_pygame-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5023 2023-07-27 18:29:43.239626 gif_pygame-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4039 2023-07-26 15:03:01.000000 gif_pygame-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 18:29:43.227600 gif_pygame-0.1.2/gif_pygame/
+-rw-rw-rw-   0        0        0       50 2023-03-27 21:16:13.000000 gif_pygame-0.1.2/gif_pygame/__init__.py
+-rw-rw-rw-   0        0        0    22552 2023-07-27 18:28:34.000000 gif_pygame-0.1.2/gif_pygame/_pygame_gif.py
+drwxrwxrwx   0        0        0        0 2023-07-27 18:29:43.238626 gif_pygame-0.1.2/gif_pygame.egg-info/
+-rw-rw-rw-   0        0        0     5023 2023-07-27 18:29:43.000000 gif_pygame-0.1.2/gif_pygame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-27 18:29:43.000000 gif_pygame-0.1.2/gif_pygame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 18:29:43.000000 gif_pygame-0.1.2/gif_pygame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-27 18:29:43.000000 gif_pygame-0.1.2/gif_pygame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 18:29:43.000000 gif_pygame-0.1.2/gif_pygame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 18:29:43.240625 gif_pygame-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2023-07-27 18:29:17.000000 gif_pygame-0.1.2/setup.py
```

### Comparing `gif_pygame-0.1.1/LICENSE` & `gif_pygame-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gif_pygame-0.1.1/PKG-INFO` & `gif_pygame-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gif_pygame
-Version: 0.1.1
+Version: 0.1.2
 Summary: A pygame addon for animated image files
 Author: Zeperox
 Keywords: python,pygame,addon,image,animation,animated images
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gif_pygame-0.1.1/README.md` & `gif_pygame-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gif_pygame-0.1.1/gif_pygame/_pygame_gif.py` & `gif_pygame-0.1.2/gif_pygame/_pygame_gif.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             self.gif.seek(frame)
             if frame == 0:
                 if "duration" in self.gif.info:
                     self.frames.append([pygame.image.load(filepath), self.gif.info["duration"]*.001])
                 else:
                     self.frames.append([pygame.image.load(filepath), 1])
             else:
-                self.frames.append([pygame.image.fromstring(self.gif.tobytes(), self.gif.size, self.gif.mode), self.gif.info["duration"]*.001])
+                self.frames.append([pygame.image.frombytes(self.gif.tobytes(), self.gif.size, self.gif.mode), self.gif.info["duration"]*.001])
         
         self.gif.close()
         self.frame = 0
         self.frame_time = 0
         self.paused_time = 0
         self.paused = False
 
@@ -481,15 +481,15 @@
                 self.gif.seek(frame)
                 if frame == 0:
                     if "duration" in self.gif.info:
                         self.frames.append((pygame.image.load(self.filepath), self.gif.info["duration"]*.001))
                     else:
                         self.frames.append((pygame.image.load(self.filepath), 1))
                 else:
-                    self.frames.append((pygame.image.fromstring(self.gif.tobytes(), self.gif.size, self.gif.mode), self.gif.info["duration"]*.001))
+                    self.frames.append((pygame.image.frombytes(self.gif.tobytes(), self.gif.size, self.gif.mode), self.gif.info["duration"]*.001))
 
             self.gif.close()
 
         self.frame = 0
         self.frame_time = 0
         self.paused_time = 0
         self.paused = False
```

### Comparing `gif_pygame-0.1.1/gif_pygame.egg-info/PKG-INFO` & `gif_pygame-0.1.2/gif_pygame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gif-pygame
-Version: 0.1.1
+Version: 0.1.2
 Summary: A pygame addon for animated image files
 Author: Zeperox
 Keywords: python,pygame,addon,image,animation,animated images
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gif_pygame-0.1.1/setup.py` & `gif_pygame-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as readme:
     LONG_DESCRIPTION = readme.read()
 
 setup(
     name="gif_pygame",
-    version="0.1.1",
+    version="0.1.2",
     author="Zeperox",
     description="A pygame addon for animated image files",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["pygame-ce", "pillow"],
     keywords=["python", "pygame", "addon", "image", "animation", "animated images"],
```

