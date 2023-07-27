# Comparing `tmp/shapes_recognition-3.1.1.tar.gz` & `tmp/shapes_recognition-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapes_recognition-3.1.1.tar", max compression
+gzip compressed data, was "shapes_recognition-3.1.2.tar", max compression
```

## Comparing `shapes_recognition-3.1.1.tar` & `shapes_recognition-3.1.2.tar`

### file list

```diff
@@ -1,19 +1,36 @@
--rw-r--r--   0        0        0      606 2023-02-16 10:59:45.000000 shapes_recognition-3.1.1/README.md
--rw-r--r--   0        0        0      450 2023-07-21 20:09:54.582790 shapes_recognition-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-07-21 19:25:32.576284 shapes_recognition-3.1.1/shapes_recognition/.DS_Store
--rw-r--r--   0        0        0      231 2023-07-21 14:53:08.313682 shapes_recognition-3.1.1/shapes_recognition/__init__.py
--rw-r--r--   0        0        0     6148 2023-07-21 19:38:34.562667 shapes_recognition-3.1.1/shapes_recognition/src/.DS_Store
--rw-r--r--   0        0        0      926 2023-07-21 15:08:18.604666 shapes_recognition-3.1.1/shapes_recognition/src/cfg.py
--rw-r--r--   0        0        0     2444 2023-07-21 15:08:18.610725 shapes_recognition-3.1.1/shapes_recognition/src/create_joint_table.py
--rw-r--r--   0        0        0     2512 2023-07-21 15:08:18.560495 shapes_recognition-3.1.1/shapes_recognition/src/create_table.py
--rw-r--r--   0        0        0     2068 2023-07-21 15:08:18.598622 shapes_recognition-3.1.1/shapes_recognition/src/create_template.py
--rw-r--r--   0        0        0     1710 2023-07-21 15:08:18.593028 shapes_recognition-3.1.1/shapes_recognition/src/get_column_data.py
--rw-r--r--   0        0        0     2667 2023-07-21 15:08:18.607481 shapes_recognition-3.1.1/shapes_recognition/src/get_peaks.py
--rw-r--r--   0        0        0     5897 2023-07-21 15:08:18.601878 shapes_recognition-3.1.1/shapes_recognition/src/get_results.py
--rw-r--r--   0        0        0     2452 2023-07-21 15:08:18.567925 shapes_recognition-3.1.1/shapes_recognition/src/recognition.py
--rw-r--r--   0        0        0     1648 2023-07-21 15:12:32.259774 shapes_recognition-3.1.1/shapes_recognition/src/save_results.py
--rw-r--r--   0        0        0     4124 2023-07-21 15:12:32.281959 shapes_recognition-3.1.1/shapes_recognition/src/self_study.py
--rw-r--r--   0        0        0     4826 2023-07-21 15:12:32.275834 shapes_recognition-3.1.1/shapes_recognition/src/shapes_similarity.py
--rw-r--r--   0        0        0      679 2023-07-21 15:12:32.284608 shapes_recognition-3.1.1/shapes_recognition/src/show_results.py
--rw-r--r--   0        0        0     2577 2023-07-21 15:12:32.278948 shapes_recognition-3.1.1/shapes_recognition/src/utils.py
--rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 shapes_recognition-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0      607 2023-07-27 10:06:20.195032 shapes_recognition-3.1.2/README.md
+-rw-r--r--   0        0        0      461 2023-07-27 10:23:19.593777 shapes_recognition-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-07-27 10:04:04.503562 shapes_recognition-3.1.2/shapes_recognition/.DS_Store
+-rw-r--r--   0        0        0      278 2023-07-27 08:17:46.702810 shapes_recognition-3.1.2/shapes_recognition/__init__.py
+-rw-r--r--   0        0        0     6148 2023-07-23 08:33:28.741036 shapes_recognition-3.1.2/shapes_recognition/src/.DS_Store
+-rw-r--r--   0        0        0     1440 2023-07-27 08:50:04.788779 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/cfg.cpython-310.pyc
+-rw-r--r--   0        0        0      626 2023-07-27 08:17:50.990666 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/check_background.cpython-310.pyc
+-rw-r--r--   0        0        0     1712 2023-07-27 08:17:51.014015 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/create_joint_table.cpython-310.pyc
+-rw-r--r--   0        0        0     2162 2023-07-27 08:17:51.012014 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/create_table.cpython-310.pyc
+-rw-r--r--   0        0        0     1872 2023-07-27 08:17:51.032320 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/create_template.cpython-310.pyc
+-rw-r--r--   0        0        0     1251 2023-07-27 08:17:50.989961 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/get_column_data.cpython-310.pyc
+-rw-r--r--   0        0        0     2076 2023-07-27 08:17:51.003845 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/get_peaks.cpython-310.pyc
+-rw-r--r--   0        0        0     3873 2023-07-27 08:17:51.030621 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/get_results.cpython-310.pyc
+-rw-r--r--   0        0        0     1668 2023-07-27 08:41:36.007614 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/get_similarity.cpython-310.pyc
+-rw-r--r--   0        0        0     1706 2023-07-27 08:17:51.015629 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/recognition.cpython-310.pyc
+-rw-r--r--   0        0        0     1720 2023-07-27 08:17:51.027607 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/save_results.cpython-310.pyc
+-rw-r--r--   0        0        0     2922 2023-07-27 08:17:50.970644 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/self_study.cpython-310.pyc
+-rw-r--r--   0        0        0     3725 2023-07-27 08:17:50.992432 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/shapes_similarity.cpython-310.pyc
+-rw-r--r--   0        0        0      792 2023-07-27 08:54:07.488118 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/show_results.cpython-310.pyc
+-rw-r--r--   0        0        0     2543 2023-07-27 08:54:07.293633 shapes_recognition-3.1.2/shapes_recognition/src/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0      926 2023-07-27 08:59:30.454217 shapes_recognition-3.1.2/shapes_recognition/src/cfg.py
+-rw-r--r--   0        0        0      428 2023-07-27 08:17:46.711278 shapes_recognition-3.1.2/shapes_recognition/src/check_background.py
+-rw-r--r--   0        0        0     2444 2023-07-21 15:08:18.610725 shapes_recognition-3.1.2/shapes_recognition/src/create_joint_table.py
+-rw-r--r--   0        0        0     2512 2023-07-21 15:08:18.560495 shapes_recognition-3.1.2/shapes_recognition/src/create_table.py
+-rw-r--r--   0        0        0     2068 2023-07-21 15:08:18.598622 shapes_recognition-3.1.2/shapes_recognition/src/create_template.py
+-rw-r--r--   0        0        0     1379 2023-07-27 08:17:46.698519 shapes_recognition-3.1.2/shapes_recognition/src/get_column_data.py
+-rw-r--r--   0        0        0     2667 2023-07-21 15:08:18.607481 shapes_recognition-3.1.2/shapes_recognition/src/get_peaks.py
+-rw-r--r--   0        0        0     5897 2023-07-21 15:08:18.601878 shapes_recognition-3.1.2/shapes_recognition/src/get_results.py
+-rw-r--r--   0        0        0     2367 2023-07-27 08:41:35.779923 shapes_recognition-3.1.2/shapes_recognition/src/get_similarity.py
+-rw-r--r--   0        0        0     2452 2023-07-21 15:08:18.567925 shapes_recognition-3.1.2/shapes_recognition/src/recognition.py
+-rw-r--r--   0        0        0     1648 2023-07-21 15:12:32.259774 shapes_recognition-3.1.2/shapes_recognition/src/save_results.py
+-rw-r--r--   0        0        0     4124 2023-07-21 15:12:32.281959 shapes_recognition-3.1.2/shapes_recognition/src/self_study.py
+-rw-r--r--   0        0        0     4826 2023-07-21 15:12:32.275834 shapes_recognition-3.1.2/shapes_recognition/src/shapes_similarity.py
+-rw-r--r--   0        0        0      660 2023-07-27 08:58:36.551350 shapes_recognition-3.1.2/shapes_recognition/src/show_results.py
+-rw-r--r--   0        0        0     2554 2023-07-27 08:54:04.824874 shapes_recognition-3.1.2/shapes_recognition/src/utils.py
+-rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 shapes_recognition-3.1.2/PKG-INFO
```

### Comparing `shapes_recognition-3.1.1/README.md` & `shapes_recognition-3.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-## SHAPES_RECOGNITION
-"shapes_recognition" is a New Recognition Technology.
+## SHAPES RECOGNITION
+**shapes recognition** is a New Recognition Technology
 
 ### Installation
 ```
-pip install shapes_recognition
+pip install shapes-recognition
 ```
-### About "shapes_recognition"
+### About "shapes-recognition"
 Recognition is an intrinsic property of the human intellect. Kids around two years old recognize shapes even if they differ in size and position or are severely deformed. 
 
 <p align="center"><img src="https://boriskravtsov.com/pypi/shapes.png"/>
 
-To simulate such recognition capability, we introduce the **shapes_recognition** library.
+To simulate such recognition capability, we introduce the **shapes-recognition** library.
 
 [Here](https://kravtsov-development.medium.com/amazing-ai-tables-44af52c993a2) 
 we show how to use it.
```

### Comparing `shapes_recognition-3.1.1/shapes_recognition/.DS_Store` & `shapes_recognition-3.1.2/shapes_recognition/.DS_Store`

 * *Files identical despite different names*

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/.DS_Store` & `shapes_recognition-3.1.2/shapes_recognition/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/cfg.py` & `shapes_recognition-3.1.2/shapes_recognition/src/cfg.py`

 * *Files identical despite different names*

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/create_joint_table.py` & `shapes_recognition-3.1.2/shapes_recognition/src/create_joint_table.py`

 * *Files identical despite different names*

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/create_table.py` & `shapes_recognition-3.1.2/shapes_recognition/src/create_table.py`

 * *Files identical despite different names*

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/create_template.py` & `shapes_recognition-3.1.2/shapes_recognition/src/create_template.py`

 * *Files identical despite different names*

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/get_column_data.py` & `shapes_recognition-3.1.2/shapes_recognition/src/get_column_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import cv2 as cv
 import numpy as np
 
 from shapes_recognition.src import cfg
+from shapes_recognition.src.check_background import check_background
 
 
 def get_column_data(list_in):
 
     column_data_width = cfg.calc_size
     column_data_height = cfg.calc_size * len(list_in)
 
@@ -26,15 +27,15 @@
             sys.exit(1)
 
         image_resize = cv.resize(
             image,
             (cfg.calc_size, cfg.calc_size),
             cv.INTER_LANCZOS4)
 
-        result = is_white_background(image_resize)
+        result = check_background(image_resize)
         if result == 0:
             print(f'\nERROR: ' + path + ' - unacceptable shape')
             sys.exit(1)
 
         image = np.invert(image_resize)
         image_norm = np.zeros((cfg.calc_size, cfg.calc_size), dtype=np.uint8)
         cv.normalize(image, image_norm, 0, 255, cv.NORM_MINMAX)
@@ -44,27 +45,7 @@
         column_data[
             shift_vert:shift_vert + cfg.calc_size:,
             0:cfg.calc_size:] = image_norm[0::, 0::]
 
         n_row += 1
 
     return column_data
-
-
-def is_white_background(any_image: np.uint8) -> int:
-
-    height: int = any_image.shape[0]
-    width: int = any_image.shape[1]
-    area: int = width * height
-
-    index = np.where(any_image == 255)
-
-    n_white = index[0].size
-
-    part_of_area: float = float(n_white) / float(area)
-
-    if part_of_area < cfg.white_part_param:
-        result = 0
-    else:
-        result = 1
-
-    return result
```

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/get_peaks.py` & `shapes_recognition-3.1.2/shapes_recognition/src/get_peaks.py`

 * *Files identical despite different names*

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/get_results.py` & `shapes_recognition-3.1.2/shapes_recognition/src/get_results.py`

 * *Files identical despite different names*

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/recognition.py` & `shapes_recognition-3.1.2/shapes_recognition/src/recognition.py`

 * *Files identical despite different names*

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/save_results.py` & `shapes_recognition-3.1.2/shapes_recognition/src/save_results.py`

 * *Files identical despite different names*

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/self_study.py` & `shapes_recognition-3.1.2/shapes_recognition/src/self_study.py`

 * *Files identical despite different names*

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/shapes_similarity.py` & `shapes_recognition-3.1.2/shapes_recognition/src/shapes_similarity.py`

 * *Files identical despite different names*

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/show_results.py` & `shapes_recognition-3.1.2/shapes_recognition/src/show_results.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import beepy
-
 from shapes_recognition.src.save_results import save_self_study_results, save_recognition_results
 from shapes_recognition.src.get_results import get_self_study_results, get_recognition_results
 
 
 def show_self_study_results(list_self_study_in,
                             list_self_study_out):
 
@@ -16,8 +14,8 @@
 
 def show_recognition_results(recogn_dictionary):
 
     save_recognition_results(recogn_dictionary)
 
     get_recognition_results(recogn_dictionary)
 
-    beepy.beep(sound='coin')
+    print(f'\nThe End')
```

### Comparing `shapes_recognition-3.1.1/shapes_recognition/src/utils.py` & `shapes_recognition-3.1.2/shapes_recognition/src/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import sys
 from pathlib import Path
 import cv2 as cv
 import random
-import beepy
 
 from shapes_recognition.src import cfg
 
 
 def init():
 
     print(f'\nWait...\n')
@@ -44,15 +43,15 @@
 
 
 def get_recognition_data(dir_name):
 
     path_dir = Path.cwd() / dir_name
 
     if not path_dir.is_dir():
-        beepy.beep(sound='coin')
+        print(f'\nThe End')
         sys.exit(0)
 
     list_recognition_in = read_data(path_dir)
 
     check_recognition_data(list_recognition_in)
 
     return list_recognition_in
@@ -100,15 +99,15 @@
 
 
 def check_recognition_data(list_recognition_in):
 
     cfg.n_items_recognition = len(list_recognition_in)
 
     if cfg.n_items_recognition == 0:
-        beepy.beep(sound='coin')
+        print(f'\nThe End')
         sys.exit(0)
 
     for path_image in list_recognition_in:
 
         image = cv.imread(path_image, cv.IMREAD_UNCHANGED)
 
         if image.shape[0] != cfg.cell_height or image.shape[1] != cfg.cell_width:
```

### Comparing `shapes_recognition-3.1.1/PKG-INFO` & `shapes_recognition-3.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: shapes-recognition
-Version: 3.1.1
-Summary: New Recognition Technology
+Version: 3.1.2
+Summary: "shapes-recognition" is a New Recognition Technology
 License: MIT
 Author: Boris Kravtsov
 Author-email: kravtsov.development@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beepy (>=1.0.7,<2.0.0)
 Requires-Dist: opencv-python-headless (>=4.8.0.74,<5.0.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
-## SHAPES_RECOGNITION
-"shapes_recognition" is a New Recognition Technology.
+## SHAPES RECOGNITION
+**shapes recognition** is a New Recognition Technology
 
 ### Installation
 ```
-pip install shapes_recognition
+pip install shapes-recognition
 ```
-### About "shapes_recognition"
+### About "shapes-recognition"
 Recognition is an intrinsic property of the human intellect. Kids around two years old recognize shapes even if they differ in size and position or are severely deformed. 
 
 <p align="center"><img src="https://boriskravtsov.com/pypi/shapes.png"/>
 
-To simulate such recognition capability, we introduce the **shapes_recognition** library.
+To simulate such recognition capability, we introduce the **shapes-recognition** library.
 
 [Here](https://kravtsov-development.medium.com/amazing-ai-tables-44af52c993a2) 
 we show how to use it.
```

