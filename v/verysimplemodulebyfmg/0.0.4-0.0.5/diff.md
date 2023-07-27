# Comparing `tmp/verysimplemodulebyfmg-0.0.4.tar.gz` & `tmp/verysimplemodulebyfmg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verysimplemodulebyfmg-0.0.4.tar", last modified: Thu Jul 27 11:50:55 2023, max compression
+gzip compressed data, was "verysimplemodulebyfmg-0.0.5.tar", last modified: Thu Jul 27 11:52:55 2023, max compression
```

## Comparing `verysimplemodulebyfmg-0.0.4.tar` & `verysimplemodulebyfmg-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 11:50:55.712266 verysimplemodulebyfmg-0.0.4/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      524 2023-07-27 11:50:55.712266 verysimplemodulebyfmg-0.0.4/PKG-INFO
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       38 2023-07-27 11:50:55.712266 verysimplemodulebyfmg-0.0.4/setup.cfg
--rw-rw-r--   0 qimia     (1000) qimia     (1000)     1038 2023-07-27 11:50:37.000000 verysimplemodulebyfmg-0.0.4/setup.py
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 11:50:55.708266 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       52 2023-07-27 11:40:23.000000 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg/__init__.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       34 2023-07-27 08:21:40.000000 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg/add.py
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 11:50:55.712266 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg/extras/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       55 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg/extras/__init__.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       40 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg/extras/divide.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       44 2023-07-27 09:57:43.000000 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg/extras/multiply.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       46 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg/substract.py
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 11:50:55.708266 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg.egg-info/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      524 2023-07-27 11:50:55.000000 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg.egg-info/PKG-INFO
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      407 2023-07-27 11:50:55.000000 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg.egg-info/SOURCES.txt
--rw-rw-r--   0 qimia     (1000) qimia     (1000)        1 2023-07-27 11:50:55.000000 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg.egg-info/dependency_links.txt
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       22 2023-07-27 11:50:55.000000 verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg.egg-info/top_level.txt
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 11:52:55.636980 verysimplemodulebyfmg-0.0.5/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      524 2023-07-27 11:52:55.632980 verysimplemodulebyfmg-0.0.5/PKG-INFO
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       38 2023-07-27 11:52:55.636980 verysimplemodulebyfmg-0.0.5/setup.cfg
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)     1038 2023-07-27 11:52:53.000000 verysimplemodulebyfmg-0.0.5/setup.py
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 11:52:55.624980 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       53 2023-07-27 11:52:42.000000 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg/__init__.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       34 2023-07-27 08:21:40.000000 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg/add.py
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 11:52:55.632980 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg/extras/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       55 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg/extras/__init__.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       40 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg/extras/divide.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       44 2023-07-27 09:57:43.000000 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg/extras/multiply.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       46 2023-07-27 09:58:10.000000 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg/substract.py
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-07-27 11:52:55.628980 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg.egg-info/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      524 2023-07-27 11:52:55.000000 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg.egg-info/PKG-INFO
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      407 2023-07-27 11:52:55.000000 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg.egg-info/SOURCES.txt
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)        1 2023-07-27 11:52:55.000000 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg.egg-info/dependency_links.txt
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       22 2023-07-27 11:52:55.000000 verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg.egg-info/top_level.txt
```

### Comparing `verysimplemodulebyfmg-0.0.4/PKG-INFO` & `verysimplemodulebyfmg-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verysimplemodulebyfmg
-Version: 0.0.4
+Version: 0.0.5
 Summary: My first Python package
 Author: Fatih GENÇ
 Author-email: f.genc@qimia.de
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `verysimplemodulebyfmg-0.0.4/setup.py` & `verysimplemodulebyfmg-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="verysimplemodulebyfmg",
```

### Comparing `verysimplemodulebyfmg-0.0.4/verysimplemodulebyfmg.egg-info/PKG-INFO` & `verysimplemodulebyfmg-0.0.5/verysimplemodulebyfmg.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verysimplemodulebyfmg
-Version: 0.0.4
+Version: 0.0.5
 Summary: My first Python package
 Author: Fatih GENÇ
 Author-email: f.genc@qimia.de
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

