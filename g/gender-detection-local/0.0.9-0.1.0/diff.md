# Comparing `tmp/gender-detection-local-0.0.9.tar.gz` & `tmp/gender-detection-local-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gender-detection-local-0.0.9.tar", last modified: Thu Jul 13 10:08:31 2023, max compression
+gzip compressed data, was "gender-detection-local-0.1.0.tar", last modified: Thu Jul 27 13:44:23 2023, max compression
```

## Comparing `gender-detection-local-0.0.9.tar` & `gender-detection-local-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:08:31.693521 gender-detection-local-0.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:08:31.693521 gender-detection-local-0.0.9/CirclesGenderDetectionPython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:08:14.000000 gender-detection-local-0.0.9/CirclesGenderDetectionPython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-07-13 10:08:14.000000 gender-detection-local-0.0.9/CirclesGenderDetectionPython/gender_detection
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-13 10:08:14.000000 gender-detection-local-0.0.9/CirclesGenderDetectionPython/gender_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-13 10:08:14.000000 gender-detection-local-0.0.9/CirclesGenderDetectionPython/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-13 10:08:31.693521 gender-detection-local-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-13 10:08:15.000000 gender-detection-local-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:08:31.693521 gender-detection-local-0.0.9/gender_detection_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-13 10:08:31.000000 gender-detection-local-0.0.9/gender_detection_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-13 10:08:31.000000 gender-detection-local-0.0.9/gender_detection_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:08:31.000000 gender-detection-local-0.0.9/gender_detection_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 10:08:31.000000 gender-detection-local-0.0.9/gender_detection_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 10:08:15.000000 gender-detection-local-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:08:31.693521 gender-detection-local-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-13 10:08:15.000000 gender-detection-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:44:23.958087 gender-detection-local-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:44:23.958087 gender-detection-local-0.1.0/CirclesGenderDetectionPython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/CirclesGenderDetectionPython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/CirclesGenderDetectionPython/gender_detection
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/CirclesGenderDetectionPython/gender_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/CirclesGenderDetectionPython/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-27 13:44:23.958087 gender-detection-local-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:44:23.958087 gender-detection-local-0.1.0/gender_detection_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-27 13:44:23.000000 gender-detection-local-0.1.0/gender_detection_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-27 13:44:23.000000 gender-detection-local-0.1.0/gender_detection_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:44:23.000000 gender-detection-local-0.1.0/gender_detection_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 13:44:23.000000 gender-detection-local-0.1.0/gender_detection_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:44:23.958087 gender-detection-local-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 13:44:12.000000 gender-detection-local-0.1.0/setup.py
```

### Comparing `gender-detection-local-0.0.9/CirclesGenderDetectionPython/gender_detection` & `gender-detection-local-0.1.0/CirclesGenderDetectionPython/gender_detection`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.0.9/CirclesGenderDetectionPython/gender_detection.py` & `gender-detection-local-0.1.0/CirclesGenderDetectionPython/gender_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,24 +119,25 @@
            image = read_file(image_path)
 
            # Decode the JPEG-encoded image into a tensor
            image = decode_jpeg(image)
        
            image = resize(image, (178,218))
         else:
+           '''
            # Permission to use webcam and work on singular image
            inquiry = input("""
            This script will take a picture with your webcam, 
            this will only be for the purposes for determining your gender. 
            Proceed? (Y/n) """)
 
            if inquiry.lower()!="y" and inquiry.lower!="yes":
               self.lgrins.info("\nAborting\n")
               exit()
-
+           '''
            # Capture Image from Webcam
            image = resize(capture_write(), (178, 218))
 
         # Rescale the pixel values to a range of [0, 1]
         image = image / 255.0
 
         # Apply data augmentation
```

### Comparing `gender-detection-local-0.0.9/README.md` & `gender-detection-local-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.0.9/setup.py` & `gender-detection-local-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='gender-detection-local',  
-     version='0.0.9',
+     version='0.1.0',
      author="Circles",
      author_email="info@circles.zone",
      description="PyPI Package for gender detection",
      long_description="This is a package for running gender detection and predicting gender",
      long_description_content_type="text/markdown",
      url="https://github.com/circles-zone/gender-detection-local-python-package",
      packages=setuptools.find_packages(),
```

