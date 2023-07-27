# Comparing `tmp/edx-rbac-1.7.0.tar.gz` & `tmp/edx-rbac-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-rbac-1.7.0.tar", last modified: Tue Apr 12 18:34:53 2022, max compression
+gzip compressed data, was "edx-rbac-1.8.0.tar", last modified: Thu Jul 27 14:19:05 2023, max compression
```

## Comparing `edx-rbac-1.7.0.tar` & `edx-rbac-1.8.0.tar`

### file list

```diff
@@ -1,35 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 18:34:53.377242 edx-rbac-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     6614 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    35117 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10240 2022-04-12 18:34:53.377242 edx-rbac-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 18:34:53.377242 edx-rbac-1.7.0/edx_rbac/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/edx_rbac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 18:34:53.377242 edx-rbac-1.7.0/edx_rbac/admin/
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/edx_rbac/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/edx_rbac/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/edx_rbac/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/edx_rbac/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/edx_rbac/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/edx_rbac/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     3412 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/edx_rbac/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 18:34:53.373242 edx-rbac-1.7.0/edx_rbac/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 18:34:53.377242 edx-rbac-1.7.0/edx_rbac/templates/edx_rbac/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/edx_rbac/templates/edx_rbac/base.html
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/edx_rbac/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     8351 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/edx_rbac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 18:34:53.377242 edx-rbac-1.7.0/edx_rbac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10240 2022-04-12 18:34:53.000000 edx-rbac-1.7.0/edx_rbac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-04-12 18:34:53.000000 edx-rbac-1.7.0/edx_rbac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-12 18:34:53.000000 edx-rbac-1.7.0/edx_rbac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-12 18:34:53.000000 edx-rbac-1.7.0/edx_rbac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-04-12 18:34:53.000000 edx-rbac-1.7.0/edx_rbac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-12 18:34:53.000000 edx-rbac-1.7.0/edx_rbac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 18:34:53.377242 edx-rbac-1.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-04-12 18:34:53.377242 edx-rbac-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5305 2022-04-12 18:34:49.000000 edx-rbac-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.997646 edx-rbac-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     6755 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    35117 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10266 2023-07-27 14:19:04.997646 edx-rbac-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.993646 edx-rbac-1.8.0/edx_rbac/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.993646 edx-rbac-1.8.0/edx_rbac/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3412 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.989646 edx-rbac-1.8.0/edx_rbac/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.993646 edx-rbac-1.8.0/edx_rbac/templates/edx_rbac/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/templates/edx_rbac/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8351 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.993646 edx-rbac-1.8.0/edx_rbac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10266 2023-07-27 14:19:04.000000 edx-rbac-1.8.0/edx_rbac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-07-27 14:19:04.000000 edx-rbac-1.8.0/edx_rbac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 14:19:04.000000 edx-rbac-1.8.0/edx_rbac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 14:19:04.000000 edx-rbac-1.8.0/edx_rbac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-27 14:19:04.000000 edx-rbac-1.8.0/edx_rbac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-27 14:19:04.000000 edx-rbac-1.8.0/edx_rbac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.997646 edx-rbac-1.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-27 14:19:04.997646 edx-rbac-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5309 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.997646 edx-rbac-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/tests/test_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2376 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8860 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24090 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/tests/test_utils.py
```

### Comparing `edx-rbac-1.7.0/CHANGELOG.rst` & `edx-rbac-1.8.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,20 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 --------------------
 
+[1.8.0]
+-------
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Added support for Django 4.2
+
 [1.7.0]
 -------
 
 * fix: ``utils.get_role_auth_claim_for_user()`` now preserves the order of (role, context) pairs
   as returned by the `get_assignment()` function.
 
 [1.6.0] - 2022-01-19
```

### Comparing `edx-rbac-1.7.0/LICENSE` & `edx-rbac-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.7.0/LICENSE.txt` & `edx-rbac-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.7.0/PKG-INFO` & `edx-rbac-1.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edx-rbac
-Version: 1.7.0
+Version: 1.8.0
 Summary: Library to help managing role based access controls for django apps
-Home-page: https://github.com/edx/edx-rbac
+Home-page: https://github.com/openedx/edx-rbac
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
@@ -28,18 +27,18 @@
 |license-badge|
 
 Overview
 --------
 
 Library to help manage role based access controls for django services.
 
-* See the `Getting started <https://github.com/edx/edx-rbac/blob/master/docs/getting_started.rst>`_ guide to setup
+* See the `Getting started <https://github.com/openedx/edx-rbac/blob/master/docs/getting_started.rst>`_ guide to setup
   your development environment.
 
-* See the `How To Guide <https://github.com/edx/edx-rbac/blob/master/docs/how_to_guide.rst>`_ to learn about the
+* See the `How To Guide <https://github.com/openedx/edx-rbac/blob/master/docs/how_to_guide.rst>`_ to learn about the
   fundamentals of edx-rbac and how to implement RBAC in your Django service.
 
 License
 -------
 
 The code in this repository is licensed under the AGPL 3.0 unless
 otherwise noted.
@@ -47,24 +46,22 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/edx-rbac/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-rbac/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/edx-rbac/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-rbac/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -76,16 +73,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-rbac.svg
     :target: https://pypi.python.org/pypi/edx-rbac/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/edx-rbac/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/edx-rbac/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/edx-rbac/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/edx-rbac/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/edx-rbac/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/edx-rbac?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/edx-rbac/badge/?version=latest
@@ -93,15 +90,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-rbac.svg
     :target: https://pypi.python.org/pypi/edx-rbac/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/edx-rbac.svg
-    :target: https://github.com/edx/edx-rbac/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/edx-rbac/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -113,14 +110,20 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 --------------------
 
+[1.8.0]
+-------
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Added support for Django 4.2
+
 [1.7.0]
 -------
 
 * fix: ``utils.get_role_auth_claim_for_user()`` now preserves the order of (role, context) pairs
   as returned by the `get_assignment()` function.
 
 [1.6.0] - 2022-01-19
@@ -317,9 +320,7 @@
 [0.1.0] - 2019-02-28
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * First release on PyPI.
-
-
```

### Comparing `edx-rbac-1.7.0/README.rst` & `edx-rbac-1.8.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 |license-badge|
 
 Overview
 --------
 
 Library to help manage role based access controls for django services.
 
-* See the `Getting started <https://github.com/edx/edx-rbac/blob/master/docs/getting_started.rst>`_ guide to setup
+* See the `Getting started <https://github.com/openedx/edx-rbac/blob/master/docs/getting_started.rst>`_ guide to setup
   your development environment.
 
-* See the `How To Guide <https://github.com/edx/edx-rbac/blob/master/docs/how_to_guide.rst>`_ to learn about the
+* See the `How To Guide <https://github.com/openedx/edx-rbac/blob/master/docs/how_to_guide.rst>`_ to learn about the
   fundamentals of edx-rbac and how to implement RBAC in your Django service.
 
 License
 -------
 
 The code in this repository is licensed under the AGPL 3.0 unless
 otherwise noted.
@@ -24,24 +24,22 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/edx-rbac/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-rbac/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/edx-rbac/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-rbac/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -53,16 +51,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-rbac.svg
     :target: https://pypi.python.org/pypi/edx-rbac/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/edx-rbac/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/edx-rbac/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/edx-rbac/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/edx-rbac/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/edx-rbac/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/edx-rbac?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/edx-rbac/badge/?version=latest
@@ -70,9 +68,9 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-rbac.svg
     :target: https://pypi.python.org/pypi/edx-rbac/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/edx-rbac.svg
-    :target: https://github.com/edx/edx-rbac/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/edx-rbac/blob/master/LICENSE.txt
     :alt: License
```

### Comparing `edx-rbac-1.7.0/edx_rbac/admin/__init__.py` & `edx-rbac-1.8.0/edx_rbac/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.7.0/edx_rbac/admin/forms.py` & `edx-rbac-1.8.0/edx_rbac/admin/forms.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.7.0/edx_rbac/decorators.py` & `edx-rbac-1.8.0/edx_rbac/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.7.0/edx_rbac/fields.py` & `edx-rbac-1.8.0/edx_rbac/fields.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.7.0/edx_rbac/mixins.py` & `edx-rbac-1.8.0/edx_rbac/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.7.0/edx_rbac/models.py` & `edx-rbac-1.8.0/edx_rbac/models.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.7.0/edx_rbac/templates/edx_rbac/base.html` & `edx-rbac-1.8.0/edx_rbac/templates/edx_rbac/base.html`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.7.0/edx_rbac/utils.py` & `edx-rbac-1.8.0/edx_rbac/utils.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.7.0/edx_rbac.egg-info/PKG-INFO` & `edx-rbac-1.8.0/edx_rbac.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edx-rbac
-Version: 1.7.0
+Version: 1.8.0
 Summary: Library to help managing role based access controls for django apps
-Home-page: https://github.com/edx/edx-rbac
+Home-page: https://github.com/openedx/edx-rbac
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
@@ -28,18 +27,18 @@
 |license-badge|
 
 Overview
 --------
 
 Library to help manage role based access controls for django services.
 
-* See the `Getting started <https://github.com/edx/edx-rbac/blob/master/docs/getting_started.rst>`_ guide to setup
+* See the `Getting started <https://github.com/openedx/edx-rbac/blob/master/docs/getting_started.rst>`_ guide to setup
   your development environment.
 
-* See the `How To Guide <https://github.com/edx/edx-rbac/blob/master/docs/how_to_guide.rst>`_ to learn about the
+* See the `How To Guide <https://github.com/openedx/edx-rbac/blob/master/docs/how_to_guide.rst>`_ to learn about the
   fundamentals of edx-rbac and how to implement RBAC in your Django service.
 
 License
 -------
 
 The code in this repository is licensed under the AGPL 3.0 unless
 otherwise noted.
@@ -47,24 +46,22 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 PR description template should be automatically applied if you are sending PR from github interface; otherwise you
-can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/edx/edx-rbac/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
+can find it it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-rbac/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
-can find it at `ISSUE_TEMPLATE.md <https://github.com/edx/edx-rbac/blob/master/.github/ISSUE_TEMPLATE.md>`_
+can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-rbac/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -76,16 +73,16 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/edx-rbac.svg
     :target: https://pypi.python.org/pypi/edx-rbac/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/edx-rbac/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/edx-rbac/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/edx-rbac/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/edx-rbac/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/edx-rbac/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/edx-rbac?branch=master
     :alt: Codecov
 
 .. |doc-badge| image:: https://readthedocs.org/projects/edx-rbac/badge/?version=latest
@@ -93,15 +90,15 @@
     :alt: Documentation
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/edx-rbac.svg
     :target: https://pypi.python.org/pypi/edx-rbac/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/edx-rbac.svg
-    :target: https://github.com/edx/edx-rbac/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/edx-rbac/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -113,14 +110,20 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 --------------------
 
+[1.8.0]
+-------
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+* Added support for Django 4.2
+
 [1.7.0]
 -------
 
 * fix: ``utils.get_role_auth_claim_for_user()`` now preserves the order of (role, context) pairs
   as returned by the `get_assignment()` function.
 
 [1.6.0] - 2022-01-19
@@ -317,9 +320,7 @@
 [0.1.0] - 2019-02-28
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * First release on PyPI.
-
-
```

### Comparing `edx-rbac-1.7.0/edx_rbac.egg-info/SOURCES.txt` & `edx-rbac-1.8.0/edx_rbac.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -20,8 +20,14 @@
 edx_rbac.egg-info/not-zip-safe
 edx_rbac.egg-info/requires.txt
 edx_rbac.egg-info/top_level.txt
 edx_rbac/admin/__init__.py
 edx_rbac/admin/forms.py
 edx_rbac/templates/edx_rbac/base.html
 requirements/base.in
-requirements/constraints.txt
+requirements/constraints.txt
+tests/test_assignments.py
+tests/test_fields.py
+tests/test_forms.py
+tests/test_mixins.py
+tests/test_models.py
+tests/test_utils.py
```

### Comparing `edx-rbac-1.7.0/requirements/constraints.txt` & `edx-rbac-1.8.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.7.0/setup.py` & `edx-rbac-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 setup(
     name='edx-rbac',
     version=VERSION,
     description="""Library to help managing role based access controls for django apps""",
     long_description=README + '\n\n' + CHANGELOG,
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/edx-rbac',
+    url='https://github.com/openedx/edx-rbac',
     packages=[
         'edx_rbac',
     ],
     include_package_data=True,
     install_requires=load_requirements('requirements/base.in'),
     license="AGPL 3.0",
     zip_safe=False,
```

