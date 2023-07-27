# Comparing `tmp/mcptbr-0.1.5.tar.gz` & `tmp/mcptbr-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.1.5.tar", last modified: Thu Jul 27 20:36:44 2023, max compression
+gzip compressed data, was "mcptbr-0.1.6.tar", last modified: Thu Jul 27 20:39:19 2023, max compression
```

## Comparing `mcptbr-0.1.5.tar` & `mcptbr-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 20:36:44.116554 mcptbr-0.1.5/
--rw-rw-rw-   0        0        0      193 2023-07-27 20:36:44.115556 mcptbr-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 20:36:44.093617 mcptbr-0.1.5/mcptbr/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.5/mcptbr/__init__.py
--rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.1.5/mcptbr/model.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:36:44.112564 mcptbr-0.1.5/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      193 2023-07-27 20:36:43.000000 mcptbr-0.1.5/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-27 20:36:43.000000 mcptbr-0.1.5/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 20:36:43.000000 mcptbr-0.1.5/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-27 20:36:43.000000 mcptbr-0.1.5/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 20:36:43.000000 mcptbr-0.1.5/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 20:36:44.116554 mcptbr-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      508 2023-07-27 20:36:28.000000 mcptbr-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:39:19.762294 mcptbr-0.1.6/
+-rw-rw-rw-   0        0        0      193 2023-07-27 20:39:19.759302 mcptbr-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 20:39:19.738358 mcptbr-0.1.6/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.6/mcptbr/__init__.py
+-rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.1.6/mcptbr/model.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:39:19.757307 mcptbr-0.1.6/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-07-27 20:39:19.000000 mcptbr-0.1.6/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-27 20:39:19.000000 mcptbr-0.1.6/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 20:39:19.000000 mcptbr-0.1.6/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-27 20:39:19.000000 mcptbr-0.1.6/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 20:39:19.000000 mcptbr-0.1.6/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 20:39:19.762294 mcptbr-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      535 2023-07-27 20:39:13.000000 mcptbr-0.1.6/setup.py
```

### Comparing `mcptbr-0.1.5/mcptbr/model.py` & `mcptbr-0.1.6/mcptbr/model.py`

 * *Files identical despite different names*

