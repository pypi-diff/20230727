# Comparing `tmp/wikidata_dl-2022.3.4.tar.gz` & `tmp/wikidata_dl-2023.7.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikidata_dl-2022.3.4.tar", last modified: Fri Mar  4 15:16:00 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `wikidata_dl-2022.3.4.tar` & `wikidata_dl-2023.7.27.tar`

### file list

```diff
@@ -1,23 +1,18 @@
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2022-03-04 15:16:00.932398 wikidata_dl-2022.3.4/
--rw-r--r--   0 rg        (1000) rg        (1000)     1072 2019-10-03 23:08:55.000000 wikidata_dl-2022.3.4/LICENSE
--rw-r--r--   0 rg        (1000) rg        (1000)      253 2019-10-03 23:53:09.000000 wikidata_dl-2022.3.4/MANIFEST.in
--rw-rw-r--   0 rg        (1000) rg        (1000)     2234 2022-03-04 15:16:00.932398 wikidata_dl-2022.3.4/PKG-INFO
--rw-r--r--   0 rg        (1000) rg        (1000)     1133 2019-11-20 22:23:55.000000 wikidata_dl-2022.3.4/README.md
--rw-r--r--   0 rg        (1000) rg        (1000)      162 2022-03-04 15:16:00.932398 wikidata_dl-2022.3.4/setup.cfg
--rw-r--r--   0 rg        (1000) rg        (1000)     1604 2019-10-05 22:47:39.000000 wikidata_dl-2022.3.4/setup.py
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2022-03-04 15:16:00.932398 wikidata_dl-2022.3.4/tests/
--rw-r--r--   0 rg        (1000) rg        (1000)       24 2019-10-04 16:03:30.000000 wikidata_dl-2022.3.4/tests/__init__.py
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2022-03-04 15:16:00.932398 wikidata_dl-2022.3.4/tests/queries/
--rw-r--r--   0 rg        (1000) rg        (1000)       54 2019-10-04 14:39:59.000000 wikidata_dl-2022.3.4/tests/queries/instance-of-inner-planet.sparql
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2022-03-04 15:16:00.932398 wikidata_dl-2022.3.4/wikidata_dl/
--rw-r--r--   0 rg        (1000) rg        (1000)      110 2022-03-04 15:13:43.000000 wikidata_dl-2022.3.4/wikidata_dl/__init__.py
--rw-r--r--   0 rg        (1000) rg        (1000)     1217 2022-03-04 11:29:01.000000 wikidata_dl-2022.3.4/wikidata_dl/cli.py
--rw-r--r--   0 rg        (1000) rg        (1000)     3627 2022-03-04 11:24:04.000000 wikidata_dl-2022.3.4/wikidata_dl/wikidata_dl.py
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2022-03-04 15:16:00.932398 wikidata_dl-2022.3.4/wikidata_dl.egg-info/
--rw-rw-r--   0 rg        (1000) rg        (1000)     2234 2022-03-04 15:16:00.000000 wikidata_dl-2022.3.4/wikidata_dl.egg-info/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)      428 2022-03-04 15:16:00.000000 wikidata_dl-2022.3.4/wikidata_dl.egg-info/SOURCES.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        1 2022-03-04 15:16:00.000000 wikidata_dl-2022.3.4/wikidata_dl.egg-info/dependency_links.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)       54 2022-03-04 15:16:00.000000 wikidata_dl-2022.3.4/wikidata_dl.egg-info/entry_points.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        1 2022-03-04 15:16:00.000000 wikidata_dl-2022.3.4/wikidata_dl.egg-info/not-zip-safe
--rw-rw-r--   0 rg        (1000) rg        (1000)       33 2022-03-04 15:16:00.000000 wikidata_dl-2022.3.4/wikidata_dl.egg-info/requires.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)       12 2022-03-04 15:16:00.000000 wikidata_dl-2022.3.4/wikidata_dl.egg-info/top_level.txt
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/.editorconfig
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/.flake8
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/Makefile
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/.vscode/settings.json
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/tests/test_wikidata.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/tests/queries/continents-on-earth.sparql
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/tests/queries/instance-of-inner-planet.sparql
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/tests/queries/nevada-events.sparql
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/wikidata_dl/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/wikidata_dl/__init__.py
+-rwxr-xr-x   0        0        0     2723 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/wikidata_dl/cli.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/wikidata_dl/vocabulary.py
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/wikidata_dl/wikidata.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/LICENSE
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/README.md
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/pyproject.toml
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 wikidata_dl-2023.7.27/PKG-INFO
```

### Comparing `wikidata_dl-2022.3.4/LICENSE` & `wikidata_dl-2023.7.27/LICENSE`

 * *Files identical despite different names*

### Comparing `wikidata_dl-2022.3.4/README.md` & `wikidata_dl-2023.7.27/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -2,35 +2,28 @@
 
 ## Description
 
 **wikidata-dl** is a command line program for downloading data from [Wikidata](https://www.wikidata.org/) based on [SPARQL](https://en.wikipedia.org/wiki/SPARQL) queries.
 
 ## Installation
 
-    pip install wikidata_dl
+    pip install wikidata-dl
 
 ## Usage
 
-Download all results returned by the query and store them in the `wikidata` directory in the current working directory:
+Download result returned from the query and save it in the directory `./wikidata`:
 
     wikidata-dl /path/to/my-query.sparql
 
-Show only the result count returned by the query without downloading anything:
-
-    wikidata-dl --dry-run /path/to/my-query.sparql
-
 For a complete reference of the command line options run:
 
     wikidata-dl --help
 
 ## Sample Query
 
 The following query returns IDs for all Wikidata entities that are an instance of ([P31](https://www.wikidata.org/wiki/Property:P31)) a continent ([Q5107](https://www.wikidata.org/wiki/Q5107)).
 
     SELECT ?item WHERE {
         ?item wdt:P31 wd:Q5107.
     }
 
-## Conventions
-
-* The SPARQL query you pass to the program must return [Wikibase](https://www.mediawiki.org/wiki/Wikibase/DataModel/Primer) IDs.
-* The query variable where the entity ID is stored must be called ``item``.
+[Try the query](https://query.wikidata.org/#SELECT%20%3Fitem%20WHERE%20%7B%20%3Fitem%20wdt%3AP31%20wd%3AQ5107.%20%7D)
```

