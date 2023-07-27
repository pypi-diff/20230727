# Comparing `tmp/xtb_broker-0.0.8.tar.gz` & `tmp/xtb_broker-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtb_broker-0.0.8.tar", last modified: Thu Jul 27 17:01:32 2023, max compression
+gzip compressed data, was "xtb_broker-0.0.9.tar", last modified: Thu Jul 27 17:05:33 2023, max compression
```

## Comparing `xtb_broker-0.0.8.tar` & `xtb_broker-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/PKG-INFO
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      453 2023-07-21 09:26:18.000000 xtb_broker-0.0.8/README.md
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      516 2023-07-20 21:52:23.000000 xtb_broker-0.0.8/pyproject.toml
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       38 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/setup.cfg
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      397 2023-07-27 17:01:08.000000 xtb_broker-0.0.8/setup.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/xtb_broker/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.8/xtb_broker/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)    12091 2023-07-21 09:26:18.000000 xtb_broker-0.0.8/xtb_broker/client.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/xtb_broker/config/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.8/xtb_broker/config/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2065 2023-05-20 14:31:15.000000 xtb_broker-0.0.8/xtb_broker/config/constants.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1702 2023-05-20 13:45:08.000000 xtb_broker-0.0.8/xtb_broker/config/exception.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      697 2023-07-21 09:26:18.000000 xtb_broker-0.0.8/xtb_broker/config/frozen.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      285 2023-07-21 09:26:18.000000 xtb_broker-0.0.8/xtb_broker/config/logger.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/xtb_broker/models/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.8/xtb_broker/models/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     5996 2023-07-21 09:26:28.000000 xtb_broker-0.0.8/xtb_broker/models/arbitrage.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2178 2023-07-21 09:26:28.000000 xtb_broker-0.0.8/xtb_broker/models/position.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      579 2023-07-21 09:26:18.000000 xtb_broker-0.0.8/xtb_broker/models/shift.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2638 2023-07-27 17:01:08.000000 xtb_broker-0.0.8/xtb_broker/models/symbol.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1247 2023-07-27 17:01:08.000000 xtb_broker-0.0.8/xtb_broker/models/tick.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1816 2023-07-21 09:26:28.000000 xtb_broker-0.0.8/xtb_broker/models/timetable.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6479 2023-07-27 17:01:08.000000 xtb_broker-0.0.8/xtb_broker/models/trade.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1816 2023-07-21 09:26:18.000000 xtb_broker-0.0.8/xtb_broker/models/transaction.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      649 2023-05-20 13:45:08.000000 xtb_broker-0.0.8/xtb_broker/utils.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2535 2023-07-22 11:42:12.000000 xtb_broker-0.0.8/xtb_broker/xtb.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:01:32.081251 xtb_broker-0.0.8/xtb_broker.egg-info/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-27 17:01:32.000000 xtb_broker-0.0.8/xtb_broker.egg-info/PKG-INFO
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      662 2023-07-27 17:01:32.000000 xtb_broker-0.0.8/xtb_broker.egg-info/SOURCES.txt
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        1 2023-07-27 17:01:32.000000 xtb_broker-0.0.8/xtb_broker.egg-info/dependency_links.txt
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       11 2023-07-27 17:01:32.000000 xtb_broker-0.0.8/xtb_broker.egg-info/top_level.txt
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:05:33.331124 xtb_broker-0.0.9/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-27 17:05:33.331124 xtb_broker-0.0.9/PKG-INFO
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      453 2023-07-21 09:26:18.000000 xtb_broker-0.0.9/README.md
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      516 2023-07-20 21:52:23.000000 xtb_broker-0.0.9/pyproject.toml
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       38 2023-07-27 17:05:33.331124 xtb_broker-0.0.9/setup.cfg
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      397 2023-07-27 17:05:30.000000 xtb_broker-0.0.9/setup.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:05:33.327124 xtb_broker-0.0.9/xtb_broker/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.9/xtb_broker/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)    12091 2023-07-21 09:26:18.000000 xtb_broker-0.0.9/xtb_broker/client.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:05:33.327124 xtb_broker-0.0.9/xtb_broker/config/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.9/xtb_broker/config/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2065 2023-05-20 14:31:15.000000 xtb_broker-0.0.9/xtb_broker/config/constants.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1702 2023-05-20 13:45:08.000000 xtb_broker-0.0.9/xtb_broker/config/exception.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      697 2023-07-21 09:26:18.000000 xtb_broker-0.0.9/xtb_broker/config/frozen.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      285 2023-07-21 09:26:18.000000 xtb_broker-0.0.9/xtb_broker/config/logger.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:05:33.331124 xtb_broker-0.0.9/xtb_broker/models/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.9/xtb_broker/models/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     5996 2023-07-21 09:26:28.000000 xtb_broker-0.0.9/xtb_broker/models/arbitrage.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2178 2023-07-21 09:26:28.000000 xtb_broker-0.0.9/xtb_broker/models/position.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      579 2023-07-21 09:26:18.000000 xtb_broker-0.0.9/xtb_broker/models/shift.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2638 2023-07-27 17:01:08.000000 xtb_broker-0.0.9/xtb_broker/models/symbol.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1247 2023-07-27 17:01:08.000000 xtb_broker-0.0.9/xtb_broker/models/tick.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1816 2023-07-21 09:26:28.000000 xtb_broker-0.0.9/xtb_broker/models/timetable.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6479 2023-07-27 17:01:08.000000 xtb_broker-0.0.9/xtb_broker/models/trade.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1816 2023-07-21 09:26:18.000000 xtb_broker-0.0.9/xtb_broker/models/transaction.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      649 2023-05-20 13:45:08.000000 xtb_broker-0.0.9/xtb_broker/utils.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2535 2023-07-22 11:42:12.000000 xtb_broker-0.0.9/xtb_broker/xtb.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-27 17:05:33.327124 xtb_broker-0.0.9/xtb_broker.egg-info/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-27 17:05:33.000000 xtb_broker-0.0.9/xtb_broker.egg-info/PKG-INFO
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      662 2023-07-27 17:05:33.000000 xtb_broker-0.0.9/xtb_broker.egg-info/SOURCES.txt
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        1 2023-07-27 17:05:33.000000 xtb_broker-0.0.9/xtb_broker.egg-info/dependency_links.txt
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       11 2023-07-27 17:05:33.000000 xtb_broker-0.0.9/xtb_broker.egg-info/top_level.txt
```

### Comparing `xtb_broker-0.0.8/pyproject.toml` & `xtb_broker-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/client.py` & `xtb_broker-0.0.9/xtb_broker/client.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/config/constants.py` & `xtb_broker-0.0.9/xtb_broker/config/constants.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/config/exception.py` & `xtb_broker-0.0.9/xtb_broker/config/exception.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/config/frozen.py` & `xtb_broker-0.0.9/xtb_broker/config/frozen.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/models/arbitrage.py` & `xtb_broker-0.0.9/xtb_broker/models/arbitrage.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/models/position.py` & `xtb_broker-0.0.9/xtb_broker/models/position.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/models/shift.py` & `xtb_broker-0.0.9/xtb_broker/models/shift.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/models/symbol.py` & `xtb_broker-0.0.9/xtb_broker/models/symbol.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/models/tick.py` & `xtb_broker-0.0.9/xtb_broker/models/tick.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/models/timetable.py` & `xtb_broker-0.0.9/xtb_broker/models/timetable.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/models/trade.py` & `xtb_broker-0.0.9/xtb_broker/models/trade.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/models/transaction.py` & `xtb_broker-0.0.9/xtb_broker/models/transaction.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/utils.py` & `xtb_broker-0.0.9/xtb_broker/utils.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker/xtb.py` & `xtb_broker-0.0.9/xtb_broker/xtb.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.8/xtb_broker.egg-info/SOURCES.txt` & `xtb_broker-0.0.9/xtb_broker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

