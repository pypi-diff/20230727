# Comparing `tmp/flask-me-1.0.1.tar.gz` & `tmp/flask-me-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-me-1.0.1.tar", last modified: Wed Jul 12 09:41:09 2023, max compression
+gzip compressed data, was "flask-me-1.0.2.tar", last modified: Thu Jul 27 03:17:56 2023, max compression
```

## Comparing `flask-me-1.0.1.tar` & `flask-me-1.0.2.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.237190 flask-me-1.0.1/
--rw-r--r--   0 surawut   (1000) surawut   (1000)      326 2023-07-11 06:33:50.000000 flask-me-1.0.1/.codeclimate.yml
--rw-r--r--   0 surawut   (1000) surawut   (1000)      468 2023-07-11 06:33:50.000000 flask-me-1.0.1/.editorconfig
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.217190 flask-me-1.0.1/.github/
--rw-r--r--   0 surawut   (1000) surawut   (1000)     3078 2023-07-11 06:33:50.000000 flask-me-1.0.1/.github/labels.yml
--rw-r--r--   0 surawut   (1000) surawut   (1000)      523 2023-07-11 06:33:50.000000 flask-me-1.0.1/.github/release-drafter.yml
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.217190 flask-me-1.0.1/.github/workflows/
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1444 2023-07-11 06:33:50.000000 flask-me-1.0.1/.github/workflows/coverage.yml
--rw-r--r--   0 surawut   (1000) surawut   (1000)      247 2023-07-11 06:33:50.000000 flask-me-1.0.1/.github/workflows/drafter.yml
--rw-r--r--   0 surawut   (1000) surawut   (1000)      380 2023-07-11 06:33:50.000000 flask-me-1.0.1/.github/workflows/labeler-check.yml
--rw-r--r--   0 surawut   (1000) surawut   (1000)      371 2023-07-11 06:33:50.000000 flask-me-1.0.1/.github/workflows/labeler.yml
--rw-r--r--   0 surawut   (1000) surawut   (1000)      692 2023-07-11 06:33:50.000000 flask-me-1.0.1/.github/workflows/linting.yml
--rw-r--r--   0 surawut   (1000) surawut   (1000)      872 2023-07-11 06:33:50.000000 flask-me-1.0.1/.github/workflows/tests.yml
--rw-r--r--   0 surawut   (1000) surawut   (1000)      190 2023-07-11 06:33:50.000000 flask-me-1.0.1/.gitignore
--rw-r--r--   0 surawut   (1000) surawut   (1000)      282 2023-07-11 06:33:50.000000 flask-me-1.0.1/.markdownlint.json
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1241 2023-07-11 06:33:50.000000 flask-me-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 surawut   (1000) surawut   (1000)      419 2023-07-11 06:33:50.000000 flask-me-1.0.1/.readthedocs.yaml
--rw-r--r--   0 surawut   (1000) surawut   (1000)      281 2023-07-11 06:33:50.000000 flask-me-1.0.1/.sourcery.yaml
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1547 2023-07-11 06:33:50.000000 flask-me-1.0.1/AUTHORS.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)     7798 2023-07-11 06:33:50.000000 flask-me-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1521 2023-07-11 06:33:50.000000 flask-me-1.0.1/LICENSE.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)      254 2023-07-11 06:33:50.000000 flask-me-1.0.1/MANIFEST.in
--rw-r--r--   0 surawut   (1000) surawut   (1000)     6130 2023-07-12 09:41:09.237190 flask-me-1.0.1/PKG-INFO
--rw-r--r--   0 surawut   (1000) surawut   (1000)     4117 2023-07-12 09:23:21.000000 flask-me-1.0.1/README.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)       15 2023-07-11 06:33:50.000000 flask-me-1.0.1/codecov.yml
--rw-r--r--   0 surawut   (1000) surawut   (1000)      418 2023-07-12 08:15:23.000000 flask-me-1.0.1/docker-compose.yml
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.225190 flask-me-1.0.1/docs/
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1547 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/AUTHORS.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)     7798 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/CONTRIBUTING.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1521 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/LICENSE.md
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.225190 flask-me-1.0.1/docs/_static/
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.225190 flask-me-1.0.1/docs/_static/css/
--rw-r--r--   0 surawut   (1000) surawut   (1000)      280 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/_static/css/custom.css
--rw-r--r--   0 surawut   (1000) surawut   (1000)   150229 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/_static/debug_toolbar.png
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.225190 flask-me-1.0.1/docs/api/
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1428 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/api/base.rst
--rw-r--r--   0 surawut   (1000) surawut   (1000)       82 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/api/index.rst
--rw-r--r--   0 surawut   (1000) surawut   (1000)      542 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/api/wtf.rst
--rw-r--r--   0 surawut   (1000) surawut   (1000)     4226 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/changelog.rst
--rw-r--r--   0 surawut   (1000) surawut   (1000)     8337 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/conf.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1816 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/custom_queryset.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1918 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/db_model.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)     4376 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/debug_toolbar.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)      589 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/example_app.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)     5630 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/flask_config.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)    30392 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/forms.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)      652 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/index.rst
--rw-r--r--   0 surawut   (1000) surawut   (1000)     3965 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/migration_to_v2.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)      147 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/requirements.txt
--rw-r--r--   0 surawut   (1000) surawut   (1000)      289 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/session_interface.md
--rw-r--r--   0 surawut   (1000) surawut   (1000)     2133 2023-07-11 06:33:50.000000 flask-me-1.0.1/docs/wtf_forms.md
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.225190 flask-me-1.0.1/example_app/
--rw-r--r--   0 surawut   (1000) surawut   (1000)        0 2023-07-11 07:20:45.000000 flask-me-1.0.1/example_app/__init__.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     2785 2023-07-11 10:29:35.000000 flask-me-1.0.1/example_app/app.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)      831 2023-07-11 10:19:55.000000 flask-me-1.0.1/example_app/boolean_demo.py
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.213190 flask-me-1.0.1/example_app/compose/
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.225190 flask-me-1.0.1/example_app/compose/flask/
--rw-r--r--   0 surawut   (1000) surawut   (1000)      377 2023-07-12 09:25:26.000000 flask-me-1.0.1/example_app/compose/flask/Dockerfile
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1025 2023-07-11 10:19:55.000000 flask-me-1.0.1/example_app/dates_demo.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)      988 2023-07-11 10:19:55.000000 flask-me-1.0.1/example_app/dict_demo.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     2456 2023-07-11 06:33:50.000000 flask-me-1.0.1/example_app/models.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)      901 2023-07-11 10:19:55.000000 flask-me-1.0.1/example_app/numbers_demo.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1056 2023-07-11 10:19:55.000000 flask-me-1.0.1/example_app/strings_demo.py
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.229190 flask-me-1.0.1/example_app/templates/
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1012 2023-07-11 06:33:50.000000 flask-me-1.0.1/example_app/templates/_formhelpers.html
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1058 2023-07-11 06:33:50.000000 flask-me-1.0.1/example_app/templates/form_demo.html
--rw-r--r--   0 surawut   (1000) surawut   (1000)      822 2023-07-11 06:33:50.000000 flask-me-1.0.1/example_app/templates/index.html
--rw-r--r--   0 surawut   (1000) surawut   (1000)      878 2023-07-11 06:33:50.000000 flask-me-1.0.1/example_app/templates/layout.html
--rw-r--r--   0 surawut   (1000) surawut   (1000)      941 2023-07-11 06:33:50.000000 flask-me-1.0.1/example_app/templates/pagination.html
--rw-r--r--   0 surawut   (1000) surawut   (1000)     3705 2023-07-11 10:19:55.000000 flask-me-1.0.1/example_app/views.py
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.229190 flask-me-1.0.1/flask_me.egg-info/
--rw-r--r--   0 surawut   (1000) surawut   (1000)     6130 2023-07-12 09:41:09.000000 flask-me-1.0.1/flask_me.egg-info/PKG-INFO
--rw-r--r--   0 surawut   (1000) surawut   (1000)     2370 2023-07-12 09:41:09.000000 flask-me-1.0.1/flask_me.egg-info/SOURCES.txt
--rw-r--r--   0 surawut   (1000) surawut   (1000)        1 2023-07-12 09:41:09.000000 flask-me-1.0.1/flask_me.egg-info/dependency_links.txt
--rw-r--r--   0 surawut   (1000) surawut   (1000)        1 2023-07-12 09:40:30.000000 flask-me-1.0.1/flask_me.egg-info/not-zip-safe
--rw-r--r--   0 surawut   (1000) surawut   (1000)      344 2023-07-12 09:41:09.000000 flask-me-1.0.1/flask_me.egg-info/requires.txt
--rw-r--r--   0 surawut   (1000) surawut   (1000)       18 2023-07-12 09:41:09.000000 flask-me-1.0.1/flask_me.egg-info/top_level.txt
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.233190 flask-me-1.0.1/flask_mongoengine/
--rw-r--r--   0 surawut   (1000) surawut   (1000)     5660 2023-07-11 06:33:50.000000 flask-me-1.0.1/flask_mongoengine/__init__.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)      160 2023-07-12 09:41:09.000000 flask-me-1.0.1/flask_mongoengine/_version.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     5230 2023-07-11 06:33:50.000000 flask-me-1.0.1/flask_mongoengine/connection.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)    44904 2023-07-11 06:33:50.000000 flask-me-1.0.1/flask_mongoengine/db_fields.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1309 2023-07-11 06:33:50.000000 flask-me-1.0.1/flask_mongoengine/decorators.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     8334 2023-07-11 06:33:50.000000 flask-me-1.0.1/flask_mongoengine/documents.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     3726 2023-07-11 06:44:03.000000 flask-me-1.0.1/flask_mongoengine/json.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     5945 2023-07-11 06:33:50.000000 flask-me-1.0.1/flask_mongoengine/pagination.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     6781 2023-07-11 06:36:38.000000 flask-me-1.0.1/flask_mongoengine/panels.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     3308 2023-07-11 06:33:50.000000 flask-me-1.0.1/flask_mongoengine/sessions.py
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.213190 flask-me-1.0.1/flask_mongoengine/templates/
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.233190 flask-me-1.0.1/flask_mongoengine/templates/panels/
--rw-r--r--   0 surawut   (1000) surawut   (1000)     2752 2023-07-11 06:33:50.000000 flask-me-1.0.1/flask_mongoengine/templates/panels/mongo-panel.html
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.233190 flask-me-1.0.1/flask_mongoengine/wtf/
--rw-r--r--   0 surawut   (1000) surawut   (1000)      116 2023-07-11 06:33:50.000000 flask-me-1.0.1/flask_mongoengine/wtf/__init__.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)    15398 2023-07-11 06:33:50.000000 flask-me-1.0.1/flask_mongoengine/wtf/fields.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)      825 2023-07-11 06:33:50.000000 flask-me-1.0.1/flask_mongoengine/wtf/models.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)    11994 2023-07-11 06:33:50.000000 flask-me-1.0.1/flask_mongoengine/wtf/orm.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     4186 2023-07-11 06:33:50.000000 flask-me-1.0.1/noxfile.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     3362 2023-07-12 09:30:05.000000 flask-me-1.0.1/pyproject.toml
--rw-r--r--   0 surawut   (1000) surawut   (1000)      437 2023-07-12 09:41:09.237190 flask-me-1.0.1/setup.cfg
--rw-r--r--   0 surawut   (1000) surawut   (1000)      122 2023-07-11 07:02:06.000000 flask-me-1.0.1/setup.py
-drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-12 09:41:09.237190 flask-me-1.0.1/tests/
--rw-r--r--   0 surawut   (1000) surawut   (1000)        0 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/__init__.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     2251 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/conftest.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)      748 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_base.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1290 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_basic_app.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)    10211 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_connection.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)    45819 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_db_fields.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     1361 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_db_fields_import_protection.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)    10690 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_debug_panel.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)      562 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_decorators.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)    16800 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_forms.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)    14247 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_forms_v2.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     2308 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_json.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     2501 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_json_app.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     2561 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_pagination.py
--rw-r--r--   0 surawut   (1000) surawut   (1000)     2491 2023-07-11 06:33:50.000000 flask-me-1.0.1/tests/test_session.py
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.204789 flask-me-1.0.2/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      326 2023-07-11 06:33:50.000000 flask-me-1.0.2/.codeclimate.yml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      468 2023-07-11 06:33:50.000000 flask-me-1.0.2/.editorconfig
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.160789 flask-me-1.0.2/.github/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     3078 2023-07-11 06:33:50.000000 flask-me-1.0.2/.github/labels.yml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      523 2023-07-11 06:33:50.000000 flask-me-1.0.2/.github/release-drafter.yml
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.168789 flask-me-1.0.2/.github/workflows/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1444 2023-07-11 06:33:50.000000 flask-me-1.0.2/.github/workflows/coverage.yml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      247 2023-07-11 06:33:50.000000 flask-me-1.0.2/.github/workflows/drafter.yml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      380 2023-07-11 06:33:50.000000 flask-me-1.0.2/.github/workflows/labeler-check.yml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      371 2023-07-11 06:33:50.000000 flask-me-1.0.2/.github/workflows/labeler.yml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      692 2023-07-11 06:33:50.000000 flask-me-1.0.2/.github/workflows/linting.yml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      872 2023-07-11 06:33:50.000000 flask-me-1.0.2/.github/workflows/tests.yml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      190 2023-07-11 06:33:50.000000 flask-me-1.0.2/.gitignore
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      282 2023-07-11 06:33:50.000000 flask-me-1.0.2/.markdownlint.json
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1241 2023-07-11 06:33:50.000000 flask-me-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      419 2023-07-11 06:33:50.000000 flask-me-1.0.2/.readthedocs.yaml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      281 2023-07-11 06:33:50.000000 flask-me-1.0.2/.sourcery.yaml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1547 2023-07-11 06:33:50.000000 flask-me-1.0.2/AUTHORS.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     7798 2023-07-11 06:33:50.000000 flask-me-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1521 2023-07-11 06:33:50.000000 flask-me-1.0.2/LICENSE.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      254 2023-07-11 06:33:50.000000 flask-me-1.0.2/MANIFEST.in
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     6101 2023-07-27 03:17:56.204789 flask-me-1.0.2/PKG-INFO
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     4088 2023-07-12 10:03:08.000000 flask-me-1.0.2/README.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)       15 2023-07-11 06:33:50.000000 flask-me-1.0.2/codecov.yml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      418 2023-07-12 08:15:23.000000 flask-me-1.0.2/docker-compose.yml
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.172789 flask-me-1.0.2/docs/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1547 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/AUTHORS.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     7798 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/CONTRIBUTING.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1521 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/LICENSE.md
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.172789 flask-me-1.0.2/docs/_static/
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.172789 flask-me-1.0.2/docs/_static/css/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      280 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/_static/css/custom.css
+-rw-r--r--   0 surawut   (1000) surawut   (1000)   150229 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/_static/debug_toolbar.png
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.176789 flask-me-1.0.2/docs/api/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1428 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/api/base.rst
+-rw-r--r--   0 surawut   (1000) surawut   (1000)       82 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/api/index.rst
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      542 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/api/wtf.rst
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     4226 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/changelog.rst
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     8337 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/conf.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1816 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/custom_queryset.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1918 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/db_model.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     4376 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/debug_toolbar.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      589 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/example_app.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     5630 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/flask_config.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)    30392 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/forms.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      652 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/index.rst
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     3965 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/migration_to_v2.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      147 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/requirements.txt
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      289 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/session_interface.md
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     2133 2023-07-11 06:33:50.000000 flask-me-1.0.2/docs/wtf_forms.md
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.180789 flask-me-1.0.2/example_app/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)        0 2023-07-11 07:20:45.000000 flask-me-1.0.2/example_app/__init__.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     2785 2023-07-11 10:29:35.000000 flask-me-1.0.2/example_app/app.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      831 2023-07-11 10:19:55.000000 flask-me-1.0.2/example_app/boolean_demo.py
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.152789 flask-me-1.0.2/example_app/compose/
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.180789 flask-me-1.0.2/example_app/compose/flask/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      377 2023-07-12 09:25:26.000000 flask-me-1.0.2/example_app/compose/flask/Dockerfile
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1025 2023-07-11 10:19:55.000000 flask-me-1.0.2/example_app/dates_demo.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      988 2023-07-11 10:19:55.000000 flask-me-1.0.2/example_app/dict_demo.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     2456 2023-07-11 06:33:50.000000 flask-me-1.0.2/example_app/models.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      901 2023-07-11 10:19:55.000000 flask-me-1.0.2/example_app/numbers_demo.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1056 2023-07-11 10:19:55.000000 flask-me-1.0.2/example_app/strings_demo.py
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.184790 flask-me-1.0.2/example_app/templates/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1012 2023-07-11 06:33:50.000000 flask-me-1.0.2/example_app/templates/_formhelpers.html
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1058 2023-07-11 06:33:50.000000 flask-me-1.0.2/example_app/templates/form_demo.html
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      822 2023-07-11 06:33:50.000000 flask-me-1.0.2/example_app/templates/index.html
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      878 2023-07-11 06:33:50.000000 flask-me-1.0.2/example_app/templates/layout.html
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      941 2023-07-11 06:33:50.000000 flask-me-1.0.2/example_app/templates/pagination.html
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     3705 2023-07-11 10:19:55.000000 flask-me-1.0.2/example_app/views.py
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.184790 flask-me-1.0.2/flask_me.egg-info/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     6101 2023-07-27 03:17:56.000000 flask-me-1.0.2/flask_me.egg-info/PKG-INFO
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     2370 2023-07-27 03:17:56.000000 flask-me-1.0.2/flask_me.egg-info/SOURCES.txt
+-rw-r--r--   0 surawut   (1000) surawut   (1000)        1 2023-07-27 03:17:56.000000 flask-me-1.0.2/flask_me.egg-info/dependency_links.txt
+-rw-r--r--   0 surawut   (1000) surawut   (1000)        1 2023-07-12 09:40:30.000000 flask-me-1.0.2/flask_me.egg-info/not-zip-safe
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      342 2023-07-27 03:17:56.000000 flask-me-1.0.2/flask_me.egg-info/requires.txt
+-rw-r--r--   0 surawut   (1000) surawut   (1000)       18 2023-07-27 03:17:56.000000 flask-me-1.0.2/flask_me.egg-info/top_level.txt
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.188789 flask-me-1.0.2/flask_mongoengine/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     5660 2023-07-11 06:33:50.000000 flask-me-1.0.2/flask_mongoengine/__init__.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      160 2023-07-27 03:17:55.000000 flask-me-1.0.2/flask_mongoengine/_version.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     5230 2023-07-11 06:33:50.000000 flask-me-1.0.2/flask_mongoengine/connection.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)    44904 2023-07-11 06:33:50.000000 flask-me-1.0.2/flask_mongoengine/db_fields.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1309 2023-07-11 06:33:50.000000 flask-me-1.0.2/flask_mongoengine/decorators.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     8334 2023-07-11 06:33:50.000000 flask-me-1.0.2/flask_mongoengine/documents.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     3726 2023-07-11 06:44:03.000000 flask-me-1.0.2/flask_mongoengine/json.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     5945 2023-07-11 06:33:50.000000 flask-me-1.0.2/flask_mongoengine/pagination.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     6781 2023-07-11 06:36:38.000000 flask-me-1.0.2/flask_mongoengine/panels.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     3308 2023-07-11 06:33:50.000000 flask-me-1.0.2/flask_mongoengine/sessions.py
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.152789 flask-me-1.0.2/flask_mongoengine/templates/
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.192789 flask-me-1.0.2/flask_mongoengine/templates/panels/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     2752 2023-07-11 06:33:50.000000 flask-me-1.0.2/flask_mongoengine/templates/panels/mongo-panel.html
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.196790 flask-me-1.0.2/flask_mongoengine/wtf/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      116 2023-07-11 06:33:50.000000 flask-me-1.0.2/flask_mongoengine/wtf/__init__.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)    15398 2023-07-11 06:33:50.000000 flask-me-1.0.2/flask_mongoengine/wtf/fields.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      825 2023-07-11 06:33:50.000000 flask-me-1.0.2/flask_mongoengine/wtf/models.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)    11994 2023-07-11 06:33:50.000000 flask-me-1.0.2/flask_mongoengine/wtf/orm.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     4186 2023-07-11 06:33:50.000000 flask-me-1.0.2/noxfile.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     3360 2023-07-27 03:14:06.000000 flask-me-1.0.2/pyproject.toml
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      437 2023-07-27 03:17:56.204789 flask-me-1.0.2/setup.cfg
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      122 2023-07-11 07:02:06.000000 flask-me-1.0.2/setup.py
+drwxr-xr-x   0 surawut   (1000) surawut   (1000)        0 2023-07-27 03:17:56.204789 flask-me-1.0.2/tests/
+-rw-r--r--   0 surawut   (1000) surawut   (1000)        0 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/__init__.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     2251 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/conftest.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      748 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/test_base.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1290 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/test_basic_app.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)    10211 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/test_connection.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)    45819 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/test_db_fields.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     1361 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/test_db_fields_import_protection.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)    10690 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/test_debug_panel.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)      562 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/test_decorators.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)    16800 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/test_forms.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)    14247 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/test_forms_v2.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     2314 2023-07-12 10:24:10.000000 flask-me-1.0.2/tests/test_json.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     2501 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/test_json_app.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     2561 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/test_pagination.py
+-rw-r--r--   0 surawut   (1000) surawut   (1000)     2491 2023-07-11 06:33:50.000000 flask-me-1.0.2/tests/test_session.py
```

### Comparing `flask-me-1.0.1/.github/labels.yml` & `flask-me-1.0.2/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/.github/release-drafter.yml` & `flask-me-1.0.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/.github/workflows/coverage.yml` & `flask-me-1.0.2/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/.github/workflows/linting.yml` & `flask-me-1.0.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/.github/workflows/tests.yml` & `flask-me-1.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/.pre-commit-config.yaml` & `flask-me-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/AUTHORS.md` & `flask-me-1.0.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/CONTRIBUTING.md` & `flask-me-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/LICENSE.md` & `flask-me-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/PKG-INFO` & `flask-me-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-me
-Version: 1.0.1
+Version: 1.0.2
 Summary: Flask extension that provides integration with MongoEngine and WTF model forms. This project is a forked of flask-mongoengine for compatable of new flask version
 Author-email: Ross Lawley <ross.lawley@gmail.com>
 Maintainer-email: Andrey Shpak <ashpak@ashpak.ru>, Surawut Saithong-in <surawut.kong@gmail.com>, Thanathip Limna <thanathip.limna@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/MongoEngine/flask-mongoengine
 Project-URL: Documentation, http://docs.mongoengine.org/projects/flask-mongoengine/en/latest/
 Project-URL: Repository, https://github.com/MongoEngine/flask-mongoengine
@@ -38,19 +38,19 @@
 Provides-Extra: legacy-dev
 License-File: LICENSE.md
 License-File: AUTHORS.md
 
 # Flask-ME is forked a Flask-MongoEngine
 
 [![PyPI version](https://badge.fury.io/py/flask-me.svg)](https://badge.fury.io/py/flask-me)
-[![CI Tests](https://github.com/MongoEngine/flask-mongoengine/actions/workflows/tests.yml/badge.svg)](https://github.com/MongoEngine/flask-mongoengine/actions/workflows/tests.yml)
+[![CI Tests](https://github.com/importstar/flask-me/actions/workflows/tests.yml/badge.svg)](https://github.com/importstar/flask-me/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/flask-mongoengine/badge/?version=latest)](http://docs.mongoengine.org/projects/flask-mongoengine/en/latest/?badge=latest)
 [![Maintainability](https://api.codeclimate.com/v1/badges/6fb8ae00b1008f5f1b20/maintainability)](https://codeclimate.com/github/MongoEngine/flask-mongoengine/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/6fb8ae00b1008f5f1b20/test_coverage)](https://codeclimate.com/github/MongoEngine/flask-mongoengine/test_coverage)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/flask-mongoengine)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/flask-me)
 
 Flask-MongoEngine is a Flask extension that provides integration with [MongoEngine],
 [WtfForms] and [FlaskDebugToolbar].
 
 ## Installation
 
 By default, Flask-MongoEngine will install integration only between [Flask] and
```

### Comparing `flask-me-1.0.1/README.md` & `flask-me-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Flask-ME is forked a Flask-MongoEngine
 
 [![PyPI version](https://badge.fury.io/py/flask-me.svg)](https://badge.fury.io/py/flask-me)
-[![CI Tests](https://github.com/MongoEngine/flask-mongoengine/actions/workflows/tests.yml/badge.svg)](https://github.com/MongoEngine/flask-mongoengine/actions/workflows/tests.yml)
+[![CI Tests](https://github.com/importstar/flask-me/actions/workflows/tests.yml/badge.svg)](https://github.com/importstar/flask-me/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/flask-mongoengine/badge/?version=latest)](http://docs.mongoengine.org/projects/flask-mongoengine/en/latest/?badge=latest)
 [![Maintainability](https://api.codeclimate.com/v1/badges/6fb8ae00b1008f5f1b20/maintainability)](https://codeclimate.com/github/MongoEngine/flask-mongoengine/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/6fb8ae00b1008f5f1b20/test_coverage)](https://codeclimate.com/github/MongoEngine/flask-mongoengine/test_coverage)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/flask-mongoengine)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/flask-me)
 
 Flask-MongoEngine is a Flask extension that provides integration with [MongoEngine],
 [WtfForms] and [FlaskDebugToolbar].
 
 ## Installation
 
 By default, Flask-MongoEngine will install integration only between [Flask] and
```

### Comparing `flask-me-1.0.1/docs/AUTHORS.md` & `flask-me-1.0.2/docs/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/CONTRIBUTING.md` & `flask-me-1.0.2/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/LICENSE.md` & `flask-me-1.0.2/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/_static/debug_toolbar.png` & `flask-me-1.0.2/docs/_static/debug_toolbar.png`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/api/base.rst` & `flask-me-1.0.2/docs/api/base.rst`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/api/wtf.rst` & `flask-me-1.0.2/docs/api/wtf.rst`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/changelog.rst` & `flask-me-1.0.2/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/conf.py` & `flask-me-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/custom_queryset.md` & `flask-me-1.0.2/docs/custom_queryset.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/db_model.md` & `flask-me-1.0.2/docs/db_model.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/debug_toolbar.md` & `flask-me-1.0.2/docs/debug_toolbar.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/example_app.md` & `flask-me-1.0.2/docs/example_app.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/flask_config.md` & `flask-me-1.0.2/docs/flask_config.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/forms.md` & `flask-me-1.0.2/docs/forms.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/index.rst` & `flask-me-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/migration_to_v2.md` & `flask-me-1.0.2/docs/migration_to_v2.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/docs/wtf_forms.md` & `flask-me-1.0.2/docs/wtf_forms.md`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/app.py` & `flask-me-1.0.2/example_app/app.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/boolean_demo.py` & `flask-me-1.0.2/example_app/boolean_demo.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/dates_demo.py` & `flask-me-1.0.2/example_app/dates_demo.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/dict_demo.py` & `flask-me-1.0.2/example_app/dict_demo.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/models.py` & `flask-me-1.0.2/example_app/models.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/numbers_demo.py` & `flask-me-1.0.2/example_app/numbers_demo.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/strings_demo.py` & `flask-me-1.0.2/example_app/strings_demo.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/templates/_formhelpers.html` & `flask-me-1.0.2/example_app/templates/_formhelpers.html`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/templates/form_demo.html` & `flask-me-1.0.2/example_app/templates/form_demo.html`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/templates/index.html` & `flask-me-1.0.2/example_app/templates/index.html`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/templates/layout.html` & `flask-me-1.0.2/example_app/templates/layout.html`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/templates/pagination.html` & `flask-me-1.0.2/example_app/templates/pagination.html`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/example_app/views.py` & `flask-me-1.0.2/example_app/views.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_me.egg-info/PKG-INFO` & `flask-me-1.0.2/flask_me.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-me
-Version: 1.0.1
+Version: 1.0.2
 Summary: Flask extension that provides integration with MongoEngine and WTF model forms. This project is a forked of flask-mongoengine for compatable of new flask version
 Author-email: Ross Lawley <ross.lawley@gmail.com>
 Maintainer-email: Andrey Shpak <ashpak@ashpak.ru>, Surawut Saithong-in <surawut.kong@gmail.com>, Thanathip Limna <thanathip.limna@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/MongoEngine/flask-mongoengine
 Project-URL: Documentation, http://docs.mongoengine.org/projects/flask-mongoengine/en/latest/
 Project-URL: Repository, https://github.com/MongoEngine/flask-mongoengine
@@ -38,19 +38,19 @@
 Provides-Extra: legacy-dev
 License-File: LICENSE.md
 License-File: AUTHORS.md
 
 # Flask-ME is forked a Flask-MongoEngine
 
 [![PyPI version](https://badge.fury.io/py/flask-me.svg)](https://badge.fury.io/py/flask-me)
-[![CI Tests](https://github.com/MongoEngine/flask-mongoengine/actions/workflows/tests.yml/badge.svg)](https://github.com/MongoEngine/flask-mongoengine/actions/workflows/tests.yml)
+[![CI Tests](https://github.com/importstar/flask-me/actions/workflows/tests.yml/badge.svg)](https://github.com/importstar/flask-me/actions/workflows/tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/flask-mongoengine/badge/?version=latest)](http://docs.mongoengine.org/projects/flask-mongoengine/en/latest/?badge=latest)
 [![Maintainability](https://api.codeclimate.com/v1/badges/6fb8ae00b1008f5f1b20/maintainability)](https://codeclimate.com/github/MongoEngine/flask-mongoengine/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/6fb8ae00b1008f5f1b20/test_coverage)](https://codeclimate.com/github/MongoEngine/flask-mongoengine/test_coverage)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/flask-mongoengine)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/flask-me)
 
 Flask-MongoEngine is a Flask extension that provides integration with [MongoEngine],
 [WtfForms] and [FlaskDebugToolbar].
 
 ## Installation
 
 By default, Flask-MongoEngine will install integration only between [Flask] and
```

### Comparing `flask-me-1.0.1/flask_me.egg-info/SOURCES.txt` & `flask-me-1.0.2/flask_me.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/__init__.py` & `flask-me-1.0.2/flask_mongoengine/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/connection.py` & `flask-me-1.0.2/flask_mongoengine/connection.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/db_fields.py` & `flask-me-1.0.2/flask_mongoengine/db_fields.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/decorators.py` & `flask-me-1.0.2/flask_mongoengine/decorators.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/documents.py` & `flask-me-1.0.2/flask_mongoengine/documents.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/json.py` & `flask-me-1.0.2/flask_mongoengine/json.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/pagination.py` & `flask-me-1.0.2/flask_mongoengine/pagination.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/panels.py` & `flask-me-1.0.2/flask_mongoengine/panels.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/sessions.py` & `flask-me-1.0.2/flask_mongoengine/sessions.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/templates/panels/mongo-panel.html` & `flask-me-1.0.2/flask_mongoengine/templates/panels/mongo-panel.html`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/wtf/fields.py` & `flask-me-1.0.2/flask_mongoengine/wtf/fields.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/wtf/models.py` & `flask-me-1.0.2/flask_mongoengine/wtf/models.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/flask_mongoengine/wtf/orm.py` & `flask-me-1.0.2/flask_mongoengine/wtf/orm.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/noxfile.py` & `flask-me-1.0.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/pyproject.toml` & `flask-me-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Framework :: Flask",
 ]
 dependencies = [
-  "Flask>=2.3.2",
+  "Flask>=2.0",
   "mongoengine>=0.21",
   'importlib-metadata; python_version<"3.8"',
 ]
 keywords = [
   "flask",
   "wtf",
   "wtf-forms",
```

### Comparing `flask-me-1.0.1/tests/conftest.py` & `flask-me-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/tests/test_base.py` & `flask-me-1.0.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/tests/test_basic_app.py` & `flask-me-1.0.2/tests/test_basic_app.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/tests/test_connection.py` & `flask-me-1.0.2/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/tests/test_db_fields.py` & `flask-me-1.0.2/tests/test_db_fields.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/tests/test_db_fields_import_protection.py` & `flask-me-1.0.2/tests/test_db_fields_import_protection.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/tests/test_debug_panel.py` & `flask-me-1.0.2/tests/test_debug_panel.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/tests/test_decorators.py` & `flask-me-1.0.2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/tests/test_forms.py` & `flask-me-1.0.2/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/tests/test_forms_v2.py` & `flask-me-1.0.2/tests/test_forms_v2.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/tests/test_json.py` & `flask-me-1.0.2/tests/test_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Extension of app JSON capabilities."""
 import flask
 import pytest
+import json
 
 from flask_mongoengine import MongoEngine
 from flask_mongoengine.json import use_json_provider
 
 
 @pytest.fixture()
 def extended_db(app):
@@ -37,15 +38,15 @@
 
     yield test_db
 
     # Clear database after tests, for graceful exit.
     test_db.connection["default"].drop_database(db_name)
 
 
-class DummyEncoder(flask.json.JSONEncoder):
+class DummyEncoder(json.JSONEncoder):
     """
     An example encoder which a user may create and override
     the apps json_encoder with.
     This class is a NO-OP, but used to test proper inheritance.
     """
```

### Comparing `flask-me-1.0.1/tests/test_json_app.py` & `flask-me-1.0.2/tests/test_json_app.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/tests/test_pagination.py` & `flask-me-1.0.2/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `flask-me-1.0.1/tests/test_session.py` & `flask-me-1.0.2/tests/test_session.py`

 * *Files identical despite different names*

