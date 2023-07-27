# Comparing `tmp/invest_life-0.0.3.tar.gz` & `tmp/invest_life-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest_life-0.0.3.tar", last modified: Thu Jul 27 06:57:29 2023, max compression
+gzip compressed data, was "invest_life-0.0.4.tar", last modified: Thu Jul 27 08:39:05 2023, max compression
```

## Comparing `invest_life-0.0.3.tar` & `invest_life-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 06:57:29.477885 invest_life-0.0.3/
--rw-r--r--   0 mac        (501) staff       (20)     1073 2023-07-25 13:12:51.000000 invest_life-0.0.3/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-27 06:57:29.477584 invest_life-0.0.3/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      159 2023-07-25 13:12:33.000000 invest_life-0.0.3/README.md
--rw-r--r--   0 mac        (501) staff       (20)      459 2023-07-27 06:56:46.000000 invest_life-0.0.3/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-27 06:57:29.477985 invest_life-0.0.3/setup.cfg
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 06:57:29.474302 invest_life-0.0.3/src/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-07-25 13:00:59.000000 invest_life-0.0.3/src/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 06:57:29.476347 invest_life-0.0.3/src/invest_life.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-27 06:57:29.000000 invest_life-0.0.3/src/invest_life.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      236 2023-07-27 06:57:29.000000 invest_life-0.0.3/src/invest_life.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-27 06:57:29.000000 invest_life-0.0.3/src/invest_life.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       20 2023-07-27 06:57:29.000000 invest_life-0.0.3/src/invest_life.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)    53621 2023-07-27 06:55:15.000000 invest_life-0.0.3/src/investlife.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 06:57:29.476788 invest_life-0.0.3/tests/
--rw-r--r--   0 mac        (501) staff       (20)       24 2023-07-25 14:03:29.000000 invest_life-0.0.3/tests/test.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 08:39:05.073386 invest_life-0.0.4/
+-rw-r--r--   0 mac        (501) staff       (20)     1073 2023-07-25 13:12:51.000000 invest_life-0.0.4/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-27 08:39:05.070343 invest_life-0.0.4/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      159 2023-07-25 13:12:33.000000 invest_life-0.0.4/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      459 2023-07-27 08:38:55.000000 invest_life-0.0.4/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-27 08:39:05.074706 invest_life-0.0.4/setup.cfg
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 08:39:05.061653 invest_life-0.0.4/src/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-07-25 13:00:59.000000 invest_life-0.0.4/src/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 08:39:05.067603 invest_life-0.0.4/src/invest_life.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      634 2023-07-27 08:39:05.000000 invest_life-0.0.4/src/invest_life.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      236 2023-07-27 08:39:05.000000 invest_life-0.0.4/src/invest_life.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-27 08:39:05.000000 invest_life-0.0.4/src/invest_life.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       20 2023-07-27 08:39:05.000000 invest_life-0.0.4/src/invest_life.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)   212847 2023-07-27 08:37:55.000000 invest_life-0.0.4/src/investlife.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-27 08:39:05.069466 invest_life-0.0.4/tests/
+-rw-r--r--   0 mac        (501) staff       (20)       24 2023-07-25 14:03:29.000000 invest_life-0.0.4/tests/test.py
```

### Comparing `invest_life-0.0.3/LICENSE` & `invest_life-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `invest_life-0.0.3/PKG-INFO` & `invest_life-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest_life
-Version: 0.0.3
+Version: 0.0.4
 Summary: a package from investor
 Author-email: kelvin <wwwhhitzxt@163.com>
 Project-URL: Homepage, https://investlife.cn/
 Project-URL: Bug Tracker, https://investlife.cn/info/author.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `invest_life-0.0.3/src/invest_life.egg-info/PKG-INFO` & `invest_life-0.0.4/src/invest_life.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-life
-Version: 0.0.3
+Version: 0.0.4
 Summary: a package from investor
 Author-email: kelvin <wwwhhitzxt@163.com>
 Project-URL: Homepage, https://investlife.cn/
 Project-URL: Bug Tracker, https://investlife.cn/info/author.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

