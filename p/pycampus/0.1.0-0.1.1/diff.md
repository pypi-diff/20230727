# Comparing `tmp/pycampus-0.1.0.tar.gz` & `tmp/pycampus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycampus-0.1.0.tar", last modified: Thu Jul 27 03:04:05 2023, max compression
+gzip compressed data, was "pycampus-0.1.1.tar", last modified: Thu Jul 27 03:21:32 2023, max compression
```

## Comparing `pycampus-0.1.0.tar` & `pycampus-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 03:04:04.988871 pycampus-0.1.0/
--rw-rw-rw-   0        0        0     1087 2023-07-27 02:36:04.000000 pycampus-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       78 2023-07-27 03:04:04.988871 pycampus-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-07-27 02:37:18.000000 pycampus-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 03:04:04.957624 pycampus-0.1.0/pycampus/
--rw-rw-rw-   0        0        0       30 2023-07-27 02:51:49.000000 pycampus-0.1.0/pycampus/__init__.py
--rw-rw-rw-   0        0        0       47 2023-07-27 02:51:29.000000 pycampus-0.1.0/pycampus/campus.py
-drwxrwxrwx   0        0        0        0 2023-07-27 03:04:04.988871 pycampus-0.1.0/pycampus.egg-info/
--rw-rw-rw-   0        0        0       78 2023-07-27 03:04:04.000000 pycampus-0.1.0/pycampus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-07-27 03:04:04.000000 pycampus-0.1.0/pycampus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 03:04:04.000000 pycampus-0.1.0/pycampus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-27 03:04:04.000000 pycampus-0.1.0/pycampus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 03:04:04.988871 pycampus-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      130 2023-07-27 02:55:54.000000 pycampus-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:21:32.032402 pycampus-0.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-07-27 02:36:04.000000 pycampus-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       78 2023-07-27 03:21:32.016785 pycampus-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-07-27 02:37:18.000000 pycampus-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 03:21:32.001150 pycampus-0.1.1/pycampus/
+-rw-rw-rw-   0        0        0       39 2023-07-27 03:19:04.000000 pycampus-0.1.1/pycampus/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-07-27 03:14:56.000000 pycampus-0.1.1/pycampus/campus.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:21:32.016785 pycampus-0.1.1/pycampus.egg-info/
+-rw-rw-rw-   0        0        0       78 2023-07-27 03:21:31.000000 pycampus-0.1.1/pycampus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-07-27 03:21:31.000000 pycampus-0.1.1/pycampus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 03:21:31.000000 pycampus-0.1.1/pycampus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 03:21:31.000000 pycampus-0.1.1/pycampus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 03:21:32.032402 pycampus-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      130 2023-07-27 03:21:27.000000 pycampus-0.1.1/setup.py
```

### Comparing `pycampus-0.1.0/LICENSE` & `pycampus-0.1.1/LICENSE`

 * *Files identical despite different names*

