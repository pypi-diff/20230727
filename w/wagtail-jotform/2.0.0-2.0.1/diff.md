# Comparing `tmp/wagtail-jotform-2.0.0.tar.gz` & `tmp/wagtail-jotform-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-jotform-2.0.0.tar", last modified: Mon Oct 24 15:35:27 2022, max compression
+gzip compressed data, was "wagtail-jotform-2.0.1.tar", last modified: Thu Jul 27 10:04:14 2023, max compression
```

## Comparing `wagtail-jotform-2.0.0.tar` & `wagtail-jotform-2.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 15:35:27.209979 wagtail-jotform-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3276 2022-10-24 15:35:27.209979 wagtail-jotform-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-10-24 15:35:27.209979 wagtail-jotform-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 15:35:27.209979 wagtail-jotform-2.0.0/wagtail_jotform/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 15:35:27.209979 wagtail-jotform-2.0.0/wagtail_jotform/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/migrations/0002_rename_embedded_form_model.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 15:35:27.209979 wagtail-jotform-2.0.0/wagtail_jotform/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 15:35:27.209979 wagtail-jotform-2.0.0/wagtail_jotform/templates/wagtail_jotform/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/templates/wagtail_jotform/embedded_form_page.html
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/templates/wagtail_jotform/thank_you.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 15:35:27.209979 wagtail-jotform-2.0.0/wagtail_jotform/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 15:35:27.209979 wagtail-jotform-2.0.0/wagtail_jotform/tests/testapp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/tests/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6234 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2221 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-10-24 15:35:21.000000 wagtail-jotform-2.0.0/wagtail_jotform/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 15:35:27.209979 wagtail-jotform-2.0.0/wagtail_jotform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3276 2022-10-24 15:35:27.000000 wagtail-jotform-2.0.0/wagtail_jotform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-10-24 15:35:27.000000 wagtail-jotform-2.0.0/wagtail_jotform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 15:35:27.000000 wagtail-jotform-2.0.0/wagtail_jotform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-24 15:35:27.000000 wagtail-jotform-2.0.0/wagtail_jotform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-24 15:35:27.000000 wagtail-jotform-2.0.0/wagtail_jotform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:04:14.926427 wagtail-jotform-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-27 10:04:14.926427 wagtail-jotform-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 10:04:14.926427 wagtail-jotform-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:04:14.922427 wagtail-jotform-2.0.1/wagtail_jotform/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:04:14.922427 wagtail-jotform-2.0.1/wagtail_jotform/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/migrations/0002_rename_embedded_form_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:04:14.922427 wagtail-jotform-2.0.1/wagtail_jotform/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:04:14.922427 wagtail-jotform-2.0.1/wagtail_jotform/templates/wagtail_jotform/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/templates/wagtail_jotform/embedded_form_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/templates/wagtail_jotform/thank_you.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:04:14.926427 wagtail-jotform-2.0.1/wagtail_jotform/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:04:14.926427 wagtail-jotform-2.0.1/wagtail_jotform/tests/testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/tests/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 10:04:11.000000 wagtail-jotform-2.0.1/wagtail_jotform/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:04:14.922427 wagtail-jotform-2.0.1/wagtail_jotform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-27 10:04:14.000000 wagtail-jotform-2.0.1/wagtail_jotform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-27 10:04:14.000000 wagtail-jotform-2.0.1/wagtail_jotform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:04:14.000000 wagtail-jotform-2.0.1/wagtail_jotform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-27 10:04:14.000000 wagtail-jotform-2.0.1/wagtail_jotform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 10:04:14.000000 wagtail-jotform-2.0.1/wagtail_jotform.egg-info/top_level.txt
```

### Comparing `wagtail-jotform-2.0.0/PKG-INFO` & `wagtail-jotform-2.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 Metadata-Version: 2.1
 Name: wagtail-jotform
-Version: 2.0.0
+Version: 2.0.1
 Summary: Embed Jotform forms in wagtail.
 Home-page: https://github.com/kevinhowbrook/wagtail-jotform
 Author: Kevin Howbrook
 Author-email: kevin.howbrook@torchbox.com
 License: BSD
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+Provides-Extra: development
 
-![tests](https://github.com/kevinhowbrook/wagtail-jotform/workflows/Tests/badge.svg)
+![tests](https://github.com/torchbox/wagtail-jotform/workflows/Tests/badge.svg)
 [![codecov](https://codecov.io/gh/kevinhowbrook/wagtail-jotform/branch/master/graph/badge.svg?token=GBDM9H1A2X)](https://codecov.io/gh/kevinhowbrook/wagtail-jotform)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Total alerts](https://img.shields.io/lgtm/alerts/g/kevinhowbrook/wagtail-jotform.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/kevinhowbrook/wagtail-jotform/alerts/)
 
 # Wagtail Jotform
 
 Embedable [Jotform](https://www.jotform.com) forms for Wagtail pages.
 
 Wagtail Jotform works by providing a new `EmbeddedFormPage` page type with a form choice field. Values for this form field are populated from the Jotform API.
 
 ## Installation
 
 Install from [pypi](https://pypi.org/project/wagtail-jotform/):
 
-```
+```bash
 pip install wagtail-jotform
 ```
 
 ## Configuration
 
 You will need an API key from Jotform. Add the following variables to your settings:
 
@@ -70,33 +72,25 @@
 
 When a form is created, the Jotform `thankurl` is set with your created form's thank you page URL, e.g. `https://mysite.com/formpage/thank-you`. When the form is submitted, the user will be redirected accordingly and be show the 'thank you' data specified on on the form page added.
 
 ## Overriding templates
 
 Wagtail Jotform has two templates:
 
-```
-embedded_form_page.html
-thank_you.html
-```
+- embedded_form_page.html
+- thank_you.html
 
 You can override these templates in your project by adding them in the following location:
 
-```
-your_project_root/
-  templates/
-    wagtail_jotform/
-        embed_form_page.html
-        thank_you.html
-```
+- your_project_root/
+  - templates/
+    - wagtail_jotform/
+      - embed_form_page.html
+      - thank_you.html
 
-## Tests
+## Contributing
 
-```
-# Install the development environment
-poetry install
-poetry shell
-
-# Run the tests
-coverage run ./runtests.py
-coverage report
-```
+We welcome contributions to this project. Please follow the [contributing instructions](docs/CONTRIBUTING.md) to get started.
+
+## Release process
+
+To release a new version, the [Release documentation](docs/RELEASE.md) should be followed.
```

### Comparing `wagtail-jotform-2.0.0/README.md` & `wagtail-jotform-2.0.1/wagtail_jotform.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,46 @@
-![tests](https://github.com/kevinhowbrook/wagtail-jotform/workflows/Tests/badge.svg)
+Metadata-Version: 2.1
+Name: wagtail-jotform
+Version: 2.0.1
+Summary: Embed Jotform forms in wagtail.
+Home-page: https://github.com/kevinhowbrook/wagtail-jotform
+Author: Kevin Howbrook
+Author-email: kevin.howbrook@torchbox.com
+License: BSD
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: development
+
+![tests](https://github.com/torchbox/wagtail-jotform/workflows/Tests/badge.svg)
 [![codecov](https://codecov.io/gh/kevinhowbrook/wagtail-jotform/branch/master/graph/badge.svg?token=GBDM9H1A2X)](https://codecov.io/gh/kevinhowbrook/wagtail-jotform)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Total alerts](https://img.shields.io/lgtm/alerts/g/kevinhowbrook/wagtail-jotform.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/kevinhowbrook/wagtail-jotform/alerts/)
 
 # Wagtail Jotform
 
 Embedable [Jotform](https://www.jotform.com) forms for Wagtail pages.
 
 Wagtail Jotform works by providing a new `EmbeddedFormPage` page type with a form choice field. Values for this form field are populated from the Jotform API.
 
 ## Installation
 
 Install from [pypi](https://pypi.org/project/wagtail-jotform/):
 
-```
+```bash
 pip install wagtail-jotform
 ```
 
 ## Configuration
 
 You will need an API key from Jotform. Add the following variables to your settings:
 
@@ -48,33 +72,25 @@
 
 When a form is created, the Jotform `thankurl` is set with your created form's thank you page URL, e.g. `https://mysite.com/formpage/thank-you`. When the form is submitted, the user will be redirected accordingly and be show the 'thank you' data specified on on the form page added.
 
 ## Overriding templates
 
 Wagtail Jotform has two templates:
 
-```
-embedded_form_page.html
-thank_you.html
-```
+- embedded_form_page.html
+- thank_you.html
 
 You can override these templates in your project by adding them in the following location:
 
-```
-your_project_root/
-  templates/
-    wagtail_jotform/
-        embed_form_page.html
-        thank_you.html
-```
+- your_project_root/
+  - templates/
+    - wagtail_jotform/
+      - embed_form_page.html
+      - thank_you.html
 
-## Tests
+## Contributing
 
-```
-# Install the development environment
-poetry install
-poetry shell
-
-# Run the tests
-coverage run ./runtests.py
-coverage report
-```
+We welcome contributions to this project. Please follow the [contributing instructions](docs/CONTRIBUTING.md) to get started.
+
+## Release process
+
+To release a new version, the [Release documentation](docs/RELEASE.md) should be followed.
```

### Comparing `wagtail-jotform-2.0.0/wagtail_jotform/migrations/0001_initial.py` & `wagtail-jotform-2.0.1/wagtail_jotform/migrations/0001_initial.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # Generated by Django 3.1.1 on 2020-10-07 08:49
 
 import django.db.models.deletion
 import wagtail.contrib.routable_page.models
-from wagtail import VERSION as WAGTAIL_VERSION
 
-if WAGTAIL_VERSION >= (3, 0):
-    import wagtail.fields as wagtail_fields
-else:
-    import wagtail.core.fields as wagtail_fields
+import wagtail.fields as wagtail_fields
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     initial = True
```

### Comparing `wagtail-jotform-2.0.0/wagtail_jotform/migrations/0002_rename_embedded_form_model.py` & `wagtail-jotform-2.0.1/wagtail_jotform/migrations/0002_rename_embedded_form_model.py`

 * *Files identical despite different names*

### Comparing `wagtail-jotform-2.0.0/wagtail_jotform/models.py` & `wagtail-jotform-2.0.1/wagtail_jotform/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 from django.db import models
 from django.forms.widgets import Select
 from django.shortcuts import render
 
-from wagtail import VERSION as WAGTAIL_VERSION
-
-if WAGTAIL_VERSION >= (3, 0):
-    from wagtail.admin.panels import FieldPanel
-    from wagtail.fields import RichTextField
-    from wagtail.models import Page
-else:
-    from wagtail.admin.edit_handlers import FieldPanel
-    from wagtail.core.fields import RichTextField
-    from wagtail.core.models import Page
-
 from wagtail.admin.forms import WagtailAdminPageForm
+from wagtail.admin.panels import FieldPanel
 from wagtail.contrib.routable_page.models import RoutablePageMixin, route
+from wagtail.fields import RichTextField
+from wagtail.models import Page
 
 from .settings import wagtail_jotform_settings
 from .utils import JotFormAPI
 
 
 def jot_form_choices():
     jot_form_data = []
```

### Comparing `wagtail-jotform-2.0.0/wagtail_jotform/tests/settings.py` & `wagtail-jotform-2.0.1/wagtail_jotform/tests/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import os
 
-from wagtail import VERSION as WAGTAIL_VERSION
-
 PROJECT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 BASE_DIR = os.path.dirname(PROJECT_DIR)
 
 
 SECRET_KEY = "not so secret"
 
 DATABASES = {"default": {"ENGINE": "django.db.backends.sqlite3", "NAME": "db.sqlite3"}}
@@ -21,15 +19,15 @@
     "wagtail.embeds",
     "wagtail.sites",
     "wagtail.users",
     "wagtail.snippets",
     "wagtail.documents",
     "wagtail.admin",
     "wagtail.images",
-    "wagtail.core",
+    "wagtail",
     "taggit",
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.sitemaps",
@@ -73,9 +71,8 @@
 
 WAGTAIL_JOTFORM = {
     "API_KEY": "somekey",
     "API_URL": "https://wagtail-jotform.com",
     "LIMIT": 50,
 }
 
-if WAGTAIL_VERSION >= (3, 0):
-    WAGTAILADMIN_BASE_URL = "http://localhost:8000"
+WAGTAILADMIN_BASE_URL = "http://localhost:8000"
```

### Comparing `wagtail-jotform-2.0.0/wagtail_jotform/tests/tests.py` & `wagtail-jotform-2.0.1/wagtail_jotform/tests/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 from unittest import mock
 
 from django.conf import settings
 from django.test import TestCase
 
-from wagtail import VERSION as WAGTAIL_VERSION
-
-if WAGTAIL_VERSION >= (3, 0):
-    from wagtail.models import Page, Site
-else:
-    from wagtail.core.models import Page, Site
+from wagtail.models import Page, Site
 
 from requests.exceptions import Timeout
 
 from ..models import EmbeddedFormPage
 from ..settings import wagtail_jotform_settings
 from ..utils import CantPullFromAPI, JotFormAPI
 from ..wagtail_hooks import do_after_publish_page
```

### Comparing `wagtail-jotform-2.0.0/wagtail_jotform/tests/urls.py` & `wagtail-jotform-2.0.1/wagtail_jotform/tests/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib import admin
 from django.urls import include, path
 
+from wagtail import urls as wagtail_urls
 from wagtail.admin import urls as wagtailadmin_urls
-from wagtail.core import urls as wagtail_urls
 from wagtail.documents import urls as wagtaildocs_urls
 
 private_urlpatterns = [
     path("django-admin/", admin.site.urls),
     path("admin/", include(wagtailadmin_urls)),
     path("documents/", include(wagtaildocs_urls)),
 ]
```

### Comparing `wagtail-jotform-2.0.0/wagtail_jotform/utils.py` & `wagtail-jotform-2.0.1/wagtail_jotform/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-jotform-2.0.0/wagtail_jotform/wagtail_hooks.py` & `wagtail-jotform-2.0.1/wagtail_jotform/wagtail_hooks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 import logging
 
-from wagtail import VERSION as WAGTAIL_VERSION
+from wagtail import hooks
 
 import requests
 
 from .models import EmbeddedFormPage
 from .settings import wagtail_jotform_settings
 from .utils import CantPullFromAPI
 
 logging.basicConfig(level=logging.CRITICAL)
 logger = logging.getLogger(__name__)
 
-if WAGTAIL_VERSION >= (3, 0):
-    from wagtail import hooks
-else:
-    from wagtail.core import hooks
-
 
 @hooks.register("after_publish_page")
 def do_after_publish_page(request, page):
     if not isinstance(page, EmbeddedFormPage) or not page.form:
         return
     thank_you_url = page.full_url + page.specific.reverse_subpage(
         "embedded_form_thank_you"
```

### Comparing `wagtail-jotform-2.0.0/wagtail_jotform.egg-info/SOURCES.txt` & `wagtail-jotform-2.0.1/wagtail_jotform.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+CHANGELOG.md
 MANIFEST.in
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 wagtail_jotform/__init__.py
 wagtail_jotform/models.py
 wagtail_jotform/settings.py
 wagtail_jotform/utils.py
 wagtail_jotform/wagtail_hooks.py
```

