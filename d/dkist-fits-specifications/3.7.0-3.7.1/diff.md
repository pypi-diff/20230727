# Comparing `tmp/dkist_fits_specifications-3.7.0.tar.gz` & `tmp/dkist_fits_specifications-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_fits_specifications-3.7.0.tar", last modified: Wed Jul 26 20:08:05 2023, max compression
+gzip compressed data, was "dkist_fits_specifications-3.7.1.tar", last modified: Wed Jul 26 23:11:05 2023, max compression
```

## Comparing `dkist_fits_specifications-3.7.0.tar` & `dkist_fits_specifications-3.7.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     3334 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     4882 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     6507 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6089 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2285 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.541564 dkist_fits_specifications-3.7.0/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.541564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/py.typed
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.541564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/
--rw-rw-rw-   0 root         (0) root         (0)     3584 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.545564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/ao.yml
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/camera.yml
--rw-rw-rw-   0 root         (0) root         (0)      515 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/compression.yml
--rw-rw-rw-   0 root         (0) root         (0)    10244 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/cryonirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/dkist-id.yml
--rw-rw-rw-   0 root         (0) root         (0)     4395 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/dlnirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/fits.yml
--rw-rw-rw-   0 root         (0) root         (0)     1934 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/pac.yml
--rw-rw-rw-   0 root         (0) root         (0)     2653 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/telescope.yml
--rw-rw-rw-   0 root         (0) root         (0)      930 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/vbi.yml
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/visp.yml
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/vtf.yml
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/wfc.yml
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/ws.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.545564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/
--rw-rw-rw-   0 root         (0) root         (0)    11880 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3117 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/level0.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.545564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/ao.yml
--rw-rw-rw-   0 root         (0) root         (0)     5886 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/camera.yml
--rw-rw-rw-   0 root         (0) root         (0)     6506 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/compression.yml
--rw-rw-rw-   0 root         (0) root         (0)    13479 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/cryonirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/datacenter.yml
--rw-rw-rw-   0 root         (0) root         (0)     4144 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dataset.yml
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dkist-id.yml
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dkist-op.yml
--rw-rw-rw-   0 root         (0) root         (0)     8355 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dlnirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/fits.yml
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/pac.yml
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/stats.yml
--rw-rw-rw-   0 root         (0) root         (0)     7410 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/telescope.yml
--rw-rw-rw-   0 root         (0) root         (0)     2085 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/vbi.yml
--rw-rw-rw-   0 root         (0) root         (0)     2939 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/visp.yml
--rw-rw-rw-   0 root         (0) root         (0)     3660 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/vtf.yml
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/wfc.yml
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/ws.yml
--rw-rw-rw-   0 root         (0) root         (0)     1001 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/spec214_full_schema.yml
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec_validation_schema.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_122.py
--rw-rw-rw-   0 root         (0) root         (0)     2687 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_214.py
--rw-rw-rw-   0 root         (0) root         (0)     2808 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_expansions.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_level0_214.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3374 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     1222 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/frozendict.py
--rw-rw-rw-   0 root         (0) root         (0)     4799 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/spec.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/sphinx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/sphinx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8553 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/sphinx/spec_table.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.541564 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6507 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3341 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3424 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/level_one.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/reference.rst
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/release_history.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/docs/specs/
--rw-rw-rw-   0 root         (0) root         (0)     1463 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/specs/spec-122.rst
--rw-rw-rw-   0 root         (0) root         (0)     2668 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/specs/spec-214.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2031 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      612 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.076486 dkist_fits_specifications-3.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5052 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     6507 2023-07-26 23:11:05.076486 dkist_fits_specifications-3.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.068487 dkist_fits_specifications-3.7.1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.068487 dkist_fits_specifications-3.7.1/dkist_fits_specifications/
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/py.typed
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.068487 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.072486 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/ao.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/camera.yml
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/compression.yml
+-rw-rw-rw-   0 root         (0) root         (0)    10244 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/cryonirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/dkist-id.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4395 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/dlnirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/fits.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/pac.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2653 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/telescope.yml
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/vbi.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/visp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/vtf.yml
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/wfc.yml
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/ws.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.072486 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/
+-rw-rw-rw-   0 root         (0) root         (0)    11880 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/level0.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.072486 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/ao.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5886 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/camera.yml
+-rw-rw-rw-   0 root         (0) root         (0)     6506 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/compression.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13479 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/cryonirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/datacenter.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4144 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/dataset.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/dkist-id.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/dkist-op.yml
+-rw-rw-rw-   0 root         (0) root         (0)     8355 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/dlnirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/fits.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/pac.yml
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/stats.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/telescope.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/vbi.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/visp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3660 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/vtf.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/wfc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/ws.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/spec214_full_schema.yml
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec_validation_schema.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.072486 dkist_fits_specifications-3.7.1/dkist_fits_specifications/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/tests/test_122.py
+-rw-rw-rw-   0 root         (0) root         (0)     2687 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/tests/test_214.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/tests/test_expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/tests/test_level0_214.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.076486 dkist_fits_specifications-3.7.1/dkist_fits_specifications/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3374 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/utils/formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/utils/frozendict.py
+-rw-rw-rw-   0 root         (0) root         (0)     4799 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/utils/spec.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.076486 dkist_fits_specifications-3.7.1/dkist_fits_specifications/utils/sphinx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/utils/sphinx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8553 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/utils/sphinx/spec_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-07-26 23:11:05.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.068487 dkist_fits_specifications-3.7.1/dkist_fits_specifications.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6507 2023-07-26 23:11:05.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2023-07-26 23:11:05.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 23:11:05.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 23:11:05.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-26 23:11:05.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-26 23:11:05.000000 dkist_fits_specifications-3.7.1/dkist_fits_specifications.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.076486 dkist_fits_specifications-3.7.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/docs/level_one.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/docs/reference.rst
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/docs/release_history.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.076486 dkist_fits_specifications-3.7.1/docs/specs/
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/docs/specs/spec-122.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/docs/specs/spec-214.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 23:11:05.076486 dkist_fits_specifications-3.7.1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-07-26 23:11:05.076486 dkist_fits_specifications-3.7.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      612 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2023-07-26 23:10:48.000000 dkist_fits_specifications-3.7.1/tox.ini
```

### Comparing `dkist_fits_specifications-3.7.0/.gitignore` & `dkist_fits_specifications-3.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/.pre-commit-config.yaml` & `dkist_fits_specifications-3.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/CHANGELOG.rst` & `dkist_fits_specifications-3.7.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+v3.7.1 (2023-07-26)
+===================
+
+Bug Fixes to the Python API
+---------------------------
+
+- Update the python version used in the Read The Docs build process.
+
+
+
 v3.7.0 (2023-07-26)
 ===================
 
 Backwards Compatible Changes to the Specification
 -------------------------------------------------
 
 - Adding the FITS standard key `ZBLANK` (`#36 <https://bitbucket.org/dkistdc/dkist-fits-specifications/pull-requests/36>`__)
```

### Comparing `dkist_fits_specifications-3.7.0/PKG-INFO` & `dkist_fits_specifications-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_fits_specifications
-Version: 3.7.0
+Version: 3.7.1
 Summary: Machine readable FITS specifications for DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-fits-specifications/src/main/
 Author: AURA/NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
```

### Comparing `dkist_fits_specifications-3.7.0/README.rst` & `dkist_fits_specifications-3.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/bitbucket-pipelines.yml` & `dkist_fits_specifications-3.7.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/check_changelog_updated.sh` & `dkist_fits_specifications-3.7.1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/__init__.py` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/__init__.py` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/ao.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/ao.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/camera.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/camera.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/compression.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/compression.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/cryonirsp.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/cryonirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/dkist-id.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/dkist-id.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/dlnirsp.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/dlnirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/fits.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/fits.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/pac.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/pac.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/telescope.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/telescope.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/vbi.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/vbi.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/visp.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/visp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/vtf.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/vtf.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/wfc.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/wfc.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/ws.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec122/schemas/ws.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/__init__.py` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/level0.py` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/level0.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/ao.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/ao.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/camera.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/camera.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/compression.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/compression.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/cryonirsp.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/cryonirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/datacenter.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/datacenter.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dataset.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/dataset.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dkist-id.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/dkist-id.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dkist-op.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/dkist-op.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dlnirsp.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/dlnirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/fits.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/fits.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/pac.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/pac.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/stats.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/stats.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/telescope.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/telescope.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/vbi.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/vbi.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/visp.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/visp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/vtf.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/vtf.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/wfc.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/wfc.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/ws.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/schemas/ws.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/spec214_full_schema.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec214/spec214_full_schema.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec_validation_schema.yml` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/spec_validation_schema.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_122.py` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/tests/test_122.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_214.py` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/tests/test_214.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_expansions.py` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/tests/test_expansions.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/formatter.py` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/frozendict.py` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/utils/frozendict.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/spec.py` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/utils/spec.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/sphinx/spec_table.py` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications/utils/sphinx/spec_table.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/PKG-INFO` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-fits-specifications
-Version: 3.7.0
+Version: 3.7.1
 Summary: Machine readable FITS specifications for DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-fits-specifications/src/main/
 Author: AURA/NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
```

### Comparing `dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/SOURCES.txt` & `dkist_fits_specifications-3.7.1/dkist_fits_specifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/docs/Makefile` & `dkist_fits_specifications-3.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/docs/conf.py` & `dkist_fits_specifications-3.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/docs/index.rst` & `dkist_fits_specifications-3.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/docs/level_one.rst` & `dkist_fits_specifications-3.7.1/docs/level_one.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/docs/make.bat` & `dkist_fits_specifications-3.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/docs/specs/spec-122.rst` & `dkist_fits_specifications-3.7.1/docs/specs/spec-122.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/docs/specs/spec-214.rst` & `dkist_fits_specifications-3.7.1/docs/specs/spec-214.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/licenses/LICENSE.rst` & `dkist_fits_specifications-3.7.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/licenses/TEMPLATE_LICENSE.rst` & `dkist_fits_specifications-3.7.1/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/pyproject.toml` & `dkist_fits_specifications-3.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/setup.cfg` & `dkist_fits_specifications-3.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/setup.py` & `dkist_fits_specifications-3.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.7.0/tox.ini` & `dkist_fits_specifications-3.7.1/tox.ini`

 * *Files identical despite different names*

