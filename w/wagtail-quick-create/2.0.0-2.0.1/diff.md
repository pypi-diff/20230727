# Comparing `tmp/wagtail-quick-create-2.0.0.tar.gz` & `tmp/wagtail-quick-create-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-quick-create-2.0.0.tar", last modified: Thu Jul 14 09:08:06 2022, max compression
+gzip compressed data, was "wagtail-quick-create-2.0.1.tar", last modified: Thu Jul 27 10:26:13 2023, max compression
```

## Comparing `wagtail-quick-create-2.0.0.tar` & `wagtail-quick-create-2.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-07-14 09:08:06.927685 wagtail-quick-create-2.0.0/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1062 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/LICENSE
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       51 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/MANIFEST.in
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2414 2022-07-14 09:08:06.927685 wagtail-quick-create-2.0.0/PKG-INFO
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2013 2022-07-14 08:50:38.000000 wagtail-quick-create-2.0.0/README.md
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      410 2022-07-14 09:08:06.927685 wagtail-quick-create-2.0.0/setup.cfg
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      985 2022-07-14 09:06:01.000000 wagtail-quick-create-2.0.0/setup.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-07-14 09:08:06.923685 wagtail-quick-create-2.0.0/wagtail_quick_create.egg-info/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2414 2022-07-14 09:08:06.000000 wagtail-quick-create-2.0.0/wagtail_quick_create.egg-info/PKG-INFO
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      850 2022-07-14 09:08:06.000000 wagtail-quick-create-2.0.0/wagtail_quick_create.egg-info/SOURCES.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)        1 2022-07-14 09:08:06.000000 wagtail-quick-create-2.0.0/wagtail_quick_create.egg-info/dependency_links.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       14 2022-07-14 09:08:06.000000 wagtail-quick-create-2.0.0/wagtail_quick_create.egg-info/requires.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       19 2022-07-14 09:08:06.000000 wagtail-quick-create-2.0.0/wagtail_quick_create.egg-info/top_level.txt
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-07-14 09:08:06.923685 wagtail-quick-create-2.0.0/wagtailquickcreate/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/__init__.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-07-14 09:08:06.923685 wagtail-quick-create-2.0.0/wagtailquickcreate/templates/
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-07-14 09:08:06.923685 wagtail-quick-create-2.0.0/wagtailquickcreate/templates/wagtailquickcreate/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1731 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/templates/wagtailquickcreate/create.html
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       93 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/templates/wagtailquickcreate/panel.html
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-07-14 09:08:06.923685 wagtail-quick-create-2.0.0/wagtailquickcreate/tests/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/tests/__init__.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2288 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/tests/settings.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-07-14 09:08:06.927685 wagtail-quick-create-2.0.0/wagtailquickcreate/tests/standardpages/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/tests/standardpages/__init__.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2022-07-14 09:08:06.927685 wagtail-quick-create-2.0.0/wagtailquickcreate/tests/standardpages/migrations/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      905 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/tests/standardpages/migrations/0001_initial.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)        0 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/tests/standardpages/migrations/__init__.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      397 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/tests/standardpages/models.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1933 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/tests/tests.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      788 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/tests/urls.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     2294 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/views.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3194 2022-06-16 13:52:33.000000 wagtail-quick-create-2.0.0/wagtailquickcreate/wagtail_hooks.py
+drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 10:26:13.783505 wagtail-quick-create-2.0.1/
+-rw-r--r--   0 nick       (502) staff       (20)     1062 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/LICENSE
+-rw-r--r--   0 nick       (502) staff       (20)       51 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/MANIFEST.in
+-rw-r--r--   0 nick       (502) staff       (20)     2949 2023-07-27 10:26:13.783607 wagtail-quick-create-2.0.1/PKG-INFO
+-rw-r--r--   0 nick       (502) staff       (20)     2032 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/README.md
+-rw-r--r--   0 nick       (502) staff       (20)      410 2023-07-27 10:26:13.784016 wagtail-quick-create-2.0.1/setup.cfg
+-rw-r--r--   0 nick       (502) staff       (20)     1514 2023-07-27 10:21:04.000000 wagtail-quick-create-2.0.1/setup.py
+drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 10:26:13.780904 wagtail-quick-create-2.0.1/wagtail_quick_create.egg-info/
+-rw-r--r--   0 nick       (502) staff       (20)     2949 2023-07-27 10:26:13.000000 wagtail-quick-create-2.0.1/wagtail_quick_create.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (502) staff       (20)      850 2023-07-27 10:26:13.000000 wagtail-quick-create-2.0.1/wagtail_quick_create.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (502) staff       (20)        1 2023-07-27 10:26:13.000000 wagtail-quick-create-2.0.1/wagtail_quick_create.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (502) staff       (20)       13 2023-07-27 10:26:13.000000 wagtail-quick-create-2.0.1/wagtail_quick_create.egg-info/requires.txt
+-rw-r--r--   0 nick       (502) staff       (20)       19 2023-07-27 10:26:13.000000 wagtail-quick-create-2.0.1/wagtail_quick_create.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 10:26:13.781473 wagtail-quick-create-2.0.1/wagtailquickcreate/
+-rw-r--r--   0 nick       (502) staff       (20)        0 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/__init__.py
+drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 10:26:13.778747 wagtail-quick-create-2.0.1/wagtailquickcreate/templates/
+drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 10:26:13.781895 wagtail-quick-create-2.0.1/wagtailquickcreate/templates/wagtailquickcreate/
+-rw-r--r--   0 nick       (502) staff       (20)     1698 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/templates/wagtailquickcreate/create.html
+-rw-r--r--   0 nick       (502) staff       (20)       93 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/templates/wagtailquickcreate/panel.html
+drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 10:26:13.782641 wagtail-quick-create-2.0.1/wagtailquickcreate/tests/
+-rw-r--r--   0 nick       (502) staff       (20)        0 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/tests/__init__.py
+-rw-r--r--   0 nick       (502) staff       (20)     2241 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/tests/settings.py
+drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 10:26:13.782966 wagtail-quick-create-2.0.1/wagtailquickcreate/tests/standardpages/
+-rw-r--r--   0 nick       (502) staff       (20)        0 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/tests/standardpages/__init__.py
+drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 10:26:13.783356 wagtail-quick-create-2.0.1/wagtailquickcreate/tests/standardpages/migrations/
+-rw-r--r--   0 nick       (502) staff       (20)      905 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/tests/standardpages/migrations/0001_initial.py
+-rw-r--r--   0 nick       (502) staff       (20)        0 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/tests/standardpages/migrations/__init__.py
+-rw-r--r--   0 nick       (502) staff       (20)      268 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/tests/standardpages/models.py
+-rw-r--r--   0 nick       (502) staff       (20)     1747 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/tests/tests.py
+-rw-r--r--   0 nick       (502) staff       (20)      651 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/tests/urls.py
+-rw-r--r--   0 nick       (502) staff       (20)     2211 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/views.py
+-rw-r--r--   0 nick       (502) staff       (20)     3835 2023-07-27 10:12:07.000000 wagtail-quick-create-2.0.1/wagtailquickcreate/wagtail_hooks.py
```

### Comparing `wagtail-quick-create-2.0.0/LICENSE` & `wagtail-quick-create-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-quick-create-2.0.0/PKG-INFO` & `wagtail-quick-create-2.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,61 @@
-Metadata-Version: 2.1
-Name: wagtail-quick-create
-Version: 2.0.0
-Summary: Offer links to the admin user to create content under sections quickly.
-Home-page: https://github.com/kevinhowbrook/wagtailquickcreate
-Author: Kevin Howbrook - Torchbox, Kate Statton - NYPR
-Author-email: kevin.howbrook@torchbox.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Wagtail Quick Create
-[![CircleCI](https://circleci.com/gh/kevinhowbrook/wagtailquickcreate.svg?style=shield&circle)](https://circleci.com/gh/kevinhowbrook/wagtailquickcreate)
 
-### Wagtail Quick Create offers shortcut links to create objects from models specified in your settings file.
+## Wagtail Quick Create offers shortcut links to create objects from models specified in your settings file.
 
 A panel is added to the admin home, offering a type:
 
-![Quick Create Panel example](https://i.imgur.com/ssDighV.png)
+![Quick Create Panel example](./docs/images/dashboard.png)
 
 Clicking a create link will offer a parent selection for the new item
 
-![Parent selection example](https://i.imgur.com/6w5w6zD.png)
+![Parent selection example](./docs/images/create.png)
+
+## Note on parent pages
 
-### Note on parent pages
 Wagtailquickcreate needs the [`parent_page_types`](http://docs.wagtail.io/en/v2.5.1/reference/pages/model_reference.html#wagtail.core.models.Page.parent_page_types) set on the model you wish to include so it can successfully provide the parent page selection. If this isn't specified, you will likely see every page offered as a parent, this will not work as it's looking up pages using `wagtail.core.models.Page` and this core wagtail class has `is_creatable = False`
 
 ### Configuration
 
 Install using pip:
 
-```[bash]
+```bash
 pip install wagtail-quick-create
 ```
 
 After installing the module, add `wagtailquickcreate` to your installed apps in your settings file:
 
-```[python]
+```python
 INSTALLED_APPS = [
     ...
     'wagtailquickcreate',
 ]
 ```
 
 Also add the models you would like to create quick links for to your settings file as `'your_app_name.YourModelName'`:
 
 EG:
-```
+
+```python
 WAGTAIL_QUICK_CREATE_PAGE_TYPES = ['news.NewsPage', 'events.EventPage']
 ```
 
 If you want the Quick Create links panel to _replace_ the wagtail summary panel, you can set this by adding the following to your settings
 
-```
+```python
 WAGTAIL_QUICK_CREATE_REPLACE_SUMMARY_PANEL = True
 ```
 
 If you would like to offer image and or document links, this can also be done by specifying the following in your settings:
 
-```
+```python
 WAGTAIL_QUICK_CREATE_DOCUMENTS = True
 WAGTAIL_QUICK_CREATE_IMAGES = True
 ```
 
-### Credits/Authors
-Concept created by Kate Statton - NYPR [@katestatton](https://twitter.com/katestatton)
+## Contributing
 
+We are happy to receive pull requests for bug fixes, improvements and new features. See [CONTRIBUTING.md](./docs/CONTRIBUTING.md) for more information.
 
+## Credits/Authors
+
+Concept created by Kate Statton - NYPR [@katestatton](https://twitter.com/katestatton)
```

### Comparing `wagtail-quick-create-2.0.0/wagtail_quick_create.egg-info/PKG-INFO` & `wagtail-quick-create-2.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,84 @@
 Metadata-Version: 2.1
 Name: wagtail-quick-create
-Version: 2.0.0
+Version: 2.0.1
 Summary: Offer links to the admin user to create content under sections quickly.
 Home-page: https://github.com/kevinhowbrook/wagtailquickcreate
 Author: Kevin Howbrook - Torchbox, Kate Statton - NYPR
 Author-email: kevin.howbrook@torchbox.com
 License: MIT
-Platform: UNKNOWN
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
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Wagtail Quick Create
-[![CircleCI](https://circleci.com/gh/kevinhowbrook/wagtailquickcreate.svg?style=shield&circle)](https://circleci.com/gh/kevinhowbrook/wagtailquickcreate)
 
-### Wagtail Quick Create offers shortcut links to create objects from models specified in your settings file.
+## Wagtail Quick Create offers shortcut links to create objects from models specified in your settings file.
 
 A panel is added to the admin home, offering a type:
 
-![Quick Create Panel example](https://i.imgur.com/ssDighV.png)
+![Quick Create Panel example](./docs/images/dashboard.png)
 
 Clicking a create link will offer a parent selection for the new item
 
-![Parent selection example](https://i.imgur.com/6w5w6zD.png)
+![Parent selection example](./docs/images/create.png)
+
+## Note on parent pages
 
-### Note on parent pages
 Wagtailquickcreate needs the [`parent_page_types`](http://docs.wagtail.io/en/v2.5.1/reference/pages/model_reference.html#wagtail.core.models.Page.parent_page_types) set on the model you wish to include so it can successfully provide the parent page selection. If this isn't specified, you will likely see every page offered as a parent, this will not work as it's looking up pages using `wagtail.core.models.Page` and this core wagtail class has `is_creatable = False`
 
 ### Configuration
 
 Install using pip:
 
-```[bash]
+```bash
 pip install wagtail-quick-create
 ```
 
 After installing the module, add `wagtailquickcreate` to your installed apps in your settings file:
 
-```[python]
+```python
 INSTALLED_APPS = [
     ...
     'wagtailquickcreate',
 ]
 ```
 
 Also add the models you would like to create quick links for to your settings file as `'your_app_name.YourModelName'`:
 
 EG:
-```
+
+```python
 WAGTAIL_QUICK_CREATE_PAGE_TYPES = ['news.NewsPage', 'events.EventPage']
 ```
 
 If you want the Quick Create links panel to _replace_ the wagtail summary panel, you can set this by adding the following to your settings
 
-```
+```python
 WAGTAIL_QUICK_CREATE_REPLACE_SUMMARY_PANEL = True
 ```
 
 If you would like to offer image and or document links, this can also be done by specifying the following in your settings:
 
-```
+```python
 WAGTAIL_QUICK_CREATE_DOCUMENTS = True
 WAGTAIL_QUICK_CREATE_IMAGES = True
 ```
 
-### Credits/Authors
-Concept created by Kate Statton - NYPR [@katestatton](https://twitter.com/katestatton)
+## Contributing
 
+We are happy to receive pull requests for bug fixes, improvements and new features. See [CONTRIBUTING.md](./docs/CONTRIBUTING.md) for more information.
 
+## Credits/Authors
+
+Concept created by Kate Statton - NYPR [@katestatton](https://twitter.com/katestatton)
```

### Comparing `wagtail-quick-create-2.0.0/wagtail_quick_create.egg-info/SOURCES.txt` & `wagtail-quick-create-2.0.1/wagtail_quick_create.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-quick-create-2.0.0/wagtailquickcreate/templates/wagtailquickcreate/create.html` & `wagtail-quick-create-2.0.1/wagtailquickcreate/templates/wagtailquickcreate/create.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 
 {% extends "wagtailadmin/base.html" %}
 {% load wagtailadmin_tags static i18n %}
-{% block titletag %}{% trans "Dashboard" %}{% endblock %}
-{% block bodyclass %}homepage{% endblock %}
+{% block titletag %}{% trans browser_title %}{% endblock %}
 
 
 {% block content %}
-    <header class="merged nice-padding">
+    <header class="w-header w-header--merged">
         <div class="row row-flush">
-            <div class="col1">
-                <div class="avatar"><img src="{% avatar_url user %}" alt="" /></div>
-            </div>
-            <div class="col9">
-                <h1>Add {{ model_verbose_name }}</h1>
+            <div class="col">
+                <h1 class="w-header__title">
+                    <img src="{% avatar_url user %}" alt="" class="avatar"/>
+                    Add {{ model_verbose_name }}
+                </h1>
                 <h2>{{ user.get_full_name|default:user.get_username }}</h2>
             </div>
         </div>
     </header>
     <div class="nice-padding">
         <ul class="listing">
             {% if parent_pages %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
  {% extends "wagtailadmin/base.html" %} {% load wagtailadmin_tags static i18n
-%} {% block titletag %}{% trans "Dashboard" %}{% endblock %} {% block bodyclass
-%}homepage{% endblock %} {% block content %}
-****** Add {{ model_verbose_name }} ******
+%} {% block titletag %}{% trans browser_title %}{% endblock %} {% block content
+%}
+ Add {{ model_verbose_name }}
 ***** {{ user.get_full_name|default:user.get_username }} *****
     * {% if parent_pages %}
       Choose a parent section for the new {{ model_verbose_name }}
     * {% else %}
       There are no parent {{ model_verbose_name }} sections created for child
       pages to be added to yet...
     * {% endif %} {% for page in parent_pages %}
```

### Comparing `wagtail-quick-create-2.0.0/wagtailquickcreate/tests/settings.py` & `wagtail-quick-create-2.0.1/wagtailquickcreate/tests/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from wagtail import VERSION as WAGTAIL_VERSION
 
 PROJECT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 BASE_DIR = os.path.dirname(PROJECT_DIR)
 
 
 SECRET_KEY = 'not so secret'
 
@@ -26,15 +25,15 @@
     'wagtail.embeds',
     'wagtail.sites',
     'wagtail.users',
     'wagtail.snippets',
     'wagtail.documents',
     'wagtail.images',
     'wagtail.admin',
-    "wagtail" if WAGTAIL_VERSION >= (3, 0) else "wagtail.core",
+    "wagtail",
 
     'taggit',
 
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
@@ -75,7 +74,9 @@
 
 WAGTAIL_SITE_NAME = 'llama-savers'
 WAGTAIL_QUICK_CREATE_REPLACE_SUMMARY_PANEL = True
 WAGTAIL_QUICK_CREATE_DOCUMENTS = True
 WAGTAIL_QUICK_CREATE_IMAGES = True
 WAGTAIL_QUICK_CREATE_PAGE_TYPES = ['wagtailquickcreate.tests.standardpages.InformationPage']
 USE_TZ = True
+
+WAGTAILADMIN_BASE_URL = 'http://localhost:8000'
```

### Comparing `wagtail-quick-create-2.0.0/wagtailquickcreate/tests/standardpages/migrations/0001_initial.py` & `wagtail-quick-create-2.0.1/wagtailquickcreate/tests/standardpages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-quick-create-2.0.0/wagtailquickcreate/tests/tests.py` & `wagtail-quick-create-2.0.1/wagtailquickcreate/tests/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 from django.test import TestCase
 from django.urls import reverse
 
-from wagtail import VERSION as WAGTAIL_VERSION
-
-if WAGTAIL_VERSION >= (3, 0):
-    from wagtail.models import Page
-    from wagtail.test.utils import WagtailTestUtils
-else:
-    from wagtail.core.models import Page
-    from wagtail.tests.utils import WagtailTestUtils
+from wagtail.models import Page
+from wagtail.test.utils import WagtailTestUtils
 
 from wagtailquickcreate.tests.standardpages.models import IndexPage
 
 
 class WagtailQuickCreateTests(TestCase, WagtailTestUtils):
     fixtures = ['wagtailquickcreate/tests/fixtures/test.json']
 
@@ -35,17 +29,17 @@
 
     def test_admin(self):
         response = self.client.get(reverse('wagtailadmin_home'))
         self.assertEqual(response.status_code, 200)
 
     def test_quickcreate_panel_links(self):
         response = self.client.get('/admin/')
-        self.assertContains(response, 'Add Image', html=True)
-        self.assertContains(response, 'Add Document', html=True)
-        self.assertContains(response, 'Add Information page', html=True)
+        self.assertTrue('Add Image' in str(response.content))
+        self.assertTrue('Add Document' in str(response.content))
+        self.assertTrue('Add Information page' in str(response.content))
 
     def test_first_level_index_page_in_shortcut_view(self):
         response = self.client.get('/admin/quickcreate/create/standardpages/informationpage/')
         self.assertContains(response, 'Home > <strong>Section 1</strong>', html=True)
 
     def test_second_level_index_in_shortcut_view(self):
         response = self.client.get('/admin/quickcreate/create/standardpages/informationpage/')
```

### Comparing `wagtail-quick-create-2.0.0/wagtailquickcreate/tests/urls.py` & `wagtail-quick-create-2.0.1/wagtailquickcreate/tests/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from django.contrib import admin
 from django.urls import include, path
 
-from wagtail import VERSION as WAGTAIL_VERSION
 from wagtail.admin import urls as wagtailadmin_urls
 
-if WAGTAIL_VERSION >= (3, 0):
-    from wagtail import urls as wagtail_urls
-else:
-    from wagtail.core import urls as wagtail_urls
+from wagtail import urls as wagtail_urls
 
 from wagtail.documents import urls as wagtaildocs_urls
 
 private_urlpatterns = [
     path('django-admin/', admin.site.urls),
     path('admin/', include(wagtailadmin_urls)),
     path('documents/', include(wagtaildocs_urls)),
```

### Comparing `wagtail-quick-create-2.0.0/wagtailquickcreate/views.py` & `wagtail-quick-create-2.0.1/wagtailquickcreate/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from django.apps import apps
 from django.views.generic import TemplateView
-from wagtail import VERSION as WAGTAIL_VERSION
 
-if WAGTAIL_VERSION >= (3, 0):
-    from wagtail.models import Page, UserPagePermissionsProxy
-else:
-    from wagtail.core.models import Page, UserPagePermissionsProxy
+from wagtail.models import Page, UserPagePermissionsProxy
 
 
 # Helper function to work out page permissions
 def filter_pages_by_permission(user, pages):
     user_permissions = UserPagePermissionsProxy(user)
     return [
         page for page in pages
@@ -53,10 +49,11 @@
             item['page'] = i
             # Also send through the section page ancestors for a clearer link path
             # to the user.
             item['ancestors'] = i.get_ancestors()
             parent_pages.append(item)
 
         context['model_verbose_name'] = model.get_verbose_name()
+        context['browser_title'] = f'Add a {model.get_verbose_name()}'
         context['model_app'] = app
         context['parent_pages'] = parent_pages
         return context
```

### Comparing `wagtail-quick-create-2.0.0/wagtailquickcreate/wagtail_hooks.py` & `wagtail-quick-create-2.0.1/wagtailquickcreate/wagtail_hooks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from django.apps import apps
 from django.conf import settings
 from django.urls import path
 from django.utils.safestring import mark_safe
 
 from wagtail.admin.site_summary import SiteSummaryPanel, SummaryItem
-from wagtail import VERSION as WAGTAIL_VERSION
 
-if WAGTAIL_VERSION >= (3, 0):
-    from wagtail import hooks
-else:
-    from wagtail.core import hooks
+from wagtail import hooks
 
 from .views import QuickCreateView
 
 
 class QuickCreatePanel(SummaryItem):
     template_name = "wagtailquickcreate/panel.html"
     order = 50
@@ -39,29 +35,42 @@
             item['name'] = model.get_verbose_name()
             page_models.append(item)
 
         # Build up an html chunk for the links to be rendered in the panel
         page_models_html_chunk = [
             """
                 <a href="/admin/quickcreate/create/{model_link}/">
-                <button class="button bicolor icon icon-plus">Add {model_name}</button></a>""".format(
+                <button class="button bicolor button--icon margin-bottom-sm" style="margin-right:6px;margin-bottom:6px;">
+                <span class="icon-wrapper">
+                <svg class="icon icon-plus icon" aria-hidden="true"><use href="#icon-plus"></use></svg>
+                </span>
+                Add {model_name}</button></a>""".format(
                 model_link=i['link'], model_name=i['name']
             )
             for i in page_models
         ]
 
         page_models_html_chunk = list(set(page_models_html_chunk))
 
         if getattr(settings, "WAGTAIL_QUICK_CREATE_IMAGES", False):
             page_models_html_chunk.append("""
-                    <a href="/admin/images/multiple/add/"><button class="button bicolor icon icon-plus">Add Image</button></a>
+                    <a href="/admin/images/multiple/add/">
+                    <button class="button bicolor button--icon" style="margin-right:6px;margin-bottom:6px;">
+                    <span class="icon-wrapper">
+                    <svg class="icon icon-plus icon" aria-hidden="true"><use href="#icon-plus"></use></svg>
+                    </span>
+                    Add Image</button></a>
                     """)
         if getattr(settings, "WAGTAIL_QUICK_CREATE_DOCUMENTS", False):
             page_models_html_chunk.append("""
-                    <a href="/admin/documents/multiple/add/"><button class="button bicolor icon icon-plus">
+                    <a href="/admin/documents/multiple/add/">
+                    <button class="button bicolor button--icon" style="margin-right:6px;margin-bottom:6px;">
+                    <span class="icon-wrapper">
+                    <svg class="icon icon-plus icon" aria-hidden="true"><use href="#icon-plus"></use></svg>
+                    </span>
                     Add Document</button></a>
                     """)
         context["models"] = mark_safe(''.join(page_models_html_chunk))
         return context
 
 
 @hooks.register('register_admin_urls')
```

