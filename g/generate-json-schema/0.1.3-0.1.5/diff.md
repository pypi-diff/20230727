# Comparing `tmp/generate-json-schema-0.1.3.tar.gz` & `tmp/generate-json-schema-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate-json-schema-0.1.3.tar", last modified: Wed Jul 26 19:00:04 2023, max compression
+gzip compressed data, was "generate-json-schema-0.1.5.tar", last modified: Thu Jul 27 18:13:54 2023, max compression
```

## Comparing `generate-json-schema-0.1.3.tar` & `generate-json-schema-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 fernnando   (501) staff       (20)        0 2023-07-26 19:00:04.166418 generate-json-schema-0.1.3/
--rw-r--r--   0 fernnando   (501) staff       (20)     1234 2023-07-26 19:00:04.165785 generate-json-schema-0.1.3/PKG-INFO
--rw-r--r--   0 fernnando   (501) staff       (20)      522 2023-07-26 18:59:42.000000 generate-json-schema-0.1.3/README.rst
-drwxr-xr-x   0 fernnando   (501) staff       (20)        0 2023-07-26 19:00:04.163607 generate-json-schema-0.1.3/generate_json_schema.egg-info/
--rw-r--r--   0 fernnando   (501) staff       (20)     1234 2023-07-26 19:00:04.000000 generate-json-schema-0.1.3/generate_json_schema.egg-info/PKG-INFO
--rw-r--r--   0 fernnando   (501) staff       (20)      234 2023-07-26 19:00:04.000000 generate-json-schema-0.1.3/generate_json_schema.egg-info/SOURCES.txt
--rw-r--r--   0 fernnando   (501) staff       (20)        1 2023-07-26 19:00:04.000000 generate-json-schema-0.1.3/generate_json_schema.egg-info/dependency_links.txt
--rw-r--r--   0 fernnando   (501) staff       (20)       22 2023-07-26 19:00:04.000000 generate-json-schema-0.1.3/generate_json_schema.egg-info/top_level.txt
--rw-r--r--   0 fernnando   (501) staff       (20)       38 2023-07-26 19:00:04.167612 generate-json-schema-0.1.3/setup.cfg
--rw-r--r--   0 fernnando   (501) staff       (20)     1763 2023-07-26 18:58:32.000000 generate-json-schema-0.1.3/setup.py
-drwxr-xr-x   0 fernnando   (501) staff       (20)        0 2023-07-26 19:00:04.164424 generate-json-schema-0.1.3/src/
--rw-r--r--   0 fernnando   (501) staff       (20)        0 2023-07-25 18:41:19.000000 generate-json-schema-0.1.3/src/__init__.py
--rw-r--r--   0 fernnando   (501) staff       (20)     2056 2023-07-26 13:48:52.000000 generate-json-schema-0.1.3/src/generate_schema.py
+drwxr-xr-x   0 fernnando   (501) staff       (20)        0 2023-07-27 18:13:54.535642 generate-json-schema-0.1.5/
+-rw-r--r--   0 fernnando   (501) staff       (20)     1234 2023-07-27 18:13:54.535000 generate-json-schema-0.1.5/PKG-INFO
+-rw-r--r--   0 fernnando   (501) staff       (20)      522 2023-07-26 18:59:42.000000 generate-json-schema-0.1.5/README.rst
+drwxr-xr-x   0 fernnando   (501) staff       (20)        0 2023-07-27 18:13:54.533145 generate-json-schema-0.1.5/generate_json_schema.egg-info/
+-rw-r--r--   0 fernnando   (501) staff       (20)     1234 2023-07-27 18:13:54.000000 generate-json-schema-0.1.5/generate_json_schema.egg-info/PKG-INFO
+-rw-r--r--   0 fernnando   (501) staff       (20)      234 2023-07-27 18:13:54.000000 generate-json-schema-0.1.5/generate_json_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 fernnando   (501) staff       (20)        1 2023-07-27 18:13:54.000000 generate-json-schema-0.1.5/generate_json_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 fernnando   (501) staff       (20)       22 2023-07-27 18:13:54.000000 generate-json-schema-0.1.5/generate_json_schema.egg-info/top_level.txt
+-rw-r--r--   0 fernnando   (501) staff       (20)       38 2023-07-27 18:13:54.535946 generate-json-schema-0.1.5/setup.cfg
+-rw-r--r--   0 fernnando   (501) staff       (20)     2243 2023-07-27 18:13:20.000000 generate-json-schema-0.1.5/setup.py
+drwxr-xr-x   0 fernnando   (501) staff       (20)        0 2023-07-27 18:13:54.534136 generate-json-schema-0.1.5/src/
+-rw-r--r--   0 fernnando   (501) staff       (20)        0 2023-07-25 18:41:19.000000 generate-json-schema-0.1.5/src/__init__.py
+-rw-r--r--   0 fernnando   (501) staff       (20)     2056 2023-07-26 13:48:52.000000 generate-json-schema-0.1.5/src/generate_schema.py
```

### Comparing `generate-json-schema-0.1.3/PKG-INFO` & `generate-json-schema-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-json-schema
-Version: 0.1.3
+Version: 0.1.5
 Summary: Json Schema Generator
 Home-page: https://github.com/fernandotoledomoreira/json-schema-generator
 Author: Fernando Toledo Moreira
 Author-email: fernandotoledomoreira@gmail.com
 Keywords: json schema generator development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `generate-json-schema-0.1.3/README.rst` & `generate-json-schema-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `generate-json-schema-0.1.3/generate_json_schema.egg-info/PKG-INFO` & `generate-json-schema-0.1.5/generate_json_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-json-schema
-Version: 0.1.3
+Version: 0.1.5
 Summary: Json Schema Generator
 Home-page: https://github.com/fernandotoledomoreira/json-schema-generator
 Author: Fernando Toledo Moreira
 Author-email: fernandotoledomoreira@gmail.com
 Keywords: json schema generator development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `generate-json-schema-0.1.3/setup.py` & `generate-json-schema-0.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 # setup.py - Packaging configuration for jsonschemagenerator
 #
 # Copyright (C) 2023 Your Name <fernandotoledomoreira@gmail.com>
 
 import os
 from setuptools import setup
+import requests
 
 # Library Information
 NAME = 'generate-json-schema'
-VERSION = '0.1.3'
 AUTHOR = 'Fernando Toledo Moreira'
 AUTHOR_EMAIL = 'fernandotoledomoreira@gmail.com'
 URL = 'https://github.com/fernandotoledomoreira/json-schema-generator'
 
 # Minimum Python version required for the library
 PYTHON_REQUIRES = '>=3.6'
 
+# Get Tag from GitHub
+def get_latest_version():
+    try:
+        url = 'https://api.github.com/repos/fernandotoledomoreira/json-schema-generator/releases/latest'
+        response = requests.get(url)
+        response.raise_for_status()  # Verifica se a resposta foi bem-sucedida
+        data = response.json()
+        return data['tag_name']
+    except Exception as e:
+        print(f"Erro ao obter a versão do GitHub: {e}")
+        return VERSION
+
+VERSION = get_latest_version()
+
 # Read the README.rst file to use as long description
 try:
     f = open("README.rst")
     readme = f.read()
     f.close()
 except Exception:
     print("failed to read readme: ignoring...")
@@ -44,8 +58,8 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     keywords='json schema generator development',   # Keywords related to the library
     python_requires=PYTHON_REQUIRES,   # Minimum required Python version
-)
+)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `generate-json-schema-0.1.3/src/generate_schema.py` & `generate-json-schema-0.1.5/src/generate_schema.py`

 * *Files identical despite different names*

