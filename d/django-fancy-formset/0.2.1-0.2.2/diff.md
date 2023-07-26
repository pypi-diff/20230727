# Comparing `tmp/django-fancy-formset-0.2.1.tar.gz` & `tmp/django-fancy-formset-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-fancy-formset-0.2.1.tar", last modified: Wed Jul 26 22:20:44 2023, max compression
+gzip compressed data, was "django-fancy-formset-0.2.2.tar", last modified: Wed Jul 26 23:09:57 2023, max compression
```

## Comparing `django-fancy-formset-0.2.1.tar` & `django-fancy-formset-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.826683 django-fancy-formset-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-26 22:20:44.826683 django-fancy-formset-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.822683 django-fancy-formset-0.2.1/django_fancy_formset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-26 22:20:44.000000 django-fancy-formset-0.2.1/django_fancy_formset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-26 22:20:44.000000 django-fancy-formset-0.2.1/django_fancy_formset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:20:44.000000 django-fancy-formset-0.2.1/django_fancy_formset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 22:20:44.000000 django-fancy-formset-0.2.1/django_fancy_formset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 22:20:44.000000 django-fancy-formset-0.2.1/django_fancy_formset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.822683 django-fancy-formset-0.2.1/fancy_formset/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/formsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.822683 django-fancy-formset-0.2.1/fancy_formset/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.822683 django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-26 22:20:37.000000 django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.css
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-26 22:20:37.000000 django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.js
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-26 22:20:37.000000 django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-26 22:20:37.000000 django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.822683 django-fancy-formset-0.2.1/fancy_formset/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.826683 django-fancy-formset-0.2.1/fancy_formset/templates/fancy_formset/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/templates/fancy_formset/default.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/templates/fancy_formset/div.html
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/templates/fancy_formset/p.html
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/templates/fancy_formset/table.html
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/templates/fancy_formset/ul.html
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:20:44.826683 django-fancy-formset-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:09:57.080984 django-fancy-formset-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-26 23:09:45.000000 django-fancy-formset-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-26 23:09:45.000000 django-fancy-formset-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-26 23:09:57.080984 django-fancy-formset-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-26 23:09:45.000000 django-fancy-formset-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:09:57.080984 django-fancy-formset-0.2.2/django_fancy_formset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-26 23:09:57.000000 django-fancy-formset-0.2.2/django_fancy_formset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-26 23:09:57.000000 django-fancy-formset-0.2.2/django_fancy_formset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:09:57.000000 django-fancy-formset-0.2.2/django_fancy_formset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 23:09:57.000000 django-fancy-formset-0.2.2/django_fancy_formset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 23:09:57.000000 django-fancy-formset-0.2.2/django_fancy_formset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:09:57.080984 django-fancy-formset-0.2.2/fancy_formset/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 23:09:45.000000 django-fancy-formset-0.2.2/fancy_formset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-26 23:09:45.000000 django-fancy-formset-0.2.2/fancy_formset/formsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:09:57.076984 django-fancy-formset-0.2.2/fancy_formset/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:09:57.080984 django-fancy-formset-0.2.2/fancy_formset/static/fancy_formset/
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-26 23:09:50.000000 django-fancy-formset-0.2.2/fancy_formset/static/fancy_formset/formset.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-26 23:09:50.000000 django-fancy-formset-0.2.2/fancy_formset/static/fancy_formset/formset.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-26 23:09:50.000000 django-fancy-formset-0.2.2/fancy_formset/static/fancy_formset/formset.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-26 23:09:50.000000 django-fancy-formset-0.2.2/fancy_formset/static/fancy_formset/formset.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:09:57.076984 django-fancy-formset-0.2.2/fancy_formset/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:09:57.080984 django-fancy-formset-0.2.2/fancy_formset/templates/fancy_formset/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-26 23:09:45.000000 django-fancy-formset-0.2.2/fancy_formset/templates/fancy_formset/default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-26 23:09:45.000000 django-fancy-formset-0.2.2/fancy_formset/templates/fancy_formset/div.html
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-26 23:09:45.000000 django-fancy-formset-0.2.2/fancy_formset/templates/fancy_formset/p.html
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-26 23:09:45.000000 django-fancy-formset-0.2.2/fancy_formset/templates/fancy_formset/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-26 23:09:45.000000 django-fancy-formset-0.2.2/fancy_formset/templates/fancy_formset/ul.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-26 23:09:45.000000 django-fancy-formset-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:09:57.080984 django-fancy-formset-0.2.2/setup.cfg
```

### Comparing `django-fancy-formset-0.2.1/LICENSE` & `django-fancy-formset-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.1/PKG-INFO` & `django-fancy-formset-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fancy-formset
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Django app and pure JavaScript library to manage formsets
 Author-email: Richard Terry <code@radiac.net>
 Project-URL: Homepage, https://radiac.net/projects/django-fancy-formset/
 Project-URL: Documentation, https://django-fancy-formset.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/radiac/django-fancy-formset
 Project-URL: NPM, https://www.npmjs.com/package/django-fancy-formset
 Project-URL: Bug Tracker, https://github.com/radiac/django-fancy-formset/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-fancy-formset Version: 0.2.1 Summary: A
+Metadata-Version: 2.1 Name: django-fancy-formset Version: 0.2.2 Summary: A
 Django app and pure JavaScript library to manage formsets Author-email: Richard
 Terry
 radiac.net> Project-URL: Homepage, https://radiac.net/projects/django-fancy-
 formset/ Project-URL: Documentation, https://django-fancy-
 formset.readthedocs.io/en/latest/ Project-URL: Source, https://github.com/
 radiac/django-fancy-formset Project-URL: NPM, https://www.npmjs.com/package/
 django-fancy-formset Project-URL: Bug Tracker, https://github.com/radiac/
```

### Comparing `django-fancy-formset-0.2.1/README.md` & `django-fancy-formset-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.1/django_fancy_formset.egg-info/PKG-INFO` & `django-fancy-formset-0.2.2/django_fancy_formset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fancy-formset
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Django app and pure JavaScript library to manage formsets
 Author-email: Richard Terry <code@radiac.net>
 Project-URL: Homepage, https://radiac.net/projects/django-fancy-formset/
 Project-URL: Documentation, https://django-fancy-formset.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/radiac/django-fancy-formset
 Project-URL: NPM, https://www.npmjs.com/package/django-fancy-formset
 Project-URL: Bug Tracker, https://github.com/radiac/django-fancy-formset/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-fancy-formset Version: 0.2.1 Summary: A
+Metadata-Version: 2.1 Name: django-fancy-formset Version: 0.2.2 Summary: A
 Django app and pure JavaScript library to manage formsets Author-email: Richard
 Terry
 radiac.net> Project-URL: Homepage, https://radiac.net/projects/django-fancy-
 formset/ Project-URL: Documentation, https://django-fancy-
 formset.readthedocs.io/en/latest/ Project-URL: Source, https://github.com/
 radiac/django-fancy-formset Project-URL: NPM, https://www.npmjs.com/package/
 django-fancy-formset Project-URL: Bug Tracker, https://github.com/radiac/
```

### Comparing `django-fancy-formset-0.2.1/django_fancy_formset.egg-info/SOURCES.txt` & `django-fancy-formset-0.2.2/django_fancy_formset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.1/fancy_formset/formsets.py` & `django-fancy-formset-0.2.2/fancy_formset/formsets.py`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.css` & `django-fancy-formset-0.2.2/fancy_formset/static/fancy_formset/formset.css`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.js` & `django-fancy-formset-0.2.2/fancy_formset/static/fancy_formset/formset.js`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.min.css` & `django-fancy-formset-0.2.2/fancy_formset/static/fancy_formset/formset.min.css`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.module.js` & `django-fancy-formset-0.2.2/fancy_formset/static/fancy_formset/formset.module.js`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.1/pyproject.toml` & `django-fancy-formset-0.2.2/pyproject.toml`

 * *Files identical despite different names*

