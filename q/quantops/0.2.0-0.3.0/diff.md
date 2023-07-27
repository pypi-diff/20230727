# Comparing `tmp/quantops-0.2.0.tar.gz` & `tmp/quantops-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantops-0.2.0.tar", last modified: Tue Jun 27 16:38:59 2023, max compression
+gzip compressed data, was "quantops-0.3.0.tar", last modified: Thu Jul 27 15:56:56 2023, max compression
```

## Comparing `quantops-0.2.0.tar` & `quantops-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-27 16:38:59.337011 quantops-0.2.0/
--rw-r--r--   0 simon      (501) staff       (20)      263 2023-06-27 16:38:59.336883 quantops-0.2.0/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      514 2023-06-27 16:38:11.000000 quantops-0.2.0/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-27 16:38:59.335916 quantops-0.2.0/quantops/
--rw-r--r--   0 simon      (501) staff       (20)       42 2023-06-02 14:53:07.000000 quantops-0.2.0/quantops/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2025 2023-06-22 10:37:01.000000 quantops-0.2.0/quantops/__main__.py
--rw-r--r--   0 simon      (501) staff       (20)    22009 2023-06-22 15:15:32.000000 quantops-0.2.0/quantops/core.py
--rw-r--r--   0 simon      (501) staff       (20)      154 2023-06-22 10:49:07.000000 quantops-0.2.0/quantops/generate.py
--rw-r--r--   0 simon      (501) staff       (20)     9729 2023-06-22 10:27:38.000000 quantops-0.2.0/quantops/parser.py
--rw-r--r--   0 simon      (501) staff       (20)     8211 2023-06-22 15:17:43.000000 quantops-0.2.0/quantops/registry.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-27 16:38:59.336699 quantops-0.2.0/quantops.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)      263 2023-06-27 16:38:59.000000 quantops-0.2.0/quantops.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      295 2023-06-27 16:38:59.000000 quantops-0.2.0/quantops.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-06-27 16:38:59.000000 quantops-0.2.0/quantops.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)       16 2023-06-27 16:38:59.000000 quantops-0.2.0/quantops.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        9 2023-06-27 16:38:59.000000 quantops-0.2.0/quantops.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-27 16:38:59.337044 quantops-0.2.0/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-27 15:56:56.426534 quantops-0.3.0/
+-rw-r--r--   0 simon      (501) staff       (20)      263 2023-07-27 15:56:56.426412 quantops-0.3.0/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      514 2023-07-27 15:56:00.000000 quantops-0.3.0/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-27 15:56:56.425360 quantops-0.3.0/quantops/
+-rw-r--r--   0 simon      (501) staff       (20)       42 2023-06-02 14:53:07.000000 quantops-0.3.0/quantops/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    22009 2023-06-22 15:15:32.000000 quantops-0.3.0/quantops/core.py
+-rw-r--r--   0 simon      (501) staff       (20)      154 2023-06-22 10:49:07.000000 quantops-0.3.0/quantops/generate.py
+-rw-r--r--   0 simon      (501) staff       (20)     9729 2023-06-22 10:27:38.000000 quantops-0.3.0/quantops/parser.py
+-rw-r--r--   0 simon      (501) staff       (20)     8211 2023-06-22 15:17:43.000000 quantops-0.3.0/quantops/registry.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-27 15:56:56.426221 quantops-0.3.0/quantops.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)      263 2023-07-27 15:56:56.000000 quantops-0.3.0/quantops.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      274 2023-07-27 15:56:56.000000 quantops-0.3.0/quantops.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-07-27 15:56:56.000000 quantops-0.3.0/quantops.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       16 2023-07-27 15:56:56.000000 quantops-0.3.0/quantops.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        9 2023-07-27 15:56:56.000000 quantops-0.3.0/quantops.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-27 15:56:56.426571 quantops-0.3.0/setup.cfg
```

### Comparing `quantops-0.2.0/pyproject.toml` & `quantops-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quantops"
-version = "0.2.0"
+version = "0.3.0"
 
 description = "Tools to define, manipulate and format physical quantities"
 readme = "readme.md"
 license = { text = "EUPL-1.2" }
 requires-python = ">=3.11"
 
 dependencies = [
```

### Comparing `quantops-0.2.0/quantops/core.py` & `quantops-0.3.0/quantops/core.py`

 * *Files identical despite different names*

### Comparing `quantops-0.2.0/quantops/parser.py` & `quantops-0.3.0/quantops/parser.py`

 * *Files identical despite different names*

### Comparing `quantops-0.2.0/quantops/registry.toml` & `quantops-0.3.0/quantops/registry.toml`

 * *Files identical despite different names*

