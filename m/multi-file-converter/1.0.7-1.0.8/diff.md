# Comparing `tmp/multi_file_converter-1.0.7.tar.gz` & `tmp/multi_file_converter-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_file_converter-1.0.7.tar", last modified: Thu Jul 27 21:06:31 2023, max compression
+gzip compressed data, was "multi_file_converter-1.0.8.tar", last modified: Thu Jul 27 21:32:09 2023, max compression
```

## Comparing `multi_file_converter-1.0.7.tar` & `multi_file_converter-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/file_converter/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/docx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/file_converter/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/jpg.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/png.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/file_converter/types/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/types/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/types/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/file_converter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/file_converter/utils/tmp_file_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/multi_file_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-27 21:06:31.000000 multi_file_converter-1.0.7/multi_file_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-27 21:06:31.000000 multi_file_converter-1.0.7/multi_file_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:06:31.000000 multi_file_converter-1.0.7/multi_file_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 21:06:31.000000 multi_file_converter-1.0.7/multi_file_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 21:06:31.000000 multi_file_converter-1.0.7/multi_file_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:06:31.305626 multi_file_converter-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 21:06:20.000000 multi_file_converter-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:32:09.168947 multi_file_converter-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-27 21:32:09.168947 multi_file_converter-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:32:09.164947 multi_file_converter-1.0.8/file_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/file_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/file_converter/docx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:32:09.164947 multi_file_converter-1.0.8/file_converter/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/file_converter/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/file_converter/jpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/file_converter/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/file_converter/png.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:32:09.164947 multi_file_converter-1.0.8/file_converter/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/file_converter/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/file_converter/types/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/file_converter/types/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:32:09.168947 multi_file_converter-1.0.8/file_converter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/file_converter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/file_converter/utils/tmp_file_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:32:09.168947 multi_file_converter-1.0.8/multi_file_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-27 21:32:09.000000 multi_file_converter-1.0.8/multi_file_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-27 21:32:09.000000 multi_file_converter-1.0.8/multi_file_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:32:09.000000 multi_file_converter-1.0.8/multi_file_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 21:32:09.000000 multi_file_converter-1.0.8/multi_file_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 21:32:09.000000 multi_file_converter-1.0.8/multi_file_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:32:09.168947 multi_file_converter-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 21:31:58.000000 multi_file_converter-1.0.8/setup.py
```

### Comparing `multi_file_converter-1.0.7/PKG-INFO` & `multi_file_converter-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi_file_converter
-Version: 1.0.7
+Version: 1.0.8
 Summary: Simple way to convert files to another formats
 Home-page: https://github.com/DAKExDUCK/FileConverter
 Author: dake_duck
 Author-email: arsengabdulin228@gmail.com
 Project-URL: GitHub, https://github.com/DAKExDUCK/FileConverter
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `multi_file_converter-1.0.7/README.md` & `multi_file_converter-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.7/file_converter/jpg.py` & `multi_file_converter-1.0.8/file_converter/jpg.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     ]
     format = 'jpeg'
 
     def __init__(self, img_or_path: str | Image.Image | BytesIO) -> None:
         super().__init__(img_or_path)
         self.img = self.img.convert('RGB')
 
-    def convert_to_pdf(self) -> BytesIO: ...
     def convert_to_png(self) -> BytesIO: ...
     def convert_to_bmp(self) -> BytesIO: ...
     def convert_to_tiff(self) -> BytesIO: ...
 
 
 class JPGs(Imgs):
     can_converts_to = [
```

### Comparing `multi_file_converter-1.0.7/file_converter/png.py` & `multi_file_converter-1.0.8/file_converter/png.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     can_converts_to = [
         'jpg',
         'bmp',
         'tiff'
     ]
     format = 'png'
 
-    def convert_to_pdf() -> BytesIO: ...
     def convert_to_jpg() -> BytesIO: ...
     def convert_to_bmp() -> BytesIO: ...
     def convert_to_tiff() -> BytesIO: ...
 
 
 class PNGs(Imgs):
     can_converts_to = [
```

### Comparing `multi_file_converter-1.0.7/file_converter/types/document.py` & `multi_file_converter-1.0.8/file_converter/types/document.py`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.7/file_converter/types/image.py` & `multi_file_converter-1.0.8/file_converter/types/image.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,30 +32,32 @@
             try:
                 if format == 'JPEG':
                     self.img = self.img.convert('RGB')
                 self.img.save(output, format=format)
             except Exception as exc:
                 raise ErrorConvertFile(str(exc))
             else:
+                output.seek(0)
                 return output
         return conversion_func
     
     def convert_to(self, format:str) -> BytesIO:
-        format = 'JPEG' if format == 'jpg' else format.upper()
+        format = 'JPEG' if format.lower() == 'jpg' else format.upper()
         # if format not in self.can_converts_to:
         #     raise ValueError("Invalid format type")
         
         output = BytesIO()
         try:
             if format == 'JPEG':
                 self.img = self.img.convert('RGB')
             self.img.save(output, format=format)
         except Exception as exc:
             raise ErrorConvertFile(str(exc))
         else:
+            output.seek(0)
             return output
     
 
 class Imgs:
     can_converts_to: list
     imgs: list[Image.Image]
 
@@ -66,20 +68,20 @@
 
     def _create_conversion_func(self, conversion_type):
         def conversion_func() -> BytesIO:
             format = conversion_type.upper()
             tmp_imgs = [ _.img for _ in self.imgs ]
             output = BytesIO()
             img = tmp_imgs.pop(0)
-            img.img.save(output, save_all=True, append_images=tmp_imgs, format=format)
+            img.save(output, save_all=True, append_images=tmp_imgs, format=format)
             return output
         return conversion_func
     
     def convert_to(self, format:str) -> BytesIO:
         if format.lower() not in self.can_converts_to:
             raise ValueError("Invalid format type")
         
-        tmp_imgs = deepcopy(self.imgs)
+        tmp_imgs = [ _.img for _ in self.imgs ]
         output = BytesIO()
         img = tmp_imgs.pop(0)
         img.save(output, save_all=True, append_images=tmp_imgs, format=format.upper())
         return output
```

### Comparing `multi_file_converter-1.0.7/file_converter/utils/tmp_file_manager.py` & `multi_file_converter-1.0.8/file_converter/utils/tmp_file_manager.py`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.7/multi_file_converter.egg-info/PKG-INFO` & `multi_file_converter-1.0.8/multi_file_converter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-file-converter
-Version: 1.0.7
+Version: 1.0.8
 Summary: Simple way to convert files to another formats
 Home-page: https://github.com/DAKExDUCK/FileConverter
 Author: dake_duck
 Author-email: arsengabdulin228@gmail.com
 Project-URL: GitHub, https://github.com/DAKExDUCK/FileConverter
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `multi_file_converter-1.0.7/multi_file_converter.egg-info/SOURCES.txt` & `multi_file_converter-1.0.8/multi_file_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.7/setup.py` & `multi_file_converter-1.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='multi_file_converter',
-  version='1.0.7',
+  version='1.0.8',
   author='dake_duck',
   author_email='arsengabdulin228@gmail.com',
   description='Simple way to convert files to another formats',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/DAKExDUCK/FileConverter',
   packages=find_packages(),
```

