# Comparing `tmp/stakepy-1.0.0.tar.gz` & `tmp/stakepy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stakepy-1.0.0.tar", last modified: Thu Jul 27 01:33:23 2023, max compression
+gzip compressed data, was "stakepy-1.0.1.tar", last modified: Thu Jul 27 05:43:54 2023, max compression
```

## Comparing `stakepy-1.0.0.tar` & `stakepy-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 01:33:23.648178 stakepy-1.0.0/
--rw-rw-rw-   0        0        0      360 2023-07-27 01:33:23.648178 stakepy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-27 01:33:23.649178 stakepy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      624 2023-07-27 01:31:46.000000 stakepy-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:33:23.628576 stakepy-1.0.0/stakepy/
--rw-rw-rw-   0        0        0     1708 2023-07-26 16:02:36.000000 stakepy-1.0.0/stakepy/__init__.py
--rw-rw-rw-   0        0        0    24760 2023-07-26 16:02:48.000000 stakepy-1.0.0/stakepy/main.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:33:23.646181 stakepy-1.0.0/stakepy.egg-info/
--rw-rw-rw-   0        0        0      360 2023-07-27 01:33:23.000000 stakepy-1.0.0/stakepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-07-27 01:33:23.000000 stakepy-1.0.0/stakepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 01:33:23.000000 stakepy-1.0.0/stakepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-27 01:33:23.000000 stakepy-1.0.0/stakepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 01:33:23.000000 stakepy-1.0.0/stakepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 05:43:54.729137 stakepy-1.0.1/
+-rw-rw-rw-   0        0        0      360 2023-07-27 05:43:54.728137 stakepy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-27 05:43:54.729137 stakepy-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-07-27 05:43:43.000000 stakepy-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 05:43:54.719137 stakepy-1.0.1/stakepy/
+-rw-rw-rw-   0        0        0      488 2023-07-27 02:49:32.000000 stakepy-1.0.1/stakepy/__init__.py
+-rw-rw-rw-   0        0        0      220 2023-07-27 05:43:54.000000 stakepy-1.0.1/stakepy/main.py
+drwxrwxrwx   0        0        0        0 2023-07-27 05:43:54.727136 stakepy-1.0.1/stakepy.egg-info/
+-rw-rw-rw-   0        0        0      360 2023-07-27 05:43:54.000000 stakepy-1.0.1/stakepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-07-27 05:43:54.000000 stakepy-1.0.1/stakepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 05:43:54.000000 stakepy-1.0.1/stakepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-27 05:43:54.000000 stakepy-1.0.1/stakepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 05:43:54.000000 stakepy-1.0.1/stakepy.egg-info/top_level.txt
```

