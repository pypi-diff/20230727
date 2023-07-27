# Comparing `tmp/tompdf_1-1.4.tar.gz` & `tmp/tompdf_1-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tompdf_1-1.4.tar", last modified: Wed Jul 26 21:48:10 2023, max compression
+gzip compressed data, was "tompdf_1-1.5.tar", last modified: Thu Jul 27 17:12:40 2023, max compression
```

## Comparing `tompdf_1-1.4.tar` & `tompdf_1-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 21:48:10.799168 tompdf_1-1.4/
--rw-rw-rw-   0        0        0    35821 2023-07-26 21:19:18.000000 tompdf_1-1.4/LICENSE
--rw-rw-rw-   0        0        0      116 2023-07-26 21:48:10.798167 tompdf_1-1.4/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-07-26 21:19:15.000000 tompdf_1-1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-26 21:48:10.800162 tompdf_1-1.4/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-07-26 21:47:56.000000 tompdf_1-1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 21:48:10.777225 tompdf_1-1.4/tompdf_1/
--rw-rw-rw-   0        0        0        0 2023-07-26 21:10:50.000000 tompdf_1-1.4/tompdf_1/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-26 21:19:29.000000 tompdf_1-1.4/tompdf_1/pdf2image.py
--rw-rw-rw-   0        0        0       39 2023-07-26 21:19:36.000000 tompdf_1-1.4/tompdf_1/pdf2text.py
-drwxrwxrwx   0        0        0        0 2023-07-26 21:48:10.795176 tompdf_1-1.4/tompdf_1.egg-info/
--rw-rw-rw-   0        0        0      116 2023-07-26 21:48:10.000000 tompdf_1-1.4/tompdf_1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-26 21:48:10.000000 tompdf_1-1.4/tompdf_1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 21:48:10.000000 tompdf_1-1.4/tompdf_1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 21:48:10.000000 tompdf_1-1.4/tompdf_1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 17:12:40.814110 tompdf_1-1.5/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 21:19:18.000000 tompdf_1-1.5/LICENSE
+-rw-rw-rw-   0        0        0      120 2023-07-27 17:12:40.796157 tompdf_1-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2023-07-27 17:09:43.000000 tompdf_1-1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 17:12:40.814110 tompdf_1-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      228 2023-07-27 17:10:53.000000 tompdf_1-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:12:40.758257 tompdf_1-1.5/tompdf_1/
+-rw-rw-rw-   0        0        0        0 2023-07-26 21:10:50.000000 tompdf_1-1.5/tompdf_1/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-26 21:19:29.000000 tompdf_1-1.5/tompdf_1/pdf2image.py
+-rw-rw-rw-   0        0        0       39 2023-07-26 21:19:36.000000 tompdf_1-1.5/tompdf_1/pdf2text.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:12:40.793162 tompdf_1-1.5/tompdf_1.egg-info/
+-rw-rw-rw-   0        0        0      120 2023-07-27 17:12:40.000000 tompdf_1-1.5/tompdf_1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-27 17:12:40.000000 tompdf_1-1.5/tompdf_1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 17:12:40.000000 tompdf_1-1.5/tompdf_1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 17:12:40.000000 tompdf_1-1.5/tompdf_1.egg-info/top_level.txt
```

### Comparing `tompdf_1-1.4/LICENSE` & `tompdf_1-1.5/LICENSE`

 * *Files identical despite different names*

