# Comparing `tmp/slippers-0.6.1.tar.gz` & `tmp/slippers-0.6.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slippers-0.6.1.tar", max compression
+gzip compressed data, was "slippers-0.6.1a0.tar", max compression
```

## Comparing `slippers-0.6.1.tar` & `slippers-0.6.1a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-07-27 18:48:26.070549 slippers-0.6.1/LICENSE
--rw-r--r--   0        0        0     2059 2023-07-27 18:48:26.070549 slippers-0.6.1/README.md
--rw-r--r--   0        0        0     1211 2023-07-27 18:48:26.078549 slippers-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       99 2023-07-27 18:48:26.078549 slippers-0.6.1/slippers/__init__.py
--rw-r--r--   0        0        0     1861 2023-07-27 18:48:26.078549 slippers-0.6.1/slippers/apps.py
--rw-r--r--   0        0        0      783 2023-07-27 18:48:26.078549 slippers-0.6.1/slippers/conf.py
--rw-r--r--   0        0        0     4833 2023-07-27 18:48:26.078549 slippers-0.6.1/slippers/props.py
--rw-r--r--   0        0        0     7361 2023-07-27 18:49:14.126619 slippers-0.6.1/slippers/static/slippers/main.css
--rw-r--r--   0        0        0   146850 2023-07-27 18:49:14.126619 slippers-0.6.1/slippers/static/slippers/main.js
--rw-r--r--   0        0        0     5801 2023-07-27 18:48:26.078549 slippers-0.6.1/slippers/template.py
--rw-r--r--   0        0        0      327 2023-07-27 18:48:26.078549 slippers-0.6.1/slippers/templates/slippers/overlay.html
--rw-r--r--   0        0        0        0 2023-07-27 18:48:26.078549 slippers-0.6.1/slippers/templatetags/__init__.py
--rw-r--r--   0        0        0     8957 2023-07-27 18:48:26.082549 slippers-0.6.1/slippers/templatetags/slippers.py
--rw-r--r--   0        0        0     3373 1970-01-01 00:00:00.000000 slippers-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-27 15:26:20.255319 slippers-0.6.1a0/LICENSE
+-rw-r--r--   0        0        0     2059 2023-07-27 15:26:20.255319 slippers-0.6.1a0/README.md
+-rw-r--r--   0        0        0     1213 2023-07-27 15:26:20.267319 slippers-0.6.1a0/pyproject.toml
+-rw-r--r--   0        0        0       52 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/__init__.py
+-rw-r--r--   0        0        0     1861 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/apps.py
+-rw-r--r--   0        0        0      783 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/conf.py
+-rw-r--r--   0        0        0     4833 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/props.py
+-rw-r--r--   0        0        0     7361 2023-07-27 15:27:36.693054 slippers-0.6.1a0/slippers/static/slippers/main.css
+-rw-r--r--   0        0        0   146850 2023-07-27 15:27:36.693054 slippers-0.6.1a0/slippers/static/slippers/main.js
+-rw-r--r--   0        0        0     5801 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/template.py
+-rw-r--r--   0        0        0      327 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/templates/slippers/overlay.html
+-rw-r--r--   0        0        0        0 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/templatetags/__init__.py
+-rw-r--r--   0        0        0     8957 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/templatetags/slippers.py
+-rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 slippers-0.6.1a0/PKG-INFO
```

### Comparing `slippers-0.6.1/LICENSE` & `slippers-0.6.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1/README.md` & `slippers-0.6.1a0/README.md`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1/pyproject.toml` & `slippers-0.6.1a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slippers"
-version = "0.6.1"
+version = "0.6.1a0"
 description = "Build reusable components in Django without writing a single line of Python."
 authors = ["Mitchel Cabuloy <mixxorz@gmail.com>"]
 keywords = ["django", "components"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/mixxorz/slippers"
 repository = "https://github.com/mixxorz/slippers"
```

### Comparing `slippers-0.6.1/slippers/apps.py` & `slippers-0.6.1a0/slippers/apps.py`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1/slippers/conf.py` & `slippers-0.6.1a0/slippers/conf.py`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1/slippers/props.py` & `slippers-0.6.1a0/slippers/props.py`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1/slippers/static/slippers/main.css` & `slippers-0.6.1a0/slippers/static/slippers/main.css`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1/slippers/static/slippers/main.js` & `slippers-0.6.1a0/slippers/static/slippers/main.js`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1/slippers/template.py` & `slippers-0.6.1a0/slippers/template.py`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1/slippers/templatetags/slippers.py` & `slippers-0.6.1a0/slippers/templatetags/slippers.py`

 * *Files identical despite different names*

### Comparing `slippers-0.6.1/PKG-INFO` & `slippers-0.6.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slippers
-Version: 0.6.1
+Version: 0.6.1a0
 Summary: Build reusable components in Django without writing a single line of Python.
 Home-page: https://github.com/mixxorz/slippers
 License: MIT
 Keywords: django,components
 Author: Mitchel Cabuloy
 Author-email: mixxorz@gmail.com
 Requires-Python: >=3.7.0
```

