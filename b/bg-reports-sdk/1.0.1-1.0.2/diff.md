# Comparing `tmp/bg_reports_sdk-1.0.1.tar.gz` & `tmp/bg_reports_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bg_reports_sdk-1.0.1.tar", last modified: Thu Jul 27 10:24:23 2023, max compression
+gzip compressed data, was "bg_reports_sdk-1.0.2.tar", last modified: Thu Jul 27 10:26:43 2023, max compression
```

## Comparing `bg_reports_sdk-1.0.1.tar` & `bg_reports_sdk-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 nikitasurov   (501) staff       (20)        0 2023-07-27 10:24:23.680207 bg_reports_sdk-1.0.1/
--rw-r--r--   0 nikitasurov   (501) staff       (20)      251 2023-07-27 10:24:23.680078 bg_reports_sdk-1.0.1/PKG-INFO
-drwxr-xr-x   0 nikitasurov   (501) staff       (20)        0 2023-07-27 10:24:23.677565 bg_reports_sdk-1.0.1/bg_reports_sdk/
--rw-r--r--   0 nikitasurov   (501) staff       (20)        0 2023-07-27 09:46:59.000000 bg_reports_sdk-1.0.1/bg_reports_sdk/__init__.py
--rw-r--r--   0 nikitasurov   (501) staff       (20)      177 2023-07-26 10:17:47.000000 bg_reports_sdk-1.0.1/bg_reports_sdk/config.py
-drwxr-xr-x   0 nikitasurov   (501) staff       (20)        0 2023-07-27 10:24:23.678623 bg_reports_sdk-1.0.1/bg_reports_sdk/data_provider/
--rw-r--r--   0 nikitasurov   (501) staff       (20)        0 2023-07-20 14:19:03.000000 bg_reports_sdk-1.0.1/bg_reports_sdk/data_provider/__init__.py
--rw-r--r--   0 nikitasurov   (501) staff       (20)     6763 2023-07-27 10:24:12.000000 bg_reports_sdk-1.0.1/bg_reports_sdk/data_provider/data_provider.py
-drwxr-xr-x   0 nikitasurov   (501) staff       (20)        0 2023-07-27 10:24:23.678929 bg_reports_sdk-1.0.1/bg_reports_sdk/report_executor/
--rw-r--r--   0 nikitasurov   (501) staff       (20)        0 2023-07-19 08:33:47.000000 bg_reports_sdk-1.0.1/bg_reports_sdk/report_executor/__init__.py
--rw-r--r--   0 nikitasurov   (501) staff       (20)     9288 2023-07-27 10:23:39.000000 bg_reports_sdk-1.0.1/bg_reports_sdk/report_executor/report_executor.py
-drwxr-xr-x   0 nikitasurov   (501) staff       (20)        0 2023-07-27 10:24:23.679779 bg_reports_sdk-1.0.1/bg_reports_sdk/scheduler_manager/
--rw-r--r--   0 nikitasurov   (501) staff       (20)        0 2023-07-19 09:45:55.000000 bg_reports_sdk-1.0.1/bg_reports_sdk/scheduler_manager/__init__.py
--rw-r--r--   0 nikitasurov   (501) staff       (20)     1372 2023-07-21 11:27:27.000000 bg_reports_sdk-1.0.1/bg_reports_sdk/scheduler_manager/scheduler.py
--rw-r--r--   0 nikitasurov   (501) staff       (20)    10343 2023-07-27 10:23:52.000000 bg_reports_sdk-1.0.1/bg_reports_sdk/scheduler_manager/scheduler_manager.py
-drwxr-xr-x   0 nikitasurov   (501) staff       (20)        0 2023-07-27 10:24:23.678411 bg_reports_sdk-1.0.1/bg_reports_sdk.egg-info/
--rw-r--r--   0 nikitasurov   (501) staff       (20)      251 2023-07-27 10:24:23.000000 bg_reports_sdk-1.0.1/bg_reports_sdk.egg-info/PKG-INFO
--rw-r--r--   0 nikitasurov   (501) staff       (20)      574 2023-07-27 10:24:23.000000 bg_reports_sdk-1.0.1/bg_reports_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 nikitasurov   (501) staff       (20)        1 2023-07-27 10:24:23.000000 bg_reports_sdk-1.0.1/bg_reports_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 nikitasurov   (501) staff       (20)       28 2023-07-27 10:24:23.000000 bg_reports_sdk-1.0.1/bg_reports_sdk.egg-info/requires.txt
--rw-r--r--   0 nikitasurov   (501) staff       (20)       15 2023-07-27 10:24:23.000000 bg_reports_sdk-1.0.1/bg_reports_sdk.egg-info/top_level.txt
--rw-r--r--   0 nikitasurov   (501) staff       (20)       38 2023-07-27 10:24:23.680250 bg_reports_sdk-1.0.1/setup.cfg
--rw-r--r--   0 nikitasurov   (501) staff       (20)      393 2023-07-27 10:24:20.000000 bg_reports_sdk-1.0.1/setup.py
+drwxr-xr-x   0 nikitasurov   (501) staff       (20)        0 2023-07-27 10:26:43.695070 bg_reports_sdk-1.0.2/
+-rw-r--r--   0 nikitasurov   (501) staff       (20)      251 2023-07-27 10:26:43.694569 bg_reports_sdk-1.0.2/PKG-INFO
+drwxr-xr-x   0 nikitasurov   (501) staff       (20)        0 2023-07-27 10:26:43.692616 bg_reports_sdk-1.0.2/bg_reports_sdk/
+-rw-r--r--   0 nikitasurov   (501) staff       (20)        0 2023-07-27 09:46:59.000000 bg_reports_sdk-1.0.2/bg_reports_sdk/__init__.py
+-rw-r--r--   0 nikitasurov   (501) staff       (20)      177 2023-07-26 10:17:47.000000 bg_reports_sdk-1.0.2/bg_reports_sdk/config.py
+drwxr-xr-x   0 nikitasurov   (501) staff       (20)        0 2023-07-27 10:26:43.693786 bg_reports_sdk-1.0.2/bg_reports_sdk/data_provider/
+-rw-r--r--   0 nikitasurov   (501) staff       (20)        0 2023-07-20 14:19:03.000000 bg_reports_sdk-1.0.2/bg_reports_sdk/data_provider/__init__.py
+-rw-r--r--   0 nikitasurov   (501) staff       (20)     6763 2023-07-27 10:24:12.000000 bg_reports_sdk-1.0.2/bg_reports_sdk/data_provider/data_provider.py
+drwxr-xr-x   0 nikitasurov   (501) staff       (20)        0 2023-07-27 10:26:43.694011 bg_reports_sdk-1.0.2/bg_reports_sdk/report_executor/
+-rw-r--r--   0 nikitasurov   (501) staff       (20)        0 2023-07-19 08:33:47.000000 bg_reports_sdk-1.0.2/bg_reports_sdk/report_executor/__init__.py
+-rw-r--r--   0 nikitasurov   (501) staff       (20)     9303 2023-07-27 10:26:25.000000 bg_reports_sdk-1.0.2/bg_reports_sdk/report_executor/report_executor.py
+drwxr-xr-x   0 nikitasurov   (501) staff       (20)        0 2023-07-27 10:26:43.694349 bg_reports_sdk-1.0.2/bg_reports_sdk/scheduler_manager/
+-rw-r--r--   0 nikitasurov   (501) staff       (20)        0 2023-07-19 09:45:55.000000 bg_reports_sdk-1.0.2/bg_reports_sdk/scheduler_manager/__init__.py
+-rw-r--r--   0 nikitasurov   (501) staff       (20)     1372 2023-07-21 11:27:27.000000 bg_reports_sdk-1.0.2/bg_reports_sdk/scheduler_manager/scheduler.py
+-rw-r--r--   0 nikitasurov   (501) staff       (20)    10358 2023-07-27 10:26:13.000000 bg_reports_sdk-1.0.2/bg_reports_sdk/scheduler_manager/scheduler_manager.py
+drwxr-xr-x   0 nikitasurov   (501) staff       (20)        0 2023-07-27 10:26:43.693518 bg_reports_sdk-1.0.2/bg_reports_sdk.egg-info/
+-rw-r--r--   0 nikitasurov   (501) staff       (20)      251 2023-07-27 10:26:43.000000 bg_reports_sdk-1.0.2/bg_reports_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 nikitasurov   (501) staff       (20)      574 2023-07-27 10:26:43.000000 bg_reports_sdk-1.0.2/bg_reports_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 nikitasurov   (501) staff       (20)        1 2023-07-27 10:26:43.000000 bg_reports_sdk-1.0.2/bg_reports_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 nikitasurov   (501) staff       (20)       28 2023-07-27 10:26:43.000000 bg_reports_sdk-1.0.2/bg_reports_sdk.egg-info/requires.txt
+-rw-r--r--   0 nikitasurov   (501) staff       (20)       15 2023-07-27 10:26:43.000000 bg_reports_sdk-1.0.2/bg_reports_sdk.egg-info/top_level.txt
+-rw-r--r--   0 nikitasurov   (501) staff       (20)       38 2023-07-27 10:26:43.695399 bg_reports_sdk-1.0.2/setup.cfg
+-rw-r--r--   0 nikitasurov   (501) staff       (20)      393 2023-07-27 10:26:34.000000 bg_reports_sdk-1.0.2/setup.py
```

### Comparing `bg_reports_sdk-1.0.1/bg_reports_sdk/data_provider/data_provider.py` & `bg_reports_sdk-1.0.2/bg_reports_sdk/data_provider/data_provider.py`

 * *Files identical despite different names*

### Comparing `bg_reports_sdk-1.0.1/bg_reports_sdk/report_executor/report_executor.py` & `bg_reports_sdk-1.0.2/bg_reports_sdk/report_executor/report_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from time import sleep
 
 import pytz
 import requests
 from bg_reports_sdk.data_provider.data_provider import DataProvider
 from bg_reports_sdk.scheduler_manager.scheduler_manager import SchedulerManager
 
-from config import *
+from bg_reports_sdk.config import *
 
 
 class ReportSDKError(Exception):
     pass
 
 
 class ReportExecutionError(Exception):
```

### Comparing `bg_reports_sdk-1.0.1/bg_reports_sdk/scheduler_manager/scheduler.py` & `bg_reports_sdk-1.0.2/bg_reports_sdk/scheduler_manager/scheduler.py`

 * *Files identical despite different names*

### Comparing `bg_reports_sdk-1.0.1/bg_reports_sdk/scheduler_manager/scheduler_manager.py` & `bg_reports_sdk-1.0.2/bg_reports_sdk/scheduler_manager/scheduler_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from abc import ABC, abstractmethod
 
 import requests
 
-from config import *
+from bg_reports_sdk.config import *
 from bg_reports_sdk.data_provider.data_provider import DataProvider
 from bg_reports_sdk.scheduler_manager.scheduler import Scheduler
 
 
 class SchedulerSDKError(Exception):
     pass
```

### Comparing `bg_reports_sdk-1.0.1/bg_reports_sdk.egg-info/SOURCES.txt` & `bg_reports_sdk-1.0.2/bg_reports_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

