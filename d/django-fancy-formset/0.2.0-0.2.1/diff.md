# Comparing `tmp/django-fancy-formset-0.2.0.tar.gz` & `tmp/django-fancy-formset-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-fancy-formset-0.2.0.tar", last modified: Tue Jul 25 23:04:11 2023, max compression
+gzip compressed data, was "django-fancy-formset-0.2.1.tar", last modified: Wed Jul 26 22:20:44 2023, max compression
```

## Comparing `django-fancy-formset-0.2.0.tar` & `django-fancy-formset-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2023-07-25 23:04:11.793532 django-fancy-formset-0.2.0/
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     1662 2023-07-25 05:50:56.000000 django-fancy-formset-0.2.0/LICENSE
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      109 2023-07-25 22:55:50.000000 django-fancy-formset-0.2.0/MANIFEST.in
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      880 2023-07-25 23:04:11.793532 django-fancy-formset-0.2.0/PKG-INFO
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     2924 2023-07-25 06:21:52.000000 django-fancy-formset-0.2.0/README.md
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2023-07-25 23:04:11.789532 django-fancy-formset-0.2.0/django_fancy_formset.egg-info/
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      880 2023-07-25 23:04:11.000000 django-fancy-formset-0.2.0/django_fancy_formset.egg-info/PKG-INFO
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      750 2023-07-25 23:04:11.000000 django-fancy-formset-0.2.0/django_fancy_formset.egg-info/SOURCES.txt
--rw-rw-r--   0 radiac    (1000) radiac    (1000)        1 2023-07-25 23:04:11.000000 django-fancy-formset-0.2.0/django_fancy_formset.egg-info/dependency_links.txt
--rw-rw-r--   0 radiac    (1000) radiac    (1000)       12 2023-07-25 23:04:11.000000 django-fancy-formset-0.2.0/django_fancy_formset.egg-info/requires.txt
--rw-rw-r--   0 radiac    (1000) radiac    (1000)       14 2023-07-25 23:04:11.000000 django-fancy-formset-0.2.0/django_fancy_formset.egg-info/top_level.txt
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2023-07-25 23:04:11.789532 django-fancy-formset-0.2.0/fancy_formset/
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      106 2023-07-25 06:19:40.000000 django-fancy-formset-0.2.0/fancy_formset/__init__.py
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     1482 2023-07-22 18:29:21.000000 django-fancy-formset-0.2.0/fancy_formset/formsets.py
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2023-07-25 23:04:11.789532 django-fancy-formset-0.2.0/fancy_formset/static/
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2023-07-25 23:04:11.793532 django-fancy-formset-0.2.0/fancy_formset/static/fancy_formset/
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     3762 2023-07-25 23:03:54.000000 django-fancy-formset-0.2.0/fancy_formset/static/fancy_formset/formset.css
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     5526 2023-07-25 23:03:54.000000 django-fancy-formset-0.2.0/fancy_formset/static/fancy_formset/formset.js
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     3220 2023-07-25 23:03:54.000000 django-fancy-formset-0.2.0/fancy_formset/static/fancy_formset/formset.min.css
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     5244 2023-07-25 23:03:54.000000 django-fancy-formset-0.2.0/fancy_formset/static/fancy_formset/formset.module.js
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2023-07-25 23:04:11.789532 django-fancy-formset-0.2.0/fancy_formset/templates/
-drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2023-07-25 23:04:11.793532 django-fancy-formset-0.2.0/fancy_formset/templates/fancy_formset/
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      290 2023-07-22 18:52:09.000000 django-fancy-formset-0.2.0/fancy_formset/templates/fancy_formset/default.html
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      304 2023-07-22 18:51:18.000000 django-fancy-formset-0.2.0/fancy_formset/templates/fancy_formset/div.html
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      300 2023-07-21 13:11:36.000000 django-fancy-formset-0.2.0/fancy_formset/templates/fancy_formset/p.html
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      368 2023-07-22 18:51:26.000000 django-fancy-formset-0.2.0/fancy_formset/templates/fancy_formset/table.html
--rw-rw-r--   0 radiac    (1000) radiac    (1000)      350 2023-07-22 22:50:15.000000 django-fancy-formset-0.2.0/fancy_formset/templates/fancy_formset/ul.html
--rw-rw-r--   0 radiac    (1000) radiac    (1000)     2260 2023-07-25 22:16:48.000000 django-fancy-formset-0.2.0/pyproject.toml
--rw-rw-r--   0 radiac    (1000) radiac    (1000)       38 2023-07-25 23:04:11.793532 django-fancy-formset-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.826683 django-fancy-formset-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-26 22:20:44.826683 django-fancy-formset-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.822683 django-fancy-formset-0.2.1/django_fancy_formset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-26 22:20:44.000000 django-fancy-formset-0.2.1/django_fancy_formset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-26 22:20:44.000000 django-fancy-formset-0.2.1/django_fancy_formset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:20:44.000000 django-fancy-formset-0.2.1/django_fancy_formset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 22:20:44.000000 django-fancy-formset-0.2.1/django_fancy_formset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 22:20:44.000000 django-fancy-formset-0.2.1/django_fancy_formset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.822683 django-fancy-formset-0.2.1/fancy_formset/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/formsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.822683 django-fancy-formset-0.2.1/fancy_formset/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.822683 django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-26 22:20:37.000000 django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-26 22:20:37.000000 django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-26 22:20:37.000000 django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-26 22:20:37.000000 django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.822683 django-fancy-formset-0.2.1/fancy_formset/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:20:44.826683 django-fancy-formset-0.2.1/fancy_formset/templates/fancy_formset/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/templates/fancy_formset/default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/templates/fancy_formset/div.html
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/templates/fancy_formset/p.html
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/templates/fancy_formset/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/fancy_formset/templates/fancy_formset/ul.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-26 22:20:33.000000 django-fancy-formset-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:20:44.826683 django-fancy-formset-0.2.1/setup.cfg
```

### Comparing `django-fancy-formset-0.2.0/LICENSE` & `django-fancy-formset-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.0/README.md` & `django-fancy-formset-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # django-fancy-formset
 
 This is a plain JavaScript library to let users add and remove forms in a Django inline
 formset. It can be installed from PyPI as a Django app, from NPM as a JavaScript module,
 or linked to directly from your HTML.
 
-<p align="center" width="100%">
-  <kbd>
-    <img src="https://github.com/radiac/django-fancy-formset/raw/main/docs/example.gif" alt="Add and remove forms in an inline formset">
-  </kbd>
-</p>
+[![PyPi version](https://badgen.net/pypi/v/django-fancy-formset/)](https://pypi.org/project/django-fancy-formset)
+[![Npm version](https://badgen.net/npm/v/django-fancy-formset)](https://npmjs.com/package/django-fancy-formset)
+[![Documentation](https://readthedocs.org/projects/django-fancy-formset/badge/?version=latest)](https://django-fancy-formset.readthedocs.io/en/latest/?badge=latest)
+[![CI](https://github.com/radiac/django-fancy-formset/actions/workflows/ci.yml/badge.svg)](https://github.com/radiac/django-fancy-formset/actions/workflows/ci.yml)
+
 
 Features:
 
 * No dependencies, just 5kB of plain JavaScript
 * Apply to formsets manually, or automatically via a ``data-`` attribute
 * Optional Django app to simplify usage
 * Raises events to allow for customisation
 * Class based and designed to be extended
 * Default styling available
 
 
+<p align="center" width="100%">
+  <kbd>
+    <img src="https://github.com/radiac/django-fancy-formset/raw/main/docs/example.gif" alt="Add and remove forms in an inline formset">
+  </kbd>
+</p>
+
+
 ## Quickstart using Python
 
 Install with:
 
 ```bash
 pip install django-fancy-formset
 ```
@@ -47,14 +54,17 @@
   {% csrf_token %}
   {{ form.as_p }}
   {{ formset.as_p }}
   <button type="submit">Save</button>
 </form>
 ```
 
+See the
+[Django installation documentation](https://django-fancy-formset.readthedocs.io/en/latest/installation-django.html)
+for more details
 
 ## Quickstart using JavaScript
 
 The Python package is a thin wrapper around the JavaScript package. For more control,
 you can integrate it yourself.
 
 Add to your page directly using [unpkg](https://unpkg.com/):
@@ -69,17 +79,17 @@
     <!-- Django formset goes here -->
     <script src="https://unpkg.com/django-fancy-formset@^1"></script>
     <script>formset.init();</script>
   </body>
 </html>
 ```
 
-You can also use it in your bundler or browser as module - see installation
-documentation.
-
+You can also use it in your bundler or browser as module - see the
+[JavaScript-only installation documentation](https://django-fancy-formset.readthedocs.io/en/latest/installation-javascript.html)
+for more details
 
 Render your formset in your Django template. The template structure which will work with
 the default configuration is:
 
 ```django
 <form method="post">
   {% csrf_token %}
@@ -98,14 +108,17 @@
     {% endfor %}
   </div>
 
   <button type="submit">Save</button>
 </form>
 ```
 
-This can all be customised with options passed as `formset.init(options)` - see
-configuration documentation for details.
+This can all be customised with options passed as `formset.init(options)` - see the
+[configuration documentation](https://django-fancy-formset.readthedocs.io/en/latest/configuration.html)
+for details.
 
 
 ## Find out more
 
-For full installation and usage instructions, see the documentation.
+For full installation and usage instructions, as well as information on events, the API
+and customisation, see the
+[documentation](https://django-fancy-formset.readthedocs.io/en/latest/).
```

#### html2text {}

```diff
@@ -1,34 +1,48 @@
 # django-fancy-formset This is a plain JavaScript library to let users add and
 remove forms in a Django inline formset. It can be installed from PyPI as a
 Django app, from NPM as a JavaScript module, or linked to directly from your
-HTML.
+HTML. [![PyPi version](https://badgen.net/pypi/v/django-fancy-formset/)](https:
+//pypi.org/project/django-fancy-formset) [![Npm version](https://badgen.net/
+npm/v/django-fancy-formset)](https://npmjs.com/package/django-fancy-formset) [!
+[Documentation](https://readthedocs.org/projects/django-fancy-formset/badge/
+?version=latest)](https://django-fancy-formset.readthedocs.io/en/latest/
+?badge=latest) [![CI](https://github.com/radiac/django-fancy-formset/actions/
+workflows/ci.yml/badge.svg)](https://github.com/radiac/django-fancy-formset/
+actions/workflows/ci.yml) Features: * No dependencies, just 5kB of plain
+JavaScript * Apply to formsets manually, or automatically via a ``data-``
+attribute * Optional Django app to simplify usage * Raises events to allow for
+customisation * Class based and designed to be extended * Default styling
+available
                   [Add and remove forms in an inline formset]
-Features: * No dependencies, just 5kB of plain JavaScript * Apply to formsets
-manually, or automatically via a ``data-`` attribute * Optional Django app to
-simplify usage * Raises events to allow for customisation * Class based and
-designed to be extended * Default styling available ## Quickstart using Python
-Install with: ```bash pip install django-fancy-formset ``` Add to your
-``INSTALLED_APPS``, then create your formsets using the provided fancy formset
-classes: ```python from fancy_formset import FancyInlineFormSet
-BookInlineFormSet = forms.inlineformset_factory( Author, Book,
-formset=InlineFancyFormSet, ) ``` then leave it to Django to render your
+## Quickstart using Python Install with: ```bash pip install django-fancy-
+formset ``` Add to your ``INSTALLED_APPS``, then create your formsets using the
+provided fancy formset classes: ```python from fancy_formset import
+FancyInlineFormSet BookInlineFormSet = forms.inlineformset_factory( Author,
+Book, formset=InlineFancyFormSet, ) ``` then leave it to Django to render your
 formset: ```django {{ formset.media }}
 {% csrf_token %} {{ form.as_p }} {{ formset.as_p }} Save
-``` ## Quickstart using JavaScript The Python package is a thin wrapper around
-the JavaScript package. For more control, you can integrate it yourself. Add to
+``` See the [Django installation documentation](https://django-fancy-
+formset.readthedocs.io/en/latest/installation-django.html) for more details ##
+Quickstart using JavaScript The Python package is a thin wrapper around the
+JavaScript package. For more control, you can integrate it yourself. Add to
 your page directly using [unpkg](https://unpkg.com/): ```html
 
-``` You can also use it in your bundler or browser as module - see installation
-documentation. Render your formset in your Django template. The template
-structure which will work with the default configuration is: ```django
+``` You can also use it in your bundler or browser as module - see the
+[JavaScript-only installation documentation](https://django-fancy-
+formset.readthedocs.io/en/latest/installation-javascript.html) for more details
+Render your formset in your Django template. The template structure which will
+work with the default configuration is: ```django
 {% csrf_token %} {{ form.as_p }}
 ***** Formset *****
 {# Formset container to target #} {{ formset.management_form }} {# Add the
 management form #}  {# Add and hide the empty form #} {
 { formset.empty_form.as_p }}  {% for form in formset %}  {# Each formset form
 has a container #} {{ form.as_p }} {# Actual form layout doesn't matter #}  {%
 endfor %}
 Save
 ``` This can all be customised with options passed as `formset.init(options)` -
-see configuration documentation for details. ## Find out more For full
-installation and usage instructions, see the documentation.
+see the [configuration documentation](https://django-fancy-
+formset.readthedocs.io/en/latest/configuration.html) for details. ## Find out
+more For full installation and usage instructions, as well as information on
+events, the API and customisation, see the [documentation](https://django-
+fancy-formset.readthedocs.io/en/latest/).
```

### Comparing `django-fancy-formset-0.2.0/django_fancy_formset.egg-info/SOURCES.txt` & `django-fancy-formset-0.2.1/django_fancy_formset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.0/fancy_formset/formsets.py` & `django-fancy-formset-0.2.1/fancy_formset/formsets.py`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.0/fancy_formset/static/fancy_formset/formset.css` & `django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.css`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.0/fancy_formset/static/fancy_formset/formset.js` & `django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.js`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.0/fancy_formset/static/fancy_formset/formset.min.css` & `django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.min.css`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.0/fancy_formset/static/fancy_formset/formset.module.js` & `django-fancy-formset-0.2.1/fancy_formset/static/fancy_formset/formset.module.js`

 * *Files identical despite different names*

### Comparing `django-fancy-formset-0.2.0/pyproject.toml` & `django-fancy-formset-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "django-fancy-formset"
 description = "A Django app and pure JavaScript library to manage formsets"
 dynamic = ["version"]
 authors = [
     { name="Richard Terry", email="code@radiac.net" },
 ]
-readme = "README.rst"
+readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Django",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
```

