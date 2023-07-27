# Comparing `tmp/gitstats_abilian-1.0.1.tar.gz` & `tmp/gitstats_abilian-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitstats_abilian-1.0.1.tar", max compression
+gzip compressed data, was "gitstats_abilian-1.0.2.tar", max compression
```

## Comparing `gitstats_abilian-1.0.1.tar` & `gitstats_abilian-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      538 2023-07-27 07:37:58.402981 gitstats_abilian-1.0.1/README.md
--rw-r--r--   0        0        0      380 2023-07-27 07:46:12.881172 gitstats_abilian-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 06:49:17.000000 gitstats_abilian-1.0.1/src/gitstats/__init__.py
--rw-r--r--   0        0        0       73 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.1/src/gitstats/assets/arrow-down.gif
--rw-r--r--   0        0        0       71 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.1/src/gitstats/assets/arrow-none.gif
--rw-r--r--   0        0        0       73 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.1/src/gitstats/assets/arrow-up.gif
--rw-r--r--   0        0        0     1645 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.1/src/gitstats/assets/gitstats.css
--rw-r--r--   0        0        0     9562 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.1/src/gitstats/assets/sortable.js
--rw-r--r--   0        0        0    25782 2023-07-27 07:50:14.780678 gitstats_abilian-1.0.1/src/gitstats/collector.py
--rw-r--r--   0        0        0      821 2023-07-27 07:48:16.895377 gitstats_abilian-1.0.1/src/gitstats/config.py
--rwxr-xr-x   0        0        0     2954 2023-07-27 07:44:44.644294 gitstats_abilian-1.0.1/src/gitstats/gitstats.py
--rw-r--r--   0        0        0      140 2023-07-27 07:26:27.359393 gitstats_abilian-1.0.1/src/gitstats/main.py
--rw-r--r--   0        0        0    30085 2023-07-27 07:44:44.667624 gitstats_abilian-1.0.1/src/gitstats/report.py
--rw-r--r--   0        0        0     3313 2023-07-27 07:45:48.884403 gitstats_abilian-1.0.1/src/gitstats/utils.py
--rw-r--r--   0        0        0      665 2023-07-27 07:44:44.671845 gitstats_abilian-1.0.1/src/gitstats/version.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 gitstats_abilian-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      545 2023-07-27 07:55:17.912726 gitstats_abilian-1.0.2/README.md
+-rw-r--r--   0        0        0      380 2023-07-27 07:55:25.162376 gitstats_abilian-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 06:49:17.000000 gitstats_abilian-1.0.2/src/gitstats/__init__.py
+-rw-r--r--   0        0        0       73 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.2/src/gitstats/assets/arrow-down.gif
+-rw-r--r--   0        0        0       71 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.2/src/gitstats/assets/arrow-none.gif
+-rw-r--r--   0        0        0       73 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.2/src/gitstats/assets/arrow-up.gif
+-rw-r--r--   0        0        0     1645 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.2/src/gitstats/assets/gitstats.css
+-rw-r--r--   0        0        0     9562 2023-07-27 06:45:33.000000 gitstats_abilian-1.0.2/src/gitstats/assets/sortable.js
+-rw-r--r--   0        0        0    25782 2023-07-27 07:50:14.780678 gitstats_abilian-1.0.2/src/gitstats/collector.py
+-rw-r--r--   0        0        0      821 2023-07-27 07:48:16.895377 gitstats_abilian-1.0.2/src/gitstats/config.py
+-rwxr-xr-x   0        0        0     2954 2023-07-27 07:44:44.644294 gitstats_abilian-1.0.2/src/gitstats/gitstats.py
+-rw-r--r--   0        0        0      140 2023-07-27 07:26:27.359393 gitstats_abilian-1.0.2/src/gitstats/main.py
+-rw-r--r--   0        0        0    30085 2023-07-27 07:44:44.667624 gitstats_abilian-1.0.2/src/gitstats/report.py
+-rw-r--r--   0        0        0     3313 2023-07-27 07:45:48.884403 gitstats_abilian-1.0.2/src/gitstats/utils.py
+-rw-r--r--   0        0        0      665 2023-07-27 07:44:44.671845 gitstats_abilian-1.0.2/src/gitstats/version.py
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 gitstats_abilian-1.0.2/PKG-INFO
```

### Comparing `gitstats_abilian-1.0.1/README.md` & `gitstats_abilian-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ```shell
 pip install gitstats-abilian
 ```
 
 or 
 
 ```shell
-pip install git-stats
+pip install gitstats-abilian
 ```
 
 ## usage
 
 ```shell
 gitstats <git-repo> <output-dir>
 ```
```

### Comparing `gitstats_abilian-1.0.1/src/gitstats/assets/gitstats.css` & `gitstats_abilian-1.0.2/src/gitstats/assets/gitstats.css`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.1/src/gitstats/assets/sortable.js` & `gitstats_abilian-1.0.2/src/gitstats/assets/sortable.js`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.1/src/gitstats/collector.py` & `gitstats_abilian-1.0.2/src/gitstats/collector.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.1/src/gitstats/config.py` & `gitstats_abilian-1.0.2/src/gitstats/config.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.1/src/gitstats/gitstats.py` & `gitstats_abilian-1.0.2/src/gitstats/gitstats.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.1/src/gitstats/report.py` & `gitstats_abilian-1.0.2/src/gitstats/report.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.1/src/gitstats/utils.py` & `gitstats_abilian-1.0.2/src/gitstats/utils.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.1/src/gitstats/version.py` & `gitstats_abilian-1.0.2/src/gitstats/version.py`

 * *Files identical despite different names*

### Comparing `gitstats_abilian-1.0.1/PKG-INFO` & `gitstats_abilian-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitstats-abilian
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,15 +23,15 @@
 ```shell
 pip install gitstats-abilian
 ```
 
 or 
 
 ```shell
-pip install git-stats
+pip install gitstats-abilian
 ```
 
 ## usage
 
 ```shell
 gitstats <git-repo> <output-dir>
 ```
```

