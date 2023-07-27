# Comparing `tmp/sciline-0.0.1.tar.gz` & `tmp/sciline-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciline-0.0.1.tar", last modified: Wed Jul 26 09:36:35 2023, max compression
+gzip compressed data, was "sciline-0.0.2.tar", last modified: Thu Jul 27 04:03:23 2023, max compression
```

## Comparing `sciline-0.0.1.tar` & `sciline-0.0.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.756704 sciline-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)      290 2023-07-26 09:36:24.000000 sciline-0.0.1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.752704 sciline-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-26 09:36:24.000000 sciline-0.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.752704 sciline-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-07-26 09:36:24.000000 sciline-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-07-26 09:36:24.000000 sciline-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-07-26 09:36:24.000000 sciline-0.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1392 2023-07-26 09:36:24.000000 sciline-0.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-26 09:36:24.000000 sciline-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-07-26 09:36:24.000000 sciline-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-07-26 09:36:24.000000 sciline-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-07-26 09:36:24.000000 sciline-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-26 09:36:24.000000 sciline-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-07-26 09:36:35.756704 sciline-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-26 09:36:24.000000 sciline-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.752704 sciline-0.0.1/conda/
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-07-26 09:36:24.000000 sciline-0.0.1/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.752704 sciline-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.752704 sciline-0.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    75109 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (122)    75109 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.752704 sciline-0.0.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/_templates/class-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.752704 sciline-0.0.1/docs/api-reference/
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.752704 sciline-0.0.1/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (122)     3541 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/developer/coding-conventions.md
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/developer/dependency-management.md
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/developer/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/developer/index.md
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.752704 sciline-0.0.1/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (122)     9425 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/user-guide/getting-started.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-26 09:36:24.000000 sciline-0.0.1/docs/user-guide/index.md
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-07-26 09:36:24.000000 sciline-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.756704 sciline-0.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      933 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      119 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     4984 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/mypy.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/test-dask.in
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/test-dask.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-26 09:36:24.000000 sciline-0.0.1/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.756704 sciline-0.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (122)     7947 2023-07-26 09:36:24.000000 sciline-0.0.1/resources/sciline.svg
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-07-26 09:36:35.760704 sciline-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.748704 sciline-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.756704 sciline-0.0.1/src/sciline/
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-07-26 09:36:24.000000 sciline-0.0.1/src/sciline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-07-26 09:36:24.000000 sciline-0.0.1/src/sciline/domain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9564 2023-07-26 09:36:24.000000 sciline-0.0.1/src/sciline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:24.000000 sciline-0.0.1/src/sciline/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-07-26 09:36:24.000000 sciline-0.0.1/src/sciline/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2042 2023-07-26 09:36:24.000000 sciline-0.0.1/src/sciline/task_graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-07-26 09:36:24.000000 sciline-0.0.1/src/sciline/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.756704 sciline-0.0.1/src/sciline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-07-26 09:36:35.000000 sciline-0.0.1/src/sciline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-07-26 09:36:35.000000 sciline-0.0.1/src/sciline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 09:36:35.000000 sciline-0.0.1/src/sciline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-26 09:36:35.000000 sciline-0.0.1/src/sciline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-26 09:36:35.000000 sciline-0.0.1/src/sciline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:36:35.756704 sciline-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3027 2023-07-26 09:36:24.000000 sciline-0.0.1/tests/complex_workflow_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-07-26 09:36:24.000000 sciline-0.0.1/tests/dask_scheduler_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-26 09:36:24.000000 sciline-0.0.1/tests/domain_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-07-26 09:36:24.000000 sciline-0.0.1/tests/package_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    15918 2023-07-26 09:36:24.000000 sciline-0.0.1/tests/pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-07-26 09:36:24.000000 sciline-0.0.1/tests/task_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-07-26 09:36:24.000000 sciline-0.0.1/tests/visualize_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-07-26 09:36:24.000000 sciline-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.815481 sciline-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-07-27 04:03:12.000000 sciline-0.0.2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.807481 sciline-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-27 04:03:12.000000 sciline-0.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.811481 sciline-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-07-27 04:03:12.000000 sciline-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-07-27 04:03:12.000000 sciline-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-07-27 04:03:12.000000 sciline-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1392 2023-07-27 04:03:12.000000 sciline-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-27 04:03:12.000000 sciline-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-07-27 04:03:12.000000 sciline-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-07-27 04:03:12.000000 sciline-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-07-27 04:03:12.000000 sciline-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-27 04:03:12.000000 sciline-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-07-27 04:03:23.815481 sciline-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-27 04:03:12.000000 sciline-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.811481 sciline-0.0.2/conda/
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-07-27 04:03:12.000000 sciline-0.0.2/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.811481 sciline-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.811481 sciline-0.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    75109 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    75109 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.811481 sciline-0.0.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/_templates/class-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.811481 sciline-0.0.2/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.811481 sciline-0.0.2/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (122)     3541 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/developer/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.811481 sciline-0.0.2/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (122)     9425 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/user-guide/getting-started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-27 04:03:12.000000 sciline-0.0.2/docs/user-guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-07-27 04:03:12.000000 sciline-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.815481 sciline-0.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      933 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4984 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/test-dask.in
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/test-dask.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-27 04:03:12.000000 sciline-0.0.2/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.815481 sciline-0.0.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)     7947 2023-07-27 04:03:12.000000 sciline-0.0.2/resources/sciline.svg
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-07-27 04:03:23.815481 sciline-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.807481 sciline-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.815481 sciline-0.0.2/src/sciline/
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-07-27 04:03:12.000000 sciline-0.0.2/src/sciline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-07-27 04:03:12.000000 sciline-0.0.2/src/sciline/domain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9564 2023-07-27 04:03:12.000000 sciline-0.0.2/src/sciline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:12.000000 sciline-0.0.2/src/sciline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-07-27 04:03:12.000000 sciline-0.0.2/src/sciline/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2042 2023-07-27 04:03:12.000000 sciline-0.0.2/src/sciline/task_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2145 2023-07-27 04:03:12.000000 sciline-0.0.2/src/sciline/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.815481 sciline-0.0.2/src/sciline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-07-27 04:03:23.000000 sciline-0.0.2/src/sciline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-07-27 04:03:23.000000 sciline-0.0.2/src/sciline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 04:03:23.000000 sciline-0.0.2/src/sciline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-27 04:03:23.000000 sciline-0.0.2/src/sciline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-27 04:03:23.000000 sciline-0.0.2/src/sciline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 04:03:23.815481 sciline-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3027 2023-07-27 04:03:12.000000 sciline-0.0.2/tests/complex_workflow_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-07-27 04:03:12.000000 sciline-0.0.2/tests/dask_scheduler_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-27 04:03:12.000000 sciline-0.0.2/tests/domain_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-07-27 04:03:12.000000 sciline-0.0.2/tests/package_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15918 2023-07-27 04:03:12.000000 sciline-0.0.2/tests/pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-07-27 04:03:12.000000 sciline-0.0.2/tests/task_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      897 2023-07-27 04:03:12.000000 sciline-0.0.2/tests/visualize_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-07-27 04:03:12.000000 sciline-0.0.2/tox.ini
```

### Comparing `sciline-0.0.1/.github/workflows/ci.yml` & `sciline-0.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/.github/workflows/docs.yml` & `sciline-0.0.2/.github/workflows/docs.yml`

 * *Files 13% similar despite different names*

```diff
@@ -50,25 +50,23 @@
 
           python-version: '3.8'
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: |
           tox --skip-pkg-install -e docs -- sciline==${VERSION}
 
-          echo "target=$(python docs/version.py --version=${VERSION} --action=get-target)" >> $GITHUB_ENV
         if: ${{ inputs.publish }}
       - run: tox -e docs
         if: ${{ !inputs.publish }}
       - uses: actions/upload-artifact@v3
         with:
           name: html
           path: html/
 
       - uses: JamesIves/github-pages-deploy-action@v4.4.3
         if: ${{ inputs.publish }}
         with:
           branch: gh-pages
           folder: html
-          target-folder: ${{ env.target }}
           single-commit: true
           clean-exclude: release
           ssh-key: ${{ secrets.GH_PAGES_DEPLOY_KEY }}
```

### Comparing `sciline-0.0.1/.github/workflows/test.yml` & `sciline-0.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/.pre-commit-config.yaml` & `sciline-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/CONTRIBUTING.md` & `sciline-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/LICENSE` & `sciline-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/PKG-INFO` & `sciline-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciline
-Version: 0.0.1
+Version: 0.0.2
 Summary: Build scientific pipelines for your data
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
         All rights reserved.
```

### Comparing `sciline-0.0.1/conda/meta.yaml` & `sciline-0.0.2/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/docs/_static/favicon.ico` & `sciline-0.0.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/docs/_static/logo-dark.svg` & `sciline-0.0.2/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/docs/_static/logo.svg` & `sciline-0.0.2/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/docs/_templates/class-template.rst` & `sciline-0.0.2/docs/_templates/class-template.rst`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/docs/conf.py` & `sciline-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/docs/developer/coding-conventions.md` & `sciline-0.0.2/docs/developer/coding-conventions.md`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/docs/developer/dependency-management.md` & `sciline-0.0.2/docs/developer/dependency-management.md`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/docs/developer/getting-started.md` & `sciline-0.0.2/docs/developer/getting-started.md`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/docs/index.md` & `sciline-0.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/docs/user-guide/getting-started.ipynb` & `sciline-0.0.2/docs/user-guide/getting-started.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998976248976249%*

 * *Differences: {"'cells'": "{8: {'source': {insert: [(33, '   For example, we can be certain that we have cleaned "*

 * *            "our data, simply by depending on `CleanedData` in the next step.\\n')], delete: "*

 * *            '[33]}}}'}*

```diff
@@ -188,15 +188,15 @@
                 "   ```\n",
                 "\n",
                 "   The clearly converts `RawData` to `CleanedData`.\n",
                 "   If we want to understand how our data is cleaned, it is obvious that we have to look at this function.\n",
                 "   If we want to refine our cleaning procedure, it is obvious that we have to change or replace this provider.\n",
                 "2. Dependencies are resolved automatically.\n",
                 "   This means that we do not have to worry about the order of function calls or passing the wrong data to a function.\n",
-                "   For example, we can be certain that we have cleaned our data, simply by depending in `CleanedData` in the next step.\n",
+                "   For example, we can be certain that we have cleaned our data, simply by depending on `CleanedData` in the next step.\n",
                 "   We do not have to worry about variable or parameter naming, which is a common source of errors.\n",
                 "   Instead, dependencies are resolved by type.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `sciline-0.0.1/pyproject.toml` & `sciline-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/requirements/ci.txt` & `sciline-0.0.2/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/requirements/dev.txt` & `sciline-0.0.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/requirements/docs.txt` & `sciline-0.0.2/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/requirements/static.txt` & `sciline-0.0.2/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/requirements/test-dask.txt` & `sciline-0.0.2/requirements/test-dask.txt`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/resources/sciline.svg` & `sciline-0.0.2/resources/sciline.svg`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/src/sciline/__init__.py` & `sciline-0.0.2/src/sciline/__init__.py`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/src/sciline/domain.py` & `sciline-0.0.2/src/sciline/domain.py`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/src/sciline/pipeline.py` & `sciline-0.0.2/src/sciline/pipeline.py`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/src/sciline/scheduler.py` & `sciline-0.0.2/src/sciline/scheduler.py`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/src/sciline/task_graph.py` & `sciline-0.0.2/src/sciline/task_graph.py`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/src/sciline/visualize.py` & `sciline-0.0.2/src/sciline/visualize.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,13 +51,16 @@
     """
     Helper for _format_graph.
 
     If tp is a generic such as Array[float], we want to return 'Array[float]',
     but strip all module prefixes from the type name as well as the params.
     We may make this configurable in the future.
     """
-    base = tp.__name__ if hasattr(tp, '__name__') else str(tp).split('.')[-1]
-    if get_origin(tp) is not None:
+
+    def get_base(tp: type) -> str:
+        return tp.__name__ if hasattr(tp, '__name__') else str(tp).split('.')[-1]
+
+    if (origin := get_origin(tp)) is not None:
         params = [_format_type(param) for param in get_args(tp)]
-        return f'{base}[{", ".join(params)}]'
+        return f'{get_base(origin)}[{", ".join(params)}]'
     else:
-        return base
+        return get_base(tp)
```

### Comparing `sciline-0.0.1/src/sciline.egg-info/PKG-INFO` & `sciline-0.0.2/src/sciline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciline
-Version: 0.0.1
+Version: 0.0.2
 Summary: Build scientific pipelines for your data
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
         All rights reserved.
```

### Comparing `sciline-0.0.1/src/sciline.egg-info/SOURCES.txt` & `sciline-0.0.2/src/sciline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/tests/complex_workflow_test.py` & `sciline-0.0.2/tests/complex_workflow_test.py`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/tests/domain_test.py` & `sciline-0.0.2/tests/domain_test.py`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/tests/pipeline_test.py` & `sciline-0.0.2/tests/pipeline_test.py`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/tests/task_graph_test.py` & `sciline-0.0.2/tests/task_graph_test.py`

 * *Files identical despite different names*

### Comparing `sciline-0.0.1/tox.ini` & `sciline-0.0.2/tox.ini`

 * *Files identical despite different names*

