# Comparing `tmp/latch-sdk-config-0.0.1.tar.gz` & `tmp/latch-sdk-config-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch-sdk-config-0.0.1.tar", last modified: Thu Jun 22 20:23:48 2023, max compression
+gzip compressed data, was "latch-sdk-config-0.0.2.tar", last modified: Thu Jul 27 20:48:55 2023, max compression
```

## Comparing `latch-sdk-config-0.0.1.tar` & `latch-sdk-config-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-06-22 20:23:48.700125 latch-sdk-config-0.0.1/
--rw-r--r--   0 ayush      (504) staff       (20)     1065 2023-06-22 20:17:42.000000 latch-sdk-config-0.0.1/LICENSE
--rw-r--r--   0 ayush      (504) staff       (20)      333 2023-06-22 20:23:48.699824 latch-sdk-config-0.0.1/PKG-INFO
--rw-r--r--   0 ayush      (504) staff       (20)       18 2023-06-22 20:17:42.000000 latch-sdk-config-0.0.1/README.md
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-06-22 20:23:48.697564 latch-sdk-config-0.0.1/latch_sdk_config/
--rw-r--r--   0 ayush      (504) staff       (20)        0 2023-06-22 20:04:50.000000 latch-sdk-config-0.0.1/latch_sdk_config/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)     2985 2023-06-22 20:04:50.000000 latch-sdk-config-0.0.1/latch_sdk_config/latch.py
--rw-r--r--   0 ayush      (504) staff       (20)     2877 2023-06-22 20:04:50.000000 latch-sdk-config-0.0.1/latch_sdk_config/user.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-06-22 20:23:48.699364 latch-sdk-config-0.0.1/latch_sdk_config.egg-info/
--rw-r--r--   0 ayush      (504) staff       (20)      333 2023-06-22 20:23:48.000000 latch-sdk-config-0.0.1/latch_sdk_config.egg-info/PKG-INFO
--rw-r--r--   0 ayush      (504) staff       (20)      266 2023-06-22 20:23:48.000000 latch-sdk-config-0.0.1/latch_sdk_config.egg-info/SOURCES.txt
--rw-r--r--   0 ayush      (504) staff       (20)        1 2023-06-22 20:23:48.000000 latch-sdk-config-0.0.1/latch_sdk_config.egg-info/dependency_links.txt
--rw-r--r--   0 ayush      (504) staff       (20)       17 2023-06-22 20:23:48.000000 latch-sdk-config-0.0.1/latch_sdk_config.egg-info/top_level.txt
--rw-r--r--   0 ayush      (504) staff       (20)       38 2023-06-22 20:23:48.700213 latch-sdk-config-0.0.1/setup.cfg
--rw-r--r--   0 ayush      (504) staff       (20)      461 2023-06-22 20:12:38.000000 latch-sdk-config-0.0.1/setup.py
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 20:48:55.943405 latch-sdk-config-0.0.2/
+-rw-r--r--   0 aidan      (501) staff       (20)     1065 2023-07-26 19:50:42.000000 latch-sdk-config-0.0.2/LICENSE
+-rw-r--r--   0 aidan      (501) staff       (20)      448 2023-07-27 20:48:55.943138 latch-sdk-config-0.0.2/PKG-INFO
+-rw-r--r--   0 aidan      (501) staff       (20)       18 2023-07-26 19:50:42.000000 latch-sdk-config-0.0.2/README.md
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 20:48:55.941764 latch-sdk-config-0.0.2/latch_sdk_config/
+-rw-r--r--   0 aidan      (501) staff       (20)        0 2023-07-26 19:50:42.000000 latch-sdk-config-0.0.2/latch_sdk_config/__init__.py
+-rw-r--r--   0 aidan      (501) staff       (20)     2985 2023-07-26 19:57:35.000000 latch-sdk-config-0.0.2/latch_sdk_config/latch.py
+-rw-r--r--   0 aidan      (501) staff       (20)     2877 2023-07-26 19:50:42.000000 latch-sdk-config-0.0.2/latch_sdk_config/user.py
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 20:48:55.942810 latch-sdk-config-0.0.2/latch_sdk_config.egg-info/
+-rw-r--r--   0 aidan      (501) staff       (20)      448 2023-07-27 20:48:55.000000 latch-sdk-config-0.0.2/latch_sdk_config.egg-info/PKG-INFO
+-rw-r--r--   0 aidan      (501) staff       (20)      266 2023-07-27 20:48:55.000000 latch-sdk-config-0.0.2/latch_sdk_config.egg-info/SOURCES.txt
+-rw-r--r--   0 aidan      (501) staff       (20)        1 2023-07-27 20:48:55.000000 latch-sdk-config-0.0.2/latch_sdk_config.egg-info/dependency_links.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       17 2023-07-27 20:48:55.000000 latch-sdk-config-0.0.2/latch_sdk_config.egg-info/top_level.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       38 2023-07-27 20:48:55.943488 latch-sdk-config-0.0.2/setup.cfg
+-rw-r--r--   0 aidan      (501) staff       (20)      511 2023-07-27 20:48:49.000000 latch-sdk-config-0.0.2/setup.py
```

### Comparing `latch-sdk-config-0.0.1/LICENSE` & `latch-sdk-config-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `latch-sdk-config-0.0.1/latch_sdk_config/latch.py` & `latch-sdk-config-0.0.2/latch_sdk_config/latch.py`

 * *Files identical despite different names*

### Comparing `latch-sdk-config-0.0.1/latch_sdk_config/user.py` & `latch-sdk-config-0.0.2/latch_sdk_config/user.py`

 * *Files identical despite different names*

