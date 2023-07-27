# Comparing `tmp/django-olympus-0.0.4.tar.gz` & `tmp/django-olympus-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-olympus-0.0.4.tar", last modified: Fri Jul 14 08:21:15 2023, max compression
+gzip compressed data, was "django-olympus-0.0.5.tar", last modified: Thu Jul 27 11:05:28 2023, max compression
```

## Comparing `django-olympus-0.0.4.tar` & `django-olympus-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:15.875556 django-olympus-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-14 08:21:06.000000 django-olympus-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 08:21:06.000000 django-olympus-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-14 08:21:15.875556 django-olympus-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-14 08:21:06.000000 django-olympus-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:15.875556 django-olympus-0.0.4/django_olympus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-14 08:21:15.000000 django-olympus-0.0.4/django_olympus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-14 08:21:15.000000 django-olympus-0.0.4/django_olympus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:21:15.000000 django-olympus-0.0.4/django_olympus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:21:15.000000 django-olympus-0.0.4/django_olympus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-14 08:21:15.000000 django-olympus-0.0.4/django_olympus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 08:21:15.000000 django-olympus-0.0.4/django_olympus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:15.875556 django-olympus-0.0.4/olympus/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:15.875556 django-olympus-0.0.4/olympus/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:15.875556 django-olympus-0.0.4/olympus/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/management/commands/push_to_es.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:15.875556 django-olympus-0.0.4/olympus/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-14 08:21:15.875556 django-olympus-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 08:21:06.000000 django-olympus-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:05:28.954333 django-olympus-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 11:05:18.000000 django-olympus-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-27 11:05:18.000000 django-olympus-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-27 11:05:28.954333 django-olympus-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-27 11:05:18.000000 django-olympus-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:05:28.954333 django-olympus-0.0.5/django_olympus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-27 11:05:28.000000 django-olympus-0.0.5/django_olympus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-27 11:05:28.000000 django-olympus-0.0.5/django_olympus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:05:28.000000 django-olympus-0.0.5/django_olympus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:05:28.000000 django-olympus-0.0.5/django_olympus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 11:05:28.000000 django-olympus-0.0.5/django_olympus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 11:05:28.000000 django-olympus-0.0.5/django_olympus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:05:28.954333 django-olympus-0.0.5/olympus/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 11:05:18.000000 django-olympus-0.0.5/olympus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-27 11:05:18.000000 django-olympus-0.0.5/olympus/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-07-27 11:05:18.000000 django-olympus-0.0.5/olympus/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:05:28.954333 django-olympus-0.0.5/olympus/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:05:18.000000 django-olympus-0.0.5/olympus/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:05:28.954333 django-olympus-0.0.5/olympus/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:05:18.000000 django-olympus-0.0.5/olympus/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-27 11:05:18.000000 django-olympus-0.0.5/olympus/management/commands/push_to_es.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:05:28.954333 django-olympus-0.0.5/olympus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-27 11:05:18.000000 django-olympus-0.0.5/olympus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-27 11:05:28.954333 django-olympus-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:05:18.000000 django-olympus-0.0.5/setup.py
```

### Comparing `django-olympus-0.0.4/LICENSE` & `django-olympus-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-olympus-0.0.4/PKG-INFO` & `django-olympus-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-olympus
-Version: 0.0.4
+Version: 0.0.5
 Summary: Collect data from django models into ElasticSearch
 Home-page: https://github.com/surface-security/django-olympus
 Author: PPB - InfoSec Engineering
 Author-email: surface@paddypowerbetfair.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-olympus-0.0.4/README.md` & `django-olympus-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `django-olympus-0.0.4/django_olympus.egg-info/PKG-INFO` & `django-olympus-0.0.5/django_olympus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-olympus
-Version: 0.0.4
+Version: 0.0.5
 Summary: Collect data from django models into ElasticSearch
 Home-page: https://github.com/surface-security/django-olympus
 Author: PPB - InfoSec Engineering
 Author-email: surface@paddypowerbetfair.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `django-olympus-0.0.4/olympus/apps.py` & `django-olympus-0.0.5/olympus/apps.py`

 * *Files identical despite different names*

### Comparing `django-olympus-0.0.4/olympus/base.py` & `django-olympus-0.0.5/olympus/base.py`

 * *Files identical despite different names*

### Comparing `django-olympus-0.0.4/olympus/management/commands/push_to_es.py` & `django-olympus-0.0.5/olympus/management/commands/push_to_es.py`

 * *Files identical despite different names*

### Comparing `django-olympus-0.0.4/olympus/tests/__init__.py` & `django-olympus-0.0.5/olympus/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-olympus-0.0.4/setup.cfg` & `django-olympus-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	Topic :: Software Development
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	Django >= 3.0, < 4
+	Django >= 3.0, < 5
 	elasticsearch >= 6.8, < 7
 	tqdm >= 4, < 5
 	django-logbasecommand < 1
 python_requires = >=3.9
 
 [options.packages.find]
 exclude =
```

