# Comparing `tmp/minlog-0.1.0.tar.gz` & `tmp/minlog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minlog-0.1.0.tar", max compression
+gzip compressed data, was "minlog-0.2.0.tar", max compression
```

## Comparing `minlog-0.1.0.tar` & `minlog-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       26 2023-06-07 18:56:59.420529 minlog-0.1.0/README.md
--rw-r--r--   0        0        0     1718 2023-06-07 18:55:13.390059 minlog-0.1.0/minlog/__init__.py
--rw-r--r--   0        0        0      277 2023-06-07 18:55:57.300254 minlog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 minlog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       26 2023-06-07 18:56:59.420529 minlog-0.2.0/README.md
+-rw-r--r--   0        0        0     1718 2023-06-07 18:55:13.390059 minlog-0.2.0/minlog/__init__.py
+-rw-r--r--   0        0        0      297 2023-07-27 02:20:10.373316 minlog-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 minlog-0.2.0/PKG-INFO
```

### Comparing `minlog-0.1.0/minlog/__init__.py` & `minlog-0.2.0/minlog/__init__.py`

 * *Files identical despite different names*

