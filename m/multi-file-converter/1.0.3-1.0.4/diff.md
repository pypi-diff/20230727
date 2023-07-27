# Comparing `tmp/multi_file_converter-1.0.3.tar.gz` & `tmp/multi_file_converter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_file_converter-1.0.3.tar", last modified: Fri Jul  7 11:23:44 2023, max compression
+gzip compressed data, was "multi_file_converter-1.0.4.tar", last modified: Thu Jul 27 20:15:29 2023, max compression
```

## Comparing `multi_file_converter-1.0.3.tar` & `multi_file_converter-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:23:44.925068 multi_file_converter-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-07 11:23:44.925068 multi_file_converter-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:23:44.921068 multi_file_converter-1.0.3/file_converter/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/file_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/file_converter/docx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:23:44.921068 multi_file_converter-1.0.3/file_converter/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/file_converter/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/file_converter/jpg.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/file_converter/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/file_converter/png.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:23:44.921068 multi_file_converter-1.0.3/file_converter/types/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/file_converter/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/file_converter/types/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/file_converter/types/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:23:44.921068 multi_file_converter-1.0.3/file_converter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/file_converter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/file_converter/utils/tmp_file_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:23:44.925068 multi_file_converter-1.0.3/multi_file_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-07 11:23:44.000000 multi_file_converter-1.0.3/multi_file_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-07 11:23:44.000000 multi_file_converter-1.0.3/multi_file_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:23:44.000000 multi_file_converter-1.0.3/multi_file_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 11:23:44.000000 multi_file_converter-1.0.3/multi_file_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 11:23:44.000000 multi_file_converter-1.0.3/multi_file_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:23:44.925068 multi_file_converter-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-07 11:23:35.000000 multi_file_converter-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:15:29.056641 multi_file_converter-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-27 20:15:29.056641 multi_file_converter-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:15:29.052641 multi_file_converter-1.0.4/file_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/file_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/file_converter/docx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:15:29.052641 multi_file_converter-1.0.4/file_converter/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/file_converter/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/file_converter/jpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/file_converter/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/file_converter/png.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:15:29.052641 multi_file_converter-1.0.4/file_converter/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/file_converter/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/file_converter/types/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/file_converter/types/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:15:29.052641 multi_file_converter-1.0.4/file_converter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/file_converter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/file_converter/utils/tmp_file_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:15:29.056641 multi_file_converter-1.0.4/multi_file_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-27 20:15:29.000000 multi_file_converter-1.0.4/multi_file_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-27 20:15:29.000000 multi_file_converter-1.0.4/multi_file_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:15:29.000000 multi_file_converter-1.0.4/multi_file_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 20:15:29.000000 multi_file_converter-1.0.4/multi_file_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 20:15:29.000000 multi_file_converter-1.0.4/multi_file_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:15:29.056641 multi_file_converter-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 20:15:11.000000 multi_file_converter-1.0.4/setup.py
```

### Comparing `multi_file_converter-1.0.3/PKG-INFO` & `multi_file_converter-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: multi_file_converter
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple way to convert files to another formats
 Home-page: https://github.com/DAKExDUCK/FileConverter
 Author: dake_duck
 Author-email: arsengabdulin228@gmail.com
-Project-URL: GutHub, https://github.com/DAKExDUCK/FileConverter
+Project-URL: GitHub, https://github.com/DAKExDUCK/FileConverter
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # ConvertFilesClass
```

### Comparing `multi_file_converter-1.0.3/README.md` & `multi_file_converter-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.3/file_converter/jpg.py` & `multi_file_converter-1.0.4/file_converter/jpg.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,12 +21,13 @@
     def convert_to_pdf(self) -> BytesIO: ...
     def convert_to_png(self) -> BytesIO: ...
     def convert_to_bmp(self) -> BytesIO: ...
     def convert_to_tiff(self) -> BytesIO: ...
 
 
 class JPGs(Imgs):
-    converts_to = [
+    can_converts_to = [
         'pdf'
     ]
+    format = 'jpeg'
 
     def convert_to_pdf(self) -> BytesIO: ...
```

### Comparing `multi_file_converter-1.0.3/file_converter/types/document.py` & `multi_file_converter-1.0.4/file_converter/types/document.py`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.3/file_converter/types/image.py` & `multi_file_converter-1.0.4/file_converter/types/image.py`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.3/file_converter/utils/tmp_file_manager.py` & `multi_file_converter-1.0.4/file_converter/utils/tmp_file_manager.py`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.3/multi_file_converter.egg-info/PKG-INFO` & `multi_file_converter-1.0.4/multi_file_converter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: multi-file-converter
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simple way to convert files to another formats
 Home-page: https://github.com/DAKExDUCK/FileConverter
 Author: dake_duck
 Author-email: arsengabdulin228@gmail.com
-Project-URL: GutHub, https://github.com/DAKExDUCK/FileConverter
+Project-URL: GitHub, https://github.com/DAKExDUCK/FileConverter
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # ConvertFilesClass
```

### Comparing `multi_file_converter-1.0.3/multi_file_converter.egg-info/SOURCES.txt` & `multi_file_converter-1.0.4/multi_file_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multi_file_converter-1.0.3/setup.py` & `multi_file_converter-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='multi_file_converter',
-  version='1.0.3',
+  version='1.0.4',
   author='dake_duck',
   author_email='arsengabdulin228@gmail.com',
   description='Simple way to convert files to another formats',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/DAKExDUCK/FileConverter',
   packages=find_packages(),
   install_requires=['Pillow>=10.0.0'],
   classifiers=[
     'Programming Language :: Python :: 3.10',
     'Operating System :: POSIX :: Linux'
   ],
   keywords='',
   project_urls={
-    'GutHub': 'https://github.com/DAKExDUCK/FileConverter'
+    'GitHub': 'https://github.com/DAKExDUCK/FileConverter'
   },
   python_requires='>=3.10'
-)
+)
```

