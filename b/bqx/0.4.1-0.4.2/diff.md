# Comparing `tmp/bqx-0.4.1.tar.gz` & `tmp/bqx-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqx-0.4.1.tar", last modified: Thu Jul 27 08:31:06 2023, max compression
+gzip compressed data, was "bqx-0.4.2.tar", last modified: Thu Jul 27 09:05:26 2023, max compression
```

## Comparing `bqx-0.4.1.tar` & `bqx-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 08:31:06.011219 bqx-0.4.1/
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)     1494 2023-07-26 06:53:46.000000 bqx-0.4.1/LICENSE
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)      106 2023-07-26 06:53:46.000000 bqx-0.4.1/MANIFEST.in
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)      753 2023-07-27 08:31:06.011351 bqx-0.4.1/PKG-INFO
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)     2393 2023-07-27 07:19:29.000000 bqx-0.4.1/README.md
-drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 08:31:06.004761 bqx-0.4.1/bqx/
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)        0 2023-07-26 06:53:46.000000 bqx-0.4.1/bqx/__init__.py
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)      996 2023-07-26 06:53:46.000000 bqx-0.4.1/bqx/_func.py
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)     3457 2023-07-26 06:53:46.000000 bqx-0.4.1/bqx/_func_generator.py
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)     2857 2023-07-26 06:53:46.000000 bqx-0.4.1/bqx/abstract.py
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)     3720 2023-07-26 06:53:46.000000 bqx-0.4.1/bqx/parts.py
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)     7676 2023-07-26 06:53:46.000000 bqx-0.4.1/bqx/query.py
-drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 08:31:06.006929 bqx-0.4.1/bqx.egg-info/
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)      753 2023-07-27 08:31:05.000000 bqx-0.4.1/bqx.egg-info/PKG-INFO
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)      430 2023-07-27 08:31:05.000000 bqx-0.4.1/bqx.egg-info/SOURCES.txt
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)        1 2023-07-27 08:31:05.000000 bqx-0.4.1/bqx.egg-info/dependency_links.txt
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)        4 2023-07-27 08:31:05.000000 bqx-0.4.1/bqx.egg-info/top_level.txt
-drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 08:31:06.009014 bqx-0.4.1/example/
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)     8393 2023-07-26 06:53:46.000000 bqx-0.4.1/example/get_started.ipynb
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)     3563 2023-07-26 06:53:46.000000 bqx-0.4.1/example/get_started.py
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)    11503 2023-07-26 06:53:46.000000 bqx-0.4.1/example/pandas_demo.ipynb
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)     1091 2023-07-26 06:53:46.000000 bqx-0.4.1/example/pandas_demo.py
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)       75 2023-07-27 08:31:06.011880 bqx-0.4.1/setup.cfg
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)     1908 2023-07-27 07:38:02.000000 bqx-0.4.1/setup.py
-drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 08:31:06.010954 bqx-0.4.1/tests/
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)      397 2023-07-26 06:53:46.000000 bqx-0.4.1/tests/test_abstract.py
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)      891 2023-07-26 06:53:46.000000 bqx-0.4.1/tests/test_func.py
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)     1916 2023-07-26 06:53:46.000000 bqx-0.4.1/tests/test_parts.py
--rw-r--r--   0 shogo.ichinose   (502) staff       (20)     6813 2023-07-26 06:53:46.000000 bqx-0.4.1/tests/test_query.py
+drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 09:05:26.623626 bqx-0.4.2/
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     1494 2023-07-26 06:53:46.000000 bqx-0.4.2/LICENSE
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)      106 2023-07-26 06:53:46.000000 bqx-0.4.2/MANIFEST.in
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     3399 2023-07-27 09:05:26.623770 bqx-0.4.2/PKG-INFO
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     2393 2023-07-27 07:19:29.000000 bqx-0.4.2/README.md
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     2645 2023-07-27 09:05:26.000000 bqx-0.4.2/README.rst
+drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 09:05:26.616888 bqx-0.4.2/bqx/
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)        0 2023-07-26 06:53:46.000000 bqx-0.4.2/bqx/__init__.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)      996 2023-07-26 06:53:46.000000 bqx-0.4.2/bqx/_func.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     3457 2023-07-26 06:53:46.000000 bqx-0.4.2/bqx/_func_generator.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     2857 2023-07-26 06:53:46.000000 bqx-0.4.2/bqx/abstract.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     3720 2023-07-26 06:53:46.000000 bqx-0.4.2/bqx/parts.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     7676 2023-07-26 06:53:46.000000 bqx-0.4.2/bqx/query.py
+drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 09:05:26.618589 bqx-0.4.2/bqx.egg-info/
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     3399 2023-07-27 09:05:26.000000 bqx-0.4.2/bqx.egg-info/PKG-INFO
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)      441 2023-07-27 09:05:26.000000 bqx-0.4.2/bqx.egg-info/SOURCES.txt
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)        1 2023-07-27 09:05:26.000000 bqx-0.4.2/bqx.egg-info/dependency_links.txt
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)        4 2023-07-27 09:05:26.000000 bqx-0.4.2/bqx.egg-info/top_level.txt
+drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 09:05:26.621297 bqx-0.4.2/example/
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     8393 2023-07-26 06:53:46.000000 bqx-0.4.2/example/get_started.ipynb
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     3563 2023-07-26 06:53:46.000000 bqx-0.4.2/example/get_started.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)    11503 2023-07-26 06:53:46.000000 bqx-0.4.2/example/pandas_demo.ipynb
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     1091 2023-07-26 06:53:46.000000 bqx-0.4.2/example/pandas_demo.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)       75 2023-07-27 09:05:26.624836 bqx-0.4.2/setup.cfg
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     1908 2023-07-27 09:04:58.000000 bqx-0.4.2/setup.py
+drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 09:05:26.623282 bqx-0.4.2/tests/
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)      397 2023-07-26 06:53:46.000000 bqx-0.4.2/tests/test_abstract.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)      891 2023-07-26 06:53:46.000000 bqx-0.4.2/tests/test_func.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     1916 2023-07-26 06:53:46.000000 bqx-0.4.2/tests/test_parts.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     6813 2023-07-26 06:53:46.000000 bqx-0.4.2/tests/test_query.py
```

### Comparing `bqx-0.4.1/LICENSE` & `bqx-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/README.md` & `bqx-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/bqx/_func.py` & `bqx-0.4.2/bqx/_func.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/bqx/_func_generator.py` & `bqx-0.4.2/bqx/_func_generator.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/bqx/abstract.py` & `bqx-0.4.2/bqx/abstract.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/bqx/parts.py` & `bqx-0.4.2/bqx/parts.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/bqx/query.py` & `bqx-0.4.2/bqx/query.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/example/get_started.ipynb` & `bqx-0.4.2/example/get_started.ipynb`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/example/get_started.py` & `bqx-0.4.2/example/get_started.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/example/pandas_demo.ipynb` & `bqx-0.4.2/example/pandas_demo.ipynb`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/example/pandas_demo.py` & `bqx-0.4.2/example/pandas_demo.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/setup.py` & `bqx-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     readme = ''
 
 if 'install' in sys.argv or 'test' in sys.argv:
     funcpy_in = os.path.join(here, 'bqx/_func.py')
     funcpy = os.path.join(here, 'bqx/func.py')
     generate_funcpy(funcpy_in, funcpy)
 
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 __license__ = 'BSD License'
 __classifiers__ = [
     'Development Status :: 7 - Inactive',
     'Environment :: Console',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: BSD License',
```

### Comparing `bqx-0.4.1/tests/test_func.py` & `bqx-0.4.2/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/tests/test_parts.py` & `bqx-0.4.2/tests/test_parts.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.1/tests/test_query.py` & `bqx-0.4.2/tests/test_query.py`

 * *Files identical despite different names*

