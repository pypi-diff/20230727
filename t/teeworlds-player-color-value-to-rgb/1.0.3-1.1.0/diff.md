# Comparing `tmp/teeworlds_player_color_value_to_rgb-1.0.3.tar.gz` & `tmp/teeworlds_player_color_value_to_rgb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teeworlds_player_color_value_to_rgb-1.0.3.tar", last modified: Thu Jul 27 19:54:59 2023, max compression
+gzip compressed data, was "teeworlds_player_color_value_to_rgb-1.1.0.tar", last modified: Thu Jul 27 20:03:05 2023, max compression
```

## Comparing `teeworlds_player_color_value_to_rgb-1.0.3.tar` & `teeworlds_player_color_value_to_rgb-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:54:59.922437 teeworlds_player_color_value_to_rgb-1.0.3/
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)     1025 2023-07-27 19:54:59.922437 teeworlds_player_color_value_to_rgb-1.0.3/PKG-INFO
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      664 2023-07-27 19:51:05.000000 teeworlds_player_color_value_to_rgb-1.0.3/README.md
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       38 2023-07-27 19:54:59.923437 teeworlds_player_color_value_to_rgb-1.0.3/setup.cfg
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      738 2023-07-27 19:54:51.000000 teeworlds_player_color_value_to_rgb-1.0.3/setup.py
-drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:54:59.922437 teeworlds_player_color_value_to_rgb-1.0.3/teeworlds_player_color_value_to_rgb/
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      824 2023-07-27 19:54:15.000000 teeworlds_player_color_value_to_rgb-1.0.3/teeworlds_player_color_value_to_rgb/__init__.py
-drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 19:54:59.922437 teeworlds_player_color_value_to_rgb-1.0.3/teeworlds_player_color_value_to_rgb.egg-info/
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)     1025 2023-07-27 19:54:59.000000 teeworlds_player_color_value_to_rgb-1.0.3/teeworlds_player_color_value_to_rgb.egg-info/PKG-INFO
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      364 2023-07-27 19:54:59.000000 teeworlds_player_color_value_to_rgb-1.0.3/teeworlds_player_color_value_to_rgb.egg-info/SOURCES.txt
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)        1 2023-07-27 19:54:59.000000 teeworlds_player_color_value_to_rgb-1.0.3/teeworlds_player_color_value_to_rgb.egg-info/dependency_links.txt
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       91 2023-07-27 19:54:59.000000 teeworlds_player_color_value_to_rgb-1.0.3/teeworlds_player_color_value_to_rgb.egg-info/entry_points.txt
--rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       36 2023-07-27 19:54:59.000000 teeworlds_player_color_value_to_rgb-1.0.3/teeworlds_player_color_value_to_rgb.egg-info/top_level.txt
+drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 20:03:05.127132 teeworlds_player_color_value_to_rgb-1.1.0/
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)     1041 2023-07-27 20:03:05.127132 teeworlds_player_color_value_to_rgb-1.1.0/PKG-INFO
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      680 2023-07-27 20:00:46.000000 teeworlds_player_color_value_to_rgb-1.1.0/README.md
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       38 2023-07-27 20:03:05.127132 teeworlds_player_color_value_to_rgb-1.1.0/setup.cfg
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      738 2023-07-27 20:03:00.000000 teeworlds_player_color_value_to_rgb-1.1.0/setup.py
+drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 20:03:05.127132 teeworlds_player_color_value_to_rgb-1.1.0/teeworlds_player_color_value_to_rgb/
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      824 2023-07-27 19:54:15.000000 teeworlds_player_color_value_to_rgb-1.1.0/teeworlds_player_color_value_to_rgb/__init__.py
+drwxr-xr-x   0 xcwqw1    (1000) xcwqw1    (1000)        0 2023-07-27 20:03:05.127132 teeworlds_player_color_value_to_rgb-1.1.0/teeworlds_player_color_value_to_rgb.egg-info/
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)     1041 2023-07-27 20:03:05.000000 teeworlds_player_color_value_to_rgb-1.1.0/teeworlds_player_color_value_to_rgb.egg-info/PKG-INFO
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)      364 2023-07-27 20:03:05.000000 teeworlds_player_color_value_to_rgb-1.1.0/teeworlds_player_color_value_to_rgb.egg-info/SOURCES.txt
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)        1 2023-07-27 20:03:05.000000 teeworlds_player_color_value_to_rgb-1.1.0/teeworlds_player_color_value_to_rgb.egg-info/dependency_links.txt
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       91 2023-07-27 20:03:05.000000 teeworlds_player_color_value_to_rgb-1.1.0/teeworlds_player_color_value_to_rgb.egg-info/entry_points.txt
+-rw-r--r--   0 xcwqw1    (1000) xcwqw1    (1000)       36 2023-07-27 20:03:05.000000 teeworlds_player_color_value_to_rgb-1.1.0/teeworlds_player_color_value_to_rgb.egg-info/top_level.txt
```

### Comparing `teeworlds_player_color_value_to_rgb-1.0.3/PKG-INFO` & `teeworlds_player_color_value_to_rgb-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: teeworlds_player_color_value_to_rgb
-Version: 1.0.3
+Version: 1.1.0
 Summary: 吧teeworlds/ddnet中有关颜色的值转换到RGB(Convert the value of the color in teeworlds/ddnet to RGB)
 Home-page: https://github.com/XCWQW1/teeworlds_player_color_value_to_rgb
 Author: XCWQW233
 Author-email: 3539757707@qq.com
 Description-Content-Type: text/markdown
 
 # teeworlds_player_color_value_to_rgb
 
 吧teeworlds/ddnet中有关颜色的值转换到RGB(Convert the value of the color in teeworlds/ddnet to RGB)
 
 安装(install):
  - `pip install teeworlds_player_color_value_to_rgb`
 
 使用/use:
-> 我使用了py自带的math和colorsys库(I used the math and colorsys libraries that come with py)
+> 我使用了py自带的math，typing和colorsys库(I used the math,typing and colorsys libraries that come with py)
  - ```
    from teeworlds_player_color_value_to_rgb import value_to_rgb
    value = 8624384
    rgb = value_to_rgb(value)
    print(rgb)
    ```
```

### Comparing `teeworlds_player_color_value_to_rgb-1.0.3/README.md` & `teeworlds_player_color_value_to_rgb-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 吧teeworlds/ddnet中有关颜色的值转换到RGB(Convert the value of the color in teeworlds/ddnet to RGB)
 
 安装(install):
  - `pip install teeworlds_player_color_value_to_rgb`
 
 使用/use:
-> 我使用了py自带的math和colorsys库(I used the math and colorsys libraries that come with py)
+> 我使用了py自带的math，typing和colorsys库(I used the math,typing and colorsys libraries that come with py)
  - ```
    from teeworlds_player_color_value_to_rgb import value_to_rgb
    value = 8624384
    rgb = value_to_rgb(value)
    print(rgb)
    ```
```

### Comparing `teeworlds_player_color_value_to_rgb-1.0.3/setup.py` & `teeworlds_player_color_value_to_rgb-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # !/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='teeworlds_player_color_value_to_rgb',
-    version='1.0.3',
+    version='1.1.0',
     author='XCWQW233',
     author_email='3539757707@qq.com',
     url='https://github.com/XCWQW1/teeworlds_player_color_value_to_rgb',
     description=u'吧teeworlds/ddnet中有关颜色的值转换到RGB(Convert the value of the color in teeworlds/ddnet to RGB)',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=['teeworlds_player_color_value_to_rgb'],
```

### Comparing `teeworlds_player_color_value_to_rgb-1.0.3/teeworlds_player_color_value_to_rgb/__init__.py` & `teeworlds_player_color_value_to_rgb-1.1.0/teeworlds_player_color_value_to_rgb/__init__.py`

 * *Files identical despite different names*

### Comparing `teeworlds_player_color_value_to_rgb-1.0.3/teeworlds_player_color_value_to_rgb.egg-info/PKG-INFO` & `teeworlds_player_color_value_to_rgb-1.1.0/teeworlds_player_color_value_to_rgb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: teeworlds-player-color-value-to-rgb
-Version: 1.0.3
+Version: 1.1.0
 Summary: 吧teeworlds/ddnet中有关颜色的值转换到RGB(Convert the value of the color in teeworlds/ddnet to RGB)
 Home-page: https://github.com/XCWQW1/teeworlds_player_color_value_to_rgb
 Author: XCWQW233
 Author-email: 3539757707@qq.com
 Description-Content-Type: text/markdown
 
 # teeworlds_player_color_value_to_rgb
 
 吧teeworlds/ddnet中有关颜色的值转换到RGB(Convert the value of the color in teeworlds/ddnet to RGB)
 
 安装(install):
  - `pip install teeworlds_player_color_value_to_rgb`
 
 使用/use:
-> 我使用了py自带的math和colorsys库(I used the math and colorsys libraries that come with py)
+> 我使用了py自带的math，typing和colorsys库(I used the math,typing and colorsys libraries that come with py)
  - ```
    from teeworlds_player_color_value_to_rgb import value_to_rgb
    value = 8624384
    rgb = value_to_rgb(value)
    print(rgb)
    ```
```

