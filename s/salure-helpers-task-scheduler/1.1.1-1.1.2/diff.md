# Comparing `tmp/salure_helpers_task_scheduler-1.1.1.tar.gz` & `tmp/salure_helpers_task_scheduler-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_task_scheduler-1.1.1.tar", last modified: Wed Jul 19 12:31:24 2023, max compression
+gzip compressed data, was "dist/salure_helpers_task_scheduler-1.1.2.tar", last modified: Thu Jul 27 09:14:17 2023, max compression
```

## Comparing `salure_helpers_task_scheduler-1.1.1.tar` & `salure_helpers_task_scheduler-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/
--rw-r--r--   0 root         (0) root         (0)      269 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers/task_scheduler/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-19 12:31:07.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers/task_scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39810 2023-07-19 12:31:07.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers/task_scheduler/task_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)      269 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      414 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      177 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/salure_helpers_task_scheduler.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 12:31:24.000000 salure_helpers_task_scheduler-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-19 12:31:07.000000 salure_helpers_task_scheduler-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:14:17.000000 salure_helpers_task_scheduler-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-27 09:14:17.000000 salure_helpers_task_scheduler-1.1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:14:17.000000 salure_helpers_task_scheduler-1.1.2/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:14:17.000000 salure_helpers_task_scheduler-1.1.2/salure_helpers/task_scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-27 09:14:05.000000 salure_helpers_task_scheduler-1.1.2/salure_helpers/task_scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39766 2023-07-27 09:14:05.000000 salure_helpers_task_scheduler-1.1.2/salure_helpers/task_scheduler/task_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:14:17.000000 salure_helpers_task_scheduler-1.1.2/salure_helpers_task_scheduler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-27 09:14:17.000000 salure_helpers_task_scheduler-1.1.2/salure_helpers_task_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-27 09:14:17.000000 salure_helpers_task_scheduler-1.1.2/salure_helpers_task_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 09:14:17.000000 salure_helpers_task_scheduler-1.1.2/salure_helpers_task_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 09:14:17.000000 salure_helpers_task_scheduler-1.1.2/salure_helpers_task_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-27 09:14:17.000000 salure_helpers_task_scheduler-1.1.2/salure_helpers_task_scheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-27 09:14:17.000000 salure_helpers_task_scheduler-1.1.2/salure_helpers_task_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 09:14:17.000000 salure_helpers_task_scheduler-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-27 09:14:05.000000 salure_helpers_task_scheduler-1.1.2/setup.py
```

### Comparing `salure_helpers_task_scheduler-1.1.1/salure_helpers/task_scheduler/task_scheduler.py` & `salure_helpers_task_scheduler-1.1.2/salure_helpers/task_scheduler/task_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,25 +26,24 @@
         with level DEBUG not is stored
         """
         super().__init__()
         self.mysql = MySQL()
         self.email_after_errors = email_after_errors
         self.task_id = task_id
         self.loglevel = loglevel
+        self.started_at = datetime.datetime.now()
         # If the task is started via the task_scheduler, the following 3 parameters will be passed by the scheduler
         if len(sys.argv[1:4]) > 0:
             self.started_local = False
             self.customer_db, self.task_id, self.run_id = sys.argv[1:4]
         # If the task is started locally, the parameters should be set locally
         else:
             self.started_local = True
             self.customer_db = 'placeholder'
-            self.task_id = self.task_id
             self.run_id = int(round(time.time() * 100000))
-            self.started_at = datetime.datetime.now()
         print(self.task_id, self.run_id)
         self.error_count = 0
 
         # Check if the log tables exists in the customer database. If not, create them
         # Mysql throws a warning when a table already exists. We don't care so we ignore warnings. (not exceptions!)
         warnings.filterwarnings('ignore')
         # self.check_if_logging_tables_exists()
```

### Comparing `salure_helpers_task_scheduler-1.1.1/setup.py` & `salure_helpers_task_scheduler-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_task_scheduler',
-    version='1.1.1',
+    version='1.1.2',
     description='Task Scheduler from Salure',
     long_description='Task Schedule from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.task_scheduler"],
     license='Salure License',
     install_requires=[
```

