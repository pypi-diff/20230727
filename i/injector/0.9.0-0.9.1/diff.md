# Comparing `tmp/injector-0.9.0.tar.gz` & `tmp/injector-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/injector-0.9.0.tar", last modified: Thu May 15 17:30:38 2014, max compression
+gzip compressed data, was "dist/injector-0.9.1.tar", last modified: Fri Oct 10 05:17:43 2014, max compression
```

## Comparing `injector-0.9.0.tar` & `injector-0.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-x---   0 alec       (501) staff       (20)        0 2014-05-15 17:30:38.000000 injector-0.9.0/
-drwxr-x---   0 alec       (501) staff       (20)        0 2014-05-15 17:30:38.000000 injector-0.9.0/injector.egg-info/
--rw-r-----   0 alec       (501) staff       (20)        1 2014-05-15 17:30:38.000000 injector-0.9.0/injector.egg-info/dependency_links.txt
--rw-r-----   0 alec       (501) staff       (20)     7637 2014-05-15 17:30:38.000000 injector-0.9.0/injector.egg-info/PKG-INFO
--rw-r-----   0 alec       (501) staff       (20)       19 2014-05-15 17:30:38.000000 injector-0.9.0/injector.egg-info/requires.txt
--rw-r-----   0 alec       (501) staff       (20)      222 2014-05-15 17:30:38.000000 injector-0.9.0/injector.egg-info/SOURCES.txt
--rw-r-----   0 alec       (501) staff       (20)        9 2014-05-15 17:30:38.000000 injector-0.9.0/injector.egg-info/top_level.txt
--rw-r-----   0 alec       (501) staff       (20)    37402 2014-05-15 17:28:54.000000 injector-0.9.0/injector.py
--rw-r-----   0 alec       (501) staff       (20)       18 2013-06-29 14:40:23.000000 injector-0.9.0/MANIFEST.in
--rw-r-----   0 alec       (501) staff       (20)     7637 2014-05-15 17:30:38.000000 injector-0.9.0/PKG-INFO
--rw-r-----   0 alec       (501) staff       (20)     5763 2014-01-24 06:35:01.000000 injector-0.9.0/README.md
--rw-r-----   0 alec       (501) staff       (20)    19927 2013-11-25 16:14:47.000000 injector-0.9.0/README.rst
--rw-r-----   0 alec       (501) staff       (20)      196 2014-05-15 17:30:38.000000 injector-0.9.0/setup.cfg
--rw-r-----   0 alec       (501) staff       (20)     1410 2013-09-17 00:15:53.000000 injector-0.9.0/setup.py
+drwxr-x---   0 alec       (501) staff       (20)        0 2014-10-10 05:17:43.000000 injector-0.9.1/
+drwxr-x---   0 alec       (501) staff       (20)        0 2014-10-10 05:17:43.000000 injector-0.9.1/injector.egg-info/
+-rw-r-----   0 alec       (501) staff       (20)        1 2014-10-10 05:17:42.000000 injector-0.9.1/injector.egg-info/dependency_links.txt
+-rw-r-----   0 alec       (501) staff       (20)     7637 2014-10-10 05:17:42.000000 injector-0.9.1/injector.egg-info/PKG-INFO
+-rw-r-----   0 alec       (501) staff       (20)       19 2014-10-10 05:17:42.000000 injector-0.9.1/injector.egg-info/requires.txt
+-rw-r-----   0 alec       (501) staff       (20)      222 2014-10-10 05:17:43.000000 injector-0.9.1/injector.egg-info/SOURCES.txt
+-rw-r-----   0 alec       (501) staff       (20)        9 2014-10-10 05:17:42.000000 injector-0.9.1/injector.egg-info/top_level.txt
+-rw-r-----   0 alec       (501) staff       (20)    37415 2014-10-10 05:16:46.000000 injector-0.9.1/injector.py
+-rw-r-----   0 alec       (501) staff       (20)       18 2013-06-29 14:40:23.000000 injector-0.9.1/MANIFEST.in
+-rw-r-----   0 alec       (501) staff       (20)     7637 2014-10-10 05:17:43.000000 injector-0.9.1/PKG-INFO
+-rw-r-----   0 alec       (501) staff       (20)     5763 2014-01-24 06:35:01.000000 injector-0.9.1/README.md
+-rw-r-----   0 alec       (501) staff       (20)    19927 2013-11-25 16:14:47.000000 injector-0.9.1/README.rst
+-rw-r-----   0 alec       (501) staff       (20)      196 2014-10-10 05:17:43.000000 injector-0.9.1/setup.cfg
+-rw-r-----   0 alec       (501) staff       (20)     1410 2013-09-17 00:15:53.000000 injector-0.9.1/setup.py
```

### Comparing `injector-0.9.0/injector.egg-info/PKG-INFO` & `injector-0.9.1/injector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: injector
-Version: 0.9.0
+Version: 0.9.1
 Summary: Injector - Python dependency injection framework, inspired by Guice
 Home-page: http://github.com/alecthomas/injector
 Author: Alec Thomas
 Author-email: alec@swapoff.org
 License: BSD
 Download-URL: http://pypi.python.org/pypi/injector
 Description: Injector - Python dependency injection framework, inspired by Guice
```

### Comparing `injector-0.9.0/injector.py` & `injector-0.9.1/injector.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     NullHandler = logging.NullHandler
 except AttributeError:
     class NullHandler(logging.Handler):
         def emit(self, record):
             pass
 
 __author__ = 'Alec Thomas <alec@swapoff.org>'
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 __version_tag__ = ''
 
 log = logging.getLogger('injector')
 log.addHandler(NullHandler())
 
 if log.level == logging.NOTSET:
     log.setLevel(logging.WARN)
@@ -966,15 +966,15 @@
         return inject
 
     def class_wrapper(cls):
         orig_init = cls.__init__
 
         original_keys = tuple(bindings.keys())
 
-        for k in bindings:
+        for k in list(bindings.keys()):
             bindings[k.lstrip('_')] = bindings.pop(k)
 
         @inject(**bindings)
         def init(self, *args, **kwargs):
             try:
                 for key in original_keys:
                     normalized_key = key.lstrip('_')
```

### Comparing `injector-0.9.0/PKG-INFO` & `injector-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: injector
-Version: 0.9.0
+Version: 0.9.1
 Summary: Injector - Python dependency injection framework, inspired by Guice
 Home-page: http://github.com/alecthomas/injector
 Author: Alec Thomas
 Author-email: alec@swapoff.org
 License: BSD
 Download-URL: http://pypi.python.org/pypi/injector
 Description: Injector - Python dependency injection framework, inspired by Guice
```

### Comparing `injector-0.9.0/README.md` & `injector-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `injector-0.9.0/README.rst` & `injector-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `injector-0.9.0/setup.py` & `injector-0.9.1/setup.py`

 * *Files identical despite different names*

