# Comparing `tmp/echoss_s3handler-0.0.1.tar.gz` & `tmp/echoss_s3handler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoss_s3handler-0.0.1.tar", last modified: Thu Jul 27 04:39:58 2023, max compression
+gzip compressed data, was "echoss_s3handler-0.0.2.tar", last modified: Thu Jul 27 05:01:01 2023, max compression
```

## Comparing `echoss_s3handler-0.0.1.tar` & `echoss_s3handler-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:39:58.882651 echoss_s3handler-0.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3585 2023-07-27 04:39:58.882651 echoss_s3handler-0.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3272 2023-07-24 08:08:30.000000 echoss_s3handler-0.0.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:39:58.882651 echoss_s3handler-0.0.1/echoss_s3handler/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-07-27 04:38:31.000000 echoss_s3handler-0.0.1/echoss_s3handler/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19274 2023-07-24 08:08:30.000000 echoss_s3handler-0.0.1/echoss_s3handler/s3_handler.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:39:58.882651 echoss_s3handler-0.0.1/echoss_s3handler.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3585 2023-07-27 04:39:58.000000 echoss_s3handler-0.0.1/echoss_s3handler.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2023-07-27 04:39:58.000000 echoss_s3handler-0.0.1/echoss_s3handler.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-27 04:39:58.000000 echoss_s3handler-0.0.1/echoss_s3handler.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-07-27 04:39:58.000000 echoss_s3handler-0.0.1/echoss_s3handler.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-27 04:39:58.882651 echoss_s3handler-0.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      630 2023-07-27 04:39:53.000000 echoss_s3handler-0.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 05:01:01.935427 echoss_s3handler-0.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3663 2023-07-27 05:01:01.935427 echoss_s3handler-0.0.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3351 2023-07-27 05:00:05.000000 echoss_s3handler-0.0.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 05:01:01.935427 echoss_s3handler-0.0.2/echoss_s3handler/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2023-07-27 05:00:33.000000 echoss_s3handler-0.0.2/echoss_s3handler/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19274 2023-07-24 08:08:30.000000 echoss_s3handler-0.0.2/echoss_s3handler/s3_handler.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 05:01:01.935427 echoss_s3handler-0.0.2/echoss_s3handler.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3663 2023-07-27 05:01:01.000000 echoss_s3handler-0.0.2/echoss_s3handler.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2023-07-27 05:01:01.000000 echoss_s3handler-0.0.2/echoss_s3handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-27 05:01:01.000000 echoss_s3handler-0.0.2/echoss_s3handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-07-27 05:01:01.000000 echoss_s3handler-0.0.2/echoss_s3handler.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-27 05:01:01.935427 echoss_s3handler-0.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      630 2023-07-27 05:00:25.000000 echoss_s3handler-0.0.2/setup.py
```

### Comparing `echoss_s3handler-0.0.1/PKG-INFO` & `echoss_s3handler-0.0.2/echoss_s3handler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
-Name: echoss_s3handler
-Version: 0.0.1
+Name: echoss-s3handler
+Version: 0.0.2
 Summary: echoss AI Bigdata Solution - S3 handler
 Home-page: 
 Author: incheolshin
 Author-email: incheolshin@12cm.co.kr
 Keywords: echoss,echoss_s3handler,s3handler,s3_handler
 Requires: boto3
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 
+## import 방법
+ -  from echoss_s3handler import s3_handler
+
 custom yolov7과 image_utils의 함수 사용시 S3에 있는 데이터를 사용하고자 하여 만든 Class
 
 크게 두가지의 class가 존재함
 1. client를 활용한 clas
 2. resource를 활용한 class
 
 # Client Class
@@ -78,7 +81,11 @@
      - S3에 있는 파일을 메모리로 읽기 위한 함수
     
     s3_resource.read_image()
      - S3에 있는 이미지 파일을 메모리로 읽는 함수
      - 이후 사용되는 이미지 형식에 따라 옵션에 "cv2", "PIL"을 선택하여 사용 가능
     
 ```
+
+```python
+
+```
```

### Comparing `echoss_s3handler-0.0.1/README.md` & `echoss_s3handler-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+## import 방법
+ -  from echoss_s3handler import s3_handler
+
 custom yolov7과 image_utils의 함수 사용시 S3에 있는 데이터를 사용하고자 하여 만든 Class
 
 크게 두가지의 class가 존재함
 1. client를 활용한 clas
 2. resource를 활용한 class
 
 # Client Class
@@ -65,8 +68,12 @@
     s3_resource.read_file()
      - S3에 있는 파일을 메모리로 읽기 위한 함수
     
     s3_resource.read_image()
      - S3에 있는 이미지 파일을 메모리로 읽는 함수
      - 이후 사용되는 이미지 형식에 따라 옵션에 "cv2", "PIL"을 선택하여 사용 가능
     
-```
+```
+
+```python
+
+```
```

### Comparing `echoss_s3handler-0.0.1/echoss_s3handler/s3_handler.py` & `echoss_s3handler-0.0.2/echoss_s3handler/s3_handler.py`

 * *Files identical despite different names*

### Comparing `echoss_s3handler-0.0.1/echoss_s3handler.egg-info/PKG-INFO` & `echoss_s3handler-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
-Name: echoss-s3handler
-Version: 0.0.1
+Name: echoss_s3handler
+Version: 0.0.2
 Summary: echoss AI Bigdata Solution - S3 handler
 Home-page: 
 Author: incheolshin
 Author-email: incheolshin@12cm.co.kr
 Keywords: echoss,echoss_s3handler,s3handler,s3_handler
 Requires: boto3
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 
+## import 방법
+ -  from echoss_s3handler import s3_handler
+
 custom yolov7과 image_utils의 함수 사용시 S3에 있는 데이터를 사용하고자 하여 만든 Class
 
 크게 두가지의 class가 존재함
 1. client를 활용한 clas
 2. resource를 활용한 class
 
 # Client Class
@@ -78,7 +81,11 @@
      - S3에 있는 파일을 메모리로 읽기 위한 함수
     
     s3_resource.read_image()
      - S3에 있는 이미지 파일을 메모리로 읽는 함수
      - 이후 사용되는 이미지 형식에 따라 옵션에 "cv2", "PIL"을 선택하여 사용 가능
     
 ```
+
+```python
+
+```
```

### Comparing `echoss_s3handler-0.0.1/setup.py` & `echoss_s3handler-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 package_name = "echoss_s3handler"
 
 setup(
     name='echoss_s3handler',
-    version='0.0.1',
+    version='0.0.2',
     url='',
     requires=['boto3'],
     license='',
     author='incheolshin',
     author_email='incheolshin@12cm.co.kr',
     description='echoss AI Bigdata Solution - S3 handler',
     long_description=long_description,
```

