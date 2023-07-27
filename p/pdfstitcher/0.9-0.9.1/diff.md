# Comparing `tmp/pdfstitcher-0.9.tar.gz` & `tmp/pdfstitcher-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfstitcher-0.9.tar", last modified: Wed Jul 26 17:47:02 2023, max compression
+gzip compressed data, was "pdfstitcher-0.9.1.tar", last modified: Thu Jul 27 15:40:17 2023, max compression
```

## Comparing `pdfstitcher-0.9.tar` & `pdfstitcher-0.9.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.348837 pdfstitcher-0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 17:46:23.000000 pdfstitcher-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-26 17:46:23.000000 pdfstitcher-0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23070 2023-07-26 17:47:02.348837 pdfstitcher-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-26 17:46:23.000000 pdfstitcher-0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.340838 pdfstitcher-0.9/pdfstitcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/bug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    21405 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/layerfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/cs_CZ/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.340838 pdfstitcher-0.9/pdfstitcher/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    18630 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.340838 pdfstitcher-0.9/pdfstitcher/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    18724 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.340838 pdfstitcher-0.9/pdfstitcher/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/es_ES/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.340838 pdfstitcher-0.9/pdfstitcher/locale/es_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    21711 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.340838 pdfstitcher-0.9/pdfstitcher/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    21412 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.344838 pdfstitcher-0.9/pdfstitcher/locale/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.344838 pdfstitcher-0.9/pdfstitcher/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19252 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/nb_NO/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.344838 pdfstitcher-0.9/pdfstitcher/locale/nb_NO/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    17562 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.344838 pdfstitcher-0.9/pdfstitcher/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.344838 pdfstitcher-0.9/pdfstitcher/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.344838 pdfstitcher-0.9/pdfstitcher/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.344838 pdfstitcher-0.9/pdfstitcher/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/zgh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.344838 pdfstitcher-0.9/pdfstitcher/locale/zgh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/zgh/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/zgh/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.336838 pdfstitcher-0.9/pdfstitcher/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.344838 pdfstitcher-0.9/pdfstitcher/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-26 17:46:53.000000 pdfstitcher-0.9/pdfstitcher/locale/zh_Hans/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/locale/zh_Hans/LC_MESSAGES/pdfstitcher.po
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/pagefilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/pdf_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.344838 pdfstitcher-0.9/pdfstitcher/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   342175 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/resources/stitcher-icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    25588 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/tile_pages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.348837 pdfstitcher-0.9/pdfstitcher/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/ui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/ui/io_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/ui/layers_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/ui/main_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/ui/tile_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/update_loc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    11795 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pdfstitcher/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.340838 pdfstitcher-0.9/pdfstitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23070 2023-07-26 17:47:02.000000 pdfstitcher-0.9/pdfstitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-26 17:47:02.000000 pdfstitcher-0.9/pdfstitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:47:02.000000 pdfstitcher-0.9/pdfstitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 17:47:02.000000 pdfstitcher-0.9/pdfstitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-26 17:47:02.000000 pdfstitcher-0.9/pdfstitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 17:47:02.000000 pdfstitcher-0.9/pdfstitcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-26 17:46:23.000000 pdfstitcher-0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:47:02.348837 pdfstitcher-0.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-07-26 17:46:23.000000 pdfstitcher-0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:47:02.348837 pdfstitcher-0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-26 17:46:23.000000 pdfstitcher-0.9/tests/test_tile_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.251669 pdfstitcher-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-07-27 15:40:17.251669 pdfstitcher-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.243669 pdfstitcher-0.9.1/pdfstitcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/bug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21405 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/layerfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.243669 pdfstitcher-0.9.1/pdfstitcher/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.239668 pdfstitcher-0.9.1/pdfstitcher/locale/cs_CZ/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.247669 pdfstitcher-0.9.1/pdfstitcher/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    18630 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.239668 pdfstitcher-0.9.1/pdfstitcher/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.247669 pdfstitcher-0.9.1/pdfstitcher/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    18724 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.239668 pdfstitcher-0.9.1/pdfstitcher/locale/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.247669 pdfstitcher-0.9.1/pdfstitcher/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.239668 pdfstitcher-0.9.1/pdfstitcher/locale/es_ES/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.247669 pdfstitcher-0.9.1/pdfstitcher/locale/es_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    21711 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.239668 pdfstitcher-0.9.1/pdfstitcher/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.247669 pdfstitcher-0.9.1/pdfstitcher/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    21412 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.239668 pdfstitcher-0.9.1/pdfstitcher/locale/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.247669 pdfstitcher-0.9.1/pdfstitcher/locale/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.239668 pdfstitcher-0.9.1/pdfstitcher/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.247669 pdfstitcher-0.9.1/pdfstitcher/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19252 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.239668 pdfstitcher-0.9.1/pdfstitcher/locale/nb_NO/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.247669 pdfstitcher-0.9.1/pdfstitcher/locale/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    17562 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.239668 pdfstitcher-0.9.1/pdfstitcher/locale/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.247669 pdfstitcher-0.9.1/pdfstitcher/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.239668 pdfstitcher-0.9.1/pdfstitcher/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.247669 pdfstitcher-0.9.1/pdfstitcher/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.239668 pdfstitcher-0.9.1/pdfstitcher/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.247669 pdfstitcher-0.9.1/pdfstitcher/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.243669 pdfstitcher-0.9.1/pdfstitcher/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.251669 pdfstitcher-0.9.1/pdfstitcher/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.243669 pdfstitcher-0.9.1/pdfstitcher/locale/zgh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.251669 pdfstitcher-0.9.1/pdfstitcher/locale/zgh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/zgh/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/zgh/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.243669 pdfstitcher-0.9.1/pdfstitcher/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.251669 pdfstitcher-0.9.1/pdfstitcher/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-27 15:40:06.000000 pdfstitcher-0.9.1/pdfstitcher/locale/zh_Hans/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/locale/zh_Hans/LC_MESSAGES/pdfstitcher.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/pagefilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/pdf_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.251669 pdfstitcher-0.9.1/pdfstitcher/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   342175 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/resources/stitcher-icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    25564 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/tile_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.251669 pdfstitcher-0.9.1/pdfstitcher/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/ui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/ui/io_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/ui/layers_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/ui/main_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/ui/tile_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/update_loc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pdfstitcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.247669 pdfstitcher-0.9.1/pdfstitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-07-27 15:40:17.000000 pdfstitcher-0.9.1/pdfstitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-27 15:40:17.000000 pdfstitcher-0.9.1/pdfstitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:40:17.000000 pdfstitcher-0.9.1/pdfstitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 15:40:17.000000 pdfstitcher-0.9.1/pdfstitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-27 15:40:17.000000 pdfstitcher-0.9.1/pdfstitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 15:40:17.000000 pdfstitcher-0.9.1/pdfstitcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 15:40:17.251669 pdfstitcher-0.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:40:17.251669 pdfstitcher-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-27 15:39:14.000000 pdfstitcher-0.9.1/tests/test_tile_pages.py
```

### Comparing `pdfstitcher-0.9/LICENSE` & `pdfstitcher-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/PKG-INFO` & `pdfstitcher-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfstitcher
-Version: 0.9
+Version: 0.9.1
 Summary: The open source PDF stitching software for sewists, by sewists.
 Author: Charlotte Curtis
 Author-email: c.f.curtis@gmail.com
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
```

### Comparing `pdfstitcher-0.9/README.md` & `pdfstitcher-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/app.py` & `pdfstitcher-0.9.1/pdfstitcher/app.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/bug_info.py` & `pdfstitcher-0.9.1/pdfstitcher/bug_info.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/layerfilter.py` & `pdfstitcher-0.9.1/pdfstitcher/layerfilter.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/zgh/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/zgh/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/zh_Hans/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.9.1/pdfstitcher/locale/zh_Hans/LC_MESSAGES/pdfstitcher.mo`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/locale/zh_Hans/LC_MESSAGES/pdfstitcher.po` & `pdfstitcher-0.9.1/pdfstitcher/locale/zh_Hans/LC_MESSAGES/pdfstitcher.po`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/pagefilter.py` & `pdfstitcher-0.9.1/pdfstitcher/pagefilter.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/pdf_operators.py` & `pdfstitcher-0.9.1/pdfstitcher/pdf_operators.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/resources/stitcher-icon.ico` & `pdfstitcher-0.9.1/pdfstitcher/resources/stitcher-icon.ico`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/tile_pages.py` & `pdfstitcher-0.9.1/pdfstitcher/tile_pages.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,15 +347,15 @@
 
         # Make sure there are no empty columns or rows
         if self.col_major:
             return self.cols * self.rows - n_tiles < self.rows
         else:
             return self.cols * self.rows - n_tiles < self.cols
 
-    def grid_position(self, tile_i: int) -> tuple[int, int]:
+    def grid_position(self, tile_i: int) -> tuple:
         """Determines the placement of the tile in the grid, returning a tuple of (row, col)"""
         if self.col_major:
             c = math.floor(tile_i / self.rows)
             r = tile_i % self.rows
         else:
             r = math.floor(tile_i / self.cols)
             c = tile_i % self.cols
@@ -364,15 +364,15 @@
             c = self.cols - c - 1
 
         if self.bottom_to_top:
             r = self.rows - r - 1
 
         return r, c
 
-    def calc_shift(self, horizontal_space: float, vertical_space: float) -> tuple[float, float]:
+    def calc_shift(self, horizontal_space: float, vertical_space: float) -> tuple:
         """
         Calculates the shift needed to align the tile in the grid.
         Returns a tuple of (shift_right, shift_up).
         Only used if a tile is smaller than the grid space.
         """
         if self.horizontal_align is SW_ALIGN_H.LEFT:
             shift_right = 0
```

### Comparing `pdfstitcher-0.9/pdfstitcher/ui/dialogs.py` & `pdfstitcher-0.9.1/pdfstitcher/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/ui/io_tab.py` & `pdfstitcher-0.9.1/pdfstitcher/ui/io_tab.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/ui/layers_tab.py` & `pdfstitcher-0.9.1/pdfstitcher/ui/layers_tab.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/ui/main_frame.py` & `pdfstitcher-0.9.1/pdfstitcher/ui/main_frame.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/ui/tile_tab.py` & `pdfstitcher-0.9.1/pdfstitcher/ui/tile_tab.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/update_loc.py` & `pdfstitcher-0.9.1/pdfstitcher/update_loc.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/updater.py` & `pdfstitcher-0.9.1/pdfstitcher/updater.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pdfstitcher/utils.py` & `pdfstitcher-0.9.1/pdfstitcher/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
         meta["xmp:CreatorTool"] = "PDFStitcher " + VERSION_STRING
 
     return new_doc
 
 
 def get_page_dims(
     page, global_rotation: float = 0, target_user_unit: float = 1
-) -> tuple[float, float]:
+) -> tuple:
     """
     Helper function to calculate the page dimensions
     Returns width, height in pixels as observed by the user
     (taking rotation and UserUnit into account)
     """
     # The mediabox is typically specified as
     # [lower left x, lower left y, upper left x, upper left y],
```

### Comparing `pdfstitcher-0.9/pdfstitcher.egg-info/PKG-INFO` & `pdfstitcher-0.9.1/pdfstitcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfstitcher
-Version: 0.9
+Version: 0.9.1
 Summary: The open source PDF stitching software for sewists, by sewists.
 Author: Charlotte Curtis
 Author-email: c.f.curtis@gmail.com
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
```

### Comparing `pdfstitcher-0.9/pdfstitcher.egg-info/SOURCES.txt` & `pdfstitcher-0.9.1/pdfstitcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.9/pyproject.toml` & `pdfstitcher-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdfstitcher"
-version = "0.9"
+version = "0.9.1"
 description = "The open source PDF stitching software for sewists, by sewists."
 readme = "README.md"
 requires-python = ">=3.8, <3.11"
 license = {file = "LICENSE"}
 keywords = ["pdf", "sewing", "utility", "stitch", "n-up", "page imposition"]
 authors = [
     {name = "Charlotte Curtis"},
```

### Comparing `pdfstitcher-0.9/setup.py` & `pdfstitcher-0.9.1/setup.py`

 * *Files identical despite different names*

