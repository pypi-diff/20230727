# Comparing `tmp/mh-logger-0.0.8.tar.gz` & `tmp/mh-logger-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mh-logger-0.0.8.tar", last modified: Thu Mar 16 21:56:24 2023, max compression
+gzip compressed data, was "mh-logger-0.0.9.tar", last modified: Tue Mar 21 13:34:48 2023, max compression
```

## Comparing `mh-logger-0.0.8.tar` & `mh-logger-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 21:56:24.567347 mh-logger-0.0.8/
--rw-rw-rw-   0        0        0     1078 2023-03-16 15:30:39.000000 mh-logger-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     4236 2023-03-16 21:56:24.568345 mh-logger-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2533 2023-03-16 21:56:01.000000 mh-logger-0.0.8/README.md
--rw-rw-rw-   0        0        0      322 2023-03-16 13:56:00.000000 mh-logger-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      829 2023-03-16 21:56:24.569380 mh-logger-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-03-16 14:55:52.000000 mh-logger-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-16 21:56:24.533264 mh-logger-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-03-16 21:56:24.542270 mh-logger-0.0.8/src/mh_logger/
--rw-rw-rw-   0        0        0       71 2023-03-16 15:01:39.000000 mh-logger-0.0.8/src/mh_logger/__init__.py
--rw-rw-rw-   0        0        0     3130 2023-03-16 21:39:44.000000 mh-logger-0.0.8/src/mh_logger/mh_logger.py
-drwxrwxrwx   0        0        0        0 2023-03-16 21:56:24.565346 mh-logger-0.0.8/src/mh_logger.egg-info/
--rw-rw-rw-   0        0        0     4236 2023-03-16 21:56:24.000000 mh-logger-0.0.8/src/mh_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-03-16 21:56:24.000000 mh-logger-0.0.8/src/mh_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 21:56:24.000000 mh-logger-0.0.8/src/mh_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-03-16 21:56:24.000000 mh-logger-0.0.8/src/mh_logger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-16 21:56:24.000000 mh-logger-0.0.8/src/mh_logger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-21 13:34:48.060733 mh-logger-0.0.9/
+-rw-rw-rw-   0        0        0     1078 2023-03-16 15:30:39.000000 mh-logger-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     4236 2023-03-21 13:34:48.061737 mh-logger-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2533 2023-03-16 21:56:01.000000 mh-logger-0.0.9/README.md
+-rw-rw-rw-   0        0        0      322 2023-03-16 13:56:00.000000 mh-logger-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      829 2023-03-21 13:34:48.063733 mh-logger-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-03-16 14:55:52.000000 mh-logger-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-21 13:34:48.029736 mh-logger-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-03-21 13:34:48.039732 mh-logger-0.0.9/src/mh_logger/
+-rw-rw-rw-   0        0        0       71 2023-03-16 15:01:39.000000 mh-logger-0.0.9/src/mh_logger/__init__.py
+-rw-rw-rw-   0        0        0     3810 2023-03-21 13:32:15.000000 mh-logger-0.0.9/src/mh_logger/mh_logger.py
+drwxrwxrwx   0        0        0        0 2023-03-21 13:34:48.058731 mh-logger-0.0.9/src/mh_logger.egg-info/
+-rw-rw-rw-   0        0        0     4236 2023-03-21 13:34:48.000000 mh-logger-0.0.9/src/mh_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-03-21 13:34:48.000000 mh-logger-0.0.9/src/mh_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-21 13:34:48.000000 mh-logger-0.0.9/src/mh_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-03-21 13:34:48.000000 mh-logger-0.0.9/src/mh_logger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-03-21 13:34:48.000000 mh-logger-0.0.9/src/mh_logger.egg-info/top_level.txt
```

### Comparing `mh-logger-0.0.8/LICENSE.txt` & `mh-logger-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mh-logger-0.0.8/PKG-INFO` & `mh-logger-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mh-logger
-Version: 0.0.8
+Version: 0.0.9
 Summary: MoonHub.ai logging manager to push logs into GCP Cloud Logging
 Home-page: https://github.com/MoonhubTeam/logger
 Author: Ahmed Shahzad
 Author-email: ahmedshahzad141@gmail.com
 Project-URL: Bug Tracker, https://github.com/MoonhubTeam/logger/issues
 Project-URL: repository, https://github.com/MoonhubTeam/logger
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mh-logger-0.0.8/README.md` & `mh-logger-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mh-logger-0.0.8/setup.cfg` & `mh-logger-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 682d 6c6f 6767 6572 0d0a 7665   = mh-logger..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 380d 0a61  rsion = 0.0.8..a
+00000020: 7273 696f 6e20 3d20 302e 302e 390d 0a61  rsion = 0.0.9..a
 00000030: 7574 686f 7220 3d20 4168 6d65 6420 5368  uthor = Ahmed Sh
 00000040: 6168 7a61 640d 0a61 7574 686f 725f 656d  ahzad..author_em
 00000050: 6169 6c20 3d20 6168 6d65 6473 6861 687a  ail = ahmedshahz
 00000060: 6164 3134 3140 676d 6169 6c2e 636f 6d0d  ad141@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 204d  .description = M
 00000080: 6f6f 6e48 7562 2e61 6920 6c6f 6767 696e  oonHub.ai loggin
 00000090: 6720 6d61 6e61 6765 7220 746f 2070 7573  g manager to pus
```

### Comparing `mh-logger-0.0.8/src/mh_logger.egg-info/PKG-INFO` & `mh-logger-0.0.9/src/mh_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mh-logger
-Version: 0.0.8
+Version: 0.0.9
 Summary: MoonHub.ai logging manager to push logs into GCP Cloud Logging
 Home-page: https://github.com/MoonhubTeam/logger
 Author: Ahmed Shahzad
 Author-email: ahmedshahzad141@gmail.com
 Project-URL: Bug Tracker, https://github.com/MoonhubTeam/logger/issues
 Project-URL: repository, https://github.com/MoonhubTeam/logger
 Classifier: Programming Language :: Python :: 3
```

