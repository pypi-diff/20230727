# Comparing `tmp/raspisump-1.9.tar.gz` & `tmp/raspisump-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspisump-1.9.tar", last modified: Tue Jul 25 12:42:26 2023, max compression
+gzip compressed data, was "raspisump-1.9.1.tar", last modified: Thu Jul 27 13:48:01 2023, max compression
```

## Comparing `raspisump-1.9.tar` & `raspisump-1.9.1.tar`

### file list

```diff
@@ -1,63 +1,61 @@
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.501028 raspisump-1.9/
--rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.9/LICENSE
--rw-r--r--   0 al        (1000) users      (984)      407 2023-07-25 12:40:07.000000 raspisump-1.9/MANIFEST.in
--rw-r--r--   0 al        (1000) users      (984)     3549 2023-07-25 12:42:26.501028 raspisump-1.9/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)     2777 2023-07-25 12:40:07.000000 raspisump-1.9/README.md
--rw-r--r--   0 al        (1000) users      (984)       11 2023-07-25 12:40:07.000000 raspisump-1.9/VERSION
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.491028 raspisump-1.9/bin/
--rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.9/bin/emailtest
--rwxr-xr-x   0 al        (1000) users      (984)     1253 2023-07-25 12:40:07.000000 raspisump-1.9/bin/rsump.py
--rwxr-xr-x   0 al        (1000) users      (984)      719 2023-07-25 12:40:07.000000 raspisump-1.9/bin/rsumpchart.py
--rwxr-xr-x   0 al        (1000) users      (984)      821 2023-07-25 12:40:07.000000 raspisump-1.9/bin/rsumpmonitor.py
--rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.9/bin/rsumpwebchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.491028 raspisump-1.9/conf/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.491028 raspisump-1.9/conf/charts/
--rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.9/conf/charts/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.491028 raspisump-1.9/conf/csv/
--rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.9/conf/csv/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.491028 raspisump-1.9/conf/logs/
--rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.9/conf/logs/README.md
--rw-r--r--   0 al        (1000) users      (984)     5756 2023-07-25 12:40:07.000000 raspisump-1.9/conf/raspisump.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.491028 raspisump-1.9/conf/systemd/
--rw-r--r--   0 al        (1000) users      (984)      135 2023-07-25 12:40:07.000000 raspisump-1.9/conf/systemd/raspisump.service
--rw-r--r--   0 al        (1000) users      (984)      137 2023-07-25 12:40:07.000000 raspisump-1.9/conf/systemd/rsumpwebchart.service
--rw-r--r--   0 al        (1000) users      (984)      130 2023-07-25 12:40:07.000000 raspisump-1.9/conf/systemd/rsumpwebchart.timer
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.494361 raspisump-1.9/conf/web/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.494361 raspisump-1.9/conf/web/css/
--rw-r--r--   0 al        (1000) users      (984)      379 2023-06-15 16:24:24.000000 raspisump-1.9/conf/web/css/includes.js
--rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.9/conf/web/css/index.html
--rw-r--r--   0 al        (1000) users      (984)      526 2023-07-25 12:40:07.000000 raspisump-1.9/conf/web/css/raspi.css
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.494361 raspisump-1.9/conf/web/images/
--rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.9/conf/web/images/logo.png
--rw-r--r--   0 al        (1000) users      (984)     3682 2023-07-25 12:40:07.000000 raspisump-1.9/conf/web/index.html
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.494361 raspisump-1.9/cron/
--rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.9/cron/README.md
--rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.9/cron/picrontab
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.497695 raspisump-1.9/docs/
--rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.9/docs/README.md
--rw-r--r--   0 al        (1000) users      (984)     8735 2023-07-25 12:40:07.000000 raspisump-1.9/docs/install.md
--rw-r--r--   0 al        (1000) users      (984)   133806 2023-06-02 22:51:18.000000 raspisump-1.9/docs/install.pdf
--rw-r--r--   0 al        (1000) users      (984)     4397 2023-07-25 12:40:07.000000 raspisump-1.9/docs/upgrade_systemd.md
--rw-r--r--   0 al        (1000) users      (984)     4937 2023-07-25 12:40:07.000000 raspisump-1.9/docs/upgrade_to_version_1.9.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.501028 raspisump-1.9/raspisump/
--rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.9/raspisump/__init__.py
--rw-r--r--   0 al        (1000) users      (984)     3781 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/alerts.py
--rw-r--r--   0 al        (1000) users      (984)     1959 2023-07-25 12:40:07.000000 raspisump-1.9/raspisump/checkpid.py
--rw-r--r--   0 al        (1000) users      (984)     2413 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/config_values.py
--rw-r--r--   0 al        (1000) users      (984)     1449 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/emailtest.py
--rw-r--r--   0 al        (1000) users      (984)     3543 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/heartbeat.py
--rw-r--r--   0 al        (1000) users      (984)      892 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/log.py
--rw-r--r--   0 al        (1000) users      (984)     2012 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/reading.py
--rw-r--r--   0 al        (1000) users      (984)     1864 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/todaychart.py
--rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.9/raspisump/webchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.501028 raspisump-1.9/raspisump.egg-info/
--rw-r--r--   0 al        (1000) users      (984)     3549 2023-07-25 12:42:26.000000 raspisump-1.9/raspisump.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)      990 2023-07-25 12:42:26.000000 raspisump-1.9/raspisump.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) users      (984)        1 2023-07-25 12:42:26.000000 raspisump-1.9/raspisump.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) users      (984)       18 2023-07-25 12:42:26.000000 raspisump-1.9/raspisump.egg-info/requires.txt
--rw-r--r--   0 al        (1000) users      (984)       10 2023-07-25 12:42:26.000000 raspisump-1.9/raspisump.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) users      (984)       38 2023-07-25 12:42:26.501028 raspisump-1.9/setup.cfg
--rwxr-xr-x   0 al        (1000) users      (984)     2804 2023-07-25 12:40:07.000000 raspisump-1.9/setup.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.501028 raspisump-1.9/tests/
--rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.9/tests/tests_logging.py
--rw-r--r--   0 al        (1000) users      (984)     3904 2023-07-04 19:19:39.000000 raspisump-1.9/tests/tests_sump.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.966688 raspisump-1.9.1/
+-rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.9.1/LICENSE
+-rw-r--r--   0 al        (1000) users      (984)      407 2023-07-25 12:40:07.000000 raspisump-1.9.1/MANIFEST.in
+-rw-r--r--   0 al        (1000) users      (984)     3551 2023-07-27 13:48:01.963354 raspisump-1.9.1/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)     2777 2023-07-25 12:40:07.000000 raspisump-1.9.1/README.md
+-rw-r--r--   0 al        (1000) users      (984)       13 2023-07-27 13:47:12.000000 raspisump-1.9.1/VERSION
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.956688 raspisump-1.9.1/bin/
+-rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.9.1/bin/emailtest
+-rwxr-xr-x   0 al        (1000) users      (984)     1253 2023-07-25 12:40:07.000000 raspisump-1.9.1/bin/rsump.py
+-rwxr-xr-x   0 al        (1000) users      (984)      719 2023-07-25 12:40:07.000000 raspisump-1.9.1/bin/rsumpchart.py
+-rwxr-xr-x   0 al        (1000) users      (984)      821 2023-07-25 12:40:07.000000 raspisump-1.9.1/bin/rsumpmonitor.py
+-rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.9.1/bin/rsumpwebchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.956688 raspisump-1.9.1/conf/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.956688 raspisump-1.9.1/conf/charts/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.9.1/conf/charts/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.956688 raspisump-1.9.1/conf/csv/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.9.1/conf/csv/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.956688 raspisump-1.9.1/conf/logs/
+-rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.9.1/conf/logs/README.md
+-rw-r--r--   0 al        (1000) users      (984)     5756 2023-07-25 12:40:07.000000 raspisump-1.9.1/conf/raspisump.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.956688 raspisump-1.9.1/conf/systemd/
+-rw-r--r--   0 al        (1000) users      (984)      135 2023-07-25 12:40:07.000000 raspisump-1.9.1/conf/systemd/raspisump.service
+-rw-r--r--   0 al        (1000) users      (984)      137 2023-07-25 12:40:07.000000 raspisump-1.9.1/conf/systemd/rsumpwebchart.service
+-rw-r--r--   0 al        (1000) users      (984)      130 2023-07-25 12:40:07.000000 raspisump-1.9.1/conf/systemd/rsumpwebchart.timer
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.960021 raspisump-1.9.1/conf/web/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.960021 raspisump-1.9.1/conf/web/css/
+-rw-r--r--   0 al        (1000) users      (984)      379 2023-06-15 16:24:24.000000 raspisump-1.9.1/conf/web/css/includes.js
+-rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.9.1/conf/web/css/index.html
+-rw-r--r--   0 al        (1000) users      (984)      526 2023-07-25 12:40:07.000000 raspisump-1.9.1/conf/web/css/raspi.css
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.960021 raspisump-1.9.1/conf/web/images/
+-rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.9.1/conf/web/images/logo.png
+-rw-r--r--   0 al        (1000) users      (984)     3682 2023-07-25 12:40:07.000000 raspisump-1.9.1/conf/web/index.html
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.960021 raspisump-1.9.1/cron/
+-rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.9.1/cron/README.md
+-rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.9.1/cron/picrontab
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.960021 raspisump-1.9.1/docs/
+-rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.9.1/docs/README.md
+-rw-r--r--   0 al        (1000) users      (984)    10408 2023-07-27 13:47:12.000000 raspisump-1.9.1/docs/install.md
+-rw-r--r--   0 al        (1000) users      (984)     5234 2023-07-27 13:47:12.000000 raspisump-1.9.1/docs/upgrade_to_version_1.9.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.963354 raspisump-1.9.1/raspisump/
+-rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.9.1/raspisump/__init__.py
+-rw-r--r--   0 al        (1000) users      (984)     3781 2023-07-04 19:19:39.000000 raspisump-1.9.1/raspisump/alerts.py
+-rw-r--r--   0 al        (1000) users      (984)     1959 2023-07-25 12:40:07.000000 raspisump-1.9.1/raspisump/checkpid.py
+-rw-r--r--   0 al        (1000) users      (984)     2412 2023-07-27 13:47:12.000000 raspisump-1.9.1/raspisump/config_values.py
+-rw-r--r--   0 al        (1000) users      (984)     1449 2023-07-04 19:19:39.000000 raspisump-1.9.1/raspisump/emailtest.py
+-rw-r--r--   0 al        (1000) users      (984)     3543 2023-07-04 19:19:39.000000 raspisump-1.9.1/raspisump/heartbeat.py
+-rw-r--r--   0 al        (1000) users      (984)      892 2023-07-04 19:19:39.000000 raspisump-1.9.1/raspisump/log.py
+-rw-r--r--   0 al        (1000) users      (984)     2012 2023-07-04 19:19:39.000000 raspisump-1.9.1/raspisump/reading.py
+-rw-r--r--   0 al        (1000) users      (984)     1864 2023-07-04 19:19:39.000000 raspisump-1.9.1/raspisump/todaychart.py
+-rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.9.1/raspisump/webchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.963354 raspisump-1.9.1/raspisump.egg-info/
+-rw-r--r--   0 al        (1000) users      (984)     3551 2023-07-27 13:48:01.000000 raspisump-1.9.1/raspisump.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)      949 2023-07-27 13:48:01.000000 raspisump-1.9.1/raspisump.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) users      (984)        1 2023-07-27 13:48:01.000000 raspisump-1.9.1/raspisump.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) users      (984)       18 2023-07-27 13:48:01.000000 raspisump-1.9.1/raspisump.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) users      (984)       10 2023-07-27 13:48:01.000000 raspisump-1.9.1/raspisump.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) users      (984)       38 2023-07-27 13:48:01.966688 raspisump-1.9.1/setup.cfg
+-rwxr-xr-x   0 al        (1000) users      (984)     2806 2023-07-27 13:47:12.000000 raspisump-1.9.1/setup.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-27 13:48:01.963354 raspisump-1.9.1/tests/
+-rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.9.1/tests/tests_logging.py
+-rw-r--r--   0 al        (1000) users      (984)     3904 2023-07-04 19:19:39.000000 raspisump-1.9.1/tests/tests_sump.py
```

### Comparing `raspisump-1.9/LICENSE` & `raspisump-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/PKG-INFO` & `raspisump-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.9
+Version: 1.9.1
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `raspisump-1.9/README.md` & `raspisump-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/bin/rsump.py` & `raspisump-1.9.1/bin/rsump.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/bin/rsumpchart.py` & `raspisump-1.9.1/bin/rsumpchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/bin/rsumpmonitor.py` & `raspisump-1.9.1/bin/rsumpmonitor.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/bin/rsumpwebchart.py` & `raspisump-1.9.1/bin/rsumpwebchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/conf/raspisump.conf` & `raspisump-1.9.1/conf/raspisump.conf`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/conf/web/css/raspi.css` & `raspisump-1.9.1/conf/web/css/raspi.css`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/conf/web/images/logo.png` & `raspisump-1.9.1/conf/web/images/logo.png`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/conf/web/index.html` & `raspisump-1.9.1/conf/web/index.html`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/docs/install.md` & `raspisump-1.9.1/docs/install.md`

 * *Files 16% similar despite different names*

```diff
@@ -234,12 +234,61 @@
 
     sudo systemctl restart lighttpd
 
 Open a web browser to http://ip_of_your_pi. Having configured the rsumpwebchart.timer earlier, a new webchart will be created every 15 minutes for viewing.
 This will also copy historical information that you can access
 from the link in the web page.
 
+# Optional - Make it Easier to initiate systemd commands
+
+If you find typing the systemctl commands cumbersome you can make it easier by creating aliases. An alias is shortcut you can type that will initiate a long command.
+
+Aliases are added to the `.bash_aliases` file in your home folder as follows
+
+        cd /home/__username__
+        nano .bash_aliases
+
+Copy and paste the following aliases for Raspi-Sump `systemd` commands in the file. Make sure there are no spaces at the beginning of each line after pasting.
+
+        alias sumpon="systemctl --user start raspisump && systemctl --user start rsumpwebchart.timer"
+        alias sumpoff="systemctl --user stop raspisump && systemctl --user stop rsumpwebchart.timer"
+        alias sumpstats="systemctl --user status raspisump"
+        alias sumpchartstats="systemctl --user status rsumpwebchart.timer"
+        alias sumpboot="systemctl --user enable raspisump && systemctl --user enable rsumpwebchart.timer"
+        alias sumpnoboot="systemctl --user disable raspisump && systemctl --user disable rsumpwebchart.timer"
+        alias sumprestart="systemctl --user restart raspisump"
+
+Save the file, logout and log back in to activate the new aliases.
+
+- Start raspisump and rsumpwebchart.timer
+
+        sumpon
+
+- Stop raspisump and rsumpwebchart.timer
+
+        sumpoff
+
+- Show status of the raspisump service
+
+        sumpstats
+
+- Show status of the rsumpwebchart timer
+
+        sumpchartstats
+
+- Enable raspisump and rsumpchart.timer on boot
+
+        sumpboot
+
+- Disable raspisump and rsumpchart.timer on boot
+
+        sumpnoboot
+
+- Restart raspisump after making a `raspisump.conf` file change
+
+        sumprestart
+
 # Support
 
 For support open an issue on the Github Issue Tracker or consider joining our discord server.
 
 For Discord simply send an email to alaudet@linuxnorth.org and request an invite link.
```

### Comparing `raspisump-1.9/docs/upgrade_systemd.md` & `raspisump-1.9.1/docs/upgrade_to_version_1.9.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+# Upgrade to Raspi-Sump Version 1.9 instructions.
+
+These instructions are for upgrading versions 1.8 and lower to version 1.9. If you are doing a new install, disregard these instructions and use the [Raspi-Sump New Install Instructions](https://github.com/alaudet/raspi-sump/blob/master/docs/install.md) instead.
+
 # Upgrade Raspi-Sump to use Systemd
 
-Raspi-Sump versions later than 1.8 use `systemd` to manage the services related to sump monitoring and chart creation.
+Raspi-Sump version 1.9 and later use `systemd` to manage the services related to sump monitoring and chart creation.
 
 `Systemd` replaces cron scheduling for taking readings and creating charts on a schedule. It also replaces `rsumpmonitor.py` for monitoring the status of the raspisump process when taking more than one reading per minute.
 
 `Systemd` will automatically restart the Raspi-Sump process if it stops and is a more robust way to handle failed processes than `rsumpmonitor.py`.
 
 ## If you currently take readings once per minute or more
 
-If you currently call `rsump.py` with cron every minute or more and are happy with this approach you can continue doing this. Nothing changes for you. However `systemd` makes it easier to stop and start processes.
+If you currently call `rsump.py` with cron every minute or more and are happy with this approach you can continue doing this. Nothing changes for you. However `systemd` makes it easier to stop and start processes. Some people are militant about deprecating cron in favour of systemd but cron is proven and works well in this situation. Nothing wrong with continuing to use as is.
+
+e.g. If `reading_interval = 0` in your `raspisump.conf` file and you use cron to call rsump.py every minute or more, you do not need to use `systemd`. It is an option to switch but Raspi-Sump will continue working as normal fine with cron when only taking one reading and exiting.
 
 # Setting up Systemd
 
 ## Upgrade to the latest version
 
 Upgrade to the latest version of Raspi-Sump
 
@@ -95,27 +101,27 @@
 If you find typing the systemctl commands cumbersome you can make it easier by creating aliases. An alias is shortcut you can type that will initiate a long command.
 
 Aliases are added to the `.bash_aliases` file in your home folder as follows
 
         cd /home/__username__
         nano .bash_aliases
 
-Copy and paste the following aliases for Raspi-Sump `systemd` commands in the file.
+Copy and paste the following aliases for Raspi-Sump `systemd` commands in the file. Make sure there are no spaces at the beginning of each line after pasting.
 
         alias sumpon="systemctl --user start raspisump && systemctl --user start rsumpwebchart.timer"
         alias sumpoff="systemctl --user stop raspisump && systemctl --user stop rsumpwebchart.timer"
         alias sumpstats="systemctl --user status raspisump"
         alias sumpchartstats="systemctl --user status rsumpwebchart.timer"
         alias sumpboot="systemctl --user enable raspisump && systemctl --user enable rsumpwebchart.timer"
         alias sumpnoboot="systemctl --user disable raspisump && systemctl --user disable rsumpwebchart.timer"
         alias sumprestart="systemctl --user restart raspisump"
 
-Save the file, logout and log back in for the aliases to activate.
+Save the file, logout and log back in to activate the new aliases.
 
-- Start raspisump and rsumpwebchar.timer
+- Start raspisump and rsumpwebchart.timer
 
         sumpon
 
 - Stop raspisump and rsumpwebchart.timer
 
         sumpoff
```

### Comparing `raspisump-1.9/raspisump/alerts.py` & `raspisump-1.9.1/raspisump/alerts.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/raspisump/checkpid.py` & `raspisump-1.9.1/raspisump/checkpid.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/raspisump/config_values.py` & `raspisump-1.9.1/raspisump/config_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     try:
         configs["alert_interval"] = config.getint("email", "alert_interval")
     except configparser.NoOptionError:
         configs["alert_interval"] = 5
 
     try:
         configs["smtp_ssl"] = config.getint("email", "smtp_ssl")
-    except configparser.NoSectionError:
+    except configparser.NoOptionError:
         configs["smtp_ssl"] = 0
 
     try:
         configs["heartbeat"] = config.getint("email", "heartbeat")
     except configparser.NoOptionError:
         configs["heartbeat"] = 0
```

### Comparing `raspisump-1.9/raspisump/emailtest.py` & `raspisump-1.9.1/raspisump/emailtest.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/raspisump/heartbeat.py` & `raspisump-1.9.1/raspisump/heartbeat.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/raspisump/log.py` & `raspisump-1.9.1/raspisump/log.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/raspisump/reading.py` & `raspisump-1.9.1/raspisump/reading.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/raspisump/todaychart.py` & `raspisump-1.9.1/raspisump/todaychart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/raspisump/webchart.py` & `raspisump-1.9.1/raspisump/webchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/raspisump.egg-info/PKG-INFO` & `raspisump-1.9.1/raspisump.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.9
+Version: 1.9.1
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `raspisump-1.9/raspisump.egg-info/SOURCES.txt` & `raspisump-1.9.1/raspisump.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 conf/web/css/index.html
 conf/web/css/raspi.css
 conf/web/images/logo.png
 cron/README.md
 cron/picrontab
 docs/README.md
 docs/install.md
-docs/install.pdf
-docs/upgrade_systemd.md
 docs/upgrade_to_version_1.9.md
 raspisump/__init__.py
 raspisump/alerts.py
 raspisump/checkpid.py
 raspisump/config_values.py
 raspisump/emailtest.py
 raspisump/heartbeat.py
```

### Comparing `raspisump-1.9/setup.py` & `raspisump-1.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = "1.9"
+version = "1.9.1"
 user = os.getlogin()
 
 
 homedir = "/home/" + user + "/raspi-sump/"
 systemd_configdir = "/home/" + user + "/.config/systemd/user/"
```

### Comparing `raspisump-1.9/tests/tests_logging.py` & `raspisump-1.9.1/tests/tests_logging.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.9/tests/tests_sump.py` & `raspisump-1.9.1/tests/tests_sump.py`

 * *Files identical despite different names*

