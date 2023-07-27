# Comparing `tmp/crop_utils-4.3.6.tar.gz` & `tmp/crop_utils-4.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crop_utils-4.3.6.tar", last modified: Fri Jul 14 09:05:53 2023, max compression
+gzip compressed data, was "crop_utils-4.3.7.tar", last modified: Thu Jul 27 03:32:51 2023, max compression
```

## Comparing `crop_utils-4.3.6.tar` & `crop_utils-4.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 09:05:53.595008 crop_utils-4.3.6/
--rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.6/LICENSE
--rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1997 2023-07-14 09:05:53.595008 crop_utils-4.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      910 2023-07-14 09:05:50.000000 crop_utils-4.3.6/README.md
--rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 09:05:53.596012 crop_utils-4.3.6/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-07-14 09:05:50.000000 crop_utils-4.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:05:53.572012 crop_utils-4.3.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 09:05:53.586007 crop_utils-4.3.6/src/crop_utils/
--rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.6/src/crop_utils/__init__.py
--rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.6/src/crop_utils/html_slot_config.py
--rw-rw-rw-   0        0        0    62960 2023-07-14 08:06:39.000000 crop_utils-4.3.6/src/crop_utils/image.py
--rw-rw-rw-   0        0        0    43480 2023-07-06 08:56:09.000000 crop_utils-4.3.6/src/crop_utils/img_crop.py
-drwxrwxrwx   0        0        0        0 2023-07-14 09:05:53.593006 crop_utils-4.3.6/src/crop_utils.egg-info/
--rw-rw-rw-   0        0        0     1997 2023-07-14 09:05:53.000000 crop_utils-4.3.6/src/crop_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-07-14 09:05:53.000000 crop_utils-4.3.6/src/crop_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 09:05:53.000000 crop_utils-4.3.6/src/crop_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-14 09:05:53.000000 crop_utils-4.3.6/src/crop_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 03:32:51.619209 crop_utils-4.3.7/
+-rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.7/LICENSE
+-rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2013 2023-07-27 03:32:51.619209 crop_utils-4.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-07-14 09:05:50.000000 crop_utils-4.3.7/README.md
+-rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 03:32:51.620213 crop_utils-4.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      910 2023-07-27 03:32:31.000000 crop_utils-4.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:32:51.598209 crop_utils-4.3.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 03:32:51.611208 crop_utils-4.3.7/src/crop_utils/
+-rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.7/src/crop_utils/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.7/src/crop_utils/html_slot_config.py
+-rw-rw-rw-   0        0        0    63340 2023-07-27 03:25:11.000000 crop_utils-4.3.7/src/crop_utils/image.py
+-rw-rw-rw-   0        0        0    43505 2023-07-27 02:42:27.000000 crop_utils-4.3.7/src/crop_utils/img_crop.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:32:51.617220 crop_utils-4.3.7/src/crop_utils.egg-info/
+-rw-rw-rw-   0        0        0     2013 2023-07-27 03:32:51.000000 crop_utils-4.3.7/src/crop_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-07-27 03:32:51.000000 crop_utils-4.3.7/src/crop_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 03:32:51.000000 crop_utils-4.3.7/src/crop_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 03:32:51.000000 crop_utils-4.3.7/src/crop_utils.egg-info/top_level.txt
```

### Comparing `crop_utils-4.3.6/LICENSE` & `crop_utils-4.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.6/PKG-INFO` & `crop_utils-4.3.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crop_utils
-Version: 4.3.6
-Summary: 鞋类ai识别
+Version: 4.3.7
+Summary: 头顶、脚底裁剪点优化
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
```

### Comparing `crop_utils-4.3.6/README.md` & `crop_utils-4.3.7/README.md`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.6/setup.py` & `crop_utils-4.3.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crop_utils",  # 包名称
-    version="4.3.6",  # 版本号
+    version="4.3.7",  # 版本号
     author="libo",
     author_email="6878595@qq.com",
-    description="鞋类ai识别",
+    description="头顶、脚底裁剪点优化",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://git.chaomy.com/libo/ecpro-utils.git",
     project_urls={
         "Bug Tracker": "https://github.com/pypa/sampleproject/issues",
     },
     classifiers=[
```

### Comparing `crop_utils-4.3.6/src/crop_utils/html_slot_config.py` & `crop_utils-4.3.7/src/crop_utils/html_slot_config.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.6/src/crop_utils/image.py` & `crop_utils-4.3.7/src/crop_utils/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,19 +503,27 @@
             mouth_y = nose_y + (nose_y - eye_y)
             nose_x = ai_crop_point_dict['nose']['top_site'][0]
             ai_crop_point_dict['mouth'] = {
                 'top_site': (nose_x, mouth_y),
                 'bottom_site': (nose_x, mouth_y)
             }
 
-        if 'eye' not in ai_crop_point_dict.keys() and 'nose' not in ai_crop_point_dict.keys() \
-                and not self.head and 'human_top' in ai_crop_point_dict.keys():
+        # if 'eye' not in ai_crop_point_dict.keys() and 'nose' not in ai_crop_point_dict.keys() \
+        #         and not self.head and 'human_top' in ai_crop_point_dict.keys():
+        #     ai_crop_point_dict.pop('human_top')
+        #
+        # if 'ankle' not in ai_crop_point_dict.keys() and 'human_bottom' in ai_crop_point_dict.keys():
+        #     ai_crop_point_dict.pop('human_bottom')
+
+        top_padding = ai_crop_point_dict['human_top']['top_site'][1] * self.image_height
+        if top_padding < 5:
             ai_crop_point_dict.pop('human_top')
 
-        if 'ankle' not in ai_crop_point_dict.keys() and 'human_bottom' in ai_crop_point_dict.keys():
+        bottom_padding = (1 - ai_crop_point_dict['human_bottom']['bottom_site'][1]) * self.image_height
+        if bottom_padding < 5:
             ai_crop_point_dict.pop('human_bottom')
 
         return ai_crop_point_dict
 
     def calculate_mandible_crop_point(self, face, human_keypoint_list):
         """
         在recognition face 内
```

### Comparing `crop_utils-4.3.6/src/crop_utils/img_crop.py` & `crop_utils-4.3.7/src/crop_utils/img_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,16 +232,16 @@
                 crop_parameter.get(RIGHT, 0)) / slot_width
             padding_top, padding_bottom = float(crop_parameter.get(TOP, 0)) / slot_height, float(
                 crop_parameter.get(BOTTOM, 0)) / slot_height
 
         x1 = max(left - padding_left, 0)
         x2 = min(right + padding_right, 1)
 
-        padding_top = (bottom - top) / (1 - padding_top - padding_bottom) * padding_top
-        padding_bottom = (bottom - top) / (1 - padding_top - padding_bottom) * padding_bottom
+        padding_top = (bottom - top) / max((1 - padding_top - padding_bottom) * padding_top, 0.0001)
+        padding_bottom = (bottom - top) / max((1 - padding_top - padding_bottom) * padding_bottom, 0.001)
 
         y1 = max(top - padding_top, 0)
         y2 = min(bottom + padding_bottom, 1)
 
         expand_y1 = top - padding_top
         expand_y2 = bottom + padding_bottom
```

### Comparing `crop_utils-4.3.6/src/crop_utils.egg-info/PKG-INFO` & `crop_utils-4.3.7/src/crop_utils.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crop-utils
-Version: 4.3.6
-Summary: 鞋类ai识别
+Version: 4.3.7
+Summary: 头顶、脚底裁剪点优化
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
```

