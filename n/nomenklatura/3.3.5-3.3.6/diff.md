# Comparing `tmp/nomenklatura-3.3.5.tar.gz` & `tmp/nomenklatura-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.3.5.tar", last modified: Wed Jul 26 15:57:27 2023, max compression
+gzip compressed data, was "nomenklatura-3.3.6.tar", last modified: Thu Jul 27 15:01:54 2023, max compression
```

## Comparing `nomenklatura-3.3.5.tar` & `nomenklatura-3.3.6.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.102639 nomenklatura-3.3.5/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.102639 nomenklatura-3.3.5/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.102639 nomenklatura-3.3.5/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/matching/heuristic/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/heuristic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/heuristic/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/matching/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.106639 nomenklatura-3.3.5/nomenklatura/matching/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/matching/v2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/statement/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/store/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:57:27.102639 nomenklatura-3.3.5/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:56:29.000000 nomenklatura-3.3.5/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 15:57:27.000000 nomenklatura-3.3.5/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:57:27.110639 nomenklatura-3.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-26 15:54:46.000000 nomenklatura-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.416193 nomenklatura-3.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-27 15:01:54.416193 nomenklatura-3.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.408193 nomenklatura-3.3.6/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.408193 nomenklatura-3.3.6/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.408193 nomenklatura-3.3.6/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.408193 nomenklatura-3.3.6/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.408193 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.412193 nomenklatura-3.3.6/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/statement/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.416193 nomenklatura-3.3.6/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/store/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.416193 nomenklatura-3.3.6/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:01:54.408193 nomenklatura-3.3.6/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:00:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 15:01:54.000000 nomenklatura-3.3.6/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 15:01:54.416193 nomenklatura-3.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-27 14:59:14.000000 nomenklatura-3.3.6/setup.py
```

### Comparing `nomenklatura-3.3.5/LICENSE` & `nomenklatura-3.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/PKG-INFO` & `nomenklatura-3.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.5
+Version: 3.3.6
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: leveldb
 License-File: LICENSE
 
 # nomenklatura
 
@@ -92,9 +91,7 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
-
-
```

### Comparing `nomenklatura-3.3.5/README.md` & `nomenklatura-3.3.6/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/cache.py` & `nomenklatura-3.3.6/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/cli.py` & `nomenklatura-3.3.6/nomenklatura/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,16 @@
 def apply(
     path: Path, outpath: Path, resolver: Optional[Path], dataset: Optional[str] = None
 ) -> None:
     resolver_ = _get_resolver(path, resolver)
     with path_writer(outpath) as outfh:
         for proxy in path_entities(path, StreamEntity):
             proxy = resolver_.apply_stream(proxy)
+            if dataset is not None:
+                proxy.datasets.add(dataset)
             write_entity(outfh, proxy)
 
 
 @cli.command("sorted-aggregate", help="Merge sort-order entities")
 @click.option("-i", "--infile", type=InPath, default="-")
 @click.option("-o", "--outfile", type=OutPath, default="-")
 def sorted_aggregate_(infile: Path, outfile: Path) -> None:
```

### Comparing `nomenklatura-3.3.5/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.3.6/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.3.6/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/dataset/catalog.py` & `nomenklatura-3.3.6/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/dataset/coverage.py` & `nomenklatura-3.3.6/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/dataset/dataset.py` & `nomenklatura-3.3.6/nomenklatura/dataset/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         self.resources: List[DataResource] = []
         for rdata in data.get("resources", []):
             if rdata is not None:
                 self.resources.append(DataResource(rdata))
 
         self._children = set(string_list(data.get("children", [])))
         self._children.update(string_list(data.get("datasets", [])))
+        self._children.update(string_list(data.get("scopes", [])))
 
     @cached_property
     def children(self: DS) -> Set[DS]:
         children: Set[DS] = set()
         for child_name in self._children:
             children.add(self.catalog.require(child_name))
         if self in children:
```

### Comparing `nomenklatura-3.3.5/nomenklatura/dataset/publisher.py` & `nomenklatura-3.3.6/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/dataset/resource.py` & `nomenklatura-3.3.6/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/dataset/util.py` & `nomenklatura-3.3.6/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/db.py` & `nomenklatura-3.3.6/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/enrich/__init__.py` & `nomenklatura-3.3.6/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/enrich/aleph.py` & `nomenklatura-3.3.6/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/enrich/common.py` & `nomenklatura-3.3.6/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.3.6/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.3.6/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.3.6/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.3.6/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.3.6/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.3.6/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.3.6/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.3.6/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/enrich/yente.py` & `nomenklatura-3.3.6/nomenklatura/enrich/yente.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/entity.py` & `nomenklatura-3.3.6/nomenklatura/entity.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/index/entry.py` & `nomenklatura-3.3.6/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/index/index.py` & `nomenklatura-3.3.6/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/index/tokenizer.py` & `nomenklatura-3.3.6/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/judgement.py` & `nomenklatura-3.3.6/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/__init__.py` & `nomenklatura-3.3.6/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/heuristic/__init__.py` & `nomenklatura-3.3.6/nomenklatura/matching/heuristic/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/heuristic/logic.py` & `nomenklatura-3.3.6/nomenklatura/matching/heuristic/logic.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/pairs.py` & `nomenklatura-3.3.6/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/types.py` & `nomenklatura-3.3.6/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/util.py` & `nomenklatura-3.3.6/nomenklatura/matching/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/v1/dates.py` & `nomenklatura-3.3.6/nomenklatura/matching/v1/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/v1/misc.py` & `nomenklatura-3.3.6/nomenklatura/matching/v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/v1/model.py` & `nomenklatura-3.3.6/nomenklatura/matching/v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/v1/names.py` & `nomenklatura-3.3.6/nomenklatura/matching/v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/v1/train.py` & `nomenklatura-3.3.6/nomenklatura/matching/v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/v1/util.py` & `nomenklatura-3.3.6/nomenklatura/matching/v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/v2/dates.py` & `nomenklatura-3.3.6/nomenklatura/matching/v2/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/v2/misc.py` & `nomenklatura-3.3.6/nomenklatura/matching/v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/v2/model.py` & `nomenklatura-3.3.6/nomenklatura/matching/v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/v2/names.py` & `nomenklatura-3.3.6/nomenklatura/matching/v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/v2/train.py` & `nomenklatura-3.3.6/nomenklatura/matching/v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/matching/v2/util.py` & `nomenklatura-3.3.6/nomenklatura/matching/v2/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/publish/dates.py` & `nomenklatura-3.3.6/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/publish/edges.py` & `nomenklatura-3.3.6/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/publish/names.py` & `nomenklatura-3.3.6/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/resolver/edge.py` & `nomenklatura-3.3.6/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/resolver/identifier.py` & `nomenklatura-3.3.6/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/resolver/resolver.py` & `nomenklatura-3.3.6/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/senzing.py` & `nomenklatura-3.3.6/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/statement/__init__.py` & `nomenklatura-3.3.6/nomenklatura/statement/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/statement/db.py` & `nomenklatura-3.3.6/nomenklatura/statement/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/statement/serialize.py` & `nomenklatura-3.3.6/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/statement/statement.py` & `nomenklatura-3.3.6/nomenklatura/statement/statement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/store/__init__.py` & `nomenklatura-3.3.6/nomenklatura/store/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/store/base.py` & `nomenklatura-3.3.6/nomenklatura/store/base.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/store/level.py` & `nomenklatura-3.3.6/nomenklatura/store/level.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/store/memory.py` & `nomenklatura-3.3.6/nomenklatura/store/memory.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/store/util.py` & `nomenklatura-3.3.6/nomenklatura/store/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/stream.py` & `nomenklatura-3.3.6/nomenklatura/stream.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/tui/app.py` & `nomenklatura-3.3.6/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/tui/comparison.py` & `nomenklatura-3.3.6/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/tui/util.py` & `nomenklatura-3.3.6/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/util.py` & `nomenklatura-3.3.6/nomenklatura/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura/xref.py` & `nomenklatura-3.3.6/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.3.6/nomenklatura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.5
+Version: 3.3.6
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: leveldb
 License-File: LICENSE
 
 # nomenklatura
 
@@ -92,9 +91,7 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
-
-
```

### Comparing `nomenklatura-3.3.5/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.3.6/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.5/setup.py` & `nomenklatura-3.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.3.5",
+    version="3.3.6",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

