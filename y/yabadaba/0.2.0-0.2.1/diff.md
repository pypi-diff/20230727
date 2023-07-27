# Comparing `tmp/yabadaba-0.2.0.tar.gz` & `tmp/yabadaba-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\lmh1\Documents\Python-packages\yabadaba\dist\.tmp-h1ms0vxj\yabadaba-0.2.0.tar", last modified: Tue Apr 18 20:07:48 2023, max compression
+gzip compressed data, was "C:\Users\lmh1\Documents\Python-packages\yabadaba\dist\.tmp-xvwqrz8l\yabadaba-0.2.1.tar", last modified: Thu Jul 27 15:26:16 2023, max compression
```

## Comparing `yabadaba-0.2.0.tar` & `yabadaba-0.2.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 20:07:48.000000 yabadaba-0.2.0/
--rw-rw-rw-   0        0        0     2776 2022-02-03 20:26:52.000000 yabadaba-0.2.0/LICENSE.TXT
--rw-rw-rw-   0        0        0     3687 2023-04-18 20:07:48.000000 yabadaba-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2868 2022-10-03 13:54:02.000000 yabadaba-0.2.0/README.rst
--rw-rw-rw-   0        0        0      108 2022-02-03 20:26:52.000000 yabadaba-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 20:07:48.000000 yabadaba-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1594 2023-04-06 16:49:21.000000 yabadaba-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:07:48.000000 yabadaba-0.2.0/tests/
--rw-rw-rw-   0        0        0    11546 2022-03-03 19:56:36.000000 yabadaba-0.2.0/tests/test_Settings.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba/
--rw-rw-rw-   0        0        0    16425 2023-04-10 16:33:33.000000 yabadaba-0.2.0/yabadaba/Settings.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba/UnitConverter/
--rw-rw-rw-   0        0        0    19559 2023-03-28 18:17:55.000000 yabadaba-0.2.0/yabadaba/UnitConverter/__init__.py
--rw-rw-rw-   0        0        0      360 2023-03-22 16:04:46.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_acceleration.py
--rw-rw-rw-   0        0        0      853 2023-03-22 16:08:23.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_capacitance.py
--rw-rw-rw-   0        0        0      430 2023-03-22 16:10:01.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_charge.py
--rw-rw-rw-   0        0        0     1018 2023-03-22 14:52:27.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_concentration.py
--rw-rw-rw-   0        0        0     4403 2023-03-22 15:46:30.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_constants.py
--rw-rw-rw-   0        0        0      508 2023-03-22 16:14:00.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_current.py
--rw-rw-rw-   0        0        0     1930 2023-03-22 15:56:01.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_energy.py
--rw-rw-rw-   0        0        0     1004 2023-03-22 14:52:23.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_force.py
--rw-rw-rw-   0        0        0     1723 2023-03-22 16:15:59.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_frequency.py
--rw-rw-rw-   0        0        0     1764 2023-03-22 16:14:55.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_length.py
--rw-rw-rw-   0        0        0      871 2023-03-22 16:21:43.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_magnetic.py
--rw-rw-rw-   0        0        0      973 2023-03-22 14:44:22.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_mass.py
--rw-rw-rw-   0        0        0     1046 2023-03-22 16:25:12.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_power.py
--rw-rw-rw-   0        0        0     1337 2023-03-22 15:13:37.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_pressure.py
--rw-rw-rw-   0        0        0     1151 2023-03-22 16:29:43.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_resistance.py
--rw-rw-rw-   0        0        0      591 2023-03-22 16:32:05.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_temperature.py
--rw-rw-rw-   0        0        0      864 2023-03-22 14:44:23.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_time.py
--rw-rw-rw-   0        0        0      657 2023-03-22 16:34:29.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_voltage.py
--rw-rw-rw-   0        0        0      837 2023-03-22 14:44:25.000000 yabadaba-0.2.0/yabadaba/UnitConverter/_volume.py
--rw-rw-rw-   0        0        0        5 2023-04-03 18:40:10.000000 yabadaba-0.2.0/yabadaba/VERSION
--rw-rw-rw-   0        0        0      870 2023-03-22 20:12:58.000000 yabadaba-0.2.0/yabadaba/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba/database/
--rw-rw-rw-   0        0        0    25471 2023-03-24 15:03:03.000000 yabadaba-0.2.0/yabadaba/database/CDCSDatabase.py
--rw-rw-rw-   0        0        0    21950 2023-03-06 20:58:23.000000 yabadaba-0.2.0/yabadaba/database/Database.py
--rw-rw-rw-   0        0        0    34293 2022-04-26 15:36:50.000000 yabadaba-0.2.0/yabadaba/database/LocalDatabase.py
--rw-rw-rw-   0        0        0    23681 2022-05-23 16:09:40.000000 yabadaba-0.2.0/yabadaba/database/MongoDatabase.py
--rw-rw-rw-   0        0        0      579 2022-03-31 17:23:57.000000 yabadaba-0.2.0/yabadaba/database/__init__.py
--rw-rw-rw-   0        0        0     2912 2022-02-03 20:26:52.000000 yabadaba-0.2.0/yabadaba/database/load_database.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba/demo/
--rw-rw-rw-   0        0        0     1928 2022-02-03 20:26:52.000000 yabadaba-0.2.0/yabadaba/demo/BadRecord.py
--rw-rw-rw-   0        0        0     4615 2023-03-28 14:18:59.000000 yabadaba-0.2.0/yabadaba/demo/FAQ.py
--rw-rw-rw-   0        0        0      448 2022-02-03 20:26:52.000000 yabadaba-0.2.0/yabadaba/demo/FAQ.xsd
--rw-rw-rw-   0        0        0      583 2022-02-03 20:26:52.000000 yabadaba-0.2.0/yabadaba/demo/FAQ.xsl
--rw-rw-rw-   0        0        0      649 2022-02-03 20:26:52.000000 yabadaba-0.2.0/yabadaba/demo/README.rst
--rw-rw-rw-   0        0        0        0 2022-02-03 20:26:52.000000 yabadaba-0.2.0/yabadaba/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba/query/
--rw-rw-rw-   0        0        0     4185 2023-04-06 17:56:05.000000 yabadaba-0.2.0/yabadaba/query/DateMatchQuery.py
--rw-rw-rw-   0        0        0     6728 2023-04-06 17:55:54.000000 yabadaba-0.2.0/yabadaba/query/FloatMatchQuery.py
--rw-rw-rw-   0        0        0     4264 2023-04-06 17:55:46.000000 yabadaba-0.2.0/yabadaba/query/IntMatchQuery.py
--rw-rw-rw-   0        0        0     4571 2023-04-06 17:55:40.000000 yabadaba-0.2.0/yabadaba/query/ListContainsQuery.py
--rw-rw-rw-   0        0        0     5205 2023-04-06 17:56:14.000000 yabadaba-0.2.0/yabadaba/query/Query.py
--rw-rw-rw-   0        0        0     4641 2023-04-06 17:55:27.000000 yabadaba-0.2.0/yabadaba/query/StrContainsQuery.py
--rw-rw-rw-   0        0        0     4072 2023-04-06 17:55:21.000000 yabadaba-0.2.0/yabadaba/query/StrMatchQuery.py
--rw-rw-rw-   0        0        0     1949 2023-03-28 14:16:07.000000 yabadaba-0.2.0/yabadaba/query/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba/record/
--rw-rw-rw-   0        0        0    11174 2023-04-10 16:34:02.000000 yabadaba-0.2.0/yabadaba/record/Record.py
--rw-rw-rw-   0        0        0     1142 2022-04-26 15:36:50.000000 yabadaba-0.2.0/yabadaba/record/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba/tools/
--rw-rw-rw-   0        0        0     4712 2022-05-23 16:09:40.000000 yabadaba-0.2.0/yabadaba/tools/ModuleManager.py
--rw-rw-rw-   0        0        0      227 2022-03-01 22:40:28.000000 yabadaba-0.2.0/yabadaba/tools/__init__.py
--rw-rw-rw-   0        0        0      464 2022-03-01 22:41:57.000000 yabadaba-0.2.0/yabadaba/tools/screen_input.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba.egg-info/
--rw-rw-rw-   0        0        0     3687 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1771 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-02-03 20:58:36.000000 yabadaba-0.2.0/yabadaba.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       65 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 20:07:48.000000 yabadaba-0.2.0/yabadaba.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/
+-rw-rw-rw-   0        0        0     2776 2022-02-03 20:26:52.000000 yabadaba-0.2.1/LICENSE.TXT
+-rw-rw-rw-   0        0        0     3636 2023-07-27 15:26:16.000000 yabadaba-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2868 2022-10-03 13:54:02.000000 yabadaba-0.2.1/README.rst
+-rw-rw-rw-   0        0        0      108 2022-02-03 20:26:52.000000 yabadaba-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 15:26:16.000000 yabadaba-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1602 2023-07-27 15:25:08.000000 yabadaba-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/tests/
+-rw-rw-rw-   0        0        0    11546 2022-03-03 19:56:36.000000 yabadaba-0.2.1/tests/test_Settings.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/
+-rw-rw-rw-   0        0        0    16425 2023-04-10 16:33:33.000000 yabadaba-0.2.1/yabadaba/Settings.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/UnitConverter/
+-rw-rw-rw-   0        0        0    19559 2023-03-28 18:17:55.000000 yabadaba-0.2.1/yabadaba/UnitConverter/__init__.py
+-rw-rw-rw-   0        0        0      360 2023-03-22 16:04:46.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_acceleration.py
+-rw-rw-rw-   0        0        0      853 2023-03-22 16:08:23.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_capacitance.py
+-rw-rw-rw-   0        0        0      430 2023-03-22 16:10:01.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_charge.py
+-rw-rw-rw-   0        0        0     1018 2023-03-22 14:52:27.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_concentration.py
+-rw-rw-rw-   0        0        0     4403 2023-03-22 15:46:30.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_constants.py
+-rw-rw-rw-   0        0        0      508 2023-03-22 16:14:00.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_current.py
+-rw-rw-rw-   0        0        0     1930 2023-03-22 15:56:01.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_energy.py
+-rw-rw-rw-   0        0        0     1004 2023-03-22 14:52:23.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_force.py
+-rw-rw-rw-   0        0        0     1723 2023-03-22 16:15:59.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_frequency.py
+-rw-rw-rw-   0        0        0     1764 2023-03-22 16:14:55.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_length.py
+-rw-rw-rw-   0        0        0      871 2023-03-22 16:21:43.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_magnetic.py
+-rw-rw-rw-   0        0        0      973 2023-03-22 14:44:22.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_mass.py
+-rw-rw-rw-   0        0        0     1046 2023-03-22 16:25:12.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_power.py
+-rw-rw-rw-   0        0        0     1337 2023-03-22 15:13:37.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_pressure.py
+-rw-rw-rw-   0        0        0     1151 2023-03-22 16:29:43.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_resistance.py
+-rw-rw-rw-   0        0        0      591 2023-03-22 16:32:05.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_temperature.py
+-rw-rw-rw-   0        0        0      864 2023-03-22 14:44:23.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_time.py
+-rw-rw-rw-   0        0        0      657 2023-03-22 16:34:29.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_voltage.py
+-rw-rw-rw-   0        0        0      837 2023-03-22 14:44:25.000000 yabadaba-0.2.1/yabadaba/UnitConverter/_volume.py
+-rw-rw-rw-   0        0        0        5 2023-07-26 14:08:45.000000 yabadaba-0.2.1/yabadaba/VERSION
+-rw-rw-rw-   0        0        0      949 2023-07-27 15:01:17.000000 yabadaba-0.2.1/yabadaba/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/database/
+-rw-rw-rw-   0        0        0    25382 2023-07-26 19:09:37.000000 yabadaba-0.2.1/yabadaba/database/CDCSDatabase.py
+-rw-rw-rw-   0        0        0    21607 2023-05-24 01:58:18.000000 yabadaba-0.2.1/yabadaba/database/Database.py
+-rw-rw-rw-   0        0        0    33742 2023-07-26 14:08:45.000000 yabadaba-0.2.1/yabadaba/database/LocalDatabase.py
+-rw-rw-rw-   0        0        0    23457 2023-07-26 14:08:45.000000 yabadaba-0.2.1/yabadaba/database/MongoDatabase.py
+-rw-rw-rw-   0        0        0      579 2022-03-31 17:23:57.000000 yabadaba-0.2.1/yabadaba/database/__init__.py
+-rw-rw-rw-   0        0        0     2932 2023-05-30 15:03:22.000000 yabadaba-0.2.1/yabadaba/database/load_database.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/demo/
+-rw-rw-rw-   0        0        0     1928 2022-02-03 20:26:52.000000 yabadaba-0.2.1/yabadaba/demo/BadRecord.py
+-rw-rw-rw-   0        0        0     4615 2023-03-28 14:18:59.000000 yabadaba-0.2.1/yabadaba/demo/FAQ.py
+-rw-rw-rw-   0        0        0      448 2022-02-03 20:26:52.000000 yabadaba-0.2.1/yabadaba/demo/FAQ.xsd
+-rw-rw-rw-   0        0        0      583 2022-02-03 20:26:52.000000 yabadaba-0.2.1/yabadaba/demo/FAQ.xsl
+-rw-rw-rw-   0        0        0      649 2022-02-03 20:26:52.000000 yabadaba-0.2.1/yabadaba/demo/README.rst
+-rw-rw-rw-   0        0        0        0 2022-02-03 20:26:52.000000 yabadaba-0.2.1/yabadaba/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/query/
+-rw-rw-rw-   0        0        0     4185 2023-04-06 17:56:05.000000 yabadaba-0.2.1/yabadaba/query/DateMatchQuery.py
+-rw-rw-rw-   0        0        0     6728 2023-04-06 17:55:54.000000 yabadaba-0.2.1/yabadaba/query/FloatMatchQuery.py
+-rw-rw-rw-   0        0        0     4264 2023-04-06 17:55:46.000000 yabadaba-0.2.1/yabadaba/query/IntMatchQuery.py
+-rw-rw-rw-   0        0        0     4571 2023-04-06 17:55:40.000000 yabadaba-0.2.1/yabadaba/query/ListContainsQuery.py
+-rw-rw-rw-   0        0        0     5205 2023-04-06 17:56:14.000000 yabadaba-0.2.1/yabadaba/query/Query.py
+-rw-rw-rw-   0        0        0     4641 2023-04-06 17:55:27.000000 yabadaba-0.2.1/yabadaba/query/StrContainsQuery.py
+-rw-rw-rw-   0        0        0     4072 2023-04-06 17:55:21.000000 yabadaba-0.2.1/yabadaba/query/StrMatchQuery.py
+-rw-rw-rw-   0        0        0     1949 2023-03-28 14:16:07.000000 yabadaba-0.2.1/yabadaba/query/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/record/
+-rw-rw-rw-   0        0        0    14645 2023-05-31 15:37:50.000000 yabadaba-0.2.1/yabadaba/record/Record.py
+-rw-rw-rw-   0        0        0     1379 2023-05-30 15:05:24.000000 yabadaba-0.2.1/yabadaba/record/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba/tools/
+-rw-rw-rw-   0        0        0     4980 2023-07-26 14:08:45.000000 yabadaba-0.2.1/yabadaba/tools/ModuleManager.py
+-rw-rw-rw-   0        0        0      227 2022-03-01 22:40:28.000000 yabadaba-0.2.1/yabadaba/tools/__init__.py
+-rw-rw-rw-   0        0        0      464 2022-03-01 22:41:57.000000 yabadaba-0.2.1/yabadaba/tools/screen_input.py
+drwxrwxrwx   0        0        0        0 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba.egg-info/
+-rw-rw-rw-   0        0        0     3636 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1771 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-02-03 20:58:36.000000 yabadaba-0.2.1/yabadaba.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       65 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 15:26:16.000000 yabadaba-0.2.1/yabadaba.egg-info/top_level.txt
```

### Comparing `yabadaba-0.2.0/LICENSE.TXT` & `yabadaba-0.2.1/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/PKG-INFO` & `yabadaba-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: yabadaba
-Version: 0.2.0
+Version: 0.2.1
 Summary: Yay, a base database! An abstraction layer allowing for common interactions with Mongo, CDCS and local directory databases and records.
 Home-page: https://github.com/usnistgov/yabadaba
 Author: Lucas Hale
 Author-email: lucas.hale@nist.gov
 Keywords: database,mongodb,CDCS
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: LICENSE.TXT
```

### Comparing `yabadaba-0.2.0/README.rst` & `yabadaba-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/setup.py` & `yabadaba-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from setuptools import setup, find_packages
 
 def getreadme():
+    """Fetches long description from the README file"""
     with open('README.rst', encoding='utf-8') as readme_file:
         return readme_file.read()
 
 def getversion():
     """Fetches version information from VERSION file"""
     with open('yabadaba/VERSION', encoding='utf-8') as version_file:
         return version_file.read().strip()
@@ -13,26 +14,25 @@
       version = getversion(),
       description = 'Yay, a base database! An abstraction layer allowing for common interactions with Mongo, CDCS and local directory databases and records.',
       long_description = getreadme(),
       classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Natural Language :: English',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Physics'
       ],
       keywords = [
         'database', 
         'mongodb', 
         'CDCS',
-      ], 
+      ],
       url = 'https://github.com/usnistgov/yabadaba',
       author = 'Lucas Hale',
       author_email = 'lucas.hale@nist.gov',
       packages = find_packages(),
       install_requires = [
         'lxml',
         'DataModelDict',
@@ -40,8 +40,8 @@
         'numpy', 
         'pandas',
         'cdcs>=0.2.1',
         'pymongo',
         'tqdm',
       ],
       package_data={'': ['*']},
-      zip_safe = False)
+      zip_safe = False)
```

### Comparing `yabadaba-0.2.0/tests/test_Settings.py` & `yabadaba-0.2.1/tests/test_Settings.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/Settings.py` & `yabadaba-0.2.1/yabadaba/Settings.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/__init__.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/__init__.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_capacitance.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_capacitance.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_concentration.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_concentration.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_constants.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_constants.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_energy.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_energy.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_force.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_force.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_frequency.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_frequency.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_length.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_length.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_magnetic.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_magnetic.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_mass.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_mass.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_power.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_power.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_pressure.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_pressure.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_resistance.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_resistance.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_temperature.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_temperature.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_time.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_time.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_voltage.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_voltage.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/UnitConverter/_volume.py` & `yabadaba-0.2.1/yabadaba/UnitConverter/_volume.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/database/CDCSDatabase.py` & `yabadaba-0.2.1/yabadaba/database/CDCSDatabase.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # Relative imports
 from ..tools import aslist, iaslist
 from . import Database
 from .. import load_record, recordmanager
 
 class CDCSDatabase(Database):
-    
+
     def __init__(self,
                  host: str,
                  username: Optional[str] = None,
                  password: Optional[str] = None,
                  auth: Optional[Tuple[str]] = None,
                  cert: Union[str, Tuple[str], None] = None, 
                  certification: Union[str, Tuple[str], None] = None,
@@ -60,41 +60,40 @@
         cdcsversion : str, optional
             For CDCS versions 2.X.X, this allows for specifying the full CDCS
             version to ensure the class methods perform the correct REST
             calls.  This can be specified as "#.#.#", or if None is given will
             default to "2.15.0".  For CDCS versions 3.X.X, this is ignored as
             version info is obtained directly from the database.
         """
-        
         # Fetch password from file if needed
         try:
-            with open(password) as f:
+            with open(password, encoding='UTF-8') as f:
                 password = f.read().strip()
-        except:
+        except Exception:
             pass
-        
+
         # Pass parameters to cdcs object
         self.__cdcs = CDCS(host, username=username, password=password, auth=auth,
                            cert=cert, certification=certification, verify=verify,
                            cdcsversion=cdcsversion)
-        
+
         # Pass host to Database initializer
         Database.__init__(self, host)
-    
+
     @property
     def style(self):
         """str: The database style"""
         return 'cdcs'
 
     @property
     def cdcs(self):
         """cdcs.CDCS : The underlying database API object."""
         return self.__cdcs
 
-    def get_records(self, style=None, name=None, return_df=False,
+    def get_records(self, style=None, return_df=False, name=None,
                     query=None, keyword=None, **kwargs):
         """
         Produces a list of all matching records in the database.
         
         Parameters
         ----------
         style : str, optional
@@ -136,21 +135,22 @@
         elif query is not None:
             assert len(kwargs) == 0, 'query cannot be given with kwargs'
         else:
             query = load_record(style).cdcsquery(**kwargs)
 
         def build_records(series):
             return load_record(series.template_title, model=series.xml_content,
-                               name=series.title)
-        
+                               name=series.title, database=self)
+
         # Build records by querying for each record name (or None)
         records = []
         for n in iaslist(name):
             data = self.cdcs.query(title=n, template=style, mongoquery=query, keyword=keyword)
-            records.extend(data.apply(build_records, axis=1))
+            if len(data) > 0:
+                records.extend(data.apply(build_records, axis=1))
         records = np.array(records)
 
         # Build df
         if len(records) > 0:
             df = []
             for record in records:
                 df.append(record.metadata())
@@ -163,15 +163,15 @@
         records = records[df.index.tolist()]
 
         # Return records (and df)
         if return_df:
             return records, df.reset_index(drop=True)
         else:
             return records
-    
+
     def get_records_df(self, style=None, name=None, query=None, keyword=None, **kwargs):
         """
         Produces a list of all matching records in the database.
         
         Parameters
         ----------
         style : str, optional
@@ -191,15 +191,15 @@
             
         Returns
         -------
         records_df : pandas.DataFrame
             The corresponding metadata values for the records.
         """
         return self.get_records(style, name=name, query=query, keyword=keyword, return_df=True, **kwargs)[1]
-    
+
     def get_record(self, style=None, name=None, query=None, keyword=None, **kwargs):
         """
         Returns a single matching record from the database.
         
         Parameters
         ----------
         style : str, optional
@@ -243,15 +243,15 @@
             return records[0]
         elif len(records) == 0:
             raise ValueError('No matching records found')
         else:
             raise ValueError('Multiple matching records found')
     
     def add_record(self, record=None, style=None, name=None, model=None,
-                   build=False, workspace=None, verbose=False):
+                   build=False, verbose=False, workspace=None):
         """
         Adds a new record to the database.
         
         Parameters
         ----------
         record : iprPy.Record, optional
             The new record to add to the database.  If not given, then name,
@@ -285,43 +285,43 @@
         
         Raises
         ------
         ValueError
             If style, name and/or model given with record, or a matching record
             already exists.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = load_record(style, model=model, name=name)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None or model is not None:
             raise ValueError('kwargs style, name, and model cannot be given with kwarg record')
-            
+
         # Retrieve/build model contents
         try:
             assert build is False
             content = record.model.xml()
-        except:
+        except Exception:
             content = record.build_model().xml()
 
         # Upload to database
         self.cdcs.upload_record(template=record.style, content=content,
                                 title=record.name)
         if verbose:
             print(f'{record} added to {self.host}')
 
         if workspace is not None:
             self.assign_records(record, workspace, verbose=verbose)
 
         return record
-    
+
     def update_record(self, record=None, style=None, name=None, model=None,
-                      build=False, workspace=None, verbose=False):
+                      build=False, verbose=False, workspace=None):
         """
         Replaces an existing record with a new record of matching name and 
         style, but new content.
         
         Parameters
         ----------
         record : Record, optional
@@ -356,51 +356,51 @@
         Raises
         ------
         TypeError
             If no new content is given.
         ValueError
             If style, model, and/or name given with record.
         """
-        
+
         # Create Record object if not given
         if record is None:
             if model is None:
                 raise TypeError('no new model given')
             oldrecord = self.get_record(name=name, style=style)
             record = load_record(oldrecord.style, model=model, name=oldrecord.name)
-        
+
         # Use given record object
         else:
             if style is not None or name is not None:
                 raise ValueError('kwargs style and name cannot be given with kwarg record')
-            
+
             # Replace model in record object
             if model is not None:
                 record = load_record(record.style, model=model, name=record.name)
-        
+
         # Retrieve/build model contents
         try:
             assert build is False
             content = record.model.xml()
-        except:
+        except Exception:
             content = record.build_model().xml()
 
         # Upload to database
         self.cdcs.update_record(template=record.style, content=content,
                                 title=record.name)
-        
+
         if verbose:
             print(f'{record} updated in {self.host}')
 
         if workspace is not None:
             self.assign_records(record, workspace, verbose=verbose)
 
         return record
-    
-    def delete_record(self, record=None, name=None, style=None, verbose=False):
+
+    def delete_record(self, record=None, style=None, name=None, verbose=False):
         """
         Permanently deletes a record from the database.  Will issue an error 
         if exactly one matching record is not found in the database.
         
         Parameters
         ----------
         record : Record, optional
@@ -415,22 +415,21 @@
             value is False.
             
         Raises
         ------
         ValueError
             If style and/or name content given with record.
         """
-        
         # Extract values from Record object if given
         if record is not None:
             if style is not None or name is not None:
                 raise ValueError('kwargs style and name cannot be given with kwarg record')
             name = record.name
             style = record.style
-         
+
         # Delete record
         self.cdcs.delete_record(template=style, title=name)
 
         if verbose:
             print(f'{record} deleted from {self.host}')
 
     def assign_records(self, records, workspace, verbose=False):
@@ -443,22 +442,22 @@
             The record(s) to assign to the workspace.
         workspace : str
             The workspace to assign the records to.
         verbose : bool, optional
             Setting this to True will print extra status messages.  Default
             value is False.
         """
-        ids = []
+        #ids = []
         for record in aslist(records):
             self.cdcs.assign_records(workspace, template=record.style,
                                      title=record.name)
             if verbose:
                 print(f'{record} assigned to workspace {workspace}')
 
-    def add_tar(self, record=None, name=None, style=None, tar=None, root_dir=None):
+    def add_tar(self, record=None, style=None, name=None, tar=None, root_dir=None):
         """
         Archives and stores a folder associated with a record.
         
         Parameters
         ----------
         record : Record, optional
             The record to associate the tar archive with.  If not given, then
@@ -479,76 +478,76 @@
         
         Raises
         ------
         ValueError
             If style and/or name content given with record or the record already
             has an archive.
         """
-        
+
         # Get Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         else:
             # Issue a ValueError for competing kwargs
             if style is not None or name is not None:
                 raise ValueError('kwargs style and name cannot be given with kwarg record')
 
             # Verify that record exists
             record = self.get_record(name=record.name, style=record.style)
-        
+
         # Check if an archive already exists
         blobs = self.cdcs.get_blobs(filename=record.name)
         if len(blobs) > 0:
             raise ValueError('Record already has an archive')
-        
+
         # Create directory archive and upload
         if tar is None: 
             if root_dir is None:
                 root_dir = Path.cwd()
-                
+
             # Make archive
             basename = Path(root_dir, record.name)
             filename = Path(root_dir, record.name + '.tar.gz')
             shutil.make_archive(basename, 'gztar', root_dir=root_dir,
                                 base_dir=record.name)
-            
+
             # Upload archive
             tries = 0
             while tries < 2:
-                if True:
+                tries += 1
+                try:
                     url = self.cdcs.upload_blob(filename.as_posix())
                     break
-                else:
-                    tries += 1
-            if tries == 2:
-                raise ValueError('Failed to upload archive 2 times')
-            
+                except Exception as err:
+                    if tries == 2:
+                        raise ValueError('Failed to upload archive 2 times') from err
+
             # Remove local archive copy
             filename.unlink()
-        
+
         # Upload pre-existing tar object
         elif root_dir is None:
             filename = Path(record.name + '.tar.gz')
 
             # Upload archive
             tries = 0
             while tries < 2:
-                if True:
+                tries += 1
+                try:
                     url = self.cdcs.upload_blob(filename=filename, blobbytes=BytesIO(tar))
                     break
-                else:
-                    tries += 1
-            if tries == 2:
-                raise ValueError('Failed to upload archive 2 times')
-        
+                except Exception as err:
+                    if tries == 2:
+                        raise ValueError('Failed to upload archive 2 times') from err
+
         else:
             raise ValueError('tar and root_dir cannot both be given')
 
-    def get_tar(self, record=None, name=None, style=None, raw=False):
+    def get_tar(self, record=None, style=None, name=None, raw=False):
         """
         Retrives the tar archive associated with a record in the database.
         
         Parameters
         ----------
         record : Record, optional
             The record to retrive the associated tar archive for.
@@ -571,67 +570,71 @@
         ValueError
             If style and/or name content given with record.
         """
 
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a TypeError for competing kwargs
         elif style is not None or name is not None:
             raise TypeError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Verify that record exists
-        else:
-            record = self.get_record(name=record.name, style=record.style)
-        
+        #else:
+        #    record = self.get_record(name=record.name, style=record.style)
+
         filename = Path(record.name + '.tar.gz')
 
         # Download tar file
         tardata = self.cdcs.get_blob_contents(filename=filename)
-        
+
+        tar = tarfile.open(fileobj = BytesIO(tardata))
+
+        record.tar = tar
+
         # Return contents
         if raw is True:
             return tardata
         else:
-            return tarfile.open(fileobj = BytesIO(tardata))
-    
-    def delete_tar(self, record=None, name=None, style=None):
+            return tar
+
+    def delete_tar(self, record=None, style=None, name=None):
         """
         Deletes a tar file from the database.
         
         Parameters
         ----------
         record : Record, optional
             The record associated with the tar archive to delete.  If not
             given, then name and/or style necessary to uniquely identify
             the record are needed.
         name : str, optional
             The name to use in uniquely identifying the record.
         style : str, optional
             The style to use in uniquely identifying the record.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a TypeError for competing kwargs
         elif style is not None or name is not None:
             raise TypeError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Verify that record exists
         else:
             record = self.get_record(name=record.name, style=record.style)
-        
+
         filename = Path(record.name + '.tar.gz')
 
         self.cdcs.delete_blob(filename=filename)
 
-    def update_tar(self, record=None, name=None, style=None, tar=None, root_dir=None):
+    def update_tar(self, record=None, style=None, name=None, tar=None, root_dir=None):
         """
         Archives and stores a folder associated with a record.
         
         Parameters
         ----------
         record : Record, optional
             The record to associate the tar archive with.  If not given, then
@@ -652,10 +655,10 @@
         
         Raises
         ------
         ValueError
             If style and/or name content given with record or the record already
             has an archive.
         """
-        
+
         self.delete_tar(record=record, name=name, style=style)
-        self.add_tar(record=record, name=name, style=style, tar=tar, root_dir=root_dir)
+        self.add_tar(record=record, name=name, style=style, tar=tar, root_dir=root_dir)
```

### Comparing `yabadaba-0.2.0/yabadaba/database/Database.py` & `yabadaba-0.2.1/yabadaba/database/Database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 # coding: utf-8
 # Standard Python libraries
 from pathlib import Path
 
 from tqdm import tqdm
 
-# https://github.com/usnistgov/DataModelDict
-from DataModelDict import DataModelDict as DM
-
 # iprPy imports
 from ..record import recordmanager, load_record
 from ..tools import screen_input
 
 class Database():
     """
     Class for handling different database styles in the same fashion.  This
     base class defines the common methods and attributes.
     """
-    
+
     def __init__(self, host):
         """
         Initializes a connection to a database.
         
         Parameters
         ----------
         host : str
             The host name (path, url, etc.) for the database.
         """
         # Check that object is a subclass
         if self.__module__ == __name__:
             raise TypeError("Don't use Database itself, only use derived classes")
-        
+
         # Set property values
         self.__host = host
-    
+
     def __str__(self):
         """
         Returns
         -------
         str
             The string representation of the database.
         """
         return f'database style {self.style} at {self.host}'
-    
+
     @property
     def style(self):
         """str: The database style"""
         raise NotImplementedError('Not defined for base class')
-    
+
     @property
     def host(self):
         """str: The database's host."""
         return self.__host
-    
+
     def get_records(self, style=None, return_df=False, **kwargs):
         """
         Produces a list of all matching records in the database.
         
         Parameters
         ----------
         style : str, optional
@@ -77,15 +74,15 @@
         
         Raises
         ------
         AttributeError
             If get_records is not defined for database style.
         """
         raise AttributeError('get_records not defined for Database style')
-    
+
     def get_record(self, style=None, **kwargs):
         """
         Returns a single matching record from the database.  Issues an error
         if multiple or no matching records are found.
         
         Parameters
         ----------
@@ -102,15 +99,15 @@
         
         Raises
         ------
         AttributeError
             If get_record is not defined for database style.
         """
         raise AttributeError('get_record not defined for Database style')
-    
+
     def get_records_df(self, style=None, **kwargs):
         """
         Produces a pandas.DataFrame of all matching records in the database.
         
         Parameters
         ----------
         style : str
@@ -126,15 +123,15 @@
         
         Raises
         ------
         AttributeError
             If get_record is not defined for database style.
         """
         raise AttributeError('get_records_df not defined for Database style')
-    
+
     def retrieve_record(self, style=None, dest=None, format='json', indent=4,
                         verbose=False, **kwargs):
         """
         Gets a single matching record from the database and saves it to a
         file based on the record's name.
 
         Parameters
@@ -168,15 +165,15 @@
         # Save as json
         if format == 'json':
             fname = Path(dest, f'{record.name}.json')
             with open(fname, 'w', encoding='UTF-8') as f:
                 record.model.json(fp=f, indent=indent, ensure_ascii=False)
             if verbose:
                 print(f'{fname} saved')
-        
+
         # Save as xml
         elif format == 'xml':
             fname = Path(dest, f'{record.name}.xml')
             with open(fname, 'w', encoding='UTF-8') as f:
                 record.model.xml(fp=f, indent=indent)
             if verbose:
                 print(f'{fname} saved')
@@ -219,15 +216,15 @@
         
         Raises
         ------
         AttributeError
             If add_record is not defined for database style.
         """
         raise AttributeError('add_record not defined for Database style')
-    
+
     def update_record(self, record=None, style=None, name=None, model=None,
                       build=False, verbose=False):
         """
         Replaces an existing record with a new record of matching name and
         style, but new content.
         
         Parameters
@@ -259,15 +256,15 @@
         
         Raises
         ------
         AttributeError
             If update_record is not defined for database style.
         """
         raise AttributeError('update_record not defined for Database style')
-    
+
     def delete_record(self, record=None, style=None, name=None):
         """
         Permanently deletes a record from the database.
         
         Parameters
         ----------
         record : Record, optional
@@ -281,16 +278,14 @@
         
         Raises
         ------
         AttributeError
             If delete_record is not defined for database style.
         """
         raise AttributeError('delete_record not defined for Database style')
-    
-    
 
     def get_tar(self, record=None, style=None, name=None, raw=False):
         """
         Retrives the tar archive associated with a record in the database.
         
         Parameters
         ----------
@@ -312,15 +307,15 @@
         
         Raises
         ------
         AttributeError
             If get_tar is not defined for database style.
         """
         raise AttributeError('get_tar not defined for Database style')
-    
+
     def add_tar(self, record=None, style=None, name=None, tar=None, root_dir=None):
         """
         Archives and stores a folder associated with a record.
         
         Parameters
         ----------
         record : Record, optional
@@ -343,15 +338,15 @@
         Raises
         ------
         ValueError
             If style and/or name content given with record or the record already
             has an archive.
         """
         raise AttributeError('add_tar not defined for Database style')
-    
+
     def update_tar(self, record=None, style=None, name=None, tar=None, root_dir=None):
         """
         Replaces an existing tar archive for a record with a new one.
         
         Parameters
         ----------
         record : Record, optional
@@ -373,37 +368,37 @@
         
         Raises
         ------
         AttributeError
             If update_tar is not defined for database style.
         """
         raise AttributeError('update_tar not defined for Database style')
-    
+
     def delete_tar(self, record=None, style=None, name=None):
         """
         Deletes a tar file from the database.
         
         Parameters
         ----------
         record : Record, optional
             The record associated with the tar archive to delete.  If not
-            given, then name and/or style necessary to uniquely identify
-            the record are needed.
+            given, then name and/or style are necessary to uniquely identify
+            the record.
         style : str, optional
             The style to use in uniquely identifying the record.
         name : str, optional
             The name to use in uniquely identifying the record.
         
         Raises
         ------
         AttributeError
             If delete_tar is not defined for database style.
         """
         raise AttributeError('delete_tar not defined for Database style')
-    
+
     def copy_records(self, dest, record_style=None, records=None, includetar=True, overwrite=False):
         """
         Copies records from the current database to another database.
         
         Parameters
         ----------
         dest :  Database
@@ -422,49 +417,49 @@
         overwrite : bool, optional
             If False (default) only new records and tars will be copied.
             If True, all existing content will be updated.
         """
         if record_style is None and records is None:
             # Prompt for record_style
             record_style = self.select_record_style()
-        
+
         if record_style is not None:
             if records is not None:
                 raise ValueError('record_style and records cannot both be given')
-            
+
             # Retrieve records from self
-            records = self.get_records(style=record_style) 
-        
+            records = self.get_records(style=record_style)
+
         elif records is None:
             # Set empty list if record_style is still None and no records given
             records = []
-        
+
         print(len(records), 'records to try to copy')
-        
+
         record_count = 0
         tar_count = 0
         # Copy records
         for record in tqdm(records, 'copying records', ascii=True):
             try:
                 # Add new records
                 dest.add_record(record=record)
                 record_count += 1
             except:
                 # Update existing records
                 if overwrite:
                     dest.update_record(record=record)
                     record_count += 1
-            
+
             # Copy archives
             if includetar:
                 try:
                     # Get tar if it exists
                     tar = self.get_tar(record=record, raw=True) 
                 except:
-                    
+
                     # Get folder if it exists
                     try:
                         root_dir = self.get_folder(record=record).parent
                     except:
                         pass
                     else:
                         try:
@@ -472,30 +467,30 @@
                             dest.add_tar(record=record, root_dir=root_dir)
                             tar_count += 1
                         except:
                             # Update existing tar
                             if overwrite:
                                 dest.update_tar(record=record, root_dir=root_dir)
                                 tar_count += 1
-                    
+
                 else:
                     try:
                         # Copy tar over
                         dest.add_tar(record=record, tar=tar)
                         tar_count += 1
                     except:
                         # Update existing tar
                         if overwrite:
                             dest.update_tar(record=record, tar=tar)
                             tar_count += 1
-        
+
         print(record_count, 'records added/updated')
         if includetar:
             print(tar_count, 'tars added/updated')
-    
+
     def destroy_records(self, record_style=None, records=None):
         """
         Permanently deletes multiple records and their associated tars all at
         once.
         
         Parameters
         ----------
@@ -511,18 +506,18 @@
         if record_style is None and records is None:
             record_style = self.select_record_style()
 
         # Get records by record_style
         if record_style is not None:
             if records is not None:
                 raise ValueError('record_style and records cannot both be given')
-            
+
             # Retrieve records with errors from self
             records = self.get_records(style=record_style) 
-        
+
         elif records is None:
             # Set empty list if record_style is still None and no records given
             records = []
 
         print(f'{len(records)} records found to be destroyed')
 
         if len(records) > 0:
@@ -542,40 +537,38 @@
                     except:
                         pass
                 if self.style == 'local':
                     for record_style in record_styles:
                         cache = self.cache(record_style, refresh=True)
                 print(count, 'records successfully deleted')
 
-    
     def select_record_style(self):
         """
         Console prompt for selecting a record_style
         """
         # Build list of calculation records
         styles = recordmanager.loaded_style_names
-        
+
         # Ask for selection
         print('Select record_style:')
         for i, style in enumerate(styles):
             print(i+1, style)
         choice = screen_input(':')
         try:
             choice = int(choice)
         except:
             record_style = choice
         else:
             record_style = styles[choice-1]
         print()
-        
+
         return record_style
 
     def record_querynames(self,
                           style: str) -> list:
         """Return the list of query parameter names for a given record style"""
         return load_record(style).querynames
-    
+
     def record_querydoc(self,
                         style: str) -> str:
         """Return the description of query parameters for a given record style"""
         return load_record(style).querydoc
-
```

### Comparing `yabadaba-0.2.0/yabadaba/database/LocalDatabase.py` & `yabadaba-0.2.1/yabadaba/database/LocalDatabase.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # iprPy imports
 from ..tools import aslist, iaslist
 from . import Database
 from .. import load_record, recordmanager
 
 class LocalDatabase(Database):
-    
+
     def __init__(self, host, format='json', indent=None):
         """
         Initializes a connection to a local database of JSON/XML records
         stored in a local directory.
         
         Parameters
         ----------
@@ -36,35 +36,35 @@
             file will be indented by multiples of this value based on the
             model's element recursion.
         """
         # Make the path if needed
         host = Path(host)
         if not host.is_dir():
             host.mkdir(parents=True)
-        
+
         # Get absolute path to host
         host = host.resolve()
 
         # Pass host to Database initializer
         Database.__init__(self, host)
 
         # Set default format and indent values
         self.__format = format
         self.__indent = indent
-    
+
     @property
     def style(self):
         """str: The database style"""
         return 'local'
 
     @property
     def format(self):
         """str: The format that records are saved as: 'json' or 'xml'"""
         return self.__format
-    
+
     @property
     def indent(self):
         """int or None: The record indentation setting to use when saving records."""
         return self.__indent
 
     def cache(self, style, refresh=False, addnew=True):
         """
@@ -83,47 +83,46 @@
             appended to the stored metadata cache.  If False, then the stored
             metadata is returned as is.
         """
         recordmanager.assert_style(style)
         cachefile = Path(self.host, f'{style}.csv')
 
         if cachefile.is_file() and refresh is False:
-            
+
             # Load cache file
             cache = pd.read_csv(cachefile)
 
             def interpret(series, key):
                 """Safely convert dict and list elements from str"""
                 try:
                     assert series[key][0] in '{['
                     return ast.literal_eval(series[key])
                 except:
                     return series[key]
-            
+
             def toint(column):
                 """Convert int columns as needed"""
                 try:
                     newcolumn = column.astype(int)
                     assert np.allclose(column, newcolumn)
                 except:
                     return column
                 else:
                     return newcolumn
-                    
+
             # Interpret int, dict and list elements
             if len(cache) > 0:
                 cache = cache.apply(toint, axis=0)
                 for key in cache.keys():
                     cache[key] = cache.apply(interpret, axis=1, args=[key])
 
         else:
             # Initialize new cache
             cache = pd.DataFrame({'name':[]})
 
-        
         if addnew is True:
 
             # Compare names in the cache to file names in the directory
             cachenames = set(cache.name)
             filenames = set([fname.stem for fname in Path(self.host, style).glob(f'*.{self.format}')])
             newnames = filenames.difference(cachenames)
             deletednames = cachenames.difference(filenames)
@@ -133,28 +132,29 @@
                 newrecords = []
                 for name in newnames:
                     fname = Path(self.host, style, f'{name}.{self.format}')
                     record = load_record(style, model=fname, name=name)
                     newrecords.append(record.metadata())
                 newrecords = pd.DataFrame(newrecords)
                 cache = cache.append(newrecords, sort=False).sort_values('name')
+                #cache = pd.concat([cache, newrecords], sort=False).sort_values('name')
                 refresh = True
-            
+
             # Delete missing entries
-            if len(deletednames) > 0:                
+            if len(deletednames) > 0:
                 cache = cache[~cache.name.isin(deletednames)]
                 refresh = True
 
         # Refresh cache file
         if refresh:
             cache.to_csv(cachefile, index=False)
 
         return cache
 
-    def get_records(self, style=None, refresh_cache=False, return_df=False, **kwargs):
+    def get_records(self, style=None, return_df=False, refresh_cache=False, **kwargs):
         """
         Produces a list of all matching records in the database.
         
         Parameters
         ----------
         style : str, optional
             The record style to search.
@@ -175,32 +175,31 @@
         ------
         records : numpy.NDArray
             All records from the database matching the given parameters.
         records_df : pandas.DataFrame
             The corresponding metadata values for the records.  Only returned
             if return_df is True.
         """
-        
         # Get df
         df = self.get_records_df(style, refresh_cache=refresh_cache, **kwargs)
-        
+
         # Load only the matching records
         records = []
         if len(df) > 0:
             for name in df.name:
                 fname = Path(self.host, style, f'{name}.{self.format}')
-                records.append(recordmanager.init(style, model=fname))
-        
+                records.append(load_record(style, model=fname, database=self))
+
         records = np.array(records)
-        
+
         if return_df:
             return records, df
         else:
             return records
-    
+
     def get_records_df(self, style=None, refresh_cache=False, **kwargs):
         """
         Produces a table of metadata for matching records in the database.
         
         Parameters
         ----------
         style : str, optional
@@ -216,42 +215,42 @@
             for.
         
         Returns
         ------
         records_df : pandas.DataFrame
             The corresponding metadata values for the records.
         """
-        
+
         # Set default search parameters
         if style is None:
             style = self.select_record_style()
-        
+
         if 'name' in kwargs and kwargs['name'] is not None:
             # Load named records
             cache = []
             for name in aslist(kwargs['name']):
                 fname = Path(self.host, style, f'{name}.{self.format}')
                 if fname.exists():
-                    record = recordmanager.init(style, model=fname)
+                    record = load_record(style, model=fname)
                     cache.append(record.metadata())
-            
+
             # Build cache DataFrame
             if len(cache) == 0:
                 cache = pd.DataFrame({'name':[]})
             else:
                 cache = pd.DataFrame(cache)
 
         else:
             # Load cache file
             cache = self.cache(style, refresh=refresh_cache)
-        
+
         # Filter based on the record's pandasfilter method
         mask = load_record(style).pandasfilter(cache, **kwargs)
         df = cache[mask].reset_index(drop=True)
-        
+
         return df
 
     def get_record(self, style=None, refresh_cache=False, **kwargs):
         """
         Returns a single matching record from the database.
         
         Parameters
@@ -274,26 +273,26 @@
             The single record from the database matching the given parameters.
         
         Raises
         ------
         ValueError
             If multiple or no matching records found.
         """
-        
+
         if style is None:
             styles = recordmanager.loaded_style_names
         else:
             styles = aslist(style)
 
         # Get records
         records = []
         for style in styles:
             records.append(self.get_records(style, refresh_cache=refresh_cache, **kwargs))
-        records = np.hstack(records)        
-        
+        records = np.hstack(records)
+
         # Verify that there is only one matching record
         if len(records) == 1:
             return records[0]
         elif len(records) == 0:
             raise ValueError('No matching records found')
         else:
             raise ValueError('Multiple matching records found')
@@ -333,47 +332,47 @@
         
         Raises
         ------
         ValueError
             If style, name and/or model given with record, or a matching record
             already exists.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = load_record(style, model=model, name=name)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None or model is not None:
             raise ValueError('kwargs style, name, and model cannot be given with kwarg record')
 
         # Verify that there isn't already a record with a matching name
         style_dir = Path(self.host, record.style)
         fname = Path(style_dir, f'{record.name}.{self.format}')
         if fname.is_file():
             raise ValueError(f'Record {record.name} already exists')
-        
+
         # Make record style directory if needed
         if not style_dir.is_dir():
             style_dir.mkdir()
-        
+
         # Retrieve/build model contents
         try:
             assert build is False
             model = record.model
         except:
             model = record.build_model()
 
         # Save record
         with open(fname, 'w', encoding='UTF-8') as f:
             if self.format == 'json':
                 model.json(fp=f, indent=self.indent, ensure_ascii=False)
             elif self.format == 'xml':
                 model.xml(fp=f, indent=self.indent)
-        
+
         if verbose:
             print(f'{record} added to {self.host}')
 
         return record
 
     def update_record(self, record=None, style=None, name=None, model=None,
                       build=False, verbose=False):
@@ -411,56 +410,56 @@
         Raises
         ------
         TypeError
             If no new content is given.
         ValueError
             If style and/or name content given with record.
         """
-        
+
         # Create Record object if not given
         if record is None:
             if model is None:
                 raise TypeError('no new model given')
-            
+
             record = load_record(style, model=model, name=name)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Replace content in record object
         elif model is not None:
             record = load_record(record.style, model=model, name=record.name)
-            
+
         # Check if record already exists
         style_dir = Path(self.host, record.style)
         fname = Path(style_dir, f'{record.name}.{self.format}')
         if not fname.is_file():
             raise ValueError(f'No existing record {record.name} found')
-        
+
         # Retrieve/build model contents
         try:
             assert build is False
             model = record.model
         except:
             model = record.build_model()
 
         # Save record
         with open(fname, 'w', encoding='UTF-8') as f:
             if self.format == 'json':
                 model.json(fp=f, indent=self.indent, ensure_ascii=False)
             elif self.format == 'xml':
                 model.xml(fp=f, indent=self.indent)
-        
+
         if verbose:
             print(f'{record} updated in {self.host}')
 
         return record
-    
-    def delete_record(self, record=None, name=None, style=None, verbose=False):
+
+    def delete_record(self, record=None, style=None, name=None, verbose=False):
         """
         Permanently deletes a record from the database.
         
         Parameters
         ----------
         record : Record, optional
             The record to delete from the database.  If not given, name and/or
@@ -474,34 +473,34 @@
             value is False.
             
         Raises
         ------
         ValueError
             If style and/or name given with record.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
-        
+
          # Delete record file
         fname = Path(self.host, record.style, f'{record.name}.{self.format}')
         if fname.is_file():
             fname.unlink()
         else:
             raise ValueError(f'No existing {record.style} record {record.name} found')
 
         if verbose:
             print(f'{record} deleted from {self.host}')
 
-    def add_tar(self, record=None, name=None, style=None, tar=None,
+    def add_tar(self, record=None, style=None, name=None, tar=None,
                 root_dir=None):
         """
         Archives and stores a folder associated with a record.
         
         Parameters
         ----------
         record : Record, optional
@@ -523,61 +522,61 @@
         
         Raises
         ------
         ValueError
             If style and/or name content given with record or the record already
             has a folder or a tar archive.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Verify that record exists
         else:
             record = self.get_record(name=record.name, style=record.style)
-        
+
         # Build path to record
         dir_path = Path(self.host, record.style, record.name)
         tar_path = Path(self.host, record.style, f'{record.name}.tar.gz')
-        
+
         # Check if an archive or folder already exists
         if tar_path.exists():
             raise ValueError('Record already has an archive')
         elif dir_path.exists():
             raise ValueError('Record already has a folder')
-        
+
         # Make archive
         if tar is None:
             if root_dir is None:
                 root_dir = '.'
             target = Path(root_dir, record.name)
 
             tar = tarfile.open(tar_path, 'w:gz')
             tar.add(target, target.name)
             tar.close()
-            
+
         elif root_dir is None:
             with open(tar_path, 'wb') as f:
                 f.write(tar)
         else:
             raise ValueError('tar and root_dir cannot both be given')
-    
-    def get_tar(self, record=None, name=None, style=None, raw=False):
+
+    def get_tar(self, record=None, style=None, name=None, raw=False):
         """
         Retrives the tar archive associated with a record in the database.
         
         Parameters
         ----------
         record : Record, optional
-            The record to retrive the associated tar archive for.
+            The record to retrieve the associated tar archive for.
         name : str, optional
             The name to use in uniquely identifying the record.
         style : str, optional
             The style to use in uniquely identifying the record.
         raw : bool, optional
             If True, return the archive as raw binary content. If 
             False, return as an open tarfile. (Default is False)
@@ -589,38 +588,41 @@
             raw=True.
         
         Raises
         ------
         ValueError
             If style and/or name content given with record.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Verify that record exists
         #else:
         #    record = self.get_record(name=record.name, style=record.style)
-        
+
         # Build path to record
         tar_path = Path(self.host, record.style, record.name+'.tar.gz')
-        
+
+        tar = tarfile.open(tar_path)
+        record.tar = tar
+
         # Return content
         if raw is True:
             with open(tar_path, 'rb') as f:
                 return f.read()
         else:
-            return tarfile.open(tar_path)
+            return tar
 
-    def delete_tar(self, record=None, name=None, style=None):
+    def delete_tar(self, record=None, style=None, name=None):
         """
         Deletes a tar file from the database.
         
         Parameters
         ----------
         record : Record, optional
             The record associated with the tar archive to delete.  If not
@@ -632,35 +634,35 @@
             The style to use in uniquely identifying the record.
         
         Raises
         ------
         ValueError
             If style and/or name content given with record.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Verify that record exists
         #else:
         #    record = self.get_record(name=record.name, style=record.style)
-        
+
         # Build path to tar file
         tar_path = Path(self.host, record.style, record.name+'.tar.gz')
-        
+
         # Delete record if it exists
         if tar_path.is_file():
             tar_path.unlink()
 
-    def update_tar(self, record=None, name=None, style=None, tar=None,
+    def update_tar(self, record=None, style=None, name=None, tar=None,
                    root_dir=None):
         """
         Replaces an existing tar archive for a record with a new one.
         
         Parameters
         ----------
         record : Record, optional
@@ -676,18 +678,18 @@
             with root_dir.
         root_dir : str, optional
             Specifies the root directory for finding the directory to archive.
             The directory to archive is at <root_dir>/<name>.  (Default is to
             set root_dir to the current working directory.)  tar cannot be given
             with root_dir.
         """
-        
+
         # Delete the existing tar archive stored in the database
         self.delete_tar(record=record, name=name)
-        
+
         # Add the new tar archive
         self.add_tar(record=record, name=name, style=style, tar=tar,
                      root_dir=root_dir)
 
     def add_folder(self, record=None, name=None, style=None, filenames=None,
                    root_dir=None):
         """
@@ -714,62 +716,62 @@
         
         Raises
         ------
         ValueError
             If style and/or name content given with record or the record already
             has a folder or a tar archive.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Verify that record exists
         else:
             record = self.get_record(name=record.name, style=record.style)
-        
+
         # Build database paths
         dir_path = Path(self.host, record.style, record.name)
         tar_path = Path(self.host, record.style, f'{record.name}.tar.gz')
-        
+
         # Check if an archive or folder already exists
         if tar_path.exists():
             raise ValueError('Record already has an archive')
         elif dir_path.exists():
             raise ValueError('Record already has a folder')
-        
+
         # Copy folder
         if filenames is None:
             if root_dir is None:
                 root_dir = '.'
             source = Path(root_dir, record.name)
             shutil.copytree(source, dir_path)
-        
+
         # Copy files
         elif root_dir is None:
             dir_path.mkdir(parents=True)
             for filename in iaslist(filenames):
                 shutil.copy2(filename, Path(dir_path, Path(filename).name))
-                
+
         else:
             raise ValueError('filenames and root_dir cannot both be given')
 
-    def get_folder(self, record=None, name=None, style=None):
+    def get_folder(self, record=None, style=None, name=None):
         """
         Retrives the location of the folder associated with a record in the
         database. 
         
         Parameters
         ----------
         record : Record, optional
-            The record to retrive the associated folder location for.
+            The record to retrieve the associated folder location for.
         name : str, optional
             The name to use in uniquely identifying the record.
         style : str, optional
             The style to use in uniquely identifying the record.
         
         Returns
         -------
@@ -779,30 +781,30 @@
         Raises
         ------
         ValueError
             If style and/or name content given with record.
         NotADirectoryError
             If the record's folder doesn't exist.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Verify that record exists
         else:
             record = self.get_record(name=record.name, style=record.style)
-        
+
         # Build path to folder
         dir_path = Path(self.host, record.style, record.name)
-        
+
         # Return path
         if dir_path.exists():
             return dir_path
         else:
             raise NotADirectoryError('No folder saved for the record')
 
     def delete_folder(self, record=None, name=None, style=None):
@@ -821,35 +823,35 @@
             The style to use in uniquely identifying the record.
         
         Raises
         ------
         ValueError
             If style and/or name content given with record.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Verify that record exists
         else:
             record = self.get_record(name=record.name, style=record.style)
-        
+
         # Build path to tar file
         dir_path = Path(self.host, record.style, record.name)
-        
+
         # Delete record if it exists
         if dir_path.exists():
             shutil.rmtree(dir_path)
 
-    def update_folder(self, record=None, name=None, style=None, filenames=None,
+    def update_folder(self, record=None, style=None, name=None, filenames=None,
                       root_dir=None, clear=True):
         """
         Updates an existing folder for a record.
         
         Parameters
         ----------
         record : Record, optional
@@ -876,36 +878,36 @@
         # Check competing parameters
         if filenames is not None and root_dir is not None:
             raise ValueError('filenames and root_dir cannot both be given')
 
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
 
         # Verify that record exists
         else:
             record = self.get_record(name=record.name, style=record.style)
-        
+
         # Build database paths
         dir_path = Path(self.host, record.style, record.name)
-        
+
         # Delete existing folder
         if clear is True:
             if dir_path.exists():
                 shutil.rmtree(dir_path)
-        
+
         # Copy folder
         if filenames is None:
             if root_dir is None:
                 root_dir = '.'
             source = Path(root_dir, record.name)
             shutil.copytree(source, dir_path)
-        
+
         # Copy files
         elif root_dir is None:
             dir_path.mkdir(parents=True)
             for filename in iaslist(filenames):
-                shutil.copy2(filename, Path(dir_path, Path(filename).name))
+                shutil.copy2(filename, Path(dir_path, Path(filename).name))
```

### Comparing `yabadaba-0.2.0/yabadaba/database/MongoDatabase.py` & `yabadaba-0.2.1/yabadaba/database/MongoDatabase.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # Relative imports
 from ..tools import aslist
 from . import Database
 from .. import load_record, recordmanager
 
 class MongoDatabase(Database):
-    
+
     def __init__(self, host='localhost', port=27017, database='iprPy', **kwargs):
         """
         Initializes a connection to a Mongo database.
         
         Parameters
         ----------
         host : str
@@ -39,37 +39,37 @@
         database : str
             The name of the database in the mongo host to interact with.
             Default value is 'iprPy'
         **kwargs : dict, optional
             Any extra keyword arguments needed to initialize a
             pymongo.MongoClient object.
         """
-        
+
         # Connect to underlying class
         self.__mongodb = MongoClient(host=host, port=port, document_class=DM, **kwargs)[database]
-        
+
         # Define class host using client's host, port and database name
-        host = self.mongodb.client.address[0]
-        port =self.mongodb.client.address[1]
-        database = self.mongodb.name
+        #host = self.mongodb.client.address[0]
+        #port = self.mongodb.client.address[1]
+        #database = self.mongodb.name
         host = f'{host}:{port}.{database}'
-        
+
         # Pass host to Database initializer
         Database.__init__(self, host)
-    
+
     @property
     def style(self):
         """str: The database style"""
         return 'mongo'
 
     @property
     def mongodb(self):
         """pymongo.Database : The underlying database API object."""
         return self.__mongodb
-    
+
     def get_records(self, style=None, return_df=False, query=None, **kwargs):
         """
         Produces a list of all matching records in the database.
         
         Parameters
         ----------
         style : str, optional
@@ -97,21 +97,21 @@
             style = self.select_record_style()
 
         # Use given query
         if query is not None:
             assert len(kwargs) == 0, 'query cannot be given with kwargs'
         else:
             query = load_record(style).mongoquery(**kwargs)
-        
+
         # Query the collection to construct records
         records = []
         collection = self.mongodb[style]
         for entry in collection.find(query):
             record = load_record(style, model=entry['content'],
-                                 name=entry['name'])
+                                 name=entry['name'], database=self)
             records.append(record)
         records = np.array(records)
 
         # Build df
         if len(records) > 0:
             df = []
             for record in records:
@@ -147,15 +147,15 @@
             
         Returns
         -------
         records_df : pandas.DataFrame
             The corresponding metadata values for the records.
         """
         return self.get_records(style, query=query, return_df=True, **kwargs)[1]
-    
+
     def get_record(self, style=None, query=None, **kwargs):
         """
         Retrieves a single matching record from the database.
         
         Parameters
         ----------
         style : str, optional
@@ -173,26 +173,26 @@
             The record from the database matching the given parameters.
         
         Raises
         ------
         ValueError
             If multiple or no matching records found.
         """
-        
+
         if style is None:
             styles = recordmanager.loaded_style_names
         else:
             styles = aslist(style)
 
         # Get records
         records = []
         for style in styles:
             records.append(self.get_records(style, query=query, **kwargs))
         records = np.hstack(records)
-        
+
         # Verify that there is only one matching record
         if len(records) == 1:
             return records[0]
         elif len(records) == 0:
             raise ValueError('No matching records found')
         else:
             raise ValueError('Multiple matching records found')
@@ -223,19 +223,19 @@
             style = self.select_record_style()
 
         # Use given query
         if query is not None:
             assert len(kwargs) == 0, 'query cannot be given with kwargs'
         else:
             query = load_record(style).mongoquery(**kwargs)
-        
+
         # Query the collection to construct records
         collection = self.mongodb[style]
         count = collection.count_documents(query)
-        
+
         return count
 
     def add_record(self, record=None, style=None, name=None, model=None,
                    build=False, verbose=False):
         """
         Adds a new record to the database.
         
@@ -293,15 +293,15 @@
         except:
             model = record.build_model()
 
         # Create meta mongo entry
         entry = OrderedDict()
         entry['name'] = record.name
         entry['content'] = model
-        
+
         # Upload to mongodb
         self.mongodb[record.style].insert_one(entry)
 
         if verbose:
             print(f'{record} added to {self.host}')
 
         return record
@@ -342,47 +342,47 @@
         Raises
         ------
         TypeError
             If no new content is given.
         ValueError
             If style and/or name content given with record.
         """
-        
+
         # Create Record object if not given
         if record is None:
             if model is None:
                 raise TypeError('no new model given')
             oldrecord = self.get_record(name=name, style=style)
             record = load_record(oldrecord.style, model=model, name=oldrecord.name)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Replace model in record object
         elif model is not None:
             oldrecord = record
             record = load_record(oldrecord.style, model=model, name=oldrecord.name)
-            
+
         # Find oldrecord matching record
         else:
             oldrecord = self.get_record(name=record.name, style=record.style)
-        
+
         # Delete oldrecord
         self.delete_record(record=oldrecord)
-        
+
         # Add new record
         self.add_record(record=record, build=build)
-        
+
         if verbose:
             print(f'{record} updated in {self.host}')
 
         return record
-    
-    def delete_record(self, record=None, name=None, style=None, verbose=False):
+
+    def delete_record(self, record=None, style=None, name=None, verbose=False):
         """
         Permanently deletes a record from the database. 
         
         Parameters
         ----------
         record : Record, optional
             The record to delete from the database.  If not given, name and/or
@@ -396,38 +396,38 @@
             value is False.
 
         Raises
         ------
         ValueError
             If style and/or name content given with record.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Verify that record exists
         else:
             record = self.get_record(name=record.name, style=record.style)
 
         # Build delete query
         query = {}
         query['name'] = record.name
 
         # Delete record 
         self.mongodb[record.style].delete_one(query)
 
         if verbose:
             print(f'{record} deleted from {self.host}')
 
-    def add_tar(self, record=None, name=None, style=None, tar=None, root_dir=None):
+    def add_tar(self, record=None, style=None, name=None, tar=None, root_dir=None):
         """
         Archives and stores a folder associated with a record.
         
         Parameters
         ----------
         record : Record, optional
             The record to associate the tar archive with.  If not given, then
@@ -459,69 +459,69 @@
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
 
         # Verify that record exists
         else:
             record = self.get_record(name=record.name, style=record.style)
-        
+
         # Define mongofs
         mongofs = GridFS(self.mongodb, collection=record.style)
-        
+
         # Check if an archive already exists
         if mongofs.exists({"recordname": record.name}):
             raise ValueError('Record already has an archive')
-        
+
         if tar is None:
             if root_dir is None:
                 root_dir = Path.cwd()
-                
+
             # Make archive
             basename = Path(root_dir, record.name)
             filename = Path(root_dir, record.name + '.tar.gz')
             shutil.make_archive(basename, 'gztar', root_dir=root_dir,
                                 base_dir=record.name)
-        
+
             # Upload archive
             with open(filename, 'rb') as f:
                 tries = 0
                 while tries < 2:
-                    if True:
+                    tries += 1
+                    try:
                         mongofs.put(f, recordname=record.name)
                         break
-                    else:
-                        tries += 1
-                if tries == 2:
-                    raise ValueError('Failed to upload archive 2 times')
-        
+                    except Exception as err:
+                        if tries == 2:
+                            raise ValueError('Failed to upload archive 2 times') from err
+
             # Remove local archive copy
             filename.unlink()
-            
+
         elif root_dir is None:
             # Upload archive
             tries = 0
             while tries < 2:
-                if True:
+                tries += 1
+                try:
                     mongofs.put(tar, recordname=record.name)
                     break
-                else:
-                    tries += 1
-            if tries == 2:
-                raise ValueError('Failed to upload archive 2 times')
+                except Exception as err:
+                    if tries == 2:
+                        raise ValueError('Failed to upload archive 2 times') from err
         else:
             raise ValueError('tar and root_dir cannot both be given')
-        
-    def get_tar(self, record=None, name=None, style=None, raw=False):
+
+    def get_tar(self, record=None, style=None, name=None, raw=False):
         """
         Retrives the tar archive associated with a record in the database.
                 
         Parameters
         ----------
         record : Record, optional
-            The record to retrive the associated tar archive for.
+            The record to retrieve the associated tar archive for.
         name : str, optional
             .The name to use in uniquely identifying the record.
         style : str, optional
             .The style to use in uniquely identifying the record.
         raw : bool, optional
             If True, return the archive as raw binary content. If 
             False, return as an open tarfile. (Default is False)
@@ -533,50 +533,53 @@
             raw=True.
         
         Raises
         ------
         ValueError
             If style and/or name content given with record.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a TypeError for competing kwargs
         elif style is not None or name is not None:
             raise TypeError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Verify that record exists
-        else:
-            record = self.get_record(name=record.name, style=record.style)
-        
+        #else:
+        #    record = self.get_record(name=record.name, style=record.style)
+
         # Define mongofs
         mongofs = GridFS(self.mongodb, collection=record.style)
-        
+
         # Build query
         query = {}
         query['recordname'] = record.name
-        
+
         # Get tar
         matches = list(mongofs.find(query))
         if len(matches) == 1:
             tar = matches[0]
         elif len(matches) == 0:
             raise ValueError('No tar found for the record')
         else:
             raise ValueError('Multiple tars found for the record')
 
+        tarobj = tarfile.open(fileobj=tar)
+        record.tar = tarobj
+
         # Return content
         if raw is True:
             return tar.read()
         else:
-            return tarfile.open(fileobj=tar)
+            return tarobj
 
-    def delete_tar(self, record=None, name=None, style=None):
+    def delete_tar(self, record=None, style=None, name=None):
         """
         Deletes a tar file from the database.
         
         Parameters
         ----------
         record : Record, optional
             The record associated with the tar archive to delete.  If not
@@ -588,47 +591,47 @@
             The style to use in uniquely identifying the record.
         
         Raises
         ------
         ValueError
             If style and/or name content given with record.
         """
-        
+
         # Create Record object if not given
         if record is None:
             record = self.get_record(name=name, style=style)
-        
+
         # Issue a ValueError for competing kwargs
         elif style is not None or name is not None:
             raise ValueError('kwargs style and name cannot be given with kwarg record')
-        
+
         # Verify that record exists
         else:
             record = self.get_record(name=record.name, style=record.style)
-        
+
         # Define mongofs
         mongofs = GridFS(self.mongodb, collection=record.style)
-        
+
         # Build query
         query = {}
         query['recordname'] = record.name
-        
+
         # Get tar
         matches = list(mongofs.find(query))
         if len(matches) == 1:
             tar = matches[0]
         elif len(matches) == 0:
             raise ValueError('No tar found for the record')
         else:
             raise ValueError('Multiple tars found for the record')
-        
+
         # Delete tar
         mongofs.delete(tar._id)
-    
-    def update_tar(self, record=None, name=None, style=None, tar=None, root_dir=None):
+
+    def update_tar(self, record=None, style=None, name=None, tar=None, root_dir=None):
         """
         Replaces an existing tar archive for a record with a new one. 
         
         Parameters
         ----------
         record : Record, optional
             The record to associate the tar archive with.  If not given, then 
@@ -643,13 +646,13 @@
             with root_dir.
         root_dir : str, optional
             Specifies the root directory for finding the directory to archive.
             The directory to archive is at <root_dir>/<name>.  (Default is to
             set root_dir to the current working directory.)  tar cannot be given
             with root_dir.
         """
-        
+
         # Delete the existing tar archive stored in the database
         self.delete_tar(record=record, name=name, style=style)
-        
+
         # Add the new tar archive
-        self.add_tar(record=record, name=name, style=style, tar=tar, root_dir=root_dir)
+        self.add_tar(record=record, name=name, style=style, tar=tar, root_dir=root_dir)
```

### Comparing `yabadaba-0.2.0/yabadaba/database/__init__.py` & `yabadaba-0.2.1/yabadaba/database/__init__.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/database/load_database.py` & `yabadaba-0.2.1/yabadaba/database/load_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,25 +62,23 @@
             if len(database_names) > 0:
                 print('Select a database:')
                 for i, database in enumerate(database_names):
                     print(i+1, database)
                 choice = screen_input(':')
                 try:
                     choice = int(choice)
-                except:
+                except ValueError:
                     name = choice
                 else:
                     name = database_names[choice-1]
             else:
                 raise KeyError('No databases currently set')
         
         try:
             kwargs = settings.databases[name]
-        except:
-            raise ValueError(f'database {name} not found')
+        except KeyError as err:
+            raise KeyError(f'database {name} not found') from err
 
         style = kwargs.pop('style')
         host = kwargs.pop('host')
 
     return databasemanager.init(style, host=host, **kwargs)
-        
-
```

### Comparing `yabadaba-0.2.0/yabadaba/demo/BadRecord.py` & `yabadaba-0.2.1/yabadaba/demo/BadRecord.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/demo/FAQ.py` & `yabadaba-0.2.1/yabadaba/demo/FAQ.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/demo/FAQ.xsl` & `yabadaba-0.2.1/yabadaba/demo/FAQ.xsl`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/demo/README.rst` & `yabadaba-0.2.1/yabadaba/demo/README.rst`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/query/DateMatchQuery.py` & `yabadaba-0.2.1/yabadaba/query/DateMatchQuery.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/query/FloatMatchQuery.py` & `yabadaba-0.2.1/yabadaba/query/FloatMatchQuery.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/query/IntMatchQuery.py` & `yabadaba-0.2.1/yabadaba/query/IntMatchQuery.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/query/ListContainsQuery.py` & `yabadaba-0.2.1/yabadaba/query/ListContainsQuery.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/query/Query.py` & `yabadaba-0.2.1/yabadaba/query/Query.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/query/StrContainsQuery.py` & `yabadaba-0.2.1/yabadaba/query/StrContainsQuery.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/query/StrMatchQuery.py` & `yabadaba-0.2.1/yabadaba/query/StrMatchQuery.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/query/__init__.py` & `yabadaba-0.2.1/yabadaba/query/__init__.py`

 * *Files identical despite different names*

### Comparing `yabadaba-0.2.0/yabadaba/record/Record.py` & `yabadaba-0.2.1/yabadaba/record/Record.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # coding: utf-8
 # Standard Python libraries
 from pathlib import Path
 from importlib import resources
 from typing import Union, Optional
 import io
+from tarfile import TarFile
 
 # https://ipython.org/
 from IPython.core.display import display, HTML
 
 # https://lxml.de/
 import lxml.etree as ET
 
@@ -23,31 +24,39 @@
     Class for handling different record styles in the same fashion.  The
     base class defines the common methods and attributes.
     """
 
     def __init__(self,
                  model: Union[str, io.IOBase, DM, None] = None,
                  name: Optional[str] = None,
+                 database = None,
                  **kwargs: any):
         """
         Initializes a Record object for a given style.
         
         Parameters
         ----------
         model : str, file-like object, or DataModelDict, optional
             The contents of the record.
         name : str, optional
             The unique name to assign to the record.  If model is a file
             path, then the default record name is the file name without
             extension.
+        database : yabadaba.Database, optional
+            A default Database to associate with the Record, typically the
+            Database that the Record was obtained from.  Can allow for Record
+            methods to perform Database operations without needing to specify
+            which Database to use.
         kwargs : any
             Any record-specific attributes to assign.
         """
         self.__model = None
         self.__name = None
+        self.tar = None
+        self.database = database
 
         if model is not None:
             assert len(kwargs) == 0, f"cannot specify kwargs with model: '{kwargs.keys()}'"
             self.load_model(model, name=name)
         else:
             self.set_values(name=name, **kwargs)
 
@@ -290,15 +299,15 @@
         # Initialize the query dictionary
         querydict = {}
         querydict['$and'] = querylist = [{}]
 
         # Apply queries based on given kwargs
         for key in kwargs:
             queries[key].mongo(querylist, kwargs[key])
-        
+
         return querydict
 
     def html(self,
              render: bool = False) -> Optional[str]:
         """
         Returns an HTML representation of the object.
         
@@ -356,7 +365,94 @@
         xml = ET.fromstring(xml_content.encode('UTF-8'))
 
         # Read xsd content
         xsd = ET.fromstring(self.xsd)
 
         schema = ET.XMLSchema(xsd)
         return schema.validate(xml)
+
+    @property
+    def database(self):
+        """yabadaba.Database or None: The default Database associated with the Record"""
+        return self.__database
+
+    @database.setter
+    def database(self, value):
+        if value is None or hasattr(value, 'get_records'):
+            self.__database = value
+        else:
+            raise TypeError('database must be a yabadaba.Database or None')
+
+    @property
+    def tar(self):
+        """tarfile.TarFile: The tar archive associated with the record"""
+        # Return tarfile if set
+        if self.__tar is not None:
+            return self.__tar
+
+        # Check if database is set
+        if self.database is None:
+            raise ValueError('tar not loaded and no database set')
+
+        # Fetch tar from database, set to cache and return
+        self.tar = self.database.get_tar(record=self)
+        return self.__tar
+
+    @tar.setter
+    def tar(self, value: Optional[TarFile]):
+        if value is None or isinstance(value, TarFile):
+            self.__tar = value
+        else:
+            raise TypeError('tar must ne a TarFile or None')
+
+    def clear_tar(self):
+        """Closes and unsets the record's tar file to save memory"""
+        if self.__tar is not None:
+            self.__tar.close()
+            self.tar = None
+
+    def get_file(self,
+                 filename: Union[str, Path],
+                 localroot: Union[str, Path, None] = None):
+        """
+        Retrieves a file either locally or from the record's tar archive.
+
+        Parameters
+        ----------
+        filename : str or Path
+            The name/path for the file.  For local files, this is taken
+            relative to localroot.  For files in the tar archive, this is taken
+            relative to the tar's root directory which is always named for the
+            record, i.e., {self.name}/{filename}.
+        localroot : str, Path or None, optional
+            The local root directory that filename (if it exists) is relative
+            to.  The default value of None will use the current working
+            directory.
+        
+        Raises
+        ------
+        ValueError
+            If filename exists in the tar but is not a file.
+
+        Returns
+        -------
+        io.IOBase
+            A file-like object in binary read mode that allows for the file
+            contents to be read.
+        """
+        # Set default root path
+        if localroot is None:
+            localroot = Path.cwd()
+        else:
+            localroot = Path(localroot)
+
+        # Return local copy of file if it exists
+        localfile = Path(localroot, filename)
+        if Path(localfile).is_file():
+            return open(localfile, 'rb')
+
+        # Return file extracted from tar
+        fileio = self.tar.extractfile(f'{self.name}/{filename}')
+        if fileio is not None:
+            return fileio
+        else:
+            raise ValueError(f'{filename} exists in tar, but is not a file')
```

### Comparing `yabadaba-0.2.0/yabadaba/record/__init__.py` & `yabadaba-0.2.1/yabadaba/record/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,32 +9,38 @@
 # Relative imports
 from .Record import Record
 from ..tools import ModuleManager
 
 # Initialize ModuleManager for records
 recordmanager = ModuleManager('Record')
 
-# Define load_record 
+# Define load_record
 def load_record(style: str,
                 model: Union[str, DM, None] = None,
                 name: Optional[str] = None,
+                database = None,
                 **kwargs) -> Record:
     """
     Loads a Record subclass associated with a given record style.
 
     Parameters
     ----------
     style : str
         The record style.
     name : str, optional
         The name to give to the specific record.
     model : str, DataModelDict, optional
         Data model content to load for the given record style.
+    database : yabadaba.Database, optional
+        Allows for a default database to be associated with the record.
     **kwargs : any
         Any extra keyword parameter supported by the record style.
 
     Returns
     -------
     subclass of Record 
         A Record object for the style
     """
-    return recordmanager.init(style, model=model, name=name, **kwargs)
+    record = recordmanager.init(style, model=model, name=name, **kwargs)
+    if database is not None:
+        record.database = database
+    return record
```

### Comparing `yabadaba-0.2.0/yabadaba/tools/ModuleManager.py` & `yabadaba-0.2.1/yabadaba/tools/ModuleManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,14 +134,19 @@
         """
         Initializes an object of the given style.
 
         Parameters
         ----------
         style : str
             The style name.
-        
+        *args : any
+            Any additional position-based arguments for the subclass being
+            created.  RECOMMENDED TO USE KWARGS OVER ARGS!!!
+        **kwargs : any
+            Any additional keyword arguments for the subclass being created.
         Returns
+        -------
         Object
             The initialized object.
         """
         self.assert_style(style)
         return self.loaded_styles[style](*args, **kwargs)
```

### Comparing `yabadaba-0.2.0/yabadaba.egg-info/PKG-INFO` & `yabadaba-0.2.1/yabadaba.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: yabadaba
-Version: 0.2.0
+Version: 0.2.1
 Summary: Yay, a base database! An abstraction layer allowing for common interactions with Mongo, CDCS and local directory databases and records.
 Home-page: https://github.com/usnistgov/yabadaba
 Author: Lucas Hale
 Author-email: lucas.hale@nist.gov
 Keywords: database,mongodb,CDCS
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: LICENSE.TXT
```

### Comparing `yabadaba-0.2.0/yabadaba.egg-info/SOURCES.txt` & `yabadaba-0.2.1/yabadaba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

