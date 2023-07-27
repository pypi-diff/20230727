# Comparing `tmp/pycampus-0.1.2.tar.gz` & `tmp/pycampus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycampus-0.1.2.tar", last modified: Thu Jul 27 04:41:36 2023, max compression
+gzip compressed data, was "pycampus-0.1.3.tar", last modified: Thu Jul 27 04:46:13 2023, max compression
```

## Comparing `pycampus-0.1.2.tar` & `pycampus-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 04:41:36.551813 pycampus-0.1.2/
--rw-rw-rw-   0        0        0     1087 2023-07-27 02:36:04.000000 pycampus-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       78 2023-07-27 04:41:36.551813 pycampus-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-07-27 02:37:18.000000 pycampus-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 04:41:36.539262 pycampus-0.1.2/pycampus/
--rw-rw-rw-   0        0        0       27 2023-07-27 04:37:47.000000 pycampus-0.1.2/pycampus/__init__.py
--rw-rw-rw-   0        0        0       76 2023-07-27 04:40:02.000000 pycampus-0.1.2/pycampus/campus.py
-drwxrwxrwx   0        0        0        0 2023-07-27 04:41:36.551813 pycampus-0.1.2/pycampus.egg-info/
--rw-rw-rw-   0        0        0       78 2023-07-27 04:41:36.000000 pycampus-0.1.2/pycampus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-27 04:41:36.000000 pycampus-0.1.2/pycampus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 04:41:36.000000 pycampus-0.1.2/pycampus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-27 04:41:36.000000 pycampus-0.1.2/pycampus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-27 04:41:36.000000 pycampus-0.1.2/pycampus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-27 04:41:36.000000 pycampus-0.1.2/pycampus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 04:41:36.551813 pycampus-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      328 2023-07-27 04:41:25.000000 pycampus-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 04:46:13.574298 pycampus-0.1.3/
+-rw-rw-rw-   0        0        0     1087 2023-07-27 02:36:04.000000 pycampus-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       78 2023-07-27 04:46:13.574298 pycampus-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-07-27 02:37:18.000000 pycampus-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 04:46:13.558685 pycampus-0.1.3/pycampus/
+-rw-rw-rw-   0        0        0       36 2023-07-27 04:45:52.000000 pycampus-0.1.3/pycampus/__init__.py
+-rw-rw-rw-   0        0        0       76 2023-07-27 04:40:02.000000 pycampus-0.1.3/pycampus/campus.py
+drwxrwxrwx   0        0        0        0 2023-07-27 04:46:13.574298 pycampus-0.1.3/pycampus.egg-info/
+-rw-rw-rw-   0        0        0       78 2023-07-27 04:46:13.000000 pycampus-0.1.3/pycampus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-27 04:46:13.000000 pycampus-0.1.3/pycampus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 04:46:13.000000 pycampus-0.1.3/pycampus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-27 04:46:13.000000 pycampus-0.1.3/pycampus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-27 04:46:13.000000 pycampus-0.1.3/pycampus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 04:46:13.000000 pycampus-0.1.3/pycampus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 04:46:13.574298 pycampus-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      328 2023-07-27 04:45:46.000000 pycampus-0.1.3/setup.py
```

### Comparing `pycampus-0.1.2/LICENSE` & `pycampus-0.1.3/LICENSE`

 * *Files identical despite different names*

