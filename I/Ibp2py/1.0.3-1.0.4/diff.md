# Comparing `tmp/Ibp2py-1.0.3.tar.gz` & `tmp/Ibp2py-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ibp2py-1.0.3.tar", last modified: Thu Jul 27 04:16:46 2023, max compression
+gzip compressed data, was "Ibp2py-1.0.4.tar", last modified: Thu Jul 27 04:26:11 2023, max compression
```

## Comparing `Ibp2py-1.0.3.tar` & `Ibp2py-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 04:16:46.243470 Ibp2py-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-07-27 04:16:46.191472 Ibp2py-1.0.3/Ibp2py.egg-info/
--rw-rw-rw-   0        0        0     2857 2023-07-27 04:16:45.000000 Ibp2py-1.0.3/Ibp2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-07-27 04:16:45.000000 Ibp2py-1.0.3/Ibp2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 04:16:45.000000 Ibp2py-1.0.3/Ibp2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-27 04:16:45.000000 Ibp2py-1.0.3/Ibp2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 04:16:45.000000 Ibp2py-1.0.3/Ibp2py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11524 2023-07-27 00:55:17.000000 Ibp2py-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2857 2023-07-27 04:16:46.227474 Ibp2py-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2121 2023-07-27 00:53:53.000000 Ibp2py-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 04:16:46.216473 Ibp2py-1.0.3/ibp2py/
--rw-rw-rw-   0        0        0    21802 2023-07-27 01:39:48.000000 Ibp2py-1.0.3/ibp2py/Ibp2py.py
--rw-rw-rw-   0        0        0       23 2023-07-27 02:58:43.000000 Ibp2py-1.0.3/ibp2py/__init__.py
--rw-rw-rw-   0        0        0     1924 2023-07-26 22:52:07.000000 Ibp2py-1.0.3/ibp2py/teste.py
--rw-rw-rw-   0        0        0       42 2023-07-27 04:16:46.243470 Ibp2py-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1027 2023-07-27 04:16:36.000000 Ibp2py-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 04:26:10.995810 Ibp2py-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-27 04:26:10.958810 Ibp2py-1.0.4/Ibp2py.egg-info/
+-rw-rw-rw-   0        0        0     2857 2023-07-27 04:26:10.000000 Ibp2py-1.0.4/Ibp2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-07-27 04:26:10.000000 Ibp2py-1.0.4/Ibp2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 04:26:10.000000 Ibp2py-1.0.4/Ibp2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-27 04:26:10.000000 Ibp2py-1.0.4/Ibp2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 04:26:10.000000 Ibp2py-1.0.4/Ibp2py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11524 2023-07-27 00:55:17.000000 Ibp2py-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2857 2023-07-27 04:26:10.991808 Ibp2py-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2121 2023-07-27 00:53:53.000000 Ibp2py-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 04:26:10.981807 Ibp2py-1.0.4/ibp2py/
+-rw-rw-rw-   0        0        0    21802 2023-07-27 01:39:48.000000 Ibp2py-1.0.4/ibp2py/Ibp2py.py
+-rw-rw-rw-   0        0        0       23 2023-07-27 04:25:52.000000 Ibp2py-1.0.4/ibp2py/__init__.py
+-rw-rw-rw-   0        0        0     1924 2023-07-26 22:52:07.000000 Ibp2py-1.0.4/ibp2py/teste.py
+-rw-rw-rw-   0        0        0       42 2023-07-27 04:26:10.997807 Ibp2py-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2023-07-27 04:26:00.000000 Ibp2py-1.0.4/setup.py
```

### Comparing `Ibp2py-1.0.3/Ibp2py.egg-info/PKG-INFO` & `Ibp2py-1.0.4/Ibp2py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ibp2py
-Version: 1.0.3
+Version: 1.0.4
 Summary: SAP Data Retrieval and Processing Library for IBP
 Home-page: https://github.com/pedrorastha/ibp2py
 Author: Pedro Rastha
 Author-email: pedrorastha@gmail.com
 Keywords: SAP IBP API ODATA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `Ibp2py-1.0.3/LICENSE` & `Ibp2py-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Ibp2py-1.0.3/PKG-INFO` & `Ibp2py-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ibp2py
-Version: 1.0.3
+Version: 1.0.4
 Summary: SAP Data Retrieval and Processing Library for IBP
 Home-page: https://github.com/pedrorastha/ibp2py
 Author: Pedro Rastha
 Author-email: pedrorastha@gmail.com
 Keywords: SAP IBP API ODATA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `Ibp2py-1.0.3/README.md` & `Ibp2py-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Ibp2py-1.0.3/ibp2py/Ibp2py.py` & `Ibp2py-1.0.4/ibp2py/Ibp2py.py`

 * *Files identical despite different names*

### Comparing `Ibp2py-1.0.3/ibp2py/teste.py` & `Ibp2py-1.0.4/ibp2py/teste.py`

 * *Files identical despite different names*

### Comparing `Ibp2py-1.0.3/setup.py` & `Ibp2py-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open ('README.md', 'r') as arq:
     readme = arq.read()
 
 setup(
     name='Ibp2py',
-    version='1.0.3',
+    version='1.0.4',
     author='Pedro Rastha',
     author_email='pedrorastha@gmail.com',
     description='SAP Data Retrieval and Processing Library for IBP',
     long_description=f'{readme}',
     long_description_content_type='text/markdown',
     url='https://github.com/pedrorastha/ibp2py',
     keywords='SAP IBP API ODATA',
```

