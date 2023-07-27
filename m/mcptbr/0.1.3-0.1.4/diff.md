# Comparing `tmp/mcptbr-0.1.3.tar.gz` & `tmp/mcptbr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.1.3.tar", last modified: Wed Jul 26 01:51:59 2023, max compression
+gzip compressed data, was "mcptbr-0.1.4.tar", last modified: Thu Jul 27 20:18:25 2023, max compression
```

## Comparing `mcptbr-0.1.3.tar` & `mcptbr-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 01:51:59.245902 mcptbr-0.1.3/
--rw-rw-rw-   0        0        0      176 2023-07-26 01:51:59.243905 mcptbr-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 01:51:59.163121 mcptbr-0.1.3/mcptbr/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.3/mcptbr/__init__.py
--rw-rw-rw-   0        0        0      744 2023-07-26 01:48:09.000000 mcptbr-0.1.3/mcptbr/model.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:51:59.239914 mcptbr-0.1.3/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      176 2023-07-26 01:51:58.000000 mcptbr-0.1.3/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-26 01:51:58.000000 mcptbr-0.1.3/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 01:51:58.000000 mcptbr-0.1.3/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-26 01:51:58.000000 mcptbr-0.1.3/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 01:51:58.000000 mcptbr-0.1.3/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 01:51:59.245902 mcptbr-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      491 2023-07-26 01:48:54.000000 mcptbr-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:18:25.130752 mcptbr-0.1.4/
+-rw-rw-rw-   0        0        0      176 2023-07-27 20:18:25.129753 mcptbr-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 20:18:25.114794 mcptbr-0.1.4/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.4/mcptbr/__init__.py
+-rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.1.4/mcptbr/model.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:18:25.126762 mcptbr-0.1.4/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-07-27 20:18:24.000000 mcptbr-0.1.4/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-27 20:18:24.000000 mcptbr-0.1.4/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 20:18:24.000000 mcptbr-0.1.4/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-27 20:18:24.000000 mcptbr-0.1.4/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 20:18:24.000000 mcptbr-0.1.4/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 20:18:25.130752 mcptbr-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      491 2023-07-27 20:17:40.000000 mcptbr-0.1.4/setup.py
```

