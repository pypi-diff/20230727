# Comparing `tmp/mlcalcdriver-1.4.1.tar.gz` & `tmp/mlcalcdriver-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcalcdriver-1.4.1.tar", last modified: Fri Jun 16 19:08:54 2023, max compression
+gzip compressed data, was "mlcalcdriver-1.4.2.tar", last modified: Thu Jul 27 19:23:13 2023, max compression
```

## Comparing `mlcalcdriver-1.4.1.tar` & `mlcalcdriver-1.4.2.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/.github/
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/.github/workflows/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1257 2023-06-16 19:07:06.000000 mlcalcdriver-1.4.1/.github/workflows/python-package.yml
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1223 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/.gitignore
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      658 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/.pep8speaks.yml
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       48 2022-01-13 18:56:41.000000 mlcalcdriver-1.4.1/.pyup.yml
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    35149 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/LICENSE
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2439 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/PKG-INFO
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2015 2023-06-16 19:07:06.000000 mlcalcdriver-1.4.1/README.md
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      230 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/.buildinfo
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/.nojekyll
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      688 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/Makefile
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4937 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/index.html
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/base/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    42890 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/base/job.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    97977 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/base/posinp.html
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/ase_calculators/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    13223 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/ase_calculators/asespkcalculator.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    12601 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/calculator.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    25087 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/ensemble.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    38307 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/schnetpack.html
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/interfaces/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     9195 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/interfaces/ase_interface.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10219 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/interfaces/schnetpack_interface.html
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/workflows/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    24450 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/workflows/geopt.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    40427 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/workflows/phonon.html
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_sources/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      170 2021-12-10 20:14:37.000000 mlcalcdriver-1.4.1/docs/_sources/ase_interface.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      109 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.1/docs/_sources/asespkcalc.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      136 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/base.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      120 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/calculator.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      215 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.1/docs/_sources/calculators.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       93 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.1/docs/_sources/ensemble.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/geopt.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       54 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/globals.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      438 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/index.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      517 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_sources/interfaces.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       61 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/job.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       87 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/phonon.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/posinp.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      140 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/schnet_interface.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       95 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/schnetcalc.rst.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      159 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.1/docs/_sources/workflows.rst.txt
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_static/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    14692 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/basic.css
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_static/css/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     3275 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/css/badge_only.css
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    87624 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    67312 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    86288 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    66444 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   165742 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   444379 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   165548 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    98024 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    77160 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   323344 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold-italic.woff
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   193308 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   309728 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold.woff
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   184912 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold.woff2
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   328412 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal-italic.woff
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   195704 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   309192 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal.woff
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   182708 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal.woff2
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   129674 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/css/theme.css
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     9758 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/doctools.js
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      355 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/documentation_options.js
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      286 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.1/docs/_static/file.png
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   287630 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/_static/jquery-3.5.1.js
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    89476 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/jquery.js
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/_static/js/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      934 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/_static/js/badge_only.js
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4370 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/_static/js/html5shiv-printshiv.min.js
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2734 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/_static/js/html5shiv.min.js
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5023 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/js/theme.js
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10854 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/language_data.js
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/_static/minus.png
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/_static/plus.png
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4846 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/pygments.css
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    16793 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/searchtools.js
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    68420 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.1/docs/_static/underscore-1.13.1.js
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    19530 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/_static/underscore.js
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     7169 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/ase_interface.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10423 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/asespkcalc.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5341 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/base.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    11101 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/calculator.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     6388 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/calculators.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    18549 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/ensemble.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    24446 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/genindex.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    14232 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/geopt.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    16804 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/globals.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    12331 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/index.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5838 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/interfaces.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    14803 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/job.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1441 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/objects.inv
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    16522 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/phonon.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    45912 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/posinp.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     7185 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/py-modindex.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     9024 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/schnet_interface.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    11395 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/schnetcalc.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4034 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/search.html
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    15533 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/searchindex.js
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/docs/source/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      170 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.1/docs/source/ase_interface.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      109 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.1/docs/source/asespkcalc.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      136 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/source/base.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      120 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/source/calculator.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      215 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/source/calculators.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2438 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/source/conf.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       93 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.1/docs/source/ensemble.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/source/geopt.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       54 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/source/globals.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      438 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.1/docs/source/index.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      517 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/source/interfaces.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       61 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/docs/source/job.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       87 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/docs/source/phonon.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/docs/source/posinp.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      140 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/docs/source/schnet_interface.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       95 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/docs/source/schnetcalc.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      159 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/docs/source/workflows.rst
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5206 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/docs/workflows.html
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       82 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/mlcalcdriver/__init__.py
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver/base/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      143 2022-01-21 22:08:52.000000 mlcalcdriver-1.4.1/mlcalcdriver/base/__init__.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10343 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/mlcalcdriver/base/job.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    26319 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/mlcalcdriver/base/posinp.py
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      623 2022-04-26 18:24:40.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/__init__.py
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/ase_calculators/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       87 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/ase_calculators/__init__.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2448 2022-03-18 20:53:07.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/ase_calculators/asespkcalculator.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2479 2022-01-21 22:12:51.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/calculator.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4414 2022-01-21 22:13:25.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/ensemble.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     8763 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/schnetpack.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     9012 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/schnetpack_patch.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1565 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/mlcalcdriver/calculators/utils.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2926 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/mlcalcdriver/globals.py
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver/interfaces/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      179 2022-04-26 18:24:40.000000 mlcalcdriver-1.4.1/mlcalcdriver/interfaces/__init__.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      966 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/mlcalcdriver/interfaces/ase_interface.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     7924 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.1/mlcalcdriver/interfaces/atoms_to_patches.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1426 2021-12-10 20:14:39.000000 mlcalcdriver-1.4.1/mlcalcdriver/interfaces/schnetpack_interface.py
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver/workflows/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       87 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/mlcalcdriver/workflows/__init__.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     6073 2022-01-21 22:13:53.000000 mlcalcdriver-1.4.1/mlcalcdriver/workflows/geopt.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10422 2023-02-23 19:49:26.000000 mlcalcdriver-1.4.1/mlcalcdriver/workflows/phonon.py
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/mlcalcdriver.egg-info/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2439 2023-06-16 19:08:53.000000 mlcalcdriver-1.4.1/mlcalcdriver.egg-info/PKG-INFO
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5169 2023-06-16 19:08:53.000000 mlcalcdriver-1.4.1/mlcalcdriver.egg-info/SOURCES.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)        1 2023-06-16 19:08:53.000000 mlcalcdriver-1.4.1/mlcalcdriver.egg-info/dependency_links.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       61 2023-06-16 19:08:53.000000 mlcalcdriver-1.4.1/mlcalcdriver.egg-info/requires.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       13 2023-06-16 19:08:53.000000 mlcalcdriver-1.4.1/mlcalcdriver.egg-info/top_level.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       47 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/pytest.ini
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      271 2023-06-16 19:07:06.000000 mlcalcdriver-1.4.1/requirements_dev.txt
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       38 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/setup.cfg
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      745 2023-06-16 19:08:51.000000 mlcalcdriver-1.4.1/setup.py
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/tests/
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/tests/models/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)  1857323 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/models/H2O_forces_model
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)  1856737 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/models/H2O_model
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)  1856737 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/models/ani1_N2_model
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)  1856737 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/models/myN2_model
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    85275 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/models/wacsf_model
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/tests/posinp_angles/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       96 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_angles/gra2.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      162 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/posinp_angles/gra4_red.xyz
-drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-06-16 19:08:54.000000 mlcalcdriver-1.4.1/tests/posinp_files/
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      143 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/posinp_files/H2O_atomic.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       82 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_files/H2O_unrelaxed.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      148 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_files/H2Orelaxed.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       58 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_files/N2.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       60 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_files/N2_unrelaxed.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      191 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/posinp_files/additional_atom.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      334 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/posinp_files/free.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      188 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/posinp_files/free_reduced.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      154 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.1/tests/posinp_files/missing_atom.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       83 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_files/perio1.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       85 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.1/tests/posinp_files/perio2.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      193 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.1/tests/posinp_files/periodic.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       82 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.1/tests/posinp_files/reduced.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      192 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.1/tests/posinp_files/surface.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      193 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.1/tests/posinp_files/surface2.xyz
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1657 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.1/tests/test_angles.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      990 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.1/tests/test_calculators.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2182 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.1/tests/test_geopt.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      796 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.1/tests/test_interface.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1552 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.1/tests/test_job.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2274 2023-02-23 19:49:26.000000 mlcalcdriver-1.4.1/tests/test_phonon.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     8277 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.1/tests/test_posinp.py
--rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2668 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.1/tests/test_schnetpack.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:13.000000 mlcalcdriver-1.4.2/
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:07.000000 mlcalcdriver-1.4.2/.github/
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:07.000000 mlcalcdriver-1.4.2/.github/workflows/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1257 2023-06-16 19:07:06.000000 mlcalcdriver-1.4.2/.github/workflows/python-package.yml
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1223 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/.gitignore
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      658 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/.pep8speaks.yml
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       48 2022-01-13 18:56:41.000000 mlcalcdriver-1.4.2/.pyup.yml
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    35149 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/LICENSE
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2820 2023-07-27 19:23:13.000000 mlcalcdriver-1.4.2/PKG-INFO
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2015 2023-06-16 19:07:06.000000 mlcalcdriver-1.4.2/README.md
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:08.000000 mlcalcdriver-1.4.2/docs/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      230 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/.buildinfo
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/.nojekyll
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      688 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/Makefile
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:08.000000 mlcalcdriver-1.4.2/docs/_modules/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4937 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/_modules/index.html
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:07.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:08.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/base/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    42890 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/base/job.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    97977 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/base/posinp.html
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:08.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/calculators/
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:08.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/calculators/ase_calculators/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    13223 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/calculators/ase_calculators/asespkcalculator.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    12601 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/calculators/calculator.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    25087 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/calculators/ensemble.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    38307 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/calculators/schnetpack.html
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:08.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/interfaces/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     9195 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/interfaces/ase_interface.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10219 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/interfaces/schnetpack_interface.html
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:09.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/workflows/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    24450 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/workflows/geopt.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    40427 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/workflows/phonon.html
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:09.000000 mlcalcdriver-1.4.2/docs/_sources/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      170 2021-12-10 20:14:37.000000 mlcalcdriver-1.4.2/docs/_sources/ase_interface.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      109 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.2/docs/_sources/asespkcalc.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      136 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/_sources/base.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      120 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/_sources/calculator.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      215 2023-02-23 19:49:10.000000 mlcalcdriver-1.4.2/docs/_sources/calculators.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       93 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.2/docs/_sources/ensemble.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/_sources/geopt.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       54 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/_sources/globals.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      438 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/_sources/index.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      517 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/_sources/interfaces.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       61 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/_sources/job.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       87 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/_sources/phonon.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/_sources/posinp.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      140 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/_sources/schnet_interface.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       95 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/_sources/schnetcalc.rst.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      159 2021-12-10 18:33:32.000000 mlcalcdriver-1.4.2/docs/_sources/workflows.rst.txt
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:10.000000 mlcalcdriver-1.4.2/docs/_static/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    14692 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/_static/basic.css
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:10.000000 mlcalcdriver-1.4.2/docs/_static/css/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     3275 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/_static/css/badge_only.css
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:11.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    87624 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    67312 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    86288 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    66444 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   165742 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   444379 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   165548 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    98024 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    77160 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   323344 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   193308 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   309728 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-bold.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   184912 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-bold.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   328412 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   195704 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   309192 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-normal.woff
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   182708 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-normal.woff2
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   129674 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/_static/css/theme.css
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     9758 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/_static/doctools.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      355 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/_static/documentation_options.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      286 2021-12-10 18:33:33.000000 mlcalcdriver-1.4.2/docs/_static/file.png
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)   287630 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.2/docs/_static/jquery-3.5.1.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    89476 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/_static/jquery.js
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:11.000000 mlcalcdriver-1.4.2/docs/_static/js/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      934 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.2/docs/_static/js/badge_only.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4370 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.2/docs/_static/js/html5shiv-printshiv.min.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2734 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.2/docs/_static/js/html5shiv.min.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5023 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/_static/js/theme.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10854 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/_static/language_data.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.2/docs/_static/minus.png
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.2/docs/_static/plus.png
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4846 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/_static/pygments.css
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    16793 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/_static/searchtools.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    68420 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.2/docs/_static/underscore-1.13.1.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    19530 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/_static/underscore.js
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     7169 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/ase_interface.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10423 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/asespkcalc.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5341 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/base.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    11101 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/calculator.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     6388 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/calculators.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    18549 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/ensemble.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    24446 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/genindex.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    14232 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/geopt.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    16804 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/globals.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    12331 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/index.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5838 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/interfaces.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    14803 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/job.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1441 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/objects.inv
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    16522 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/phonon.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    45912 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/posinp.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     7185 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/py-modindex.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     9024 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/schnet_interface.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    11395 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/schnetcalc.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4034 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/search.html
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    15533 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/searchindex.js
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:11.000000 mlcalcdriver-1.4.2/docs/source/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      170 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.2/docs/source/ase_interface.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      109 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.2/docs/source/asespkcalc.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      136 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.2/docs/source/base.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      120 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.2/docs/source/calculator.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      215 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/source/calculators.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2438 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/source/conf.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       93 2021-12-10 20:14:38.000000 mlcalcdriver-1.4.2/docs/source/ensemble.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.2/docs/source/geopt.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       54 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.2/docs/source/globals.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      438 2021-12-10 18:33:34.000000 mlcalcdriver-1.4.2/docs/source/index.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      517 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/source/interfaces.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       61 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/docs/source/job.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       87 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/docs/source/phonon.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       90 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/docs/source/posinp.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      140 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/docs/source/schnet_interface.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       95 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/docs/source/schnetcalc.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      159 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/docs/source/workflows.rst
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5206 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/docs/workflows.html
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:11.000000 mlcalcdriver-1.4.2/mlcalcdriver/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       82 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/mlcalcdriver/__init__.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:12.000000 mlcalcdriver-1.4.2/mlcalcdriver/base/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      143 2022-01-21 22:08:52.000000 mlcalcdriver-1.4.2/mlcalcdriver/base/__init__.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    10343 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.2/mlcalcdriver/base/job.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    27481 2023-07-21 18:30:58.000000 mlcalcdriver-1.4.2/mlcalcdriver/base/posinp.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:12.000000 mlcalcdriver-1.4.2/mlcalcdriver/calculators/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      623 2022-04-26 18:24:40.000000 mlcalcdriver-1.4.2/mlcalcdriver/calculators/__init__.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:12.000000 mlcalcdriver-1.4.2/mlcalcdriver/calculators/ase_calculators/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       87 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/mlcalcdriver/calculators/ase_calculators/__init__.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2448 2022-03-18 20:53:07.000000 mlcalcdriver-1.4.2/mlcalcdriver/calculators/ase_calculators/asespkcalculator.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2679 2023-07-21 18:30:58.000000 mlcalcdriver-1.4.2/mlcalcdriver/calculators/calculator.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     4414 2022-01-21 22:13:25.000000 mlcalcdriver-1.4.2/mlcalcdriver/calculators/ensemble.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     8763 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/mlcalcdriver/calculators/schnetpack.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     9012 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/mlcalcdriver/calculators/schnetpack_patch.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1565 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/mlcalcdriver/calculators/utils.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2980 2023-07-21 18:30:58.000000 mlcalcdriver-1.4.2/mlcalcdriver/globals.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:12.000000 mlcalcdriver-1.4.2/mlcalcdriver/interfaces/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      179 2022-04-26 18:24:40.000000 mlcalcdriver-1.4.2/mlcalcdriver/interfaces/__init__.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      966 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.2/mlcalcdriver/interfaces/ase_interface.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     7924 2023-02-23 19:49:11.000000 mlcalcdriver-1.4.2/mlcalcdriver/interfaces/atoms_to_patches.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1426 2021-12-10 20:14:39.000000 mlcalcdriver-1.4.2/mlcalcdriver/interfaces/schnetpack_interface.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:12.000000 mlcalcdriver-1.4.2/mlcalcdriver/workflows/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       87 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/mlcalcdriver/workflows/__init__.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     6073 2022-01-21 22:13:53.000000 mlcalcdriver-1.4.2/mlcalcdriver/workflows/geopt.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    12034 2023-07-27 19:22:42.000000 mlcalcdriver-1.4.2/mlcalcdriver/workflows/phonon.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:12.000000 mlcalcdriver-1.4.2/mlcalcdriver.egg-info/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2820 2023-07-27 19:23:07.000000 mlcalcdriver-1.4.2/mlcalcdriver.egg-info/PKG-INFO
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     5169 2023-07-27 19:23:07.000000 mlcalcdriver-1.4.2/mlcalcdriver.egg-info/SOURCES.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)        1 2023-07-27 19:23:07.000000 mlcalcdriver-1.4.2/mlcalcdriver.egg-info/dependency_links.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       61 2023-07-27 19:23:07.000000 mlcalcdriver-1.4.2/mlcalcdriver.egg-info/requires.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       13 2023-07-27 19:23:07.000000 mlcalcdriver-1.4.2/mlcalcdriver.egg-info/top_level.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       47 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/pytest.ini
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      331 2023-07-27 19:22:42.000000 mlcalcdriver-1.4.2/requirements_dev.txt
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       38 2023-07-27 19:23:13.000000 mlcalcdriver-1.4.2/setup.cfg
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      745 2023-07-27 19:22:58.000000 mlcalcdriver-1.4.2/setup.py
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:12.000000 mlcalcdriver-1.4.2/tests/
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:13.000000 mlcalcdriver-1.4.2/tests/models/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)  1857323 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/tests/models/H2O_forces_model
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)  1856737 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/tests/models/H2O_model
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)  1856737 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/tests/models/ani1_N2_model
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)  1856737 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/tests/models/myN2_model
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)    85275 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/tests/models/wacsf_model
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:13.000000 mlcalcdriver-1.4.2/tests/posinp_angles/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       96 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.2/tests/posinp_angles/gra2.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      162 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/tests/posinp_angles/gra4_red.xyz
+drwxr-s---   0 olimt    (3040358) rrg-cotemich-ac (6004866)        0 2023-07-27 19:23:13.000000 mlcalcdriver-1.4.2/tests/posinp_files/
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      143 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/tests/posinp_files/H2O_atomic.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       82 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.2/tests/posinp_files/H2O_unrelaxed.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      148 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.2/tests/posinp_files/H2Orelaxed.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       58 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.2/tests/posinp_files/N2.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       60 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.2/tests/posinp_files/N2_unrelaxed.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      191 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/tests/posinp_files/additional_atom.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      334 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/tests/posinp_files/free.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      188 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/tests/posinp_files/free_reduced.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      154 2021-12-10 18:33:35.000000 mlcalcdriver-1.4.2/tests/posinp_files/missing_atom.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       83 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.2/tests/posinp_files/perio1.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       85 2022-01-21 23:40:53.000000 mlcalcdriver-1.4.2/tests/posinp_files/perio2.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      193 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.2/tests/posinp_files/periodic.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)       82 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.2/tests/posinp_files/reduced.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      192 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.2/tests/posinp_files/surface.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      193 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.2/tests/posinp_files/surface2.xyz
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1657 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.2/tests/test_angles.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      990 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.2/tests/test_calculators.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2182 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.2/tests/test_geopt.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)      796 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.2/tests/test_interface.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     1552 2021-12-10 18:33:36.000000 mlcalcdriver-1.4.2/tests/test_job.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2626 2023-07-21 18:30:58.000000 mlcalcdriver-1.4.2/tests/test_phonon.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     8277 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.2/tests/test_posinp.py
+-rw-r-----   0 olimt    (3040358) rrg-cotemich-ac (6004866)     2668 2022-01-21 23:40:54.000000 mlcalcdriver-1.4.2/tests/test_schnetpack.py
```

### Comparing `mlcalcdriver-1.4.1/.github/workflows/python-package.yml` & `mlcalcdriver-1.4.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/.gitignore` & `mlcalcdriver-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/.pep8speaks.yml` & `mlcalcdriver-1.4.2/.pep8speaks.yml`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/LICENSE` & `mlcalcdriver-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/PKG-INFO` & `mlcalcdriver-1.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: mlcalcdriver
-Version: 1.4.1
-Summary: A package to drive atomic calculations using machine learned models.
-Home-page: https://github.com/OMalenfantThuot/ML_Calc_Driver
-Author: Olivier Malenfant-Thuot
-Author-email: malenfantthuotolivier@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Machine Learning Calculations Driver (ML\_Calc\_Driver)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Build Status](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver.svg?branch=master&kill_cache=1)](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver)
 [![Coverage Status](https://coveralls.io/repos/github/OMalenfantThuot/ML_Calc_Driver/badge.svg?branch=master&kill_cache=1)](https://coveralls.io/github/OMalenfantThuot/ML_Calc_Driver)
 [![PyPi](https://img.shields.io/pypi/v/mlcalcdriver.svg?kill_cache=1)](https://pypi.org/project/mlcalcdriver/)
 [![python](https://img.shields.io/pypi/pyversions/mlcalcdriver.svg)](https://www.python.org/)
@@ -56,9 +43,7 @@
 pip install .
 ```
 To modify the sources, instead of `pip install .`, use
 
 ```
 pip install -e .
 ```
-
-
```

### Comparing `mlcalcdriver-1.4.1/README.md` & `mlcalcdriver-1.4.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,61 @@
-# Machine Learning Calculations Driver (ML\_Calc\_Driver)
-
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-[![Build Status](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver.svg?branch=master&kill_cache=1)](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver)
-[![Coverage Status](https://coveralls.io/repos/github/OMalenfantThuot/ML_Calc_Driver/badge.svg?branch=master&kill_cache=1)](https://coveralls.io/github/OMalenfantThuot/ML_Calc_Driver)
-[![PyPi](https://img.shields.io/pypi/v/mlcalcdriver.svg?kill_cache=1)](https://pypi.org/project/mlcalcdriver/)
-[![python](https://img.shields.io/pypi/pyversions/mlcalcdriver.svg)](https://www.python.org/)
-[![PyUp](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver/shield.svg?kill_cache=1)](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver)
-
-ML\_Calc\_Driver is a driver to emulate DFT calculations using machine learned predictive models.
-To use this package, one needs an already trained model, that can predict energy or forces from an input atomic geometry.
-Supported systems depends on the model, this package should not be a limitation.
-
-This package is tested with python 3.10.
-
-Credit to [mmoriniere](https://gitlab.com/mmoriniere) for the [MyBigDFT package](https://gitlab.com/mmoriniere/MyBigDFT)
-which served as a foundation for this work. Some classes have been directly adapted from MyBigDFT.
-
-**Dependencies scanned by [PyUp.io](https://pyup.io/)**
-
-## Documentation
-
-The documentation is available [here](https://omalenfantthuot.github.io/ML_Calc_Driver/).
-
-## Installation
-
-### From PyPi
-
-To install the latest version available on PyPi:
-
-`pip install mlcalcdriver`
-
-To upgrade to last version:
-
-`pip install -U mlcalcdriver`
-
-### From sources
-
-```
-git clone git@github.com:OMalenfantThuot/ML_Calc_Driver.git
-cd ML_Calc_Driver/
-pip install -r requirements_dev.txt
-pip install .
-```
-To modify the sources, instead of `pip install .`, use
-
-```
-pip install -e .
-```
+Metadata-Version: 2.1
+Name: mlcalcdriver
+Version: 1.4.2
+Summary: A package to drive atomic calculations using machine learned models.
+Home-page: https://github.com/OMalenfantThuot/ML_Calc_Driver
+Author: Olivier Malenfant-Thuot
+Author-email: malenfantthuotolivier@gmail.com
+License: UNKNOWN
+Description: # Machine Learning Calculations Driver (ML\_Calc\_Driver)
+        
+        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+        [![Build Status](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver.svg?branch=master&kill_cache=1)](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver)
+        [![Coverage Status](https://coveralls.io/repos/github/OMalenfantThuot/ML_Calc_Driver/badge.svg?branch=master&kill_cache=1)](https://coveralls.io/github/OMalenfantThuot/ML_Calc_Driver)
+        [![PyPi](https://img.shields.io/pypi/v/mlcalcdriver.svg?kill_cache=1)](https://pypi.org/project/mlcalcdriver/)
+        [![python](https://img.shields.io/pypi/pyversions/mlcalcdriver.svg)](https://www.python.org/)
+        [![PyUp](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver/shield.svg?kill_cache=1)](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver)
+        
+        ML\_Calc\_Driver is a driver to emulate DFT calculations using machine learned predictive models.
+        To use this package, one needs an already trained model, that can predict energy or forces from an input atomic geometry.
+        Supported systems depends on the model, this package should not be a limitation.
+        
+        This package is tested with python 3.10.
+        
+        Credit to [mmoriniere](https://gitlab.com/mmoriniere) for the [MyBigDFT package](https://gitlab.com/mmoriniere/MyBigDFT)
+        which served as a foundation for this work. Some classes have been directly adapted from MyBigDFT.
+        
+        **Dependencies scanned by [PyUp.io](https://pyup.io/)**
+        
+        ## Documentation
+        
+        The documentation is available [here](https://omalenfantthuot.github.io/ML_Calc_Driver/).
+        
+        ## Installation
+        
+        ### From PyPi
+        
+        To install the latest version available on PyPi:
+        
+        `pip install mlcalcdriver`
+        
+        To upgrade to last version:
+        
+        `pip install -U mlcalcdriver`
+        
+        ### From sources
+        
+        ```
+        git clone git@github.com:OMalenfantThuot/ML_Calc_Driver.git
+        cd ML_Calc_Driver/
+        pip install -r requirements_dev.txt
+        pip install .
+        ```
+        To modify the sources, instead of `pip install .`, use
+        
+        ```
+        pip install -e .
+        ```
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
```

### Comparing `mlcalcdriver-1.4.1/docs/Makefile` & `mlcalcdriver-1.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_modules/index.html` & `mlcalcdriver-1.4.2/docs/_modules/index.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/base/job.html` & `mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/base/job.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/base/posinp.html` & `mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/base/posinp.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/ase_calculators/asespkcalculator.html` & `mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/calculators/ase_calculators/asespkcalculator.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/calculator.html` & `mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/calculators/calculator.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/ensemble.html` & `mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/calculators/ensemble.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/calculators/schnetpack.html` & `mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/calculators/schnetpack.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/interfaces/ase_interface.html` & `mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/interfaces/ase_interface.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/interfaces/schnetpack_interface.html` & `mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/interfaces/schnetpack_interface.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/workflows/geopt.html` & `mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/workflows/geopt.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_modules/mlcalcdriver/workflows/phonon.html` & `mlcalcdriver-1.4.2/docs/_modules/mlcalcdriver/workflows/phonon.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_sources/interfaces.rst.txt` & `mlcalcdriver-1.4.2/docs/_sources/interfaces.rst.txt`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/basic.css` & `mlcalcdriver-1.4.2/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/badge_only.css` & `mlcalcdriver-1.4.2/docs/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.eot` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.svg` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.ttf` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.woff` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/fontawesome-webfont.woff2` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold-italic.woff` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold-italic.woff2` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold.woff` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-bold.woff2` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal-italic.woff` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal-italic.woff2` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal.woff` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/fonts/lato-normal.woff2` & `mlcalcdriver-1.4.2/docs/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/css/theme.css` & `mlcalcdriver-1.4.2/docs/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/doctools.js` & `mlcalcdriver-1.4.2/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/jquery-3.5.1.js` & `mlcalcdriver-1.4.2/docs/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/jquery.js` & `mlcalcdriver-1.4.2/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/js/badge_only.js` & `mlcalcdriver-1.4.2/docs/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/js/html5shiv-printshiv.min.js` & `mlcalcdriver-1.4.2/docs/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/js/html5shiv.min.js` & `mlcalcdriver-1.4.2/docs/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/js/theme.js` & `mlcalcdriver-1.4.2/docs/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/language_data.js` & `mlcalcdriver-1.4.2/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/pygments.css` & `mlcalcdriver-1.4.2/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/searchtools.js` & `mlcalcdriver-1.4.2/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/underscore-1.13.1.js` & `mlcalcdriver-1.4.2/docs/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/_static/underscore.js` & `mlcalcdriver-1.4.2/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/ase_interface.html` & `mlcalcdriver-1.4.2/docs/ase_interface.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/asespkcalc.html` & `mlcalcdriver-1.4.2/docs/asespkcalc.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/base.html` & `mlcalcdriver-1.4.2/docs/base.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/calculator.html` & `mlcalcdriver-1.4.2/docs/calculator.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/calculators.html` & `mlcalcdriver-1.4.2/docs/calculators.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/ensemble.html` & `mlcalcdriver-1.4.2/docs/ensemble.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/genindex.html` & `mlcalcdriver-1.4.2/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/geopt.html` & `mlcalcdriver-1.4.2/docs/geopt.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/globals.html` & `mlcalcdriver-1.4.2/docs/globals.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/index.html` & `mlcalcdriver-1.4.2/docs/index.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/interfaces.html` & `mlcalcdriver-1.4.2/docs/interfaces.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/job.html` & `mlcalcdriver-1.4.2/docs/job.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/objects.inv` & `mlcalcdriver-1.4.2/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/phonon.html` & `mlcalcdriver-1.4.2/docs/phonon.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/posinp.html` & `mlcalcdriver-1.4.2/docs/posinp.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/py-modindex.html` & `mlcalcdriver-1.4.2/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/schnet_interface.html` & `mlcalcdriver-1.4.2/docs/schnet_interface.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/schnetcalc.html` & `mlcalcdriver-1.4.2/docs/schnetcalc.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/search.html` & `mlcalcdriver-1.4.2/docs/search.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/searchindex.js` & `mlcalcdriver-1.4.2/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/source/conf.py` & `mlcalcdriver-1.4.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/source/interfaces.rst` & `mlcalcdriver-1.4.2/docs/source/interfaces.rst`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/docs/workflows.html` & `mlcalcdriver-1.4.2/docs/workflows.html`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/base/job.py` & `mlcalcdriver-1.4.2/mlcalcdriver/base/job.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/base/posinp.py` & `mlcalcdriver-1.4.2/mlcalcdriver/base/posinp.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,14 +134,33 @@
         <BLANKLINE>
         """
         with open(filename, "r") as stream:
             lines = [line.split() for line in stream.readlines()]
             return cls._from_lines(lines)
 
     @classmethod
+    def read(cls, filename):
+        r"""
+        Initialize the input positions from a file on disk.
+        Uses ase.io.read to support many file formats.
+
+        Parameters
+        ----------
+        filename : str
+            Name of the input file
+
+        Returns
+        -------
+        Posinp
+        """
+        from ase.io import read
+
+        return Posinp.from_ase(read(filename))
+
+    @classmethod
     def from_string(cls, posinp):
         r"""
         Initialize the input positions from a string.
 
         Parameters
         ----------
         posinp : str
@@ -201,15 +220,16 @@
                 "number of atoms ({} != {})".format(len(lines), n_at)
             )
         # Decode the atoms
         atoms = []
         for line in lines:
             atom_type = line[0]
             position = np.array(line[1:4], dtype=float)
-            atoms.append(Atom(atom_type, position))
+            isotope = line[4] if len(line) > 4 else None
+            atoms.append(Atom(atom_type, position, isotope=isotope))
         return cls(atoms, units, boundary_conditions, cell=cell, angles=angles)
 
     @classmethod
     def from_dict(cls, posinp):
         r"""
         Initialize the input positions from a dictionary.
 
@@ -713,15 +733,15 @@
 
 
 class Atom(object):
     r"""
     Class allowing to represent an atom by its type and position.
     """
 
-    def __init__(self, atom_type, position):
+    def __init__(self, atom_type, position, isotope=None):
         r"""
         Parameters
         ----------
         atom_type : str
             Type of the atom.
         position : list or :class:`numpy.array` of length 3
             Position of the atom.
@@ -734,15 +754,16 @@
         array([0., 0., 0.])
         >>> a.mass
         12.011
         """
         # TODO: Check that the atom type exists
         self.type = atom_type
         self.position = position
-        self.mass = ATOMS_MASS[self.type]
+        self.isotope = isotope
+        # self.mass = ATOMS_MASS[self.isotope] if self.isotope else ATOMS_MASS[self.type]
 
     @classmethod
     def from_dict(cls, atom_dict):
         r"""
         Parameters
         ----------
         atom_dict : dict
@@ -782,26 +803,36 @@
 
     @position.setter
     def position(self, position):
         assert len(position) == 3, "The position must have three components."
         self._position = np.array(position, dtype=float)
 
     @property
+    def isotope(self):
+        r"""
+        Returns
+        -------
+        str or None
+            Isotope of the atom
+        """
+        return self._isotope
+
+    @isotope.setter
+    def isotope(self, isotope):
+        self._isotope = isotope
+
+    @property
     def mass(self):
         r"""
         Returns
         -------
         float
             Mass of the atom in atomic mass units.
         """
-        return self._mass
-
-    @mass.setter
-    def mass(self, mass):
-        self._mass = mass
+        return ATOMS_MASS[self.isotope] if self.isotope else ATOMS_MASS[self.type]
 
     def translate(self, vector):
         r"""
         Translate the coordinates of the atom by the values of the
         vector.
 
         Returns
@@ -827,24 +858,32 @@
         r"""
         Returns
         -------
         str
             String representation of the atom, mainly used to create the
             string representation of a Posinp instance.
         """
-        return "{t}  {: .15}  {: .15}  {: .15}\n".format(t=self.type, *self.position)
+        return (
+            f"{self.type}  {self.position[0]:.15}  {self.position[1]:.15}  {self.position[2]:.15}  {self.isotope}\n"
+            if self.isotope
+            else f"{self.type}  {self.position[0]:.15}  {self.position[1]:.15}  {self.position[2]:.15}\n"
+        )
 
     def __repr__(self):
         r"""
         Returns
         -------
         str
             General string representation of an Atom instance.
         """
-        return "Atom('{}', {})".format(self.type, list(self.position))
+        return (
+            "Atom('{}', {}, {})".format(self.type, list(self.position), self.isotope)
+            if self.isotope
+            else "Atom('{}', {})".format(self.type, list(self.position))
+        )
 
     def __eq__(self, other):
         r"""
         Two atoms are the same if they are located on the same position
         and have the same type.
 
         Parameters
```

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/calculators/__init__.py` & `mlcalcdriver-1.4.2/mlcalcdriver/calculators/__init__.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/calculators/ase_calculators/asespkcalculator.py` & `mlcalcdriver-1.4.2/mlcalcdriver/calculators/ase_calculators/asespkcalculator.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/calculators/calculator.py` & `mlcalcdriver-1.4.2/mlcalcdriver/calculators/calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from mlcalcdriver.globals import eVA
+
 r"""
 The :class:`Calculator` is the general class for a machine learning
 calculator. A specific class derived from this one must be implemented
 for each new type of model.
 """
 
 
@@ -80,7 +82,13 @@
                 [k in ["positions", "energy", "dipole_moment"] for k in units.keys()]
             ):
                 self._units = units
             else:
                 raise KeyError("Units key not recognized.")
         else:
             raise TypeError("Units should be given in a dictionary.")
+
+
+class DummyCalculator(Calculator):
+    def __init__(self):
+        properties = ["energy"]
+        super().__init__(available_properties=properties, units=eVA)
```

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/calculators/ensemble.py` & `mlcalcdriver-1.4.2/mlcalcdriver/calculators/ensemble.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/calculators/schnetpack.py` & `mlcalcdriver-1.4.2/mlcalcdriver/calculators/schnetpack.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/calculators/schnetpack_patch.py` & `mlcalcdriver-1.4.2/mlcalcdriver/calculators/schnetpack_patch.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/calculators/utils.py` & `mlcalcdriver-1.4.2/mlcalcdriver/calculators/utils.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/globals.py` & `mlcalcdriver-1.4.2/mlcalcdriver/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 ATOMS_MASS = {
     "H": 1.00794,
     "He": 4.002602,
     "Li": 6.941,
     "Be": 9.012182,
     "B": 10.811,
     "C": 12.011,
+    "C12": 12,
+    "C13": 13.003,
+    "C14": 14.003,
     "N": 14.00674,
     "O": 15.9994,
     "F": 18.9984032,
     "Ne": 20.1797,
     "Na": 22.989768,
     "Mg": 24.3050,
     "Al": 26.981539,
@@ -95,15 +98,15 @@
     "Ac": 227.028,
     "Th": 232.038,
     "Pa": 231.036,
     "U": 238.029,
     "Np": 237.048,
     "Pu": 244.064,
     "Am": 243.061,
-    "Cm": 247.070
+    "Cm": 247.070,
 }
 r"""
 `Dictionnary` containing elemental masses, in atomic mass units.
 Used to compute vibrational energies.
 """
 
 ####
```

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/interfaces/ase_interface.py` & `mlcalcdriver-1.4.2/mlcalcdriver/interfaces/ase_interface.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/interfaces/atoms_to_patches.py` & `mlcalcdriver-1.4.2/mlcalcdriver/interfaces/atoms_to_patches.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/interfaces/schnetpack_interface.py` & `mlcalcdriver-1.4.2/mlcalcdriver/interfaces/schnetpack_interface.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/workflows/geopt.py` & `mlcalcdriver-1.4.2/mlcalcdriver/workflows/geopt.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver/workflows/phonon.py` & `mlcalcdriver-1.4.2/mlcalcdriver/workflows/phonon.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The :class:`Phonon` class allows to compute the normal modes
 and vibration energies of a system using a machine
 learning trained model.
 """
 
 import numpy as np
 from mlcalcdriver import Job, Posinp
-from mlcalcdriver.calculators import Calculator
+from mlcalcdriver.calculators.calculator import Calculator, DummyCalculator
 from mlcalcdriver.workflows import Geopt
 from copy import deepcopy
 from mlcalcdriver.globals import ANG_TO_B, B_TO_ANG, EV_TO_HA, HA_TO_CMM1, AMU_TO_EMU
 
 
 class Phonon:
     r"""
@@ -290,15 +290,15 @@
         Computes the hessian matrix from the forces
         """
         n_at = len(self.posinp)
         if "hessian" in job.results.keys():
             h = (
                 job.results["hessian"].reshape(3 * n_at, 3 * n_at)
                 * EV_TO_HA
-                * B_TO_ANG ** 2
+                * B_TO_ANG**2
             )
             return (h + h.T) / 2.0
         else:
             hessian = np.zeros((3 * n_at, 3 * n_at))
             forces = np.array(job.results["forces"]) * EV_TO_HA * B_TO_ANG
             for i in range(3 * n_at):
                 hessian[i, :] = (
@@ -312,7 +312,56 @@
         r"""
         Obtains the eigenvalues and eigenvectors from
         the dynamical matrix
         """
         eigs, vecs = np.linalg.eigh(self.dyn_mat)
         eigs = np.sign(eigs) * np.sqrt(np.where(eigs < 0, -eigs, eigs))
         return eigs, vecs
+
+
+class PhononFromHessian(Phonon):
+    r"""
+    Similar to the main Phonon class, but can be used when calculating
+    many structures with the same hessian matrix (isotopes study). Saves
+    the time to compute the hessian matrix each time
+    """
+
+    def __init__(self, posinp, hessian):
+        r"""
+        Parameters
+        ----------
+        posinp : mlcaldriver.Posinp
+            Initial positions of the system under consideration.
+        hessian : np.ndarray or str
+            Hessian matrix calculated before instanciating this class.
+            Can be the array or a path to .npy file (created with np.save).
+        """
+        super().__init__(
+            posinp=posinp,
+            calculator=DummyCalculator(),
+            relax=False,
+            finite_difference=False,
+        )
+        self.hessian = hessian
+
+    @property
+    def hessian(self):
+        return self._hessian
+
+    @hessian.setter
+    def hessian(self, hessian):
+        if isinstance(hessian, str):
+            hessian = np.load(hessian)
+
+        if isinstance(hessian, np.ndarray):
+            assert hessian[0].shape == (
+                3 * len(self.posinp),
+                3 * len(self.posinp),
+            ), f"The hessian shape {hessian.shape} does not match the number of atoms {len(self.posinp)}"
+            self._hessian = hessian
+        else:
+            raise TypeError("The hessian matrix should be a numpy array.")
+
+    def run(self):
+        job = Job(posinp=self.posinp, calculator=self.calculator)
+        job.results["hessian"] = self.hessian
+        self._post_proc(job)
```

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver.egg-info/PKG-INFO` & `mlcalcdriver-1.4.2/mlcalcdriver.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,61 @@
 Metadata-Version: 2.1
 Name: mlcalcdriver
-Version: 1.4.1
+Version: 1.4.2
 Summary: A package to drive atomic calculations using machine learned models.
 Home-page: https://github.com/OMalenfantThuot/ML_Calc_Driver
 Author: Olivier Malenfant-Thuot
 Author-email: malenfantthuotolivier@gmail.com
 License: UNKNOWN
+Description: # Machine Learning Calculations Driver (ML\_Calc\_Driver)
+        
+        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+        [![Build Status](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver.svg?branch=master&kill_cache=1)](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver)
+        [![Coverage Status](https://coveralls.io/repos/github/OMalenfantThuot/ML_Calc_Driver/badge.svg?branch=master&kill_cache=1)](https://coveralls.io/github/OMalenfantThuot/ML_Calc_Driver)
+        [![PyPi](https://img.shields.io/pypi/v/mlcalcdriver.svg?kill_cache=1)](https://pypi.org/project/mlcalcdriver/)
+        [![python](https://img.shields.io/pypi/pyversions/mlcalcdriver.svg)](https://www.python.org/)
+        [![PyUp](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver/shield.svg?kill_cache=1)](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver)
+        
+        ML\_Calc\_Driver is a driver to emulate DFT calculations using machine learned predictive models.
+        To use this package, one needs an already trained model, that can predict energy or forces from an input atomic geometry.
+        Supported systems depends on the model, this package should not be a limitation.
+        
+        This package is tested with python 3.10.
+        
+        Credit to [mmoriniere](https://gitlab.com/mmoriniere) for the [MyBigDFT package](https://gitlab.com/mmoriniere/MyBigDFT)
+        which served as a foundation for this work. Some classes have been directly adapted from MyBigDFT.
+        
+        **Dependencies scanned by [PyUp.io](https://pyup.io/)**
+        
+        ## Documentation
+        
+        The documentation is available [here](https://omalenfantthuot.github.io/ML_Calc_Driver/).
+        
+        ## Installation
+        
+        ### From PyPi
+        
+        To install the latest version available on PyPi:
+        
+        `pip install mlcalcdriver`
+        
+        To upgrade to last version:
+        
+        `pip install -U mlcalcdriver`
+        
+        ### From sources
+        
+        ```
+        git clone git@github.com:OMalenfantThuot/ML_Calc_Driver.git
+        cd ML_Calc_Driver/
+        pip install -r requirements_dev.txt
+        pip install .
+        ```
+        To modify the sources, instead of `pip install .`, use
+        
+        ```
+        pip install -e .
+        ```
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Machine Learning Calculations Driver (ML\_Calc\_Driver)
-
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-[![Build Status](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver.svg?branch=master&kill_cache=1)](https://travis-ci.org/OMalenfantThuot/ML_Calc_Driver)
-[![Coverage Status](https://coveralls.io/repos/github/OMalenfantThuot/ML_Calc_Driver/badge.svg?branch=master&kill_cache=1)](https://coveralls.io/github/OMalenfantThuot/ML_Calc_Driver)
-[![PyPi](https://img.shields.io/pypi/v/mlcalcdriver.svg?kill_cache=1)](https://pypi.org/project/mlcalcdriver/)
-[![python](https://img.shields.io/pypi/pyversions/mlcalcdriver.svg)](https://www.python.org/)
-[![PyUp](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver/shield.svg?kill_cache=1)](https://pyup.io/repos/github/OMalenfantThuot/ML_Calc_Driver)
-
-ML\_Calc\_Driver is a driver to emulate DFT calculations using machine learned predictive models.
-To use this package, one needs an already trained model, that can predict energy or forces from an input atomic geometry.
-Supported systems depends on the model, this package should not be a limitation.
-
-This package is tested with python 3.10.
-
-Credit to [mmoriniere](https://gitlab.com/mmoriniere) for the [MyBigDFT package](https://gitlab.com/mmoriniere/MyBigDFT)
-which served as a foundation for this work. Some classes have been directly adapted from MyBigDFT.
-
-**Dependencies scanned by [PyUp.io](https://pyup.io/)**
-
-## Documentation
-
-The documentation is available [here](https://omalenfantthuot.github.io/ML_Calc_Driver/).
-
-## Installation
-
-### From PyPi
-
-To install the latest version available on PyPi:
-
-`pip install mlcalcdriver`
-
-To upgrade to last version:
-
-`pip install -U mlcalcdriver`
-
-### From sources
-
-```
-git clone git@github.com:OMalenfantThuot/ML_Calc_Driver.git
-cd ML_Calc_Driver/
-pip install -r requirements_dev.txt
-pip install .
-```
-To modify the sources, instead of `pip install .`, use
-
-```
-pip install -e .
-```
-
-
```

### Comparing `mlcalcdriver-1.4.1/mlcalcdriver.egg-info/SOURCES.txt` & `mlcalcdriver-1.4.2/mlcalcdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/setup.py` & `mlcalcdriver-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "torch>=2.0.1",
     "schnetpack==1.0.1",
     "ase>=3.22.0",
 ]
 
 setup(
     name="mlcalcdriver",
-    version="1.4.1",
+    version="1.4.2",
     author="Olivier Malenfant-Thuot",
     author_email="malenfantthuotolivier@gmail.com",
     description="A package to drive atomic calculations using machine learned models.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/OMalenfantThuot/ML_Calc_Driver",
     packages=find_packages(),
```

### Comparing `mlcalcdriver-1.4.1/tests/models/H2O_forces_model` & `mlcalcdriver-1.4.2/tests/models/H2O_forces_model`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/tests/models/H2O_model` & `mlcalcdriver-1.4.2/tests/models/H2O_model`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/tests/models/ani1_N2_model` & `mlcalcdriver-1.4.2/tests/models/ani1_N2_model`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/tests/models/myN2_model` & `mlcalcdriver-1.4.2/tests/models/myN2_model`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/tests/models/wacsf_model` & `mlcalcdriver-1.4.2/tests/models/wacsf_model`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/tests/test_angles.py` & `mlcalcdriver-1.4.2/tests/test_angles.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/tests/test_calculators.py` & `mlcalcdriver-1.4.2/tests/test_calculators.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/tests/test_geopt.py` & `mlcalcdriver-1.4.2/tests/test_geopt.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/tests/test_interface.py` & `mlcalcdriver-1.4.2/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/tests/test_job.py` & `mlcalcdriver-1.4.2/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/tests/test_phonon.py` & `mlcalcdriver-1.4.2/tests/test_phonon.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 import pytest
 import numpy as np
 from mlcalcdriver import Posinp, Job
 from mlcalcdriver.calculators import SchnetPackCalculator
-from mlcalcdriver.workflows import Phonon
+from mlcalcdriver.workflows.phonon import Phonon, PhononFromHessian
 
 pos_folder = "tests/posinp_files/"
 model_folder = "tests/models/"
 
 
 class TestPhononFinite:
-
     posN2 = Posinp.from_file(os.path.join(pos_folder, "N2_unrelaxed.xyz"))
     calcN2 = SchnetPackCalculator(os.path.join(model_folder, "myN2_model"))
 
     def test_ph_N2(self):
         ph1 = Phonon(posinp=self.posN2, calculator=self.calcN2, finite_difference=True)
         ph1.run(batch_size=1)
         assert np.isclose(ph1.energies.max(), 2339.53, atol=0.01)
@@ -45,15 +44,14 @@
 
     def test_phonon_calc_error(self):
         with pytest.raises(TypeError):
             ph = Phonon(posinp=self.posN2, calculator=None)
 
 
 class TestPhononAutoGrad:
-
     posH2O = Posinp.from_file(os.path.join(pos_folder, "H2Orelaxed.xyz"))
     calc_ener = SchnetPackCalculator(os.path.join(model_folder, "H2O_model"))
     calc_for = SchnetPackCalculator(os.path.join(model_folder, "H2O_forces_model"))
 
     def test_ph_h2o_autograd_2nd_derivative(self):
         ph1 = Phonon(posinp=self.posH2O, calculator=self.calc_ener)
         ph1.run()
@@ -61,7 +59,15 @@
         assert np.allclose(ph1.energies[6:9], [1726, 3856, 3942], atol=1)
 
     def test_ph_h2o_autograd_1st_derivative(self):
         ph1 = Phonon(posinp=self.posH2O, calculator=self.calc_for)
         ph1.run()
         ph1.energies.sort()
         assert np.allclose(ph1.energies[6:9], [1589, 3703, 3812], atol=1)
+
+    def test_ph_from_hessian(self):
+        job = Job(posinp=self.posH2O, calculator=self.calc_for)
+        job.run("hessian")
+        ph = PhononFromHessian(posinp=self.posH2O, hessian=job.results["hessian"])
+        ph.run()
+        ph.energies.sort()
+        assert np.allclose(ph.energies[6:9], [1589, 3705, 3814], atol=1)
```

### Comparing `mlcalcdriver-1.4.1/tests/test_posinp.py` & `mlcalcdriver-1.4.2/tests/test_posinp.py`

 * *Files identical despite different names*

### Comparing `mlcalcdriver-1.4.1/tests/test_schnetpack.py` & `mlcalcdriver-1.4.2/tests/test_schnetpack.py`

 * *Files identical despite different names*

