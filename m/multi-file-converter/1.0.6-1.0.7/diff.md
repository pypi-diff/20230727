# Comparing `tmp/multi_file_converter-1.0.6.tar.gz` & `tmp/multi_file_converter-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_file_converter-1.0.6.tar", last modified: Thu Jul 27 20:59:08 2023, max compression
+gzip compressed data, was "multi_file_converter-1.0.7.tar", last modified: Thu Jul 27 21:06:31 2023, max compression
```

## Comparing `multi_file_converter-1.0.6.tar` & `multi_file_converter-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:59:08.088623 multi_file_converter-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-27 20:59:08.088623 multi_file_converter-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:59:08.084623 multi_file_converter-1.0.6/file_converter/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/file_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/file_converter/docx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:59:08.084623 multi_file_converter-1.0.6/file_converter/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/file_converter/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/file_converter/jpg.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/file_converter/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/file_converter/png.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:59:08.084623 multi_file_converter-1.0.6/file_converter/types/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/file_converter/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/file_converter/types/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/file_converter/types/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:59:08.084623 multi_file_converter-1.0.6/file_converter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/file_converter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/file_converter/utils/tmp_file_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:59:08.088623 multi_file_converter-1.0.6/multi_file_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-27 20:59:08.000000 multi_file_converter-1.0.6/multi_file_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-27 20:59:08.000000 multi_file_converter-1.0.6/multi_file_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:59:08.000000 multi_file_converter-1.0.6/multi_file_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 20:59:08.000000 multi_file_converter-1.0.6/multi_file_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 20:59:08.000000 multi_file_converter-1.0.6/multi_file_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:59:08.088623 multi_file_converter-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 20:58:58.000000 multi_file_converter-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/file_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/docx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/file_converter/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/jpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/png.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/file_converter/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/types/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/types/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/file_converter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/utils/tmp_file_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/multi_file_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-27 21:06:31.000000 multi_file_converter-1.0.7/multi_file_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-27 21:06:31.000000 multi_file_converter-1.0.7/multi_file_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:06:31.000000 multi_file_converter-1.0.7/multi_file_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 21:06:31.000000 multi_file_converter-1.0.7/multi_file_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 21:06:31.000000 multi_file_converter-1.0.7/multi_file_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/setup.py
```

### Comparing `multi_file_converter-1.0.6/PKG-INFO` & `multi_file_converter-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi_file_converter
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple way to convert files to another formats
 Home-page: https://github.com/DAKExDUCK/FileConverter
 Author: dake_duck
 Author-email: arsengabdulin228@gmail.com
 Project-URL: GitHub, https://github.com/DAKExDUCK/FileConverter
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `multi_file_converter-1.0.6/README.md` & `multi_file_converter-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.6/file_converter/jpg.py` & `multi_file_converter-1.0.7/file_converter/jpg.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from PIL import Image
 
 from .types.image import Img, Imgs
 
 
 class JPG(Img):
     can_converts_to = [
-        'pdf',
         'png',
         'bmp',
         'tiff'
     ]
     format = 'jpeg'
 
     def __init__(self, img_or_path: str | Image.Image | BytesIO) -> None:
```

### Comparing `multi_file_converter-1.0.6/file_converter/png.py` & `multi_file_converter-1.0.7/file_converter/png.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from PIL import Image
 
 from .types.image import Img, Imgs
 
 
 class PNG(Img):
     can_converts_to = [
-        'pdf',
         'jpg',
         'bmp',
         'tiff'
     ]
     format = 'png'
 
     def convert_to_pdf() -> BytesIO: ...
```

### Comparing `multi_file_converter-1.0.6/file_converter/types/document.py` & `multi_file_converter-1.0.7/file_converter/types/document.py`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.6/file_converter/types/image.py` & `multi_file_converter-1.0.7/file_converter/types/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,18 @@
         for conversion_type in self.can_converts_to:
             conversion_func_name = f'convert_to_{conversion_type}'
             setattr(self, conversion_func_name, self._create_conversion_func(conversion_type))
 
     def _create_conversion_func(self, conversion_type):
         def conversion_func() -> BytesIO:
             format = conversion_type.upper()
-            tmp_imgs = deepcopy(self.imgs)
+            tmp_imgs = [ _.img for _ in self.imgs ]
             output = BytesIO()
             img = tmp_imgs.pop(0)
-            img.save(output, save_all=True, append_images=tmp_imgs, format=format)
+            img.img.save(output, save_all=True, append_images=tmp_imgs, format=format)
             return output
         return conversion_func
     
     def convert_to(self, format:str) -> BytesIO:
         if format.lower() not in self.can_converts_to:
             raise ValueError("Invalid format type")
```

### Comparing `multi_file_converter-1.0.6/file_converter/utils/tmp_file_manager.py` & `multi_file_converter-1.0.7/file_converter/utils/tmp_file_manager.py`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.6/multi_file_converter.egg-info/PKG-INFO` & `multi_file_converter-1.0.7/multi_file_converter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-file-converter
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple way to convert files to another formats
 Home-page: https://github.com/DAKExDUCK/FileConverter
 Author: dake_duck
 Author-email: arsengabdulin228@gmail.com
 Project-URL: GitHub, https://github.com/DAKExDUCK/FileConverter
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `multi_file_converter-1.0.6/multi_file_converter.egg-info/SOURCES.txt` & `multi_file_converter-1.0.7/multi_file_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.6/setup.py` & `multi_file_converter-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='multi_file_converter',
-  version='1.0.6',
+  version='1.0.7',
   author='dake_duck',
   author_email='arsengabdulin228@gmail.com',
   description='Simple way to convert files to another formats',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/DAKExDUCK/FileConverter',
   packages=find_packages(),
```

