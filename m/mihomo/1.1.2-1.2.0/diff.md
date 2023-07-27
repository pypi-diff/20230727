# Comparing `tmp/mihomo-1.1.2.tar.gz` & `tmp/mihomo-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mihomo-1.1.2.tar", max compression
+gzip compressed data, was "mihomo-1.2.0.tar", max compression
```

## Comparing `mihomo-1.1.2.tar` & `mihomo-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1090 2023-06-01 05:14:24.496130 mihomo-1.1.2/LICENSE
--rw-r--r--   0        0        0       90 2023-06-07 08:41:32.652372 mihomo-1.1.2/mihomo/__init__.py
--rw-r--r--   0        0        0     9776 2023-06-11 14:18:31.889759 mihomo-1.1.2/mihomo/api.py
--rw-r--r--   0        0        0     2580 2023-06-10 14:25:51.380485 mihomo-1.1.2/mihomo/model.py
--rw-r--r--   0        0        0      479 2023-06-11 14:20:16.892668 mihomo-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1434 2023-06-01 05:26:11.111124 mihomo-1.1.2/README.md
--rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 mihomo-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-01 05:14:24.496130 mihomo-1.2.0/LICENSE
+-rw-r--r--   0        0        0       90 2023-06-07 08:41:32.652372 mihomo-1.2.0/mihomo/__init__.py
+-rw-r--r--   0        0        0     9776 2023-07-27 06:37:14.996641 mihomo-1.2.0/mihomo/api.py
+-rw-r--r--   0        0        0     2580 2023-06-10 14:25:51.380485 mihomo-1.2.0/mihomo/model.py
+-rw-r--r--   0        0        0      479 2023-07-27 07:37:14.949222 mihomo-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1434 2023-06-01 05:26:11.111124 mihomo-1.2.0/README.md
+-rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 mihomo-1.2.0/PKG-INFO
```

### Comparing `mihomo-1.1.2/LICENSE` & `mihomo-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mihomo-1.1.2/mihomo/api.py` & `mihomo-1.2.0/mihomo/api.py`

 * *Files identical despite different names*

### Comparing `mihomo-1.1.2/mihomo/model.py` & `mihomo-1.2.0/mihomo/model.py`

 * *Files identical despite different names*

### Comparing `mihomo-1.1.2/README.md` & `mihomo-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mihomo-1.1.2/PKG-INFO` & `mihomo-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mihomo
-Version: 1.1.2
+Version: 1.2.0
 Summary: Library for API wrapper data from mihomo
 Home-page: https://github.com/Mar-7th/mihomo.py
 License: MIT
 Author: mobyw
 Author-email: mobyw66@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: msgspec (>=0.15.1,<0.16.0)
-Requires-Dist: starrailres (>=1.1.2,<2.0.0)
+Requires-Dist: starrailres (>=1.2.0,<2.0.0)
 Project-URL: Repository, https://github.com/Mar-7th/mihomo.py
 Description-Content-Type: text/markdown
 
 # mihomo.py
 
 ## Introduction
```

