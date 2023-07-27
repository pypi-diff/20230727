# Comparing `tmp/teeworlds_player_color_value_to_rgb-1.0.0.tar.gz` & `tmp/teeworlds_player_color_value_to_rgb-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teeworlds_player_color_value_to_rgb-1.0.0.tar", last modified: Thu Jul 27 19:35:54 2023, max compression
+gzip compressed data, was "teeworlds_player_color_value_to_rgb-1.0.1.tar", last modified: Thu Jul 27 19:40:50 2023, max compression
```

## Comparing `teeworlds_player_color_value_to_rgb-1.0.0.tar` & `teeworlds_player_color_value_to_rgb-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:35:54.546519 teeworlds_player_color_value_to_rgb-1.0.0/
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      320 2023-07-27 19:35:54.546519 teeworlds_player_color_value_to_rgb-1.0.0/PKG-INFO
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       38 2023-07-27 19:35:54.546519 teeworlds_player_color_value_to_rgb-1.0.0/setup.cfg
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      631 2023-07-27 19:27:16.000000 teeworlds_player_color_value_to_rgb-1.0.0/setup.py
-drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:35:54.545519 teeworlds_player_color_value_to_rgb-1.0.0/teeworlds_player_color_value_to_rgb/
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      770 2023-07-27 19:29:37.000000 teeworlds_player_color_value_to_rgb-1.0.0/teeworlds_player_color_value_to_rgb/__init__.py
-drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:35:54.546519 teeworlds_player_color_value_to_rgb-1.0.0/teeworlds_player_color_value_to_rgb.egg-info/
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      320 2023-07-27 19:35:54.000000 teeworlds_player_color_value_to_rgb-1.0.0/teeworlds_player_color_value_to_rgb.egg-info/PKG-INFO
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      354 2023-07-27 19:35:54.000000 teeworlds_player_color_value_to_rgb-1.0.0/teeworlds_player_color_value_to_rgb.egg-info/SOURCES.txt
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)        1 2023-07-27 19:35:54.000000 teeworlds_player_color_value_to_rgb-1.0.0/teeworlds_player_color_value_to_rgb.egg-info/dependency_links.txt
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       82 2023-07-27 19:35:54.000000 teeworlds_player_color_value_to_rgb-1.0.0/teeworlds_player_color_value_to_rgb.egg-info/entry_points.txt
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       36 2023-07-27 19:35:54.000000 teeworlds_player_color_value_to_rgb-1.0.0/teeworlds_player_color_value_to_rgb.egg-info/top_level.txt
+drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:40:50.001724 teeworlds_player_color_value_to_rgb-1.0.1/
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      320 2023-07-27 19:40:50.000724 teeworlds_player_color_value_to_rgb-1.0.1/PKG-INFO
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       38 2023-07-27 19:40:50.001724 teeworlds_player_color_value_to_rgb-1.0.1/setup.cfg
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      631 2023-07-27 19:40:16.000000 teeworlds_player_color_value_to_rgb-1.0.1/setup.py
+drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:40:50.000724 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb/
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      824 2023-07-27 19:39:36.000000 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb/__init__.py
+drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:40:50.000724 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb.egg-info/
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      320 2023-07-27 19:40:49.000000 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb.egg-info/PKG-INFO
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      354 2023-07-27 19:40:49.000000 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb.egg-info/SOURCES.txt
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)        1 2023-07-27 19:40:49.000000 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb.egg-info/dependency_links.txt
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       82 2023-07-27 19:40:49.000000 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb.egg-info/entry_points.txt
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       36 2023-07-27 19:40:49.000000 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb.egg-info/top_level.txt
```

### Comparing `teeworlds_player_color_value_to_rgb-1.0.0/setup.py` & `teeworlds_player_color_value_to_rgb-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # !/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='teeworlds_player_color_value_to_rgb',
-    version='1.0.0',
+    version='1.0.1',
     author='XCWQW233',
     author_email='3539757707@qq.com',
     url='https://github.com/XCWQW1/teeworlds_player_color_value_to_rgb',
     description=u'吧teeworlds/ddnet中有关颜色的值转换到RGB(Convert the value of the color in teeworlds/ddnet to RGB)',
     packages=['teeworlds_player_color_value_to_rgb'],
     install_requires=[],
     entry_points={
```

### Comparing `teeworlds_player_color_value_to_rgb-1.0.0/teeworlds_player_color_value_to_rgb/__init__.py` & `teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # !/usr/bin/env python
 # coding: utf-8
 import math
 import colorsys
+from typing import Tuple
 
 
-def value_to_rgb(value):
+def value_to_rgb(value: int) -> tuple[int, int, int]:
     def hsl_to_rgb(h, s, l):
         # 将h, s, l的值范围映射到0到1之间
         h /= 360.0
         s /= 100.0
         l /= 100.0
 
         # 调用colorsys模块函数进行转换
```

