# Comparing `tmp/tortoise_api_model-0.0.3.tar.gz` & `tmp/tortoise_api_model-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise_api_model-0.0.3.tar", last modified: Tue Jul 25 15:10:37 2023, max compression
+gzip compressed data, was "tortoise_api_model-0.0.4.tar", last modified: Thu Jul 27 09:57:18 2023, max compression
```

## Comparing `tortoise_api_model-0.0.3.tar` & `tortoise_api_model-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-25 15:10:37.303622 tortoise_api_model-0.0.3/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-25 15:10:37.303413 tortoise_api_model-0.0.3/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-25 15:10:37.303674 tortoise_api_model-0.0.3/setup.cfg
--rw-r--r--   0 sol        (501) staff       (20)      819 2023-07-25 15:09:57.000000 tortoise_api_model-0.0.3/setup.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-25 15:10:37.301468 tortoise_api_model-0.0.3/tortoise_api_model/
--rw-r--r--   0 sol        (501) staff       (20)       50 2023-07-25 15:09:00.000000 tortoise_api_model-0.0.3/tortoise_api_model/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)      519 2023-07-25 15:08:25.000000 tortoise_api_model-0.0.3/tortoise_api_model/model.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-25 15:10:37.303176 tortoise_api_model-0.0.3/tortoise_api_model.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-25 15:10:37.000000 tortoise_api_model-0.0.3/tortoise_api_model.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      276 2023-07-25 15:10:37.000000 tortoise_api_model-0.0.3/tortoise_api_model.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-25 15:10:37.000000 tortoise_api_model-0.0.3/tortoise_api_model.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-25 15:10:37.000000 tortoise_api_model-0.0.3/tortoise_api_model.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-25 15:10:37.000000 tortoise_api_model-0.0.3/tortoise_api_model.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 09:57:18.849882 tortoise_api_model-0.0.4/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-27 09:57:18.849678 tortoise_api_model-0.0.4/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-27 09:57:18.849935 tortoise_api_model-0.0.4/setup.cfg
+-rw-r--r--   0 sol        (501) staff       (20)      819 2023-07-27 09:56:38.000000 tortoise_api_model-0.0.4/setup.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 09:57:18.848434 tortoise_api_model-0.0.4/tortoise_api_model/
+-rw-r--r--   0 sol        (501) staff       (20)       50 2023-07-25 15:09:00.000000 tortoise_api_model-0.0.4/tortoise_api_model/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)      943 2023-07-27 09:56:17.000000 tortoise_api_model-0.0.4/tortoise_api_model/model.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 09:57:18.849428 tortoise_api_model-0.0.4/tortoise_api_model.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-27 09:57:18.000000 tortoise_api_model-0.0.4/tortoise_api_model.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      276 2023-07-27 09:57:18.000000 tortoise_api_model-0.0.4/tortoise_api_model.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-27 09:57:18.000000 tortoise_api_model-0.0.4/tortoise_api_model.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-27 09:57:18.000000 tortoise_api_model-0.0.4/tortoise_api_model.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-27 09:57:18.000000 tortoise_api_model-0.0.4/tortoise_api_model.egg-info/top_level.txt
```

### Comparing `tortoise_api_model-0.0.3/setup.py` & `tortoise_api_model-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Base model for tortoise-api'
 LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="tortoise_api_model",
     version=VERSION,
```

