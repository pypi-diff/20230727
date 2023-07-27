# Comparing `tmp/pumaz-0.1.0.tar.gz` & `tmp/pumaz-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pumaz-0.1.0.tar", last modified: Thu Jul 27 07:36:53 2023, max compression
+gzip compressed data, was "pumaz-0.2.0.tar", last modified: Thu Jul 27 08:18:30 2023, max compression
```

## Comparing `pumaz-0.1.0.tar` & `pumaz-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 07:36:53.424714 pumaz-0.1.0/
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     7084 2023-07-27 07:36:53.424714 pumaz-0.1.0/PKG-INFO
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     5833 2023-07-27 07:34:55.000000 pumaz-0.1.0/README.md
-drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 07:36:53.424714 pumaz-0.1.0/pumaz/
--rw-rw-r--   0 lalith    (1000) lalith    (1000)      305 2023-07-07 18:44:14.000000 pumaz-0.1.0/pumaz/__init__.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     1573 2023-07-27 07:34:55.000000 pumaz-0.1.0/pumaz/constants.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     3526 2023-07-08 08:44:00.000000 pumaz-0.1.0/pumaz/display.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     4197 2023-07-07 20:08:58.000000 pumaz-0.1.0/pumaz/download.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     4281 2023-07-27 07:34:55.000000 pumaz-0.1.0/pumaz/file_utilities.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     7661 2023-07-27 07:34:55.000000 pumaz-0.1.0/pumaz/image_conversion.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)    14300 2023-07-27 07:34:55.000000 pumaz-0.1.0/pumaz/image_processing.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     2306 2023-07-08 08:25:48.000000 pumaz-0.1.0/pumaz/input_validation.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     5275 2023-07-27 07:34:55.000000 pumaz-0.1.0/pumaz/pumaz.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     1688 2023-07-04 19:36:14.000000 pumaz-0.1.0/pumaz/resources.py
-drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 07:36:53.424714 pumaz-0.1.0/pumaz.egg-info/
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     7084 2023-07-27 07:36:53.000000 pumaz-0.1.0/pumaz.egg-info/PKG-INFO
--rw-rw-r--   0 lalith    (1000) lalith    (1000)      402 2023-07-27 07:36:53.000000 pumaz-0.1.0/pumaz.egg-info/SOURCES.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)        1 2023-07-27 07:36:53.000000 pumaz-0.1.0/pumaz.egg-info/dependency_links.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)       44 2023-07-27 07:36:53.000000 pumaz-0.1.0/pumaz.egg-info/entry_points.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)      235 2023-07-27 07:36:53.000000 pumaz-0.1.0/pumaz.egg-info/requires.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)        6 2023-07-27 07:36:53.000000 pumaz-0.1.0/pumaz.egg-info/top_level.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)       38 2023-07-27 07:36:53.424714 pumaz-0.1.0/setup.cfg
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     1977 2023-07-27 07:36:49.000000 pumaz-0.1.0/setup.py
+drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 08:18:30.452992 pumaz-0.2.0/
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     7084 2023-07-27 08:18:30.452992 pumaz-0.2.0/PKG-INFO
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     5833 2023-07-27 07:34:55.000000 pumaz-0.2.0/README.md
+drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 08:18:30.452992 pumaz-0.2.0/pumaz/
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      305 2023-07-07 18:44:14.000000 pumaz-0.2.0/pumaz/__init__.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     1924 2023-07-27 08:14:47.000000 pumaz-0.2.0/pumaz/constants.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     3526 2023-07-08 08:44:00.000000 pumaz-0.2.0/pumaz/display.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     4197 2023-07-07 20:08:58.000000 pumaz-0.2.0/pumaz/download.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     4281 2023-07-27 07:34:55.000000 pumaz-0.2.0/pumaz/file_utilities.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     7661 2023-07-27 07:34:55.000000 pumaz-0.2.0/pumaz/image_conversion.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)    14300 2023-07-27 07:34:55.000000 pumaz-0.2.0/pumaz/image_processing.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     2306 2023-07-08 08:25:48.000000 pumaz-0.2.0/pumaz/input_validation.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     5275 2023-07-27 07:34:55.000000 pumaz-0.2.0/pumaz/pumaz.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     1688 2023-07-04 19:36:14.000000 pumaz-0.2.0/pumaz/resources.py
+drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 08:18:30.452992 pumaz-0.2.0/pumaz.egg-info/
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     7084 2023-07-27 08:18:30.000000 pumaz-0.2.0/pumaz.egg-info/PKG-INFO
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      402 2023-07-27 08:18:30.000000 pumaz-0.2.0/pumaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)        1 2023-07-27 08:18:30.000000 pumaz-0.2.0/pumaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)       44 2023-07-27 08:18:30.000000 pumaz-0.2.0/pumaz.egg-info/entry_points.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      235 2023-07-27 08:18:30.000000 pumaz-0.2.0/pumaz.egg-info/requires.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)        6 2023-07-27 08:18:30.000000 pumaz-0.2.0/pumaz.egg-info/top_level.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)       38 2023-07-27 08:18:30.452992 pumaz-0.2.0/setup.cfg
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     1977 2023-07-27 08:17:33.000000 pumaz-0.2.0/setup.py
```

### Comparing `pumaz-0.1.0/PKG-INFO` & `pumaz-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pumaz
-Version: 0.1.0
+Version: 0.2.0
 Summary: PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.
 Home-page: https://github.com/QIMP-Team/PUMA
 Author: Sebastian Gutschmayer, Lalith Kumar Shiyam Sundar
 Author-email: Sebastian.Gutschmayer@meduniwien.ac.at, Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: PET tracer alignment,diffeomorphic imaging,image processing,multiplexed tracers
 Platform: UNKNOWN
```

### Comparing `pumaz-0.1.0/README.md` & `pumaz-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pumaz-0.1.0/pumaz/constants.py` & `pumaz-0.2.0/pumaz/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,39 +18,46 @@
 
 import os
 from pumaz import file_utilities
 from datetime import datetime
 
 project_root = file_utilities.get_virtual_env_root()
 BINARY_PATH = os.path.join(project_root, 'bin')
-GREEDY_PATH = os.path.join(BINARY_PATH, f'greedy-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
-                           'greedy')
+
+# SET PATHS TO BINARIES
+
+if file_utilities.get_system()[0] == 'windows':
+    GREEDY_PATH = os.path.join(BINARY_PATH, f'greedy-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+                               'greedy.exe')
+elif file_utilities.get_system()[0] in ['linux', 'mac']:
+    GREEDY_PATH = os.path.join(BINARY_PATH, f'greedy-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+                               'greedy')
+else:
+    raise ValueError('Unsupported OS')
+
 
 # COLOR CODES
 ANSI_ORANGE = '\033[38;5;208m'
 ANSI_GREEN = '\033[38;5;40m'
 ANSI_VIOLET = '\033[38;5;141m'
 ANSI_RESET = '\033[0m'
 
-
 # EXPECTED MODALITIES
 
 MODALITIES = ['PET', 'CT']
 MODALITIES_PREFIX = ['PT_ for PET', 'CT_ for CT']
 
-
 # FILE NAMES
 
 RESAMPLED_PREFIX = 'resampled_'
 ALIGNED_PREFIX = 'aligned_'
 
-
 # FOLDER NAMES
 
-PUMA_WORKING_FOLDER = 'PUMAZ-V01'+'-' + datetime.now().strftime('%Y-%m-%d-%H-%M-%S')
+PUMA_WORKING_FOLDER = 'PUMAZ-V01' + '-' + datetime.now().strftime('%Y-%m-%d-%H-%M-%S')
 TRANSFORMS_FOLDER = 'transforms'
 ALIGNED_CT_FOLDER = 'aligned_CT'
 ALIGNED_PET_FOLDER = 'aligned_PT'
 
 # HYPERPARAMETERS
 
-MULTI_RESOLUTION_SCHEME = '100x25x10'
+MULTI_RESOLUTION_SCHEME = '100x25x10'
```

### Comparing `pumaz-0.1.0/pumaz/display.py` & `pumaz-0.2.0/pumaz/display.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.1.0/pumaz/download.py` & `pumaz-0.2.0/pumaz/download.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.1.0/pumaz/file_utilities.py` & `pumaz-0.2.0/pumaz/file_utilities.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.1.0/pumaz/image_conversion.py` & `pumaz-0.2.0/pumaz/image_conversion.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.1.0/pumaz/image_processing.py` & `pumaz-0.2.0/pumaz/image_processing.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.1.0/pumaz/input_validation.py` & `pumaz-0.2.0/pumaz/input_validation.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.1.0/pumaz/pumaz.py` & `pumaz-0.2.0/pumaz/pumaz.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.1.0/pumaz/resources.py` & `pumaz-0.2.0/pumaz/resources.py`

 * *Files identical despite different names*

### Comparing `pumaz-0.1.0/pumaz.egg-info/PKG-INFO` & `pumaz-0.2.0/pumaz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pumaz
-Version: 0.1.0
+Version: 0.2.0
 Summary: PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.
 Home-page: https://github.com/QIMP-Team/PUMA
 Author: Sebastian Gutschmayer, Lalith Kumar Shiyam Sundar
 Author-email: Sebastian.Gutschmayer@meduniwien.ac.at, Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: PET tracer alignment,diffeomorphic imaging,image processing,multiplexed tracers
 Platform: UNKNOWN
```

### Comparing `pumaz-0.1.0/setup.py` & `pumaz-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='pumaz',
-    version='0.1.0',
+    version='0.2.0',
     author='Sebastian Gutschmayer, Lalith Kumar Shiyam Sundar',
     author_email='Sebastian.Gutschmayer@meduniwien.ac.at, Lalith.shiyamsundar@meduniwien.ac.at',
     description='PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.',
     python_requires='>=3.9',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/QIMP-Team/PUMA',
```

