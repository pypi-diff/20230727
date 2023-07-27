# Comparing `tmp/teeworlds_player_color_value_to_rgb-1.0.1.tar.gz` & `tmp/teeworlds_player_color_value_to_rgb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teeworlds_player_color_value_to_rgb-1.0.1.tar", last modified: Thu Jul 27 19:40:50 2023, max compression
+gzip compressed data, was "teeworlds_player_color_value_to_rgb-1.0.2.tar", last modified: Thu Jul 27 19:47:43 2023, max compression
```

## Comparing `teeworlds_player_color_value_to_rgb-1.0.1.tar` & `teeworlds_player_color_value_to_rgb-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:40:50.001724 teeworlds_player_color_value_to_rgb-1.0.1/
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      320 2023-07-27 19:40:50.000724 teeworlds_player_color_value_to_rgb-1.0.1/PKG-INFO
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       38 2023-07-27 19:40:50.001724 teeworlds_player_color_value_to_rgb-1.0.1/setup.cfg
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      631 2023-07-27 19:40:16.000000 teeworlds_player_color_value_to_rgb-1.0.1/setup.py
-drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:40:50.000724 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb/
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      824 2023-07-27 19:39:36.000000 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb/__init__.py
-drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:40:50.000724 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb.egg-info/
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      320 2023-07-27 19:40:49.000000 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb.egg-info/PKG-INFO
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      354 2023-07-27 19:40:49.000000 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb.egg-info/SOURCES.txt
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)        1 2023-07-27 19:40:49.000000 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb.egg-info/dependency_links.txt
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       82 2023-07-27 19:40:49.000000 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb.egg-info/entry_points.txt
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       36 2023-07-27 19:40:49.000000 teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb.egg-info/top_level.txt
+drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:47:43.544611 teeworlds_player_color_value_to_rgb-1.0.2/
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)     1025 2023-07-27 19:47:43.544611 teeworlds_player_color_value_to_rgb-1.0.2/PKG-INFO
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      664 2023-07-27 19:45:13.000000 teeworlds_player_color_value_to_rgb-1.0.2/README.md
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       38 2023-07-27 19:47:43.544611 teeworlds_player_color_value_to_rgb-1.0.2/setup.cfg
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      729 2023-07-27 19:47:36.000000 teeworlds_player_color_value_to_rgb-1.0.2/setup.py
+drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:47:43.543611 teeworlds_player_color_value_to_rgb-1.0.2/teeworlds_player_color_value_to_rgb/
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      824 2023-07-27 19:39:36.000000 teeworlds_player_color_value_to_rgb-1.0.2/teeworlds_player_color_value_to_rgb/__init__.py
+drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:47:43.544611 teeworlds_player_color_value_to_rgb-1.0.2/teeworlds_player_color_value_to_rgb.egg-info/
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)     1025 2023-07-27 19:47:43.000000 teeworlds_player_color_value_to_rgb-1.0.2/teeworlds_player_color_value_to_rgb.egg-info/PKG-INFO
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      364 2023-07-27 19:47:43.000000 teeworlds_player_color_value_to_rgb-1.0.2/teeworlds_player_color_value_to_rgb.egg-info/SOURCES.txt
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)        1 2023-07-27 19:47:43.000000 teeworlds_player_color_value_to_rgb-1.0.2/teeworlds_player_color_value_to_rgb.egg-info/dependency_links.txt
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       82 2023-07-27 19:47:43.000000 teeworlds_player_color_value_to_rgb-1.0.2/teeworlds_player_color_value_to_rgb.egg-info/entry_points.txt
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       36 2023-07-27 19:47:43.000000 teeworlds_player_color_value_to_rgb-1.0.2/teeworlds_player_color_value_to_rgb.egg-info/top_level.txt
```

### Comparing `teeworlds_player_color_value_to_rgb-1.0.1/setup.py` & `teeworlds_player_color_value_to_rgb-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # !/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='teeworlds_player_color_value_to_rgb',
-    version='1.0.1',
+    version='1.0.2',
     author='XCWQW233',
     author_email='3539757707@qq.com',
     url='https://github.com/XCWQW1/teeworlds_player_color_value_to_rgb',
     description=u'吧teeworlds/ddnet中有关颜色的值转换到RGB(Convert the value of the color in teeworlds/ddnet to RGB)',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     packages=['teeworlds_player_color_value_to_rgb'],
     install_requires=[],
     entry_points={
         'console_scripts': [
             'value_to_rgb=teeworlds_player_color_value_to_rgb:value_to_rgb'
         ]
     }
```

### Comparing `teeworlds_player_color_value_to_rgb-1.0.1/teeworlds_player_color_value_to_rgb/__init__.py` & `teeworlds_player_color_value_to_rgb-1.0.2/teeworlds_player_color_value_to_rgb/__init__.py`

 * *Files identical despite different names*

