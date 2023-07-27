# Comparing `tmp/deforum-0.1.3.tar.gz` & `tmp/deforum-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deforum-0.1.3.tar", last modified: Thu Jul 27 06:36:51 2023, max compression
+gzip compressed data, was "deforum-0.1.4.tar", last modified: Thu Jul 27 17:32:14 2023, max compression
```

## Comparing `deforum-0.1.3.tar` & `deforum-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 06:36:51.424112 deforum-0.1.3/
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 04:42:40.000000 deforum-0.1.3/LICENSE
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)      869 2023-07-27 06:36:51.424112 deforum-0.1.3/PKG-INFO
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)      276 2023-07-27 06:02:47.000000 deforum-0.1.3/README.md
-drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 06:36:51.424112 deforum-0.1.3/deforum/
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)       35 2023-07-27 06:34:00.000000 deforum-0.1.3/deforum/__init__.py
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)     1414 2023-07-27 06:34:00.000000 deforum-0.1.3/deforum/deforum.py
-drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 06:36:51.424112 deforum-0.1.3/deforum/pipeline/
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)       53 2023-07-27 06:29:13.000000 deforum-0.1.3/deforum/pipeline/__init__.py
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)    47633 2023-07-27 06:18:11.000000 deforum-0.1.3/deforum/pipeline/img2img.py
-drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 06:36:51.424112 deforum-0.1.3/deforum.egg-info/
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)      869 2023-07-27 06:36:51.000000 deforum-0.1.3/deforum.egg-info/PKG-INFO
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)      290 2023-07-27 06:36:51.000000 deforum-0.1.3/deforum.egg-info/SOURCES.txt
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)        1 2023-07-27 06:36:51.000000 deforum-0.1.3/deforum.egg-info/dependency_links.txt
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)      167 2023-07-27 06:36:51.000000 deforum-0.1.3/deforum.egg-info/requires.txt
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)        8 2023-07-27 06:36:51.000000 deforum-0.1.3/deforum.egg-info/top_level.txt
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)       38 2023-07-27 06:36:51.424112 deforum-0.1.3/setup.cfg
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)     1038 2023-07-27 06:36:09.000000 deforum-0.1.3/setup.py
-drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 06:36:51.424112 deforum-0.1.3/tests/
--rw-rw-r--   0 snorlax   (1000) snorlax   (1000)      255 2023-07-27 05:43:27.000000 deforum-0.1.3/tests/test.py
+drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 17:32:14.578323 deforum-0.1.4/
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)    34570 2023-07-27 17:25:15.000000 deforum-0.1.4/LICENSE
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)      978 2023-07-27 17:32:14.578323 deforum-0.1.4/PKG-INFO
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)      510 2023-07-27 16:53:06.000000 deforum-0.1.4/README.md
+drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 17:32:14.578323 deforum-0.1.4/deforum/
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)       28 2023-07-27 17:13:49.000000 deforum-0.1.4/deforum/__init__.py
+drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 17:32:14.578323 deforum-0.1.4/deforum/backend/
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 17:29:22.000000 deforum-0.1.4/deforum/backend/__init__.py
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)     2999 2023-07-27 17:19:48.000000 deforum-0.1.4/deforum/deforum.py
+drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 17:32:14.578323 deforum-0.1.4/deforum/modules/
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 17:29:28.000000 deforum-0.1.4/deforum/modules/__init__.py
+drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 17:32:14.578323 deforum-0.1.4/deforum/pipelines/
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)       70 2023-07-27 17:12:40.000000 deforum-0.1.4/deforum/pipelines/__init__.py
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)    47633 2023-07-27 06:18:11.000000 deforum-0.1.4/deforum/pipelines/img2img.py
+drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 17:32:14.578323 deforum-0.1.4/deforum/server/
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 17:29:35.000000 deforum-0.1.4/deforum/server/__init__.py
+drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 17:32:14.578323 deforum-0.1.4/deforum/utils/
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 17:29:42.000000 deforum-0.1.4/deforum/utils/__init__.py
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)     2511 2023-07-27 16:53:06.000000 deforum-0.1.4/deforum/utils/make_video.py
+drwxrwxr-x   0 snorlax   (1000) snorlax   (1000)        0 2023-07-27 17:32:14.578323 deforum-0.1.4/deforum.egg-info/
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)      978 2023-07-27 17:32:14.000000 deforum-0.1.4/deforum.egg-info/PKG-INFO
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)      415 2023-07-27 17:32:14.000000 deforum-0.1.4/deforum.egg-info/SOURCES.txt
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)        1 2023-07-27 17:32:14.000000 deforum-0.1.4/deforum.egg-info/dependency_links.txt
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)      187 2023-07-27 17:32:14.000000 deforum-0.1.4/deforum.egg-info/requires.txt
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)        8 2023-07-27 17:32:14.000000 deforum-0.1.4/deforum.egg-info/top_level.txt
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)       38 2023-07-27 17:32:14.578323 deforum-0.1.4/setup.cfg
+-rw-rw-r--   0 snorlax   (1000) snorlax   (1000)      948 2023-07-27 17:31:36.000000 deforum-0.1.4/setup.py
```

### Comparing `deforum-0.1.3/deforum/pipeline/img2img.py` & `deforum-0.1.4/deforum/pipelines/img2img.py`

 * *Files identical despite different names*

### Comparing `deforum-0.1.3/setup.py` & `deforum-0.1.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from setuptools import setup, find_packages
 
 setup(
     name='deforum',
-    version='0.1.3',
+    version='0.1.4',
     author='deforum',
     author_email='deforum.art@gmail.com',
     description='diffusion animation toolkit',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/deforum-art/deforum',  
     packages=find_packages(),
     install_requires=[
         'diffusers==0.19.0',
         'torch==2.0.1',
+        'torchvision==0.15.2',
         'transformers==4.31.0',
         'accelerate==0.21.0',
         'safetensors==0.3.1',
         'opencv-python==4.8.0.74',
         'imageio==2.31.1',
         'imageio-ffmpeg==0.4.8',
         'natsort==8.4.0',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
+        'License :: OSI Approved :: GNU Affero General Public License v3',
+        'Programming Language :: Python :: 3.10',
     ],
 )
```

