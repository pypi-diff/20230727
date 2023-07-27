# Comparing `tmp/hankel-1.2.1.tar.gz` & `tmp/hankel-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hankel-1.2.1.tar", last modified: Fri Apr 29 22:23:31 2022, max compression
+gzip compressed data, was "hankel-1.2.2.tar", last modified: Thu Jul 27 13:36:31 2023, max compression
```

## Comparing `hankel-1.2.1.tar` & `hankel-1.2.2.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 22:23:31.765997 hankel-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-04-29 22:23:20.000000 hankel-1.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 22:23:31.753997 hankel-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 22:23:31.753997 hankel-1.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-04-29 22:23:20.000000 hankel-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-04-29 22:23:20.000000 hankel-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-04-29 22:23:20.000000 hankel-1.2.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-04-29 22:23:20.000000 hankel-1.2.1/.github/dependabot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 22:23:31.753997 hankel-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-04-29 22:23:20.000000 hankel-1.2.1/.github/workflows/deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-04-29 22:23:20.000000 hankel-1.2.1/.github/workflows/test_suite.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-04-29 22:23:20.000000 hankel-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-04-29 22:23:20.000000 hankel-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-04-29 22:23:20.000000 hankel-1.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-04-29 22:23:20.000000 hankel-1.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4799 2022-04-29 22:23:20.000000 hankel-1.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4368 2022-04-29 22:23:20.000000 hankel-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-04-29 22:23:20.000000 hankel-1.2.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-04-29 22:23:20.000000 hankel-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5135 2022-04-29 22:23:31.765997 hankel-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3586 2022-04-29 22:23:20.000000 hankel-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 22:23:31.761997 hankel-1.2.1/devel/
--rw-r--r--   0 runner    (1001) docker     (121)  5483604 2022-04-29 22:23:20.000000 hankel-1.2.1/devel/stepsizes_for_fourier.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)  1568119 2022-04-29 22:23:20.000000 hankel-1.2.1/devel/stepsizes_for_integrals.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   535941 2022-04-29 22:23:20.000000 hankel-1.2.1/devel/stepsizes_for_transforms.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 22:23:31.761997 hankel-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5458 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 22:23:31.765997 hankel-1.2.1/docs/demos/
--rw-r--r--   0 runner    (1001) docker     (121)   131461 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/demos/choosing_resolution_parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    39996 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/demos/getting_started.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   422322 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/demos/laplacian_hankel_vs_fft.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   250443 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/demos/paper_plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    99368 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/demos/testing_forward_and_inverse_transforms.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/example_toc.rst
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 22:23:31.765997 hankel-1.2.1/docs/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-04-29 22:23:20.000000 hankel-1.2.1/docs/templates/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 22:23:31.765997 hankel-1.2.1/hankel/
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-04-29 22:23:20.000000 hankel-1.2.1/hankel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-04-29 22:23:30.000000 hankel-1.2.1/hankel/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    16574 2022-04-29 22:23:20.000000 hankel-1.2.1/hankel/hankel.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8208 2022-04-29 22:23:20.000000 hankel-1.2.1/hankel/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 22:23:31.765997 hankel-1.2.1/hankel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5135 2022-04-29 22:23:31.000000 hankel-1.2.1/hankel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-04-29 22:23:31.000000 hankel-1.2.1/hankel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-29 22:23:31.000000 hankel-1.2.1/hankel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-04-29 22:23:31.000000 hankel-1.2.1/hankel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-29 22:23:31.000000 hankel-1.2.1/hankel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 22:23:31.765997 hankel-1.2.1/paper/
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-04-29 22:23:20.000000 hankel-1.2.1/paper/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    98285 2022-04-29 22:23:20.000000 hankel-1.2.1/paper/joss-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    10474 2022-04-29 22:23:20.000000 hankel-1.2.1/paper/latex.template
--rw-r--r--   0 runner    (1001) docker     (121)     4287 2022-04-29 22:23:20.000000 hankel-1.2.1/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (121)     6416 2022-04-29 22:23:20.000000 hankel-1.2.1/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-04-29 22:23:20.000000 hankel-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-04-29 22:23:31.769997 hankel-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-04-29 22:23:20.000000 hankel-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-29 22:23:31.765997 hankel-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-04-29 22:23:20.000000 hankel-1.2.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-04-29 22:23:20.000000 hankel-1.2.1/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (121)     3747 2022-04-29 22:23:20.000000 hankel-1.2.1/tests/test_get_h.py
--rw-r--r--   0 runner    (1001) docker     (121)     4134 2022-04-29 22:23:20.000000 hankel-1.2.1/tests/test_known_integrals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-04-29 22:23:20.000000 hankel-1.2.1/tests/test_round_trip.py
--rw-r--r--   0 runner    (1001) docker     (121)     4709 2022-04-29 22:23:20.000000 hankel-1.2.1/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:36:31.904252 hankel-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-27 13:36:18.000000 hankel-1.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:36:31.888252 hankel-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:36:31.888252 hankel-1.2.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-27 13:36:18.000000 hankel-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-07-27 13:36:18.000000 hankel-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-27 13:36:18.000000 hankel-1.2.2/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-27 13:36:18.000000 hankel-1.2.2/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:36:31.888252 hankel-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1835 2023-07-27 13:36:18.000000 hankel-1.2.2/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-07-27 13:36:18.000000 hankel-1.2.2/.github/workflows/test_suite.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-27 13:36:18.000000 hankel-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1521 2023-07-27 13:36:18.000000 hankel-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-07-27 13:36:18.000000 hankel-1.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-27 13:36:18.000000 hankel-1.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4799 2023-07-27 13:36:18.000000 hankel-1.2.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4368 2023-07-27 13:36:18.000000 hankel-1.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-07-27 13:36:18.000000 hankel-1.2.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-07-27 13:36:18.000000 hankel-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4864 2023-07-27 13:36:31.904252 hankel-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-07-27 13:36:18.000000 hankel-1.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-07-27 13:36:18.000000 hankel-1.2.2/codecov.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:36:31.896252 hankel-1.2.2/devel/
+-rw-r--r--   0 runner    (1001) docker     (122)  5483604 2023-07-27 13:36:18.000000 hankel-1.2.2/devel/stepsizes_for_fourier.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)  1568119 2023-07-27 13:36:18.000000 hankel-1.2.2/devel/stepsizes_for_integrals.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)   535941 2023-07-27 13:36:18.000000 hankel-1.2.2/devel/stepsizes_for_transforms.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:36:31.900252 hankel-1.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:36:31.900252 hankel-1.2.2/docs/demos/
+-rw-r--r--   0 runner    (1001) docker     (122)   131461 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/demos/choosing_resolution_parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    39996 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/demos/getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)   422322 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/demos/laplacian_hankel_vs_fft.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)   250443 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/demos/paper_plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    99368 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/demos/testing_forward_and_inverse_transforms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/example_toc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:36:31.900252 hankel-1.2.2/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-07-27 13:36:18.000000 hankel-1.2.2/docs/templates/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:36:31.900252 hankel-1.2.2/hankel/
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-07-27 13:36:18.000000 hankel-1.2.2/hankel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-27 13:36:31.000000 hankel-1.2.2/hankel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16572 2023-07-27 13:36:18.000000 hankel-1.2.2/hankel/hankel.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8208 2023-07-27 13:36:18.000000 hankel-1.2.2/hankel/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:36:31.900252 hankel-1.2.2/hankel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4864 2023-07-27 13:36:31.000000 hankel-1.2.2/hankel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-27 13:36:31.000000 hankel-1.2.2/hankel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 13:36:31.000000 hankel-1.2.2/hankel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-27 13:36:31.000000 hankel-1.2.2/hankel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-27 13:36:31.000000 hankel-1.2.2/hankel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:36:31.904252 hankel-1.2.2/paper/
+-rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-07-27 13:36:18.000000 hankel-1.2.2/paper/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)    98285 2023-07-27 13:36:18.000000 hankel-1.2.2/paper/joss-logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)    10474 2023-07-27 13:36:18.000000 hankel-1.2.2/paper/latex.template
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-07-27 13:36:18.000000 hankel-1.2.2/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (122)     6416 2023-07-27 13:36:18.000000 hankel-1.2.2/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-27 13:36:18.000000 hankel-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-07-27 13:36:31.904252 hankel-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-27 13:36:18.000000 hankel-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:36:31.904252 hankel-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-07-27 13:36:18.000000 hankel-1.2.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-07-27 13:36:18.000000 hankel-1.2.2/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-07-27 13:36:18.000000 hankel-1.2.2/tests/test_get_h.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4134 2023-07-27 13:36:18.000000 hankel-1.2.2/tests/test_known_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-07-27 13:36:18.000000 hankel-1.2.2/tests/test_round_trip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4709 2023-07-27 13:36:18.000000 hankel-1.2.2/tests/test_transforms.py
```

### Comparing `hankel-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `hankel-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/.github/workflows/deploy.yaml` & `hankel-1.2.2/.github/workflows/deploy.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -44,22 +44,22 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/download-artifact@v2
         with:
           name: artifact
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.5.0
+      - uses: pypa/gh-action-pypi-publish@v1.8.8
         name: Deploy to Test PyPi
         if: github.event_name == 'push' && github.ref == 'refs/heads/main'
         with:
           user: __token__
           password: ${{ secrets.test_pypi_password }}
           repository_url: https://test.pypi.org/legacy/
           skip_existing: true
 
-      - uses: pypa/gh-action-pypi-publish@v1.5.0
+      - uses: pypa/gh-action-pypi-publish@v1.8.8
         name: Deploy To PyPI
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/v')
         with:
           user: __token__
           password: ${{ secrets.pypi_password }}
```

### Comparing `hankel-1.2.1/.github/workflows/test_suite.yaml` & `hankel-1.2.2/.github/workflows/test_suite.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       OS: ${{ matrix.os }}
     name: Testing
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [3.6, 3.7, 3.8, 3.9, '3.10']
+        python-version: [3.7, 3.8, 3.9, '3.10', '3.11']
     steps:
       - uses: actions/checkout@main
         with:
           fetch-depth: 1
 
       - uses: actions/setup-python@v2
         with:
```

### Comparing `hankel-1.2.1/.pre-commit-config.yaml` & `hankel-1.2.2/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 exclude: '(^docs/conf.py)'
 
 repos:
     - repo: https://github.com/pre-commit/pre-commit-hooks
-      rev: v4.2.0
+      rev: v4.4.0
       hooks:
           - id: trailing-whitespace
           - id: check-added-large-files
           - id: check-ast
           - id: check-json
           - id: check-merge-conflict
           - id: check-xml
@@ -14,45 +14,45 @@
           - id: debug-statements
           - id: end-of-file-fixer
           - id: requirements-txt-fixer
           - id: mixed-line-ending
             args: ['--fix=no']
 
     - repo: https://github.com/PyCQA/flake8
-      rev: 4.0.1
+      rev: 6.0.0
       hooks:
         - id: flake8
           additional_dependencies:
-            - flake8-comprehensions
+            # - flake8-comprehensions  # flake8<6 only
             - flake8-builtins
-            - flake8-eradicate
+            # - flake8-eradicate       flake8 <6 only
             - pep8-naming
             - flake8-rst-docstrings
-            - flake8-copyright
+            # - flake8-copyright      # flake8<6 only
             - flake8-docstrings
 
     - repo: https://github.com/psf/black
-      rev: 22.3.0
+      rev: 23.7.0
       hooks:
           - id: black
 
     - repo: https://github.com/PyCQA/isort
-      rev: 5.10.1
+      rev: 5.12.0
       hooks:
       - id: isort
 
     - repo: https://github.com/pre-commit/pygrep-hooks
-      rev: v1.9.0
+      rev: v1.10.0
       hooks:
         - id: rst-backticks
 
     - repo: https://github.com/asottile/pyupgrade
-      rev: v2.32.0
+      rev: v3.9.0
       hooks:
       - id: pyupgrade
-        args: [--py36-plus]
+        args: [--py37-plus]
 
     - repo: https://github.com/asottile/setup-cfg-fmt
-      rev: v1.20.1
+      rev: v2.4.0
       hooks:
       - id: setup-cfg-fmt
         args: ['--min-py3-version=3.6']
```

### Comparing `hankel-1.2.1/CHANGELOG.rst` & `hankel-1.2.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/CONTRIBUTING.rst` & `hankel-1.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/LICENSE.rst` & `hankel-1.2.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/PKG-INFO` & `hankel-1.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 Metadata-Version: 2.1
 Name: hankel
-Version: 1.2.1
+Version: 1.2.2
 Summary: Hankel Transformations using method of Ogata 2005
 Home-page: https://github.com/steven-murray/hankel
 Author: Steven Murray
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Project-URL: Documentation, https://hankel.readthedocs.io
 Project-URL: Source, https://github.com/steven-murray/hankel
 Project-URL: Tracker, https://github.com/steven-murray/hankel/issues
 Project-URL: Changelog, https://github.com/steven-murray/hankel/blob/master/CHANGELOG.rst
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/hankel
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
@@ -128,9 +122,7 @@
 
 Also draws inspiration from
 
     Fast Edge-corrected Measurement of the Two-Point Correlation
     Function and the Power Spectrum Szapudi, Istvan; Pan, Jun; Prunet,
     Simon; Budavari, Tamas (2005) The Astrophysical Journal vol. 631 (1)
     DOI: 10.1086/496971
-
-
```

### Comparing `hankel-1.2.1/README.rst` & `hankel-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/devel/stepsizes_for_fourier.ipynb` & `hankel-1.2.2/devel/stepsizes_for_fourier.ipynb`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/devel/stepsizes_for_integrals.ipynb` & `hankel-1.2.2/devel/stepsizes_for_integrals.ipynb`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/devel/stepsizes_for_transforms.ipynb` & `hankel-1.2.2/devel/stepsizes_for_transforms.ipynb`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/docs/Makefile` & `hankel-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/docs/conf.py` & `hankel-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/docs/demos/choosing_resolution_parameters.ipynb` & `hankel-1.2.2/docs/demos/choosing_resolution_parameters.ipynb`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/docs/demos/getting_started.ipynb` & `hankel-1.2.2/docs/demos/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/docs/demos/laplacian_hankel_vs_fft.ipynb` & `hankel-1.2.2/docs/demos/laplacian_hankel_vs_fft.ipynb`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/docs/demos/paper_plots.ipynb` & `hankel-1.2.2/docs/demos/paper_plots.ipynb`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/docs/demos/testing_forward_and_inverse_transforms.ipynb` & `hankel-1.2.2/docs/demos/testing_forward_and_inverse_transforms.ipynb`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/docs/make.bat` & `hankel-1.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/docs/templates/class.rst` & `hankel-1.2.2/docs/templates/class.rst`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/docs/templates/modules.rst` & `hankel-1.2.2/docs/templates/modules.rst`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/hankel/__init__.py` & `hankel-1.2.2/hankel/__init__.py`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/hankel/hankel.py` & `hankel-1.2.2/hankel/hankel.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         The step-size of the integration.
     alt : bool, optional
         Whether to use the alternative definition of the hankel transform.
         should be used
     """
 
     def __init__(self, nu=0, N=None, h=0.05, alt=False):
-
         N = int(np.pi / h) if N is None else N
         if not np.isscalar(N):
             raise ValueError("N must be a scalar")
         if not np.isscalar(h):
             raise ValueError("h must be a scalar")
         if not np.isscalar(nu):
             raise ValueError("nu must be a scalar")
@@ -413,15 +412,14 @@
     .. math:: f(r) = \sqrt{\frac{|b|}{(2\pi)^{1+a}}}^n
               \frac{(2\pi)^{n/2}}{(br)^{n/2-1}}
               \int_0^\infty k^{n/2-1} f(k) J_{n/2-1}(bkr) k dk.
 
     """
 
     def __init__(self, ndim=2, a=1, b=1, N=None, h=0.05, alt=True):
-
         super().__init__(nu=dim_to_nu(ndim), N=N, h=h, alt=alt)
 
         self.ndim = ndim
         self.fourier_norm_a = a
         self.fourier_norm_b = b
         self._r_power = (ndim - 1) / 2.0 if alt else ndim / 2.0
         self._k_power = (ndim - 1) / 2.0 if alt else ndim / 2.0 - 1
```

### Comparing `hankel-1.2.1/hankel/tools.py` & `hankel-1.2.2/hankel/tools.py`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/hankel.egg-info/PKG-INFO` & `hankel-1.2.2/hankel.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 Metadata-Version: 2.1
 Name: hankel
-Version: 1.2.1
+Version: 1.2.2
 Summary: Hankel Transformations using method of Ogata 2005
 Home-page: https://github.com/steven-murray/hankel
 Author: Steven Murray
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Project-URL: Documentation, https://hankel.readthedocs.io
 Project-URL: Source, https://github.com/steven-murray/hankel
 Project-URL: Tracker, https://github.com/steven-murray/hankel/issues
 Project-URL: Changelog, https://github.com/steven-murray/hankel/blob/master/CHANGELOG.rst
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/hankel
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
@@ -128,9 +122,7 @@
 
 Also draws inspiration from
 
     Fast Edge-corrected Measurement of the Two-Point Correlation
     Function and the Power Spectrum Szapudi, Istvan; Pan, Jun; Prunet,
     Simon; Budavari, Tamas (2005) The Astrophysical Journal vol. 631 (1)
     DOI: 10.1086/496971
-
-
```

### Comparing `hankel-1.2.1/hankel.egg-info/SOURCES.txt` & `hankel-1.2.2/hankel.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
+codecov.yaml
 pyproject.toml
 setup.cfg
 setup.py
 .github/dependabot.yaml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/question.md
```

### Comparing `hankel-1.2.1/paper/Makefile` & `hankel-1.2.2/paper/Makefile`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/paper/joss-logo.png` & `hankel-1.2.2/paper/joss-logo.png`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/paper/latex.template` & `hankel-1.2.2/paper/latex.template`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/paper/paper.bib` & `hankel-1.2.2/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/paper/paper.md` & `hankel-1.2.2/paper/paper.md`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/pyproject.toml` & `hankel-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/tests/test_api.py` & `hankel-1.2.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/tests/test_fourier.py` & `hankel-1.2.2/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/tests/test_get_h.py` & `hankel-1.2.2/tests/test_get_h.py`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/tests/test_known_integrals.py` & `hankel-1.2.2/tests/test_known_integrals.py`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/tests/test_round_trip.py` & `hankel-1.2.2/tests/test_round_trip.py`

 * *Files identical despite different names*

### Comparing `hankel-1.2.1/tests/test_transforms.py` & `hankel-1.2.2/tests/test_transforms.py`

 * *Files identical despite different names*

