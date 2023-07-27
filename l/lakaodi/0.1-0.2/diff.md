# Comparing `tmp/lakaodi-0.1.tar.gz` & `tmp/lakaodi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakaodi-0.1.tar", last modified: Thu Jul 27 11:05:38 2023, max compression
+gzip compressed data, was "lakaodi-0.2.tar", last modified: Thu Jul 27 11:13:57 2023, max compression
```

## Comparing `lakaodi-0.1.tar` & `lakaodi-0.2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:05:38.191344 lakaodi-0.1/
--rw-rw-rw-   0        0        0      338 2023-07-27 11:05:38.191344 lakaodi-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 11:05:38.189895 lakaodi-0.1/lakaodi.egg-info/
--rw-rw-rw-   0        0        0      338 2023-07-27 11:05:38.000000 lakaodi-0.1/lakaodi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-07-27 11:05:38.000000 lakaodi-0.1/lakaodi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 11:05:38.000000 lakaodi-0.1/lakaodi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-27 11:05:38.000000 lakaodi-0.1/lakaodi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 11:05:38.000000 lakaodi-0.1/lakaodi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 11:05:38.191344 lakaodi-0.1/setup.cfg
--rw-rw-rw-   0        0        0      848 2023-07-27 11:00:24.000000 lakaodi-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:13:57.246567 lakaodi-0.2/
+-rw-rw-rw-   0        0        0      338 2023-07-27 11:13:57.246567 lakaodi-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 11:13:57.237050 lakaodi-0.2/lakaodi/
+-rw-rw-rw-   0        0        0        0 2023-07-27 11:10:41.000000 lakaodi-0.2/lakaodi/__init__.py
+-rw-rw-rw-   0        0        0      652 2023-07-27 11:11:49.000000 lakaodi-0.2/lakaodi/send_notification_telegram.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:13:57.245566 lakaodi-0.2/lakaodi.egg-info/
+-rw-rw-rw-   0        0        0      338 2023-07-27 11:13:57.000000 lakaodi-0.2/lakaodi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-07-27 11:13:57.000000 lakaodi-0.2/lakaodi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:13:57.000000 lakaodi-0.2/lakaodi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-27 11:13:57.000000 lakaodi-0.2/lakaodi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-27 11:13:57.000000 lakaodi-0.2/lakaodi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 11:13:57.000000 lakaodi-0.2/lakaodi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:13:57.247071 lakaodi-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      506 2023-07-27 11:13:41.000000 lakaodi-0.2/setup.py
```

