# Comparing `tmp/gpthistory-0.2.tar.gz` & `tmp/gpthistory-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpthistory-0.2.tar", last modified: Thu Jul 27 07:03:10 2023, max compression
+gzip compressed data, was "gpthistory-0.3.tar", last modified: Thu Jul 27 07:05:34 2023, max compression
```

## Comparing `gpthistory-0.2.tar` & `gpthistory-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shrikar    (501) staff       (20)        0 2023-07-27 07:03:10.630484 gpthistory-0.2/
--rw-r--r--   0 shrikar    (501) staff       (20)     1466 2023-07-27 06:26:36.000000 gpthistory-0.2/LICENSE.md
--rw-r--r--   0 shrikar    (501) staff       (20)      206 2023-07-27 07:03:10.630353 gpthistory-0.2/PKG-INFO
--rw-r--r--   0 shrikar    (501) staff       (20)     2685 2023-07-27 06:52:10.000000 gpthistory-0.2/README.md
-drwxr-xr-x   0 shrikar    (501) staff       (20)        0 2023-07-27 07:03:10.629400 gpthistory-0.2/gpthistory/
--rw-r--r--   0 shrikar    (501) staff       (20)        0 2023-07-26 05:52:10.000000 gpthistory-0.2/gpthistory/__init__.py
--rw-r--r--   0 shrikar    (501) staff       (20)     3953 2023-07-27 06:18:44.000000 gpthistory-0.2/gpthistory/gpthistory.py
--rw-r--r--   0 shrikar    (501) staff       (20)     3184 2023-07-27 06:21:18.000000 gpthistory-0.2/gpthistory/helpers.py
-drwxr-xr-x   0 shrikar    (501) staff       (20)        0 2023-07-27 07:03:10.630180 gpthistory-0.2/gpthistory.egg-info/
--rw-r--r--   0 shrikar    (501) staff       (20)      206 2023-07-27 07:03:10.000000 gpthistory-0.2/gpthistory.egg-info/PKG-INFO
--rw-r--r--   0 shrikar    (501) staff       (20)      305 2023-07-27 07:03:10.000000 gpthistory-0.2/gpthistory.egg-info/SOURCES.txt
--rw-r--r--   0 shrikar    (501) staff       (20)        1 2023-07-27 07:03:10.000000 gpthistory-0.2/gpthistory.egg-info/dependency_links.txt
--rw-r--r--   0 shrikar    (501) staff       (20)       58 2023-07-27 07:03:10.000000 gpthistory-0.2/gpthistory.egg-info/entry_points.txt
--rw-r--r--   0 shrikar    (501) staff       (20)       33 2023-07-27 07:03:10.000000 gpthistory-0.2/gpthistory.egg-info/requires.txt
--rw-r--r--   0 shrikar    (501) staff       (20)       11 2023-07-27 07:03:10.000000 gpthistory-0.2/gpthistory.egg-info/top_level.txt
--rw-r--r--   0 shrikar    (501) staff       (20)       38 2023-07-27 07:03:10.630521 gpthistory-0.2/setup.cfg
--rw-r--r--   0 shrikar    (501) staff       (20)      527 2023-07-27 07:02:57.000000 gpthistory-0.2/setup.py
+drwxr-xr-x   0 shrikar    (501) staff       (20)        0 2023-07-27 07:05:34.606440 gpthistory-0.3/
+-rw-r--r--   0 shrikar    (501) staff       (20)     1466 2023-07-27 06:26:36.000000 gpthistory-0.3/LICENSE.md
+-rw-r--r--   0 shrikar    (501) staff       (20)      206 2023-07-27 07:05:34.606322 gpthistory-0.3/PKG-INFO
+-rw-r--r--   0 shrikar    (501) staff       (20)     2685 2023-07-27 06:52:10.000000 gpthistory-0.3/README.md
+drwxr-xr-x   0 shrikar    (501) staff       (20)        0 2023-07-27 07:05:34.605394 gpthistory-0.3/gpthistory/
+-rw-r--r--   0 shrikar    (501) staff       (20)        0 2023-07-26 05:52:10.000000 gpthistory-0.3/gpthistory/__init__.py
+-rw-r--r--   0 shrikar    (501) staff       (20)     3953 2023-07-27 06:18:44.000000 gpthistory-0.3/gpthistory/gpthistory.py
+-rw-r--r--   0 shrikar    (501) staff       (20)     3184 2023-07-27 06:21:18.000000 gpthistory-0.3/gpthistory/helpers.py
+drwxr-xr-x   0 shrikar    (501) staff       (20)        0 2023-07-27 07:05:34.606161 gpthistory-0.3/gpthistory.egg-info/
+-rw-r--r--   0 shrikar    (501) staff       (20)      206 2023-07-27 07:05:34.000000 gpthistory-0.3/gpthistory.egg-info/PKG-INFO
+-rw-r--r--   0 shrikar    (501) staff       (20)      305 2023-07-27 07:05:34.000000 gpthistory-0.3/gpthistory.egg-info/SOURCES.txt
+-rw-r--r--   0 shrikar    (501) staff       (20)        1 2023-07-27 07:05:34.000000 gpthistory-0.3/gpthistory.egg-info/dependency_links.txt
+-rw-r--r--   0 shrikar    (501) staff       (20)       58 2023-07-27 07:05:34.000000 gpthistory-0.3/gpthistory.egg-info/entry_points.txt
+-rw-r--r--   0 shrikar    (501) staff       (20)       40 2023-07-27 07:05:34.000000 gpthistory-0.3/gpthistory.egg-info/requires.txt
+-rw-r--r--   0 shrikar    (501) staff       (20)       11 2023-07-27 07:05:34.000000 gpthistory-0.3/gpthistory.egg-info/top_level.txt
+-rw-r--r--   0 shrikar    (501) staff       (20)       38 2023-07-27 07:05:34.606470 gpthistory-0.3/setup.cfg
+-rw-r--r--   0 shrikar    (501) staff       (20)      534 2023-07-27 07:05:27.000000 gpthistory-0.3/setup.py
```

### Comparing `gpthistory-0.2/LICENSE.md` & `gpthistory-0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gpthistory-0.2/README.md` & `gpthistory-0.3/README.md`

 * *Files identical despite different names*

### Comparing `gpthistory-0.2/gpthistory/gpthistory.py` & `gpthistory-0.3/gpthistory/gpthistory.py`

 * *Files identical despite different names*

### Comparing `gpthistory-0.2/gpthistory/helpers.py` & `gpthistory-0.3/gpthistory/helpers.py`

 * *Files identical despite different names*

### Comparing `gpthistory-0.2/setup.py` & `gpthistory-0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gpthistory',
-    version='0.2',
+    version='0.3',
     description='A tool for searching through your chatgpt conversation history',
     author='Shrikar Archak',
     author_email='shrikar84@gmail.com',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'Click',
-        'dotenv',
+        'python-dotenv',
         'openai',
         'pandas',
         'numpy'
     ],
     entry_points='''
         [console_scripts]
         gpthistory=gpthistory.gpthistory:main
```

