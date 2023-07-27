# Comparing `tmp/mylibrarysina-1.1.4.tar.gz` & `tmp/mylibrarysina-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mylibrarysina-1.1.4.tar", last modified: Thu Jul 27 12:45:44 2023, max compression
+gzip compressed data, was "mylibrarysina-1.1.5.tar", last modified: Thu Jul 27 12:48:02 2023, max compression
```

## Comparing `mylibrarysina-1.1.4.tar` & `mylibrarysina-1.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-07-27 12:45:44.216406 mylibrarysina-1.1.4/
--rw-rw-r--   0 sina      (1000) sina      (1000)        0 2023-07-27 11:15:26.000000 mylibrarysina-1.1.4/LICENSE
--rw-rw-r--   0 sina      (1000) sina      (1000)      252 2023-07-27 12:45:44.216406 mylibrarysina-1.1.4/PKG-INFO
--rw-rw-r--   0 sina      (1000) sina      (1000)       21 2023-07-27 11:14:06.000000 mylibrarysina-1.1.4/README.md
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-07-27 12:45:44.216406 mylibrarysina-1.1.4/mylibrarysina.egg-info/
--rw-rw-r--   0 sina      (1000) sina      (1000)      252 2023-07-27 12:45:44.000000 mylibrarysina-1.1.4/mylibrarysina.egg-info/PKG-INFO
--rw-rw-r--   0 sina      (1000) sina      (1000)      174 2023-07-27 12:45:44.000000 mylibrarysina-1.1.4/mylibrarysina.egg-info/SOURCES.txt
--rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-07-27 12:45:44.000000 mylibrarysina-1.1.4/mylibrarysina.egg-info/dependency_links.txt
--rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-07-27 12:45:44.000000 mylibrarysina-1.1.4/mylibrarysina.egg-info/top_level.txt
--rw-rw-r--   0 sina      (1000) sina      (1000)       38 2023-07-27 12:45:44.216406 mylibrarysina-1.1.4/setup.cfg
--rw-rw-r--   0 sina      (1000) sina      (1000)      313 2023-07-27 12:45:34.000000 mylibrarysina-1.1.4/setup.py
+drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-07-27 12:48:02.369215 mylibrarysina-1.1.5/
+-rw-rw-r--   0 sina      (1000) sina      (1000)        0 2023-07-27 11:15:26.000000 mylibrarysina-1.1.5/LICENSE
+-rw-rw-r--   0 sina      (1000) sina      (1000)      690 2023-07-27 12:48:02.369215 mylibrarysina-1.1.5/PKG-INFO
+-rw-rw-r--   0 sina      (1000) sina      (1000)       21 2023-07-27 11:14:06.000000 mylibrarysina-1.1.5/README.md
+drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-07-27 12:48:02.369215 mylibrarysina-1.1.5/mylibrarysina.egg-info/
+-rw-rw-r--   0 sina      (1000) sina      (1000)      690 2023-07-27 12:48:02.000000 mylibrarysina-1.1.5/mylibrarysina.egg-info/PKG-INFO
+-rw-rw-r--   0 sina      (1000) sina      (1000)      174 2023-07-27 12:48:02.000000 mylibrarysina-1.1.5/mylibrarysina.egg-info/SOURCES.txt
+-rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-07-27 12:48:02.000000 mylibrarysina-1.1.5/mylibrarysina.egg-info/dependency_links.txt
+-rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-07-27 12:48:02.000000 mylibrarysina-1.1.5/mylibrarysina.egg-info/top_level.txt
+-rw-rw-r--   0 sina      (1000) sina      (1000)       38 2023-07-27 12:48:02.369215 mylibrarysina-1.1.5/setup.cfg
+-rw-rw-r--   0 sina      (1000) sina      (1000)      742 2023-07-27 12:47:57.000000 mylibrarysina-1.1.5/setup.py
```

