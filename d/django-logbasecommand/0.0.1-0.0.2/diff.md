# Comparing `tmp/django-logbasecommand-0.0.1.tar.gz` & `tmp/django-logbasecommand-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-logbasecommand-0.0.1.tar", last modified: Mon Jan 17 12:44:40 2022, max compression
+gzip compressed data, was "django-logbasecommand-0.0.2.tar", last modified: Thu Jul 27 11:07:53 2023, max compression
```

## Comparing `django-logbasecommand-0.0.1.tar` & `django-logbasecommand-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 12:44:40.749714 django-logbasecommand-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-01-17 12:44:29.000000 django-logbasecommand-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-01-17 12:44:29.000000 django-logbasecommand-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3346 2022-01-17 12:44:40.749714 django-logbasecommand-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-01-17 12:44:29.000000 django-logbasecommand-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 12:44:40.749714 django-logbasecommand-0.0.1/django_logbasecommand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3346 2022-01-17 12:44:40.000000 django-logbasecommand-0.0.1/django_logbasecommand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-01-17 12:44:40.000000 django-logbasecommand-0.0.1/django_logbasecommand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-17 12:44:40.000000 django-logbasecommand-0.0.1/django_logbasecommand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-17 12:44:40.000000 django-logbasecommand-0.0.1/django_logbasecommand.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-17 12:44:40.000000 django-logbasecommand-0.0.1/django_logbasecommand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-17 12:44:40.000000 django-logbasecommand-0.0.1/django_logbasecommand.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 12:44:40.749714 django-logbasecommand-0.0.1/logbasecommand/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-17 12:44:29.000000 django-logbasecommand-0.0.1/logbasecommand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-01-17 12:44:29.000000 django-logbasecommand-0.0.1/logbasecommand/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-01-17 12:44:40.749714 django-logbasecommand-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-17 12:44:29.000000 django-logbasecommand-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:07:53.505845 django-logbasecommand-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 11:07:43.000000 django-logbasecommand-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-27 11:07:43.000000 django-logbasecommand-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-27 11:07:53.505845 django-logbasecommand-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-27 11:07:43.000000 django-logbasecommand-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:07:53.505845 django-logbasecommand-0.0.2/django_logbasecommand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-27 11:07:53.000000 django-logbasecommand-0.0.2/django_logbasecommand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-27 11:07:53.000000 django-logbasecommand-0.0.2/django_logbasecommand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:07:53.000000 django-logbasecommand-0.0.2/django_logbasecommand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:07:53.000000 django-logbasecommand-0.0.2/django_logbasecommand.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:07:53.000000 django-logbasecommand-0.0.2/django_logbasecommand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:07:53.000000 django-logbasecommand-0.0.2/django_logbasecommand.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:07:53.505845 django-logbasecommand-0.0.2/logbasecommand/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 11:07:43.000000 django-logbasecommand-0.0.2/logbasecommand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-27 11:07:43.000000 django-logbasecommand-0.0.2/logbasecommand/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-27 11:07:53.505845 django-logbasecommand-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:07:43.000000 django-logbasecommand-0.0.2/setup.py
```

### Comparing `django-logbasecommand-0.0.1/LICENSE` & `django-logbasecommand-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-logbasecommand-0.0.1/PKG-INFO` & `django-logbasecommand-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: django-logbasecommand
-Version: 0.0.1
+Version: 0.0.2
 Summary: Minimal package to add logging helpers to Django management commands
 Home-page: https://github.com/surface-security/django-logbasecommand/
 Author: PPB - InfoSec Engineering
 Author-email: surface@paddypowerbetfair.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Environment :: Web Environment
 Classifier: Topic :: Software Development
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-logbasecommand
 
 Minimal package to add logging helpers to Django management commands
 
@@ -103,8 +102,7 @@
             'handlers': ['console_minimal', 'console_debug_minimal'],
             'level': 'DEBUG',
             'propagate': False,
         },
     },
 }
 ```
-
```

### Comparing `django-logbasecommand-0.0.1/README.md` & `django-logbasecommand-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-logbasecommand-0.0.1/django_logbasecommand.egg-info/PKG-INFO` & `django-logbasecommand-0.0.2/django_logbasecommand.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: django-logbasecommand
-Version: 0.0.1
+Version: 0.0.2
 Summary: Minimal package to add logging helpers to Django management commands
 Home-page: https://github.com/surface-security/django-logbasecommand/
 Author: PPB - InfoSec Engineering
 Author-email: surface@paddypowerbetfair.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Environment :: Web Environment
 Classifier: Topic :: Software Development
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-logbasecommand
 
 Minimal package to add logging helpers to Django management commands
 
@@ -103,8 +102,7 @@
             'handlers': ['console_minimal', 'console_debug_minimal'],
             'level': 'DEBUG',
             'propagate': False,
         },
     },
 }
 ```
-
```

### Comparing `django-logbasecommand-0.0.1/logbasecommand/base.py` & `django-logbasecommand-0.0.2/logbasecommand/base.py`

 * *Files identical despite different names*

### Comparing `django-logbasecommand-0.0.1/setup.cfg` & `django-logbasecommand-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 	Topic :: Software Development
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	Django >= 3.0, < 4
-python_requires = >=3.6
+	Django >= 3.0, < 5
+python_requires = >=3.9
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 
 [coverage:run]
```

