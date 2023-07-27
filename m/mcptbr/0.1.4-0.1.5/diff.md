# Comparing `tmp/mcptbr-0.1.4.tar.gz` & `tmp/mcptbr-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.1.4.tar", last modified: Thu Jul 27 20:18:25 2023, max compression
+gzip compressed data, was "mcptbr-0.1.5.tar", last modified: Thu Jul 27 20:36:44 2023, max compression
```

## Comparing `mcptbr-0.1.4.tar` & `mcptbr-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 20:18:25.130752 mcptbr-0.1.4/
--rw-rw-rw-   0        0        0      176 2023-07-27 20:18:25.129753 mcptbr-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 20:18:25.114794 mcptbr-0.1.4/mcptbr/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.4/mcptbr/__init__.py
--rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.1.4/mcptbr/model.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:18:25.126762 mcptbr-0.1.4/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      176 2023-07-27 20:18:24.000000 mcptbr-0.1.4/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-27 20:18:24.000000 mcptbr-0.1.4/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 20:18:24.000000 mcptbr-0.1.4/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-27 20:18:24.000000 mcptbr-0.1.4/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 20:18:24.000000 mcptbr-0.1.4/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 20:18:25.130752 mcptbr-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      491 2023-07-27 20:17:40.000000 mcptbr-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:36:44.116554 mcptbr-0.1.5/
+-rw-rw-rw-   0        0        0      193 2023-07-27 20:36:44.115556 mcptbr-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 20:36:44.093617 mcptbr-0.1.5/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.5/mcptbr/__init__.py
+-rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.1.5/mcptbr/model.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:36:44.112564 mcptbr-0.1.5/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-07-27 20:36:43.000000 mcptbr-0.1.5/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-27 20:36:43.000000 mcptbr-0.1.5/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 20:36:43.000000 mcptbr-0.1.5/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-27 20:36:43.000000 mcptbr-0.1.5/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 20:36:43.000000 mcptbr-0.1.5/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 20:36:44.116554 mcptbr-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      508 2023-07-27 20:36:28.000000 mcptbr-0.1.5/setup.py
```

### Comparing `mcptbr-0.1.4/mcptbr/model.py` & `mcptbr-0.1.5/mcptbr/model.py`

 * *Files identical despite different names*

