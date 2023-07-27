# Comparing `tmp/typeguard-4.0.0rc6.tar.gz` & `tmp/typeguard-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeguard-4.0.0rc6.tar", last modified: Sun May  7 10:35:57 2023, max compression
+gzip compressed data, was "typeguard-4.0.1.tar", last modified: Thu Jul 27 13:37:36 2023, max compression
```

## Comparing `typeguard-4.0.0rc6.tar` & `typeguard-4.0.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.707884 typeguard-4.0.0rc6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.695884 typeguard-4.0.0rc6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.699884 typeguard-4.0.0rc6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.github/ISSUE_TEMPLATE/features_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.699884 typeguard-4.0.0rc6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-07 10:35:57.707884 typeguard-4.0.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.699884 typeguard-4.0.0rc6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/extending.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 10:35:57.707884 typeguard-4.0.0rc6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.695884 typeguard-4.0.0rc6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.703884 typeguard-4.0.0rc6/src/typeguard/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26071 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)    41863 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.703884 typeguard-4.0.0rc6/src/typeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-07 10:35:57.000000 typeguard-4.0.0rc6/src/typeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-07 10:35:57.000000 typeguard-4.0.0rc6/src/typeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 10:35:57.000000 typeguard-4.0.0rc6/src/typeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-07 10:35:57.000000 typeguard-4.0.0rc6/src/typeguard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-07 10:35:57.000000 typeguard-4.0.0rc6/src/typeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 10:35:57.000000 typeguard-4.0.0rc6/src/typeguard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.707884 typeguard-4.0.0rc6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/dummymodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.707884 typeguard-4.0.0rc6/tests/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/mypy/negative.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/mypy/positive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/mypy/test_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    31816 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_instrumentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)    43600 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16646 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_typechecked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_warn_on_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.232788 typeguard-4.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.224788 typeguard-4.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.224788 typeguard-4.0.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-27 13:37:26.000000 typeguard-4.0.1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 13:37:26.000000 typeguard-4.0.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-27 13:37:26.000000 typeguard-4.0.1/.github/ISSUE_TEMPLATE/features_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.224788 typeguard-4.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-27 13:37:26.000000 typeguard-4.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-27 13:37:26.000000 typeguard-4.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-27 13:37:26.000000 typeguard-4.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-27 13:37:26.000000 typeguard-4.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-27 13:37:26.000000 typeguard-4.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-27 13:37:26.000000 typeguard-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-27 13:37:36.232788 typeguard-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-27 13:37:26.000000 typeguard-4.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.228788 typeguard-4.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19756 2023-07-27 13:37:26.000000 typeguard-4.0.1/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-27 13:37:26.000000 typeguard-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:37:36.232788 typeguard-4.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.224788 typeguard-4.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.228788 typeguard-4.0.1/src/typeguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27389 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43580 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:26.000000 typeguard-4.0.1/src/typeguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.228788 typeguard-4.0.1/src/typeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-27 13:37:36.000000 typeguard-4.0.1/src/typeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-27 13:37:36.000000 typeguard-4.0.1/src/typeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:37:36.000000 typeguard-4.0.1/src/typeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-27 13:37:36.000000 typeguard-4.0.1/src/typeguard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 13:37:36.000000 typeguard-4.0.1/src/typeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 13:37:36.000000 typeguard-4.0.1/src/typeguard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.232788 typeguard-4.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/dummymodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:36.232788 typeguard-4.0.1/tests/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/mypy/negative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/mypy/positive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/mypy/test_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32870 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44319 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_typechecked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 13:37:26.000000 typeguard-4.0.1/tests/test_warn_on_error.py
```

### Comparing `typeguard-4.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.yaml` & `typeguard-4.0.1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/.github/ISSUE_TEMPLATE/features_request.yaml` & `typeguard-4.0.1/.github/ISSUE_TEMPLATE/features_request.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/.github/workflows/publish.yml` & `typeguard-4.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/.github/workflows/test.yml` & `typeguard-4.0.1/.github/workflows/test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,23 @@
   pull_request:
 
 jobs:
   test:
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", pypy-3.9]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12", pypy-3.9]
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+        allow-prereleases: true
         cache: pip
         cache-dependency-path: pyproject.toml
     - name: Install dependencies
       run: pip install -e .[test] coveralls coverage[toml]
     - name: Test with pytest
       run: coverage run -m pytest
     - name: Upload Coverage
```

### Comparing `typeguard-4.0.0rc6/.pre-commit-config.yaml` & `typeguard-4.0.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+    rev: v0.0.280
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
 
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
         exclude: "^tests/mypy/negative.py"
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         additional_dependencies: [ "typing_extensions" ]
         exclude: "^tests/"
```

### Comparing `typeguard-4.0.0rc6/LICENSE` & `typeguard-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/PKG-INFO` & `typeguard-4.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.0.0rc6
+Version: 4.0.1
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7.4
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 .. image:: https://github.com/agronholm/typeguard/actions/workflows/test.yml/badge.svg
```

### Comparing `typeguard-4.0.0rc6/README.rst` & `typeguard-4.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/docs/api.rst` & `typeguard-4.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/docs/conf.py` & `typeguard-4.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/docs/contributing.rst` & `typeguard-4.0.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/docs/extending.rst` & `typeguard-4.0.1/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/docs/features.rst` & `typeguard-4.0.1/docs/features.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/docs/userguide.rst` & `typeguard-4.0.1/docs/userguide.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/docs/versionhistory.rst` & `typeguard-4.0.1/docs/versionhistory.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,31 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <https://semver.org/#semantic-versioning-200>`_.
 
+**4.0.1** (2023-07-27)
+
+- Fixed handling of ``typing_extensions.Literal`` on Python 3.8 and 3.9 when
+  ``typing_extensions>=4.6.0`` is installed
+  (`#363 <https://github.com/agronholm/typeguard/issues/363>`_; PR by Alex Waygood)
+- Fixed ``NameError`` when generated type checking code references an imported name from
+  a method (`#362 <https://github.com/agronholm/typeguard/issues/362>`_)
+- Fixed docstrings disappearing from instrumented functions
+  (`#359 <https://github.com/agronholm/typeguard/issues/359>`_)
+- Fixed ``@typechecked`` failing to instrument functions when there are more than one
+  function within the same scope
+  (`#355 <https://github.com/agronholm/typeguard/issues/355>`_)
+- Fixed ``frozenset`` not being checked
+  (`#367 <https://github.com/agronholm/typeguard/issues/367>`_)
+
+**4.0.0** (2023-05-12)
+
+- No changes
+
 **4.0.0rc6** (2023-05-07)
 
 - Fixed ``@typechecked`` optimization causing compilation of instrumented code to fail
   when an ``if`` block was left empty by the AST transformer
   (`#352 <https://github.com/agronholm/typeguard/issues/352>`_)
 - Fixed the AST transformer trying to parse the second argument of ``typing.Annotated``
   as a forward reference (`#353 <https://github.com/agronholm/typeguard/issues/353>`_)
```

### Comparing `typeguard-4.0.0rc6/pyproject.toml` & `typeguard-4.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,20 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">= 3.7.4"
 dependencies = [
     "importlib_metadata >= 3.6; python_version < '3.10'",
-    "typing_extensions >= 4.4.0; python_version < '3.11'",
+    "typing_extensions >= 4.7.0; python_version < '3.12'",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://typeguard.readthedocs.io/en/latest/"
 "Change log" = "https://typeguard.readthedocs.io/en/latest/versionhistory.html"
 "Source code" = "https://github.com/agronholm/typeguard"
@@ -39,14 +40,15 @@
 [project.optional-dependencies]
 test = [
     "pytest >= 7",
     'mypy >= 1.2.0; python_implementation != "PyPy"',
 ]
 doc = [
     "packaging",
+    "Sphinx < 7",
     "sphinx_rtd_theme",
     "sphinx-autodoc-typehints >= 1.2.0",
 ]
 
 [project.entry-points]
 pytest11 = {typeguard = "typeguard._pytest_plugin"}
 
@@ -93,15 +95,15 @@
 python_version = "3.9"
 strict = true
 pretty = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = pypy3, py37, py38, py39, py310, py311
+envlist = pypy3, py37, py38, py39, py310, py311, py312
 skip_missing_interpreters = true
 minversion = 4.0
 
 [testenv]
 extras = test
 commands = python -m pytest {posargs}
```

### Comparing `typeguard-4.0.0rc6/src/typeguard/__init__.py` & `typeguard-4.0.1/src/typeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/src/typeguard/_checkers.py` & `typeguard-4.0.1/src/typeguard/_checkers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import collections.abc
 import inspect
 import sys
 import types
+import typing
 import warnings
 from enum import Enum
 from inspect import Parameter, isclass, isfunction
 from io import BufferedIOBase, IOBase, RawIOBase, TextIOBase
 from textwrap import indent
 from typing import (
     IO,
@@ -28,42 +29,39 @@
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 from unittest.mock import Mock
 
+try:
+    import typing_extensions
+except ImportError:
+    typing_extensions = None  # type: ignore[assignment]
+
 from ._config import ForwardRefPolicy
 from ._exceptions import TypeCheckError, TypeHintWarning
 from ._memo import TypeCheckMemo
 from ._utils import evaluate_forwardref, get_stacklevel, get_type_name, qualified_name
 
 if sys.version_info >= (3, 11):
     from typing import (
         Annotated,
-        Literal,
-        LiteralString,
-        Self,
         TypeAlias,
-        TypeGuard,
         get_args,
         get_origin,
         get_type_hints,
         is_typeddict,
     )
 
     SubclassableAny = Any
 else:
     from typing_extensions import (
         Annotated,
-        Literal,
-        LiteralString,
-        Self,
         TypeAlias,
-        TypeGuard,
         get_args,
         get_origin,
         get_type_hints,
         is_typeddict,
     )
     from typing_extensions import Any as SubclassableAny
 
@@ -314,15 +312,18 @@
 
 def check_set(
     value: Any,
     origin_type: Any,
     args: tuple[Any, ...],
     memo: TypeCheckMemo,
 ) -> None:
-    if not isinstance(value, AbstractSet):
+    if origin_type is frozenset:
+        if not isinstance(value, frozenset):
+            raise TypeCheckError("is not a frozenset")
+    elif not isinstance(value, AbstractSet):
         raise TypeCheckError("is not a set")
 
     if args and args != (Any,):
         samples = memo.config.collection_check_strategy.iterate_samples(value)
         for v in samples:
             try:
                 check_type_internal(v, args[0], memo)
@@ -526,24 +527,41 @@
                 get_type_name(constraint) for constraint in origin_type.__constraints__
             )
             raise TypeCheckError(
                 f"does not match any of the constraints " f"({formatted_constraints})"
             )
 
 
+if sys.version_info >= (3, 8):
+    if typing_extensions is None:
+
+        def _is_literal_type(typ: object) -> bool:
+            return typ is typing.Literal
+
+    else:
+
+        def _is_literal_type(typ: object) -> bool:
+            return typ is typing.Literal or typ is typing_extensions.Literal
+
+else:
+
+    def _is_literal_type(typ: object) -> bool:
+        return typ is typing_extensions.Literal
+
+
 def check_literal(
     value: Any,
     origin_type: Any,
     args: tuple[Any, ...],
     memo: TypeCheckMemo,
 ) -> None:
     def get_literal_args(literal_args: tuple[Any, ...]) -> tuple[Any, ...]:
         retval: list[Any] = []
         for arg in literal_args:
-            if get_origin(arg) is Literal:
+            if _is_literal_type(get_origin(arg)):
                 # The first check works on py3.6 and lower, the second one on py3.7+
                 retval.extend(get_literal_args(arg.__args__))
             elif arg is None or isinstance(arg, (int, str, bytes, bool, Enum)):
                 retval.append(arg)
             else:
                 raise TypeError(
                     f"Illegal literal value: {arg}"
@@ -775,40 +793,54 @@
     BinaryIO: check_io,
     Callable: check_callable,
     collections.abc.Callable: check_callable,
     complex: check_number,
     dict: check_mapping,
     Dict: check_mapping,
     float: check_number,
+    frozenset: check_set,
     IO: check_io,
     list: check_list,
     List: check_list,
-    Literal: check_literal,
-    LiteralString: check_literal_string,
     Mapping: check_mapping,
     MutableMapping: check_mapping,
     None: check_none,
     collections.abc.Mapping: check_mapping,
     collections.abc.MutableMapping: check_mapping,
-    Self: check_self,
     Sequence: check_sequence,
     collections.abc.Sequence: check_sequence,
     collections.abc.Set: check_set,
     set: check_set,
     Set: check_set,
     TextIO: check_io,
     tuple: check_tuple,
     Tuple: check_tuple,
     type: check_class,
     Type: check_class,
-    TypeGuard: check_typeguard,
     Union: check_union,
 }
+if sys.version_info >= (3, 8):
+    origin_type_checkers[typing.Literal] = check_literal
 if sys.version_info >= (3, 10):
     origin_type_checkers[types.UnionType] = check_uniontype
+    origin_type_checkers[typing.TypeGuard] = check_typeguard
+if sys.version_info >= (3, 11):
+    origin_type_checkers.update(
+        {typing.LiteralString: check_literal_string, typing.Self: check_self}
+    )
+if typing_extensions is not None:
+    # On some Python versions, these may simply be re-exports from typing,
+    # but exactly which Python versions is subject to change,
+    # so it's best to err on the safe side
+    # and update the dictionary on all Python versions
+    # if typing_extensions is installed
+    origin_type_checkers[typing_extensions.Literal] = check_literal
+    origin_type_checkers[typing_extensions.LiteralString] = check_literal_string
+    origin_type_checkers[typing_extensions.Self] = check_self
+    origin_type_checkers[typing_extensions.TypeGuard] = check_typeguard
 
 
 def builtin_checker_lookup(
     origin_type: Any, args: tuple[Any, ...], extras: tuple[Any, ...]
 ) -> TypeCheckerCallable | None:
     checker = origin_type_checkers.get(origin_type)
     if checker is not None:
```

### Comparing `typeguard-4.0.0rc6/src/typeguard/_config.py` & `typeguard-4.0.1/src/typeguard/_config.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/src/typeguard/_decorators.py` & `typeguard-4.0.1/src/typeguard/_decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import ast
 import inspect
 import sys
+from collections.abc import Sequence
 from functools import partial
 from inspect import isclass, isfunction
 from types import CodeType, FrameType, FunctionType
 from typing import TYPE_CHECKING, Any, Callable, ForwardRef, TypeVar, cast, overload
 from warnings import warn
 
 from ._config import CollectionCheckStrategy, ForwardRefPolicy, global_config
@@ -30,14 +31,33 @@
 T_CallableOrType = TypeVar("T_CallableOrType", bound=Callable[..., Any])
 
 
 def make_cell(value: object) -> _Cell:
     return (lambda: value).__closure__[0]  # type: ignore[index]
 
 
+def find_target_function(
+    new_code: CodeType, target_path: Sequence[str], firstlineno: int
+) -> CodeType | None:
+    target_name = target_path[0]
+    for const in new_code.co_consts:
+        if isinstance(const, CodeType):
+            if const.co_name == target_name:
+                if const.co_firstlineno == firstlineno:
+                    return const
+                elif len(target_path) > 1:
+                    target_code = find_target_function(
+                        const, target_path[1:], firstlineno
+                    )
+                    if target_code:
+                        return target_code
+
+    return None
+
+
 def instrument(f: T_CallableOrType) -> FunctionType | str:
     if not getattr(f, "__code__", None):
         return "no code associated"
     elif not getattr(f, "__module__", None):
         return "__module__ attribute is not set"
     elif f.__code__.co_filename == "<stdin>":
         return "cannot instrument functions defined in a REPL"
@@ -46,47 +66,39 @@
             "@typechecked only supports instrumenting functions wrapped with "
             "@classmethod, @staticmethod or @property"
         )
 
     target_path = [item for item in f.__qualname__.split(".") if item != "<locals>"]
     module_source = inspect.getsource(sys.modules[f.__module__])
     module_ast = ast.parse(module_source)
-    instrumentor = TypeguardTransformer(target_path)
+    instrumentor = TypeguardTransformer(target_path, f.__code__.co_firstlineno)
     instrumentor.visit(module_ast)
 
-    if global_config.debug_instrumentation and sys.version_info >= (3, 9):
-        # Find the matching AST node, then unparse it to source and print to stdout
-        level = 0
-        for node in ast.walk(module_ast):
-            if isinstance(node, (ast.ClassDef, ast.FunctionDef)):
-                if node.name == target_path[level]:
-                    if level == len(target_path) - 1:
-                        print(
-                            f"Source code of {f.__qualname__}() after instrumentation:"
-                            "\n----------------------------------------------",
-                            file=sys.stderr,
-                        )
-                        print(ast.unparse(node), file=sys.stderr)
-                        print(
-                            "----------------------------------------------",
-                            file=sys.stderr,
-                        )
-                    else:
-                        level += 1
+    if not instrumentor.target_node or instrumentor.target_lineno is None:
+        return "instrumentor did not find the target function"
 
     module_code = compile(module_ast, f.__code__.co_filename, "exec", dont_inherit=True)
-    new_code = module_code
-    for name in target_path:
-        for const in new_code.co_consts:
-            if isinstance(const, CodeType):
-                if const.co_name == name:
-                    new_code = const
-                    break
-        else:
-            return "cannot find the target function in the AST"
+    new_code = find_target_function(
+        module_code, target_path, instrumentor.target_lineno
+    )
+    if not new_code:
+        return "cannot find the target function in the AST"
+
+    if global_config.debug_instrumentation and sys.version_info >= (3, 9):
+        # Find the matching AST node, then unparse it to source and print to stdout
+        print(
+            f"Source code of {f.__qualname__}() after instrumentation:"
+            "\n----------------------------------------------",
+            file=sys.stderr,
+        )
+        print(ast.unparse(instrumentor.target_node), file=sys.stderr)
+        print(
+            "----------------------------------------------",
+            file=sys.stderr,
+        )
 
     closure = f.__closure__
     if new_code.co_freevars != f.__code__.co_freevars:
         # Create a new closure and find values for the new free variables
         frame = cast(FrameType, inspect.currentframe())
         frame = cast(FrameType, frame.f_back)
         frame_locals = cast(FrameType, frame.f_back).f_locals
```

### Comparing `typeguard-4.0.0rc6/src/typeguard/_exceptions.py` & `typeguard-4.0.1/src/typeguard/_exceptions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/src/typeguard/_functions.py` & `typeguard-4.0.1/src/typeguard/_functions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/src/typeguard/_importhook.py` & `typeguard-4.0.1/src/typeguard/_importhook.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,41 +6,35 @@
 from collections.abc import Callable, Iterable
 from importlib.abc import MetaPathFinder
 from importlib.machinery import ModuleSpec, SourceFileLoader
 from importlib.util import cache_from_source, decode_source
 from inspect import isclass
 from os import PathLike
 from types import CodeType, ModuleType, TracebackType
-from typing import TYPE_CHECKING, Any, Sequence, TypeVar
+from typing import Sequence, TypeVar
 from unittest.mock import patch
 
 from ._config import global_config
 from ._transformer import TypeguardTransformer
 
+if sys.version_info >= (3, 12):
+    from collections.abc import Buffer
+else:
+    from typing_extensions import Buffer
+
 if sys.version_info >= (3, 11):
     from typing import ParamSpec
 else:
     from typing_extensions import ParamSpec
 
 if sys.version_info >= (3, 10):
     from importlib.metadata import PackageNotFoundError, version
 else:
     from importlib_metadata import PackageNotFoundError, version
 
-if TYPE_CHECKING:
-    from array import array
-    from mmap import mmap
-    from pickle import PickleBuffer
-
-    # This is guarded because sphinx-autodoc-typehints tries to import these
-    try:
-        from ctypes import _CData
-    except ImportError:
-        pass
-
 try:
     OPTIMIZATION = "typeguard" + "".join(version("typeguard").split(".")[:3])
 except PackageNotFoundError:
     OPTIMIZATION = "typeguard"
 
 P = ParamSpec("P")
 T = TypeVar("T")
@@ -56,34 +50,16 @@
 def optimized_cache_from_source(path: str, debug_override: bool | None = None) -> str:
     return cache_from_source(path, debug_override, optimization=OPTIMIZATION)
 
 
 class TypeguardLoader(SourceFileLoader):
     @staticmethod
     def source_to_code(
-        data: bytes
-        | bytearray
-        | memoryview
-        | array[Any]
-        | mmap
-        | _CData
-        | PickleBuffer
-        | str
-        | ast.Module
-        | ast.Expression
-        | ast.Interactive,
-        path: bytes
-        | bytearray
-        | memoryview
-        | array[Any]
-        | mmap
-        | _CData
-        | PickleBuffer
-        | str
-        | PathLike[str] = "<string>",
+        data: Buffer | str | ast.Module | ast.Expression | ast.Interactive,
+        path: Buffer | str | PathLike[str] = "<string>",
     ) -> CodeType:
         if isinstance(data, (ast.Module, ast.Expression, ast.Interactive)):
             tree = data
         else:
             if isinstance(data, str):
                 source = data
             else:
```

### Comparing `typeguard-4.0.0rc6/src/typeguard/_memo.py` & `typeguard-4.0.1/src/typeguard/_memo.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/src/typeguard/_pytest_plugin.py` & `typeguard-4.0.1/src/typeguard/_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/src/typeguard/_suppression.py` & `typeguard-4.0.1/src/typeguard/_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/src/typeguard/_transformer.py` & `typeguard-4.0.1/src/typeguard/_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import ast
 import builtins
 import sys
+import typing
 from ast import (
     AST,
     Add,
     AnnAssign,
     Assign,
     AsyncFunctionDef,
     Attribute,
@@ -132,14 +133,15 @@
     )
     has_yield_expressions: bool = field(init=False, default=False)
     has_return_expressions: bool = field(init=False, default=False)
     memo_var_name: Name | None = field(init=False, default=None)
     should_instrument: bool = field(init=False, default=True)
     variable_annotations: dict[str, expr] = field(init=False, default_factory=dict)
     configuration_overrides: dict[str, Any] = field(init=False, default_factory=dict)
+    code_inject_index: int = field(init=False, default=0)
 
     def __post_init__(self) -> None:
         elements: list[str] = []
         memo = self
         while isinstance(memo.node, (ClassDef, FunctionDef, AsyncFunctionDef)):
             elements.insert(0, memo.node.name)
             if not memo.parent:
@@ -147,14 +149,31 @@
 
             memo = memo.parent
             if isinstance(memo.node, (FunctionDef, AsyncFunctionDef)):
                 elements.insert(0, "<locals>")
 
         self.joined_path = Constant(".".join(elements))
 
+        # Figure out where to insert instrumentation code
+        if self.node:
+            for index, child in enumerate(self.node.body):
+                if isinstance(child, ImportFrom) and child.module == "__future__":
+                    # (module only) __future__ imports must come first
+                    continue
+                elif isinstance(child, Expr):
+                    if isinstance(child.value, Constant) and isinstance(
+                        child.value.value, str
+                    ):
+                        continue  # docstring
+                    elif sys.version_info < (3, 8) and isinstance(child.value, Str):
+                        continue  # docstring
+
+                self.code_inject_index = index
+                break
+
     def get_unused_name(self, name: str) -> str:
         memo: TransformMemo | None = self
         while memo is not None:
             if name in memo.local_names:
                 memo = self
                 name += "_"
             else:
@@ -207,28 +226,20 @@
 
     def insert_imports(self, node: Module | FunctionDef | AsyncFunctionDef) -> None:
         """Insert imports needed by injected code."""
         if not self.load_names:
             return
 
         # Insert imports after any "from __future__ ..." imports and any docstring
-        for i, child in enumerate(node.body):
-            if isinstance(child, ImportFrom) and child.module == "__future__":
-                continue
-            elif isinstance(child, Expr) and isinstance(child.value, Str):
-                continue  # module docstring
-
-            for modulename, names in self.load_names.items():
-                aliases = [
-                    alias(orig_name, new_name.id if orig_name != new_name.id else None)
-                    for orig_name, new_name in sorted(names.items())
-                ]
-                node.body.insert(i, ImportFrom(modulename, aliases, 0))
-
-            break
+        for modulename, names in self.load_names.items():
+            aliases = [
+                alias(orig_name, new_name.id if orig_name != new_name.id else None)
+                for orig_name, new_name in sorted(names.items())
+            ]
+            node.body.insert(self.code_inject_index, ImportFrom(modulename, aliases, 0))
 
     def name_matches(self, expression: expr | Expr | None, *names: str) -> bool:
         if expression is None:
             return False
 
         path: list[str] = []
         top_expression = (
@@ -391,22 +402,31 @@
             else:
                 slice_value = node.slice
 
             if isinstance(slice_value, Tuple):
                 if self._memo.name_matches(node.value, *annotated_names):
                     # Only treat the first argument to typing.Annotated as a potential
                     # forward reference
-                    items = [self.visit(slice_value.elts[0])] + slice_value.elts[1:]
+                    items = cast(
+                        typing.List[expr],
+                        [self.generic_visit(slice_value.elts[0])]
+                        + slice_value.elts[1:],
+                    )
                 else:
-                    items = [self.visit(item) for item in slice_value.elts]
+                    items = cast(
+                        typing.List[expr],
+                        [self.generic_visit(item) for item in slice_value.elts],
+                    )
 
-                # If this is a Union and any of the items is None, erase the entire
+                # If this is a Union and any of the items is Any, erase the entire
                 # annotation
                 if self._memo.name_matches(node.value, "typing.Union") and any(
-                    item is None for item in items
+                    isinstance(item, expr)
+                    and self._memo.name_matches(item, *anytype_names)
+                    for item in items
                 ):
                     return None
 
                 # If all items in the subscript were Any, erase the subscript entirely
                 if all(item is None for item in items):
                     return node.value
 
@@ -464,18 +484,22 @@
         if new_node:
             return copy_location(new_node.body, node)
         else:
             return None
 
 
 class TypeguardTransformer(NodeTransformer):
-    def __init__(self, target_path: Sequence[str] | None = None) -> None:
+    def __init__(
+        self, target_path: Sequence[str] | None = None, target_lineno: int | None = None
+    ) -> None:
         self._target_path = tuple(target_path) if target_path else None
         self._memo = self._module_memo = TransformMemo(None, None, ())
         self.names_used_in_annotations: set[str] = set()
+        self.target_node: FunctionDef | AsyncFunctionDef | None = None
+        self.target_lineno = target_lineno
 
     @contextmanager
     def _use_memo(
         self, node: ClassDef | FunctionDef | AsyncFunctionDef
     ) -> Generator[None, Any, None]:
         new_memo = TransformMemo(node, self._memo, self._memo.path + (node.name,))
         if isinstance(node, (FunctionDef, AsyncFunctionDef)):
@@ -640,28 +664,42 @@
             for decorator in node.decorator_list:
                 if self._memo.name_matches(decorator, *ignore_decorators):
                     return node
 
         with self._use_memo(node):
             arg_annotations: dict[str, Any] = {}
             if self._target_path is None or self._memo.path == self._target_path:
+                # Find line number we're supposed to match against
+                if node.decorator_list:
+                    first_lineno = node.decorator_list[0].lineno
+                else:
+                    first_lineno = node.lineno
+
                 for decorator in node.decorator_list.copy():
                     if self._memo.name_matches(decorator, "typing.overload"):
                         # Remove overloads entirely
                         return None
                     elif self._memo.name_matches(decorator, "typeguard.typechecked"):
                         # Remove the decorator to prevent duplicate instrumentation
                         node.decorator_list.remove(decorator)
 
                         # Store any configuration overrides
                         if isinstance(decorator, Call) and decorator.keywords:
                             self._memo.configuration_overrides = {
                                 kw.arg: kw.value for kw in decorator.keywords if kw.arg
                             }
 
+                if self.target_lineno == first_lineno:
+                    assert self.target_node is None
+                    self.target_node = node
+                    if node.decorator_list and sys.version_info >= (3, 8):
+                        self.target_lineno = node.decorator_list[0].lineno
+                    else:
+                        self.target_lineno = node.lineno
+
                 all_args = node.args.args + node.args.kwonlyargs
                 if sys.version_info >= (3, 8):
                     all_args.extend(node.args.posonlyargs)
 
                 # Ensure that any type shadowed by the positional or keyword-only
                 # argument names are ignored in this function
                 for arg in all_args:
@@ -743,15 +781,17 @@
                     "typeguard._functions", "check_argument_types"
                 )
                 args = [
                     self._memo.joined_path,
                     annotations_dict,
                     self._memo.get_memo_name(),
                 ]
-                node.body.insert(0, Expr(Call(func_name, args, [])))
+                node.body.insert(
+                    self._memo.code_inject_index, Expr(Call(func_name, args, []))
+                )
 
             # Add a checked "return None" to the end if there's no explicit return
             # Skip if the return annotation is None or Any
             if (
                 self._memo.return_annotation
                 and (not self._memo.is_async or not self._memo.has_yield_expressions)
                 and not isinstance(node.body[-1], Return)
@@ -845,15 +885,15 @@
                 locals_call = Call(Name(id="locals", ctx=Load()), [], [])
                 memo_expr = Call(
                     self._get_import("typeguard", "TypeCheckMemo"),
                     [globals_call, locals_call],
                     [keyword(key, value) for key, value in memo_kwargs.items()],
                 )
                 node.body.insert(
-                    0,
+                    self._memo.code_inject_index,
                     Assign([memo_store_name], memo_expr),
                 )
 
                 self._memo.insert_imports(node)
 
                 # Rmove any placeholder "pass" at the end
                 if isinstance(node.body[-1], Pass):
@@ -898,15 +938,14 @@
         This injects type checks into "yield" expressions, checking both the yielded
         value and the value sent back to the generator, when appropriate.
 
         """
         self._memo.has_yield_expressions = True
         self.generic_visit(node)
 
-        self.generic_visit(node)
         if (
             self._memo.yield_annotation
             and self._memo.should_instrument
             and not self._memo.is_ignored_name(self._memo.yield_annotation)
         ):
             func_name = self._get_import("typeguard._functions", "check_yield_type")
             yieldval = node.value or Constant(None)
```

### Comparing `typeguard-4.0.0rc6/src/typeguard/_union_transformer.py` & `typeguard-4.0.1/src/typeguard/_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/src/typeguard/_utils.py` & `typeguard-4.0.1/src/typeguard/_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/src/typeguard.egg-info/PKG-INFO` & `typeguard-4.0.1/src/typeguard.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.0.0rc6
+Version: 4.0.1
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7.4
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 .. image:: https://github.com/agronholm/typeguard/actions/workflows/test.yml/badge.svg
```

### Comparing `typeguard-4.0.0rc6/src/typeguard.egg-info/SOURCES.txt` & `typeguard-4.0.1/src/typeguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/__init__.py` & `typeguard-4.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/conftest.py` & `typeguard-4.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/dummymodule.py` & `typeguard-4.0.1/tests/dummymodule.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/mypy/negative.py` & `typeguard-4.0.1/tests/mypy/negative.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/mypy/positive.py` & `typeguard-4.0.1/tests/mypy/positive.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/mypy/test_type_annotations.py` & `typeguard-4.0.1/tests/mypy/test_type_annotations.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/test_checkers.py` & `typeguard-4.0.1/tests/test_checkers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     AnyStr,
     BinaryIO,
     Callable,
     Collection,
     ContextManager,
     Dict,
     ForwardRef,
+    FrozenSet,
     Iterator,
     List,
     Mapping,
     MutableMapping,
     Optional,
     Sequence,
     Set,
@@ -602,14 +603,46 @@
             check_type,
             {1, 2, "bb"},
             Set[int],
             collection_check_strategy=CollectionCheckStrategy.ALL_ITEMS,
         ).match("set is not an instance of int")
 
 
+class TestFrozenSet:
+    def test_bad_type(self):
+        pytest.raises(TypeCheckError, check_type, 5, FrozenSet[int]).match(
+            "int is not a frozenset"
+        )
+
+    def test_valid(self):
+        check_type(frozenset({1, 2}), FrozenSet[int])
+
+    def test_first_check_empty(self):
+        check_type(frozenset(), FrozenSet[int])
+
+    def test_first_check_fail(self, sample_set: set):
+        pytest.raises(
+            TypeCheckError, check_type, frozenset(sample_set), FrozenSet[int]
+        ).match("set is not an instance of int")
+
+    def test_full_check_fail(self):
+        pytest.raises(
+            TypeCheckError,
+            check_type,
+            frozenset({1, 2, "bb"}),
+            FrozenSet[int],
+            collection_check_strategy=CollectionCheckStrategy.ALL_ITEMS,
+        ).match("set is not an instance of int")
+
+    def test_set_against_frozenset(self, sample_set: set):
+        pytest.raises(TypeCheckError, check_type, sample_set, FrozenSet[int]).match(
+            "set is not a frozenset"
+        )
+
+
 @pytest.mark.parametrize(
     "annotated_type",
     [
         pytest.param(Tuple, id="typing"),
         pytest.param(
             tuple,
             id="builtin",
```

### Comparing `typeguard-4.0.0rc6/tests/test_importhook.py` & `typeguard-4.0.1/tests/test_importhook.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/test_instrumentation.py` & `typeguard-4.0.1/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/test_plugins.py` & `typeguard-4.0.1/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/test_suppression.py` & `typeguard-4.0.1/tests/test_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/test_transformer.py` & `typeguard-4.0.1/tests/test_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1517,7 +1517,34 @@
                 from typeguard import TypeCheckMemo
                 from typeguard._functions import check_argument_types
                 memo = TypeCheckMemo(globals(), locals())
                 check_argument_types('foo', {'x': (x, Annotated[str, 'foo bar'])}, memo)
             """
         ).strip()
     )
+
+
+def test_respect_docstring() -> None:
+    # Regression test for #359
+    node = parse(
+        dedent(
+            '''
+            def foo() -> int:
+                """This is a docstring."""
+                return 1
+            '''
+        )
+    )
+    TypeguardTransformer(["foo"]).visit(node)
+    assert (
+        unparse(node)
+        == dedent(
+            '''
+            def foo() -> int:
+                """This is a docstring."""
+                from typeguard import TypeCheckMemo
+                from typeguard._functions import check_return_type
+                memo = TypeCheckMemo(globals(), locals())
+                return check_return_type('foo', 1, int, memo)
+            '''
+        ).strip()
+    )
```

### Comparing `typeguard-4.0.0rc6/tests/test_typechecked.py` & `typeguard-4.0.1/tests/test_typechecked.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from textwrap import dedent
 from typing import (
     Any,
     AsyncGenerator,
     AsyncIterable,
     AsyncIterator,
+    Dict,
     Generator,
     Iterable,
     Iterator,
     List,
 )
 from unittest.mock import Mock
 
@@ -618,7 +619,54 @@
     )
     assert process.returncode == expected_return_code
     if process.returncode == 1:
         assert process.stderr.endswith(
             b'typeguard.TypeCheckError: argument "x" (str) is not an instance of '
             b"int\n"
         )
+
+
+def test_reference_imported_name_from_method() -> None:
+    # Regression test for #362
+    @typechecked
+    class A:
+        def foo(self) -> Dict[str, Any]:
+            return {}
+
+    A().foo()
+
+
+def test_getter_setter():
+    """Regression test for #355."""
+
+    @typechecked
+    class Foo:
+        def __init__(self, x: int):
+            self._x = x
+
+        @property
+        def x(self) -> int:
+            return self._x
+
+        @x.setter
+        def x(self, value: int) -> None:
+            self._x = value
+
+    f = Foo(1)
+    f.x = 2
+    assert f.x == 2
+    with pytest.raises(TypeCheckError):
+        f.x = "foo"
+
+
+def test_duplicate_method():
+    class Foo:
+        def x(self) -> str:
+            return "first"
+
+        @typechecked()
+        def x(self, value: int) -> str:  # noqa: F811
+            return "second"
+
+    assert Foo().x(1) == "second"
+    with pytest.raises(TypeCheckError):
+        Foo().x("wrong")
```

### Comparing `typeguard-4.0.0rc6/tests/test_union_transformer.py` & `typeguard-4.0.1/tests/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/test_utils.py` & `typeguard-4.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc6/tests/test_warn_on_error.py` & `typeguard-4.0.1/tests/test_warn_on_error.py`

 * *Files identical despite different names*

