# Comparing `tmp/chichicha-2.2.0.2.tar.gz` & `tmp/chichicha-2.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\chichicha-2.2.0.2.tar", last modified: Thu Jul 27 08:49:58 2023, max compression
+gzip compressed data, was "dist\chichicha-2.3.0.2.tar", last modified: Thu Jul 27 08:59:18 2023, max compression
```

## Comparing `chichicha-2.2.0.2.tar` & `chichicha-2.3.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 08:49:58.070811 chichicha-2.2.0.2/
--rw-rw-rw-   0        0        0     1074 2022-08-31 06:39:42.000000 chichicha-2.2.0.2/LICENSE
--rw-rw-rw-   0        0        0       33 2022-08-31 08:45:36.000000 chichicha-2.2.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      290 2023-07-27 08:49:58.062811 chichicha-2.2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1557 2022-10-14 02:43:05.000000 chichicha-2.2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 08:49:57.970810 chichicha-2.2.0.2/chichicha/
--rw-rw-rw-   0        0        0        0 2022-10-06 06:11:11.000000 chichicha-2.2.0.2/chichicha/__init__.py
--rw-rw-rw-   0        0        0  8180224 2023-07-27 04:39:02.000000 chichicha-2.2.0.2/chichicha/pywpc.pyd
--rw-rw-rw-   0        0        0       17 2023-07-27 08:49:39.000000 chichicha-2.2.0.2/chichicha/version.py
-drwxrwxrwx   0        0        0        0 2023-07-27 08:49:58.056824 chichicha-2.2.0.2/chichicha.egg-info/
--rw-rw-rw-   0        0        0      290 2023-07-27 08:49:56.000000 chichicha-2.2.0.2/chichicha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-27 08:49:57.000000 chichicha-2.2.0.2/chichicha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 08:49:56.000000 chichicha-2.2.0.2/chichicha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      145 2023-07-27 08:49:57.000000 chichicha-2.2.0.2/chichicha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 08:49:57.000000 chichicha-2.2.0.2/chichicha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 08:49:58.071811 chichicha-2.2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1324 2023-07-27 08:49:05.000000 chichicha-2.2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:59:18.464924 chichicha-2.3.0.2/
+-rw-rw-rw-   0        0        0     1074 2022-08-31 06:39:42.000000 chichicha-2.3.0.2/LICENSE
+-rw-rw-rw-   0        0        0       33 2022-08-31 08:45:36.000000 chichicha-2.3.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      290 2023-07-27 08:59:18.456920 chichicha-2.3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1557 2022-10-14 02:43:05.000000 chichicha-2.3.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 08:59:18.381919 chichicha-2.3.0.2/chichicha/
+-rw-rw-rw-   0        0        0        0 2022-10-06 06:11:11.000000 chichicha-2.3.0.2/chichicha/__init__.py
+-rw-rw-rw-   0        0        0  8180224 2023-07-27 04:39:02.000000 chichicha-2.3.0.2/chichicha/pywpc.pyd
+-rw-rw-rw-   0        0        0       17 2023-07-27 08:59:06.000000 chichicha-2.3.0.2/chichicha/version.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:59:18.450930 chichicha-2.3.0.2/chichicha.egg-info/
+-rw-rw-rw-   0        0        0      290 2023-07-27 08:59:17.000000 chichicha-2.3.0.2/chichicha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-07-27 08:59:18.000000 chichicha-2.3.0.2/chichicha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 08:59:17.000000 chichicha-2.3.0.2/chichicha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      145 2023-07-27 08:59:17.000000 chichicha-2.3.0.2/chichicha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 08:59:17.000000 chichicha-2.3.0.2/chichicha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 08:59:18.465943 chichicha-2.3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1324 2023-07-27 08:49:05.000000 chichicha-2.3.0.2/setup.py
```

### Comparing `chichicha-2.2.0.2/LICENSE` & `chichicha-2.3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chichicha-2.2.0.2/README.md` & `chichicha-2.3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `chichicha-2.2.0.2/setup.py` & `chichicha-2.3.0.2/setup.py`

 * *Files identical despite different names*

