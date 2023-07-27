# Comparing `tmp/crop_utils-4.3.8.tar.gz` & `tmp/crop_utils-4.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crop_utils-4.3.8.tar", last modified: Thu Jul 27 03:37:13 2023, max compression
+gzip compressed data, was "crop_utils-4.3.9.tar", last modified: Thu Jul 27 07:33:14 2023, max compression
```

## Comparing `crop_utils-4.3.8.tar` & `crop_utils-4.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 03:37:13.264086 crop_utils-4.3.8/
--rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.8/LICENSE
--rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2013 2023-07-27 03:37:13.263083 crop_utils-4.3.8/PKG-INFO
--rw-rw-rw-   0        0        0      910 2023-07-27 03:37:09.000000 crop_utils-4.3.8/README.md
--rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 03:37:13.265089 crop_utils-4.3.8/setup.cfg
--rw-rw-rw-   0        0        0      910 2023-07-27 03:37:08.000000 crop_utils-4.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 03:37:13.241086 crop_utils-4.3.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 03:37:13.255083 crop_utils-4.3.8/src/crop_utils/
--rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.8/src/crop_utils/__init__.py
--rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.8/src/crop_utils/html_slot_config.py
--rw-rw-rw-   0        0        0    63399 2023-07-27 03:37:08.000000 crop_utils-4.3.8/src/crop_utils/image.py
--rw-rw-rw-   0        0        0    43505 2023-07-27 02:42:27.000000 crop_utils-4.3.8/src/crop_utils/img_crop.py
-drwxrwxrwx   0        0        0        0 2023-07-27 03:37:13.261082 crop_utils-4.3.8/src/crop_utils.egg-info/
--rw-rw-rw-   0        0        0     2013 2023-07-27 03:37:13.000000 crop_utils-4.3.8/src/crop_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-07-27 03:37:13.000000 crop_utils-4.3.8/src/crop_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 03:37:13.000000 crop_utils-4.3.8/src/crop_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-27 03:37:13.000000 crop_utils-4.3.8/src/crop_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 07:33:14.747856 crop_utils-4.3.9/
+-rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.9/LICENSE
+-rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2004 2023-07-27 07:33:14.746857 crop_utils-4.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-07-27 07:33:06.000000 crop_utils-4.3.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 07:33:14.747856 crop_utils-4.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      901 2023-07-27 07:33:06.000000 crop_utils-4.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:33:14.725866 crop_utils-4.3.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 07:33:14.738864 crop_utils-4.3.9/src/crop_utils/
+-rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.9/src/crop_utils/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.9/src/crop_utils/html_slot_config.py
+-rw-rw-rw-   0        0        0    63399 2023-07-27 03:37:08.000000 crop_utils-4.3.9/src/crop_utils/image.py
+-rw-rw-rw-   0        0        0    43502 2023-07-27 07:32:32.000000 crop_utils-4.3.9/src/crop_utils/img_crop.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:33:14.745856 crop_utils-4.3.9/src/crop_utils.egg-info/
+-rw-rw-rw-   0        0        0     2004 2023-07-27 07:33:14.000000 crop_utils-4.3.9/src/crop_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-07-27 07:33:14.000000 crop_utils-4.3.9/src/crop_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 07:33:14.000000 crop_utils-4.3.9/src/crop_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 07:33:14.000000 crop_utils-4.3.9/src/crop_utils.egg-info/top_level.txt
```

### Comparing `crop_utils-4.3.8/LICENSE` & `crop_utils-4.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.8/PKG-INFO` & `crop_utils-4.3.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crop_utils
-Version: 4.3.8
-Summary: 头顶、脚底裁剪点优化
+Version: 4.3.9
+Summary: 头顶裁剪点优化
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
         
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==4.3.8 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.9 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `crop_utils-4.3.8/README.md` & `crop_utils-4.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,8 +65,8 @@
 
 
 
 # 安装
 
 
 
-pip install crop-utils==4.3.8 -i  https://pypi.python.org/simple/
+pip install crop-utils==4.3.9 -i  https://pypi.python.org/simple/
```

### Comparing `crop_utils-4.3.8/setup.py` & `crop_utils-4.3.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crop_utils",  # 包名称
-    version="4.3.8",  # 版本号
+    version="4.3.9",  # 版本号
     author="libo",
     author_email="6878595@qq.com",
-    description="头顶、脚底裁剪点优化",
+    description="头顶裁剪点优化",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://git.chaomy.com/libo/ecpro-utils.git",
     project_urls={
         "Bug Tracker": "https://github.com/pypa/sampleproject/issues",
     },
     classifiers=[
```

### Comparing `crop_utils-4.3.8/src/crop_utils/html_slot_config.py` & `crop_utils-4.3.9/src/crop_utils/html_slot_config.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.8/src/crop_utils/image.py` & `crop_utils-4.3.9/src/crop_utils/image.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.8/src/crop_utils/img_crop.py` & `crop_utils-4.3.9/src/crop_utils/img_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,16 +232,16 @@
                 crop_parameter.get(RIGHT, 0)) / slot_width
             padding_top, padding_bottom = float(crop_parameter.get(TOP, 0)) / slot_height, float(
                 crop_parameter.get(BOTTOM, 0)) / slot_height
 
         x1 = max(left - padding_left, 0)
         x2 = min(right + padding_right, 1)
 
-        padding_top = (bottom - top) / max((1 - padding_top - padding_bottom) * padding_top, 0.0001)
-        padding_bottom = (bottom - top) / max((1 - padding_top - padding_bottom) * padding_bottom, 0.001)
+        padding_top = (bottom - top) / max((1 - padding_top - padding_bottom), 0.01) * padding_top
+        padding_bottom = (bottom - top) / max((1 - padding_top - padding_bottom), 0.01) * padding_bottom
 
         y1 = max(top - padding_top, 0)
         y2 = min(bottom + padding_bottom, 1)
 
         expand_y1 = top - padding_top
         expand_y2 = bottom + padding_bottom
```

### Comparing `crop_utils-4.3.8/src/crop_utils.egg-info/PKG-INFO` & `crop_utils-4.3.9/src/crop_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crop-utils
-Version: 4.3.8
-Summary: 头顶、脚底裁剪点优化
+Version: 4.3.9
+Summary: 头顶裁剪点优化
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
         
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==4.3.8 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.9 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

