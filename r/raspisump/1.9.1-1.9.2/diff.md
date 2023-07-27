# Comparing `tmp/raspisump-1.9.1.tar.gz` & `tmp/raspisump-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspisump-1.9.1.tar", last modified: Thu Jul 27 13:48:01 2023, max compression
+gzip compressed data, was "raspisump-1.9.2.tar", last modified: Thu Jul 27 14:03:31 2023, max compression
```

## Comparing `raspisump-1.9.1.tar` & `raspisump-1.9.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.966688 raspisump-1.9.1/
--rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.9.1/LICENSE
--rw-r--r--   0 al        (1000) users      (984)      407 2023-07-25 12:40:07.000000 raspisump-1.9.1/MANIFEST.in
--rw-r--r--   0 al        (1000) users      (984)     3551 2023-07-27 13:48:01.963354 raspisump-1.9.1/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)     2777 2023-07-25 12:40:07.000000 raspisump-1.9.1/README.md
--rw-r--r--   0 al        (1000) users      (984)       13 2023-07-27 13:47:12.000000 raspisump-1.9.1/VERSION
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.956688 raspisump-1.9.1/bin/
--rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.9.1/bin/emailtest
--rwxr-xr-x   0 al        (1000) users      (984)     1253 2023-07-25 12:40:07.000000 raspisump-1.9.1/bin/rsump.py
--rwxr-xr-x   0 al        (1000) users      (984)      719 2023-07-25 12:40:07.000000 raspisump-1.9.1/bin/rsumpchart.py
--rwxr-xr-x   0 al        (1000) users      (984)      821 2023-07-25 12:40:07.000000 raspisump-1.9.1/bin/rsumpmonitor.py
--rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.9.1/bin/rsumpwebchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.956688 raspisump-1.9.1/conf/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.956688 raspisump-1.9.1/conf/charts/
--rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.9.1/conf/charts/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.956688 raspisump-1.9.1/conf/csv/
--rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.9.1/conf/csv/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.956688 raspisump-1.9.1/conf/logs/
--rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.9.1/conf/logs/README.md
--rw-r--r--   0 al        (1000) users      (984)     5756 2023-07-25 12:40:07.000000 raspisump-1.9.1/conf/raspisump.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.956688 raspisump-1.9.1/conf/systemd/
--rw-r--r--   0 al        (1000) users      (984)      135 2023-07-25 12:40:07.000000 raspisump-1.9.1/conf/systemd/raspisump.service
--rw-r--r--   0 al        (1000) users      (984)      137 2023-07-25 12:40:07.000000 raspisump-1.9.1/conf/systemd/rsumpwebchart.service
--rw-r--r--   0 al        (1000) users      (984)      130 2023-07-25 12:40:07.000000 raspisump-1.9.1/conf/systemd/rsumpwebchart.timer
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.960021 raspisump-1.9.1/conf/web/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.960021 raspisump-1.9.1/conf/web/css/
--rw-r--r--   0 al        (1000) users      (984)      379 2023-06-15 16:24:24.000000 raspisump-1.9.1/conf/web/css/includes.js
--rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.9.1/conf/web/css/index.html
--rw-r--r--   0 al        (1000) users      (984)      526 2023-07-25 12:40:07.000000 raspisump-1.9.1/conf/web/css/raspi.css
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.960021 raspisump-1.9.1/conf/web/images/
--rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.9.1/conf/web/images/logo.png
--rw-r--r--   0 al        (1000) users      (984)     3682 2023-07-25 12:40:07.000000 raspisump-1.9.1/conf/web/index.html
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.960021 raspisump-1.9.1/cron/
--rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.9.1/cron/README.md
--rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.9.1/cron/picrontab
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.960021 raspisump-1.9.1/docs/
--rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.9.1/docs/README.md
--rw-r--r--   0 al        (1000) users      (984)    10408 2023-07-27 13:47:12.000000 raspisump-1.9.1/docs/install.md
--rw-r--r--   0 al        (1000) users      (984)     5234 2023-07-27 13:47:12.000000 raspisump-1.9.1/docs/upgrade_to_version_1.9.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.963354 raspisump-1.9.1/raspisump/
--rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.9.1/raspisump/__init__.py
--rw-r--r--   0 al        (1000) users      (984)     3781 2023-07-04 19:19:39.000000 raspisump-1.9.1/raspisump/alerts.py
--rw-r--r--   0 al        (1000) users      (984)     1959 2023-07-25 12:40:07.000000 raspisump-1.9.1/raspisump/checkpid.py
--rw-r--r--   0 al        (1000) users      (984)     2412 2023-07-27 13:47:12.000000 raspisump-1.9.1/raspisump/config_values.py
--rw-r--r--   0 al        (1000) users      (984)     1449 2023-07-04 19:19:39.000000 raspisump-1.9.1/raspisump/emailtest.py
--rw-r--r--   0 al        (1000) users      (984)     3543 2023-07-04 19:19:39.000000 raspisump-1.9.1/raspisump/heartbeat.py
--rw-r--r--   0 al        (1000) users      (984)      892 2023-07-04 19:19:39.000000 raspisump-1.9.1/raspisump/log.py
--rw-r--r--   0 al        (1000) users      (984)     2012 2023-07-04 19:19:39.000000 raspisump-1.9.1/raspisump/reading.py
--rw-r--r--   0 al        (1000) users      (984)     1864 2023-07-04 19:19:39.000000 raspisump-1.9.1/raspisump/todaychart.py
--rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.9.1/raspisump/webchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.963354 raspisump-1.9.1/raspisump.egg-info/
--rw-r--r--   0 al        (1000) users      (984)     3551 2023-07-27 13:48:01.000000 raspisump-1.9.1/raspisump.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)      949 2023-07-27 13:48:01.000000 raspisump-1.9.1/raspisump.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) users      (984)        1 2023-07-27 13:48:01.000000 raspisump-1.9.1/raspisump.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) users      (984)       18 2023-07-27 13:48:01.000000 raspisump-1.9.1/raspisump.egg-info/requires.txt
--rw-r--r--   0 al        (1000) users      (984)       10 2023-07-27 13:48:01.000000 raspisump-1.9.1/raspisump.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) users      (984)       38 2023-07-27 13:48:01.966688 raspisump-1.9.1/setup.cfg
--rwxr-xr-x   0 al        (1000) users      (984)     2806 2023-07-27 13:47:12.000000 raspisump-1.9.1/setup.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.963354 raspisump-1.9.1/tests/
--rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.9.1/tests/tests_logging.py
--rw-r--r--   0 al        (1000) users      (984)     3904 2023-07-04 19:19:39.000000 raspisump-1.9.1/tests/tests_sump.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.107618 raspisump-1.9.2/
+-rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.9.2/LICENSE
+-rw-r--r--   0 al        (1000) users      (984)      407 2023-07-25 12:40:07.000000 raspisump-1.9.2/MANIFEST.in
+-rw-r--r--   0 al        (1000) users      (984)     3551 2023-07-27 14:03:31.107618 raspisump-1.9.2/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)     2777 2023-07-25 12:40:07.000000 raspisump-1.9.2/README.md
+-rw-r--r--   0 al        (1000) users      (984)       13 2023-07-27 14:03:11.000000 raspisump-1.9.2/VERSION
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.100952 raspisump-1.9.2/bin/
+-rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.9.2/bin/emailtest
+-rwxr-xr-x   0 al        (1000) users      (984)     1253 2023-07-25 12:40:07.000000 raspisump-1.9.2/bin/rsump.py
+-rwxr-xr-x   0 al        (1000) users      (984)      719 2023-07-25 12:40:07.000000 raspisump-1.9.2/bin/rsumpchart.py
+-rwxr-xr-x   0 al        (1000) users      (984)      821 2023-07-25 12:40:07.000000 raspisump-1.9.2/bin/rsumpmonitor.py
+-rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.9.2/bin/rsumpwebchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.100952 raspisump-1.9.2/conf/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.104285 raspisump-1.9.2/conf/charts/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.9.2/conf/charts/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.104285 raspisump-1.9.2/conf/csv/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.9.2/conf/csv/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.104285 raspisump-1.9.2/conf/logs/
+-rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.9.2/conf/logs/README.md
+-rw-r--r--   0 al        (1000) users      (984)     5756 2023-07-25 12:40:07.000000 raspisump-1.9.2/conf/raspisump.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.104285 raspisump-1.9.2/conf/systemd/
+-rw-r--r--   0 al        (1000) users      (984)      135 2023-07-25 12:40:07.000000 raspisump-1.9.2/conf/systemd/raspisump.service
+-rw-r--r--   0 al        (1000) users      (984)      137 2023-07-25 12:40:07.000000 raspisump-1.9.2/conf/systemd/rsumpwebchart.service
+-rw-r--r--   0 al        (1000) users      (984)      130 2023-07-25 12:40:07.000000 raspisump-1.9.2/conf/systemd/rsumpwebchart.timer
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.104285 raspisump-1.9.2/conf/web/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.104285 raspisump-1.9.2/conf/web/css/
+-rw-r--r--   0 al        (1000) users      (984)      379 2023-06-15 16:24:24.000000 raspisump-1.9.2/conf/web/css/includes.js
+-rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.9.2/conf/web/css/index.html
+-rw-r--r--   0 al        (1000) users      (984)      526 2023-07-25 12:40:07.000000 raspisump-1.9.2/conf/web/css/raspi.css
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.104285 raspisump-1.9.2/conf/web/images/
+-rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.9.2/conf/web/images/logo.png
+-rw-r--r--   0 al        (1000) users      (984)     3682 2023-07-25 12:40:07.000000 raspisump-1.9.2/conf/web/index.html
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.104285 raspisump-1.9.2/cron/
+-rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.9.2/cron/README.md
+-rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.9.2/cron/picrontab
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.104285 raspisump-1.9.2/docs/
+-rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.9.2/docs/README.md
+-rw-r--r--   0 al        (1000) users      (984)    10408 2023-07-27 13:47:12.000000 raspisump-1.9.2/docs/install.md
+-rw-r--r--   0 al        (1000) users      (984)     5234 2023-07-27 13:47:12.000000 raspisump-1.9.2/docs/upgrade_to_version_1.9.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.104285 raspisump-1.9.2/raspisump/
+-rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.9.2/raspisump/__init__.py
+-rw-r--r--   0 al        (1000) users      (984)     3781 2023-07-04 19:19:39.000000 raspisump-1.9.2/raspisump/alerts.py
+-rw-r--r--   0 al        (1000) users      (984)     1959 2023-07-25 12:40:07.000000 raspisump-1.9.2/raspisump/checkpid.py
+-rw-r--r--   0 al        (1000) users      (984)     2411 2023-07-27 13:57:27.000000 raspisump-1.9.2/raspisump/config_values.py
+-rw-r--r--   0 al        (1000) users      (984)     1449 2023-07-04 19:19:39.000000 raspisump-1.9.2/raspisump/emailtest.py
+-rw-r--r--   0 al        (1000) users      (984)     3543 2023-07-04 19:19:39.000000 raspisump-1.9.2/raspisump/heartbeat.py
+-rw-r--r--   0 al        (1000) users      (984)      892 2023-07-04 19:19:39.000000 raspisump-1.9.2/raspisump/log.py
+-rw-r--r--   0 al        (1000) users      (984)     2012 2023-07-04 19:19:39.000000 raspisump-1.9.2/raspisump/reading.py
+-rw-r--r--   0 al        (1000) users      (984)     1864 2023-07-04 19:19:39.000000 raspisump-1.9.2/raspisump/todaychart.py
+-rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.9.2/raspisump/webchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.107618 raspisump-1.9.2/raspisump.egg-info/
+-rw-r--r--   0 al        (1000) users      (984)     3551 2023-07-27 14:03:31.000000 raspisump-1.9.2/raspisump.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)      949 2023-07-27 14:03:31.000000 raspisump-1.9.2/raspisump.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) users      (984)        1 2023-07-27 14:03:31.000000 raspisump-1.9.2/raspisump.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) users      (984)       18 2023-07-27 14:03:31.000000 raspisump-1.9.2/raspisump.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) users      (984)       10 2023-07-27 14:03:31.000000 raspisump-1.9.2/raspisump.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) users      (984)       38 2023-07-27 14:03:31.107618 raspisump-1.9.2/setup.cfg
+-rwxr-xr-x   0 al        (1000) users      (984)     2806 2023-07-27 14:03:11.000000 raspisump-1.9.2/setup.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 14:03:31.107618 raspisump-1.9.2/tests/
+-rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.9.2/tests/tests_logging.py
+-rw-r--r--   0 al        (1000) users      (984)     3904 2023-07-04 19:19:39.000000 raspisump-1.9.2/tests/tests_sump.py
```

### Comparing `raspisump-1.9.1/LICENSE` & `raspisump-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/PKG-INFO` & `raspisump-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.9.1
+Version: 1.9.2
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `raspisump-1.9.1/README.md` & `raspisump-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/bin/rsump.py` & `raspisump-1.9.2/bin/rsump.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/bin/rsumpchart.py` & `raspisump-1.9.2/bin/rsumpchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/bin/rsumpmonitor.py` & `raspisump-1.9.2/bin/rsumpmonitor.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/bin/rsumpwebchart.py` & `raspisump-1.9.2/bin/rsumpwebchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/conf/raspisump.conf` & `raspisump-1.9.2/conf/raspisump.conf`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/conf/web/css/raspi.css` & `raspisump-1.9.2/conf/web/css/raspi.css`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/conf/web/images/logo.png` & `raspisump-1.9.2/conf/web/images/logo.png`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/conf/web/index.html` & `raspisump-1.9.2/conf/web/index.html`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/docs/install.md` & `raspisump-1.9.2/docs/install.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/docs/upgrade_to_version_1.9.md` & `raspisump-1.9.2/docs/upgrade_to_version_1.9.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/raspisump/alerts.py` & `raspisump-1.9.2/raspisump/alerts.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/raspisump/checkpid.py` & `raspisump-1.9.2/raspisump/checkpid.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/raspisump/config_values.py` & `raspisump-1.9.2/raspisump/config_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,11 +60,11 @@
     try:
         configs["heartbeat_interval"] = config.getint("email", "heartbeat_interval")
     except configparser.NoOptionError:
         configs["heartbeat_interval"] = 10080
 
     try:
         configs["line_color"] = config.get("charts", "line_color")
-    except configparser.NoSectionError:
+    except configparser.NoOptionError:
         configs["line_color"] = "FB921D"
 
     return configs
```

### Comparing `raspisump-1.9.1/raspisump/emailtest.py` & `raspisump-1.9.2/raspisump/emailtest.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/raspisump/heartbeat.py` & `raspisump-1.9.2/raspisump/heartbeat.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/raspisump/log.py` & `raspisump-1.9.2/raspisump/log.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/raspisump/reading.py` & `raspisump-1.9.2/raspisump/reading.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/raspisump/todaychart.py` & `raspisump-1.9.2/raspisump/todaychart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/raspisump/webchart.py` & `raspisump-1.9.2/raspisump/webchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/raspisump.egg-info/PKG-INFO` & `raspisump-1.9.2/raspisump.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.9.1
+Version: 1.9.2
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `raspisump-1.9.1/raspisump.egg-info/SOURCES.txt` & `raspisump-1.9.2/raspisump.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/setup.py` & `raspisump-1.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = "1.9.1"
+version = "1.9.2"
 user = os.getlogin()
 
 
 homedir = "/home/" + user + "/raspi-sump/"
 systemd_configdir = "/home/" + user + "/.config/systemd/user/"
```

### Comparing `raspisump-1.9.1/tests/tests_logging.py` & `raspisump-1.9.2/tests/tests_logging.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9.1/tests/tests_sump.py` & `raspisump-1.9.2/tests/tests_sump.py`

 * *Files identical despite different names*

