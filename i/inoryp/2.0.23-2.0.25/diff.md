# Comparing `tmp/inoryp-2.0.23.tar.gz` & `tmp/inoryp-2.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inoryp-2.0.23.tar", last modified: Sun Sep 18 01:12:42 2022, max compression
+gzip compressed data, was "inoryp-2.0.25.tar", last modified: Thu Jul 27 18:38:15 2023, max compression
```

## Comparing `inoryp-2.0.23.tar` & `inoryp-2.0.25.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-09-18 01:12:42.346959 inoryp-2.0.23/
--rw-rw-rw-   0        0        0     3858 2022-09-18 01:12:42.347953 inoryp-2.0.23/PKG-INFO
--rw-rw-rw-   0        0        0     2501 2022-09-18 01:12:30.000000 inoryp-2.0.23/README.md
-drwxrwxrwx   0        0        0        0 2022-09-18 01:12:42.331000 inoryp-2.0.23/inoryp/
--rw-rw-rw-   0        0        0     8395 2022-09-18 01:06:30.000000 inoryp-2.0.23/inoryp/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-18 01:12:42.345958 inoryp-2.0.23/inoryp.egg-info/
--rw-rw-rw-   0        0        0     3858 2022-09-18 01:12:42.000000 inoryp-2.0.23/inoryp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2022-09-18 01:12:42.000000 inoryp-2.0.23/inoryp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-18 01:12:42.000000 inoryp-2.0.23/inoryp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2022-09-18 01:12:42.000000 inoryp-2.0.23/inoryp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-09-18 01:12:42.000000 inoryp-2.0.23/inoryp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-18 01:12:42.349948 inoryp-2.0.23/setup.cfg
--rw-rw-rw-   0        0        0      970 2022-09-18 01:12:33.000000 inoryp-2.0.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 18:38:15.010993 inoryp-2.0.25/
+-rw-rw-rw-   0        0        0     3858 2023-07-27 18:38:15.010993 inoryp-2.0.25/PKG-INFO
+-rw-rw-rw-   0        0        0     2501 2022-09-18 01:12:30.000000 inoryp-2.0.25/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 18:38:15.002018 inoryp-2.0.25/inoryp/
+-rw-rw-rw-   0        0        0     6037 2023-07-27 18:36:16.000000 inoryp-2.0.25/inoryp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 18:38:15.009995 inoryp-2.0.25/inoryp.egg-info/
+-rw-rw-rw-   0        0        0     3858 2023-07-27 18:38:14.000000 inoryp-2.0.25/inoryp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-07-27 18:38:14.000000 inoryp-2.0.25/inoryp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 18:38:14.000000 inoryp-2.0.25/inoryp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-27 18:38:14.000000 inoryp-2.0.25/inoryp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 18:38:14.000000 inoryp-2.0.25/inoryp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 18:38:15.012987 inoryp-2.0.25/setup.cfg
+-rw-rw-rw-   0        0        0      970 2023-07-27 18:34:20.000000 inoryp-2.0.25/setup.py
```

### Comparing `inoryp-2.0.23/PKG-INFO` & `inoryp-2.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inoryp
-Version: 2.0.23
+Version: 2.0.25
 Summary: Essa biblioteca foi desenvolvida com o intuito de fornecer o acesso rápido ao seu Endereço IP(LAN).
 Home-page: https://github.com/R0htg0r
 Author: R0htg0r
 Author-email: osvaldo.pedreiro.ecaminhoneiro@gmail.com
 License: MIT
 Description: ## Instalar & Importar
         * import inoryp
```

### Comparing `inoryp-2.0.23/README.md` & `inoryp-2.0.25/README.md`

 * *Files identical despite different names*

### Comparing `inoryp-2.0.23/inoryp.egg-info/PKG-INFO` & `inoryp-2.0.25/inoryp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inoryp
-Version: 2.0.23
+Version: 2.0.25
 Summary: Essa biblioteca foi desenvolvida com o intuito de fornecer o acesso rápido ao seu Endereço IP(LAN).
 Home-page: https://github.com/R0htg0r
 Author: R0htg0r
 Author-email: osvaldo.pedreiro.ecaminhoneiro@gmail.com
 License: MIT
 Description: ## Instalar & Importar
         * import inoryp
```

### Comparing `inoryp-2.0.23/setup.py` & `inoryp-2.0.25/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 30/04/2021
 
 import pathlib
 from setuptools import setup, find_packages
 
 setup(
     name="inoryp",
-    version="2.0.23",
+    version="2.0.25",
     author="R0htg0r",
     author_email="osvaldo.pedreiro.ecaminhoneiro@gmail.com",
     url="https://github.com/R0htg0r",
     description="Essa biblioteca foi desenvolvida com o intuito de fornecer o acesso rápido ao seu Endereço IP(LAN).",
     long_description=open("README.md", 'r').read(),
     long_description_content_type="text/markdown",
```

