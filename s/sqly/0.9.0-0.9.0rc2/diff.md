# Comparing `tmp/sqly-0.9.0.tar.gz` & `tmp/sqly-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqly-0.9.0.tar", last modified: Wed Jul 26 23:58:10 2023, max compression
+gzip compressed data, was "sqly-0.9.0rc2.tar", last modified: Wed Jul 26 23:01:33 2023, max compression
```

## Comparing `sqly-0.9.0.tar` & `sqly-0.9.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:58:10.328876 sqly-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 23:58:08.000000 sqly-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-26 23:58:08.000000 sqly-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-26 23:58:10.328876 sqly-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-26 23:58:08.000000 sqly-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-26 23:58:10.328876 sqly-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-26 23:58:08.000000 sqly-0.9.0/setup.json
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-26 23:58:08.000000 sqly-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:58:10.328876 sqly-0.9.0/sqly/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 23:58:08.000000 sqly-0.9.0/sqly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-26 23:58:08.000000 sqly-0.9.0/sqly/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-26 23:58:08.000000 sqly-0.9.0/sqly/dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-26 23:58:08.000000 sqly-0.9.0/sqly/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-07-26 23:58:08.000000 sqly-0.9.0/sqly/migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:58:10.328876 sqly-0.9.0/sqly/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-26 23:58:08.000000 sqly-0.9.0/sqly/migrations/20211105034808482_init.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-26 23:58:08.000000 sqly-0.9.0/sqly/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-26 23:58:08.000000 sqly-0.9.0/sqly/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-07-26 23:58:08.000000 sqly-0.9.0/sqly/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:58:10.328876 sqly-0.9.0/sqly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-26 23:58:10.000000 sqly-0.9.0/sqly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-26 23:58:10.000000 sqly-0.9.0/sqly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:58:10.000000 sqly-0.9.0/sqly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 23:58:10.000000 sqly-0.9.0/sqly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-26 23:58:10.000000 sqly-0.9.0/sqly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 23:58:10.000000 sqly-0.9.0/sqly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:58:10.328876 sqly-0.9.0/testapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 23:58:08.000000 sqly-0.9.0/testapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-26 23:01:32.000000 sqly-0.9.0rc2/setup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/sqly/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/sqly/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/migrations/20211105034808482_init.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/sqly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-26 23:01:33.000000 sqly-0.9.0rc2/sqly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-26 23:01:33.000000 sqly-0.9.0rc2/sqly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:01:33.000000 sqly-0.9.0rc2/sqly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 23:01:33.000000 sqly-0.9.0rc2/sqly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-26 23:01:33.000000 sqly-0.9.0rc2/sqly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 23:01:33.000000 sqly-0.9.0rc2/sqly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/testapp/__init__.py
```

### Comparing `sqly-0.9.0/LICENSE` & `sqly-0.9.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqly-0.9.0/PKG-INFO` & `sqly-0.9.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqly
-Version: 0.9.0
+Version: 0.9.0rc2
 Summary: Write SQL in SQL
 Home-page: https://github.com/kruxia/sqly
 Author: Sean Harrison
 Author-email: sah@kruxia.com
 License: MPL 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sqly-0.9.0/README.md` & `sqly-0.9.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `sqly-0.9.0/setup.json` & `sqly-0.9.0rc2/setup.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.9.0rc2'"}*

```diff
@@ -17,9 +17,9 @@
     "license": "MPL 2.0",
     "name": "sqly",
     "package_data": {
         "": []
     },
     "scripts": [],
     "url": "https://github.com/kruxia/sqly",
-    "version": "0.9.0"
+    "version": "0.9.0rc2"
 }
```

### Comparing `sqly-0.9.0/setup.py` & `sqly-0.9.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `sqly-0.9.0/sqly/__main__.py` & `sqly-0.9.0rc2/sqly/__main__.py`

 * *Files identical despite different names*

### Comparing `sqly-0.9.0/sqly/dialect.py` & `sqly-0.9.0rc2/sqly/dialect.py`

 * *Files identical despite different names*

### Comparing `sqly-0.9.0/sqly/migration.py` & `sqly-0.9.0rc2/sqly/migration.py`

 * *Files identical despite different names*

### Comparing `sqly-0.9.0/sqly/migrations/20211105034808482_init.yaml` & `sqly-0.9.0rc2/sqly/migrations/20211105034808482_init.yaml`

 * *Files identical despite different names*

### Comparing `sqly-0.9.0/sqly/queries.py` & `sqly-0.9.0rc2/sqly/queries.py`

 * *Files identical despite different names*

### Comparing `sqly-0.9.0/sqly/query.py` & `sqly-0.9.0rc2/sqly/query.py`

 * *Files identical despite different names*

### Comparing `sqly-0.9.0/sqly/sql.py` & `sqly-0.9.0rc2/sqly/sql.py`

 * *Files identical despite different names*

### Comparing `sqly-0.9.0/sqly.egg-info/PKG-INFO` & `sqly-0.9.0rc2/sqly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqly
-Version: 0.9.0
+Version: 0.9.0rc2
 Summary: Write SQL in SQL
 Home-page: https://github.com/kruxia/sqly
 Author: Sean Harrison
 Author-email: sah@kruxia.com
 License: MPL 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

