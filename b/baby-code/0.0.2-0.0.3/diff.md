# Comparing `tmp/baby-code-0.0.2.tar.gz` & `tmp/baby-code-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baby-code-0.0.2.tar", last modified: Thu Jul 27 02:26:26 2023, max compression
+gzip compressed data, was "baby-code-0.0.3.tar", last modified: Thu Jul 27 02:39:20 2023, max compression
```

## Comparing `baby-code-0.0.2.tar` & `baby-code-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 marconeves   (502) staff       (20)        0 2023-07-27 02:26:26.709261 baby-code-0.0.2/
--rw-r--r--   0 marconeves   (502) staff       (20)      199 2023-07-27 02:26:26.709125 baby-code-0.0.2/PKG-INFO
--rw-r--r--   0 marconeves   (502) staff       (20)     3761 2023-07-27 02:12:16.000000 baby-code-0.0.2/README.md
-drwxr-xr-x   0 marconeves   (502) staff       (20)        0 2023-07-27 02:26:26.708942 baby-code-0.0.2/baby_code.egg-info/
--rw-r--r--   0 marconeves   (502) staff       (20)      199 2023-07-27 02:26:26.000000 baby-code-0.0.2/baby_code.egg-info/PKG-INFO
--rw-r--r--   0 marconeves   (502) staff       (20)      218 2023-07-27 02:26:26.000000 baby-code-0.0.2/baby_code.egg-info/SOURCES.txt
--rw-r--r--   0 marconeves   (502) staff       (20)        1 2023-07-27 02:26:26.000000 baby-code-0.0.2/baby_code.egg-info/dependency_links.txt
--rw-r--r--   0 marconeves   (502) staff       (20)       50 2023-07-27 02:26:26.000000 baby-code-0.0.2/baby_code.egg-info/entry_points.txt
--rw-r--r--   0 marconeves   (502) staff       (20)       44 2023-07-27 02:26:26.000000 baby-code-0.0.2/baby_code.egg-info/requires.txt
--rw-r--r--   0 marconeves   (502) staff       (20)        1 2023-07-27 02:26:26.000000 baby-code-0.0.2/baby_code.egg-info/top_level.txt
--rw-r--r--   0 marconeves   (502) staff       (20)       38 2023-07-27 02:26:26.709300 baby-code-0.0.2/setup.cfg
--rw-r--r--   0 marconeves   (502) staff       (20)      526 2023-07-27 02:24:51.000000 baby-code-0.0.2/setup.py
+drwxr-xr-x   0 marconeves   (502) staff       (20)        0 2023-07-27 02:39:20.872181 baby-code-0.0.3/
+-rw-r--r--   0 marconeves   (502) staff       (20)      199 2023-07-27 02:39:20.872077 baby-code-0.0.3/PKG-INFO
+-rw-r--r--   0 marconeves   (502) staff       (20)     3761 2023-07-27 02:12:16.000000 baby-code-0.0.3/README.md
+drwxr-xr-x   0 marconeves   (502) staff       (20)        0 2023-07-27 02:39:20.871917 baby-code-0.0.3/baby_code.egg-info/
+-rw-r--r--   0 marconeves   (502) staff       (20)      199 2023-07-27 02:39:20.000000 baby-code-0.0.3/baby_code.egg-info/PKG-INFO
+-rw-r--r--   0 marconeves   (502) staff       (20)      218 2023-07-27 02:39:20.000000 baby-code-0.0.3/baby_code.egg-info/SOURCES.txt
+-rw-r--r--   0 marconeves   (502) staff       (20)        1 2023-07-27 02:39:20.000000 baby-code-0.0.3/baby_code.egg-info/dependency_links.txt
+-rw-r--r--   0 marconeves   (502) staff       (20)       61 2023-07-27 02:39:20.000000 baby-code-0.0.3/baby_code.egg-info/entry_points.txt
+-rw-r--r--   0 marconeves   (502) staff       (20)       44 2023-07-27 02:39:20.000000 baby-code-0.0.3/baby_code.egg-info/requires.txt
+-rw-r--r--   0 marconeves   (502) staff       (20)        1 2023-07-27 02:39:20.000000 baby-code-0.0.3/baby_code.egg-info/top_level.txt
+-rw-r--r--   0 marconeves   (502) staff       (20)       38 2023-07-27 02:39:20.872217 baby-code-0.0.3/setup.cfg
+-rw-r--r--   0 marconeves   (502) staff       (20)      537 2023-07-27 02:38:56.000000 baby-code-0.0.3/setup.py
```

### Comparing `baby-code-0.0.2/README.md` & `baby-code-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `baby-code-0.0.2/setup.py` & `baby-code-0.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='baby-code',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[
         'Flask',
         'langchain',
         'llama-cpp-python',
         'flask_cors',
     ],
     entry_points={
         'console_scripts': [
-            'baby-code = baby_code.main:main',
+            'baby-code = baby_code.engine.run_llm.:main',
         ],
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

