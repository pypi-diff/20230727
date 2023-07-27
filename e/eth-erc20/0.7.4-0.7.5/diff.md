# Comparing `tmp/eth-erc20-0.7.4.tar.gz` & `tmp/eth-erc20-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-erc20-0.7.4.tar", last modified: Tue May 30 16:38:31 2023, max compression
+gzip compressed data, was "eth-erc20-0.7.5.tar", last modified: Thu Jul 27 06:35:48 2023, max compression
```

## Comparing `eth-erc20-0.7.4.tar` & `eth-erc20-0.7.5.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/
--rw-r--r--   0 lash      (1000) lash      (1000)     1642 2023-05-30 16:38:03.000000 eth-erc20-0.7.4/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 08:00:05.000000 eth-erc20-0.7.4/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      153 2023-02-14 06:40:00.000000 eth-erc20-0.7.4/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      786 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 08:00:13.000000 eth-erc20-0.7.4/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 08:03:07.000000 eth-erc20-0.7.4/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/eth_erc20/
--rw-r--r--   0 lash      (1000) lash      (1000)       25 2021-05-02 11:58:48.000000 eth-erc20-0.7.4/eth_erc20/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/eth_erc20/data/
--rw-r--r--   0 lash      (1000) lash      (1000)     2605 2021-05-02 12:53:06.000000 eth-erc20-0.7.4/eth_erc20/data/ERC20.json
--rw-r--r--   0 lash      (1000) lash      (1000)     8888 2022-11-23 16:04:50.000000 eth-erc20-0.7.4/eth_erc20/erc20.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/eth_erc20/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     3703 2023-02-19 16:09:00.000000 eth-erc20-0.7.4/eth_erc20/runnable/balance.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3804 2023-02-13 06:39:32.000000 eth-erc20-0.7.4/eth_erc20/runnable/info.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3700 2022-11-06 10:30:18.000000 eth-erc20-0.7.4/eth_erc20/runnable/transfer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/eth_erc20/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-23 08:04:29.000000 eth-erc20-0.7.4/eth_erc20/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6489 2023-02-23 08:03:36.000000 eth-erc20-0.7.4/eth_erc20/unittest/base.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/eth_erc20.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      786 2023-05-30 16:38:31.000000 eth-erc20-0.7.4/eth_erc20.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1125 2023-05-30 16:38:31.000000 eth-erc20-0.7.4/eth_erc20.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-05-30 16:38:31.000000 eth-erc20-0.7.4/eth_erc20.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      288 2023-05-30 16:38:31.000000 eth-erc20-0.7.4/eth_erc20.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       69 2023-05-30 16:38:31.000000 eth-erc20-0.7.4/eth_erc20.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-05-30 16:38:31.000000 eth-erc20-0.7.4/eth_erc20.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/giftable_erc20_token/
--rw-r--r--   0 lash      (1000) lash      (1000)      119 2023-02-14 06:40:00.000000 eth-erc20-0.7.4/giftable_erc20_token/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/giftable_erc20_token/data/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-05-08 04:03:57.000000 eth-erc20-0.7.4/giftable_erc20_token/data/.chainlib
--rw-r--r--   0 lash      (1000) lash      (1000)    18930 2023-03-26 07:09:01.000000 eth-erc20-0.7.4/giftable_erc20_token/data/GiftableToken.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     6791 2023-03-26 07:09:01.000000 eth-erc20-0.7.4/giftable_erc20_token/data/GiftableToken.json
--rw-r--r--   0 lash      (1000) lash      (1000)       66 2021-02-24 16:44:15.000000 eth-erc20-0.7.4/giftable_erc20_token/data/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5307 2023-05-30 16:30:35.000000 eth-erc20-0.7.4/giftable_erc20_token/factory.py
--rw-r--r--   0 lash      (1000) lash      (1000)      108 2023-02-13 12:12:59.000000 eth-erc20-0.7.4/giftable_erc20_token/gen.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/giftable_erc20_token/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     2803 2023-01-24 15:09:24.000000 eth-erc20-0.7.4/giftable_erc20_token/runnable/gift.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3431 2023-01-24 15:53:09.000000 eth-erc20-0.7.4/giftable_erc20_token/runnable/minter.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3255 2023-02-21 18:21:49.000000 eth-erc20-0.7.4/giftable_erc20_token/runnable/publish.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/giftable_erc20_token/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-21 17:44:31.000000 eth-erc20-0.7.4/giftable_erc20_token/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1677 2023-05-05 07:48:30.000000 eth-erc20-0.7.4/giftable_erc20_token/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)       69 2023-03-22 10:40:04.000000 eth-erc20-0.7.4/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1465 2023-05-30 16:38:31.866638 eth-erc20-0.7.4/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      666 2021-04-04 12:48:14.000000 eth-erc20-0.7.4/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/static_token/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/static_token/data/
--rw-r--r--   0 lash      (1000) lash      (1000)    11366 2023-03-02 11:29:39.000000 eth-erc20-0.7.4/static_token/data/StaticToken.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     3288 2023-03-02 11:29:39.000000 eth-erc20-0.7.4/static_token/data/StaticToken.json
--rw-r--r--   0 lash      (1000) lash      (1000)       66 2022-04-22 18:28:18.000000 eth-erc20-0.7.4/static_token/data/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)       51 2021-05-02 12:00:59.000000 eth-erc20-0.7.4/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      266 2023-02-23 08:04:58.000000 eth-erc20-0.7.4/tests/test_erc20_interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4318 2023-02-22 10:16:13.000000 eth-erc20-0.7.4/tests/test_giftable.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.949988 eth-erc20-0.7.5/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1705 2023-07-27 06:34:01.000000 eth-erc20-0.7.5/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 08:00:05.000000 eth-erc20-0.7.5/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      153 2023-02-14 06:40:00.000000 eth-erc20-0.7.5/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      786 2023-07-27 06:35:48.949988 eth-erc20-0.7.5/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 08:00:13.000000 eth-erc20-0.7.5/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 08:03:07.000000 eth-erc20-0.7.5/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.943322 eth-erc20-0.7.5/eth_erc20/
+-rw-r--r--   0 lash      (1000) lash      (1000)       25 2021-05-02 11:58:48.000000 eth-erc20-0.7.5/eth_erc20/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.943322 eth-erc20-0.7.5/eth_erc20/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2605 2021-05-02 12:53:06.000000 eth-erc20-0.7.5/eth_erc20/data/ERC20.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     8888 2022-11-23 16:04:50.000000 eth-erc20-0.7.5/eth_erc20/erc20.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.946655 eth-erc20-0.7.5/eth_erc20/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3703 2023-02-19 16:09:00.000000 eth-erc20-0.7.5/eth_erc20/runnable/balance.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3804 2023-02-13 06:39:32.000000 eth-erc20-0.7.5/eth_erc20/runnable/info.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3700 2022-11-06 10:30:18.000000 eth-erc20-0.7.5/eth_erc20/runnable/transfer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.946655 eth-erc20-0.7.5/eth_erc20/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-23 08:04:29.000000 eth-erc20-0.7.5/eth_erc20/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6429 2023-06-29 19:53:13.000000 eth-erc20-0.7.5/eth_erc20/unittest/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.943322 eth-erc20-0.7.5/eth_erc20.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      786 2023-07-27 06:35:48.000000 eth-erc20-0.7.5/eth_erc20.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1146 2023-07-27 06:35:48.000000 eth-erc20-0.7.5/eth_erc20.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-07-27 06:35:48.000000 eth-erc20-0.7.5/eth_erc20.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      288 2023-07-27 06:35:48.000000 eth-erc20-0.7.5/eth_erc20.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       69 2023-07-27 06:35:48.000000 eth-erc20-0.7.5/eth_erc20.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-07-27 06:35:48.000000 eth-erc20-0.7.5/eth_erc20.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.946655 eth-erc20-0.7.5/giftable_erc20_token/
+-rw-r--r--   0 lash      (1000) lash      (1000)      119 2023-02-14 06:40:00.000000 eth-erc20-0.7.5/giftable_erc20_token/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.946655 eth-erc20-0.7.5/giftable_erc20_token/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-05-08 04:03:57.000000 eth-erc20-0.7.5/giftable_erc20_token/data/.chainlib
+-rw-r--r--   0 lash      (1000) lash      (1000)    18930 2023-03-26 07:09:01.000000 eth-erc20-0.7.5/giftable_erc20_token/data/GiftableToken.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     6791 2023-03-26 07:09:01.000000 eth-erc20-0.7.5/giftable_erc20_token/data/GiftableToken.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       66 2021-02-24 16:44:15.000000 eth-erc20-0.7.5/giftable_erc20_token/data/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5307 2023-05-30 16:30:35.000000 eth-erc20-0.7.5/giftable_erc20_token/factory.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      108 2023-02-13 12:12:59.000000 eth-erc20-0.7.5/giftable_erc20_token/gen.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.946655 eth-erc20-0.7.5/giftable_erc20_token/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2803 2023-01-24 15:09:24.000000 eth-erc20-0.7.5/giftable_erc20_token/runnable/gift.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3431 2023-01-24 15:53:09.000000 eth-erc20-0.7.5/giftable_erc20_token/runnable/minter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3255 2023-02-21 18:21:49.000000 eth-erc20-0.7.5/giftable_erc20_token/runnable/publish.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.949988 eth-erc20-0.7.5/giftable_erc20_token/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-21 17:44:31.000000 eth-erc20-0.7.5/giftable_erc20_token/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2056 2023-07-26 08:51:01.000000 eth-erc20-0.7.5/giftable_erc20_token/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       69 2023-03-22 10:40:04.000000 eth-erc20-0.7.5/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1465 2023-07-27 06:35:48.949988 eth-erc20-0.7.5/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      666 2021-04-04 12:48:14.000000 eth-erc20-0.7.5/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.943322 eth-erc20-0.7.5/static_token/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.949988 eth-erc20-0.7.5/static_token/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)    11366 2023-03-02 11:29:39.000000 eth-erc20-0.7.5/static_token/data/StaticToken.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     3288 2023-03-02 11:29:39.000000 eth-erc20-0.7.5/static_token/data/StaticToken.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       66 2022-04-22 18:28:18.000000 eth-erc20-0.7.5/static_token/data/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       51 2021-05-02 12:00:59.000000 eth-erc20-0.7.5/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-07-27 06:35:48.949988 eth-erc20-0.7.5/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      266 2023-02-23 08:04:58.000000 eth-erc20-0.7.5/tests/test_erc20_interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4318 2023-02-22 10:16:13.000000 eth-erc20-0.7.5/tests/test_giftable.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      733 2023-06-29 19:52:55.000000 eth-erc20-0.7.5/tests/test_static.py
```

### Comparing `eth-erc20-0.7.4/CHANGELOG` & `eth-erc20-0.7.5/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+* 0.7.5
+	- Factor out token publish method in unittest fixture
 * 0.7.4
 	- Add missing unittest module to python package
 * 0.7.3
 	- Add ERC5679Ext20 fills
 * 0.7.2
 	- Update python classifiers
 	- Upgrade to beta
```

### Comparing `eth-erc20-0.7.4/LICENSE` & `eth-erc20-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/PKG-INFO` & `eth-erc20-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-erc20
-Version: 0.7.4
+Version: 0.7.5
 Summary: ERC20 interface and simple contract with deployment script that lets any address mint and gift itself tokens.
 Home-page: https://git.defalsify.org/eth-erc20
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,ethereum,token,blockchain,cryptocurrency
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-erc20-0.7.4/WAIVER` & `eth-erc20-0.7.5/WAIVER`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/WAIVER.asc` & `eth-erc20-0.7.5/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/eth_erc20/data/ERC20.json` & `eth-erc20-0.7.5/eth_erc20/data/ERC20.json`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/eth_erc20/erc20.py` & `eth-erc20-0.7.5/eth_erc20/erc20.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/eth_erc20/runnable/balance.py` & `eth-erc20-0.7.5/eth_erc20/runnable/balance.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/eth_erc20/runnable/info.py` & `eth-erc20-0.7.5/eth_erc20/runnable/info.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/eth_erc20/runnable/transfer.py` & `eth-erc20-0.7.5/eth_erc20/runnable/transfer.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/eth_erc20/unittest/base.py` & `eth-erc20-0.7.5/eth_erc20/unittest/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from chainlib.eth.tx import (
         transaction,
         receipt,
         )
 from hexathon import strip_0x
 
 # local imports
-from giftable_erc20_token.unittest import TestGiftableToken
 from eth_erc20 import ERC20
 
 logging.basicConfig(level=logging.DEBUG)
 logg = logging.getLogger(__name__)
 
 
 class TestInterface:
@@ -49,20 +48,21 @@
         c = ERC20(self.chain_spec)
         o = c.symbol(self.address, sender_address=self.accounts[0])
         r = self.conn.do(o)
         symbol = ERC20.parse_symbol(r)
         self.assertEqual(self.symbol, symbol)
 
 
-    def test_transfer(self):
+    def test_direct_transfer(self):
         nonce_oracle = RPCNonceOracle(self.accounts[0], conn=self.conn)
         gas_oracle = OverrideGasOracle(limit=100000, conn=self.conn)
         c = ERC20(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle, gas_oracle=gas_oracle)
+
         (tx_hash, o) = c.transfer(self.address, self.accounts[0], self.accounts[1], 1000)
-        r = self.rpc.do(o)
+        self.rpc.do(o)
         o = receipt(tx_hash)
         r = self.rpc.do(o)
         self.assertEqual(r['status'], 1)
 
         o = c.balance_of(self.address, self.accounts[0], sender_address=self.accounts[0])
         r = self.rpc.do(o)
         balance = c.parse_balance(r)
@@ -81,15 +81,15 @@
 
 
     def test_transfer_from(self):
         nonce_oracle = RPCNonceOracle(self.accounts[0], conn=self.conn)
         gas_oracle = OverrideGasOracle(limit=100000, conn=self.conn)
         c = ERC20(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle, gas_oracle=gas_oracle)
         (tx_hash, o) = c.approve(self.address, self.accounts[0], self.accounts[1], 1000)
-        r = self.rpc.do(o)
+        self.rpc.do(o)
         o = receipt(tx_hash)
         r = self.rpc.do(o)
         self.assertEqual(r['status'], 1)
 
         o = c.allowance(self.address, self.accounts[0], self.accounts[1], sender_address=self.accounts[0])
         r = self.rpc.do(o)
         allowance = c.parse_allowance(r)
```

### Comparing `eth-erc20-0.7.4/eth_erc20.egg-info/PKG-INFO` & `eth-erc20-0.7.5/eth_erc20.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-erc20
-Version: 0.7.4
+Version: 0.7.5
 Summary: ERC20 interface and simple contract with deployment script that lets any address mint and gift itself tokens.
 Home-page: https://git.defalsify.org/eth-erc20
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,ethereum,token,blockchain,cryptocurrency
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-erc20-0.7.4/eth_erc20.egg-info/SOURCES.txt` & `eth-erc20-0.7.5/eth_erc20.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -33,8 +33,9 @@
 giftable_erc20_token/runnable/publish.py
 giftable_erc20_token/unittest/__init__.py
 giftable_erc20_token/unittest/base.py
 static_token/data/StaticToken.bin
 static_token/data/StaticToken.json
 static_token/data/__init__.py
 tests/test_erc20_interface.py
-tests/test_giftable.py
+tests/test_giftable.py
+tests/test_static.py
```

### Comparing `eth-erc20-0.7.4/giftable_erc20_token/data/GiftableToken.bin` & `eth-erc20-0.7.5/giftable_erc20_token/data/GiftableToken.bin`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/giftable_erc20_token/data/GiftableToken.json` & `eth-erc20-0.7.5/giftable_erc20_token/data/GiftableToken.json`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/giftable_erc20_token/factory.py` & `eth-erc20-0.7.5/giftable_erc20_token/factory.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/giftable_erc20_token/runnable/gift.py` & `eth-erc20-0.7.5/giftable_erc20_token/runnable/gift.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/giftable_erc20_token/runnable/minter.py` & `eth-erc20-0.7.5/giftable_erc20_token/runnable/minter.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/giftable_erc20_token/runnable/publish.py` & `eth-erc20-0.7.5/giftable_erc20_token/runnable/publish.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/giftable_erc20_token/unittest/base.py` & `eth-erc20-0.7.5/giftable_erc20_token/unittest/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,34 +18,42 @@
 class TestGiftableToken(EthTesterCase):
 
     expire = 0
 
     def setUp(self):
         super(TestGiftableToken, self).setUp()
         self.conn = RPCConnection.connect(self.chain_spec, 'default')
+       
+        address = self.publish_giftable_token('Foo Token', 'FOO', 16, expire=self.expire)
+        self.address = to_checksum_address(address)
         nonce_oracle = RPCNonceOracle(self.accounts[0], conn=self.conn)
         c = GiftableToken(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
-        self.symbol = 'FOO'
-        self.name = 'Foo Token'
-        self.decimals = 16
-        (tx_hash, o) = c.constructor(self.accounts[0], self.name, self.symbol, self.decimals, expire=self.expire)
-        self.rpc.do(o)
-        o = receipt(tx_hash)
-        r = self.rpc.do(o)
-        self.assertEqual(r['status'], 1)
-        self.address = to_checksum_address(r['contract_address'])
-        logg.debug('published on address {} with hash {}'.format(self.address, tx_hash))
-
         self.initial_supply = 1 << 40
         (tx_hash, o) = c.mint_to(self.address, self.accounts[0], self.accounts[0], self.initial_supply)
         r = self.conn.do(o)
         o = receipt(tx_hash)
         r = self.conn.do(o)
         self.assertEqual(r['status'], 1)
 
 
+    def publish_giftable_token(self, name, symbol, decimals=16, expire=None):
+        nonce_oracle = RPCNonceOracle(self.accounts[0], conn=self.conn)
+        c = GiftableToken(self.chain_spec, signer=self.signer, nonce_oracle=nonce_oracle)
+        self.symbol = name
+        self.name = symbol
+        self.decimals = decimals
+        (tx_hash, o) = c.constructor(self.accounts[0], self.name, self.symbol, self.decimals, expire=expire)
+        self.rpc.do(o)
+        o = receipt(tx_hash)
+        r = self.rpc.do(o)
+        self.assertEqual(r['status'], 1)
+        address = r['contract_address'] 
+        logg.debug('published on address {} with hash {}'.format(address, tx_hash))
+        return address
+
+
 class TestGiftableExpireToken(TestGiftableToken):
 
     expire = int(time.time()) + 100000
 
     def setUp(self):
         super(TestGiftableExpireToken, self).setUp()
```

### Comparing `eth-erc20-0.7.4/setup.cfg` & `eth-erc20-0.7.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-erc20
-version = 0.7.4
+version = 0.7.5
 description = ERC20 interface and simple contract with deployment script that lets any address mint and gift itself tokens.
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-erc20
 keywords = 
 	dlt
 	ethereum
```

### Comparing `eth-erc20-0.7.4/setup.py` & `eth-erc20-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/static_token/data/StaticToken.bin` & `eth-erc20-0.7.5/static_token/data/StaticToken.bin`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/static_token/data/StaticToken.json` & `eth-erc20-0.7.5/static_token/data/StaticToken.json`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.4/tests/test_giftable.py` & `eth-erc20-0.7.5/tests/test_giftable.py`

 * *Files identical despite different names*

