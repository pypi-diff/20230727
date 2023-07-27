# Comparing `tmp/feincms3_forms-0.3.0.tar.gz` & `tmp/feincms3_forms-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feincms3_forms-0.3.0.tar", last modified: Tue Nov 22 13:16:43 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `feincms3_forms-0.3.0.tar` & `feincms3_forms-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,13 @@
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2022-11-22 13:16:43.127387 feincms3_forms-0.3.0/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1548 2022-09-15 13:25:47.000000 feincms3_forms-0.3.0/LICENSE
--rw-r--r--   0 matthias  (1000) matthias  (1000)      184 2022-09-15 13:25:47.000000 feincms3_forms-0.3.0/MANIFEST.in
--rw-r--r--   0 matthias  (1000) matthias  (1000)     9565 2022-11-22 13:16:43.127387 feincms3_forms-0.3.0/PKG-INFO
--rw-r--r--   0 matthias  (1000) matthias  (1000)     8593 2022-11-22 09:15:05.000000 feincms3_forms-0.3.0/README.rst
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2022-11-22 13:16:43.126387 feincms3_forms-0.3.0/feincms3_forms/
--rw-r--r--   0 matthias  (1000) matthias  (1000)       62 2022-11-22 13:16:04.000000 feincms3_forms-0.3.0/feincms3_forms/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4683 2022-11-22 11:10:08.000000 feincms3_forms-0.3.0/feincms3_forms/admin.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2022-11-22 13:16:43.125387 feincms3_forms-0.3.0/feincms3_forms/locale/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2022-11-22 13:16:43.125387 feincms3_forms-0.3.0/feincms3_forms/locale/de/
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2022-11-22 13:16:43.127387 feincms3_forms-0.3.0/feincms3_forms/locale/de/LC_MESSAGES/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3460 2022-11-22 09:15:05.000000 feincms3_forms-0.3.0/feincms3_forms/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias  (1000) matthias  (1000)     4412 2022-11-22 09:15:05.000000 feincms3_forms-0.3.0/feincms3_forms/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 matthias  (1000) matthias  (1000)    14500 2022-11-22 13:15:41.000000 feincms3_forms-0.3.0/feincms3_forms/models.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1768 2022-11-22 11:09:59.000000 feincms3_forms-0.3.0/feincms3_forms/renderer.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      941 2022-11-22 11:09:59.000000 feincms3_forms-0.3.0/feincms3_forms/reporting.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2578 2022-11-22 11:09:59.000000 feincms3_forms-0.3.0/feincms3_forms/validation.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2022-11-22 13:16:43.127387 feincms3_forms-0.3.0/feincms3_forms.egg-info/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     9565 2022-11-22 13:16:43.000000 feincms3_forms-0.3.0/feincms3_forms.egg-info/PKG-INFO
--rw-r--r--   0 matthias  (1000) matthias  (1000)      529 2022-11-22 13:16:43.000000 feincms3_forms-0.3.0/feincms3_forms.egg-info/SOURCES.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2022-11-22 13:16:43.000000 feincms3_forms-0.3.0/feincms3_forms.egg-info/dependency_links.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2022-11-01 14:11:12.000000 feincms3_forms-0.3.0/feincms3_forms.egg-info/not-zip-safe
--rw-r--r--   0 matthias  (1000) matthias  (1000)       48 2022-11-22 13:16:43.000000 feincms3_forms-0.3.0/feincms3_forms.egg-info/requires.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)       15 2022-11-22 13:16:43.000000 feincms3_forms-0.3.0/feincms3_forms.egg-info/top_level.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1244 2022-11-22 13:16:43.127387 feincms3_forms-0.3.0/setup.cfg
--rwxr-xr-x   0 matthias  (1000) matthias  (1000)       62 2022-09-15 13:25:47.000000 feincms3_forms-0.3.0/setup.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/feincms3_forms/__init__.py
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/feincms3_forms/admin.py
+-rw-r--r--   0        0        0    14549 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/feincms3_forms/models.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/feincms3_forms/renderer.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/feincms3_forms/reporting.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/feincms3_forms/validation.py
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/feincms3_forms/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/feincms3_forms/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/LICENSE
+-rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/README.rst
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11799 2020-02-02 00:00:00.000000 feincms3_forms-0.4.0/PKG-INFO
```

### Comparing `feincms3_forms-0.3.0/LICENSE` & `feincms3_forms-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3_forms-0.3.0/PKG-INFO` & `feincms3_forms-0.4.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,115 @@
-Metadata-Version: 2.1
-Name: feincms3_forms
-Version: 0.3.0
-Home-page: https://github.com/matthiask/feincms3-forms/
-Author: Matthias Kestenholz
-Author-email: mk@feinheit.ch
-License: BSD-3-Clause
-Platform: OS Independent
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-Provides-Extra: tests
-License-File: LICENSE
-
 ==============
 feincms3-forms
 ==============
 
 .. image:: https://github.com/matthiask/feincms3-forms/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/matthiask/feincms3-forms/
     :alt: CI Status
 
-This is an extremely flexible forms builder for the Django admin interface.
+This is an extremely flexible forms builder for the Django admin interface. It
+allows using `django-content-editor
+<https://django-content-editor.readthedocs.io/>`__ for your form which enables:
+
+- Build your own form in the CMS and not have to ask programmers to change
+  anything.
+- Reorder, add and remove pre-existing fields.
+- Add content (text, images, anything) between form fields.
+- Use regions to add additional structure to a form, e.g. to build configurable
+  multi-step forms (wizards).
+- Add your own form field plugins with all the flexibility and configurability
+  you desire.
 
 If you only want to integrate short and simple forms (e.g. a contact form)
 you're probably better off using `form_designer
 <https://github.com/feincms/form_designer>`__. The feincms3 documentation
 contains a `guide showing how to integrate it
 <https://feincms3.readthedocs.io/en/latest/guides/apps-form-builder.html>`__.
 
-If you need more flexibility, multi page forms, forms with other content
-between fields, a relatively straightforward way to define you own (compound)
-fields etc. etc. then feincms3-forms may be for you.
-
-
-Design decisions
-================
-
-This is a list of things which should be explained but are not at the moment.
-
-- Form fields have to inherit ``FormFieldBase``. ``FormFieldBase`` only has a
-  ``name`` field. This field can be checked for clashes etc. The base class is
-  used instead of duck typing in various places where the code may encounter
-  not only form field plugins but also other django-content-editor plugins. The
-  latter are useful e.g. to add blocks of text or other content between form
-  fields.
-- The ``FormField`` offers a basic set of attributes for standard fields such
-  as a label, a help text and whether the field should be required or not.
-- The ``SimpleFieldBase`` should be instantiated in your project and can be
-  used to cheaply generate standard form field plugin proxies for HTML5 input
-  fields. (Sorry for the jargon.) Those proxies are standard Django model
-  proxies.
+
+High level overview
+===================
+
+The documentation is very sparse, sorry for that.
+
+
+Models
+~~~~~~
+
+
+FormFieldBase
+-------------
+
+Form fields have to inherit ``FormFieldBase``. ``FormFieldBase`` only has a
+``name`` field. This field can be checked for clashes etc. The base class is
+used instead of duck typing in various places where the code may encounter not
+only form field plugins but also other django-content-editor plugins. The
+latter are useful e.g. to add blocks of text or other content between form
+fields.
+
+The ``FormFieldBase`` model defines the basic API of form fields:
+
+- ``get_fields()``: Return a dictionary of form fields.
+- ``get_initial()``: Return initial values of said fields.
+- ``get_cleaners()``: Return a list of callables which receive the form
+  instance, return the cleaned data and may raise ``ValidationError``
+  exceptions.
+- ``get_loaders()``: Return a list of loaders. The purpose of loaders is to
+  load form submissions, e.g. for reporting purposes. Loaders are callables
+  which receive the serialized form data and return a dictionary of the
+  following shape: ``{"name": ..., "label": ..., "value": ...}``.
+
+
+FormField
+---------
+
+The ``FormField`` offers a basic set of attributes for standard fields such as
+a label, a help text and whether the field should be required or not. You do
+not have to use this model if you want to define your own. It's purpose is just
+to offer a few good defaults.
+
+
+SimpleFieldBase
+---------------
+
+The ``SimpleFieldBase`` should be instantiated in your project and can be used
+to cheaply add support for many basic field types such as text fields, email
+fields, checkboxes, choice fields and more with a single backing database table
+and model.
+
+The ``SimpleFieldBase`` has a corresponding ``SimpleFieldInline`` in the
+``feincms3_forms.admin`` module which shows and hides fields depending on the
+field type. For example, it makes no sense to define placeholders for
+checkboxes (browsers do not support them) therefore the field is omitted in the
+CMS.
+
+
+Renderer
+~~~~~~~~
+
+The renderer functions are responsible for creating and instantiating the form
+class. Form class creation and instantiation happens at once.
+
+
+Validation
+~~~~~~~~~~
+
+The validation module offers utilities to validate a form when it it defined in
+the CMS. For example, the backend code may require that an email field always
+exists and always has a certain predefined name (for example ``email`` 😏).
+These rules are not enforced at the moment but the user is always notified and
+can therefore choose to head them. Or bad things may happen depending on the
+code you write.
+
+
+Reporting
+~~~~~~~~~
+
+The reporting functions are mostly useful if you want to do something with
+submitted data.
 
 
 Installation and usage
 ======================
 
 Create a module containing the models for the form builder (``app.forms.models``):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `feincms3_forms-0.3.0/feincms3_forms/admin.py` & `feincms3_forms-0.4.0/feincms3_forms/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -91,41 +91,57 @@
     form = SimpleFieldForm
 
     def get_queryset(self, request):
         return super().get_queryset(request).filter(type=self.model.TYPE)
 
     @classmethod
     def create(cls, model, **kwargs):
-        T = model.Type
-        if model.TYPE in {T.TEXT, T.TEXTAREA}:
+        type = model.Type
+        if model.TYPE in {type.TEXT, type.TEXTAREA}:
             kwargs.setdefault(
                 "advanced_fields",
                 ["help_text", "placeholder", "default_value", "max_length"],
             )
 
-        elif model.TYPE in {T.EMAIL, T.URL, T.DATE, T.INTEGER}:
+        elif model.TYPE in {type.EMAIL, type.URL, type.DATE, type.INTEGER}:
             kwargs.setdefault(
                 "advanced_fields", ["help_text", "placeholder", "default_value"]
             )
 
-        elif model.TYPE in {T.CHECKBOX}:
+        elif model.TYPE in {type.CHECKBOX}:
             kwargs.setdefault("advanced_fields", ["help_text", "default_value"])
 
-        elif model.TYPE in {T.SELECT}:
+        elif model.TYPE in {type.SELECT}:
             kwargs.setdefault(
                 "core_fields", ["name", "label", "is_required", "choices"]
             )
             kwargs.setdefault(
                 "advanced_fields", ["help_text", "placeholder", "default_value"]
             )
 
         elif model.TYPE in {
-            T.RADIO,
-            T.SELECT_MULTIPLE,
-            T.CHECKBOX_SELECT_MULTIPLE,
+            type.RADIO,
+            type.SELECT_MULTIPLE,
+            type.CHECKBOX_SELECT_MULTIPLE,
         }:
             kwargs.setdefault(
                 "core_fields", ["name", "label", "is_required", "choices"]
             )
             kwargs.setdefault("advanced_fields", ["help_text", "default_value"])
 
+        icons = {
+            type.TEXT: "short_text",
+            type.EMAIL: "alternate_email",
+            type.URL: "link",
+            type.DATE: "event",
+            type.INTEGER: "looks_one",
+            type.TEXTAREA: "notes",
+            type.CHECKBOX: "check_box",
+            type.SELECT: "arrow_drop_down_circle",
+            type.RADIO: "radio_button_checked",
+            type.SELECT_MULTIPLE: "check_box",
+            type.CHECKBOX_SELECT_MULTIPLE: "check_box",
+        }
+        if icon := icons.get(model.TYPE):
+            kwargs.setdefault("button", f'<span class="material-icons">{icon}</span>')
+
         return super().create(model, **kwargs)
```

### Comparing `feincms3_forms-0.3.0/feincms3_forms/locale/de/LC_MESSAGES/django.mo` & `feincms3_forms-0.4.0/feincms3_forms/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_forms-0.3.0/feincms3_forms/locale/de/LC_MESSAGES/django.po` & `feincms3_forms-0.4.0/feincms3_forms/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_forms-0.3.0/feincms3_forms/models.py` & `feincms3_forms-0.4.0/feincms3_forms/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import re
 import warnings
 from functools import partial, reduce
 
 from content_editor.models import Type
 from django import forms
 from django.core import validators
@@ -25,18 +26,18 @@
         kwargs.setdefault("form_class", forms.Form)
         kwargs.setdefault("validate", lambda configured_form: [])
         super().__init__(**kwargs)
 
     def __getattr__(self, attr):
         value = super().__getattr__(attr)
         if isinstance(value, str) and re.match(r"^\w+\.([\w\.]+)+$", value):
-            try:
-                return import_string(value)
-            except ModuleNotFoundError:
-                pass
+            with contextlib.suppress(ModuleNotFoundError):
+                value = import_string(value)
+
+        setattr(self, attr, value)
         return value
 
 
 RANDOM_STRING_CHARS = "abcdefghijklmnopqrstuvwxyz0123456789"
 
 
 class NameField(models.CharField):
@@ -308,25 +309,27 @@
                 "TYPE": type_name,
             },
         )
 
     def clean_fields(self, exclude=None):
         super().clean_fields(exclude)
 
-        if self.choices and self.default_value:
-            if slugify(self.default_value) not in dict(self.get_choices()):
-                raise validation_error(
-                    _(
-                        'The specified default value "%(default)s" isn\'t part of'
-                        " the available choices."
-                    )
-                    % {"default": self.default_value},
-                    field="default_value",
-                    exclude=exclude,
+        if (
+            self.choices
+            and self.default_value
+            and slugify(self.default_value) not in dict(self.get_choices())
+        ):
+            raise validation_error(
+                _(
+                    'The specified default value "%(default)s" isn\'t part of the available choices.'
                 )
+                % {"default": self.default_value},
+                field="default_value",
+                exclude=exclude,
+            )
 
     def get_choices(self):
         def _choice(value):
             parts = [part.strip() for part in value.split("|", 1)]
             if len(parts) == 1:
                 return (slugify(value), value)
             else:
@@ -338,99 +341,99 @@
         if not self.default_value:
             return {}
         if self.choices:
             return {self.name: slugify(self.default_value)}
         return {self.name: self.default_value}
 
     def get_fields(self, **kwargs):
-        T = self.Type
+        type = self.Type
 
-        if self.type == T.TEXT:
+        if self.type == type.TEXT:
             return self.get_field(
                 form_class=forms.CharField,
                 max_length=self.max_length,
                 widget=forms.CharField.widget(
                     attrs={"placeholder": self.placeholder or False}
                 ),
             )
 
-        elif self.type == T.EMAIL:
+        elif self.type == type.EMAIL:
             return self.get_field(
                 form_class=forms.EmailField,
                 widget=forms.EmailField.widget(
                     attrs={"placeholder": self.placeholder or False}
                 ),
             )
 
-        elif self.type == T.URL:
+        elif self.type == type.URL:
             return self.get_field(
                 form_class=forms.URLField,
                 widget=forms.URLField.widget(
                     attrs={"placeholder": self.placeholder or False}
                 ),
             )
 
-        elif self.type == T.DATE:
+        elif self.type == type.DATE:
             return self.get_field(
                 form_class=forms.DateField,
                 widget=forms.DateInput(
                     attrs={"placeholder": self.placeholder or False, "type": "date"}
                 ),
             )
 
-        elif self.type == T.INTEGER:
+        elif self.type == type.INTEGER:
             return self.get_field(
                 form_class=forms.IntegerField,
                 widget=forms.IntegerField.widget(
                     attrs={"placeholder": self.placeholder or False}
                 ),
             )
 
-        elif self.type == T.TEXTAREA:
+        elif self.type == type.TEXTAREA:
             return self.get_field(
                 form_class=forms.CharField,
                 max_length=self.max_length,
                 widget=forms.Textarea(
                     attrs={
                         "maxlength": self.max_length or False,
                         "placeholder": self.placeholder or False,
                         "rows": 5,
                     },
                 ),
             )
 
-        elif self.type == T.CHECKBOX:
+        elif self.type == type.CHECKBOX:
             return self.get_field(form_class=forms.BooleanField)
 
-        elif self.type == T.SELECT:
+        elif self.type == type.SELECT:
             choices = self.get_choices()
             if not self.is_required or not self.default_value:
                 blank_choice = (
                     [("", self.placeholder)] if self.placeholder else BLANK_CHOICE_DASH
                 )
                 choices = blank_choice + choices
             return self.get_field(
                 form_class=forms.ChoiceField,
                 choices=choices,
             )
 
-        elif self.type == T.RADIO:
+        elif self.type == type.RADIO:
             return self.get_field(
                 form_class=forms.ChoiceField,
                 widget=forms.RadioSelect,
                 choices=self.get_choices(),
             )
 
-        elif self.type == T.SELECT_MULTIPLE:
+        elif self.type == type.SELECT_MULTIPLE:
             return self.get_field(
                 form_class=forms.MultipleChoiceField,
                 choices=self.get_choices(),
             )
 
-        elif self.type == T.CHECKBOX_SELECT_MULTIPLE:
+        elif self.type == type.CHECKBOX_SELECT_MULTIPLE:
             return self.get_field(
                 form_class=forms.MultipleChoiceField,
                 widget=forms.CheckboxSelectMultiple,
                 choices=self.get_choices(),
             )
 
         else:
```

### Comparing `feincms3_forms-0.3.0/feincms3_forms/renderer.py` & `feincms3_forms-0.4.0/feincms3_forms/renderer.py`

 * *Files identical despite different names*

### Comparing `feincms3_forms-0.3.0/feincms3_forms/reporting.py` & `feincms3_forms-0.4.0/feincms3_forms/reporting.py`

 * *Files identical despite different names*

### Comparing `feincms3_forms-0.3.0/feincms3_forms/validation.py` & `feincms3_forms-0.4.0/feincms3_forms/validation.py`

 * *Files identical despite different names*

### Comparing `feincms3_forms-0.3.0/feincms3_forms.egg-info/PKG-INFO` & `feincms3_forms-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,142 @@
 Metadata-Version: 2.1
 Name: feincms3-forms
-Version: 0.3.0
-Home-page: https://github.com/matthiask/feincms3-forms/
-Author: Matthias Kestenholz
-Author-email: mk@feinheit.ch
+Version: 0.4.0
+Project-URL: Homepage, https://github.com/matthiask/feincms3-forms/
+Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
-Platform: OS Independent
+License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Requires-Dist: django>=3.2
+Requires-Dist: feincms3>=0.90b17
 Provides-Extra: tests
-License-File: LICENSE
+Requires-Dist: coverage; extra == 'tests'
+Description-Content-Type: text/x-rst
 
 ==============
 feincms3-forms
 ==============
 
 .. image:: https://github.com/matthiask/feincms3-forms/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/matthiask/feincms3-forms/
     :alt: CI Status
 
-This is an extremely flexible forms builder for the Django admin interface.
+This is an extremely flexible forms builder for the Django admin interface. It
+allows using `django-content-editor
+<https://django-content-editor.readthedocs.io/>`__ for your form which enables:
+
+- Build your own form in the CMS and not have to ask programmers to change
+  anything.
+- Reorder, add and remove pre-existing fields.
+- Add content (text, images, anything) between form fields.
+- Use regions to add additional structure to a form, e.g. to build configurable
+  multi-step forms (wizards).
+- Add your own form field plugins with all the flexibility and configurability
+  you desire.
 
 If you only want to integrate short and simple forms (e.g. a contact form)
 you're probably better off using `form_designer
 <https://github.com/feincms/form_designer>`__. The feincms3 documentation
 contains a `guide showing how to integrate it
 <https://feincms3.readthedocs.io/en/latest/guides/apps-form-builder.html>`__.
 
-If you need more flexibility, multi page forms, forms with other content
-between fields, a relatively straightforward way to define you own (compound)
-fields etc. etc. then feincms3-forms may be for you.
-
-
-Design decisions
-================
-
-This is a list of things which should be explained but are not at the moment.
-
-- Form fields have to inherit ``FormFieldBase``. ``FormFieldBase`` only has a
-  ``name`` field. This field can be checked for clashes etc. The base class is
-  used instead of duck typing in various places where the code may encounter
-  not only form field plugins but also other django-content-editor plugins. The
-  latter are useful e.g. to add blocks of text or other content between form
-  fields.
-- The ``FormField`` offers a basic set of attributes for standard fields such
-  as a label, a help text and whether the field should be required or not.
-- The ``SimpleFieldBase`` should be instantiated in your project and can be
-  used to cheaply generate standard form field plugin proxies for HTML5 input
-  fields. (Sorry for the jargon.) Those proxies are standard Django model
-  proxies.
+
+High level overview
+===================
+
+The documentation is very sparse, sorry for that.
+
+
+Models
+~~~~~~
+
+
+FormFieldBase
+-------------
+
+Form fields have to inherit ``FormFieldBase``. ``FormFieldBase`` only has a
+``name`` field. This field can be checked for clashes etc. The base class is
+used instead of duck typing in various places where the code may encounter not
+only form field plugins but also other django-content-editor plugins. The
+latter are useful e.g. to add blocks of text or other content between form
+fields.
+
+The ``FormFieldBase`` model defines the basic API of form fields:
+
+- ``get_fields()``: Return a dictionary of form fields.
+- ``get_initial()``: Return initial values of said fields.
+- ``get_cleaners()``: Return a list of callables which receive the form
+  instance, return the cleaned data and may raise ``ValidationError``
+  exceptions.
+- ``get_loaders()``: Return a list of loaders. The purpose of loaders is to
+  load form submissions, e.g. for reporting purposes. Loaders are callables
+  which receive the serialized form data and return a dictionary of the
+  following shape: ``{"name": ..., "label": ..., "value": ...}``.
+
+
+FormField
+---------
+
+The ``FormField`` offers a basic set of attributes for standard fields such as
+a label, a help text and whether the field should be required or not. You do
+not have to use this model if you want to define your own. It's purpose is just
+to offer a few good defaults.
+
+
+SimpleFieldBase
+---------------
+
+The ``SimpleFieldBase`` should be instantiated in your project and can be used
+to cheaply add support for many basic field types such as text fields, email
+fields, checkboxes, choice fields and more with a single backing database table
+and model.
+
+The ``SimpleFieldBase`` has a corresponding ``SimpleFieldInline`` in the
+``feincms3_forms.admin`` module which shows and hides fields depending on the
+field type. For example, it makes no sense to define placeholders for
+checkboxes (browsers do not support them) therefore the field is omitted in the
+CMS.
+
+
+Renderer
+~~~~~~~~
+
+The renderer functions are responsible for creating and instantiating the form
+class. Form class creation and instantiation happens at once.
+
+
+Validation
+~~~~~~~~~~
+
+The validation module offers utilities to validate a form when it it defined in
+the CMS. For example, the backend code may require that an email field always
+exists and always has a certain predefined name (for example ``email`` 😏).
+These rules are not enforced at the moment but the user is always notified and
+can therefore choose to head them. Or bad things may happen depending on the
+code you write.
+
+
+Reporting
+~~~~~~~~~
+
+The reporting functions are mostly useful if you want to do something with
+submitted data.
 
 
 Installation and usage
 ======================
 
 Create a module containing the models for the form builder (``app.forms.models``):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

