# Comparing `tmp/untrusted_process-0.2.tar.gz` & `tmp/untrusted_process-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untrusted_process-0.2.tar", last modified: Wed Jul 26 21:09:32 2023, max compression
+gzip compressed data, was "untrusted_process-0.3.tar", last modified: Wed Jul 26 21:55:23 2023, max compression
```

## Comparing `untrusted_process-0.2.tar` & `untrusted_process-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 21:09:32.402700 untrusted_process-0.2/
--rw-rw-rw-   0        0        0      643 2023-07-26 21:09:32.401518 untrusted_process-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 21:09:32.402700 untrusted_process-0.2/setup.cfg
--rw-rw-rw-   0        0        0      889 2023-07-26 21:09:26.000000 untrusted_process-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 21:09:32.393343 untrusted_process-0.2/untrusted_process/
--rw-rw-rw-   0        0        0       39 2023-07-26 20:45:22.000000 untrusted_process-0.2/untrusted_process/__init__.py
--rw-rw-rw-   0        0        0     3352 2023-07-26 21:07:15.000000 untrusted_process-0.2/untrusted_process/core.py
--rw-rw-rw-   0        0        0      889 2023-07-26 20:37:18.000000 untrusted_process-0.2/untrusted_process/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 21:09:32.400519 untrusted_process-0.2/untrusted_process.egg-info/
--rw-rw-rw-   0        0        0      643 2023-07-26 21:09:32.000000 untrusted_process-0.2/untrusted_process.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-07-26 21:09:32.000000 untrusted_process-0.2/untrusted_process.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 21:09:32.000000 untrusted_process-0.2/untrusted_process.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-26 21:09:32.000000 untrusted_process-0.2/untrusted_process.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-26 21:09:32.000000 untrusted_process-0.2/untrusted_process.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 21:55:23.866706 untrusted_process-0.3/
+-rw-rw-rw-   0        0        0      643 2023-07-26 21:55:23.864294 untrusted_process-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-26 21:55:23.866706 untrusted_process-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      889 2023-07-26 21:44:51.000000 untrusted_process-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 21:55:23.847034 untrusted_process-0.3/untrusted_process/
+-rw-rw-rw-   0        0        0       39 2023-07-26 21:32:23.000000 untrusted_process-0.3/untrusted_process/__init__.py
+-rw-rw-rw-   0        0        0     3352 2023-07-26 21:32:23.000000 untrusted_process-0.3/untrusted_process/core.py
+-rw-rw-rw-   0        0        0      891 2023-07-26 21:44:34.000000 untrusted_process-0.3/untrusted_process/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 21:55:23.862983 untrusted_process-0.3/untrusted_process.egg-info/
+-rw-rw-rw-   0        0        0      643 2023-07-26 21:55:23.000000 untrusted_process-0.3/untrusted_process.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-07-26 21:55:23.000000 untrusted_process-0.3/untrusted_process.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 21:55:23.000000 untrusted_process-0.3/untrusted_process.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-26 21:55:23.000000 untrusted_process-0.3/untrusted_process.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-26 21:55:23.000000 untrusted_process-0.3/untrusted_process.egg-info/top_level.txt
```

### Comparing `untrusted_process-0.2/PKG-INFO` & `untrusted_process-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untrusted_process
-Version: 0.2
+Version: 0.3
 Summary: A package to analyze and visualize untrusted processes using osquery.
 Home-page: https://github.com/your_username/untrusted_process
 Author: Ahsan Ali
 Author-email: misterj503@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `untrusted_process-0.2/setup.py` & `untrusted_process-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 setup(
     name='untrusted_process',
-    version='0.2',
+    version='0.3',
     packages=['untrusted_process'],
     install_requires=[
         'pandas',
         'matplotlib',
-        'tkinter',
+        'Tkinter',
     ],
     python_requires='>=3.6',
     author='Ahsan Ali',
     author_email='misterj503@gmail.com',
     description='A package to analyze and visualize untrusted processes using osquery.',
     long_description='Please refer to the README.md file for detailed information.',
     long_description_content_type='text/markdown',
```

### Comparing `untrusted_process-0.2/untrusted_process/core.py` & `untrusted_process-0.3/untrusted_process/core.py`

 * *Files identical despite different names*

### Comparing `untrusted_process-0.2/untrusted_process/setup.py` & `untrusted_process-0.3/untrusted_process/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 setup(
     name='untrusted_process',
     version='0.1',
     packages=['untrusted_process'],
     install_requires=[
         'pandas',
         'matplotlib',
-        'tkinter',
+        'Tkinter',
     ],
     python_requires='>=3.6',
     author='Ahsan Ali',
     author_email='misterj503@gmail.com',
     description='A package to analyze and visualize untrusted processes using osquery.',
-    long_description='Please refer to the README.md file for detailed information.',
+    long_description='"Please refer to the README.md file for detailed information."',
     long_description_content_type='text/markdown',
     url='https://github.com/your_username/untrusted_process',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `untrusted_process-0.2/untrusted_process.egg-info/PKG-INFO` & `untrusted_process-0.3/untrusted_process.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: untrusted-process
-Version: 0.2
+Version: 0.3
 Summary: A package to analyze and visualize untrusted processes using osquery.
 Home-page: https://github.com/your_username/untrusted_process
 Author: Ahsan Ali
 Author-email: misterj503@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

