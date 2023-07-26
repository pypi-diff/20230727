# Comparing `tmp/libtimed-0.4.3.tar.gz` & `tmp/libtimed-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtimed-0.4.3.tar", max compression
+gzip compressed data, was "libtimed-0.4.4.tar", max compression
```

## Comparing `libtimed-0.4.3.tar` & `libtimed-0.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34454 2023-07-25 08:48:09.724395 libtimed-0.4.3/LICENSE
--rw-r--r--   0        0        0      750 2023-07-25 08:48:09.724395 libtimed-0.4.3/README.md
--rw-r--r--   0        0        0     1307 2023-07-25 08:48:10.824418 libtimed-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1376 2023-07-25 08:48:09.724395 libtimed-0.4.3/src/libtimed/__init__.py
--rw-r--r--   0        0        0     9528 2023-07-25 08:48:09.724395 libtimed-0.4.3/src/libtimed/models.py
--rw-r--r--   0        0        0     4555 2023-07-25 08:48:09.724395 libtimed-0.4.3/src/libtimed/oidc.py
--rw-r--r--   0        0        0     6195 2023-07-25 08:48:09.724395 libtimed-0.4.3/src/libtimed/transforms.py
--rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 libtimed-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-26 22:10:19.305066 libtimed-0.4.4/LICENSE
+-rw-r--r--   0        0        0      750 2023-07-26 22:10:19.305066 libtimed-0.4.4/README.md
+-rw-r--r--   0        0        0     1307 2023-07-26 22:10:20.121081 libtimed-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1376 2023-07-26 22:10:19.305066 libtimed-0.4.4/src/libtimed/__init__.py
+-rw-r--r--   0        0        0     9583 2023-07-26 22:10:19.305066 libtimed-0.4.4/src/libtimed/models.py
+-rw-r--r--   0        0        0     4555 2023-07-26 22:10:19.305066 libtimed-0.4.4/src/libtimed/oidc.py
+-rw-r--r--   0        0        0     6195 2023-07-26 22:10:19.305066 libtimed-0.4.4/src/libtimed/transforms.py
+-rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 libtimed-0.4.4/PKG-INFO
```

### Comparing `libtimed-0.4.3/LICENSE` & `libtimed-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.3/README.md` & `libtimed-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.3/pyproject.toml` & `libtimed-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libtimed"
-version = "0.4.3"
+version = "0.4.4"
 description = "Library to intreact with timed webapp."
 authors = [
   "Arthur Deierlein <arthur.deierlein@adfinis.com>",
   "Gian Klug <gian.klug@adfinis.com>",
 ]
 readme = "README.md"
 packages = [{ include = "libtimed", from = "src" }]
```

### Comparing `libtimed-0.4.3/src/libtimed/__init__.py` & `libtimed-0.4.4/src/libtimed/__init__.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.3/src/libtimed/models.py` & `libtimed-0.4.4/src/libtimed/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,14 +255,15 @@
         ("active", None, transforms.Type(bool)),
         ("day", date.today(), transforms.Date),
     ]
 
     attributes = [
         ("from-time", datetime.now(), transforms.Time),
         ("to-time", None, transforms.Time),
+        ("transferred", False, transforms.Type(bool)),
         COMMENT,
         DATE,
         REVIEW,
         NOT_BILLABLE,
     ]
 
     relationships = [
```

### Comparing `libtimed-0.4.3/src/libtimed/oidc.py` & `libtimed-0.4.4/src/libtimed/oidc.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.3/src/libtimed/transforms.py` & `libtimed-0.4.4/src/libtimed/transforms.py`

 * *Files identical despite different names*

### Comparing `libtimed-0.4.3/PKG-INFO` & `libtimed-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libtimed
-Version: 0.4.3
+Version: 0.4.4
 Summary: Library to intreact with timed webapp.
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

