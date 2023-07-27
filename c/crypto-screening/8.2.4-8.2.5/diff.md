# Comparing `tmp/crypto-screening-8.2.4.tar.gz` & `tmp/crypto-screening-8.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.2.4.tar", last modified: Wed Jul 26 10:57:23 2023, max compression
+gzip compressed data, was "crypto-screening-8.2.5.tar", last modified: Thu Jul 27 15:12:04 2023, max compression
```

## Comparing `crypto-screening-8.2.4.tar` & `crypto-screening-8.2.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.104889 crypto-screening-8.2.4/
--rw-rw-rw-   0        0        0      196 2023-07-26 10:57:21.000000 crypto-screening-8.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-26 10:57:23.103890 crypto-screening-8.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.2.4/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.2.4/build.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:22.933188 crypto-screening-8.2.4/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:22.965495 crypto-screening-8.2.4/crypto_screening/collect/
--rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.2.4/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     5005 2023-07-24 18:29:23.000000 crypto-screening-8.2.4/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:22.994465 crypto-screening-8.2.4/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.2.4/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.2.4/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.016529 crypto-screening-8.2.4/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.2.4/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24665 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16516 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21653 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    18731 2023-07-26 10:53:46.000000 crypto-screening-8.2.4/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19569 2023-07-24 18:21:12.000000 crypto-screening-8.2.4/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.2.4/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.2.4/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.2.4/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.056038 crypto-screening-8.2.4/crypto_screening/screeners/
--rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.2.4/crypto_screening/screeners/__init__.py
--rw-rw-rw-   0        0        0    23312 2023-07-24 09:37:18.000000 crypto-screening-8.2.4/crypto_screening/screeners/base.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.067038 crypto-screening-8.2.4/crypto_screening/screeners/callbacks/
--rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.2.4/crypto_screening/screeners/callbacks/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.2.4/crypto_screening/screeners/callbacks/base.py
--rw-rw-rw-   0        0        0     4400 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/screeners/callbacks/database.py
--rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/screeners/callbacks/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.078038 crypto-screening-8.2.4/crypto_screening/screeners/collectors/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.2.4/crypto_screening/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6271 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.2.4/crypto_screening/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.2.4/crypto_screening/screeners/combined.py
--rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.2.4/crypto_screening/screeners/container.py
--rw-rw-rw-   0        0        0    10976 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/screeners/database.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.086038 crypto-screening-8.2.4/crypto_screening/screeners/foundation/
--rw-rw-rw-   0        0        0    10462 2023-07-24 09:37:33.000000 crypto-screening-8.2.4/crypto_screening/screeners/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.2.4/crypto_screening/screeners/foundation/protocols.py
--rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.2.4/crypto_screening/screeners/foundation/state.py
--rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.2.4/crypto_screening/screeners/foundation/waiting.py
--rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/screeners/market.py
--rw-rw-rw-   0        0        0    22099 2023-07-24 09:38:59.000000 crypto-screening-8.2.4/crypto_screening/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11814 2023-07-24 09:39:14.000000 crypto-screening-8.2.4/crypto_screening/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11410 2023-07-24 09:39:34.000000 crypto-screening-8.2.4/crypto_screening/screeners/orders.py
--rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.2.4/crypto_screening/screeners/recorder.py
--rw-rw-rw-   0        0        0    11479 2023-07-24 09:39:59.000000 crypto-screening-8.2.4/crypto_screening/screeners/trades.py
--rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.2.4/crypto_screening/screeners/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:22.898298 crypto-screening-8.2.4/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.091069 crypto-screening-8.2.4/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.2.4/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10353 2023-07-25 10:48:04.000000 crypto-screening-8.2.4/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.102888 crypto-screening-8.2.4/crypto_screening/utils/
--rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.2.4/crypto_screening/utils/base.py
--rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.2.4/crypto_screening/utils/process.py
--rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.2.4/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:22.947189 crypto-screening-8.2.4/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-26 10:57:22.000000 crypto-screening-8.2.4/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2023-07-26 10:57:22.000000 crypto-screening-8.2.4/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 10:57:22.000000 crypto-screening-8.2.4/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-26 10:57:22.000000 crypto-screening-8.2.4/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 10:57:22.000000 crypto-screening-8.2.4/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-26 10:57:21.000000 crypto-screening-8.2.4/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.2.4/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.2.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 10:57:23.104889 crypto-screening-8.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-26 10:57:18.000000 crypto-screening-8.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.501993 crypto-screening-8.2.5/
+-rw-rw-rw-   0        0        0      196 2023-07-27 15:12:04.000000 crypto-screening-8.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-27 15:12:04.501993 crypto-screening-8.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.2.5/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.2.5/build.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.462483 crypto-screening-8.2.5/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.475486 crypto-screening-8.2.5/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.2.5/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4940 2023-07-27 15:04:17.000000 crypto-screening-8.2.5/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.479482 crypto-screening-8.2.5/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.2.5/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.2.5/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.2.5/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.2.5/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.482482 crypto-screening-8.2.5/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.2.5/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24665 2023-07-24 09:29:05.000000 crypto-screening-8.2.5/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16516 2023-07-24 09:29:05.000000 crypto-screening-8.2.5/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21653 2023-07-24 09:29:05.000000 crypto-screening-8.2.5/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.2.5/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    20755 2023-07-27 15:10:03.000000 crypto-screening-8.2.5/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19564 2023-07-27 15:04:24.000000 crypto-screening-8.2.5/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.2.5/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.2.5/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.2.5/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.491486 crypto-screening-8.2.5/crypto_screening/screeners/
+-rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.2.5/crypto_screening/screeners/__init__.py
+-rw-rw-rw-   0        0        0    23843 2023-07-27 14:49:56.000000 crypto-screening-8.2.5/crypto_screening/screeners/base.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.493486 crypto-screening-8.2.5/crypto_screening/screeners/callbacks/
+-rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.2.5/crypto_screening/screeners/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.2.5/crypto_screening/screeners/callbacks/base.py
+-rw-rw-rw-   0        0        0     4400 2023-07-24 09:29:05.000000 crypto-screening-8.2.5/crypto_screening/screeners/callbacks/database.py
+-rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.2.5/crypto_screening/screeners/callbacks/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.496486 crypto-screening-8.2.5/crypto_screening/screeners/collectors/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.2.5/crypto_screening/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6271 2023-07-24 09:29:05.000000 crypto-screening-8.2.5/crypto_screening/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.2.5/crypto_screening/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.2.5/crypto_screening/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.2.5/crypto_screening/screeners/combined.py
+-rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.2.5/crypto_screening/screeners/container.py
+-rw-rw-rw-   0        0        0    10976 2023-07-24 09:29:05.000000 crypto-screening-8.2.5/crypto_screening/screeners/database.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.498989 crypto-screening-8.2.5/crypto_screening/screeners/foundation/
+-rw-rw-rw-   0        0        0    10678 2023-07-27 14:21:39.000000 crypto-screening-8.2.5/crypto_screening/screeners/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.2.5/crypto_screening/screeners/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.2.5/crypto_screening/screeners/foundation/state.py
+-rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.2.5/crypto_screening/screeners/foundation/waiting.py
+-rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.2.5/crypto_screening/screeners/market.py
+-rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.2.5/crypto_screening/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.2.5/crypto_screening/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.2.5/crypto_screening/screeners/orders.py
+-rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.2.5/crypto_screening/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.2.5/crypto_screening/screeners/trades.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.2.5/crypto_screening/screeners/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.453507 crypto-screening-8.2.5/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.498989 crypto-screening-8.2.5/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.2.5/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10353 2023-07-25 10:48:04.000000 crypto-screening-8.2.5/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.500993 crypto-screening-8.2.5/crypto_screening/utils/
+-rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.2.5/crypto_screening/utils/base.py
+-rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.2.5/crypto_screening/utils/process.py
+-rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.2.5/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:12:04.472483 crypto-screening-8.2.5/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-27 15:12:04.000000 crypto-screening-8.2.5/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-07-27 15:12:04.000000 crypto-screening-8.2.5/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 15:12:04.000000 crypto-screening-8.2.5/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-27 15:12:04.000000 crypto-screening-8.2.5/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-27 15:12:04.000000 crypto-screening-8.2.5/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-27 15:12:04.000000 crypto-screening-8.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.2.5/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.2.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 15:12:04.501993 crypto-screening-8.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-27 15:11:25.000000 crypto-screening-8.2.5/setup.py
```

### Comparing `crypto-screening-8.2.4/PKG-INFO` & `crypto-screening-8.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.2.4
+Version: 8.2.5
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.2.4/README.md` & `crypto-screening-8.2.5/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/build.py` & `crypto-screening-8.2.5/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/collect/assets.py` & `crypto-screening-8.2.5/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/collect/exchanges.py` & `crypto-screening-8.2.5/crypto_screening/collect/exchanges.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,30 +14,19 @@
 )
 
 __all__ = [
     "exchanges_data",
     "exchanges_values"
 ]
 
-_R = TypeVar("_R")
-
-Collector = Callable[
-    [
-        str,
-        Optional[str],
-        Optional[bool],
-        Optional[Iterable[str]],
-        Optional[Iterable[str]],
-        Optional[Iterable[str]]
-    ], _R
-]
+ExchangesData = Union[Dict[str, Iterable[str]], Iterable[str]]
 
 def exchanges_values(
         exchanges: Iterable[str],
-        values: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+        values: Optional[ExchangesData] = None
 ) -> Dict[str, Iterable[str]]:
     """
     Collects the values to the structure of the exchanges.
 
     :param exchanges: The exchanges for the structure.
     :param values: The values to process.
 
@@ -80,23 +69,37 @@
 
     return (
         (values[exchange] if exchange in values else default)
         if isinstance(values, dict) else values
     )
 # end exchange_value
 
+_R = TypeVar("_R")
+
+Collector = Callable[
+    [
+        str,
+        Optional[str],
+        Optional[bool],
+        Optional[Iterable[str]],
+        Optional[Iterable[str]],
+        Optional[Iterable[str]],
+        Optional[Iterable[str]]
+    ], _R
+]
+
 def exchanges_data(
         collector: Collector,
         adjust: Optional[bool] = True,
         separator: Optional[str] = None,
         exchanges: Optional[Iterable[str]] = None,
-        bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
-        excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+        bases: Optional[ExchangesData] = None,
+        quotes: Optional[ExchangesData] = None,
+        included: Optional[ExchangesData] = None,
+        excluded: Optional[ExchangesData] = None
 ) -> Dict[str, _R]:
     """
     Collects the symbols from the exchanges.
 
     :param collector: The collector function to collect data from an exchange.
     :param exchanges: The exchanges.
     :param bases: The bases of the asset pairs.
```

### Comparing `crypto-screening-8.2.4/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.2.5/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.2.5/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/collect/market/orders.py` & `crypto-screening-8.2.5/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.2.5/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.2.5/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.2.5/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/collect/market/trades.py` & `crypto-screening-8.2.5/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/collect/screeners.py` & `crypto-screening-8.2.5/crypto_screening/collect/screeners.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # screeners.py
 
 from typing import (
-    Optional, Dict, Iterable,
-    Set, Union, Tuple, List
+    Optional, Dict, Iterable, TypeVar,
+    Set, Union, Tuple, Type, List
 )
 
 import pandas as pd
 from attrs import define
 
-from crypto_screening.symbols import symbol_to_pair, symbol_to_parts, adjust_symbol
+from crypto_screening.symbols import (
+    symbol_to_pair, symbol_to_parts, adjust_symbol
+)
 from crypto_screening.utils.process import string_in_values
 from crypto_screening.collect.symbols import (
     matching_symbol_pair, MarketSymbolSignature, exchanges_symbols
 )
-from crypto_screening.screeners import BaseScreener, BaseMarketScreener
+from crypto_screening.screeners import (
+    BaseScreener, BaseMarketScreener, OHLCVScreener
+)
 
 __all__ = [
     "matching_screener_signatures",
     "matching_screener_pair",
     "matching_screener_pairs",
     "MarketScreenerSignature",
     "find_screeners",
@@ -32,15 +36,16 @@
     "screeners_to_multiple_symbols_screeners",
     "screeners_to_assets_screeners",
     "screeners_to_symbols_screeners",
     "screeners_to_multiple_assets_screeners",
     "screeners_to_multiple_assets_datasets",
     "screeners_to_multiple_symbols_datasets",
     "nonempty_screeners",
-    "running_screeners"
+    "running_screeners",
+    "find_screener"
 ]
 
 AssetMatches = Iterable[Iterable[str]]
 
 def matching_screener_pair(
         screener1: BaseScreener,
         screener2: BaseScreener, /, *,
@@ -82,15 +87,15 @@
     :param matches: The currencies.
     :param separator: The separator of the assets.
     :param empty: Allows empty screeners.
 
     :return: The validation value for the symbols.
     """
 
-    pairs: List[Tuple[BaseScreener, BaseScreener]] = []
+    pairs: Set[Tuple[BaseScreener, BaseScreener]] = set()
 
     if not empty:
         screeners = remove_empty_screeners(screeners=screeners)
     # end if
 
     for screener1 in screeners:
         for screener2 in screeners:
@@ -104,15 +109,15 @@
             )
 
             if matching_screener_pair(
                 screener1, screener2,
                 matches=exchanges_matches or None,
                 separator=separator
             ):
-                pairs.append((screener1, screener2))
+                pairs.add((screener1, screener2))
             # end if
         # end for
     # end for
 
     return set(pairs)
 # end matching_screener_pairs
 
@@ -148,26 +153,26 @@
             f"when 'data' is superior to 'screeners'."
         )
 
     elif (not screeners) and (not data):
         return set()
     # end if
 
-    pairs: List[Tuple[MarketScreenerSignature, MarketScreenerSignature]] = []
+    pairs: Set[Tuple[MarketScreenerSignature, MarketScreenerSignature]] = set()
 
     data = data or matching_screener_pairs(
         screeners=screeners, matches=matches,
         separator=separator, empty=empty
     )
 
     for screener1, screener2 in data:
         asset1, currency1 = symbol_to_parts(adjust_symbol(screener1.symbol))
         asset2, currency2 = symbol_to_pair(adjust_symbol(screener2.symbol))
 
-        pairs.append(
+        pairs.add(
             (
                 MarketScreenerSignature(
                     asset=asset1, currency=currency1,
                     exchange=screener1.exchange,
                     screener=screener1
                 ),
                 MarketScreenerSignature(
@@ -281,36 +286,97 @@
             setdefault(screener.symbol, set())
         ).add(screener)
     # end for
 
     return structure
 # end structure_screeners
 
+_S = TypeVar("_S")
+
 def find_screeners(
-        screeners: Iterable[BaseScreener],
+        screeners: Iterable[_S],
+        base: Optional[Type[_S]] = None,
         exchange: Optional[str] = None,
-        symbol: Optional[str] = None
-) -> Set[BaseScreener]:
+        symbol: Optional[str] = None,
+        interval: Optional[str] = None
+) -> List[_S]:
     """
     Finds all the screeners with the matching exchange and symbol key.
 
     :param screeners: The screeners to process.
+    :param base: The base type for the screeners.
     :param exchange: The exchange key for the symbol.
     :param symbol: The pair symbol to search its screeners.
+    :param interval: The interval of the screener.
 
     :return: The matching screeners.
     """
 
-    return {
+    return [
         screener for screener in screeners
         if (
+            ((base is None) or (isinstance(screener, base))) and
             ((symbol is None) or (screener.symbol.lower() == symbol.lower())) and
-            ((exchange is None) or (exchange.lower() == screener.exchange.lower()))
+            ((exchange is None) or (exchange.lower() == screener.exchange.lower())) and
+            (
+                (interval is None) or
+                (
+                    isinstance(screener, OHLCVScreener) and
+                    (screener.interval.lower() == interval.lower())
+                )
+            )
         )
-    }
+    ]
+# end find_screeners
+
+def find_screener(
+        screeners: Iterable[_S],
+        base: Optional[Type[_S]] = None,
+        exchange: Optional[str] = None,
+        symbol: Optional[str] = None,
+        interval: Optional[str] = None,
+        index: Optional[int] = None
+) -> _S:
+    """
+    Finds all the screeners with the matching exchange and symbol key.
+
+    :param screeners: The screeners to process.
+    :param base: The base type for the screeners.
+    :param exchange: The exchange key for the symbol.
+    :param symbol: The pair symbol to search its screeners.
+    :param interval: The interval of the screener.
+    :param index: The index for the screener.
+
+    :return: The matching screeners.
+    """
+
+    found_screeners = find_screeners(
+        screeners=screeners, base=base, exchange=exchange,
+        symbol=symbol, interval=interval
+    )
+
+    if not found_screeners:
+        raise ValueError(
+            f"Cannot find screeners  matching to "
+            f"type - {base}, exchange - {exchange}, "
+            f"symbol - {symbol}, interval - {interval}."
+        )
+    # end if
+
+    try:
+        return found_screeners[index or 0]
+
+    except IndexError:
+        raise IndexError(
+            f"Cannot find screeners matching to "
+            f"type - {base}, exchange - {exchange}, "
+            f"symbol - {symbol}, interval - {interval}, "
+            f"index - {index}."
+        )
+    # end try
 # end find_screeners
 
 def remove_empty_screeners(screeners: Iterable[BaseScreener]) -> Set[BaseScreener]:
     """
     Removes the empty screeners.
 
     :param screeners: The screeners of the assets and exchanges.
@@ -468,31 +534,31 @@
             )
         )
     }
 # end exchanges_symbols_screeners
 
 def screeners_to_multiple_symbols_screeners(
         screeners: Iterable[BaseScreener]
-) -> Dict[str, Dict[str, List[BaseScreener]]]:
+) -> Dict[str, Dict[str, Set[BaseScreener]]]:
     """
     Converts the datasets structure to the structure of the data rows.
 
     :param screeners: The screeners to process.
 
     :return: The new data.
     """
 
-    results: Dict[str, Dict[str, List[BaseScreener]]] = {}
+    results: Dict[str, Dict[str, Set[BaseScreener]]] = {}
 
     for screener in screeners:
         (
             results.
             setdefault(screener.exchange, {}).
-            setdefault(screener.symbol, []).
-            append(screener)
+            setdefault(screener.symbol, set()).
+            add(screener)
         )
     # end for
 
     return results
 # end symbols_datasets_to_symbols_data
 
 def screeners_to_symbols_screeners(
@@ -518,34 +584,34 @@
 
     return results
 # end symbols_datasets_to_symbols_data
 
 def screeners_to_multiple_assets_screeners(
         screeners: Iterable[BaseScreener],
         separator: Optional[str] = None
-) -> Dict[str, Dict[str, Dict[str, List[BaseScreener]]]]:
+) -> Dict[str, Dict[str, Dict[str, Set[BaseScreener]]]]:
     """
     Converts the datasets structure to the structure of the data rows.
 
     :param screeners: The screeners to process.
     :param separator: The separator for the symbols.
 
     :return: The new data.
     """
 
-    results: Dict[str, Dict[str, Dict[str, List[BaseScreener]]]] = {}
+    results: Dict[str, Dict[str, Dict[str, Set[BaseScreener]]]] = {}
 
     for screener in screeners:
         base, quote = symbol_to_parts(screener.symbol, separator=separator)
         (
             results.
             setdefault(screener.exchange, {}).
             setdefault(base, {}).
-            setdefault(quote, []).
-            append(screener)
+            setdefault(quote, set()).
+            add(screener)
         )
     # end for
 
     return results
 # end screeners_to_multiple_assets_screeners
 
 def screeners_to_assets_screeners(
@@ -574,58 +640,58 @@
     # end for
 
     return results
 # end screeners_to_multiple_assets_screeners
 
 def screeners_to_multiple_symbols_datasets(
         screeners: Iterable[BaseScreener]
-) -> Dict[str, Dict[str, List[pd.DataFrame]]]:
+) -> Dict[str, Dict[str, Set[pd.DataFrame]]]:
     """
     Converts the datasets structure to the structure of the data rows.
 
     :param screeners: The screeners to process.
 
     :return: The new data.
     """
 
-    results: Dict[str, Dict[str, List[pd.DataFrame]]] = {}
+    results: Dict[str, Dict[str, Set[pd.DataFrame]]] = {}
 
     for screener in screeners:
         (
             results.
             setdefault(screener.exchange, {}).
-            setdefault(screener.symbol, []).
-            append(screener.market)
+            setdefault(screener.symbol, set()).
+            add(screener.market)
         )
     # end for
 
     return results
 # end screeners_to_multiple_symbols_datasets
 
 def screeners_to_multiple_assets_datasets(
         screeners: Iterable[BaseScreener],
         separator: Optional[str] = None
-) -> Dict[str, Dict[str, Dict[str, List[pd.DataFrame]]]]:
+) -> Dict[str, Dict[str, Dict[str, Set[pd.DataFrame]]]]:
     """
     Converts the datasets structure to the structure of the data rows.
 
     :param screeners: The screeners to process.
     :param separator: The separator for the symbols.
 
     :return: The new data.
     """
 
-    results: Dict[str, Dict[str, Dict[str, List[pd.DataFrame]]]] = {}
+    results: Dict[str, Dict[str, Dict[str, Set[pd.DataFrame]]]] = {}
 
     for screener in screeners:
         base, quote = symbol_to_parts(screener.symbol, separator=separator)
         (
             results.
             setdefault(screener.exchange, {}).
             setdefault(base, {}).
-            setdefault(quote, []).
-            append(screener.market)
+            setdefault(quote, set()).
+            add(screener.market)
         )
     # end for
 
     return results
 # end screeners_to_multiple_assets_datasets
```

### Comparing `crypto-screening-8.2.4/crypto_screening/collect/symbols.py` & `crypto-screening-8.2.5/crypto_screening/collect/symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # symbols.py
 
 import warnings
 from typing import (
-    Optional, Dict, Iterable,
-    Set, Union, Tuple
+    Optional, Dict, Iterable, Set, Union, Tuple
 )
 
 from attrs import define
 
 from represent import represent
 
 from multithreading import Caller, multi_threaded_call
```

### Comparing `crypto-screening-8.2.4/crypto_screening/dataset.py` & `crypto-screening-8.2.5/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/exchanges.py` & `crypto-screening-8.2.5/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/interval.py` & `crypto-screening-8.2.5/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/base.py` & `crypto-screening-8.2.5/crypto_screening/screeners/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
 
     NAME: Optional[str] = "BASE"
     COLUMNS: Iterable[str] = []
 
     SCREENER_NAME_TYPE_MATCHES: Dict[str, Any] = {}
     SCREENER_TYPE_NAME_MATCHES: Dict[Any, str] = {}
 
+    __slots__ = "symbol", "exchange", "market"
+
     def __init__(
             self,
             symbol: str,
             exchange: str,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None,
@@ -558,14 +560,36 @@
     >>> from crypto_screening.screeners import BaseScreenersContainer, BaseScreener
     >>>
     >>> container = BaseScreenersContainer(
     >>>     screeners=[BaseScreener(exchange="binance", symbol="BTC/USDT")]
     >>> )
     """
 
+    @property
+    def screeners(self) -> List[BaseScreener]:
+        """
+        Returns a list of all the screeners.
+
+        :return: The screeners.
+        """
+
+        return self._screeners
+    # end screeners
+
+    @screeners.setter
+    def screeners(self, value: List[BaseScreener]) -> None:
+        """
+        Returns a list of all the screeners.
+
+        :param value: The screeners.
+        """
+
+        self._screeners = value
+    # end screeners
+
     def update_screeners(self) -> None:
         """Updates the records of the object."""
     # end update_screeners
 
     def add(
             self,
             screeners: Iterable[BaseScreener],
```

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/callbacks/base.py` & `crypto-screening-8.2.5/crypto_screening/screeners/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/callbacks/database.py` & `crypto-screening-8.2.5/crypto_screening/screeners/callbacks/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/callbacks/sockets.py` & `crypto-screening-8.2.5/crypto_screening/screeners/callbacks/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/collectors/base.py` & `crypto-screening-8.2.5/crypto_screening/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/collectors/database.py` & `crypto-screening-8.2.5/crypto_screening/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/collectors/sockets.py` & `crypto-screening-8.2.5/crypto_screening/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/combined.py` & `crypto-screening-8.2.5/crypto_screening/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/container.py` & `crypto-screening-8.2.5/crypto_screening/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/database.py` & `crypto-screening-8.2.5/crypto_screening/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/foundation/data.py` & `crypto-screening-8.2.5/crypto_screening/screeners/foundation/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,20 @@
     """A class to represent an abstract parent class of data collectors."""
 
     LOCATION = "datasets"
 
     DELAY = 0
     CANCEL = 0
 
+    __slots__ = (
+        "location", "delay", "cancel", "_screening",
+        "_blocking", "_saving", "_updating", "_screening_process",
+        "_timeout_process", "_saving_process", "_update_process"
+    )
+
     def __init__(
             self,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
             delay: Optional[Union[float, dt.timedelta]] = None
     ) -> None:
         """
```

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/foundation/protocols.py` & `crypto-screening-8.2.5/crypto_screening/screeners/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/foundation/state.py` & `crypto-screening-8.2.5/crypto_screening/screeners/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/foundation/waiting.py` & `crypto-screening-8.2.5/crypto_screening/screeners/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/market.py` & `crypto-screening-8.2.5/crypto_screening/screeners/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/ohlcv.py` & `crypto-screening-8.2.5/crypto_screening/screeners/ohlcv.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,16 @@
     """
 
     INTERVAL = "1m"
     NAME = "OHLCV"
 
     COLUMNS = OHLCV_COLUMNS
 
+    __slots__ = "interval", "orderbook_market"
+
     def __init__(
             self,
             symbol: str,
             exchange: str,
             interval: Optional[str] = None,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
```

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/orderbook.py` & `crypto-screening-8.2.5/crypto_screening/screeners/orderbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,16 @@
         The dataset of the market data as BID/ASK spread.
     """
 
     NAME = "ORDERBOOK"
 
     COLUMNS = ORDERBOOK_COLUMNS
 
+    __slots__ = ()
+
     @property
     def orderbook_market(self) -> pd.DataFrame:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
```

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/orders.py` & `crypto-screening-8.2.5/crypto_screening/screeners/orders.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,16 @@
         The dataset of the market data as orders.
     """
 
     NAME = "ORDERS"
 
     COLUMNS = ORDERS_COLUMNS
 
+    __slots__ = ()
+
     @property
     def orders_market(self) -> pd.DataFrame:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
```

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/recorder.py` & `crypto-screening-8.2.5/crypto_screening/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/trades.py` & `crypto-screening-8.2.5/crypto_screening/screeners/trades.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         The dataset of the market data as trades.
     """
 
     NAME = "TRADES"
 
     COLUMNS = TRADES_COLUMNS
 
+    __slots__ = ()
+
     @property
     def trades_market(self) -> pd.DataFrame:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
         """
```

### Comparing `crypto-screening-8.2.4/crypto_screening/screeners/waiting.py` & `crypto-screening-8.2.5/crypto_screening/screeners/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.2.5/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/symbols.py` & `crypto-screening-8.2.5/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/utils/base.py` & `crypto-screening-8.2.5/crypto_screening/utils/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/utils/process.py` & `crypto-screening-8.2.5/crypto_screening/utils/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening/validate.py` & `crypto-screening-8.2.5/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.2.5/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.2.4
+Version: 8.2.5
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.2.4/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.2.5/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.4/pyproject.toml` & `crypto-screening-8.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.2.4'
+version = '8.2.5'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.2.4/setup.py` & `crypto-screening-8.2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='8.2.4',
+        version='8.2.5',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

