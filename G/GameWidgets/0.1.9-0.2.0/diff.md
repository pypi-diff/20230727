# Comparing `tmp/GameWidgets-0.1.9.tar.gz` & `tmp/GameWidgets-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameWidgets-0.1.9.tar", last modified: Fri Jul 14 00:38:17 2023, max compression
+gzip compressed data, was "GameWidgets-0.2.0.tar", last modified: Thu Jul 27 21:18:53 2023, max compression
```

## Comparing `GameWidgets-0.1.9.tar` & `GameWidgets-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,62 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.433046 GameWidgets-0.1.9/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.421047 GameWidgets-0.1.9/GameWidgets/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.421047 GameWidgets-0.1.9/GameWidgets/Assets/
--rw-------   0 runner    (1000) runner    (1000)        0 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/Assets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     5845 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/Constants.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.425047 GameWidgets-0.1.9/GameWidgets/Engine/
--rw-------   0 runner    (1000) runner    (1000)     1011 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Engine/Backdrop.py
--rw-------   0 runner    (1000) runner    (1000)     1211 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Engine/Entity.py
--rw-------   0 runner    (1000) runner    (1000)     1607 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Engine/Group.py
--rw-------   0 runner    (1000) runner    (1000)     1082 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Engine/Manager.py
--rw-------   0 runner    (1000) runner    (1000)      164 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Engine/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.425047 GameWidgets-0.1.9/GameWidgets/Examples/
--rw-------   0 runner    (1000) runner    (1000)     1758 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
--rw-------   0 runner    (1000) runner    (1000)        4 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Examples/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.425047 GameWidgets-0.1.9/GameWidgets/GameWidgets/
--rw-------   0 runner    (1000) runner    (1000)     1422 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/Animatrix.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.425047 GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/
--rw-------   0 runner    (1000) runner    (1000)     1497 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/Button.py
--rw-------   0 runner    (1000) runner    (1000)     1404 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/Joystick.py
--rw-------   0 runner    (1000) runner    (1000)       13 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/R1_R2.py
--rw-------   0 runner    (1000) runner    (1000)      148 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      735 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/Draw.py
--rw-------   0 runner    (1000) runner    (1000)      652 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/ScreenSlide.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.425047 GameWidgets-0.1.9/GameWidgets/GameWidgets/TileMaps/
--rw-------   0 runner    (1000) runner    (1000)      424 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/TileMaps/Sprite.py
--rw-------   0 runner    (1000) runner    (1000)      703 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/TileMaps/Tile.py
--rw-------   0 runner    (1000) runner    (1000)      124 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/TileMaps/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      121 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/GameWidgets/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.429046 GameWidgets-0.1.9/GameWidgets/RuntimeTests/
--rw-------   0 runner    (1000) runner    (1000)      649 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/RuntimeTests/AllTest.py
--rw-------   0 runner    (1000) runner    (1000)      397 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/RuntimeTests/GameWidgetTest.py
--rw-------   0 runner    (1000) runner    (1000)      359 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/RuntimeTests/SetUpTest.py
--rw-------   0 runner    (1000) runner    (1000)      369 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/RuntimeTests/WidgetTest.py
--rw-------   0 runner    (1000) runner    (1000)        4 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/RuntimeTests/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.429046 GameWidgets-0.1.9/GameWidgets/SetUp/
--rw-------   0 runner    (1000) runner    (1000)     1689 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/SetUp/ScreenCommands.py
--rw-------   0 runner    (1000) runner    (1000)      109 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/SetUp/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.433046 GameWidgets-0.1.9/GameWidgets/Widgets/
--rw-------   0 runner    (1000) runner    (1000)     3691 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/Widgets/Btn.py
--rw-------   0 runner    (1000) runner    (1000)      597 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/Widgets/Clock.py
--rw-------   0 runner    (1000) runner    (1000)     1489 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/Widgets/Cursor.py
--rw-------   0 runner    (1000) runner    (1000)     2761 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/Widgets/DialogeBox.py
--rw-------   0 runner    (1000) runner    (1000)     1574 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Widgets/ImgDecoder.py
--rw-------   0 runner    (1000) runner    (1000)      246 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Widgets/Sound.py
--rw-------   0 runner    (1000) runner    (1000)     1876 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Widgets/TextInp.py
--rw-------   0 runner    (1000) runner    (1000)     2807 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Widgets/ToggleBtn.py
--rw-------   0 runner    (1000) runner    (1000)      201 2023-07-14 00:37:57.000000 GameWidgets-0.1.9/GameWidgets/Widgets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      116 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      567 2023-07-14 00:37:56.000000 GameWidgets-0.1.9/GameWidgets/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 00:38:17.421047 GameWidgets-0.1.9/GameWidgets.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1823 2023-07-14 00:38:17.000000 GameWidgets-0.1.9/GameWidgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1523 2023-07-14 00:38:17.000000 GameWidgets-0.1.9/GameWidgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-14 00:38:17.000000 GameWidgets-0.1.9/GameWidgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-07-14 00:38:17.000000 GameWidgets-0.1.9/GameWidgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-14 00:38:17.000000 GameWidgets-0.1.9/GameWidgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1823 2023-07-14 00:38:17.433046 GameWidgets-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      385 2022-09-11 21:19:38.000000 GameWidgets-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-14 00:38:17.433046 GameWidgets-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 21:18:53.195726 GameWidgets-0.2.0/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 21:18:53.123719 GameWidgets-0.2.0/GameWidgets/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 21:18:53.123719 GameWidgets-0.2.0/GameWidgets/Assets/
+-rw-------   0 runner    (1000) runner    (1000)        0 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Assets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     5845 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Constants.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 21:18:53.127719 GameWidgets-0.2.0/GameWidgets/Engine/
+-rw-------   0 runner    (1000) runner    (1000)     1011 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Engine/Backdrop.py
+-rw-------   0 runner    (1000) runner    (1000)     1446 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Engine/Entity.py
+-rw-------   0 runner    (1000) runner    (1000)     1609 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Engine/Group.py
+-rw-------   0 runner    (1000) runner    (1000)     1104 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Engine/Manager.py
+-rw-------   0 runner    (1000) runner    (1000)     1211 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Engine/Object.py
+-rw-------   0 runner    (1000) runner    (1000)     5566 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Engine/ParticleEffect.py
+-rw-------   0 runner    (1000) runner    (1000)     1214 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Engine/ScreenShade.py
+-rw-------   0 runner    (1000) runner    (1000)      164 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Engine/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 21:18:53.127719 GameWidgets-0.2.0/GameWidgets/Examples/
+-rw-------   0 runner    (1000) runner    (1000)     1541 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Examples/ParticleEffectExample.py
+-rw-------   0 runner    (1000) runner    (1000)     1758 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
+-rw-------   0 runner    (1000) runner    (1000)     1690 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Examples/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 21:18:53.131720 GameWidgets-0.2.0/GameWidgets/GameWidgets/
+-rw-------   0 runner    (1000) runner    (1000)     1422 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/GameWidgets/Animatrix.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 21:18:53.131720 GameWidgets-0.2.0/GameWidgets/GameWidgets/Controller/
+-rw-------   0 runner    (1000) runner    (1000)     1497 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/GameWidgets/Controller/Button.py
+-rw-------   0 runner    (1000) runner    (1000)     1404 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/GameWidgets/Controller/Joystick.py
+-rw-------   0 runner    (1000) runner    (1000)       13 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/GameWidgets/Controller/R1_R2.py
+-rw-------   0 runner    (1000) runner    (1000)      148 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/GameWidgets/Controller/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      735 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/GameWidgets/Draw.py
+-rw-------   0 runner    (1000) runner    (1000)      652 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/GameWidgets/ScreenSlide.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 21:18:53.183725 GameWidgets-0.2.0/GameWidgets/GameWidgets/TileMaps/
+-rw-------   0 runner    (1000) runner    (1000)      424 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/GameWidgets/TileMaps/Sprite.py
+-rw-------   0 runner    (1000) runner    (1000)      703 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/GameWidgets/TileMaps/Tile.py
+-rw-------   0 runner    (1000) runner    (1000)      124 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/GameWidgets/TileMaps/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      121 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/GameWidgets/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 21:18:53.183725 GameWidgets-0.2.0/GameWidgets/RuntimeTests/
+-rw-------   0 runner    (1000) runner    (1000)      649 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/RuntimeTests/AllTest.py
+-rw-------   0 runner    (1000) runner    (1000)      397 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/RuntimeTests/GameWidgetTest.py
+-rw-------   0 runner    (1000) runner    (1000)      359 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/RuntimeTests/SetUpTest.py
+-rw-------   0 runner    (1000) runner    (1000)      369 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/RuntimeTests/WidgetTest.py
+-rw-------   0 runner    (1000) runner    (1000)        4 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/RuntimeTests/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 21:18:53.187725 GameWidgets-0.2.0/GameWidgets/SetUp/
+-rw-------   0 runner    (1000) runner    (1000)     1689 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/SetUp/ScreenCommands.py
+-rw-------   0 runner    (1000) runner    (1000)      109 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/SetUp/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 21:18:53.191725 GameWidgets-0.2.0/GameWidgets/Widgets/
+-rw-------   0 runner    (1000) runner    (1000)     3691 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Widgets/Btn.py
+-rw-------   0 runner    (1000) runner    (1000)      597 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Widgets/Clock.py
+-rw-------   0 runner    (1000) runner    (1000)     1489 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Widgets/Cursor.py
+-rw-------   0 runner    (1000) runner    (1000)     2761 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Widgets/DialogueBox.py
+-rw-------   0 runner    (1000) runner    (1000)     1574 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Widgets/ImgDecoder.py
+-rw-------   0 runner    (1000) runner    (1000)      246 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Widgets/Sound.py
+-rw-------   0 runner    (1000) runner    (1000)     1876 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Widgets/TextInp.py
+-rw-------   0 runner    (1000) runner    (1000)     2807 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Widgets/ToggleBtn.py
+-rw-------   0 runner    (1000) runner    (1000)      164 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/Widgets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      116 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      570 2023-07-27 21:16:25.000000 GameWidgets-0.2.0/GameWidgets/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-27 21:18:53.123719 GameWidgets-0.2.0/GameWidgets.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1519 2023-07-27 21:18:52.000000 GameWidgets-0.2.0/GameWidgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1670 2023-07-27 21:18:53.000000 GameWidgets-0.2.0/GameWidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-27 21:18:52.000000 GameWidgets-0.2.0/GameWidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2023-07-27 21:18:52.000000 GameWidgets-0.2.0/GameWidgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-27 21:18:52.000000 GameWidgets-0.2.0/GameWidgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1519 2023-07-27 21:18:53.195726 GameWidgets-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      385 2022-09-11 21:19:38.000000 GameWidgets-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-27 21:18:53.195726 GameWidgets-0.2.0/setup.cfg
```

### Comparing `GameWidgets-0.1.9/GameWidgets/Constants.py` & `GameWidgets-0.2.0/GameWidgets/Constants.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/Engine/Backdrop.py` & `GameWidgets-0.2.0/GameWidgets/Engine/Backdrop.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/Engine/Entity.py` & `GameWidgets-0.2.0/GameWidgets/Engine/Object.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pygame
 import time
 
 pygame.init()
 
 
-class Entity:
+class Object:
     def __init__(self,Screen):
         self.frame = 0
         self.stime = 0
         self.ctime = 0
         self.screen = Screen
         self.animationStart = False
         self.xyanituple = (0,0)
```

### Comparing `GameWidgets-0.1.9/GameWidgets/Engine/Group.py` & `GameWidgets-0.2.0/GameWidgets/Engine/Group.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,8 @@
         for i in self.items:
             for iden in i:
                 if iden == identifier:
                     index = self.items.index(i)
         self.items.pop(index)
 
     def Return(self):
-        return self.items
+        return self.items
```

### Comparing `GameWidgets-0.1.9/GameWidgets/Engine/Manager.py` & `GameWidgets-0.2.0/GameWidgets/Engine/Manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import pygame
 
+
 class Manager:
     def __init__(self, screen, *args):
         self.screen = screen
         self.drawlist = []
         for key in args:
             self.drawlist.append(key)
 
-    def ReturnLayer(self, layer:int):
-        return self.drawlist[layer-1]
+    def ReturnLayer(self, layer: int):
+        return self.drawlist[layer - 1]
 
     def Return(self):
         return self.drawlist
 
-    def DeleteLayer(self, layer:int):
-        self.drawlist.pop(layer-1)
+    def DeleteLayer(self, layer: int):
+        self.drawlist.pop(layer - 1)
 
-    def Drawlayer(self,layer:int):
+    def Drawlayer(self, layer: int):
         try:
-            for i in self.drawlist[layer-1]:
+            for i in self.drawlist[layer - 1]:
                 if i[1] != "False":
-                    self.screen.blit(i[2],i[3])
+                    self.screen.blit(i[2], i[3])
         except:
-            for i in self.drawlist[layer-1]:
+            for i in self.drawlist[layer - 1]:
                 if i[1] != "False":
                     i[2].Draw()
 
-    def AddLayer(self,item,index:int):
-        self.drawlist.insert(index,item)
+    def AddLayer(self, item, index: int):
+        self.drawlist.insert(index, item)
 
     def DrawAll(self):
         for i in self.drawlist:
             for thing in i:
                 if thing[1]:
                     try:
-                        self.screen.blit(thing[2],thing[3])
+                        self.screen.blit(thing[2], thing[3])
                     except:
-                        thing[2].Draw()
+                        thing[2].Draw()
```

### Comparing `GameWidgets-0.1.9/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py` & `GameWidgets-0.2.0/GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/GameWidgets/Animatrix.py` & `GameWidgets-0.2.0/GameWidgets/GameWidgets/Animatrix.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/Button.py` & `GameWidgets-0.2.0/GameWidgets/GameWidgets/Controller/Button.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/GameWidgets/Controller/Joystick.py` & `GameWidgets-0.2.0/GameWidgets/GameWidgets/Controller/Joystick.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/GameWidgets/Draw.py` & `GameWidgets-0.2.0/GameWidgets/GameWidgets/Draw.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/GameWidgets/ScreenSlide.py` & `GameWidgets-0.2.0/GameWidgets/GameWidgets/ScreenSlide.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/GameWidgets/TileMaps/Tile.py` & `GameWidgets-0.2.0/GameWidgets/GameWidgets/TileMaps/Tile.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/RuntimeTests/AllTest.py` & `GameWidgets-0.2.0/GameWidgets/RuntimeTests/AllTest.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/SetUp/ScreenCommands.py` & `GameWidgets-0.2.0/GameWidgets/SetUp/ScreenCommands.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/Widgets/Btn.py` & `GameWidgets-0.2.0/GameWidgets/Widgets/Btn.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/Widgets/Clock.py` & `GameWidgets-0.2.0/GameWidgets/Widgets/Clock.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/Widgets/Cursor.py` & `GameWidgets-0.2.0/GameWidgets/Widgets/Cursor.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/Widgets/DialogeBox.py` & `GameWidgets-0.2.0/GameWidgets/Widgets/DialogueBox.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/Widgets/ImgDecoder.py` & `GameWidgets-0.2.0/GameWidgets/Widgets/ImgDecoder.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/Widgets/TextInp.py` & `GameWidgets-0.2.0/GameWidgets/Widgets/TextInp.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/Widgets/ToggleBtn.py` & `GameWidgets-0.2.0/GameWidgets/Widgets/ToggleBtn.py`

 * *Files identical despite different names*

### Comparing `GameWidgets-0.1.9/GameWidgets/setup.py` & `GameWidgets-0.2.0/GameWidgets/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
   
 with open("GameWidgets/README.md", "r") as fh:
     description = fh.read()
   
 setup(
     name="GameWidgets",
-    version="0.1.9",
+    version="0.2.0",
     author="Manomay tyagi",
     author_email="tyagimanomay57@gmail.com",
     description="Make Game Easier with pygame and GameWidgets",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/SuperGuy123456/GameWidgets",
     license='MIT',
     python_requires='>=3.8',
-    install_requires=['pygame'],
+    install_requires=['pygame-ce'],
     packages=find_packages()
 )
```

### Comparing `GameWidgets-0.1.9/GameWidgets.egg-info/SOURCES.txt` & `GameWidgets-0.2.0/GameWidgets.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 GameWidgets.egg-info/requires.txt
 GameWidgets.egg-info/top_level.txt
 GameWidgets/Assets/__init__.py
 GameWidgets/Engine/Backdrop.py
 GameWidgets/Engine/Entity.py
 GameWidgets/Engine/Group.py
 GameWidgets/Engine/Manager.py
+GameWidgets/Engine/Object.py
+GameWidgets/Engine/ParticleEffect.py
+GameWidgets/Engine/ScreenShade.py
 GameWidgets/Engine/__init__.py
+GameWidgets/Examples/ParticleEffectExample.py
 GameWidgets/Examples/Widget_Screen_GameWidgets_Example.py
 GameWidgets/Examples/__init__.py
 GameWidgets/GameWidgets/Animatrix.py
 GameWidgets/GameWidgets/Draw.py
 GameWidgets/GameWidgets/ScreenSlide.py
 GameWidgets/GameWidgets/__init__.py
 GameWidgets/GameWidgets/Controller/Button.py
@@ -32,13 +36,13 @@
 GameWidgets/RuntimeTests/WidgetTest.py
 GameWidgets/RuntimeTests/__init__.py
 GameWidgets/SetUp/ScreenCommands.py
 GameWidgets/SetUp/__init__.py
 GameWidgets/Widgets/Btn.py
 GameWidgets/Widgets/Clock.py
 GameWidgets/Widgets/Cursor.py
-GameWidgets/Widgets/DialogeBox.py
+GameWidgets/Widgets/DialogueBox.py
 GameWidgets/Widgets/ImgDecoder.py
 GameWidgets/Widgets/Sound.py
 GameWidgets/Widgets/TextInp.py
 GameWidgets/Widgets/ToggleBtn.py
 GameWidgets/Widgets/__init__.py
```

