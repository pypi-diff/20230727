# Comparing `tmp/fastfs-0.0.0.tar.gz` & `tmp/fastfs-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfs-0.0.0.tar", last modified: Thu Jul 20 21:33:21 2023, max compression
+gzip compressed data, was "fastfs-0.9.0.tar", last modified: Thu Jul 27 00:07:02 2023, max compression
```

## Comparing `fastfs-0.0.0.tar` & `fastfs-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,33 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-20 21:33:21.943097 fastfs-0.0.0/
--rw-r--r--   0 josh       (501) staff       (20)      441 2023-07-20 21:33:21.942967 fastfs-0.0.0/PKG-INFO
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-20 21:33:21.942784 fastfs-0.0.0/fastfs.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)      441 2023-07-20 21:33:21.000000 fastfs-0.0.0/fastfs.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)      128 2023-07-20 21:33:21.000000 fastfs-0.0.0/fastfs.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2023-07-20 21:33:21.000000 fastfs-0.0.0/fastfs.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2023-07-20 21:33:21.000000 fastfs-0.0.0/fastfs.egg-info/top_level.txt
--rw-r--r--   0 josh       (501) staff       (20)       38 2023-07-20 21:33:21.943134 fastfs-0.0.0/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)     2041 2023-07-20 21:33:02.000000 fastfs-0.0.0/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-27 00:07:02.288412 fastfs-0.9.0/
+-rw-r--r--   0 josh       (501) staff       (20)     1069 2023-07-20 23:57:24.000000 fastfs-0.9.0/LICENSE
+-rw-r--r--   0 josh       (501) staff       (20)      551 2023-07-27 00:07:02.288275 fastfs-0.9.0/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     6324 2023-07-27 00:02:39.000000 fastfs-0.9.0/README.md
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-27 00:07:02.286024 fastfs-0.9.0/fastfs/
+-rw-r--r--   0 josh       (501) staff       (20)     4488 2023-07-26 22:47:00.000000 fastfs-0.9.0/fastfs/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)      211 2023-07-25 00:20:28.000000 fastfs-0.9.0/fastfs/data_types.py
+-rw-r--r--   0 josh       (501) staff       (20)      813 2023-07-25 18:37:29.000000 fastfs-0.9.0/fastfs/decorators.py
+-rw-r--r--   0 josh       (501) staff       (20)     2759 2023-07-25 00:26:39.000000 fastfs-0.9.0/fastfs/exceptions.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-27 00:07:02.286866 fastfs-0.9.0/fastfs/extensions/
+-rw-r--r--   0 josh       (501) staff       (20)     2347 2023-07-26 22:46:45.000000 fastfs-0.9.0/fastfs/extensions/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-27 00:07:02.287509 fastfs-0.9.0/fastfs/file_managers/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2023-07-25 18:23:29.000000 fastfs-0.9.0/fastfs/file_managers/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     6219 2023-07-26 23:06:07.000000 fastfs-0.9.0/fastfs/file_managers/abstract_file_manager.py
+-rw-r--r--   0 josh       (501) staff       (20)    11416 2023-07-26 20:27:23.000000 fastfs-0.9.0/fastfs/file_managers/base_file_manager.py
+-rw-r--r--   0 josh       (501) staff       (20)     3508 2023-07-26 23:06:31.000000 fastfs-0.9.0/fastfs/file_managers/extension_manager.py
+-rw-r--r--   0 josh       (501) staff       (20)      194 2023-07-26 22:46:07.000000 fastfs-0.9.0/fastfs/file_managers/fast_file_manager.py
+-rw-r--r--   0 josh       (501) staff       (20)      148 2023-07-26 23:05:39.000000 fastfs-0.9.0/fastfs/global_instance.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-27 00:07:02.287630 fastfs-0.9.0/fastfs/utils/
+-rw-r--r--   0 josh       (501) staff       (20)     6360 2023-07-26 22:46:53.000000 fastfs-0.9.0/fastfs/utils/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-27 00:07:02.286716 fastfs-0.9.0/fastfs.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)      551 2023-07-27 00:07:02.000000 fastfs-0.9.0/fastfs.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)      659 2023-07-27 00:07:02.000000 fastfs-0.9.0/fastfs.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-07-27 00:07:02.000000 fastfs-0.9.0/fastfs.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)      116 2023-07-27 00:07:02.000000 fastfs-0.9.0/fastfs.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)        7 2023-07-27 00:07:02.000000 fastfs-0.9.0/fastfs.egg-info/top_level.txt
+-rw-r--r--   0 josh       (501) staff       (20)       38 2023-07-27 00:07:02.288451 fastfs-0.9.0/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)     2234 2023-07-27 00:05:46.000000 fastfs-0.9.0/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-07-27 00:07:02.288075 fastfs-0.9.0/tests/
+-rw-r--r--   0 josh       (501) staff       (20)     3744 2023-07-25 22:19:09.000000 fastfs-0.9.0/tests/test_fast_fs.py
+-rw-r--r--   0 josh       (501) staff       (20)     3911 2023-07-26 22:54:32.000000 fastfs-0.9.0/tests/test_fast_fs_directory.py
+-rw-r--r--   0 josh       (501) staff       (20)     2673 2023-07-26 23:19:23.000000 fastfs-0.9.0/tests/test_fast_fs_extensions.py
+-rw-r--r--   0 josh       (501) staff       (20)     2493 2023-07-25 23:06:01.000000 fastfs-0.9.0/tests/tests_fast_fs_utils.py
```

### Comparing `fastfs-0.0.0/setup.py` & `fastfs-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fastfs',
-    version='0.0.0',
+    version='0.9.0',
     url='http://github.com/breisoft/fastfs',
     author='Josh Breidinger',
     author_email='company@breisoft.com',
-    description="""FastFS is a comprehensive and efficient Python library designed to bridge the gap in Python's file management capabilities. It encapsulates powerful features for reading, writing, and managing data across a variety of file formats and for handling complex directory structures.
+    description="""fastfs is a comprehensive and efficient Python library designed to bridge the gap in Python's file management capabilities. It encapsulates powerful features for reading, writing, and managing data across a variety of file formats and for handling complex directory structures.
 
-FastFS supports a wide range of file formats, including JSON, CSV, Pickle, HDF5, INI, YAML, and XML. This makes it your one-stop solution for all data storage and retrieval needs, facilitating a seamless transition between different data formats within the Python environment.
+fastfs supports a wide range of file formats, including JSON, CSV, Pickle, HDF5, INI, and YAML. This makes it your one-stop solution for all data storage and retrieval needs, facilitating a seamless transition between different data formats within the Python environment.
 
-One of FastFS's standout features is its robust directory management system. By handling all operations relative to a designated 'fastfs' directory, it simplifies file path handling, encouraging cleaner, more organized code.
+One of fastfs's standout features is its robust directory management system. By handling all operations relative to a designated 'fastfs' directory, it simplifies file path handling, encouraging cleaner, more organized code.
 
-Key features of FastFS include:
+Key features of fastfs include:
 
-Versatile Data Handling: FastFS offers extensive functions for reading and writing data across a multitude of formats. Whether your data is in JSON, CSV, or any other supported format, FastFS has you covered.
+Versatile Data Handling: fastfs offers extensive functions for reading and writing data across a multitude of formats. Whether your data is in JSON, CSV, or any other supported format, fastfs has you covered.
 
-Advanced Directory Management: FastFS revolutionizes the way directory structures are handled in Python. By operating relative to a specified 'fastfs' directory, it ensures efficient and user-friendly management of your file system.
+Advanced Directory Management: fastfs revolutionizes the way directory structures are handled in Python. By operating relative to a specified 'fastfs' directory, it ensures efficient and user-friendly management of your file system.
 
-The Missing Piece: Python's standard library, while powerful, lacks a dedicated, comprehensive system for file and directory management. FastFS fills this void, offering an intuitive, Pythonic interface to manage your files and directories.
+The Missing Piece: Python's standard library, while powerful, lacks a dedicated, comprehensive system for file and directory management. fastfs fills this void, offering an intuitive, Pythonic interface to manage your files and directories.
 
-FastFS is the missing piece in Python's file management ecosystem, designed to accelerate your data operations and enhance your productivity. Start using FastFS today and discover a faster, more efficient way to manage your file system in Python.""",
-    packages=find_packages(),    
+fastfs is the missing piece in Python's file management ecosystem, designed to accelerate your data operations and enhance your productivity. Start using fastfs today and discover a faster, more efficient way to manage your file system in Python.""",
+    packages=find_packages(),
     install_requires=[],
+    extras_require={
+        'pandas': ['pandas>=0.20.0'],
+        'h5py': ['h5py>=2.5.0'],
+        'PyYAML': ['PyYAML>=3.11'],
+        'full': ['pandas>=0.20.0', 'h5py>=2.5.0', 'PyYAML>=3.11']
+    }
+
+
 )
```

