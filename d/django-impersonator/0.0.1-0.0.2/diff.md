# Comparing `tmp/django-impersonator-0.0.1.tar.gz` & `tmp/django-impersonator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-impersonator-0.0.1.tar", last modified: Thu Mar 30 10:32:39 2023, max compression
+gzip compressed data, was "django-impersonator-0.0.2.tar", last modified: Thu Jul 27 12:43:05 2023, max compression
```

## Comparing `django-impersonator-0.0.1.tar` & `django-impersonator-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:39.130748 django-impersonator-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:39.126748 django-impersonator-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:39.126748 django-impersonator-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-30 10:32:39.130748 django-impersonator-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:39.130748 django-impersonator-0.0.1/django_impersonator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-30 10:32:39.000000 django-impersonator-0.0.1/django_impersonator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-30 10:32:39.000000 django-impersonator-0.0.1/django_impersonator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 10:32:39.000000 django-impersonator-0.0.1/django_impersonator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 10:32:39.000000 django-impersonator-0.0.1/django_impersonator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-30 10:32:39.000000 django-impersonator-0.0.1/django_impersonator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:39.130748 django-impersonator-0.0.1/impersonate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/impersonate/__init__,py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/impersonate/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/impersonate/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:39.126748 django-impersonator-0.0.1/impersonate/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:39.130748 django-impersonator-0.0.1/impersonate/templates/impersonate/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/impersonate/templates/impersonate/popup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 10:32:39.130748 django-impersonator-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:39.130748 django-impersonator-0.0.1/testapp/
--rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:39.130748 django-impersonator-0.0.1/testapp/testapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/testapp/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/testapp/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:39.130748 django-impersonator-0.0.1/testapp/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/testapp/migrations/0001_create_users.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/testapp/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/testapp/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/testapp/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:39.130748 django-impersonator-0.0.1/testapp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-30 10:32:15.000000 django-impersonator-0.0.1/testapp/tests/test_generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:43:05.159291 django-impersonator-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:43:05.155291 django-impersonator-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:43:05.159291 django-impersonator-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-27 12:43:05.159291 django-impersonator-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:43:05.159291 django-impersonator-0.0.2/django_impersonator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-27 12:43:05.000000 django-impersonator-0.0.2/django_impersonator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-27 12:43:05.000000 django-impersonator-0.0.2/django_impersonator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:43:05.000000 django-impersonator-0.0.2/django_impersonator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 12:43:05.000000 django-impersonator-0.0.2/django_impersonator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 12:43:05.000000 django-impersonator-0.0.2/django_impersonator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:43:05.159291 django-impersonator-0.0.2/impersonate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/impersonate/__init__,py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/impersonate/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/impersonate/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:43:05.155291 django-impersonator-0.0.2/impersonate/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:43:05.159291 django-impersonator-0.0.2/impersonate/templates/impersonate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/impersonate/templates/impersonate/popup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:43:05.159291 django-impersonator-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:43:05.159291 django-impersonator-0.0.2/testapp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:43:05.159291 django-impersonator-0.0.2/testapp/testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/testapp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/testapp/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:43:05.159291 django-impersonator-0.0.2/testapp/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/testapp/migrations/0001_create_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/testapp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/testapp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/testapp/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:43:05.159291 django-impersonator-0.0.2/testapp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-27 12:42:48.000000 django-impersonator-0.0.2/testapp/tests/test_generic.py
```

### Comparing `django-impersonator-0.0.1/.github/workflows/publish.yml` & `django-impersonator-0.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/.github/workflows/publish_test.yml` & `django-impersonator-0.0.2/.github/workflows/publish_test.yml`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/.gitignore` & `django-impersonator-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/LICENSE` & `django-impersonator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/PKG-INFO` & `django-impersonator-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-impersonator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Impersonate middleware to let you impersonate other users.
 Author-email: InfoSec Engineering <surface@paddypowerbetfair.com>
 License: MIT
 Keywords: django,impersonate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-impersonator-0.0.1/README.md` & `django-impersonator-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/django_impersonator.egg-info/PKG-INFO` & `django-impersonator-0.0.2/django_impersonator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-impersonator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Impersonate middleware to let you impersonate other users.
 Author-email: InfoSec Engineering <surface@paddypowerbetfair.com>
 License: MIT
 Keywords: django,impersonate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-impersonator-0.0.1/django_impersonator.egg-info/SOURCES.txt` & `django-impersonator-0.0.2/django_impersonator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/impersonate/admin.py` & `django-impersonator-0.0.2/impersonate/admin.py`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/impersonate/middleware.py` & `django-impersonator-0.0.2/impersonate/middleware.py`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/impersonate/templates/impersonate/popup.html` & `django-impersonator-0.0.2/impersonate/templates/impersonate/popup.html`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/pyproject.toml` & `django-impersonator-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-impersonator"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "InfoSec Engineering", email = "surface@paddypowerbetfair.com"},
 ]
 description = "Impersonate middleware to let you impersonate other users."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["django", "impersonate"]
@@ -20,15 +20,15 @@
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Environment :: Web Environment",
     "Topic :: Software Development",
 ]
 dependencies = [
-    "Django >= 3.1, < 4.0",
+    "Django >= 3.1, < 5.0",
 ]
 
 [project.optional-dependencies]
 dev = ["black==23.1.0", "ruff==0.0.256"]
 
 [tool.setuptools]
 packages = ["impersonate"]
```

### Comparing `django-impersonator-0.0.1/testapp/manage.py` & `django-impersonator-0.0.2/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/testapp/testapp/migrations/0001_create_users.py` & `django-impersonator-0.0.2/testapp/testapp/migrations/0001_create_users.py`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/testapp/testapp/settings.py` & `django-impersonator-0.0.2/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/testapp/testapp/urls.py` & `django-impersonator-0.0.2/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `django-impersonator-0.0.1/testapp/tests/test_generic.py` & `django-impersonator-0.0.2/testapp/tests/test_generic.py`

 * *Files identical despite different names*

