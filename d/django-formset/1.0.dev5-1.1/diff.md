# Comparing `tmp/django-formset-1.0.dev5.tar.gz` & `tmp/django-formset-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-formset-1.0.dev5.tar", last modified: Tue Jun 13 21:48:08 2023, max compression
+gzip compressed data, was "django-formset-1.1.tar", last modified: Thu Jul 27 21:18:50 2023, max compression
```

## Comparing `django-formset-1.0.dev5.tar` & `django-formset-1.1.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.151450 django-formset-1.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-13 21:48:08.151450 django-formset-1.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.123449 django-formset-1.0.dev5/django_formset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-13 21:48:08.000000 django-formset-1.0.dev5/django_formset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-06-13 21:48:08.000000 django-formset-1.0.dev5/django_formset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:48:08.000000 django-formset-1.0.dev5/django_formset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:48:07.000000 django-formset-1.0.dev5/django_formset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 21:48:08.000000 django-formset-1.0.dev5/django_formset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 21:48:08.000000 django-formset-1.0.dev5/django_formset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.127449 django-formset-1.0.dev5/formset/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/fieldset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.119449 django-formset-1.0.dev5/formset/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.119449 django-formset-1.0.dev5/formset/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.127449 django-formset-1.0.dev5/formset/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.127449 django-formset-1.0.dev5/formset/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/bulma.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/foundation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/tailwind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/renderers/uikit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.127449 django-formset-1.0.dev5/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/richtext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/richtext/controls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/richtext/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/richtext/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/richtext/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.119449 django-formset-1.0.dev5/formset/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.123449 django-formset-1.0.dev5/formset/static/formset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.127449 django-formset-1.0.dev5/formset/static/formset/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-13 21:47:58.000000 django-formset-1.0.dev5/formset/static/formset/css/bootstrap5-extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-13 21:47:58.000000 django-formset-1.0.dev5/formset/static/formset/css/bootstrap5-extra.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-13 21:47:58.000000 django-formset-1.0.dev5/formset/static/formset/css/collections.css
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-13 21:47:58.000000 django-formset-1.0.dev5/formset/static/formset/css/collections.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-06-13 21:47:59.000000 django-formset-1.0.dev5/formset/static/formset/css/tailwind.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/static/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/icons/file-zip.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/static/formset/js/
--rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/DateTimePicker-TF2GNHHS.js
--rw-r--r--   0 runner    (1001) docker     (123)    55693 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/DjangoSelectize-W4FTVNOW.js
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/DjangoSlug-226MVQ6E.js
--rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/DualSelector-ZVBIRYKG.js
--rw-r--r--   0 runner    (1001) docker     (123)   316874 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/RichtextArea-YV4E7SHM.js
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/SortableSelect-MAAIASIY.js
--rw-r--r--   0 runner    (1001) docker     (123)    43947 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-APVD22ED.js
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-ISEEQP4V.js
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-KDP4ZIAK.js
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-MD4VW33H.js
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-NLMHZ7JJ.js
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-R2VNGMYE.js
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/chunk-USKSTMSP.js
--rw-r--r--   0 runner    (1001) docker     (123)   105257 2023-06-13 21:48:00.000000 django-formset-1.0.dev5/formset/static/formset/js/django-formset.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/static/formset/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/scss/bootstrap5-extra.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/static/formset/scss/collections.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.123449 django-formset-1.0.dev5/formset/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.123449 django-formset-1.0.dev5/formset/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/templates/admin/formset/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/admin/formset/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/templates/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/calendar/hours.html
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/calendar/months.html
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/calendar/weeks.html
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/calendar/years.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/templates/formset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.131450 django-formset-1.0.dev5/formset/templates/formset/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.135450 django-formset-1.0.dev5/formset/templates/formset/bootstrap/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.135450 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/richtextarea.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.135450 django-formset-1.0.dev5/formset/templates/formset/bulma/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.135450 django-formset-1.0.dev5/formset/templates/formset/bulma/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.135450 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.135450 django-formset-1.0.dev5/formset/templates/formset/default/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.139449 django-formset-1.0.dev5/formset/templates/formset/default/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/move_all_left.html
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/move_all_right.html
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/move_selected_left.html
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/move_selected_right.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/redo_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_control.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_separator.html
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/buttons/undo_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/dialog_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/field_errors.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.139449 django-formset-1.0.dev5/formset/templates/formset/default/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/datetimepicker.html
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/richtextarea.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/default/widgets/selectize.html
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/form_attrs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.139449 django-formset-1.0.dev5/formset/templates/formset/foundation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.139449 django-formset-1.0.dev5/formset/templates/formset/foundation/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.139449 django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/inlined_input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.143449 django-formset-1.0.dev5/formset/templates/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/add-fill.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/align-center.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/align-justify.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/align-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/align-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/arrow-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/arrow-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/blockquote.svg
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/bold.svg
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/bulletlist.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/calendar-today.svg
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/chevron-double-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/chevron-double-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/clearformat.svg
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/codeblock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/decreasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/delete-back.svg
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/double-chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/double-chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/hardbreak.svg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading.svg
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading1.svg
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading3.svg
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/heading6.svg
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/horizontalrule.svg
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/increasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/indentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/letters.svg
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/orderedlist.svg
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/outdentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/placeholder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/questionmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/send.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/separator.svg
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/subscript.svg
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/superscript.svg
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/textcolor.svg
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/trash.svg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/underline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/icons/unlink.svg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/non_field_errors.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/formset/tailwind/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/formset/tailwind/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/radio.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/formset/uikit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/formset/uikit/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/field_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/formset/uikit/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/formset/uikit/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/richtext/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/bulletlist.html
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/doc.html
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/horizontalrule.html
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/listitem.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.147450 django-formset-1.0.dev5/formset/templates/richtext/marks/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/marks/bold.html
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/marks/code.html
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/marks/italic.html
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/marks/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/marks/textcolor.html
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/marks/underline.html
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/orderedlist.html
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/paragraph.html
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templates/richtext/text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:48:08.151450 django-formset-1.0.dev5/formset/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templatetags/formsetify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/templatetags/richtext.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/formset/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:48:08.151450 django-formset-1.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-13 21:47:19.000000 django-formset-1.0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.854637 django-formset-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-27 21:18:09.000000 django-formset-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-27 21:18:09.000000 django-formset-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-27 21:18:50.854637 django-formset-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-27 21:18:09.000000 django-formset-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.830637 django-formset-1.1/django_formset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-27 21:18:50.000000 django-formset-1.1/django_formset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-07-27 21:18:50.000000 django-formset-1.1/django_formset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:18:50.000000 django-formset-1.1/django_formset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:18:50.000000 django-formset-1.1/django_formset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 21:18:50.000000 django-formset-1.1/django_formset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 21:18:50.000000 django-formset-1.1/django_formset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.830637 django-formset-1.1/formset/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 21:18:09.000000 django-formset-1.1/formset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-27 21:18:09.000000 django-formset-1.1/formset/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-07-27 21:18:09.000000 django-formset-1.1/formset/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-07-27 21:18:09.000000 django-formset-1.1/formset/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 21:18:09.000000 django-formset-1.1/formset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-27 21:18:09.000000 django-formset-1.1/formset/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-27 21:18:09.000000 django-formset-1.1/formset/fieldset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.826637 django-formset-1.1/formset/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.826637 django-formset-1.1/formset/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.830637 django-formset-1.1/formset/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-27 21:18:43.000000 django-formset-1.1/formset/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-07-27 21:18:09.000000 django-formset-1.1/formset/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.834637 django-formset-1.1/formset/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:09.000000 django-formset-1.1/formset/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-27 21:18:09.000000 django-formset-1.1/formset/renderers/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-27 21:18:09.000000 django-formset-1.1/formset/renderers/bulma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-07-27 21:18:09.000000 django-formset-1.1/formset/renderers/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-27 21:18:09.000000 django-formset-1.1/formset/renderers/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-27 21:18:09.000000 django-formset-1.1/formset/renderers/tailwind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-27 21:18:09.000000 django-formset-1.1/formset/renderers/uikit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.834637 django-formset-1.1/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:09.000000 django-formset-1.1/formset/richtext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-27 21:18:09.000000 django-formset-1.1/formset/richtext/controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-27 21:18:09.000000 django-formset-1.1/formset/richtext/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-27 21:18:09.000000 django-formset-1.1/formset/richtext/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-27 21:18:09.000000 django-formset-1.1/formset/richtext/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.826637 django-formset-1.1/formset/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.826637 django-formset-1.1/formset/static/formset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.834637 django-formset-1.1/formset/static/formset/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-27 21:18:41.000000 django-formset-1.1/formset/static/formset/css/bootstrap5-extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-27 21:18:41.000000 django-formset-1.1/formset/static/formset/css/bootstrap5-extra.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-27 21:18:41.000000 django-formset-1.1/formset/static/formset/css/collections.css
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-27 21:18:41.000000 django-formset-1.1/formset/static/formset/css/collections.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    35875 2023-07-27 21:18:42.000000 django-formset-1.1/formset/static/formset/css/tailwind.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.834637 django-formset-1.1/formset/static/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-27 21:18:09.000000 django-formset-1.1/formset/static/formset/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-27 21:18:09.000000 django-formset-1.1/formset/static/formset/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-27 21:18:09.000000 django-formset-1.1/formset/static/formset/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-27 21:18:09.000000 django-formset-1.1/formset/static/formset/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-27 21:18:09.000000 django-formset-1.1/formset/static/formset/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-27 21:18:09.000000 django-formset-1.1/formset/static/formset/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-27 21:18:09.000000 django-formset-1.1/formset/static/formset/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-27 21:18:09.000000 django-formset-1.1/formset/static/formset/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-27 21:18:09.000000 django-formset-1.1/formset/static/formset/icons/file-zip.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.838637 django-formset-1.1/formset/static/formset/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    25365 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/DateTimePicker-UTHDUQQK.js
+-rw-r--r--   0 runner    (1001) docker     (123)    55842 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/DjangoSelectize-2WEWGVUV.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/DjangoSlug-226MVQ6E.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/DualSelector-WBPG3AWC.js
+-rw-r--r--   0 runner    (1001) docker     (123)   316875 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/RichtextArea-XHFBZVPO.js
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/SortableSelect-XJMQCTYG.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43947 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/chunk-APVD22ED.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/chunk-ISEEQP4V.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/chunk-KDP4ZIAK.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/chunk-MD4VW33H.js
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/chunk-NLMHZ7JJ.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/chunk-Q2GK6FIZ.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/chunk-R2VNGMYE.js
+-rw-r--r--   0 runner    (1001) docker     (123)   109797 2023-07-27 21:18:43.000000 django-formset-1.1/formset/static/formset/js/django-formset.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.838637 django-formset-1.1/formset/static/formset/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-27 21:18:09.000000 django-formset-1.1/formset/static/formset/scss/bootstrap5-extra.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-27 21:18:09.000000 django-formset-1.1/formset/static/formset/scss/collections.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.830637 django-formset-1.1/formset/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.826637 django-formset-1.1/formset/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.838637 django-formset-1.1/formset/templates/admin/formset/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/admin/formset/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.838637 django-formset-1.1/formset/templates/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/calendar/hours.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/calendar/months.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/calendar/weeks.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/calendar/years.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.838637 django-formset-1.1/formset/templates/formset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.838637 django-formset-1.1/formset/templates/formset/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.838637 django-formset-1.1/formset/templates/formset/bootstrap/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.838637 django-formset-1.1/formset/templates/formset/bootstrap/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bootstrap/widgets/richtextarea.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.838637 django-formset-1.1/formset/templates/formset/bulma/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.838637 django-formset-1.1/formset/templates/formset/bulma/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bulma/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bulma/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bulma/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bulma/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.842637 django-formset-1.1/formset/templates/formset/bulma/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bulma/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bulma/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bulma/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bulma/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bulma/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/bulma/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.842637 django-formset-1.1/formset/templates/formset/default/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.842637 django-formset-1.1/formset/templates/formset/default/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/move_all_left.html
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/move_all_right.html
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/move_selected_left.html
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/move_selected_right.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/redo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/richtext_control.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/richtext_separator.html
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/buttons/undo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/dialog_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/field_errors.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.842637 django-formset-1.1/formset/templates/formset/default/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/widgets/datetimepicker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/widgets/richtextarea.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/default/widgets/selectize.html
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/form_attrs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.846637 django-formset-1.1/formset/templates/formset/foundation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.846637 django-formset-1.1/formset/templates/formset/foundation/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/foundation/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/foundation/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/foundation/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/foundation/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.846637 django-formset-1.1/formset/templates/formset/foundation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/foundation/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/foundation/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/foundation/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/foundation/widgets/inlined_input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/foundation/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.850637 django-formset-1.1/formset/templates/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/add-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/align-center.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/align-justify.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/align-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/align-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/blockquote.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/bold.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/bulletlist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/calendar-today.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/chevron-double-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/chevron-double-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/clearformat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/codeblock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/decreasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/delete-back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/double-chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/double-chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/hardbreak.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/heading.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/heading1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/heading2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/heading3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/heading4.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/heading5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/heading6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/horizontalrule.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/increasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/indentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/letters.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/orderedlist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/outdentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/placeholder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/questionmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/send.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/separator.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/subscript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/superscript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/textcolor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/underline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/icons/unlink.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/non_field_errors.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.850637 django-formset-1.1/formset/templates/formset/tailwind/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.850637 django-formset-1.1/formset/templates/formset/tailwind/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/tailwind/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/tailwind/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/tailwind/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/tailwind/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/tailwind/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.854637 django-formset-1.1/formset/templates/formset/tailwind/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/tailwind/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/tailwind/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/tailwind/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/tailwind/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/tailwind/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/tailwind/widgets/radio.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.854637 django-formset-1.1/formset/templates/formset/uikit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.854637 django-formset-1.1/formset/templates/formset/uikit/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/uikit/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/uikit/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/uikit/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/uikit/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.854637 django-formset-1.1/formset/templates/formset/uikit/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/uikit/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/uikit/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/uikit/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/formset/uikit/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.854637 django-formset-1.1/formset/templates/richtext/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/bulletlist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/doc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/horizontalrule.html
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/listitem.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.854637 django-formset-1.1/formset/templates/richtext/marks/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/marks/bold.html
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/marks/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/marks/italic.html
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/marks/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/marks/textcolor.html
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/marks/underline.html
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/orderedlist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templates/richtext/text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:50.854637 django-formset-1.1/formset/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templatetags/formsetify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-27 21:18:09.000000 django-formset-1.1/formset/templatetags/richtext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-27 21:18:09.000000 django-formset-1.1/formset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-07-27 21:18:09.000000 django-formset-1.1/formset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-07-27 21:18:09.000000 django-formset-1.1/formset/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-07-27 21:18:09.000000 django-formset-1.1/formset/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:18:50.854637 django-formset-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-27 21:18:09.000000 django-formset-1.1/setup.py
```

### Comparing `django-formset-1.0.dev5/LICENSE` & `django-formset-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/PKG-INFO` & `django-formset-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.0.dev5
+Version: 1.1
 Summary: Prevalidate Django Forms in the browser
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
@@ -15,16 +15,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-formset – Better UX for Django Forms 
 
 This library handles single forms and collections of forms with a way better user experience than
 the internal Django implementation for
@@ -32,15 +34,15 @@
 
 [![Build Status](https://github.com/jrief/django-formset/actions/workflows/tests.yml/badge.svg)](https://github.com/jrief/django-formset/actions)
 [![PyPI version](https://img.shields.io/pypi/v/django-formset.svg)](https://pypi.python.org/pypi/django-formset)
 [![Django versions](https://img.shields.io/pypi/djversions/django-formset)](https://pypi.python.org/pypi/django-formset)
 [![Python versions](https://img.shields.io/pypi/pyversions/django-formset.svg)](https://pypi.python.org/pypi/django-formset)
 [![Software license](https://img.shields.io/pypi/l/django-formset.svg)](https://github.com/jrief/django-formset/blob/master/LICENSE)
 
-[Full documentation on ReadTheDocs](https://django-formset.readthedocs.io/en/latest/)
+[Interactive documentation](https://django-formset.fly.dev/)
 
 Let's explain it using a short example. Say, we have a Django form with three fields:
 
 ```python
 from django.forms import fields, forms
 
 class AddressForm(forms.Form):
@@ -128,15 +130,15 @@
 
 * It can handle relations where the source contains too many entries to be loaded once. Instead,
   this widget queries the database when searching for an option. It uses the same autocomplete
   endpoint.
 * The right part of the widget can be filtered as well.
 * The widget has a redo/undo functionality in case the user mistakenly selected wrong option(s).
 * Optionally, selected options in the right part of the widget can be sorted. This order then is
-  can be refelected in an
+  reflected in an
   [extra field](https://docs.djangoproject.com/en/stable/topics/db/models/#intermediary-manytomany)
    on the many-to-many relationship.
 
 
 ## Button actions
 
 In **django-formset**, the button used for submission can hold a chain of actions. This for instance
@@ -182,16 +184,16 @@
 
 
 ## Conditional hiding/disabling
 
 Since each formset holds its state (the current value of their fields), that information can be used
 to conditionally hide or disable other fields or even a complete fieldset.
 
-By adding the special attributes `show-if="condition"`, `hide-if="condition"` or
-`disable-if="condition"` on an input fields or on a fieldsets, one can hide or disable these marked
+By adding the special attributes `df-show="condition"`, `df-hide="condition"` or
+`df-disable="condition"` on an input fields or on a fieldsets, one can hide or disable these marked
 fields. This `condition` can be any expression evaluating the current field values of the formset.
 
 
 ## How does this all work?
 
 **django-formset** makes use of the
 [form renderer](https://docs.djangoproject.com/en/stable/ref/forms/renderers/) introduced in
```

### Comparing `django-formset-1.0.dev5/README.md` & `django-formset-1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [![Build Status](https://github.com/jrief/django-formset/actions/workflows/tests.yml/badge.svg)](https://github.com/jrief/django-formset/actions)
 [![PyPI version](https://img.shields.io/pypi/v/django-formset.svg)](https://pypi.python.org/pypi/django-formset)
 [![Django versions](https://img.shields.io/pypi/djversions/django-formset)](https://pypi.python.org/pypi/django-formset)
 [![Python versions](https://img.shields.io/pypi/pyversions/django-formset.svg)](https://pypi.python.org/pypi/django-formset)
 [![Software license](https://img.shields.io/pypi/l/django-formset.svg)](https://github.com/jrief/django-formset/blob/master/LICENSE)
 
-[Full documentation on ReadTheDocs](https://django-formset.readthedocs.io/en/latest/)
+[Interactive documentation](https://django-formset.fly.dev/)
 
 Let's explain it using a short example. Say, we have a Django form with three fields:
 
 ```python
 from django.forms import fields, forms
 
 class AddressForm(forms.Form):
@@ -102,15 +102,15 @@
 
 * It can handle relations where the source contains too many entries to be loaded once. Instead,
   this widget queries the database when searching for an option. It uses the same autocomplete
   endpoint.
 * The right part of the widget can be filtered as well.
 * The widget has a redo/undo functionality in case the user mistakenly selected wrong option(s).
 * Optionally, selected options in the right part of the widget can be sorted. This order then is
-  can be refelected in an
+  reflected in an
   [extra field](https://docs.djangoproject.com/en/stable/topics/db/models/#intermediary-manytomany)
    on the many-to-many relationship.
 
 
 ## Button actions
 
 In **django-formset**, the button used for submission can hold a chain of actions. This for instance
@@ -156,16 +156,16 @@
 
 
 ## Conditional hiding/disabling
 
 Since each formset holds its state (the current value of their fields), that information can be used
 to conditionally hide or disable other fields or even a complete fieldset.
 
-By adding the special attributes `show-if="condition"`, `hide-if="condition"` or
-`disable-if="condition"` on an input fields or on a fieldsets, one can hide or disable these marked
+By adding the special attributes `df-show="condition"`, `df-hide="condition"` or
+`df-disable="condition"` on an input fields or on a fieldsets, one can hide or disable these marked
 fields. This `condition` can be any expression evaluating the current field values of the formset.
 
 
 ## How does this all work?
 
 **django-formset** makes use of the
 [form renderer](https://docs.djangoproject.com/en/stable/ref/forms/renderers/) introduced in
```

### Comparing `django-formset-1.0.dev5/django_formset.egg-info/PKG-INFO` & `django-formset-1.1/django_formset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.0.dev5
+Version: 1.1
 Summary: Prevalidate Django Forms in the browser
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
@@ -15,16 +15,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-formset – Better UX for Django Forms 
 
 This library handles single forms and collections of forms with a way better user experience than
 the internal Django implementation for
@@ -32,15 +34,15 @@
 
 [![Build Status](https://github.com/jrief/django-formset/actions/workflows/tests.yml/badge.svg)](https://github.com/jrief/django-formset/actions)
 [![PyPI version](https://img.shields.io/pypi/v/django-formset.svg)](https://pypi.python.org/pypi/django-formset)
 [![Django versions](https://img.shields.io/pypi/djversions/django-formset)](https://pypi.python.org/pypi/django-formset)
 [![Python versions](https://img.shields.io/pypi/pyversions/django-formset.svg)](https://pypi.python.org/pypi/django-formset)
 [![Software license](https://img.shields.io/pypi/l/django-formset.svg)](https://github.com/jrief/django-formset/blob/master/LICENSE)
 
-[Full documentation on ReadTheDocs](https://django-formset.readthedocs.io/en/latest/)
+[Interactive documentation](https://django-formset.fly.dev/)
 
 Let's explain it using a short example. Say, we have a Django form with three fields:
 
 ```python
 from django.forms import fields, forms
 
 class AddressForm(forms.Form):
@@ -128,15 +130,15 @@
 
 * It can handle relations where the source contains too many entries to be loaded once. Instead,
   this widget queries the database when searching for an option. It uses the same autocomplete
   endpoint.
 * The right part of the widget can be filtered as well.
 * The widget has a redo/undo functionality in case the user mistakenly selected wrong option(s).
 * Optionally, selected options in the right part of the widget can be sorted. This order then is
-  can be refelected in an
+  reflected in an
   [extra field](https://docs.djangoproject.com/en/stable/topics/db/models/#intermediary-manytomany)
    on the many-to-many relationship.
 
 
 ## Button actions
 
 In **django-formset**, the button used for submission can hold a chain of actions. This for instance
@@ -182,16 +184,16 @@
 
 
 ## Conditional hiding/disabling
 
 Since each formset holds its state (the current value of their fields), that information can be used
 to conditionally hide or disable other fields or even a complete fieldset.
 
-By adding the special attributes `show-if="condition"`, `hide-if="condition"` or
-`disable-if="condition"` on an input fields or on a fieldsets, one can hide or disable these marked
+By adding the special attributes `df-show="condition"`, `df-hide="condition"` or
+`df-disable="condition"` on an input fields or on a fieldsets, one can hide or disable these marked
 fields. This `condition` can be any expression evaluating the current field values of the formset.
 
 
 ## How does this all work?
 
 **django-formset** makes use of the
 [form renderer](https://docs.djangoproject.com/en/stable/ref/forms/renderers/) introduced in
```

### Comparing `django-formset-1.0.dev5/django_formset.egg-info/SOURCES.txt` & `django-formset-1.1/django_formset.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,27 +43,27 @@
 formset/static/formset/icons/file-font.svg
 formset/static/formset/icons/file-missing.svg
 formset/static/formset/icons/file-pdf.svg
 formset/static/formset/icons/file-picture.svg
 formset/static/formset/icons/file-unknown.svg
 formset/static/formset/icons/file-video.svg
 formset/static/formset/icons/file-zip.svg
-formset/static/formset/js/DateTimePicker-TF2GNHHS.js
-formset/static/formset/js/DjangoSelectize-W4FTVNOW.js
+formset/static/formset/js/DateTimePicker-UTHDUQQK.js
+formset/static/formset/js/DjangoSelectize-2WEWGVUV.js
 formset/static/formset/js/DjangoSlug-226MVQ6E.js
-formset/static/formset/js/DualSelector-ZVBIRYKG.js
-formset/static/formset/js/RichtextArea-YV4E7SHM.js
-formset/static/formset/js/SortableSelect-MAAIASIY.js
+formset/static/formset/js/DualSelector-WBPG3AWC.js
+formset/static/formset/js/RichtextArea-XHFBZVPO.js
+formset/static/formset/js/SortableSelect-XJMQCTYG.js
 formset/static/formset/js/chunk-APVD22ED.js
 formset/static/formset/js/chunk-ISEEQP4V.js
 formset/static/formset/js/chunk-KDP4ZIAK.js
 formset/static/formset/js/chunk-MD4VW33H.js
 formset/static/formset/js/chunk-NLMHZ7JJ.js
+formset/static/formset/js/chunk-Q2GK6FIZ.js
 formset/static/formset/js/chunk-R2VNGMYE.js
-formset/static/formset/js/chunk-USKSTMSP.js
 formset/static/formset/js/django-formset.js
 formset/static/formset/scss/bootstrap5-extra.scss
 formset/static/formset/scss/collections.scss
 formset/templates/admin/formset/change_form.html
 formset/templates/calendar/hours.html
 formset/templates/calendar/months.html
 formset/templates/calendar/weeks.html
```

### Comparing `django-formset-1.0.dev5/formset/boundfield.py` & `django-formset-1.1/formset/boundfield.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/calendar.py` & `django-formset-1.1/formset/calendar.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/collection.py` & `django-formset-1.1/formset/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import operator
+from functools import reduce
+
+from django.core import validators
 from django.core.exceptions import NON_FIELD_ERRORS
 from django.db.utils import IntegrityError
 from django.forms.forms import BaseForm
 from django.forms.models import BaseModelForm, construct_instance, model_to_dict
 from django.forms.utils import ErrorDict, ErrorList, RenderableMixin
 from django.forms.widgets import MediaDefiningClass
 from django.utils.datastructures import MultiValueDict
@@ -63,14 +67,15 @@
     max_siblings = None
     extra_siblings = None
     is_sortable = None
     legend = None
     help_text = None
     add_label = None
     ignore_marked_for_removal = None
+    empty_values = list(validators.EMPTY_VALUES)
 
     def __init__(self, data=None, initial=None, renderer=None, auto_id=None, prefix=None, instance=None,
                  min_siblings=None, max_siblings=None, extra_siblings=None, is_sortable=None, legend=None,
                  help_text=None):
         self.data = MultiValueDict() if data is None else data
         self.initial = initial
         if auto_id is not None:
@@ -89,14 +94,15 @@
         if self.has_many:
             if self.min_siblings is None:
                 self.min_siblings = 1
             if self.extra_siblings is None:
                 self.extra_siblings = 0
             if is_sortable is not None:
                 self.is_sortable = is_sortable
+            self.fresh_and_empty = False
         else:
             self.is_sortable = False
         if legend is not None:
             self.legend = legend
         if help_text is not None:
             self.help_text = help_text
 
@@ -154,14 +160,16 @@
                     ignore_marked_for_removal=self.ignore_marked_for_removal,
                 )
                 holder.position = position
                 if item_num == first:
                     holder.is_first = True
                 if item_num == last:
                     holder.is_last = True
+                if initial in self.empty_values and (position >= self.min_siblings or self.fresh_and_empty):
+                    holder.fresh_and_empty = True
                 yield holder
         # add empty placeholder as template for extra collections
         for item_num, (name, declared_holder) in enumerate(self.declared_holders.items()):
             if self.prefix:
                 count = self.prefix.count('${position')
                 assert count < 10, "Maximum number of nested FormCollections reached"
                 # this context rewriting is necessary to render nested templates properly
@@ -209,14 +217,15 @@
             if isinstance(errors, list):
                 return all(is_valid(e) for e in errors)
             assert isinstance(errors, str)
             return False
 
         if self._errors is None:
             self.full_clean()
+            self.validate_siblings_count()
         return is_valid(self._errors)
 
 
     def full_clean(self):
         if self.has_many:
             self.valid_holders = []
             self._errors = ErrorList()
@@ -229,34 +238,31 @@
                 for name, declared_holder in self.declared_holders.items():
                     if name in data:
                         holder = declared_holder.replicate(
                             data=data[name],
                             instance=instance,
                             ignore_marked_for_removal=self.ignore_marked_for_removal,
                         )
-                        if holder.ignore_marked_for_removal and MARKED_FOR_REMOVAL in holder.data:
-                            break
+                        if MARKED_FOR_REMOVAL in holder.data:
+                            if holder.ignore_marked_for_removal:
+                                break
+                            if getattr(holder, 'has_many', False):
+                                holder.marked_for_removal = True
+                            elif self.has_many:
+                                self.marked_for_removal = True
                         if holder.is_valid():
                             valid_holders[name] = holder
                         errors[name] = holder._errors
                     else:
                         # can only happen, if client bypasses browser control
                         errors[name] = {NON_FIELD_ERRORS: ["Form data is missing."]}
                 else:
                     self.valid_holders.append(valid_holders)
                     self._errors.append(errors)
             self.validate_unique()
-            if len(self.valid_holders) < self.min_siblings:
-                # can only happen, if client bypasses browser control
-                self._errors.clear()
-                self._errors.append({COLLECTION_ERRORS: ["Too few siblings."]})
-            if self.max_siblings and len(self.valid_holders) > self.max_siblings:
-                # can only happen, if client bypasses browser control
-                self._errors.clear()
-                self._errors.append({COLLECTION_ERRORS: ["Too many siblings."]})
         else:
             self.valid_holders = {}
             self._errors = ErrorDict()
             for name, declared_holder in self.declared_holders.items():
                 if name in self.data:
                     instance = self.retrieve_instance(self.data[name])
                     holder = declared_holder.replicate(
@@ -319,14 +325,32 @@
     def get_unique_error_message(self, unique_check):
         if len(unique_check) == 1:
             return gettext_lazy("Please correct the duplicate data for {0}.").format(*unique_check)
         else:
             fields = get_text_list(unique_check, gettext_lazy("and"))
             return gettext_lazy("Please correct the duplicate data for {0}, which must be unique.").format(fields)
 
+    def validate_siblings_count(self):
+        if not self.has_many or self.marked_for_removal:
+            return
+        num_valid_siblings = reduce(
+            operator.add,
+            (all(not h.marked_for_removal for h in vh.values()) for vh in self.valid_holders),
+            0
+        )
+        collection_name = self.legend if self.legend else self.__class__.__name__
+        if num_valid_siblings < self.min_siblings:
+            self._errors.clear()
+            msg = gettext_lazy("Not enough entries in “{collection_name}”, please add another.")
+            self._errors.append({COLLECTION_ERRORS: [msg.format(collection_name=collection_name)]})
+        if self.max_siblings and num_valid_siblings > self.max_siblings:
+            self._errors.clear()
+            msg = gettext_lazy("Too many entries in “{collection_name}”, please remove one.")
+            self._errors.append({COLLECTION_ERRORS: [msg.format(collection_name=collection_name)]})
+
     def retrieve_instance(self, data):
         """
         Hook to retrieve the main object for a multi object collection.
         """
         return self.instance
 
     def clean(self):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-formset-1.0.dev5/formset/fields.py` & `django-formset-1.1/formset/fields.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/locale/de/LC_MESSAGES/django.mo` & `django-formset-1.1/formset/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/locale/de/LC_MESSAGES/django.po` & `django-formset-1.1/formset/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/renderers/bootstrap.py` & `django-formset-1.1/formset/renderers/bootstrap.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from django.utils.html import format_html
+
 from formset.boundfield import ClassList
 from formset.renderers.default import FormRenderer as DefaultFormRenderer
 
-from django.utils.html import format_html
-
 
 class FormRenderer(DefaultFormRenderer):
     max_options_per_line = 4
     framework = 'bootstrap'
 
     def __init__(self, **kwargs):
         kwargs.setdefault('label_css_classes', 'form-label')
```

### Comparing `django-formset-1.0.dev5/formset/renderers/bulma.py` & `django-formset-1.1/formset/renderers/bulma.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/renderers/default.py` & `django-formset-1.1/formset/renderers/default.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/renderers/foundation.py` & `django-formset-1.1/formset/renderers/foundation.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/renderers/tailwind.py` & `django-formset-1.1/formset/renderers/tailwind.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/renderers/uikit.py` & `django-formset-1.1/formset/renderers/uikit.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/richtext/controls.py` & `django-formset-1.1/formset/richtext/controls.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/richtext/dialogs.py` & `django-formset-1.1/formset/richtext/dialogs.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/richtext/widgets.py` & `django-formset-1.1/formset/richtext/widgets.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/css/bootstrap5-extra.css` & `django-formset-1.1/formset/static/formset/css/bootstrap5-extra.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/css/bootstrap5-extra.css.map` & `django-formset-1.1/formset/static/formset/css/bootstrap5-extra.css.map`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/css/collections.css` & `django-formset-1.1/formset/static/formset/css/collections.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/css/tailwind.css` & `django-formset-1.1/formset/static/formset/css/tailwind.css`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/icons/file-audio.svg` & `django-formset-1.1/formset/static/formset/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/icons/file-empty.svg` & `django-formset-1.1/formset/static/formset/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/icons/file-font.svg` & `django-formset-1.1/formset/static/formset/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/icons/file-missing.svg` & `django-formset-1.1/formset/static/formset/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/icons/file-pdf.svg` & `django-formset-1.1/formset/static/formset/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/icons/file-picture.svg` & `django-formset-1.1/formset/static/formset/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/icons/file-unknown.svg` & `django-formset-1.1/formset/static/formset/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/icons/file-video.svg` & `django-formset-1.1/formset/static/formset/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/icons/file-zip.svg` & `django-formset-1.1/formset/static/formset/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/DateTimePicker-TF2GNHHS.js` & `django-formset-1.1/formset/static/formset/js/DateTimePicker-UTHDUQQK.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -31,33 +31,33 @@
                     middleware: [g(), m()]
                 }).then(({
                     y: e
                 }) => Object.assign(this.calendarElement.style, {
                     top: `${e}px`
                 }))
             };
-            this.handleFocus = e => {
+            this.handleFocus = () => {
                 if (this.isOpen) return;
                 this.calendarElement.parentElement.style.position = "relative", this.cleanup = E(this.inputElement, this.calendarElement, this.updatePosition), this.inputElement.setAttribute("aria-expanded", "true");
-                let t = this.inputElement.value;
-                this.inputElement.value = t.trimEnd(), this.inputElement.value !== t && this.inputElement.dispatchEvent(new Event("input")), this.isOpen = !0
+                let e = this.inputElement.value;
+                this.inputElement.value = e.trimEnd(), this.inputElement.value !== e && this.inputElement.dispatchEvent(new Event("input")), this.isOpen = !0
             };
-            this.handleBlur = e => {
+            this.handleBlur = () => {
                 this.isOpen ? this.inputElement.focus() : this.validate()
             };
             this.handleInput = e => {
                 this.isOpen && this.close(), e instanceof InputEvent && e.inputType === "insertText" && (this.inputElement.value = this.inputElement.value.replace("  ", " ").replace(this.delimiter.concat(this.delimiter), this.delimiter).replace("::", ":"), this.autoZeroRegExps.forEach(t => {
                     this.inputElement.value.match(t) && (this.inputElement.value = this.inputElement.value.replace(t, "$10$2"))
                 }), this.autoDelimiterRegExps.forEach(t => {
                     this.inputElement.value.match(t) && (this.inputElement.value = this.inputElement.value.concat(this.delimiter))
                 }), this.autoSpaceRegExp && this.inputElement.value.match(this.autoSpaceRegExp) && (this.inputElement.value = this.inputElement.value.concat(" ")), this.autoColonRegExp && this.inputElement.value.match(this.autoColonRegExp) && (this.inputElement.value = this.inputElement.value.concat(":")))
             };
-            this.handleChange = e => {
-                let t = this.validate();
-                t && this.fetchCalendar(t, this.viewMode)
+            this.handleChange = () => {
+                let e = this.validate();
+                e && this.fetchCalendar(e, this.viewMode)
             };
             this.handleKeypress = async e => {
                 if (!this.isOpen) return;
                 let t = null,
                     s = new Map([
                         ["y", "m"],
                         ["m", "w"],
@@ -85,15 +85,15 @@
                     case "PageUp":
                         t = this.calendarElement.querySelector("button.prev"), t && await this.fetchCalendar(this.getDate(t), this.viewMode);
                         break;
                     case "PageDown":
                         t = this.calendarElement.querySelector("button.next"), t && await this.fetchCalendar(this.getDate(t), this.viewMode);
                         break;
                     case "Enter":
-                        t = this.calendarElement.querySelector(".ranges .selected"), t && (this.viewMode === "h" || this.viewMode === "w" && this.dateOnly ? this.selectDate(t) : this.fetchCalendar(this.getDate(t), s.get(this.viewMode)));
+                        t = this.calendarElement.querySelector(".ranges .selected"), t && (this.viewMode === "h" || this.viewMode === "w" && this.dateOnly ? this.selectDate(t) : await this.fetchCalendar(this.getDate(t), s.get(this.viewMode)));
                         break;
                     default:
                         return
                 }
                 e.preventDefault()
             };
             this.turnPrev = () => {
@@ -158,15 +158,15 @@
             }
         }
         setDateTimeFormat() {
             let e = Array(),
                 t = Array(),
                 s = Array();
             if (this.inputElement.getAttribute("date-format") === "iso") {
-                this.autoZeroRegExps.length = this.autoDelimiterRegExps.length = 0, this.autoZeroRegExps.push(new RegExp("^(\\d{4}-)(\\d{1}-)$")), this.autoZeroRegExps.push(new RegExp("^(\\d{4}-\\d{2}-)(\\d{1}\\s)$")), this.autoDelimiterRegExps.push(new RegExp("^\\d{4}$")), this.autoDelimiterRegExps.push(new RegExp("^\\d{4}-\\d{2}$")), this.dateOnly || (this.autoZeroRegExps.push(new RegExp("^(\\d{4}-\\d{2}-\\d{2}\\s)(\\d{1}:)$")), this.autoSpaceRegExp = new RegExp("^\\d{4}-\\d{2}-\\d{2}$"), this.autoColonRegExp = new RegExp("^\\d{4}-\\d{2}-\\d{2}\\s\\d{2}$")), this.dateOnly ? this.setExtraAttributes("yyyy-mm-dd", "\\d{4}-\\d{2}-\\d{2}") : this.setExtraAttributes("yyyy-mm-dd HH:MM", "\\d{4}-\\d{2}-\\d{2} \\d{2}:\\d{2}");
+                this.autoZeroRegExps.length = this.autoDelimiterRegExps.length = 0, this.autoZeroRegExps.push(new RegExp("^(\\d{4}-)(\\d-)$")), this.autoZeroRegExps.push(new RegExp("^(\\d{4}-\\d{2}-)(\\d\\s)$")), this.autoDelimiterRegExps.push(new RegExp("^\\d{4}$")), this.autoDelimiterRegExps.push(new RegExp("^\\d{4}-\\d{2}$")), this.dateOnly || (this.autoZeroRegExps.push(new RegExp("^(\\d{4}-\\d{2}-\\d{2}\\s)(\\d:)$")), this.autoSpaceRegExp = new RegExp("^\\d{4}-\\d{2}-\\d{2}$"), this.autoColonRegExp = new RegExp("^\\d{4}-\\d{2}-\\d{2}\\s\\d{2}$")), this.dateOnly ? this.setExtraAttributes("yyyy-mm-dd", "\\d{4}-\\d{2}-\\d{2}") : this.setExtraAttributes("yyyy-mm-dd HH:MM", "\\d{4}-\\d{2}-\\d{2} \\d{2}:\\d{2}");
                 return
             }
             this.dateTimeFormat = Intl.DateTimeFormat(navigator.language, {
                 year: "numeric",
                 month: "2-digit",
                 day: "2-digit",
                 hour: "2-digit",
@@ -192,15 +192,15 @@
                         break;
                     case "minute":
                         this.dateOnly || (e.push("MM"), t.push("\\d{2}"), s.push("(?<minute>\\d{1,2})"));
                         break;
                     default:
                         break
                 }
-            }), this.dateTimeRegExp = new RegExp(s.join("")), this.autoZeroRegExps.length = this.autoDelimiterRegExps.length = 0, this.autoDelimiterRegExps.push(new RegExp("^\\d{2}$")), this.delimiter === "." ? (this.autoZeroRegExps.push(new RegExp("^(\\D*)(\\d{1}\\.)$")), this.autoZeroRegExps.push(new RegExp("^(\\d{2}\\.)(\\d{1}\\.)$")), this.autoDelimiterRegExps.push(new RegExp("^\\d{2}\\.\\d{2}$")), this.dateOnly || (this.autoZeroRegExps.push(new RegExp("^(\\d{2}\\.\\d{2}\\.\\d{4}\\s)(\\d{1}:)$")), this.autoSpaceRegExp = new RegExp("^(\\d{2}\\.\\d{2}\\.\\d{4})$"), this.autoColonRegExp = new RegExp("^\\d{2}\\.\\d{2}\\.\\d{4}\\s\\d{2}$"))) : (this.autoZeroRegExps.push(new RegExp("^(\\D*)(\\d{1}/)$")), this.autoZeroRegExps.push(new RegExp("^(\\d{2}/)(\\d{1}/)$")), this.autoDelimiterRegExps.push(new RegExp("^\\d{2}/\\d{2}$")), this.dateOnly || (this.autoZeroRegExps.push(new RegExp("^(\\d{2}/\\d{2}/\\d{4}\\s)(\\d{1}:)$")), this.autoSpaceRegExp = new RegExp("^(\\d{2}/\\d{2}/\\d{4})$"), this.autoColonRegExp = new RegExp("^\\d{2}/\\d{2}/\\d{4}\\s\\d{2}$"))), this.setExtraAttributes(e.join(""), t.join(""))
+            }), this.dateTimeRegExp = new RegExp(s.join("")), this.autoZeroRegExps.length = this.autoDelimiterRegExps.length = 0, this.autoDelimiterRegExps.push(new RegExp("^\\d{2}$")), this.delimiter === "." ? (this.autoZeroRegExps.push(new RegExp("^(\\D*)(\\d\\.)$")), this.autoZeroRegExps.push(new RegExp("^(\\d{2}\\.)(\\d\\.)$")), this.autoDelimiterRegExps.push(new RegExp("^\\d{2}\\.\\d{2}$")), this.dateOnly || (this.autoZeroRegExps.push(new RegExp("^(\\d{2}\\.\\d{2}\\.\\d{4}\\s)(\\d:)$")), this.autoSpaceRegExp = new RegExp("^(\\d{2}\\.\\d{2}\\.\\d{4})$"), this.autoColonRegExp = new RegExp("^\\d{2}\\.\\d{2}\\.\\d{4}\\s\\d{2}$"))) : (this.autoZeroRegExps.push(new RegExp("^(\\D*)(\\d/)$")), this.autoZeroRegExps.push(new RegExp("^(\\d{2}/)(\\d/)$")), this.autoDelimiterRegExps.push(new RegExp("^\\d{2}/\\d{2}$")), this.dateOnly || (this.autoZeroRegExps.push(new RegExp("^(\\d{2}/\\d{2}/\\d{4}\\s)(\\d:)$")), this.autoSpaceRegExp = new RegExp("^(\\d{2}/\\d{2}/\\d{4})$"), this.autoColonRegExp = new RegExp("^\\d{2}/\\d{2}/\\d{4}\\s\\d{2}$"))), this.setExtraAttributes(e.join(""), t.join(""))
         }
         setExtraAttributes(e, t) {
             this.inputElement.hasAttribute("placeholder") || this.inputElement.setAttribute("placeholder", e), this.inputElement.hasAttribute("pattern") || this.inputElement.setAttribute("pattern", t)
         }
         installEventHandlers() {
             this.inputElement.addEventListener("focus", this.handleFocus), this.inputElement.addEventListener("blur", this.handleBlur), this.inputElement.addEventListener("input", this.handleInput), this.inputElement.addEventListener("change", this.handleChange), document.addEventListener("click", this.handleClick), document.addEventListener("keydown", this.handleKeypress)
         }
@@ -450,18 +450,15 @@
         }
         async fetchCalendar(e, t) {
             let s = new URLSearchParams("calendar");
             s.set("date", e.toISOString().slice(0, 10)), s.set("mode", t), this.interval && s.set("interval", String(this.interval));
             let i = await fetch(`${this.endpoint}?${s.toString()}`, {
                 method: "GET"
             });
-            if (i.status === 200) {
-                let a = await i.text();
-                this.calendarElement.innerHTML = a
-            } else console.error(`Failed to fetch from ${this.endpoint} (status=${i.status})`)
+            i.status === 200 ? this.calendarElement.innerHTML = await i.text() : console.error(`Failed to fetch from ${this.endpoint} (status=${i.status})`)
         }
         transferStyles() {
             var s, i, a;
             for (let n = 0; n < document.styleSheets.length; ++n) {
                 let r = (a = (i = (s = document == null ? void 0 : document.styleSheets) == null ? void 0 : s.item(n)) == null ? void 0 : i.cssRules) == null ? void 0 : a.item(0);
                 if (r instanceof CSSStyleRule && r.selectorText.startsWith(':is([is="django-datepicker"], [is="django-datetimepicker"])')) return
             }
@@ -469,15 +466,15 @@
             e.innerText = D, document.head.appendChild(e);
             let t = window.getComputedStyle(this.inputElement).getPropertyValue("height");
             for (let n = 0; e.sheet && n < e.sheet.cssRules.length; n++) {
                 let r = e.sheet.cssRules.item(n),
                     l;
                 switch (r.selectorText) {
                     case ':is([is="django-datepicker"], [is="django-datetimepicker"]) + .dj-calendar':
-                        l = d.extractStyles(this.inputElement, ["background-color", "border", "border-radius", "font-family", "font-size", "font-strech", "font-style", "font-weight", "letter-spacing", "white-space", "line-height"]), e.sheet.insertRule(`${r.selectorText}{${l}}`, ++n);
+                        l = d.extractStyles(this.inputElement, ["background-color", "border", "border-radius", "font-family", "font-size", "font-stretch", "font-style", "font-weight", "letter-spacing", "white-space", "line-height"]), e.sheet.insertRule(`${r.selectorText}{${l}}`, ++n);
                         break;
                     case ':is([is="django-datepicker"], [is="django-datetimepicker"]) + .dj-calendar .controls':
                         l = d.extractStyles(this.inputElement, ["padding"]), e.sheet.insertRule(`${r.selectorText}{${l}}`, ++n);
                         break;
                     case ':is([is="django-datepicker"], [is="django-datetimepicker"]) + .dj-calendar .ranges':
                         l = d.extractStyles(this.inputElement, ["padding"]), e.sheet.insertRule(`${r.selectorText}{${l}}`, ++n);
                         break;
@@ -497,34 +494,34 @@
         formSubmitted(e) {}
         valueAsDate() {
             let e = this.asDate();
             return e ? (this.localTime || e.setTime(e.getTime() - 6e4 * e.getTimezoneOffset()), e) : null
         }
     },
     o = Symbol("DateTimePickerElement"),
-    v = class extends HTMLInputElement {
+    w = class extends HTMLInputElement {
         connectedCallback() {
             let e = this.closest('[role="group"]');
             if (!e) throw new Error(`Attempt to initialize ${this} outside <django-formset>`);
             let t = e.querySelector('[aria-label="calendar"]');
             this[o] = new c(this, t)
         }
         get valueAsDate() {
             return this[o].valueAsDate()
         }
     };
 o;
-var w = class extends HTMLInputElement {
+var v = class extends HTMLInputElement {
     connectedCallback() {
         let e = this.closest('[role="group"]');
         if (!e) throw new Error(`Attempt to initialize ${this} outside <django-formset>`);
         let t = e.querySelector('[aria-label="calendar"]');
         this[o] = new c(this, t)
     }
     get valueAsDate() {
         return this[o].valueAsDate()
     }
 };
 o;
 export {
-    v as DatePickerElement, w as DateTimePickerElement
+    w as DatePickerElement, v as DateTimePickerElement
 };
```

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/DjangoSelectize-W4FTVNOW.js` & `django-formset-1.1/formset/static/formset/js/DjangoSelectize-2WEWGVUV.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1961,15 +1961,15 @@
                     j(p, !0), !e.isLocked && e.shouldDelete([r], p) && (e.removeItem(r), e.refreshOptions(!1), e.inputState())
                 }), r
             }
         })
     }
 }
 var tt = ve(nt());
-var Xe = ".ts-wrapper{position:relative}.ts-wrapper .ts-control{overflow:hidden;box-sizing:border-box;display:flex;flex-wrap:wrap;align-content:center}.ts-wrapper .ts-control>input{flex:1 1 auto;box-sizing:border-box;user-select:auto;box-shadow:none;border:none;padding:0;font-size:inherit;font-weight:inherit;font-style:inherit;font-family:inherit;caret-color:rgba(0,0,0,.15)}.ts-wrapper .ts-control>input::placeholder{opacity:1}.ts-wrapper .ts-control>input::-ms-clear{display:none}.ts-wrapper .ts-control>input:focus{outline:none !important}.ts-wrapper .ts-control>div{flex:0 1 auto;box-sizing:border-box}.ts-wrapper.multi .ts-control{padding:0 6px 3px 10px}.ts-wrapper.multi .ts-control>div{border:1px solid rgba(0,0,0,.15);border-radius:3px;margin:3px 3px 0 0}.ts-wrapper.multi .ts-control>div .remove{text-decoration:none;color:rgba(0,0,0,.15);border-left:1px solid rgba(0,0,0,.15);padding-left:2px;margin-left:2px}.ts-wrapper.multi .ts-control>div .remove:hover{color:inherit}.ts-wrapper.multi .ts-control>div.active{background-color:rgba(0,0,0,.05)}.ts-wrapper.multi.full .ts-control>input{visibility:hidden}.ts-wrapper.multi.has-items:not(.dirty) .ts-control>input::placeholder{opacity:0}.ts-wrapper.focus .ts-control{opacity:1}.ts-wrapper.disabled .ts-control{opacity:1}.ts-wrapper.input-hidden .ts-control>input{opacity:0;position:absolute;left:-10000px}.ts-wrapper:not(.multi).dirty.focus .ts-control .item{display:none}.ts-wrapper .ts-dropdown{position:absolute;top:100%;left:0;width:100%;z-index:10;background:#f4f4f4;backdrop-filter:blur(0.5rem);margin:.125rem 0 0 0;border-top:0 none;box-sizing:border-box}.ts-wrapper .ts-dropdown [data-selectable]{cursor:pointer;overflow:hidden}.ts-wrapper .ts-dropdown [data-selectable]:hover{background-color:#e0ecf4}.ts-wrapper .ts-dropdown [data-selectable] .highlight{background:rgba(255,237,40,.4);border-radius:1px}.ts-wrapper .ts-dropdown .ts-dropdown-content{overflow-y:auto;overflow-x:hidden;overflow-scrolling:touch;scroll-behavior:smooth}.ts-wrapper .ts-dropdown .optgroup .optgroup-header{opacity:.5}.ts-wrapper .ts-dropdown .optgroup .option{margin-left:1em}:host-context([role=group].dj-touched) .ts-wrapper.has-items:not(.input-active) .ts-control{border-color:var(--django-formset-color-valid)}:host-context([role=group].dj-touched) .ts-wrapper.invalid:not(.input-active) .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid.focus .ts-control{opacity:1}";
+var Xe = ".ts-wrapper{position:relative}.ts-wrapper .ts-control{overflow:hidden;box-sizing:border-box;display:flex;flex-wrap:wrap;align-content:center}.ts-wrapper .ts-control>input{flex:1 1 auto;box-sizing:border-box;user-select:auto;box-shadow:none;border:none;padding:0;font-size:inherit;font-weight:inherit;font-style:inherit;font-family:inherit;caret-color:rgba(0,0,0,.15)}.ts-wrapper .ts-control>input::placeholder{opacity:1}.ts-wrapper .ts-control>input::-ms-clear{display:none}.ts-wrapper .ts-control>input:focus{outline:none !important}.ts-wrapper .ts-control>div{flex:0 1 auto;box-sizing:border-box}.ts-wrapper.multi .ts-control{padding:0 6px 3px 10px}.ts-wrapper.multi .ts-control>div{border:1px solid rgba(0,0,0,.15);border-radius:3px;margin:3px 3px 0 0}.ts-wrapper.multi .ts-control>div .remove{text-decoration:none;color:rgba(0,0,0,.15);border-left:1px solid rgba(0,0,0,.15);padding-left:2px;margin-left:2px}.ts-wrapper.multi .ts-control>div .remove:hover{color:inherit}.ts-wrapper.multi.full .ts-control>input{visibility:hidden}.ts-wrapper.multi.has-items:not(.dirty) .ts-control>input::placeholder{opacity:0}.ts-wrapper.focus .ts-control{opacity:1}.ts-wrapper.disabled .ts-control{opacity:1}.ts-wrapper.input-hidden .ts-control>input{opacity:0;position:absolute;left:-10000px}.ts-wrapper:not(.multi).dirty.focus .ts-control .item{display:none}.ts-wrapper .ts-dropdown{position:absolute;top:100%;left:0;width:100%;z-index:10;background:#f4f4f4;backdrop-filter:blur(0.5rem);margin:.125rem 0 0 0;border-top:0 none;box-sizing:border-box}.ts-wrapper .ts-dropdown [data-selectable]{cursor:pointer;overflow:hidden}.ts-wrapper .ts-dropdown [data-selectable][aria-selected=true]{background-color:rgba(0,0,0,.05)}.ts-wrapper .ts-dropdown [data-selectable].selected{background-color:#e0ecf4}.ts-wrapper .ts-dropdown [data-selectable] .highlight{background:rgba(255,237,40,.4);border-radius:1px}.ts-wrapper .ts-dropdown .ts-dropdown-content{overflow-y:auto;overflow-x:hidden;overflow-scrolling:touch;scroll-behavior:smooth}.ts-wrapper .ts-dropdown .optgroup .optgroup-header{opacity:.5}.ts-wrapper .ts-dropdown .optgroup .option{margin-left:1em}:host-context([role=group].dj-touched) .ts-wrapper.has-items:not(.input-active) .ts-control{border-color:var(--django-formset-color-valid)}:host-context([role=group].dj-touched) .ts-wrapper.invalid:not(.input-active) .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid.focus .ts-control{opacity:1}";
 de.define("remove_button", We);
 var He = class extends Pe {
         constructor(e) {
             var o, r;
             super(e);
             this.numOptions = 12;
             this.load = (e, t) => {
@@ -2077,15 +2077,15 @@
                 r = this.shadowRoot.styleSheets.item(0),
                 f = Math.min(Math.max(this.numOptions, 8), 25);
             for (let p = 0; r && p < r.cssRules.length; p++) {
                 let m = r.cssRules.item(p),
                     w;
                 switch (m.selectorText) {
                     case ".ts-wrapper":
-                        w = se.extractStyles(e, ["font-family", "font-size", "font-strech", "font-style", "font-weight", "letter-spacing", "white-space"]), r.insertRule(`${m.selectorText}{${w}}`, ++p);
+                        w = se.extractStyles(e, ["font-family", "font-size", "font-stretch", "font-style", "font-weight", "letter-spacing", "white-space"]), r.insertRule(`${m.selectorText}{${w}}`, ++p);
                         break;
                     case ".ts-wrapper .ts-control":
                         w = se.extractStyles(e, ["background-color", "border", "border-radius", "box-shadow", "color", "padding"]).concat(`width: ${t.width}; min-height: ${t.height};`), r.insertRule(`${m.selectorText}{${w}}`, ++p);
                         break;
                     case ".ts-wrapper .ts-control > input":
                     case ".ts-wrapper .ts-control > div":
                         o && (w = se.extractStyles(o, ["padding-left", "padding-right"]), r.insertRule(`${m.selectorText}{${w}}`, ++p));
@@ -2096,19 +2096,22 @@
                     case ".ts-wrapper.focus .ts-control":
                         e.style.transition = "none", e.classList.add("-focus-"), w = se.extractStyles(e, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), e.classList.remove("-focus-"), r.insertRule(`${m.selectorText}{${w}}`, ++p), e.style.transition = "";
                         break;
                     case ".ts-wrapper.disabled .ts-control":
                         e.classList.add("-disabled-"), w = se.extractStyles(e, ["background-color", "border", "box-shadow", "color", "opacity", "outline", "transition"]), e.classList.remove("-disabled-"), r.insertRule(`${m.selectorText}{${w}}`, ++p);
                         break;
                     case ".ts-wrapper .ts-dropdown":
-                        w = se.extractStyles(e, ["border-right", "border-bottom", "border-left", "color", "padding-left"]).concat(parseFloat(s) > 0 ? `line-height: calc(${s} * 1.2);` : "line-height: 1.4em;"), r.insertRule(`${m.selectorText}{${w}}`, ++p);
+                        w = se.extractStyles(e, ["border-right", "border-bottom", "border-left", "color"]).concat(parseFloat(s) > 0 ? `line-height: calc(${s} * 1.2);` : "line-height: 1.4em;"), r.insertRule(`${m.selectorText}{${w}}`, ++p);
                         break;
                     case ".ts-wrapper .ts-dropdown .ts-dropdown-content":
                         parseFloat(s) > 0 ? w = `max-height: calc(${s} * 1.2 * ${f});` : w = `max-height: ${f*1.4}em;`, r.insertRule(`${m.selectorText}{${w}}`, ++p);
                         break;
+                    case ".ts-wrapper .ts-dropdown [data-selectable]":
+                        w = se.extractStyles(e, ["padding-left"]), r.insertRule(`${m.selectorText}{${w}}`, ++p);
+                        break;
                     case ':host-context([role="group"].dj-submitted) .ts-wrapper.invalid.focus .ts-control':
                         e.style.transition = "none", e.classList.add("-focus-", "-invalid-", "is-invalid"), w = se.extractStyles(e, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), e.classList.remove("-focus-", "-invalid-", "is-invalid"), r.insertRule(`${m.selectorText}{${w}}`, ++p), e.style.transition = "";
                         break;
                     default:
                         break
                 }
             }
```

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/DjangoSlug-226MVQ6E.js` & `django-formset-1.1/formset/static/formset/js/DjangoSlug-226MVQ6E.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/DualSelector-ZVBIRYKG.js` & `django-formset-1.1/formset/static/formset/js/DualSelector-WBPG3AWC.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as d
 } from "./chunk-MD4VW33H.js";
 import {
     a as u,
     b as p
-} from "./chunk-USKSTMSP.js";
+} from "./chunk-Q2GK6FIZ.js";
 import "./chunk-APVD22ED.js";
 import {
     a as g
 } from "./chunk-KDP4ZIAK.js";
 import {
     a as r
 } from "./chunk-R2VNGMYE.js";
```

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/RichtextArea-YV4E7SHM.js` & `django-formset-1.1/formset/static/formset/js/RichtextArea-XHFBZVPO.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -13920,15 +13920,15 @@
                     case ".dj-richtext-wrapper.focused":
                         this.textAreaElement.style.transition = "none", this.textAreaElement.focus(), o = Ue.extractStyles(this.textAreaElement, ["border", "box-shadow", "outline"]), this.textAreaElement.blur(), t.insertRule(`${s.selectorText}{${o}}`, ++i), this.textAreaElement.style.transition = "";
                         break;
                     case ".dj-submitted .dj-richtext-wrapper.focused.invalid":
                         this.textAreaElement.style.transition = "none", this.textAreaElement.classList.add("-focus-", "-invalid-", "is-invalid"), o = Ue.extractStyles(this.textAreaElement, ["border", "box-shadow", "outline"]), this.textAreaElement.classList.remove("-focus-", "-invalid-", "is-invalid"), t.insertRule(`${s.selectorText}{${o}}`, ++i), this.textAreaElement.style.transition = "";
                         break;
                     case ".dj-richtext-wrapper .ProseMirror":
-                        o = Ue.extractStyles(this.textAreaElement, ["font-family", "font-size", "font-strech", "font-style", "font-weight", "letter-spacing", "white-space", "line-height", "overflow", "padding"]), o = o.concat(`top:${e+1}px;`), t.insertRule(`${s.selectorText}{${o}}`, ++i);
+                        o = Ue.extractStyles(this.textAreaElement, ["font-family", "font-size", "font-stretch", "font-style", "font-weight", "letter-spacing", "white-space", "line-height", "overflow", "padding"]), o = o.concat(`top:${e+1}px;`), t.insertRule(`${s.selectorText}{${o}}`, ++i);
                         break;
                     case '.dj-richtext-wrapper [role="menubar"]':
                         o = Ue.extractStyles(this.textAreaElement, ["border-bottom"]), t.insertRule(`${s.selectorText}{${o}}`, ++i);
                         break;
                     case '.dj-richtext-wrapper [role="menubar"] button[aria-haspopup="true"] + ul[role="menu"]':
                         o = Ue.extractStyles(this.textAreaElement, ["border", "z-index"]);
                         let l = new RegExp("z-index:(\\d+);"),
```

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/chunk-APVD22ED.js` & `django-formset-1.1/formset/static/formset/js/chunk-APVD22ED.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/chunk-ISEEQP4V.js` & `django-formset-1.1/formset/static/formset/js/chunk-ISEEQP4V.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/chunk-KDP4ZIAK.js` & `django-formset-1.1/formset/static/formset/js/chunk-KDP4ZIAK.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/chunk-MD4VW33H.js` & `django-formset-1.1/formset/static/formset/js/chunk-MD4VW33H.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/chunk-NLMHZ7JJ.js` & `django-formset-1.1/formset/static/formset/js/chunk-NLMHZ7JJ.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/chunk-R2VNGMYE.js` & `django-formset-1.1/formset/static/formset/js/chunk-R2VNGMYE.js`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/chunk-USKSTMSP.js` & `django-formset-1.1/formset/static/formset/js/chunk-Q2GK6FIZ.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -60,15 +60,15 @@
             let t = this.declaredStyles.sheet,
                 s = e.querySelector("option");
             for (let o = 0; t && o < t.cssRules.length; o++) {
                 let n = t.cssRules.item(o),
                     a;
                 switch (n.selectorText) {
                     case "django-sortable-select":
-                        a = r.extractStyles(e, ["display", "width", "height", "border", "box-shadow", "outline", "overflow", "font-family", "font-size", "font-strech", "font-style", "font-weight", "letter-spacing", "white-space", "line-height"]), t.insertRule(`${n.selectorText}{${a}}`, ++o);
+                        a = r.extractStyles(e, ["display", "width", "height", "border", "box-shadow", "outline", "overflow", "font-family", "font-size", "font-stretch", "font-style", "font-weight", "letter-spacing", "white-space", "line-height"]), t.insertRule(`${n.selectorText}{${a}}`, ++o);
                         break;
                     case "django-sortable-select.focus":
                         e.style.transition = "none", e.focus(), a = r.extractStyles(e, ["border", "box-shadow", "outline"]), e.blur(), t.insertRule(`${n.selectorText}{${a}}`, ++o), e.style.transition = "";
                         break;
                     case "django-sortable-select option.sortable-chosen, django-sortable-select option.sortable-selected":
                         s && (s.selected = !0, a = r.extractStyles(s, ["color", "background-color"]), t.insertRule(`${n.selectorText}{${a}}`, ++o), s.selected = !1);
                         break;
```

### Comparing `django-formset-1.0.dev5/formset/static/formset/js/django-formset.js` & `django-formset-1.1/formset/static/formset/js/django-formset.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,1322 +1,1491 @@
 import {
-    b as lr
+    b as Ar
 } from "./chunk-APVD22ED.js";
 import {
-    a as sr
+    a as kr
 } from "./chunk-KDP4ZIAK.js";
 import {
-    a as dr
+    a as Tr
 } from "./chunk-R2VNGMYE.js";
 import {
-    a as yt,
-    b as _e
+    a as Ye,
+    b as be
 } from "./chunk-NLMHZ7JJ.js";
-var wr = yt((ks, Er) => {
-    var qn = "Expected a function",
-        mr = "__lodash_hash_undefined__",
-        gr = 1 / 0,
-        zn = "[object Function]",
-        Un = "[object GeneratorFunction]",
-        Kn = "[object Symbol]",
-        Jn = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
-        Wn = /^\w*$/,
-        Xn = /^\./,
-        Zn = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
-        Yn = /[\\^$.*+?()[\]{}|]/g,
-        Qn = /\\(\\)?/g,
-        eo = /^\[object .+?Constructor\]$/,
-        to = typeof global == "object" && global && global.Object === Object && global,
-        ro = typeof self == "object" && self && self.Object === Object && self,
-        xt = to || ro || Function("return this")();
+var Br = Ye((Ol, Hr) => {
+    var Eo = "Expected a function",
+        Lr = "__lodash_hash_undefined__",
+        $r = 1 / 0,
+        wo = "[object Function]",
+        ko = "[object GeneratorFunction]",
+        Ao = "[object Symbol]",
+        To = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
+        Co = /^\w*$/,
+        _o = /^\./,
+        Fo = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
+        So = /[\\^$.*+?()[\]{}|]/g,
+        Lo = /\\(\\)?/g,
+        $o = /^\[object .+?Constructor\]$/,
+        Mo = typeof global == "object" && global && global.Object === Object && global,
+        Io = typeof self == "object" && self && self.Object === Object && self,
+        Ft = Mo || Io || Function("return this")();
 
-    function no(t, e) {
+    function Po(t, e) {
         return t == null ? void 0 : t[e]
     }
 
-    function oo(t) {
+    function Oo(t) {
         var e = !1;
         if (t != null && typeof t.toString != "function") try {
             e = !!(t + "")
         } catch {}
         return e
     }
-    var io = Array.prototype,
-        ao = Function.prototype,
-        hr = Object.prototype,
-        jt = xt["__core-js_shared__"],
-        cr = function() {
-            var t = /[^.]+$/.exec(jt && jt.keys && jt.keys.IE_PROTO || "");
+    var Do = Array.prototype,
+        Ro = Function.prototype,
+        Mr = Object.prototype,
+        _t = Ft["__core-js_shared__"],
+        Cr = function() {
+            var t = /[^.]+$/.exec(_t && _t.keys && _t.keys.IE_PROTO || "");
             return t ? "Symbol(src)_1." + t : ""
         }(),
-        br = ao.toString,
-        Et = hr.hasOwnProperty,
-        vr = hr.toString,
-        so = RegExp("^" + br.call(Et).replace(Yn, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
-        ur = xt.Symbol,
-        lo = io.splice,
-        co = yr(xt, "Map"),
-        Ce = yr(Object, "create"),
-        fr = ur ? ur.prototype : void 0,
-        pr = fr ? fr.toString : void 0;
+        Ir = Ro.toString,
+        St = Mr.hasOwnProperty,
+        Pr = Mr.toString,
+        Ho = RegExp("^" + Ir.call(St).replace(So, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
+        _r = Ft.Symbol,
+        Bo = Do.splice,
+        No = Or(Ft, "Map"),
+        $e = Or(Object, "create"),
+        Fr = _r ? _r.prototype : void 0,
+        Sr = Fr ? Fr.toString : void 0;
 
     function ne(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function uo() {
-        this.__data__ = Ce ? Ce(null) : {}
+    function qo() {
+        this.__data__ = $e ? $e(null) : {}
     }
 
-    function fo(t) {
+    function Vo(t) {
         return this.has(t) && delete this.__data__[t]
     }
 
-    function po(t) {
+    function Go(t) {
         var e = this.__data__;
-        if (Ce) {
+        if ($e) {
             var r = e[t];
-            return r === mr ? void 0 : r
+            return r === Lr ? void 0 : r
         }
-        return Et.call(e, t) ? e[t] : void 0
+        return St.call(e, t) ? e[t] : void 0
     }
 
-    function mo(t) {
+    function zo(t) {
         var e = this.__data__;
-        return Ce ? e[t] !== void 0 : Et.call(e, t)
+        return $e ? e[t] !== void 0 : St.call(e, t)
     }
 
-    function go(t, e) {
+    function Uo(t, e) {
         var r = this.__data__;
-        return r[t] = Ce && e === void 0 ? mr : e, this
+        return r[t] = $e && e === void 0 ? Lr : e, this
     }
-    ne.prototype.clear = uo;
-    ne.prototype.delete = fo;
-    ne.prototype.get = po;
-    ne.prototype.has = mo;
-    ne.prototype.set = go;
+    ne.prototype.clear = qo;
+    ne.prototype.delete = Vo;
+    ne.prototype.get = Go;
+    ne.prototype.has = zo;
+    ne.prototype.set = Uo;
 
-    function me(t) {
+    function ye(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function ho() {
+    function Ko() {
         this.__data__ = []
     }
 
-    function bo(t) {
+    function Jo(t) {
         var e = this.__data__,
-            r = Ue(e, t);
+            r = Qe(e, t);
         if (r < 0) return !1;
         var n = e.length - 1;
-        return r == n ? e.pop() : lo.call(e, r, 1), !0
+        return r == n ? e.pop() : Bo.call(e, r, 1), !0
     }
 
-    function vo(t) {
+    function Wo(t) {
         var e = this.__data__,
-            r = Ue(e, t);
+            r = Qe(e, t);
         return r < 0 ? void 0 : e[r][1]
     }
 
-    function yo(t) {
-        return Ue(this.__data__, t) > -1
+    function Xo(t) {
+        return Qe(this.__data__, t) > -1
     }
 
-    function jo(t, e) {
+    function Zo(t, e) {
         var r = this.__data__,
-            n = Ue(r, t);
+            n = Qe(r, t);
         return n < 0 ? r.push([t, e]) : r[n][1] = e, this
     }
-    me.prototype.clear = ho;
-    me.prototype.delete = bo;
-    me.prototype.get = vo;
-    me.prototype.has = yo;
-    me.prototype.set = jo;
+    ye.prototype.clear = Ko;
+    ye.prototype.delete = Jo;
+    ye.prototype.get = Wo;
+    ye.prototype.has = Xo;
+    ye.prototype.set = Zo;
 
     function oe(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function xo() {
+    function Yo() {
         this.__data__ = {
             hash: new ne,
-            map: new(co || me),
+            map: new(No || ye),
             string: new ne
         }
     }
 
-    function Eo(t) {
-        return Ke(this, t).delete(t)
+    function Qo(t) {
+        return et(this, t).delete(t)
     }
 
-    function wo(t) {
-        return Ke(this, t).get(t)
+    function ei(t) {
+        return et(this, t).get(t)
     }
 
-    function ko(t) {
-        return Ke(this, t).has(t)
+    function ti(t) {
+        return et(this, t).has(t)
     }
 
-    function Ao(t, e) {
-        return Ke(this, t).set(t, e), this
+    function ri(t, e) {
+        return et(this, t).set(t, e), this
     }
-    oe.prototype.clear = xo;
-    oe.prototype.delete = Eo;
-    oe.prototype.get = wo;
-    oe.prototype.has = ko;
-    oe.prototype.set = Ao;
+    oe.prototype.clear = Yo;
+    oe.prototype.delete = Qo;
+    oe.prototype.get = ei;
+    oe.prototype.has = ti;
+    oe.prototype.set = ri;
 
-    function Ue(t, e) {
+    function Qe(t, e) {
         for (var r = t.length; r--;)
-            if (Do(t[r][0], e)) return r;
+            if (pi(t[r][0], e)) return r;
         return -1
     }
 
-    function To(t, e) {
-        e = So(e, t) ? [e] : Fo(e);
-        for (var r = 0, n = e.length; t != null && r < n;) t = t[Io(e[r++])];
+    function ni(t, e) {
+        e = si(e, t) ? [e] : ai(e);
+        for (var r = 0, n = e.length; t != null && r < n;) t = t[ui(e[r++])];
         return r && r == n ? t : void 0
     }
 
-    function _o(t) {
-        if (!xr(t) || $o(t)) return !1;
-        var e = Oo(t) || oo(t) ? so : eo;
-        return e.test(Po(t))
+    function oi(t) {
+        if (!Rr(t) || di(t)) return !1;
+        var e = mi(t) || Oo(t) ? Ho : $o;
+        return e.test(fi(t))
     }
 
-    function Co(t) {
+    function ii(t) {
         if (typeof t == "string") return t;
-        if (kt(t)) return pr ? pr.call(t) : "";
+        if ($t(t)) return Sr ? Sr.call(t) : "";
         var e = t + "";
-        return e == "0" && 1 / t == -gr ? "-0" : e
+        return e == "0" && 1 / t == -$r ? "-0" : e
     }
 
-    function Fo(t) {
-        return jr(t) ? t : Mo(t)
+    function ai(t) {
+        return Dr(t) ? t : ci(t)
     }
 
-    function Ke(t, e) {
+    function et(t, e) {
         var r = t.__data__;
-        return Lo(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
+        return li(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
     }
 
-    function yr(t, e) {
-        var r = no(t, e);
-        return _o(r) ? r : void 0
+    function Or(t, e) {
+        var r = Po(t, e);
+        return oi(r) ? r : void 0
     }
 
-    function So(t, e) {
-        if (jr(t)) return !1;
+    function si(t, e) {
+        if (Dr(t)) return !1;
         var r = typeof t;
-        return r == "number" || r == "symbol" || r == "boolean" || t == null || kt(t) ? !0 : Wn.test(t) || !Jn.test(t) || e != null && t in Object(e)
+        return r == "number" || r == "symbol" || r == "boolean" || t == null || $t(t) ? !0 : Co.test(t) || !To.test(t) || e != null && t in Object(e)
     }
 
-    function Lo(t) {
+    function li(t) {
         var e = typeof t;
         return e == "string" || e == "number" || e == "symbol" || e == "boolean" ? t !== "__proto__" : t === null
     }
 
-    function $o(t) {
-        return !!cr && cr in t
+    function di(t) {
+        return !!Cr && Cr in t
     }
-    var Mo = wt(function(t) {
-        t = Ro(t);
+    var ci = Lt(function(t) {
+        t = gi(t);
         var e = [];
-        return Xn.test(t) && e.push(""), t.replace(Zn, function(r, n, i, o) {
-            e.push(i ? o.replace(Qn, "$1") : n || r)
+        return _o.test(t) && e.push(""), t.replace(Fo, function(r, n, i, o) {
+            e.push(i ? o.replace(Lo, "$1") : n || r)
         }), e
     });
 
-    function Io(t) {
-        if (typeof t == "string" || kt(t)) return t;
+    function ui(t) {
+        if (typeof t == "string" || $t(t)) return t;
         var e = t + "";
-        return e == "0" && 1 / t == -gr ? "-0" : e
+        return e == "0" && 1 / t == -$r ? "-0" : e
     }
 
-    function Po(t) {
+    function fi(t) {
         if (t != null) {
             try {
-                return br.call(t)
+                return Ir.call(t)
             } catch {}
             try {
                 return t + ""
             } catch {}
         }
         return ""
     }
 
-    function wt(t, e) {
-        if (typeof t != "function" || e && typeof e != "function") throw new TypeError(qn);
+    function Lt(t, e) {
+        if (typeof t != "function" || e && typeof e != "function") throw new TypeError(Eo);
         var r = function() {
             var n = arguments,
                 i = e ? e.apply(this, n) : n[0],
                 o = r.cache;
             if (o.has(i)) return o.get(i);
             var s = t.apply(this, n);
             return r.cache = o.set(i, s), s
         };
-        return r.cache = new(wt.Cache || oe), r
+        return r.cache = new(Lt.Cache || oe), r
     }
-    wt.Cache = oe;
+    Lt.Cache = oe;
 
-    function Do(t, e) {
+    function pi(t, e) {
         return t === e || t !== t && e !== e
     }
-    var jr = Array.isArray;
+    var Dr = Array.isArray;
 
-    function Oo(t) {
-        var e = xr(t) ? vr.call(t) : "";
-        return e == zn || e == Un
+    function mi(t) {
+        var e = Rr(t) ? Pr.call(t) : "";
+        return e == wo || e == ko
     }
 
-    function xr(t) {
+    function Rr(t) {
         var e = typeof t;
         return !!t && (e == "object" || e == "function")
     }
 
-    function Ho(t) {
+    function hi(t) {
         return !!t && typeof t == "object"
     }
 
-    function kt(t) {
-        return typeof t == "symbol" || Ho(t) && vr.call(t) == Kn
+    function $t(t) {
+        return typeof t == "symbol" || hi(t) && Pr.call(t) == Ao
     }
 
-    function Ro(t) {
-        return t == null ? "" : Co(t)
+    function gi(t) {
+        return t == null ? "" : ii(t)
     }
 
-    function Bo(t, e, r) {
-        var n = t == null ? void 0 : To(t, e);
+    function bi(t, e, r) {
+        var n = t == null ? void 0 : ni(t, e);
         return n === void 0 ? r : n
     }
-    Er.exports = Bo
+    Hr.exports = bi
 });
-var Or = yt((As, Dr) => {
-    var No = "Expected a function",
-        Cr = "__lodash_hash_undefined__",
-        Fr = 1 / 0,
-        Vo = 9007199254740991,
-        Go = "[object Function]",
-        qo = "[object GeneratorFunction]",
-        zo = "[object Symbol]",
-        Uo = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
-        Ko = /^\w*$/,
-        Jo = /^\./,
-        Wo = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
-        Xo = /[\\^$.*+?()[\]{}|]/g,
-        Zo = /\\(\\)?/g,
-        Yo = /^\[object .+?Constructor\]$/,
-        Qo = /^(?:0|[1-9]\d*)$/,
-        ei = typeof global == "object" && global && global.Object === Object && global,
-        ti = typeof self == "object" && self && self.Object === Object && self,
-        Tt = ei || ti || Function("return this")();
+var en = Ye((Dl, Qr) => {
+    var yi = "Expected a function",
+        zr = "__lodash_hash_undefined__",
+        Ur = 1 / 0,
+        vi = 9007199254740991,
+        ji = "[object Function]",
+        xi = "[object GeneratorFunction]",
+        Ei = "[object Symbol]",
+        wi = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
+        ki = /^\w*$/,
+        Ai = /^\./,
+        Ti = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
+        Ci = /[\\^$.*+?()[\]{}|]/g,
+        _i = /\\(\\)?/g,
+        Fi = /^\[object .+?Constructor\]$/,
+        Si = /^(?:0|[1-9]\d*)$/,
+        Li = typeof global == "object" && global && global.Object === Object && global,
+        $i = typeof self == "object" && self && self.Object === Object && self,
+        It = Li || $i || Function("return this")();
 
-    function ri(t, e) {
+    function Mi(t, e) {
         return t == null ? void 0 : t[e]
     }
 
-    function ni(t) {
+    function Ii(t) {
         var e = !1;
         if (t != null && typeof t.toString != "function") try {
             e = !!(t + "")
         } catch {}
         return e
     }
-    var oi = Array.prototype,
-        ii = Function.prototype,
-        Sr = Object.prototype,
-        At = Tt["__core-js_shared__"],
-        kr = function() {
-            var t = /[^.]+$/.exec(At && At.keys && At.keys.IE_PROTO || "");
+    var Pi = Array.prototype,
+        Oi = Function.prototype,
+        Kr = Object.prototype,
+        Mt = It["__core-js_shared__"],
+        Nr = function() {
+            var t = /[^.]+$/.exec(Mt && Mt.keys && Mt.keys.IE_PROTO || "");
             return t ? "Symbol(src)_1." + t : ""
         }(),
-        Lr = ii.toString,
-        We = Sr.hasOwnProperty,
-        $r = Sr.toString,
-        ai = RegExp("^" + Lr.call(We).replace(Xo, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
-        Ar = Tt.Symbol,
-        si = oi.splice,
-        li = Mr(Tt, "Map"),
-        Fe = Mr(Object, "create"),
-        Tr = Ar ? Ar.prototype : void 0,
-        _r = Tr ? Tr.toString : void 0;
+        Jr = Oi.toString,
+        rt = Kr.hasOwnProperty,
+        Wr = Kr.toString,
+        Di = RegExp("^" + Jr.call(rt).replace(Ci, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
+        qr = It.Symbol,
+        Ri = Pi.splice,
+        Hi = Xr(It, "Map"),
+        Me = Xr(Object, "create"),
+        Vr = qr ? qr.prototype : void 0,
+        Gr = Vr ? Vr.toString : void 0;
 
     function ie(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function di() {
-        this.__data__ = Fe ? Fe(null) : {}
+    function Bi() {
+        this.__data__ = Me ? Me(null) : {}
     }
 
-    function ci(t) {
+    function Ni(t) {
         return this.has(t) && delete this.__data__[t]
     }
 
-    function ui(t) {
+    function qi(t) {
         var e = this.__data__;
-        if (Fe) {
+        if (Me) {
             var r = e[t];
-            return r === Cr ? void 0 : r
+            return r === zr ? void 0 : r
         }
-        return We.call(e, t) ? e[t] : void 0
+        return rt.call(e, t) ? e[t] : void 0
     }
 
-    function fi(t) {
+    function Vi(t) {
         var e = this.__data__;
-        return Fe ? e[t] !== void 0 : We.call(e, t)
+        return Me ? e[t] !== void 0 : rt.call(e, t)
     }
 
-    function pi(t, e) {
+    function Gi(t, e) {
         var r = this.__data__;
-        return r[t] = Fe && e === void 0 ? Cr : e, this
+        return r[t] = Me && e === void 0 ? zr : e, this
     }
-    ie.prototype.clear = di;
-    ie.prototype.delete = ci;
-    ie.prototype.get = ui;
-    ie.prototype.has = fi;
-    ie.prototype.set = pi;
+    ie.prototype.clear = Bi;
+    ie.prototype.delete = Ni;
+    ie.prototype.get = qi;
+    ie.prototype.has = Vi;
+    ie.prototype.set = Gi;
 
-    function ge(t) {
+    function ve(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function mi() {
+    function zi() {
         this.__data__ = []
     }
 
-    function gi(t) {
+    function Ui(t) {
         var e = this.__data__,
-            r = Xe(e, t);
+            r = nt(e, t);
         if (r < 0) return !1;
         var n = e.length - 1;
-        return r == n ? e.pop() : si.call(e, r, 1), !0
+        return r == n ? e.pop() : Ri.call(e, r, 1), !0
     }
 
-    function hi(t) {
+    function Ki(t) {
         var e = this.__data__,
-            r = Xe(e, t);
+            r = nt(e, t);
         return r < 0 ? void 0 : e[r][1]
     }
 
-    function bi(t) {
-        return Xe(this.__data__, t) > -1
+    function Ji(t) {
+        return nt(this.__data__, t) > -1
     }
 
-    function vi(t, e) {
+    function Wi(t, e) {
         var r = this.__data__,
-            n = Xe(r, t);
+            n = nt(r, t);
         return n < 0 ? r.push([t, e]) : r[n][1] = e, this
     }
-    ge.prototype.clear = mi;
-    ge.prototype.delete = gi;
-    ge.prototype.get = hi;
-    ge.prototype.has = bi;
-    ge.prototype.set = vi;
+    ve.prototype.clear = zi;
+    ve.prototype.delete = Ui;
+    ve.prototype.get = Ki;
+    ve.prototype.has = Ji;
+    ve.prototype.set = Wi;
 
     function ae(t) {
         var e = -1,
             r = t ? t.length : 0;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function yi() {
+    function Xi() {
         this.__data__ = {
             hash: new ie,
-            map: new(li || ge),
+            map: new(Hi || ve),
             string: new ie
         }
     }
 
-    function ji(t) {
-        return Ze(this, t).delete(t)
+    function Zi(t) {
+        return ot(this, t).delete(t)
     }
 
-    function xi(t) {
-        return Ze(this, t).get(t)
+    function Yi(t) {
+        return ot(this, t).get(t)
     }
 
-    function Ei(t) {
-        return Ze(this, t).has(t)
+    function Qi(t) {
+        return ot(this, t).has(t)
     }
 
-    function wi(t, e) {
-        return Ze(this, t).set(t, e), this
+    function ea(t, e) {
+        return ot(this, t).set(t, e), this
     }
-    ae.prototype.clear = yi;
-    ae.prototype.delete = ji;
-    ae.prototype.get = xi;
-    ae.prototype.has = Ei;
-    ae.prototype.set = wi;
+    ae.prototype.clear = Xi;
+    ae.prototype.delete = Zi;
+    ae.prototype.get = Yi;
+    ae.prototype.has = Qi;
+    ae.prototype.set = ea;
 
-    function ki(t, e, r) {
+    function ta(t, e, r) {
         var n = t[e];
-        (!(We.call(t, e) && Ir(n, r)) || r === void 0 && !(e in t)) && (t[e] = r)
+        (!(rt.call(t, e) && Zr(n, r)) || r === void 0 && !(e in t)) && (t[e] = r)
     }
 
-    function Xe(t, e) {
+    function nt(t, e) {
         for (var r = t.length; r--;)
-            if (Ir(t[r][0], e)) return r;
+            if (Zr(t[r][0], e)) return r;
         return -1
     }
 
-    function Ai(t) {
-        if (!Je(t) || $i(t)) return !1;
-        var e = Di(t) || ni(t) ? ai : Yo;
-        return e.test(Pi(t))
+    function ra(t) {
+        if (!tt(t) || da(t)) return !1;
+        var e = pa(t) || Ii(t) ? Di : Fi;
+        return e.test(fa(t))
     }
 
-    function Ti(t, e, r, n) {
-        if (!Je(t)) return t;
-        e = Si(e, t) ? [e] : Ci(e);
-        for (var i = -1, o = e.length, s = o - 1, u = t; u != null && ++i < o;) {
-            var f = Ii(e[i]),
-                d = r;
+    function na(t, e, r, n) {
+        if (!tt(t)) return t;
+        e = sa(e, t) ? [e] : ia(e);
+        for (var i = -1, o = e.length, s = o - 1, d = t; d != null && ++i < o;) {
+            var f = ua(e[i]),
+                c = r;
             if (i != s) {
-                var h = u[f];
-                d = n ? n(h, f, u) : void 0, d === void 0 && (d = Je(h) ? h : Fi(e[i + 1]) ? [] : {})
+                var g = d[f];
+                c = n ? n(g, f, d) : void 0, c === void 0 && (c = tt(g) ? g : aa(e[i + 1]) ? [] : {})
             }
-            ki(u, f, d), u = u[f]
+            ta(d, f, c), d = d[f]
         }
         return t
     }
 
-    function _i(t) {
+    function oa(t) {
         if (typeof t == "string") return t;
-        if (Ct(t)) return _r ? _r.call(t) : "";
+        if (Ot(t)) return Gr ? Gr.call(t) : "";
         var e = t + "";
-        return e == "0" && 1 / t == -Fr ? "-0" : e
+        return e == "0" && 1 / t == -Ur ? "-0" : e
     }
 
-    function Ci(t) {
-        return Pr(t) ? t : Mi(t)
+    function ia(t) {
+        return Yr(t) ? t : ca(t)
     }
 
-    function Ze(t, e) {
+    function ot(t, e) {
         var r = t.__data__;
-        return Li(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
+        return la(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
     }
 
-    function Mr(t, e) {
-        var r = ri(t, e);
-        return Ai(r) ? r : void 0
+    function Xr(t, e) {
+        var r = Mi(t, e);
+        return ra(r) ? r : void 0
     }
 
-    function Fi(t, e) {
-        return e = e ?? Vo, !!e && (typeof t == "number" || Qo.test(t)) && t > -1 && t % 1 == 0 && t < e
+    function aa(t, e) {
+        return e = e ?? vi, !!e && (typeof t == "number" || Si.test(t)) && t > -1 && t % 1 == 0 && t < e
     }
 
-    function Si(t, e) {
-        if (Pr(t)) return !1;
+    function sa(t, e) {
+        if (Yr(t)) return !1;
         var r = typeof t;
-        return r == "number" || r == "symbol" || r == "boolean" || t == null || Ct(t) ? !0 : Ko.test(t) || !Uo.test(t) || e != null && t in Object(e)
+        return r == "number" || r == "symbol" || r == "boolean" || t == null || Ot(t) ? !0 : ki.test(t) || !wi.test(t) || e != null && t in Object(e)
     }
 
-    function Li(t) {
+    function la(t) {
         var e = typeof t;
         return e == "string" || e == "number" || e == "symbol" || e == "boolean" ? t !== "__proto__" : t === null
     }
 
-    function $i(t) {
-        return !!kr && kr in t
+    function da(t) {
+        return !!Nr && Nr in t
     }
-    var Mi = _t(function(t) {
-        t = Hi(t);
+    var ca = Pt(function(t) {
+        t = ha(t);
         var e = [];
-        return Jo.test(t) && e.push(""), t.replace(Wo, function(r, n, i, o) {
-            e.push(i ? o.replace(Zo, "$1") : n || r)
+        return Ai.test(t) && e.push(""), t.replace(Ti, function(r, n, i, o) {
+            e.push(i ? o.replace(_i, "$1") : n || r)
         }), e
     });
 
-    function Ii(t) {
-        if (typeof t == "string" || Ct(t)) return t;
+    function ua(t) {
+        if (typeof t == "string" || Ot(t)) return t;
         var e = t + "";
-        return e == "0" && 1 / t == -Fr ? "-0" : e
+        return e == "0" && 1 / t == -Ur ? "-0" : e
     }
 
-    function Pi(t) {
+    function fa(t) {
         if (t != null) {
             try {
-                return Lr.call(t)
+                return Jr.call(t)
             } catch {}
             try {
                 return t + ""
             } catch {}
         }
         return ""
     }
 
-    function _t(t, e) {
-        if (typeof t != "function" || e && typeof e != "function") throw new TypeError(No);
+    function Pt(t, e) {
+        if (typeof t != "function" || e && typeof e != "function") throw new TypeError(yi);
         var r = function() {
             var n = arguments,
                 i = e ? e.apply(this, n) : n[0],
                 o = r.cache;
             if (o.has(i)) return o.get(i);
             var s = t.apply(this, n);
             return r.cache = o.set(i, s), s
         };
-        return r.cache = new(_t.Cache || ae), r
+        return r.cache = new(Pt.Cache || ae), r
     }
-    _t.Cache = ae;
+    Pt.Cache = ae;
 
-    function Ir(t, e) {
+    function Zr(t, e) {
         return t === e || t !== t && e !== e
     }
-    var Pr = Array.isArray;
+    var Yr = Array.isArray;
 
-    function Di(t) {
-        var e = Je(t) ? $r.call(t) : "";
-        return e == Go || e == qo
+    function pa(t) {
+        var e = tt(t) ? Wr.call(t) : "";
+        return e == ji || e == xi
     }
 
-    function Je(t) {
+    function tt(t) {
         var e = typeof t;
         return !!t && (e == "object" || e == "function")
     }
 
-    function Oi(t) {
+    function ma(t) {
         return !!t && typeof t == "object"
     }
 
-    function Ct(t) {
-        return typeof t == "symbol" || Oi(t) && $r.call(t) == zo
+    function Ot(t) {
+        return typeof t == "symbol" || ma(t) && Wr.call(t) == Ei
     }
 
-    function Hi(t) {
-        return t == null ? "" : _i(t)
+    function ha(t) {
+        return t == null ? "" : oa(t)
     }
 
-    function Ri(t, e, r) {
-        return t == null ? t : Ti(t, e, r)
+    function ga(t, e, r) {
+        return t == null ? t : na(t, e, r)
     }
-    Dr.exports = Ri
+    Qr.exports = ga
 });
-var yn = yt((Se, be) => {
-    var Bi = 200,
-        Rt = "__lodash_hash_undefined__",
-        it = 1,
-        Wr = 2,
-        Xr = 9007199254740991,
-        Ye = "[object Arguments]",
-        $t = "[object Array]",
-        Ni = "[object AsyncFunction]",
-        Zr = "[object Boolean]",
-        Yr = "[object Date]",
-        Qr = "[object Error]",
-        en = "[object Function]",
-        Vi = "[object GeneratorFunction]",
-        Qe = "[object Map]",
-        tn = "[object Number]",
-        Gi = "[object Null]",
-        he = "[object Object]",
-        Hr = "[object Promise]",
-        qi = "[object Proxy]",
-        rn = "[object RegExp]",
-        et = "[object Set]",
-        nn = "[object String]",
-        zi = "[object Symbol]",
-        Ui = "[object Undefined]",
-        Mt = "[object WeakMap]",
-        on = "[object ArrayBuffer]",
-        tt = "[object DataView]",
-        Ki = "[object Float32Array]",
-        Ji = "[object Float64Array]",
-        Wi = "[object Int8Array]",
-        Xi = "[object Int16Array]",
-        Zi = "[object Int32Array]",
-        Yi = "[object Uint8Array]",
-        Qi = "[object Uint8ClampedArray]",
-        ea = "[object Uint16Array]",
-        ta = "[object Uint32Array]",
-        ra = /[\\^$.*+?()[\]{}|]/g,
-        na = /^\[object .+?Constructor\]$/,
-        oa = /^(?:0|[1-9]\d*)$/,
+var On = Ye((Ie, xe) => {
+    var ba = 200,
+        Kt = "__lodash_hash_undefined__",
+        ft = 1,
+        pn = 2,
+        mn = 9007199254740991,
+        it = "[object Arguments]",
+        Bt = "[object Array]",
+        ya = "[object AsyncFunction]",
+        hn = "[object Boolean]",
+        gn = "[object Date]",
+        bn = "[object Error]",
+        yn = "[object Function]",
+        va = "[object GeneratorFunction]",
+        at = "[object Map]",
+        vn = "[object Number]",
+        ja = "[object Null]",
+        je = "[object Object]",
+        tn = "[object Promise]",
+        xa = "[object Proxy]",
+        jn = "[object RegExp]",
+        st = "[object Set]",
+        xn = "[object String]",
+        Ea = "[object Symbol]",
+        wa = "[object Undefined]",
+        Nt = "[object WeakMap]",
+        En = "[object ArrayBuffer]",
+        lt = "[object DataView]",
+        ka = "[object Float32Array]",
+        Aa = "[object Float64Array]",
+        Ta = "[object Int8Array]",
+        Ca = "[object Int16Array]",
+        _a = "[object Int32Array]",
+        Fa = "[object Uint8Array]",
+        Sa = "[object Uint8ClampedArray]",
+        La = "[object Uint16Array]",
+        $a = "[object Uint32Array]",
+        Ma = /[\\^$.*+?()[\]{}|]/g,
+        Ia = /^\[object .+?Constructor\]$/,
+        Pa = /^(?:0|[1-9]\d*)$/,
         S = {};
-    S[Ki] = S[Ji] = S[Wi] = S[Xi] = S[Zi] = S[Yi] = S[Qi] = S[ea] = S[ta] = !0;
-    S[Ye] = S[$t] = S[on] = S[Zr] = S[tt] = S[Yr] = S[Qr] = S[en] = S[Qe] = S[tn] = S[he] = S[rn] = S[et] = S[nn] = S[Mt] = !1;
-    var an = typeof global == "object" && global && global.Object === Object && global,
-        ia = typeof self == "object" && self && self.Object === Object && self,
-        W = an || ia || Function("return this")(),
-        sn = typeof Se == "object" && Se && !Se.nodeType && Se,
-        Rr = sn && typeof be == "object" && be && !be.nodeType && be,
-        ln = Rr && Rr.exports === sn,
-        Ft = ln && an.process,
-        Br = function() {
+    S[ka] = S[Aa] = S[Ta] = S[Ca] = S[_a] = S[Fa] = S[Sa] = S[La] = S[$a] = !0;
+    S[it] = S[Bt] = S[En] = S[hn] = S[lt] = S[gn] = S[bn] = S[yn] = S[at] = S[vn] = S[je] = S[jn] = S[st] = S[xn] = S[Nt] = !1;
+    var wn = typeof global == "object" && global && global.Object === Object && global,
+        Oa = typeof self == "object" && self && self.Object === Object && self,
+        W = wn || Oa || Function("return this")(),
+        kn = typeof Ie == "object" && Ie && !Ie.nodeType && Ie,
+        rn = kn && typeof xe == "object" && xe && !xe.nodeType && xe,
+        An = rn && rn.exports === kn,
+        Dt = An && wn.process,
+        nn = function() {
             try {
-                return Ft && Ft.binding && Ft.binding("util")
+                return Dt && Dt.binding && Dt.binding("util")
             } catch {}
         }(),
-        Nr = Br && Br.isTypedArray;
+        on = nn && nn.isTypedArray;
 
-    function aa(t, e) {
+    function Da(t, e) {
         for (var r = -1, n = t == null ? 0 : t.length, i = 0, o = []; ++r < n;) {
             var s = t[r];
             e(s, r, t) && (o[i++] = s)
         }
         return o
     }
 
-    function sa(t, e) {
+    function Ra(t, e) {
         for (var r = -1, n = e.length, i = t.length; ++r < n;) t[i + r] = e[r];
         return t
     }
 
-    function la(t, e) {
+    function Ha(t, e) {
         for (var r = -1, n = t == null ? 0 : t.length; ++r < n;)
             if (e(t[r], r, t)) return !0;
         return !1
     }
 
-    function da(t, e) {
+    function Ba(t, e) {
         for (var r = -1, n = Array(t); ++r < t;) n[r] = e(r);
         return n
     }
 
-    function ca(t) {
+    function Na(t) {
         return function(e) {
             return t(e)
         }
     }
 
-    function ua(t, e) {
+    function qa(t, e) {
         return t.has(e)
     }
 
-    function fa(t, e) {
+    function Va(t, e) {
         return t == null ? void 0 : t[e]
     }
 
-    function pa(t) {
+    function Ga(t) {
         var e = -1,
             r = Array(t.size);
         return t.forEach(function(n, i) {
             r[++e] = [i, n]
         }), r
     }
 
-    function ma(t, e) {
+    function za(t, e) {
         return function(r) {
             return t(e(r))
         }
     }
 
-    function ga(t) {
+    function Ua(t) {
         var e = -1,
             r = Array(t.size);
         return t.forEach(function(n) {
             r[++e] = n
         }), r
     }
-    var ha = Array.prototype,
-        ba = Function.prototype,
-        at = Object.prototype,
-        St = W["__core-js_shared__"],
-        dn = ba.toString,
-        K = at.hasOwnProperty,
-        Vr = function() {
-            var t = /[^.]+$/.exec(St && St.keys && St.keys.IE_PROTO || "");
+    var Ka = Array.prototype,
+        Ja = Function.prototype,
+        pt = Object.prototype,
+        Rt = W["__core-js_shared__"],
+        Tn = Ja.toString,
+        K = pt.hasOwnProperty,
+        an = function() {
+            var t = /[^.]+$/.exec(Rt && Rt.keys && Rt.keys.IE_PROTO || "");
             return t ? "Symbol(src)_1." + t : ""
         }(),
-        cn = at.toString,
-        va = RegExp("^" + dn.call(K).replace(ra, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
-        Gr = ln ? W.Buffer : void 0,
-        rt = W.Symbol,
-        qr = W.Uint8Array,
-        un = at.propertyIsEnumerable,
-        ya = ha.splice,
-        se = rt ? rt.toStringTag : void 0,
-        zr = Object.getOwnPropertySymbols,
-        ja = Gr ? Gr.isBuffer : void 0,
-        xa = ma(Object.keys, Object),
-        It = ve(W, "DataView"),
-        Le = ve(W, "Map"),
-        Pt = ve(W, "Promise"),
-        Dt = ve(W, "Set"),
-        Ot = ve(W, "WeakMap"),
-        $e = ve(Object, "create"),
-        Ea = ce(It),
-        wa = ce(Le),
-        ka = ce(Pt),
-        Aa = ce(Dt),
-        Ta = ce(Ot),
-        Ur = rt ? rt.prototype : void 0,
-        Lt = Ur ? Ur.valueOf : void 0;
+        Cn = pt.toString,
+        Wa = RegExp("^" + Tn.call(K).replace(Ma, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
+        sn = An ? W.Buffer : void 0,
+        dt = W.Symbol,
+        ln = W.Uint8Array,
+        _n = pt.propertyIsEnumerable,
+        Xa = Ka.splice,
+        se = dt ? dt.toStringTag : void 0,
+        dn = Object.getOwnPropertySymbols,
+        Za = sn ? sn.isBuffer : void 0,
+        Ya = za(Object.keys, Object),
+        qt = Ee(W, "DataView"),
+        Pe = Ee(W, "Map"),
+        Vt = Ee(W, "Promise"),
+        Gt = Ee(W, "Set"),
+        zt = Ee(W, "WeakMap"),
+        Oe = Ee(Object, "create"),
+        Qa = ce(qt),
+        es = ce(Pe),
+        ts = ce(Vt),
+        rs = ce(Gt),
+        ns = ce(zt),
+        cn = dt ? dt.prototype : void 0,
+        Ht = cn ? cn.valueOf : void 0;
 
     function le(t) {
         var e = -1,
             r = t == null ? 0 : t.length;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function _a() {
-        this.__data__ = $e ? $e(null) : {}, this.size = 0
+    function os() {
+        this.__data__ = Oe ? Oe(null) : {}, this.size = 0
     }
 
-    function Ca(t) {
+    function is(t) {
         var e = this.has(t) && delete this.__data__[t];
         return this.size -= e ? 1 : 0, e
     }
 
-    function Fa(t) {
+    function as(t) {
         var e = this.__data__;
-        if ($e) {
+        if (Oe) {
             var r = e[t];
-            return r === Rt ? void 0 : r
+            return r === Kt ? void 0 : r
         }
         return K.call(e, t) ? e[t] : void 0
     }
 
-    function Sa(t) {
+    function ss(t) {
         var e = this.__data__;
-        return $e ? e[t] !== void 0 : K.call(e, t)
+        return Oe ? e[t] !== void 0 : K.call(e, t)
     }
 
-    function La(t, e) {
+    function ls(t, e) {
         var r = this.__data__;
-        return this.size += this.has(t) ? 0 : 1, r[t] = $e && e === void 0 ? Rt : e, this
+        return this.size += this.has(t) ? 0 : 1, r[t] = Oe && e === void 0 ? Kt : e, this
     }
-    le.prototype.clear = _a;
-    le.prototype.delete = Ca;
-    le.prototype.get = Fa;
-    le.prototype.has = Sa;
-    le.prototype.set = La;
+    le.prototype.clear = os;
+    le.prototype.delete = is;
+    le.prototype.get = as;
+    le.prototype.has = ss;
+    le.prototype.set = ls;
 
     function X(t) {
         var e = -1,
             r = t == null ? 0 : t.length;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function $a() {
+    function ds() {
         this.__data__ = [], this.size = 0
     }
 
-    function Ma(t) {
+    function cs(t) {
         var e = this.__data__,
-            r = st(e, t);
+            r = mt(e, t);
         if (r < 0) return !1;
         var n = e.length - 1;
-        return r == n ? e.pop() : ya.call(e, r, 1), --this.size, !0
+        return r == n ? e.pop() : Xa.call(e, r, 1), --this.size, !0
     }
 
-    function Ia(t) {
+    function us(t) {
         var e = this.__data__,
-            r = st(e, t);
+            r = mt(e, t);
         return r < 0 ? void 0 : e[r][1]
     }
 
-    function Pa(t) {
-        return st(this.__data__, t) > -1
+    function fs(t) {
+        return mt(this.__data__, t) > -1
     }
 
-    function Da(t, e) {
+    function ps(t, e) {
         var r = this.__data__,
-            n = st(r, t);
+            n = mt(r, t);
         return n < 0 ? (++this.size, r.push([t, e])) : r[n][1] = e, this
     }
-    X.prototype.clear = $a;
-    X.prototype.delete = Ma;
-    X.prototype.get = Ia;
-    X.prototype.has = Pa;
-    X.prototype.set = Da;
+    X.prototype.clear = ds;
+    X.prototype.delete = cs;
+    X.prototype.get = us;
+    X.prototype.has = fs;
+    X.prototype.set = ps;
 
     function de(t) {
         var e = -1,
             r = t == null ? 0 : t.length;
         for (this.clear(); ++e < r;) {
             var n = t[e];
             this.set(n[0], n[1])
         }
     }
 
-    function Oa() {
+    function ms() {
         this.size = 0, this.__data__ = {
             hash: new le,
-            map: new(Le || X),
+            map: new(Pe || X),
             string: new le
         }
     }
 
-    function Ha(t) {
-        var e = lt(this, t).delete(t);
+    function hs(t) {
+        var e = ht(this, t).delete(t);
         return this.size -= e ? 1 : 0, e
     }
 
-    function Ra(t) {
-        return lt(this, t).get(t)
+    function gs(t) {
+        return ht(this, t).get(t)
     }
 
-    function Ba(t) {
-        return lt(this, t).has(t)
+    function bs(t) {
+        return ht(this, t).has(t)
     }
 
-    function Na(t, e) {
-        var r = lt(this, t),
+    function ys(t, e) {
+        var r = ht(this, t),
             n = r.size;
         return r.set(t, e), this.size += r.size == n ? 0 : 1, this
     }
-    de.prototype.clear = Oa;
-    de.prototype.delete = Ha;
-    de.prototype.get = Ra;
-    de.prototype.has = Ba;
-    de.prototype.set = Na;
+    de.prototype.clear = ms;
+    de.prototype.delete = hs;
+    de.prototype.get = gs;
+    de.prototype.has = bs;
+    de.prototype.set = ys;
 
-    function nt(t) {
+    function ct(t) {
         var e = -1,
             r = t == null ? 0 : t.length;
         for (this.__data__ = new de; ++e < r;) this.add(t[e])
     }
 
-    function Va(t) {
-        return this.__data__.set(t, Rt), this
+    function vs(t) {
+        return this.__data__.set(t, Kt), this
     }
 
-    function Ga(t) {
+    function js(t) {
         return this.__data__.has(t)
     }
-    nt.prototype.add = nt.prototype.push = Va;
-    nt.prototype.has = Ga;
+    ct.prototype.add = ct.prototype.push = vs;
+    ct.prototype.has = js;
 
     function re(t) {
         var e = this.__data__ = new X(t);
         this.size = e.size
     }
 
-    function qa() {
+    function xs() {
         this.__data__ = new X, this.size = 0
     }
 
-    function za(t) {
+    function Es(t) {
         var e = this.__data__,
             r = e.delete(t);
         return this.size = e.size, r
     }
 
-    function Ua(t) {
+    function ws(t) {
         return this.__data__.get(t)
     }
 
-    function Ka(t) {
+    function ks(t) {
         return this.__data__.has(t)
     }
 
-    function Ja(t, e) {
+    function As(t, e) {
         var r = this.__data__;
         if (r instanceof X) {
             var n = r.__data__;
-            if (!Le || n.length < Bi - 1) return n.push([t, e]), this.size = ++r.size, this;
+            if (!Pe || n.length < ba - 1) return n.push([t, e]), this.size = ++r.size, this;
             r = this.__data__ = new de(n)
         }
         return r.set(t, e), this.size = r.size, this
     }
-    re.prototype.clear = qa;
-    re.prototype.delete = za;
-    re.prototype.get = Ua;
-    re.prototype.has = Ka;
-    re.prototype.set = Ja;
-
-    function Wa(t, e) {
-        var r = ot(t),
-            n = !r && cs(t),
-            i = !r && !n && Ht(t),
-            o = !r && !n && !i && vn(t),
+    re.prototype.clear = xs;
+    re.prototype.delete = Es;
+    re.prototype.get = ws;
+    re.prototype.has = ks;
+    re.prototype.set = As;
+
+    function Ts(t, e) {
+        var r = ut(t),
+            n = !r && Ns(t),
+            i = !r && !n && Ut(t),
+            o = !r && !n && !i && Pn(t),
             s = r || n || i || o,
-            u = s ? da(t.length, String) : [],
-            f = u.length;
-        for (var d in t)(e || K.call(t, d)) && !(s && (d == "length" || i && (d == "offset" || d == "parent") || o && (d == "buffer" || d == "byteLength" || d == "byteOffset") || is(d, f))) && u.push(d);
-        return u
+            d = s ? Ba(t.length, String) : [],
+            f = d.length;
+        for (var c in t)(e || K.call(t, c)) && !(s && (c == "length" || i && (c == "offset" || c == "parent") || o && (c == "buffer" || c == "byteLength" || c == "byteOffset") || Os(c, f))) && d.push(c);
+        return d
     }
 
-    function st(t, e) {
+    function mt(t, e) {
         for (var r = t.length; r--;)
-            if (mn(t[r][0], e)) return r;
+            if (Ln(t[r][0], e)) return r;
         return -1
     }
 
-    function Xa(t, e, r) {
+    function Cs(t, e, r) {
         var n = e(t);
-        return ot(t) ? n : sa(n, r(t))
+        return ut(t) ? n : Ra(n, r(t))
     }
 
-    function Ie(t) {
-        return t == null ? t === void 0 ? Ui : Gi : se && se in Object(t) ? ns(t) : ds(t)
+    function Re(t) {
+        return t == null ? t === void 0 ? wa : ja : se && se in Object(t) ? Is(t) : Bs(t)
     }
 
-    function Kr(t) {
-        return Me(t) && Ie(t) == Ye
+    function un(t) {
+        return De(t) && Re(t) == it
     }
 
-    function fn(t, e, r, n, i) {
-        return t === e ? !0 : t == null || e == null || !Me(t) && !Me(e) ? t !== t && e !== e : Za(t, e, r, n, fn, i)
+    function Fn(t, e, r, n, i) {
+        return t === e ? !0 : t == null || e == null || !De(t) && !De(e) ? t !== t && e !== e : _s(t, e, r, n, Fn, i)
     }
 
-    function Za(t, e, r, n, i, o) {
-        var s = ot(t),
-            u = ot(e),
-            f = s ? $t : te(t),
-            d = u ? $t : te(e);
-        f = f == Ye ? he : f, d = d == Ye ? he : d;
-        var h = f == he,
-            v = d == he,
-            A = f == d;
-        if (A && Ht(t)) {
-            if (!Ht(e)) return !1;
-            s = !0, h = !1
+    function _s(t, e, r, n, i, o) {
+        var s = ut(t),
+            d = ut(e),
+            f = s ? Bt : te(t),
+            c = d ? Bt : te(e);
+        f = f == it ? je : f, c = c == it ? je : c;
+        var g = f == je,
+            y = c == je,
+            A = f == c;
+        if (A && Ut(t)) {
+            if (!Ut(e)) return !1;
+            s = !0, g = !1
         }
-        if (A && !h) return o || (o = new re), s || vn(t) ? pn(t, e, r, n, i, o) : ts(t, e, f, r, n, i, o);
-        if (!(r & it)) {
-            var L = h && K.call(t, "__wrapped__"),
-                I = v && K.call(e, "__wrapped__");
+        if (A && !g) return o || (o = new re), s || Pn(t) ? Sn(t, e, r, n, i, o) : $s(t, e, f, r, n, i, o);
+        if (!(r & ft)) {
+            var L = g && K.call(t, "__wrapped__"),
+                I = y && K.call(e, "__wrapped__");
             if (L || I) {
                 var B = L ? t.value() : t,
                     N = I ? e.value() : e;
                 return o || (o = new re), i(B, N, r, n, o)
             }
         }
-        return A ? (o || (o = new re), rs(t, e, r, n, i, o)) : !1
+        return A ? (o || (o = new re), Ms(t, e, r, n, i, o)) : !1
     }
 
-    function Ya(t) {
-        if (!bn(t) || ss(t)) return !1;
-        var e = gn(t) ? va : na;
+    function Fs(t) {
+        if (!In(t) || Rs(t)) return !1;
+        var e = $n(t) ? Wa : Ia;
         return e.test(ce(t))
     }
 
-    function Qa(t) {
-        return Me(t) && hn(t.length) && !!S[Ie(t)]
+    function Ss(t) {
+        return De(t) && Mn(t.length) && !!S[Re(t)]
     }
 
-    function es(t) {
-        if (!ls(t)) return xa(t);
+    function Ls(t) {
+        if (!Hs(t)) return Ya(t);
         var e = [];
         for (var r in Object(t)) K.call(t, r) && r != "constructor" && e.push(r);
         return e
     }
 
-    function pn(t, e, r, n, i, o) {
-        var s = r & it,
-            u = t.length,
+    function Sn(t, e, r, n, i, o) {
+        var s = r & ft,
+            d = t.length,
             f = e.length;
-        if (u != f && !(s && f > u)) return !1;
-        var d = o.get(t);
-        if (d && o.get(e)) return d == e;
-        var h = -1,
-            v = !0,
-            A = r & Wr ? new nt : void 0;
-        for (o.set(t, e), o.set(e, t); ++h < u;) {
-            var L = t[h],
-                I = e[h];
-            if (n) var B = s ? n(I, L, h, e, t, o) : n(L, I, h, t, e, o);
+        if (d != f && !(s && f > d)) return !1;
+        var c = o.get(t);
+        if (c && o.get(e)) return c == e;
+        var g = -1,
+            y = !0,
+            A = r & pn ? new ct : void 0;
+        for (o.set(t, e), o.set(e, t); ++g < d;) {
+            var L = t[g],
+                I = e[g];
+            if (n) var B = s ? n(I, L, g, e, t, o) : n(L, I, g, t, e, o);
             if (B !== void 0) {
                 if (B) continue;
-                v = !1;
+                y = !1;
                 break
             }
             if (A) {
-                if (!la(e, function(N, q) {
-                        if (!ua(A, q) && (L === N || i(L, N, r, n, o))) return A.push(q)
+                if (!Ha(e, function(N, G) {
+                        if (!qa(A, G) && (L === N || i(L, N, r, n, o))) return A.push(G)
                     })) {
-                    v = !1;
+                    y = !1;
                     break
                 }
             } else if (!(L === I || i(L, I, r, n, o))) {
-                v = !1;
+                y = !1;
                 break
             }
         }
-        return o.delete(t), o.delete(e), v
+        return o.delete(t), o.delete(e), y
     }
 
-    function ts(t, e, r, n, i, o, s) {
+    function $s(t, e, r, n, i, o, s) {
         switch (r) {
-            case tt:
+            case lt:
                 if (t.byteLength != e.byteLength || t.byteOffset != e.byteOffset) return !1;
                 t = t.buffer, e = e.buffer;
-            case on:
-                return !(t.byteLength != e.byteLength || !o(new qr(t), new qr(e)));
-            case Zr:
-            case Yr:
-            case tn:
-                return mn(+t, +e);
-            case Qr:
+            case En:
+                return !(t.byteLength != e.byteLength || !o(new ln(t), new ln(e)));
+            case hn:
+            case gn:
+            case vn:
+                return Ln(+t, +e);
+            case bn:
                 return t.name == e.name && t.message == e.message;
-            case rn:
-            case nn:
+            case jn:
+            case xn:
                 return t == e + "";
-            case Qe:
-                var u = pa;
-            case et:
-                var f = n & it;
-                if (u || (u = ga), t.size != e.size && !f) return !1;
-                var d = s.get(t);
-                if (d) return d == e;
-                n |= Wr, s.set(t, e);
-                var h = pn(u(t), u(e), n, i, o, s);
-                return s.delete(t), h;
-            case zi:
-                if (Lt) return Lt.call(t) == Lt.call(e)
+            case at:
+                var d = Ga;
+            case st:
+                var f = n & ft;
+                if (d || (d = Ua), t.size != e.size && !f) return !1;
+                var c = s.get(t);
+                if (c) return c == e;
+                n |= pn, s.set(t, e);
+                var g = Sn(d(t), d(e), n, i, o, s);
+                return s.delete(t), g;
+            case Ea:
+                if (Ht) return Ht.call(t) == Ht.call(e)
         }
         return !1
     }
 
-    function rs(t, e, r, n, i, o) {
-        var s = r & it,
-            u = Jr(t),
-            f = u.length,
-            d = Jr(e),
-            h = d.length;
-        if (f != h && !s) return !1;
-        for (var v = f; v--;) {
-            var A = u[v];
+    function Ms(t, e, r, n, i, o) {
+        var s = r & ft,
+            d = fn(t),
+            f = d.length,
+            c = fn(e),
+            g = c.length;
+        if (f != g && !s) return !1;
+        for (var y = f; y--;) {
+            var A = d[y];
             if (!(s ? A in e : K.call(e, A))) return !1
         }
         var L = o.get(t);
         if (L && o.get(e)) return L == e;
         var I = !0;
         o.set(t, e), o.set(e, t);
-        for (var B = s; ++v < f;) {
-            A = u[v];
+        for (var B = s; ++y < f;) {
+            A = d[y];
             var N = t[A],
-                q = e[A];
-            if (n) var O = s ? n(q, N, A, e, t, o) : n(N, q, A, t, e, o);
-            if (!(O === void 0 ? N === q || i(N, q, r, n, o) : O)) {
+                G = e[A];
+            if (n) var D = s ? n(G, N, A, e, t, o) : n(N, G, A, t, e, o);
+            if (!(D === void 0 ? N === G || i(N, G, r, n, o) : D)) {
                 I = !1;
                 break
             }
             B || (B = A == "constructor")
         }
         if (I && !B) {
             var b = t.constructor,
                 F = e.constructor;
             b != F && "constructor" in t && "constructor" in e && !(typeof b == "function" && b instanceof b && typeof F == "function" && F instanceof F) && (I = !1)
         }
         return o.delete(t), o.delete(e), I
     }
 
-    function Jr(t) {
-        return Xa(t, ps, os)
+    function fn(t) {
+        return Cs(t, Gs, Ps)
     }
 
-    function lt(t, e) {
+    function ht(t, e) {
         var r = t.__data__;
-        return as(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
+        return Ds(e) ? r[typeof e == "string" ? "string" : "hash"] : r.map
     }
 
-    function ve(t, e) {
-        var r = fa(t, e);
-        return Ya(r) ? r : void 0
+    function Ee(t, e) {
+        var r = Va(t, e);
+        return Fs(r) ? r : void 0
     }
 
-    function ns(t) {
+    function Is(t) {
         var e = K.call(t, se),
             r = t[se];
         try {
             t[se] = void 0;
             var n = !0
         } catch {}
-        var i = cn.call(t);
+        var i = Cn.call(t);
         return n && (e ? t[se] = r : delete t[se]), i
     }
-    var os = zr ? function(t) {
-            return t == null ? [] : (t = Object(t), aa(zr(t), function(e) {
-                return un.call(t, e)
+    var Ps = dn ? function(t) {
+            return t == null ? [] : (t = Object(t), Da(dn(t), function(e) {
+                return _n.call(t, e)
             }))
-        } : ms,
-        te = Ie;
-    (It && te(new It(new ArrayBuffer(1))) != tt || Le && te(new Le) != Qe || Pt && te(Pt.resolve()) != Hr || Dt && te(new Dt) != et || Ot && te(new Ot) != Mt) && (te = function(t) {
-        var e = Ie(t),
-            r = e == he ? t.constructor : void 0,
+        } : zs,
+        te = Re;
+    (qt && te(new qt(new ArrayBuffer(1))) != lt || Pe && te(new Pe) != at || Vt && te(Vt.resolve()) != tn || Gt && te(new Gt) != st || zt && te(new zt) != Nt) && (te = function(t) {
+        var e = Re(t),
+            r = e == je ? t.constructor : void 0,
             n = r ? ce(r) : "";
         if (n) switch (n) {
-            case Ea:
-                return tt;
-            case wa:
-                return Qe;
-            case ka:
-                return Hr;
-            case Aa:
-                return et;
-            case Ta:
-                return Mt
+            case Qa:
+                return lt;
+            case es:
+                return at;
+            case ts:
+                return tn;
+            case rs:
+                return st;
+            case ns:
+                return Nt
         }
         return e
     });
 
-    function is(t, e) {
-        return e = e ?? Xr, !!e && (typeof t == "number" || oa.test(t)) && t > -1 && t % 1 == 0 && t < e
+    function Os(t, e) {
+        return e = e ?? mn, !!e && (typeof t == "number" || Pa.test(t)) && t > -1 && t % 1 == 0 && t < e
     }
 
-    function as(t) {
+    function Ds(t) {
         var e = typeof t;
         return e == "string" || e == "number" || e == "symbol" || e == "boolean" ? t !== "__proto__" : t === null
     }
 
-    function ss(t) {
-        return !!Vr && Vr in t
+    function Rs(t) {
+        return !!an && an in t
     }
 
-    function ls(t) {
+    function Hs(t) {
         var e = t && t.constructor,
-            r = typeof e == "function" && e.prototype || at;
+            r = typeof e == "function" && e.prototype || pt;
         return t === r
     }
 
-    function ds(t) {
-        return cn.call(t)
+    function Bs(t) {
+        return Cn.call(t)
     }
 
     function ce(t) {
         if (t != null) {
             try {
-                return dn.call(t)
+                return Tn.call(t)
             } catch {}
             try {
                 return t + ""
             } catch {}
         }
         return ""
     }
 
-    function mn(t, e) {
+    function Ln(t, e) {
         return t === e || t !== t && e !== e
     }
-    var cs = Kr(function() {
+    var Ns = un(function() {
             return arguments
-        }()) ? Kr : function(t) {
-            return Me(t) && K.call(t, "callee") && !un.call(t, "callee")
+        }()) ? un : function(t) {
+            return De(t) && K.call(t, "callee") && !_n.call(t, "callee")
         },
-        ot = Array.isArray;
+        ut = Array.isArray;
 
-    function us(t) {
-        return t != null && hn(t.length) && !gn(t)
+    function qs(t) {
+        return t != null && Mn(t.length) && !$n(t)
     }
-    var Ht = ja || gs;
+    var Ut = Za || Us;
 
-    function fs(t, e) {
-        return fn(t, e)
+    function Vs(t, e) {
+        return Fn(t, e)
     }
 
-    function gn(t) {
-        if (!bn(t)) return !1;
-        var e = Ie(t);
-        return e == en || e == Vi || e == Ni || e == qi
+    function $n(t) {
+        if (!In(t)) return !1;
+        var e = Re(t);
+        return e == yn || e == va || e == ya || e == xa
     }
 
-    function hn(t) {
-        return typeof t == "number" && t > -1 && t % 1 == 0 && t <= Xr
+    function Mn(t) {
+        return typeof t == "number" && t > -1 && t % 1 == 0 && t <= mn
     }
 
-    function bn(t) {
+    function In(t) {
         var e = typeof t;
         return t != null && (e == "object" || e == "function")
     }
 
-    function Me(t) {
+    function De(t) {
         return t != null && typeof t == "object"
     }
-    var vn = Nr ? ca(Nr) : Qa;
+    var Pn = on ? Na(on) : Ss;
 
-    function ps(t) {
-        return us(t) ? Wa(t) : es(t)
+    function Gs(t) {
+        return qs(t) ? Ts(t) : Ls(t)
     }
 
-    function ms() {
+    function zs() {
         return []
     }
 
-    function gs() {
+    function Us() {
         return !1
     }
-    be.exports = fs
+    xe.exports = Vs
+});
+var Wn = Ye((He, we) => {
+    var Ks = 9007199254740991,
+        Js = "[object Arguments]",
+        Ws = "[object Function]",
+        Xs = "[object GeneratorFunction]",
+        Wt = "[object Map]",
+        Zs = "[object Object]",
+        Dn = "[object Promise]",
+        Xt = "[object Set]",
+        Rn = "[object WeakMap]",
+        Hn = "[object DataView]",
+        Ys = /[\\^$.*+?()[\]{}|]/g,
+        Qs = /^\[object .+?Constructor\]$/,
+        el = typeof global == "object" && global && global.Object === Object && global,
+        tl = typeof self == "object" && self && self.Object === Object && self,
+        fe = el || tl || Function("return this")(),
+        Vn = typeof He == "object" && He && !He.nodeType && He,
+        Bn = Vn && typeof we == "object" && we && !we.nodeType && we,
+        rl = Bn && Bn.exports === Vn;
+
+    function nl(t, e) {
+        return t == null ? void 0 : t[e]
+    }
+
+    function ol(t) {
+        var e = !1;
+        if (t != null && typeof t.toString != "function") try {
+            e = !!(t + "")
+        } catch {}
+        return e
+    }
+
+    function il(t, e) {
+        return function(r) {
+            return t(e(r))
+        }
+    }
+    var al = Function.prototype,
+        gt = Object.prototype,
+        Jt = fe["__core-js_shared__"],
+        Nn = function() {
+            var t = /[^.]+$/.exec(Jt && Jt.keys && Jt.keys.IE_PROTO || "");
+            return t ? "Symbol(src)_1." + t : ""
+        }(),
+        Gn = al.toString,
+        rr = gt.hasOwnProperty,
+        bt = gt.toString,
+        sl = RegExp("^" + Gn.call(rr).replace(Ys, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
+        qn = rl ? fe.Buffer : void 0,
+        zn = gt.propertyIsEnumerable,
+        ll = qn ? qn.isBuffer : void 0,
+        dl = il(Object.keys, Object),
+        Zt = Be(fe, "DataView"),
+        Yt = Be(fe, "Map"),
+        Qt = Be(fe, "Promise"),
+        er = Be(fe, "Set"),
+        tr = Be(fe, "WeakMap"),
+        cl = !zn.call({
+            valueOf: 1
+        }, "valueOf"),
+        ul = pe(Zt),
+        fl = pe(Yt),
+        pl = pe(Qt),
+        ml = pe(er),
+        hl = pe(tr);
+
+    function gl(t) {
+        return bt.call(t)
+    }
+
+    function bl(t) {
+        if (!Jn(t) || yl(t)) return !1;
+        var e = Kn(t) || ol(t) ? sl : Qs;
+        return e.test(pe(t))
+    }
+
+    function Be(t, e) {
+        var r = nl(t, e);
+        return bl(r) ? r : void 0
+    }
+    var ue = gl;
+    (Zt && ue(new Zt(new ArrayBuffer(1))) != Hn || Yt && ue(new Yt) != Wt || Qt && ue(Qt.resolve()) != Dn || er && ue(new er) != Xt || tr && ue(new tr) != Rn) && (ue = function(t) {
+        var e = bt.call(t),
+            r = e == Zs ? t.constructor : void 0,
+            n = r ? pe(r) : void 0;
+        if (n) switch (n) {
+            case ul:
+                return Hn;
+            case fl:
+                return Wt;
+            case pl:
+                return Dn;
+            case ml:
+                return Xt;
+            case hl:
+                return Rn
+        }
+        return e
+    });
+
+    function yl(t) {
+        return !!Nn && Nn in t
+    }
+
+    function vl(t) {
+        var e = t && t.constructor,
+            r = typeof e == "function" && e.prototype || gt;
+        return t === r
+    }
+
+    function pe(t) {
+        if (t != null) {
+            try {
+                return Gn.call(t)
+            } catch {}
+            try {
+                return t + ""
+            } catch {}
+        }
+        return ""
+    }
+
+    function jl(t) {
+        return El(t) && rr.call(t, "callee") && (!zn.call(t, "callee") || bt.call(t) == Js)
+    }
+    var xl = Array.isArray;
+
+    function Un(t) {
+        return t != null && Al(t.length) && !Kn(t)
+    }
+
+    function El(t) {
+        return Tl(t) && Un(t)
+    }
+    var wl = ll || Cl;
+
+    function kl(t) {
+        if (Un(t) && (xl(t) || typeof t == "string" || typeof t.splice == "function" || wl(t) || jl(t))) return !t.length;
+        var e = ue(t);
+        if (e == Wt || e == Xt) return !t.size;
+        if (cl || vl(t)) return !dl(t).length;
+        for (var r in t)
+            if (rr.call(t, r)) return !1;
+        return !0
+    }
+
+    function Kn(t) {
+        var e = Jn(t) ? bt.call(t) : "";
+        return e == Ws || e == Xs
+    }
+
+    function Al(t) {
+        return typeof t == "number" && t > -1 && t % 1 == 0 && t <= Ks
+    }
+
+    function Jn(t) {
+        var e = typeof t;
+        return !!t && (e == "object" || e == "function")
+    }
+
+    function Tl(t) {
+        return !!t && typeof t == "object"
+    }
+
+    function Cl() {
+        return !1
+    }
+    we.exports = kl
 });
 (function() {
     "use strict";
-    var t = function(m, c) {
-        var g = function(T) {
+    var t = function(m, u) {
+        var h = function(T) {
                 for (var w = 0, $ = T.length; w < $; w++) j(T[w])
             },
             j = function(T) {
                 var w = T.target,
                     $ = T.attributeName,
                     P = T.oldValue;
                 w.attributeChangedCallback($, P, w.getAttribute($))
             };
         return function(x, T) {
             var w = x.constructor.observedAttributes;
             return w && m(T).then(function() {
-                new c(g).observe(x, {
+                new u(h).observe(x, {
                     attributes: !0,
                     attributeOldValue: !0,
                     attributeFilter: w
                 });
                 for (var $ = 0, P = w.length; $ < P; $++) x.hasAttribute(w[$]) && j({
                     target: x,
                     attributeName: w[$],
                     oldValue: null
                 })
             }), x
         }
     };
 
-    function e(m, c) {
+    function e(m, u) {
         if (m) {
-            if (typeof m == "string") return r(m, c);
-            var g = Object.prototype.toString.call(m).slice(8, -1);
-            if (g === "Object" && m.constructor && (g = m.constructor.name), g === "Map" || g === "Set") return Array.from(m);
-            if (g === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(g)) return r(m, c)
+            if (typeof m == "string") return r(m, u);
+            var h = Object.prototype.toString.call(m).slice(8, -1);
+            if (h === "Object" && m.constructor && (h = m.constructor.name), h === "Map" || h === "Set") return Array.from(m);
+            if (h === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(h)) return r(m, u)
         }
     }
 
-    function r(m, c) {
-        (c == null || c > m.length) && (c = m.length);
-        for (var g = 0, j = new Array(c); g < c; g++) j[g] = m[g];
+    function r(m, u) {
+        (u == null || u > m.length) && (u = m.length);
+        for (var h = 0, j = new Array(u); h < u; h++) j[h] = m[h];
         return j
     }
 
-    function n(m, c) {
-        var g = typeof Symbol < "u" && m[Symbol.iterator] || m["@@iterator"];
-        if (!g) {
-            if (Array.isArray(m) || (g = e(m)) || c && m && typeof m.length == "number") {
-                g && (m = g);
+    function n(m, u) {
+        var h = typeof Symbol < "u" && m[Symbol.iterator] || m["@@iterator"];
+        if (!h) {
+            if (Array.isArray(m) || (h = e(m)) || u && m && typeof m.length == "number") {
+                h && (m = h);
                 var j = 0,
                     x = function() {};
                 return {
                     s: x,
                     n: function() {
                         return j >= m.length ? {
                             done: !0
@@ -1335,378 +1504,379 @@
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
         }
         var T = !0,
             w = !1,
             $;
         return {
             s: function() {
-                g = g.call(m)
+                h = h.call(m)
             },
             n: function() {
-                var P = g.next();
+                var P = h.next();
                 return T = P.done, P
             },
             e: function(P) {
                 w = !0, $ = P
             },
             f: function() {
                 try {
-                    !T && g.return != null && g.return()
+                    !T && h.return != null && h.return()
                 } finally {
                     if (w) throw $
                 }
             }
         }
     }
     var i = !0,
         o = !1,
         s = "querySelectorAll",
-        u = function(c) {
-            var g = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : document,
+        d = function(u) {
+            var h = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : document,
                 j = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : MutationObserver,
                 x = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : ["*"],
-                T = function P(Q, ee, R, k, M, D) {
-                    var G = n(Q),
-                        pe;
+                T = function P(Q, ee, H, k, M, O) {
+                    var V = n(Q),
+                        ge;
                     try {
-                        for (G.s(); !(pe = G.n()).done;) {
-                            var H = pe.value;
-                            (D || s in H) && (M ? R.has(H) || (R.add(H), k.delete(H), c(H, M)) : k.has(H) || (k.add(H), R.delete(H), c(H, M)), D || P(H[s](ee), ee, R, k, M, i))
+                        for (V.s(); !(ge = V.n()).done;) {
+                            var R = ge.value;
+                            (O || s in R) && (M ? H.has(R) || (H.add(R), k.delete(R), u(R, M)) : k.has(R) || (k.add(R), H.delete(R), u(R, M)), O || P(R[s](ee), ee, H, k, M, i))
                         }
-                    } catch (vt) {
-                        G.e(vt)
+                    } catch (Ct) {
+                        V.e(Ct)
                     } finally {
-                        G.f()
+                        V.f()
                     }
                 },
                 w = new j(function(P) {
                     if (x.length) {
                         var Q = x.join(","),
                             ee = new Set,
-                            R = new Set,
+                            H = new Set,
                             k = n(P),
                             M;
                         try {
                             for (k.s(); !(M = k.n()).done;) {
-                                var D = M.value,
-                                    G = D.addedNodes,
-                                    pe = D.removedNodes;
-                                T(pe, Q, ee, R, o, o), T(G, Q, ee, R, i, o)
+                                var O = M.value,
+                                    V = O.addedNodes,
+                                    ge = O.removedNodes;
+                                T(ge, Q, ee, H, o, o), T(V, Q, ee, H, i, o)
                             }
-                        } catch (H) {
-                            k.e(H)
+                        } catch (R) {
+                            k.e(R)
                         } finally {
                             k.f()
                         }
                     }
                 }),
                 $ = w.observe;
             return (w.observe = function(P) {
                 return $.call(w, P, {
                     subtree: i,
                     childList: i
                 })
-            })(g), w
+            })(h), w
         },
         f = "querySelectorAll",
-        d = self,
-        h = d.document,
-        v = d.Element,
-        A = d.MutationObserver,
-        L = d.Set,
-        I = d.WeakMap,
-        B = function(c) {
-            return f in c
+        c = self,
+        g = c.document,
+        y = c.Element,
+        A = c.MutationObserver,
+        L = c.Set,
+        I = c.WeakMap,
+        B = function(u) {
+            return f in u
         },
         N = [].filter,
-        q = function(m) {
-            var c = new I,
-                g = function(k) {
-                    for (var M = 0, D = k.length; M < D; M++) c.delete(k[M])
+        G = function(m) {
+            var u = new I,
+                h = function(k) {
+                    for (var M = 0, O = k.length; M < O; M++) u.delete(k[M])
                 },
                 j = function() {
-                    for (var k = Q.takeRecords(), M = 0, D = k.length; M < D; M++) w(N.call(k[M].removedNodes, B), !1), w(N.call(k[M].addedNodes, B), !0)
+                    for (var k = Q.takeRecords(), M = 0, O = k.length; M < O; M++) w(N.call(k[M].removedNodes, B), !1), w(N.call(k[M].addedNodes, B), !0)
                 },
                 x = function(k) {
                     return k.matches || k.webkitMatchesSelector || k.msMatchesSelector
                 },
                 T = function(k, M) {
-                    var D;
+                    var O;
                     if (M)
-                        for (var G, pe = x(k), H = 0, vt = $.length; H < vt; H++) pe.call(k, G = $[H]) && (c.has(k) || c.set(k, new L), D = c.get(k), D.has(G) || (D.add(G), m.handle(k, M, G)));
-                    else c.has(k) && (D = c.get(k), c.delete(k), D.forEach(function(Gn) {
-                        m.handle(k, M, Gn)
+                        for (var V, ge = x(k), R = 0, Ct = $.length; R < Ct; R++) ge.call(k, V = $[R]) && (u.has(k) || u.set(k, new L), O = u.get(k), O.has(V) || (O.add(V), m.handle(k, M, V)));
+                    else u.has(k) && (O = u.get(k), u.delete(k), O.forEach(function(xo) {
+                        m.handle(k, M, xo)
                     }))
                 },
                 w = function(k) {
-                    for (var M = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0, D = 0, G = k.length; D < G; D++) T(k[D], M)
+                    for (var M = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0, O = 0, V = k.length; O < V; O++) T(k[O], M)
                 },
                 $ = m.query,
-                P = m.root || h,
-                Q = u(T, P, A, $),
-                ee = v.prototype.attachShadow;
-            return ee && (v.prototype.attachShadow = function(R) {
-                var k = ee.call(this, R);
+                P = m.root || g,
+                Q = d(T, P, A, $),
+                ee = y.prototype.attachShadow;
+            return ee && (y.prototype.attachShadow = function(H) {
+                var k = ee.call(this, H);
                 return Q.observe(k), k
             }), $.length && w(P[f]($)), {
-                drop: g,
+                drop: h,
                 flush: j,
                 observer: Q,
                 parse: w
             }
         },
-        O = self,
-        b = O.document,
-        F = O.Map,
-        ft = O.MutationObserver,
-        ue = O.Object,
-        fe = O.Set,
-        Pe = O.WeakMap,
-        Y = O.Element,
-        De = O.HTMLElement,
-        Oe = O.Node,
-        we = O.Error,
-        y = O.TypeError,
-        He = O.Reflect,
-        p = ue.defineProperty,
-        l = ue.keys,
-        a = ue.getOwnPropertyNames,
-        C = ue.setPrototypeOf,
-        _ = !self.customElements,
-        V = function(c) {
-            for (var g = l(c), j = [], x = g.length, T = 0; T < x; T++) j[T] = c[g[T]], delete c[g[T]];
+        D = self,
+        b = D.document,
+        F = D.Map,
+        xt = D.MutationObserver,
+        me = D.Object,
+        he = D.Set,
+        Ne = D.WeakMap,
+        Y = D.Element,
+        qe = D.HTMLElement,
+        Ve = D.Node,
+        _e = D.Error,
+        v = D.TypeError,
+        Ge = D.Reflect,
+        p = me.defineProperty,
+        l = me.keys,
+        a = me.getOwnPropertyNames,
+        _ = me.setPrototypeOf,
+        C = !self.customElements,
+        q = function(u) {
+            for (var h = l(u), j = [], x = h.length, T = 0; T < x; T++) j[T] = u[h[T]], delete u[h[T]];
             return function() {
-                for (var w = 0; w < x; w++) c[g[w]] = j[w]
+                for (var w = 0; w < x; w++) u[h[w]] = j[w]
             }
         };
-    if (_) {
+    if (C) {
         var E = function() {
-                var c = this.constructor;
-                if (!Ae.has(c)) throw new y("Illegal constructor");
-                var g = Ae.get(c);
-                if (Be) return Xt(Be, g);
-                var j = ke.call(b, g);
-                return Xt(C(j, c.prototype), g)
+                var u = this.constructor;
+                if (!Se.has(u)) throw new v("Illegal constructor");
+                var h = Se.get(u);
+                if (Ue) return pr(Ue, h);
+                var j = Fe.call(b, h);
+                return pr(_(j, u.prototype), h)
             },
-            ke = b.createElement,
-            Ae = new F,
-            Re = new F,
-            Jt = new F,
-            Te = new F,
-            Wt = [],
-            Fn = function(c, g, j) {
-                var x = Jt.get(j);
-                if (g && !x.isPrototypeOf(c)) {
-                    var T = V(c);
-                    Be = C(c, x);
+            Fe = b.createElement,
+            Se = new F,
+            ze = new F,
+            ur = new F,
+            Le = new F,
+            fr = [],
+            ao = function(u, h, j) {
+                var x = ur.get(j);
+                if (h && !x.isPrototypeOf(u)) {
+                    var T = q(u);
+                    Ue = _(u, x);
                     try {
                         new x.constructor
                     } finally {
-                        Be = null, T()
+                        Ue = null, T()
                     }
                 }
-                var w = "".concat(g ? "" : "dis", "connectedCallback");
-                w in x && c[w]()
+                var w = "".concat(h ? "" : "dis", "connectedCallback");
+                w in x && u[w]()
             },
-            Sn = q({
-                query: Wt,
-                handle: Fn
+            so = G({
+                query: fr,
+                handle: ao
             }),
-            Ln = Sn.parse,
-            Be = null,
-            pt = function(c) {
-                if (!Re.has(c)) {
-                    var g, j = new Promise(function(x) {
-                        g = x
+            lo = so.parse,
+            Ue = null,
+            Et = function(u) {
+                if (!ze.has(u)) {
+                    var h, j = new Promise(function(x) {
+                        h = x
                     });
-                    Re.set(c, {
+                    ze.set(u, {
                         $: j,
-                        _: g
+                        _: h
                     })
                 }
-                return Re.get(c).$
+                return ze.get(u).$
             },
-            Xt = t(pt, ft);
+            pr = t(Et, xt);
         self.customElements = {
-            define: function(c, g) {
-                if (Te.has(c)) throw new we('the name "'.concat(c, '" has already been used with this registry'));
-                Ae.set(g, c), Jt.set(c, g.prototype), Te.set(c, g), Wt.push(c), pt(c).then(function() {
-                    Ln(b.querySelectorAll(c))
-                }), Re.get(c)._(g)
+            define: function(u, h) {
+                if (Le.has(u)) throw new _e('the name "'.concat(u, '" has already been used with this registry'));
+                Se.set(h, u), ur.set(u, h.prototype), Le.set(u, h), fr.push(u), Et(u).then(function() {
+                    lo(b.querySelectorAll(u))
+                }), ze.get(u)._(h)
             },
-            get: function(c) {
-                return Te.get(c)
+            get: function(u) {
+                return Le.get(u)
             },
-            whenDefined: pt
-        }, p(E.prototype = De.prototype, "constructor", {
+            whenDefined: Et
+        }, p(E.prototype = qe.prototype, "constructor", {
             value: E
-        }), self.HTMLElement = E, b.createElement = function(m, c) {
-            var g = c && c.is,
-                j = g ? Te.get(g) : Te.get(m);
-            return j ? new j : ke.call(b, m)
-        }, "isConnected" in Oe.prototype || p(Oe.prototype, "isConnected", {
+        }), self.HTMLElement = E, b.createElement = function(m, u) {
+            var h = u && u.is,
+                j = h ? Le.get(h) : Le.get(m);
+            return j ? new j : Fe.call(b, m)
+        }, "isConnected" in Ve.prototype || p(Ve.prototype, "isConnected", {
             configurable: !0,
             get: function() {
                 return !(this.ownerDocument.compareDocumentPosition(this) & this.DOCUMENT_POSITION_DISCONNECTED)
             }
         })
-    } else if (_ = !self.customElements.get("extends-li"), _) try {
-        var Zt = function m() {
+    } else if (C = !self.customElements.get("extends-li"), C) try {
+        var mr = function m() {
             return self.Reflect.construct(HTMLLIElement, [], m)
         };
-        Zt.prototype = HTMLLIElement.prototype;
-        var Yt = "extends-li";
-        self.customElements.define("extends-li", Zt, {
+        mr.prototype = HTMLLIElement.prototype;
+        var hr = "extends-li";
+        self.customElements.define("extends-li", mr, {
             extends: "li"
-        }), _ = b.createElement("li", {
-            is: Yt
-        }).outerHTML.indexOf(Yt) < 0;
-        var Qt = self.customElements,
-            $n = Qt.get,
-            Mn = Qt.whenDefined;
+        }), C = b.createElement("li", {
+            is: hr
+        }).outerHTML.indexOf(hr) < 0;
+        var gr = self.customElements,
+            co = gr.get,
+            uo = gr.whenDefined;
         self.customElements.whenDefined = function(m) {
-            var c = this;
-            return Mn.call(this, m).then(function(g) {
-                return g || $n.call(c, m)
+            var u = this;
+            return uo.call(this, m).then(function(h) {
+                return h || co.call(u, m)
             })
         }
     } catch {}
-    if (_) {
-        var er = function(c) {
-                var g = mt.get(c);
-                ir(g.querySelectorAll(this), c.isConnected)
+    if (C) {
+        var br = function(u) {
+                var h = wt.get(u);
+                Er(h.querySelectorAll(this), u.isConnected)
             },
             U = self.customElements,
-            tr = b.createElement,
-            In = U.define,
-            Pn = U.get,
-            Dn = U.upgrade,
-            On = He || {
-                construct: function(c) {
-                    return c.call(this)
+            yr = b.createElement,
+            fo = U.define,
+            po = U.get,
+            mo = U.upgrade,
+            ho = Ge || {
+                construct: function(u) {
+                    return u.call(this)
                 }
             },
-            Hn = On.construct,
-            mt = new Pe,
-            gt = new fe,
-            Ne = new F,
-            Ve = new F,
-            rr = new F,
-            Ge = new F,
-            nr = [],
-            qe = [],
-            or = function(c) {
-                return Ge.get(c) || Pn.call(U, c)
+            go = ho.construct,
+            wt = new Ne,
+            kt = new he,
+            Ke = new F,
+            Je = new F,
+            vr = new F,
+            We = new F,
+            jr = [],
+            Xe = [],
+            xr = function(u) {
+                return We.get(u) || po.call(U, u)
             },
-            Rn = function(c, g, j) {
-                var x = rr.get(j);
-                if (g && !x.isPrototypeOf(c)) {
-                    var T = V(c);
-                    ze = C(c, x);
+            bo = function(u, h, j) {
+                var x = vr.get(j);
+                if (h && !x.isPrototypeOf(u)) {
+                    var T = q(u);
+                    Ze = _(u, x);
                     try {
                         new x.constructor
                     } finally {
-                        ze = null, T()
+                        Ze = null, T()
                     }
                 }
-                var w = "".concat(g ? "" : "dis", "connectedCallback");
-                w in x && c[w]()
+                var w = "".concat(h ? "" : "dis", "connectedCallback");
+                w in x && u[w]()
             },
-            Bn = q({
-                query: qe,
-                handle: Rn
+            yo = G({
+                query: Xe,
+                handle: bo
             }),
-            ir = Bn.parse,
-            Nn = q({
-                query: nr,
-                handle: function(c, g) {
-                    mt.has(c) && (g ? gt.add(c) : gt.delete(c), qe.length && er.call(qe, c))
+            Er = yo.parse,
+            vo = G({
+                query: jr,
+                handle: function(u, h) {
+                    wt.has(u) && (h ? kt.add(u) : kt.delete(u), Xe.length && br.call(Xe, u))
                 }
             }),
-            Vn = Nn.parse,
-            ar = Y.prototype.attachShadow;
-        ar && (Y.prototype.attachShadow = function(m) {
-            var c = ar.call(this, m);
-            return mt.set(this, c), c
+            jo = vo.parse,
+            wr = Y.prototype.attachShadow;
+        wr && (Y.prototype.attachShadow = function(m) {
+            var u = wr.call(this, m);
+            return wt.set(this, u), u
         });
-        var ht = function(c) {
-                if (!Ve.has(c)) {
-                    var g, j = new Promise(function(x) {
-                        g = x
+        var At = function(u) {
+                if (!Je.has(u)) {
+                    var h, j = new Promise(function(x) {
+                        h = x
                     });
-                    Ve.set(c, {
+                    Je.set(u, {
                         $: j,
-                        _: g
+                        _: h
                     })
                 }
-                return Ve.get(c).$
+                return Je.get(u).$
             },
-            bt = t(ht, ft),
-            ze = null;
+            Tt = t(At, xt),
+            Ze = null;
         a(self).filter(function(m) {
             return /^HTML.*Element$/.test(m)
         }).forEach(function(m) {
-            var c = self[m];
+            var u = self[m];
 
-            function g() {
+            function h() {
                 var j = this.constructor;
-                if (!Ne.has(j)) throw new y("Illegal constructor");
-                var x = Ne.get(j),
+                if (!Ke.has(j)) throw new v("Illegal constructor");
+                var x = Ke.get(j),
                     T = x.is,
                     w = x.tag;
                 if (T) {
-                    if (ze) return bt(ze, T);
-                    var $ = tr.call(b, w);
-                    return $.setAttribute("is", T), bt(C($, j.prototype), T)
-                } else return Hn.call(this, c, [], j)
+                    if (Ze) return Tt(Ze, T);
+                    var $ = yr.call(b, w);
+                    return $.setAttribute("is", T), Tt(_($, j.prototype), T)
+                } else return go.call(this, u, [], j)
             }
-            p(g.prototype = c.prototype, "constructor", {
-                value: g
+            p(h.prototype = u.prototype, "constructor", {
+                value: h
             }), p(self, m, {
-                value: g
+                value: h
             })
-        }), b.createElement = function(m, c) {
-            var g = c && c.is;
-            if (g) {
-                var j = Ge.get(g);
-                if (j && Ne.get(j).tag === m) return new j
-            }
-            var x = tr.call(b, m);
-            return g && x.setAttribute("is", g), x
-        }, U.get = or, U.whenDefined = ht, U.upgrade = function(m) {
-            var c = m.getAttribute("is");
-            if (c) {
-                var g = Ge.get(c);
-                if (g) {
-                    bt(C(m, g.prototype), c);
+        }), b.createElement = function(m, u) {
+            var h = u && u.is;
+            if (h) {
+                var j = We.get(h);
+                if (j && Ke.get(j).tag === m) return new j
+            }
+            var x = yr.call(b, m);
+            return h && x.setAttribute("is", h), x
+        }, U.get = xr, U.whenDefined = At, U.upgrade = function(m) {
+            var u = m.getAttribute("is");
+            if (u) {
+                var h = We.get(u);
+                if (h) {
+                    Tt(_(m, h.prototype), u);
                     return
                 }
             }
-            Dn.call(U, m)
-        }, U.define = function(m, c, g) {
-            if (or(m)) throw new we("'".concat(m, "' has already been defined as a custom element"));
-            var j, x = g && g.extends;
-            Ne.set(c, x ? {
+            mo.call(U, m)
+        }, U.define = function(m, u, h) {
+            if (xr(m)) throw new _e("'".concat(m, "' has already been defined as a custom element"));
+            var j, x = h && h.extends;
+            Ke.set(u, x ? {
                 is: m,
                 tag: x
             } : {
                 is: "",
                 tag: m
-            }), x ? (j = "".concat(x, '[is="').concat(m, '"]'), rr.set(j, c.prototype), Ge.set(m, c), qe.push(j)) : (In.apply(U, arguments), nr.push(j = m)), ht(m).then(function() {
-                x ? (ir(b.querySelectorAll(j)), gt.forEach(er, [j])) : Vn(b.querySelectorAll(j))
-            }), Ve.get(m)._(c)
+            }), x ? (j = "".concat(x, '[is="').concat(m, '"]'), vr.set(j, u.prototype), We.set(m, u), Xe.push(j)) : (fo.apply(U, arguments), jr.push(j = m)), At(m).then(function() {
+                x ? (Er(b.querySelectorAll(j)), kt.forEach(br, [j])) : jo(b.querySelectorAll(j))
+            }), Je.get(m)._(u)
         }
     }
 })();
-var xe = _e(wr()),
-    An = _e(Or()),
-    Tn = _e(yn()),
-    _n = _e(sr());
-var jn = _e(sr()),
-    dt = class {
+var Te = be(Br()),
+    to = be(en()),
+    ro = be(On()),
+    no = be(Wn()),
+    oo = be(kr());
+var Xn = be(kr()),
+    yt = class {
         constructor(e, r) {
             this.progressBar = null;
             this.fileDrop = e => {
                 this.swallowEvent(e), e.dataTransfer && (this.fieldGroup.touch(), this.inputElement.files = e.dataTransfer.files, this.uploadFiles(this.inputElement.files).then(() => {
                     this.fieldGroup.inputted(), this.fieldGroup.validate()
                 }))
             };
@@ -1718,15 +1888,15 @@
                 e.stopPropagation(), e.preventDefault()
             };
             if (this.fieldGroup = e, this.inputElement = r, this.maxUploadSize = parseInt(this.inputElement.getAttribute("max-size") ?? "0"), this.dropbox = this.fieldGroup.element.querySelector("figure.dj-dropbox"), !this.dropbox) throw new Error('Element <input type="file"> requires sibling element <figure class="dj-dropbox"></figure>');
             if (this.chooseFileButton = this.fieldGroup.element.querySelector("button.dj-choose-file"), !this.chooseFileButton) throw new Error('Element <input type="file"> requires sibling element <button class="dj-choose-file"></button>');
             if (this.progressBar = this.fieldGroup.element.querySelector("progress"), this.progressBar && (this.progressBar.style.visibility = "hidden"), this.emptyDropboxItem = this.dropbox.querySelector("div.dj-empty-item"), !this.emptyDropboxItem) throw new Error('Element <input type="file"> requires sibling element <figure><div class="dj-empty-item"></div></figure>');
             let n = this.fieldGroup.element.querySelector(".dj-dropbox-items");
             if (!n) throw new Error('Element <input type="file"> requires sibling element <template class="dj-dropbox-items"></template>');
-            this.dropboxItemTemplate = (0, jn.default)(n.innerHTML), this.observer = new MutationObserver(o => this.attributesChanged(o)), this.observer.observe(this.inputElement, {
+            this.dropboxItemTemplate = (0, Xn.default)(n.innerHTML), this.observer = new MutationObserver(o => this.attributesChanged(o)), this.observer.observe(this.inputElement, {
                 attributes: !0
             }), this.chooseFileButton.disabled = r.disabled;
             let i = document.getElementById(`initial_${r.id}`);
             i != null && i.textContent ? (this.uploadedFiles = this.initialData = [JSON.parse(i.textContent)], this.renderDropbox()) : this.uploadedFiles = this.initialData = [], this.dropbox.addEventListener("dragenter", this.swallowEvent), this.dropbox.addEventListener("dragover", this.swallowEvent), this.dropbox.addEventListener("drop", this.fileDrop), this.chooseFileButton.addEventListener("click", () => {
                 r.click()
             }), r.addEventListener("change", () => this.uploadFiles(this.inputElement.files).then(() => {
                 this.fieldGroup.inputted(), this.fieldGroup.validate()
@@ -1746,26 +1916,26 @@
                 }) : n()
             })
         }
         async uploadFile(e, r) {
             let n = this;
 
             function i(s) {
-                let u = s.lengthComputable ? s.loaded / s.total : 0;
-                n.progressBar && (n.progressBar.style.visibility = "visible", n.progressBar.value = .97 * u)
+                let d = s.lengthComputable ? s.loaded / s.total : 0;
+                n.progressBar && (n.progressBar.style.visibility = "visible", n.progressBar.value = .97 * d)
             }
             let o = new FormData;
-            return o.append("temp_file", e), o.append("image_height", r.toString()), new Promise((s, u) => {
+            return o.append("temp_file", e), o.append("image_height", r.toString()), new Promise((s, d) => {
                 function f() {
-                    n.progressBar && (n.progressBar.value = 1, window.setTimeout(() => n.progressBar.style.visibility = "hidden", 333)), d.status === 200 ? s(d.response) : u(d.response)
+                    n.progressBar && (n.progressBar.value = 1, window.setTimeout(() => n.progressBar.style.visibility = "hidden", 333)), c.status === 200 ? s(c.response) : d(c.response)
                 }
-                let d = new XMLHttpRequest;
-                n.progressBar && (d.addEventListener("loadstart", i), d.upload.addEventListener("progress", i, !1)), d.addEventListener("loadend", f), d.open("POST", this.fieldGroup.form.formset.endpoint, !0);
-                let h = this.fieldGroup.form.formset.CSRFToken;
-                h && d.setRequestHeader("X-CSRFToken", h), d.responseType = "json", d.send(o)
+                let c = new XMLHttpRequest;
+                n.progressBar && (c.addEventListener("loadstart", i), c.upload.addEventListener("progress", i, !1)), c.addEventListener("loadend", f), c.open("POST", this.fieldGroup.form.formset.endpoint, !0);
+                let g = this.fieldGroup.form.formset.CSRFToken;
+                g && c.setRequestHeader("X-CSRFToken", g), c.responseType = "json", c.send(o)
             })
         }
         renderDropbox() {
             let e = [];
             for (let n of this.uploadedFiles) e.push(this.dropboxItemTemplate(n));
             e.length > 0 ? this.dropbox.innerHTML = e.join("") : this.dropbox.replaceChildren(this.emptyDropboxItem);
             let r = this.dropbox.querySelector(".dj-delete-file");
@@ -1780,113 +1950,113 @@
             return !!this.inputElement.files && this.inputElement.files.length > 0 && !this.uploadedFiles.length
         }
         resetToInitial() {
             this.uploadedFiles = this.initialData, this.renderDropbox()
         }
     };
 
-function Bt(t, e, r) {
+function nr(t, e, r) {
     return r = r || " ", t.length > e ? t : (e -= t.length, r += r.repeat(e), t + r.slice(0, e))
 }
 var Z = class extends Error {
     constructor(r, n, i, o) {
         super();
         this.message = r, this.expected = n, this.found = i, this.location = o, this.name = "SyntaxError", typeof Object.setPrototypeOf == "function" ? Object.setPrototypeOf(this, Z.prototype) : this.__proto__ = Z.prototype, typeof Error.captureStackTrace == "function" && Error.captureStackTrace(this, Z)
     }
     static buildMessage(r, n) {
-        function i(h) {
-            return h.charCodeAt(0).toString(16).toUpperCase()
+        function i(g) {
+            return g.charCodeAt(0).toString(16).toUpperCase()
         }
 
-        function o(h) {
-            return h.replace(/\\/g, "\\\\").replace(/"/g, '\\"').replace(/\0/g, "\\0").replace(/\t/g, "\\t").replace(/\n/g, "\\n").replace(/\r/g, "\\r").replace(/[\x00-\x0F]/g, v => "\\x0" + i(v)).replace(/[\x10-\x1F\x7F-\x9F]/g, v => "\\x" + i(v))
+        function o(g) {
+            return g.replace(/\\/g, "\\\\").replace(/"/g, '\\"').replace(/\0/g, "\\0").replace(/\t/g, "\\t").replace(/\n/g, "\\n").replace(/\r/g, "\\r").replace(/[\x00-\x0F]/g, y => "\\x0" + i(y)).replace(/[\x10-\x1F\x7F-\x9F]/g, y => "\\x" + i(y))
         }
 
-        function s(h) {
-            return h.replace(/\\/g, "\\\\").replace(/\]/g, "\\]").replace(/\^/g, "\\^").replace(/-/g, "\\-").replace(/\0/g, "\\0").replace(/\t/g, "\\t").replace(/\n/g, "\\n").replace(/\r/g, "\\r").replace(/[\x00-\x0F]/g, v => "\\x0" + i(v)).replace(/[\x10-\x1F\x7F-\x9F]/g, v => "\\x" + i(v))
+        function s(g) {
+            return g.replace(/\\/g, "\\\\").replace(/\]/g, "\\]").replace(/\^/g, "\\^").replace(/-/g, "\\-").replace(/\0/g, "\\0").replace(/\t/g, "\\t").replace(/\n/g, "\\n").replace(/\r/g, "\\r").replace(/[\x00-\x0F]/g, y => "\\x0" + i(y)).replace(/[\x10-\x1F\x7F-\x9F]/g, y => "\\x" + i(y))
         }
 
-        function u(h) {
-            switch (h.type) {
+        function d(g) {
+            switch (g.type) {
                 case "literal":
-                    return '"' + o(h.text) + '"';
+                    return '"' + o(g.text) + '"';
                 case "class":
-                    let v = h.parts.map(A => Array.isArray(A) ? s(A[0]) + "-" + s(A[1]) : s(A));
-                    return "[" + (h.inverted ? "^" : "") + v + "]";
+                    let y = g.parts.map(A => Array.isArray(A) ? s(A[0]) + "-" + s(A[1]) : s(A));
+                    return "[" + (g.inverted ? "^" : "") + y + "]";
                 case "any":
                     return "any character";
                 case "end":
                     return "end of input";
                 case "other":
-                    return h.description
+                    return g.description
             }
         }
 
-        function f(h) {
-            let v = h.map(u),
+        function f(g) {
+            let y = g.map(d),
                 A, L;
-            if (v.sort(), v.length > 0) {
-                for (A = 1, L = 1; A < v.length; A++) v[A - 1] !== v[A] && (v[L] = v[A], L++);
-                v.length = L
+            if (y.sort(), y.length > 0) {
+                for (A = 1, L = 1; A < y.length; A++) y[A - 1] !== y[A] && (y[L] = y[A], L++);
+                y.length = L
             }
-            switch (v.length) {
+            switch (y.length) {
                 case 1:
-                    return v[0];
+                    return y[0];
                 case 2:
-                    return v[0] + " or " + v[1];
+                    return y[0] + " or " + y[1];
                 default:
-                    return v.slice(0, -1).join(", ") + ", or " + v[v.length - 1]
+                    return y.slice(0, -1).join(", ") + ", or " + y[y.length - 1]
             }
         }
 
-        function d(h) {
-            return h ? '"' + o(h) + '"' : "end of input"
+        function c(g) {
+            return g ? '"' + o(g) + '"' : "end of input"
         }
-        return "Expected " + f(r) + " but " + d(n) + " found."
+        return "Expected " + f(r) + " but " + c(n) + " found."
     }
     format(r) {
         let n = "Error: " + this.message;
         if (this.location) {
             let i = null,
                 o;
             for (o = 0; o < r.length; o++)
                 if (r[o].source === this.location.source) {
                     i = r[o].text.split(/\r\n|\n|\r/g);
                     break
                 } let s = this.location.start,
-                u = this.location.source + ":" + s.line + ":" + s.column;
+                d = this.location.source + ":" + s.line + ":" + s.column;
             if (i) {
                 let f = this.location.end,
-                    d = Bt("", s.line.toString().length, " "),
-                    h = i[s.line - 1],
-                    v = s.line === f.line ? f.column : h.length + 1;
+                    c = nr("", s.line.toString().length, " "),
+                    g = i[s.line - 1],
+                    y = s.line === f.line ? f.column : g.length + 1;
                 n += `
- --> ` + u + `
-` + d + ` |
-` + s.line + " | " + h + `
-` + d + " | " + Bt("", s.column - 1, " ") + Bt("", v - s.column, "^")
+ --> ` + d + `
+` + c + ` |
+` + s.line + " | " + g + `
+` + c + " | " + nr("", s.column - 1, " ") + nr("", y - s.column, "^")
             } else n += `
- at ` + u
+ at ` + d
         }
         return n
     }
 };
 
-function hs(t, e) {
+function _l(t, e) {
     e = e !== void 0 ? e : {};
     let r = {},
         n = e.grammarSource,
         i = {
             Actions: 5,
             Expression: 0
         },
         o = 5,
         s = [function(p, l) {
-            return l.reduce(function(a, C) {
-                return a + C[1] + C[3]
+            return l.reduce(function(a, _) {
+                return a + _[1] + _[3]
             }, p)
         }, function() {
             return "false"
         }, "===", b("===", !1), "==", b("==", !1), "!==", b("!==", !1), "!=", b("!=", !1), "<=", b("<=", !1), ">=", b(">=", !1), "<", b("<", !1), ">", b(">", !1), "+", b("+", !1), "-", b("-", !1), "*", b("*", !1), "/", b("/", !1), "&&", b("&&", !1), "&", b("&", !1), "||", b("||", !1), "|", b("|", !1), "!", b("!", !1), "(", b("(", !1), ")", b(")", !1), function(p) {
             return "(" + p + ")"
         }, function(p) {
             return "'" + p + "'"
@@ -1919,16 +2089,16 @@
         }, ",", b(",", !1), function(p) {
             return [p]
         }, /^[ \t\n\r]/, F([" ", "	", `
 `, "\r"], !1, !1), "[", b("[", !1), "{", b("{", !1), "]", b("]", !1), "}", b("}", !1), ":", b(":", !1), function(p, l) {
             return l
         }, function(p, l) {
             var a = {};
-            return [p].concat(l).forEach(function(C) {
-                a[C.name] = C.value
+            return [p].concat(l).forEach(function(_) {
+                a[_.name] = _.value
             }), a
         }, function(p) {
             return p !== null ? p : {}
         }, function(p, l) {
             return {
                 name: p,
                 value: l
@@ -1940,39 +2110,39 @@
             ["a", "z"], "_"
         ], !1, !1), function(p, l) {
             return l
         }, function(p, l) {
             return [p].concat(l)
         }, function(p) {
             return p !== null ? p : []
-        }, fe("number"), function() {
+        }, he("number"), function() {
             return parseFloat(B())
         }, ".", b(".", !1), /^[1-9]/, F([
             ["1", "9"]
-        ], !1, !1), /^[eE]/, F(["e", "E"], !1, !1), "0", b("0", !1), fe("string"), '"', b('"', !1), function(p) {
+        ], !1, !1), /^[eE]/, F(["e", "E"], !1, !1), "0", b("0", !1), he("string"), '"', b('"', !1), function(p) {
             return p
         }, "'", b("'", !1), /^[^\0-\x1F"\\]/, F([
             ["\0", ""], '"', "\\"
         ], !0, !1), '\\"', b('\\"', !1), function() {
             return '"'
         }, /^[^\0-\x1F'\\]/, F([
             ["\0", ""], "'", "\\"
         ], !0, !1), "\\'", b("\\'", !1), function() {
             return "'"
         }, "\\\\", b("\\\\", !1), "\\b", b("\\b", !1), "\\f", b("\\f", !1), "\\n", b("\\n", !1), "\\r", b("\\r", !1), "\\t", b("\\t", !1), "\\u", b("\\u", !1), function(p) {
             return String.fromCharCode(parseInt(p, 16))
-        }, fe("boolean"), function() {
+        }, he("boolean"), function() {
             return !0
         }, function() {
             return !1
         }, function() {
             return null
         }, "false", b("false", !1), "true", b("true", !1), "null", b("null", !1), function(p, l) {
-            return l.reduce(function(a, C) {
-                return a + "." + C[1]
+            return l.reduce(function(a, _) {
+                return a + "." + _[1]
             }, p)
         }, "...", b("...", !1), "..", b("..", !1), function(p, l) {
             return p + l
         }, function(p, l) {
             return p + l
         }, /^[$a-zA-Z_]/, F(["$", ["a", "z"],
             ["A", "Z"], "_"
@@ -1983,44 +2153,44 @@
             return p instanceof Array ? p.join("") : p
         }, /^[0-9]/, F([
             ["0", "9"]
         ], !1, !1), /^[0-9a-f]/i, F([
             ["0", "9"],
             ["a", "f"]
         ], !1, !0)],
-        u = [y(`%;*/\x9E#;#/\x95$;*/\x8C$$%;*/>#;!/5$;*/,$; /#$+$)($'#(#'#("'#&'#0H*%;*/>#;!/5$;*/,$; /#$+$)($'#(#'#("'#&'#&/2$;*/)$8%: %"#!)(%'#($'#(#'#("'#&'#.. &%;*/& 8!:!! )`), y(`2"""6"7#.\xD1 &2$""6$7%.\xC5 &2&""6&7'.\xB9 &2(""6(7).\xAD &2*""6*7+.\xA1 &2,""6,7-.\x95 &2.""6.7/.\x89 &20""6071.} &22""6273.q &24""6475.e &26""6677.Y &28""6879.M &2:""6:7;.A &2<""6<7=.5 &2>""6>7?.) &2@""6@7A`), y('2B""6B7C'), y(`%2D""6D7E/R#;*/I$; /@$;*/7$2F""6F7G/($8%:H%!")(%'#($'#(#'#("'#&'#.A &;6.; &;D.5 &;$./ &%;@/' 8!:I!! )`), y("%;H/' 8!:J!! )"), y(`%;&/\\#;*/S$2K""6K7L/D$;*/;$;&/2$;*/)$8&:M&"%!)(&'#(%'#($'#(#'#("'#&'#./ &%;&/' 8!:N!! )`), y(`%;'/\\#;*/S$2O""6O7P/D$;*/;$;&/2$;*/)$8&:Q&"%!)(&'#(%'#($'#(#'#("'#&'#./ &%;'/' 8!:R!! )`), y(`%;*/i#%;4/"!&,)/Y$2D""6D7E/J$;(/A$2F""6F7G/2$;*/)$8&:S&"$")(&'#(%'#($'#(#'#("'#&'#.a &%%;4/"!&,)/7#2T""6T7U/($8":V"!!)("'#&'#.6 &%%;4/"!&,)/' 8!:V!! )`), y(`%;)/S#;*/J$2W""6W7X/;$;*/2$;(/)$8%:Q%"$ )(%'#($'#(#'#("'#&'#./ &%;)/' 8!:Y!! )`), y(";6./ &;@.) &;2.# &;5"), y('$4Z""5!7[0)*4Z""5!7[&'), y(`%;*/;#2\\""6\\7]/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2^""6^7_/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2\`""6\`7a/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2b""6b7c/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2d""6d7e/,$;*/#$+#)(#'#("'#&'#`), y(`%;*/;#2W""6W7X/,$;*/#$+#)(#'#("'#&'#`), y(";D.5 &;2./ &;5.) &;6.# &;@"), y(`%;,/\x91#%;3/k#$%;0/2#;3/)$8":f""$ )("'#&'#0<*%;0/2#;3/)$8":f""$ )("'#&'#&/)$8":g""! )("'#&'#." &"/1$;./($8#:h#!!)(#'#("'#&'#`), y(`%;@/;#;//2$;1/)$8#:i#"" )(#'#("'#&'#.L &%%;4/"!&,)/;#;//2$;1/)$8#:i#"" )(#'#("'#&'#`), y(`%4j""5!7k/?#$4l""5!7m0)*4l""5!7m&/#$+")("'#&'#`), y(`%;+/\x91#%;1/k#$%;0/2#;1/)$8":n""$ )("'#&'#0<*%;0/2#;1/)$8":n""$ )("'#&'#&/)$8":o""! )("'#&'#." &"/1$;-/($8#:p#!!)(#'#("'#&'#`), y(`<%;=." &"/L#;</C$;;." &"/5$;:." &"/'$8$:r$ )($'#(#'#("'#&'#=." 7q`), y('2s""6s7t'), y('4u""5!7v'), y('4w""5!7x'), y(`%;9/M#;=.# &;>." &"/9$$;M/&#0#*;M&&&#/#$+#)(#'#("'#&'#`), y(`%;7/9#$;M/&#0#*;M&&&#/#$+")("'#&'#`), y(`;?.= &%;8/3#$;M0#*;M&/#$+")("'#&'#`), y('24""6475'), y('22""6273'), y('2y""6y7z'), y(`<%2|""6|7}/N#%$;A0#*;A&/"!&,)/7$2|""6|7}/($8#:~#!!)(#'#("'#&'#.^ &%2\x7F""6\x7F7\x80/N#%$;B0#*;B&/"!&,)/7$2\x7F""6\x7F7\x80/($8#:~#!!)(#'#("'#&'#=." 7{`), y('4\x81""5!7\x82.: &%2\x83""6\x837\x84/& 8!:\x85! ).# &;C'), y('4\x86""5!7\x87.: &%2\x88""6\x887\x89/& 8!:\x8A! ).# &;C'), y(`2\x8B""6\x8B7\x8C.\xA9 &2\x8D""6\x8D7\x8E.\x9D &2\x8F""6\x8F7\x90.\x91 &2\x91""6\x917\x92.\x85 &2\x93""6\x937\x94.y &2\x95""6\x957\x96.m &%2\x97""6\x977\x98/]#%%;N/>#;N/5$;N/,$;N/#$+$)($'#(#'#("'#&'#/"!&,)/($8":\x99"! )("'#&'#`), y('<%;F/& 8!:\x9B! ).? &%;E/& 8!:\x9C! ).. &%;G/& 8!:\x9D! )=." 7\x9A'), y('2\x9E""6\x9E7\x9F'), y('2\xA0""6\xA07\xA1'), y('2\xA2""6\xA27\xA3'), y(`%;I/\x91#$%2s""6s7t/?#;J.0 &$;M/&#0#*;M&&&#/#$+")("'#&'#0O*%2s""6s7t/?#;J.0 &$;M/&#0#*;M&&&#/#$+")("'#&'#&/)$8":\xA4""! )("'#&'#`), y(`%2\xA5""6\xA57\xA6.5 &2\xA7""6\xA77\xA8.) &2s""6s7t/2#;J/)$8":\xA9""! )("'#&'#.# &;J`), y(`%;K/2#;L/)$8":\xAA""! )("'#&'#`), y('4\xAB""5!7\xAC'), y(`%$4\xAD""5!7\xAE0)*4\xAD""5!7\xAE&/' 8!:\xAF!! )`), y('4\xB0""5!7\xB1'), y('4\xB2""5!7\xB3')],
+        d = [v(`%;*/\x9E#;#/\x95$;*/\x8C$$%;*/>#;!/5$;*/,$; /#$+$)($'#(#'#("'#&'#0H*%;*/>#;!/5$;*/,$; /#$+$)($'#(#'#("'#&'#&/2$;*/)$8%: %"#!)(%'#($'#(#'#("'#&'#.. &%;*/& 8!:!! )`), v(`2"""6"7#.\xD1 &2$""6$7%.\xC5 &2&""6&7'.\xB9 &2(""6(7).\xAD &2*""6*7+.\xA1 &2,""6,7-.\x95 &2.""6.7/.\x89 &20""6071.} &22""6273.q &24""6475.e &26""6677.Y &28""6879.M &2:""6:7;.A &2<""6<7=.5 &2>""6>7?.) &2@""6@7A`), v('2B""6B7C'), v(`%2D""6D7E/R#;*/I$; /@$;*/7$2F""6F7G/($8%:H%!")(%'#($'#(#'#("'#&'#.A &;6.; &;D.5 &;$./ &%;@/' 8!:I!! )`), v("%;H/' 8!:J!! )"), v(`%;&/\\#;*/S$2K""6K7L/D$;*/;$;&/2$;*/)$8&:M&"%!)(&'#(%'#($'#(#'#("'#&'#./ &%;&/' 8!:N!! )`), v(`%;'/\\#;*/S$2O""6O7P/D$;*/;$;&/2$;*/)$8&:Q&"%!)(&'#(%'#($'#(#'#("'#&'#./ &%;'/' 8!:R!! )`), v(`%;*/i#%;4/"!&,)/Y$2D""6D7E/J$;(/A$2F""6F7G/2$;*/)$8&:S&"$")(&'#(%'#($'#(#'#("'#&'#.a &%%;4/"!&,)/7#2T""6T7U/($8":V"!!)("'#&'#.6 &%%;4/"!&,)/' 8!:V!! )`), v(`%;)/S#;*/J$2W""6W7X/;$;*/2$;(/)$8%:Q%"$ )(%'#($'#(#'#("'#&'#./ &%;)/' 8!:Y!! )`), v(";6./ &;@.) &;2.# &;5"), v('$4Z""5!7[0)*4Z""5!7[&'), v(`%;*/;#2\\""6\\7]/,$;*/#$+#)(#'#("'#&'#`), v(`%;*/;#2^""6^7_/,$;*/#$+#)(#'#("'#&'#`), v(`%;*/;#2\`""6\`7a/,$;*/#$+#)(#'#("'#&'#`), v(`%;*/;#2b""6b7c/,$;*/#$+#)(#'#("'#&'#`), v(`%;*/;#2d""6d7e/,$;*/#$+#)(#'#("'#&'#`), v(`%;*/;#2W""6W7X/,$;*/#$+#)(#'#("'#&'#`), v(";D.5 &;2./ &;5.) &;6.# &;@"), v(`%;,/\x91#%;3/k#$%;0/2#;3/)$8":f""$ )("'#&'#0<*%;0/2#;3/)$8":f""$ )("'#&'#&/)$8":g""! )("'#&'#." &"/1$;./($8#:h#!!)(#'#("'#&'#`), v(`%;@/;#;//2$;1/)$8#:i#"" )(#'#("'#&'#.L &%%;4/"!&,)/;#;//2$;1/)$8#:i#"" )(#'#("'#&'#`), v(`%4j""5!7k/?#$4l""5!7m0)*4l""5!7m&/#$+")("'#&'#`), v(`%;+/\x91#%;1/k#$%;0/2#;1/)$8":n""$ )("'#&'#0<*%;0/2#;1/)$8":n""$ )("'#&'#&/)$8":o""! )("'#&'#." &"/1$;-/($8#:p#!!)(#'#("'#&'#`), v(`<%;=." &"/L#;</C$;;." &"/5$;:." &"/'$8$:r$ )($'#(#'#("'#&'#=." 7q`), v('2s""6s7t'), v('4u""5!7v'), v('4w""5!7x'), v(`%;9/M#;=.# &;>." &"/9$$;M/&#0#*;M&&&#/#$+#)(#'#("'#&'#`), v(`%;7/9#$;M/&#0#*;M&&&#/#$+")("'#&'#`), v(`;?.= &%;8/3#$;M0#*;M&/#$+")("'#&'#`), v('24""6475'), v('22""6273'), v('2y""6y7z'), v(`<%2|""6|7}/N#%$;A0#*;A&/"!&,)/7$2|""6|7}/($8#:~#!!)(#'#("'#&'#.^ &%2\x7F""6\x7F7\x80/N#%$;B0#*;B&/"!&,)/7$2\x7F""6\x7F7\x80/($8#:~#!!)(#'#("'#&'#=." 7{`), v('4\x81""5!7\x82.: &%2\x83""6\x837\x84/& 8!:\x85! ).# &;C'), v('4\x86""5!7\x87.: &%2\x88""6\x887\x89/& 8!:\x8A! ).# &;C'), v(`2\x8B""6\x8B7\x8C.\xA9 &2\x8D""6\x8D7\x8E.\x9D &2\x8F""6\x8F7\x90.\x91 &2\x91""6\x917\x92.\x85 &2\x93""6\x937\x94.y &2\x95""6\x957\x96.m &%2\x97""6\x977\x98/]#%%;N/>#;N/5$;N/,$;N/#$+$)($'#(#'#("'#&'#/"!&,)/($8":\x99"! )("'#&'#`), v('<%;F/& 8!:\x9B! ).? &%;E/& 8!:\x9C! ).. &%;G/& 8!:\x9D! )=." 7\x9A'), v('2\x9E""6\x9E7\x9F'), v('2\xA0""6\xA07\xA1'), v('2\xA2""6\xA27\xA3'), v(`%;I/\x91#$%2s""6s7t/?#;J.0 &$;M/&#0#*;M&&&#/#$+")("'#&'#0O*%2s""6s7t/?#;J.0 &$;M/&#0#*;M&&&#/#$+")("'#&'#&/)$8":\xA4""! )("'#&'#`), v(`%2\xA5""6\xA57\xA6.5 &2\xA7""6\xA77\xA8.) &2s""6s7t/2#;J/)$8":\xA9""! )("'#&'#.# &;J`), v(`%;K/2#;L/)$8":\xAA""! )("'#&'#`), v('4\xAB""5!7\xAC'), v(`%$4\xAD""5!7\xAE0)*4\xAD""5!7\xAE&/' 8!:\xAF!! )`), v('4\xB0""5!7\xB1'), v('4\xB2""5!7\xB3')],
         f = 0,
-        d = 0,
-        h = [{
+        c = 0,
+        g = [{
             line: 1,
             column: 1
         }],
-        v = 0,
+        y = 0,
         A = [],
         L = 0,
         I;
     if (e.startRule !== void 0) {
         if (!(e.startRule in i)) throw new Error(`Can't start parsing from rule "` + e.startRule + '".');
         o = i[e.startRule]
     }
 
     function B() {
-        return t.substring(d, f)
+        return t.substring(c, f)
     }
 
     function N() {
-        return Y(d, f)
+        return Y(c, f)
     }
 
-    function q(p, l) {
-        throw l = l !== void 0 ? l : Y(d, f), we([fe(p)], t.substring(d, f), l)
+    function G(p, l) {
+        throw l = l !== void 0 ? l : Y(c, f), _e([he(p)], t.substring(c, f), l)
     }
 
-    function O(p, l) {
-        throw l = l !== void 0 ? l : Y(d, f), Oe(p, l)
+    function D(p, l) {
+        throw l = l !== void 0 ? l : Y(c, f), Ve(p, l)
     }
 
     function b(p, l) {
         return {
             type: "literal",
             text: p,
             ignoreCase: l
@@ -2032,89 +2202,89 @@
             type: "class",
             parts: p,
             inverted: l,
             ignoreCase: a
         }
     }
 
-    function ft() {
+    function xt() {
         return {
             type: "any"
         }
     }
 
-    function ue() {
+    function me() {
         return {
             type: "end"
         }
     }
 
-    function fe(p) {
+    function he(p) {
         return {
             type: "other",
             description: p
         }
     }
 
-    function Pe(p) {
-        let l = h[p],
+    function Ne(p) {
+        let l = g[p],
             a;
         if (l) return l;
-        for (a = p - 1; !h[a];) a--;
-        for (l = h[a], l = {
+        for (a = p - 1; !g[a];) a--;
+        for (l = g[a], l = {
                 line: l.line,
                 column: l.column
             }; a < p;) t.charCodeAt(a) === 10 ? (l.line++, l.column = 1) : l.column++, a++;
-        return h[p] = l, l
+        return g[p] = l, l
     }
 
     function Y(p, l) {
-        let a = Pe(p),
-            C = Pe(l);
+        let a = Ne(p),
+            _ = Ne(l);
         return {
             source: n,
             start: {
                 offset: p,
                 line: a.line,
                 column: a.column
             },
             end: {
                 offset: l,
-                line: C.line,
-                column: C.column
+                line: _.line,
+                column: _.column
             }
         }
     }
 
-    function De(p) {
-        f < v || (f > v && (v = f, A = []), A.push(p))
+    function qe(p) {
+        f < y || (f > y && (y = f, A = []), A.push(p))
     }
 
-    function Oe(p, l) {
+    function Ve(p, l) {
         return new Z(p, [], "", l)
     }
 
-    function we(p, l, a) {
+    function _e(p, l, a) {
         return new Z(Z.buildMessage(p, l), p, l, a)
     }
 
-    function y(p) {
+    function v(p) {
         return p.split("").map(l => l.charCodeAt(0) - 32)
     }
 
-    function He(p) {
-        let l = u[p],
+    function Ge(p) {
+        let l = d[p],
             a = 0,
-            C = [],
-            _ = l.length,
-            V = [],
+            _ = [],
+            C = l.length,
+            q = [],
             E = [],
-            ke;
+            Fe;
         for (;;) {
-            for (; a < _;) switch (l[a]) {
+            for (; a < C;) switch (l[a]) {
                 case 0:
                     E.push(s[l[a + 1]]), a += 2;
                     break;
                 case 1:
                     E.push(void 0), a++;
                     break;
                 case 2:
@@ -2147,153 +2317,153 @@
                 case 11:
                     E.push(E.splice(E.length - l[a + 1], l[a + 1])), a += 2;
                     break;
                 case 12:
                     E.push(t.substring(E.pop(), f)), a++;
                     break;
                 case 13:
-                    V.push(_), C.push(a + 3 + l[a + 1] + l[a + 2]), E[E.length - 1] ? (_ = a + 3 + l[a + 1], a += 3) : (_ = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
+                    q.push(C), _.push(a + 3 + l[a + 1] + l[a + 2]), E[E.length - 1] ? (C = a + 3 + l[a + 1], a += 3) : (C = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
                     break;
                 case 14:
-                    V.push(_), C.push(a + 3 + l[a + 1] + l[a + 2]), E[E.length - 1] === r ? (_ = a + 3 + l[a + 1], a += 3) : (_ = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
+                    q.push(C), _.push(a + 3 + l[a + 1] + l[a + 2]), E[E.length - 1] === r ? (C = a + 3 + l[a + 1], a += 3) : (C = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
                     break;
                 case 15:
-                    V.push(_), C.push(a + 3 + l[a + 1] + l[a + 2]), E[E.length - 1] !== r ? (_ = a + 3 + l[a + 1], a += 3) : (_ = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
+                    q.push(C), _.push(a + 3 + l[a + 1] + l[a + 2]), E[E.length - 1] !== r ? (C = a + 3 + l[a + 1], a += 3) : (C = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
                     break;
                 case 16:
-                    E[E.length - 1] !== r ? (V.push(_), C.push(a), _ = a + 2 + l[a + 1], a += 2) : a += 2 + l[a + 1];
+                    E[E.length - 1] !== r ? (q.push(C), _.push(a), C = a + 2 + l[a + 1], a += 2) : a += 2 + l[a + 1];
                     break;
                 case 17:
-                    V.push(_), C.push(a + 3 + l[a + 1] + l[a + 2]), t.length > f ? (_ = a + 3 + l[a + 1], a += 3) : (_ = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
+                    q.push(C), _.push(a + 3 + l[a + 1] + l[a + 2]), t.length > f ? (C = a + 3 + l[a + 1], a += 3) : (C = a + 3 + l[a + 1] + l[a + 2], a += 3 + l[a + 1]);
                     break;
                 case 18:
-                    V.push(_), C.push(a + 4 + l[a + 2] + l[a + 3]), t.substr(f, s[l[a + 1]].length) === s[l[a + 1]] ? (_ = a + 4 + l[a + 2], a += 4) : (_ = a + 4 + l[a + 2] + l[a + 3], a += 4 + l[a + 2]);
+                    q.push(C), _.push(a + 4 + l[a + 2] + l[a + 3]), t.substr(f, s[l[a + 1]].length) === s[l[a + 1]] ? (C = a + 4 + l[a + 2], a += 4) : (C = a + 4 + l[a + 2] + l[a + 3], a += 4 + l[a + 2]);
                     break;
                 case 19:
-                    V.push(_), C.push(a + 4 + l[a + 2] + l[a + 3]), t.substr(f, s[l[a + 1]].length).toLowerCase() === s[l[a + 1]] ? (_ = a + 4 + l[a + 2], a += 4) : (_ = a + 4 + l[a + 2] + l[a + 3], a += 4 + l[a + 2]);
+                    q.push(C), _.push(a + 4 + l[a + 2] + l[a + 3]), t.substr(f, s[l[a + 1]].length).toLowerCase() === s[l[a + 1]] ? (C = a + 4 + l[a + 2], a += 4) : (C = a + 4 + l[a + 2] + l[a + 3], a += 4 + l[a + 2]);
                     break;
                 case 20:
-                    V.push(_), C.push(a + 4 + l[a + 2] + l[a + 3]), s[l[a + 1]].test(t.charAt(f)) ? (_ = a + 4 + l[a + 2], a += 4) : (_ = a + 4 + l[a + 2] + l[a + 3], a += 4 + l[a + 2]);
+                    q.push(C), _.push(a + 4 + l[a + 2] + l[a + 3]), s[l[a + 1]].test(t.charAt(f)) ? (C = a + 4 + l[a + 2], a += 4) : (C = a + 4 + l[a + 2] + l[a + 3], a += 4 + l[a + 2]);
                     break;
                 case 21:
                     E.push(t.substr(f, l[a + 1])), f += l[a + 1], a += 2;
                     break;
                 case 22:
                     E.push(s[l[a + 1]]), f += s[l[a + 1]].length, a += 2;
                     break;
                 case 23:
-                    E.push(r), L === 0 && De(s[l[a + 1]]), a += 2;
+                    E.push(r), L === 0 && qe(s[l[a + 1]]), a += 2;
                     break;
                 case 24:
-                    d = E[E.length - 1 - l[a + 1]], a += 2;
+                    c = E[E.length - 1 - l[a + 1]], a += 2;
                     break;
                 case 25:
-                    d = f, a++;
+                    c = f, a++;
                     break;
                 case 26:
-                    ke = l.slice(a + 4, a + 4 + l[a + 3]).map(function(Ae) {
-                        return E[E.length - 1 - Ae]
-                    }), E.splice(E.length - l[a + 2], l[a + 2], s[l[a + 1]].apply(null, ke)), a += 4 + l[a + 3];
+                    Fe = l.slice(a + 4, a + 4 + l[a + 3]).map(function(Se) {
+                        return E[E.length - 1 - Se]
+                    }), E.splice(E.length - l[a + 2], l[a + 2], s[l[a + 1]].apply(null, Fe)), a += 4 + l[a + 3];
                     break;
                 case 27:
-                    E.push(He(l[a + 1])), a += 2;
+                    E.push(Ge(l[a + 1])), a += 2;
                     break;
                 case 28:
                     L++, a++;
                     break;
                 case 29:
                     L--, a++;
                     break;
                 default:
                     throw new Error("Invalid opcode: " + l[a] + ".")
             }
-            if (V.length > 0) _ = V.pop(), a = C.pop();
+            if (q.length > 0) C = q.pop(), a = _.pop();
             else break
         }
         return E[0]
     }
-    if (I = He(o), I !== r && f === t.length) return I;
-    throw I !== r && f < t.length && De(ue()), we(A, v < t.length ? t.charAt(v) : null, v < t.length ? Y(v, v + 1) : Y(v, v))
+    if (I = Ge(o), I !== r && f === t.length) return I;
+    throw I !== r && f < t.length && qe(me()), _e(A, y < t.length ? t.charAt(y) : null, y < t.length ? Y(y, y + 1) : Y(y, y))
 }
-var ye = hs;
-var xn = `select::placeholder{color:gray}select.ts-hidden-accessible{display:none}django-formset{--django-formset-color-invalid: rgb(255, 3, 0);--django-formset-shadow-invalid: rgb(255, 3, 0, 0.25);--django-formset-color-valid: rgb(0, 122, 0);--django-formset-icon-invalid: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(255, 3, 0)"><path fill-rule="evenodd" d="M8 15A7 7 0 1 0 8 1a7 7 0 0 0 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"/><path d="M7.002 11a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 4.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 4.995z"/></svg>');--django-formset-icon-warning: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(255, 165, 0)"><path fill-rule="evenodd" d="M7.938 2.016a.146.146 0 0 0-.054.057L1.027 13.74a.176.176 0 0 0-.002.183c.016.03.037.05.054.06.015.01.034.017.066.017h13.713a.12.12 0 0 0 .066-.017.163.163 0 0 0 .055-.06.176.176 0 0 0-.003-.183L8.12 2.073a.146.146 0 0 0-.054-.057A.13.13 0 0 0 8.002 2a.13.13 0 0 0-.064.016zm1.044-.45a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566z"/><path d="M7.002 12a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 5.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995z"/></svg>');--django-formset-icon-valid: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(0, 122, 0)"><path fill-rule="evenodd" d="M10.97 4.97a.75.75 0 0 1 1.071 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.236.236 0 0 1 .02-.022z"/></svg>')}django-formset ul.dj-errorlist{list-style:none;margin-top:0;margin-bottom:0;margin-left:0;padding-left:0;color:var(--django-formset-color-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=email]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=email]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=text]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=text]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=number]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=number]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=date]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=date]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=datetime-local]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=url]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=url]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=password]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=password]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>select:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>select:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>textarea:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>textarea:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=email]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=email]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=text]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=text]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=number]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=number]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=date]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=date]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=datetime-local]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=url]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=url]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=password]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=password]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset [role=group]{display:block}django-formset [role=group][hidden]{display:none}django-formset [role=group].dj-required>label,django-formset [role=group].dj-required-any>label{font-weight:bolder}django-formset [role=group].dj-submitted>input[type=email]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=email]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=text]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=text]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=number]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=number]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=date]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=date]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=datetime-local]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=url]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=url]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=password]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=password]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>select:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>select:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>textarea:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>textarea:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group] input{background-repeat:no-repeat !important;background-position:center right !important;background-origin:content-box !important}django-formset [role=group] input[type=date],django-formset [role=group] input[type=datetime-local]{position:relative}django-formset [role=group] input[type=date]::-webkit-datetime-edit-fields-wrapper,django-formset [role=group] input[type=datetime-local]::-webkit-datetime-edit-fields-wrapper{margin-left:1.75em}django-formset [role=group] input[type=date]::-webkit-calendar-picker-indicator,django-formset [role=group] input[type=datetime-local]::-webkit-calendar-picker-indicator{cursor:pointer;position:absolute;left:.75em}django-formset [role=group] input[type=date]:hover::-webkit-calendar-picker-indicator,django-formset [role=group] input[type=datetime-local]:hover::-webkit-calendar-picker-indicator{cursor:pointer}django-formset [role=group] select,django-formset [role=group] textarea{background-image:none !important}django-formset [role=group] select.dj-concealed,django-formset [role=group] textarea.dj-concealed{display:block !important;height:1px !important;min-height:initial !important;max-height:initial !important;padding:0 !important;margin:-1px 0 0 0 !important;border:none !important;opacity:0 !important;resize:none}django-formset [role=group] .dj-help-text{font-style:oblique}django-formset [role=group] .dj-form-optgroup{margin-bottom:.5rem}django-formset [role=group] .dj-form-optgroup>em{margin-left:.75rem}django-formset [role=group] .dj-form-inlined{display:inline-block}django-formset [role=group] input[type=file]{width:0 !important;height:0 !important}django-formset [role=group] .dj-control-panel{display:flex}django-formset [role=group] .dj-control-panel>div{height:fit-content;margin-left:.5rem}django-formset [role=group] .dj-control-panel>div progress{width:100%;margin-top:.25rem}django-formset [role=group] figure.dj-dropbox{all:unset;display:inline-flex;align-items:center;justify-content:space-between;background-color:#f5f5f5;margin:0 0 .25rem .25rem;padding:0;list-style:none;height:8rem;min-width:8rem;outline:gray thin dotted}django-formset [role=group] figure.dj-dropbox>div.dj-empty-item{flex-grow:1;text-align:center;height:auto}django-formset [role=group] figure.dj-dropbox>div.dj-empty-item p{padding-left:.5rem;padding-right:.5rem}django-formset [role=group] figure.dj-dropbox>img{all:unset;flex-grow:1;display:block;height:inherit;max-width:calc(100% - 12rem)}django-formset [role=group] figure.dj-dropbox>figcaption{all:unset;padding:.25rem .5rem;background-color:#fff;overflow-x:hidden;min-width:12rem}django-formset [role=group] figure.dj-dropbox>figcaption dl{font-size:small;margin:0 0 .25rem 0}django-formset [role=group] figure.dj-dropbox>figcaption dl dd{margin:0}django-formset [role=group] figure.dj-dropbox>figcaption .dj-delete-file,django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file{font-weight:bold;display:inline-block;cursor:pointer;text-decoration:none}django-formset [role=group] figure.dj-dropbox>figcaption .dj-delete-file:hover,django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file:hover{text-decoration:underline}django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file{margin-left:1rem;float:right}django-formset [role=group] .dj-dual-selector{display:flex}django-formset [role=group] .dj-dual-selector .left-column,django-formset [role=group] .dj-dual-selector .right-column,django-formset [role=group] .dj-dual-selector .control-column,django-formset [role=group] .dj-dual-selector .control-panel{display:flex;flex-direction:column}django-formset [role=group] .dj-dual-selector .control-column{justify-content:center;align-items:center}django-formset [role=group] .dj-dual-selector .control-panel{padding:1rem .5rem}django-formset [role=group] .dj-dual-selector select,django-formset [role=group] .dj-dual-selector django-sortable-select{min-width:10rem}django-formset [role=group] .dj-dual-selector select{height:auto}django-formset [role=group] .dj-dual-selector input{z-index:1}django-formset [role=group] .dj-dual-selector button svg{vertical-align:middle;width:16px;height:16px}django-formset [role=group] .dj-dual-selector.invalid .right-column input{border-color:var(--django-formset-color-invalid)}django-formset [role=group] .dj-dual-selector.invalid .right-column input:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group] .dj-dual-selector.invalid .right-column select,django-formset [role=group] .dj-dual-selector.invalid .right-column django-sortable-select{border-left-color:var(--django-formset-color-invalid);border-right-color:var(--django-formset-color-invalid);border-bottom-color:var(--django-formset-color-invalid)}django-formset [role=group] .dj-dual-selector.invalid .right-column select:focus,django-formset [role=group] .dj-dual-selector.invalid .right-column django-sortable-select.focus{border-top-color:var(--django-formset-color-invalid);box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}.dj-button-decorator{line-height:initial}.dj-button-decorator svg{vertical-align:baseline;width:1rem;height:1rem}.dj-button-decorator svg .path{stroke-dasharray:1000;stroke-dashoffset:0}.dj-button-decorator svg .path.circle{animation:dash .9s ease-in-out}.dj-button-decorator svg .path.line{stroke-dashoffset:1000;animation:dash .9s .35s ease-in-out forwards}.dj-button-decorator svg .path.check{stroke-dashoffset:-100;animation:dash-check .9s .35s ease-in-out forwards}.dj-button-decorator svg .spinner{transform-origin:center;animation:rotate 1.5s infinite linear}@keyframes dash{0%{stroke-dashoffset:1000}100%{stroke-dashoffset:0}}@keyframes dash-check{0%{stroke-dashoffset:-100}100%{stroke-dashoffset:900}}@keyframes rotate{from{transform:rotate(0deg)}to{transform:rotate(360deg)}}.dj-button-decorator .dj-icon{display:inline-block;width:1em;height:1em}`;
-var En = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
+var ke = _l;
+var Zn = `select::placeholder{color:gray}select.ts-hidden-accessible{display:none}django-formset{--django-formset-color-invalid: rgb(255, 3, 0);--django-formset-shadow-invalid: rgb(255, 3, 0, 0.25);--django-formset-color-valid: rgb(0, 122, 0);--django-formset-icon-invalid: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(255, 3, 0)"><path fill-rule="evenodd" d="M8 15A7 7 0 1 0 8 1a7 7 0 0 0 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"/><path d="M7.002 11a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 4.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 4.995z"/></svg>');--django-formset-icon-warning: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(255, 165, 0)"><path fill-rule="evenodd" d="M7.938 2.016a.146.146 0 0 0-.054.057L1.027 13.74a.176.176 0 0 0-.002.183c.016.03.037.05.054.06.015.01.034.017.066.017h13.713a.12.12 0 0 0 .066-.017.163.163 0 0 0 .055-.06.176.176 0 0 0-.003-.183L8.12 2.073a.146.146 0 0 0-.054-.057A.13.13 0 0 0 8.002 2a.13.13 0 0 0-.064.016zm1.044-.45a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566z"/><path d="M7.002 12a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 5.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995z"/></svg>');--django-formset-icon-valid: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 16" fill="rgb(0, 122, 0)"><path fill-rule="evenodd" d="M10.97 4.97a.75.75 0 0 1 1.071 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.236.236 0 0 1 .02-.022z"/></svg>')}django-formset ul.dj-errorlist{list-style:none;margin-top:0;margin-bottom:0;margin-left:0;padding-left:0;color:var(--django-formset-color-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid:not(:focus),django-formset.dj-feedback-errors [role=group].dj-touched:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid:not(:focus){border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid:focus,django-formset.dj-feedback-warnings [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid:focus{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=email]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=email]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=text]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=text]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=number]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=number]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=date]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=date]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=datetime-local]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=url]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=url]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>input[type=password]:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>input[type=password]:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>select:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>select:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted)>textarea:not(.dj-exempt-feedback):invalid,django-formset.dj-feedback-warnings:not(.dj-feedback-errors) [role=group].dj-dirty:not(.dj-submitted) :not([role=group])>textarea:not(.dj-exempt-feedback):invalid{background-image:var(--django-formset-icon-warning)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=email]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=email]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=text]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=text]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=number]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=number]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=date]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=date]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=datetime-local]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=url]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=url]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=password]:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=password]:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>select:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>select:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>textarea:not(.dj-exempt-feedback):valid:not(:focus),django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>textarea:not(.dj-exempt-feedback):valid:not(:focus){border-color:var(--django-formset-color-valid)}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=email]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=email]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=text]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=text]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=number]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=number]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=date]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=date]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=datetime-local]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=datetime-local]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=url]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=url]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset.dj-feedback-success [role=group].dj-dirty>input[type=password]:not(.dj-exempt-feedback):valid,django-formset.dj-feedback-success [role=group].dj-dirty :not([role=group])>input[type=password]:not(.dj-exempt-feedback):valid{background-image:var(--django-formset-icon-valid) !important}django-formset [role=group]{display:block}django-formset [role=group][hidden]{display:none}django-formset [role=group].dj-required>label,django-formset [role=group].dj-required-any>label{font-weight:bolder}django-formset [role=group].dj-submitted>input[type=email]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=email]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=text]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=text]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=number]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=number]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=date]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=date]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=datetime-local]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=datetime-local]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=url]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=url]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>input[type=password]:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>input[type=password]:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>select:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>select:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group].dj-submitted>textarea:not(.dj-exempt-feedback):invalid{border-color:var(--django-formset-color-invalid);background-image:var(--django-formset-icon-invalid)}django-formset [role=group].dj-submitted>textarea:not(.dj-exempt-feedback):invalid:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group] input{background-repeat:no-repeat !important;background-position:center right !important;background-origin:content-box !important}django-formset [role=group] input[type=date],django-formset [role=group] input[type=datetime-local]{position:relative}django-formset [role=group] input[type=date]::-webkit-datetime-edit-fields-wrapper,django-formset [role=group] input[type=datetime-local]::-webkit-datetime-edit-fields-wrapper{margin-left:1.75em}django-formset [role=group] input[type=date]::-webkit-calendar-picker-indicator,django-formset [role=group] input[type=datetime-local]::-webkit-calendar-picker-indicator{cursor:pointer;position:absolute;left:.75em}django-formset [role=group] input[type=date]:hover::-webkit-calendar-picker-indicator,django-formset [role=group] input[type=datetime-local]:hover::-webkit-calendar-picker-indicator{cursor:pointer}django-formset [role=group] select,django-formset [role=group] textarea{background-image:none !important}django-formset [role=group] select.dj-concealed,django-formset [role=group] textarea.dj-concealed{display:block !important;height:1px !important;min-height:initial !important;max-height:initial !important;padding:0 !important;margin:-1px 0 0 0 !important;border:none !important;opacity:0 !important;resize:none}django-formset [role=group] .dj-help-text{font-style:oblique}django-formset [role=group] .dj-form-optgroup{margin-bottom:.5rem}django-formset [role=group] .dj-form-optgroup>em{margin-left:.75rem}django-formset [role=group] .dj-form-inlined{display:inline-block}django-formset [role=group] input[type=file]{width:0 !important;height:0 !important}django-formset [role=group] .dj-control-panel{display:flex}django-formset [role=group] .dj-control-panel>div{height:fit-content;margin-left:.5rem}django-formset [role=group] .dj-control-panel>div progress{width:100%;margin-top:.25rem}django-formset [role=group] figure.dj-dropbox{all:unset;display:inline-flex;align-items:center;justify-content:space-between;background-color:#f5f5f5;margin:0 0 .25rem .25rem;padding:0;list-style:none;height:8rem;min-width:8rem;outline:gray thin dotted}django-formset [role=group] figure.dj-dropbox>div.dj-empty-item{flex-grow:1;text-align:center;height:auto}django-formset [role=group] figure.dj-dropbox>div.dj-empty-item p{padding-left:.5rem;padding-right:.5rem}django-formset [role=group] figure.dj-dropbox>img{all:unset;flex-grow:1;display:block;height:inherit;max-width:calc(100% - 12rem)}django-formset [role=group] figure.dj-dropbox>figcaption{all:unset;padding:.25rem .5rem;background-color:#fff;overflow-x:hidden;min-width:12rem}django-formset [role=group] figure.dj-dropbox>figcaption dl{font-size:small;margin:0 0 .25rem 0}django-formset [role=group] figure.dj-dropbox>figcaption dl dd{margin:0}django-formset [role=group] figure.dj-dropbox>figcaption .dj-delete-file,django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file{font-weight:bold;display:inline-block;cursor:pointer;text-decoration:none}django-formset [role=group] figure.dj-dropbox>figcaption .dj-delete-file:hover,django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file:hover{text-decoration:underline}django-formset [role=group] figure.dj-dropbox>figcaption .dj-download-file{margin-left:1rem;float:right}django-formset [role=group] .dj-dual-selector{display:flex}django-formset [role=group] .dj-dual-selector .left-column,django-formset [role=group] .dj-dual-selector .right-column,django-formset [role=group] .dj-dual-selector .control-column,django-formset [role=group] .dj-dual-selector .control-panel{display:flex;flex-direction:column}django-formset [role=group] .dj-dual-selector .control-column{justify-content:center;align-items:center}django-formset [role=group] .dj-dual-selector .control-panel{padding:1rem .5rem}django-formset [role=group] .dj-dual-selector select,django-formset [role=group] .dj-dual-selector django-sortable-select{min-width:10rem}django-formset [role=group] .dj-dual-selector select{height:auto}django-formset [role=group] .dj-dual-selector input{z-index:1}django-formset [role=group] .dj-dual-selector button svg{vertical-align:middle;width:16px;height:16px}django-formset [role=group] .dj-dual-selector.invalid .right-column input{border-color:var(--django-formset-color-invalid)}django-formset [role=group] .dj-dual-selector.invalid .right-column input:focus{box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}django-formset [role=group] .dj-dual-selector.invalid .right-column select,django-formset [role=group] .dj-dual-selector.invalid .right-column django-sortable-select{border-left-color:var(--django-formset-color-invalid);border-right-color:var(--django-formset-color-invalid);border-bottom-color:var(--django-formset-color-invalid)}django-formset [role=group] .dj-dual-selector.invalid .right-column select:focus,django-formset [role=group] .dj-dual-selector.invalid .right-column django-sortable-select.focus{border-top-color:var(--django-formset-color-invalid);box-shadow:0 0 0 .2rem var(--django-formset-shadow-invalid)}.dj-button-decorator{line-height:initial}.dj-button-decorator svg{vertical-align:baseline;width:1rem;height:1rem}.dj-button-decorator svg .path{stroke-dasharray:1000;stroke-dashoffset:0}.dj-button-decorator svg .path.circle{animation:dash .9s ease-in-out}.dj-button-decorator svg .path.line{stroke-dashoffset:1000;animation:dash .9s .35s ease-in-out forwards}.dj-button-decorator svg .path.check{stroke-dashoffset:-100;animation:dash-check .9s .35s ease-in-out forwards}.dj-button-decorator svg .spinner{transform-origin:center;animation:rotate 1.5s infinite linear}@keyframes dash{0%{stroke-dashoffset:1000}100%{stroke-dashoffset:0}}@keyframes dash-check{0%{stroke-dashoffset:-100}100%{stroke-dashoffset:900}}@keyframes rotate{from{transform:rotate(0deg)}to{transform:rotate(360deg)}}.dj-button-decorator .dj-icon{display:inline-block;width:1em;height:1em}`;
+var Yn = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<g class="spinner">
 		<path style="stroke-width:0.729" d="m 12.73285,23.212276 -10e-7,-4.393157 A 0.27932072,0.27932072 0 0 0 12.27476,18.604602 l -2.6367848,2.196577 a 0.27932072,0.27932072 0 0 0 -10e-8,0.429037 l 2.6367859,2.196577 a 0.27932072,0.27932072 0 0 0 0.458089,-0.214517 z" />
 		<path style="stroke-width:0.729" d="m 11.298326,5.191792 -10e-7,-4.39315704 a 0.27932072,0.27932072 0 0 1 0.458086,-0.214519 L 14.393193,2.780699 a 0.27932072,0.27932072 0 0 1 2e-6,0.429033 l -2.636785,2.19658 a 0.27932072,0.27932072 0 0 1 -0.458084,-0.21452 z" />
 		<path style="fill:none;stroke:currentColor;stroke-width:2;stroke-linecap:round;stroke-miterlimit:10;stroke-dashoffset:89.339;stroke-dasharray:none" d="M 12.5,2.9179688 C 12.333705,2.9010187 12.166975,2.8886442 12,2.8808594 6.9635919,2.8807514 2.8807499,6.9635934 2.8808594,12 c 0.00661,2.530252 1.064217,4.944009 2.9199218,6.664062" />
 		<path style="fill:none;stroke:currentColor;stroke-width:2;stroke-linecap:round;stroke-miterlimit:10;stroke-dashoffset:89.339;stroke-dasharray:none" d="m 11.458261,21.082031 c 0.166295,0.01695 0.333025,0.02933 0.5,0.03711 C 16.994669,21.119249 21.077511,17.036407 21.077402,12 21.070802,9.469748 20.013185,7.055991 18.15748,5.335938" />
 	</g>
 </svg>
 `;
-var wn = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
+var Qn = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<circle class="path circle" fill="none" stroke="currentColor" stroke-width="1.93833" stroke-miterlimit="10" cx="12.000002" cy="12.000002" r="10.030837" />
 	<polyline class="path check" fill="none" stroke="currentColor" stroke-width="12" stroke-linecap="round" stroke-miterlimit="10" points="100.2,40.2 51.5,88.8 29.8,67.5 " transform="matrix(0.18,0,0,0.18,-0.284,0.544)" />
 </svg>
 `;
-var kn = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
+var eo = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<circle class="path circle" fill="none" stroke="currentColor" stroke-width="1.93833" stroke-miterlimit="10" cx="12.000002" cy="12.000002" r="10.030837" />
 	<line class="path line" fill="none" stroke="currentColor" stroke-width="2.12533" stroke-linecap="round" stroke-miterlimit="10" x1="6.562665" y1="7.1626649" x2="17.437328" y2="16.79755" />
 	<line class="path line" fill="none" stroke="currentColor" stroke-width="2.12534" stroke-linecap="round" stroke-miterlimit="10" x1="17.437338" y1="7.1626701" x2="6.5626698" y2="16.762127" />
 </svg>
 `;
-var xs = "__all__",
-    Es = "_collection_errors_",
-    ws = "_marked_for_removal_",
-    Cn = document.createElement("style");
-Cn.innerText = xn;
-document.head.appendChild(Cn);
-var Nt = class {
+var Ml = "__all__",
+    Il = "_collection_errors_",
+    Pl = "_marked_for_removal_",
+    io = document.createElement("style");
+io.innerText = Zn;
+document.head.appendChild(io);
+var or = class {
         constructor(e) {
             this.value = e
         }
     },
-    Vt = class extends Map {
+    ir = class extends Map {
         constructor(e) {
             super();
-            let r = e.element.querySelector("django-error-messages");
-            if (!r) throw new Error(`<div role="group"> for '${e.name}' requires one <django-error-messages> tag.`);
+            let r = e.element.querySelector('meta[name="error-messages"]');
+            if (!r) throw new Error(`<div role="group"> for '${e.name}' requires one <meta name="error-messages"> tag.`);
             for (let n of r.getAttributeNames()) {
                 let i = n.replace(/([_][a-z])/g, s => s.toUpperCase().replace("_", "")),
                     o = r.getAttribute(n);
                 o && this.set(i, o)
             }
         }
     },
-    Gt = class {
+    ar = class {
         constructor(e, r) {
-            this.form = e, this.element = r, this.errorPlaceholder = r.querySelector(".dj-errorlist > .dj-placeholder"), this.errorMessages = new Vt(this);
+            this.form = e, this.element = r, this.errorPlaceholder = r.querySelector(".dj-errorlist > .dj-placeholder"), this.errorMessages = new ir(this);
             let n = r.classList.contains("dj-required-any"),
-                i = h => h instanceof HTMLInputElement && h.name && h.form === e.element && h.type !== "hidden",
+                i = g => g instanceof HTMLInputElement && g.name && g.form === e.element && g.type !== "hidden",
                 o = Array.from(r.getElementsByTagName("INPUT")).filter(i);
-            for (let h of o) switch (h.type) {
+            for (let g of o) switch (g.type) {
                 case "checkbox":
                 case "radio":
-                    h.addEventListener("input", () => {
+                    g.addEventListener("input", () => {
                         this.touch(), this.inputted()
-                    }), h.addEventListener("change", () => {
+                    }), g.addEventListener("change", () => {
                         n ? this.validateCheckboxSelectMultiple() : this.validate()
                     });
                     break;
                 case "file":
-                    this.fileUploader = new dt(this, h);
+                    this.fileUploader = new yt(this, g);
                     break;
                 default:
-                    h.addEventListener("focus", () => this.touch()), h.addEventListener("input", () => this.inputted()), h.addEventListener("blur", () => this.validate());
+                    g.addEventListener("focus", () => this.touch()), g.addEventListener("input", () => this.inputted()), g.addEventListener("blur", () => this.validate());
                     break
             }
             this.fieldElements = Array(0).concat(o);
-            let s = h => h instanceof HTMLSelectElement && h.name && h.form === e.element,
-                u = Array.from(r.getElementsByTagName("SELECT")).filter(s).at(0);
-            u instanceof HTMLSelectElement && (u.addEventListener("focus", () => this.touch()), u.addEventListener("change", () => {
+            let s = g => g instanceof HTMLSelectElement && g.name && g.form === e.element,
+                d = Array.from(r.getElementsByTagName("SELECT")).filter(s).at(0);
+            d instanceof HTMLSelectElement && (d.addEventListener("focus", () => this.touch()), d.addEventListener("change", () => {
                 this.setDirty(), this.clearCustomError(), this.validate()
-            }), this.fieldElements.push(u));
-            let f = h => h instanceof HTMLTextAreaElement && h.name && h.form === e.element,
-                d = Array.from(r.getElementsByTagName("TEXTAREA")).filter(f).at(0);
-            d instanceof HTMLTextAreaElement && (d.addEventListener("focus", () => this.touch()), d.addEventListener("input", () => this.inputted()), d.addEventListener("blur", () => this.validate()), this.fieldElements.push(d)), this.name = this.assertUniqueName(), this.initialDisabled = this.fieldElements.map(h => h.disabled), n ? this.validateCheckboxSelectMultiple() : this.validateBoundField(), this.pristineValue = new Nt(this.aggregateValue()), this.updateVisibility = this.evalVisibility("show-if", !0) ?? this.evalVisibility("hide-if", !1) ?? function() {}, this.updateDisabled = this.evalDisable(), this.untouch(), this.setPristine()
+            }), this.fieldElements.push(d));
+            let f = g => g instanceof HTMLTextAreaElement && g.name && g.form === e.element,
+                c = Array.from(r.getElementsByTagName("TEXTAREA")).filter(f).at(0);
+            c instanceof HTMLTextAreaElement && (c.addEventListener("focus", () => this.touch()), c.addEventListener("input", () => this.inputted()), c.addEventListener("blur", () => this.validate()), this.fieldElements.push(c)), this.name = this.assertUniqueName(), this.initialDisabled = this.fieldElements.map(g => g.disabled), this.initialRequired = this.fieldElements.map(g => g.required), n ? this.validateCheckboxSelectMultiple() : this.validateBoundField(), this.pristineValue = new or(this.aggregateValue()), this.updateVisibility = this.evalVisibility("df-show", !0) ?? this.evalVisibility("df-hide", !1) ?? function() {}, this.updateDisabled = this.evalDisable(), this.untouch(), this.setPristine()
         }
         aggregateValue() {
             var e, r;
             if (this.fieldElements.length === 1) {
                 let n = this.fieldElements[0];
                 if (n.type === "checkbox") return n.checked ? n.value : "";
                 if (n.type === "select-multiple") {
@@ -2308,14 +2478,20 @@
                     else if (i.type === "radio" && i.checked) return i.value;
                 return n
             }
         }
         updateOperability() {
             this.updateVisibility(), this.updateDisabled()
         }
+        disableRequiredConstraint() {
+            this.fieldElements.forEach(e => e.required = !1)
+        }
+        restoreRequiredConstraint() {
+            this.fieldElements.forEach((e, r) => e.required = this.initialRequired[r])
+        }
         assertUniqueName() {
             let e = "__undefined__";
             for (let r of this.fieldElements)
                 if (e === "__undefined__") e = r.name;
                 else if (e !== r.name) throw new Error(`Duplicate name '${e}' on multiple input fields on '${r.name}'`);
             return e
         }
@@ -2324,46 +2500,46 @@
 
             function n(s) {
                 return Array.isArray(s) ? s.length !== 0 : !!s
             }
             let i = (o = this.fieldElements[0]) == null ? void 0 : o.getAttribute(e);
             if (typeof i != "string") return null;
             try {
-                let s = new Function("return " + ye(i, {
+                let s = new Function("return " + ke(i, {
                     startRule: "Expression"
                 }));
                 return () => {
-                    let u = r != n(s.call(this));
-                    this.element.hasAttribute("hidden") !== u && (this.fieldElements.forEach((f, d) => f.disabled = u || this.initialDisabled[d]), this.element.toggleAttribute("hidden", u))
+                    let d = r != n(s.call(this));
+                    this.element.hasAttribute("hidden") !== d && (this.fieldElements.forEach((f, c) => f.disabled = d || this.initialDisabled[c]), this.element.toggleAttribute("hidden", d))
                 }
             } catch (s) {
-                throw new Error(`Error while parsing <... show-if/hide-if="${i}">: ${s}.`)
+                throw new Error(`Error while parsing <... df-show/hide="${i}">: ${s}.`)
             }
         }
         evalDisable() {
             var r;
-            let e = (r = this.fieldElements[0]) == null ? void 0 : r.getAttribute("disable-if");
+            let e = (r = this.fieldElements[0]) == null ? void 0 : r.getAttribute("df-disable");
             if (typeof e != "string") return () => {};
             try {
-                let n = new Function("return " + ye(e, {
+                let n = new Function("return " + ke(e, {
                     startRule: "Expression"
                 }));
                 return () => {
                     let i = n.call(this);
                     this.fieldElements.forEach((o, s) => o.disabled = i || this.initialDisabled[s])
                 }
             } catch (n) {
-                throw new Error(`Error while parsing <... disable-if="${e}">: ${n}.`)
+                throw new Error(`Error while parsing <... df-disable="${e}">: ${n}.`)
             }
         }
         getDataValue(e) {
             return this.form.getDataValue(e)
         }
         inputted() {
-            (0, Tn.default)(this.pristineValue, this.aggregateValue()) ? this.setPristine(): this.setDirty(), this.clearCustomError()
+            (0, ro.default)(this.pristineValue, this.aggregateValue()) ? this.setPristine(): this.setDirty(), this.clearCustomError(), this.form.restoreRequiredConstraints()
         }
         clearCustomError() {
             this.form.clearCustomErrors(), this.errorPlaceholder && (this.errorPlaceholder.innerHTML = "");
             for (let e of this.fieldElements) e.validity.customError && e.setCustomValidity("")
         }
         resetToInitial() {
             var e;
@@ -2383,14 +2559,17 @@
         }
         setDirty() {
             this.element.classList.remove("dj-submitted", "dj-pristine"), this.element.classList.add("dj-dirty")
         }
         setPristine() {
             this.element.classList.remove("dj-dirty"), this.element.classList.add("dj-pristine")
         }
+        isPristine() {
+            return this.element.classList.contains("dj-pristine")
+        }
         setSubmitted() {
             this.element.classList.add("dj-submitted")
         }
         validate() {
             let e = null;
             for (e of this.fieldElements)
                 if (!e.validity.valid) break;
@@ -2440,33 +2619,33 @@
         reportCustomError(e) {
             this.errorPlaceholder && (this.errorPlaceholder.innerHTML = e), this.fieldElements[0].setCustomValidity(e)
         }
         reportFailedUpload() {
             this.errorPlaceholder && (this.errorPlaceholder.innerHTML = this.errorMessages.get("badInput") ?? "File upload failed")
         }
     },
-    ct = class {
+    vt = class {
         constructor(e, r) {
             this.func = e, this.args = r
         }
     },
-    qt = class {
+    sr = class {
         constructor(e, r) {
             this.successActions = Array(0);
             this.rejectActions = Array(0);
             this.clicked = () => {
                 let e;
                 for (let [r, n] of this.successActions.entries()) e ? e = e.then(n.func.apply(this, n.args)) : e = n.func.apply(this, n.args)();
                 if (e) {
                     for (let [r, n] of this.rejectActions.entries()) r === 0 ? e = e.catch(n.func.apply(this, n.args)) : e = e.then(n.func.apply(this, n.args));
                     e.finally(this.restore.apply(this))
                 }
             };
             var n;
-            this.formset = e, this.element = r, this.initialClass = r.getAttribute("class") ?? "", this.isAutoDisabled = !!JSON.parse((r.getAttribute("auto-disable") ?? "false").toLowerCase()), this.decoratorElement = r.querySelector(".dj-button-decorator"), this.originalDecorator = (n = this.decoratorElement) == null ? void 0 : n.cloneNode(!0), this.spinnerElement = document.createElement("i"), this.spinnerElement.classList.add("dj-icon", "dj-spinner"), this.spinnerElement.innerHTML = En, this.okayElement = document.createElement("i"), this.okayElement.classList.add("dj-icon", "dj-okay"), this.okayElement.innerHTML = wn, this.bummerElement = document.createElement("i"), this.bummerElement.classList.add("dj-icon", "dj-bummer"), this.bummerElement.innerHTML = kn, this.parseActionsQueue(r.getAttribute("click")), r.addEventListener("click", this.clicked)
+            this.formset = e, this.element = r, this.initialClass = r.getAttribute("class") ?? "", this.isAutoDisabled = !!JSON.parse((r.getAttribute("auto-disable") ?? "false").toLowerCase()), this.decoratorElement = r.querySelector(".dj-button-decorator"), this.originalDecorator = (n = this.decoratorElement) == null ? void 0 : n.cloneNode(!0), this.spinnerElement = document.createElement("i"), this.spinnerElement.classList.add("dj-icon", "dj-spinner"), this.spinnerElement.innerHTML = Yn, this.okayElement = document.createElement("i"), this.okayElement.classList.add("dj-icon", "dj-okay"), this.okayElement.innerHTML = Qn, this.bummerElement = document.createElement("i"), this.bummerElement.classList.add("dj-icon", "dj-bummer"), this.bummerElement.innerHTML = eo, this.parseActionsQueue(r.getAttribute("df-click")), r.addEventListener("click", this.clicked)
         }
         autoDisable(e) {
             this.isAutoDisabled && (this.element.disabled = !e)
         }
         disable() {
             return e => (this.element.disabled = !0, Promise.resolve(e))
         }
@@ -2575,74 +2754,74 @@
         }
         parseActionsQueue(e) {
             if (!e) return;
             let r = (n, i) => {
                 for (let o of i) {
                     let s = this[o.funcname];
                     if (typeof s != "function") throw new Error(`Unknown function '${o.funcname}'.`);
-                    n.push(new ct(s, o.args))
+                    n.push(new vt(s, o.args))
                 }
-                n.length === 0 && n.push(new ct(this.noop, []))
+                n.length === 0 && n.push(new vt(this.noop, []))
             };
             try {
-                let n = ye(e, {
+                let n = ke(e, {
                     startRule: "Actions"
                 });
                 r(this.successActions, n.successChain), r(this.rejectActions, n.rejectChain)
             } catch (n) {
-                throw new Error(`Error while parsing <button click="${e}">: ${n}.`)
+                throw new Error(`Error while parsing <button df-click="${e}">: ${n}.`)
             }
         }
         restoreToInitial() {
             var e;
             this.element.disabled = !1, this.element.setAttribute("class", this.initialClass), this.originalDecorator && ((e = this.decoratorElement) == null || e.replaceChildren(...this.originalDecorator.cloneNode(!0).childNodes))
         }
         abortAction() {
             this.timeoutHandler && (clearTimeout(this.timeoutHandler), this.timeoutHandler = void 0)
         }
     },
-    zt = class {
+    lr = class {
         constructor(e, r) {
-            this.form = e, this.element = r, this.updateVisibility = this.evalVisibility("show-if", !0) ?? this.evalVisibility("hide-if", !1) ?? function() {}, this.updateDisabled = this.evalDisable()
+            this.form = e, this.element = r, this.updateVisibility = this.evalVisibility("df-show", !0) ?? this.evalVisibility("df-hide", !1) ?? function() {}, this.updateDisabled = this.evalDisable()
         }
         evalVisibility(e, r) {
             let n = this.element.getAttribute(e);
             if (n === null) return null;
             try {
-                let i = new Function("return " + ye(n, {
+                let i = new Function("return " + ke(n, {
                     startRule: "Expression"
                 }));
                 return () => {
                     let o = r != !!i.call(this);
                     this.element.hasAttribute("hidden") !== o && this.element.toggleAttribute("hidden", o)
                 }
             } catch (i) {
-                throw new Error(`Error while parsing <fieldset show-if/hide-if="${n}">: ${i}.`)
+                throw new Error(`Error while parsing <fieldset df-show/hide="${n}">: ${i}.`)
             }
         }
         evalDisable() {
-            let e = this.element.getAttribute("disable-if");
+            let e = this.element.getAttribute("df-disable");
             if (typeof e != "string") return () => {};
             try {
-                let r = new Function("return " + ye(e, {
+                let r = new Function("return " + ke(e, {
                     startRule: "Expression"
                 }));
                 return () => this.element.disabled = r.call(this)
             } catch (r) {
-                throw new Error(`Error while parsing <fieldset disable-if="${e}">: ${r}.`)
+                throw new Error(`Error while parsing <fieldset df-disable="${e}">: ${r}.`)
             }
         }
         getDataValue(e) {
             return this.form.getDataValue(e)
         }
         updateOperability() {
             this.updateVisibility(), this.updateDisabled()
         }
     },
-    Ut = class {
+    dr = class {
         constructor(e, r) {
             this.errorList = null;
             this.errorPlaceholder = null;
             this.fieldGroups = Array(0);
             this.hiddenInputFields = Array(0);
             this.markedForRemoval = !1;
             this.handleSubmit = e => {
@@ -2650,15 +2829,15 @@
             };
             this.handleReset = () => {
                 for (let e of this.fieldGroups) e.resetToInitial()
             };
             var o, s;
             this.formset = e, this.element = r, this.path = ((o = this.name) == null ? void 0 : o.split(".")) ?? [];
             let n = r.nextSibling;
-            this.fieldset = n instanceof HTMLFieldSetElement && n.form === r ? new zt(this, n) : null;
+            this.fieldset = n instanceof HTMLFieldSetElement && n.form === r ? new lr(this, n) : null;
             let i = (s = r.nextElementSibling) == null ? void 0 : s.querySelector(".dj-form-errors > .dj-errorlist > .dj-placeholder");
             i && (this.errorList = i.parentElement, this.errorPlaceholder = this.errorList.removeChild(i)), this.element.addEventListener("submit", this.handleSubmit), this.element.addEventListener("reset", this.handleReset)
         }
         aggregateValues() {
             let e = new Map;
             for (let r of this.fieldGroups) e.set(r.name, r.aggregateValue());
             for (let r of this.hiddenInputFields.filter(n => n.type === "hidden")) e.set(r.name, r.value);
@@ -2713,15 +2892,15 @@
         }
         toggleForRemoval(e) {
             this.markedForRemoval = e;
             for (let r of this.fieldGroups) e ? (r.resetToInitial(), r.disableAllFields()) : r.reenableAllFields()
         }
         reportCustomErrors(e) {
             this.clearCustomErrors();
-            let r = e.get(xs);
+            let r = e.get(Ml);
             if (this.errorList && r instanceof Array && this.errorPlaceholder)
                 for (let n of r) {
                     let i = this.errorPlaceholder.cloneNode();
                     i.innerHTML = n, this.errorList.appendChild(i)
                 }
             for (let n of this.fieldGroups) {
                 let i = e.get(n.name);
@@ -2731,26 +2910,35 @@
         findFirstErrorReport() {
             var e, r;
             if ((e = this.errorList) != null && e.textContent) return this.element;
             for (let n of this.fieldGroups)
                 if ((r = n.errorPlaceholder) != null && r.textContent) return n.element;
             return null
         }
+        isPristine() {
+            return this.fieldGroups.every(e => e.isPristine())
+        }
+        disableRequiredConstraints() {
+            this.fieldGroups.forEach(e => e.disableRequiredConstraint())
+        }
+        restoreRequiredConstraints() {
+            this.fieldGroups.forEach(e => e.restoreRequiredConstraint())
+        }
     },
     J = class {
-        constructor(e, r, n, i) {
+        constructor(e, r, n) {
             this.forms = Array(0);
             this.children = Array(0);
             this.markedForRemoval = !1;
             this.formset = e, this.element = r, this.parent = n, this.findFormCollections()
         }
         findFormCollections() {
             for (let e of J.getChildCollections(this.element)) this.children.push(e.hasAttribute("sibling-position") ? new z(this.formset, e, this) : new J(this.formset, e, this));
             for (let e of this.children) e.updateRemoveButtonAttrs();
-            this.formCollectionTemplate = Ee.findFormCollectionTemplate(this.formset, this.element, this)
+            this.formCollectionTemplate = Ce.findFormCollectionTemplate(this.formset, this.element, this)
         }
         assignForms(e) {
             this.forms = e.filter(r => {
                 var n;
                 return (n = r.element.parentElement) == null ? void 0 : n.isEqualNode(this.element)
             });
             for (let r of this.children) r.assignForms(e)
@@ -2776,14 +2964,26 @@
         }
         repositionSiblings() {}
         repositionForms(e, r) {
             this.forms.forEach(n => {
                 n.path[e] = String(r), n.element.setAttribute("name", n.path.join("."))
             }), this.children.forEach(n => n.repositionForms(e, r))
         }
+        markAsFreshAndEmpty(e) {
+            this.children.forEach(r => r.markAsFreshAndEmpty(e)), e && this.forms.forEach(r => r.disableRequiredConstraints())
+        }
+        restoreRequiredConstraint() {
+            this.forms.forEach(e => e.restoreRequiredConstraints()), this.children.forEach(e => e.restoreRequiredConstraint())
+        }
+        isFreshAndEmpty() {
+            return this.forms.every(e => e.isPristine()) && this.children.every(e => e.isFreshAndEmpty())
+        }
+        removeFreshAndEmpty() {
+            Array.from(this.children).reverse().forEach(r => r.removeFreshAndEmpty())
+        }
         static getChildCollections(e) {
             var n;
             let r = (n = e.querySelector("django-form-collection")) == null ? void 0 : n.parentElement;
             return r ? r.querySelectorAll(":scope > django-form-collection") : []
         }
         static resetCollectionsToInitial(e) {
             var i;
@@ -2792,36 +2992,35 @@
             r.forEach(o => e.splice(e.indexOf(o), 1)), e.sort((o, s) => o instanceof z && s instanceof z ? o.initialPosition - s.initialPosition : 0);
             let n = null;
             for (let o of e) o instanceof z && (o.initialPosition === 0 ? (i = o.element.parentElement) == null || i.insertAdjacentElement("afterbegin", o.element) : n == null || n.insertAdjacentElement("afterend", o.element), n = o.element);
             e.forEach(o => o.repositionSiblings())
         }
     },
     z = class extends J {
-        constructor(r, n, i, o) {
+        constructor(r, n, i) {
             super(r, n, i);
             this.minSiblings = 0;
             this.maxSiblings = null;
             this.justAdded = !1;
             this.removeCollection = () => {
                 var i, o;
                 let r = ((i = this.parent) == null ? void 0 : i.children) ?? this.formset.formCollections;
                 this.justAdded ? (this.disconnect(), r.splice(r.indexOf(this), 1), this.repositionSiblings()) : (this.toggleForRemoval(!this.markedForRemoval), this.removeButton.disabled = !this.markedForRemoval), r.forEach(s => s.updateRemoveButtonAttrs()), (((o = this.parent) == null ? void 0 : o.formCollectionTemplate) ?? this.formset.formCollectionTemplate).updateAddButtonAttrs()
             };
-            this.justAdded = o ?? !1;
-            let s = n.getAttribute("sibling-position");
-            if (!s) throw new Error("Missing argument 'sibling-position' in <django-form-collection>");
-            this.position = this.initialPosition = parseInt(s);
-            let u = n.getAttribute("min-siblings");
-            if (!u) throw new Error("Missing argument 'min-siblings' in <django-form-collection>");
-            this.minSiblings = parseInt(u);
-            let f = n.getAttribute("max-siblings");
-            f && (this.maxSiblings = parseInt(f));
-            let d = n.querySelector(":scope > button.remove-collection");
-            if (!d) throw new Error('<django-form-collection> with siblings requires child element <button class="remove-collection">');
-            this.removeButton = d, this.removeButton.addEventListener("click", this.removeCollection)
+            let o = n.getAttribute("sibling-position");
+            if (!o) throw new Error("Missing argument 'sibling-position' in <django-form-collection>");
+            this.position = this.initialPosition = parseInt(o);
+            let s = n.getAttribute("min-siblings");
+            if (!s) throw new Error("Missing argument 'min-siblings' in <django-form-collection>");
+            this.minSiblings = parseInt(s);
+            let d = n.getAttribute("max-siblings");
+            d && (this.maxSiblings = parseInt(d));
+            let f = n.querySelector(":scope > button.remove-collection");
+            if (!f) throw new Error('<django-form-collection> with siblings requires child element <button class="remove-collection">');
+            this.removeButton = f, this.removeButton.addEventListener("click", this.removeCollection)
         }
         disconnect() {
             this.removeButton.removeEventListener("click", this.removeCollection), super.disconnect()
         }
         repositionSiblings() {
             var n;
             (((n = this.parent) == null ? void 0 : n.children) ?? this.formset.formCollections).forEach((i, o) => {
@@ -2830,58 +3029,68 @@
         }
         updateRemoveButtonAttrs() {
             var i;
             if (!this.removeButton) return;
             let n = (((i = this.parent) == null ? void 0 : i.children) ?? this.formset.formCollections).filter(o => !o.markedForRemoval).length;
             this.markedForRemoval ? this.maxSiblings ? this.removeButton.disabled = n >= this.maxSiblings : this.removeButton.disabled = !1 : this.removeButton.disabled = n <= this.minSiblings
         }
+        markAsFreshAndEmpty(r) {
+            this.justAdded = r || this.element.hasAttribute("fresh-and-empty"), super.markAsFreshAndEmpty(this.justAdded)
+        }
+        isFreshAndEmpty() {
+            return this.justAdded && super.isFreshAndEmpty()
+        }
+        removeFreshAndEmpty() {
+            !this.removeButton.disabled && this.isFreshAndEmpty() ? this.removeCollection() : super.removeFreshAndEmpty()
+        }
         resetToInitial() {
             return this.justAdded ? (this.disconnect(), !0) : (super.resetToInitial(), !1)
         }
     },
-    Ee = class {
+    Ce = class {
         constructor(e, r, n) {
             this.maxSiblings = null;
             this.baseContext = new Map;
             this.markedForRemoval = !1;
             this.resortSiblings = e => {
                 var o;
                 let r = e.oldDraggableIndex ?? NaN,
                     n = e.newDraggableIndex ?? NaN;
                 if (!isFinite(r) || !isFinite(n) || r === n) return;
                 let i = ((o = this.parent) == null ? void 0 : o.children) ?? this.formset.formCollections;
                 if (i.at(r) instanceof z) {
                     let s = i.splice(r, 1);
                     i.splice(n, 0, ...s), s.at(0).repositionSiblings();
-                    let u = this.prefix === "0" ? 0 : this.prefix.split(".").length;
-                    i.forEach((f, d) => f.repositionForms(u, d)), this.formset.validate()
+                    let d = this.prefix === "0" ? 0 : this.prefix.split(".").length;
+                    i.forEach((f, c) => f.repositionForms(d, c)), this.formset.validate()
                 }
             };
             this.appendFormCollectionSibling = () => {
-                var o;
+                var s;
                 let e = Object.fromEntries(this.baseContext);
                 e.position = (this.getHighestPosition() + 1).toString(), e.position_1 = "${position}";
-                for (let s = 1; s < 10; ++s) e[`position_${s+1}`] = `\${position_${s}}`;
+                for (let d = 1; d < 10; ++d) e[`position_${d+1}`] = `\${position_${d}}`;
                 let r = this.renderEmptyCollection(e);
                 this.element.insertAdjacentHTML("beforebegin", r);
                 let n = this.element.previousElementSibling;
                 if (!(n instanceof HTMLElement)) throw new Error("Unable to insert empty <django-form-collection> element.");
-                let i = ((o = this.parent) == null ? void 0 : o.children) ?? this.formset.formCollections;
-                i.push(new z(this.formset, n, this.parent, !0)), this.formset.findForms(n), this.formset.assignFieldsToForms(n), this.formset.assignFormsToCollections(), this.formset.validate(), i.forEach(s => s.updateRemoveButtonAttrs()), this.updateAddButtonAttrs()
+                let i = ((s = this.parent) == null ? void 0 : s.children) ?? this.formset.formCollections,
+                    o = new z(this.formset, n, this.parent);
+                i.push(o), this.formset.findForms(n), this.formset.assignFieldsToForms(n), this.formset.assignFormsToCollections(), this.formset.findCollectionErrorsList(), o.markAsFreshAndEmpty(!0), this.formset.validate(), i.forEach(d => d.updateRemoveButtonAttrs()), this.updateAddButtonAttrs()
             };
             var f;
             this.formset = e, this.element = r, this.parent = n;
             let i = r.innerHTML.matchAll(/\$\{([^} ]+)\}/g);
-            for (let d of i) this.baseContext.set(d[1], d[0]);
+            for (let c of i) this.baseContext.set(c[1], c[0]);
             let o = r.getAttribute("prefix");
             if (!o) throw new Error('<template class="empty-collection" ...> requires attribute "prefix"');
-            this.prefix = o, e.pushTemplatePrefix(this.prefix), this.renderEmptyCollection = (0, _n.default)(r.innerHTML), (f = r.nextElementSibling) != null && f.matches("button.add-collection") && (this.addButton = r.nextElementSibling, this.addButton.addEventListener("click", this.appendFormCollectionSibling));
+            this.prefix = o, e.pushTemplatePrefix(this.prefix), this.renderEmptyCollection = (0, oo.default)(r.innerHTML), (f = r.nextElementSibling) != null && f.matches("button.add-collection") && (this.addButton = r.nextElementSibling, this.addButton.addEventListener("click", this.appendFormCollectionSibling));
             let s = this.element.content.querySelector("django-form-collection"),
-                u = s == null ? void 0 : s.getAttribute("max-siblings");
-            u && (this.maxSiblings = parseInt(u)), r.hasAttribute("sortable") && new lr(r.parentElement, {
+                d = s == null ? void 0 : s.getAttribute("max-siblings");
+            d && (this.maxSiblings = parseInt(d)), r.hasAttribute("sortable") && new Ar(r.parentElement, {
                 animation: 150,
                 handle: "django-form-collection[sibling-position]:not(.dj-marked-for-removal) > .collection-drag-handle",
                 draggable: "django-form-collection[sibling-position]",
                 selectedClass: "selected",
                 ghostClass: "dj-ghost-collection",
                 onEnd: this.resortSiblings
             })
@@ -2905,32 +3114,32 @@
             }
             let r = (((n = this.parent) == null ? void 0 : n.children) ?? this.formset.formCollections).filter(i => !i.markedForRemoval).length;
             this.addButton.disabled = this.maxSiblings === null ? !1 : r >= this.maxSiblings
         }
         static findFormCollectionTemplate(e, r, n) {
             let i = r.querySelector(":scope > .collection-siblings > template.empty-collection");
             if (i) {
-                let o = new Ee(e, i, n);
+                let o = new Ce(e, i, n);
                 return o.updateAddButtonAttrs(), o
             }
         }
     },
-    Kt = class {
+    cr = class {
         constructor(e) {
             this.buttons = Array(0);
             this.forms = Array(0);
             this.formCollections = Array(0);
             this.collectionErrorsList = new Map;
             this.abortController = new AbortController;
             this.emptyCollectionPrefixes = Array(0);
             this.data = {};
             this.element = e, this.showFeedbackMessages = this.parseWithholdFeedback(), this.CSRFToken = this.element.getAttribute("csrf-token")
         }
         connectedCallback() {
-            this.findButtons(), this.findForms(), this.findFormCollections(), this.findCollectionErrorsList(), this.assignFieldsToForms(), this.assignFormsToCollections(), window.setTimeout(() => this.validate(), 0)
+            this.findButtons(), this.findForms(), this.findFormCollections(), this.findCollectionErrorsList(), this.assignFieldsToForms(), this.assignFormsToCollections(), this.formCollections.forEach(e => e.markAsFreshAndEmpty()), window.setTimeout(() => this.validate(), 0)
         }
         get endpoint() {
             return this.element.getAttribute("endpoint") ?? ""
         }
         get forceSubmission() {
             return this.element.hasAttribute("force-submission")
         }
@@ -2965,26 +3174,26 @@
             r >= 0 && this.emptyCollectionPrefixes.splice(r, 1)
         }
         assignFieldsToForms(e) {
             e = e ?? this.element;
             for (let r of e.querySelectorAll("INPUT, SELECT, TEXTAREA")) {
                 let n = r.getAttribute("form");
                 if (!n) continue;
-                let i = this.forms.filter(u => u.formId && u.formId === n);
+                let i = this.forms.filter(d => d.formId && d.formId === n);
                 if (i.length < 1) continue;
                 if (i.length > 1) throw new Error(`More than one form has id="${n}"`);
                 let o = i[0],
                     s = r.closest('[role="group"]');
-                s ? o.fieldGroups.filter(u => u.element === s).length === 0 && o.fieldGroups.push(new Gt(o, s)) : r instanceof HTMLInputElement && r.type === "hidden" && (o.hiddenInputFields.includes(r) || o.hiddenInputFields.push(r))
+                s ? o.fieldGroups.filter(d => d.element === s).length === 0 && o.fieldGroups.push(new ar(o, s)) : r instanceof HTMLInputElement && r.type === "hidden" && (o.hiddenInputFields.includes(r) || o.hiddenInputFields.push(r))
             }
         }
         findForms(e) {
             e = e ?? this.element;
             for (let r of e.getElementsByTagName("FORM")) {
-                let n = new Ut(this, r);
+                let n = new dr(this, r);
                 this.forms.push(n)
             }
             this.checkForUniqueness()
         }
         checkForUniqueness() {
             let e = this.forms.filter(n => n.provideData);
             if (e.length === 1) return;
@@ -2993,36 +3202,40 @@
                 if (!n.name) throw new Error("Multiple <form>-elements in a <django-formset> require a unique name each.");
                 if (n.name in r) throw new Error(`Duplicate name "${n.name}" used in multiple forms of same <django-formset>.`);
                 r.push(n.name)
             })
         }
         findFormCollections() {
             for (let e of J.getChildCollections(this.element)) this.formCollections.push(e.hasAttribute("sibling-position") ? new z(this, e) : new J(this, e));
-            this.formCollections.forEach(e => e.updateRemoveButtonAttrs()), this.formCollectionTemplate = Ee.findFormCollectionTemplate(this, this.element)
+            this.formCollections.forEach(e => e.updateRemoveButtonAttrs()), this.formCollectionTemplate = Ce.findFormCollectionTemplate(this, this.element)
         }
         findCollectionErrorsList() {
+            this.collectionErrorsList.clear();
             for (let e of this.element.getElementsByClassName("dj-collection-errors")) {
                 let r = e.getAttribute("prefix") ?? "",
                     n = e.querySelector("ul.dj-errorlist");
                 this.collectionErrorsList.set(r, n)
             }
         }
         findButtons() {
             this.buttons.length = 0;
-            for (let e of this.element.getElementsByTagName("BUTTON")) e.hasAttribute("click") && this.buttons.push(new qt(this, e))
+            for (let e of this.element.getElementsByTagName("BUTTON")) e.hasAttribute("df-click") && this.buttons.push(new sr(this, e))
         }
         assignFormsToCollections() {
-            for (let e of this.formCollections) e.assignForms(this.forms)
+            this.formCollections.forEach(e => e.assignForms(this.forms))
         }
         removeForm(e) {
             this.forms.splice(this.forms.indexOf(e), 1)
         }
+        removeFreshCollections() {
+            Array.from(this.formCollections).reverse().forEach(r => r.removeFreshAndEmpty())
+        }
         aggregateValues() {
             this.data = {};
-            for (let e of this.forms) e.provideData && (0, An.default)(this.data, e.getAbsPath(), Object.fromEntries(e.aggregateValues()));
+            for (let e of this.forms) e.provideData && (0, to.default)(this.data, e.getAbsPath(), Object.fromEntries(e.aggregateValues()));
             for (let e of this.forms) e.markedForRemoval || e.updateOperability()
         }
         validate() {
             let e = !0;
             for (let r of this.forms) e = (r.markedForRemoval || r.checkValidity()) && e;
             for (let r of this.buttons) r.autoDisable(e);
             return this.aggregateValues(), e
@@ -3032,226 +3245,227 @@
 
             function n(o, s) {
                 if (s.length === 1) {
                     Array.isArray(o) ? r && !o.includes(r) && o.push(r) : o[s[0]] = r ?? [];
                     return
                 }
                 if (isNaN(parseInt(s[1]))) {
-                    let u = o[s[0]] ?? {};
-                    n(u, s.slice(1));
+                    let d = o[s[0]] ?? {};
+                    n(d, s.slice(1));
                     let f = parseInt(s[0]);
-                    isNaN(f) ? o[s[0]] = u : o[f] = {
+                    isNaN(f) ? o[s[0]] = d : o[f] = {
                         ...o[f],
-                        ...u
+                        ...d
                     }
                 } else {
                     if (Array.isArray(o)) throw new Error("Invalid form structure: Contains nested arrays.");
-                    let u = o[s[0]] ?? [];
-                    if (!Array.isArray(u)) throw new Error("Invalid form structure: Inner array is missing.");
-                    n(u, s.slice(1)), o[s[0]] = u
+                    let d = o[s[0]] ?? [];
+                    if (!Array.isArray(d)) throw new Error("Invalid form structure: Inner array is missing.");
+                    n(d, s.slice(1)), o[s[0]] = d
                 }
             }
             let i = {};
             for (let o of this.emptyCollectionPrefixes) {
                 let s = ["formset_data", ...o.split(".")];
-                r = (0, xe.default)(i, s), n(i, s)
+                r = (0, Te.default)(i, s), n(i, s)
             }
             for (let o of this.forms) {
                 if (!o.name) return Object.assign({}, this.data, {
                     _extra: e
                 });
                 let s = o.getAbsPath();
-                r = (0, xe.default)(this.data, s), o.markedForRemoval && (r[ws] = !0), n(i, s)
+                r = (0, Te.default)(this.data, s), o.markedForRemoval && (r[Pl] = !0), n(i, s)
             }
             return Object.assign({}, i, {
                 _extra: e
             })
         }
         async submit(e) {
             let r = !0;
             if (this.setSubmitted(), !this.forceSubmission)
                 for (let n of this.forms) r = (n.markedForRemoval || n.isValid()) && r;
             if (r) {
                 if (!this.endpoint) throw new Error(`<django-formset> requires attribute 'endpoint="server endpoint"' for submission`);
+                this.removeFreshCollections();
                 let n = this.buildBody(e);
                 try {
                     let i = new Headers;
                     i.append("Accept", "application/json"), i.append("Content-Type", "application/json"), this.CSRFToken && i.append("X-CSRFToken", this.CSRFToken);
                     let o = await fetch(this.endpoint, {
                         method: "POST",
                         headers: i,
                         body: JSON.stringify(n),
                         signal: this.abortController.signal
                     });
                     switch (o.status) {
                         case 200:
                             this.clearErrors();
-                            for (let u of this.forms) u.element.dispatchEvent(new Event("submitted"));
+                            for (let d of this.forms) d.element.dispatchEvent(new Event("submitted"));
                             return o;
                         case 422:
                             this.clearErrors();
                             let s = await o.clone().json();
                             return this.reportErrors(s), o;
                         default:
-                            return console.warn(`Unknown response status: ${o.status}`), this.clearErrors(), this.buttons.forEach(u => u.restoreToInitial()), o
+                            return console.warn(`Unknown response status: ${o.status}`), this.clearErrors(), this.buttons.forEach(d => d.restoreToInitial()), o
                     }
                 } catch (i) {
                     this.clearErrors(), this.buttons.forEach(o => o.restoreToInitial()), alert(i)
                 }
             } else {
                 this.clearErrors();
                 for (let n of this.forms) n.reportValidity()
             }
         }
         reportErrors(e) {
             for (let r of this.forms) {
-                let n = r.name ? (0, xe.default)(e, r.name.split("."), null) : e;
-                n ? (r.reportCustomErrors(new Map(Object.entries(n))), r.reportValidity()) : r.clearCustomErrors()
+                let n = r.name ? (0, Te.default)(e, r.name.split("."), null) : e;
+                (0, no.default)(n) ? r.clearCustomErrors(): (r.reportCustomErrors(new Map(Object.entries(n))), r.reportValidity())
             }
             for (let [r, n] of this.collectionErrorsList) {
                 let i = r ? r.split(".") : [];
-                i = [...i, "0", Es];
-                for (let o of (0, xe.default)(e, i, [])) {
+                i = [...i, "0", Il];
+                for (let o of (0, Te.default)(e, i, [])) {
                     let s = document.createElement("li");
                     s.classList.add("dj-placeholder"), s.innerText = o, n.appendChild(s)
                 }
             }
         }
         resetToInitial() {
             var e;
-            J.resetCollectionsToInitial(this.formCollections), (e = this.formCollectionTemplate) == null || e.updateAddButtonAttrs(), this.forms.forEach(r => r.resetToInitial())
+            J.resetCollectionsToInitial(this.formCollections), (e = this.formCollectionTemplate) == null || e.updateAddButtonAttrs(), this.forms.forEach(r => r.resetToInitial()), this.validate()
         }
         abort() {
             for (let e of this.buttons) e.abortAction();
             this.abortController.abort()
         }
         setSubmitted() {
             for (let e of this.forms) e.setSubmitted()
         }
         getDataValue(e) {
             let r = ["formset_data", ...e];
-            return (0, xe.default)(this.data, r, null)
+            return (0, Te.default)(this.data, r, null)
         }
         findFirstErrorReport() {
             for (let e of this.forms) {
                 let r = e.findFirstErrorReport();
                 if (r) return r
             }
             return null
         }
         clearErrors() {
             for (let e of this.forms) e.clearCustomErrors();
             for (let e of this.collectionErrorsList.values())
                 for (; e.firstElementChild;) e.removeChild(e.firstElementChild)
         }
     },
-    je = Symbol("DjangoFormset"),
-    ut = class extends HTMLElement {
+    Ae = Symbol("DjangoFormset"),
+    jt = class extends HTMLElement {
         constructor() {
             super();
-            this[je] = new Kt(this)
+            this[Ae] = new cr(this)
         }
         static get observedAttributes() {
-            return ["endpoint", "withhold-messages", "force-submission"]
+            return ["endpoint", "withhold-feedback", "force-submission"]
         }
         connectedCallback() {
-            this[je].connectedCallback()
+            this[Ae].connectedCallback()
         }
         async submit(r) {
-            return this[je].submit(r)
+            return this[Ae].submit(r)
         }
         async abort() {
-            return this[je].abort()
+            return this[Ae].abort()
         }
         async reset() {
-            return this[je].resetToInitial()
+            return this[Ae].resetToInitial()
         }
     };
-je;
+Ae;
 window.addEventListener("DOMContentLoaded", t => {
-    let e = dr.convertPseudoClasses(),
+    let e = Tr.convertPseudoClasses(),
         r = Array();
 
-    function n(s, u, f, d = void 0) {
-        customElements.get(u) instanceof Function ? s() : (window.customElements.define(u, f, d), window.customElements.whenDefined(u).then(() => s()))
+    function n(s, d, f, c = void 0) {
+        customElements.get(d) instanceof Function ? s() : (window.customElements.define(d, f, c), window.customElements.whenDefined(d).then(() => s()))
     }
 
     function i(s) {
-        s.querySelector('select[is="django-selectize"]') && r.push(new Promise((u, f) => {
-            import("./DjangoSelectize-W4FTVNOW.js").then(({
-                DjangoSelectizeElement: d
+        s.querySelector('select[is="django-selectize"]') && r.push(new Promise((d, f) => {
+            import("./DjangoSelectize-2WEWGVUV.js").then(({
+                DjangoSelectizeElement: c
             }) => {
-                n(u, "django-selectize", d, {
+                n(d, "django-selectize", c, {
                     extends: "select"
                 })
-            }).catch(d => f(d))
-        })), s.querySelector("django-sortable-select") ? r.push(new Promise((u, f) => {
-            import("./SortableSelect-MAAIASIY.js").then(({
-                SortableSelectElement: d
+            }).catch(c => f(c))
+        })), s.querySelector("django-sortable-select") ? r.push(new Promise((d, f) => {
+            import("./SortableSelect-XJMQCTYG.js").then(({
+                SortableSelectElement: c
             }) => {
-                customElements.get("django-sortable-select") instanceof Function ? u() : window.customElements.define("django-sortable-select", d), import("./DualSelector-ZVBIRYKG.js").then(({
-                    DualSelectorElement: h
+                customElements.get("django-sortable-select") instanceof Function ? d() : window.customElements.define("django-sortable-select", c), import("./DualSelector-WBPG3AWC.js").then(({
+                    DualSelectorElement: g
                 }) => {
-                    customElements.get("django-dual-selector") instanceof Function ? u() : (window.customElements.define("django-dual-selector", h, {
+                    customElements.get("django-dual-selector") instanceof Function ? d() : (window.customElements.define("django-dual-selector", g, {
                         extends: "select"
-                    }), Promise.all([window.customElements.whenDefined("django-sortable-select"), window.customElements.whenDefined("django-dual-selector")]).then(() => u()))
-                }).catch(h => f(h))
-            }).catch(d => f(d))
-        })) : s.querySelector('select[is="django-dual-selector"]') && r.push(new Promise((u, f) => {
-            import("./DualSelector-ZVBIRYKG.js").then(({
-                DualSelectorElement: d
+                    }), Promise.all([window.customElements.whenDefined("django-sortable-select"), window.customElements.whenDefined("django-dual-selector")]).then(() => d()))
+                }).catch(g => f(g))
+            }).catch(c => f(c))
+        })) : s.querySelector('select[is="django-dual-selector"]') && r.push(new Promise((d, f) => {
+            import("./DualSelector-WBPG3AWC.js").then(({
+                DualSelectorElement: c
             }) => {
-                n(u, "django-dual-selector", d, {
+                n(d, "django-dual-selector", c, {
                     extends: "select"
                 })
-            }).catch(d => f(d))
-        })), s.querySelector('textarea[is="django-richtext"]') && r.push(new Promise((u, f) => {
-            import("./RichtextArea-YV4E7SHM.js").then(({
-                RichTextAreaElement: d
+            }).catch(c => f(c))
+        })), s.querySelector('textarea[is="django-richtext"]') && r.push(new Promise((d, f) => {
+            import("./RichtextArea-XHFBZVPO.js").then(({
+                RichTextAreaElement: c
             }) => {
-                n(u, "django-richtext", d, {
+                n(d, "django-richtext", c, {
                     extends: "textarea"
                 })
-            }).catch(d => f(d))
-        })), s.querySelector('input[is="django-slug"]') && r.push(new Promise((u, f) => {
+            }).catch(c => f(c))
+        })), s.querySelector('input[is="django-slug"]') && r.push(new Promise((d, f) => {
             import("./DjangoSlug-226MVQ6E.js").then(({
-                DjangoSlugElement: d
+                DjangoSlugElement: c
             }) => {
-                n(u, "django-slug", d, {
+                n(d, "django-slug", c, {
                     extends: "input"
                 })
-            }).catch(d => f(d))
-        })), s.querySelector('input[is="django-datepicker"]') && r.push(new Promise((u, f) => {
-            import("./DateTimePicker-TF2GNHHS.js").then(({
-                DatePickerElement: d
+            }).catch(c => f(c))
+        })), s.querySelector('input[is="django-datepicker"]') && r.push(new Promise((d, f) => {
+            import("./DateTimePicker-UTHDUQQK.js").then(({
+                DatePickerElement: c
             }) => {
-                n(u, "django-datepicker", d, {
+                n(d, "django-datepicker", c, {
                     extends: "input"
                 })
-            }).catch(d => f(d))
-        })), s.querySelector('input[is="django-datetimepicker"]') && r.push(new Promise((u, f) => {
-            import("./DateTimePicker-TF2GNHHS.js").then(({
-                DateTimePickerElement: d
+            }).catch(c => f(c))
+        })), s.querySelector('input[is="django-datetimepicker"]') && r.push(new Promise((d, f) => {
+            import("./DateTimePicker-UTHDUQQK.js").then(({
+                DateTimePickerElement: c
             }) => {
-                n(u, "django-datetimepicker", d, {
+                n(d, "django-datetimepicker", c, {
                     extends: "input"
                 })
-            }).catch(d => f(d))
+            }).catch(c => f(c))
         }))
     }
     document.querySelectorAll("template.empty-collection").forEach(s => {
         s instanceof HTMLTemplateElement && s.content instanceof DocumentFragment && i(s.content)
     }), i(document);
     let o = new Set;
     document.querySelectorAll("django-formset [id]").forEach(s => {
-        let u = s.getAttribute("id");
-        if (o.has(u)) throw new Error(`There are at least two elements with attribute id="${u}"`);
-        o.add(u)
+        let d = s.getAttribute("id");
+        if (o.has(d)) throw new Error(`There are at least two elements with attribute id="${d}"`);
+        o.add(d)
     }), Promise.all(r).then(() => {
-        window.customElements.define("django-formset", ut), window.customElements.whenDefined("django-formset").then(() => {
+        window.customElements.define("django-formset", jt), window.customElements.whenDefined("django-formset").then(() => {
             e.remove()
         })
     }).catch(s => console.error(`Failed to initialize django-formset: ${s}`))
 });
 /*! Bundled license information:
 
 @ungap/custom-elements/index.js:
```

### Comparing `django-formset-1.0.dev5/formset/static/formset/scss/bootstrap5-extra.scss` & `django-formset-1.1/formset/static/formset/scss/bootstrap5-extra.scss`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/static/formset/scss/collections.scss` & `django-formset-1.1/formset/static/formset/scss/collections.scss`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/calendar/hours.html` & `django-formset-1.1/formset/templates/calendar/hours.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/calendar/months.html` & `django-formset-1.1/formset/templates/calendar/months.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/calendar/weeks.html` & `django-formset-1.1/formset/templates/calendar/weeks.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/calendar/years.html` & `django-formset-1.1/formset/templates/calendar/years.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/dual_selector.html` & `django-formset-1.1/formset/templates/formset/bootstrap/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/bootstrap/widgets/file.html` & `django-formset-1.1/formset/templates/formset/bootstrap/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/dual_selector.html` & `django-formset-1.1/formset/templates/formset/bulma/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/bulma/widgets/file.html` & `django-formset-1.1/formset/templates/formset/bulma/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_align.html` & `django-formset-1.1/formset/templates/formset/default/buttons/richtext_align.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_color.html` & `django-formset-1.1/formset/templates/formset/default/buttons/richtext_color.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/default/buttons/richtext_heading.html` & `django-formset-1.1/formset/templates/formset/default/buttons/richtext_heading.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/default/collection.html` & `django-formset-1.1/formset/templates/formset/default/collection.html`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 {% for holder in collection %}
 	{% if holder.is_single %}
 	<django-form-collection{% if css_classes %} class="{{ css_classes }}"{% endif %}>
 	{% elif holder.is_first %}
 		{% if holder.is_template %}
 	<template{% if collection.is_sortable %} sortable="true"{% endif %} prefix="{{ collection.prefix|default_if_none:0 }}" class="empty-collection">
 		{% endif %}
-	<django-form-collection sibling-position="{{ holder.position }}" min-siblings="{{ collection.min_siblings }}"{% if collection.max_siblings %} max-siblings="{{ collection.max_siblings }}"{% endif %}{% if css_classes %} class="{{ css_classes }}"{% endif %}>
+	<django-form-collection sibling-position="{{ holder.position }}" min-siblings="{{ collection.min_siblings }}"{% if collection.max_siblings %} max-siblings="{{ collection.max_siblings }}"{% endif %}{% if css_classes %} class="{{ css_classes }}"{% endif %}{% if holder.fresh_and_empty %} fresh-and-empty{% endif %}>
 		{% if collection.is_sortable %}
 	<div class="collection-drag-handle"></div>
 		{% endif %}
 	{% endif %}
 	{{ holder }}
 	{% if holder.is_single %}
 	</django-form-collection>
```

### Comparing `django-formset-1.0.dev5/formset/templates/formset/default/dialog_form.html` & `django-formset-1.1/formset/templates/formset/default/dialog_form.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/default/fieldset.html` & `django-formset-1.1/formset/templates/formset/default/fieldset.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% spaceless %}
 <form{% include "formset/form_attrs.html" %}></form>
-<fieldset form="{{ form_id }}"{% if css_classes %} class="{{ css_classes }}"{% endif %}{% if show_if %} show-if="{{ show_if }}"{% endif %}{% if hide_if %} hide-if="{{ hide_if }}"{% endif %}{% if disable_if %} disable-if="{{ disable_if }}"{% endif %}>
+<fieldset form="{{ form_id }}"{% if css_classes %} class="{{ css_classes }}"{% endif %}{% if show_condition %} df-show="{{ show_condition }}"{% endif %}{% if hide_condition %} df-hide="{{ hide_condition }}"{% endif %}{% if disable_condition %} df-disable="{{ disable_condition }}"{% endif %}>
 	{% if legend %}<legend>{{ legend }}</legend>{% endif %}
 	{% include "formset/non_field_errors.html" %}
 	{% for field in form %}
 		{% if field.is_hidden %}
 			{{ field }}
 		{% else %}
 			{% include "formset/default/field_group.html" %}
```

### Comparing `django-formset-1.0.dev5/formset/templates/formset/default/widgets/dual_selector.html` & `django-formset-1.1/formset/templates/formset/default/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/default/widgets/file.html` & `django-formset-1.1/formset/templates/formset/default/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/default/widgets/selectize.html` & `django-formset-1.1/formset/templates/formset/default/widgets/selectize.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/dual_selector.html` & `django-formset-1.1/formset/templates/formset/foundation/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/foundation/widgets/file.html` & `django-formset-1.1/formset/templates/formset/foundation/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/icons/blockquote.svg` & `django-formset-1.1/formset/templates/formset/icons/blockquote.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/icons/letters.svg` & `django-formset-1.1/formset/templates/formset/icons/letters.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/icons/placeholder.svg` & `django-formset-1.1/formset/templates/formset/icons/placeholder.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/icons/questionmark.svg` & `django-formset-1.1/formset/templates/formset/icons/questionmark.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/icons/subscript.svg` & `django-formset-1.1/formset/templates/formset/icons/subscript.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/icons/unlink.svg` & `django-formset-1.1/formset/templates/formset/icons/unlink.svg`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/dual_selector.html` & `django-formset-1.1/formset/templates/formset/tailwind/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/tailwind/widgets/file.html` & `django-formset-1.1/formset/templates/formset/tailwind/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templates/formset/uikit/widgets/file.html` & `django-formset-1.1/formset/templates/formset/uikit/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templatetags/formsetify.py` & `django-formset-1.1/formset/templatetags/formsetify.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/templatetags/richtext.py` & `django-formset-1.1/formset/templatetags/richtext.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/upload.py` & `django-formset-1.1/formset/upload.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/utils.py` & `django-formset-1.1/formset/utils.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/views.py` & `django-formset-1.1/formset/views.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/formset/widgets.py` & `django-formset-1.1/formset/widgets.py`

 * *Files identical despite different names*

### Comparing `django-formset-1.0.dev5/setup.py` & `django-formset-1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,18 @@
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
 ]
 
 setup(
     name='django-formset',
     version=__version__,
     description='Prevalidate Django Forms in the browser',
     author='Jacob Rief',
```

