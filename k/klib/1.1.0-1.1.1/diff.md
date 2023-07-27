# Comparing `tmp/klib-1.1.0.tar.gz` & `tmp/klib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klib-1.1.0.tar", max compression
+gzip compressed data, was "klib-1.1.1.tar", max compression
```

## Comparing `klib-1.1.0.tar` & `klib-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2022-07-29 17:32:38.054377 klib-1.1.0/LICENSE
--rw-r--r--   0        0        0     6641 2023-07-27 15:29:23.883519 klib-1.1.0/README.md
--rw-r--r--   0        0        0     2791 2023-07-27 16:14:46.581492 klib-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1033 2023-07-27 16:15:40.773253 klib-1.1.0/src/klib/__init__.py
--rw-r--r--   0        0        0       54 2023-07-27 16:12:00.886675 klib-1.1.0/src/klib/_version.py
--rw-r--r--   0        0        0    20871 2023-07-27 15:29:23.896625 klib-1.1.0/src/klib/clean.py
--rw-r--r--   0        0        0    35236 2023-07-27 16:14:17.270224 klib-1.1.0/src/klib/describe.py
--rw-r--r--   0        0        0        0 2023-07-27 15:29:23.897081 klib-1.1.0/src/klib/scripts/__init__.py
--rw-r--r--   0        0        0     1745 2023-07-27 15:29:23.897579 klib-1.1.0/src/klib/scripts/performance.py
--rw-r--r--   0        0        0     9779 2023-07-27 15:29:23.897878 klib-1.1.0/src/klib/utils.py
--rw-r--r--   0        0        0        0 2022-07-29 17:32:38.390459 klib-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0    10815 2023-07-27 15:29:23.898195 klib-1.1.0/tests/test_clean.py
--rw-r--r--   0        0        0     3799 2023-07-27 15:29:23.898345 klib-1.1.0/tests/test_describe.py
--rw-r--r--   0        0        0     9181 2023-07-27 15:29:23.898650 klib-1.1.0/tests/test_util.py
--rw-r--r--   0        0        0     7508 1970-01-01 00:00:00.000000 klib-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-07-29 17:32:38.054377 klib-1.1.1/LICENSE
+-rw-r--r--   0        0        0     6641 2023-07-27 15:29:23.883519 klib-1.1.1/README.md
+-rw-r--r--   0        0        0     2791 2023-07-27 16:43:14.339407 klib-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1033 2023-07-27 16:15:40.773253 klib-1.1.1/src/klib/__init__.py
+-rw-r--r--   0        0        0       54 2023-07-27 16:43:18.499492 klib-1.1.1/src/klib/_version.py
+-rw-r--r--   0        0        0    20871 2023-07-27 15:29:23.896625 klib-1.1.1/src/klib/clean.py
+-rw-r--r--   0        0        0    35202 2023-07-27 16:40:52.007334 klib-1.1.1/src/klib/describe.py
+-rw-r--r--   0        0        0        0 2023-07-27 15:29:23.897081 klib-1.1.1/src/klib/scripts/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-27 15:29:23.897579 klib-1.1.1/src/klib/scripts/performance.py
+-rw-r--r--   0        0        0     9779 2023-07-27 15:29:23.897878 klib-1.1.1/src/klib/utils.py
+-rw-r--r--   0        0        0        0 2022-07-29 17:32:38.390459 klib-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    10815 2023-07-27 15:29:23.898195 klib-1.1.1/tests/test_clean.py
+-rw-r--r--   0        0        0     3799 2023-07-27 15:29:23.898345 klib-1.1.1/tests/test_describe.py
+-rw-r--r--   0        0        0     9181 2023-07-27 15:29:23.898650 klib-1.1.1/tests/test_util.py
+-rw-r--r--   0        0        0     7508 1970-01-01 00:00:00.000000 klib-1.1.1/PKG-INFO
```

### Comparing `klib-1.1.0/LICENSE` & `klib-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `klib-1.1.0/README.md` & `klib-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `klib-1.1.0/pyproject.toml` & `klib-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "klib"
-version = "1.1.0"
+version = "1.1.1"
 description = "Customized data preprocessing functions for frequent tasks."
 authors = ["Andreas Kanz <andreas@akanz.de>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [{ include = "klib", from = "src" }]
 include = [{ path = "tests", format = "sdist" }]
```

### Comparing `klib-1.1.0/src/klib/__init__.py` & `klib-1.1.1/src/klib/__init__.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.0/src/klib/clean.py` & `klib-1.1.1/src/klib/clean.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.0/src/klib/describe.py` & `klib-1.1.1/src/klib/describe.py`

 * *Files 1% similar despite different names*

```diff
@@ -610,29 +610,28 @@
             hoverongaps=False,
             xgap=1,
             ygap=1,
             **kwargs,
         ),
     )
 
-    dpi = 96  # more or less arbitrary default value
+    dpi = None
     for monitor in get_monitors():
         if monitor.is_primary:
             if monitor.width_mm is None or monitor.height_mm is None:
                 continue
             dpi = monitor.width / (monitor.width_mm / 25.4)
             break
 
     if dpi is None:
-        try:
-            monitor = get_monitors()[0]
+        monitor = get_monitors()[0]
+        if monitor.width_mm is None or monitor.height_mm is None:
+            dpi = 96  # more or less arbitrary default value
+        else:
             dpi = monitor.width / (monitor.width_mm / 25.4)
-        except ValueError as exc:
-            msg = "Monitor doesn't exist"
-            raise LookupError(msg) from exc
 
     heatmap.update_layout(
         title=f"Feature-correlation ({method})",
         title_font={"size": 24},
         title_x=0.5,
         autosize=True,
         width=figsize[0] * dpi,
```

### Comparing `klib-1.1.0/src/klib/scripts/performance.py` & `klib-1.1.1/src/klib/scripts/performance.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.0/src/klib/utils.py` & `klib-1.1.1/src/klib/utils.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.0/tests/test_clean.py` & `klib-1.1.1/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.0/tests/test_describe.py` & `klib-1.1.1/tests/test_describe.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.0/tests/test_util.py` & `klib-1.1.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `klib-1.1.0/PKG-INFO` & `klib-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klib
-Version: 1.1.0
+Version: 1.1.1
 Summary: Customized data preprocessing functions for frequent tasks.
 License: MIT
 Author: Andreas Kanz
 Author-email: andreas@akanz.de
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

