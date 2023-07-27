# Comparing `tmp/test-library-sina-0.1.tar.gz` & `tmp/test-library-sina-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-library-sina-0.1.tar", last modified: Thu Jul 27 09:08:52 2023, max compression
+gzip compressed data, was "test-library-sina-0.2.tar", last modified: Thu Jul 27 09:52:54 2023, max compression
```

## Comparing `test-library-sina-0.1.tar` & `test-library-sina-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-07-27 09:08:52.505301 test-library-sina-0.1/
--rw-rw-r--   0 sina      (1000) sina      (1000)      233 2023-07-27 09:08:52.505301 test-library-sina-0.1/PKG-INFO
--rw-rw-r--   0 sina      (1000) sina      (1000)       24 2023-07-27 09:01:30.000000 test-library-sina-0.1/README.md
--rw-rw-r--   0 sina      (1000) sina      (1000)       38 2023-07-27 09:08:52.505301 test-library-sina-0.1/setup.cfg
--rw-rw-r--   0 sina      (1000) sina      (1000)      259 2023-07-27 09:06:37.000000 test-library-sina-0.1/setup.py
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-07-27 09:08:52.505301 test-library-sina-0.1/test_library_sina.egg-info/
--rw-rw-r--   0 sina      (1000) sina      (1000)      233 2023-07-27 09:08:52.000000 test-library-sina-0.1/test_library_sina.egg-info/PKG-INFO
--rw-rw-r--   0 sina      (1000) sina      (1000)      182 2023-07-27 09:08:52.000000 test-library-sina-0.1/test_library_sina.egg-info/SOURCES.txt
--rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-07-27 09:08:52.000000 test-library-sina-0.1/test_library_sina.egg-info/dependency_links.txt
--rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-07-27 09:08:52.000000 test-library-sina-0.1/test_library_sina.egg-info/top_level.txt
+drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-07-27 09:52:54.926968 test-library-sina-0.2/
+-rw-rw-r--   0 sina      (1000) sina      (1000)      233 2023-07-27 09:52:54.926968 test-library-sina-0.2/PKG-INFO
+-rw-rw-r--   0 sina      (1000) sina      (1000)       24 2023-07-27 09:01:30.000000 test-library-sina-0.2/README.md
+-rw-rw-r--   0 sina      (1000) sina      (1000)       38 2023-07-27 09:52:54.926968 test-library-sina-0.2/setup.cfg
+-rw-rw-r--   0 sina      (1000) sina      (1000)      259 2023-07-27 09:41:34.000000 test-library-sina-0.2/setup.py
+drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2023-07-27 09:52:54.926968 test-library-sina-0.2/test_library_sina.egg-info/
+-rw-rw-r--   0 sina      (1000) sina      (1000)      233 2023-07-27 09:52:54.000000 test-library-sina-0.2/test_library_sina.egg-info/PKG-INFO
+-rw-rw-r--   0 sina      (1000) sina      (1000)      182 2023-07-27 09:52:54.000000 test-library-sina-0.2/test_library_sina.egg-info/SOURCES.txt
+-rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-07-27 09:52:54.000000 test-library-sina-0.2/test_library_sina.egg-info/dependency_links.txt
+-rw-rw-r--   0 sina      (1000) sina      (1000)        1 2023-07-27 09:52:54.000000 test-library-sina-0.2/test_library_sina.egg-info/top_level.txt
```

