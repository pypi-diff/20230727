# Comparing `tmp/diagrams-as-code-0.0.1.tar.gz` & `tmp/diagrams-as-code-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diagrams-as-code-0.0.1.tar", last modified: Tue Jul 25 15:45:07 2023, max compression
+gzip compressed data, was "diagrams-as-code-0.0.2.tar", last modified: Thu Jul 27 18:02:11 2023, max compression
```

## Comparing `diagrams-as-code-0.0.1.tar` & `diagrams-as-code-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:45:07.672834 diagrams-as-code-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 15:44:41.000000 diagrams-as-code-0.0.1/.project-version
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 15:44:41.000000 diagrams-as-code-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-25 15:44:41.000000 diagrams-as-code-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21589 2023-07-25 15:45:07.672834 diagrams-as-code-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20698 2023-07-25 15:44:41.000000 diagrams-as-code-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:45:07.672834 diagrams-as-code-0.0.1/diagrams_as_code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 15:44:41.000000 diagrams-as-code-0.0.1/diagrams_as_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-25 15:44:41.000000 diagrams-as-code-0.0.1/diagrams_as_code/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-25 15:44:41.000000 diagrams-as-code-0.0.1/diagrams_as_code/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-25 15:44:41.000000 diagrams-as-code-0.0.1/diagrams_as_code/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-25 15:44:41.000000 diagrams-as-code-0.0.1/diagrams_as_code/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:45:07.672834 diagrams-as-code-0.0.1/diagrams_as_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21589 2023-07-25 15:45:07.000000 diagrams-as-code-0.0.1/diagrams_as_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-25 15:45:07.000000 diagrams-as-code-0.0.1/diagrams_as_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:45:07.000000 diagrams-as-code-0.0.1/diagrams_as_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-25 15:45:07.000000 diagrams-as-code-0.0.1/diagrams_as_code.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 15:45:07.000000 diagrams-as-code-0.0.1/diagrams_as_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 15:45:07.000000 diagrams-as-code-0.0.1/diagrams_as_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-25 15:44:41.000000 diagrams-as-code-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:45:07.672834 diagrams-as-code-0.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 15:44:41.000000 diagrams-as-code-0.0.1/requirements/project.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 15:45:07.672834 diagrams-as-code-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-25 15:44:41.000000 diagrams-as-code-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:02:11.391606 diagrams-as-code-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/.project-version
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-07-27 18:02:11.391606 diagrams-as-code-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20791 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:02:11.387606 diagrams-as-code-0.0.2/diagrams_as_code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/diagrams_as_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/diagrams_as_code/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/diagrams_as_code/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/diagrams_as_code/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/diagrams_as_code/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:02:11.391606 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-07-27 18:02:11.000000 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-27 18:02:11.000000 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:02:11.000000 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 18:02:11.000000 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 18:02:11.000000 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 18:02:11.000000 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:02:11.391606 diagrams-as-code-0.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/requirements/project.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 18:02:11.391606 diagrams-as-code-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/setup.py
```

### Comparing `diagrams-as-code-0.0.1/LICENSE` & `diagrams-as-code-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `diagrams-as-code-0.0.1/PKG-INFO` & `diagrams-as-code-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagrams-as-code
-Version: 0.0.1
+Version: 0.0.2
 Summary: Diagrams as code: declarative configurations using YAML for drawing cloud system architectures.
 Home-page: https://github.com/dmytrostriletskyi/diagrams-as-code
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dmytrostriletskyi/diagrams-as-code/issues
 Project-URL: Source Code, https://github.com/dmytrostriletskyi/diagrams-as-code
@@ -19,14 +19,16 @@
 License-File: LICENSE
 
 `Diagrams as code`: declarative configurations using `YAML` for drawing cloud system architectures.
 
 [![](https://github.com/dmytrostriletskyi/diagrams-as-code/actions/workflows/main.yaml/badge.svg?branch=main)](https://github.com/dmytrostriletskyi/diagrams-as-code/actions/workflows/main.yaml)
 [![](https://img.shields.io/github/release/dmytrostriletskyi/diagrams-as-code.svg)](https://github.com/dmytrostriletskyi/diagrams-as-code/releases)
 [![](https://img.shields.io/pypi/v/diagrams-as-code.svg)](https://pypi.python.org/pypi/diagrams-as-code)
+
+[![](https://pepy.tech/badge/diagrams-as-code)](https://pepy.tech/project/diagrams-as-code)
 [![](https://img.shields.io/pypi/l/diagrams-as-code.svg)](https://pypi.python.org/pypi/diagrams-as-code/)
 [![](https://img.shields.io/pypi/pyversions/diagrams-as-code.svg)](https://pypi.python.org/pypi/diagrams-as-code/)
 
 ![](./assets/configurations-architecture-aligned.png)
 
 Table of content:
```

### Comparing `diagrams-as-code-0.0.1/README.md` & `diagrams-as-code-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 `Diagrams as code`: declarative configurations using `YAML` for drawing cloud system architectures.
 
 [![](https://github.com/dmytrostriletskyi/diagrams-as-code/actions/workflows/main.yaml/badge.svg?branch=main)](https://github.com/dmytrostriletskyi/diagrams-as-code/actions/workflows/main.yaml)
 [![](https://img.shields.io/github/release/dmytrostriletskyi/diagrams-as-code.svg)](https://github.com/dmytrostriletskyi/diagrams-as-code/releases)
 [![](https://img.shields.io/pypi/v/diagrams-as-code.svg)](https://pypi.python.org/pypi/diagrams-as-code)
+
+[![](https://pepy.tech/badge/diagrams-as-code)](https://pepy.tech/project/diagrams-as-code)
 [![](https://img.shields.io/pypi/l/diagrams-as-code.svg)](https://pypi.python.org/pypi/diagrams-as-code/)
 [![](https://img.shields.io/pypi/pyversions/diagrams-as-code.svg)](https://pypi.python.org/pypi/diagrams-as-code/)
 
 ![](./assets/configurations-architecture-aligned.png)
 
 Table of content:
```

### Comparing `diagrams-as-code-0.0.1/diagrams_as_code/entrypoint.py` & `diagrams-as-code-0.0.2/diagrams_as_code/entrypoint.py`

 * *Files identical despite different names*

### Comparing `diagrams-as-code-0.0.1/diagrams_as_code/enums.py` & `diagrams-as-code-0.0.2/diagrams_as_code/enums.py`

 * *Files identical despite different names*

### Comparing `diagrams-as-code-0.0.1/diagrams_as_code/resources.py` & `diagrams-as-code-0.0.2/diagrams_as_code/resources.py`

 * *Files identical despite different names*

### Comparing `diagrams-as-code-0.0.1/diagrams_as_code/schema.py` & `diagrams-as-code-0.0.2/diagrams_as_code/schema.py`

 * *Files identical despite different names*

### Comparing `diagrams-as-code-0.0.1/diagrams_as_code.egg-info/PKG-INFO` & `diagrams-as-code-0.0.2/diagrams_as_code.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagrams-as-code
-Version: 0.0.1
+Version: 0.0.2
 Summary: Diagrams as code: declarative configurations using YAML for drawing cloud system architectures.
 Home-page: https://github.com/dmytrostriletskyi/diagrams-as-code
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dmytrostriletskyi/diagrams-as-code/issues
 Project-URL: Source Code, https://github.com/dmytrostriletskyi/diagrams-as-code
@@ -19,14 +19,16 @@
 License-File: LICENSE
 
 `Diagrams as code`: declarative configurations using `YAML` for drawing cloud system architectures.
 
 [![](https://github.com/dmytrostriletskyi/diagrams-as-code/actions/workflows/main.yaml/badge.svg?branch=main)](https://github.com/dmytrostriletskyi/diagrams-as-code/actions/workflows/main.yaml)
 [![](https://img.shields.io/github/release/dmytrostriletskyi/diagrams-as-code.svg)](https://github.com/dmytrostriletskyi/diagrams-as-code/releases)
 [![](https://img.shields.io/pypi/v/diagrams-as-code.svg)](https://pypi.python.org/pypi/diagrams-as-code)
+
+[![](https://pepy.tech/badge/diagrams-as-code)](https://pepy.tech/project/diagrams-as-code)
 [![](https://img.shields.io/pypi/l/diagrams-as-code.svg)](https://pypi.python.org/pypi/diagrams-as-code/)
 [![](https://img.shields.io/pypi/pyversions/diagrams-as-code.svg)](https://pypi.python.org/pypi/diagrams-as-code/)
 
 ![](./assets/configurations-architecture-aligned.png)
 
 Table of content:
```

### Comparing `diagrams-as-code-0.0.1/setup.py` & `diagrams-as-code-0.0.2/setup.py`

 * *Files identical despite different names*

