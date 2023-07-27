# Comparing `tmp/HandyLLM-0.1.0.tar.gz` & `tmp/HandyLLM-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandyLLM-0.1.0.tar", last modified: Fri Jun 30 05:37:57 2023, max compression
+gzip compressed data, was "HandyLLM-0.2.0.tar", last modified: Thu Jul 27 03:54:14 2023, max compression
```

## Comparing `HandyLLM-0.1.0.tar` & `HandyLLM-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:37:57.410127 HandyLLM-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-30 05:37:57.410127 HandyLLM-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-30 05:37:47.000000 HandyLLM-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-30 05:37:47.000000 HandyLLM-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 05:37:57.410127 HandyLLM-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:37:57.406128 HandyLLM-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:37:57.410127 HandyLLM-0.1.0/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-30 05:37:57.000000 HandyLLM-0.1.0/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-30 05:37:57.000000 HandyLLM-0.1.0/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 05:37:57.000000 HandyLLM-0.1.0/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 05:37:57.000000 HandyLLM-0.1.0/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 05:37:57.000000 HandyLLM-0.1.0/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:37:57.410127 HandyLLM-0.1.0/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-30 05:37:47.000000 HandyLLM-0.1.0/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-30 05:37:47.000000 HandyLLM-0.1.0/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-30 05:37:47.000000 HandyLLM-0.1.0/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-30 05:37:47.000000 HandyLLM-0.1.0/src/handyllm/prompt_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-27 03:54:14.000000 HandyLLM-0.2.0/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 03:54:14.000000 HandyLLM-0.2.0/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:54:14.000000 HandyLLM-0.2.0/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 03:54:14.000000 HandyLLM-0.2.0/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 03:54:14.000000 HandyLLM-0.2.0/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/src/handyllm/prompt_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/tests/test_stream.py
```

### Comparing `HandyLLM-0.1.0/pyproject.toml` & `HandyLLM-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `HandyLLM-0.1.0/src/handyllm/endpoint_manager.py` & `HandyLLM-0.2.0/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.1.0/src/handyllm/prompt_converter.py` & `HandyLLM-0.2.0/src/handyllm/prompt_converter.py`

 * *Files identical despite different names*

