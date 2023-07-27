# Comparing `tmp/robotframework-imagedetection-0.0.3.tar.gz` & `tmp/robotframework-imagedetection-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-imagedetection-0.0.3.tar", last modified: Wed Jul 26 08:21:33 2023, max compression
+gzip compressed data, was "robotframework-imagedetection-0.0.4.tar", last modified: Thu Jul 27 06:19:13 2023, max compression
```

## Comparing `robotframework-imagedetection-0.0.3.tar` & `robotframework-imagedetection-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:21:33.189602 robotframework-imagedetection-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:21:33.127764 robotframework-imagedetection-0.0.3/Imagedetection/
--rw-rw-rw-   0        0        0     6207 2023-07-26 08:20:32.000000 robotframework-imagedetection-0.0.3/Imagedetection/Base_detection.py
--rw-rw-rw-   0        0        0      369 2023-07-26 08:09:00.000000 robotframework-imagedetection-0.0.3/Imagedetection/Imagedetection.py
--rw-rw-rw-   0        0        0       42 2023-07-26 08:08:15.000000 robotframework-imagedetection-0.0.3/Imagedetection/__init__.py
--rw-rw-rw-   0        0        0    11558 2023-07-26 08:04:08.000000 robotframework-imagedetection-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1294 2023-07-26 08:21:33.188603 robotframework-imagedetection-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       87 2023-07-26 08:04:08.000000 robotframework-imagedetection-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 08:21:33.185610 robotframework-imagedetection-0.0.3/robotframework_imagedetection.egg-info/
--rw-rw-rw-   0        0        0     1294 2023-07-26 08:21:33.000000 robotframework-imagedetection-0.0.3/robotframework_imagedetection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-07-26 08:21:33.000000 robotframework-imagedetection-0.0.3/robotframework_imagedetection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 08:21:33.000000 robotframework-imagedetection-0.0.3/robotframework_imagedetection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      782 2023-07-26 08:21:33.000000 robotframework-imagedetection-0.0.3/robotframework_imagedetection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-26 08:21:33.000000 robotframework-imagedetection-0.0.3/robotframework_imagedetection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 08:21:33.190598 robotframework-imagedetection-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1893 2023-07-26 08:04:08.000000 robotframework-imagedetection-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:19:13.933087 robotframework-imagedetection-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-27 06:19:13.912365 robotframework-imagedetection-0.0.4/Imagedetection/
+-rw-rw-rw-   0        0        0     6207 2023-07-27 06:17:35.000000 robotframework-imagedetection-0.0.4/Imagedetection/Base_detection.py
+-rw-rw-rw-   0        0        0      369 2023-07-27 06:17:35.000000 robotframework-imagedetection-0.0.4/Imagedetection/Imagedetection.py
+-rw-rw-rw-   0        0        0       44 2023-07-27 06:17:35.000000 robotframework-imagedetection-0.0.4/Imagedetection/__init__.py
+-rw-rw-rw-   0        0        0    11558 2023-07-27 06:17:35.000000 robotframework-imagedetection-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1335 2023-07-27 06:19:13.932084 robotframework-imagedetection-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2023-07-27 06:17:35.000000 robotframework-imagedetection-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 06:19:13.929591 robotframework-imagedetection-0.0.4/robotframework_imagedetection.egg-info/
+-rw-rw-rw-   0        0        0     1335 2023-07-27 06:19:13.000000 robotframework-imagedetection-0.0.4/robotframework_imagedetection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-27 06:19:13.000000 robotframework-imagedetection-0.0.4/robotframework_imagedetection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 06:19:13.000000 robotframework-imagedetection-0.0.4/robotframework_imagedetection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      782 2023-07-27 06:19:13.000000 robotframework-imagedetection-0.0.4/robotframework_imagedetection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-27 06:19:13.000000 robotframework-imagedetection-0.0.4/robotframework_imagedetection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 06:19:13.934086 robotframework-imagedetection-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1893 2023-07-27 06:17:35.000000 robotframework-imagedetection-0.0.4/setup.py
```

### Comparing `robotframework-imagedetection-0.0.3/Imagedetection/Base_detection.py` & `robotframework-imagedetection-0.0.4/Imagedetection/Base_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import tensorflow as tf
 from robot.api import logger
 from keras.models import load_model
 from keras.preprocessing import image
 from keras.preprocessing.image import ImageDataGenerator
 
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 class Base_Detect:
 
     def __init__(self):
         self.epoch = 20
 
     def train_model(self,training_path, validation_path):
```

### Comparing `robotframework-imagedetection-0.0.3/LICENSE` & `robotframework-imagedetection-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-imagedetection-0.0.3/PKG-INFO` & `robotframework-imagedetection-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: robotframework-imagedetection
-Version: 0.0.3
+Version: 0.0.4
 Summary: Image detection for Robot-Framework
 Home-page: https://github.com/Alpha-Centauri-00/robotframework-imagedetection
 Author: M.Kherki(Alpha-Centauri-00)
 Author-email: alpha_Centauri@posteo.de
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Classifier: Framework :: Robot Framework
 Requires-Python: >=3.6
@@ -27,7 +29,9 @@
 
 # robotframework-objectdetection
 <br/>
 
 [My Awesome Wiki](../../wiki)
 
 [TODO...]
+
+
```

### Comparing `robotframework-imagedetection-0.0.3/robotframework_imagedetection.egg-info/PKG-INFO` & `robotframework-imagedetection-0.0.4/robotframework_imagedetection.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: robotframework-imagedetection
-Version: 0.0.3
+Version: 0.0.4
 Summary: Image detection for Robot-Framework
 Home-page: https://github.com/Alpha-Centauri-00/robotframework-imagedetection
 Author: M.Kherki(Alpha-Centauri-00)
 Author-email: alpha_Centauri@posteo.de
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Classifier: Framework :: Robot Framework
 Requires-Python: >=3.6
@@ -27,7 +29,9 @@
 
 # robotframework-objectdetection
 <br/>
 
 [My Awesome Wiki](../../wiki)
 
 [TODO...]
+
+
```

### Comparing `robotframework-imagedetection-0.0.3/robotframework_imagedetection.egg-info/requires.txt` & `robotframework-imagedetection-0.0.4/robotframework_imagedetection.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `robotframework-imagedetection-0.0.3/setup.py` & `robotframework-imagedetection-0.0.4/setup.py`

 * *Files identical despite different names*

