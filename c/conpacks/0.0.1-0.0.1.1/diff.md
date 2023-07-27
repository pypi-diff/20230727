# Comparing `tmp/conpacks-0.0.1.tar.gz` & `tmp/conpacks-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conpacks-0.0.1.tar", last modified: Thu Jul 27 03:46:00 2023, max compression
+gzip compressed data, was "conpacks-0.0.1.1.tar", last modified: Thu Jul 27 04:06:54 2023, max compression
```

## Comparing `conpacks-0.0.1.tar` & `conpacks-0.0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 connorsheehan   (501) staff       (20)        0 2023-07-27 03:46:00.775345 conpacks-0.0.1/
--rw-r--r--   0 connorsheehan   (501) staff       (20)     1067 2023-07-27 03:44:58.000000 conpacks-0.0.1/LICENSE
--rw-r--r--   0 connorsheehan   (501) staff       (20)      544 2023-07-27 03:46:00.775232 conpacks-0.0.1/PKG-INFO
--rw-r--r--   0 connorsheehan   (501) staff       (20)       51 2023-07-27 03:14:51.000000 conpacks-0.0.1/README.md
-drwxr-xr-x   0 connorsheehan   (501) staff       (20)        0 2023-07-27 03:46:00.775089 conpacks-0.0.1/conpacks.egg-info/
--rw-r--r--   0 connorsheehan   (501) staff       (20)      544 2023-07-27 03:46:00.000000 conpacks-0.0.1/conpacks.egg-info/PKG-INFO
--rw-r--r--   0 connorsheehan   (501) staff       (20)      154 2023-07-27 03:46:00.000000 conpacks-0.0.1/conpacks.egg-info/SOURCES.txt
--rw-r--r--   0 connorsheehan   (501) staff       (20)        1 2023-07-27 03:46:00.000000 conpacks-0.0.1/conpacks.egg-info/dependency_links.txt
--rw-r--r--   0 connorsheehan   (501) staff       (20)        1 2023-07-27 03:46:00.000000 conpacks-0.0.1/conpacks.egg-info/top_level.txt
--rw-r--r--   0 connorsheehan   (501) staff       (20)       38 2023-07-27 03:46:00.775378 conpacks-0.0.1/setup.cfg
--rw-r--r--   0 connorsheehan   (501) staff       (20)      957 2023-07-27 03:44:02.000000 conpacks-0.0.1/setup.py
+drwxr-xr-x   0 connorsheehan   (501) staff       (20)        0 2023-07-27 04:06:54.474300 conpacks-0.0.1.1/
+-rw-r--r--   0 connorsheehan   (501) staff       (20)     1067 2023-07-27 03:44:58.000000 conpacks-0.0.1.1/LICENSE
+-rw-r--r--   0 connorsheehan   (501) staff       (20)      724 2023-07-27 04:06:54.474200 conpacks-0.0.1.1/PKG-INFO
+-rw-r--r--   0 connorsheehan   (501) staff       (20)      229 2023-07-27 04:05:38.000000 conpacks-0.0.1.1/README.md
+drwxr-xr-x   0 connorsheehan   (501) staff       (20)        0 2023-07-27 04:06:54.474063 conpacks-0.0.1.1/conpacks.egg-info/
+-rw-r--r--   0 connorsheehan   (501) staff       (20)      724 2023-07-27 04:06:54.000000 conpacks-0.0.1.1/conpacks.egg-info/PKG-INFO
+-rw-r--r--   0 connorsheehan   (501) staff       (20)      154 2023-07-27 04:06:54.000000 conpacks-0.0.1.1/conpacks.egg-info/SOURCES.txt
+-rw-r--r--   0 connorsheehan   (501) staff       (20)        1 2023-07-27 04:06:54.000000 conpacks-0.0.1.1/conpacks.egg-info/dependency_links.txt
+-rw-r--r--   0 connorsheehan   (501) staff       (20)        1 2023-07-27 04:06:54.000000 conpacks-0.0.1.1/conpacks.egg-info/top_level.txt
+-rw-r--r--   0 connorsheehan   (501) staff       (20)       38 2023-07-27 04:06:54.474332 conpacks-0.0.1.1/setup.cfg
+-rw-r--r--   0 connorsheehan   (501) staff       (20)      958 2023-07-27 04:06:46.000000 conpacks-0.0.1.1/setup.py
```

### Comparing `conpacks-0.0.1/LICENSE` & `conpacks-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conpacks-0.0.1/setup.py` & `conpacks-0.0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.1.1'
 DESCRIPTION = 'A small package'
-LONG_DESCRIPTION = 'A laregr package'
+LONG_DESCRIPTION = 'A large package'
 
 # Setting up
 setup(
     name="conpacks",
     version=VERSION,
     author="conacts",
     author_email="<csheehan630@gmail.com>",
```

