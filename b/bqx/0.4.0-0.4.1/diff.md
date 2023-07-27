# Comparing `tmp/bqx-0.4.0.tar.gz` & `tmp/bqx-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bqx-0.4.0.tar", last modified: Tue Apr  4 04:33:46 2017, max compression
+gzip compressed data, was "bqx-0.4.1.tar", last modified: Thu Jul 27 08:31:06 2023, max compression
```

## Comparing `bqx-0.4.0.tar` & `bqx-0.4.1.tar`

### file list

```diff
@@ -1,46 +1,29 @@
-drwxr-xr-x   0 Takumi     (501) staff       (20)        0 2017-04-04 04:33:46.000000 bqx-0.4.0/
-drwxr-xr-x   0 Takumi     (501) staff       (20)        0 2017-04-04 04:33:46.000000 bqx-0.4.0/bqx/
--rw-r--r--   0 Takumi     (501) staff       (20)        0 2016-01-12 12:59:49.000000 bqx-0.4.0/bqx/__init__.py
--rw-r--r--   0 Takumi     (501) staff       (20)      996 2016-11-01 05:04:04.000000 bqx-0.4.0/bqx/_func.py
--rw-r--r--   0 Takumi     (501) staff       (20)     3457 2016-03-16 06:12:47.000000 bqx-0.4.0/bqx/_func_generator.py
--rw-r--r--   0 Takumi     (501) staff       (20)     2857 2016-03-16 02:52:19.000000 bqx-0.4.0/bqx/abstract.py
--rw-r--r--   0 Takumi     (501) staff       (20)     6314 2017-04-04 04:11:55.000000 bqx-0.4.0/bqx/func.py
--rw-r--r--   0 Takumi     (501) staff       (20)     3720 2017-04-04 04:13:46.000000 bqx-0.4.0/bqx/parts.py
--rw-r--r--   0 Takumi     (501) staff       (20)     7676 2017-03-31 06:04:24.000000 bqx-0.4.0/bqx/query.py
-drwxr-xr-x   0 Takumi     (501) staff       (20)        0 2017-04-04 04:33:46.000000 bqx-0.4.0/bqx.egg-info/
--rw-r--r--   0 Takumi     (501) staff       (20)        1 2017-04-04 04:33:46.000000 bqx-0.4.0/bqx.egg-info/dependency_links.txt
--rw-r--r--   0 Takumi     (501) staff       (20)     4168 2017-04-04 04:33:46.000000 bqx-0.4.0/bqx.egg-info/PKG-INFO
--rw-r--r--   0 Takumi     (501) staff       (20)     1138 2017-04-04 04:33:46.000000 bqx-0.4.0/bqx.egg-info/SOURCES.txt
--rw-r--r--   0 Takumi     (501) staff       (20)        4 2017-04-04 04:33:46.000000 bqx-0.4.0/bqx.egg-info/top_level.txt
-drwxr-xr-x   0 Takumi     (501) staff       (20)        0 2017-04-04 04:33:46.000000 bqx-0.4.0/example/
--rw-r--r--   0 Takumi     (501) staff       (20)     8393 2017-01-04 11:07:18.000000 bqx-0.4.0/example/get_started.ipynb
--rw-r-----   0 Takumi     (501) staff       (20)     3563 2016-01-12 15:16:21.000000 bqx-0.4.0/example/get_started.py
--rw-r--r--   0 Takumi     (501) staff       (20)    11503 2017-04-04 03:04:13.000000 bqx-0.4.0/example/pandas_demo.ipynb
--rw-r-----   0 Takumi     (501) staff       (20)     1091 2016-01-12 15:22:18.000000 bqx-0.4.0/example/pandas_demo.py
--rw-r--r--   0 Takumi     (501) staff       (20)     1494 2016-01-26 10:01:05.000000 bqx-0.4.0/LICENSE
--rw-r--r--   0 Takumi     (501) staff       (20)      106 2016-11-01 06:05:22.000000 bqx-0.4.0/MANIFEST.in
--rw-r--r--   0 Takumi     (501) staff       (20)     4168 2017-04-04 04:33:46.000000 bqx-0.4.0/PKG-INFO
--rw-r--r--   0 Takumi     (501) staff       (20)     2329 2016-03-16 04:59:56.000000 bqx-0.4.0/README.md
--rw-r--r--   0 Takumi     (501) staff       (20)     2572 2017-04-04 04:33:46.000000 bqx-0.4.0/README.rst
--rw-r--r--   0 Takumi     (501) staff       (20)       96 2017-04-04 04:33:46.000000 bqx-0.4.0/setup.cfg
--rw-r--r--   0 Takumi     (501) staff       (20)     2037 2017-04-04 04:13:46.000000 bqx-0.4.0/setup.py
-drwxr-xr-x   0 Takumi     (501) staff       (20)        0 2017-04-04 04:33:46.000000 bqx-0.4.0/tests/
--rw-r--r--   0 Takumi     (501) staff       (20)     6148 2016-01-28 00:27:51.000000 bqx-0.4.0/tests/.DS_Store
-drwxr-xr-x   0 Takumi     (501) staff       (20)        0 2017-04-04 04:33:46.000000 bqx-0.4.0/tests/__pycache__/
--rw-r--r--   0 Takumi     (501) staff       (20)     2724 2016-02-25 14:42:25.000000 bqx-0.4.0/tests/__pycache__/test_abstract.cpython-33-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)     1986 2016-02-25 07:21:52.000000 bqx-0.4.0/tests/__pycache__/test_abstract.cpython-34-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)     1960 2016-02-25 13:15:53.000000 bqx-0.4.0/tests/__pycache__/test_abstract.cpython-35-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)     9691 2016-11-01 04:39:48.000000 bqx-0.4.0/tests/__pycache__/test_func.cpython-33-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)     7115 2016-11-01 04:39:52.000000 bqx-0.4.0/tests/__pycache__/test_func.cpython-34-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)     7034 2016-11-01 04:39:55.000000 bqx-0.4.0/tests/__pycache__/test_func.cpython-35-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)     9296 2016-11-01 04:48:53.000000 bqx-0.4.0/tests/__pycache__/test_parts.cpython-33-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)     7214 2016-11-01 04:48:56.000000 bqx-0.4.0/tests/__pycache__/test_parts.cpython-34-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)     8933 2017-04-04 04:11:56.000000 bqx-0.4.0/tests/__pycache__/test_parts.cpython-35-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)    22910 2016-01-13 00:37:41.000000 bqx-0.4.0/tests/__pycache__/test_query.cpython-27-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)    42715 2016-11-01 04:48:53.000000 bqx-0.4.0/tests/__pycache__/test_query.cpython-33-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)    32586 2016-11-01 04:48:56.000000 bqx-0.4.0/tests/__pycache__/test_query.cpython-34-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)    32117 2017-01-04 10:41:23.000000 bqx-0.4.0/tests/__pycache__/test_query.cpython-35-PYTEST.pyc
--rw-r--r--   0 Takumi     (501) staff       (20)      397 2016-01-13 14:33:43.000000 bqx-0.4.0/tests/test_abstract.py
--rw-r--r--   0 Takumi     (501) staff       (20)      891 2016-07-05 01:48:50.000000 bqx-0.4.0/tests/test_func.py
--rw-r--r--   0 Takumi     (501) staff       (20)     1916 2017-04-04 04:13:46.000000 bqx-0.4.0/tests/test_parts.py
--rw-r--r--   0 Takumi     (501) staff       (20)     6813 2016-11-01 05:04:04.000000 bqx-0.4.0/tests/test_query.py
+drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 08:31:06.011219 bqx-0.4.1/
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     1494 2023-07-26 06:53:46.000000 bqx-0.4.1/LICENSE
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)      106 2023-07-26 06:53:46.000000 bqx-0.4.1/MANIFEST.in
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)      753 2023-07-27 08:31:06.011351 bqx-0.4.1/PKG-INFO
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     2393 2023-07-27 07:19:29.000000 bqx-0.4.1/README.md
+drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 08:31:06.004761 bqx-0.4.1/bqx/
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)        0 2023-07-26 06:53:46.000000 bqx-0.4.1/bqx/__init__.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)      996 2023-07-26 06:53:46.000000 bqx-0.4.1/bqx/_func.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     3457 2023-07-26 06:53:46.000000 bqx-0.4.1/bqx/_func_generator.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     2857 2023-07-26 06:53:46.000000 bqx-0.4.1/bqx/abstract.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     3720 2023-07-26 06:53:46.000000 bqx-0.4.1/bqx/parts.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     7676 2023-07-26 06:53:46.000000 bqx-0.4.1/bqx/query.py
+drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 08:31:06.006929 bqx-0.4.1/bqx.egg-info/
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)      753 2023-07-27 08:31:05.000000 bqx-0.4.1/bqx.egg-info/PKG-INFO
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)      430 2023-07-27 08:31:05.000000 bqx-0.4.1/bqx.egg-info/SOURCES.txt
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)        1 2023-07-27 08:31:05.000000 bqx-0.4.1/bqx.egg-info/dependency_links.txt
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)        4 2023-07-27 08:31:05.000000 bqx-0.4.1/bqx.egg-info/top_level.txt
+drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 08:31:06.009014 bqx-0.4.1/example/
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     8393 2023-07-26 06:53:46.000000 bqx-0.4.1/example/get_started.ipynb
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     3563 2023-07-26 06:53:46.000000 bqx-0.4.1/example/get_started.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)    11503 2023-07-26 06:53:46.000000 bqx-0.4.1/example/pandas_demo.ipynb
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     1091 2023-07-26 06:53:46.000000 bqx-0.4.1/example/pandas_demo.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)       75 2023-07-27 08:31:06.011880 bqx-0.4.1/setup.cfg
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     1908 2023-07-27 07:38:02.000000 bqx-0.4.1/setup.py
+drwxr-xr-x   0 shogo.ichinose   (502) staff       (20)        0 2023-07-27 08:31:06.010954 bqx-0.4.1/tests/
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)      397 2023-07-26 06:53:46.000000 bqx-0.4.1/tests/test_abstract.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)      891 2023-07-26 06:53:46.000000 bqx-0.4.1/tests/test_func.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     1916 2023-07-26 06:53:46.000000 bqx-0.4.1/tests/test_parts.py
+-rw-r--r--   0 shogo.ichinose   (502) staff       (20)     6813 2023-07-26 06:53:46.000000 bqx-0.4.1/tests/test_query.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bqx-0.4.0/bqx/_func.py` & `bqx-0.4.1/bqx/_func.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.0/bqx/_func_generator.py` & `bqx-0.4.1/bqx/_func_generator.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.0/bqx/abstract.py` & `bqx-0.4.1/bqx/abstract.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.0/bqx/parts.py` & `bqx-0.4.1/bqx/parts.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.0/bqx/query.py` & `bqx-0.4.1/bqx/query.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.0/example/get_started.ipynb` & `bqx-0.4.1/example/get_started.ipynb`

 * *Files identical despite different names*

### Comparing `bqx-0.4.0/example/get_started.py` & `bqx-0.4.1/example/get_started.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.0/example/pandas_demo.ipynb` & `bqx-0.4.1/example/pandas_demo.ipynb`

 * *Files identical despite different names*

### Comparing `bqx-0.4.0/example/pandas_demo.py` & `bqx-0.4.1/example/pandas_demo.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.0/LICENSE` & `bqx-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bqx-0.4.0/README.md` & `bqx-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 BQX
 =====
 [![Build Status](https://img.shields.io/travis/fuller-inc/bqx/master.svg?style=flat-square)](https://travis-ci.org/fuller-inc/bqx)
 [![Coverage Status](https://img.shields.io/coveralls/fuller-inc/bqx/master.svg?style=flat-square)](https://coveralls.io/github/fuller-inc/bqx?branch=master)
 
-Generage sophisticated query for Google BigQuery in simple way.
+Generate sophisticated query for Google BigQuery in simple way.
 
+## ARCHIVED
+
+This project is archived and no longer maintained.
 
 ## What is BQX?
 BQX is a minimal query generator for Google BigQuery.
 It's mainly intended for being used by data analysts / scientists
 who want to analyze big data.
 
 BQX fires its power especially on making LONG and NESTED query.
```

### Comparing `bqx-0.4.0/setup.py` & `bqx-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,32 +17,30 @@
     readme = ''
 
 if 'install' in sys.argv or 'test' in sys.argv:
     funcpy_in = os.path.join(here, 'bqx/_func.py')
     funcpy = os.path.join(here, 'bqx/func.py')
     generate_funcpy(funcpy_in, funcpy)
 
-__version__ = '0.4.0'
-__author__ = 'Takumi Sueda'
-__author_email__ = 'takumi.sueda@fuller.co.jp'
+__version__ = '0.4.1'
 __license__ = 'BSD License'
-__classifiers__ = (
-    'Development Status :: 4 - Beta',
+__classifiers__ = [
+    'Development Status :: 7 - Inactive',
     'Environment :: Console',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: SQL',
     'Topic :: Database',
     'Topic :: Software Development :: Code Generators',
-)
+]
 
 
 class PyTest(TestCommand):
     def finalize_options(self):
         TestCommand.finalize_options(self)
         self.test_args = []
         self.test_suite = True
@@ -50,16 +48,14 @@
     def run_tests(self):
         import pytest
         pytest.main(self.test_args)
 
 setup(
     name='bqx',
     version=__version__,
-    author=__author__,
-    author_email=__author_email__,
     url='https://github.com/fuller-inc/bqx',
     description='Query generator for Google BigQuery and other SQL environments',
     long_description=readme,
     classifiers=__classifiers__,
     packages=find_packages(exclude=['test*']),
     license=__license__,
     include_package_data=True,
```

### Comparing `bqx-0.4.0/tests/test_func.py` & `bqx-0.4.1/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.0/tests/test_parts.py` & `bqx-0.4.1/tests/test_parts.py`

 * *Files identical despite different names*

### Comparing `bqx-0.4.0/tests/test_query.py` & `bqx-0.4.1/tests/test_query.py`

 * *Files identical despite different names*

