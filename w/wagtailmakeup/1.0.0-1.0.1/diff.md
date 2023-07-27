# Comparing `tmp/wagtailmakeup-1.0.0.tar.gz` & `tmp/wagtailmakeup-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailmakeup-1.0.0.tar", last modified: Mon Apr  3 08:34:07 2023, max compression
+gzip compressed data, was "wagtailmakeup-1.0.1.tar", last modified: Thu Jul 27 10:43:42 2023, max compression
```

## Comparing `wagtailmakeup-1.0.0.tar` & `wagtailmakeup-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:07.726720 wagtailmakeup-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-03 08:34:07.726720 wagtailmakeup-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-03 08:34:07.730720 wagtailmakeup-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:07.726720 wagtailmakeup-1.0.0/wagtailmakeup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/wagtailmakeup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/wagtailmakeup/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:07.726720 wagtailmakeup-1.0.0/wagtailmakeup/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/wagtailmakeup/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:07.726720 wagtailmakeup-1.0.0/wagtailmakeup/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/wagtailmakeup/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/wagtailmakeup/management/commands/make_up.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:07.726720 wagtailmakeup-1.0.0/wagtailmakeup/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/wagtailmakeup/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/wagtailmakeup/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:07.726720 wagtailmakeup-1.0.0/wagtailmakeup/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/wagtailmakeup/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/wagtailmakeup/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/wagtailmakeup/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-03 08:34:04.000000 wagtailmakeup-1.0.0/wagtailmakeup/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:34:07.726720 wagtailmakeup-1.0.0/wagtailmakeup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-03 08:34:07.000000 wagtailmakeup-1.0.0/wagtailmakeup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-03 08:34:07.000000 wagtailmakeup-1.0.0/wagtailmakeup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 08:34:07.000000 wagtailmakeup-1.0.0/wagtailmakeup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-03 08:34:07.000000 wagtailmakeup-1.0.0/wagtailmakeup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-03 08:34:07.000000 wagtailmakeup-1.0.0/wagtailmakeup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:42.545406 wagtailmakeup-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-27 10:43:42.545406 wagtailmakeup-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-27 10:43:42.545406 wagtailmakeup-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:42.541406 wagtailmakeup-1.0.1/wagtailmakeup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/wagtailmakeup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/wagtailmakeup/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:42.541406 wagtailmakeup-1.0.1/wagtailmakeup/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/wagtailmakeup/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:42.541406 wagtailmakeup-1.0.1/wagtailmakeup/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/wagtailmakeup/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/wagtailmakeup/management/commands/make_up.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:42.541406 wagtailmakeup-1.0.1/wagtailmakeup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/wagtailmakeup/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/wagtailmakeup/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:42.545406 wagtailmakeup-1.0.1/wagtailmakeup/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/wagtailmakeup/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/wagtailmakeup/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/wagtailmakeup/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 10:43:38.000000 wagtailmakeup-1.0.1/wagtailmakeup/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:42.541406 wagtailmakeup-1.0.1/wagtailmakeup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-27 10:43:42.000000 wagtailmakeup-1.0.1/wagtailmakeup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-27 10:43:42.000000 wagtailmakeup-1.0.1/wagtailmakeup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:43:42.000000 wagtailmakeup-1.0.1/wagtailmakeup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 10:43:42.000000 wagtailmakeup-1.0.1/wagtailmakeup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 10:43:42.000000 wagtailmakeup-1.0.1/wagtailmakeup.egg-info/top_level.txt
```

### Comparing `wagtailmakeup-1.0.0/PKG-INFO` & `wagtailmakeup-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,77 @@
 Metadata-Version: 2.1
 Name: wagtailmakeup
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wagtail Makeup
 Home-page: https://github.com/kevinhowbrook/wagtail-makeup
 Author: Kevin Howbrook
 License: MIT
 Keywords: wagtail,django
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 
 # Wagtail Makeup
 
 ![tests](https://github.com/kevinhowbrook/wagtail-makeup/workflows/Tests/badge.svg)
 [![codecov](https://codecov.io/gh/kevinhowbrook/wagtail-makeup/branch/main/graph/badge.svg?token=A4H7PFEL9J)](https://codecov.io/gh/kevinhowbrook/wagtail-makeup)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/kevinhowbrook/wagtail-makeup.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/kevinhowbrook/wagtail-makeup/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/kevinhowbrook/wagtail-makeup.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/kevinhowbrook/wagtail-makeup/context:python)
 
 Tired of having no images locally when you need them? Don't want to fill your computer up with images?
 Use Wagtail Makeup ;)
 
 ## Installation
 
-Wagail makeup depends on python unsplash:
+Wagtail makeup depends on python unsplash:
 
-`pip install python-unsplash wagtailmakeup`
+```bash
+pip install python-unsplash wagtailmakeup
+```
 
 ## Configuration
 
 Sign up for an Unsplash api key and add this to your settings:
 
-```
+```python
 # settings.py
 WAGTAIL_UNSPLASH = {
     "CLIENT_ID": "",
     "CLIENT_SECRET": ""
 }
 ```
 
 The API is rate limited to 50 request/hour... you can apply for a [higher rate limit](https://help.unsplash.com/en/articles/3887917-when-should-i-apply-for-a-higher-rate-limit).
 
 ## Using
 
 You probably don't want this in your production settings, so add the following to you local.py settings:
 
-```
+```python
 INSTALLED_APPS.append('wagtailmakeup')
 ```
 
 Wagtail Makeup works by providing a new management command:
 
-```
+```bash
 python manage.py make_up [search query] [amount of images]
 ```
 
 So you want to replace all your broken images on your site with dogs (who wouldn't)
 you can do it like this:
 
-```
+```python
 python manage.py make_up dogs 10
 ```
 
-Note: the amount value is the number of images to download, the higher this is, the more
-variance you will get.
+Note: the amount value is the number of images to download, the higher this is, the more variance you will get 😎
+
+## Contributing
 
-:cool:
+Contributions are welcome, please see our [contributing guide](docs/CONTRIBUTING.md) for more details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wagtailmakeup-1.0.0/README.md` & `wagtailmakeup-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 # Wagtail Makeup
 
 ![tests](https://github.com/kevinhowbrook/wagtail-makeup/workflows/Tests/badge.svg)
 [![codecov](https://codecov.io/gh/kevinhowbrook/wagtail-makeup/branch/main/graph/badge.svg?token=A4H7PFEL9J)](https://codecov.io/gh/kevinhowbrook/wagtail-makeup)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/kevinhowbrook/wagtail-makeup.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/kevinhowbrook/wagtail-makeup/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/kevinhowbrook/wagtail-makeup.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/kevinhowbrook/wagtail-makeup/context:python)
 
 Tired of having no images locally when you need them? Don't want to fill your computer up with images?
 Use Wagtail Makeup ;)
 
 ## Installation
 
-Wagail makeup depends on python unsplash:
+Wagtail makeup depends on python unsplash:
 
-`pip install python-unsplash wagtailmakeup`
+```bash
+pip install python-unsplash wagtailmakeup
+```
 
 ## Configuration
 
 Sign up for an Unsplash api key and add this to your settings:
 
-```
+```python
 # settings.py
 WAGTAIL_UNSPLASH = {
     "CLIENT_ID": "",
     "CLIENT_SECRET": ""
 }
 ```
 
 The API is rate limited to 50 request/hour... you can apply for a [higher rate limit](https://help.unsplash.com/en/articles/3887917-when-should-i-apply-for-a-higher-rate-limit).
 
 ## Using
 
 You probably don't want this in your production settings, so add the following to you local.py settings:
 
-```
+```python
 INSTALLED_APPS.append('wagtailmakeup')
 ```
 
 Wagtail Makeup works by providing a new management command:
 
-```
+```bash
 python manage.py make_up [search query] [amount of images]
 ```
 
 So you want to replace all your broken images on your site with dogs (who wouldn't)
 you can do it like this:
 
-```
+```python
 python manage.py make_up dogs 10
 ```
 
-Note: the amount value is the number of images to download, the higher this is, the more
-variance you will get.
+Note: the amount value is the number of images to download, the higher this is, the more variance you will get 😎
+
+## Contributing
 
-:cool:
+Contributions are welcome, please see our [contributing guide](docs/CONTRIBUTING.md) for more details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wagtailmakeup-1.0.0/setup.cfg` & `wagtailmakeup-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtailmakeup-1.0.0/setup.py` & `wagtailmakeup-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 testing_extras = [
     "coverage>=4.5",
 ]
 
 setup(
     name="wagtailmakeup",
-    version="1.0.0",
+    version="1.0.1",
     description="Wagtail Makeup",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kevinhowbrook/wagtail-makeup",
     author="Kevin Howbrook",
     license="MIT",
     packages=find_packages(exclude=["tests*"]),
@@ -30,13 +30,14 @@
     install_requires=["wagtail>=4.1", "python-unsplash>=1.1.0"],
     extras_require={"testing": testing_extras},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Framework :: Wagtail",
         "Framework :: Wagtail :: 4",
+        "Framework :: Wagtail :: 5",
     ],
 ),
```

### Comparing `wagtailmakeup-1.0.0/wagtailmakeup/management/commands/make_up.py` & `wagtailmakeup-1.0.1/wagtailmakeup/management/commands/make_up.py`

 * *Files identical despite different names*

### Comparing `wagtailmakeup-1.0.0/wagtailmakeup/tests/settings.py` & `wagtailmakeup-1.0.1/wagtailmakeup/tests/settings.py`

 * *Files identical despite different names*

### Comparing `wagtailmakeup-1.0.0/wagtailmakeup/tests/tests.py` & `wagtailmakeup-1.0.1/wagtailmakeup/tests/tests.py`

 * *Files identical despite different names*

### Comparing `wagtailmakeup-1.0.0/wagtailmakeup/tests/urls.py` & `wagtailmakeup-1.0.1/wagtailmakeup/tests/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailmakeup-1.0.0/wagtailmakeup.egg-info/PKG-INFO` & `wagtailmakeup-1.0.1/wagtailmakeup.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,77 @@
 Metadata-Version: 2.1
 Name: wagtailmakeup
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wagtail Makeup
 Home-page: https://github.com/kevinhowbrook/wagtail-makeup
 Author: Kevin Howbrook
 License: MIT
 Keywords: wagtail,django
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 
 # Wagtail Makeup
 
 ![tests](https://github.com/kevinhowbrook/wagtail-makeup/workflows/Tests/badge.svg)
 [![codecov](https://codecov.io/gh/kevinhowbrook/wagtail-makeup/branch/main/graph/badge.svg?token=A4H7PFEL9J)](https://codecov.io/gh/kevinhowbrook/wagtail-makeup)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/kevinhowbrook/wagtail-makeup.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/kevinhowbrook/wagtail-makeup/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/kevinhowbrook/wagtail-makeup.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/kevinhowbrook/wagtail-makeup/context:python)
 
 Tired of having no images locally when you need them? Don't want to fill your computer up with images?
 Use Wagtail Makeup ;)
 
 ## Installation
 
-Wagail makeup depends on python unsplash:
+Wagtail makeup depends on python unsplash:
 
-`pip install python-unsplash wagtailmakeup`
+```bash
+pip install python-unsplash wagtailmakeup
+```
 
 ## Configuration
 
 Sign up for an Unsplash api key and add this to your settings:
 
-```
+```python
 # settings.py
 WAGTAIL_UNSPLASH = {
     "CLIENT_ID": "",
     "CLIENT_SECRET": ""
 }
 ```
 
 The API is rate limited to 50 request/hour... you can apply for a [higher rate limit](https://help.unsplash.com/en/articles/3887917-when-should-i-apply-for-a-higher-rate-limit).
 
 ## Using
 
 You probably don't want this in your production settings, so add the following to you local.py settings:
 
-```
+```python
 INSTALLED_APPS.append('wagtailmakeup')
 ```
 
 Wagtail Makeup works by providing a new management command:
 
-```
+```bash
 python manage.py make_up [search query] [amount of images]
 ```
 
 So you want to replace all your broken images on your site with dogs (who wouldn't)
 you can do it like this:
 
-```
+```python
 python manage.py make_up dogs 10
 ```
 
-Note: the amount value is the number of images to download, the higher this is, the more
-variance you will get.
+Note: the amount value is the number of images to download, the higher this is, the more variance you will get 😎
+
+## Contributing
 
-:cool:
+Contributions are welcome, please see our [contributing guide](docs/CONTRIBUTING.md) for more details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wagtailmakeup-1.0.0/wagtailmakeup.egg-info/SOURCES.txt` & `wagtailmakeup-1.0.1/wagtailmakeup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

