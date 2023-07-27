# Comparing `tmp/tomotok-1.2.2.tar.gz` & `tmp/tomotok-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomotok-1.2.2.tar", last modified: Mon Dec  5 16:39:56 2022, max compression
+gzip compressed data, was "tomotok-1.3.tar", last modified: Thu Jul 27 10:46:38 2023, max compression
```

## Comparing `tomotok-1.2.2.tar` & `tomotok-1.3.tar`

### file list

```diff
@@ -1,102 +1,104 @@
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:56.941258 tomotok-1.2.2/
--rw-r--r--   0 svoboda   (1281) users      (100)       78 2022-05-12 17:54:41.000000 tomotok-1.2.2/.gitignore
--rw-r--r--   0 svoboda   (1281) users      (100)       75 2021-11-15 15:38:39.000000 tomotok-1.2.2/AUTHORS.txt
--rw-r--r--   0 svoboda   (1281) users      (100)     1174 2022-04-22 12:52:52.000000 tomotok-1.2.2/CONTRIBUTING.md
--rw-r--r--   0 svoboda   (1281) users      (100)    13793 2021-11-12 12:45:01.000000 tomotok-1.2.2/LICENCE.txt
--rw-r--r--   0 svoboda   (1281) users      (100)      231 2021-11-12 12:45:01.000000 tomotok-1.2.2/MANIFEST.in
--rw-r--r--   0 svoboda   (1281) users      (100)     3328 2022-12-05 16:39:56.909258 tomotok-1.2.2/PKG-INFO
--rw-r--r--   0 svoboda   (1281) users      (100)     2997 2022-10-14 07:33:19.000000 tomotok-1.2.2/README.md
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:54.509207 tomotok-1.2.2/docs/
--rw-r--r--   0 svoboda   (1281) users      (100)     8067 2021-10-25 08:50:22.000000 tomotok-1.2.2/docs/Makefile
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:54.717211 tomotok-1.2.2/docs/source/
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:54.937216 tomotok-1.2.2/docs/source/api/
--rw-r--r--   0 svoboda   (1281) users      (100)     1240 2021-10-25 08:50:22.000000 tomotok-1.2.2/docs/source/api/tomotok.core.geometry.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      802 2022-12-02 13:48:54.000000 tomotok-1.2.2/docs/source/api/tomotok.core.inversions.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      640 2021-10-25 08:50:22.000000 tomotok-1.2.2/docs/source/api/tomotok.core.io.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      607 2021-10-25 08:50:22.000000 tomotok-1.2.2/docs/source/api/tomotok.core.rst
--rw-r--r--   0 svoboda   (1281) users      (100)     1031 2021-10-25 08:50:22.000000 tomotok-1.2.2/docs/source/api/tomotok.core.tools.rst
--rw-r--r--   0 svoboda   (1281) users      (100)     1184 2021-10-25 08:50:22.000000 tomotok-1.2.2/docs/source/api/tomotok.gui.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      188 2021-10-25 08:50:22.000000 tomotok-1.2.2/docs/source/api/tomotok.rst
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:55.117220 tomotok-1.2.2/docs/source/auxilia/
--rw-r--r--   0 svoboda   (1281) users      (100)     1481 2021-10-25 08:50:22.000000 tomotok-1.2.2/docs/source/auxilia/auxilia.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      323 2021-10-25 08:50:22.000000 tomotok-1.2.2/docs/source/auxilia/derivative.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      521 2021-11-12 12:45:01.000000 tomotok-1.2.2/docs/source/auxilia/geometry.rst
--rw-r--r--   0 svoboda   (1281) users      (100)     1051 2021-11-12 12:45:01.000000 tomotok-1.2.2/docs/source/auxilia/io.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      315 2021-11-12 12:45:01.000000 tomotok-1.2.2/docs/source/auxilia/phantoms.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      554 2021-11-12 12:45:01.000000 tomotok-1.2.2/docs/source/auxilia/tools.rst
--rw-r--r--   0 svoboda   (1281) users      (100)     9992 2022-11-02 13:21:26.000000 tomotok-1.2.2/docs/source/conf.py
--rw-r--r--   0 svoboda   (1281) users      (100)      961 2021-10-25 08:50:22.000000 tomotok-1.2.2/docs/source/glossary.rst
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:55.257223 tomotok-1.2.2/docs/source/gui/
--rw-r--r--   0 svoboda   (1281) users      (100)      215 2021-11-12 12:45:01.000000 tomotok-1.2.2/docs/source/gui/apps.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      241 2021-11-12 12:45:01.000000 tomotok-1.2.2/docs/source/gui/common.rst
--rw-r--r--   0 svoboda   (1281) users      (100)     1546 2021-10-25 08:50:22.000000 tomotok-1.2.2/docs/source/gui/gui.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      800 2021-11-12 12:45:01.000000 tomotok-1.2.2/docs/source/gui/tomo.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      692 2021-11-12 12:45:01.000000 tomotok-1.2.2/docs/source/index.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      362 2021-11-12 14:25:22.000000 tomotok-1.2.2/docs/source/install.rst
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:55.381225 tomotok-1.2.2/docs/source/inversions/
--rw-r--r--   0 svoboda   (1281) users      (100)     3636 2021-10-25 08:50:23.000000 tomotok-1.2.2/docs/source/inversions/bob.rst
--rw-r--r--   0 svoboda   (1281) users      (100)     1996 2021-11-12 12:45:01.000000 tomotok-1.2.2/docs/source/inversions/inversions.rst
--rw-r--r--   0 svoboda   (1281) users      (100)     5395 2021-10-25 08:50:23.000000 tomotok-1.2.2/docs/source/inversions/lame.rst
--rw-r--r--   0 svoboda   (1281) users      (100)     3568 2021-11-12 12:45:01.000000 tomotok-1.2.2/docs/source/inversions/mfr.rst
--rw-r--r--   0 svoboda   (1281) users      (100)    13838 2021-11-12 12:45:01.000000 tomotok-1.2.2/docs/source/licence.rst
--rw-r--r--   0 svoboda   (1281) users      (100)     1011 2021-10-25 08:50:23.000000 tomotok-1.2.2/docs/source/welcome.rst
--rw-r--r--   0 svoboda   (1281) users      (100)      103 2021-11-12 12:45:01.000000 tomotok-1.2.2/pyproject.toml
--rw-r--r--   0 svoboda   (1281) users      (100)       88 2022-10-14 07:33:19.000000 tomotok-1.2.2/requirements.txt
--rw-r--r--   0 svoboda   (1281) users      (100)       38 2022-12-05 16:39:56.945258 tomotok-1.2.2/setup.cfg
--rw-r--r--   0 svoboda   (1281) users      (100)      919 2022-10-14 07:33:19.000000 tomotok-1.2.2/setup.py
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:55.409226 tomotok-1.2.2/tomotok/
--rw-r--r--   0 svoboda   (1281) users      (100)      177 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/__init__.py
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:55.717232 tomotok-1.2.2/tomotok/core/
--rw-r--r--   0 svoboda   (1281) users      (100)        5 2022-12-02 16:24:56.000000 tomotok-1.2.2/tomotok/core/VERSION
--rwxr-xr-x   0 svoboda   (1281) users      (100)      438 2021-11-12 12:45:01.000000 tomotok-1.2.2/tomotok/core/__init__.py
--rwxr-xr-x   0 svoboda   (1281) users      (100)    11225 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/derivative.py
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:55.953237 tomotok-1.2.2/tomotok/core/geometry/
--rw-r--r--   0 svoboda   (1281) users      (100)      609 2022-02-23 13:56:30.000000 tomotok-1.2.2/tomotok/core/geometry/__init__.py
--rw-r--r--   0 svoboda   (1281) users      (100)     7836 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/geometry/analytical.py
--rw-r--r--   0 svoboda   (1281) users      (100)     3687 2022-02-23 13:56:30.000000 tomotok-1.2.2/tomotok/core/geometry/generators.py
--rw-r--r--   0 svoboda   (1281) users      (100)     5637 2022-05-12 16:42:17.000000 tomotok-1.2.2/tomotok/core/geometry/grids.py
--rw-r--r--   0 svoboda   (1281) users      (100)     4283 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/geometry/handler.py
--rw-r--r--   0 svoboda   (1281) users      (100)     2563 2022-02-23 13:56:30.000000 tomotok-1.2.2/tomotok/core/geometry/io.py
--rw-r--r--   0 svoboda   (1281) users      (100)     4453 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/geometry/los.py
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:56.121241 tomotok-1.2.2/tomotok/core/inversions/
--rwxr-xr-x   0 svoboda   (1281) users      (100)      471 2022-05-12 17:51:29.000000 tomotok-1.2.2/tomotok/core/inversions/__init__.py
--rw-r--r--   0 svoboda   (1281) users      (100)     9830 2022-12-02 14:40:28.000000 tomotok-1.2.2/tomotok/core/inversions/bob.py
--rw-r--r--   0 svoboda   (1281) users      (100)    12274 2022-12-02 16:53:21.000000 tomotok-1.2.2/tomotok/core/inversions/lame.py
--rw-r--r--   0 svoboda   (1281) users      (100)    12620 2022-12-02 16:41:41.000000 tomotok-1.2.2/tomotok/core/inversions/mfr.py
--rw-r--r--   0 svoboda   (1281) users      (100)     7879 2022-12-02 16:44:04.000000 tomotok-1.2.2/tomotok/core/inversions/tikhonov.py
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:56.237243 tomotok-1.2.2/tomotok/core/io/
--rwxr-xr-x   0 svoboda   (1281) users      (100)      442 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/io/__init__.py
--rw-r--r--   0 svoboda   (1281) users      (100)    10199 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/io/diag.py
--rw-r--r--   0 svoboda   (1281) users      (100)      942 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/io/support.py
--rwxr-xr-x   0 svoboda   (1281) users      (100)     8928 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/io/tokamaks.py
--rw-r--r--   0 svoboda   (1281) users      (100)     3459 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/phantoms.py
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:56.265244 tomotok-1.2.2/tomotok/core/tests/
--rwxr-xr-x   0 svoboda   (1281) users      (100)      122 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/tests/__init__.py
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:56.449248 tomotok-1.2.2/tomotok/core/tools/
--rwxr-xr-x   0 svoboda   (1281) users      (100)      320 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/tools/__init__.py
--rw-r--r--   0 svoboda   (1281) users      (100)     5696 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/tools/checkers.py
--rw-r--r--   0 svoboda   (1281) users      (100)    14922 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/tools/data.py
--rw-r--r--   0 svoboda   (1281) users      (100)     1316 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/tools/gifmaker.py
--rw-r--r--   0 svoboda   (1281) users      (100)     1564 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/tools/postproc.py
--rw-r--r--   0 svoboda   (1281) users      (100)     2461 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/core/tools/projection.py
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:56.705253 tomotok-1.2.2/tomotok/gui/
--rwxr-xr-x   0 svoboda   (1281) users      (100)      149 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/gui/__init__.py
--rw-r--r--   0 svoboda   (1281) users      (100)    18225 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/gui/apps.py
--rw-r--r--   0 svoboda   (1281) users      (100)    13385 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/gui/menus.py
--rw-r--r--   0 svoboda   (1281) users      (100)     5779 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/gui/merfer.py
--rw-r--r--   0 svoboda   (1281) users      (100)    10676 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/gui/profiler.py
--rw-r--r--   0 svoboda   (1281) users      (100)    26408 2021-11-12 12:45:01.000000 tomotok-1.2.2/tomotok/gui/roi.py
--rw-r--r--   0 svoboda   (1281) users      (100)    14461 2021-10-25 08:50:23.000000 tomotok-1.2.2/tomotok/gui/widgets.py
--rw-r--r--   0 svoboda   (1281) users      (100)    21916 2021-11-12 12:45:01.000000 tomotok-1.2.2/tomotok/gui/widgets_tomo.py
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:55.597230 tomotok-1.2.2/tomotok.egg-info/
--rw-r--r--   0 svoboda   (1281) users      (100)     3328 2022-12-05 16:39:53.000000 tomotok-1.2.2/tomotok.egg-info/PKG-INFO
--rw-r--r--   0 svoboda   (1281) users      (100)     2246 2022-12-05 16:39:53.000000 tomotok-1.2.2/tomotok.egg-info/SOURCES.txt
--rw-r--r--   0 svoboda   (1281) users      (100)        1 2022-12-05 16:39:53.000000 tomotok-1.2.2/tomotok.egg-info/dependency_links.txt
--rw-r--r--   0 svoboda   (1281) users      (100)        8 2022-12-05 16:39:53.000000 tomotok-1.2.2/tomotok.egg-info/namespace_packages.txt
--rw-r--r--   0 svoboda   (1281) users      (100)       57 2022-12-05 16:39:53.000000 tomotok-1.2.2/tomotok.egg-info/requires.txt
--rw-r--r--   0 svoboda   (1281) users      (100)        8 2022-12-05 16:39:53.000000 tomotok-1.2.2/tomotok.egg-info/top_level.txt
-drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2022-12-05 16:39:56.877257 tomotok-1.2.2/tutorials/
--rw-r--r--   0 svoboda   (1281) users      (100)     8526 2022-11-01 16:00:06.000000 tomotok-1.2.2/tutorials/biorthogonal.ipynb
--rw-r--r--   0 svoboda   (1281) users      (100)       48 2021-09-14 13:13:45.000000 tomotok-1.2.2/tutorials/gui.py
--rw-r--r--   0 svoboda   (1281) users      (100)     5730 2022-05-12 16:33:45.000000 tomotok-1.2.2/tutorials/linear.ipynb
--rw-r--r--   0 svoboda   (1281) users      (100)     7031 2022-12-02 16:50:58.000000 tomotok-1.2.2/tutorials/minfisher.ipynb
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:38.584007 tomotok-1.3/
+-rw-r--r--   0 svoboda   (1281) users      (100)       78 2022-05-12 17:54:41.000000 tomotok-1.3/.gitignore
+-rw-r--r--   0 svoboda   (1281) users      (100)       75 2021-11-15 15:38:39.000000 tomotok-1.3/AUTHORS.txt
+-rw-r--r--   0 svoboda   (1281) users      (100)     1174 2022-04-22 12:52:52.000000 tomotok-1.3/CONTRIBUTING.md
+-rw-r--r--   0 svoboda   (1281) users      (100)    13793 2021-11-12 12:45:01.000000 tomotok-1.3/LICENCE.txt
+-rw-r--r--   0 svoboda   (1281) users      (100)      231 2021-11-12 12:45:01.000000 tomotok-1.3/MANIFEST.in
+-rw-r--r--   0 svoboda   (1281) users      (100)     3402 2023-07-27 10:46:38.580007 tomotok-1.3/PKG-INFO
+-rw-r--r--   0 svoboda   (1281) users      (100)     2997 2022-10-14 07:33:19.000000 tomotok-1.3/README.md
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:36.696015 tomotok-1.3/docs/
+-rw-r--r--   0 svoboda   (1281) users      (100)     8067 2021-10-25 08:50:22.000000 tomotok-1.3/docs/Makefile
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:36.920014 tomotok-1.3/docs/source/
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:37.164013 tomotok-1.3/docs/source/api/
+-rw-r--r--   0 svoboda   (1281) users      (100)     1217 2023-05-16 14:12:26.000000 tomotok-1.3/docs/source/api/tomotok.core.geometry.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      874 2023-05-16 14:12:26.000000 tomotok-1.3/docs/source/api/tomotok.core.inversions.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      626 2023-05-16 14:12:26.000000 tomotok-1.3/docs/source/api/tomotok.core.io.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      608 2023-05-16 14:12:26.000000 tomotok-1.3/docs/source/api/tomotok.core.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)     1166 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/api/tomotok.core.tools.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)     1158 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/api/tomotok.gui.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      198 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/api/tomotok.rst
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:37.316012 tomotok-1.3/docs/source/auxilia/
+-rw-r--r--   0 svoboda   (1281) users      (100)     1043 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/auxilia/auxilia.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      413 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/auxilia/derivative.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      640 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/auxilia/geometry.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)     1315 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/auxilia/io.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      315 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/auxilia/phantoms.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      666 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/auxilia/tools.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)    10519 2023-05-17 15:15:05.000000 tomotok-1.3/docs/source/conf.py
+-rw-r--r--   0 svoboda   (1281) users      (100)      966 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/glossary.rst
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:37.456011 tomotok-1.3/docs/source/gui/
+-rw-r--r--   0 svoboda   (1281) users      (100)      215 2021-11-12 12:45:01.000000 tomotok-1.3/docs/source/gui/apps.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      241 2021-11-12 12:45:01.000000 tomotok-1.3/docs/source/gui/common.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)     1632 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/gui/gui.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      746 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/gui/tomo.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      706 2023-05-16 14:12:27.000000 tomotok-1.3/docs/source/index.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      362 2021-11-12 14:25:22.000000 tomotok-1.3/docs/source/install.rst
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:37.584011 tomotok-1.3/docs/source/inversions/
+-rw-r--r--   0 svoboda   (1281) users      (100)     3636 2023-04-20 18:31:16.000000 tomotok-1.3/docs/source/inversions/bob.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)     1996 2021-11-12 12:45:01.000000 tomotok-1.3/docs/source/inversions/inversions.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)     5395 2023-04-20 18:31:01.000000 tomotok-1.3/docs/source/inversions/lame.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)     3568 2023-04-20 18:30:49.000000 tomotok-1.3/docs/source/inversions/mfr.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)    13838 2021-11-12 12:45:01.000000 tomotok-1.3/docs/source/licence.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)     1095 2022-12-20 09:28:24.000000 tomotok-1.3/docs/source/welcome.rst
+-rw-r--r--   0 svoboda   (1281) users      (100)      103 2021-11-12 12:45:01.000000 tomotok-1.3/pyproject.toml
+-rw-r--r--   0 svoboda   (1281) users      (100)      161 2023-05-17 15:15:05.000000 tomotok-1.3/requirements.txt
+-rw-r--r--   0 svoboda   (1281) users      (100)       38 2023-07-27 10:46:38.592007 tomotok-1.3/setup.cfg
+-rw-r--r--   0 svoboda   (1281) users      (100)      946 2023-04-06 12:09:06.000000 tomotok-1.3/setup.py
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:37.624011 tomotok-1.3/tomotok/
+-rw-r--r--   0 svoboda   (1281) users      (100)      177 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/__init__.py
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:37.816010 tomotok-1.3/tomotok/core/
+-rw-r--r--   0 svoboda   (1281) users      (100)        3 2023-07-27 10:43:35.000000 tomotok-1.3/tomotok/core/VERSION
+-rwxr-xr-x   0 svoboda   (1281) users      (100)      438 2021-11-12 12:45:01.000000 tomotok-1.3/tomotok/core/__init__.py
+-rwxr-xr-x   0 svoboda   (1281) users      (100)    18522 2023-07-12 13:37:31.000000 tomotok-1.3/tomotok/core/derivative.py
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:37.960009 tomotok-1.3/tomotok/core/geometry/
+-rw-r--r--   0 svoboda   (1281) users      (100)      609 2022-02-23 13:56:30.000000 tomotok-1.3/tomotok/core/geometry/__init__.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     7836 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/core/geometry/analytical.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     5458 2023-07-27 10:43:35.000000 tomotok-1.3/tomotok/core/geometry/generators.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     6734 2023-04-06 12:17:20.000000 tomotok-1.3/tomotok/core/geometry/grids.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     4283 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/core/geometry/handler.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     2563 2022-02-23 13:56:30.000000 tomotok-1.3/tomotok/core/geometry/io.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     4450 2023-05-17 15:15:05.000000 tomotok-1.3/tomotok/core/geometry/los.py
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:38.064009 tomotok-1.3/tomotok/core/inversions/
+-rwxr-xr-x   0 svoboda   (1281) users      (100)      548 2023-04-06 12:09:06.000000 tomotok-1.3/tomotok/core/inversions/__init__.py
+-rw-r--r--   0 svoboda   (1281) users      (100)    11282 2023-05-17 16:23:35.000000 tomotok-1.3/tomotok/core/inversions/bob.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     8284 2023-07-27 10:41:00.000000 tomotok-1.3/tomotok/core/inversions/fixed.py
+-rw-r--r--   0 svoboda   (1281) users      (100)    12274 2023-04-20 18:31:47.000000 tomotok-1.3/tomotok/core/inversions/lame.py
+-rw-r--r--   0 svoboda   (1281) users      (100)    12649 2023-07-12 13:42:27.000000 tomotok-1.3/tomotok/core/inversions/mfr.py
+-rw-r--r--   0 svoboda   (1281) users      (100)    13796 2023-05-16 09:17:27.000000 tomotok-1.3/tomotok/core/inversions/tikhonov.py
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:38.128009 tomotok-1.3/tomotok/core/io/
+-rwxr-xr-x   0 svoboda   (1281) users      (100)      442 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/core/io/__init__.py
+-rw-r--r--   0 svoboda   (1281) users      (100)    10210 2023-05-30 14:52:50.000000 tomotok-1.3/tomotok/core/io/diag.py
+-rw-r--r--   0 svoboda   (1281) users      (100)      942 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/core/io/support.py
+-rwxr-xr-x   0 svoboda   (1281) users      (100)     8928 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/core/io/tokamaks.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     3459 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/core/phantoms.py
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:38.148009 tomotok-1.3/tomotok/core/tests/
+-rwxr-xr-x   0 svoboda   (1281) users      (100)      122 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/core/tests/__init__.py
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:38.292008 tomotok-1.3/tomotok/core/tools/
+-rwxr-xr-x   0 svoboda   (1281) users      (100)      320 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/core/tools/__init__.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     5696 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/core/tools/checkers.py
+-rw-r--r--   0 svoboda   (1281) users      (100)    15069 2023-05-17 15:54:02.000000 tomotok-1.3/tomotok/core/tools/data.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     1316 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/core/tools/gifmaker.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     3380 2023-05-16 14:12:27.000000 tomotok-1.3/tomotok/core/tools/hdf.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     1564 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/core/tools/postproc.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     2461 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/core/tools/projection.py
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:38.456007 tomotok-1.3/tomotok/gui/
+-rwxr-xr-x   0 svoboda   (1281) users      (100)      149 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/gui/__init__.py
+-rw-r--r--   0 svoboda   (1281) users      (100)    18225 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/gui/apps.py
+-rw-r--r--   0 svoboda   (1281) users      (100)    13385 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/gui/menus.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     5779 2021-10-25 08:50:23.000000 tomotok-1.3/tomotok/gui/merfer.py
+-rw-r--r--   0 svoboda   (1281) users      (100)    10632 2023-05-16 14:12:27.000000 tomotok-1.3/tomotok/gui/profiler.py
+-rw-r--r--   0 svoboda   (1281) users      (100)    26367 2023-05-16 14:12:28.000000 tomotok-1.3/tomotok/gui/roi.py
+-rw-r--r--   0 svoboda   (1281) users      (100)    14450 2023-05-16 14:12:28.000000 tomotok-1.3/tomotok/gui/widgets.py
+-rw-r--r--   0 svoboda   (1281) users      (100)    21895 2023-05-16 14:12:28.000000 tomotok-1.3/tomotok/gui/widgets_tomo.py
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:37.744010 tomotok-1.3/tomotok.egg-info/
+-rw-r--r--   0 svoboda   (1281) users      (100)     3402 2023-07-27 10:46:36.000000 tomotok-1.3/tomotok.egg-info/PKG-INFO
+-rw-r--r--   0 svoboda   (1281) users      (100)     2305 2023-07-27 10:46:36.000000 tomotok-1.3/tomotok.egg-info/SOURCES.txt
+-rw-r--r--   0 svoboda   (1281) users      (100)        1 2023-07-27 10:46:36.000000 tomotok-1.3/tomotok.egg-info/dependency_links.txt
+-rw-r--r--   0 svoboda   (1281) users      (100)        8 2023-07-27 10:46:36.000000 tomotok-1.3/tomotok.egg-info/namespace_packages.txt
+-rw-r--r--   0 svoboda   (1281) users      (100)       57 2023-07-27 10:46:36.000000 tomotok-1.3/tomotok.egg-info/requires.txt
+-rw-r--r--   0 svoboda   (1281) users      (100)        8 2023-07-27 10:46:36.000000 tomotok-1.3/tomotok.egg-info/top_level.txt
+drwxr-xr-x   0 svoboda   (1281) users      (100)        0 2023-07-27 10:46:38.560007 tomotok-1.3/tutorials/
+-rw-r--r--   0 svoboda   (1281) users      (100)     8689 2023-05-17 16:20:50.000000 tomotok-1.3/tutorials/biorthogonal.ipynb
+-rw-r--r--   0 svoboda   (1281) users      (100)       48 2021-09-14 13:13:45.000000 tomotok-1.3/tutorials/gui.py
+-rw-r--r--   0 svoboda   (1281) users      (100)     5730 2022-05-12 16:33:45.000000 tomotok-1.3/tutorials/linear.ipynb
+-rw-r--r--   0 svoboda   (1281) users      (100)     7896 2023-07-27 10:44:40.000000 tomotok-1.3/tutorials/minfisher.ipynb
```

### Comparing `tomotok-1.2.2/CONTRIBUTING.md` & `tomotok-1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/LICENCE.txt` & `tomotok-1.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/PKG-INFO` & `tomotok-1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: tomotok
-Version: 1.2.2
+Version: 1.3
 Summary: Collection of algorithms used for tokamak plasma tomography
+Home-page: https://github.com/tomotok/core
 Author: Jakub Svoboda, Jordan Cavalier, Ondrej Ficker, Martin Imrisek et al.
+Author-email: svoboda@ipp.cas.cz
 License: EUPL 1.2
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 License-File: AUTHORS.txt
 
 # Tomotok
```

### Comparing `tomotok-1.2.2/README.md` & `tomotok-1.3/README.md`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/docs/Makefile` & `tomotok-1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/docs/source/api/tomotok.core.geometry.rst` & `tomotok-1.3/docs/source/api/tomotok.core.geometry.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,58 @@
 tomotok.core.geometry package
 =============================
 
 .. automodule:: tomotok.core.geometry
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 Submodules
 ----------
 
 tomotok.core.geometry.analytical module
 ---------------------------------------
 
 .. automodule:: tomotok.core.geometry.analytical
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.geometry.generators module
 ---------------------------------------
 
 .. automodule:: tomotok.core.geometry.generators
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.geometry.grids module
 ----------------------------------
 
 .. automodule:: tomotok.core.geometry.grids
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.geometry.handler module
 ------------------------------------
 
 .. automodule:: tomotok.core.geometry.handler
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.geometry.io module
 -------------------------------
 
 .. automodule:: tomotok.core.geometry.io
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.geometry.los module
 --------------------------------
 
 .. automodule:: tomotok.core.geometry.los
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
-
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `tomotok-1.2.2/docs/source/api/tomotok.core.inversions.rst` & `tomotok-1.3/docs/source/api/tomotok.core.inversions.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 tomotok.core.inversions package
 ===============================
 
 .. automodule:: tomotok.core.inversions
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 Submodules
 ----------
 
 tomotok.core.inversions.bob module
 ----------------------------------
 
 .. automodule:: tomotok.core.inversions.bob
-    :members:
-    :undoc-members:
-    :show-inheritance:
-    :special-members: __call__
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+tomotok.core.inversions.fixed module
+------------------------------------
+
+.. automodule:: tomotok.core.inversions.fixed
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.inversions.lame module
 -----------------------------------
 
 .. automodule:: tomotok.core.inversions.lame
-    :members:
-    :undoc-members:
-    :show-inheritance:
-    :special-members: __call__
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.inversions.mfr module
 ----------------------------------
 
 .. automodule:: tomotok.core.inversions.mfr
-    :members:
-    :undoc-members:
-    :show-inheritance:
-    :special-members: __call__
-
-
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `tomotok-1.2.2/docs/source/api/tomotok.core.io.rst` & `tomotok-1.3/docs/source/api/tomotok.core.io.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 tomotok.core.io package
 =======================
 
 .. automodule:: tomotok.core.io
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 Submodules
 ----------
 
 tomotok.core.io.diag module
 ---------------------------
 
 .. automodule:: tomotok.core.io.diag
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.io.support module
 ------------------------------
 
 .. automodule:: tomotok.core.io.support
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.io.tokamaks module
 -------------------------------
 
 .. automodule:: tomotok.core.io.tokamaks
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
-
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `tomotok-1.2.2/docs/source/api/tomotok.core.rst` & `tomotok-1.3/docs/source/api/tomotok.core.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 tomotok.core package
 ====================
 
 .. automodule:: tomotok.core
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 Subpackages
 -----------
 
 .. toctree::
+   :maxdepth: 4
 
-    tomotok.core.geometry
-    tomotok.core.inversions
-    tomotok.core.io
-    tomotok.core.tools
+   tomotok.core.geometry
+   tomotok.core.inversions
+   tomotok.core.io
+   tomotok.core.tools
 
 Submodules
 ----------
 
 tomotok.core.derivative module
 ------------------------------
 
 .. automodule:: tomotok.core.derivative
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.phantoms module
 ----------------------------
 
 .. automodule:: tomotok.core.phantoms
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
-
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `tomotok-1.2.2/docs/source/api/tomotok.core.tools.rst` & `tomotok-1.3/docs/source/api/tomotok.core.tools.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 tomotok.core.tools package
 ==========================
 
 .. automodule:: tomotok.core.tools
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 Submodules
 ----------
 
 tomotok.core.tools.checkers module
 ----------------------------------
 
 .. automodule:: tomotok.core.tools.checkers
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.tools.data module
 ------------------------------
 
 .. automodule:: tomotok.core.tools.data
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.tools.gifmaker module
 ----------------------------------
 
 .. automodule:: tomotok.core.tools.gifmaker
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+tomotok.core.tools.hdf module
+-----------------------------
+
+.. automodule:: tomotok.core.tools.hdf
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.tools.postproc module
 ----------------------------------
 
 .. automodule:: tomotok.core.tools.postproc
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.core.tools.projection module
 ------------------------------------
 
 .. automodule:: tomotok.core.tools.projection
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
-
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `tomotok-1.2.2/docs/source/api/tomotok.gui.rst` & `tomotok-1.3/docs/source/api/tomotok.gui.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,66 @@
 tomotok.gui package
 ===================
 
 .. automodule:: tomotok.gui
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 Submodules
 ----------
 
 tomotok.gui.apps module
 -----------------------
 
 .. automodule:: tomotok.gui.apps
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.gui.menus module
 ------------------------
 
 .. automodule:: tomotok.gui.menus
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.gui.merfer module
 -------------------------
 
 .. automodule:: tomotok.gui.merfer
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.gui.profiler module
 ---------------------------
 
 .. automodule:: tomotok.gui.profiler
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.gui.roi module
 ----------------------
 
 .. automodule:: tomotok.gui.roi
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.gui.widgets module
 --------------------------
 
 .. automodule:: tomotok.gui.widgets
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 tomotok.gui.widgets\_tomo module
 --------------------------------
 
 .. automodule:: tomotok.gui.widgets_tomo
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
-
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `tomotok-1.2.2/docs/source/auxilia/tools.rst` & `tomotok-1.3/docs/source/auxilia/tools.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 Tools
 =====
 
-Simple functions complementing the core functionalities. Includes post processing and visualisations.
+Utilities complementing the core functionalities. Includes post-processing and visualizations.
+
+
+HDF interface
+-------------
+
+.. automodule:: tomotok.core.tools.hdf
+    :members:
+    :undoc-members:
+    :noindex:
+
 
 Post Processing
 ---------------
 Processing of tomography results. Planned to be expanded. Currently only power computation implemented.
 
-.. automodule :: tomotok.core.tools.postproc
+.. automodule:: tomotok.core.tools.postproc
     :members: compute_power
     :noindex:
 
+
 Projection space
 ----------------
-Transforms lines of sights into projections space parametrisation.
+Transforms lines of sights into projections space parametrization.
 
 .. automodule:: tomotok.core.tools.projection
     :members: projection_space
     :undoc-members:
     :noindex:
```

### Comparing `tomotok-1.2.2/docs/source/conf.py` & `tomotok-1.3/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
     'sphinx.ext.todo',
     'sphinx.ext.mathjax',
     'sphinx.ext.githubpages',
+    # 'sphinx.ext.napoleon',
     'numpydoc',
     # 'sphinx_markdown_builder',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
@@ -92,14 +93,25 @@
 # Else, today_fmt is used as the format for a strftime call.
 #today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = []
 
+# Definition of extension options
+# Autodoc
+autodoc_default_options = {
+    'members' : True,
+    'special-members' : '__call__',
+    }
+
+# numpydoc
+numpydoc_show_inherited_class_members = False
+numpydoc_class_members_toctree = False
+
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
 #default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 #add_function_parentheses = True
 
@@ -288,15 +300,15 @@
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (master_doc, 'tomotok', 'tomotok Documentation',
-     author, 'tomotok', 'One line description of project.',
+     author, 'tomotok', 'Algorithms for tomography of tokamak plasma radiation.',
      'Miscellaneous'),
 ]
 
 # Documents to append as an appendix to all manuals.
 #texinfo_appendices = []
 
 # If false, no module index is generated.
@@ -306,8 +318,11 @@
 #texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 #texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+intersphinx_mapping = {'python': ('https://docs.python.org/3', None),
+                       'numpy': ('https://numpy.org/doc/stable/', None),
+                       'scipy': ('https://docs.scipy.org/doc/scipy/', None),
+                       'matplotlib': ('https://matplotlib.org/stable/', None)}
```

### Comparing `tomotok-1.2.2/docs/source/glossary.rst` & `tomotok-1.3/docs/source/glossary.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,33 +3,40 @@
 
 Terminology
 -----------
 
 .. glossary::
 
     detector
-        a piece of hardware that changes incident photons to signal, can consist of several sensitive segments or channels (e.g. photodiode array) \\
+        a piece of hardware that changes incident photons to signal, can consist of several sensitive segments or channels (e.g. photodiode array)
+
     pixel
     channel
         one sensitive unit in detector, one unit in recorded signal
+
     reconstruction plane 
         a plane that is either observed by detectors or lines of sights are transformed to it, usually poloidal cut is used for tokamaks
+
     node
     voxel
         one segment in reconstruction plane described by a local basis function
+
     camera
         enclosure for detector defining view and ensuring survival of detector (shielding, cooling...)
+
     line of sight
     chord
         line approximating area that given detector channel can observe
 
 Shortcuts
 ---------
 
 .. glossary::
 
     MFR
         Minimum Fisher Regularisation
+
     LAME
         Linear Algebraic Methods
+
     BOB
-        Biorthogonal Basis Decomposition
+        Biorthogonal Basis Decomposition
```

### Comparing `tomotok-1.2.2/docs/source/gui/gui.rst` & `tomotok-1.3/docs/source/gui/gui.rst`

 * *Files 11% similar despite different names*

```diff
@@ -9,10 +9,18 @@
 
 GUI consist of widgets that are controlled by objects called Applications. Currently, there are two types, one that tries to load from a predefined local database the other allow user to specify a location of hdf file. They might need to redirect standard output and should be launched using special convenience function launcher.
 
 The application consist of menu widgets and after data were loaded, it can be used to creates other widget windows for displaying the results.
 
 Widgets could be categorized according to they purpose. There are general purpose widgets that enhance the application, widgets for data visualisation and also widgets that apart from visualisation can also process the data. For description of the displaying and processing methods for multiple reconstructions see [G1]_.
 
+.. toctree::
+    :caption: Categories
+    :maxdepth: 1
+
+    apps
+    tomo
+    common
+
 .. rubric:: References
 
 .. [G1] J. Svoboda, et al. "Comparative analysis and new post-processing methods for plasma tomography at tokamaks." Journal of Instrumentation 14.11 (2019): C11001.
```

### Comparing `tomotok-1.2.2/docs/source/gui/tomo.rst` & `tomotok-1.3/docs/source/gui/tomo.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Tomography widgets
 ==================
 
 Used for displaying or processing results [G1]_. 
 
-.. [G1] J. Svoboda, et al. "Comparative analysis and new post-processing methods for plasma tomography at tokamaks." Journal of Instrumentation 14.11 (2019): C11001.
-
 Displaying
 ----------
-A basic window capable of displaying a single reconstruction DiagGraphWindow. Can load a sequence of reconstructions and be synchronized with other windows.  
+A basic window capable of displaying a single reconstruction DiagGraphWindow. Can load a sequence of reconstructions and be synchronized with other windows. 
+
+.. automodule:: tomotok.gui.widgets_tomo
+    :members:
+    :undoc-members:
+    :show-inheritance:
+    :noindex:
+
 
 Processing
 ----------
 
 .. automodule:: tomotok.gui.roi
     :members: GraphRectangles, GraphContours
     :undoc-members:
```

### Comparing `tomotok-1.2.2/docs/source/index.rst` & `tomotok-1.3/docs/source/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
    install
    inversions/inversions
    auxilia/auxilia
    gui/gui
    glossary
 
 .. toctree::
+   :numbered:
    :caption: Api Doc
 
    api/tomotok.core
    api/tomotok.gui
 
 Indices and tables
 ------------------
```

### Comparing `tomotok-1.2.2/docs/source/inversions/bob.rst` & `tomotok-1.3/docs/source/inversions/bob.rst`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/docs/source/inversions/inversions.rst` & `tomotok-1.3/docs/source/inversions/inversions.rst`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/docs/source/inversions/lame.rst` & `tomotok-1.3/docs/source/inversions/lame.rst`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/docs/source/inversions/mfr.rst` & `tomotok-1.3/docs/source/inversions/mfr.rst`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/docs/source/licence.rst` & `tomotok-1.3/docs/source/licence.rst`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/docs/source/welcome.rst` & `tomotok-1.3/docs/source/welcome.rst`

 * *Files 12% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 * Ondrej Ficker (algorithms, math)
 * Martin Imrisek (algorithms, coding)
 
 Citations
 ---------
 If used for a scientific publication, please cite the software using the references below together with references for inversion methods used. These can be found in section :doc:`inversions/inversions`.
 
-"J. Svoboda, J. Cavalier, O.Ficker, M. Imrisek, J. Mlynar and M. Hron, *Tomotok: python package for tomography of tokamak plasma radiation*, 4th ECPD Conference (2021), Journal of Instrumentation"
+"J. Svoboda, J. Cavalier, O. Ficker, M. Imríšek, J. Mlynář and M. Hron, Tomotok: python package for tomography of tokamak plasma radiation, Journal of Instrumentation 16.12 (2021): C12015." `DOI 10.1088/1748-0221/16/12/C12015 <http://doi.org/10.1088/1748-0221/16/12/c12015>`_
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tomotok-1.2.2/setup.py` & `tomotok-1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     version = version_file.read().strip()
 
 setup(
     name='tomotok',
     version=version,
     license='EUPL 1.2',
     author='Jakub Svoboda, Jordan Cavalier, Ondrej Ficker, Martin Imrisek et al.',
-    # author_email='svoboda@ipp.cas.cz',
+    author_email='svoboda@ipp.cas.cz',
     description='Collection of algorithms used for tokamak plasma tomography',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    # url='',
+    url='https://github.com/tomotok/core',
     packages=find_packages(),
     namespace_packages=['tomotok'],
     include_package_data=True,
     python_requires='>=3.5',
     install_requires=['numpy>=1.13.3', 'scipy>=1.1.0', 'matplotlib>=2.2.2', 'h5py>=2.7.1'],
 )
```

### Comparing `tomotok-1.2.2/tomotok/core/geometry/__init__.py` & `tomotok-1.3/tomotok/core/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/core/geometry/analytical.py` & `tomotok-1.3/tomotok/core/geometry/analytical.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/core/geometry/grids.py` & `tomotok-1.3/tomotok/core/geometry/grids.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Licensed under the EUPL-1.2 or later.
 """
 Contains class describing regularly spaced node grid
 """
 from typing import Tuple
 
 import numpy as np
-from matplotlib.path import Path
+from matplotlib.path import Path as MplPath
 
 
 class RegularGrid(object):
     """
     Rectangular grid of regularly spaced rectangles of same size
 
     Describes rectangular reconstruction grid consisting of regularly spaced toroidally symmetric nodes
@@ -123,15 +123,15 @@
     def __repr__(self):
         msg = 'Node grid with resolution {}h{}'.format(self.nr, self.nz)
         msg += ' and bounds ({};{})r, ({};{})z.'.format(*self.extent)
         return msg
 
     def is_inside(self, r: np.ndarray, z: np.ndarray) -> np.ndarray:
         """
-        Determines whether node centers are inside given polygon.
+        Selects nodes with centers inside given polygon.
 
         Parameters
         ----------
         r, z : numpy.ndarray
             Coordinate vectors of polygon
 
         Returns
@@ -139,18 +139,49 @@
         numpy.ndarray
             Mask matrix for pixgrid with True values for nodes inside polygon
         """
         rm, zm = np.meshgrid(self.r_center, self.z_center)
         rm, zm = rm.flatten(), zm.flatten()
         points = np.stack((rm, zm), axis=1)
         limiter_coords = np.stack((r, z), axis=1)
-        p = Path(limiter_coords)
+        p = MplPath(limiter_coords)
         grid_points = p.contains_points(points)
         inside = grid_points.reshape(self.shape)
         return inside
+    
+    def is_inside_any(self, r: np.ndarray, z: np.ndarray) -> np.ndarray:
+        """
+        Selects nodes with at least one corner inside given polygon.
+
+        Parameters
+        ----------
+        r, z : numpy.ndarray
+            Coordinate vectors of polygon
+
+        Returns
+        -------
+        numpy.ndarray
+            Mask matrix for pixgrid with True values for nodes inside polygon
+        """
+        rm, zm = np.meshgrid(self.r_border, self.z_border)
+        rm, zm = rm.flatten(), zm.flatten()
+        points = np.stack((rm, zm), axis=1)
+        limiter_coords = np.stack((r, z), axis=1)
+        p = MplPath(limiter_coords)
+        corners = p.contains_points(points)
+        corners = corners.reshape((self.nz+1, self.nr+1))
+        inside = np.zeros(self.shape, dtype=bool)
+        for i in range(self.nz):
+            for j in range(self.nr):
+                bl = corners[i, j]
+                br = corners[i, j+1]
+                tl = corners[i+1, j]
+                tr = corners[i+1, j+1]
+                inside[i, j] = any([bl, br, tl, tr])
+        return inside
 
     def corners(self, mask: np.ndarray=None) -> np.ndarray:
         """
         Creates an array with r, z coordinates of node corners. 
         
         Corners are in clockwise order starting with top left corner.
```

### Comparing `tomotok-1.2.2/tomotok/core/geometry/handler.py` & `tomotok-1.3/tomotok/core/geometry/handler.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/core/geometry/io.py` & `tomotok-1.3/tomotok/core/geometry/io.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/core/geometry/los.py` & `tomotok-1.3/tomotok/core/geometry/los.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     ----------
     points : numpy.ndarray 
         3D coordinates of points to be rotated with shape (#points, 3)
     angle : float
         angle of rotation in radians
 
     Returns
-    --------
+    -------
     numpy.ndarray
         array of rotated points
     """
     s = np.sin(angle)
     c = np.cos(angle)
     mat = np.array(((c, 0, s),
                     (0, 1, 0),
@@ -129,22 +129,22 @@
 
 
 def rot_h(points, angle):
     """
     Rotates given points in horizontal direction, that is about vertical axis z.
 
     Parameters
-    -----------
+    ----------
     points : numpy.ndarray 
         3D coordinates of points to be rotated with shape (#points, 3)
     angle : float
         angle of rotation in radians
 
     Returns
-    --------
+    -------
     numpy.ndarray
         array of rotated points
     """
     s = np.sin(angle)
     c = np.cos(angle)
     mat = np.array(((c, s, 0),
                     (-s, c, 0),
```

### Comparing `tomotok-1.2.2/tomotok/core/inversions/bob.py` & `tomotok-1.3/tomotok/core/inversions/bob.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,30 +6,35 @@
 It is a simplified form of wavelet-vaguelette decomposition algorithm by R. Nguyen van Yen
 
 .. [BOB1] Jordan Cavalier et al., Nucl. Fusion 59 (2019): 056025
 .. [BOB2] R. Nguyen van Yen et al., Nucl. Fusion 52 (2011): 013005
 """
 import warnings
 
+import h5py
 import numpy as np
 import scipy.sparse as sparse
 
+from tomotok.core.tools.hdf import sparse_to_hdf, hdf_to_sparse
+
 
 class Bob(object):
     """
     BiOrthogonal Basis decomposition
 
     Attributes
     ----------
-    basis : array_like
+    basis : scipy.sparse.dia_matrix
         :math:`\mathbf{b}_i` basis vectors of reconstruction plane
     dec_mat : scipy.sparse.csr_matrix
         :math:`\hat{\mathbf{e}}_i` decomposed matrix used to transform image into reconstruction plane
     dec_mat_normed : scipy.sparse.csr_matrix
-        normalised decomposed matrix
+        normalised decomposed matrix, deprecated v1.3
+    norms : numpy.ndarray
+        node norms used in thresholding
     """
 
     def __init__(self, dec_mat=None, basis=None):
         """
         Parameters
         ----------
         dec_mat : scipy.sparse.csr_matrix, optional
@@ -37,15 +42,15 @@
         basis : array_like, optional
             A set of basis vectors used for decomposition
         """
         # TODO one parameter holding both dec_mat and basis?
         super().__init__()
         self.basis = basis
         self.dec_mat = dec_mat
-        self.dec_mat_normed = None
+        self.norms = None
         return
 
     def decompose(self, gmat, basis, reg_factor=0, solver_kw: dict=None):
         """
         Decomposes the geometry matrix using basis vectors
 
         Parameters
@@ -60,22 +65,22 @@
         solver_kw : dict
             keyword parameters passed to the solver function
         """
         solver_kw = solver_kw or {}
         if gmat.shape[0] < gmat.shape[1]:
             warnings.warn('Biorthogonal algorithm requires more lines of sights than nodes in reconstruction plane to run reliably')
         self.basis = basis
-        image_base = gmat.dot(self.basis)  # e_i previously known as chi, gmat in basis
-        a = image_base.T.dot(image_base).toarray()  # symmetrized geometry matrix in basis
+        image_base = gmat @ self.basis  # e_i previously known as chi, gmat in basis
+        a = (image_base.T @ image_base).toarray()  # symmetrized geometry matrix in basis
         if reg_factor:
             a = a + a.max() * reg_factor * np.eye(*a.shape)
         b = np.eye(gmat.shape[1])
         res = np.linalg.lstsq(a, b, **solver_kw)
         c = sparse.csr_matrix(res[0])  # coefficient matrix
-        self.dec_mat = image_base.dot(c)  # \hat{e}_i previously known as xi, decomposed matrix
+        self.dec_mat = image_base @ c  # \hat{e}_i previously known as xi, decomposed matrix
         return
 
     def __call__(self, data, gmat=None, thresholding=None, **kw):
         """
         Decomposes geometry matrix and projects images
 
         Parameters
@@ -96,35 +101,61 @@
         if thresholding is not None:
             warnings.warn('Thresholding not implemented to call method. Ignoring.')
         if self.dec_mat is None:
             if gmat is None:
                 raise ValueError('Gmat must be provided for decomposition')
             else:
                 self.decompose(gmat)
-        coeffs = self.dec_mat.T.dot(data)  # coordinates in reconstruction basis
-        res = self.basis.dot(coeffs)  # result in node basis
+        coeffs = self.dec_mat.T @ data  # coordinates in decomposition basis
+        res = self.basis @ coeffs  # result in node basis
         return res
 
-    # TODO remove? remove normalised parameter?
-    def save_decomposition(self, floc, normalised=False):
+    def save_decomposition(self, floc, description=''):
         """
-        Saves 
+        Saves decomposition matrix and basis to hdf file. Norms are also included if calculated.
 
         Parameters
         ----------
         floc : str or pathlib.Path
             file location with name
-        normalised : bool, optional
-            selects whether to save normalised matrix, by default False
+        description : str, optional
+            short user description for file identification
         """
+        if self.dec_mat is None:
+            raise ValueError('Can not save decomposition before it is calculated.')
         floc = str(floc)
-        if normalised:
-            sparse.save_npz(floc, self.dec_mat_normed, compressed=True)
-        else:
-            sparse.save_npz(floc, self.dec_mat, compressed=True)
+        with h5py.File(floc, 'w') as f:
+            f.attrs['version'] = '0.1'
+            f.attrs['description'] = description
+            dec_mat = f.create_group('decomposed_matrix')
+            sparse_to_hdf(self.dec_mat, dec_mat)
+            basis = f.create_group('basis')
+            sparse_to_hdf(self.basis, basis)
+            if self.norms is not None:
+                f.create_dataset('norms', data=self.norms)
+    
+    def load_decomposition(self, floc):
+        """
+        Loads decomposed matrix and basis from an HDF file.
+
+        Norms are loaded only if available in file.
+
+        Parameters
+        ----------
+        floc : str or pathlib.Path
+            location of hdf file with saved decomposition
+        """
+        with h5py.File(floc, 'r') as f:
+            self.dec_mat = hdf_to_sparse(f['decomposed_matrix'])
+            self.basis = hdf_to_sparse(f['basis'])
+            try:
+                self.norms = f['norms'][:]
+            except KeyError:
+                self.norms = None
+        return
 
     def normalise(self, precision=1e-6):
         """
         Computes normalised decomposition matrix.
 
         Parameters
         ----------
@@ -132,19 +163,28 @@
             neglects decomposition matrix rows with lower norm, by default 1e-6
         """
         image_base_adj = self.dec_mat
         kappa = sparse.linalg.norm(image_base_adj, axis=0)
         idx = kappa > precision
         norms = np.zeros(kappa.size)
         norms[idx] = (1 / kappa[idx])
-        xi_norm = image_base_adj.multiply(sparse.csr_matrix(norms))
-        self.dec_mat_normed = xi_norm
+        self.norms = norms[:, None]  # change to expected shape
+
+    @property
+    def dec_mat_normed(self):
+        """
+        .. deprecated :: 1.3
+        """
+        warnings.warn('dec_mat_normed was deprecated in v1.3', DeprecationWarning)
+        if self.norms is None:
+            return None
+        else:
+            return self.dec_mat.multiply(sparse.csr_matrix(self.norms[:, 0]))
+
 
-    # TODO replace image by reconstruction?
-    # TODO return mask only?
     def thresholding(self, image, c: int, precision: float=1e-6, conv: float=1e-9):
         """
         Applies thresholding method to provided image.
 
         Parameters
         ----------
         image : numpy.ndarray
@@ -163,29 +203,32 @@
         Raises
         ------
         RuntimeError
             If thresholding is called before decomposition of geometry matrix
         """
         if self.dec_mat is None:
             raise RuntimeError('Decomposition must be computed prior to thresholding.')
-        if self.dec_mat_normed is None:
+        if self.norms is None:
             self.normalise(precision)
-        temp = sparse.csr_matrix(image)
-        a = np.abs(self.dec_mat_normed.T.dot(temp).toarray())
 
-        threshold_2 = np.sqrt(c**2 / a.size * a.T.dot(a))
+        # calculate plane basis coefficients
+        coeffs = self.dec_mat.T @ image
+
+        # thresholding loop
+        a = np.abs(coeffs * self.norms)  # normalised coefficients
+        threshold_2 = np.sqrt(c**2 / a.size * a.T @ a)
         threshold_1 = 0
         while np.abs(threshold_1-threshold_2) >= conv:
             threshold_1 = threshold_2
             a_temp = a[a <= threshold_1]
-            threshold_2 = np.sqrt(c**2 / a_temp.size * a_temp.T.dot(a_temp))
+            threshold_2 = np.sqrt(c**2 / a_temp.size * a_temp.T @ a_temp)
 
-        out = self.dec_mat.T.dot(image)
-        out = self.basis.dot(out)
-        out[a < threshold_2] = 0
+        # remove plane basis with contributions below threshold and transform to nodes
+        coeffs[a < threshold_2] = 0
+        out = self.basis @ coeffs
         return out
 
 
 class SimpleBob(Bob):
     """
     Automatically creates simple one node basis as an sparse identity matrix
 
@@ -211,23 +254,23 @@
     def decompose(self, gmat, basis, reg_factor=0, solver_kw=None):
         if solver_kw is not None:
             raise TypeError('scipy.sparse.linalg.inv does not take any keywords')
         if gmat.shape[0] < gmat.shape[1]:
             warnings.warn('Biorthogonal algorithm requires more '
             'lines of sights than nodes in reconstruction plane to run reliably')
         self.basis = basis
-        image_base = gmat.dot(self.basis)  # chi
-        a = image_base.T.dot(image_base)
+        image_base = gmat @ self.basis  # chi
+        a = image_base.T @ image_base
         if reg_factor:
             a = a + a.max() * reg_factor * sparse.eye(*a.shape)
         try:
             c = sparse.linalg.inv(a)
         except RuntimeError:
             raise ValueError('Singular symmetrized matrix factor. Try increasing regularisation factor.')
-        self.dec_mat = image_base.dot(c)  # xi
+        self.dec_mat = image_base @ c  # xi
         return
 
 
 class CholmodBob(Bob):
     """
     Decomposition optimized for sparse matrices using Cholesky decomposition
 
@@ -253,17 +296,17 @@
         """
         solver_kw = solver_kw or {}
         from sksparse.cholmod import cholesky, CholmodNotPositiveDefiniteError
         if gmat.shape[0] < gmat.shape[1]:
             warnings.warn('Biorthogonal algorithm can be prone to failure if there are more '
             'lines of sights than nodes in reconstruction plane')
         self.basis = basis
-        image_base = gmat.dot(self.basis)  # chi
-        a = image_base.T.dot(image_base)
+        image_base = gmat @ self.basis  # chi
+        a = image_base.T @ image_base
         try:
             factor = cholesky(a, a.max()*reg_factor, **solver_kw)
         except CholmodNotPositiveDefiniteError:
             raise ValueError('Symmetrized matrix was not positive definite. Try increasing regularisation factor.')
         b = sparse.csc_matrix(np.eye(gmat.shape[1]))
         c = factor(b)
-        self.dec_mat = image_base.dot(c)  # xi
+        self.dec_mat = image_base @ c  # xi
         return
```

### Comparing `tomotok-1.2.2/tomotok/core/inversions/lame.py` & `tomotok-1.3/tomotok/core/inversions/lame.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/core/inversions/mfr.py` & `tomotok-1.3/tomotok/core/inversions/mfr.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,38 +16,24 @@
 from scipy.sparse.linalg import spsolve
 from scipy.optimize import minimize_scalar
 
 
 class Mfr(object):
     r"""
     Inverses provided data using Minimum Fisher Regularization scheme.
-
-    Attributes
-    ----------
-    last_chi : float
-        person test result of the last computed inversion
-    logalpha : float
-        :math:`\log(\alpha)` logarithm of regularisation parameter
-    gmat : numpy.ndarray
-        geometry matrix with shape (#channels, #nodes)
-    signal : numpy.ndarray
-    gdg : numpy.ndarray
-       :math:`\mathbf{T}^T \cdot \mathbf{T}` symmetrised geometry matrix, shape (#nodes, #nodes)
-    gdsig : numpy.ndarray
-        right side of regularisation scheme :math:`\mathbf{T}^T \cdot \mathbf{f}`
     """
     def __init__(self):
         super().__init__()
         self._gmat = None
         self._signal = None
         self._gdg = None
         self._gdsig = None
 
     @staticmethod
-    def solve(a, b):
+    def invert(a, b):
         r"""
         Finds solution of :math:`\mathbf{Ax}=\mathbf{b}` using scipy.sparse.linalg.spsolve
         """
         return spsolve(a, b)
 
     def _test_regularization(self, logalpha, objective):
         """
@@ -68,145 +54,162 @@
         Returns
         -------
         abs(chi2 - 1) : float
             1D Euclidean distance from ideal Pearson test result
         """
         alpha = 10 ** logalpha
         mod_mat = self._gdg + alpha * objective
-        g = self.solve(mod_mat, self._gdsig)
+        g = self.invert(mod_mat, self._gdsig)
         chi2 = self._pearson_test(g)
         return abs(chi2 - 1)
 
-    def invert(self, signals, gmat, derivatives, w_factor=None, mfi_num=3, bounds=(-15, 0), iter_max=15, w_max=1,
-               aniso=0, tolerance=0.05):
+    def solve(self, signals, gmat, derivatives, derivative_weights=None, w_factor=None, mfi_num=3, bounds=(-15, 0), iter_max=15, w_max=1,
+              tolerance=0.05, zero_negative=False):
         """
-        Inverses normalised signals using `mfi_num` Fisher Information cycles each with 
-        `iter_max` steps of regularisation parameter optimisation.
+        Solves the tomography problem for given normalised signals using 'mfi_num' Fisher Information cycles
+        each with 'iter_max' steps of regularisation parameter optimisation.
 
         See regularisation_matrix documentation for more information about derivative matrix formats.
 
         Parameters
         ----------
         signals : numpy.ndarray
             error normalised signals on detector channels
         gmat : scipy.sparse.csr_matrix
-            geometry matrix normalised by estimated errors
+            geometry matrix normalised by estimated errors, shape (#channels, #nodes)
         derivatives : list
-            list of tuples containing pairs of sparse derivatives matrices
+            list of sparse derivative matrices used to create regularisation matrix
+        derivative_weights : list of float
+            list of weights for individual derivative matrices
         w_factor : numpy.ndarray, optional
             weight matrix multipliers with shape (#nodes, )
         mfi_num : float, optional
             number of MFR iterations
         bounds : tuple of two floats, optional
             exponent values for bounds of regularisation parameter alpha
         iter_max : float, optional
             maximum number of root finding iterations
         w_max : float, optional
             value used in weigh matrix for zero or negative nodes
         aniso : float, optional
             Determines anisotropy of derivative matrices
         tolerance : float, optional
             End MFI loop if residuum reaches interval (1-tolerance; 1+tolerance), by default 0.05
+        zero_negative : bool
+            sets negative values in previous step result to zero when initializing MFI loop
 
         Returns
         -------
         g : numpy.ndarray
             vector with nodes emissivities, shape (#nodes, )
         stats : dict
             inversion statistics
-
-                chi : float
-                    Pearson test value of final result
-                niter : list of int
+                chi : list of float
+                    Pearson test value of each optimization result
+                iter_num : list of int
                     numbers of iterations taken in each MFI loop
-                logalpha : float
-                    logarithm of final regularisation parameter
+                logalpha : list of float
+                    final regularisation parameter logarithm of each MFI loop
 
         See Also
         --------
         regularisation_matrix
         """
         ela = time.time()
         self._signal = signals
         self._gmat = gmat
-        self._gdg = gmat.T.dot(gmat)
-        self._gdsig = gmat.T.dot(signals)
-        npix = gmat.shape[1]
-        g = np.ones(npix)
+        self._gdg = gmat.T @ gmat
+        self._gdsig = gmat.T @ signals
+        g = np.ones(gmat.shape[1])
         mfi_count = 0
-        niter = []
+        iter_nums = []
+        alphas = []
+        chis = []
         while mfi_count < mfi_num:
             # MFI loop searching for ideal value of regularisation parameter
             w = 1 / g
             w[w < 0] = w_max
             w = sparse.diags(w)
             if w_factor is not None:
                 w = w * sparse.diags(w_factor)
-            objective = self.regularisation_matrix(derivatives, w, aniso)
-            res = minimize_scalar(self._test_regularization,
-                                  method='bounded',
-                                  bounds=bounds,
-                                  args=objective,
-                                  options={'maxiter': iter_max, 'xatol': tolerance},
-                                  )
-            if res.status == 1:
-                warn('Maximum number of iteration in MFI loop reached. Consider increasing iter_max.')
-            niter.append(res.nfev)
-            # TODO write custom optimisation routine to avoid recalculating optimal solution?
-            m = self._gdg + 10 ** res.x * objective
-            g = self.solve(m, self._gdsig)
+            if zero_negative:
+                g[g < 0] = 0
+            regularisation, stats = self.determine_regularisation(
+                derivatives,
+                w,
+                derivative_weights,
+                bounds,
+                iter_max,
+                tolerance
+            )
+            iter_nums.append(stats['iter_num'])
+            alphas.append(stats['logalpha'])
+            m = self._gdg + regularisation
+            g = self.invert(m, self._gdsig)
+            chi_sq = self._pearson_test(g)
+            chis.append(chi_sq)
             mfi_count += 1
-        logalpha = res.x
-        last_chi = self._pearson_test(g)
+        # logalpha = res.x
         ela = time.time() - ela
-        print('last chi^2 = {:.4f}, time: {:.2f} s'.format(last_chi, ela))
-        stats = dict(chi=last_chi, logalpha=logalpha, niter=niter)
+        stats = dict(chi=chis, logalpha=alphas, iter_num=iter_nums, elapsed=ela)
         return g, stats
 
-    def smoothing_mat(self, w, derivatives, danis):
+    def determine_regularisation(self, derivatives, w, derivative_weights, bounds, iter_max, tolerance):
         """
-        .. deprecated :: 1.1
-            Use :meth:`regularisation_matrix`  
+        Uses minimize scalar function from scipy to iteratively minimize chi square (Pearson test).
         """
-        warn('Smoothing_mat deprecated by regularisation_matrix method since v1.1.', DeprecationWarning)
-        self.regularisation_matrix(derivatives, w, danis)
+        stats = dict()
+        objective = self.regularisation_matrix(derivatives, w, derivative_weights)
+        # TODO write custom optimisation routine to avoid recalculating optimal solution to get chi sq
+        res = minimize_scalar(
+            self._test_regularization,
+            method='bounded',
+            bounds=bounds,
+            args=objective,
+            options={'maxiter': iter_max, 'xatol': tolerance},
+        )
+        if res.status == 1:
+            warn('Maximum number of iteration in MFI loop reached. Consider increasing iter_max.')
+        stats['iter_num'] = res.nfev
+        stats['logalpha'] = res.x
+        regularisation = 10**res.x * objective
+        return regularisation, stats
 
-    def regularisation_matrix(self, derivatives, w, aniso=0):
+    def regularisation_matrix(self, derivatives, weights, derivative_weights=None):
         """
         Computes nonlinear regularisation matrix from provided derivative matrices and node weight factors 
         determined by emissivity from previous iteration of the inversion loop.
         
-        Anisotropic coefficients are computed using sigmoid function.
-
-        Multiple pairs of derivatives matrices computed by different numerical scheme can be used. Each pair should
-        contain derivatives in each locally orthogonal direction.
+        Multiple derivative matrices can be used allowing to combine matrices computed by 
+        different numerical schemes. 
+        
+        Each matrix can have different weight assigned to introduce anisotropy.
 
         Parameters
         ----------
-        w : scipy.sparse.dia.dia_matrix
-            (#nodes, #nodes) diagonal matrix with pixel weight factors
-        derivatives : list of scipy.sparse.csc_matrix pairs
-            contains sparse derivative matrices, each pair contains derivatives in both locally orthogonal coordinates
-        aniso : float
-            anistropic factor, positive values make derivatives along first coordinate more significant
+        derivatives : list of scipy sparse matrix
+            a list of derivative matrices, with shape (# nodes, # nodes) 
+        weights : scipy.sparse.dia_matrix
+            node weight factors, (#nodes, #nodes) 
+        weight_coefficients : list of float
+            allows to specify anisotropy by assign weights for each matrix
 
         Returns
         -------
         scipy.sparse.csc_matrix
         """
-        # sigmoid function
-        w1 = 1 / (1 + np.exp(-aniso))
-        w2 = 1 / (1 + np.exp(aniso))
-        h1 = 0
-        h2 = 0
-        for pair in derivatives:
-            h1 = h1 + pair[0].T.dot(w).dot(pair[0])
-            h2 = h2 + pair[1].T.dot(w).dot(pair[1])
-        smooth = w1 * h1 + w2 * h2
-        return smooth
+        if isinstance(derivatives, sparse.spmatrix):
+            derivatives = [derivatives]
+        if derivative_weights is None:
+            derivative_weights = [1] * len(derivatives)
+        total = sum(derivative_weights)
+        regularisation = sparse.csr_matrix(derivatives[0].shape)
+        for dw, dmat in zip(derivative_weights, derivatives):
+            regularisation += dw / total * dmat.T @ weights @ dmat
+        return regularisation
 
     def _pearson_test(self, g):
         r"""
         Computes retrofit and residuum :math:`\chi^2` using pearson test
 
         .. math ::
             \chi^2 = \frac{1}{M} \sum_{i}^{M} \left(\tilde{\mathbf{f}} - \tilde{\mathbf{T}} \cdot \mathbf{g} \right)_i^2
@@ -219,16 +222,16 @@
         Returns
         -------
         float
         """
         retrofit = self._gmat.dot(g)
         misfit = retrofit - self._signal
         misfit_sq = np.power(misfit, 2)
-        res = np.average(misfit_sq)
-        return res
+        self._chisq = np.average(misfit_sq)
+        return self._chisq
 
     def __call__(self, data, gmat, derivatives, errors, **kwargs):
         """
         Normalises signal and geometry matrix using estimated errors of measurement and
         then executes a sequence of MFR reconstructions.
 
         Parameters
@@ -238,33 +241,27 @@
         gmat : sparse.csr_matrix
             shape (#channels, #nodes)
         derivatives : list
             list of tuples with derivative matrix pairs
         errors : int, float or np.ndarray
             Can have shapes (#channels, ), (#time slices,) or (#time slices, #channels)
         **kwargs : dict
-            keywords passed to invert method
+            keywords passed to solve method
         
         Returns
         -------
         res : numpy.ndarray
             tomographic reconstruction, with shape (#time slices, #nodes)
         stats_list : list of dicts
-            contains dicts with inversion statistics returned by invert method
+            contains dicts with inversion statistics returned by solve method
         
         See also
         --------
-        invert
+        solve
         """
-        try:
-            kwargs['aniso'] = kwargs.pop('danis')
-            warn('Parameter `danis` renamed to `aniso` since v1.1', DeprecationWarning)
-        except KeyError:
-            pass
-
         data_ndim = np.ndim(data)
         if data_ndim == 0:
             raise ValueError('Data must be at least an 1D array of values.')
         elif data_ndim == 1:  # flat data, assume one time slice
             data = data.reshape(1, -1)
         elif data_ndim > 2:
             raise ValueError('Data array has too many dimension: {}. Max is 2.'.format(data_ndim))
@@ -300,15 +297,15 @@
         res = np.empty((nslices, nnodes))
         stats_list = []
 
         for i in range(nslices):
             signal_np = signal_nrm[i, :]
             error_sp = sparse.diags(1/errors[i, :])
             gmat_nrm = error_sp.dot(gmat)
-            res[i], stats = self.invert(signal_np, gmat_nrm, derivatives, **kwargs)
+            res[i], stats = self.solve(signal_np, gmat_nrm, derivatives, **kwargs)
             stats_list.append(stats)
 
         return res, stats_list
 
 
 class CholmodMfr(Mfr):
     """
@@ -321,15 +318,15 @@
         """
         Executes standard initialization and imports sksparse.cholmod
         """
         super().__init__()
         from sksparse.cholmod import cholesky
         self.cholesky = cholesky
 
-    def solve(self, a, b):
+    def invert(self, a, b):
         r"""
         Finds solution of :math:`\mathbf{Ax}=\mathbf{b}` using sksparse.cholmod.cholesky
 
         Parameters
         ----------
         a : scipy.sparse.csr_matrix
             square and positive definite matrix
```

### Comparing `tomotok-1.2.2/tomotok/core/inversions/tikhonov.py` & `tomotok-1.3/tomotok/core/inversions/fixed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # Copyright 2021 Institute of Plasma Physics of the Czech Academy of Sciences. 
 #
 # Licensed under the EUPL-1.2 or later.
 """
-Implementation of Phillips-Tikhonov regularisation scheme
+Fixed parameter Tikhonov scheme with MFR like regularisation matrix
 """
-
 import time
+from warnings import warn
 
 import numpy as np
 import scipy.sparse as sparse
 from scipy.sparse.linalg import spsolve
-from scipy.optimize import minimize_scalar
 
+from .mfr import Mfr, CholmodMfr
 
-class Tikhonov(object):
+class Fixt(Mfr):
     r"""
-    Template class that implements Phillips-Tikhonov regularisation scheme.
-    
-    Does not implement any method for obtaining regularisation matrix nor inversion run
+    Inverses provided data using fixed parameter value Minimum Fisher Regularization scheme.
 
     Attributes
     ----------
     last_chi : float
         person test result of the last computed inversion
     logalpha : float
         :math:`\log(\alpha)` logarithm of regularisation parameter
@@ -31,195 +29,202 @@
     gdg : numpy.ndarray
        :math:`\mathbf{T}^T \cdot \mathbf{T}` symmetrised geometry matrix, shape (#nodes, #nodes)
     gdsig : numpy.ndarray
         right side of regularisation scheme :math:`\mathbf{T}^T \cdot \mathbf{f}`
     """
     def __init__(self):
         super().__init__()
-        self.last_chi = None
-        self.logalpha = None
-        self.gmat = None
-        self.signal = None
-        self.gdg = None
-        self.gdsig = None
-
-    @staticmethod
-    def solve(a, b):
-        r"""
-        Finds solution of :math:`\mathbf{Ax}=\mathbf{b}` using scipy.sparse.linalg.spsolve
-        """
-        return spsolve(a, b)
+        self._gmat = None
+        self._signal = None
+        self._gdg = None
+        self._gdsig = None
 
-    def invert(self, signals, gmat, derivatives, w_factor=None, mfi_num=3, bounds=(-15, 0), iter_max=10, w_max=1,
-               aniso=0):
+    def solve(self, signals, gmat, derivatives, parameters, derivative_weights=None, 
+              w_factor=None, mfi_num=3, w_max=1, zero_negative=False):
         """
-        Inverses normalised signals using `mfi_num` Fisher Information cycles each with `iter_max` steps of regularisation parameter optimisation.
+        Inverses normalised signals using fixed value of regularisation parameter.
 
-        See smoothing_mat documentation for more information about derivative matrix formats.
+        See regularisation_matrix documentation for more information about derivative matrix formats.
 
         Parameters
         ----------
         signals : numpy.ndarray
             error normalised signals on detector channels
         gmat : scipy.sparse.csr_matrix
             geometry matrix normalised by estimated errors
         derivatives : list
             list of tuples containing pairs of sparse derivatives matrices
+        parameters : float or list of float
+            regularisation parameter value(s), list length must match mfi_num
         w_factor : numpy.ndarray, optional
             weight matrix multipliers with shape (#nodes, )
-        mfi_num : float, optional
-            number of MFR iterations
-        bounds : tuple of two floats, optional
-            exponent values for bounds of regularisation parameter alpha
-        iter_max : float, optional
-            maximum number of root finding iterations
         w_max : float, optional
             value used in weigh matrix for zero or negative nodes
-        aniso : float
-            Determines anisotropy of derivative matrices, passed to sigmoid function
+        aniso : float, optional
+            Determines anisotropy of derivative matrices
 
         Returns
         -------
-        numpy.ndarray
+        g : numpy.ndarray
             vector with nodes emissivities, shape (#nodes, )
-        
+        stats : dict
+            inversion statistics
+
+                chi : float
+                    Pearson test value of final result
+                niter : list of int
+                    numbers of iterations taken in each MFI loop
+                logalpha : float
+                    logarithm of final regularisation parameter
 
         See Also
         --------
-        smoothing_mat
+        regularisation_matrix
         """
+        if isinstance(parameters, float):
+            parameters = mfi_num * [parameters]
+        elif len(parameters) != mfi_num:
+            msg = 'Different number of regularisation parameters: {} and MFI loops: {}.'
+            raise ValueError(msg.format(len(parameters), mfi_num))
         ela = time.time()
-        self.signal = signals
-        self.gmat = gmat
-        self.gdg = gmat.T.dot(gmat)
-        self.gdsig = gmat.T.dot(signals)
-        npix = gmat.shape[1]
-        g = np.ones(npix)
-        mfi_count = 0
-        while mfi_count < mfi_num:
+        self._signal = signals
+        self._gmat = gmat
+        self._gdg = gmat.T @ gmat
+        self._gdsig = gmat.T @ signals
+        g = np.ones(gmat.shape[1])
+        mfi_counter = 0
+        chis = []
+        while mfi_counter < mfi_num:
+            # MFI loop searching for ideal value of regularisation parameter
             w = 1 / g
             w[w < 0] = w_max
             w = sparse.diags(w)
             if w_factor is not None:
                 w = w * sparse.diags(w_factor)
-            objective = self.smoothing_mat(w, derivatives, aniso)
-            res = minimize_scalar(self.test_regularization,
-                                  method='bounded',
-                                  bounds=bounds,
-                                  args=objective,
-                                  options={'maxiter': iter_max},
-                                  )
-            self.logalpha = res.x
-            m = self.gdg + 10 ** res.x * objective
-            g = self.solve(m, self.gdsig)
-            mfi_count += 1
+            if zero_negative:
+                g[g < 0] = 0
+            objective = self.regularisation_matrix(derivatives, w, derivative_weights)
+            m = self._gdg + parameters[mfi_counter] * objective
+            g = self.invert(m, self._gdsig)
+            chi_sq = self._pearson_test(g)
+            chis.append(chi_sq)
+            mfi_counter += 1
+        # logalpha = res.x
         ela = time.time() - ela
-        print('last chi^2 = {:.4f}, time: {:.2f} s'.format(self.last_chi, ela))
-        return g
-
-    def smoothing_mat(self, w, derivatives, aniso):
-        """
-        Computes smoothing matrix from provided derivative matrices and weight factors determined by emissivity from
-        previous iteration of minimisation of Fisher Information.
-
-        Multiple pairs of derivatives matrices computed by different numerical scheme can be used. Each pair should
-        contain derivatives in each locally orthogonal direction.
-
-        Parameters
-        ----------
-        w : scipy.sparse.dia.dia_matrix
-            (#nodes, #nodes) diagonal matrix with pixel weight factors
-        derivatives : list of scipy.sparse.csc_matrix pairs
-            contains sparse derivative matrices, each pair contains derivatives in both locally orthogonal coordinates
-        aniso : float
-            anistropic factor, positive values make derivatives along first coordinate more significant
+        stats = dict(chi=chis, logalpha=parameters, elapsed=ela)
+        return g, stats
 
-        Returns
-        -------
-        smooth
-            smoothing matrix
-        """
-        s1 = 0
-        s2 = 0
-        for pair in derivatives:
-            s1 = s1 + pair[0].T.dot(w).dot(pair[0])
-            s2 = s2 + pair[1].T.dot(w).dot(pair[1])
-        smooth = self.sigmoid(aniso) * s1 + self.sigmoid(-aniso) * s2
-        return smooth
-
-    @staticmethod
-    def sigmoid(x):
-        return 1 / (1 + np.exp(-x))
-
-    def pearson_test(self, g):
-        r"""
-        Computes retrofit and residuum :math:`\chi^2` using pearson test
-
-        .. math ::
-            \chi^2 = \frac{1}{M} \sum_{i}^{M} \left(\tilde{\mathbf{f}} - \tilde{\mathbf{T}} \cdot \mathbf{g} \right)_i^2
-
-        Parameters
-        ----------
-        g : numpy.ndarray
-            vector of tested emissivity
-
-        Returns
-        -------
-        numpy.float64
-        """
-        retrofit = self.gmat.dot(g)
-        misfit = retrofit - self.signal
-        misfit_sq = np.power(misfit, 2)
-        res = np.average(misfit_sq)
-        return res
 
-    def __call__(self, data, gmat, dmats, errors, **kwargs):
+    def __call__(self, data, gmat, derivatives, errors, parameters, **kwargs):
         """
         Normalises signal and geometry matrix using estimated errors of measurement and
         then executes a sequence of MFR reconstructions.
 
         Parameters
         ----------
         data : numpy.ndarray
-            input to be inverted with shape (#time slices, #channels)
+            input to be inverted with shape (#channels,), (#time slices, #channels)
         gmat : sparse.csr_matrix
             shape (#channels, #nodes)
-        dmats : list
+        derivatives : list
             list of tuples with derivative matrix pairs
         errors : int, float or np.ndarray
-            Can have shapes (#channels, ), (#time slices,) or (#tslices, #channels)
+            Can have shapes (#channels, ), (#time slices,) or (#time slices, #channels)
+        parameters : float or list of float
+            regularisation parameter value(s), list length must match mfi_num
+        **kwargs : dict
+            keywords passed to invert method
         
         Returns
         -------
-        res : np.ndarray
+        res : numpy.ndarray
             tomographic reconstruction, with shape (#time slices, #nodes)
-        chi : np.ndarray
-            Pearson test values for final results, shape (#time slices, )
+        stats_list : list of dicts
+            contains dicts with inversion statistics returned by invert method
+        
+        See also
+        --------
+        invert
         """
-        if np.ndim(data) == 1:  # flat data, assume one time slice
+        try:
+            kwargs['aniso'] = kwargs.pop('danis')
+            warn('Parameter `danis` renamed to `aniso` since v1.1', DeprecationWarning)
+        except KeyError:
+            pass
+
+        data_ndim = np.ndim(data)
+        if data_ndim == 0:
+            raise ValueError('Data must be at least an 1D array of values.')
+        elif data_ndim == 1:  # flat data, assume one time slice
             data = data.reshape(1, -1)
+        elif data_ndim > 2:
+            raise ValueError('Data array has too many dimension: {}. Max is 2.'.format(data_ndim))
+
+        if len(gmat.shape) != 2:
+            raise ValueError('Gmat must be a 2D array or matrix')
+
         nslices = data.shape[0]
         nchnls = data.shape[1]
+        if nchnls != gmat.shape[0]:
+            raise ValueError('Different number of channels in data and gmat')
         nnodes = gmat.shape[1]
 
-        if np.ndim(errors) == 1:
+        err_ndim = np.ndim(errors)
+        if err_ndim == 0:  # constant errors
+            errors = np.full_like(data, errors)
+        elif err_ndim == 1:  # flat errors, check for matching shape
             if errors.size == nslices:
                 errors = errors.reshape(-1, 1)
             elif errors.size == nchnls:
                 errors = errors.reshape(1, -1)
             else:
                 raise ValueError('Incompatible shape of errors {} with the data {}'.format(errors.shape, data.shape))
-        
-        errors = errors * np.ones_like(data)
+            errors = errors * np.ones_like(data)  # broadcast to right shape
+        elif err_ndim > 2:
+            raise ValueError('Errors array has too many dimensions.')
+
+        if errors.shape != data.shape:
+            raise ValueError('Data shape {} does not match errors shape {}.'.format(data.shape, errors.shape))
+
         signal_nrm = data / errors
 
         res = np.empty((nslices, nnodes))
-        chi = np.empty(nslices)
+        stats_list = []
 
         for i in range(nslices):
             signal_np = signal_nrm[i, :]
             error_sp = sparse.diags(1/errors[i, :])
             gmat_nrm = error_sp.dot(gmat)
-            res[i] = self.invert(signal_np, gmat_nrm, dmats, **kwargs)
-            chi[i] = self.last_chi
+            res[i], stats = self.solve(signal_np, gmat_nrm, derivatives, parameters, **kwargs)
+            stats_list.append(stats)
 
-        return res, chi
+        return res, stats_list
+
+
+class CholmodFixt(Fixt):
+    """
+    Cholmod version of fixed parameter MFR
+    Requires scikit sparse to be installed in order to initialize properly.
+
+    Uses sksparse.cholmod.cholesky to solve the inversion problem
+    """
+    def __init__(self):
+        """
+        Executes standard initialization and imports sksparse.cholmod
+        """
+        super().__init__()
+        from sksparse.cholmod import cholesky
+        self.cholesky = cholesky
+
+    def invert(self, a, b):
+        r"""
+        Finds solution of :math:`\mathbf{Ax}=\mathbf{b}` using sksparse.cholmod.cholesky
+
+        Parameters
+        ----------
+        a : scipy.sparse.csr_matrix
+            square and positive definite matrix
+        b : array_like
+            right hand side vector
+        """
+        factor = self.cholesky(a)
+        return factor(b)
```

### Comparing `tomotok-1.2.2/tomotok/core/io/diag.py` & `tomotok-1.3/tomotok/core/io/diag.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         Number of rows and columns should be same in all files containing coordinates
 
         Returns
         -------
         xchords, ychords : numpy.ndarray
             arrays with coordinates of chord points with shape (#chords, #points)
         """
-        warnings.warn('Support for LoS saving to txt will be removed. Transfer your coordinates to hdf.', FutureWarning)
+        warnings.warn('Support for LoS saving to txt will be removed. Transfer your coordinates to hdf or json.', FutureWarning)
         geometry_path = self.geometry_path
         ychords = np.zeros((0, 0))
         xchords = np.zeros((0, 0))
         nl = 0
         i = 0
 #        print(geometry_path / 'detector_{}_x.txt'.format(i))
         while (geometry_path / 'detector_{}_x.txt'.format(i)).exists():
@@ -291,19 +291,20 @@
         if not bdr_path.exists():
             print('border coord not found at {}.'.format(bdr_path))
             bdr_path = self.geometry_path.parent / 'border.txt'
             print('Tyring to load from {}'.format(bdr_path))
         bdr = np.loadtxt(str(bdr_path))
         return bdr
 
-    # TODO move to Pixgrid?
     def compute_bd_mat(self, grid, loc=None):
         """
         Simple generation of boundary matrix 1 inside rec area, 0 outside
 
+        .. deprecated:: 1.3.0
+
         Parameters
         ----------
         grid : RegularGrid
 
         Returns
         -------
         boundary_matrix : numpy.ndarray of bool
```

### Comparing `tomotok-1.2.2/tomotok/core/io/support.py` & `tomotok-1.3/tomotok/core/io/support.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/core/io/tokamaks.py` & `tomotok-1.3/tomotok/core/io/tokamaks.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/core/phantoms.py` & `tomotok-1.3/tomotok/core/phantoms.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/core/tools/checkers.py` & `tomotok-1.3/tomotok/core/tools/checkers.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/core/tools/data.py` & `tomotok-1.3/tomotok/core/tools/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,20 @@
         Parameters
         ----------
         data : dict
             [description]
         min_error : float, optional
             [description], by default 0
         """
-        self.chnls = data['chnl']
+        self.chnls = np.array(data['chnl'])
         self.time = data['time']
-        self.data = data['values']
+        if data['values'].shape == (self.time.size, self.chnls.size):
+            self.data = data['values']
+        else:
+            raise ValueError('Wrong shape of values {}. Expected {}'.format(data['values'].shape ,(self.time.size, self.chnls.size)))
         self._original = data.copy()
         self.errors = np.zeros_like(self.data) + min_error
         return
 
     # @property
     # def errors(self):
     #     return self._errors
@@ -262,26 +265,25 @@
         Cuts data to requested interval
 
         Parameters
         ----------
         tlim : tuple
             contains limits of requested time axis
         extend_num : int, optional
-            contains number of points outside tlim for filtering methods
-            (default value is calculated to fit chosen filtering method) <- should be determined by user
+            number of points outside tlim that are added to be used by filtering methods
         """
         if tlim[0] < self.time.min() or self.time.max() < tlim[1]:
-            raise ValueError('Requested time range out of data time vector.')
+            raise ValueError('Requested time range is out of data time vector.')
         t0 = np.searchsorted(self.time, tlim[0])
         t1 = np.searchsorted(self.time, tlim[0], side='right')
         if extend_num is None:
             self.data = self.data[t0:t1, :]
             self.errors = self.errors[t0:t1, :]
         else:
-            raise NotImplementedError('Extension of croping interval was not implemented.')
+            raise NotImplementedError('Extension of cropping interval was not implemented.')
             # FIXME make the method work with data attribute, remove return statement
             # TODO reconsider extend_num
             # ind_t0 = np.where(self.tvec >= tlim[0])[0][0]
             # ind_t1 = np.where(self.tvec <= tlim[1])[0][-1]
             #
             # try:
             #     self.data = self.data[:, ind_t0 - extend_num:ind_t1 + extend_num + 1]
```

### Comparing `tomotok-1.2.2/tomotok/core/tools/gifmaker.py` & `tomotok-1.3/tomotok/core/tools/gifmaker.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/core/tools/postproc.py` & `tomotok-1.3/tomotok/core/tools/postproc.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/core/tools/projection.py` & `tomotok-1.3/tomotok/core/tools/projection.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/gui/apps.py` & `tomotok-1.3/tomotok/gui/apps.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/gui/menus.py` & `tomotok-1.3/tomotok/gui/menus.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/gui/merfer.py` & `tomotok-1.3/tomotok/gui/merfer.py`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tomotok/gui/profiler.py` & `tomotok-1.3/tomotok/gui/profiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,23 @@
 
 from tomotok.core.phantoms import iso_psi
 from .widgets_tomo import GraphRgb
 
 
 class GraphProfiler(GraphRgb):
     """
-    Based on GraphRgb class. Usefull for observing power profile in respect to
-    magentic flux surfaces.
+    A window that can calculate power profile in respect to magnetic flux surfaces.
     
     Parameters
     ----------
     parent : TKInter class parent
         Default is None.
     data : dict
         Contains data, default is empty dict.
-    
-    Keywords
-    --------
-    title : str
+    title : str, optional
         Name of window.
     """
 
     def __init__(self, parent=None, **kw):
         #        tk.Toplevel.__init__(self, parent)
         GraphRgb.__init__(self, parent, **kw)
         if not 'title' in kw:
```

### Comparing `tomotok-1.2.2/tomotok/gui/roi.py` & `tomotok-1.3/tomotok/gui/roi.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,15 @@
     
     Parameters
     ----------
     parent : TKInter class parent
         Default is None.
     data : dict
         Contains data, default is empty dict.
-    
-    Keywords
-    --------
-    title : str
+    title : str, optional
         Name of window.
     """
 
     # TODO axis limits in cm
     def __init__(self, parent=None, **kw):
         #        tk.Toplevel.__init__(self, parent)
         GraphRgb.__init__(self, parent, **kw)
@@ -380,18 +377,15 @@
     
     Parameters
     ----------
     parent : TKInter class parent
         Default is None.
     data : dict
         Contains data, default is empty dict.
-    
-    Keywords
-    --------
-    title : str
+    title : str, optional
         Name of window.
     """
 
     def __init__(self, parent=None, **kw):
         #        tk.Toplevel.__init__(self, parent)
         GraphRgb.__init__(self, parent, **kw)
         if 'title' not in kw:
@@ -475,15 +469,15 @@
 
     def get_levels(self, pnum):
         """
         Gets levels from contour object. If length of levels is one,
         returns array with zero as minimum.
         
         Parameters
-        ---------
+        ----------
         pnum : int
             Number of patch
         
         Returns
         -------
         limits : np.ndarray
             Array with minimum and maximum limited by given contours.
```

### Comparing `tomotok-1.2.2/tomotok/gui/widgets.py` & `tomotok-1.3/tomotok/gui/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,26 +118,21 @@
     By default it consists of listbox with data sequence, frame for buttons,
     canvas for plot and slider for navigation.
     
     Parameters
     ----------
     parent : TKInter widget
         Default is None. Used in GUI interface to specify hierarchy.
-    
-    Keywords
-    --------
-    vals : array-like
+    vals : array-like, optional
         Contains data from time vector to be shown in listbox and
         under slider.
-    
-    slices : int
+    slices : int, optional
         Number of time steps. Use ether vals or slices. Use if no time 
         vector data are available. Creates vals as range(slices).
-    
-    slavechbutton : bool
+    slavechbutton : bool, optional
         Switches whether slave check button will be created. If True a button
         is created, that if unchecked will switch off control from master.
     """
     def __init__(self, parent=None, **kw):
         tk.Toplevel.__init__(self, parent)
         self.bind('<Left>', self.go_prev)
         self.bind('<Right>', self.go_next)
```

### Comparing `tomotok-1.2.2/tomotok/gui/widgets_tomo.py` & `tomotok-1.3/tomotok/gui/widgets_tomo.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,18 +206,15 @@
     
     Parameters
     ----------
     parent : TKInter class parent
         Default is None.
     data : dict
         Contains data, default is empty dict.
-    
-    Keywords
-    --------
-    title : str
+    title : str, optional
         Name of graph window. Is used for saving. Default is 'RGB plot'
     """
 
     def __init__(self, parent=None, data=None, **kw):
         GraphWindow.__init__(self, parent, **kw)
         if data is None:
             data = {}
```

### Comparing `tomotok-1.2.2/tomotok.egg-info/PKG-INFO` & `tomotok-1.3/tomotok.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: tomotok
-Version: 1.2.2
+Version: 1.3
 Summary: Collection of algorithms used for tokamak plasma tomography
+Home-page: https://github.com/tomotok/core
 Author: Jakub Svoboda, Jordan Cavalier, Ondrej Ficker, Martin Imrisek et al.
+Author-email: svoboda@ipp.cas.cz
 License: EUPL 1.2
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 License-File: AUTHORS.txt
 
 # Tomotok
```

### Comparing `tomotok-1.2.2/tomotok.egg-info/SOURCES.txt` & `tomotok-1.3/tomotok.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,26 +51,28 @@
 tomotok/core/geometry/generators.py
 tomotok/core/geometry/grids.py
 tomotok/core/geometry/handler.py
 tomotok/core/geometry/io.py
 tomotok/core/geometry/los.py
 tomotok/core/inversions/__init__.py
 tomotok/core/inversions/bob.py
+tomotok/core/inversions/fixed.py
 tomotok/core/inversions/lame.py
 tomotok/core/inversions/mfr.py
 tomotok/core/inversions/tikhonov.py
 tomotok/core/io/__init__.py
 tomotok/core/io/diag.py
 tomotok/core/io/support.py
 tomotok/core/io/tokamaks.py
 tomotok/core/tests/__init__.py
 tomotok/core/tools/__init__.py
 tomotok/core/tools/checkers.py
 tomotok/core/tools/data.py
 tomotok/core/tools/gifmaker.py
+tomotok/core/tools/hdf.py
 tomotok/core/tools/postproc.py
 tomotok/core/tools/projection.py
 tomotok/gui/__init__.py
 tomotok/gui/apps.py
 tomotok/gui/menus.py
 tomotok/gui/merfer.py
 tomotok/gui/profiler.py
```

### Comparing `tomotok-1.2.2/tutorials/biorthogonal.ipynb` & `tomotok-1.3/tutorials/biorthogonal.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989880952380952%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(1, 'grid = RegularGrid(nr, nz, rlims=(0.2, 0.7), "*

 * *            "zlims=(-0.3, 0.3))\\n'), (2, 'phantom = gauss_iso(grid.nr, grid.nz, cen=0.3, w=0.05) "*

 * *            "* 2000\\n'), (3, 'phantom = np.roll(phantom, (3, -5), (0, 1))  # move the phantom "*

 * *            "from the center of the grid')], delete: [3, 2, 1]}}, 6: {'source': {insert: [(0, "*

 * *            "'pinhole = (0.8, -0.1, 0.2)\\n'), (4, 'axis = (-1, -0.3, -0.3)')], delete: [4, 0]}}, "*

 * *            '29: {\'source\': […]*

```diff
@@ -32,17 +32,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "nr, nz = 50, 60\n",
-                "grid = RegularGrid(nr, nz, (.2, .7), (-.3, .3))\n",
-                "phantom = gauss_iso(grid.nr, grid.nz, cen=.3, w=.05) * 2000\n",
-                "phantom = np.roll(phantom, (3, -5), (0, 1))"
+                "grid = RegularGrid(nr, nz, rlims=(0.2, 0.7), zlims=(-0.3, 0.3))\n",
+                "phantom = gauss_iso(grid.nr, grid.nz, cen=0.3, w=0.05) * 2000\n",
+                "phantom = np.roll(phantom, (3, -5), (0, 1))  # move the phantom from the center of the grid"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -64,19 +64,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pinhole = (.8, -.1, .2)\n",
+                "pinhole = (0.8, -0.1, 0.2)\n",
                 "resolution = (60, 60)\n",
                 "# resolution = (800, 800)  # higher resolutions requires significant amount of memory\n",
                 "fov = (40, 40)\n",
-                "axis = (-1, -.3, -.3)"
+                "axis = (-1, -0.3, -0.3)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -321,15 +321,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# bob.save_decomposition('path/to/decomposed_mat')"
+                "# bob.save_decomposition('path/to/decomposed_mat')\n",
+                "# bob2 = CholmodBob()\n",
+                "# bob2.load_decomposition('path/to/decomposed_mat')"
             ]
         }
     ],
     "metadata": {
         "interpreter": {
             "hash": "1151b7ff23027c657d789cc46e8e163c83031cce3e7a08e093da0d0529a3264f"
         },
```

### Comparing `tomotok-1.2.2/tutorials/linear.ipynb` & `tomotok-1.3/tutorials/linear.ipynb`

 * *Files identical despite different names*

### Comparing `tomotok-1.2.2/tutorials/minfisher.ipynb` & `tomotok-1.3/tutorials/minfisher.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9901092876421824%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(3, 'from tomotok.core.derivative import derivative_matrix, "*

 * *            "laplace_matrix\\n')], delete: [3]}}, 1: {'source': ['# define inversion grid with 25 "*

 * *            "radial and 50 vertical segments\\n', 'grid = RegularGrid(nr=25, nz=50, rlims=(0.2, "*

 * *            "0.7), zlims=(-0.5, 0.5))']}, 2: {'source': {insert: [(0, '# create phantom "*

 * *            "emissivity\\n'), (3, 'phantom = gauss(ipsi, w=0.1, cen=0.4, amp=100)  # produces the "*

 * *            "same output […]*

```diff
@@ -5,38 +5,40 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "\n",
-                "from tomotok.core.derivative import compute_iso_dmats, compute_aniso_dmats\n",
+                "from tomotok.core.derivative import derivative_matrix, laplace_matrix\n",
                 "from tomotok.core.phantoms import gauss_iso, iso_psi, gauss\n",
                 "from tomotok.core.geometry import sparse_line_3d, RegularGrid, generate_los\n",
                 "from tomotok.core.inversions import CholmodMfr, Mfr"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "grid = RegularGrid(25, 50, (.2, .7), (-.5, .5))"
+                "# define inversion grid with 25 radial and 50 vertical segments\n",
+                "grid = RegularGrid(nr=25, nz=50, rlims=(0.2, 0.7), zlims=(-0.5, 0.5))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# create phantom emissivity\n",
                 "# phantom = gauss_iso(grid.nx, grid.ny, cen=.3, amp=100)\n",
                 "ipsi = iso_psi(grid.nr, grid.nz, span=1.2)  # circular \"flux\" surfaces\n",
-                "phantom = gauss(ipsi, cen=.3, amp=100)  # should be the same as gauss_iso"
+                "phantom = gauss(ipsi, w=0.1, cen=0.4, amp=100)  # produces the same output as gauss_iso"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -164,47 +166,70 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# estimation of measurement errors\n",
-                "errors = (data + data.max() ) / 2 * .05\n",
-                "# errors = .001"
+                "errors = (data + data.max() ) / 2 * .01\n",
+                "# errors = data.max() * 0.01  # one percent of maximum for all channels"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "derivatives = [\n",
+                "    derivative_matrix(grid, 'right'),\n",
+                "    derivative_matrix(grid, 'top'),\n",
+                "    derivative_matrix(grid, 'left'),\n",
+                "    derivative_matrix(grid, 'bottom'),\n",
+                "    derivative_matrix(grid, 'top-right'),\n",
+                "    derivative_matrix(grid, 'top-left'),\n",
+                "    derivative_matrix(grid, 'bottom-left'),\n",
+                "    derivative_matrix(grid, 'bottom-right'),\n",
+                "    # laplace_matrix(grid),\n",
+                "]\n",
+                "# derivatives = laplace_matrix(grid, diagonals=False)\n",
                 "# dmats = compute_iso_dmats(grid)\n",
-                "dmats = compute_aniso_dmats(grid, magflux=ipsi)"
+                "# dmats = compute_aniso_dmats(grid, magflux=ipsi)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "res, stats = solver(data, gmat, dmats, errors, aniso=0)"
+                "res, stats = solver(data, gmat, derivatives, errors)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "stats"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "rec = res[0].reshape(grid.shape)\n",
+                "\n",
                 "# plot result\n",
                 "f, a = plt.subplots()\n",
                 "# img = a.imshow(res.reshape(grid.shape), origin='lower', extent=grid.extent)  # nodes should be squares\n",
-                "img = a.pcolorfast(grid.r_center, grid.z_center, res[0].reshape(grid.shape))  # rectangular nodes\n",
+                "img = a.pcolorfast(grid.r_center, grid.z_center, rec)  # rectangular nodes\n",
                 "a.set_aspect(1)\n",
                 "a.set_xlabel('R [-]')\n",
                 "a.set_ylabel('z [-]')\n",
                 "f.colorbar(img, ax=a, label='Emissivity [-]')\n",
                 "# plt.colorbar(label='Emissivity [-]')\n",
                 "plt.show()"
             ]
@@ -214,15 +239,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# plot result and phantom using contours\n",
                 "levels = np.linspace(0, res[0].max(), 10)\n",
                 "plt.figure()\n",
-                "plt.contour(grid.r_center, grid.z_center, res.reshape(grid.shape), levels=levels)\n",
+                "plt.contour(grid.r_center, grid.z_center, rec, levels=levels)\n",
                 "plt.contour(grid.r_center, grid.z_center, phantom, linestyles='dotted', levels=levels)\n",
                 "\n",
                 "# make legend entries\n",
                 "proxy = [plt.Line2D([], [], c='k', ls='solid'), plt.Line2D([], [], c='k', ls='dotted')]\n",
                 "plt.legend(proxy, ['Result', 'Phantom'])\n",
                 "\n",
                 "plt.xlabel('R [-]')\n",
```

