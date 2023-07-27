# Comparing `tmp/Ibp2py-1.0.1.tar.gz` & `tmp/Ibp2py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ibp2py-1.0.1.tar", last modified: Thu Jul 27 01:43:37 2023, max compression
+gzip compressed data, was "Ibp2py-1.0.2.tar", last modified: Thu Jul 27 03:02:40 2023, max compression
```

## Comparing `Ibp2py-1.0.1.tar` & `Ibp2py-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 01:43:37.092538 Ibp2py-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-27 01:43:36.933620 Ibp2py-1.0.1/API/
--rw-rw-rw-   0        0        0    21802 2023-07-27 01:39:48.000000 Ibp2py-1.0.1/API/Ibp2py.py
--rw-rw-rw-   0        0        0       52 2023-07-27 01:42:09.000000 Ibp2py-1.0.1/API/__init__.py
--rw-rw-rw-   0        0        0     1924 2023-07-26 22:52:07.000000 Ibp2py-1.0.1/API/teste.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:43:37.088539 Ibp2py-1.0.1/Ibp2py.egg-info/
--rw-rw-rw-   0        0        0      765 2023-07-27 01:43:36.000000 Ibp2py-1.0.1/Ibp2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-27 01:43:36.000000 Ibp2py-1.0.1/Ibp2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 01:43:36.000000 Ibp2py-1.0.1/Ibp2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-27 01:43:36.000000 Ibp2py-1.0.1/Ibp2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-27 01:43:36.000000 Ibp2py-1.0.1/Ibp2py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11524 2023-07-27 00:55:17.000000 Ibp2py-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      765 2023-07-27 01:43:37.091538 Ibp2py-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2121 2023-07-27 00:53:53.000000 Ibp2py-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-27 01:43:37.093538 Ibp2py-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      981 2023-07-27 01:26:01.000000 Ibp2py-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:02:40.446629 Ibp2py-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-27 03:02:40.388625 Ibp2py-1.0.2/API/
+-rw-rw-rw-   0        0        0    21802 2023-07-27 01:39:48.000000 Ibp2py-1.0.2/API/Ibp2py.py
+-rw-rw-rw-   0        0        0       23 2023-07-27 02:58:43.000000 Ibp2py-1.0.2/API/__init__.py
+-rw-rw-rw-   0        0        0     1924 2023-07-26 22:52:07.000000 Ibp2py-1.0.2/API/teste.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:02:40.442632 Ibp2py-1.0.2/Ibp2py.egg-info/
+-rw-rw-rw-   0        0        0     2857 2023-07-27 03:02:39.000000 Ibp2py-1.0.2/Ibp2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-27 03:02:40.000000 Ibp2py-1.0.2/Ibp2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 03:02:39.000000 Ibp2py-1.0.2/Ibp2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-27 03:02:39.000000 Ibp2py-1.0.2/Ibp2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-27 03:02:39.000000 Ibp2py-1.0.2/Ibp2py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11524 2023-07-27 00:55:17.000000 Ibp2py-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2857 2023-07-27 03:02:40.445628 Ibp2py-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2121 2023-07-27 00:53:53.000000 Ibp2py-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 03:02:40.447626 Ibp2py-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2023-07-27 03:02:33.000000 Ibp2py-1.0.2/setup.py
```

### Comparing `Ibp2py-1.0.1/API/Ibp2py.py` & `Ibp2py-1.0.2/API/Ibp2py.py`

 * *Files identical despite different names*

### Comparing `Ibp2py-1.0.1/API/teste.py` & `Ibp2py-1.0.2/API/teste.py`

 * *Files identical despite different names*

### Comparing `Ibp2py-1.0.1/LICENSE` & `Ibp2py-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Ibp2py-1.0.1/README.md` & `Ibp2py-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Ibp2py-1.0.1/setup.py` & `Ibp2py-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from setuptools import setup, find_packages
 
+with open ('README.md', 'r') as arq:
+    readme = arq.read()
+
 setup(
     name='Ibp2py',
-    version='1.0.1',
+    version='1.0.2',
     author='Pedro Rastha',
     author_email='pedrorastha@gmail.com',
     description='SAP Data Retrieval and Processing Library for IBP',
-    long_description='A Python library to fetch and process data from SAP IBP.',
+    long_description=f'{readme}',
     long_description_content_type='text/markdown',
     url='https://github.com/pedrorastha/ibp2py',
-    packages=find_packages(),
+    keywords='SAP IBP API ODATA',
+    packages=['API'],
     install_requires=[
         'requests>=2.28.1',
         'pandas>=1.5.2',
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

