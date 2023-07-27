# Comparing `tmp/astroplan-0.8.tar.gz` & `tmp/astroplan-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/folders/b3/hq8c10h90xdc3mxwlk53tvzm0000gn/T/tmpl33fgora/tmp16xithi7/astroplan-0.8.tar", last modified: Tue Jan 26 07:57:37 2021, max compression
+gzip compressed data, was "astroplan-0.9.tar", last modified: Thu Jul 27 17:53:53 2023, max compression
```

## Comparing `astroplan-0.8.tar` & `astroplan-0.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/.github/
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/.github/workflows/
--rw-r--r--   0 bmmorris   (501) staff       (20)     2932 2021-01-25 15:09:23.000000 astroplan-0.8/.github/workflows/ci_tests.yml
--rw-r--r--   0 bmmorris   (501) staff       (20)      622 2017-10-20 15:41:05.000000 astroplan-0.8/.gitignore
--rw-r--r--   0 bmmorris   (501) staff       (20)        0 2021-01-25 15:09:23.000000 astroplan-0.8/.gitmodules
--rw-r--r--   0 bmmorris   (501) staff       (20)      570 2021-01-26 07:51:48.000000 astroplan-0.8/.readthedocs.yml
--rw-r--r--   0 bmmorris   (501) staff       (20)     2992 2021-01-26 07:56:11.000000 astroplan-0.8/CHANGES.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      964 2018-05-03 13:53:28.000000 astroplan-0.8/CITATION
--rw-r--r--   0 bmmorris   (501) staff       (20)     1497 2017-10-20 15:41:05.000000 astroplan-0.8/LICENSE.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      477 2017-10-20 15:40:57.000000 astroplan-0.8/LONG_DESCRIPTION.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1090 2017-10-24 00:57:25.000000 astroplan-0.8/MANIFEST.in
--rw-r--r--   0 bmmorris   (501) staff       (20)     2584 2021-01-26 07:57:37.000000 astroplan-0.8/PKG-INFO
--rw-r--r--   0 bmmorris   (501) staff       (20)     1783 2021-01-26 07:51:48.000000 astroplan-0.8/README.rst
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan/
--rw-r--r--   0 bmmorris   (501) staff       (20)     1147 2020-10-27 08:19:06.000000 astroplan-0.8/astroplan/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     1799 2021-01-25 15:09:23.000000 astroplan-0.8/astroplan/_astropy_init.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     1817 2021-01-25 15:09:23.000000 astroplan-0.8/astroplan/conftest.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    49300 2019-08-14 06:54:46.000000 astroplan-0.8/astroplan/constraints.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     1063 2017-09-15 08:45:47.000000 astroplan-0.8/astroplan/exceptions.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     1732 2017-10-20 15:41:05.000000 astroplan-0.8/astroplan/moon.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    79134 2020-08-10 07:50:19.000000 astroplan-0.8/astroplan/observer.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    10665 2018-12-28 03:43:22.000000 astroplan-0.8/astroplan/periodic.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan/plots/
--rw-r--r--   0 bmmorris   (501) staff       (20)      317 2019-11-19 19:05:33.000000 astroplan-0.8/astroplan/plots/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     4429 2019-11-17 10:00:02.000000 astroplan-0.8/astroplan/plots/finder.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     2728 2017-10-20 15:41:05.000000 astroplan-0.8/astroplan/plots/mplstyles.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    11731 2021-01-25 15:09:23.000000 astroplan-0.8/astroplan/plots/sky.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan/plots/tests/
--rw-r--r--   0 bmmorris   (501) staff       (20)        0 2016-04-07 17:58:38.000000 astroplan-0.8/astroplan/plots/tests/__init__.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan/plots/tests/baseline_images/
--rw-r--r--   0 bmmorris   (501) staff       (20)    17609 2016-04-07 17:58:38.000000 astroplan-0.8/astroplan/plots/tests/baseline_images/test_image_example.png
--rw-r--r--   0 bmmorris   (501) staff       (20)     1357 2020-08-10 07:50:19.000000 astroplan-0.8/astroplan/plots/tests/test_sky.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    23689 2021-01-25 15:09:23.000000 astroplan-0.8/astroplan/plots/time_dependent.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    42861 2019-11-06 08:12:49.000000 astroplan-0.8/astroplan/scheduling.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      273 2016-04-07 17:58:38.000000 astroplan-0.8/astroplan/setup_package.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    10255 2019-11-06 08:12:49.000000 astroplan-0.8/astroplan/target.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan/tests/
--rw-r--r--   0 bmmorris   (501) staff       (20)        0 2016-01-08 00:37:04.000000 astroplan-0.8/astroplan/tests/__init__.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      768 2016-01-08 00:37:04.000000 astroplan-0.8/astroplan/tests/coveragerc
--rw-r--r--   0 bmmorris   (501) staff       (20)    22312 2020-10-27 08:19:06.000000 astroplan-0.8/astroplan/tests/test_constraints.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     1726 2017-10-24 01:42:38.000000 astroplan-0.8/astroplan/tests/test_moon.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    52460 2020-10-27 08:19:06.000000 astroplan-0.8/astroplan/tests/test_observer.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     3438 2017-10-24 00:57:25.000000 astroplan-0.8/astroplan/tests/test_periodic.py
--rw-r--r--   0 bmmorris   (501) staff       (20)    14635 2021-01-25 15:09:23.000000 astroplan-0.8/astroplan/tests/test_scheduling.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     2982 2019-11-06 08:12:49.000000 astroplan-0.8/astroplan/tests/test_target.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     1066 2019-11-19 19:05:53.000000 astroplan-0.8/astroplan/tests/test_utils.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     8539 2020-10-27 08:19:06.000000 astroplan-0.8/astroplan/utils.py
--rw-r--r--   0 bmmorris   (501) staff       (20)      335 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan/version.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan.egg-info/
--rw-r--r--   0 bmmorris   (501) staff       (20)     2584 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan.egg-info/PKG-INFO
--rw-r--r--   0 bmmorris   (501) staff       (20)     1852 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan.egg-info/SOURCES.txt
--rw-r--r--   0 bmmorris   (501) staff       (20)        1 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan.egg-info/dependency_links.txt
--rw-r--r--   0 bmmorris   (501) staff       (20)        1 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan.egg-info/not-zip-safe
--rw-r--r--   0 bmmorris   (501) staff       (20)      210 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan.egg-info/requires.txt
--rw-r--r--   0 bmmorris   (501) staff       (20)       10 2021-01-26 07:57:37.000000 astroplan-0.8/astroplan.egg-info/top_level.txt
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/docs/
--rw-r--r--   0 bmmorris   (501) staff       (20)     4581 2017-10-20 15:41:05.000000 astroplan-0.8/docs/Makefile
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/docs/_templates/
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/docs/_templates/autosummary/
--rw-r--r--   0 bmmorris   (501) staff       (20)      250 2016-01-08 00:37:18.000000 astroplan-0.8/docs/_templates/autosummary/base.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      251 2016-01-08 00:37:18.000000 astroplan-0.8/docs/_templates/autosummary/class.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      252 2016-01-08 00:37:18.000000 astroplan-0.8/docs/_templates/autosummary/module.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      112 2016-04-07 17:58:38.000000 astroplan-0.8/docs/api.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)       75 2017-10-20 15:41:05.000000 astroplan-0.8/docs/changelog.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     7081 2021-01-26 07:51:48.000000 astroplan-0.8/docs/conf.py
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/docs/faq/
--rw-r--r--   0 bmmorris   (501) staff       (20)     1268 2021-01-25 15:09:23.000000 astroplan-0.8/docs/faq/contribute.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     5860 2021-01-25 15:09:23.000000 astroplan-0.8/docs/faq/iers.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      328 2017-10-20 15:41:05.000000 astroplan-0.8/docs/faq/index.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     3313 2019-12-08 11:15:20.000000 astroplan-0.8/docs/faq/precision.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     2658 2017-10-20 15:41:05.000000 astroplan-0.8/docs/faq/terminology.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     3133 2021-01-25 15:09:23.000000 astroplan-0.8/docs/getting_started.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1933 2021-01-25 15:09:23.000000 astroplan-0.8/docs/index.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     1921 2021-01-26 07:51:48.000000 astroplan-0.8/docs/installation.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     4513 2016-01-08 00:37:19.000000 astroplan-0.8/docs/make.bat
--rw-r--r--   0 bmmorris   (501) staff       (20)      377 2021-01-25 15:09:23.000000 astroplan-0.8/docs/references.txt
--rw-r--r--   0 bmmorris   (501) staff       (20)       77 2021-01-26 07:51:48.000000 astroplan-0.8/docs/rtd-pip-requirements
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/docs/tutorials/
--rw-r--r--   0 bmmorris   (501) staff       (20)    20165 2017-10-24 01:43:13.000000 astroplan-0.8/docs/tutorials/constraints.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      620 2019-12-08 11:45:50.000000 astroplan-0.8/docs/tutorials/index.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)    10917 2019-12-08 11:15:20.000000 astroplan-0.8/docs/tutorials/periodic.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)    40900 2021-01-25 15:09:23.000000 astroplan-0.8/docs/tutorials/plots.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)    35038 2017-10-20 15:41:05.000000 astroplan-0.8/docs/tutorials/scheduling.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)     3402 2021-01-26 07:51:48.000000 astroplan-0.8/docs/tutorials/speed.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)    19085 2021-01-25 15:09:23.000000 astroplan-0.8/docs/tutorials/summer_triangle.rst
-drwxr-xr-x   0 bmmorris   (501) staff       (20)        0 2021-01-26 07:57:37.000000 astroplan-0.8/licenses/
--rw-r--r--   0 bmmorris   (501) staff       (20)      251 2017-10-20 15:41:05.000000 astroplan-0.8/licenses/README.rst
--rw-r--r--   0 bmmorris   (501) staff       (20)      132 2021-01-25 15:09:23.000000 astroplan-0.8/pyproject.toml
--rw-r--r--   0 bmmorris   (501) staff       (20)     1754 2021-01-26 07:57:37.000000 astroplan-0.8/setup.cfg
--rwxr-xr-x   0 bmmorris   (501) staff       (20)     1943 2021-01-25 15:09:23.000000 astroplan-0.8/setup.py
--rw-r--r--   0 bmmorris   (501) staff       (20)     2922 2021-01-25 15:09:23.000000 astroplan-0.8/tox.ini
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.866352 astroplan-0.9/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.851363 astroplan-0.9/.github/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.854565 astroplan-0.9/.github/workflows/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2438 2023-06-05 01:40:13.000000 astroplan-0.9/.github/workflows/ci_tests.yml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      622 2022-10-11 18:10:24.000000 astroplan-0.9/.gitignore
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        0 2022-10-11 18:11:36.000000 astroplan-0.9/.gitmodules
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      641 2023-03-17 00:33:25.000000 astroplan-0.9/.readthedocs.yml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3392 2023-07-27 17:29:43.000000 astroplan-0.9/CHANGES.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      795 2023-01-10 18:38:43.000000 astroplan-0.9/CITATION.bib
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1497 2022-10-11 18:10:24.000000 astroplan-0.9/LICENSE.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      477 2022-10-11 18:10:24.000000 astroplan-0.9/LONG_DESCRIPTION.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      339 2023-01-10 18:38:43.000000 astroplan-0.9/MANIFEST.in
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2507 2023-07-27 17:53:53.866453 astroplan-0.9/PKG-INFO
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2095 2023-07-27 17:52:32.000000 astroplan-0.9/README.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.856802 astroplan-0.9/astroplan/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1147 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      613 2022-10-11 18:11:36.000000 astroplan-0.9/astroplan/_astropy_init.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1629 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/conftest.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    50032 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/constraints.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1230 2023-01-10 18:38:43.000000 astroplan-0.9/astroplan/exceptions.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1760 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/moon.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    81969 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/observer.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    10665 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/periodic.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.859337 astroplan-0.9/astroplan/plots/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      317 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/plots/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4443 2022-10-11 19:38:39.000000 astroplan-0.9/astroplan/plots/finder.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2728 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/plots/mplstyles.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    11776 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/plots/sky.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.859617 astroplan-0.9/astroplan/plots/tests/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        0 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/plots/tests/__init__.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.859770 astroplan-0.9/astroplan/plots/tests/baseline_images/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    17609 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/plots/tests/baseline_images/test_image_example.png
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1357 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/plots/tests/test_sky.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    23885 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/plots/time_dependent.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    42960 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/scheduling.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      273 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/setup_package.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    10255 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/target.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.861543 astroplan-0.9/astroplan/tests/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        0 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/tests/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      768 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/tests/coveragerc
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    23079 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/tests/test_constraints.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1726 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/tests/test_moon.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    53640 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/tests/test_observer.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3438 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/tests/test_periodic.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    15796 2023-07-27 17:29:43.000000 astroplan-0.9/astroplan/tests/test_scheduling.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2982 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/tests/test_target.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1066 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/tests/test_utils.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     8539 2022-10-11 18:10:24.000000 astroplan-0.9/astroplan/utils.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      335 2023-07-27 17:53:53.000000 astroplan-0.9/astroplan/version.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.858574 astroplan-0.9/astroplan.egg-info/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2507 2023-07-27 17:53:53.000000 astroplan-0.9/astroplan.egg-info/PKG-INFO
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1856 2023-07-27 17:53:53.000000 astroplan-0.9/astroplan.egg-info/SOURCES.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-07-27 17:53:53.000000 astroplan-0.9/astroplan.egg-info/dependency_links.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2022-10-11 18:22:53.000000 astroplan-0.9/astroplan.egg-info/not-zip-safe
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      214 2023-07-27 17:53:53.000000 astroplan-0.9/astroplan.egg-info/requires.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       10 2023-07-27 17:53:53.000000 astroplan-0.9/astroplan.egg-info/top_level.txt
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.863224 astroplan-0.9/docs/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4581 2022-10-11 18:10:24.000000 astroplan-0.9/docs/Makefile
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.852090 astroplan-0.9/docs/_templates/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.863707 astroplan-0.9/docs/_templates/autosummary/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      250 2022-10-11 18:10:24.000000 astroplan-0.9/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      251 2022-10-11 18:10:24.000000 astroplan-0.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      252 2022-10-11 18:10:24.000000 astroplan-0.9/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      112 2022-10-11 18:10:24.000000 astroplan-0.9/docs/api.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       75 2022-10-11 18:10:24.000000 astroplan-0.9/docs/changelog.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     7564 2023-07-27 17:29:43.000000 astroplan-0.9/docs/conf.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.864540 astroplan-0.9/docs/faq/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1268 2022-10-11 18:11:36.000000 astroplan-0.9/docs/faq/contribute.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     5833 2022-10-11 19:38:39.000000 astroplan-0.9/docs/faq/iers.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      328 2022-10-11 18:10:24.000000 astroplan-0.9/docs/faq/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3313 2022-10-11 18:10:24.000000 astroplan-0.9/docs/faq/precision.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2658 2022-10-11 18:10:24.000000 astroplan-0.9/docs/faq/terminology.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2877 2023-07-27 17:29:43.000000 astroplan-0.9/docs/getting_started.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2645 2023-07-27 17:52:32.000000 astroplan-0.9/docs/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1736 2023-07-27 17:29:43.000000 astroplan-0.9/docs/installation.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4513 2022-10-11 18:10:24.000000 astroplan-0.9/docs/make.bat
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      377 2022-10-11 18:11:36.000000 astroplan-0.9/docs/references.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       75 2023-03-17 00:33:25.000000 astroplan-0.9/docs/rtd-pip-requirements
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.866046 astroplan-0.9/docs/tutorials/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    20189 2023-03-17 00:33:25.000000 astroplan-0.9/docs/tutorials/constraints.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      620 2022-10-11 18:10:24.000000 astroplan-0.9/docs/tutorials/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    10948 2022-10-11 19:38:39.000000 astroplan-0.9/docs/tutorials/periodic.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    40914 2023-07-27 17:05:05.000000 astroplan-0.9/docs/tutorials/plots.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    35038 2022-10-11 18:10:24.000000 astroplan-0.9/docs/tutorials/scheduling.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3402 2022-10-11 18:11:36.000000 astroplan-0.9/docs/tutorials/speed.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    19085 2023-07-27 17:12:03.000000 astroplan-0.9/docs/tutorials/summer_triangle.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-27 17:53:53.866220 astroplan-0.9/licenses/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      251 2022-10-11 18:10:24.000000 astroplan-0.9/licenses/README.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      132 2022-10-11 18:11:36.000000 astroplan-0.9/pyproject.toml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1759 2023-07-27 17:53:53.866874 astroplan-0.9/setup.cfg
+-rwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)     1943 2022-10-11 18:11:36.000000 astroplan-0.9/setup.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2929 2023-01-10 19:27:48.000000 astroplan-0.9/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `astroplan-0.8/.github/workflows/ci_tests.yml` & `astroplan-0.9/.github/workflows/ci_tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 # This file performs testing using tox and tox.ini to define and configure the test environments.
 
 name: CI Tests
 
 on:
   push:
     branches:
-      - master  # GitHub now defaults to 'main' as the name of the primary branch. Change this as needed.
-  #  tags: # run CI if specific tags are pushed
+      - main
   pull_request:
-    # branches: # only build on PRs against 'main' if you need to further limit when CI is run.
-    #    - main
+     branches: # only build on PRs against 'main' if you need to further limit when CI is run.
+      - main
+
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
 
 jobs:
   # Github Actions supports ubuntu, windows, and macos virtual environments:
   # https://help.github.com/en/actions/reference/virtual-environments-for-github-hosted-runners
   ci_tests:
     name: ${{ matrix.name }}
     runs-on: ${{ matrix.os }}
@@ -28,63 +31,52 @@
             toxenv: codestyle
 
           - name: Python 3.7 with minimal dependencies
             os: ubuntu-latest
             python: 3.7
             toxenv: py37-test
 
-          - name: Python 3.8 with all optional dependencies, coverage checking and remote data
-            os: ubuntu-latest
-            python: 3.8
-            toxenv: py38-test-alldeps-cov
-            toxposargs: --remote-data
-
-          - name: OS X - Python 3.8 with all optional dependencies
+          - name: OS X - Python 3.9 with minimal dependencies
             os: macos-latest
-            python: 3.8
-            toxenv: py38-test-alldeps
+            python: 3.9
+            toxenv: py39-test
 
-          - name: Windows - Python 3.8 with all optional dependencies
+          - name: Windows - Python 3.11 with all optional dependencies
             os: windows-latest
-            python: 3.8
-            toxenv: py38-test-alldeps
+            python: 3.11
+            toxenv: py11-test-alldeps
 
-          # - name: Python 3.7 with oldest supported version of all dependencies
-          #   os: ubuntu-16.04
-          #   python: 3.7
-          #   toxenv: py37-test-oldestdeps
+          - name: Python 3.11 with remote data, all dependencies, and coverage
+            os: ubuntu-latest
+            python: 3.11
+            toxenv: py11-test-alldeps-cov
+            toxposargs: --remote-data
 
-          - name: Python 3.9 with latest dev versions of key dependencies
+          - name: Python 3.11 with latest dev versions of key dependencies
             os: ubuntu-latest
-            python: 3.9
-            toxenv: py39-test-devdeps
+            python: 3.11
+            toxenv: py11-test-devdeps
 
           - name: Test building of Sphinx docs
             os: ubuntu-latest
             python: 3.x
             toxenv: build_docs
 
     steps:
     - name: Checkout code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v1
       with:
         fetch-depth: 0
     - name: Set up python ${{ matrix.python }} on ${{ matrix.os }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python }}
     - name: Install base dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox codecov
     - name: Install graphviz dependency
       if: ${{ contains(matrix.toxenv, 'build_docs') }}
       run: sudo apt-get -y install graphviz
     - name: Test with tox
       run: |
         tox -e ${{ matrix.toxenv }}
-    # This is an example of how to upload coverage to codecov
-    # - name: Upload coverage to codecov
-    #   if: "contains(matrix.toxenv, '-cov')"
-    #   uses: codecov/codecov-action@v1
-    #   with:
-    #     file: ./coverage.xml
```

### Comparing `astroplan-0.8/.gitignore` & `astroplan-0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/.readthedocs.yml` & `astroplan-0.9/.readthedocs.yml`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,23 @@
 sphinx:
    configuration: docs/conf.py
 
 # Optionally build your docs in additional formats such as PDF
 formats:
    - pdf
 
+build:
+  os: ubuntu-20.04
+  apt_packages:
+    - graphviz
+  tools:
+    python: "3.9"
+
+
 # Optionally set the version of Python and requirements required to build your docs
 python:
-  version: 3.7
   install:
     - requirements: docs/rtd-pip-requirements
     - method: pip
       path: .
       extra_requirements:
         - docs
```

### Comparing `astroplan-0.8/CHANGES.rst` & `astroplan-0.9/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+0.9 (unreleased)
+----------------
+
+- Fix time range in ``months_observable`` to not be only in 2014. Function now
+  accepts argument ``time_range`` and defaults to the current year. [#458]
+
+- Fix ``Observer`` not having longtitude, latitude, and elevation parameters
+  as class attributes. They are now properties calculated from the ``location``.
+
+- Documentation revisions and theme update [#563]
+
 0.8 (2021-01-26)
 ----------------
 
 - Fix Read The Docs compatibility [#497]
 
 - Move to APE 17 infrastructure, change to github actions [#493]
```

### Comparing `astroplan-0.8/CITATION` & `astroplan-0.9/CITATION.bib`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-If you use astroplan in your work, please cite this paper: 
-
-http://adsabs.harvard.edu/abs/2018AJ....155..128M
-
-The recommended BibTeX entry for the above citation is:
-
 @ARTICLE{astroplan2018,
    author = {{Morris}, B.~M. and {Tollerud}, E. and {Sip{\H o}cz}, B. and
     {Deil}, C. and {Douglas}, S.~T. and {Berlanga Medina}, J. and
     {Vyhmeister}, K. and {Smith}, T.~R. and {Littlefair}, S. and
     {Price-Whelan}, A.~M. and {Gee}, W.~T. and {Jeschke}, E.},
     title = "{astroplan: An Open Source Observation Planning Package in Python}",
   journal = {\aj},
```

### Comparing `astroplan-0.8/LICENSE.rst` & `astroplan-0.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/PKG-INFO` & `astroplan-0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,71 @@
 Metadata-Version: 2.1
 Name: astroplan
-Version: 0.8
+Version: 0.9
 Summary: Observation planning package for astronomers
 Home-page: https://github.com/astropy/astroplan
 Author: Astroplan developers
 Author-email: astropy-dev@googlegroups.com
 License: BSD
-Description: astroplan
-        =========
-        
-        Observation planning package for astronomers
-        
-        * Code: https://github.com/astropy/astroplan
-        * Docs: https://astroplan.readthedocs.io/
-        * License: BSD-3
-        
-        .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
-            :target: http://www.astropy.org/
-        
-        .. image:: http://img.shields.io/pypi/v/astroplan.svg?text=version
-            :target: https://pypi.python.org/pypi/astroplan/
-            :alt: Latest release
-            
-        .. image:: http://img.shields.io/badge/arXiv-1709.03913-red.svg?style=flat
-            :target: https://arxiv.org/abs/1712.09631
-            :alt: arXiv paper
-        
-        Attribution
-        +++++++++++
-        
-        If you use astroplan in your work, please cite `Morris et al. 2018 <https://ui.adsabs.harvard.edu/abs/2018AJ....155..128M/abstract>`_: 
-        
-        .. code :: bibtex
-        
-          @ARTICLE{2018AJ....155..128M,
-                 author = {{Morris}, Brett M. and {Tollerud}, Erik and {Sip{\H{o}}cz}, Brigitta and {Deil}, Christoph and {Douglas}, Stephanie T. and {Berlanga Medina}, Jazmin and {Vyhmeister}, Karl and {Smith}, Toby R. and {Littlefair}, Stuart and {Price-Whelan}, Adrian M. and {Gee}, Wilfred T. and {Jeschke}, Eric},
-                  title = "{astroplan: An Open Source Observation Planning Package in Python}",
-                journal = {\aj},
-               keywords = {methods: numerical, methods: observational, Astrophysics - Instrumentation and Methods for Astrophysics},
-                   year = 2018,
-                  month = mar,
-                 volume = {155},
-                 number = {3},
-                    eid = {128},
-                  pages = {128},
-                    doi = {10.3847/1538-3881/aaa47e},
-          archivePrefix = {arXiv},
-                 eprint = {1712.09631},
-           primaryClass = {astro-ph.IM},
-                 adsurl = {https://ui.adsabs.harvard.edu/abs/2018AJ....155..128M},
-                adsnote = {Provided by the SAO/NASA Astrophysics Data System}
-          }
-        
-        
-        
-        
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: plotting
+License-File: LICENSE.rst
+
+astroplan
+=========
+
+Observation planning package for astronomers
+
+* Code: https://github.com/astropy/astroplan
+* Docs: https://astroplan.readthedocs.io/
+* License: BSD-3
+
+.. image:: https://readthedocs.org/projects/astroplan/badge/?version=latest
+    :target: https://astroplan.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: http://img.shields.io/badge/arXiv-1709.03913-red.svg?style=flat
+    :target: https://arxiv.org/abs/1712.09631
+    :alt: arXiv paper
+
+.. image:: https://github.com/astropy/astroplan/workflows/CI%20Tests/badge.svg
+    :target: https://github.com/astropy/astroplan/actions
+
+.. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
+    :target: http://www.astropy.org/
+
+.. image:: http://img.shields.io/pypi/v/astroplan.svg?text=version
+    :target: https://pypi.python.org/pypi/astroplan/
+    :alt: Latest release
+
+Attribution
++++++++++++
+
+If you use astroplan in your work, please cite `Morris et al. 2018 <https://ui.adsabs.harvard.edu/abs/2018AJ....155..128M/abstract>`_: 
+
+.. code :: bibtex
+
+  @ARTICLE{2018AJ....155..128M,
+         author = {{Morris}, Brett M. and {Tollerud}, Erik and {Sip{\H{o}}cz}, Brigitta and {Deil}, Christoph and {Douglas}, Stephanie T. and {Berlanga Medina}, Jazmin and {Vyhmeister}, Karl and {Smith}, Toby R. and {Littlefair}, Stuart and {Price-Whelan}, Adrian M. and {Gee}, Wilfred T. and {Jeschke}, Eric},
+          title = "{astroplan: An Open Source Observation Planning Package in Python}",
+        journal = {\aj},
+       keywords = {methods: numerical, methods: observational, Astrophysics - Instrumentation and Methods for Astrophysics},
+           year = 2018,
+          month = mar,
+         volume = {155},
+         number = {3},
+            eid = {128},
+          pages = {128},
+            doi = {10.3847/1538-3881/aaa47e},
+  archivePrefix = {arXiv},
+         eprint = {1712.09631},
+   primaryClass = {astro-ph.IM},
+         adsurl = {https://ui.adsabs.harvard.edu/abs/2018AJ....155..128M},
+        adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+  }
+
+
+
```

### Comparing `astroplan-0.8/README.rst` & `astroplan-0.9/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,31 @@
 
 Observation planning package for astronomers
 
 * Code: https://github.com/astropy/astroplan
 * Docs: https://astroplan.readthedocs.io/
 * License: BSD-3
 
+.. image:: https://readthedocs.org/projects/astroplan/badge/?version=latest
+    :target: https://astroplan.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: http://img.shields.io/badge/arXiv-1709.03913-red.svg?style=flat
+    :target: https://arxiv.org/abs/1712.09631
+    :alt: arXiv paper
+
+.. image:: https://github.com/astropy/astroplan/workflows/CI%20Tests/badge.svg
+    :target: https://github.com/astropy/astroplan/actions
+
 .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
     :target: http://www.astropy.org/
 
 .. image:: http://img.shields.io/pypi/v/astroplan.svg?text=version
     :target: https://pypi.python.org/pypi/astroplan/
     :alt: Latest release
-    
-.. image:: http://img.shields.io/badge/arXiv-1709.03913-red.svg?style=flat
-    :target: https://arxiv.org/abs/1712.09631
-    :alt: arXiv paper
 
 Attribution
 +++++++++++
 
 If you use astroplan in your work, please cite `Morris et al. 2018 <https://ui.adsabs.harvard.edu/abs/2018AJ....155..128M/abstract>`_: 
 
 .. code :: bibtex
```

### Comparing `astroplan-0.8/astroplan/__init__.py` & `astroplan-0.9/astroplan/__init__.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/astroplan/conftest.py` & `astroplan-0.9/astroplan/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 """
 try:
     from pytest_astropy_header.display import PYTEST_HEADER_MODULES, TESTED_VERSIONS
 except ImportError:  # In case this plugin is not installed
     PYTEST_HEADER_MODULES = {}
     TESTED_VERSIONS = {}
 
-from astropy.tests.helper import enable_deprecations_as_exceptions
-
 # We do this to pick up the test header report even when using LTS astropy
 try:
     from astropy.tests.pytest_plugins import pytest_report_header  # noqa
 except ImportError:
     pass
 
 import os
@@ -32,18 +30,14 @@
 except ImportError:
     version = 'dev'
 
 packagename = os.path.basename(os.path.dirname(__file__))
 TESTED_VERSIONS[packagename] = version
 
 
-# Comment out this line to avoid deprecation warnings being raised as
-# exceptions
-enable_deprecations_as_exceptions()
-
 # Define list of packages for which to display version numbers in the test log
 try:
     PYTEST_HEADER_MODULES['Astropy'] = 'astropy'
     PYTEST_HEADER_MODULES['pytz'] = 'pytz'
     PYTEST_HEADER_MODULES['pyephem'] = 'ephem'
     PYTEST_HEADER_MODULES['matplotlib'] = 'matplotlib'
     PYTEST_HEADER_MODULES['pytest-mpl'] = 'pytest_mpl'
```

### Comparing `astroplan-0.8/astroplan/constraints.py` & `astroplan-0.9/astroplan/constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,39 +6,47 @@
 
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
 
 # Standard library
 from abc import ABCMeta, abstractmethod
 import datetime
+import time
 import warnings
 
 # Third-party
 from astropy.time import Time
 import astropy.units as u
-from astropy.coordinates import get_body, get_sun, get_moon, Galactic, SkyCoord
+from astropy.coordinates import get_body, get_sun, Galactic, SkyCoord
 from astropy import table
 
 import numpy as np
 from numpy.lib.stride_tricks import as_strided
 
 # Package
 from .moon import moon_illumination
 from .utils import time_grid_from_range
 from .target import get_skycoord
+from .exceptions import MissingConstraintWarning
 
 __all__ = ["AltitudeConstraint", "AirmassConstraint", "AtNightConstraint",
            "is_observable", "is_always_observable", "time_grid_from_range",
            "GalacticLatitudeConstraint", "SunSeparationConstraint",
            "MoonSeparationConstraint", "MoonIlluminationConstraint",
            "LocalTimeConstraint", "PrimaryEclipseConstraint",
            "SecondaryEclipseConstraint", "Constraint", "TimeConstraint",
            "observability_table", "months_observable", "max_best_rescale",
            "min_best_rescale", "PhaseConstraint", "is_event_observable"]
 
+_current_year = time.localtime().tm_year  # needed for backward compatibility
+_current_year_time_range = Time(  # needed for backward compatibility
+    [str(_current_year) + '-01-01',
+     str(_current_year) + '-12-31']
+)
+
 
 def _make_cache_key(times, targets):
     """
     Make a unique key to reference this combination of ``times`` and ``targets``.
 
     Often, we wish to store expensive calculations for a combination of
     ``targets`` and ``times`` in a cache on an ``observer``` object. This
@@ -342,15 +350,15 @@
         cached_altaz = _get_altaz(times, observer, targets)
         alt = cached_altaz['altaz'].alt
         if self.boolean_constraint:
             lowermask = self.min <= alt
             uppermask = alt <= self.max
             return lowermask & uppermask
         else:
-            return max_best_rescale(alt, self.min, self.max)
+            return max_best_rescale(alt, self.min, self.max, greater_than_max=0)
 
 
 class AirmassConstraint(AltitudeConstraint):
     """
     Constrain the airmass of a target.
 
     In the current implementation the airmass is approximated by the secant of
@@ -578,19 +586,15 @@
             set to 'builtin' by default).
         """
         self.min = min
         self.max = max
         self.ephemeris = ephemeris
 
     def compute_constraint(self, times, observer, targets):
-        # removed the location argument here, which causes small <1 deg
-        # innacuracies, but it is needed until astropy PR #5897 is released
-        # which should be astropy 1.3.2
-        moon = get_moon(times,
-                        ephemeris=self.ephemeris)
+        moon = get_body("moon", times, location=observer.location, ephemeris=self.ephemeris)
         # note to future editors - the order matters here
         # moon.separation(targets) is NOT the same as targets.separation(moon)
         # the former calculates the separation in the frame of the moon coord
         # which is GCRS, and that is what we want.
         moon_separation = moon.separation(targets)
 
         if self.min is None and self.max is not None:
@@ -1082,30 +1086,35 @@
 
         constraint_arr = np.logical_and(np.logical_and.reduce(applied_constraints_ing),
                                         np.logical_and.reduce(applied_constraints_egr))
     return constraint_arr
 
 
 def months_observable(constraints, observer, targets,
+                      time_range=_current_year_time_range,
                       time_grid_resolution=0.5*u.hour):
     """
     Determines which month the specified ``targets`` are observable for a
-    specific ``observer``, given the supplied ``constriants``.
+    specific ``observer``, given the supplied ``constraints``.
 
     Parameters
     ----------
     constraints : list or `~astroplan.constraints.Constraint`
         Observational constraint(s)
 
     observer : `~astroplan.Observer`
         The observer who has constraints ``constraints``
 
     targets : {list, `~astropy.coordinates.SkyCoord`, `~astroplan.FixedTarget`}
         Target or list of targets
 
+    time_range : `~astropy.time.Time` (optional)
+        Lower and upper bounds on time sequence
+        If ``time_range`` is not specified, defaults to current year (localtime)
+
     time_grid_resolution : `~astropy.units.Quantity` (optional)
         If ``time_range`` is specified, determine whether constraints are met
         between test times in ``time_range`` by checking constraint at
         linearly-spaced times separated by ``time_resolution``. Default is 0.5
         hours.
 
     Returns
@@ -1117,22 +1126,28 @@
 
     """
     # TODO: This method could be sped up a lot by dropping to the trigonometric
     # altitude calculations.
     if not hasattr(constraints, '__len__'):
         constraints = [constraints]
 
-    # Calculate throughout the year of 2014 so as not to require forward
-    # extrapolation off of the IERS tables
-    time_range = Time(['2014-01-01', '2014-12-31'])
     times = time_grid_from_range(time_range, time_grid_resolution)
 
+    # If the constraints don't include AltitudeConstraint or its subclasses,
+    # warn the user that they may get months when the target is below the horizon
+    altitude_constraint_supplied = any(
+        [isinstance(constraint, AltitudeConstraint) for constraint in constraints]
+    )
+    if not altitude_constraint_supplied:
+        message = ("months_observable usually expects an AltitudeConstraint or "
+                   "AirmassConstraint to ensure targets are above horizon.")
+        warnings.warn(message, MissingConstraintWarning)
+
     # TODO: This method could be sped up a lot by dropping to the trigonometric
     # altitude calculations.
-
     applied_constraints = [constraint(observer, targets,
                                       times=times,
                                       grid_times_targets=True)
                            for constraint in constraints]
     constraint_arr = np.logical_and.reduce(applied_constraints)
 
     months_observable = []
```

### Comparing `astroplan-0.8/astroplan/exceptions.py` & `astroplan-0.9/astroplan/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
 
 from astropy.utils.exceptions import AstropyWarning
 
 __all__ = ["TargetAlwaysUpWarning", "TargetNeverUpWarning",
            "OldEarthOrientationDataWarning", "PlotWarning",
-           "PlotBelowHorizonWarning", "AstroplanWarning"]
+           "PlotBelowHorizonWarning", "AstroplanWarning",
+           "MissingConstraintWarning"]
 
 
 class AstroplanWarning(AstropyWarning):
     """Superclass for warnings used by astroplan"""
 
 
 class TargetAlwaysUpWarning(AstroplanWarning):
@@ -32,7 +33,12 @@
     """Warnings dealing with the plotting aspects of astroplan"""
     pass
 
 
 class PlotBelowHorizonWarning(PlotWarning):
     """Warning for when something is hidden on a plot because it's below the horizon"""
     pass
+
+
+class MissingConstraintWarning(AstroplanWarning):
+    """Triggered when a constraint is expected but not supplied"""
+    pass
```

### Comparing `astroplan-0.8/astroplan/moon.py` & `astroplan-0.9/astroplan/moon.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
 
 # Third-party
 import numpy as np
-from astropy.coordinates import get_moon, get_sun
+from astropy.coordinates import get_sun, get_body
 
 __all__ = ["moon_phase_angle", "moon_illumination"]
 
 
 def moon_phase_angle(time, ephemeris=None):
     """
     Calculate lunar orbital phase in radians.
@@ -25,21 +25,21 @@
     ephemeris : str, optional
         Ephemeris to use.  If not given, use the one set with
         `~astropy.coordinates.solar_system_ephemeris` (which is
         set to 'builtin' by default).
 
     Returns
     -------
-    i : float
+    i : `~astropy.units.Quantity`
         Phase angle of the moon [radians]
     """
     # TODO: cache these sun/moon SkyCoord objects
 
     sun = get_sun(time)
-    moon = get_moon(time, ephemeris=ephemeris)
+    moon = get_body("moon", time, ephemeris=ephemeris)
     elongation = sun.separation(moon)
     return np.arctan2(sun.distance*np.sin(elongation),
                       moon.distance - sun.distance*np.cos(elongation))
 
 
 def moon_illumination(time, ephemeris=None):
     """
```

### Comparing `astroplan-0.8/astroplan/observer.py` & `astroplan-0.9/astroplan/observer.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,17 @@
                         unicode_literals)
 from six import string_types
 
 # Standard library
 import sys
 import datetime
 import warnings
-
 # Third-party
 from astropy.coordinates import (EarthLocation, SkyCoord, AltAz, get_sun,
-                                 get_moon, Angle, Longitude)
+                                 get_body, Angle, Longitude)
 import astropy.units as u
 from astropy.time import Time
 from astropy.utils.exceptions import AstropyDeprecationWarning
 import numpy as np
 import pytz
 
 # Package
@@ -44,14 +43,28 @@
     return DeprecateWrapper()
 
 
 sys.modules[__name__] = deprecation_wrap_module(sys.modules[__name__],
                                                 deprecated=['MAGIC_TIME'])
 
 
+def _process_nans_in_jds(jds):
+    """
+    Some functions calculate times for events that won't happen, yielding nans. This wrapper
+    manages vectors of (potentially) invalid JDs that must be passed to the astropy.time.Time
+    constructor. Returns a masked Time object.
+    """
+    if np.isscalar(jds):
+        jds = np.array([jds])
+    not_finite = ~np.isfinite(jds)
+    masked_jds = np.ma.masked_array(jds.to(u.day).value if hasattr(jds, 'unit') else jds.copy())
+    masked_jds[not_finite] = np.ma.masked
+    return masked_jds
+
+
 def _generate_24hr_grid(t0, start, end, n_grid_points, for_deriv=False):
     """
     Generate a nearly linearly spaced grid of time durations.
 
     The midpoints of these grid points will span times from ``t0``+``start``
     to ``t0``+``end``, including the end points, which is useful when taking
     numerical derivatives.
@@ -205,14 +218,29 @@
             self.timezone = timezone
         elif isinstance(timezone, string_types):
             self.timezone = pytz.timezone(timezone)
         else:
             raise TypeError('timezone keyword should be a string, or an '
                             'instance of datetime.tzinfo')
 
+    @property
+    def longitude(self):
+        """The longitude of the observing location, derived from the location."""
+        return self.location.lon
+
+    @property
+    def latitude(self):
+        """The latitude of the observing location, derived from the location."""
+        return self.location.lat
+
+    @property
+    def elevation(self):
+        """The elevation of the observing location with respect to sea level."""
+        return self.location.height
+
     def __repr__(self):
         """
         String representation of the `~astroplan.Observer` object.
 
         Examples
         --------
 
@@ -241,14 +269,93 @@
                     if name != 'name':
                         value = repr(value)
                     else:
                         value = "'{}'".format(value)
                     attributes_strings.append("{}={}".format(name, value))
         return "<{}: {}>".format(class_name, ",\n    ".join(attributes_strings))
 
+    def _key(self):
+        """
+        Generate a tuple of the attributes that determine uniqueness of
+        `~astroplan.Observer` objects.
+
+        Returns
+        -------
+        key : tuple
+
+        Examples
+        --------
+
+        >>> from astroplan import Observer
+        >>> keck = Observer.at_site("Keck", timezone="US/Hawaii")
+        >>> keck._key()
+        ('Keck', None, None, None, <Longitude -155.47833333 deg>,
+            <Latitude 19.82833333 deg>, <Quantity 4160. m>,
+            <DstTzInfo 'US/Hawaii' LMT-1 day, 13:29:00 STD>)
+        """
+
+        return (self.name,
+                self.pressure,
+                self.temperature,
+                self.relative_humidity,
+                self.longitude,
+                self.latitude,
+                self.elevation,
+                self.timezone,)
+
+    def __hash__(self):
+        """
+        Hash the `~astroplan.Observer` object.
+
+        Examples
+        --------
+
+        >>> from astroplan import Observer
+        >>> keck = Observer.at_site("Keck", timezone="US/Hawaii")
+        >>> hash(keck)
+        -3872382927731250571
+        """
+
+        return hash(self._key())
+
+    def __eq__(self, other):
+        """
+        Equality check for `~astroplan.Observer` objects.
+
+        Examples
+        --------
+
+        >>> from astroplan import Observer
+        >>> keck = Observer.at_site("Keck", timezone="US/Hawaii")
+        >>> keck2 = Observer.at_site("Keck", timezone="US/Hawaii")
+        >>> keck == keck2
+        True
+        """
+
+        if isinstance(other, Observer):
+            return self._key() == other._key()
+        else:
+            return NotImplemented
+
+    def __ne__(self, other):
+        """
+        Inequality check for `~astroplan.Observer` objects.
+
+        Examples
+        --------
+
+        >>> from astroplan import Observer
+        >>> keck = Observer.at_site("Keck", timezone="US/Hawaii")
+        >>> kpno = Observer.at_site("KPNO", timezone="US/Arizona")
+        >>> keck != kpno
+        True
+        """
+
+        return not self.__eq__(other)
+
     @classmethod
     def at_site(cls, site_name, **kwargs):
         """
         Initialize an `~astroplan.observer.Observer` object with a site name.
 
         Extra keyword arguments are passed to the `~astroplan.Observer`
         constructor (see `~astroplan.Observer` for available keyword
@@ -480,27 +587,33 @@
 
         Alternatively, construct an alt/az frame and transform the target to
         that frame all in one step:
 
         >>> target_altaz = apo.altaz(time, target) # doctest: +SKIP
         """
         if target is not None:
+            if target is MoonFlag:
+                target = get_body("moon", time, location=self.location)
+            elif target is SunFlag:
+                target = get_sun(time)
+
             time, target = self._preprocess_inputs(time, target, grid_times_targets)
 
         altaz_frame = AltAz(location=self.location, obstime=time,
                             pressure=self.pressure, obswl=obswl,
                             temperature=self.temperature,
                             relative_humidity=self.relative_humidity)
         if target is None:
             # Return just the frame
             return altaz_frame
         else:
             return target.transform_to(altaz_frame)
 
-    def parallactic_angle(self, time, target, grid_times_targets=False):
+    def parallactic_angle(self, time, target, grid_times_targets=False,
+                          kind='mean', model=None):
         """
         Calculate the parallactic angle.
 
         Parameters
         ----------
         time : `~astropy.time.Time`
             Observation time.
@@ -510,14 +623,23 @@
 
         grid_times_targets: bool
             If True, the target object will have extra dimensions packed onto
             the end, so that calculations with M targets and N times will
             return an (M, N) shaped result. Otherwise, we rely on broadcasting
             the shapes together using standard numpy rules.
 
+        kind : str
+            Argument to the `~astropy.time.Time.sidereal_time` function, which may
+            be either ``'mean'`` or ``'apparent'``, i.e., accounting for precession only,
+            or also for nutation.
+
+        model : str or None; optional
+            Precession (and nutation) model to use in the call to
+            `~astropy.time.Time.sidereal_time`, see docs for that method for details.
+
         Returns
         -------
         `~astropy.coordinates.Angle`
             Parallactic angle.
 
         Notes
         -----
@@ -527,15 +649,15 @@
 
         .. [1] https://en.wikipedia.org/wiki/Parallactic_angle
 
         """
         time, coordinate = self._preprocess_inputs(time, target, grid_times_targets)
 
         # Eqn (14.1) of Meeus' Astronomical Algorithms
-        LST = time.sidereal_time('mean', longitude=self.location.lon)
+        LST = time.sidereal_time(kind, longitude=self.location.lon, model=model)
         H = (LST - coordinate.ra).radian
         q = np.arctan2(np.sin(H),
                        (np.tan(self.location.lat.radian) *
                         np.cos(coordinate.dec.radian) -
                         np.sin(coordinate.dec.radian)*np.cos(H)))*u.rad
 
         return Angle(q)
@@ -680,25 +802,17 @@
             Time when target crosses the horizon
 
         """
         # Approximate the horizon-crossing time:
         slope = (alt_after-alt_before) / ((jd_after - jd_before) * u.d)
         crossing_jd = (jd_after * u.d - ((alt_after - horizon) / slope))
 
-        # TODO: edit after https://github.com/astropy/astropy/issues/9612 has
-        # been addressed.
-
         # Determine whether or not there are NaNs in the crossing_jd array which
         # represent computations where no horizon crossing was found:
-        nans = np.isnan(crossing_jd)
-        # If there are, set them equal to zero, rather than np.nan
-        crossing_jd[nans] = 0
-        times = Time(crossing_jd, format='jd')
-        # Create a Time object with masked out times where there were NaNs
-        times[nans] = np.ma.masked
+        times = Time(_process_nans_in_jds(crossing_jd), format='jd')
 
         return np.squeeze(times)
 
     def _altitude_trig(self, LST, target, grid_times_targets=False):
         """
         Calculate the altitude of ``target`` at local sidereal times ``LST``.
 
@@ -785,23 +899,16 @@
         else:
             start = (-1 - (target.approx_sidereal_drift.to(u.day).value
                            if hasattr(target, 'approx_sidereal_drift') else 0))
             end = 0
 
         times = _generate_24hr_grid(time, start, end, n_grid_points)
 
-        if target is MoonFlag:
-            altaz = self.altaz(times, get_moon(times, location=self.location),
-                               grid_times_targets=grid_times_targets)
-        elif target is SunFlag:
-            altaz = self.altaz(times, get_sun(times),
-                               grid_times_targets=grid_times_targets)
-        else:
-            altaz = self.altaz(times, target,
-                               grid_times_targets=grid_times_targets)
+        altaz = self.altaz(times, target,
+                           grid_times_targets=grid_times_targets)
 
         altitudes = altaz.alt
 
         al1, al2, jd1, jd2 = self._horiz_cross(times, altitudes, rise_set,
                                                horizon)
         return self._two_point_interp(jd1, jd2, al1, al2,
                                       horizon=horizon)
@@ -859,15 +966,17 @@
         # The derivative of the altitude with respect to time is increasing
         # from negative to positive values at the anti-transit of the meridian
         if antitransit:
             rise_set = 'rising'
         else:
             rise_set = 'setting'
 
-        altaz = self.altaz(times, target, grid_times_targets=grid_times_targets)
+        altaz = self.altaz(times, target,
+                           grid_times_targets=grid_times_targets)
+
         altitudes = altaz.alt
         if altitudes.ndim > 2:
             # shape is (M, N, ...) where M is targets and N is grid
             d_altitudes = altitudes.diff(axis=1)
         else:
             # shape is (N, M) where M is targets and N is grid
             d_altitudes = altitudes.diff(axis=0)
@@ -920,28 +1029,21 @@
 
         if which == 'previous' or which == 'nearest':
             previous_event = event_function('previous')
             if which == 'previous':
                 return previous_event
 
         if which == 'nearest':
-            # Use some hacks to handle the non-rising/non-setting cases
             try:
                 mask = abs(time - previous_event) < abs(time - next_event)
+                ma = np.where(mask, previous_event.utc.jd, next_event.utc.jd)
             except TypeError:
                 # encountered if time is scalar & nan
-                return next_event
-            ma = np.where(mask, previous_event.utc.jd, next_event.utc.jd)
-            # HACK: Time objects cannot be initiated w/NaN, so we first
-            # make them zero, then change them to NaN
-            not_finite = ~np.isfinite(ma)
-            ma[not_finite] = 0
-            tm = Time(ma, format='jd')
-            tm[not_finite] = np.nan
-            return tm
+                ma = next_event.utc.jd if not next_event.isscalar else [next_event.utc.jd]
+            return Time(_process_nans_in_jds(ma), format='jd', scale='utc')
 
         raise ValueError('"which" kwarg must be "next", "previous" or '
                          '"nearest".')
 
     @u.quantity_input(horizon=u.deg)
     def target_rise_time(self, time, target, which='nearest',
                          horizon=0*u.degree, grid_times_targets=False, n_grid_points=150):
@@ -1707,15 +1809,15 @@
         >>> altaz_moon = apo.moon_altaz(time) # doctest: +SKIP
         >>> print("alt: {0.alt}, az: {0.az}".format(altaz_moon)) # doctest: +SKIP
         alt: -63.72706397691421 deg, az: 345.3640380598265 deg
         """
         if not isinstance(time, Time):
             time = Time(time)
 
-        moon = get_moon(time, location=self.location, ephemeris=ephemeris)
+        moon = get_body("moon", time, location=self.location, ephemeris=ephemeris)
         return self.altaz(time, moon)
 
     def sun_altaz(self, time):
         """
         Returns the position of the Sun in alt/az.
 
         Parameters
```

### Comparing `astroplan-0.8/astroplan/periodic.py` & `astroplan-0.9/astroplan/periodic.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/astroplan/plots/finder.py` & `astroplan-0.9/astroplan/plots/finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     hdu = SkyView.get_images(position=position, coordinates=coordinates,
                              survey=survey, radius=fov_radius, grid=grid)[0][0]
     wcs = WCS(hdu.header)
 
     # Set up axes & plot styles if needed.
     if ax is None:
-        ax = plt.gca(projection=wcs)
+        ax = plt.gcf().add_subplot(projection=wcs)
     if style_kwargs is None:
         style_kwargs = {}
     style_kwargs = dict(style_kwargs)
     style_kwargs.setdefault('cmap', 'Greys')
     style_kwargs.setdefault('origin', 'lower')
 
     if log:
```

### Comparing `astroplan-0.8/astroplan/plots/mplstyles.py` & `astroplan-0.9/astroplan/plots/mplstyles.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/astroplan/plots/sky.py` & `astroplan-0.9/astroplan/plots/sky.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import numpy as np
 import astropy.units as u
 from astropy.time import Time
 import warnings
 
 from ..exceptions import PlotBelowHorizonWarning
 from ..utils import _set_mpl_style_sheet
@@ -113,15 +110,21 @@
     if style_sheet is not None:
         _set_mpl_style_sheet(style_sheet)
 
     import matplotlib.pyplot as plt
 
     # Set up axes & plot styles if needed.
     if ax is None:
-        ax = plt.gca(projection='polar')
+        if isinstance(plt.gca(), plt.PolarAxes):
+            ax = plt.gca()
+        else:
+            plt.close()
+            fig = plt.gcf()
+            ax = fig.add_subplot(projection='polar')
+
     if style_kwargs is None:
         style_kwargs = {}
     style_kwargs = dict(style_kwargs)
     style_kwargs.setdefault('marker', 'o')
 
     # Turn scalar Time objects into arrays.
     time = Time(time)
```

### Comparing `astroplan-0.8/astroplan/plots/tests/baseline_images/test_image_example.png` & `astroplan-0.9/astroplan/plots/tests/baseline_images/test_image_example.png`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/astroplan/plots/tests/test_sky.py` & `astroplan-0.9/astroplan/plots/tests/test_sky.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/astroplan/plots/time_dependent.py` & `astroplan-0.9/astroplan/plots/time_dependent.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,17 +148,19 @@
 
     # Set up plot axes and style if needed.
     if ax is None:
         ax = plt.gca()
     if style_kwargs is None:
         style_kwargs = {}
     style_kwargs = dict(style_kwargs)
-    style_kwargs.setdefault('linestyle', '-')
-    style_kwargs.setdefault('linewidth', 1.5)
-    style_kwargs.setdefault('fmt', '-')
+
+    if 'lw' not in style_kwargs:
+        style_kwargs.setdefault('linewidth', 1.5)
+    if 'ls' not in style_kwargs and 'linestyle' not in style_kwargs:
+        style_kwargs.setdefault('fmt', '-')
 
     if hasattr(time, 'utcoffset') and use_local_tz:
         tzoffset = time.utcoffset()
         tzname = time.tzname()
         tzinfo = time.tzinfo
     else:
         tzoffset = 0
@@ -363,17 +365,18 @@
 
     # Set up plot axes and style if needed.
     if ax is None:
         ax = plt.gca()
     if style_kwargs is None:
         style_kwargs = {}
     style_kwargs = dict(style_kwargs)
-    style_kwargs.setdefault('linestyle', '-')
-    style_kwargs.setdefault('linewidth', 1.5)
-    style_kwargs.setdefault('fmt', '-')
+    if 'ls' not in style_kwargs and 'fmt' not in style_kwargs:
+        style_kwargs.setdefault('linestyle', '-')
+    if 'lw' not in style_kwargs:
+        style_kwargs.setdefault('linewidth', 1.5)
 
     # Populate time window if needed.
     time = Time(time)
     if time.isscalar:
         time = time + np.linspace(-12, 12, 100)*u.hour
     elif len(time) == 1:
         warnings.warn('You used a Time array of length 1.  You probably meant '
@@ -588,16 +591,17 @@
 
     # Set up plot axes and style if needed.
     if ax is None:
         ax = plt.gca()
     if style_kwargs is None:
         style_kwargs = {}
     style_kwargs = dict(style_kwargs)
-    style_kwargs.setdefault('linestyle', '-')
     style_kwargs.setdefault('fmt', '-')
+    if 'ls' not in style_kwargs and 'fmt' not in style_kwargs:
+        style_kwargs.setdefault('linestyle', '-')
 
     # Populate time window if needed.
     time = Time(time)
     if time.isscalar:
         time = time + np.linspace(-12, 12, 100)*u.hour
     elif len(time) == 1:
         warnings.warn('You used a Time array of length 1.  You probably meant '
```

### Comparing `astroplan-0.8/astroplan/scheduling.py` & `astroplan-0.9/astroplan/scheduling.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 class ObservingBlock(object):
     """
     An observation to be scheduled, consisting of a target and associated
     constraints on observations.
     """
     @u.quantity_input(duration=u.second)
-    def __init__(self, target, duration, priority, configuration={}, constraints=None):
+    def __init__(self, target, duration, priority, configuration={}, constraints=None, name=None):
         """
         Parameters
         ----------
         target : `~astroplan.FixedTarget`
             Target to observe
 
         duration : `~astropy.units.Quantity`
@@ -48,20 +48,24 @@
             Configuration metadata
 
         constraints : list of `~astroplan.constraints.Constraint` objects
             The constraints to apply to this particular observing block.  Note
             that constraints applicable to the entire list should go into the
             scheduler.
 
+        name : integer or str
+            User-defined name or ID.
+
         """
         self.target = target
         self.duration = duration
         self.priority = priority
         self.configuration = configuration
         self.constraints = constraints
+        self.name = name
         self.start_time = self.end_time = None
         self.observer = None
 
     def __repr__(self):
         orig_repr = object.__repr__(self)
         if self.start_time is None or self.end_time is None:
             return orig_repr.replace('object at',
@@ -227,15 +231,15 @@
     """
     # as currently written, there should be no consecutive unoccupied slots
     # this should change to allow for more flexibility (e.g. dark slots, grey slots)
 
     def __init__(self, start_time, end_time, constraints=None):
         """
         Parameters
-        -----------
+        ----------
         start_time : `~astropy.time.Time`
             The starting time of the schedule; the start of your
             observing window.
         end_time : `~astropy.time.Time`
            The ending time of the schedule; the end of your
            observing window
         constraints : sequence of `~astroplan.constraints.Constraint` s
@@ -274,16 +278,16 @@
         config = []
         for slot in self.slots:
             if hasattr(slot.block, 'target'):
                 start_times.append(slot.start.iso)
                 end_times.append(slot.end.iso)
                 durations.append(slot.duration.to(u.minute).value)
                 target_names.append(slot.block.target.name)
-                ra.append(slot.block.target.ra)
-                dec.append(slot.block.target.dec)
+                ra.append(u.Quantity(slot.block.target.ra))
+                dec.append(u.Quantity(slot.block.target.dec))
                 config.append(slot.block.configuration)
             elif show_transitions and slot.block:
                 start_times.append(slot.start.iso)
                 end_times.append(slot.end.iso)
                 durations.append(slot.duration.to(u.minute).value)
                 target_names.append('TransitionBlock')
                 ra.append('')
@@ -296,16 +300,15 @@
                 start_times.append(slot.start.iso)
                 end_times.append(slot.end.iso)
                 durations.append(slot.duration.to(u.minute).value)
                 target_names.append('Unused Time')
                 ra.append('')
                 dec.append('')
                 config.append('')
-        return Table([target_names, start_times, end_times, durations,
-                      u.Quantity(ra), u.Quantity(dec), config],
+        return Table([target_names, start_times, end_times, durations, ra, dec, config],
                      names=('target', 'start time (UTC)', 'end time (UTC)',
                             'duration (minutes)', 'ra', 'dec', 'configuration'))
 
     def new_slots(self, slot_index, start_time, end_time):
         """
         Create new slots by splitting a current slot.
 
@@ -424,15 +427,15 @@
     """
     A time slot consisting of a start and end time
     """
 
     def __init__(self, start_time, end_time):
         """
         Parameters
-        -----------
+        ----------
         start_time : `~astropy.time.Time`
             The starting time of the slot
         end_time : `~astropy.time.Time`
             The ending time of the slot
         """
         self.start = start_time
         self.end = end_time
@@ -741,15 +744,15 @@
 
         # generate the score arrays for all of the blocks
         scorer = Scorer(blocks, self.observer, self.schedule,
                         global_constraints=self.constraints)
         score_array = scorer.create_score_array(time_resolution)
 
         # Sort the list of blocks by priority
-        sorted_indices = np.argsort(_block_priorities)
+        sorted_indices = np.argsort(_block_priorities, kind='mergesort')
 
         unscheduled_blocks = []
         # Compute the optimal observation time in priority order
         for i in sorted_indices:
             b = blocks[i]
             # Compute possible observing times by combining object constraints
             # with the master open times mask
@@ -759,15 +762,15 @@
             # And then remove any times that are already scheduled
             is_open_time = self._get_filled_indices(times)
             constraint_scores[~is_open_time] = 0
 
             # Select the most optimal time
 
             # calculate the number of time slots needed for this exposure
-            _stride_by = np.int(np.ceil(float(b.duration / time_resolution)))
+            _stride_by = int(np.ceil(float(b.duration / time_resolution)))
 
             # Stride the score arrays by that number
             _strided_scores = stride_array(constraint_scores, _stride_by)
 
             # Collapse the sub-arrays
             # (run them through scorekeeper again? Just add them?
             # If there's a zero anywhere in there, def. have to skip)
@@ -779,15 +782,15 @@
                 # No further calculation if no times meet the constraints
                 _is_scheduled = False
             else:
                 # schedulable in principle, provided the transition
                 # does not prevent us from fitting it in.
                 # loop over valid times and see if it fits
                 # TODO: speed up by searching multiples of time resolution?
-                for idx in np.argsort(sum_scores)[::-1]:
+                for idx in np.argsort(-sum_scores, kind='mergesort'):
                     if sum_scores[idx] <= 0.0:
                         # we've run through all optimal blocks
                         _is_scheduled = False
                         break
                     try:
                         start_time_idx = idx
                         new_start_time = times[start_time_idx]
@@ -803,15 +806,15 @@
             if not _is_scheduled:
                 unscheduled_blocks.append(b)
 
         return self.schedule
 
     def attempt_insert_block(self, b, new_start_time, start_time_idx):
         # set duration to be exact multiple of time resolution
-        duration_indices = np.int(np.ceil(
+        duration_indices = int(np.floor(
             float(b.duration / self.time_resolution)))
         b.duration = duration_indices * self.time_resolution
 
         # add 1 second to the start time to allow for scheduling at the start of a slot
         slot_index = [q for q, slot in enumerate(self.schedule.slots)
                       if slot.start < new_start_time + 1*u.second < slot.end][0]
         slots_before = self.schedule.slots[:slot_index]
@@ -870,15 +873,15 @@
                 tb_after = self.transitioner(
                     b, self.schedule.slots[slot_index + slot_offset].block,
                     new_start_time + b.duration, self.observer)
 
         # tweak durations to exact multiple of time resolution
         for block in (tb_before, tb_after):
             if block is not None:
-                block.duration = self.time_resolution * np.int(
+                block.duration = self.time_resolution * int(
                     np.ceil(float(block.duration / self.time_resolution))
                 )
 
         # if we want to shift the OBs to minimise gaps, here is
         # where we should do it.
         # Find the smallest shift (forward or backward) to close gap
         # Check against tolerances (constraints must still be met)
@@ -887,30 +890,30 @@
         # Now let's see if the block and transition can fit in the schedule
         if slots_before:
             # we're OK if the index at the end of the updated transition
             # is less than or equal to `start_time_idx`
             ob_offset = 2 if tb_before_already_exists else 1
             previous_ob = self.schedule.slots[slot_index - ob_offset]
             if tb_before:
-                transition_indices = np.int(tb_before.duration / self.time_resolution)
+                transition_indices = int(tb_before.duration / self.time_resolution)
             else:
                 transition_indices = 0
 
             if start_time_idx < previous_ob.block.end_idx + transition_indices:
                 # cannot schedule
                 return False
 
         if slots_after:
             # we're OK if the index at end of OB (plus transition)
             # is smaller than the start_index of the slot after
             slot_offset = 2 if delete_this_block_first else 1
             next_ob = self.schedule.slots[slot_index + slot_offset].block
             end_idx = start_time_idx + duration_indices
             if tb_after:
-                end_idx += np.int(tb_after.duration/self.time_resolution)
+                end_idx += int(tb_after.duration / self.time_resolution)
                 if end_idx >= next_ob.start_idx:
                     # cannot schedule
                     return False
 
         # OK, we should be OK to schedule now!
         try:
             # delete this block if it's a TransitionBlock
```

### Comparing `astroplan-0.8/astroplan/target.py` & `astroplan-0.9/astroplan/target.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/astroplan/tests/coveragerc` & `astroplan-0.9/astroplan/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/astroplan/tests/test_constraints.py` & `astroplan-0.9/astroplan/tests/test_constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
 import datetime as dt
 
 import numpy as np
 import astropy.units as u
 from astropy.time import Time
-from astropy.coordinates import Galactic, SkyCoord, get_sun, get_moon
+from astropy.coordinates import Galactic, SkyCoord, get_sun, get_body
 from astropy.utils import minversion
 import pytest
 
 from ..observer import Observer
 from ..target import FixedTarget, get_skycoord
 from ..constraints import (AltitudeConstraint, AirmassConstraint, AtNightConstraint,
                            is_observable, is_always_observable, observability_table,
@@ -18,14 +18,16 @@
                            SunSeparationConstraint,
                            MoonSeparationConstraint, MoonIlluminationConstraint,
                            TimeConstraint, LocalTimeConstraint, months_observable,
                            max_best_rescale, min_best_rescale, PhaseConstraint,
                            PrimaryEclipseConstraint, SecondaryEclipseConstraint,
                            is_event_observable)
 from ..periodic import EclipsingSystem
+from ..exceptions import MissingConstraintWarning
+
 
 APY_LT104 = not minversion('astropy', '1.0.4')
 
 vega = FixedTarget(coord=SkyCoord(ra=279.23473479*u.deg, dec=38.78368896*u.deg),
                    name="Vega")
 rigel = FixedTarget(coord=SkyCoord(ra=78.63446707*u.deg, dec=8.20163837*u.deg),
                     name="Rigel")
@@ -92,14 +94,25 @@
     stab = observability_table(constraints, subaru, targets,
                                time_range=time_range[0])
 
     assert all(ttab['fraction of time observable'] == stab['fraction of time observable'])
     assert 'time observable' in stab.colnames
 
 
+def test_altitude_constraint():
+    subaru = Observer.at_site("Subaru")
+    time = Time('2001-02-03 15:35:00')
+    time_range = Time([time, time+3*u.hour])
+
+    constraint = AltitudeConstraint(min=40*u.deg, max=50*u.deg, boolean_constraint=False)
+    results = constraint(subaru, vega, times=time_grid_from_range(time_range))
+    # Check if below min and above max values are 0
+    assert np.all([results != 0][0] == [False, False, True,  True,  False, False])
+
+
 def test_compare_altitude_constraint_and_observer():
     time = Time('2001-02-03 04:05:06')
     time_ranges = [Time([time, time+1*u.hour]) + offset
                    for offset in np.arange(0, 400, 100)*u.day]
     for time_range in time_ranges:
         subaru = Observer.at_site("Subaru")
         targets = [vega, rigel, polaris]
@@ -187,15 +200,15 @@
     assert np.all(is_constraint_met == [False, True, True])
 
 
 def test_moon_separation():
     time = Time('2003-04-05 06:07:08')
     apo = Observer.at_site("APO")
     altaz_frame = apo.altaz(time)
-    moon = get_moon(time, apo.location).transform_to(altaz_frame)
+    moon = get_body("moon", time, apo.location).transform_to(altaz_frame)
     one_deg_away = SkyCoord(az=moon.az, alt=moon.alt+1*u.deg, frame=altaz_frame)
     five_deg_away = SkyCoord(az=moon.az+5*u.deg, alt=moon.alt,
                              frame=altaz_frame)
     twenty_deg_away = SkyCoord(az=moon.az+20*u.deg, alt=moon.alt,
                                frame=altaz_frame)
 
     constraint = MoonSeparationConstraint(min=2*u.deg, max=10*u.deg)
@@ -372,21 +385,26 @@
     coords = [SkyCoord(ra=0*u.hourangle, dec=0*u.deg),
               SkyCoord(ra=6*u.hourangle, dec=0*u.deg),
               SkyCoord(ra=12*u.hourangle, dec=0*u.deg),
               SkyCoord(ra=18*u.hourangle, dec=0*u.deg)]
     targets = [FixedTarget(coord=coord) for coord in coords]
     constraints = [AltitudeConstraint(min=80*u.deg),
                    AtNightConstraint.twilight_astronomical()]
-    months = months_observable(constraints, obs, targets)
+    time_range = Time(['2014-01-01', '2014-12-31'])
+    months = months_observable(constraints, obs, targets, time_range)
 
     should_be = [set({7, 8, 9, 10, 11, 12}), set({1, 2, 3, 10, 11, 12}),
                  set({1, 2, 3, 4, 5, 6}), set({4, 5, 6, 7, 8, 9})]
 
     assert months == should_be
 
+    with pytest.warns(MissingConstraintWarning):
+        constraints = [AtNightConstraint.twilight_astronomical()]
+        months_observable(constraints, obs, targets, time_range)
+
 
 def test_rescale_minmax():
     a = np.array([2])
     rescaled = np.zeros(5)
     rescaled[0] = (min_best_rescale(a, 1, 6))[0]
     rescaled[1] = (max_best_rescale(a, 1, 6))[0]
     rescaled[2] = (max_best_rescale(a, 0, 1))[0]
```

### Comparing `astroplan-0.8/astroplan/tests/test_moon.py` & `astroplan-0.9/astroplan/tests/test_moon.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/astroplan/tests/test_observer.py` & `astroplan-0.9/astroplan/tests/test_observer.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,33 +152,38 @@
     vega = SkyCoord(279.23473479*u.deg, 38.78368896*u.deg)
     mira = SkyCoord(34.83663376*u.deg, -2.97763767*u.deg)
     sirius = SkyCoord(101.28715533*u.deg, -16.71611586*u.deg)
     polaris = SkyCoord(37.95456067*u.degree, 89.26410897*u.degree)
     sc_list = [vega, mira, sirius, polaris]
 
     location = EarthLocation(10*u.deg, 45*u.deg, 0*u.m)
-    time = Time('1995-06-21 00:00:00')
+    time = Time('2022-06-21 00:00:00')
 
     obs = Observer(location=location)
-    rise_vector = obs.target_rise_time(time, sc_list)
+
+    with pytest.warns(TargetAlwaysUpWarning):
+        rise_vector = obs.target_rise_time(time, sc_list)
+        polaris_rise = obs.target_rise_time(time, polaris)
+
     vega_rise = obs.target_rise_time(time, vega)
     mira_rise = obs.target_rise_time(time, mira)
     sirius_rise = obs.target_rise_time(time, sirius)
-    polaris_rise = obs.target_rise_time(time, polaris)
 
     assert rise_vector[0] == vega_rise
     assert rise_vector[1] == mira_rise
     assert rise_vector[2] == sirius_rise
     assert rise_vector[3].value.mask and polaris_rise.value.mask
 
-    set_vector = obs.target_set_time(time, sc_list)
+    with pytest.warns(TargetAlwaysUpWarning):
+        set_vector = obs.target_set_time(time, sc_list)
+        polaris_set = obs.target_set_time(time, polaris)
+
     vega_set = obs.target_set_time(time, vega)
     mira_set = obs.target_set_time(time, mira)
     sirius_set = obs.target_set_time(time, sirius)
-    polaris_set = obs.target_set_time(time, polaris)
 
     assert set_vector[0] == vega_set
     assert set_vector[1] == mira_set
     assert set_vector[2] == sirius_set
     assert set_vector[3].value.mask and polaris_set.value.mask
 
     transit_vector = obs.target_meridian_transit_time(time, sc_list)
@@ -1340,7 +1345,45 @@
     mmt = Observer(location=loc, pressure=0*u.bar)
 
     # Compute equivalent time with astroplan
     astroplan_sunset = mmt.sun_set_time(mmto_sunset - 10*u.min,
                                         horizon=-0.8333*u.deg, which='next')
 
     assert abs(mmto_sunset - astroplan_sunset) < 1 * u.min
+
+
+def test_observer_lon_lat_el():
+    """Test that astropy.EarthLocation conversion to longitude,
+    latitude, and elevation works correctly.
+    """
+    obs = Observer.at_site('Subaru')
+    for attr in ['longitude', 'latitude', 'elevation']:
+        assert hasattr(obs, attr)
+
+
+def test_hash_observer():
+    """Test that Observer objects are hashable."""
+    obs1 = Observer.at_site('Subaru')
+    obs2 = Observer.at_site('Subaru')
+    assert hash(obs1) == hash(obs2)
+
+    obs3 = Observer.at_site('Keck', timezone='US/Hawaii')
+    assert hash(obs1) != hash(obs3)
+
+    obs4 = Observer.at_site('Keck', timezone='US/Hawaii')
+    assert hash(obs3) == hash(obs4)
+
+
+def test_eq_observer():
+    """Test that Observer objects are comparable."""
+    obs1 = Observer.at_site('Subaru')
+    obs2 = Observer.at_site('Subaru')
+    assert obs1 == obs2
+
+    obs3 = Observer.at_site('Keck')
+    assert obs1 != obs3
+
+    obs4 = Observer.at_site('Subaru', timezone='US/Hawaii')
+    assert obs1 != obs4
+
+    obs5 = Observer.at_site('Subaru', timezone='US/Hawaii')
+    assert obs4 == obs5
```

### Comparing `astroplan-0.8/astroplan/tests/test_periodic.py` & `astroplan-0.9/astroplan/tests/test_periodic.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/astroplan/tests/test_scheduling.py` & `astroplan-0.9/astroplan/tests/test_scheduling.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,24 +27,24 @@
 targets = [vega, polaris, rigel]
 default_time = Time('2016-02-06 03:00:00')
 only_at_night = [AtNightConstraint()]
 
 
 def test_observing_block():
     block = ObservingBlock(rigel, 1*u.minute, 0, configuration={'filter': 'b'})
-    assert(block.configuration['filter'] == 'b')
-    assert(block.target == rigel)
+    assert block.configuration['filter'] == 'b'
+    assert block.target == rigel
     times_per_exposure = [1*u.minute, 4*u.minute, 15*u.minute, 5*u.minute]
     numbers_of_exposures = [100, 4, 3, 12]
     readout_time = 0.5*u.minute
     for index in range(len(times_per_exposure)):
         block = ObservingBlock.from_exposures(vega, 0, times_per_exposure[index],
                                               numbers_of_exposures[index], readout_time)
-        assert(block.duration == numbers_of_exposures[index] *
-               (times_per_exposure[index] + readout_time))
+        assert (block.duration == numbers_of_exposures[index] *
+                (times_per_exposure[index] + readout_time))
 
 
 def test_slot():
     start_time = Time('2016-02-06 03:00:00')
     end_time = start_time + 24 * u.hour
     slot = Slot(start_time, end_time)
     slots = slot.split_slot(start_time, start_time+1*u.hour)
@@ -154,14 +154,38 @@
     assert schedule.slots[0].block.target == polaris
     assert schedule.slots[2].block.target == rigel
     # test that the scheduler does not error when called with a partially
     # filled schedule
     scheduler(blocks, schedule)
     scheduler(blocks, schedule)
 
+    # Check if the order of equal values is respected:
+    # 1. For equal priorities in blocks
+    # 2. For equal scores (boolean_constraint)
+    constraints = [AirmassConstraint(3, boolean_constraint=True)]
+    scheduler.constraints = constraints
+    # Any resolution coarser than this may result in gaps between the blocks
+    scheduler.time_resolution = 20*u.second
+    # This only happens with more than 16 items or so
+    targets_18 = [polaris, polaris, polaris, polaris, polaris, polaris,
+                  polaris, polaris, polaris, polaris, polaris, polaris,
+                  polaris, polaris, polaris, polaris, polaris, polaris]
+    blocks = [ObservingBlock(t, 4*u.minute, 5, name=i) for i, t in enumerate(targets_18)]
+
+    schedule = Schedule(start_time, end_time)
+    scheduler(blocks, schedule)
+
+    for i, t in enumerate(targets_18):
+        # Order of blocks
+        block = schedule.observing_blocks[i]
+        assert block.name == i
+        if i < len(targets_18) - 1:
+            # Same score for all timeslots, should be filled from the start without gaps
+            assert block.end_time.isclose(schedule.observing_blocks[i+1].start_time)
+
 
 def test_sequential_scheduler():
     constraints = [AirmassConstraint(2.5, boolean_constraint=False)]
     blocks = [ObservingBlock(t, 55 * u.minute, i) for i, t in enumerate(targets)]
     start_time = Time('2016-02-06 03:00:00')
     end_time = start_time + 18 * u.hour
     scheduler = SequentialScheduler(constraints=constraints, observer=apo,
```

### Comparing `astroplan-0.8/astroplan/tests/test_target.py` & `astroplan-0.9/astroplan/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/astroplan/tests/test_utils.py` & `astroplan-0.9/astroplan/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/astroplan/utils.py` & `astroplan-0.9/astroplan/utils.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/astroplan.egg-info/PKG-INFO` & `astroplan-0.9/astroplan.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,71 @@
 Metadata-Version: 2.1
 Name: astroplan
-Version: 0.8
+Version: 0.9
 Summary: Observation planning package for astronomers
 Home-page: https://github.com/astropy/astroplan
 Author: Astroplan developers
 Author-email: astropy-dev@googlegroups.com
 License: BSD
-Description: astroplan
-        =========
-        
-        Observation planning package for astronomers
-        
-        * Code: https://github.com/astropy/astroplan
-        * Docs: https://astroplan.readthedocs.io/
-        * License: BSD-3
-        
-        .. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
-            :target: http://www.astropy.org/
-        
-        .. image:: http://img.shields.io/pypi/v/astroplan.svg?text=version
-            :target: https://pypi.python.org/pypi/astroplan/
-            :alt: Latest release
-            
-        .. image:: http://img.shields.io/badge/arXiv-1709.03913-red.svg?style=flat
-            :target: https://arxiv.org/abs/1712.09631
-            :alt: arXiv paper
-        
-        Attribution
-        +++++++++++
-        
-        If you use astroplan in your work, please cite `Morris et al. 2018 <https://ui.adsabs.harvard.edu/abs/2018AJ....155..128M/abstract>`_: 
-        
-        .. code :: bibtex
-        
-          @ARTICLE{2018AJ....155..128M,
-                 author = {{Morris}, Brett M. and {Tollerud}, Erik and {Sip{\H{o}}cz}, Brigitta and {Deil}, Christoph and {Douglas}, Stephanie T. and {Berlanga Medina}, Jazmin and {Vyhmeister}, Karl and {Smith}, Toby R. and {Littlefair}, Stuart and {Price-Whelan}, Adrian M. and {Gee}, Wilfred T. and {Jeschke}, Eric},
-                  title = "{astroplan: An Open Source Observation Planning Package in Python}",
-                journal = {\aj},
-               keywords = {methods: numerical, methods: observational, Astrophysics - Instrumentation and Methods for Astrophysics},
-                   year = 2018,
-                  month = mar,
-                 volume = {155},
-                 number = {3},
-                    eid = {128},
-                  pages = {128},
-                    doi = {10.3847/1538-3881/aaa47e},
-          archivePrefix = {arXiv},
-                 eprint = {1712.09631},
-           primaryClass = {astro-ph.IM},
-                 adsurl = {https://ui.adsabs.harvard.edu/abs/2018AJ....155..128M},
-                adsnote = {Provided by the SAO/NASA Astrophysics Data System}
-          }
-        
-        
-        
-        
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: plotting
+License-File: LICENSE.rst
+
+astroplan
+=========
+
+Observation planning package for astronomers
+
+* Code: https://github.com/astropy/astroplan
+* Docs: https://astroplan.readthedocs.io/
+* License: BSD-3
+
+.. image:: https://readthedocs.org/projects/astroplan/badge/?version=latest
+    :target: https://astroplan.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: http://img.shields.io/badge/arXiv-1709.03913-red.svg?style=flat
+    :target: https://arxiv.org/abs/1712.09631
+    :alt: arXiv paper
+
+.. image:: https://github.com/astropy/astroplan/workflows/CI%20Tests/badge.svg
+    :target: https://github.com/astropy/astroplan/actions
+
+.. image:: http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat
+    :target: http://www.astropy.org/
+
+.. image:: http://img.shields.io/pypi/v/astroplan.svg?text=version
+    :target: https://pypi.python.org/pypi/astroplan/
+    :alt: Latest release
+
+Attribution
++++++++++++
+
+If you use astroplan in your work, please cite `Morris et al. 2018 <https://ui.adsabs.harvard.edu/abs/2018AJ....155..128M/abstract>`_: 
+
+.. code :: bibtex
+
+  @ARTICLE{2018AJ....155..128M,
+         author = {{Morris}, Brett M. and {Tollerud}, Erik and {Sip{\H{o}}cz}, Brigitta and {Deil}, Christoph and {Douglas}, Stephanie T. and {Berlanga Medina}, Jazmin and {Vyhmeister}, Karl and {Smith}, Toby R. and {Littlefair}, Stuart and {Price-Whelan}, Adrian M. and {Gee}, Wilfred T. and {Jeschke}, Eric},
+          title = "{astroplan: An Open Source Observation Planning Package in Python}",
+        journal = {\aj},
+       keywords = {methods: numerical, methods: observational, Astrophysics - Instrumentation and Methods for Astrophysics},
+           year = 2018,
+          month = mar,
+         volume = {155},
+         number = {3},
+            eid = {128},
+          pages = {128},
+            doi = {10.3847/1538-3881/aaa47e},
+  archivePrefix = {arXiv},
+         eprint = {1712.09631},
+   primaryClass = {astro-ph.IM},
+         adsurl = {https://ui.adsabs.harvard.edu/abs/2018AJ....155..128M},
+        adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+  }
+
+
+
```

### Comparing `astroplan-0.8/astroplan.egg-info/SOURCES.txt` & `astroplan-0.9/astroplan.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .gitignore
 .gitmodules
 .readthedocs.yml
 CHANGES.rst
-CITATION
+CITATION.bib
 LICENSE.rst
 LONG_DESCRIPTION.rst
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
```

### Comparing `astroplan-0.8/docs/Makefile` & `astroplan-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/docs/conf.py` & `astroplan-0.9/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 # Note that not all possible configuration values are present in this file.
 #
 # All configuration values have a default. Some values are defined in
 # the global Astropy configuration which is loaded here before anything else.
 # See astropy.sphinx.conf for which values are set there.
 
 from configparser import ConfigParser
-import os
+from astroplan import __version__
 import sys
 import datetime
 
 try:
-    from sphinx_astropy.conf.v1 import *  # noqa
+    from sphinx_astropy.conf.v2 import *  # noqa
 except ImportError:
     print('ERROR: the documentation requires the sphinx-astropy package to '
           'be installed')
     sys.exit(1)
 
 # Get configuration information from setup.cfg
 conf = ConfigParser()
@@ -30,15 +30,15 @@
 
 
 # -- General configuration ----------------------------------------------------
 # By default, highlight as Python 3.
 highlight_language = 'python3'
 
 # If your documentation needs a minimal Sphinx version, state it here.
-needs_sphinx = '1.7'
+# needs_sphinx = '1.7'
 
 # Extend astropy intersphinx_mapping with packages we use here
 intersphinx_mapping['astroquery'] = ('http://astroquery.readthedocs.io/en/latest/', None)
 
 # Exclude astropy intersphinx_mapping for unused packages
 del intersphinx_mapping['h5py']  # noqa
 
@@ -81,20 +81,14 @@
 # A NOTE ON HTML THEMES
 # The global astropy configuration uses a custom theme, 'bootstrap-astropy',
 # which is installed along with astropy. A different theme can be used or
 # the options for this theme can be modified by overriding some of the
 # variables set in the global configuration. The variables set in the
 # global configuration are listed below, commented out.
 
-html_theme_options = {
-    'logotext1': 'astro',  # white,  semi-bold
-    'logotext2': 'plan',  # orange, light
-    'logotext3': ':docs'   # white,  light
-    }
-
 # Add any paths that contain custom themes here, relative to this directory.
 # To use a different custom theme, add the directory containing the theme.
 #html_theme_path = []
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes. To override the custom theme, set this to the
 # name of a builtin theme or the name of a custom theme in html_theme_path.
@@ -155,15 +149,18 @@
 # Currently this is not needed because of the content of the tests, but we leave
 # it here in case it's needed again in the future.  BUT beware of:
 # https://github.com/astropy/astroplan/issues/96
 #from astroplan.utils import _mock_remote_data
 #_mock_remote_data()
 
 # Add additional Sphinx extensions:
-extensions += ['matplotlib.sphinxext.plot_directive']
+extensions += [
+    'matplotlib.sphinxext.plot_directive',
+    'sphinx.ext.graphviz'
+]
 
 # -- Resolving issue number to links in changelog -----------------------------
 github_issues_url = 'https://github.com/{0}/issues/'.format(setup_cfg['github_p\
 roject'])
 
 # -- Options for linkcheck output -------------------------------------------
 linkcheck_retry = 5
@@ -172,14 +169,39 @@
 ]
 linkcheck_timeout = 180
 linkcheck_anchors = False
 
 # -- Turn on nitpicky mode for sphinx (to warn about references not found) ----
 nitpicky = True
 
+release = __version__
+dev = "dev" in release
+
+html_copy_source = False
+
+html_theme_options.update(  # noqa: F405
+    {
+        "github_url": "https://github.com/astropy/astroplan",
+        "external_links": [
+            {"name": "astropy docs", "url": "https://docs.astropy.org/en/stable/"},
+        ],
+        "use_edit_page_button": True,
+    }
+)
+
+html_context = {
+    "default_mode": "light",
+    "to_be_indexed": ["stable", "latest"],
+    "is_development": dev,
+    "github_user": "astropy",
+    "github_repo": "astroplan",
+    "github_version": "main",
+    "doc_path": "docs",
+}
+
 #
 # Some warnings are impossible to suppress, and you can list specific references
 # that should be ignored in a nitpick-exceptions file which should be inside
 # the docs/ directory. The format of the file should be:
 #
 # <type> <class>
 #
```

### Comparing `astroplan-0.8/docs/faq/contribute.rst` & `astroplan-0.9/docs/faq/contribute.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/docs/faq/iers.rst` & `astroplan-0.9/docs/faq/iers.rst`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     # allowing times "outside of the table"
     DUT1_a, success_a = time_range.get_delta_ut1_utc(return_status=True,
                                                      iers_table=iers_a)
     DUT1_b, success_b = time_range.get_delta_ut1_utc(return_status=True,
                                                      iers_table=iers_b)
 
     # Compare input times to the times available in the table. For details, see
-    # https://github.com/astropy/astropy/blob/master/astropy/utils/iers/iers.py#L80
+    # https://docs.astropy.org/en/stable/utils/iers.html
     measurements_from_b = (success_b == FROM_IERS_B)
 
     # Make a plot of the time difference
     fig, ax = plt.subplots(figsize=(10,8))
     ax.axhline(0, color='gray', ls='--', lw=2)
 
     ax.plot_date(time_range.plot_date,
```

### Comparing `astroplan-0.8/docs/faq/precision.rst` & `astroplan-0.9/docs/faq/precision.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/docs/faq/terminology.rst` & `astroplan-0.9/docs/faq/terminology.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/docs/getting_started.rst` & `astroplan-0.9/docs/getting_started.rst`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ***************
 Getting Started
 ***************
 
 General Guidelines
 ==================
 
-`astroplan` is based on `Astropy <https://astropy.org>`__ and was built around the creation of Python
+`astroplan` is based on `astropy <https://astropy.org>`__ and was built around the creation of Python
 objects that contain all the information needed to perform certain tasks.  You,
 the user, will create and manipulate these objects to plan your observation. For
 instance, an `~astroplan.Target` object contains information associated with
 targets, such as right ascension, declination, etc.
 
 Objects representing celestial bodies like stars (which, if we ignore proper
 motion, are fixed on the celestial sphere) are created (or "instantiated") via
@@ -53,27 +53,23 @@
                    location=location,
                    pressure=0.615 * u.bar,
                    relative_humidity=0.11,
                    temperature=0 * u.deg_C,
                    timezone=timezone('US/Hawaii'),
                    description="Subaru Telescope on Maunakea, Hawaii")
 
-`astroplan` makes heavy use of certain `Astropy <https://astropy.org>`__ machinery, including the
+`astroplan` makes heavy use of certain `astropy <https://astropy.org>`__ machinery, including the
 `~astropy.coordinates` objects and transformations and
 `~astropy.units`. Most importantly for basic use of `astroplan` is the
 representation of dates/times as `~astropy.time.Time` objects (note that
 these are in the UTC timezone by default)::
 
     from astropy.time import Time
     time = Time(['2015-06-16 06:00:00'])
 
-Since `astroplan` objects are Python objects, manipulating them or accessing
-attributes follows Python syntax and conventions.  See Python documentation on
-`objects <https://docs.python.org/2/tutorial/classes.html#instance-objects>`_
-for more information.
 
 Doing More
 ==========
 
 Now that you know the basics of working with `astroplan`, check out our
 :ref:`tutorials` page for high-level examples of using `astroplan`, as well as
 the :ref:`api` section for more exhaustive documentation and lower-level usage
```

### Comparing `astroplan-0.8/docs/installation.rst` & `astroplan-0.9/docs/installation.rst`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,17 @@
 Installation
 ************
 
 Requirements
 ============
 
 **astroplan** works on Linux, Mac OS X and Windows.
-It requires Python 2.7 or 3.5+ (2.6 and 3.2 or earlier are not
-supported, 3.3 and 3.4 may work) as well as the following packages:
-
-* `Numpy`_ (1.10 or later)
-* `Astropy <https://astropy.org>`__ (v1.3 or later)
-* `pytz`_
-
-Optional packages:
-
-* `Matplotlib`_
-* `astroquery`_
-
-For testing:
-
-* `pytest-astropy`_
+It requires Python 3.7+ as well as numpy, astropy, pytz, and six.
+Additional features are available when you install `Matplotlib`_
+and `astroquery`_.
 
 First-time Python users may want to consider an all-in-one Python installation
 package, such as the `Anaconda Python Distribution
 <http://continuum.io/downloads>`_ which provides all of the above dependencies.
 
 Installation
 ============
@@ -45,33 +33,32 @@
 cloning the git repository::
 
     git clone https://github.com/astropy/astroplan
 
 ...then installing the package with::
 
     cd astroplan
-    python setup.py install
+    pip install .
 
 Testing
 =======
 
 If you want to check that all the tests are running correctly with your Python
-configuration, start up python, and type::
+configuration, run the following from the command line::
 
-    import astroplan
-    astroplan.test()
+    tox -e test
 
 If there are no errors, you are good to go!
 
 .. note::
 	If you want to run the tests that access the internet, you'll need to
-	replace the last line above with ``astroplan.test(remote_data=True)`` and
+	replace the last line above with ``tox -e test -- --remote-data`` and
 	have an active connection to the internet.  Also, if you want the tests
 	that check plotting to work, you need `Matplotlib`_ and `pytest-mpl`_.
 
 More
 ====
 
-astroplan follows `Astropy <https://astropy.org>`__'s guidelines for affiliated packages--installation
-and testing for the two are quite similar! Please see Astropy's
+astroplan follows `astropy <https://astropy.org>`__'s guidelines for affiliated packages--installation
+and testing for the two are quite similar! Please see astropy's
 `installation page <http://astropy.readthedocs.io/en/latest/install.html>`_
 for more information.
```

### Comparing `astroplan-0.8/docs/make.bat` & `astroplan-0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/docs/tutorials/constraints.rst` & `astroplan-0.9/docs/tutorials/constraints.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     # Are targets *ever* observable in the time range?
     ever_observable = is_observable(constraints, subaru, targets, time_range=time_range)
 
     # Are targets *always* observable in the time range?
     always_observable = is_always_observable(constraints, subaru, targets, time_range=time_range)
 
     # During what months are the targets ever observable?
-    best_months = months_observable(constraints, subaru, targets)
+    best_months = months_observable(constraints, subaru, targets, time_range)
 
 The `~astroplan.is_observable` and `~astroplan.is_always_observable` functions
 will return boolean arrays which tell you whether or not each target is
 observable given your constraints. Let's print these results in tabular form:
 
     >>> from astropy.table import Table
     >>> import numpy as np
@@ -180,17 +180,17 @@
     cmap = cm.Set1             # Cycle through this colormap
 
     for i, target in enumerate(targets):
         ax = plot_sky(target, subaru, time_grid,
                       style_kwargs=dict(color=cmap(float(i)/len(targets)),
                                         label=target.name))
 
-    legend = ax.legend(loc='lower center')
-    legend.get_frame().set_facecolor('w')
-    plt.show()
+        legend = ax.legend(loc='lower center')
+        legend.get_frame().set_facecolor('w')
+        plt.show()
 
 We can see that Vega is in the sweet spot in altitude and azimuth for this
 time range and is always observable. Albireo is not always observable given
 these criteria because it rises above 80 degrees altitude. Polaris hardly moves
 and is therefore always observable, and Algol starts out observable but sets
 below the lower altitude limit, and then the airmass limit. Rigel and Regulus
 never rise above those limits within the time range.
```

### Comparing `astroplan-0.8/docs/tutorials/index.rst` & `astroplan-0.9/docs/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/docs/tutorials/periodic.rst` & `astroplan-0.9/docs/tutorials/periodic.rst`

 * *Files 4% similar despite different names*

```diff
@@ -96,32 +96,33 @@
 .. _periodic-transit_times_via_astroquery:
 
 Transit times via astroquery
 ============================
 
 The development version of `astroquery`_ allows users to query for properties of
 known exoplanets with three different services:
-`~astroquery.exoplanet_orbit_database`, `~astroquery.nasa_exoplanet_archive`,
+`~astroquery.ipac.nexsci.nasa_exoplanet_archive`, `~astroquery.exoplanet_orbit_database`,
 and `~astroquery.open_exoplanet_catalogue`. In the example below, we will query
 for the properties of the transiting exoplanet TRAPPIST-1 b with astroquery, and
 calculate the times of the next three transits with
 `~astroplan.EclipsingSystem`.
 
 .. code-block:: python
 
     >>> # NASA Exoplanet Archive for planet properties
     >>> import astropy.units as u
     >>> from astropy.time import Time
-    >>> from astroquery.nasa_exoplanet_archive import NasaExoplanetArchive
-    >>> planet_properties = NasaExoplanetArchive.query_planet('TRAPPIST-1 b', all_columns=True)
+    >>> from astroquery.ipac.nexsci.nasa_exoplanet_archive import NasaExoplanetArchive
+    >>> planet_properties = NasaExoplanetArchive.query_object('TRAPPIST-1 b', select='*', table='pscomppars')
+
 
     >>> # get relevant planet properties
     >>> epoch = Time(planet_properties['pl_tranmid'], format='jd')
     >>> period = planet_properties['pl_orbper']
-    >>> transit_duration = planet_properties['pl_trandur'] * u.day
+    >>> transit_duration = planet_properties['pl_trandur']
 
     >>> # Create an EclipsingSystem object for HD 209458
     >>> from astroplan import EclipsingSystem
     >>> trappist1b = EclipsingSystem(primary_eclipse_time=epoch, orbital_period=period,
     ...                              duration=transit_duration)
 
     >>> # Calculate next three mid-transit times which occur after ``obs_time``
```

### Comparing `astroplan-0.8/docs/tutorials/plots.rst` & `astroplan-0.9/docs/tutorials/plots.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1070,15 +1070,15 @@
     >>> plot_sky(altair, observer, observe_time, my_ax)
 
 We can also create a `~matplotlib.axes.Axes` object entirely outside of
 `~astroplan.plots.plot_sky`, then pass it in:
 
 .. code-block:: python
 
-    >>> my_ax = plt.gca(projection='polar')
+    >>> my_ax = plt.gcf().add_subplot(projection='polar')
     >>> plot_sky(polaris, observer, observe_time, my_ax)
 
 Passing in named `matplotlib.axes.Axes` objects comes in handy when you want to
 make multiple plots:
 
 .. code-block:: python
```

### Comparing `astroplan-0.8/docs/tutorials/scheduling.rst` & `astroplan-0.9/docs/tutorials/scheduling.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/docs/tutorials/speed.rst` & `astroplan-0.9/docs/tutorials/speed.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/docs/tutorials/summer_triangle.rst` & `astroplan-0.9/docs/tutorials/summer_triangle.rst`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/setup.cfg` & `astroplan-0.9/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -20,26 +20,27 @@
 	numpy>=1.17
 	astropy>=4
 	pytz
 	six
 
 [options.extras_require]
 all = 
-	matplotlib>=1.4,<3.3
+	matplotlib>=1.4
 	astroquery
 test = 
 	pytest-astropy
+	pytest-mpl
 docs = 
-	sphinx-astropy
-	sphinx_rtd_theme
-	matplotlib>=1.4,<3.3
+	sphinx-astropy[confv2]
+	sphinx-rtd-theme
+	matplotlib>=1.4
 	astroquery
 plotting = 
 	astroquery
-	matplotlib>=1.4,<3.3
+	matplotlib>=1.4
 
 [options.package_data]
 astroplan = data/*
 
 [tool:pytest]
 testpaths = "astroplan" "docs"
 astropy_header = true
```

### Comparing `astroplan-0.8/setup.py` & `astroplan-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `astroplan-0.8/tox.ini` & `astroplan-0.9/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     NIGHTLY = https://pypi.anaconda.org/scipy-wheels-nightly/simple
 
 [testenv]
 # Suppress display of matplotlib plots generated during docs build
 setenv = MPLBACKEND=agg
 
 # Pass through the following environment variables which may be needed for the CI
-passenv = HOME WINDIR LC_ALL LC_CTYPE CC CI TRAVIS
+passenv = HOME, WINDIR, LC_ALL, LC_CTYPE, CC, CI, TRAVIS
 
 # Run the tests in a temporary directory to make sure that we don't import
 # this package from the source tree
 changedir = .tmp/{envname}
 
 # tox environments are constructed with so-called 'factors' (or terms)
 # separated by hyphens, e.g. test-devdeps-cov. Lines below starting with factor:
@@ -58,15 +58,15 @@
 
     astropy30: astropy==3.0.*
     astropy40: astropy==4.0.*
     astropylts: astropy==4.0.*
     astropy41: astropy==4.1.*
     astropy42: astropy==4.2.*
 
-    devdeps: :NIGHTLY:numpy
+    devdeps: numpy>=0.0.dev0
     devdeps: git+https://github.com/astropy/astropy.git#egg=astropy
 
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
     test
     alldeps: all
```

