# Comparing `tmp/mcptbr-0.1.7.tar.gz` & `tmp/mcptbr-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.1.7.tar", last modified: Thu Jul 27 20:46:05 2023, max compression
+gzip compressed data, was "mcptbr-0.1.8.tar", last modified: Thu Jul 27 20:50:41 2023, max compression
```

## Comparing `mcptbr-0.1.7.tar` & `mcptbr-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:05.378549 mcptbr-0.1.7/
--rw-rw-rw-   0        0        0      193 2023-07-27 20:46:05.377552 mcptbr-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:05.359598 mcptbr-0.1.7/mcptbr/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.7/mcptbr/__init__.py
--rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.1.7/mcptbr/model.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:46:05.375557 mcptbr-0.1.7/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      193 2023-07-27 20:46:05.000000 mcptbr-0.1.7/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-27 20:46:05.000000 mcptbr-0.1.7/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 20:46:05.000000 mcptbr-0.1.7/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-27 20:46:05.000000 mcptbr-0.1.7/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 20:46:05.000000 mcptbr-0.1.7/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 20:46:05.378549 mcptbr-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      535 2023-07-27 20:45:47.000000 mcptbr-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:50:40.995519 mcptbr-0.1.8/
+-rw-rw-rw-   0        0        0      718 2023-07-27 20:50:40.995519 mcptbr-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 20:50:40.979903 mcptbr-0.1.8/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.8/mcptbr/__init__.py
+-rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.1.8/mcptbr/model.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:50:40.995519 mcptbr-0.1.8/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      718 2023-07-27 20:50:40.000000 mcptbr-0.1.8/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-27 20:50:40.000000 mcptbr-0.1.8/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 20:50:40.000000 mcptbr-0.1.8/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-27 20:50:40.000000 mcptbr-0.1.8/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 20:50:40.000000 mcptbr-0.1.8/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 20:50:40.995519 mcptbr-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      608 2023-07-27 20:50:32.000000 mcptbr-0.1.8/setup.py
```

### Comparing `mcptbr-0.1.7/mcptbr/model.py` & `mcptbr-0.1.8/mcptbr/model.py`

 * *Files identical despite different names*

