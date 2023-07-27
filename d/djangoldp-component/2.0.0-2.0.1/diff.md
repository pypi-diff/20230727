# Comparing `tmp/djangoldp_component-2.0.0.tar.gz` & `tmp/djangoldp_component-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_component-2.0.0.tar", last modified: Thu Jul 27 15:06:58 2023, max compression
+gzip compressed data, was "djangoldp_component-2.0.1.tar", last modified: Thu Jul 27 19:08:50 2023, max compression
```

## Comparing `djangoldp_component-2.0.0.tar` & `djangoldp_component-2.0.1.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:58.480415 djangoldp_component-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-27 15:06:58.480415 djangoldp_component-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:58.476415 djangoldp_component-2.0.0/djangoldp_component/
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-27 15:06:55.000000 djangoldp_component-2.0.0/djangoldp_component/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1512 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:58.480415 djangoldp_component-2.0.0/djangoldp_component/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    12897 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/migrations/0002_delete_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/migrations/0003_component_auto_menu.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9712 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/models.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:58.476415 djangoldp_component-2.0.0/djangoldp_component.egg-info/
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-27 15:06:58.000000 djangoldp_component-2.0.0/djangoldp_component.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-27 15:06:58.000000 djangoldp_component-2.0.0/djangoldp_component.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 15:06:58.000000 djangoldp_component-2.0.0/djangoldp_component.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 15:06:58.000000 djangoldp_component-2.0.0/djangoldp_component.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-27 15:06:58.000000 djangoldp_component-2.0.0/djangoldp_component.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-27 15:06:58.480415 djangoldp_component-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:08:50.882600 djangoldp_component-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-27 19:08:50.882600 djangoldp_component-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:08:50.882600 djangoldp_component-2.0.1/djangoldp_component/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-27 19:08:48.000000 djangoldp_component-2.0.1/djangoldp_component/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/djangoldp_component/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/djangoldp_component/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:08:50.882600 djangoldp_component-2.0.1/djangoldp_component/auth/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/djangoldp_component/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1645 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/djangoldp_component/auth/backends.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/djangoldp_component/djangoldp_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:08:50.882600 djangoldp_component-2.0.1/djangoldp_component/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    12897 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/djangoldp_component/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/djangoldp_component/migrations/0002_delete_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/djangoldp_component/migrations/0003_component_auto_menu.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/djangoldp_component/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9712 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/djangoldp_component/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/djangoldp_component/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:08:50.882600 djangoldp_component-2.0.1/djangoldp_component.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-27 19:08:50.000000 djangoldp_component-2.0.1/djangoldp_component.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      715 2023-07-27 19:08:50.000000 djangoldp_component-2.0.1/djangoldp_component.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 19:08:50.000000 djangoldp_component-2.0.1/djangoldp_component.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 19:08:50.000000 djangoldp_component-2.0.1/djangoldp_component.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-27 19:08:50.000000 djangoldp_component-2.0.1/djangoldp_component.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-27 19:08:50.882600 djangoldp_component-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-27 19:08:31.000000 djangoldp_component-2.0.1/setup.py
```

### Comparing `djangoldp_component-2.0.0/README.md` & `djangoldp_component-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_component-2.0.0/djangoldp_component/admin.py` & `djangoldp_component-2.0.1/djangoldp_component/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_component-2.0.0/djangoldp_component/migrations/0001_initial.py` & `djangoldp_component-2.0.1/djangoldp_component/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_component-2.0.0/djangoldp_component/migrations/0003_component_auto_menu.py` & `djangoldp_component-2.0.1/djangoldp_component/migrations/0003_component_auto_menu.py`

 * *Files identical despite different names*

### Comparing `djangoldp_component-2.0.0/djangoldp_component/models.py` & `djangoldp_component-2.0.1/djangoldp_component/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_component-2.0.0/djangoldp_component.egg-info/SOURCES.txt` & `djangoldp_component-2.0.1/djangoldp_component.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 README.md
 setup.cfg
 setup.py
 djangoldp_component/__init__.py
 djangoldp_component/admin.py
 djangoldp_component/apps.py
+djangoldp_component/djangoldp_settings.py
 djangoldp_component/models.py
 djangoldp_component/settings.py
 djangoldp_component.egg-info/PKG-INFO
 djangoldp_component.egg-info/SOURCES.txt
 djangoldp_component.egg-info/dependency_links.txt
 djangoldp_component.egg-info/requires.txt
 djangoldp_component.egg-info/top_level.txt
+djangoldp_component/auth/__init__.py
+djangoldp_component/auth/backends.py
 djangoldp_component/migrations/0001_initial.py
 djangoldp_component/migrations/0002_delete_dependency.py
 djangoldp_component/migrations/0003_component_auto_menu.py
 djangoldp_component/migrations/__init__.py
```

### Comparing `djangoldp_component-2.0.0/setup.cfg` & `djangoldp_component-2.0.1/setup.cfg`

 * *Files identical despite different names*

