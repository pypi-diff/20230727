# Comparing `tmp/django-dkron-dev-0.8.tar.gz` & `tmp/django-dkron-dev-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dkron-dev-0.8.tar", last modified: Thu Apr 20 12:27:11 2023, max compression
+gzip compressed data, was "django-dkron-dev-0.9.tar", last modified: Thu Apr 20 15:06:34 2023, max compression
```

## Comparing `django-dkron-dev-0.8.tar` & `django-dkron-dev-0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:11.484416 django-dkron-dev-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-20 12:27:11.484416 django-dkron-dev-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 12:27:09.000000 django-dkron-dev-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:11.484416 django-dkron-dev-0.8/django_dkron_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-20 12:27:11.000000 django-dkron-dev-0.8/django_dkron_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-20 12:27:11.000000 django-dkron-dev-0.8/django_dkron_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:27:11.000000 django-dkron-dev-0.8/django_dkron_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:27:11.000000 django-dkron-dev-0.8/django_dkron_dev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-20 12:27:11.000000 django-dkron-dev-0.8/django_dkron_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 12:27:11.000000 django-dkron-dev-0.8/django_dkron_dev.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:11.484416 django-dkron-dev-0.8/dkron/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-20 12:27:09.000000 django-dkron-dev-0.8/dkron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:11.484416 django-dkron-dev-0.8/dkron/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:11.484416 django-dkron-dev-0.8/dkron/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/management/commands/cleanup_dkron.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/management/commands/resync_dkron.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/management/commands/run_dkron.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/management/commands/run_dkron_async_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:11.484416 django-dkron-dev-0.8/dkron/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/migrations/0001_initial_20210729.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/migrations/0002_job_retries.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/migrations/0003_alter_job_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:11.480416 django-dkron-dev-0.8/dkron/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:11.480416 django-dkron-dev-0.8/dkron/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:11.480416 django-dkron-dev-0.8/dkron/templates/admin/dkron/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:11.484416 django-dkron-dev-0.8/dkron/templates/admin/dkron/job/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/templates/admin/dkron/job/change_list_object_tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:27:11.484416 django-dkron-dev-0.8/dkron/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/templatetags/dkron.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/urls_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/dkron/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-20 12:27:11.484416 django-dkron-dev-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:26:59.000000 django-dkron-dev-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:34.421856 django-dkron-dev-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-20 15:06:34.421856 django-dkron-dev-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 15:06:32.000000 django-dkron-dev-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:34.417856 django-dkron-dev-0.9/django_dkron_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-20 15:06:34.000000 django-dkron-dev-0.9/django_dkron_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-20 15:06:34.000000 django-dkron-dev-0.9/django_dkron_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:06:34.000000 django-dkron-dev-0.9/django_dkron_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:06:34.000000 django-dkron-dev-0.9/django_dkron_dev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-20 15:06:34.000000 django-dkron-dev-0.9/django_dkron_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 15:06:34.000000 django-dkron-dev-0.9/django_dkron_dev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:34.417856 django-dkron-dev-0.9/dkron/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-20 15:06:32.000000 django-dkron-dev-0.9/dkron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:34.421856 django-dkron-dev-0.9/dkron/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:34.421856 django-dkron-dev-0.9/dkron/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/management/commands/cleanup_dkron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/management/commands/resync_dkron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/management/commands/run_dkron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/management/commands/run_dkron_async_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:34.421856 django-dkron-dev-0.9/dkron/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/migrations/0001_initial_20210729.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/migrations/0002_job_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/migrations/0003_alter_job_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:34.417856 django-dkron-dev-0.9/dkron/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:34.417856 django-dkron-dev-0.9/dkron/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:34.417856 django-dkron-dev-0.9/dkron/templates/admin/dkron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:34.421856 django-dkron-dev-0.9/dkron/templates/admin/dkron/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/templates/admin/dkron/job/change_list_object_tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:34.421856 django-dkron-dev-0.9/dkron/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/templatetags/dkron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/urls_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/dkron/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-20 15:06:34.421856 django-dkron-dev-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:06:23.000000 django-dkron-dev-0.9/setup.py
```

### Comparing `django-dkron-dev-0.8/LICENSE` & `django-dkron-dev-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/PKG-INFO` & `django-dkron-dev-0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dkron-dev
-Version: 0.8
+Version: 0.9
 Summary: Manage and run jobs in Dkron from your django project
 Home-page: https://github.com/surface-security/django-dkron
 Author: PPB - InfoSec Engineering
 Author-email: surface@paddypowerbetfair.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-dkron-dev-0.8/django_dkron_dev.egg-info/PKG-INFO` & `django-dkron-dev-0.9/django_dkron_dev.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dkron-dev
-Version: 0.8
+Version: 0.9
 Summary: Manage and run jobs in Dkron from your django project
 Home-page: https://github.com/surface-security/django-dkron
 Author: PPB - InfoSec Engineering
 Author-email: surface@paddypowerbetfair.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-dkron-dev-0.8/django_dkron_dev.egg-info/SOURCES.txt` & `django-dkron-dev-0.9/django_dkron_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/dkron/admin.py` & `django-dkron-dev-0.9/dkron/admin.py`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/dkron/apps.py` & `django-dkron-dev-0.9/dkron/apps.py`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/dkron/management/commands/cleanup_dkron.py` & `django-dkron-dev-0.9/dkron/management/commands/cleanup_dkron.py`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/dkron/management/commands/resync_dkron.py` & `django-dkron-dev-0.9/dkron/management/commands/resync_dkron.py`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/dkron/management/commands/run_dkron.py` & `django-dkron-dev-0.9/dkron/management/commands/run_dkron.py`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/dkron/management/commands/run_dkron_async_command.py` & `django-dkron-dev-0.9/dkron/management/commands/run_dkron_async_command.py`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/dkron/migrations/0001_initial_20210729.py` & `django-dkron-dev-0.9/dkron/migrations/0001_initial_20210729.py`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/dkron/migrations/0003_alter_job_schedule.py` & `django-dkron-dev-0.9/dkron/migrations/0003_alter_job_schedule.py`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/dkron/models.py` & `django-dkron-dev-0.9/dkron/models.py`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/dkron/templates/admin/dkron/job/change_list_object_tools.html` & `django-dkron-dev-0.9/dkron/templates/admin/dkron/job/change_list_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/dkron/utils.py` & `django-dkron-dev-0.9/dkron/utils.py`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/dkron/views.py` & `django-dkron-dev-0.9/dkron/views.py`

 * *Files identical despite different names*

### Comparing `django-dkron-dev-0.8/setup.cfg` & `django-dkron-dev-0.9/setup.cfg`

 * *Files identical despite different names*

