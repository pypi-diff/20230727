# Comparing `tmp/scraper_util_avliu-0.0.2.tar.gz` & `tmp/scraper_util_avliu-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scraper_util_avliu-0.0.2.tar", last modified: Thu Jul 27 15:46:15 2023, max compression
+gzip compressed data, was "scraper_util_avliu-0.1.0.tar", last modified: Thu Jul 27 16:03:39 2023, max compression
```

## Comparing `scraper_util_avliu-0.0.2.tar` & `scraper_util_avliu-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 15:46:15.441604 scraper_util_avliu-0.0.2/
--rw-r--r--   0 avliu      (504) staff       (20)        5 2023-06-20 08:37:43.000000 scraper_util_avliu-0.0.2/LICENSE
--rw-r--r--   0 avliu      (504) staff       (20)       84 2023-07-27 15:46:15.439623 scraper_util_avliu-0.0.2/PKG-INFO
--rw-r--r--   0 avliu      (504) staff       (20)       13 2023-06-20 08:37:43.000000 scraper_util_avliu-0.0.2/README.md
--rw-r--r--   0 avliu      (504) staff       (20)      189 2023-07-27 15:46:00.000000 scraper_util_avliu-0.0.2/pyproject.toml
--rw-r--r--   0 avliu      (504) staff       (20)       38 2023-07-27 15:46:15.441676 scraper_util_avliu-0.0.2/setup.cfg
-drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 15:46:15.436922 scraper_util_avliu-0.0.2/src/
-drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 15:46:15.438372 scraper_util_avliu-0.0.2/src/scraper_util_avliu/
--rw-r--r--   0 avliu      (504) staff       (20)        1 2023-06-20 08:37:43.000000 scraper_util_avliu-0.0.2/src/scraper_util_avliu/__init__.py
--rw-r--r--   0 avliu      (504) staff       (20)     1717 2023-07-27 15:39:29.000000 scraper_util_avliu-0.0.2/src/scraper_util_avliu/example.py
-drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 15:46:15.439396 scraper_util_avliu-0.0.2/src/scraper_util_avliu.egg-info/
--rw-r--r--   0 avliu      (504) staff       (20)       84 2023-07-27 15:46:15.000000 scraper_util_avliu-0.0.2/src/scraper_util_avliu.egg-info/PKG-INFO
--rw-r--r--   0 avliu      (504) staff       (20)      330 2023-07-27 15:46:15.000000 scraper_util_avliu-0.0.2/src/scraper_util_avliu.egg-info/SOURCES.txt
--rw-r--r--   0 avliu      (504) staff       (20)        1 2023-07-27 15:46:15.000000 scraper_util_avliu-0.0.2/src/scraper_util_avliu.egg-info/dependency_links.txt
--rw-r--r--   0 avliu      (504) staff       (20)       23 2023-07-27 15:46:15.000000 scraper_util_avliu-0.0.2/src/scraper_util_avliu.egg-info/requires.txt
--rw-r--r--   0 avliu      (504) staff       (20)       19 2023-07-27 15:46:15.000000 scraper_util_avliu-0.0.2/src/scraper_util_avliu.egg-info/top_level.txt
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:03:39.244171 scraper_util_avliu-0.1.0/
+-rw-r--r--   0 avliu      (504) staff       (20)        5 2023-06-20 08:37:43.000000 scraper_util_avliu-0.1.0/LICENSE
+-rw-r--r--   0 avliu      (504) staff       (20)       84 2023-07-27 16:03:39.243984 scraper_util_avliu-0.1.0/PKG-INFO
+-rw-r--r--   0 avliu      (504) staff       (20)      228 2023-07-27 15:54:00.000000 scraper_util_avliu-0.1.0/README.md
+-rw-r--r--   0 avliu      (504) staff       (20)      269 2023-07-27 16:03:32.000000 scraper_util_avliu-0.1.0/pyproject.toml
+-rw-r--r--   0 avliu      (504) staff       (20)       38 2023-07-27 16:03:39.244228 scraper_util_avliu-0.1.0/setup.cfg
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:03:39.241094 scraper_util_avliu-0.1.0/src/
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:03:39.242775 scraper_util_avliu-0.1.0/src/scraper_util_avliu/
+-rw-r--r--   0 avliu      (504) staff       (20)        1 2023-06-20 08:37:43.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu/__init__.py
+-rw-r--r--   0 avliu      (504) staff       (20)       36 2023-07-27 16:01:51.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu/example.py
+-rw-r--r--   0 avliu      (504) staff       (20)     3246 2023-07-27 15:36:17.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu/util.py
+drwxr-xr-x   0 avliu      (504) staff       (20)        0 2023-07-27 16:03:39.243755 scraper_util_avliu-0.1.0/src/scraper_util_avliu.egg-info/
+-rw-r--r--   0 avliu      (504) staff       (20)       84 2023-07-27 16:03:39.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu.egg-info/PKG-INFO
+-rw-r--r--   0 avliu      (504) staff       (20)      361 2023-07-27 16:03:39.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu.egg-info/SOURCES.txt
+-rw-r--r--   0 avliu      (504) staff       (20)        1 2023-07-27 16:03:39.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu.egg-info/dependency_links.txt
+-rw-r--r--   0 avliu      (504) staff       (20)       72 2023-07-27 16:03:39.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu.egg-info/requires.txt
+-rw-r--r--   0 avliu      (504) staff       (20)       19 2023-07-27 16:03:39.000000 scraper_util_avliu-0.1.0/src/scraper_util_avliu.egg-info/top_level.txt
```

