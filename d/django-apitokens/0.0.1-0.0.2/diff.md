# Comparing `tmp/django-apitokens-0.0.1.tar.gz` & `tmp/django-apitokens-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-apitokens-0.0.1.tar", last modified: Thu Mar 30 11:18:59 2023, max compression
+gzip compressed data, was "django-apitokens-0.0.2.tar", last modified: Thu Jul 27 10:46:26 2023, max compression
```

## Comparing `django-apitokens-0.0.1.tar` & `django-apitokens-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.180194 django-apitokens-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.176194 django-apitokens-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.180194 django-apitokens-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-03-30 11:18:59.180194 django-apitokens-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.180194 django-apitokens-0.0.1/apitokens/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/apitokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/apitokens/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/apitokens/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.180194 django-apitokens-0.0.1/apitokens/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/apitokens/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/apitokens/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/apitokens/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.176194 django-apitokens-0.0.1/apitokens/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.176194 django-apitokens-0.0.1/apitokens/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.176194 django-apitokens-0.0.1/apitokens/templates/admin/apitokens/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.180194 django-apitokens-0.0.1/apitokens/templates/admin/apitokens/mytoken/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/apitokens/templates/admin/apitokens/mytoken/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.180194 django-apitokens-0.0.1/apitokens/templates/admin/apitokens/token/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/apitokens/templates/admin/apitokens/token/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.180194 django-apitokens-0.0.1/django_apitokens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-03-30 11:18:59.000000 django-apitokens-0.0.1/django_apitokens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-30 11:18:59.000000 django-apitokens-0.0.1/django_apitokens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 11:18:59.000000 django-apitokens-0.0.1/django_apitokens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-30 11:18:59.000000 django-apitokens-0.0.1/django_apitokens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-30 11:18:59.000000 django-apitokens-0.0.1/django_apitokens.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 11:18:59.180194 django-apitokens-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.180194 django-apitokens-0.0.1/testapp/
--rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/testapp/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/testapp/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:59.180194 django-apitokens-0.0.1/testapp/testapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/testapp/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/testapp/testapp/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/testapp/testapp/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/testapp/testapp/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-30 11:18:42.000000 django-apitokens-0.0.1/testapp/testapp/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.741248 django-apitokens-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.733248 django-apitokens-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.737248 django-apitokens-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-27 10:46:26.737248 django-apitokens-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.737248 django-apitokens-0.0.2/apitokens/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/apitokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/apitokens/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/apitokens/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.737248 django-apitokens-0.0.2/apitokens/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/apitokens/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/apitokens/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/apitokens/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.733248 django-apitokens-0.0.2/apitokens/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.733248 django-apitokens-0.0.2/apitokens/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.733248 django-apitokens-0.0.2/apitokens/templates/admin/apitokens/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.737248 django-apitokens-0.0.2/apitokens/templates/admin/apitokens/mytoken/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/apitokens/templates/admin/apitokens/mytoken/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.737248 django-apitokens-0.0.2/apitokens/templates/admin/apitokens/token/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/apitokens/templates/admin/apitokens/token/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.737248 django-apitokens-0.0.2/django_apitokens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-27 10:46:26.000000 django-apitokens-0.0.2/django_apitokens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-27 10:46:26.000000 django-apitokens-0.0.2/django_apitokens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:46:26.000000 django-apitokens-0.0.2/django_apitokens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 10:46:26.000000 django-apitokens-0.0.2/django_apitokens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 10:46:26.000000 django-apitokens-0.0.2/django_apitokens.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 10:46:26.741248 django-apitokens-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.737248 django-apitokens-0.0.2/testapp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/testapp/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/testapp/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.737248 django-apitokens-0.0.2/testapp/testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/testapp/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/testapp/testapp/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/testapp/testapp/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.733248 django-apitokens-0.0.2/testapp/testapp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:46:26.737248 django-apitokens-0.0.2/testapp/testapp/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/testapp/testapp/templates/admin/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/testapp/testapp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-27 10:46:11.000000 django-apitokens-0.0.2/testapp/testapp/wsgi.py
```

### Comparing `django-apitokens-0.0.1/.github/workflows/publish.yml` & `django-apitokens-0.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `django-apitokens-0.0.1/.github/workflows/publish_test.yml` & `django-apitokens-0.0.2/.github/workflows/publish_test.yml`

 * *Files identical despite different names*

### Comparing `django-apitokens-0.0.1/.gitignore` & `django-apitokens-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django-apitokens-0.0.1/LICENSE` & `django-apitokens-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-apitokens-0.0.1/PKG-INFO` & `django-apitokens-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-apitokens
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate API tokens for django-restframework
 Author-email: InfoSec Engineering <surface@paddypowerbetfair.com>
 License: MIT
 Keywords: django,api,restframework,tokens,self-service
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-apitokens-0.0.1/README.md` & `django-apitokens-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-apitokens-0.0.1/apitokens/admin.py` & `django-apitokens-0.0.2/apitokens/admin.py`

 * *Files identical despite different names*

### Comparing `django-apitokens-0.0.1/apitokens/migrations/0001_initial.py` & `django-apitokens-0.0.2/apitokens/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-apitokens-0.0.1/apitokens/models.py` & `django-apitokens-0.0.2/apitokens/models.py`

 * *Files identical despite different names*

### Comparing `django-apitokens-0.0.1/apitokens/templates/admin/apitokens/mytoken/change_list.html` & `django-apitokens-0.0.2/apitokens/templates/admin/apitokens/mytoken/change_list.html`

 * *Files identical despite different names*

### Comparing `django-apitokens-0.0.1/django_apitokens.egg-info/PKG-INFO` & `django-apitokens-0.0.2/django_apitokens.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-apitokens
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate API tokens for django-restframework
 Author-email: InfoSec Engineering <surface@paddypowerbetfair.com>
 License: MIT
 Keywords: django,api,restframework,tokens,self-service
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-apitokens-0.0.1/django_apitokens.egg-info/SOURCES.txt` & `django-apitokens-0.0.2/django_apitokens.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 django_apitokens.egg-info/top_level.txt
 testapp/manage.py
 testapp/requirements.txt
 testapp/testapp/__init__.py
 testapp/testapp/asgi.py
 testapp/testapp/settings.py
 testapp/testapp/urls.py
-testapp/testapp/wsgi.py
+testapp/testapp/wsgi.py
+testapp/testapp/templates/admin/base.html
```

### Comparing `django-apitokens-0.0.1/pyproject.toml` & `django-apitokens-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
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
     "django-rest-knox == 4.2.0",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "apitokens.__version__"}
 
 [tool.setuptools]
```

### Comparing `django-apitokens-0.0.1/testapp/manage.py` & `django-apitokens-0.0.2/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `django-apitokens-0.0.1/testapp/testapp/settings.py` & `django-apitokens-0.0.2/testapp/testapp/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,25 @@
 """
 
 from pathlib import Path
 
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent.parent
 
-
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/3.2/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = 'django-insecure-5d&l457uxd83a^)z*ew=*!#1udp^he_nx3ps*4*p#^y)db@q1z'
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
 ALLOWED_HOSTS = []
 
-
 # Application definition
 
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
@@ -52,41 +50,39 @@
 ]
 
 ROOT_URLCONF = 'testapp.urls'
 
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': [],
+        'DIRS': [BASE_DIR / 'testapp' / 'templates'],
         'APP_DIRS': True,
         'OPTIONS': {
             'context_processors': [
                 'django.template.context_processors.debug',
                 'django.template.context_processors.request',
                 'django.contrib.auth.context_processors.auth',
                 'django.contrib.messages.context_processors.messages',
             ],
         },
     },
 ]
 
 WSGI_APPLICATION = 'testapp.wsgi.application'
 
-
 # Database
 # https://docs.djangoproject.com/en/3.2/ref/settings/#databases
 
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.sqlite3',
         'NAME': BASE_DIR / 'db.sqlite3',
     }
 }
 
-
 # Password validation
 # https://docs.djangoproject.com/en/3.2/ref/settings/#auth-password-validators
 
 AUTH_PASSWORD_VALIDATORS = [
     {
         'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',
     },
@@ -97,29 +93,27 @@
         'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator',
     },
     {
         'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator',
     },
 ]
 
-
 # Internationalization
 # https://docs.djangoproject.com/en/3.2/topics/i18n/
 
 LANGUAGE_CODE = 'en-us'
 
 TIME_ZONE = 'UTC'
 
 USE_I18N = True
 
 USE_L10N = True
 
 USE_TZ = True
 
-
 # Static files (CSS, JavaScript, Images)
 # https://docs.djangoproject.com/en/3.2/howto/static-files/
 
 STATIC_URL = '/static/'
 
 # Default primary key field type
 # https://docs.djangoproject.com/en/3.2/ref/settings/#default-auto-field
```

### Comparing `django-apitokens-0.0.1/testapp/testapp/urls.py` & `django-apitokens-0.0.2/testapp/testapp/urls.py`

 * *Files identical despite different names*

