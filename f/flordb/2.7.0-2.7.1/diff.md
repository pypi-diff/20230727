# Comparing `tmp/flordb-2.7.0.tar.gz` & `tmp/flordb-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flordb-2.7.0.tar", last modified: Thu Jul 20 18:12:11 2023, max compression
+gzip compressed data, was "flordb-2.7.1.tar", last modified: Thu Jul 27 19:19:41 2023, max compression
```

## Comparing `flordb-2.7.0.tar` & `flordb-2.7.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.739399 flordb-2.7.0/
--rw-r--r--   0 rogarcia   (501) staff       (20)    11357 2023-03-12 17:55:35.000000 flordb-2.7.0/LICENSE
--rw-r--r--   0 rogarcia   (501) staff       (20)    19202 2023-07-20 18:12:11.739253 flordb-2.7.0/PKG-INFO
--rw-r--r--   0 rogarcia   (501) staff       (20)    18770 2023-07-20 17:48:12.000000 flordb-2.7.0/README.md
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.730409 flordb-2.7.0/flor/
--rw-r--r--   0 rogarcia   (501) staff       (20)      281 2023-05-24 17:15:50.000000 flordb-2.7.0/flor/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3100 2023-07-20 16:43:24.000000 flordb-2.7.0/flor/__main__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      922 2023-05-17 00:21:40.000000 flordb-2.7.0/flor/batch.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      544 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/constants.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     6150 2023-07-03 18:24:51.000000 flordb-2.7.0/flor/database.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     6481 2023-07-18 16:49:26.000000 flordb-2.7.0/flor/flags.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.731065 flordb-2.7.0/flor/hlast/
--rw-r--r--   0 rogarcia   (501) staff       (20)     4677 2023-07-20 16:43:24.000000 flordb-2.7.0/flor/hlast/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8884 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gtpropagate.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.732325 flordb-2.7.0/flor/hlast/gumtree/
--rw-r--r--   0 rogarcia   (501) staff       (20)     6337 2023-06-19 14:24:18.000000 flordb-2.7.0/flor/hlast/gumtree/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2916 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gumtree/adapter.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gumtree/idmap.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1085 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gumtree/priorityq.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2110 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gumtree/python.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     8350 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gumtree/test.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      903 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/hlast/gumtree/tree.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3195 2023-06-19 14:24:18.000000 flordb-2.7.0/flor/hlast/visitors.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2634 2023-07-05 15:29:17.000000 flordb-2.7.0/flor/iterator.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.732458 flordb-2.7.0/flor/journal/
--rw-r--r--   0 rogarcia   (501) staff       (20)     2955 2023-07-05 15:27:49.000000 flordb-2.7.0/flor/journal/__init__.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.732895 flordb-2.7.0/flor/journal/entry/
--rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      710 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      284 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/constants.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.733859 flordb-2.7.0/flor/journal/entry/data/
--rw-r--r--   0 rogarcia   (501) staff       (20)      427 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/data/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      588 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/data/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2073 2023-03-23 13:19:05.000000 flordb-2.7.0/flor/journal/entry/data/dataframe.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2093 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/data/reference.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1904 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/data/torch_chkpt.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      711 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/data/value.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.734627 flordb-2.7.0/flor/journal/entry/metadata/
--rw-r--r--   0 rogarcia   (501) staff       (20)      149 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/metadata/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      461 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/metadata/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      741 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/metadata/bracket.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1032 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/entry/metadata/eof.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.735231 flordb-2.7.0/flor/journal/tree/
--rw-r--r--   0 rogarcia   (501) staff       (20)       23 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/tree/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1285 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/tree/block.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      929 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/tree/group.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3472 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/journal/tree/tree.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     4323 2023-07-05 15:27:49.000000 flordb-2.7.0/flor/journal/tree/window.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2046 2023-07-05 15:30:58.000000 flordb-2.7.0/flor/kits.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.736065 flordb-2.7.0/flor/logger/
--rw-r--r--   0 rogarcia   (501) staff       (20)     3518 2023-06-19 14:24:18.000000 flordb-2.7.0/flor/logger/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2179 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/logger/checkpoint_logger.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1592 2023-05-04 17:16:10.000000 flordb-2.7.0/flor/logger/exp_json.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      536 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/logger/future.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2013 2023-03-16 16:35:51.000000 flordb-2.7.0/flor/logger/log_records.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.736996 flordb-2.7.0/flor/query/
--rw-r--r--   0 rogarcia   (501) staff       (20)     9665 2023-07-20 16:43:24.000000 flordb-2.7.0/flor/query/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3663 2023-07-05 15:29:55.000000 flordb-2.7.0/flor/query/database.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1769 2023-07-05 15:30:42.000000 flordb-2.7.0/flor/query/engine.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2481 2023-07-20 16:43:24.000000 flordb-2.7.0/flor/query/pivot.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     9686 2023-07-20 17:21:04.000000 flordb-2.7.0/flor/query/unpack.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.737401 flordb-2.7.0/flor/shelf/
--rw-r--r--   0 rogarcia   (501) staff       (20)        0 2023-03-12 17:55:35.000000 flordb-2.7.0/flor/shelf/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     5063 2023-07-19 21:03:15.000000 flordb-2.7.0/flor/shelf/cwd_shelf.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3176 2023-05-10 13:18:25.000000 flordb-2.7.0/flor/shelf/home_shelf.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.738514 flordb-2.7.0/flor/skipblock/
--rw-r--r--   0 rogarcia   (501) staff       (20)       32 2023-03-12 17:55:36.000000 flordb-2.7.0/flor/skipblock/__init__.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      689 2023-03-12 17:55:36.000000 flordb-2.7.0/flor/skipblock/abstract.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     2623 2023-03-22 14:08:08.000000 flordb-2.7.0/flor/skipblock/readblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      349 2023-03-12 17:55:36.000000 flordb-2.7.0/flor/skipblock/seemblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     3819 2023-04-14 18:08:18.000000 flordb-2.7.0/flor/skipblock/writeblock.py
--rw-r--r--   0 rogarcia   (501) staff       (20)      913 2023-06-19 14:24:18.000000 flordb-2.7.0/flor/state.py
--rw-r--r--   0 rogarcia   (501) staff       (20)     1078 2023-05-24 17:15:50.000000 flordb-2.7.0/flor/utils.py
-drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-20 18:12:11.739116 flordb-2.7.0/flordb.egg-info/
--rw-r--r--   0 rogarcia   (501) staff       (20)    19202 2023-07-20 18:12:11.000000 flordb-2.7.0/flordb.egg-info/PKG-INFO
--rw-r--r--   0 rogarcia   (501) staff       (20)     1684 2023-07-20 18:12:11.000000 flordb-2.7.0/flordb.egg-info/SOURCES.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)        1 2023-07-20 18:12:11.000000 flordb-2.7.0/flordb.egg-info/dependency_links.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)       91 2023-07-20 18:12:11.000000 flordb-2.7.0/flordb.egg-info/requires.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)        5 2023-07-20 18:12:11.000000 flordb-2.7.0/flordb.egg-info/top_level.txt
--rw-r--r--   0 rogarcia   (501) staff       (20)       38 2023-07-20 18:12:11.739432 flordb-2.7.0/setup.cfg
--rw-r--r--   0 rogarcia   (501) staff       (20)      904 2023-07-20 18:10:15.000000 flordb-2.7.0/setup.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.873298 flordb-2.7.1/
+-rw-r--r--   0 rogarcia   (501) staff       (20)    11357 2023-03-12 17:55:35.000000 flordb-2.7.1/LICENSE
+-rw-r--r--   0 rogarcia   (501) staff       (20)    19422 2023-07-27 19:19:41.873159 flordb-2.7.1/PKG-INFO
+-rw-r--r--   0 rogarcia   (501) staff       (20)    18990 2023-07-20 20:13:32.000000 flordb-2.7.1/README.md
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.864023 flordb-2.7.1/flor/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      281 2023-05-24 17:15:50.000000 flordb-2.7.1/flor/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3100 2023-07-20 16:43:24.000000 flordb-2.7.1/flor/__main__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      922 2023-05-17 00:21:40.000000 flordb-2.7.1/flor/batch.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      544 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/constants.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6150 2023-07-03 18:24:51.000000 flordb-2.7.1/flor/database.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6481 2023-07-18 16:49:26.000000 flordb-2.7.1/flor/flags.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.864641 flordb-2.7.1/flor/hlast/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4677 2023-07-20 16:43:24.000000 flordb-2.7.1/flor/hlast/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8884 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/hlast/gtpropagate.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.865809 flordb-2.7.1/flor/hlast/gumtree/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     6337 2023-06-19 14:24:18.000000 flordb-2.7.1/flor/hlast/gumtree/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2916 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/hlast/gumtree/adapter.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/hlast/gumtree/idmap.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1085 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/hlast/gumtree/priorityq.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2110 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/hlast/gumtree/python.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     8350 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/hlast/gumtree/test.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      903 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/hlast/gumtree/tree.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3195 2023-06-19 14:24:18.000000 flordb-2.7.1/flor/hlast/visitors.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2634 2023-07-05 15:29:17.000000 flordb-2.7.1/flor/iterator.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.865995 flordb-2.7.1/flor/journal/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2955 2023-07-05 15:27:49.000000 flordb-2.7.1/flor/journal/__init__.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.866429 flordb-2.7.1/flor/journal/entry/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      876 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/entry/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      710 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/entry/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      284 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/entry/constants.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.867512 flordb-2.7.1/flor/journal/entry/data/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      427 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/entry/data/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      588 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/entry/data/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2073 2023-03-23 13:19:05.000000 flordb-2.7.1/flor/journal/entry/data/dataframe.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2093 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/entry/data/reference.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1904 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/entry/data/torch_chkpt.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      711 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/entry/data/value.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.868282 flordb-2.7.1/flor/journal/entry/metadata/
+-rw-r--r--   0 rogarcia   (501) staff       (20)      149 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/entry/metadata/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      461 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/entry/metadata/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      741 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/entry/metadata/bracket.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1032 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/entry/metadata/eof.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.868915 flordb-2.7.1/flor/journal/tree/
+-rw-r--r--   0 rogarcia   (501) staff       (20)       23 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/tree/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1285 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/tree/block.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      929 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/tree/group.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3472 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/journal/tree/tree.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     4323 2023-07-05 15:27:49.000000 flordb-2.7.1/flor/journal/tree/window.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2046 2023-07-05 15:30:58.000000 flordb-2.7.1/flor/kits.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.869849 flordb-2.7.1/flor/logger/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3518 2023-06-19 14:24:18.000000 flordb-2.7.1/flor/logger/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2179 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/logger/checkpoint_logger.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1592 2023-05-04 17:16:10.000000 flordb-2.7.1/flor/logger/exp_json.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      536 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/logger/future.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2013 2023-03-16 16:35:51.000000 flordb-2.7.1/flor/logger/log_records.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.870900 flordb-2.7.1/flor/query/
+-rw-r--r--   0 rogarcia   (501) staff       (20)     9665 2023-07-20 16:43:24.000000 flordb-2.7.1/flor/query/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3663 2023-07-05 15:29:55.000000 flordb-2.7.1/flor/query/database.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1769 2023-07-05 15:30:42.000000 flordb-2.7.1/flor/query/engine.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2481 2023-07-20 16:43:24.000000 flordb-2.7.1/flor/query/pivot.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     9686 2023-07-20 17:21:04.000000 flordb-2.7.1/flor/query/unpack.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.871423 flordb-2.7.1/flor/shelf/
+-rw-r--r--   0 rogarcia   (501) staff       (20)        0 2023-03-12 17:55:35.000000 flordb-2.7.1/flor/shelf/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     5063 2023-07-19 21:03:15.000000 flordb-2.7.1/flor/shelf/cwd_shelf.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3176 2023-05-10 13:18:25.000000 flordb-2.7.1/flor/shelf/home_shelf.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.872266 flordb-2.7.1/flor/skipblock/
+-rw-r--r--   0 rogarcia   (501) staff       (20)       32 2023-03-12 17:55:36.000000 flordb-2.7.1/flor/skipblock/__init__.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      689 2023-03-12 17:55:36.000000 flordb-2.7.1/flor/skipblock/abstract.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     2623 2023-03-22 14:08:08.000000 flordb-2.7.1/flor/skipblock/readblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      349 2023-03-12 17:55:36.000000 flordb-2.7.1/flor/skipblock/seemblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     3819 2023-04-14 18:08:18.000000 flordb-2.7.1/flor/skipblock/writeblock.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)      913 2023-06-19 14:24:18.000000 flordb-2.7.1/flor/state.py
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1078 2023-05-24 17:15:50.000000 flordb-2.7.1/flor/utils.py
+drwxr-xr-x   0 rogarcia   (501) staff       (20)        0 2023-07-27 19:19:41.873011 flordb-2.7.1/flordb.egg-info/
+-rw-r--r--   0 rogarcia   (501) staff       (20)    19422 2023-07-27 19:19:41.000000 flordb-2.7.1/flordb.egg-info/PKG-INFO
+-rw-r--r--   0 rogarcia   (501) staff       (20)     1684 2023-07-27 19:19:41.000000 flordb-2.7.1/flordb.egg-info/SOURCES.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)        1 2023-07-27 19:19:41.000000 flordb-2.7.1/flordb.egg-info/dependency_links.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)       91 2023-07-27 19:19:41.000000 flordb-2.7.1/flordb.egg-info/requires.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)        5 2023-07-27 19:19:41.000000 flordb-2.7.1/flordb.egg-info/top_level.txt
+-rw-r--r--   0 rogarcia   (501) staff       (20)       38 2023-07-27 19:19:41.873331 flordb-2.7.1/setup.cfg
+-rw-r--r--   0 rogarcia   (501) staff       (20)      904 2023-07-27 19:19:11.000000 flordb-2.7.1/setup.py
```

### Comparing `flordb-2.7.0/LICENSE` & `flordb-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/PKG-INFO` & `flordb-2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: flordb
-Version: 2.7.0
+Version: 2.7.1
 Summary: Fast Low-Overhead Recovery
 Home-page: https://github.com/ucbrise/flor
 Author: Rolando Garcia
 Author-email: rogarcia@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 FlorDB: Nimble Experiment Management for Iterative ML
 ================================
+[![PyPI](https://img.shields.io/pypi/v/flordb)](https://pypi.org/project/flordb/)
+
 
 Flor (for "fast low-overhead recovery") is a record-replay system for deep learning, and other forms of machine learning that train models on GPUs. Flor was developed to speed-up hindsight logging: a cyclic-debugging practice that involves adding logging statements *after* encountering a surprise, and efficiently re-training with more logging. Flor takes low-overhead checkpoints during training, or the record phase, and uses those checkpoints for replay speedups based on memoization and parallelism.
 
 FlorDB integrates Flor, `git` and `sqlite3` to manage model developer's logs, execution data, versions of code, and training checkpoints. In addition to serving as an experiment management solution for ML Engineers, FlorDB extends hindsight logging across model trainging versions for the retroactive evaluation of iterative ML.
 
 Flor and FlorDB are software developed at UC Berkeley's [RISE](https://rise.cs.berkeley.edu/) Lab.
 
-[![Napa Retreat Demo](https://i.ytimg.com/vi/TNSt5-i7kR4/sddefault.jpg)](https://youtu.be/TNSt5-i7kR4)
+<!-- [![Napa Retreat Demo](https://i.ytimg.com/vi/TNSt5-i7kR4/sddefault.jpg)](https://youtu.be/TNSt5-i7kR4) -->
+
+You can follow along yourself by starting a Jupyter server from this directory and opening [`tutorial.ipynb`](tutorial.ipynb).
 
 # Installation
 
 ```bash
 pip install flordb
 ```
```

### Comparing `flordb-2.7.0/README.md` & `flordb-2.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 FlorDB: Nimble Experiment Management for Iterative ML
 ================================
+[![PyPI](https://img.shields.io/pypi/v/flordb)](https://pypi.org/project/flordb/)
+
 
 Flor (for "fast low-overhead recovery") is a record-replay system for deep learning, and other forms of machine learning that train models on GPUs. Flor was developed to speed-up hindsight logging: a cyclic-debugging practice that involves adding logging statements *after* encountering a surprise, and efficiently re-training with more logging. Flor takes low-overhead checkpoints during training, or the record phase, and uses those checkpoints for replay speedups based on memoization and parallelism.
 
 FlorDB integrates Flor, `git` and `sqlite3` to manage model developer's logs, execution data, versions of code, and training checkpoints. In addition to serving as an experiment management solution for ML Engineers, FlorDB extends hindsight logging across model trainging versions for the retroactive evaluation of iterative ML.
 
 Flor and FlorDB are software developed at UC Berkeley's [RISE](https://rise.cs.berkeley.edu/) Lab.
 
-[![Napa Retreat Demo](https://i.ytimg.com/vi/TNSt5-i7kR4/sddefault.jpg)](https://youtu.be/TNSt5-i7kR4)
+<!-- [![Napa Retreat Demo](https://i.ytimg.com/vi/TNSt5-i7kR4/sddefault.jpg)](https://youtu.be/TNSt5-i7kR4) -->
+
+You can follow along yourself by starting a Jupyter server from this directory and opening [`tutorial.ipynb`](tutorial.ipynb).
 
 # Installation
 
 ```bash
 pip install flordb
 ```
```

### Comparing `flordb-2.7.0/flor/__main__.py` & `flordb-2.7.1/flor/__main__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/batch.py` & `flordb-2.7.1/flor/batch.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/constants.py` & `flordb-2.7.1/flor/constants.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/database.py` & `flordb-2.7.1/flor/database.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/flags.py` & `flordb-2.7.1/flor/flags.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/hlast/__init__.py` & `flordb-2.7.1/flor/hlast/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/hlast/gtpropagate.py` & `flordb-2.7.1/flor/hlast/gtpropagate.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/hlast/gumtree/__init__.py` & `flordb-2.7.1/flor/hlast/gumtree/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/hlast/gumtree/adapter.py` & `flordb-2.7.1/flor/hlast/gumtree/adapter.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/hlast/gumtree/idmap.py` & `flordb-2.7.1/flor/hlast/gumtree/idmap.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/hlast/gumtree/priorityq.py` & `flordb-2.7.1/flor/hlast/gumtree/priorityq.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/hlast/gumtree/python.py` & `flordb-2.7.1/flor/hlast/gumtree/python.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/hlast/gumtree/test.py` & `flordb-2.7.1/flor/hlast/gumtree/test.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/hlast/gumtree/tree.py` & `flordb-2.7.1/flor/hlast/gumtree/tree.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/hlast/visitors.py` & `flordb-2.7.1/flor/hlast/visitors.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/iterator.py` & `flordb-2.7.1/flor/iterator.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/__init__.py` & `flordb-2.7.1/flor/journal/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/entry/__init__.py` & `flordb-2.7.1/flor/journal/entry/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/entry/abstract.py` & `flordb-2.7.1/flor/journal/entry/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/entry/data/abstract.py` & `flordb-2.7.1/flor/journal/entry/data/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/entry/data/dataframe.py` & `flordb-2.7.1/flor/journal/entry/data/dataframe.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/entry/data/reference.py` & `flordb-2.7.1/flor/journal/entry/data/reference.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/entry/data/torch_chkpt.py` & `flordb-2.7.1/flor/journal/entry/data/torch_chkpt.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/entry/data/value.py` & `flordb-2.7.1/flor/journal/entry/data/value.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/entry/metadata/bracket.py` & `flordb-2.7.1/flor/journal/entry/metadata/bracket.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/entry/metadata/eof.py` & `flordb-2.7.1/flor/journal/entry/metadata/eof.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/tree/block.py` & `flordb-2.7.1/flor/journal/tree/block.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/tree/group.py` & `flordb-2.7.1/flor/journal/tree/group.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/tree/tree.py` & `flordb-2.7.1/flor/journal/tree/tree.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/journal/tree/window.py` & `flordb-2.7.1/flor/journal/tree/window.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/kits.py` & `flordb-2.7.1/flor/kits.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/logger/__init__.py` & `flordb-2.7.1/flor/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/logger/checkpoint_logger.py` & `flordb-2.7.1/flor/logger/checkpoint_logger.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/logger/exp_json.py` & `flordb-2.7.1/flor/logger/exp_json.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/logger/future.py` & `flordb-2.7.1/flor/logger/future.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/logger/log_records.py` & `flordb-2.7.1/flor/logger/log_records.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/query/__init__.py` & `flordb-2.7.1/flor/query/__init__.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/query/database.py` & `flordb-2.7.1/flor/query/database.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/query/engine.py` & `flordb-2.7.1/flor/query/engine.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/query/pivot.py` & `flordb-2.7.1/flor/query/pivot.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/query/unpack.py` & `flordb-2.7.1/flor/query/unpack.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/shelf/cwd_shelf.py` & `flordb-2.7.1/flor/shelf/cwd_shelf.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/shelf/home_shelf.py` & `flordb-2.7.1/flor/shelf/home_shelf.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/skipblock/abstract.py` & `flordb-2.7.1/flor/skipblock/abstract.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/skipblock/readblock.py` & `flordb-2.7.1/flor/skipblock/readblock.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/skipblock/writeblock.py` & `flordb-2.7.1/flor/skipblock/writeblock.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/state.py` & `flordb-2.7.1/flor/state.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flor/utils.py` & `flordb-2.7.1/flor/utils.py`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/flordb.egg-info/PKG-INFO` & `flordb-2.7.1/flordb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: flordb
-Version: 2.7.0
+Version: 2.7.1
 Summary: Fast Low-Overhead Recovery
 Home-page: https://github.com/ucbrise/flor
 Author: Rolando Garcia
 Author-email: rogarcia@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 FlorDB: Nimble Experiment Management for Iterative ML
 ================================
+[![PyPI](https://img.shields.io/pypi/v/flordb)](https://pypi.org/project/flordb/)
+
 
 Flor (for "fast low-overhead recovery") is a record-replay system for deep learning, and other forms of machine learning that train models on GPUs. Flor was developed to speed-up hindsight logging: a cyclic-debugging practice that involves adding logging statements *after* encountering a surprise, and efficiently re-training with more logging. Flor takes low-overhead checkpoints during training, or the record phase, and uses those checkpoints for replay speedups based on memoization and parallelism.
 
 FlorDB integrates Flor, `git` and `sqlite3` to manage model developer's logs, execution data, versions of code, and training checkpoints. In addition to serving as an experiment management solution for ML Engineers, FlorDB extends hindsight logging across model trainging versions for the retroactive evaluation of iterative ML.
 
 Flor and FlorDB are software developed at UC Berkeley's [RISE](https://rise.cs.berkeley.edu/) Lab.
 
-[![Napa Retreat Demo](https://i.ytimg.com/vi/TNSt5-i7kR4/sddefault.jpg)](https://youtu.be/TNSt5-i7kR4)
+<!-- [![Napa Retreat Demo](https://i.ytimg.com/vi/TNSt5-i7kR4/sddefault.jpg)](https://youtu.be/TNSt5-i7kR4) -->
+
+You can follow along yourself by starting a Jupyter server from this directory and opening [`tutorial.ipynb`](tutorial.ipynb).
 
 # Installation
 
 ```bash
 pip install flordb
 ```
```

### Comparing `flordb-2.7.0/flordb.egg-info/SOURCES.txt` & `flordb-2.7.1/flordb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flordb-2.7.0/setup.py` & `flordb-2.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io
 
 with io.open("README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="flordb",
-    version="2.7.0",
+    version="2.7.1",
     author="Rolando Garcia",
     author_email="rogarcia@berkeley.edu",
     description="Fast Low-Overhead Recovery",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ucbrise/flor",
     packages=setuptools.find_packages(),
```

