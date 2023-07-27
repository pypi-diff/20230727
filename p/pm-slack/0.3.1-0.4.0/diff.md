# Comparing `tmp/pm_slack-0.3.1.tar.gz` & `tmp/pm_slack-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm_slack-0.3.1.tar", max compression
+gzip compressed data, was "pm_slack-0.4.0.tar", max compression
```

## Comparing `pm_slack-0.3.1.tar` & `pm_slack-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1078 2023-05-25 09:25:16.560981 pm_slack-0.3.1/LICENSE
--rw-r--r--   0        0        0       45 2023-05-25 09:25:16.560981 pm_slack-0.3.1/README.md
--rw-r--r--   0        0        0       76 2023-05-25 09:25:16.560981 pm_slack-0.3.1/pm_slack/__init__.py
--rw-r--r--   0        0        0     1064 2023-05-25 09:25:16.560981 pm_slack-0.3.1/pm_slack/main.py
--rw-r--r--   0        0        0        0 2023-05-25 09:25:16.560981 pm_slack-0.3.1/pm_slack/py.typed
--rw-r--r--   0        0        0     1079 2023-05-25 09:25:16.560981 pm_slack-0.3.1/pm_slack/templates/__init__.py
--rw-r--r--   0        0        0    21356 2023-05-25 09:25:16.560981 pm_slack-0.3.1/pm_slack/templates/_templates.py
--rw-r--r--   0        0        0     1107 2023-05-25 09:25:44.417058 pm_slack-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 pm_slack-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-27 11:16:37.077473 pm_slack-0.4.0/LICENSE
+-rw-r--r--   0        0        0       45 2023-07-27 11:16:37.077473 pm_slack-0.4.0/README.md
+-rw-r--r--   0        0        0       76 2023-07-27 11:16:37.077473 pm_slack-0.4.0/pm_slack/__init__.py
+-rw-r--r--   0        0        0       40 2023-07-27 11:16:37.077473 pm_slack-0.4.0/pm_slack/constants.py
+-rw-r--r--   0        0        0     2413 2023-07-27 11:16:37.077473 pm_slack-0.4.0/pm_slack/main.py
+-rw-r--r--   0        0        0        0 2023-07-27 11:16:37.077473 pm_slack-0.4.0/pm_slack/py.typed
+-rw-r--r--   0        0        0     1079 2023-07-27 11:16:37.077473 pm_slack-0.4.0/pm_slack/templates/__init__.py
+-rw-r--r--   0        0        0    21356 2023-07-27 11:16:37.077473 pm_slack-0.4.0/pm_slack/templates/_templates.py
+-rw-r--r--   0        0        0     1107 2023-07-27 11:17:05.201936 pm_slack-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 pm_slack-0.4.0/PKG-INFO
```

### Comparing `pm_slack-0.3.1/LICENSE` & `pm_slack-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pm_slack-0.3.1/pm_slack/templates/__init__.py` & `pm_slack-0.4.0/pm_slack/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pm_slack-0.3.1/pm_slack/templates/_templates.py` & `pm_slack-0.4.0/pm_slack/templates/_templates.py`

 * *Files identical despite different names*

### Comparing `pm_slack-0.3.1/pyproject.toml` & `pm_slack-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pm_slack"
-version = "0.3.1"
+version = "0.4.0"
 description = "A Slack Library for Paket Mutfak"
 authors = ["Paket Mutfak Dev Team <dev@paketmutfak.com.tr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pm_slack-0.3.1/PKG-INFO` & `pm_slack-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm-slack
-Version: 0.3.1
+Version: 0.4.0
 Summary: A Slack Library for Paket Mutfak
 License: MIT
 Author: Paket Mutfak Dev Team
 Author-email: dev@paketmutfak.com.tr
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

