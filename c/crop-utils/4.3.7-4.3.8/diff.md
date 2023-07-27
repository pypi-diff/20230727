# Comparing `tmp/crop_utils-4.3.7.tar.gz` & `tmp/crop_utils-4.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crop_utils-4.3.7.tar", last modified: Thu Jul 27 03:32:51 2023, max compression
+gzip compressed data, was "crop_utils-4.3.8.tar", last modified: Thu Jul 27 03:37:13 2023, max compression
```

## Comparing `crop_utils-4.3.7.tar` & `crop_utils-4.3.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 03:32:51.619209 crop_utils-4.3.7/
--rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.7/LICENSE
--rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2013 2023-07-27 03:32:51.619209 crop_utils-4.3.7/PKG-INFO
--rw-rw-rw-   0        0        0      910 2023-07-14 09:05:50.000000 crop_utils-4.3.7/README.md
--rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 03:32:51.620213 crop_utils-4.3.7/setup.cfg
--rw-rw-rw-   0        0        0      910 2023-07-27 03:32:31.000000 crop_utils-4.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 03:32:51.598209 crop_utils-4.3.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 03:32:51.611208 crop_utils-4.3.7/src/crop_utils/
--rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.7/src/crop_utils/__init__.py
--rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.7/src/crop_utils/html_slot_config.py
--rw-rw-rw-   0        0        0    63340 2023-07-27 03:25:11.000000 crop_utils-4.3.7/src/crop_utils/image.py
--rw-rw-rw-   0        0        0    43505 2023-07-27 02:42:27.000000 crop_utils-4.3.7/src/crop_utils/img_crop.py
-drwxrwxrwx   0        0        0        0 2023-07-27 03:32:51.617220 crop_utils-4.3.7/src/crop_utils.egg-info/
--rw-rw-rw-   0        0        0     2013 2023-07-27 03:32:51.000000 crop_utils-4.3.7/src/crop_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-07-27 03:32:51.000000 crop_utils-4.3.7/src/crop_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 03:32:51.000000 crop_utils-4.3.7/src/crop_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-27 03:32:51.000000 crop_utils-4.3.7/src/crop_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 03:37:13.264086 crop_utils-4.3.8/
+-rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.8/LICENSE
+-rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2013 2023-07-27 03:37:13.263083 crop_utils-4.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-07-27 03:37:09.000000 crop_utils-4.3.8/README.md
+-rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 03:37:13.265089 crop_utils-4.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      910 2023-07-27 03:37:08.000000 crop_utils-4.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:37:13.241086 crop_utils-4.3.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 03:37:13.255083 crop_utils-4.3.8/src/crop_utils/
+-rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.8/src/crop_utils/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.8/src/crop_utils/html_slot_config.py
+-rw-rw-rw-   0        0        0    63399 2023-07-27 03:37:08.000000 crop_utils-4.3.8/src/crop_utils/image.py
+-rw-rw-rw-   0        0        0    43505 2023-07-27 02:42:27.000000 crop_utils-4.3.8/src/crop_utils/img_crop.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:37:13.261082 crop_utils-4.3.8/src/crop_utils.egg-info/
+-rw-rw-rw-   0        0        0     2013 2023-07-27 03:37:13.000000 crop_utils-4.3.8/src/crop_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-07-27 03:37:13.000000 crop_utils-4.3.8/src/crop_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 03:37:13.000000 crop_utils-4.3.8/src/crop_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 03:37:13.000000 crop_utils-4.3.8/src/crop_utils.egg-info/top_level.txt
```

### Comparing `crop_utils-4.3.7/LICENSE` & `crop_utils-4.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.7/PKG-INFO` & `crop_utils-4.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crop_utils
-Version: 4.3.7
+Version: 4.3.8
 Summary: 头顶、脚底裁剪点优化
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==4.3.6 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.8 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `crop_utils-4.3.7/README.md` & `crop_utils-4.3.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -65,8 +65,8 @@
 
 
 
 # 安装
 
 
 
-pip install crop-utils==4.3.6 -i  https://pypi.python.org/simple/
+pip install crop-utils==4.3.8 -i  https://pypi.python.org/simple/
```

### Comparing `crop_utils-4.3.7/setup.py` & `crop_utils-4.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crop_utils",  # 包名称
-    version="4.3.7",  # 版本号
+    version="4.3.8",  # 版本号
     author="libo",
     author_email="6878595@qq.com",
     description="头顶、脚底裁剪点优化",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://git.chaomy.com/libo/ecpro-utils.git",
     project_urls={
```

### Comparing `crop_utils-4.3.7/src/crop_utils/html_slot_config.py` & `crop_utils-4.3.8/src/crop_utils/html_slot_config.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.7/src/crop_utils/image.py` & `crop_utils-4.3.8/src/crop_utils/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,25 +506,26 @@
                 'top_site': (nose_x, mouth_y),
                 'bottom_site': (nose_x, mouth_y)
             }
 
         # if 'eye' not in ai_crop_point_dict.keys() and 'nose' not in ai_crop_point_dict.keys() \
         #         and not self.head and 'human_top' in ai_crop_point_dict.keys():
         #     ai_crop_point_dict.pop('human_top')
-        #
-        # if 'ankle' not in ai_crop_point_dict.keys() and 'human_bottom' in ai_crop_point_dict.keys():
-        #     ai_crop_point_dict.pop('human_bottom')
 
+        if 'ankle' not in ai_crop_point_dict.keys() and 'human_bottom' in ai_crop_point_dict.keys():
+            ai_crop_point_dict.pop('human_bottom')
+
+        # 先修改头顶的逻辑，暂时没时间测脚底的
         top_padding = ai_crop_point_dict['human_top']['top_site'][1] * self.image_height
         if top_padding < 5:
             ai_crop_point_dict.pop('human_top')
 
-        bottom_padding = (1 - ai_crop_point_dict['human_bottom']['bottom_site'][1]) * self.image_height
-        if bottom_padding < 5:
-            ai_crop_point_dict.pop('human_bottom')
+        # bottom_padding = (1 - ai_crop_point_dict['human_bottom']['bottom_site'][1]) * self.image_height
+        # if bottom_padding < 5:
+        #     ai_crop_point_dict.pop('human_bottom')
 
         return ai_crop_point_dict
 
     def calculate_mandible_crop_point(self, face, human_keypoint_list):
         """
         在recognition face 内
         置信度小于0.8不可信
```

### Comparing `crop_utils-4.3.7/src/crop_utils/img_crop.py` & `crop_utils-4.3.8/src/crop_utils/img_crop.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.7/src/crop_utils.egg-info/PKG-INFO` & `crop_utils-4.3.8/src/crop_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crop-utils
-Version: 4.3.7
+Version: 4.3.8
 Summary: 头顶、脚底裁剪点优化
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==4.3.6 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.8 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

