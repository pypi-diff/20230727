# Comparing `tmp/litellm-0.1.0.tar.gz` & `tmp/litellm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.0.tar", last modified: Thu Jul 27 00:36:08 2023, max compression
+gzip compressed data, was "litellm-0.1.1.tar", last modified: Thu Jul 27 05:06:49 2023, max compression
```

## Comparing `litellm-0.1.0.tar` & `litellm-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-27 00:36:08.994420 litellm-0.1.0/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-07-27 00:10:35.000000 litellm-0.1.0/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      219 2023-07-27 00:36:08.994315 litellm-0.1.0/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        9 2023-07-27 00:10:35.000000 litellm-0.1.0/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-27 00:36:08.993509 litellm-0.1.0/litellm/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       58 2023-07-27 00:22:07.000000 litellm-0.1.0/litellm/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2942 2023-07-27 00:31:01.000000 litellm-0.1.0/litellm/main.py
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-27 00:36:08.994165 litellm-0.1.0/litellm.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      219 2023-07-27 00:36:08.000000 litellm-0.1.0/litellm.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      216 2023-07-27 00:36:08.000000 litellm-0.1.0/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-27 00:36:08.000000 litellm-0.1.0/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       17 2023-07-27 00:36:08.000000 litellm-0.1.0/litellm.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        8 2023-07-27 00:36:08.000000 litellm-0.1.0/litellm.egg-info/top_level.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-27 00:36:08.994459 litellm-0.1.0/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      313 2023-07-27 00:34:23.000000 litellm-0.1.0/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-27 05:06:49.030132 litellm-0.1.1/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-07-27 00:10:35.000000 litellm-0.1.1/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      219 2023-07-27 05:06:49.029932 litellm-0.1.1/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        9 2023-07-27 00:10:35.000000 litellm-0.1.1/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-27 05:06:49.029042 litellm-0.1.1/litellm/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       58 2023-07-27 00:22:07.000000 litellm-0.1.1/litellm/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2942 2023-07-27 00:31:01.000000 litellm-0.1.1/litellm/main.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-27 05:06:49.029783 litellm-0.1.1/litellm.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      219 2023-07-27 05:06:49.000000 litellm-0.1.1/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      216 2023-07-27 05:06:49.000000 litellm-0.1.1/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-27 05:06:49.000000 litellm-0.1.1/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       14 2023-07-27 05:06:49.000000 litellm-0.1.1/litellm.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        8 2023-07-27 05:06:49.000000 litellm-0.1.1/litellm.egg-info/top_level.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-27 05:06:49.030171 litellm-0.1.1/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      299 2023-07-27 05:06:30.000000 litellm-0.1.1/setup.py
```

### Comparing `litellm-0.1.0/LICENSE` & `litellm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.0/litellm/main.py` & `litellm-0.1.1/litellm/main.py`

 * *Files identical despite different names*

