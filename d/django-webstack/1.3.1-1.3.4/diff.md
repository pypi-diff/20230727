# Comparing `tmp/django-webstack-1.3.1.tar.gz` & `tmp/django-webstack-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webstack-1.3.1.tar", last modified: Tue Jul 25 06:05:52 2023, max compression
+gzip compressed data, was "django-webstack-1.3.4.tar", last modified: Thu Jul 27 09:26:20 2023, max compression
```

## Comparing `django-webstack-1.3.1.tar` & `django-webstack-1.3.4.tar`

### file list

```diff
@@ -1,53 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.905418 django-webstack-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-25 06:05:35.000000 django-webstack-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-25 06:05:35.000000 django-webstack-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-25 06:05:52.905418 django-webstack-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-25 06:05:35.000000 django-webstack-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.897417 django-webstack-1.3.1/django_webstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-25 06:05:52.000000 django-webstack-1.3.1/django_webstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-25 06:05:52.000000 django-webstack-1.3.1/django_webstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:05:52.000000 django-webstack-1.3.1/django_webstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 06:05:52.000000 django-webstack-1.3.1/django_webstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 06:05:52.000000 django-webstack-1.3.1/django_webstack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:05:52.905418 django-webstack-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-25 06:05:35.000000 django-webstack-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.897417 django-webstack-1.3.1/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.897417 django-webstack-1.3.1/webstack/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/migrations/0002_auto_20230724_1835.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/migrations/0003_auto_20230725_1401.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.893417 django-webstack-1.3.1/webstack/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.893417 django-webstack-1.3.1/webstack/static/webstack/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.893417 django-webstack-1.3.1/webstack/static/webstack/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.901418 django-webstack-1.3.1/webstack/static/webstack/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/css/nav.css
--rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-components.css
--rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-core.css
--rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-forms.css
--rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-skins.css
--rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.901418 django-webstack-1.3.1/webstack/static/webstack/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/images/favicon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/images/logo-collapsed@2x.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/images/logo@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/images/preview.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.905418 django-webstack-1.3.1/webstack/static/webstack/assets/js/
--rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/TweenMax.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/joinable.js
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/lozad.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/resizeable.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/xenon-api.js
--rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/xenon-custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/static/webstack/assets/js/xenon-toggles.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.893417 django-webstack-1.3.1/webstack/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:52.905418 django-webstack-1.3.1/webstack/templates/webstack/
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/templates/webstack/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/templates/webstack/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-25 06:05:35.000000 django-webstack-1.3.1/webstack/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.488070 django-webstack-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-27 09:26:10.000000 django-webstack-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 09:26:10.000000 django-webstack-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-27 09:26:20.488070 django-webstack-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-27 09:26:10.000000 django-webstack-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.480069 django-webstack-1.3.4/django_webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:10.000000 django-webstack-1.3.4/django_webstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-27 09:26:10.000000 django-webstack-1.3.4/django_webstack/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-27 09:26:10.000000 django-webstack-1.3.4/django_webstack/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-27 09:26:10.000000 django-webstack-1.3.4/django_webstack/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.480069 django-webstack-1.3.4/django_webstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-27 09:26:20.000000 django-webstack-1.3.4/django_webstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-27 09:26:20.000000 django-webstack-1.3.4/django_webstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:26:20.000000 django-webstack-1.3.4/django_webstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 09:26:20.000000 django-webstack-1.3.4/django_webstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 09:26:20.000000 django-webstack-1.3.4/django_webstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 09:26:20.488070 django-webstack-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-27 09:26:10.000000 django-webstack-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.480069 django-webstack-1.3.4/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.484069 django-webstack-1.3.4/webstack/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/migrations/0002_auto_20230724_1835.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/migrations/0003_auto_20230725_1401.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.476069 django-webstack-1.3.4/webstack/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.476069 django-webstack-1.3.4/webstack/static/webstack/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.476069 django-webstack-1.3.4/webstack/static/webstack/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.484069 django-webstack-1.3.4/webstack/static/webstack/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/css/nav.css
+-rw-r--r--   0 runner    (1001) docker     (123)   178177 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/css/xenon-components.css
+-rw-r--r--   0 runner    (1001) docker     (123)   213030 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/css/xenon-core.css
+-rw-r--r--   0 runner    (1001) docker     (123)    58514 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/css/xenon-forms.css
+-rw-r--r--   0 runner    (1001) docker     (123)   288245 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/css/xenon-skins.css
+-rw-r--r--   0 runner    (1001) docker     (123)   699452 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/css/xenon.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.484069 django-webstack-1.3.4/webstack/static/webstack/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/images/favicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1260 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/images/logo-collapsed@2x.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/images/logo@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1392068 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/images/preview.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.488070 django-webstack-1.3.4/webstack/static/webstack/assets/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    98785 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/js/TweenMax.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/js/joinable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/js/lozad.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/js/resizeable.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/js/xenon-api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44384 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/js/xenon-custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/static/webstack/assets/js/xenon-toggles.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.476069 django-webstack-1.3.4/webstack/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:26:20.488070 django-webstack-1.3.4/webstack/templates/webstack/
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/templates/webstack/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/templates/webstack/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-27 09:26:10.000000 django-webstack-1.3.4/webstack/views.py
```

### Comparing `django-webstack-1.3.1/LICENSE` & `django-webstack-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/PKG-INFO` & `django-webstack-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.3.1
+Version: 1.3.4
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `django-webstack-1.3.1/README.md` & `django-webstack-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/django_webstack.egg-info/PKG-INFO` & `django-webstack-1.3.4/django_webstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webstack
-Version: 1.3.1
+Version: 1.3.4
 Summary: webstack of Django
 Home-page: https://github.com/Hopetree/django-webstack
 Author: Hopetree
 Author-email: zlwork2014@163.com
 Keywords: django webstack navigation
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `django-webstack-1.3.1/django_webstack.egg-info/SOURCES.txt` & `django-webstack-1.3.4/django_webstack.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+django_webstack/__init__.py
+django_webstack/settings.py
+django_webstack/urls.py
+django_webstack/wsgi.py
 django_webstack.egg-info/PKG-INFO
 django_webstack.egg-info/SOURCES.txt
 django_webstack.egg-info/dependency_links.txt
 django_webstack.egg-info/requires.txt
 django_webstack.egg-info/top_level.txt
 webstack/__init__.py
 webstack/admin.py
```

### Comparing `django-webstack-1.3.1/setup.py` & `django-webstack-1.3.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding:utf-8 -*-
 # Author: https://github.com/Hopetree
 # Date: 2023/7/24
 from setuptools import find_packages, setup
 
-VERSION = '1.3.1'
+# 这里的版本号根据tag去动态设置
+VERSION = '1.3.4'
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='django-webstack',
     version=VERSION,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-webstack-1.3.1/webstack/admin.py` & `django-webstack-1.3.4/webstack/admin.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/migrations/0001_initial.py` & `django-webstack-1.3.4/webstack/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/migrations/0002_auto_20230724_1835.py` & `django-webstack-1.3.4/webstack/migrations/0002_auto_20230724_1835.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/migrations/0003_auto_20230725_1401.py` & `django-webstack-1.3.4/webstack/migrations/0003_auto_20230725_1401.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/models.py` & `django-webstack-1.3.4/webstack/models.py`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/css/nav.css` & `django-webstack-1.3.4/webstack/static/webstack/assets/css/nav.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-components.css` & `django-webstack-1.3.4/webstack/static/webstack/assets/css/xenon-components.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-core.css` & `django-webstack-1.3.4/webstack/static/webstack/assets/css/xenon-core.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-forms.css` & `django-webstack-1.3.4/webstack/static/webstack/assets/css/xenon-forms.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon-skins.css` & `django-webstack-1.3.4/webstack/static/webstack/assets/css/xenon-skins.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/css/xenon.css` & `django-webstack-1.3.4/webstack/static/webstack/assets/css/xenon.css`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/images/favicon.png` & `django-webstack-1.3.4/webstack/static/webstack/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/images/logo-collapsed@2x.png` & `django-webstack-1.3.4/webstack/static/webstack/assets/images/logo-collapsed@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/images/logo@2x.png` & `django-webstack-1.3.4/webstack/static/webstack/assets/images/logo@2x.png`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/images/preview.gif` & `django-webstack-1.3.4/webstack/static/webstack/assets/images/preview.gif`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/js/TweenMax.min.js` & `django-webstack-1.3.4/webstack/static/webstack/assets/js/TweenMax.min.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/js/joinable.js` & `django-webstack-1.3.4/webstack/static/webstack/assets/js/joinable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/js/lozad.js` & `django-webstack-1.3.4/webstack/static/webstack/assets/js/lozad.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/js/resizeable.js` & `django-webstack-1.3.4/webstack/static/webstack/assets/js/resizeable.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/js/xenon-api.js` & `django-webstack-1.3.4/webstack/static/webstack/assets/js/xenon-api.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/js/xenon-custom.js` & `django-webstack-1.3.4/webstack/static/webstack/assets/js/xenon-custom.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/static/webstack/assets/js/xenon-toggles.js` & `django-webstack-1.3.4/webstack/static/webstack/assets/js/xenon-toggles.js`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/templates/webstack/base.html` & `django-webstack-1.3.4/webstack/templates/webstack/base.html`

 * *Files identical despite different names*

### Comparing `django-webstack-1.3.1/webstack/templates/webstack/index.html` & `django-webstack-1.3.4/webstack/templates/webstack/index.html`

 * *Files identical despite different names*

