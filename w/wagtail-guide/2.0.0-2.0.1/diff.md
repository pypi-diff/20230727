# Comparing `tmp/wagtail_guide-2.0.0.tar.gz` & `tmp/wagtail_guide-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_guide-2.0.0.tar", last modified: Sun Apr  2 16:47:56 2023, max compression
+gzip compressed data, was "wagtail_guide-2.0.1.tar", last modified: Thu Jul 27 09:51:46 2023, max compression
```

## Comparing `wagtail_guide-2.0.0.tar` & `wagtail_guide-2.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:56.073775 wagtail_guide-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-02 16:47:56.073775 wagtail_guide-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-02 16:47:56.073775 wagtail_guide-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:56.069775 wagtail_guide-2.0.0/wagtail_guide/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:56.069775 wagtail_guide-2.0.0/wagtail_guide/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/migrations/0002_alter_editorguide_sections_w30_usejsonfield.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:56.069775 wagtail_guide-2.0.0/wagtail_guide/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:56.069775 wagtail_guide-2.0.0/wagtail_guide/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/static/css/wagtailguide.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:56.069775 wagtail_guide-2.0.0/wagtail_guide/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:56.069775 wagtail_guide-2.0.0/wagtail_guide/templates/wagtail_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/templates/wagtail_guide/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:56.069775 wagtail_guide-2.0.0/wagtail_guide/templates/wagtail_guide/streamfield/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:56.073775 wagtail_guide-2.0.0/wagtail_guide/templates/wagtail_guide/streamfield/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/templates/wagtail_guide/streamfield/blocks/embed_block.html
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/templates/wagtail_guide/streamfield/blocks/heading_block.html
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/templates/wagtail_guide/streamfield/blocks/image_block.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/templates/wagtail_guide/streamfield/blocks/pull_quote_block.html
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/templates/wagtail_guide/streamfield/blocks/quote_block.html
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/templates/wagtail_guide/streamfield/blocks/video_block.html
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/templates/wagtail_guide/streamfield/stream_block.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:56.073775 wagtail_guide-2.0.0/wagtail_guide/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-02 16:47:53.000000 wagtail_guide-2.0.0/wagtail_guide/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:47:56.069775 wagtail_guide-2.0.0/wagtail_guide.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-02 16:47:56.000000 wagtail_guide-2.0.0/wagtail_guide.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-02 16:47:56.000000 wagtail_guide-2.0.0/wagtail_guide.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 16:47:56.000000 wagtail_guide-2.0.0/wagtail_guide.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-02 16:47:56.000000 wagtail_guide-2.0.0/wagtail_guide.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-02 16:47:56.000000 wagtail_guide-2.0.0/wagtail_guide.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:46.959938 wagtail_guide-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-27 09:51:46.959938 wagtail_guide-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-27 09:51:46.959938 wagtail_guide-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:46.955938 wagtail_guide-2.0.1/wagtail_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:46.955938 wagtail_guide-2.0.1/wagtail_guide/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/migrations/0002_alter_editorguide_sections_w30_usejsonfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:46.951938 wagtail_guide-2.0.1/wagtail_guide/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:46.955938 wagtail_guide-2.0.1/wagtail_guide/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/static/css/wagtailguide.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:46.951938 wagtail_guide-2.0.1/wagtail_guide/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:46.955938 wagtail_guide-2.0.1/wagtail_guide/templates/wagtail_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/templates/wagtail_guide/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:46.955938 wagtail_guide-2.0.1/wagtail_guide/templates/wagtail_guide/streamfield/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:46.955938 wagtail_guide-2.0.1/wagtail_guide/templates/wagtail_guide/streamfield/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/templates/wagtail_guide/streamfield/blocks/embed_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/templates/wagtail_guide/streamfield/blocks/heading_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/templates/wagtail_guide/streamfield/blocks/image_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/templates/wagtail_guide/streamfield/blocks/pull_quote_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/templates/wagtail_guide/streamfield/blocks/quote_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/templates/wagtail_guide/streamfield/blocks/video_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/templates/wagtail_guide/streamfield/stream_block.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:46.959938 wagtail_guide-2.0.1/wagtail_guide/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-27 09:51:43.000000 wagtail_guide-2.0.1/wagtail_guide/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:51:46.955938 wagtail_guide-2.0.1/wagtail_guide.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-27 09:51:46.000000 wagtail_guide-2.0.1/wagtail_guide.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-27 09:51:46.000000 wagtail_guide-2.0.1/wagtail_guide.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:51:46.000000 wagtail_guide-2.0.1/wagtail_guide.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-27 09:51:46.000000 wagtail_guide-2.0.1/wagtail_guide.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 09:51:46.000000 wagtail_guide-2.0.1/wagtail_guide.egg-info/top_level.txt
```

### Comparing `wagtail_guide-2.0.0/LICENSE` & `wagtail_guide-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_guide-2.0.0/PKG-INFO` & `wagtail_guide-2.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: wagtail_guide
-Version: 2.0.0
+Version: 2.0.1
 Summary: Adds functionality to add and edit a CMS guide page for editors.
 Home-page: https://github.com/kevinhowbrook/wagtailguide
 Author: Kevin Howbrook - Torchbox
 Author-email: kevin.howbrook@torchbox.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: lint
+Provides-Extra: testing
 License-File: LICENSE
 
 # Wagtail Guide
 
-![tests](https://github.com/kevinhowbrook/wagtailguide/workflows/Test/badge.svg) [![codecov](https://codecov.io/gh/kevinhowbrook/wagtailguide/branch/master/graph/badge.svg?token=K2XKBfubBh)](https://codecov.io/gh/kevinhowbrook/wagtailguide)
+![tests](https://github.com/torchbox/wagtailguide/workflows/Test/badge.svg) [![codecov](https://codecov.io/gh/kevinhowbrook/wagtailguide/branch/master/graph/badge.svg?token=K2XKBfubBh)](https://codecov.io/gh/kevinhowbrook/wagtailguide)
 
 ## What is it?
 
 The Wagtail Guide app adds functionality for creating and editing a guide for editors and publishers to help them create good content.
 
 ## Installation
 
 Wagtailguide has a pypi package and can be installed with:
 
-```
+```bash
 pip install wagtail-guide
 ```
 
 After installing, add it to your settings file along with `wagtail.contrib.settings`, the settings inclusion should be placed with your other wagtail.contrib libraries:
 
-```
+```python
 INSTALLED_APPS = [
     ...
     'wagtail_guide',
     'wagtail.contrib.settings',
 ]
 ```
 
@@ -50,39 +51,39 @@
 You can use this setting to turn off the Wagtail core Editor Guide link
 
 ### Examples of customisation via settings
 
 Here is an example of a custom menu label (outlined here in orange),
 and placing the editor guide link in the help menu:
 
-```
+```python
 WAGTAIL_GUIDE_SETTINGS = {
     "ADD_WAGTAIL_GUIDE_TO_HELP_MENU": True,
     "WAGTAIL_GUIDE_MENU_LABEL": "CMS Publishing Guide",
     "HIDE_WAGTAIL_CORE_EDITOR_GUIDE": False,
 }
 ```
 
-![](screenshots/custom-label.png)
+![custom label](screenshots/custom-label.png)
 
 Here is an example of hiding the core Editor Guide link and just using ours:
 
-```
+```python
 WAGTAIL_GUIDE_SETTINGS = {
     "ADD_WAGTAIL_GUIDE_TO_HELP_MENU": True,
     "WAGTAIL_GUIDE_MENU_LABEL": "CMS Publishing Guide",
     "HIDE_WAGTAIL_CORE_EDITOR_GUIDE": True,
 }
 ```
 
-![](screenshots/remove-help.png)
+![remove help](screenshots/remove-help.png)
 
 You can define them in your project settings file like this:
 
-```
+```python
 WAGTAIL_GUIDE_SETTINGS = {
     "ADD_WAGTAIL_GUIDE_TO_HELP_MENU": False,
     "WAGTAIL_GUIDE_MENU_LABEL": "WG guide menu label",
     "HIDE_WAGTAIL_CORE_EDITOR_GUIDE": True,
 }
 ```
 
@@ -105,7 +106,11 @@
 Once logged in, a new menu icon towards the bottom of the left hand menu will be visible labeled as 'Editor guide':
 
 ![guide view](screenshots/default.png)
 
 ## Dependencies
 
 Wagtail Guide requires `wagtail>=4.1`
+
+## Contributing
+
+We welcome contributions to this project, see [CONTRIBUTING.md](docs/CONTRIBUTING.md) for more details.
```

### Comparing `wagtail_guide-2.0.0/README.md` & `wagtail_guide-2.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Wagtail Guide
 
-![tests](https://github.com/kevinhowbrook/wagtailguide/workflows/Test/badge.svg) [![codecov](https://codecov.io/gh/kevinhowbrook/wagtailguide/branch/master/graph/badge.svg?token=K2XKBfubBh)](https://codecov.io/gh/kevinhowbrook/wagtailguide)
+![tests](https://github.com/torchbox/wagtailguide/workflows/Test/badge.svg) [![codecov](https://codecov.io/gh/kevinhowbrook/wagtailguide/branch/master/graph/badge.svg?token=K2XKBfubBh)](https://codecov.io/gh/kevinhowbrook/wagtailguide)
 
 ## What is it?
 
 The Wagtail Guide app adds functionality for creating and editing a guide for editors and publishers to help them create good content.
 
 ## Installation
 
 Wagtailguide has a pypi package and can be installed with:
 
-```
+```bash
 pip install wagtail-guide
 ```
 
 After installing, add it to your settings file along with `wagtail.contrib.settings`, the settings inclusion should be placed with your other wagtail.contrib libraries:
 
-```
+```python
 INSTALLED_APPS = [
     ...
     'wagtail_guide',
     'wagtail.contrib.settings',
 ]
 ```
 
@@ -38,39 +38,39 @@
 You can use this setting to turn off the Wagtail core Editor Guide link
 
 ### Examples of customisation via settings
 
 Here is an example of a custom menu label (outlined here in orange),
 and placing the editor guide link in the help menu:
 
-```
+```python
 WAGTAIL_GUIDE_SETTINGS = {
     "ADD_WAGTAIL_GUIDE_TO_HELP_MENU": True,
     "WAGTAIL_GUIDE_MENU_LABEL": "CMS Publishing Guide",
     "HIDE_WAGTAIL_CORE_EDITOR_GUIDE": False,
 }
 ```
 
-![](screenshots/custom-label.png)
+![custom label](screenshots/custom-label.png)
 
 Here is an example of hiding the core Editor Guide link and just using ours:
 
-```
+```python
 WAGTAIL_GUIDE_SETTINGS = {
     "ADD_WAGTAIL_GUIDE_TO_HELP_MENU": True,
     "WAGTAIL_GUIDE_MENU_LABEL": "CMS Publishing Guide",
     "HIDE_WAGTAIL_CORE_EDITOR_GUIDE": True,
 }
 ```
 
-![](screenshots/remove-help.png)
+![remove help](screenshots/remove-help.png)
 
 You can define them in your project settings file like this:
 
-```
+```python
 WAGTAIL_GUIDE_SETTINGS = {
     "ADD_WAGTAIL_GUIDE_TO_HELP_MENU": False,
     "WAGTAIL_GUIDE_MENU_LABEL": "WG guide menu label",
     "HIDE_WAGTAIL_CORE_EDITOR_GUIDE": True,
 }
 ```
 
@@ -93,7 +93,11 @@
 Once logged in, a new menu icon towards the bottom of the left hand menu will be visible labeled as 'Editor guide':
 
 ![guide view](screenshots/default.png)
 
 ## Dependencies
 
 Wagtail Guide requires `wagtail>=4.1`
+
+## Contributing
+
+We welcome contributions to this project, see [CONTRIBUTING.md](docs/CONTRIBUTING.md) for more details.
```

### Comparing `wagtail_guide-2.0.0/setup.py` & `wagtail_guide-2.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,21 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="wagtail_guide",
-    version="2.0.0",
+    version="2.0.1",
     description="Adds functionality to add and edit a CMS guide page for editors.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kevinhowbrook/wagtailguide",
     author="Kevin Howbrook - Torchbox",
     author_email="kevin.howbrook@torchbox.com",
     license="MIT",
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     install_requires=[
         "wagtail>=4.1",
     ],
-    testing_extras=[
-        "coverage>=6.4.1",
-    ],
 )
```

### Comparing `wagtail_guide-2.0.0/wagtail_guide/migrations/0001_initial.py` & `wagtail_guide-2.0.1/wagtail_guide/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_guide-2.0.0/wagtail_guide/migrations/0002_alter_editorguide_sections_w30_usejsonfield.py` & `wagtail_guide-2.0.1/wagtail_guide/migrations/0002_alter_editorguide_sections_w30_usejsonfield.py`

 * *Files identical despite different names*

### Comparing `wagtail_guide-2.0.0/wagtail_guide/models.py` & `wagtail_guide-2.0.1/wagtail_guide/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_guide-2.0.0/wagtail_guide/settings.py` & `wagtail_guide-2.0.1/wagtail_guide/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_guide-2.0.0/wagtail_guide/static/css/wagtailguide.css` & `wagtail_guide-2.0.1/wagtail_guide/static/css/wagtailguide.css`

 * *Files identical despite different names*

### Comparing `wagtail_guide-2.0.0/wagtail_guide/templates/wagtail_guide/base.html` & `wagtail_guide-2.0.1/wagtail_guide/templates/wagtail_guide/base.html`

 * *Files identical despite different names*

### Comparing `wagtail_guide-2.0.0/wagtail_guide/tests/settings.py` & `wagtail_guide-2.0.1/wagtail_guide/tests/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_guide-2.0.0/wagtail_guide/tests/tests.py` & `wagtail_guide-2.0.1/wagtail_guide/tests/tests.py`

 * *Files identical despite different names*

### Comparing `wagtail_guide-2.0.0/wagtail_guide/tests/urls.py` & `wagtail_guide-2.0.1/wagtail_guide/tests/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_guide-2.0.0/wagtail_guide/views.py` & `wagtail_guide-2.0.1/wagtail_guide/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_guide-2.0.0/wagtail_guide/wagtail_hooks.py` & `wagtail_guide-2.0.1/wagtail_guide/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_guide-2.0.0/wagtail_guide.egg-info/PKG-INFO` & `wagtail_guide-2.0.1/wagtail_guide.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: wagtail-guide
-Version: 2.0.0
+Version: 2.0.1
 Summary: Adds functionality to add and edit a CMS guide page for editors.
 Home-page: https://github.com/kevinhowbrook/wagtailguide
 Author: Kevin Howbrook - Torchbox
 Author-email: kevin.howbrook@torchbox.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: lint
+Provides-Extra: testing
 License-File: LICENSE
 
 # Wagtail Guide
 
-![tests](https://github.com/kevinhowbrook/wagtailguide/workflows/Test/badge.svg) [![codecov](https://codecov.io/gh/kevinhowbrook/wagtailguide/branch/master/graph/badge.svg?token=K2XKBfubBh)](https://codecov.io/gh/kevinhowbrook/wagtailguide)
+![tests](https://github.com/torchbox/wagtailguide/workflows/Test/badge.svg) [![codecov](https://codecov.io/gh/kevinhowbrook/wagtailguide/branch/master/graph/badge.svg?token=K2XKBfubBh)](https://codecov.io/gh/kevinhowbrook/wagtailguide)
 
 ## What is it?
 
 The Wagtail Guide app adds functionality for creating and editing a guide for editors and publishers to help them create good content.
 
 ## Installation
 
 Wagtailguide has a pypi package and can be installed with:
 
-```
+```bash
 pip install wagtail-guide
 ```
 
 After installing, add it to your settings file along with `wagtail.contrib.settings`, the settings inclusion should be placed with your other wagtail.contrib libraries:
 
-```
+```python
 INSTALLED_APPS = [
     ...
     'wagtail_guide',
     'wagtail.contrib.settings',
 ]
 ```
 
@@ -50,39 +51,39 @@
 You can use this setting to turn off the Wagtail core Editor Guide link
 
 ### Examples of customisation via settings
 
 Here is an example of a custom menu label (outlined here in orange),
 and placing the editor guide link in the help menu:
 
-```
+```python
 WAGTAIL_GUIDE_SETTINGS = {
     "ADD_WAGTAIL_GUIDE_TO_HELP_MENU": True,
     "WAGTAIL_GUIDE_MENU_LABEL": "CMS Publishing Guide",
     "HIDE_WAGTAIL_CORE_EDITOR_GUIDE": False,
 }
 ```
 
-![](screenshots/custom-label.png)
+![custom label](screenshots/custom-label.png)
 
 Here is an example of hiding the core Editor Guide link and just using ours:
 
-```
+```python
 WAGTAIL_GUIDE_SETTINGS = {
     "ADD_WAGTAIL_GUIDE_TO_HELP_MENU": True,
     "WAGTAIL_GUIDE_MENU_LABEL": "CMS Publishing Guide",
     "HIDE_WAGTAIL_CORE_EDITOR_GUIDE": True,
 }
 ```
 
-![](screenshots/remove-help.png)
+![remove help](screenshots/remove-help.png)
 
 You can define them in your project settings file like this:
 
-```
+```python
 WAGTAIL_GUIDE_SETTINGS = {
     "ADD_WAGTAIL_GUIDE_TO_HELP_MENU": False,
     "WAGTAIL_GUIDE_MENU_LABEL": "WG guide menu label",
     "HIDE_WAGTAIL_CORE_EDITOR_GUIDE": True,
 }
 ```
 
@@ -105,7 +106,11 @@
 Once logged in, a new menu icon towards the bottom of the left hand menu will be visible labeled as 'Editor guide':
 
 ![guide view](screenshots/default.png)
 
 ## Dependencies
 
 Wagtail Guide requires `wagtail>=4.1`
+
+## Contributing
+
+We welcome contributions to this project, see [CONTRIBUTING.md](docs/CONTRIBUTING.md) for more details.
```

### Comparing `wagtail_guide-2.0.0/wagtail_guide.egg-info/SOURCES.txt` & `wagtail_guide-2.0.1/wagtail_guide.egg-info/SOURCES.txt`

 * *Files identical despite different names*

