# Comparing `tmp/panthon-0.1.1.tar.gz` & `tmp/panthon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panthon-0.1.1.tar", last modified: Thu Jul 27 17:43:25 2023, max compression
+gzip compressed data, was "panthon-0.1.2.tar", last modified: Thu Jul 27 17:57:22 2023, max compression
```

## Comparing `panthon-0.1.1.tar` & `panthon-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-27 17:43:25.712100 panthon-0.1.1/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1072 2023-07-23 10:41:07.000000 panthon-0.1.1/LICENSE
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      700 2023-07-27 17:43:25.711964 panthon-0.1.1/PKG-INFO
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1041 2023-07-27 17:32:12.000000 panthon-0.1.1/README.md
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-27 17:43:25.710590 panthon-0.1.1/panthon.egg-info/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      700 2023-07-27 17:43:25.000000 panthon-0.1.1/panthon.egg-info/PKG-INFO
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      353 2023-07-27 17:43:25.000000 panthon-0.1.1/panthon.egg-info/SOURCES.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)        1 2023-07-27 17:43:25.000000 panthon-0.1.1/panthon.egg-info/dependency_links.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)       22 2023-07-27 17:43:25.000000 panthon-0.1.1/panthon.egg-info/requires.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)        4 2023-07-27 17:43:25.000000 panthon-0.1.1/panthon.egg-info/top_level.txt
--rw-r--r--   0 nripeshniketan   (501) staff       (20)       38 2023-07-27 17:43:25.712162 panthon-0.1.1/setup.cfg
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1065 2023-07-27 17:37:36.000000 panthon-0.1.1/setup.py
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-27 17:43:25.711427 panthon-0.1.1/src/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      205 2023-07-27 12:21:02.000000 panthon-0.1.1/src/__init__.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1521 2023-07-27 12:21:21.000000 panthon-0.1.1/src/ddos_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1391 2023-07-27 12:21:17.000000 panthon-0.1.1/src/dos_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1605 2023-07-27 12:18:28.000000 panthon-0.1.1/src/mitm_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      392 2023-07-27 11:39:03.000000 panthon-0.1.1/src/random_string_generator.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      486 2023-07-27 12:07:07.000000 panthon-0.1.1/src/sql_injection.py
-drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-27 17:43:25.711722 panthon-0.1.1/test/
--rw-r--r--   0 nripeshniketan   (501) staff       (20)      443 2023-07-23 11:45:30.000000 panthon-0.1.1/test/test_ddos_attack.py
--rw-r--r--   0 nripeshniketan   (501) staff       (20)     1542 2023-07-23 15:46:37.000000 panthon-0.1.1/test/test_dos_attack.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-27 17:57:22.142251 panthon-0.1.2/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1072 2023-07-23 10:41:07.000000 panthon-0.1.2/LICENSE
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      700 2023-07-27 17:57:22.142116 panthon-0.1.2/PKG-INFO
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1041 2023-07-27 17:32:12.000000 panthon-0.1.2/README.md
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-27 17:57:22.140767 panthon-0.1.2/panthon.egg-info/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      700 2023-07-27 17:57:22.000000 panthon-0.1.2/panthon.egg-info/PKG-INFO
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      353 2023-07-27 17:57:22.000000 panthon-0.1.2/panthon.egg-info/SOURCES.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)        1 2023-07-27 17:57:22.000000 panthon-0.1.2/panthon.egg-info/dependency_links.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)       22 2023-07-27 17:57:22.000000 panthon-0.1.2/panthon.egg-info/requires.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)        4 2023-07-27 17:57:22.000000 panthon-0.1.2/panthon.egg-info/top_level.txt
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)       38 2023-07-27 17:57:22.142305 panthon-0.1.2/setup.cfg
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1065 2023-07-27 17:56:46.000000 panthon-0.1.2/setup.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-27 17:57:22.141620 panthon-0.1.2/src/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      205 2023-07-27 12:21:02.000000 panthon-0.1.2/src/__init__.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1521 2023-07-27 12:21:21.000000 panthon-0.1.2/src/ddos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1391 2023-07-27 12:21:17.000000 panthon-0.1.2/src/dos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     2065 2023-07-27 17:45:54.000000 panthon-0.1.2/src/mitm_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      392 2023-07-27 11:39:03.000000 panthon-0.1.2/src/random_string_generator.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      486 2023-07-27 12:07:07.000000 panthon-0.1.2/src/sql_injection.py
+drwxr-xr-x   0 nripeshniketan   (501) staff       (20)        0 2023-07-27 17:57:22.141917 panthon-0.1.2/test/
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)      443 2023-07-23 11:45:30.000000 panthon-0.1.2/test/test_ddos_attack.py
+-rw-r--r--   0 nripeshniketan   (501) staff       (20)     1542 2023-07-23 15:46:37.000000 panthon-0.1.2/test/test_dos_attack.py
```

### Comparing `panthon-0.1.1/LICENSE` & `panthon-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `panthon-0.1.1/PKG-INFO` & `panthon-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panthon
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Machine Learning-powered Cybersecurity Attack Simulation Library
 Home-page: https://github.com/nripeshn/panthon
 Author: Nripesh Niketan
 Author-email: nripesh14@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `panthon-0.1.1/README.md` & `panthon-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `panthon-0.1.1/panthon.egg-info/PKG-INFO` & `panthon-0.1.2/panthon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panthon
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Machine Learning-powered Cybersecurity Attack Simulation Library
 Home-page: https://github.com/nripeshn/panthon
 Author: Nripesh Niketan
 Author-email: nripesh14@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `panthon-0.1.1/setup.py` & `panthon-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Read in requirements.txt with specified encoding
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='panthon',
-    version='0.1.1',
+    version='0.1.2',
     url='https://github.com/nripeshn/panthon',
     author='Nripesh Niketan',
     author_email='nripesh14@gmail.com',
     description='A Machine Learning-powered Cybersecurity Attack Simulation Library',
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
```

### Comparing `panthon-0.1.1/src/ddos_attack.py` & `panthon-0.1.2/src/ddos_attack.py`

 * *Files identical despite different names*

### Comparing `panthon-0.1.1/src/dos_attack.py` & `panthon-0.1.2/src/dos_attack.py`

 * *Files identical despite different names*

### Comparing `panthon-0.1.1/test/test_dos_attack.py` & `panthon-0.1.2/test/test_dos_attack.py`

 * *Files identical despite different names*

