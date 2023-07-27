# Comparing `tmp/ak-ipatool-py-0.0.4.tar.gz` & `tmp/ak-ipatool-py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak-ipatool-py-0.0.4.tar", last modified: Thu Jul 27 11:06:27 2023, max compression
+gzip compressed data, was "ak-ipatool-py-0.0.5.tar", last modified: Thu Jul 27 11:54:07 2023, max compression
```

## Comparing `ak-ipatool-py-0.0.4.tar` & `ak-ipatool-py-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,26 @@
-drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-07-27 11:06:27.455834 ak-ipatool-py-0.0.4/
--rw-r--r--   0 subho      (501) staff       (20)      361 2023-07-27 11:06:27.455972 ak-ipatool-py-0.0.4/PKG-INFO
--rw-r--r--   0 subho      (501) staff       (20)     3162 2023-06-16 14:09:40.000000 ak-ipatool-py-0.0.4/README.md
-drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-07-27 11:06:27.453860 ak-ipatool-py-0.0.4/ak_ipatool_py.egg-info/
--rw-r--r--   0 subho      (501) staff       (20)      361 2023-07-27 11:06:27.000000 ak-ipatool-py-0.0.4/ak_ipatool_py.egg-info/PKG-INFO
--rw-r--r--   0 subho      (501) staff       (20)      316 2023-07-27 11:06:27.000000 ak-ipatool-py-0.0.4/ak_ipatool_py.egg-info/SOURCES.txt
--rw-r--r--   0 subho      (501) staff       (20)        1 2023-07-27 11:06:27.000000 ak-ipatool-py-0.0.4/ak_ipatool_py.egg-info/dependency_links.txt
--rw-r--r--   0 subho      (501) staff       (20)       40 2023-07-27 11:06:27.000000 ak-ipatool-py-0.0.4/ak_ipatool_py.egg-info/entry_points.txt
--rw-r--r--   0 subho      (501) staff       (20)       25 2023-07-27 11:06:27.000000 ak-ipatool-py-0.0.4/ak_ipatool_py.egg-info/requires.txt
--rw-r--r--   0 subho      (501) staff       (20)       11 2023-07-27 11:06:27.000000 ak-ipatool-py-0.0.4/ak_ipatool_py.egg-info/top_level.txt
-drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-07-27 11:06:27.455165 ak-ipatool-py-0.0.4/ipatool_py/
--rwxr-xr-x   0 subho      (501) staff       (20)      406 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.4/ipatool_py/__init__.py
--rwxr-xr-x   0 subho      (501) staff       (20)     4774 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.4/ipatool_py/itunes.py
--rwxr-xr-x   0 subho      (501) staff       (20)     7795 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.4/ipatool_py/store.py
--rw-r--r--   0 subho      (501) staff       (20)      172 2023-07-27 11:06:27.456592 ak-ipatool-py-0.0.4/setup.cfg
--rw-r--r--   0 subho      (501) staff       (20)      660 2023-07-27 11:06:19.000000 ak-ipatool-py-0.0.4/setup.py
+drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-07-27 11:54:07.664578 ak-ipatool-py-0.0.5/
+-rw-r--r--   0 subho      (501) staff       (20)      361 2023-07-27 11:54:07.664741 ak-ipatool-py-0.0.5/PKG-INFO
+-rw-r--r--   0 subho      (501) staff       (20)     3162 2023-06-16 14:09:40.000000 ak-ipatool-py-0.0.5/README.md
+drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-07-27 11:54:07.649177 ak-ipatool-py-0.0.5/ak_ipatool_py.egg-info/
+-rw-r--r--   0 subho      (501) staff       (20)      361 2023-07-27 11:54:07.000000 ak-ipatool-py-0.0.5/ak_ipatool_py.egg-info/PKG-INFO
+-rw-r--r--   0 subho      (501) staff       (20)      678 2023-07-27 11:54:07.000000 ak-ipatool-py-0.0.5/ak_ipatool_py.egg-info/SOURCES.txt
+-rw-r--r--   0 subho      (501) staff       (20)        1 2023-07-27 11:54:07.000000 ak-ipatool-py-0.0.5/ak_ipatool_py.egg-info/dependency_links.txt
+-rw-r--r--   0 subho      (501) staff       (20)       40 2023-07-27 11:54:07.000000 ak-ipatool-py-0.0.5/ak_ipatool_py.egg-info/entry_points.txt
+-rw-r--r--   0 subho      (501) staff       (20)       25 2023-07-27 11:54:07.000000 ak-ipatool-py-0.0.5/ak_ipatool_py.egg-info/requires.txt
+-rw-r--r--   0 subho      (501) staff       (20)       11 2023-07-27 11:54:07.000000 ak-ipatool-py-0.0.5/ak_ipatool_py.egg-info/top_level.txt
+drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-07-27 11:54:07.650852 ak-ipatool-py-0.0.5/ipatool_py/
+-rwxr-xr-x   0 subho      (501) staff       (20)      406 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.5/ipatool_py/__init__.py
+-rwxr-xr-x   0 subho      (501) staff       (20)     4774 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.5/ipatool_py/itunes.py
+drwxr-xr-x   0 subho      (501) staff       (20)        0 2023-07-27 11:54:07.662427 ak-ipatool-py-0.0.5/ipatool_py/schemas/
+-rw-r--r--   0 subho      (501) staff       (20)      683 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.5/ipatool_py/schemas/README.md
+-rwxr-xr-x   0 subho      (501) staff       (20)      618 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.5/ipatool_py/schemas/__init__.py
+-rwxr-xr-x   0 subho      (501) staff       (20)    62860 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.5/ipatool_py/schemas/itunes_lookup_resp.py
+-rwxr-xr-x   0 subho      (501) staff       (20)     7530 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.5/ipatool_py/schemas/store_authenticate_req.py
+-rwxr-xr-x   0 subho      (501) staff       (20)   100271 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.5/ipatool_py/schemas/store_authenticate_resp.py
+-rw-r--r--   0 subho      (501) staff       (20)    27435 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.5/ipatool_py/schemas/store_buyproduct_req.py
+-rw-r--r--   0 subho      (501) staff       (20)   218096 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.5/ipatool_py/schemas/store_buyproduct_resp.py
+-rwxr-xr-x   0 subho      (501) staff       (20)     5001 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.5/ipatool_py/schemas/store_download_req.py
+-rwxr-xr-x   0 subho      (501) staff       (20)   151466 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.5/ipatool_py/schemas/store_download_resp.py
+-rwxr-xr-x   0 subho      (501) staff       (20)     7795 2023-07-27 11:00:04.000000 ak-ipatool-py-0.0.5/ipatool_py/store.py
+-rw-r--r--   0 subho      (501) staff       (20)      172 2023-07-27 11:54:07.665322 ak-ipatool-py-0.0.5/setup.cfg
+-rw-r--r--   0 subho      (501) staff       (20)      708 2023-07-27 11:53:57.000000 ak-ipatool-py-0.0.5/setup.py
```

### Comparing `ak-ipatool-py-0.0.4/README.md` & `ak-ipatool-py-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ak-ipatool-py-0.0.4/ipatool_py/itunes.py` & `ak-ipatool-py-0.0.5/ipatool_py/itunes.py`

 * *Files identical despite different names*

### Comparing `ak-ipatool-py-0.0.4/ipatool_py/store.py` & `ak-ipatool-py-0.0.5/ipatool_py/store.py`

 * *Files identical despite different names*

### Comparing `ak-ipatool-py-0.0.4/setup.py` & `ak-ipatool-py-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools
 
-__VERSION__ = '0.0.4'
+__VERSION__ = '0.0.5'
 
 setuptools.setup(
     name='ak-ipatool-py',
     version=__VERSION__,
     entry_points={
         'console_scripts': [
             'ipatoolpy = main:main'
         ]
     },
     author='appknox',
     author_email='engineering@appknox.com',
     url='https://github.com/appknox/ak-ipatool-py',
     description='Appknox forked ipatoolpy is a command line tool that allows you to search for iOS apps on the App Store and download a copy of the app package, known as an ipa file.',
     packages=['ipatool_py'],
+    package_data={'ipatool_py': ['schemas/*']},
     install_requires=[
         'setuptools',
         'requests',
         'rich'
     ],
     python_requires='>=3.7'
 )
```

