# Comparing `tmp/sqlwhat-3.8.1.tar.gz` & `tmp/sqlwhat-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlwhat-3.8.1.tar", last modified: Fri Oct 18 11:56:43 2019, max compression
+gzip compressed data, was "dist/sqlwhat-3.9.0.tar", last modified: Thu Jul 27 13:54:53 2023, max compression
```

## Comparing `sqlwhat-3.8.1.tar` & `sqlwhat-3.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-18 11:56:43.000000 sqlwhat-3.8.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2019-10-18 11:55:48.000000 sqlwhat-3.8.1/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-18 11:56:43.000000 sqlwhat-3.8.1/sqlwhat.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4122 2019-10-18 11:56:43.000000 sqlwhat-3.8.1/sqlwhat.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-18 11:56:43.000000 sqlwhat-3.8.1/sqlwhat.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-10-18 11:56:43.000000 sqlwhat-3.8.1/sqlwhat.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      378 2019-10-18 11:56:43.000000 sqlwhat-3.8.1/sqlwhat.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2019-10-18 11:56:43.000000 sqlwhat-3.8.1/sqlwhat.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      192 2019-10-18 11:55:48.000000 sqlwhat-3.8.1/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4122 2019-10-18 11:56:43.000000 sqlwhat-3.8.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2804 2019-10-18 11:55:48.000000 sqlwhat-3.8.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-10-18 11:56:43.000000 sqlwhat-3.8.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    34523 2019-10-18 11:55:48.000000 sqlwhat-3.8.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1658 2019-10-18 11:55:48.000000 sqlwhat-3.8.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-18 11:56:43.000000 sqlwhat-3.8.1/sqlwhat/
--rw-rw-r--   0 travis    (2000) travis    (2000)      973 2019-10-18 11:55:48.000000 sqlwhat-3.8.1/sqlwhat/test_exercise.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-18 11:56:43.000000 sqlwhat-3.8.1/sqlwhat/checks/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7787 2019-10-18 11:55:48.000000 sqlwhat-3.8.1/sqlwhat/checks/has_funcs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12948 2019-10-18 11:55:48.000000 sqlwhat-3.8.1/sqlwhat/checks/check_funcs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      674 2019-10-18 11:55:48.000000 sqlwhat-3.8.1/sqlwhat/checks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2019-10-18 11:55:48.000000 sqlwhat-3.8.1/sqlwhat/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      516 2019-10-18 11:55:48.000000 sqlwhat-3.8.1/sqlwhat/sct_syntax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1521 2019-10-18 11:55:48.000000 sqlwhat-3.8.1/sqlwhat/State.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-27 13:54:53.000000 sqlwhat-3.9.0/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-27 13:54:53.000000 sqlwhat-3.9.0/sqlwhat/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-27 13:54:53.000000 sqlwhat-3.9.0/sqlwhat/checks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2023-07-27 13:23:59.000000 sqlwhat-3.9.0/sqlwhat/checks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12948 2023-07-27 13:23:59.000000 sqlwhat-3.9.0/sqlwhat/checks/check_funcs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7787 2023-07-27 13:23:59.000000 sqlwhat-3.9.0/sqlwhat/checks/has_funcs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1589 2023-07-27 13:23:59.000000 sqlwhat-3.9.0/sqlwhat/State.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       64 2023-07-27 13:54:40.000000 sqlwhat-3.9.0/sqlwhat/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      516 2023-07-27 13:23:59.000000 sqlwhat-3.9.0/sqlwhat/sct_syntax.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      973 2023-07-27 13:23:59.000000 sqlwhat-3.9.0/sqlwhat/test_exercise.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-27 13:54:53.000000 sqlwhat-3.9.0/sqlwhat.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4290 2023-07-27 13:54:52.000000 sqlwhat-3.9.0/sqlwhat.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-07-27 13:54:52.000000 sqlwhat-3.9.0/sqlwhat.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-27 13:54:52.000000 sqlwhat-3.9.0/sqlwhat.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2023-07-27 13:54:52.000000 sqlwhat-3.9.0/sqlwhat.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-07-27 13:54:52.000000 sqlwhat-3.9.0/sqlwhat.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34523 2023-07-27 13:23:59.000000 sqlwhat-3.9.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2023-07-27 13:23:59.000000 sqlwhat-3.9.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2948 2023-07-27 13:23:59.000000 sqlwhat-3.9.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      158 2023-07-27 13:23:59.000000 sqlwhat-3.9.0/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1658 2023-07-27 13:23:59.000000 sqlwhat-3.9.0/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4290 2023-07-27 13:54:53.000000 sqlwhat-3.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-27 13:54:53.000000 sqlwhat-3.9.0/setup.cfg
```

### Comparing `sqlwhat-3.8.1/sqlwhat.egg-info/PKG-INFO` & `sqlwhat-3.9.0/sqlwhat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: sqlwhat
-Version: 3.8.1
+Version: 3.9.0
 Summary: Submission correctness tests for SQL
 Home-page: https://github.com/datacamp/sqlwhat
 Author: Michael Chow, Filip Schouwenaars
 Author-email: michael@datacamp.com
 Maintainer: Jeroen Hermans
 Maintainer-email: content-engineering@datacamp.com
 License: UNKNOWN
-Description: # sqlwhat
+Description: > :warning: **This repo has outdated tokens in its travisci config** 
+        > To make new releases for this project it needs to be moved to circleci
+        
+        # sqlwhat
         
         [![Build Status](https://travis-ci.org/datacamp/sqlwhat.svg?branch=master)](https://travis-ci.org/datacamp/sqlwhat)
         [![codecov](https://codecov.io/gh/datacamp/sqlwhat/branch/master/graph/badge.svg)](https://codecov.io/gh/datacamp/sqlwhat)
         [![PyPI version](https://badge.fury.io/py/sqlwhat.svg)](https://badge.fury.io/py/sqlwhat)
         
         `sqlwhat` enables you to write Submission Correctness Tests (SCTs) for interactive SQL exercises on DataCamp.
```

### Comparing `sqlwhat-3.8.1/PKG-INFO` & `sqlwhat-3.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: sqlwhat
-Version: 3.8.1
+Version: 3.9.0
 Summary: Submission correctness tests for SQL
 Home-page: https://github.com/datacamp/sqlwhat
 Author: Michael Chow, Filip Schouwenaars
 Author-email: michael@datacamp.com
 Maintainer: Jeroen Hermans
 Maintainer-email: content-engineering@datacamp.com
 License: UNKNOWN
-Description: # sqlwhat
+Description: > :warning: **This repo has outdated tokens in its travisci config** 
+        > To make new releases for this project it needs to be moved to circleci
+        
+        # sqlwhat
         
         [![Build Status](https://travis-ci.org/datacamp/sqlwhat.svg?branch=master)](https://travis-ci.org/datacamp/sqlwhat)
         [![codecov](https://codecov.io/gh/datacamp/sqlwhat/branch/master/graph/badge.svg)](https://codecov.io/gh/datacamp/sqlwhat)
         [![PyPI version](https://badge.fury.io/py/sqlwhat.svg)](https://badge.fury.io/py/sqlwhat)
         
         `sqlwhat` enables you to write Submission Correctness Tests (SCTs) for interactive SQL exercises on DataCamp.
```

### Comparing `sqlwhat-3.8.1/README.md` & `sqlwhat-3.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+> :warning: **This repo has outdated tokens in its travisci config** 
+> To make new releases for this project it needs to be moved to circleci
+
 # sqlwhat
 
 [![Build Status](https://travis-ci.org/datacamp/sqlwhat.svg?branch=master)](https://travis-ci.org/datacamp/sqlwhat)
 [![codecov](https://codecov.io/gh/datacamp/sqlwhat/branch/master/graph/badge.svg)](https://codecov.io/gh/datacamp/sqlwhat)
 [![PyPI version](https://badge.fury.io/py/sqlwhat.svg)](https://badge.fury.io/py/sqlwhat)
 
 `sqlwhat` enables you to write Submission Correctness Tests (SCTs) for interactive SQL exercises on DataCamp.
```

### Comparing `sqlwhat-3.8.1/LICENSE` & `sqlwhat-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.8.1/setup.py` & `sqlwhat-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.8.1/sqlwhat/test_exercise.py` & `sqlwhat-3.9.0/sqlwhat/test_exercise.py`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.8.1/sqlwhat/checks/has_funcs.py` & `sqlwhat-3.9.0/sqlwhat/checks/has_funcs.py`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.8.1/sqlwhat/checks/check_funcs.py` & `sqlwhat-3.9.0/sqlwhat/checks/check_funcs.py`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.8.1/sqlwhat/checks/__init__.py` & `sqlwhat-3.9.0/sqlwhat/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.8.1/sqlwhat/sct_syntax.py` & `sqlwhat-3.9.0/sqlwhat/sct_syntax.py`

 * *Files identical despite different names*

### Comparing `sqlwhat-3.8.1/sqlwhat/State.py` & `sqlwhat-3.9.0/sqlwhat/State.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from functools import wraps
 
 PARSER_MODULES = {
     "postgresql": "antlr_plsql.ast",
     "sqlite": "antlr_plsql.ast",  # uses postgres parser for now
     "oracle": "antlr_plsql.ast",  # uses postgres parser for now
     "mssql": "antlr_tsql.ast",
+    "snowflake": "antlr_plsql.ast",  # uses postgres parser for now
 }
 
 
 def lower_case(f):
     """Decorator specifically for turning mssql AST into lowercase"""
     # if it has already been wrapped, we return original
     if hasattr(f, "lower_cased"):
```

