# Comparing `tmp/PyAPplus64-1.0.1.tar.gz` & `tmp/PyAPplus64-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAPplus64-1.0.1.tar", last modified: Sat May  6 20:22:25 2023, max compression
+gzip compressed data, was "PyAPplus64-1.1.0.tar", last modified: Thu Jul 27 09:34:23 2023, max compression
```

## Comparing `PyAPplus64-1.0.1.tar` & `PyAPplus64-1.1.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:25.056602 PyAPplus64-1.0.1/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1095 2023-05-04 13:06:10.000000 PyAPplus64-1.0.1/LICENSE
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      116 2023-05-04 12:51:18.000000 PyAPplus64-1.0.1/MANIFEST.in
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4008 2023-05-06 20:22:25.053602 PyAPplus64-1.0.1/PKG-INFO
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3158 2023-05-04 14:57:06.000000 PyAPplus64-1.0.1/README.md
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.423595 PyAPplus64-1.0.1/docs/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      638 2023-03-25 10:16:40.000000 PyAPplus64-1.0.1/docs/Makefile
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.321594 PyAPplus64-1.0.1/docs/build/
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.528596 PyAPplus64-1.0.1/docs/build/html/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      230 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/.buildinfo
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.581597 PyAPplus64-1.0.1/docs/build/html/_sources/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1393 2023-03-25 15:50:40.000000 PyAPplus64-1.0.1/docs/build/html/_sources/abhaengigkeiten.rst.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4585 2023-05-06 17:30:57.000000 PyAPplus64-1.0.1/docs/build/html/_sources/anwendungen.rst.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2299 2023-04-28 09:19:27.000000 PyAPplus64-1.0.1/docs/build/html/_sources/beschreibung.rst.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2825 2023-05-06 17:30:57.000000 PyAPplus64-1.0.1/docs/build/html/_sources/examples.rst.txt
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.589597 PyAPplus64-1.0.1/docs/build/html/_sources/generated/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1711 2023-03-25 10:47:31.000000 PyAPplus64-1.0.1/docs/build/html/_sources/generated/PyAPplus64.rst.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      186 2023-03-25 17:36:43.000000 PyAPplus64-1.0.1/docs/build/html/_sources/index.rst.txt
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.734598 PyAPplus64-1.0.1/docs/build/html/_static/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     8133 2021-11-17 15:47:22.000000 PyAPplus64-1.0.1/docs/build/html/_static/base-stemmer.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    14667 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/_static/basic.css
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     9630 2021-11-17 15:50:47.000000 PyAPplus64-1.0.1/docs/build/html/_static/doctools.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      353 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      286 2021-01-01 06:53:29.000000 PyAPplus64-1.0.1/docs/build/html/_static/file.png
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    17647 2021-11-17 15:47:22.000000 PyAPplus64-1.0.1/docs/build/html/_static/german-stemmer.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)   288550 2022-02-21 10:29:39.000000 PyAPplus64-1.0.1/docs/build/html/_static/jquery.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    16661 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/_static/language_data.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       90 2021-01-01 06:53:29.000000 PyAPplus64-1.0.1/docs/build/html/_static/minus.png
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4181 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/_static/nature.css
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       90 2021-01-01 06:53:29.000000 PyAPplus64-1.0.1/docs/build/html/_static/plus.png
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5432 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/_static/pygments.css
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    16950 2021-12-19 12:55:13.000000 PyAPplus64-1.0.1/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3792 2021-12-19 12:55:13.000000 PyAPplus64-1.0.1/docs/build/html/_static/translations.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    68398 2021-12-16 10:20:19.000000 PyAPplus64-1.0.1/docs/build/html/_static/underscore.js
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     8606 2023-05-06 20:11:52.000000 PyAPplus64-1.0.1/docs/build/html/abhaengigkeiten.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    23321 2023-05-06 20:11:52.000000 PyAPplus64-1.0.1/docs/build/html/anwendungen.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     7705 2023-05-06 20:11:52.000000 PyAPplus64-1.0.1/docs/build/html/beschreibung.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)   109765 2023-05-06 20:11:52.000000 PyAPplus64-1.0.1/docs/build/html/examples.html
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.742598 PyAPplus64-1.0.1/docs/build/html/generated/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)   321089 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/generated/PyAPplus64.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    46923 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/genindex.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4654 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/index.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1962 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/objects.inv
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5996 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/py-modindex.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3448 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/search.html
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    25310 2023-05-06 20:11:53.000000 PyAPplus64-1.0.1/docs/build/html/searchindex.js
--rwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)      114 2023-05-04 12:56:52.000000 PyAPplus64-1.0.1/docs/builddocs.sh
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      804 2023-05-04 12:57:07.000000 PyAPplus64-1.0.1/docs/make.bat
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.806599 PyAPplus64-1.0.1/docs/source/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1393 2023-03-25 15:50:40.000000 PyAPplus64-1.0.1/docs/source/abhaengigkeiten.rst
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4585 2023-05-06 17:30:57.000000 PyAPplus64-1.0.1/docs/source/anwendungen.rst
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2299 2023-04-28 09:19:27.000000 PyAPplus64-1.0.1/docs/source/beschreibung.rst
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1561 2023-05-06 20:20:57.000000 PyAPplus64-1.0.1/docs/source/conf.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2825 2023-05-06 17:30:57.000000 PyAPplus64-1.0.1/docs/source/examples.rst
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      186 2023-03-25 17:36:43.000000 PyAPplus64-1.0.1/docs/source/index.rst
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.858600 PyAPplus64-1.0.1/examples/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1393 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/examples/adhoc_report.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      756 2023-05-04 12:59:22.000000 PyAPplus64-1.0.1/examples/applus-server.yaml
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1266 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/examples/check_dokumente.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2295 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/examples/copy_artikel.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     7447 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/examples/mengenabweichung.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      988 2023-05-06 20:20:57.000000 PyAPplus64-1.0.1/pyproject.toml
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       38 2023-05-06 20:22:25.058602 PyAPplus64-1.0.1/setup.cfg
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.355594 PyAPplus64-1.0.1/src/
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:24.973601 PyAPplus64-1.0.1/src/PyAPplus64/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      735 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/src/PyAPplus64/__init__.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    12530 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/src/PyAPplus64/applus.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5691 2023-05-06 20:00:37.000000 PyAPplus64-1.0.1/src/PyAPplus64/applus_db.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     6563 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/applus_scripttool.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3148 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/applus_server.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2130 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/applus_sysconf.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    12187 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/applus_usexml.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    22880 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/duplicate.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4765 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/pandas.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 12:51:19.000000 PyAPplus64-1.0.1/src/PyAPplus64/py.typed
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    27330 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/sql_utils.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1724 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/src/PyAPplus64/utils.py
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:25.023601 PyAPplus64-1.0.1/src/PyAPplus64.egg-info/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4008 2023-05-06 20:22:24.000000 PyAPplus64-1.0.1/src/PyAPplus64.egg-info/PKG-INFO
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2180 2023-05-06 20:22:24.000000 PyAPplus64-1.0.1/src/PyAPplus64.egg-info/SOURCES.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)        1 2023-05-06 20:22:24.000000 PyAPplus64-1.0.1/src/PyAPplus64.egg-info/dependency_links.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       48 2023-05-06 20:22:24.000000 PyAPplus64-1.0.1/src/PyAPplus64.egg-info/requires.txt
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       11 2023-05-06 20:22:24.000000 PyAPplus64-1.0.1/src/PyAPplus64.egg-info/top_level.txt
-drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-06 20:22:25.042601 PyAPplus64-1.0.1/tests/
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      786 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/tests/test_applus_db.py
--rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    13162 2023-05-06 20:00:38.000000 PyAPplus64-1.0.1/tests/test_sql_utils.py
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:23.186708 PyAPplus64-1.1.0/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1095 2023-05-04 13:06:10.000000 PyAPplus64-1.1.0/LICENSE
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      116 2023-05-04 12:51:18.000000 PyAPplus64-1.1.0/MANIFEST.in
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4239 2023-07-27 09:34:23.181708 PyAPplus64-1.1.0/PKG-INFO
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3389 2023-07-27 09:14:50.000000 PyAPplus64-1.1.0/README.md
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:22.614702 PyAPplus64-1.1.0/docs/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      638 2023-03-25 10:16:40.000000 PyAPplus64-1.1.0/docs/Makefile
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:22.520702 PyAPplus64-1.1.0/docs/build/
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:22.706703 PyAPplus64-1.1.0/docs/build/html/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      230 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/.buildinfo
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:22.754704 PyAPplus64-1.1.0/docs/build/html/_sources/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1393 2023-03-25 15:50:40.000000 PyAPplus64-1.1.0/docs/build/html/_sources/abhaengigkeiten.rst.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4603 2023-07-27 08:29:36.000000 PyAPplus64-1.1.0/docs/build/html/_sources/anwendungen.rst.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2299 2023-04-28 09:19:27.000000 PyAPplus64-1.1.0/docs/build/html/_sources/beschreibung.rst.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2825 2023-05-06 17:30:57.000000 PyAPplus64-1.1.0/docs/build/html/_sources/examples.rst.txt
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:22.762704 PyAPplus64-1.1.0/docs/build/html/_sources/generated/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1711 2023-03-25 10:47:31.000000 PyAPplus64-1.1.0/docs/build/html/_sources/generated/PyAPplus64.rst.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      186 2023-03-25 17:36:43.000000 PyAPplus64-1.1.0/docs/build/html/_sources/index.rst.txt
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:22.913705 PyAPplus64-1.1.0/docs/build/html/_static/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     8133 2021-11-17 15:47:22.000000 PyAPplus64-1.1.0/docs/build/html/_static/base-stemmer.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    14667 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/_static/basic.css
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     9630 2021-11-17 15:50:47.000000 PyAPplus64-1.1.0/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      353 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      286 2021-01-01 06:53:29.000000 PyAPplus64-1.1.0/docs/build/html/_static/file.png
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    17647 2021-11-17 15:47:22.000000 PyAPplus64-1.1.0/docs/build/html/_static/german-stemmer.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)   288550 2022-02-21 10:29:39.000000 PyAPplus64-1.1.0/docs/build/html/_static/jquery.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    16661 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       90 2021-01-01 06:53:29.000000 PyAPplus64-1.1.0/docs/build/html/_static/minus.png
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4181 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/_static/nature.css
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       90 2021-01-01 06:53:29.000000 PyAPplus64-1.1.0/docs/build/html/_static/plus.png
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5432 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    16950 2021-12-19 12:55:13.000000 PyAPplus64-1.1.0/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3792 2021-12-19 12:55:13.000000 PyAPplus64-1.1.0/docs/build/html/_static/translations.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    68398 2021-12-16 10:20:19.000000 PyAPplus64-1.1.0/docs/build/html/_static/underscore.js
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     8606 2023-07-27 08:31:10.000000 PyAPplus64-1.1.0/docs/build/html/abhaengigkeiten.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    23339 2023-07-27 08:31:10.000000 PyAPplus64-1.1.0/docs/build/html/anwendungen.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     7705 2023-07-27 08:31:10.000000 PyAPplus64-1.1.0/docs/build/html/beschreibung.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)   111269 2023-07-27 08:31:10.000000 PyAPplus64-1.1.0/docs/build/html/examples.html
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:22.920705 PyAPplus64-1.1.0/docs/build/html/generated/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)   327782 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/generated/PyAPplus64.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    48079 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/genindex.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4654 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/index.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2001 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/objects.inv
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5996 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/py-modindex.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     3448 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/search.html
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    25887 2023-07-27 08:31:11.000000 PyAPplus64-1.1.0/docs/build/html/searchindex.js
+-rwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)      114 2023-05-04 12:56:52.000000 PyAPplus64-1.1.0/docs/builddocs.sh
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      804 2023-05-04 12:57:07.000000 PyAPplus64-1.1.0/docs/make.bat
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:22.974706 PyAPplus64-1.1.0/docs/source/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1703 2023-07-27 09:17:32.000000 PyAPplus64-1.1.0/docs/source/abhaengigkeiten.rst
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4603 2023-07-27 08:52:52.000000 PyAPplus64-1.1.0/docs/source/anwendungen.rst
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2299 2023-04-28 09:19:27.000000 PyAPplus64-1.1.0/docs/source/beschreibung.rst
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1561 2023-05-06 20:20:57.000000 PyAPplus64-1.1.0/docs/source/conf.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2825 2023-05-06 17:30:57.000000 PyAPplus64-1.1.0/docs/source/examples.rst
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      186 2023-03-25 17:36:43.000000 PyAPplus64-1.1.0/docs/source/index.rst
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:23.016706 PyAPplus64-1.1.0/examples/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1393 2023-05-06 20:00:37.000000 PyAPplus64-1.1.0/examples/adhoc_report.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      937 2023-07-27 08:52:52.000000 PyAPplus64-1.1.0/examples/applus-server.yaml
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1266 2023-05-06 20:00:37.000000 PyAPplus64-1.1.0/examples/check_dokumente.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2295 2023-05-06 20:00:37.000000 PyAPplus64-1.1.0/examples/copy_artikel.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     7447 2023-05-06 20:00:37.000000 PyAPplus64-1.1.0/examples/mengenabweichung.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      988 2023-07-27 09:13:15.000000 PyAPplus64-1.1.0/pyproject.toml
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       38 2023-07-27 09:34:23.188708 PyAPplus64-1.1.0/setup.cfg
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:22.552702 PyAPplus64-1.1.0/src/
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:23.117707 PyAPplus64-1.1.0/src/PyAPplus64/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      735 2023-05-06 20:00:37.000000 PyAPplus64-1.1.0/src/PyAPplus64/__init__.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    13366 2023-07-27 08:52:52.000000 PyAPplus64-1.1.0/src/PyAPplus64/applus.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5691 2023-05-06 20:00:37.000000 PyAPplus64-1.1.0/src/PyAPplus64/applus_db.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     6566 2023-07-27 08:52:52.000000 PyAPplus64-1.1.0/src/PyAPplus64/applus_scripttool.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     5058 2023-07-27 08:52:52.000000 PyAPplus64-1.1.0/src/PyAPplus64/applus_server.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2133 2023-07-27 08:52:52.000000 PyAPplus64-1.1.0/src/PyAPplus64/applus_sysconf.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    12187 2023-05-06 20:00:38.000000 PyAPplus64-1.1.0/src/PyAPplus64/applus_usexml.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    22880 2023-05-06 20:00:38.000000 PyAPplus64-1.1.0/src/PyAPplus64/duplicate.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4765 2023-05-06 20:00:38.000000 PyAPplus64-1.1.0/src/PyAPplus64/pandas.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)        0 2023-05-04 12:51:19.000000 PyAPplus64-1.1.0/src/PyAPplus64/py.typed
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    27330 2023-05-06 20:00:38.000000 PyAPplus64-1.1.0/src/PyAPplus64/sql_utils.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     1724 2023-05-06 20:00:38.000000 PyAPplus64-1.1.0/src/PyAPplus64/utils.py
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:23.152708 PyAPplus64-1.1.0/src/PyAPplus64.egg-info/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     4239 2023-07-27 09:34:22.000000 PyAPplus64-1.1.0/src/PyAPplus64.egg-info/PKG-INFO
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)     2180 2023-07-27 09:34:22.000000 PyAPplus64-1.1.0/src/PyAPplus64.egg-info/SOURCES.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)        1 2023-07-27 09:34:22.000000 PyAPplus64-1.1.0/src/PyAPplus64.egg-info/dependency_links.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       48 2023-07-27 09:34:22.000000 PyAPplus64-1.1.0/src/PyAPplus64.egg-info/requires.txt
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)       11 2023-07-27 09:34:22.000000 PyAPplus64-1.1.0/src/PyAPplus64.egg-info/top_level.txt
+drwxrwxr-x   0 thtuerk   (1000) thtuerk   (1000)        0 2023-07-27 09:34:23.171708 PyAPplus64-1.1.0/tests/
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)      786 2023-05-06 20:00:38.000000 PyAPplus64-1.1.0/tests/test_applus_db.py
+-rw-rw-r--   0 thtuerk   (1000) thtuerk   (1000)    13162 2023-05-06 20:00:38.000000 PyAPplus64-1.1.0/tests/test_sql_utils.py
```

### Comparing `PyAPplus64-1.0.1/LICENSE` & `PyAPplus64-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/PKG-INFO` & `PyAPplus64-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAPplus64
-Version: 1.0.1
+Version: 1.1.0
 Summary: Verschiedene Hilfsmittel, um mit dem ERP System APplus zu interagieren. Dieses Packet wurde für APplus 6.4 entwickelt, funktioniert vermutlich aber auch mit anderen Versionen.
 Author-email: Thomas Tuerk <kontakt@thomas-tuerk.de>
 Project-URL: homepage, https://www.thomas-tuerk.de/de/pyapplus64
 Project-URL: repository, https://git.thomas-tuerk.de/thtuerk/PyAPplus64
 Project-URL: documentation, https://www.thomas-tuerk.de/assets/PyAPplus64/html/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,30 +13,30 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyAPplus64
 
-## Beschreibung 
-Das Paket `PyAPplus64` enthält eine Sammlung von Python Tools für die Interaktion mit dem ERP-System APplus 6.4. 
-Es sollte auch für andere APplus Versionen nützlich sein. 
+## Beschreibung
+Das Paket `PyAPplus64` enthält eine Sammlung von Python Tools für die Interaktion mit dem ERP-System APplus 6.4.
+Es sollte auch für andere APplus Versionen nützlich sein.
 
 Zielgruppe sind APplus-Administratoren und Anpassungs-Entwickler. Die Tools erlauben u.a.
 
 - einfacher Zugriff auf SOAP-Schnittstelle des App-Servers
    + damit Zugriff auf SysConfig
    + Zugriff auf Tools `nextNumber` für Erzeugung der nächsten Nummer für ein Business-Object
-   + ...   
+   + ...
 - Zugriff auf APplus DB per direktem DB-Zugriff und mittels SOAP
    + automatischer Aufruf von `completeSQL`, um per App-Server SQL-Statements um z.B. Mandanten erweitern zu lassen
    + Tools für einfache Benutzung von `useXML`, d.h. für das Einfügen, Löschen und Ändern von Datensätzen
-     mit Hilfe des APP-Servers. Genau wie bei Änderungen an Datensätzen über die Web-Oberfläche und im Gegensatz 
-     zum direkten Zugriff über die Datenbank werden dabei evtl. zusätzliche 
-     Checks ausgeführt, bestimmte Felder automatisch gesetzt oder bestimmte Aktionen angestoßen. 
+     mit Hilfe des APP-Servers. Genau wie bei Änderungen an Datensätzen über die Web-Oberfläche und im Gegensatz
+     zum direkten Zugriff über die Datenbank werden dabei evtl. zusätzliche
+     Checks ausgeführt, bestimmte Felder automatisch gesetzt oder bestimmte Aktionen angestoßen.
 - das Duplizieren von Datensätzen
    + zu kopierende Felder aus XML-Definitionen werden ausgewertet
    + Abhängige Objekte können einfach ebenfalls mit-kopiert werden
    + Änderungen wie beispielsweise Nummer des Objektes möglich
    + Unterstützung für Kopieren dyn. Attribute
    + Anlage neuer Objekte mittels APP-Server
    + Datensätze können zwischen Systemen kopiert und auch in Dateien gespeichert werden
@@ -48,26 +48,34 @@
 
 In `PyAPplus64` wurden die Features (vielleicht leicht verallgemeinert)
 implementiert, die ich für konkrete Aufgabenstellungen benötigte. Ich gehe davon
 aus, dass im Laufe der Zeit weitere Features hinzukommen.
 
 ## Warnung
 
-`PyAPplus64` erlaubt den schreibenden Zugriff auf die APplus Datenbank und beliebige 
-Aufrufe von SOAP-Methoden. Unsachgemäße Nutzung kann Ihre Daten zerstören. Benutzen Sie 
-`PyAPplus64` daher bitte vorsichtig. 
+`PyAPplus64` erlaubt den schreibenden Zugriff auf die APplus Datenbank und beliebige
+Aufrufe von SOAP-Methoden. Unsachgemäße Nutzung kann Ihre Daten zerstören. Benutzen Sie
+`PyAPplus64` daher bitte vorsichtig.
 
 ## Installation
 
 PyAPplus64 wurde auf PyPi veröffentlicht. Es lässt sich daher einfach mittel `pip` installieren
 
 ````
   pip install PyAPplus64
 ````
 
+Zur Nutzung von ASMX-Seiten ist die Authentifizierungsmethode Negotiate nötig. Für diese muss `requests-negotiate-sspi` installiert werden,
+was aber leider nur unter Windows verfügbar ist.
+
+````
+  pip install requests-negotiate-sspi
+````
+
+
 ## Links
 
 - [PyPi](https://pypi.org/project/PyAPplus64/)
 - Doku [PDF](https://www.thomas-tuerk.de/assets/PyAPplus64/pyapplus64.pdf), [HTML](https://www.thomas-tuerk.de/assets/PyAPplus64/html/index.html)
 - [GIT-Repository](https://git.thomas-tuerk.de/thtuerk/PyAPplus64)
 - [GitHub](https://github.com/thtuerk/PyAPplus64)
```

### Comparing `PyAPplus64-1.0.1/README.md` & `PyAPplus64-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # PyAPplus64
 
-## Beschreibung 
-Das Paket `PyAPplus64` enthält eine Sammlung von Python Tools für die Interaktion mit dem ERP-System APplus 6.4. 
-Es sollte auch für andere APplus Versionen nützlich sein. 
+## Beschreibung
+Das Paket `PyAPplus64` enthält eine Sammlung von Python Tools für die Interaktion mit dem ERP-System APplus 6.4.
+Es sollte auch für andere APplus Versionen nützlich sein.
 
 Zielgruppe sind APplus-Administratoren und Anpassungs-Entwickler. Die Tools erlauben u.a.
 
 - einfacher Zugriff auf SOAP-Schnittstelle des App-Servers
    + damit Zugriff auf SysConfig
    + Zugriff auf Tools `nextNumber` für Erzeugung der nächsten Nummer für ein Business-Object
-   + ...   
+   + ...
 - Zugriff auf APplus DB per direktem DB-Zugriff und mittels SOAP
    + automatischer Aufruf von `completeSQL`, um per App-Server SQL-Statements um z.B. Mandanten erweitern zu lassen
    + Tools für einfache Benutzung von `useXML`, d.h. für das Einfügen, Löschen und Ändern von Datensätzen
-     mit Hilfe des APP-Servers. Genau wie bei Änderungen an Datensätzen über die Web-Oberfläche und im Gegensatz 
-     zum direkten Zugriff über die Datenbank werden dabei evtl. zusätzliche 
-     Checks ausgeführt, bestimmte Felder automatisch gesetzt oder bestimmte Aktionen angestoßen. 
+     mit Hilfe des APP-Servers. Genau wie bei Änderungen an Datensätzen über die Web-Oberfläche und im Gegensatz
+     zum direkten Zugriff über die Datenbank werden dabei evtl. zusätzliche
+     Checks ausgeführt, bestimmte Felder automatisch gesetzt oder bestimmte Aktionen angestoßen.
 - das Duplizieren von Datensätzen
    + zu kopierende Felder aus XML-Definitionen werden ausgewertet
    + Abhängige Objekte können einfach ebenfalls mit-kopiert werden
    + Änderungen wie beispielsweise Nummer des Objektes möglich
    + Unterstützung für Kopieren dyn. Attribute
    + Anlage neuer Objekte mittels APP-Server
    + Datensätze können zwischen Systemen kopiert und auch in Dateien gespeichert werden
@@ -31,26 +31,34 @@
 
 In `PyAPplus64` wurden die Features (vielleicht leicht verallgemeinert)
 implementiert, die ich für konkrete Aufgabenstellungen benötigte. Ich gehe davon
 aus, dass im Laufe der Zeit weitere Features hinzukommen.
 
 ## Warnung
 
-`PyAPplus64` erlaubt den schreibenden Zugriff auf die APplus Datenbank und beliebige 
-Aufrufe von SOAP-Methoden. Unsachgemäße Nutzung kann Ihre Daten zerstören. Benutzen Sie 
-`PyAPplus64` daher bitte vorsichtig. 
+`PyAPplus64` erlaubt den schreibenden Zugriff auf die APplus Datenbank und beliebige
+Aufrufe von SOAP-Methoden. Unsachgemäße Nutzung kann Ihre Daten zerstören. Benutzen Sie
+`PyAPplus64` daher bitte vorsichtig.
 
 ## Installation
 
 PyAPplus64 wurde auf PyPi veröffentlicht. Es lässt sich daher einfach mittel `pip` installieren
 
 ````
   pip install PyAPplus64
 ````
 
+Zur Nutzung von ASMX-Seiten ist die Authentifizierungsmethode Negotiate nötig. Für diese muss `requests-negotiate-sspi` installiert werden,
+was aber leider nur unter Windows verfügbar ist.
+
+````
+  pip install requests-negotiate-sspi
+````
+
+
 ## Links
 
 - [PyPi](https://pypi.org/project/PyAPplus64/)
 - Doku [PDF](https://www.thomas-tuerk.de/assets/PyAPplus64/pyapplus64.pdf), [HTML](https://www.thomas-tuerk.de/assets/PyAPplus64/html/index.html)
 - [GIT-Repository](https://git.thomas-tuerk.de/thtuerk/PyAPplus64)
 - [GitHub](https://github.com/thtuerk/PyAPplus64)
```

### Comparing `PyAPplus64-1.0.1/docs/Makefile` & `PyAPplus64-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_sources/abhaengigkeiten.rst.txt` & `PyAPplus64-1.1.0/docs/build/html/_sources/abhaengigkeiten.rst.txt`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_sources/anwendungen.rst.txt` & `PyAPplus64-1.1.0/docs/build/html/_sources/anwendungen.rst.txt`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,14 @@
 werden automatisch die für die Umgebung nötigen Mandanten zu den SQL Statements hinzugefügt. Zudem ist einfach ein
 Zugriff auf die Sysconf möglich::
 
    print (server.sysconf.getString("STAMM", "MYLAND"))
    print (server.sysconf.getList("STAMM", "EULAENDER"))
 
 Dank der Bibliothek `zeep` ist es auch sehr einfach möglich, auf beliebige SOAP-Methoden zuzugreifen.
-Beispielsweise kann auf die Sys-Config auch händisch, d.h. durch direkten Aufruf einer SOAP-Methode,
-zugegriffen werden::
+Beispielsweise kann auf die Sys-Config auch händisch, d.h. durch direkten Aufruf einer SOAP-Methode
+des APP-Servers zugegriffen werden::
 
-   client = server.server_conn.getClient("p2system", "SysConf");
+   client = server.server_conn.getAppClient("p2system", "SysConf");
    print (client.service.getString("STAMM", "MYLAND"))
```

### Comparing `PyAPplus64-1.0.1/docs/build/html/_sources/beschreibung.rst.txt` & `PyAPplus64-1.1.0/docs/build/html/_sources/beschreibung.rst.txt`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_sources/examples.rst.txt` & `PyAPplus64-1.1.0/docs/build/html/_sources/examples.rst.txt`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_sources/generated/PyAPplus64.rst.txt` & `PyAPplus64-1.1.0/docs/build/html/_sources/generated/PyAPplus64.rst.txt`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_static/base-stemmer.js` & `PyAPplus64-1.1.0/docs/build/html/_static/base-stemmer.js`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_static/basic.css` & `PyAPplus64-1.1.0/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_static/doctools.js` & `PyAPplus64-1.1.0/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_static/german-stemmer.js` & `PyAPplus64-1.1.0/docs/build/html/_static/german-stemmer.js`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_static/jquery.js` & `PyAPplus64-1.1.0/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_static/language_data.js` & `PyAPplus64-1.1.0/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_static/nature.css` & `PyAPplus64-1.1.0/docs/build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_static/pygments.css` & `PyAPplus64-1.1.0/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_static/searchtools.js` & `PyAPplus64-1.1.0/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_static/translations.js` & `PyAPplus64-1.1.0/docs/build/html/_static/translations.js`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/_static/underscore.js` & `PyAPplus64-1.1.0/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/abhaengigkeiten.html` & `PyAPplus64-1.1.0/docs/build/html/abhaengigkeiten.html`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/anwendungen.html` & `PyAPplus64-1.1.0/docs/build/html/anwendungen.html`

 * *Files 0% similar despite different names*

```diff
@@ -165,17 +165,17 @@
 werden automatisch die für die Umgebung nötigen Mandanten zu den SQL Statements hinzugefügt. Zudem ist einfach ein
 Zugriff auf die Sysconf möglich:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="nb">print</span> <span class="p">(</span><span class="n">server</span><span class="o">.</span><span class="n">sysconf</span><span class="o">.</span><span class="n">getString</span><span class="p">(</span><span class="s2">&quot;STAMM&quot;</span><span class="p">,</span> <span class="s2">&quot;MYLAND&quot;</span><span class="p">))</span>
 <span class="nb">print</span> <span class="p">(</span><span class="n">server</span><span class="o">.</span><span class="n">sysconf</span><span class="o">.</span><span class="n">getList</span><span class="p">(</span><span class="s2">&quot;STAMM&quot;</span><span class="p">,</span> <span class="s2">&quot;EULAENDER&quot;</span><span class="p">))</span>
 </pre></div>
 </div>
 <p>Dank der Bibliothek <cite>zeep</cite> ist es auch sehr einfach möglich, auf beliebige SOAP-Methoden zuzugreifen.
-Beispielsweise kann auf die Sys-Config auch händisch, d.h. durch direkten Aufruf einer SOAP-Methode,
-zugegriffen werden:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">client</span> <span class="o">=</span> <span class="n">server</span><span class="o">.</span><span class="n">server_conn</span><span class="o">.</span><span class="n">getClient</span><span class="p">(</span><span class="s2">&quot;p2system&quot;</span><span class="p">,</span> <span class="s2">&quot;SysConf&quot;</span><span class="p">);</span>
+Beispielsweise kann auf die Sys-Config auch händisch, d.h. durch direkten Aufruf einer SOAP-Methode
+des APP-Servers zugegriffen werden:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">client</span> <span class="o">=</span> <span class="n">server</span><span class="o">.</span><span class="n">server_conn</span><span class="o">.</span><span class="n">getAppClient</span><span class="p">(</span><span class="s2">&quot;p2system&quot;</span><span class="p">,</span> <span class="s2">&quot;SysConf&quot;</span><span class="p">);</span>
 <span class="nb">print</span> <span class="p">(</span><span class="n">client</span><span class="o">.</span><span class="n">service</span><span class="o">.</span><span class="n">getString</span><span class="p">(</span><span class="s2">&quot;STAMM&quot;</span><span class="p">,</span> <span class="s2">&quot;MYLAND&quot;</span><span class="p">))</span>
 </pre></div>
 </div>
 </section>
 </section>
```

#### html2text {}

```diff
@@ -136,16 +136,17 @@
 Zugriff auf die DB. Hierbei werden automatisch die fÃ¼r die Umgebung nÃ¶tigen
 Mandanten zu den SQL Statements hinzugefÃ¼gt. Zudem ist einfach ein Zugriff auf
 die Sysconf mÃ¶glich:
 print (server.sysconf.getString("STAMM", "MYLAND"))
 print (server.sysconf.getList("STAMM", "EULAENDER"))
 Dank der Bibliothekzeepist es auch sehr einfach mÃ¶glich, auf beliebige SOAP-
 Methoden zuzugreifen. Beispielsweise kann auf die Sys-Config auch hÃ¤ndisch,
-d.h. durch direkten Aufruf einer SOAP-Methode, zugegriffen werden:
-client = server.server_conn.getClient("p2system", "SysConf");
+d.h. durch direkten Aufruf einer SOAP-Methode des APP-Servers zugegriffen
+werden:
+client = server.server_conn.getAppClient("p2system", "SysConf");
 print (client.service.getString("STAMM", "MYLAND"))
 
 **** Inhaltsverzeichnis ****
     * typische_AnwendungsfÃ¤lle
           o einfache_Admin-Aufgaben
           o Ad-hoc_Reports
           o Anbindung_eigener_Tools
```

### Comparing `PyAPplus64-1.0.1/docs/build/html/beschreibung.html` & `PyAPplus64-1.1.0/docs/build/html/beschreibung.html`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/examples.html` & `PyAPplus64-1.1.0/docs/build/html/examples.html`

 * *Files 0% similar despite different names*

```diff
@@ -59,22 +59,25 @@
 <span class="linenos"> 4</span><span class="nt">appserver </span><span class="p">:</span><span class="w"> </span><span class="p p-Indicator">{</span><span class="w"></span>
 <span class="linenos"> 5</span><span class="nt">  server </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;some-server&quot;</span><span class="p p-Indicator">,</span><span class="w"></span>
 <span class="linenos"> 6</span><span class="nt">  port </span><span class="p">:</span><span class="w"> </span><span class="nv">2037</span><span class="p p-Indicator">,</span><span class="w"></span>
 <span class="linenos"> 7</span><span class="nt">  user </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;asol.projects&quot;</span><span class="p p-Indicator">,</span><span class="w"></span>
 <span class="linenos"> 8</span><span class="nt">  env  </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;default-umgebung&quot;</span><span class="w"> </span><span class="c1"># hier wirklich Umgebung, nicht Mandant verwenden</span><span class="w"></span>
 <span class="linenos"> 9</span><span class="p p-Indicator">}</span><span class="w"></span>
 <span class="linenos">10</span><span class="nt">webserver </span><span class="p">:</span><span class="w"> </span><span class="p p-Indicator">{</span><span class="w"></span>
-<span class="linenos">11</span><span class="nt">  baseurl </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;http://some-server/APplusProd6/&quot;</span><span class="w"></span>
-<span class="linenos">12</span><span class="p p-Indicator">}</span><span class="w"></span>
-<span class="linenos">13</span><span class="nt">dbserver </span><span class="p">:</span><span class="w"> </span><span class="p p-Indicator">{</span><span class="w"></span>
-<span class="linenos">14</span><span class="nt">  server </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;some-server&quot;</span><span class="p p-Indicator">,</span><span class="w"></span>
-<span class="linenos">15</span><span class="nt">  db </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;APplusProd6&quot;</span><span class="p p-Indicator">,</span><span class="w"></span>
-<span class="linenos">16</span><span class="nt">  user </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;SA&quot;</span><span class="p p-Indicator">,</span><span class="w"></span>
-<span class="linenos">17</span><span class="nt">  password </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;your-db-password&quot;</span><span class="w"></span>
-<span class="linenos">18</span><span class="p p-Indicator">}</span><span class="w"></span>
+<span class="linenos">11</span><span class="nt">  baseurl </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;http://some-server/APplusProd6/&quot;</span><span class="p p-Indicator">,</span><span class="w"></span>
+<span class="linenos">12</span><span class="nt">  user </span><span class="p">:</span><span class="w"> </span><span class="nv">null</span><span class="p p-Indicator">,</span><span class="w"> </span><span class="c1"># oft &quot;ASOL.Projects&quot;, wenn nicht gesetzt, wird aktueller Windows-Nutzer verwendet</span><span class="w"></span>
+<span class="linenos">13</span><span class="nt">  userDomain </span><span class="p">:</span><span class="w"> </span><span class="nv">null</span><span class="p p-Indicator">,</span><span class="w"> </span><span class="c1"># Domain für ASOL.PROJECTS</span><span class="w"></span>
+<span class="linenos">14</span><span class="nt">  password </span><span class="p">:</span><span class="w"> </span><span class="nv">null</span><span class="w"> </span><span class="c1"># das Passwort</span><span class="w"></span>
+<span class="linenos">15</span><span class="p p-Indicator">}</span><span class="w"></span>
+<span class="linenos">16</span><span class="nt">dbserver </span><span class="p">:</span><span class="w"> </span><span class="p p-Indicator">{</span><span class="w"></span>
+<span class="linenos">17</span><span class="nt">  server </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;some-server&quot;</span><span class="p p-Indicator">,</span><span class="w"></span>
+<span class="linenos">18</span><span class="nt">  db </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;APplusProd6&quot;</span><span class="p p-Indicator">,</span><span class="w"></span>
+<span class="linenos">19</span><span class="nt">  user </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;SA&quot;</span><span class="p p-Indicator">,</span><span class="w"></span>
+<span class="linenos">20</span><span class="nt">  password </span><span class="p">:</span><span class="w"> </span><span class="s">&quot;your-db-password&quot;</span><span class="w"></span>
+<span class="linenos">21</span><span class="p p-Indicator">}</span><span class="w"></span>
 </pre></div>
 </div>
 <p>Damit nicht in jedem Script immer wieder neu die Konfig-Dateien ausgewählt werden müssen, werden die Konfigs für
 das Prod-, Test- und Deploy-System in <code class="docutils literal notranslate"><span class="pre">examples/applus_configs.py</span></code> hinterlegt. Diese Datei wird in allen Scripten importiert,
 so dass das Config-Verzeichnis und die darin enthaltenen Configs einfach zur Verfügung stehen.</p>
 <div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos">1</span><span class="kn">import</span> <span class="nn">pathlib</span>
 <span class="linenos">2</span>
@@ -128,17 +131,19 @@
 <span class="linenos">36</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  Mandant:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getMandant</span><span class="p">())</span>
 <span class="linenos">37</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  MandantName:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getMandantName</span><span class="p">())</span>
 <span class="linenos">38</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  InstallPath:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getInstallPath</span><span class="p">())</span>
 <span class="linenos">39</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  InstallPathAppServer:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getInstallPathAppServer</span><span class="p">())</span>
 <span class="linenos">40</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  InstallPathWebServer:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getInstallPathWebServer</span><span class="p">())</span>
 <span class="linenos">41</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;  ServerInfo - Version:&quot;</span><span class="p">,</span> <span class="n">server</span><span class="o">.</span><span class="n">scripttool</span><span class="o">.</span><span class="n">getServerInfo</span><span class="p">()</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;version&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">text</span><span class="p">)</span>
 <span class="linenos">42</span>
-<span class="linenos">43</span>
-<span class="linenos">44</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-<span class="linenos">45</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">)</span>
+<span class="linenos">43</span>    <span class="n">client</span> <span class="o">=</span> <span class="n">server</span><span class="o">.</span><span class="n">getWebClient</span><span class="p">(</span><span class="s2">&quot;masterdata/artikel.asmx&quot;</span><span class="p">)</span>
+<span class="linenos">44</span>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;ARTIKEL-ASMX Date:&quot;</span><span class="p">,</span> <span class="n">client</span><span class="o">.</span><span class="n">service</span><span class="o">.</span><span class="n">getServerDate</span><span class="p">())</span>
+<span class="linenos">45</span>
+<span class="linenos">46</span><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+<span class="linenos">47</span>    <span class="n">main</span><span class="p">(</span><span class="n">applus_configs</span><span class="o">.</span><span class="n">serverConfYamlTest</span><span class="p">)</span>
 </pre></div>
 </div>
 </section>
 <section id="check-dokumente-py">
 <h2><code class="docutils literal notranslate"><span class="pre">check_dokumente.py</span></code><a class="headerlink" href="#check-dokumente-py" title="Link zu dieser Überschrift">¶</a></h2>
 <p>Einfaches Beispiel für lesenden und schreibenden Zugriff auf APplus Datenbank.</p>
 <div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="linenos"> 1</span><span class="kn">import</span> <span class="nn">pathlib</span>
```

#### html2text {}

```diff
@@ -30,22 +30,26 @@
  4appserver : {
  5  server : "some-server",
  6  port : 2037,
  7  user : "asol.projects",
  8  env  : "default-umgebung" # hier wirklich Umgebung, nicht Mandant verwenden
  9}
 10webserver : {
-11  baseurl : "http://some-server/APplusProd6/"
-12}
-13dbserver : {
-14  server : "some-server",
-15  db : "APplusProd6",
-16  user : "SA",
-17  password : "your-db-password"
-18}
+11  baseurl : "http://some-server/APplusProd6/",
+12  user : null, # oft "ASOL.Projects", wenn nicht gesetzt, wird aktueller
+Windows-Nutzer verwendet
+13  userDomain : null, # Domain fÃ¼r ASOL.PROJECTS
+14  password : null # das Passwort
+15}
+16dbserver : {
+17  server : "some-server",
+18  db : "APplusProd6",
+19  user : "SA",
+20  password : "your-db-password"
+21}
 Damit nicht in jedem Script immer wieder neu die Konfig-Dateien ausgewÃ¤hlt
 werden mÃ¼ssen, werden die Konfigs fÃ¼r das Prod-, Test- und Deploy-System in
 examples/applus_configs.py hinterlegt. Diese Datei wird in allen Scripten
 importiert, so dass das Config-Verzeichnis und die darin enthaltenen Configs
 einfach zur VerfÃ¼gung stehen.
 1import pathlib
 2
@@ -103,17 +107,19 @@
 39    print("  InstallPathAppServer:",
 server.scripttool.getInstallPathAppServer())
 40    print("  InstallPathWebServer:",
 server.scripttool.getInstallPathWebServer())
 41    print("  ServerInfo - Version:", server.scripttool.getServerInfo().find
 ("version").text)
 42
-43
-44if __name__ == "__main__":
-45    main(applus_configs.serverConfYamlTest)
+43    client = server.getWebClient("masterdata/artikel.asmx")
+44    print("ARTIKEL-ASMX Date:", client.service.getServerDate())
+45
+46if __name__ == "__main__":
+47    main(applus_configs.serverConfYamlTest)
 
 ***** check_dokumente.pyÂ¶ *****
 Einfaches Beispiel fÃ¼r lesenden und schreibenden Zugriff auf APplus Datenbank.
  1import pathlib
  2import PyAPplus64
  3import applus_configs
  4from typing import Optional
```

### Comparing `PyAPplus64-1.0.1/docs/build/html/generated/PyAPplus64.html` & `PyAPplus64-1.1.0/docs/build/html/generated/PyAPplus64.html`

 * *Files 0% similar despite different names*

```diff
@@ -45,23 +45,23 @@
 <section id="submodules">
 <h2>Submodules<a class="headerlink" href="#submodules" title="Link zu dieser Überschrift">¶</a></h2>
 </section>
 <section id="module-PyAPplus64.applus">
 <span id="pyapplus64-applus-module"></span><h2>PyAPplus64.applus module<a class="headerlink" href="#module-PyAPplus64.applus" title="Link zu dieser Überschrift">¶</a></h2>
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.applus.</span></span><span class="sig-name descname"><span class="pre">APplusServer</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">db_settings</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.applus_db.APplusDBSettings" title="PyAPplus64.applus_db.APplusDBSettings"><span class="pre">PyAPplus64.applus_db.APplusDBSettings</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">server_settings</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.applus_server.APplusAppServerSettings" title="PyAPplus64.applus_server.APplusAppServerSettings"><span class="pre">PyAPplus64.applus_server.APplusAppServerSettings</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">web_settings</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.applus_server.APplusWebServerSettings" title="PyAPplus64.applus_server.APplusWebServerSettings"><span class="pre">PyAPplus64.applus_server.APplusWebServerSettings</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.applus.APplusServer" title="Link zu dieser Definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.applus.</span></span><span class="sig-name descname"><span class="pre">APplusServer</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">db_settings</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.applus_db.APplusDBSettings" title="PyAPplus64.applus_db.APplusDBSettings"><span class="pre">PyAPplus64.applus_db.APplusDBSettings</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">server_settings</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.applus_server.APplusServerSettings" title="PyAPplus64.applus_server.APplusServerSettings"><span class="pre">PyAPplus64.applus_server.APplusServerSettings</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.applus.APplusServer" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>Verbindung zu einem APplus DB und App Server mit Hilfsfunktionen für den komfortablen Zugriff.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>db_settings</strong> (<a class="reference internal" href="#PyAPplus64.applus_db.APplusDBSettings" title="PyAPplus64.applus_db.APplusDBSettings"><em>APplusDBSettings</em></a>) – die Einstellungen für die Verbindung mit der Datenbank</p></li>
-<li><p><strong>server_settings</strong> (<a class="reference internal" href="#PyAPplus64.applus_server.APplusAppServerSettings" title="PyAPplus64.applus_server.APplusAppServerSettings"><em>APplusAppServerSettings</em></a>) – die Einstellungen für die Verbindung mit dem APplus App Server</p></li>
-<li><p><strong>web_settings</strong> (<a class="reference internal" href="#PyAPplus64.applus_server.APplusWebServerSettings" title="PyAPplus64.applus_server.APplusWebServerSettings"><em>APplusWebServerSettings</em></a>) – die Einstellungen für die Verbindung mit dem APplus Web Server</p></li>
+<li><p><strong>server_settings</strong> (<em>APplusAppServerSettings</em>) – die Einstellungen für die Verbindung mit dem APplus App Server</p></li>
+<li><p><strong>web_settings</strong> (<em>APplusWebServerSettings</em>) – die Einstellungen für die Verbindung mit dem APplus Web Server</p></li>
 </ul>
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.completeSQL">
 <span class="sig-name descname"><span class="pre">completeSQL</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">sql</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlStatementSelect" title="PyAPplus64.sql_utils.SqlStatementSelect"><span class="pre">PyAPplus64.sql_utils.SqlStatementSelect</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.completeSQL" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Vervollständigt das SQL-Statement. Es wird z.B. der Mandant hinzugefügt.</p>
@@ -80,56 +80,56 @@
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.dbQuery">
 <span class="sig-name descname"><span class="pre">dbQuery</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">sql</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlStatementSelect" title="PyAPplus64.sql_utils.SqlStatementSelect"><span class="pre">PyAPplus64.sql_utils.SqlStatementSelect</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">f</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">pyodbc.Row</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">None</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Any</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.dbQuery" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Führt eine SQL Query aus und führt für jede Zeile die übergeben Funktion aus. 
+<dd><p>Führt eine SQL Query aus und führt für jede Zeile die übergeben Funktion aus.
 Das SQL wird zunächst vom Server angepasst, so dass z.B. Mandanteninformation hinzugefügt werden.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.dbQueryAll">
 <span class="sig-name descname"><span class="pre">dbQueryAll</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">sql</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlStatementSelect" title="PyAPplus64.sql_utils.SqlStatementSelect"><span class="pre">PyAPplus64.sql_utils.SqlStatementSelect</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Any</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">apply</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">pyodbc.Row</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.dbQueryAll" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Führt eine SQL Query aus und liefert alle Zeilen zurück. Das SQL wird zunächst 
+<dd><p>Führt eine SQL Query aus und liefert alle Zeilen zurück. Das SQL wird zunächst
 vom Server angepasst, so dass z.B. Mandanteninformation hinzugefügt werden.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.dbQuerySingleRow">
 <span class="sig-name descname"><span class="pre">dbQuerySingleRow</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">sql</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlStatementSelect" title="PyAPplus64.sql_utils.SqlStatementSelect"><span class="pre">PyAPplus64.sql_utils.SqlStatementSelect</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Any</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">pyodbc.Row</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.dbQuerySingleRow" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Führt eine SQL Query aus, die maximal eine Zeile zurückliefern soll. Diese Zeile wird geliefert.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.dbQuerySingleRowDict">
 <span class="sig-name descname"><span class="pre">dbQuerySingleRowDict</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">sql</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlStatementSelect" title="PyAPplus64.sql_utils.SqlStatementSelect"><span class="pre">PyAPplus64.sql_utils.SqlStatementSelect</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Any</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.dbQuerySingleRowDict" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Führt eine SQL Query aus, die maximal eine Zeile zurückliefern soll. 
+<dd><p>Führt eine SQL Query aus, die maximal eine Zeile zurückliefern soll.
 Diese Zeile wird als Dictionary geliefert.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.dbQuerySingleValue">
 <span class="sig-name descname"><span class="pre">dbQuerySingleValue</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">sql</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlStatementSelect" title="PyAPplus64.sql_utils.SqlStatementSelect"><span class="pre">PyAPplus64.sql_utils.SqlStatementSelect</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Any</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.dbQuerySingleValue" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Führt eine SQL Query aus, die maximal einen Wert zurückliefern soll. 
+<dd><p>Führt eine SQL Query aus, die maximal einen Wert zurückliefern soll.
 Dieser Wert oder None wird geliefert.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.dbQuerySingleValues">
 <span class="sig-name descname"><span class="pre">dbQuerySingleValues</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">sql</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlStatementSelect" title="PyAPplus64.sql_utils.SqlStatementSelect"><span class="pre">PyAPplus64.sql_utils.SqlStatementSelect</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Any</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.dbQuerySingleValues" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Führt eine SQL Query aus, die nur eine Spalte zurückliefern soll.</p>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.db_conn">
 <span class="sig-name descname"><span class="pre">db_conn</span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.db_conn" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Eine pyodbc-Connection zur APplus DB. Diese muss genutzt werden, wenn mehrere Operationen in einer Transaktion
-genutzt werden sollen. Ansonsten sind die Hilfsmethoden wie <a class="reference internal" href="#PyAPplus64.applus.APplusServer.dbQuery" title="PyAPplus64.applus.APplusServer.dbQuery"><code class="xref py py-meth docutils literal notranslate"><span class="pre">APplusServer.dbQuery()</span></code></a> zu bevorzugen. 
+genutzt werden sollen. Ansonsten sind die Hilfsmethoden wie <a class="reference internal" href="#PyAPplus64.applus.APplusServer.dbQuery" title="PyAPplus64.applus.APplusServer.dbQuery"><code class="xref py py-meth docutils literal notranslate"><span class="pre">APplusServer.dbQuery()</span></code></a> zu bevorzugen.
 Diese Connection kann in Verbindung mit den Funktionen aus <a class="reference internal" href="#module-PyAPplus64.applus_db" title="PyAPplus64.applus_db"><code class="xref py py-mod docutils literal notranslate"><span class="pre">PyAPplus64.applus_db</span></code></a> genutzt werden.</p>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.db_settings">
 <span class="sig-name descname"><span class="pre">db_settings</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference internal" href="#PyAPplus64.applus_db.APplusDBSettings" title="PyAPplus64.applus_db.APplusDBSettings"><span class="pre">PyAPplus64.applus_db.APplusDBSettings</span></a></em><a class="headerlink" href="#PyAPplus64.applus.APplusServer.db_settings" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Die Einstellungen für die Datenbankverbindung</p>
@@ -137,19 +137,19 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.execUseXMLRowDelete">
 <span class="sig-name descname"><span class="pre">execUseXMLRowDelete</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">table</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.execUseXMLRowDelete" title="Link zu dieser Definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
-<dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.getClient">
-<span class="sig-name descname"><span class="pre">getClient</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">package</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">zeep.client.Client</span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.getClient" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Erzeugt einen zeep - Client.
-Mittels dieses Clients kann die WSDL Schnittstelle angesprochen werden.
-Wird als <em>package</em> „p2core“ und als <em>name</em> „Table“ verwendet und der 
+<dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.getAppClient">
+<span class="sig-name descname"><span class="pre">getAppClient</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">package</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">zeep.client.Client</span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.getAppClient" title="Link zu dieser Definition">¶</a></dt>
+<dd><p>Erzeugt einen zeep - Client für den APP-Server.
+Mittels dieses Clients kann eines WSDL Schnittstelle des APP-Servers angesprochen werden.
+Wird als <em>package</em> „p2core“ und als <em>name</em> „Table“ verwendet und der
 resultierende client „client“ genannt, dann kann
 z.B. mittels „client.service.getCompleteSQL(sql)“ vom AppServer ein Vervollständigen
 des SQLs angefordert werden.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>package</strong> (<em>string</em>) – das Packet, z.B. „p2core“</p></li>
@@ -184,21 +184,41 @@
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.getUniqueFieldsOfTable">
 <span class="sig-name descname"><span class="pre">getUniqueFieldsOfTable</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">table</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.getUniqueFieldsOfTable" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Liefert alle Spalten einer Tabelle, die eindeutig sein müssen. 
-Diese werden als Dictionary gruppiert nach Index-Namen geliefert. 
-Jeder Eintrag enthält eine Liste von Feldern, die zusammen eindeutig sein 
+<dd><p>Liefert alle Spalten einer Tabelle, die eindeutig sein müssen.
+Diese werden als Dictionary gruppiert nach Index-Namen geliefert.
+Jeder Eintrag enthält eine Liste von Feldern, die zusammen eindeutig sein
 müssen.</p>
 </dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.getWebClient">
+<span class="sig-name descname"><span class="pre">getWebClient</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">url</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">zeep.client.Client</span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.getWebClient" title="Link zu dieser Definition">¶</a></dt>
+<dd><p>Erzeugt einen zeep - Client für den Web-Server.
+Mittels dieses Clients kann die von einer ASMX-Seite zur Verfügung gestellte Schnittstelle angesprochen werden.
+Als parameter wird die relative URL der ASMX-Seite erwartet. Die Base-URL automatisch ergänzt.
+Ein Beispiel für eine solche relative URL ist „masterdata/artikel.asmx“.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameter</dt>
+<dd class="field-odd"><p><strong>url</strong> – die relative URL der ASMX Seite, z.B. „masterdata/artikel.asmx“</p>
+</dd>
+<dt class="field-even">Rückgabe</dt>
+<dd class="field-even"><p>den Client</p>
+</dd>
+<dt class="field-odd">Rückgabetyp</dt>
+<dd class="field-odd"><p>Client</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.isDBTableKnown">
 <span class="sig-name descname"><span class="pre">isDBTableKnown</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">table</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.isDBTableKnown" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Prüft, ob eine Tabelle im System bekannt ist</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.makeWebLink">
@@ -284,31 +304,31 @@
 <dl class="py attribute">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.server_conn">
 <span class="sig-name descname"><span class="pre">server_conn</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference internal" href="#PyAPplus64.applus_server.APplusServerConnection" title="PyAPplus64.applus_server.APplusServerConnection"><span class="pre">PyAPplus64.applus_server.APplusServerConnection</span></a></em><a class="headerlink" href="#PyAPplus64.applus.APplusServer.server_conn" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>erlaubt den Zugriff auf den AppServer</p>
 </dd></dl>
 
 <dl class="py attribute">
+<dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.server_settings">
+<span class="sig-name descname"><span class="pre">server_settings</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference internal" href="#PyAPplus64.applus_server.APplusServerSettings" title="PyAPplus64.applus_server.APplusServerSettings"><span class="pre">PyAPplus64.applus_server.APplusServerSettings</span></a></em><a class="headerlink" href="#PyAPplus64.applus.APplusServer.server_settings" title="Link zu dieser Definition">¶</a></dt>
+<dd><p>Einstellung für die Verbindung zum APP- und Webserver</p>
+</dd></dl>
+
+<dl class="py attribute">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.sysconf">
 <span class="sig-name descname"><span class="pre">sysconf</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference internal" href="#PyAPplus64.applus_sysconf.APplusSysConf" title="PyAPplus64.applus_sysconf.APplusSysConf"><span class="pre">PyAPplus64.applus_sysconf.APplusSysConf</span></a></em><a class="headerlink" href="#PyAPplus64.applus.APplusServer.sysconf" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>erlaubt den Zugriff auf die Sysconfig</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.useXML">
 <span class="sig-name descname"><span class="pre">useXML</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">xml</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span></span></span><a class="headerlink" href="#PyAPplus64.applus.APplusServer.useXML" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Ruft <code class="docutils literal notranslate"><span class="pre">p2core.xml.usexml</span></code> auf. Wird meist durch ein <code class="docutils literal notranslate"><span class="pre">UseXMLRow-Objekt</span></code> aufgerufen.</p>
 </dd></dl>
 
-<dl class="py attribute">
-<dt class="sig sig-object py" id="PyAPplus64.applus.APplusServer.web_settings">
-<span class="sig-name descname"><span class="pre">web_settings</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference internal" href="#PyAPplus64.applus_server.APplusWebServerSettings" title="PyAPplus64.applus_server.APplusWebServerSettings"><span class="pre">PyAPplus64.applus_server.APplusWebServerSettings</span></a></em><a class="headerlink" href="#PyAPplus64.applus.APplusServer.web_settings" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Die Einstellungen für die Datenbankverbindung</p>
-</dd></dl>
-
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="PyAPplus64.applus.applusFromConfig">
 <span class="sig-prename descclassname"><span class="pre">PyAPplus64.applus.</span></span><span class="sig-name descname"><span class="pre">applusFromConfig</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">yamlString</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">user</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">env</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#PyAPplus64.applus.APplusServer" title="PyAPplus64.applus.APplusServer"><span class="pre">PyAPplus64.applus.APplusServer</span></a></span></span><a class="headerlink" href="#PyAPplus64.applus.applusFromConfig" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Läd Einstellungen aus einer Config-Datei und erzeugt daraus ein APplus-Objekt</p>
 </dd></dl>
@@ -382,17 +402,17 @@
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="PyAPplus64.applus_db.getUniqueFieldsOfTable">
 <span class="sig-prename descclassname"><span class="pre">PyAPplus64.applus_db.</span></span><span class="sig-name descname"><span class="pre">getUniqueFieldsOfTable</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">cnxn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">pyodbc.Connection</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">table</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.applus_db.getUniqueFieldsOfTable" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Liefert alle Spalten einer Tabelle, die eindeutig sein müssen. 
-Diese werden als Dictionary gruppiert nach Index-Namen geliefert. 
-Jeder Eintrag enthält eine Liste von Feldern, die zusammen eindeutig sein 
+<dd><p>Liefert alle Spalten einer Tabelle, die eindeutig sein müssen.
+Diese werden als Dictionary gruppiert nach Index-Namen geliefert.
+Jeder Eintrag enthält eine Liste von Feldern, die zusammen eindeutig sein
 müssen.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="PyAPplus64.applus_db.rawQuery">
 <span class="sig-prename descclassname"><span class="pre">PyAPplus64.applus_db.</span></span><span class="sig-name descname"><span class="pre">rawQuery</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">cnxn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">pyodbc.Connection</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sql</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlStatementSelect" title="PyAPplus64.sql_utils.SqlStatementSelect"><span class="pre">PyAPplus64.sql_utils.SqlStatementSelect</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">f</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">pyodbc.Row</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">None</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Any</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.applus_db.rawQuery" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Führt eine SQL Query direkt aus und führt für jede Zeile die übergeben Funktion aus.</p>
@@ -448,14 +468,32 @@
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_scripttool.APplusScriptTool.getCurrentTime">
 <span class="sig-name descname"><span class="pre">getCurrentTime</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.applus_scripttool.APplusScriptTool.getCurrentTime" title="Link zu dieser Definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="PyAPplus64.applus_scripttool.APplusScriptTool.getInstallPath">
+<span class="sig-name descname"><span class="pre">getInstallPath</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.applus_scripttool.APplusScriptTool.getInstallPath" title="Link zu dieser Definition">¶</a></dt>
+<dd><p>Liefert den Installionspfad des Appservers</p>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="PyAPplus64.applus_scripttool.APplusScriptTool.getInstallPathAppServer">
+<span class="sig-name descname"><span class="pre">getInstallPathAppServer</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">pathlib.Path</span></span></span><a class="headerlink" href="#PyAPplus64.applus_scripttool.APplusScriptTool.getInstallPathAppServer" title="Link zu dieser Definition">¶</a></dt>
+<dd><p>Liefert den Installionspfad des Appservers als PathLib-Path</p>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="PyAPplus64.applus_scripttool.APplusScriptTool.getInstallPathWebServer">
+<span class="sig-name descname"><span class="pre">getInstallPathWebServer</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">pathlib.Path</span></span></span><a class="headerlink" href="#PyAPplus64.applus_scripttool.APplusScriptTool.getInstallPathWebServer" title="Link zu dieser Definition">¶</a></dt>
+<dd><p>Liefert den Installionspfad des Webservers als PathLib-Path</p>
+</dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_scripttool.APplusScriptTool.getLoginName">
 <span class="sig-name descname"><span class="pre">getLoginName</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.applus_scripttool.APplusScriptTool.getLoginName" title="Link zu dieser Definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_scripttool.APplusScriptTool.getMandant">
 <span class="sig-name descname"><span class="pre">getMandant</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.applus_scripttool.APplusScriptTool.getMandant" title="Link zu dieser Definition">¶</a></dt>
@@ -465,14 +503,42 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_scripttool.APplusScriptTool.getMandantName">
 <span class="sig-name descname"><span class="pre">getMandantName</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.applus_scripttool.APplusScriptTool.getMandantName" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Liefert den Namen des aktuellen Mandanten</p>
 </dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="PyAPplus64.applus_scripttool.APplusScriptTool.getServerInfo">
+<span class="sig-name descname"><span class="pre">getServerInfo</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">lxml.etree.Element</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.applus_scripttool.APplusScriptTool.getServerInfo" title="Link zu dieser Definition">¶</a></dt>
+<dd><p>Liefert Informationen zum Server als ein XML Dokument.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Rückgabe</dt>
+<dd class="field-odd"><p>das gefundene und geparste XML-Dokument</p>
+</dd>
+<dt class="field-even">Rückgabetyp</dt>
+<dd class="field-even"><p>ET.Element</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py method">
+<dt class="sig sig-object py" id="PyAPplus64.applus_scripttool.APplusScriptTool.getServerInfoString">
+<span class="sig-name descname"><span class="pre">getServerInfoString</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.applus_scripttool.APplusScriptTool.getServerInfoString" title="Link zu dieser Definition">¶</a></dt>
+<dd><p>Liefert Informationen zum Server als String. Dieser String repräsentiert ein XML Dokument.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Rückgabe</dt>
+<dd class="field-odd"><p>das XML-Dokument als String</p>
+</dd>
+<dt class="field-even">Rückgabetyp</dt>
+<dd class="field-even"><p>str</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_scripttool.APplusScriptTool.getSystemName">
 <span class="sig-name descname"><span class="pre">getSystemName</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.applus_scripttool.APplusScriptTool.getSystemName" title="Link zu dieser Definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_scripttool.APplusScriptTool.getUserFullName">
 <span class="sig-name descname"><span class="pre">getUserFullName</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.applus_scripttool.APplusScriptTool.getUserFullName" title="Link zu dieser Definition">¶</a></dt>
@@ -491,37 +557,37 @@
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>obj</strong> (<em>str</em>) – das Objekt, dessen Definition zu laden ist, „Artikel“ läd z.B. „ArtikelDefinition.xml“</p></li>
 <li><p><strong>mandant</strong> (<em>str optional</em>) – der Mandant, dessen XML-Doku geladen werden soll, wenn „“ wird der Standard-Mandant verwendet</p></li>
 </ul>
 </dd>
 <dt class="field-even">Rückgabe</dt>
-<dd class="field-even"><p>das gefundene und mittels ElementTree geparste XML-Dokument</p>
+<dd class="field-even"><p>das gefundene und geparste XML-Dokument</p>
 </dd>
 <dt class="field-odd">Rückgabetyp</dt>
 <dd class="field-odd"><p>ET.Element</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_scripttool.APplusScriptTool.getXMLDefinitionObj">
 <span class="sig-name descname"><span class="pre">getXMLDefinitionObj</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">obj</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">mandant</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">''</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.applus_scripttool.XMLDefinition" title="PyAPplus64.applus_scripttool.XMLDefinition"><span class="pre">PyAPplus64.applus_scripttool.XMLDefinition</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.applus_scripttool.APplusScriptTool.getXMLDefinitionObj" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Benutzt getXMLDefinitionObj und liefert den Top-Level „Object“ Knoten zurück, falls zusätzlich 
+<dd><p>Benutzt getXMLDefinitionObj und liefert den Top-Level „Object“ Knoten zurück, falls zusätzlich
 ein MD5 Knoten existiert, also falls das Dokument wirklich vom Dateisystem geladen werden konnte.
 Ansonten wird None geliefert.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>obj</strong> (<em>str</em>) – das Objekt, dess Definition zu laden ist, „Artikel“ läd z.B. „ArtikelDefinition.xml“</p></li>
 <li><p><strong>mandant</strong> (<em>str optional</em>) – der Mandant, dessen XML-Doku geladen werden soll, wenn „“ wird der Standard-Mandant verwendet</p></li>
 </ul>
 </dd>
 <dt class="field-even">Rückgabe</dt>
-<dd class="field-even"><p>das gefundene und mittels ElementTree geparste XML-Dokument</p>
+<dd class="field-even"><p>das gefundene und geparste XML-Dokument</p>
 </dd>
 <dt class="field-odd">Rückgabetyp</dt>
 <dd class="field-odd"><p>Optional[<a class="reference internal" href="#PyAPplus64.applus_scripttool.XMLDefinition" title="PyAPplus64.applus_scripttool.XMLDefinition">XMLDefinition</a>]</p>
 </dd>
 </dl>
 </dd></dl>
 
@@ -571,36 +637,29 @@
 
 </dd></dl>
 
 </section>
 <section id="module-PyAPplus64.applus_server">
 <span id="pyapplus64-applus-server-module"></span><h2>PyAPplus64.applus_server module<a class="headerlink" href="#module-PyAPplus64.applus_server" title="Link zu dieser Überschrift">¶</a></h2>
 <dl class="py class">
-<dt class="sig sig-object py" id="PyAPplus64.applus_server.APplusAppServerSettings">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.applus_server.</span></span><span class="sig-name descname"><span class="pre">APplusAppServerSettings</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">appserver</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">appserverPort</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">user</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">env</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.applus_server.APplusAppServerSettings" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
-<p>Einstellungen, mit welchem APplus App-Server sich verbunden werden soll.</p>
-</dd></dl>
-
-<dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.applus_server.APplusServerConnection">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.applus_server.</span></span><span class="sig-name descname"><span class="pre">APplusServerConnection</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">settings</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.applus_server.APplusAppServerSettings" title="PyAPplus64.applus_server.APplusAppServerSettings"><span class="pre">PyAPplus64.applus_server.APplusAppServerSettings</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.applus_server.APplusServerConnection" title="Link zu dieser Definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.applus_server.</span></span><span class="sig-name descname"><span class="pre">APplusServerConnection</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">settings</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.applus_server.APplusServerSettings" title="PyAPplus64.applus_server.APplusServerSettings"><span class="pre">PyAPplus64.applus_server.APplusServerSettings</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.applus_server.APplusServerConnection" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
-<p>Verbindung zu einem APplus APP-Server</p>
+<p>Verbindung zu einem APplus APP- und Web-Server</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
-<dd class="field-odd"><p><strong>settings</strong> (<a class="reference internal" href="#PyAPplus64.applus_server.APplusAppServerSettings" title="PyAPplus64.applus_server.APplusAppServerSettings"><em>APplusAppServerSettings</em></a>) – die Einstellungen für die Verbindung mit dem APplus Server</p>
+<dd class="field-odd"><p><strong>settings</strong> (<em>APplusAppServerSettings</em>) – die Einstellungen für die Verbindung mit dem APplus Server</p>
 </dd>
 </dl>
 <dl class="py method">
-<dt class="sig sig-object py" id="PyAPplus64.applus_server.APplusServerConnection.getClient">
-<span class="sig-name descname"><span class="pre">getClient</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">package</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">zeep.client.Client</span></span></span><a class="headerlink" href="#PyAPplus64.applus_server.APplusServerConnection.getClient" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Erzeugt einen zeep - Client.
+<dt class="sig sig-object py" id="PyAPplus64.applus_server.APplusServerConnection.getAppClient">
+<span class="sig-name descname"><span class="pre">getAppClient</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">package</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">zeep.client.Client</span></span></span><a class="headerlink" href="#PyAPplus64.applus_server.APplusServerConnection.getAppClient" title="Link zu dieser Definition">¶</a></dt>
+<dd><p>Erzeugt einen zeep - Client für den APP-Server.
 Mittels dieses Clients kann die WSDL Schnittstelle angesprochen werden.
-Wird als <em>package</em> „p2core“ und als <em>name</em> „Table“ verwendet und der 
+Wird als <em>package</em> „p2core“ und als <em>name</em> „Table“ verwendet und der
 resultierende client „client“ genannt, dann kann
 z.B. mittels „client.service.getCompleteSQL(sql)“ vom AppServer ein Vervollständigen
 des SQLs angefordert werden.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>package</strong> (<em>string</em>) – das Packet, z.B. „p2core“</p></li>
@@ -612,21 +671,41 @@
 </dd>
 <dt class="field-odd">Rückgabetyp</dt>
 <dd class="field-odd"><p>Client</p>
 </dd>
 </dl>
 </dd></dl>
 
+<dl class="py method">
+<dt class="sig sig-object py" id="PyAPplus64.applus_server.APplusServerConnection.getWebClient">
+<span class="sig-name descname"><span class="pre">getWebClient</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">url</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">zeep.client.Client</span></span></span><a class="headerlink" href="#PyAPplus64.applus_server.APplusServerConnection.getWebClient" title="Link zu dieser Definition">¶</a></dt>
+<dd><p>Erzeugt einen zeep - Client für den Web-Server.
+Mittels dieses Clients kann die von einer ASMX-Seite zur Verfügung gestellte Schnittstelle angesprochen werden.
+Als parameter wird die relative URL der ASMX-Seite erwartet. Die Base-URL automatisch ergänzt.
+Ein Beispiel für eine solche relative URL ist „masterdata/artikel.asmx“.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameter</dt>
+<dd class="field-odd"><p><strong>url</strong> – die relative URL der ASMX Seite, z.B. „masterdata/artikel.asmx“</p>
+</dd>
+<dt class="field-even">Rückgabe</dt>
+<dd class="field-even"><p>den Client</p>
+</dd>
+<dt class="field-odd">Rückgabetyp</dt>
+<dd class="field-odd"><p>Client</p>
+</dd>
+</dl>
+</dd></dl>
+
 </dd></dl>
 
 <dl class="py class">
-<dt class="sig sig-object py" id="PyAPplus64.applus_server.APplusWebServerSettings">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.applus_server.</span></span><span class="sig-name descname"><span class="pre">APplusWebServerSettings</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">baseurl</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.applus_server.APplusWebServerSettings" title="Link zu dieser Definition">¶</a></dt>
+<dt class="sig sig-object py" id="PyAPplus64.applus_server.APplusServerSettings">
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.applus_server.</span></span><span class="sig-name descname"><span class="pre">APplusServerSettings</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">webserver</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">appserver</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">appserverPort</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">user</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">env</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">webserverUser</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">webserverUserDomain</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">webserverPassword</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.applus_server.APplusServerSettings" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
-<p>Einstellungen, mit welchem APplus Web-Server sich verbunden werden soll.</p>
+<p>Einstellungen, mit welchem APplus App- and Web-Server sich verbunden werden soll.</p>
 </dd></dl>
 
 </section>
 <section id="module-PyAPplus64.applus_sysconf">
 <span id="pyapplus64-applus-sysconf-module"></span><h2>PyAPplus64.applus_sysconf module<a class="headerlink" href="#module-PyAPplus64.applus_sysconf" title="Link zu dieser Überschrift">¶</a></h2>
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.applus_sysconf.APplusSysConf">
@@ -673,53 +752,53 @@
 </section>
 <section id="module-PyAPplus64.applus_usexml">
 <span id="pyapplus64-applus-usexml-module"></span><h2>PyAPplus64.applus_usexml module<a class="headerlink" href="#module-PyAPplus64.applus_usexml" title="Link zu dieser Überschrift">¶</a></h2>
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.applus_usexml.UseXmlRow">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.applus_usexml.</span></span><span class="sig-name descname"><span class="pre">UseXmlRow</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">applus</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">APplusServer</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">table</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cmd</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.applus_usexml.UseXmlRow" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
-<p>Klasse, die eine XML-Datei erzeugen kann, die mittels p2core.useXML 
+<p>Klasse, die eine XML-Datei erzeugen kann, die mittels p2core.useXML
 genutzt werden kann. Damit ist es möglich APplus BusinessObjekte zu
 erzeugen, ändern und zu löschen. Im Gegensatz zu direkten DB-Zugriffen,
 werden diese Anfragen über den APP-Server ausgeführt. Dabei werden
 die von der Weboberfläche bekannten Checks und Änderungen ausgeführt.
 Als sehr einfaches Beispiel wird z.B. INSDATE oder UPDDATE automatisch gesetzt.
 Interessanter sind automatische Änderungen und Checks.</p>
-<p>Bei der Benutzung wird zunächst ein Objekt erzeugt, dann evtl. 
-mittels <a class="reference internal" href="#PyAPplus64.applus_usexml.UseXmlRow.addField" title="PyAPplus64.applus_usexml.UseXmlRow.addField"><code class="xref py py-meth docutils literal notranslate"><span class="pre">addField()</span></code></a> Felder hinzugefügt und schließlich mittels 
-<a class="reference internal" href="#PyAPplus64.applus_usexml.UseXmlRow.exec" title="PyAPplus64.applus_usexml.UseXmlRow.exec"><code class="xref py py-meth docutils literal notranslate"><span class="pre">exec()</span></code></a> an den AppServer übergeben. 
+<p>Bei der Benutzung wird zunächst ein Objekt erzeugt, dann evtl.
+mittels <a class="reference internal" href="#PyAPplus64.applus_usexml.UseXmlRow.addField" title="PyAPplus64.applus_usexml.UseXmlRow.addField"><code class="xref py py-meth docutils literal notranslate"><span class="pre">addField()</span></code></a> Felder hinzugefügt und schließlich mittels
+<a class="reference internal" href="#PyAPplus64.applus_usexml.UseXmlRow.exec" title="PyAPplus64.applus_usexml.UseXmlRow.exec"><code class="xref py py-meth docutils literal notranslate"><span class="pre">exec()</span></code></a> an den AppServer übergeben.
 Normalerweise sollte die Klasse nicht direkt, sondern über Unterklassen
 für das Einfügen, Ändern oder Löschen benutzt werden.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>applus</strong> (<a class="reference internal" href="#PyAPplus64.applus.APplusServer" title="PyAPplus64.applus.APplusServer"><em>APplusServer</em></a>) – Verbindung zu APplus</p></li>
 <li><p><strong>table</strong> (<em>str</em>) – die Tabelle</p></li>
 <li><p><strong>cmd</strong> (<em>str</em>) – cmd-attribut der row, also ob es sich um ein Update, ein Insert oder ein Delete handelt</p></li>
 </ul>
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_usexml.UseXmlRow.addField">
-<span class="sig-name descname"><span class="pre">addField</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Any</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.applus_usexml.UseXmlRow.addField" title="Link zu dieser Definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">addField</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Any</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.applus_usexml.UseXmlRow.addField" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Fügt ein Feld zum Row-Node hinzu.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>name</strong> (<em>string</em>) – das Feld</p></li>
 <li><p><strong>value</strong> – Wert des Feldes</p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_usexml.UseXmlRow.addTimestampField">
 <span class="sig-name descname"><span class="pre">addTimestampField</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ts</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.applus_usexml.UseXmlRow.addTimestampField" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Fügt ein Timestamp-Feld hinzu. Wird kein Timestamp übergeben, wird mittels der ID der aktuelle 
+<dd><p>Fügt ein Timestamp-Feld hinzu. Wird kein Timestamp übergeben, wird mittels der ID der aktuelle
 Timestamp aus der DB geladen. Dabei kann ein Fehler auftreten.
 Ein Timestamp-Feld ist für Updates und das Löschen nötig um sicherzustellen, dass die richtige
 Version des Objekts geändert oder gelöscht wird. Wird z.B. ein Objekt aus der DB geladen, inspiziert
 und sollen dann Änderungen gespeichert werden, so sollte der Timestamp des Ladens übergeben werden.
 So wird sichergestellt, dass nicht ein anderer User zwischenzeitlich Änderungen vornahm. Ist dies
 der Fall, wird dann bei „exec“ eine Exception geworfen.</p>
 <dl class="field-list simple">
@@ -731,15 +810,15 @@
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_usexml.UseXmlRow.addTimestampIDFields">
 <span class="sig-name descname"><span class="pre">addTimestampIDFields</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">id</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ts</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.applus_usexml.UseXmlRow.addTimestampIDFields" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Fügt ein Timestamp-Feld sowie ein Feld id hinzu. Wird kein Timestamp übergeben, wird mittels der ID der aktuelle 
+<dd><p>Fügt ein Timestamp-Feld sowie ein Feld id hinzu. Wird kein Timestamp übergeben, wird mittels der ID der aktuelle
 Timestamp aus der DB geladen. Dabei kann ein Fehler auftreten. Intern wird <a class="reference internal" href="#PyAPplus64.applus_usexml.UseXmlRow.addTimestampField" title="PyAPplus64.applus_usexml.UseXmlRow.addTimestampField"><code class="xref py py-meth docutils literal notranslate"><span class="pre">addTimestampField()</span></code></a> benutzt.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>id</strong> (<em>string</em>) – DB-id des Objektes dessen Timestamp hinzugefügt werden soll</p></li>
 <li><p><strong>ts</strong> (<em>bytes</em>) – Fester Timestamp der verwendet werden soll, wenn None wird der Timestamp aus der DB geladen.</p></li>
 </ul>
@@ -771,15 +850,15 @@
 <span class="sig-name descname"><span class="pre">getField</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span></span></span><a class="headerlink" href="#PyAPplus64.applus_usexml.UseXmlRow.getField" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Liefert den Wert eines gesetzten Feldes</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_usexml.UseXmlRow.toprettyxml">
 <span class="sig-name descname"><span class="pre">toprettyxml</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.applus_usexml.UseXmlRow.toprettyxml" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Gibt das formatierte XML aus. Dieses kann per useXML an den AppServer übergeben werden. 
+<dd><p>Gibt das formatierte XML aus. Dieses kann per useXML an den AppServer übergeben werden.
 Dies wird mittels <a class="reference internal" href="#PyAPplus64.applus_usexml.UseXmlRow.exec" title="PyAPplus64.applus_usexml.UseXmlRow.exec"><code class="xref py py-meth docutils literal notranslate"><span class="pre">exec()</span></code></a> automatisiert.</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.applus_usexml.UseXmlRowDelete">
@@ -832,28 +911,28 @@
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.applus_usexml.UseXmlRowInsertOrUpdate">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.applus_usexml.</span></span><span class="sig-name descname"><span class="pre">UseXmlRowInsertOrUpdate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">applus</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">APplusServer</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">table</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.applus_usexml.UseXmlRowInsertOrUpdate" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#PyAPplus64.applus_usexml.UseXmlRow" title="PyAPplus64.applus_usexml.UseXmlRow"><code class="xref py py-class docutils literal notranslate"><span class="pre">PyAPplus64.applus_usexml.UseXmlRow</span></code></a></p>
 <p>Klasse, die eine XML-Datei für das Einfügen oder Ändern eines neuen Datensatzes, erzeugen kann.
 Die Methode <cite>checkExists</cite> erlaubt es zu prüfen, ob ein Objekt bereits existiert. Dafür werden die
 gesetzten Felder mit den Feldern aus eindeutigen Indices verglichen. Existiert ein Objekt bereits, wird
-ein Update ausgeführt, ansonsten ein Insert. Bei Updates werden die Felder <cite>id</cite> und <cite>timestamp</cite> 
+ein Update ausgeführt, ansonsten ein Insert. Bei Updates werden die Felder <cite>id</cite> und <cite>timestamp</cite>
 automatisch gesetzt.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>applus</strong> (<a class="reference internal" href="#PyAPplus64.applus.APplusServer" title="PyAPplus64.applus.APplusServer"><em>APplusServer</em></a>) – Verbindung zu APplus</p></li>
 <li><p><strong>table</strong> (<em>string</em>) – die Tabelle</p></li>
 </ul>
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_usexml.UseXmlRowInsertOrUpdate.checkExists">
-<span class="sig-name descname"><span class="pre">checkExists</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">int</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.applus_usexml.UseXmlRowInsertOrUpdate.checkExists" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Prüft, ob der Datensatz bereits in der DB existiert. 
+<span class="sig-name descname"><span class="pre">checkExists</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">int</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.applus_usexml.UseXmlRowInsertOrUpdate.checkExists" title="Link zu dieser Definition">¶</a></dt>
+<dd><p>Prüft, ob der Datensatz bereits in der DB existiert.
 Ist dies der Fall, wird die ID geliefert, sonst None</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.applus_usexml.UseXmlRowInsertOrUpdate.exec">
 <span class="sig-name descname"><span class="pre">exec</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">int</span></span></span><a class="headerlink" href="#PyAPplus64.applus_usexml.UseXmlRowInsertOrUpdate.exec" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Führt entweder ein Update oder ein Insert durch. Dies hängt davon ab, ob das Objekt bereits in
@@ -916,25 +995,25 @@
 <dt class="sig sig-object py" id="PyAPplus64.duplicate.DuplicateBusinessObject">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.duplicate.</span></span><span class="sig-name descname"><span class="pre">DuplicateBusinessObject</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">table</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fields</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fieldsNotCopied</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">{}</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">allowUpdate</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.duplicate.DuplicateBusinessObject" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>Klasse, die alle Daten zu einem BusinessObject speichert und zum Duplizieren dieses Objektes dient.
 Dies beinhaltet Daten zu abhängigen Objekten sowie die Beziehung zu diesen Objekten. Zu einem Artikel
 wird z.B. der Arbeitsplan gespeichert, der wiederum Arbeitsplanpositionen enthält. Als Beziehung ist u.a.
 hinterlegt, dass das Feld „APLAN“ der Arbeitsplans dem Feld „ARTIKEL“ des Artikels entsprechen muss und dass
-„APLAN“ aus den Positionen, „APLAN“ aus dem APlan entsprichen muss. So kann beim Duplizieren ein 
+„APLAN“ aus den Positionen, „APLAN“ aus dem APlan entsprichen muss. So kann beim Duplizieren ein
 anderer Name des Artikels gesetzt werden und automatisch die Felder der abhängigen Objekte angepasst werden.
 Einige Felder der Beziehung sind dabei statisch, d.h. können direkt aus den zu speichernden Daten abgelesen werden.
-Andere Felder sind dynamisch, d.h. das Parent-Objekt muss in der DB angelegt werden, damit ein solcher dynamischer Wert erstellt 
+Andere Felder sind dynamisch, d.h. das Parent-Objekt muss in der DB angelegt werden, damit ein solcher dynamischer Wert erstellt
 und geladen werden kann. Ein typisches Beispiel für ein dynamisches Feld ist „GUID“.</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.duplicate.DuplicateBusinessObject.addDependentBusinessObject">
 <span class="sig-name descname"><span class="pre">addDependentBusinessObject</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">dObj</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.duplicate.DuplicateBusinessObject" title="PyAPplus64.duplicate.DuplicateBusinessObject"><span class="pre">PyAPplus64.duplicate.DuplicateBusinessObject</span></a><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.duplicate.DuplicateBusinessObject.addDependentBusinessObject" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Fügt ein neues Unterobjekt zum DuplicateBusinessObject hinzu.
 Dabei handelt es sich selbst um ein DuplicateBusinessObject, das zusammen mit dem
-Parent-Objekt dupliziert werden sollen. Zum Beispiel sollen zu einem 
+Parent-Objekt dupliziert werden sollen. Zum Beispiel sollen zu einem
 Auftrag auch die Positionen dupliziert werden.
 Zusätzlich zum Objekt selbst können mehrere (keine, eine oder viele)
 Paare von Feldern übergeben werden. Ein Paar („pf“, „sf“) verbindet das
 Feld „pf“ des Parent-Objekts mit dem Feld „sf“ des Sub-Objekts. So ist es möglich,
 Werte des Parent-Objekts zu ändern und diese Änderungen für Sub-Objekte zu übernehmen.
 Üblicherweise muss zum Beispiel die Nummer des Hauptobjekts geändert werden. Die
 gleiche Änderung ist für alle abhängigen  Objekte nötig, damit die neuen Objekte sich auf das
@@ -972,15 +1051,15 @@
 <span class="sig-name descname"><span class="pre">fieldsNotCopied</span></span><a class="headerlink" href="#PyAPplus64.duplicate.DuplicateBusinessObject.fieldsNotCopied" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Datenfelder, die im Original vorhanden sind, aber nicht kopiert werden sollen</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.duplicate.DuplicateBusinessObject.getField">
 <span class="sig-name descname"><span class="pre">getField</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">field</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">onlyCopied</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span></span></span><a class="headerlink" href="#PyAPplus64.duplicate.DuplicateBusinessObject.getField" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Schlägt den Wert eines Feldes nach. Wenn onlyCopied gesetzt ist, werden nur Felder zurückgeliefert, die auch kopiert 
+<dd><p>Schlägt den Wert eines Feldes nach. Wenn onlyCopied gesetzt ist, werden nur Felder zurückgeliefert, die auch kopiert
 werden sollen.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.duplicate.DuplicateBusinessObject.insert">
 <span class="sig-name descname"><span class="pre">insert</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">server</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.applus.APplusServer" title="PyAPplus64.applus.APplusServer"><span class="pre">PyAPplus64.applus.APplusServer</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#PyAPplus64.applus_db.DBTableIDs" title="PyAPplus64.applus_db.DBTableIDs"><span class="pre">PyAPplus64.applus_db.DBTableIDs</span></a></span></span><a class="headerlink" href="#PyAPplus64.duplicate.DuplicateBusinessObject.insert" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Fügt alle Objekte zur DB hinzu. Es wird die Menge der IDs der erzeugten
@@ -1014,15 +1093,15 @@
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.duplicate.</span></span><span class="sig-name descname"><span class="pre">FieldsToCopyForTableCache</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">server</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.applus.APplusServer" title="PyAPplus64.applus.APplusServer"><span class="pre">PyAPplus64.applus.APplusServer</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.duplicate.FieldsToCopyForTableCache" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>Cache für welche Felder für welche Tabelle kopiert werden sollen</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.duplicate.FieldsToCopyForTableCache.getFieldsToCopyForTable">
 <span class="sig-name descname"><span class="pre">getFieldsToCopyForTable</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">table</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Set</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.duplicate.FieldsToCopyForTableCache.getFieldsToCopyForTable" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bestimmt die für eine Tabelle zu kopierenden Spalten. Dazu wird in den XML-Definitionen geschaut.
-Ist dort ‚include‘ hinterlegt, werden diese Spalten verwendet. Ansonsten alle nicht generierten Spalten, 
+Ist dort ‚include‘ hinterlegt, werden diese Spalten verwendet. Ansonsten alle nicht generierten Spalten,
 ohne die ‚exclude‘ Spalten. In jedem Fall werden Spalten wie „ID“, die nie kopiert werden sollten, entfernt.</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="PyAPplus64.duplicate.addSachgruppeDependentObjects">
@@ -1039,15 +1118,15 @@
 </dl>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="PyAPplus64.duplicate.getFieldsToCopyForTable">
 <span class="sig-prename descclassname"><span class="pre">PyAPplus64.duplicate.</span></span><span class="sig-name descname"><span class="pre">getFieldsToCopyForTable</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">server</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.applus.APplusServer" title="PyAPplus64.applus.APplusServer"><span class="pre">PyAPplus64.applus.APplusServer</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">table</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">force</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Set</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.duplicate.getFieldsToCopyForTable" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bestimmt die für eine Tabelle zu kopierenden Spalten. Dazu wird in den XML-Definitionen geschaut.
-Ist dort ‚include‘ hinterlegt, werden diese Spalten verwendet. Ansonsten alle nicht generierten Spalten, 
+Ist dort ‚include‘ hinterlegt, werden diese Spalten verwendet. Ansonsten alle nicht generierten Spalten,
 ohne die ‚exclude‘ Spalten. In jedem Fall werden Spalten wie „ID“, die nie kopiert werden sollten, entfernt.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="PyAPplus64.duplicate.initFieldsToCopyForTableCacheIfNeeded">
 <span class="sig-prename descclassname"><span class="pre">PyAPplus64.duplicate.</span></span><span class="sig-name descname"><span class="pre">initFieldsToCopyForTableCacheIfNeeded</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">server</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.applus.APplusServer" title="PyAPplus64.applus.APplusServer"><span class="pre">PyAPplus64.applus.APplusServer</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">cache</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.duplicate.FieldsToCopyForTableCache" title="PyAPplus64.duplicate.FieldsToCopyForTableCache"><span class="pre">PyAPplus64.duplicate.FieldsToCopyForTableCache</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#PyAPplus64.duplicate.FieldsToCopyForTableCache" title="PyAPplus64.duplicate.FieldsToCopyForTableCache"><span class="pre">PyAPplus64.duplicate.FieldsToCopyForTableCache</span></a></span></span><a class="headerlink" href="#PyAPplus64.duplicate.initFieldsToCopyForTableCacheIfNeeded" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Hilfsfunktion, die einen Cache erzeugt, falls dies noch nicht geschehen ist.</p>
@@ -1097,15 +1176,15 @@
 </dl>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="PyAPplus64.duplicate.loadDBDuplicateBusinessObject">
 <span class="sig-prename descclassname"><span class="pre">PyAPplus64.duplicate.</span></span><span class="sig-name descname"><span class="pre">loadDBDuplicateBusinessObject</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">server</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.applus.APplusServer" title="PyAPplus64.applus.APplusServer"><span class="pre">PyAPplus64.applus.APplusServer</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">table</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cond</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.sql_utils.SqlCondition" title="PyAPplus64.sql_utils.SqlCondition"><span class="pre">PyAPplus64.sql_utils.SqlCondition</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">cache</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.duplicate.FieldsToCopyForTableCache" title="PyAPplus64.duplicate.FieldsToCopyForTableCache"><span class="pre">PyAPplus64.duplicate.FieldsToCopyForTableCache</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">allowUpdate</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.duplicate.DuplicateBusinessObject" title="PyAPplus64.duplicate.DuplicateBusinessObject"><span class="pre">PyAPplus64.duplicate.DuplicateBusinessObject</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.duplicate.loadDBDuplicateBusinessObject" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Läd ein einzelnes DuplicateBusinessObjekt aus der DB. Die Bedingung sollte dabei
-einen eindeutigen Datensatz auswählen. Werden mehrere zurückgeliefert, wird ein 
+einen eindeutigen Datensatz auswählen. Werden mehrere zurückgeliefert, wird ein
 zufälliger ausgewählt. Wird kein Datensatz gefunden, wird None geliefert.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>server</strong> (<a class="reference internal" href="#PyAPplus64.applus.APplusServer" title="PyAPplus64.applus.APplusServer"><em>APplusServer</em></a>) – Verbindung zum APP-Server, benutzt zum Nachschlagen der zu kopierenden Felder</p></li>
 <li><p><strong>table</strong> (<em>str</em>) – Tabelle für das neue DuplicateBusinessObjekt</p></li>
 <li><p><strong>cond</strong> (<a class="reference internal" href="#PyAPplus64.sql_utils.SqlCondition" title="PyAPplus64.sql_utils.SqlCondition"><em>sql_utils.SqlCondition</em></a>) – SQL-Bedingung zur Auswahl eines Objektes</p></li>
@@ -1381,15 +1460,15 @@
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlConditionDateTimeFieldInRange">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlConditionDateTimeFieldInRange</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">field</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">datetimeVon</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">datetime.datetime</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">datetimeBis</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">datetime.datetime</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionDateTimeFieldInRange" title="Link zu dieser Definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlConditionDateTimeFieldInRange</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">field</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">datetimeVon</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">datetimeBis</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionDateTimeFieldInRange" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#PyAPplus64.sql_utils.SqlConditionPrepared" title="PyAPplus64.sql_utils.SqlConditionPrepared"><code class="xref py py-class docutils literal notranslate"><span class="pre">PyAPplus64.sql_utils.SqlConditionPrepared</span></code></a></p>
 <p>Liegt Datetime in einem bestimmten Zeitraum?</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>field</strong> (<em>str</em>) – das Feld</p></li>
 <li><p><strong>datetimeVon</strong> – der untere Wert (einschließlich), None erlaubt beliebige Zeiten</p></li>
@@ -1412,15 +1491,15 @@
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlConditionEq">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlConditionEq</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">value1</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value2</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionEq" title="Link zu dieser Definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlConditionEq</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">value1</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">None</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value2</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">None</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionEq" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#PyAPplus64.sql_utils.SqlConditionPrepared" title="PyAPplus64.sql_utils.SqlConditionPrepared"><code class="xref py py-class docutils literal notranslate"><span class="pre">PyAPplus64.sql_utils.SqlConditionPrepared</span></code></a></p>
 <p>Bedingung der Form ‚v1 is null‘, ‚v2 is null‘, ‚v1 = v2‘, ‚(1=1)‘ oder ‚(0=1)‘</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>value1</strong> – der Wert, kann unterschiedliche Typen besitzen</p></li>
 <li><p><strong>value2</strong> – der Wert, kann unterschiedliche Typen besitzen</p></li>
@@ -1434,15 +1513,15 @@
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlConditionFalse</span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionFalse" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#PyAPplus64.sql_utils.SqlConditionPrepared" title="PyAPplus64.sql_utils.SqlConditionPrepared"><code class="xref py py-class docutils literal notranslate"><span class="pre">PyAPplus64.sql_utils.SqlConditionPrepared</span></code></a></p>
 <p>False-Bedingung</p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlConditionFieldEq">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlConditionFieldEq</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">field</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionFieldEq" title="Link zu dieser Definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlConditionFieldEq</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">field</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">None</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionFieldEq" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#PyAPplus64.sql_utils.SqlConditionEq" title="PyAPplus64.sql_utils.SqlConditionEq"><code class="xref py py-class docutils literal notranslate"><span class="pre">PyAPplus64.sql_utils.SqlConditionEq</span></code></a></p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlConditionFieldGe">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlConditionFieldGe</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">field</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionFieldGe" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#PyAPplus64.sql_utils.SqlConditionGe" title="PyAPplus64.sql_utils.SqlConditionGe"><code class="xref py py-class docutils literal notranslate"><span class="pre">PyAPplus64.sql_utils.SqlConditionGe</span></code></a></p>
@@ -1593,25 +1672,25 @@
 <li><p><strong>connector</strong> (<em>str</em>) – wie werden Listenelemente verbunden (AND oder OR)</p></li>
 <li><p><strong>emptyCond</strong> (<em>str</em>) – Rückgabewert für leere Liste</p></li>
 </ul>
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlConditionList.addCondition">
-<span class="sig-name descname"><span class="pre">addCondition</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">cond</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.sql_utils.SqlCondition" title="PyAPplus64.sql_utils.SqlCondition"><span class="pre">PyAPplus64.sql_utils.SqlCondition</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionList.addCondition" title="Link zu dieser Definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">addCondition</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">cond</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlCondition" title="PyAPplus64.sql_utils.SqlCondition"><span class="pre">PyAPplus64.sql_utils.SqlCondition</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionList.addCondition" title="Link zu dieser Definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlConditionList.addConditionEq">
-<span class="sig-name descname"><span class="pre">addConditionEq</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">value1</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value2</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionList.addConditionEq" title="Link zu dieser Definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">addConditionEq</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">value1</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">None</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value2</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">None</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionList.addConditionEq" title="Link zu dieser Definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlConditionList.addConditionFieldEq">
-<span class="sig-name descname"><span class="pre">addConditionFieldEq</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">field</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionList.addConditionFieldEq" title="Link zu dieser Definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">addConditionFieldEq</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">field</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">None</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionList.addConditionFieldEq" title="Link zu dieser Definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlConditionList.addConditionFieldGe">
 <span class="sig-name descname"><span class="pre">addConditionFieldGe</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">field</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionList.addConditionFieldGe" title="Link zu dieser Definition">¶</a></dt>
 <dd></dd></dl>
 
@@ -1693,15 +1772,15 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlConditionList.addConditionLt">
 <span class="sig-name descname"><span class="pre">addConditionLt</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">value1</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">value2</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.sql_utils.SqlValue" title="PyAPplus64.sql_utils.SqlValue"><span class="pre">SqlValue</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionList.addConditionLt" title="Link zu dieser Definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlConditionList.addConditions">
-<span class="sig-name descname"><span class="pre">addConditions</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">conds</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.sql_utils.SqlCondition" title="PyAPplus64.sql_utils.SqlCondition"><span class="pre">PyAPplus64.sql_utils.SqlCondition</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionList.addConditions" title="Link zu dieser Definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">addConditions</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">conds</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlCondition" title="PyAPplus64.sql_utils.SqlCondition"><span class="pre">PyAPplus64.sql_utils.SqlCondition</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionList.addConditions" title="Link zu dieser Definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlConditionList.getCondition">
 <span class="sig-name descname"><span class="pre">getCondition</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionList.getCondition" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Liefert die Bedingung als String</p>
 <dl class="field-list simple">
@@ -1809,27 +1888,27 @@
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlConditionTrue</span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlConditionTrue" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#PyAPplus64.sql_utils.SqlConditionPrepared" title="PyAPplus64.sql_utils.SqlConditionPrepared"><code class="xref py py-class docutils literal notranslate"><span class="pre">PyAPplus64.sql_utils.SqlConditionPrepared</span></code></a></p>
 <p>True-Bedingung</p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlDate">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlDate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">d</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">datetime.date</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">5,</span> <span class="pre">6,</span> <span class="pre">22,</span> <span class="pre">11,</span> <span class="pre">50,</span> <span class="pre">888219)</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlDate" title="Link zu dieser Definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlDate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">d</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">datetime.date</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">7,</span> <span class="pre">27,</span> <span class="pre">10,</span> <span class="pre">31,</span> <span class="pre">9,</span> <span class="pre">391798)</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlDate" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>Wrapper um DateTime, die die Formatierung erleichtern</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><p><strong>d</strong> (<em>Union</em><em>[</em><em>datetime.datetime</em><em>, </em><em>datetime.date</em><em>]</em>) – das Datum</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlDateTime">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlDateTime</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">dt</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">datetime.date</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">5,</span> <span class="pre">6,</span> <span class="pre">22,</span> <span class="pre">11,</span> <span class="pre">50,</span> <span class="pre">888210)</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlDateTime" title="Link zu dieser Definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlDateTime</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">dt</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">datetime.date</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">7,</span> <span class="pre">27,</span> <span class="pre">10,</span> <span class="pre">31,</span> <span class="pre">9,</span> <span class="pre">391788)</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlDateTime" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>Wrapper um DateTime, die die Formatierung erleichtern</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><p><strong>dt</strong> (<em>Union</em><em>[</em><em>datetime.datetime</em><em>, </em><em>datetime.date</em><em>]</em>) – der Zeitpunkt</p>
 </dd>
 </dl>
@@ -1960,15 +2039,15 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlStatementSelect.addInnerJoin">
 <span class="sig-name descname"><span class="pre">addInnerJoin</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">table</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">conds</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlCondition" title="PyAPplus64.sql_utils.SqlCondition"><span class="pre">PyAPplus64.sql_utils.SqlCondition</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#PyAPplus64.sql_utils.SqlInnerJoin" title="PyAPplus64.sql_utils.SqlInnerJoin"><span class="pre">PyAPplus64.sql_utils.SqlInnerJoin</span></a></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlStatementSelect.addInnerJoin" title="Link zu dieser Definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlStatementSelect.addJoin">
-<span class="sig-name descname"><span class="pre">addJoin</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">j</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#PyAPplus64.sql_utils.SqlJoin" title="PyAPplus64.sql_utils.SqlJoin"><span class="pre">PyAPplus64.sql_utils.SqlJoin</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlStatementSelect.addJoin" title="Link zu dieser Definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">addJoin</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">j</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlJoin" title="PyAPplus64.sql_utils.SqlJoin"><span class="pre">PyAPplus64.sql_utils.SqlJoin</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlStatementSelect.addJoin" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Fügt ein Join zum SQL-Statement hinzu. Beispiel: ‚LEFT JOIN personal p ON t.UPDUSER = p.PERSONAL‘</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlStatementSelect.addLeftJoin">
 <span class="sig-name descname"><span class="pre">addLeftJoin</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">table</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">conds</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlCondition" title="PyAPplus64.sql_utils.SqlCondition"><span class="pre">PyAPplus64.sql_utils.SqlCondition</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#PyAPplus64.sql_utils.SqlLeftJoin" title="PyAPplus64.sql_utils.SqlLeftJoin"><span class="pre">PyAPplus64.sql_utils.SqlLeftJoin</span></a></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlStatementSelect.addLeftJoin" title="Link zu dieser Definition">¶</a></dt>
 <dd></dd></dl>
@@ -1995,15 +2074,15 @@
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlStatementSelect.having">
 <span class="sig-name descname"><span class="pre">having</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlConditionList" title="PyAPplus64.sql_utils.SqlConditionList"><span class="pre">PyAPplus64.sql_utils.SqlConditionList</span></a></em><a class="headerlink" href="#PyAPplus64.sql_utils.SqlStatementSelect.having" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>die Bedingung having, Default ist True</p>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlStatementSelect.joins">
-<span class="sig-name descname"><span class="pre">joins</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlJoin" title="PyAPplus64.sql_utils.SqlJoin"><span class="pre">PyAPplus64.sql_utils.SqlJoin</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#PyAPplus64.sql_utils.SqlStatementSelect.joins" title="Link zu dieser Definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">joins</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#PyAPplus64.sql_utils.SqlJoin" title="PyAPplus64.sql_utils.SqlJoin"><span class="pre">PyAPplus64.sql_utils.SqlJoin</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#PyAPplus64.sql_utils.SqlStatementSelect.joins" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Joins mit extra Tabellen</p>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlStatementSelect.order">
 <span class="sig-name descname"><span class="pre">order</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#PyAPplus64.sql_utils.SqlStatementSelect.order" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Sortierung</p>
@@ -2033,15 +2112,15 @@
 <dd><p>die Bedingung, Default ist True</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.SqlTime">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlTime</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">t</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">datetime.time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">5,</span> <span class="pre">6,</span> <span class="pre">22,</span> <span class="pre">11,</span> <span class="pre">50,</span> <span class="pre">888223)</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlTime" title="Link zu dieser Definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">SqlTime</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">t</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime.datetime</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">datetime.time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">7,</span> <span class="pre">27,</span> <span class="pre">10,</span> <span class="pre">31,</span> <span class="pre">9,</span> <span class="pre">391802)</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#PyAPplus64.sql_utils.SqlTime" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>Wrapper um DateTime, die die Formatierung erleichtern</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><p><strong>t</strong> (<em>Union</em><em>[</em><em>datetime.datetime</em><em>, </em><em>datetime.time</em><em>]</em>) – die Zeit</p>
 </dd>
 </dl>
@@ -2070,15 +2149,15 @@
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.formatSqlValueString">
 <span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">formatSqlValueString</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">s</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.formatSqlValueString" title="Link zu dieser Definition">¶</a></dt>
-<dd><p>Formatiert einen String für ein Sql-Statement. Der String wird in „‘“ eingeschlossen 
+<dd><p>Formatiert einen String für ein Sql-Statement. Der String wird in „‘“ eingeschlossen
 und Hochkomma im Text maskiert.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameter</dt>
 <dd class="field-odd"><p><strong>s</strong> (<em>str</em>) – der String</p>
 </dd>
 <dt class="field-even">Rückgabe</dt>
 <dd class="field-even"><p>der formatierte String</p>
@@ -2093,15 +2172,15 @@
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.normaliseDBfield">
 <span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">normaliseDBfield</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">f</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.normaliseDBfield" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Normalisiert die Darstellung eines DB-Feldes</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.normaliseDBfieldList">
-<span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">normaliseDBfieldList</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">l</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.normaliseDBfieldList" title="Link zu dieser Definition">¶</a></dt>
+<span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">normaliseDBfieldList</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fields</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.normaliseDBfieldList" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Normalisiert eine Menge von DB-Feldern</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="PyAPplus64.sql_utils.normaliseDBfieldSet">
 <span class="sig-prename descclassname"><span class="pre">PyAPplus64.sql_utils.</span></span><span class="sig-name descname"><span class="pre">normaliseDBfieldSet</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">s</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Set</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Set</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#PyAPplus64.sql_utils.normaliseDBfieldSet" title="Link zu dieser Definition">¶</a></dt>
 <dd><p>Normalisiert eine Menge von DB-Feldern</p>
```

#### html2text {}

```diff
@@ -12,16 +12,15 @@
     * PyAPplus64 package
 ****** PyAPplus64 packageÂ¶ ******
 ***** SubmodulesÂ¶ *****
 
 ***** PyAPplus64.applus moduleÂ¶ *****
   classPyAPplus64.applus.APplusServer(db_settings:
   PyAPplus64.applus_db.APplusDBSettings, server_settings:
-  PyAPplus64.applus_server.APplusAppServerSettings, web_settings:
-  PyAPplus64.applus_server.APplusWebServerSettings)Â¶
+  PyAPplus64.applus_server.APplusServerSettings)Â¶
       Bases: object
       Verbindung zu einem APplus DB und App Server mit Hilfsfunktionen fÃ¼r den
       komfortablen Zugriff.
         Parameter
                 * db_settings (APplusDBSettings) â die Einstellungen fÃ¼r die
                   Verbindung mit der Datenbank
                 * server_settings (APplusAppServerSettings) â die
@@ -73,21 +72,21 @@
             wenn mehrere Operationen in einer Transaktion genutzt werden
             sollen. Ansonsten sind die Hilfsmethoden wie APplusServer.dbQuery()
             zu bevorzugen. Diese Connection kann in Verbindung mit den
             Funktionen aus PyAPplus64.applus_db genutzt werden.
         db_settings: PyAPplus64.applus_db.APplusDBSettingsÂ¶
             Die Einstellungen fÃ¼r die Datenbankverbindung
         execUseXMLRowDelete(table: str, id: int) &#x2192; NoneÂ¶
-        getClient(package: str, name: str) &#x2192; zeep.client.ClientÂ¶
-            Erzeugt einen zeep - Client. Mittels dieses Clients kann die WSDL
-            Schnittstelle angesprochen werden. Wird als package âp2coreâ
-            und als name âTableâ verwendet und der resultierende client
-            âclientâ genannt, dann kann z.B. mittels
-            âclient.service.getCompleteSQL(sql)â vom AppServer ein
-            VervollstÃ¤ndigen des SQLs angefordert werden.
+        getAppClient(package: str, name: str) &#x2192; zeep.client.ClientÂ¶
+            Erzeugt einen zeep - Client fÃ¼r den APP-Server. Mittels dieses
+            Clients kann eines WSDL Schnittstelle des APP-Servers angesprochen
+            werden. Wird als package âp2coreâ und als name âTableâ
+            verwendet und der resultierende client âclientâ genannt, dann
+            kann z.B. mittels âclient.service.getCompleteSQL(sql)â vom
+            AppServer ein VervollstÃ¤ndigen des SQLs angefordert werden.
               Parameter
                       * package (string) â das Packet, z.B. âp2coreâ
                       * name â der Name im Packet, z.B. âTableâ
               RÃ¼ckgabe
                   den Client
               RÃ¼ckgabetyp
                   Client
@@ -104,14 +103,28 @@
               RÃ¼ckgabetyp
                   {str}
         getUniqueFieldsOfTable(table: str) &#x2192; Dict[str, List[str]]Â¶
             Liefert alle Spalten einer Tabelle, die eindeutig sein mÃ¼ssen.
             Diese werden als Dictionary gruppiert nach Index-Namen geliefert.
             Jeder Eintrag enthÃ¤lt eine Liste von Feldern, die zusammen
             eindeutig sein mÃ¼ssen.
+        getWebClient(url: str) &#x2192; zeep.client.ClientÂ¶
+            Erzeugt einen zeep - Client fÃ¼r den Web-Server. Mittels dieses
+            Clients kann die von einer ASMX-Seite zur VerfÃ¼gung gestellte
+            Schnittstelle angesprochen werden. Als parameter wird die relative
+            URL der ASMX-Seite erwartet. Die Base-URL automatisch ergÃ¤nzt. Ein
+            Beispiel fÃ¼r eine solche relative URL ist âmasterdata/
+            artikel.asmxâ.
+              Parameter
+                  url â die relative URL der ASMX Seite, z.B. âmasterdata/
+                  artikel.asmxâ
+              RÃ¼ckgabe
+                  den Client
+              RÃ¼ckgabetyp
+                  Client
         isDBTableKnown(table: str) &#x2192; boolÂ¶
             PrÃ¼ft, ob eine Tabelle im System bekannt ist
         makeWebLink(base: str, **kwargs: Any) &#x2192; strÂ¶
         makeWebLinkBauftrag(**kwargs: Any) &#x2192; strÂ¶
         makeWebLinkWauftrag(**kwargs: Any) &#x2192; strÂ¶
         makeWebLinkWauftragPos(**kwargs: Any) &#x2192; strÂ¶
         mkUseXMLRowDelete(table: str, id: int) &#x2192;
@@ -140,21 +153,21 @@
             Erstellt eine neue Nummer fÃ¼r das Objekt und legt diese Nummer
             zurÃ¼ck.
         reconnectDB() &#x2192; NoneÂ¶
         scripttool: PyAPplus64.applus_scripttool.APplusScriptToolÂ¶
             erlaubt den einfachen Zugriff auf Funktionen des ScriptTools
         server_conn: PyAPplus64.applus_server.APplusServerConnectionÂ¶
             erlaubt den Zugriff auf den AppServer
+        server_settings: PyAPplus64.applus_server.APplusServerSettingsÂ¶
+            Einstellung fÃ¼r die Verbindung zum APP- und Webserver
         sysconf: PyAPplus64.applus_sysconf.APplusSysConfÂ¶
             erlaubt den Zugriff auf die Sysconfig
         useXML(xml: str) &#x2192; AnyÂ¶
             Ruft p2core.xml.usexml auf. Wird meist durch ein UseXMLRow-Objekt
             aufgerufen.
-        web_settings: PyAPplus64.applus_server.APplusWebServerSettingsÂ¶
-            Die Einstellungen fÃ¼r die Datenbankverbindung
   PyAPplus64.applus.applusFromConfig(yamlString: str, user: Optional[str] =
   None, env: Optional[str] = None) &#x2192; PyAPplus64.applus.APplusServerÂ¶
       LÃ¤d Einstellungen aus einer Config-Datei und erzeugt daraus ein APplus-
       Objekt
   PyAPplus64.applus.applusFromConfigDict(yamlDict: Dict[str, Any], user:
   Optional[str] = None, env: Optional[str] = None) &#x2192;
   PyAPplus64.applus.APplusServerÂ¶
@@ -223,19 +236,38 @@
       Bases: object
       Zugriff auf AppServer ScriptTool
         Parameter
             server (APplusServerConnection) â die Verbindung zum Server
         getCurrentDate() &#x2192; strÂ¶
         getCurrentDateTime() &#x2192; strÂ¶
         getCurrentTime() &#x2192; strÂ¶
+        getInstallPath() &#x2192; strÂ¶
+            Liefert den Installionspfad des Appservers
+        getInstallPathAppServer() &#x2192; pathlib.PathÂ¶
+            Liefert den Installionspfad des Appservers als PathLib-Path
+        getInstallPathWebServer() &#x2192; pathlib.PathÂ¶
+            Liefert den Installionspfad des Webservers als PathLib-Path
         getLoginName() &#x2192; strÂ¶
         getMandant() &#x2192; strÂ¶
             Liefert den aktuellen Mandanten
         getMandantName() &#x2192; strÂ¶
             Liefert den Namen des aktuellen Mandanten
+        getServerInfo() &#x2192; Optional[lxml.etree.Element]Â¶
+            Liefert Informationen zum Server als ein XML Dokument.
+              RÃ¼ckgabe
+                  das gefundene und geparste XML-Dokument
+              RÃ¼ckgabetyp
+                  ET.Element
+        getServerInfoString() &#x2192; strÂ¶
+            Liefert Informationen zum Server als String. Dieser String
+            reprÃ¤sentiert ein XML Dokument.
+              RÃ¼ckgabe
+                  das XML-Dokument als String
+              RÃ¼ckgabetyp
+                  str
         getSystemName() &#x2192; strÂ¶
         getUserFullName() &#x2192; strÂ¶
         getUserName() &#x2192; strÂ¶
         getXMLDefinition(obj: str, mandant: str = '', checkFileExists: bool =
         False) &#x2192; Optional[lxml.etree.Element]Â¶
             LÃ¤d die XML-Definition als String vom APPServer. und parst das XML
             in ein minidom-Dokument.
@@ -243,15 +275,15 @@
                       * obj (str) â das Objekt, dessen Definition zu laden
                         ist, âArtikelâ lÃ¤d z.B.
                         âArtikelDefinition.xmlâ
                       * mandant (str optional) â der Mandant, dessen XML-Doku
                         geladen werden soll, wenn ââ wird der Standard-
                         Mandant verwendet
               RÃ¼ckgabe
-                  das gefundene und mittels ElementTree geparste XML-Dokument
+                  das gefundene und geparste XML-Dokument
               RÃ¼ckgabetyp
                   ET.Element
         getXMLDefinitionObj(obj: str, mandant: str = '') &#x2192; Optional
         [PyAPplus64.applus_scripttool.XMLDefinition]Â¶
             Benutzt getXMLDefinitionObj und liefert den Top-Level âObjectâ
             Knoten zurÃ¼ck, falls zusÃ¤tzlich ein MD5 Knoten existiert, also
             falls das Dokument wirklich vom Dateisystem geladen werden konnte.
@@ -259,15 +291,15 @@
               Parameter
                       * obj (str) â das Objekt, dess Definition zu laden ist,
                         âArtikelâ lÃ¤d z.B. âArtikelDefinition.xmlâ
                       * mandant (str optional) â der Mandant, dessen XML-Doku
                         geladen werden soll, wenn ââ wird der Standard-
                         Mandant verwendet
               RÃ¼ckgabe
-                  das gefundene und mittels ElementTree geparste XML-Dokument
+                  das gefundene und geparste XML-Dokument
               RÃ¼ckgabetyp
                   Optional[XMLDefinition]
         getXMLDefinitionString(obj: str, mandant: str = '') &#x2192; strÂ¶
             LÃ¤d die XML-Defintion als String vom APPServer. Auch wenn kein
             XML-Dokument im Dateisystem gefunden wird, wird ein String
             zurÃ¼ckgeliefert, der einen leeren Top-âObjectâ Knoten
             enthÃ¤lt. FÃ¼r gefundene XML-Dokumente gibt es zusÃ¤tzlich einen
@@ -292,43 +324,56 @@
             ausgeschlossen werden sollen. :return: Tuple aus allen Properties
             und ob dies aus- (True) oder ein-(False) zuschlieÃen sind. :rtype:
             Tuple[Set[str], bool]
         root: lxml.etree.ElementÂ¶
             das Root-Element, reprÃ¤sentiert âobjectâ aus Datei.
 
 ***** PyAPplus64.applus_server moduleÂ¶ *****
-  classPyAPplus64.applus_server.APplusAppServerSettings(appserver: str,
-  appserverPort: int, user: str, env: Optional[str] = None)Â¶
-      Bases: object
-      Einstellungen, mit welchem APplus App-Server sich verbunden werden soll.
   classPyAPplus64.applus_server.APplusServerConnection(settings:
-  PyAPplus64.applus_server.APplusAppServerSettings)Â¶
+  PyAPplus64.applus_server.APplusServerSettings)Â¶
       Bases: object
-      Verbindung zu einem APplus APP-Server
+      Verbindung zu einem APplus APP- und Web-Server
         Parameter
             settings (APplusAppServerSettings) â die Einstellungen fÃ¼r die
             Verbindung mit dem APplus Server
-        getClient(package: str, name: str) &#x2192; zeep.client.ClientÂ¶
-            Erzeugt einen zeep - Client. Mittels dieses Clients kann die WSDL
-            Schnittstelle angesprochen werden. Wird als package âp2coreâ
-            und als name âTableâ verwendet und der resultierende client
-            âclientâ genannt, dann kann z.B. mittels
+        getAppClient(package: str, name: str) &#x2192; zeep.client.ClientÂ¶
+            Erzeugt einen zeep - Client fÃ¼r den APP-Server. Mittels dieses
+            Clients kann die WSDL Schnittstelle angesprochen werden. Wird als
+            package âp2coreâ und als name âTableâ verwendet und der
+            resultierende client âclientâ genannt, dann kann z.B. mittels
             âclient.service.getCompleteSQL(sql)â vom AppServer ein
             VervollstÃ¤ndigen des SQLs angefordert werden.
               Parameter
                       * package (string) â das Packet, z.B. âp2coreâ
                       * name â der Name im Packet, z.B. âTableâ
               RÃ¼ckgabe
                   den Client
               RÃ¼ckgabetyp
                   Client
-  classPyAPplus64.applus_server.APplusWebServerSettings(baseurl: Optional[str]
-  = None)Â¶
+        getWebClient(url: str) &#x2192; zeep.client.ClientÂ¶
+            Erzeugt einen zeep - Client fÃ¼r den Web-Server. Mittels dieses
+            Clients kann die von einer ASMX-Seite zur VerfÃ¼gung gestellte
+            Schnittstelle angesprochen werden. Als parameter wird die relative
+            URL der ASMX-Seite erwartet. Die Base-URL automatisch ergÃ¤nzt. Ein
+            Beispiel fÃ¼r eine solche relative URL ist âmasterdata/
+            artikel.asmxâ.
+              Parameter
+                  url â die relative URL der ASMX Seite, z.B. âmasterdata/
+                  artikel.asmxâ
+              RÃ¼ckgabe
+                  den Client
+              RÃ¼ckgabetyp
+                  Client
+  classPyAPplus64.applus_server.APplusServerSettings(webserver: str, appserver:
+  str, appserverPort: int, user: str, env: Optional[str] = None, webserverUser:
+  Optional[str] = None, webserverUserDomain: Optional[str] = None,
+  webserverPassword: Optional[str] = None)Â¶
       Bases: object
-      Einstellungen, mit welchem APplus Web-Server sich verbunden werden soll.
+      Einstellungen, mit welchem APplus App- and Web-Server sich verbunden
+      werden soll.
 
 ***** PyAPplus64.applus_sysconf moduleÂ¶ *****
   classPyAPplus64.applus_sysconf.APplusSysConf(server: APplusServer)Â¶
       Bases: object
       SysConf Zugriff mit Cache Ã¼ber AppServer
         Parameter
             server (APplusServer) â die Verbindung zum Server
@@ -359,15 +404,15 @@
       sondern Ã¼ber Unterklassen fÃ¼r das EinfÃ¼gen, Ãndern oder LÃ¶schen
       benutzt werden.
         Parameter
                 * applus (APplusServer) â Verbindung zu APplus
                 * table (str) â die Tabelle
                 * cmd (str) â cmd-attribut der row, also ob es sich um ein
                   Update, ein Insert oder ein Delete handelt
-        addField(name: str | None, value: Any) &#x2192; NoneÂ¶
+        addField(name: Optional[str], value: Any) &#x2192; NoneÂ¶
             FÃ¼gt ein Feld zum Row-Node hinzu.
               Parameter
                       * name (string) â das Feld
                       * value â Wert des Feldes
         addTimestampField(id: int, ts: Optional[bytes] = None) &#x2192; NoneÂ¶
             FÃ¼gt ein Timestamp-Feld hinzu. Wird kein Timestamp Ã¼bergeben,
             wird mittels der ID der aktuelle Timestamp aus der DB geladen.
@@ -444,15 +489,15 @@
       ob ein Objekt bereits existiert. DafÃ¼r werden die gesetzten Felder mit
       den Feldern aus eindeutigen Indices verglichen. Existiert ein Objekt
       bereits, wird ein Update ausgefÃ¼hrt, ansonsten ein Insert. Bei Updates
       werden die Felderidundtimestampautomatisch gesetzt.
         Parameter
                 * applus (APplusServer) â Verbindung zu APplus
                 * table (string) â die Tabelle
-        checkExists() &#x2192; int | NoneÂ¶
+        checkExists() &#x2192; Optional[int]Â¶
             PrÃ¼ft, ob der Datensatz bereits in der DB existiert. Ist dies der
             Fall, wird die ID geliefert, sonst None
         exec() &#x2192; intÂ¶
             FÃ¼hrt entweder ein Update oder ein Insert durch. Dies hÃ¤ngt davon
             ab, ob das Objekt bereits in der DB existiert. In jedem Fall wird
             die ID des erzeugten oder geÃ¤nderten Objekts geliefert.
         insert() &#x2192; intÂ¶
@@ -826,16 +871,16 @@
       Bases: PyAPplus64.sql_utils.SqlConditionPrepared
       Liegt Datetime in einem bestimmten Monat?
         Parameter
                 * field (string) â das Feld
                 * year â das Jahr
                 * month â der Monat
   classPyAPplus64.sql_utils.SqlConditionDateTimeFieldInRange(field: str,
-  datetimeVon: datetime.datetime | None, datetimeBis: datetime.datetime |
-  None)Â¶
+  datetimeVon: Optional[datetime.datetime], datetimeBis: Optional
+  [datetime.datetime])Â¶
       Bases: PyAPplus64.sql_utils.SqlConditionPrepared
       Liegt Datetime in einem bestimmten Zeitraum?
         Parameter
                 * field (str) â das Feld
                 * datetimeVon â der untere Wert (einschlieÃlich), None
                   erlaubt beliebige Zeiten
                 * datetimeBis â der obere Wert (ausschlieÃlich), None
@@ -843,27 +888,27 @@
   classPyAPplus64.sql_utils.SqlConditionDateTimeFieldInYear(field: str, year:
   int)Â¶
       Bases: PyAPplus64.sql_utils.SqlConditionPrepared
       Liegt Datetime in einem bestimmten Jahr?
         Parameter
                 * field (str) â das Feld
                 * year â das Jahr
-  classPyAPplus64.sql_utils.SqlConditionEq(value1: Optional[Union[SqlValue,
-  bool]], value2: Optional[Union[SqlValue, bool]])Â¶
+  classPyAPplus64.sql_utils.SqlConditionEq(value1: Union[SqlValue, bool, None],
+  value2: Union[SqlValue, bool, None])Â¶
       Bases: PyAPplus64.sql_utils.SqlConditionPrepared
       Bedingung der Form âv1 is nullâ, âv2 is nullâ, âv1 = v2â, â
       (1=1)â oder â(0=1)â
         Parameter
                 * value1 â der Wert, kann unterschiedliche Typen besitzen
                 * value2 â der Wert, kann unterschiedliche Typen besitzen
   classPyAPplus64.sql_utils.SqlConditionFalseÂ¶
       Bases: PyAPplus64.sql_utils.SqlConditionPrepared
       False-Bedingung
-  classPyAPplus64.sql_utils.SqlConditionFieldEq(field: str, value: Optional
-  [Union[SqlValue, bool]])Â¶
+  classPyAPplus64.sql_utils.SqlConditionFieldEq(field: str, value: Union
+  [SqlValue, bool, None])Â¶
       Bases: PyAPplus64.sql_utils.SqlConditionEq
   classPyAPplus64.sql_utils.SqlConditionFieldGe(field: str, value: SqlValue)Â¶
       Bases: PyAPplus64.sql_utils.SqlConditionGe
   classPyAPplus64.sql_utils.SqlConditionFieldGt(field: str, value: SqlValue)Â¶
       Bases: PyAPplus64.sql_utils.SqlConditionGt
   classPyAPplus64.sql_utils.SqlConditionFieldInÂ¶
       Bases: PyAPplus64.sql_utils.SqlConditionIn
@@ -923,19 +968,19 @@
       Bases: PyAPplus64.sql_utils.SqlCondition
       Eine SQL Bedingung, die sich aus einer Liste anderer Bedingungen
       zusammensetzen. Dies kann eine âANDâ oder eine âORâ Liste sein.
         Parameter
                 * connector (str) â wie werden Listenelemente verbunden (AND
                   oder OR)
                 * emptyCond (str) â RÃ¼ckgabewert fÃ¼r leere Liste
-        addCondition(cond: PyAPplus64.sql_utils.SqlCondition | str | None)
-        &#x2192; NoneÂ¶
-        addConditionEq(value1: Optional[Union[SqlValue, bool]], value2:
-        Optional[Union[SqlValue, bool]]) &#x2192; NoneÂ¶
-        addConditionFieldEq(field: str, value: Optional[Union[SqlValue, bool]])
+        addCondition(cond: Optional[Union[PyAPplus64.sql_utils.SqlCondition,
+        str]]) &#x2192; NoneÂ¶
+        addConditionEq(value1: Union[SqlValue, bool, None], value2: Union
+        [SqlValue, bool, None]) &#x2192; NoneÂ¶
+        addConditionFieldEq(field: str, value: Union[SqlValue, bool, None])
         &#x2192; NoneÂ¶
         addConditionFieldGe(field: str, value: SqlValue) &#x2192; NoneÂ¶
         addConditionFieldGt(field: str, value: SqlValue) &#x2192; NoneÂ¶
         addConditionFieldIn()Â¶
         addConditionFieldIsNotNull(field: str) &#x2192; NoneÂ¶
         addConditionFieldIsNull(field: str) &#x2192; NoneÂ¶
         addConditionFieldLe(field: str, value: SqlValue) &#x2192; NoneÂ¶
@@ -946,16 +991,16 @@
         addConditionFieldsGt(field1: str, field2: str) &#x2192; NoneÂ¶
         addConditionFieldsLe(field1: str, field2: str) &#x2192; NoneÂ¶
         addConditionFieldsLt(field1: str, field2: str) &#x2192; NoneÂ¶
         addConditionGe(value1: SqlValue, value2: SqlValue) &#x2192; NoneÂ¶
         addConditionGt(value1: SqlValue, value2: SqlValue) &#x2192; NoneÂ¶
         addConditionLe(value1: SqlValue, value2: SqlValue) &#x2192; NoneÂ¶
         addConditionLt(value1: SqlValue, value2: SqlValue) &#x2192; NoneÂ¶
-        addConditions(*conds: PyAPplus64.sql_utils.SqlCondition | str | None)
-        &#x2192; NoneÂ¶
+        addConditions(*conds: Optional[Union[PyAPplus64.sql_utils.SqlCondition,
+        str]]) &#x2192; NoneÂ¶
         getCondition() &#x2192; strÂ¶
             Liefert die Bedingung als String
               RÃ¼ckgabe
                   die Bedingung
               RÃ¼ckgabetyp
                   str
         isEmpty() &#x2192; boolÂ¶
@@ -998,21 +1043,21 @@
         Parameter
                 * field (str) â das Feld
                 * value (str) â der Wert
   classPyAPplus64.sql_utils.SqlConditionTrueÂ¶
       Bases: PyAPplus64.sql_utils.SqlConditionPrepared
       True-Bedingung
   classPyAPplus64.sql_utils.SqlDate(d: Union[datetime.datetime, datetime.date]
-  = datetime.datetime(2023, 5, 6, 22, 11, 50, 888219))Â¶
+  = datetime.datetime(2023, 7, 27, 10, 31, 9, 391798))Â¶
       Bases: object
       Wrapper um DateTime, die die Formatierung erleichtern
         Parameter
             d (Union[datetime.datetime,datetime.date]) â das Datum
   classPyAPplus64.sql_utils.SqlDateTime(dt: Union[datetime.datetime,
-  datetime.date] = datetime.datetime(2023, 5, 6, 22, 11, 50, 888210))Â¶
+  datetime.date] = datetime.datetime(2023, 7, 27, 10, 31, 9, 391788))Â¶
       Bases: object
       Wrapper um DateTime, die die Formatierung erleichtern
         Parameter
             dt (Union[datetime.datetime,datetime.date]) â der Zeitpunkt
   classPyAPplus64.sql_utils.SqlField(fn: str)Â¶
       Bases: object
       Wrapper um SQL Feldnamen, die die Formatierung erleichtern
@@ -1072,43 +1117,43 @@
             Strings wird die Tabelle mit einem Punkt getrennt gesetzt. Dies
             kann im Vergleich zu âaddFieldsâ Schreibarbeit erleitern.
         addGroupBy(*fields: str) &#x2192; NoneÂ¶
             FÃ¼gt ein oder mehrere GroupBy Felder zu einem SQL-Statement hinzu.
         addInnerJoin(table: str, *conds: Union
         [PyAPplus64.sql_utils.SqlCondition, str]) &#x2192;
         PyAPplus64.sql_utils.SqlInnerJoinÂ¶
-        addJoin(j: PyAPplus64.sql_utils.SqlJoin | str) &#x2192; NoneÂ¶
+        addJoin(j: Union[PyAPplus64.sql_utils.SqlJoin, str]) &#x2192; NoneÂ¶
             FÃ¼gt ein Join zum SQL-Statement hinzu. Beispiel: âLEFT JOIN
             personal p ON t.UPDUSER = p.PERSONALâ
         addLeftJoin(table: str, *conds: Union
         [PyAPplus64.sql_utils.SqlCondition, str]) &#x2192;
         PyAPplus64.sql_utils.SqlLeftJoinÂ¶
         fields: List[str]Â¶
             Liste von auszuwÃ¤hlenden Feldern
         getSql() &#x2192; strÂ¶
             Liefert das SQL-SELECT-Statement als String
         groupBy: List[str]Â¶
             die Bedingung, Default ist True
         having: PyAPplus64.sql_utils.SqlConditionListÂ¶
             die Bedingung having, Default ist True
-        joins: List[PyAPplus64.sql_utils.SqlJoin | str]Â¶
+        joins: List[Union[PyAPplus64.sql_utils.SqlJoin, str]]Â¶
             Joins mit extra Tabellen
         order: Optional[str]Â¶
             Sortierung
         setTop(t: int) &#x2192; NoneÂ¶
             Wie viele DatensÃ¤tze sollen maximal zurÃ¼ckgeliefert werden? 0
             fÃ¼r alle
         table: strÂ¶
             die Tabelle
         top: intÂ¶
             wie viele DatensÃ¤tze auswÃ¤hlen? 0 fÃ¼r alle
         where: PyAPplus64.sql_utils.SqlConditionListÂ¶
             die Bedingung, Default ist True
   classPyAPplus64.sql_utils.SqlTime(t: Union[datetime.datetime, datetime.time]
-  = datetime.datetime(2023, 5, 6, 22, 11, 50, 888223))Â¶
+  = datetime.datetime(2023, 7, 27, 10, 31, 9, 391802))Â¶
       Bases: object
       Wrapper um DateTime, die die Formatierung erleichtern
         Parameter
             t (Union[datetime.datetime,datetime.time]) â die Zeit
   PyAPplus64.sql_utils.SqlValueÂ¶
       Union-Type aller unterstÃ¼tzter SQL-Werte
       alias of Union[str, int, float, PyAPplus64.sql_utils.SqlParam,
@@ -1131,16 +1176,16 @@
             s (str) â der String
         RÃ¼ckgabe
             der formatierte String
         RÃ¼ckgabetyp
             str
   PyAPplus64.sql_utils.normaliseDBfield(f: str) &#x2192; strÂ¶
       Normalisiert die Darstellung eines DB-Feldes
-  PyAPplus64.sql_utils.normaliseDBfieldList(l: Sequence[str]) &#x2192; Sequence
-  [str]Â¶
+  PyAPplus64.sql_utils.normaliseDBfieldList(fields: Sequence[str]) &#x2192;
+  Sequence[str]Â¶
       Normalisiert eine Menge von DB-Feldern
   PyAPplus64.sql_utils.normaliseDBfieldSet(s: Set[str]) &#x2192; Set[str]Â¶
       Normalisiert eine Menge von DB-Feldern
   PyAPplus64.sql_utils.sqlParam= <PyAPplus64.sql_utils.SqlParam object>Â¶
       Da SqlParam keinen Zustand hat, reicht ein einzelner statischer Wert
 
 ***** PyAPplus64.utils moduleÂ¶ *****
```

### Comparing `PyAPplus64-1.0.1/docs/build/html/genindex.html` & `PyAPplus64-1.1.0/docs/build/html/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -102,18 +102,18 @@
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlConditionList.addConditionGt">addConditionGt() (Methode von PyAPplus64.sql_utils.SqlConditionList)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlConditionList.addConditionLe">addConditionLe() (Methode von PyAPplus64.sql_utils.SqlConditionList)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlConditionList.addConditionLt">addConditionLt() (Methode von PyAPplus64.sql_utils.SqlConditionList)</a>
 </li>
-      <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlConditionList.addConditions">addConditions() (Methode von PyAPplus64.sql_utils.SqlConditionList)</a>
-</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlConditionList.addConditions">addConditions() (Methode von PyAPplus64.sql_utils.SqlConditionList)</a>
+</li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.duplicate.DuplicateBusinessObject.addDependentBusinessObject">addDependentBusinessObject() (Methode von PyAPplus64.duplicate.DuplicateBusinessObject)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_usexml.UseXmlRow.addField">addField() (Methode von PyAPplus64.applus_usexml.UseXmlRow)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlStatementSelect.addFields">addFields() (Methode von PyAPplus64.sql_utils.SqlStatementSelect)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlStatementSelect.addFieldsTable">addFieldsTable() (Methode von PyAPplus64.sql_utils.SqlStatementSelect)</a>
@@ -130,33 +130,31 @@
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_usexml.UseXmlRow.addTimestampField">addTimestampField() (Methode von PyAPplus64.applus_usexml.UseXmlRow)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_usexml.UseXmlRow.addTimestampIDFields">addTimestampIDFields() (Methode von PyAPplus64.applus_usexml.UseXmlRow)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.duplicate.DuplicateBusinessObject.allowUpdate">allowUpdate (Attribut von PyAPplus64.duplicate.DuplicateBusinessObject)</a>
 </li>
-      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_server.APplusAppServerSettings">APplusAppServerSettings (Klasse in PyAPplus64.applus_server)</a>
-</li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_db.APplusDBSettings">APplusDBSettings (Klasse in PyAPplus64.applus_db)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus.applusFromConfig">applusFromConfig() (im Modul PyAPplus64.applus)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus.applusFromConfigDict">applusFromConfigDict() (im Modul PyAPplus64.applus)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus.applusFromConfigFile">applusFromConfigFile() (im Modul PyAPplus64.applus)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool">APplusScriptTool (Klasse in PyAPplus64.applus_scripttool)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus.APplusServer">APplusServer (Klasse in PyAPplus64.applus)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_server.APplusServerConnection">APplusServerConnection (Klasse in PyAPplus64.applus_server)</a>
 </li>
-      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_sysconf.APplusSysConf">APplusSysConf (Klasse in PyAPplus64.applus_sysconf)</a>
+      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_server.APplusServerSettings">APplusServerSettings (Klasse in PyAPplus64.applus_server)</a>
 </li>
-      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_server.APplusWebServerSettings">APplusWebServerSettings (Klasse in PyAPplus64.applus_server)</a>
+      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_sysconf.APplusSysConf">APplusSysConf (Klasse in PyAPplus64.applus_sysconf)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="C">C</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
@@ -256,22 +254,22 @@
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="G">G</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_sysconf.APplusSysConf.getBoolean">getBoolean() (Methode von PyAPplus64.applus_sysconf.APplusSysConf)</a>
-</li>
-      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus.APplusServer.getClient">getClient() (Methode von PyAPplus64.applus.APplusServer)</a>
+      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus.APplusServer.getAppClient">getAppClient() (Methode von PyAPplus64.applus.APplusServer)</a>
 
       <ul>
-        <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_server.APplusServerConnection.getClient">(Methode von PyAPplus64.applus_server.APplusServerConnection)</a>
+        <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_server.APplusServerConnection.getAppClient">(Methode von PyAPplus64.applus_server.APplusServerConnection)</a>
 </li>
       </ul></li>
+      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_sysconf.APplusSysConf.getBoolean">getBoolean() (Methode von PyAPplus64.applus_sysconf.APplusSysConf)</a>
+</li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlCondition.getCondition">getCondition() (Methode von PyAPplus64.sql_utils.SqlCondition)</a>
 
       <ul>
         <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlConditionList.getCondition">(Methode von PyAPplus64.sql_utils.SqlConditionList)</a>
 </li>
         <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlConditionNot.getCondition">(Methode von PyAPplus64.sql_utils.SqlConditionNot)</a>
 </li>
@@ -298,28 +296,38 @@
       </ul></li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.duplicate.getFieldsToCopyForTable">getFieldsToCopyForTable() (im Modul PyAPplus64.duplicate)</a>
 
       <ul>
         <li><a href="generated/PyAPplus64.html#PyAPplus64.duplicate.FieldsToCopyForTableCache.getFieldsToCopyForTable">(Methode von PyAPplus64.duplicate.FieldsToCopyForTableCache)</a>
 </li>
       </ul></li>
+      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getInstallPath">getInstallPath() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
+</li>
+      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getInstallPathAppServer">getInstallPathAppServer() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
+</li>
+      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getInstallPathWebServer">getInstallPathWebServer() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
+</li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_sysconf.APplusSysConf.getInt">getInt() (Methode von PyAPplus64.applus_sysconf.APplusSysConf)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlJoin.getJoin">getJoin() (Methode von PyAPplus64.sql_utils.SqlJoin)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_sysconf.APplusSysConf.getList">getList() (Methode von PyAPplus64.applus_sysconf.APplusSysConf)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getLoginName">getLoginName() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getMandant">getMandant() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getMandantName">getMandantName() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
 </li>
+      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getServerInfo">getServerInfo() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
+</li>
+      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getServerInfoString">getServerInfoString() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
+</li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlStatementSelect.getSql">getSql() (Methode von PyAPplus64.sql_utils.SqlStatementSelect)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_sysconf.APplusSysConf.getString">getString() (Methode von PyAPplus64.applus_sysconf.APplusSysConf)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getSystemName">getSystemName() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_db.DBTableIDs.getTable">getTable() (Methode von PyAPplus64.applus_db.DBTableIDs)</a>
@@ -332,14 +340,20 @@
         <li><a href="generated/PyAPplus64.html#PyAPplus64.applus.APplusServer.getUniqueFieldsOfTable">(Methode von PyAPplus64.applus.APplusServer)</a>
 </li>
       </ul></li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getUserFullName">getUserFullName() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getUserName">getUserName() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
 </li>
+      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus.APplusServer.getWebClient">getWebClient() (Methode von PyAPplus64.applus.APplusServer)</a>
+
+      <ul>
+        <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_server.APplusServerConnection.getWebClient">(Methode von PyAPplus64.applus_server.APplusServerConnection)</a>
+</li>
+      </ul></li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getXMLDefinition">getXMLDefinition() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getXMLDefinitionObj">getXMLDefinitionObj() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus_scripttool.APplusScriptTool.getXMLDefinitionString">getXMLDefinitionString() (Methode von PyAPplus64.applus_scripttool.APplusScriptTool)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlStatementSelect.groupBy">groupBy (Attribut von PyAPplus64.sql_utils.SqlStatementSelect)</a>
@@ -602,14 +616,16 @@
 <h2 id="S">S</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus.APplusServer.scripttool">scripttool (Attribut von PyAPplus64.applus.APplusServer)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.applus.APplusServer.server_conn">server_conn (Attribut von PyAPplus64.applus.APplusServer)</a>
 </li>
+      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus.APplusServer.server_settings">server_settings (Attribut von PyAPplus64.applus.APplusServer)</a>
+</li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.duplicate.DuplicateBusinessObject.setFields">setFields() (Methode von PyAPplus64.duplicate.DuplicateBusinessObject)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlStatementSelect.setTop">setTop() (Methode von PyAPplus64.sql_utils.SqlStatementSelect)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlCondition">SqlCondition (Klasse in PyAPplus64.sql_utils)</a>
 </li>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlConditionAnd">SqlConditionAnd (Klasse in PyAPplus64.sql_utils)</a>
@@ -750,18 +766,14 @@
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="W">W</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="generated/PyAPplus64.html#PyAPplus64.applus.APplusServer.web_settings">web_settings (Attribut von PyAPplus64.applus.APplusServer)</a>
-</li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="generated/PyAPplus64.html#PyAPplus64.sql_utils.SqlStatementSelect.where">where (Attribut von PyAPplus64.sql_utils.SqlStatementSelect)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="X">X</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
```

#### html2text {}

```diff
@@ -7,59 +7,57 @@
     * Index
     * Module |
     * PyAPplus64_1.0.1_Dokumentation »
     * Stichwortverzeichnis
 ****** Stichwortverzeichnis ******
 A | C | D | E | F | G | H | I | J | L | M | N | O | P | R | S | T | U | W | X
 ***** A *****
-    * add()_(Methode_von
-      PyAPplus64.applus_db.DBTableIDs)           * addDependentBusinessObject()_(Methode_von
-    * addCondition()_(Methode_von                  PyAPplus64.duplicate.DuplicateBusinessObject)
-      PyAPplus64.sql_utils.SqlConditionList)     * addField()_(Methode_von
-    * addConditionEq()_(Methode_von                PyAPplus64.applus_usexml.UseXmlRow)
-      PyAPplus64.sql_utils.SqlConditionList)     * addFields()_(Methode_von
-    * addConditionFieldEq()_(Methode_von           PyAPplus64.sql_utils.SqlStatementSelect)
-      PyAPplus64.sql_utils.SqlConditionList)     * addFieldsTable()_(Methode_von
-    * addConditionFieldGe()_(Methode_von           PyAPplus64.sql_utils.SqlStatementSelect)
-      PyAPplus64.sql_utils.SqlConditionList)     * addGroupBy()_(Methode_von
-    * addConditionFieldGt()_(Methode_von           PyAPplus64.sql_utils.SqlStatementSelect)
-      PyAPplus64.sql_utils.SqlConditionList)     * addInnerJoin()_(Methode_von
-    * addConditionFieldIn()_(Methode_von           PyAPplus64.sql_utils.SqlStatementSelect)
-      PyAPplus64.sql_utils.SqlConditionList)     * addJoin()_(Methode_von
-    * addConditionFieldIsNotNull()_(Methode        PyAPplus64.sql_utils.SqlStatementSelect)
-      von                                        * addLeftJoin()_(Methode_von
-      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.sql_utils.SqlStatementSelect)
-    * addConditionFieldIsNull()_(Methode_von     * addSachgruppeDependentObjects()_(im_Modul
-      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.duplicate)
-    * addConditionFieldLe()_(Methode_von         * addTimestampField()_(Methode_von
-      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.applus_usexml.UseXmlRow)
-    * addConditionFieldLt()_(Methode_von         * addTimestampIDFields()_(Methode_von
-      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.applus_usexml.UseXmlRow)
-    * addConditionFieldsEq()_(Methode_von        * allowUpdate_(Attribut_von
+    * add()_(Methode_von                         * addConditions()_(Methode_von
+      PyAPplus64.applus_db.DBTableIDs)             PyAPplus64.sql_utils.SqlConditionList)
+    * addCondition()_(Methode_von                * addDependentBusinessObject()_(Methode_von
       PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.duplicate.DuplicateBusinessObject)
-    * addConditionFieldsGe()_(Methode_von        * APplusAppServerSettings_(Klasse_in
-      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.applus_server)
-    * addConditionFieldsGt()_(Methode_von        * APplusDBSettings_(Klasse_in
-      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.applus_db)
-    * addConditionFieldsLe()_(Methode_von        * applusFromConfig()_(im_Modul
-      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.applus)
-    * addConditionFieldsLt()_(Methode_von        * applusFromConfigDict()_(im_Modul
-      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.applus)
-    * addConditionFieldStringNotEmpty()_         * applusFromConfigFile()_(im_Modul
-      (Methode_von                                 PyAPplus64.applus)
-      PyAPplus64.sql_utils.SqlConditionList)     * APplusScriptTool_(Klasse_in
-    * addConditionGe()_(Methode_von                PyAPplus64.applus_scripttool)
-      PyAPplus64.sql_utils.SqlConditionList)     * APplusServer_(Klasse_in_PyAPplus64.applus)
-    * addConditionGt()_(Methode_von              * APplusServerConnection_(Klasse_in
-      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.applus_server)
-    * addConditionLe()_(Methode_von              * APplusSysConf_(Klasse_in
-      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.applus_sysconf)
-    * addConditionLt()_(Methode_von              * APplusWebServerSettings_(Klasse_in
-      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.applus_server)
-    * addConditions()_(Methode_von
+    * addConditionEq()_(Methode_von              * addField()_(Methode_von
+      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.applus_usexml.UseXmlRow)
+    * addConditionFieldEq()_(Methode_von         * addFields()_(Methode_von
+      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.sql_utils.SqlStatementSelect)
+    * addConditionFieldGe()_(Methode_von         * addFieldsTable()_(Methode_von
+      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.sql_utils.SqlStatementSelect)
+    * addConditionFieldGt()_(Methode_von         * addGroupBy()_(Methode_von
+      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.sql_utils.SqlStatementSelect)
+    * addConditionFieldIn()_(Methode_von         * addInnerJoin()_(Methode_von
+      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.sql_utils.SqlStatementSelect)
+    * addConditionFieldIsNotNull()_(Methode      * addJoin()_(Methode_von
+      von                                          PyAPplus64.sql_utils.SqlStatementSelect)
+      PyAPplus64.sql_utils.SqlConditionList)     * addLeftJoin()_(Methode_von
+    * addConditionFieldIsNull()_(Methode_von       PyAPplus64.sql_utils.SqlStatementSelect)
+      PyAPplus64.sql_utils.SqlConditionList)     * addSachgruppeDependentObjects()_(im_Modul
+    * addConditionFieldLe()_(Methode_von           PyAPplus64.duplicate)
+      PyAPplus64.sql_utils.SqlConditionList)     * addTimestampField()_(Methode_von
+    * addConditionFieldLt()_(Methode_von           PyAPplus64.applus_usexml.UseXmlRow)
+      PyAPplus64.sql_utils.SqlConditionList)     * addTimestampIDFields()_(Methode_von
+    * addConditionFieldsEq()_(Methode_von          PyAPplus64.applus_usexml.UseXmlRow)
+      PyAPplus64.sql_utils.SqlConditionList)     * allowUpdate_(Attribut_von
+    * addConditionFieldsGe()_(Methode_von          PyAPplus64.duplicate.DuplicateBusinessObject)
+      PyAPplus64.sql_utils.SqlConditionList)     * APplusDBSettings_(Klasse_in
+    * addConditionFieldsGt()_(Methode_von          PyAPplus64.applus_db)
+      PyAPplus64.sql_utils.SqlConditionList)     * applusFromConfig()_(im_Modul
+    * addConditionFieldsLe()_(Methode_von          PyAPplus64.applus)
+      PyAPplus64.sql_utils.SqlConditionList)     * applusFromConfigDict()_(im_Modul
+    * addConditionFieldsLt()_(Methode_von          PyAPplus64.applus)
+      PyAPplus64.sql_utils.SqlConditionList)     * applusFromConfigFile()_(im_Modul
+    * addConditionFieldStringNotEmpty()_           PyAPplus64.applus)
+      (Methode_von                               * APplusScriptTool_(Klasse_in
+      PyAPplus64.sql_utils.SqlConditionList)       PyAPplus64.applus_scripttool)
+    * addConditionGe()_(Methode_von              * APplusServer_(Klasse_in_PyAPplus64.applus)
+      PyAPplus64.sql_utils.SqlConditionList)     * APplusServerConnection_(Klasse_in
+    * addConditionGt()_(Methode_von                PyAPplus64.applus_server)
+      PyAPplus64.sql_utils.SqlConditionList)     * APplusServerSettings_(Klasse_in
+    * addConditionLe()_(Methode_von                PyAPplus64.applus_server)
+      PyAPplus64.sql_utils.SqlConditionList)     * APplusSysConf_(Klasse_in
+    * addConditionLt()_(Methode_von                PyAPplus64.applus_sysconf)
       PyAPplus64.sql_utils.SqlConditionList)
 ***** C *****
                                                             * clearCache()_(Methode_von
     * checkDirExists()_(im_Modul_PyAPplus64.utils)            PyAPplus64.applus_sysconf.APplusSysConf)
     * checkExists()_(Methode_von                            * completeSQL()_(Methode_von
       PyAPplus64.applus_usexml.UseXmlRowInsertOrUpdate)       PyAPplus64.applus.APplusServer)
     * checkFieldSet()_(Methode_von                          * connect()_(Methode_von
@@ -98,48 +96,54 @@
             PyAPplus64.sql_utils.SqlStatementSelect)     * formatSqlValue()_(im
     * fieldsNotCopied_(Attribut_von                        Modul
       PyAPplus64.duplicate.DuplicateBusinessObject)        PyAPplus64.sql_utils)
                                                          * formatSqlValueString()_
                                                            (im_Modul
                                                            PyAPplus64.sql_utils)
 ***** G *****
-    * getBoolean()_(Methode_von                                  * getJoin()_(Methode_von
-      PyAPplus64.applus_sysconf.APplusSysConf)                     PyAPplus64.sql_utils.SqlJoin)
-    * getClient()_(Methode_von                                   * getList()_(Methode_von
-      PyAPplus64.applus.APplusServer)                              PyAPplus64.applus_sysconf.APplusSysConf)
-          o (Methode_von                                         * getLoginName()_(Methode_von
-            PyAPplus64.applus_server.APplusServerConnection)       PyAPplus64.applus_scripttool.APplusScriptTool)
-    * getCondition()_(Methode_von                                * getMandant()_(Methode_von
-      PyAPplus64.sql_utils.SqlCondition)                           PyAPplus64.applus_scripttool.APplusScriptTool)
-          o (Methode_von                                         * getMandantName()_(Methode_von
-            PyAPplus64.sql_utils.SqlConditionList)                 PyAPplus64.applus_scripttool.APplusScriptTool)
-          o (Methode_von                                         * getSql()_(Methode_von
-            PyAPplus64.sql_utils.SqlConditionNot)                  PyAPplus64.sql_utils.SqlStatementSelect)
-          o (Methode_von                                         * getString()_(Methode_von
-            PyAPplus64.sql_utils.SqlConditionPrepared)             PyAPplus64.applus_sysconf.APplusSysConf)
-    * getConnectionString()_(Methode_von                         * getSystemName()_(Methode_von
-      PyAPplus64.applus_db.APplusDBSettings)                       PyAPplus64.applus_scripttool.APplusScriptTool)
-    * getCurrentDate()_(Methode_von                              * getTable()_(Methode_von
-      PyAPplus64.applus_scripttool.APplusScriptTool)               PyAPplus64.applus_db.DBTableIDs)
-    * getCurrentDateTime()_(Methode_von                          * getTableFields()_(Methode_von
-      PyAPplus64.applus_scripttool.APplusScriptTool)               PyAPplus64.applus.APplusServer)
-    * getCurrentTime()_(Methode_von                              * getUniqueFieldsOfTable()_(im_Modul
-      PyAPplus64.applus_scripttool.APplusScriptTool)               PyAPplus64.applus_db)
-    * getDouble()_(Methode_von                                         o (Methode_von
-      PyAPplus64.applus_sysconf.APplusSysConf)                           PyAPplus64.applus.APplusServer)
-    * getDuplicate()_(Methode_von                                * getUserFullName()_(Methode_von
-      PyAPplus64.applus_scripttool.XMLDefinition)                  PyAPplus64.applus_scripttool.APplusScriptTool)
-    * getField()_(Methode_von                                    * getUserName()_(Methode_von
+    * getAppClient()_(Methode_von                                * getJoin()_(Methode_von_PyAPplus64.sql_utils.SqlJoin)
+      PyAPplus64.applus.APplusServer)                            * getList()_(Methode_von
+          o (Methode_von                                           PyAPplus64.applus_sysconf.APplusSysConf)
+            PyAPplus64.applus_server.APplusServerConnection)     * getLoginName()_(Methode_von
+    * getBoolean()_(Methode_von                                    PyAPplus64.applus_scripttool.APplusScriptTool)
+      PyAPplus64.applus_sysconf.APplusSysConf)                   * getMandant()_(Methode_von
+    * getCondition()_(Methode_von                                  PyAPplus64.applus_scripttool.APplusScriptTool)
+      PyAPplus64.sql_utils.SqlCondition)                         * getMandantName()_(Methode_von
+          o (Methode_von                                           PyAPplus64.applus_scripttool.APplusScriptTool)
+            PyAPplus64.sql_utils.SqlConditionList)               * getServerInfo()_(Methode_von
+          o (Methode_von                                           PyAPplus64.applus_scripttool.APplusScriptTool)
+            PyAPplus64.sql_utils.SqlConditionNot)                * getServerInfoString()_(Methode_von
+          o (Methode_von                                           PyAPplus64.applus_scripttool.APplusScriptTool)
+            PyAPplus64.sql_utils.SqlConditionPrepared)           * getSql()_(Methode_von
+    * getConnectionString()_(Methode_von                           PyAPplus64.sql_utils.SqlStatementSelect)
+      PyAPplus64.applus_db.APplusDBSettings)                     * getString()_(Methode_von
+    * getCurrentDate()_(Methode_von                                PyAPplus64.applus_sysconf.APplusSysConf)
+      PyAPplus64.applus_scripttool.APplusScriptTool)             * getSystemName()_(Methode_von
+    * getCurrentDateTime()_(Methode_von                            PyAPplus64.applus_scripttool.APplusScriptTool)
+      PyAPplus64.applus_scripttool.APplusScriptTool)             * getTable()_(Methode_von
+    * getCurrentTime()_(Methode_von                                PyAPplus64.applus_db.DBTableIDs)
+      PyAPplus64.applus_scripttool.APplusScriptTool)             * getTableFields()_(Methode_von
+    * getDouble()_(Methode_von                                     PyAPplus64.applus.APplusServer)
+      PyAPplus64.applus_sysconf.APplusSysConf)                   * getUniqueFieldsOfTable()_(im_Modul
+    * getDuplicate()_(Methode_von                                  PyAPplus64.applus_db)
+      PyAPplus64.applus_scripttool.XMLDefinition)                      o (Methode_von_PyAPplus64.applus.APplusServer)
+    * getField()_(Methode_von                                    * getUserFullName()_(Methode_von
       PyAPplus64.applus_usexml.UseXmlRow)                          PyAPplus64.applus_scripttool.APplusScriptTool)
-          o (Methode_von                                         * getXMLDefinition()_(Methode_von
+          o (Methode_von                                         * getUserName()_(Methode_von
             PyAPplus64.duplicate.DuplicateBusinessObject)          PyAPplus64.applus_scripttool.APplusScriptTool)
-    * getFieldsToCopyForTable()_(im_Modul                        * getXMLDefinitionObj()_(Methode_von
-      PyAPplus64.duplicate)                                        PyAPplus64.applus_scripttool.APplusScriptTool)
-          o (Methode_von                                         * getXMLDefinitionString()_(Methode_von
-            PyAPplus64.duplicate.FieldsToCopyForTableCache)        PyAPplus64.applus_scripttool.APplusScriptTool)
+    * getFieldsToCopyForTable()_(im_Modul                        * getWebClient()_(Methode_von
+      PyAPplus64.duplicate)                                        PyAPplus64.applus.APplusServer)
+          o (Methode_von                                               o (Methode_von
+            PyAPplus64.duplicate.FieldsToCopyForTableCache)              PyAPplus64.applus_server.APplusServerConnection)
+    * getInstallPath()_(Methode_von                              * getXMLDefinition()_(Methode_von
+      PyAPplus64.applus_scripttool.APplusScriptTool)               PyAPplus64.applus_scripttool.APplusScriptTool)
+    * getInstallPathAppServer()_(Methode_von                     * getXMLDefinitionObj()_(Methode_von
+      PyAPplus64.applus_scripttool.APplusScriptTool)               PyAPplus64.applus_scripttool.APplusScriptTool)
+    * getInstallPathWebServer()_(Methode_von                     * getXMLDefinitionString()_(Methode_von
+      PyAPplus64.applus_scripttool.APplusScriptTool)               PyAPplus64.applus_scripttool.APplusScriptTool)
     * getInt()_(Methode_von                                      * groupBy_(Attribut_von
       PyAPplus64.applus_sysconf.APplusSysConf)                     PyAPplus64.sql_utils.SqlStatementSelect)
 ***** H *****
     * having_(Attribut_von_PyAPplus64.sql_utils.SqlStatementSelect)
 ***** I *****
     * initFieldsToCopyForTableCacheIfNeeded()_(im_Modul
       PyAPplus64.duplicate)
@@ -213,63 +217,63 @@
       PyAPplus64.applus_db)         PyAPplus64.applus.APplusServer)
     * rawQuerySingleRow()_(im     * root_(Attribut_von
       Modul                         PyAPplus64.applus_scripttool.XMLDefinition)
       PyAPplus64.applus_db)       * row_to_dict()_(im_Modul
                                     PyAPplus64.applus_db)
 ***** S *****
                                                         * SqlConditionGt_(Klasse_in
-                                                          PyAPplus64.sql_utils)
-    * scripttool_(Attribut_von                          * SqlConditionIn_(Klasse_in
-      PyAPplus64.applus.APplusServer)                     PyAPplus64.sql_utils)
-    * server_conn_(Attribut_von                         * SqlConditionIsNotNull_(Klasse
-      PyAPplus64.applus.APplusServer)                     in_PyAPplus64.sql_utils)
-    * setFields()_(Methode_von                          * SqlConditionIsNull_(Klasse_in
-      PyAPplus64.duplicate.DuplicateBusinessObject)       PyAPplus64.sql_utils)
-    * setTop()_(Methode_von                             * SqlConditionLe_(Klasse_in
-      PyAPplus64.sql_utils.SqlStatementSelect)            PyAPplus64.sql_utils)
-    * SqlCondition_(Klasse_in_PyAPplus64.sql_utils)     * SqlConditionList_(Klasse_in
-    * SqlConditionAnd_(Klasse_in                          PyAPplus64.sql_utils)
-      PyAPplus64.sql_utils)                             * SqlConditionLt_(Klasse_in
-    * SqlConditionBinComp_(Klasse_in                      PyAPplus64.sql_utils)
-      PyAPplus64.sql_utils)                             * SqlConditionNot_(Klasse_in
-    * SqlConditionBool_(Klasse_in                         PyAPplus64.sql_utils)
-      PyAPplus64.sql_utils)                             * SqlConditionOr_(Klasse_in
-    * SqlConditionDateTimeFieldInDay_(Klasse_in           PyAPplus64.sql_utils)
-      PyAPplus64.sql_utils)                             * SqlConditionPrepared_(Klasse_in
-    * SqlConditionDateTimeFieldInMonth_(Klasse_in         PyAPplus64.sql_utils)
-      PyAPplus64.sql_utils)                             * SqlConditionStringStartsWith_
-    * SqlConditionDateTimeFieldInRange_(Klasse_in         (Klasse_in
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionDateTimeFieldInYear_(Klasse_in        * SqlConditionTrue_(Klasse_in
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionEq_(Klasse_in                         * SqlDate_(Klasse_in
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionFalse_(Klasse_in                      * SqlDateTime_(Klasse_in
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionFieldEq_(Klasse_in                    * SqlField_(Klasse_in
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionFieldGe_(Klasse_in                    * SqlFixed_(Klasse_in
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionFieldGt_(Klasse_in                    * SqlInnerJoin_(Klasse_in
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionFieldIn_(Klasse_in                    * SqlJoin_(Klasse_in
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionFieldIsNotNull_(Klasse_in             * SqlLeftJoin_(Klasse_in
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionFieldIsNull_(Klasse_in                * sqlParam_(in_Modul
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionFieldLe_(Klasse_in                    * SqlParam_(Klasse_in
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionFieldLt_(Klasse_in                    * SqlStatementSelect_(Klasse_in
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionFieldStringNotEmpty_(Klasse_in        * SqlTime_(Klasse_in
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-    * SqlConditionGe_(Klasse_in                         * SqlValue_(in_Modul
-      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
-                                                        * sysconf_(Attribut_von
+    * scripttool_(Attribut_von                            PyAPplus64.sql_utils)
+      PyAPplus64.applus.APplusServer)                   * SqlConditionIn_(Klasse_in
+    * server_conn_(Attribut_von                           PyAPplus64.sql_utils)
+      PyAPplus64.applus.APplusServer)                   * SqlConditionIsNotNull_(Klasse
+    * server_settings_(Attribut_von                       in_PyAPplus64.sql_utils)
+      PyAPplus64.applus.APplusServer)                   * SqlConditionIsNull_(Klasse_in
+    * setFields()_(Methode_von                            PyAPplus64.sql_utils)
+      PyAPplus64.duplicate.DuplicateBusinessObject)     * SqlConditionLe_(Klasse_in
+    * setTop()_(Methode_von                               PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils.SqlStatementSelect)          * SqlConditionList_(Klasse_in
+    * SqlCondition_(Klasse_in_PyAPplus64.sql_utils)       PyAPplus64.sql_utils)
+    * SqlConditionAnd_(Klasse_in                        * SqlConditionLt_(Klasse_in
+      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
+    * SqlConditionBinComp_(Klasse_in                    * SqlConditionNot_(Klasse_in
+      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
+    * SqlConditionBool_(Klasse_in                       * SqlConditionOr_(Klasse_in
+      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
+    * SqlConditionDateTimeFieldInDay_(Klasse_in         * SqlConditionPrepared_(Klasse_in
+      PyAPplus64.sql_utils)                               PyAPplus64.sql_utils)
+    * SqlConditionDateTimeFieldInMonth_(Klasse_in       * SqlConditionStringStartsWith_
+      PyAPplus64.sql_utils)                               (Klasse_in
+    * SqlConditionDateTimeFieldInRange_(Klasse_in         PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * SqlConditionTrue_(Klasse_in
+    * SqlConditionDateTimeFieldInYear_(Klasse_in          PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * SqlDate_(Klasse_in
+    * SqlConditionEq_(Klasse_in                           PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * SqlDateTime_(Klasse_in
+    * SqlConditionFalse_(Klasse_in                        PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * SqlField_(Klasse_in
+    * SqlConditionFieldEq_(Klasse_in                      PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * SqlFixed_(Klasse_in
+    * SqlConditionFieldGe_(Klasse_in                      PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * SqlInnerJoin_(Klasse_in
+    * SqlConditionFieldGt_(Klasse_in                      PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * SqlJoin_(Klasse_in
+    * SqlConditionFieldIn_(Klasse_in                      PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * SqlLeftJoin_(Klasse_in
+    * SqlConditionFieldIsNotNull_(Klasse_in               PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * sqlParam_(in_Modul
+    * SqlConditionFieldIsNull_(Klasse_in                  PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * SqlParam_(Klasse_in
+    * SqlConditionFieldLe_(Klasse_in                      PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * SqlStatementSelect_(Klasse_in
+    * SqlConditionFieldLt_(Klasse_in                      PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * SqlTime_(Klasse_in
+    * SqlConditionFieldStringNotEmpty_(Klasse_in          PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * SqlValue_(in_Modul
+    * SqlConditionGe_(Klasse_in                           PyAPplus64.sql_utils)
+      PyAPplus64.sql_utils)                             * sysconf_(Attribut_von
                                                           PyAPplus64.applus.APplusServer)
 ***** T *****
     * table_(Attribut_von                                * top_(Attribut_von
       PyAPplus64.duplicate.DuplicateBusinessObject)        PyAPplus64.sql_utils.SqlStatementSelect)
           o (Attribut_von                                * toprettyxml()_(Methode_von
             PyAPplus64.sql_utils.SqlStatementSelect)       PyAPplus64.applus_usexml.UseXmlRow)
 ***** U *****
@@ -284,16 +288,15 @@
       PyAPplus64.applus_usexml.UseXmlRowInsertOrUpdate)     * UseXmlRowInsertOrUpdate_
     * useXML()_(Methode_von                                   (Klasse_in
       PyAPplus64.applus.APplusServer)                         PyAPplus64.applus_usexml)
                                                             * UseXmlRowUpdate_(Klasse
                                                               in
                                                               PyAPplus64.applus_usexml)
 ***** W *****
-    * web_settings_(Attribut_von          * where_(Attribut_von
-      PyAPplus64.applus.APplusServer)       PyAPplus64.sql_utils.SqlStatementSelect)
+    * where_(Attribut_von_PyAPplus64.sql_utils.SqlStatementSelect)
 ***** X *****
     * XMLDefinition_(Klasse_in_PyAPplus64.applus_scripttool)
 **** Schnellsuche ****
 [q                   ] [Los]
 **** Navigation ****
     * Index
     * Module |
```

### Comparing `PyAPplus64-1.0.1/docs/build/html/index.html` & `PyAPplus64-1.1.0/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/py-modindex.html` & `PyAPplus64-1.1.0/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/search.html` & `PyAPplus64-1.1.0/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/build/html/searchindex.js` & `PyAPplus64-1.1.0/docs/build/html/searchindex.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -31,33 +31,34 @@
             [4, 2, 1, "", "dbQuerySingleRow"],
             [4, 2, 1, "", "dbQuerySingleRowDict"],
             [4, 2, 1, "", "dbQuerySingleValue"],
             [4, 2, 1, "", "dbQuerySingleValues"],
             [4, 3, 1, "", "db_conn"],
             [4, 3, 1, "", "db_settings"],
             [4, 2, 1, "", "execUseXMLRowDelete"],
-            [4, 2, 1, "", "getClient"],
+            [4, 2, 1, "", "getAppClient"],
             [4, 2, 1, "", "getTableFields"],
             [4, 2, 1, "", "getUniqueFieldsOfTable"],
+            [4, 2, 1, "", "getWebClient"],
             [4, 2, 1, "", "isDBTableKnown"],
             [4, 2, 1, "", "makeWebLink"],
             [4, 2, 1, "", "makeWebLinkBauftrag"],
             [4, 2, 1, "", "makeWebLinkWauftrag"],
             [4, 2, 1, "", "makeWebLinkWauftragPos"],
             [4, 2, 1, "", "mkUseXMLRowDelete"],
             [4, 2, 1, "", "mkUseXMLRowInsert"],
             [4, 2, 1, "", "mkUseXMLRowInsertOrUpdate"],
             [4, 2, 1, "", "mkUseXMLRowUpdate"],
             [4, 2, 1, "", "nextNumber"],
             [4, 2, 1, "", "reconnectDB"],
             [4, 3, 1, "", "scripttool"],
             [4, 3, 1, "", "server_conn"],
+            [4, 3, 1, "", "server_settings"],
             [4, 3, 1, "", "sysconf"],
-            [4, 2, 1, "", "useXML"],
-            [4, 3, 1, "", "web_settings"]
+            [4, 2, 1, "", "useXML"]
         ],
         "PyAPplus64.applus_db": [
             [4, 1, 1, "", "APplusDBSettings"],
             [4, 1, 1, "", "DBTableIDs"],
             [4, 4, 1, "", "getUniqueFieldsOfTable"],
             [4, 4, 1, "", "rawQuery"],
             [4, 4, 1, "", "rawQueryAll"],
@@ -77,35 +78,40 @@
             [4, 1, 1, "", "APplusScriptTool"],
             [4, 1, 1, "", "XMLDefinition"]
         ],
         "PyAPplus64.applus_scripttool.APplusScriptTool": [
             [4, 2, 1, "", "getCurrentDate"],
             [4, 2, 1, "", "getCurrentDateTime"],
             [4, 2, 1, "", "getCurrentTime"],
+            [4, 2, 1, "", "getInstallPath"],
+            [4, 2, 1, "", "getInstallPathAppServer"],
+            [4, 2, 1, "", "getInstallPathWebServer"],
             [4, 2, 1, "", "getLoginName"],
             [4, 2, 1, "", "getMandant"],
             [4, 2, 1, "", "getMandantName"],
+            [4, 2, 1, "", "getServerInfo"],
+            [4, 2, 1, "", "getServerInfoString"],
             [4, 2, 1, "", "getSystemName"],
             [4, 2, 1, "", "getUserFullName"],
             [4, 2, 1, "", "getUserName"],
             [4, 2, 1, "", "getXMLDefinition"],
             [4, 2, 1, "", "getXMLDefinitionObj"],
             [4, 2, 1, "", "getXMLDefinitionString"]
         ],
         "PyAPplus64.applus_scripttool.XMLDefinition": [
             [4, 2, 1, "", "getDuplicate"],
             [4, 3, 1, "", "root"]
         ],
         "PyAPplus64.applus_server": [
-            [4, 1, 1, "", "APplusAppServerSettings"],
             [4, 1, 1, "", "APplusServerConnection"],
-            [4, 1, 1, "", "APplusWebServerSettings"]
+            [4, 1, 1, "", "APplusServerSettings"]
         ],
         "PyAPplus64.applus_server.APplusServerConnection": [
-            [4, 2, 1, "", "getClient"]
+            [4, 2, 1, "", "getAppClient"],
+            [4, 2, 1, "", "getWebClient"]
         ],
         "PyAPplus64.applus_sysconf": [
             [4, 1, 1, "", "APplusSysConf"]
         ],
         "PyAPplus64.applus_sysconf.APplusSysConf": [
             [4, 2, 1, "", "clearCache"],
             [4, 2, 1, "", "getBoolean"],
@@ -327,62 +333,73 @@
     terms: {
         "0": [3, 4],
         "001": 3,
         "01": 3,
         "02d": 3,
         "04d": 3,
         "1": [3, 4],
-        "11": 4,
+        "10": 4,
+        "11": [],
         "12": 3,
         "14": [],
         "15": 3,
         "17": [],
         "18": [],
         "2": [0, 1, 3],
         "2012": 0,
         "2023": 4,
         "2037": 3,
-        "22": 4,
+        "22": [],
         "24": [],
         "247492": [],
         "247501": [],
         "247507": [],
-        "27": [],
+        "27": 4,
         "29": [],
         "3": 3,
+        "30": [],
+        "31": 4,
+        "391788": 4,
+        "391798": 4,
+        "391802": 4,
         "4": [2, 3],
         "45": [],
         "46": [],
         "48": [],
-        "5": [3, 4],
-        "50": 4,
+        "5": 3,
+        "50": [],
         "51": [],
         "533586": [],
         "533594": [],
         "533598": [],
         "58": [],
-        "6": [2, 4],
+        "6": 2,
+        "7": 4,
         "734716": [],
         "734722": [],
         "734726": [],
         "746273": [],
         "746286": [],
         "746292": [],
         "80523": [],
         "80533": [],
         "80538": [],
         "873776": [],
         "873786": [],
         "873790": [],
-        "888210": 4,
-        "888219": 4,
-        "888223": 4,
+        "888210": [],
+        "888219": [],
+        "888223": [],
+        "9": 4,
         "917696": [],
         "917703": [],
         "917707": [],
+        "952998": [],
+        "953005": [],
+        "953008": [],
         "\u00c4nderung": 4,
         "\u00c4nderungen": [1, 2, 4],
         "boolean": 4,
         "break": 3,
         "class": 4,
         "default": [3, 4],
         "do": 4,
@@ -529,14 +546,15 @@
         applusfromconf: 4,
         applusfromconfigdict: 4,
         applusfromconfigfil: [1, 3, 4],
         applusprod6: 3,
         applusscripttool: 4,
         applusserv: [3, 4],
         applusserverconnection: 4,
+        applusserversetting: 4,
         applussysconf: 4,
         appluswebserversetting: 4,
         apply: 4,
         appserv: [2, 3, 4],
         appserverport: 4,
         arbeit: 4,
         arbeitsplan: [2, 3, 4],
@@ -549,14 +567,15 @@
         artikelnam: 3,
         artikelneu: 3,
         artikelrec: 1,
         artikelstell: 3,
         artklassifnrlaeng: 3,
         as: [1, 3],
         as_posix: 3,
+        asmx: [3, 4],
         asol: 3,
         aspx: 1,
         at: [],
         attribut: [2, 4],
         aufgabenstell: 2,
         aufgeruf: 4,
         aufruf: [0, 1, 2, 4],
@@ -580,15 +599,15 @@
         auszuwahl: 4,
         automat: [1, 2, 3, 4],
         automatisi: 1,
         automatisiert: [0, 4],
         b: [2, 4],
         bas: 4,
         basedir: 3,
-        baseurl: [3, 4],
+        baseurl: 3,
         basi: 4,
         basicconf: 3,
         bat: 0,
         bau: 4,
         baufposag: 3,
         bauftrag: 3,
         be: [],
@@ -646,15 +665,15 @@
         check: [2, 4],
         checkdirexist: 4,
         checkexist: 4,
         checkfieldset: 4,
         checkfieldsset: 4,
         checkfileexist: 4,
         clearcach: 4,
-        client: [0, 1, 4],
+        client: [0, 1, 3, 4],
         clos: 3,
         close_when_date_chos: 3,
         cmd: 4,
         cmonth: 3,
         cnxn: 4,
         cod: 1,
         colnam: 3,
@@ -753,14 +772,15 @@
         docdir: [1, 3],
         doclib: [1, 3],
         docs: 0,
         document: [1, 3],
         doku: [0, 4],
         dokument: 4,
         dokumentation: 0,
+        domain: 3,
         drop: 3,
         dt: 4,
         dump: 3,
         dupaplan: 4,
         duplicat: 3,
         duplicatebusinessobject: [3, 4],
         duplicatebusinessobjekt: 4,
@@ -783,41 +803,43 @@
         einricht: [1, 3],
         einschliess: [3, 4],
         einstell: [3, 4],
         eintrag: [1, 4],
         einzeln: 4,
         einzig: 4,
         element: 4,
-        elementtre: 4,
+        elementtre: [],
         els: 3,
         emptycond: 4,
         engin: 4,
         entfernt: 4,
         enthalt: [2, 3, 4],
         entsprech: 4,
         entsprich: 4,
         entwed: 4,
         entwickelt: 1,
         entwickl: [1, 2],
         env: [3, 4],
         erfolgreich: 3,
         erfolgt: 1,
+        erganzt: 4,
         ergebnis: [1, 4],
         erlaub: 4,
         erlaubt: [1, 2, 3, 4],
         erled: 4,
         erleicht: 4,
         erleit: 4,
         erp: 2,
         error: 3,
         erschwert: 4,
         ersetz: 4,
         erst: 4,
         erstell: [1, 2, 3, 4],
         erstellt: 4,
+        erwartet: 4,
         erweit: 2,
         erweiter: 1,
         erweiternd: 4,
         erweitert: 4,
         erzeug: [1, 2, 3, 4],
         erzeugt: [0, 1, 3, 4],
         et: 4,
@@ -912,51 +934,55 @@
         genug: 1,
         genutzt: [1, 4],
         geparst: 4,
         geschaut: 4,
         gescheh: 4,
         geschickt: 4,
         geschrieb: [0, 1, 3],
-        gesetzt: [1, 2, 4],
+        gesetzt: [1, 2, 3, 4],
         gespeichert: [2, 3, 4],
         gestellt: 4,
         gesucht: 4,
         get: 3,
+        getappclient: [1, 4],
         getboolean: [3, 4],
-        getclient: [1, 4],
+        getclient: [],
         getcompletesql: 4,
         getcondition: 4,
         getconnectionstring: 4,
         getcurrentdat: [3, 4],
         getcurrentdatetim: [3, 4],
         getcurrenttim: [3, 4],
         getdoubl: 4,
         getduplicat: 4,
         getfield: 4,
         getfieldstocopyfortabl: 4,
-        getinstallpath: 3,
-        getinstallpathappserv: 3,
-        getinstallpathwebserv: [1, 3],
+        getinstallpath: [3, 4],
+        getinstallpathappserv: [3, 4],
+        getinstallpathwebserv: [1, 3, 4],
         getint: [3, 4],
         getjoin: 4,
         getlist: [1, 3, 4],
         getlogg: 3,
         getloginnam: [3, 4],
         getmandant: [3, 4],
         getmandantnam: [3, 4],
         getrennt: 4,
-        getserverinfo: 3,
+        getserverdat: 3,
+        getserverinfo: [3, 4],
+        getserverinfostring: 4,
         getsql: 4,
         getstring: [1, 3, 4],
         getsystemnam: [3, 4],
         gettabl: 4,
         gettablefield: 4,
         getuniquefieldsoftabl: 4,
         getuserfullnam: [3, 4],
         getusernam: [3, 4],
+        getwebclient: [3, 4],
         getxmldefinition: 4,
         getxmldefinitionobj: 4,
         getxmldefinitionstring: 4,
         geworf: 4,
         gibt: 4,
         gleich: [1, 4],
         governed: [],
@@ -1001,27 +1027,28 @@
         implementier: 1,
         implementiert: 2,
         importiert: 3,
         includ: 4,
         index: [3, 4],
         indic: 4,
         info: 3,
-        information: 3,
+        information: [3, 4],
         initfieldstocopyfortablecacheifneeded: 4,
         initialisier: 1,
         inklusiv: 3,
         inn: 4,
         inplac: 3,
         inputtext: 3,
         insbesond: 3,
         insdat: 4,
         insert: [3, 4],
         inspiziert: 4,
         install: 0,
         installiert: [0, 1],
+        installionspfad: 4,
         installpath: 3,
         installpathappserv: 3,
         installpathwebserv: 3,
         insus: 4,
         interaktion: 2,
         interessant: [1, 4],
         interfac: 4,
@@ -1059,15 +1086,15 @@
         konvertiert: 4,
         kopi: [2, 4],
         kopier: [2, 4],
         kopiert: [2, 4],
         korrekt: 1,
         kurz: 1,
         kwarg: 4,
-        l: 4,
+        l: [],
         lad: 4,
         ladeallewerkstattauftragmengenabweich: 3,
         ladeallewerkstattauftragposmengenabweich: 3,
         lambda: 3,
         langsam: 1,
         lass: [1, 2],
         lauf: 2,
@@ -1116,14 +1143,15 @@
         makeweblinkwauftragpos: [3, 4],
         manag: 3,
         mandant: [1, 2, 3, 4],
         mandanteninformation: 4,
         mandantnam: 3,
         maschin: 1,
         maskiert: 4,
+        masterdata: [3, 4],
         material: [1, 3],
         materiali: [1, 3],
         maximal: 4,
         md5: 4,
         mehr: 4,
         meist: [3, 4],
         meng: [3, 4],
@@ -1170,30 +1198,30 @@
         not: [1, 3],
         notig: [1, 4],
         now: 3,
         nr: 3,
         nscripttool: 3,
         nsysconf: 3,
         numm: [2, 3, 4],
-        nutz: 1,
+        nutz: [1, 3],
         nutzlich: 2,
         nutzt: 1,
         nutzung: [2, 4],
         nyear: 3,
         o: 0,
         oben: 1,
         ober: 4,
         oberflach: 2,
         obig: 1,
         obj: 4,
         object: [2, 4],
         objekt: [2, 4],
         odbc: [0, 4],
         of: 4,
-        oft: [1, 4],
+        oft: [1, 3, 4],
         ohn: [1, 4],
         on: 4,
         onlycopied: 4,
         op: 4,
         opensourc: [],
         operation: [1, 4],
         optional: [1, 3, 4],
@@ -1261,15 +1289,15 @@
         read: 3,
         read_sql: 4,
         rechenzeit: 1,
         rechn: 1,
         reconnectdb: 4,
         regelmass: 1,
         reicht: 4,
-        relativ: 1,
+        relativ: [1, 4],
         renam: 3,
         reord: 3,
         report: 2,
         reprasentation: 4,
         reprasentiert: 4,
         res: 3,
         resultier: 4,
@@ -1293,29 +1321,30 @@
         schreib: 3,
         schreibarbeit: 4,
         schreibend: [1, 2, 3],
         schreibt: 4,
         script: [1, 3],
         scripttool: [1, 3, 4],
         see: [],
+        seit: 4,
         selb: 4,
         select: [1, 3, 4],
         selektiert: 4,
         selt: 1,
         sep: [3, 4],
         sequenc: 4,
         seri: 4,
         serv: [0, 1, 2, 3, 4],
         server_conn: [1, 4],
         server_setting: 4,
         serverconfyamldeploy: 3,
         serverconfyamlprod: 3,
         serverconfyamlt: [1, 3],
         serverinfo: 3,
-        servic: [1, 4],
+        servic: [1, 3, 4],
         set: 4,
         setfield: [3, 4],
         setlevel: 3,
         setting: 4,
         settop: 4,
         setzend: 4,
         setzt: 4,
@@ -1474,18 +1503,20 @@
         upd: [1, 3, 4],
         updat: [1, 3, 4],
         updatedb: [1, 3],
         updateorinsert: 4,
         upddat: [1, 3, 4],
         updnam: 3,
         updus: [1, 3, 4],
+        url: 4,
         ursprung: 1,
         use: [],
         usecach: 4,
         user: [3, 4],
+        userdomain: 3,
         userfullnam: 3,
         usernam: 3,
         usexml: [1, 2, 4],
         usexmlrow: 4,
         usexmlrowdelet: 4,
         usexmlrowinsert: 4,
         usexmlrowinsertorupdat: 4,
@@ -1509,15 +1540,15 @@
         verglich: 4,
         verschied: 3,
         verschlimmert: 1,
         version: [2, 3, 4],
         vervollstand: 4,
         vervollstandigt: 4,
         verwend: [3, 4],
-        verwendet: [0, 1, 4],
+        verwendet: [0, 1, 3, 4],
         verwies: 1,
         verzeichnis: [0, 1, 3, 4],
         viele: [1, 4],
         vielen: [1, 3],
         vielleicht: 2,
         vonS: 3,
         vonok: 3,
@@ -1530,28 +1561,31 @@
         wahl: 3,
         wartungsarbeit: 1,
         wauftrag: 3,
         wauftragpos: 3,
         web: [2, 3, 4],
         web_setting: 4,
         weboberflach: 4,
-        webserv: 3,
+        webserv: [3, 4],
+        webserverpassword: 4,
+        webserverus: 4,
+        webserveruserdomain: 4,
         weit: [2, 4],
         welch: [1, 3, 4],
         werd: [0, 1, 2, 3, 4],
         werkstattauftrag: 3,
         werkstattauftragsposition: 3,
         wert: [1, 3, 4],
         wher: [1, 3, 4],
         whil: 3,
         wied: [3, 4],
         wiederum: 4,
         win_closed: 3,
         window: 3,
-        windows: 1,
+        windows: [1, 3],
         wirklich: [3, 4],
         wohl: 3,
         wortlich: 4,
         wrapp: [2, 4],
         writeexcelbuff: 4,
         wsdl: 4,
         wurd: [1, 2, 3, 4],
```

### Comparing `PyAPplus64-1.0.1/docs/make.bat` & `PyAPplus64-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/source/abhaengigkeiten.rst` & `PyAPplus64-1.1.0/docs/source/abhaengigkeiten.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 Abhängigkeiten
 ==============
 
 pyodbc
 ------
-Für die Datenbankverbindung wird ``pyodbc`` (``python -m pip install pyodbc``) verwendet. 
-Der passende ODBC Treiber, MS SQL Server 2012 Native Client, wird zusätzlich benötigt. 
+Für die Datenbankverbindung wird ``pyodbc`` (``python -m pip install pyodbc``) verwendet.
+Der passende ODBC Treiber, MS SQL Server 2012 Native Client, wird zusätzlich benötigt.
 Dieser kann von Microsoft bezogen werden.
 
 
 zeep
 ----
 Die Soap-Library ``zeep`` wird benutzt (``python -m pip install zeep``).
 
 
+requests-negotiate-sspi
+-----------------------
+Die Authentifzierungsmethode Negotiate Wird für Zugriffe auf ASMX-Seiten benutzt (``python -m pip install requests-negotiate-sspi``).
+Leider ist dies nur unter Windows verfügbar. Alle anderen Funktionen können aber auch ohne
+dieses Paket benutzt werden.
+
+
 PyYaml
 ------
 
 Die Library ``pyyaml`` wird für Config-Dateien benutzt (``python -m pip install pyyaml``).
 
 
-Sphinx 
+Sphinx
 ------
-Diese Dokumentation ist mit Sphinx geschrieben. 
-``python -m pip install sphinx``. Dokumentation ist im Unterverzeichnis 
-`docs` zu finden. Sie kann mittels ``make.bat html`` erzeugt werden, 
-dies ruft intern ``sphinx-build -M html source build`` auf. Die Dokumentation 
+Diese Dokumentation ist mit Sphinx geschrieben.
+``python -m pip install sphinx``. Dokumentation ist im Unterverzeichnis
+`docs` zu finden. Sie kann mittels ``make.bat html`` erzeugt werden,
+dies ruft intern ``sphinx-build -M html source build`` auf. Die Dokumentation
 der Python-API sollte evtl. vorher
 mittels ``sphinx-apidoc -T -f ../src/PyAPplus64 -o source/generated`` erzeugt
 oder aktualisiert werden. Evtl. können 2 Aufrufe von ``make.bat html`` sinnvoll
 sein, falls sich die Struktur der Dokumentation ändert.
 Diese Aufrufe werden von ``builddocs.sh`` automatisiert.
 
 Die erzeugte Doku findet sich im Verzeichnis ``build/html``.
 
 
 Pandas / SqlAlchemy / xlsxwriter
 --------------------------------
-Sollen Excel-Dateien mit Pandas erzeugt, werden, so muss Pandas, SqlAlchemy und xlsxwriter installiert sein 
-(`python -m pip install pandas sqlalchemy xlsxwriter`).
+Sollen Excel-Dateien mit Pandas erzeugt, werden, so muss Pandas, SqlAlchemy und xlsxwriter installiert sein
+(`python -m pip install pandas sqlalchemy xlsxwriter`).
+
```

### Comparing `PyAPplus64-1.0.1/docs/source/anwendungen.rst` & `PyAPplus64-1.1.0/docs/source/anwendungen.rst`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,14 @@
 werden automatisch die für die Umgebung nötigen Mandanten zu den SQL Statements hinzugefügt. Zudem ist einfach ein
 Zugriff auf die Sysconf möglich::
 
    print (server.sysconf.getString("STAMM", "MYLAND"))
    print (server.sysconf.getList("STAMM", "EULAENDER"))
 
 Dank der Bibliothek `zeep` ist es auch sehr einfach möglich, auf beliebige SOAP-Methoden zuzugreifen.
-Beispielsweise kann auf die Sys-Config auch händisch, d.h. durch direkten Aufruf einer SOAP-Methode,
-zugegriffen werden::
+Beispielsweise kann auf die Sys-Config auch händisch, d.h. durch direkten Aufruf einer SOAP-Methode
+des APP-Servers zugegriffen werden::
 
-   client = server.server_conn.getClient("p2system", "SysConf");
+   client = server.server_conn.getAppClient("p2system", "SysConf");
    print (client.service.getString("STAMM", "MYLAND"))
```

### Comparing `PyAPplus64-1.0.1/docs/source/beschreibung.rst` & `PyAPplus64-1.1.0/docs/source/beschreibung.rst`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/source/conf.py` & `PyAPplus64-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/docs/source/examples.rst` & `PyAPplus64-1.1.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/examples/adhoc_report.py` & `PyAPplus64-1.1.0/examples/adhoc_report.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/examples/applus-server.yaml` & `PyAPplus64-1.1.0/examples/applus-server.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 appserver : {
   server : "some-server",
   port : 2037,
   user : "asol.projects",
   env  : "default-umgebung" # hier wirklich Umgebung, nicht Mandant verwenden
 }
 webserver : {
-  baseurl : "http://some-server/APplusProd6/"
+  baseurl : "http://some-server/APplusProd6/",
+  user : null, # oft "ASOL.Projects", wenn nicht gesetzt, wird aktueller Windows-Nutzer verwendet
+  userDomain : null, # Domain für ASOL.PROJECTS
+  password : null # das Passwort
 }
 dbserver : {
   server : "some-server",
   db : "APplusProd6",
   user : "SA",
   password : "your-db-password"
 }
```

### Comparing `PyAPplus64-1.0.1/examples/check_dokumente.py` & `PyAPplus64-1.1.0/examples/check_dokumente.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/examples/copy_artikel.py` & `PyAPplus64-1.1.0/examples/copy_artikel.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/examples/mengenabweichung.py` & `PyAPplus64-1.1.0/examples/mengenabweichung.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/pyproject.toml` & `PyAPplus64-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyAPplus64"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="Thomas Tuerk", email="kontakt@thomas-tuerk.de" },
 ]
 description = "Verschiedene Hilfsmittel, um mit dem ERP System APplus zu interagieren. Dieses Packet wurde für APplus 6.4 entwickelt, funktioniert vermutlich aber auch mit anderen Versionen."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `PyAPplus64-1.0.1/src/PyAPplus64/__init__.py` & `PyAPplus64-1.1.0/src/PyAPplus64/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/src/PyAPplus64/applus.py` & `PyAPplus64-1.1.0/src/PyAPplus64/applus.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,22 +31,21 @@
     :param server_settings: die Einstellungen für die Verbindung mit dem APplus App Server
     :type server_settings: APplusAppServerSettings
     :param web_settings: die Einstellungen für die Verbindung mit dem APplus Web Server
     :type web_settings: APplusWebServerSettings
     """
     def __init__(self,
                  db_settings: applus_db.APplusDBSettings,
-                 server_settings: applus_server.APplusAppServerSettings,
-                 web_settings: applus_server.APplusWebServerSettings):
+                 server_settings: applus_server.APplusServerSettings):
 
         self.db_settings: applus_db.APplusDBSettings = db_settings
         """Die Einstellungen für die Datenbankverbindung"""
 
-        self.web_settings: applus_server.APplusWebServerSettings = web_settings
-        """Die Einstellungen für die Datenbankverbindung"""
+        self.server_settings : applus_server.APplusServerSettings = server_settings
+        """Einstellung für die Verbindung zum APP- und Webserver"""
 
         self.db_conn = db_settings.connect()
         """
         Eine pyodbc-Connection zur APplus DB. Diese muss genutzt werden, wenn mehrere Operationen in einer Transaktion
         genutzt werden sollen. Ansonsten sind die Hilfsmethoden wie :meth:`APplusServer.dbQuery` zu bevorzugen.
         Diese Connection kann in Verbindung mit den Funktionen aus :mod:`PyAPplus64.applus_db` genutzt werden.
         """
@@ -56,17 +55,17 @@
 
         self.sysconf: applus_sysconf.APplusSysConf = applus_sysconf.APplusSysConf(self)
         """erlaubt den Zugriff auf die Sysconfig"""
 
         self.scripttool: applus_scripttool.APplusScriptTool = applus_scripttool.APplusScriptTool(self)
         """erlaubt den einfachen Zugriff auf Funktionen des ScriptTools"""
 
-        self.client_table = self.server_conn.getClient("p2core", "Table")
-        self.client_xml = self.server_conn.getClient("p2core", "XML")
-        self.client_nummer = self.server_conn.getClient("p2system", "Nummer")
+        self.client_table = self.server_conn.getAppClient("p2core", "Table")
+        self.client_xml = self.server_conn.getAppClient("p2core", "XML")
+        self.client_nummer = self.server_conn.getAppClient("p2system", "Nummer")
 
     def reconnectDB(self) -> None:
         try:
             self.db_conn.close()
         except:
             pass
         self.db_conn = self.db_settings.connect()
@@ -126,30 +125,43 @@
 
     def isDBTableKnown(self, table: str) -> bool:
         """Prüft, ob eine Tabelle im System bekannt ist"""
         sql = "select count(*) from SYS.TABLES T where T.NAME=?"
         c = self.dbQuerySingleValue(sql, table)
         return (c > 0)
 
-    def getClient(self, package: str, name: str) -> Client:
-        """Erzeugt einen zeep - Client.
-           Mittels dieses Clients kann die WSDL Schnittstelle angesprochen werden.
+    def getAppClient(self, package: str, name: str) -> Client:
+        """Erzeugt einen zeep - Client für den APP-Server.
+           Mittels dieses Clients kann eines WSDL Schnittstelle des APP-Servers angesprochen werden.
            Wird als *package* "p2core" und als *name* "Table" verwendet und der
            resultierende client "client" genannt, dann kann
            z.B. mittels "client.service.getCompleteSQL(sql)" vom AppServer ein Vervollständigen
            des SQLs angefordert werden.
 
            :param package: das Packet, z.B. "p2core"
            :type package: str
            :param name: der Name im Packet, z.B. "Table"
            :type package: string
            :return: den Client
            :rtype: Client
            """
-        return self.server_conn.getClient(package, name)
+        return self.server_conn.getAppClient(package, name)
+
+    def getWebClient(self, url: str) -> Client:
+        """Erzeugt einen zeep - Client für den Web-Server.
+           Mittels dieses Clients kann die von einer ASMX-Seite zur Verfügung gestellte Schnittstelle angesprochen werden.
+           Als parameter wird die relative URL der ASMX-Seite erwartet. Die Base-URL automatisch ergänzt.
+           Ein Beispiel für eine solche relative URL ist "masterdata/artikel.asmx".
+
+           :param url: die relative URL der ASMX Seite, z.B. "masterdata/artikel.asmx"
+           :type package: str
+           :return: den Client
+           :rtype: Client
+           """
+        return self.server_conn.getWebClient(url)
 
     def getTableFields(self, table: str, isComputed: Optional[bool] = None) -> Set[str]:
         """
         Liefert die Namen aller Felder einer Tabelle.
 
         :param table: Name der Tabelle
         :param isComputed: wenn gesetzt, werden nur die Felder geliefert, die berechnet werden oder nicht berechnet werden
@@ -216,18 +228,18 @@
     def nextNumber(self, obj: str) -> str:
         """
         Erstellt eine neue Nummer für das Objekt und legt diese Nummer zurück.
         """
         return self.client_nummer.service.nextNumber(obj)
 
     def makeWebLink(self, base: str, **kwargs: Any) -> str:
-        if not self.web_settings.baseurl:
+        if not self.server_settings.webserver:
             raise Exception("keine Webserver-BaseURL gesetzt")
 
-        url = str(self.web_settings.baseurl) + base
+        url = str(self.server_settings.webserver) + base
         firstArg = True
         for arg, argv in kwargs.items():
             if not (argv is None):
                 if firstArg:
                     firstArg = False
                     url += "?"
                 else:
@@ -247,28 +259,29 @@
 
 def applusFromConfigDict(yamlDict: Dict[str, Any], user: Optional[str] = None, env: Optional[str] = None) -> APplusServer:
     """Läd Einstellungen aus einer Config und erzeugt daraus ein APplus-Objekt"""
     if user is None or user == '':
         user = yamlDict["appserver"]["user"]
     if env is None or env == '':
         env = yamlDict["appserver"]["env"]
-    app_server = applus_server.APplusAppServerSettings(
+    server_settings = applus_server.APplusServerSettings(
+        webserver=yamlDict.get("webserver", {}).get("baseurl", None),
         appserver=yamlDict["appserver"]["server"],
         appserverPort=yamlDict["appserver"]["port"],
         user=user,  # type: ignore
-        env=env)
-    web_server = applus_server.APplusWebServerSettings(
-        baseurl=yamlDict.get("webserver", {}).get("baseurl", None)
-    )
+        env=env,
+        webserverUser=yamlDict.get("webserver", {}).get("user", None),
+        webserverUserDomain=yamlDict.get("webserver", {}).get("userDomain", None),
+        webserverPassword=yamlDict.get("webserver", {}).get("password", None))
     dbparams = applus_db.APplusDBSettings(
         server=yamlDict["dbserver"]["server"],
         database=yamlDict["dbserver"]["db"],
         user=yamlDict["dbserver"]["user"],
         password=yamlDict["dbserver"]["password"])
-    return APplusServer(dbparams, app_server, web_server)
+    return APplusServer(dbparams, server_settings)
 
 
 def applusFromConfigFile(yamlfile: 'FileDescriptorOrPath',
                          user: Optional[str] = None, env: Optional[str] = None) -> APplusServer:
     """Läd Einstellungen aus einer Config-Datei und erzeugt daraus ein APplus-Objekt"""
     yamlDict = {}
     with open(yamlfile, "r") as stream:
```

### Comparing `PyAPplus64-1.0.1/src/PyAPplus64/applus_db.py` & `PyAPplus64-1.1.0/src/PyAPplus64/applus_db.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/src/PyAPplus64/applus_scripttool.py` & `PyAPplus64-1.1.0/src/PyAPplus64/applus_scripttool.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     :param server: die Verbindung zum Server
     :type server: APplusServerConnection
 
     """
 
     def __init__(self, server: APplusServer) -> None:
-        self.client = server.getClient("p2script", "ScriptTool")
+        self.client = server.getAppClient("p2script", "ScriptTool")
 
     def getCurrentDate(self) -> str:
         return self.client.service.getCurrentDate()
 
     def getCurrentTime(self) -> str:
         return self.client.service.getCurrentTime()
```

### Comparing `PyAPplus64-1.0.1/src/PyAPplus64/applus_sysconf.py` & `PyAPplus64-1.1.0/src/PyAPplus64/applus_sysconf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     :param server: die Verbindung zum Server
     :type server: APplusServer
 
     """
 
     def __init__(self, server: 'APplusServer') -> None:
-        self.client = server.getClient("p2system", "SysConf")
+        self.client = server.getAppClient("p2system", "SysConf")
         self.cache: Dict[str, type] = {}
 
     def clearCache(self) -> None:
         self.cache = {}
 
     def _getGeneral(self, ty: str, f: Callable[[str, str], Any], module: str, name: str, useCache: bool) -> Any:
         cacheKey = module + "/" + name + "/" + ty
```

### Comparing `PyAPplus64-1.0.1/src/PyAPplus64/applus_usexml.py` & `PyAPplus64-1.1.0/src/PyAPplus64/applus_usexml.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/src/PyAPplus64/duplicate.py` & `PyAPplus64-1.1.0/src/PyAPplus64/duplicate.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/src/PyAPplus64/pandas.py` & `PyAPplus64-1.1.0/src/PyAPplus64/pandas.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/src/PyAPplus64/sql_utils.py` & `PyAPplus64-1.1.0/src/PyAPplus64/sql_utils.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/src/PyAPplus64/utils.py` & `PyAPplus64-1.1.0/src/PyAPplus64/utils.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/src/PyAPplus64.egg-info/PKG-INFO` & `PyAPplus64-1.1.0/src/PyAPplus64.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAPplus64
-Version: 1.0.1
+Version: 1.1.0
 Summary: Verschiedene Hilfsmittel, um mit dem ERP System APplus zu interagieren. Dieses Packet wurde für APplus 6.4 entwickelt, funktioniert vermutlich aber auch mit anderen Versionen.
 Author-email: Thomas Tuerk <kontakt@thomas-tuerk.de>
 Project-URL: homepage, https://www.thomas-tuerk.de/de/pyapplus64
 Project-URL: repository, https://git.thomas-tuerk.de/thtuerk/PyAPplus64
 Project-URL: documentation, https://www.thomas-tuerk.de/assets/PyAPplus64/html/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,30 +13,30 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyAPplus64
 
-## Beschreibung 
-Das Paket `PyAPplus64` enthält eine Sammlung von Python Tools für die Interaktion mit dem ERP-System APplus 6.4. 
-Es sollte auch für andere APplus Versionen nützlich sein. 
+## Beschreibung
+Das Paket `PyAPplus64` enthält eine Sammlung von Python Tools für die Interaktion mit dem ERP-System APplus 6.4.
+Es sollte auch für andere APplus Versionen nützlich sein.
 
 Zielgruppe sind APplus-Administratoren und Anpassungs-Entwickler. Die Tools erlauben u.a.
 
 - einfacher Zugriff auf SOAP-Schnittstelle des App-Servers
    + damit Zugriff auf SysConfig
    + Zugriff auf Tools `nextNumber` für Erzeugung der nächsten Nummer für ein Business-Object
-   + ...   
+   + ...
 - Zugriff auf APplus DB per direktem DB-Zugriff und mittels SOAP
    + automatischer Aufruf von `completeSQL`, um per App-Server SQL-Statements um z.B. Mandanten erweitern zu lassen
    + Tools für einfache Benutzung von `useXML`, d.h. für das Einfügen, Löschen und Ändern von Datensätzen
-     mit Hilfe des APP-Servers. Genau wie bei Änderungen an Datensätzen über die Web-Oberfläche und im Gegensatz 
-     zum direkten Zugriff über die Datenbank werden dabei evtl. zusätzliche 
-     Checks ausgeführt, bestimmte Felder automatisch gesetzt oder bestimmte Aktionen angestoßen. 
+     mit Hilfe des APP-Servers. Genau wie bei Änderungen an Datensätzen über die Web-Oberfläche und im Gegensatz
+     zum direkten Zugriff über die Datenbank werden dabei evtl. zusätzliche
+     Checks ausgeführt, bestimmte Felder automatisch gesetzt oder bestimmte Aktionen angestoßen.
 - das Duplizieren von Datensätzen
    + zu kopierende Felder aus XML-Definitionen werden ausgewertet
    + Abhängige Objekte können einfach ebenfalls mit-kopiert werden
    + Änderungen wie beispielsweise Nummer des Objektes möglich
    + Unterstützung für Kopieren dyn. Attribute
    + Anlage neuer Objekte mittels APP-Server
    + Datensätze können zwischen Systemen kopiert und auch in Dateien gespeichert werden
@@ -48,26 +48,34 @@
 
 In `PyAPplus64` wurden die Features (vielleicht leicht verallgemeinert)
 implementiert, die ich für konkrete Aufgabenstellungen benötigte. Ich gehe davon
 aus, dass im Laufe der Zeit weitere Features hinzukommen.
 
 ## Warnung
 
-`PyAPplus64` erlaubt den schreibenden Zugriff auf die APplus Datenbank und beliebige 
-Aufrufe von SOAP-Methoden. Unsachgemäße Nutzung kann Ihre Daten zerstören. Benutzen Sie 
-`PyAPplus64` daher bitte vorsichtig. 
+`PyAPplus64` erlaubt den schreibenden Zugriff auf die APplus Datenbank und beliebige
+Aufrufe von SOAP-Methoden. Unsachgemäße Nutzung kann Ihre Daten zerstören. Benutzen Sie
+`PyAPplus64` daher bitte vorsichtig.
 
 ## Installation
 
 PyAPplus64 wurde auf PyPi veröffentlicht. Es lässt sich daher einfach mittel `pip` installieren
 
 ````
   pip install PyAPplus64
 ````
 
+Zur Nutzung von ASMX-Seiten ist die Authentifizierungsmethode Negotiate nötig. Für diese muss `requests-negotiate-sspi` installiert werden,
+was aber leider nur unter Windows verfügbar ist.
+
+````
+  pip install requests-negotiate-sspi
+````
+
+
 ## Links
 
 - [PyPi](https://pypi.org/project/PyAPplus64/)
 - Doku [PDF](https://www.thomas-tuerk.de/assets/PyAPplus64/pyapplus64.pdf), [HTML](https://www.thomas-tuerk.de/assets/PyAPplus64/html/index.html)
 - [GIT-Repository](https://git.thomas-tuerk.de/thtuerk/PyAPplus64)
 - [GitHub](https://github.com/thtuerk/PyAPplus64)
```

### Comparing `PyAPplus64-1.0.1/src/PyAPplus64.egg-info/SOURCES.txt` & `PyAPplus64-1.1.0/src/PyAPplus64.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/tests/test_applus_db.py` & `PyAPplus64-1.1.0/tests/test_applus_db.py`

 * *Files identical despite different names*

### Comparing `PyAPplus64-1.0.1/tests/test_sql_utils.py` & `PyAPplus64-1.1.0/tests/test_sql_utils.py`

 * *Files identical despite different names*

