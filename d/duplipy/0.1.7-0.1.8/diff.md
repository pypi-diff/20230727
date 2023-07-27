# Comparing `tmp/duplipy-0.1.7.tar.gz` & `tmp/duplipy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duplipy-0.1.7.tar", last modified: Thu Jul 27 15:52:00 2023, max compression
+gzip compressed data, was "duplipy-0.1.8.tar", last modified: Thu Jul 27 16:31:03 2023, max compression
```

## Comparing `duplipy-0.1.7.tar` & `duplipy-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 15:52:00.435133 duplipy-0.1.7/
--rw-rw-rw-   0        0        0      955 2023-07-07 14:42:48.000000 duplipy-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     1027 2023-07-27 15:52:00.433131 duplipy-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 15:52:00.377135 duplipy-0.1.7/duplipy/
--rw-rw-rw-   0        0        0      636 2023-07-27 15:31:14.000000 duplipy-0.1.7/duplipy/__init__.py
--rw-rw-rw-   0        0        0     6539 2023-07-07 08:39:46.000000 duplipy-0.1.7/duplipy/formatting.py
--rw-rw-rw-   0        0        0    14031 2023-07-27 15:49:07.000000 duplipy-0.1.7/duplipy/replication.py
--rw-rw-rw-   0        0        0     1533 2023-07-07 14:20:43.000000 duplipy-0.1.7/duplipy/similarity.py
--rw-rw-rw-   0        0        0      897 2023-07-07 14:21:51.000000 duplipy-0.1.7/duplipy/text_analysis.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:52:00.420136 duplipy-0.1.7/duplipy.egg-info/
--rw-rw-rw-   0        0        0     1027 2023-07-27 15:51:59.000000 duplipy-0.1.7/duplipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-07-27 15:51:59.000000 duplipy-0.1.7/duplipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 15:51:59.000000 duplipy-0.1.7/duplipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-27 15:51:59.000000 duplipy-0.1.7/duplipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 15:51:59.000000 duplipy-0.1.7/duplipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 15:52:00.436132 duplipy-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1302 2023-07-27 15:37:49.000000 duplipy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:31:03.918130 duplipy-0.1.8/
+-rw-rw-rw-   0        0        0      955 2023-07-07 14:42:48.000000 duplipy-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     1027 2023-07-27 16:31:03.914131 duplipy-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4204 2023-07-27 16:04:10.000000 duplipy-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 16:31:03.857136 duplipy-0.1.8/duplipy/
+-rw-rw-rw-   0        0        0      636 2023-07-27 15:31:14.000000 duplipy-0.1.8/duplipy/__init__.py
+-rw-rw-rw-   0        0        0     6539 2023-07-07 08:39:46.000000 duplipy-0.1.8/duplipy/formatting.py
+-rw-rw-rw-   0        0        0    10946 2023-07-27 16:28:39.000000 duplipy-0.1.8/duplipy/replication.py
+-rw-rw-rw-   0        0        0     1533 2023-07-07 14:20:43.000000 duplipy-0.1.8/duplipy/similarity.py
+-rw-rw-rw-   0        0        0      897 2023-07-07 14:21:51.000000 duplipy-0.1.8/duplipy/text_analysis.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:31:03.908135 duplipy-0.1.8/duplipy.egg-info/
+-rw-rw-rw-   0        0        0     1027 2023-07-27 16:31:01.000000 duplipy-0.1.8/duplipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-27 16:31:02.000000 duplipy-0.1.8/duplipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 16:31:01.000000 duplipy-0.1.8/duplipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-27 16:31:02.000000 duplipy-0.1.8/duplipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 16:31:02.000000 duplipy-0.1.8/duplipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 16:31:03.921134 duplipy-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1302 2023-07-27 16:27:52.000000 duplipy-0.1.8/setup.py
```

### Comparing `duplipy-0.1.7/LICENSE` & `duplipy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `duplipy-0.1.7/PKG-INFO` & `duplipy-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplipy
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for formatting and text replication, with added support for image augmentation.
 Home-page: https://github.com/infinitode/duplipy
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplipy-0.1.7/duplipy/__init__.py` & `duplipy-0.1.8/duplipy/__init__.py`

 * *Files identical despite different names*

### Comparing `duplipy-0.1.7/duplipy/formatting.py` & `duplipy-0.1.8/duplipy/formatting.py`

 * *Files identical despite different names*

### Comparing `duplipy-0.1.7/duplipy/replication.py` & `duplipy-0.1.8/duplipy/replication.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,18 +13,16 @@
 - `flip_horizontal(image)`: Flip the input image horizontally.
 - `flip_vertical(image)`: Flip the input image vertically.
 - `rotate(image, angle)`: Rotate the input image by a specified angle.
 - `random_rotation(image, max_angle)`: Randomly rotate the input image by an angle within the specified range.
 - `resize(image, size)`: Resize the input image to the specified size.
 - `crop(image, box)`: Crop the input image to the specified rectangular region.
 - `random_crop(image, size)`: Randomly crop a region from the input image.
-- `perform_image_augmentation(source_dir, target_dir, flip_horizontal=False, flip_vertical=False, rotate=False, random_rotation=False, resize=False, crop=False, max_angle=30, target_size=(224, 224), crop_size=(150, 150))`: Perform image augmentation on images in the source directory and its subdirectories.
 """
 
-import os
 import random
 import time
 import nltk
 from nltk.corpus import wordnet
 from PIL import Image
 
 nltk.download("wordnet", quiet=True)
@@ -325,77 +323,8 @@
     - `PIL.Image.Image`: The randomly cropped image region.
     """
     width, height = image.size
     left = random.randint(0, width - size[0])
     upper = random.randint(0, height - size[1])
     right = left + size[0]
     lower = upper + size[1]
-    return crop(image, (left, upper, right, lower))
-
-def perform_image_augmentation(
-    source_dir,
-    target_dir,
-    flip_horizontal=False,
-    flip_vertical=False,
-    rotate=False,
-    random_rotation=False,
-    resize=False,
-    crop=False,
-    max_angle=30,
-    target_size=(224, 224),
-    crop_size=(150, 150)
-):
-    """
-    Perform image augmentation on images in the source directory and its subdirectories.
-
-    Parameters:
-    - `source_dir` (str): The path to the source directory containing the images.
-    - `target_dir` (str): The path to the target directory where augmented images will be saved.
-    - `flip_horizontal` (bool): Perform horizontal flipping if True. Default is False.
-    - `flip_vertical` (bool): Perform vertical flipping if True. Default is False.
-    - `rotate` (bool): Perform rotation if True. Default is False.
-    - `random_rotation` (bool): Perform random rotation if True. Default is False.
-    - `resize` (bool): Perform resizing if True. Default is False.
-    - `crop` (bool): Perform cropping if True. Default is False.
-    - `max_angle` (float): The maximum absolute angle of rotation in degrees. Default is 30.
-    - `target_size` (tuple): The target size for resizing in the format (width, height). Default is (224, 224).
-    - `crop_size` (tuple): The size of the cropped region in the format (width, height). Default is (150, 150).
-    """
-
-    def augment_image(image_path):
-        image = Image.open(image_path)
-
-        if flip_horizontal and random.random() > 0.5:
-            image = flip_horizontal(image)
-
-        if flip_vertical and random.random() > 0.5:
-            image = flip_vertical(image)
-
-        if rotate and random.random() > 0.5:
-            image = rotate(image, max_angle)
-
-        if random_rotation and random.random() > 0.5:
-            image = random_rotation(image, max_angle)
-
-        if resize and random.random() > 0.5:
-            image = resize(image, target_size)
-
-        if crop and random.random() > 0.5:
-            image = random_crop(image, crop_size)
-
-        target_path = os.path.join(target_dir, os.path.relpath(image_path, source_dir))
-        os.makedirs(os.path.dirname(target_path), exist_ok=True)
-        image.save(target_path)
-
-    num_images = 0
-    num_directories = 0
-
-    for root, _, files in os.walk(source_dir):
-        num_directories += 1
-        for file in files:
-            if file.lower().endswith(('.jpg', '.jpeg', '.png', '.gif', '.bmp')):
-                num_images += 1
-                image_path = os.path.join(root, file)
-                augment_image(image_path)
-                print(f"Processed {num_images} images in {num_directories} directories.", end='\r')
-
-    print("\nImage augmentation completed successfully.")
+    return crop(image, (left, upper, right, lower))
```

### Comparing `duplipy-0.1.7/duplipy/similarity.py` & `duplipy-0.1.8/duplipy/similarity.py`

 * *Files identical despite different names*

### Comparing `duplipy-0.1.7/duplipy/text_analysis.py` & `duplipy-0.1.8/duplipy/text_analysis.py`

 * *Files identical despite different names*

### Comparing `duplipy-0.1.7/duplipy.egg-info/PKG-INFO` & `duplipy-0.1.8/duplipy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplipy
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for formatting and text replication, with added support for image augmentation.
 Home-page: https://github.com/infinitode/duplipy
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplipy-0.1.7/setup.py` & `duplipy-0.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='duplipy',
-    version='0.1.7',
+    version='0.1.8',
     author='Infinitode Pty Ltd',
     author_email='infinitode.ltd@gmail.com',
     description='A package for formatting and text replication, with added support for image augmentation.',
     long_description='DupliPy is a quick and easy-to-use package that can handle text formatting and data augmentation tasks for NLP in Python, with added support for image augmentation.',
     long_description_content_type='text/markdown',
     url='https://github.com/infinitode/duplipy',
     packages=find_packages(),
```

