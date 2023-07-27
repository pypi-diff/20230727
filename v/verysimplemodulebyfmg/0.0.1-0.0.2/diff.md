# Comparing `tmp/verysimplemodulebyfmg-0.0.1.tar.gz` & `tmp/verysimplemodulebyfmg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verysimplemodulebyfmg-0.0.1.tar", last modified: Thu Jul 27 10:23:54 2023, max compression
+gzip compressed data, was "verysimplemodulebyfmg-0.0.2.tar", last modified: Thu Jul 27 11:33:08 2023, max compression
```

## Comparing `verysimplemodulebyfmg-0.0.1.tar` & `verysimplemodulebyfmg-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 10:23:54.679361 verysimplemodulebyfmg-0.0.1/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      524 2023-07-27 10:23:54.679361 verysimplemodulebyfmg-0.0.1/PKG-INFO
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       38 2023-07-27 10:23:54.679361 verysimplemodulebyfmg-0.0.1/setup.cfg
--rw-rw-r--   0 qimia     (1000) qimia     (1000)     1038 2023-07-27 10:22:10.000000 verysimplemodulebyfmg-0.0.1/setup.py
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 10:23:54.675361 verysimplemodulebyfmg-0.0.1/verysimplemodule/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       49 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.1/verysimplemodule/__init__.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       34 2023-07-27 08:21:40.000000 verysimplemodulebyfmg-0.0.1/verysimplemodule/add.py
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 10:23:54.675361 verysimplemodulebyfmg-0.0.1/verysimplemodule/extras/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       55 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.1/verysimplemodule/extras/__init__.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       40 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.1/verysimplemodule/extras/divide.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       44 2023-07-27 09:57:43.000000 verysimplemodulebyfmg-0.0.1/verysimplemodule/extras/multiply.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       46 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.1/verysimplemodule/substract.py
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 10:23:54.679361 verysimplemodulebyfmg-0.0.1/verysimplemodulebyfmg.egg-info/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      524 2023-07-27 10:23:54.000000 verysimplemodulebyfmg-0.0.1/verysimplemodulebyfmg.egg-info/PKG-INFO
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      377 2023-07-27 10:23:54.000000 verysimplemodulebyfmg-0.0.1/verysimplemodulebyfmg.egg-info/SOURCES.txt
--rw-rw-r--   0 qimia     (1000) qimia     (1000)        1 2023-07-27 10:23:54.000000 verysimplemodulebyfmg-0.0.1/verysimplemodulebyfmg.egg-info/dependency_links.txt
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       17 2023-07-27 10:23:54.000000 verysimplemodulebyfmg-0.0.1/verysimplemodulebyfmg.egg-info/top_level.txt
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 11:33:08.337212 verysimplemodulebyfmg-0.0.2/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      524 2023-07-27 11:33:08.337212 verysimplemodulebyfmg-0.0.2/PKG-INFO
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       38 2023-07-27 11:33:08.337212 verysimplemodulebyfmg-0.0.2/setup.cfg
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)     1038 2023-07-27 11:32:47.000000 verysimplemodulebyfmg-0.0.2/setup.py
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 11:33:08.337212 verysimplemodulebyfmg-0.0.2/verysimplemodule/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       50 2023-07-27 10:32:53.000000 verysimplemodulebyfmg-0.0.2/verysimplemodule/__init__.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       34 2023-07-27 08:21:40.000000 verysimplemodulebyfmg-0.0.2/verysimplemodule/add.py
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 11:33:08.337212 verysimplemodulebyfmg-0.0.2/verysimplemodule/extras/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       55 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.2/verysimplemodule/extras/__init__.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       40 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.2/verysimplemodule/extras/divide.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       44 2023-07-27 09:57:43.000000 verysimplemodulebyfmg-0.0.2/verysimplemodule/extras/multiply.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       46 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.2/verysimplemodule/substract.py
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 11:33:08.337212 verysimplemodulebyfmg-0.0.2/verysimplemodulebyfmg.egg-info/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      524 2023-07-27 11:33:08.000000 verysimplemodulebyfmg-0.0.2/verysimplemodulebyfmg.egg-info/PKG-INFO
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      377 2023-07-27 11:33:08.000000 verysimplemodulebyfmg-0.0.2/verysimplemodulebyfmg.egg-info/SOURCES.txt
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)        1 2023-07-27 11:33:08.000000 verysimplemodulebyfmg-0.0.2/verysimplemodulebyfmg.egg-info/dependency_links.txt
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       17 2023-07-27 11:33:08.000000 verysimplemodulebyfmg-0.0.2/verysimplemodulebyfmg.egg-info/top_level.txt
```

### Comparing `verysimplemodulebyfmg-0.0.1/PKG-INFO` & `verysimplemodulebyfmg-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verysimplemodulebyfmg
-Version: 0.0.1
+Version: 0.0.2
 Summary: My first Python package
 Author: Fatih GENÇ
 Author-email: f.genc@qimia.de
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `verysimplemodulebyfmg-0.0.1/setup.py` & `verysimplemodulebyfmg-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="verysimplemodulebyfmg",
```

### Comparing `verysimplemodulebyfmg-0.0.1/verysimplemodulebyfmg.egg-info/PKG-INFO` & `verysimplemodulebyfmg-0.0.2/verysimplemodulebyfmg.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verysimplemodulebyfmg
-Version: 0.0.1
+Version: 0.0.2
 Summary: My first Python package
 Author: Fatih GENÇ
 Author-email: f.genc@qimia.de
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

