# Comparing `tmp/veris-priv-tab-0.1.0.tar.gz` & `tmp/veris-priv-tab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veris-priv-tab-0.1.0.tar", last modified: Wed Jul 26 22:48:02 2023, max compression
+gzip compressed data, was "veris-priv-tab-0.1.1.tar", last modified: Wed Jul 26 22:54:37 2023, max compression
```

## Comparing `veris-priv-tab-0.1.0.tar` & `veris-priv-tab-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 aditya    (1000) aditya    (1000)        0 2023-07-26 22:48:02.731197 veris-priv-tab-0.1.0/
--rw-rw-r--   0 aditya    (1000) aditya    (1000)     1341 2023-07-26 22:48:02.731197 veris-priv-tab-0.1.0/PKG-INFO
--rw-rw-r--   0 aditya    (1000) aditya    (1000)      849 2023-07-26 22:46:54.000000 veris-priv-tab-0.1.0/README.md
--rw-rw-r--   0 aditya    (1000) aditya    (1000)       38 2023-07-26 22:48:02.731197 veris-priv-tab-0.1.0/setup.cfg
--rw-rw-r--   0 aditya    (1000) aditya    (1000)      742 2023-07-26 22:47:19.000000 veris-priv-tab-0.1.0/setup.py
-drwxrwxr-x   0 aditya    (1000) aditya    (1000)        0 2023-07-26 22:48:02.731197 veris-priv-tab-0.1.0/veris_priv_tab.egg-info/
--rw-rw-r--   0 aditya    (1000) aditya    (1000)     1341 2023-07-26 22:48:02.000000 veris-priv-tab-0.1.0/veris_priv_tab.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1000) aditya    (1000)      207 2023-07-26 22:48:02.000000 veris-priv-tab-0.1.0/veris_priv_tab.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1000) aditya    (1000)        1 2023-07-26 22:48:02.000000 veris-priv-tab-0.1.0/veris_priv_tab.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1000) aditya    (1000)       16 2023-07-26 22:48:02.000000 veris-priv-tab-0.1.0/veris_priv_tab.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1000) aditya    (1000)        1 2023-07-26 22:48:02.000000 veris-priv-tab-0.1.0/veris_priv_tab.egg-info/top_level.txt
+drwxrwxr-x   0 aditya    (1000) aditya    (1000)        0 2023-07-26 22:54:37.000804 veris-priv-tab-0.1.1/
+-rw-rw-r--   0 aditya    (1000) aditya    (1000)     1341 2023-07-26 22:54:37.000804 veris-priv-tab-0.1.1/PKG-INFO
+-rw-rw-r--   0 aditya    (1000) aditya    (1000)      849 2023-07-26 22:46:54.000000 veris-priv-tab-0.1.1/README.md
+-rw-rw-r--   0 aditya    (1000) aditya    (1000)       38 2023-07-26 22:54:37.000804 veris-priv-tab-0.1.1/setup.cfg
+-rw-rw-r--   0 aditya    (1000) aditya    (1000)      742 2023-07-26 22:54:13.000000 veris-priv-tab-0.1.1/setup.py
+drwxrwxr-x   0 aditya    (1000) aditya    (1000)        0 2023-07-26 22:54:37.000804 veris-priv-tab-0.1.1/veris_priv_tab.egg-info/
+-rw-rw-r--   0 aditya    (1000) aditya    (1000)     1341 2023-07-26 22:54:36.000000 veris-priv-tab-0.1.1/veris_priv_tab.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1000) aditya    (1000)      207 2023-07-26 22:54:36.000000 veris-priv-tab-0.1.1/veris_priv_tab.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1000) aditya    (1000)        1 2023-07-26 22:54:36.000000 veris-priv-tab-0.1.1/veris_priv_tab.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1000) aditya    (1000)       16 2023-07-26 22:54:36.000000 veris-priv-tab-0.1.1/veris_priv_tab.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1000) aditya    (1000)        1 2023-07-26 22:54:36.000000 veris-priv-tab-0.1.1/veris_priv_tab.egg-info/top_level.txt
```

### Comparing `veris-priv-tab-0.1.0/PKG-INFO` & `veris-priv-tab-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veris-priv-tab
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generates a "private duplicate" of a given table, obfuscating any potential PII.
 Home-page: http://veris.ai
 Author: Aditya Rai
 Author-email: team@veris.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `veris-priv-tab-0.1.0/README.md` & `veris-priv-tab-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `veris-priv-tab-0.1.0/setup.py` & `veris-priv-tab-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='veris-priv-tab',
-    version='0.1.0',
+    version='0.1.1',
     author='Aditya Rai',
     author_email='team@veris.ai',
     packages=find_packages(),
     description='Generates a "private duplicate" of a given table, obfuscating any potential PII.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='http://veris.ai',  # replace with the real url of your package
```

### Comparing `veris-priv-tab-0.1.0/veris_priv_tab.egg-info/PKG-INFO` & `veris-priv-tab-0.1.1/veris_priv_tab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veris-priv-tab
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generates a "private duplicate" of a given table, obfuscating any potential PII.
 Home-page: http://veris.ai
 Author: Aditya Rai
 Author-email: team@veris.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

