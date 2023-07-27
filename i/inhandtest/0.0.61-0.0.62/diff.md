# Comparing `tmp/inhandtest-0.0.61.tar.gz` & `tmp/inhandtest-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.61.tar", last modified: Thu Jul 13 10:13:10 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.62.tar", last modified: Thu Jul 27 06:49:58 2023, max compression
```

## Comparing `inhandtest-0.0.61.tar` & `inhandtest-0.0.62.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.61/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-07-13 10:13:10.000000 inhandtest-0.0.61/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.61/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.61/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.61/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    43260 2023-07-03 08:13:32.000000 inhandtest-0.0.61/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.61/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.61/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    63709 2023-07-10 10:33:04.000000 inhandtest-0.0.61/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    26127 2023-07-05 03:02:01.000000 inhandtest-0.0.61/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.61/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3971 2023-06-16 00:48:06.000000 inhandtest-0.0.61/inhandtest/file.py
--rw-rw-rw-   0        0        0    11506 2023-07-10 10:34:36.000000 inhandtest-0.0.61/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.61/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.61/inhandtest/inmqtt.py
-drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/inrequest/
--rw-rw-rw-   0        0        0      573 2023-07-13 10:11:38.000000 inhandtest-0.0.61/inhandtest/inrequest/__init__.py
--rw-rw-rw-   0        0        0     8343 2023-07-13 10:03:57.000000 inhandtest-0.0.61/inhandtest/inrequest/console.py
--rw-rw-rw-   0        0        0    26186 2023-07-05 05:25:12.000000 inhandtest-0.0.61/inhandtest/inrequest/dm.py
--rw-rw-rw-   0        0        0     4043 2023-07-05 05:22:24.000000 inhandtest-0.0.61/inhandtest/inrequest/dn.py
--rw-rw-rw-   0        0        0    15433 2023-07-13 10:03:57.000000 inhandtest-0.0.61/inhandtest/inrequest/er_default_config.py
--rw-rw-rw-   0        0        0    16311 2023-07-13 10:10:47.000000 inhandtest-0.0.61/inhandtest/inrequest/er_device.py
--rw-rw-rw-   0        0        0     7352 2023-07-05 05:27:06.000000 inhandtest-0.0.61/inhandtest/inrequest/ics.py
--rw-rw-rw-   0        0        0    10205 2023-07-13 10:03:57.000000 inhandtest-0.0.61/inhandtest/inrequest/inrequest.py
--rw-rw-rw-   0        0        0    32013 2023-07-13 10:03:57.000000 inhandtest-0.0.61/inhandtest/inrequest/nezha.py
--rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.61/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    16027 2023-07-06 07:21:54.000000 inhandtest-0.0.61/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.61/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.61/inhandtest/ip.py
--rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.61/inhandtest/log.py
--rw-rw-rw-   0        0        0    13757 2023-06-15 05:47:54.000000 inhandtest-0.0.61/inhandtest/mail.py
--rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.61/inhandtest/notice_email.html
-drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.61/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0    67902 2023-07-10 10:29:49.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0    72695 2023-07-10 09:51:55.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     3247 2023-07-05 03:12:45.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0    11890 2023-07-05 02:55:07.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    68039 2023-07-05 01:05:37.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    86226 2023-07-05 01:05:03.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0    30656 2023-06-26 05:24:31.000000 inhandtest-0.0.61/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.61/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    35349 2023-07-13 10:03:57.000000 inhandtest-0.0.61/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    30375 2023-07-13 10:03:57.000000 inhandtest-0.0.61/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-13 10:13:10.000000 inhandtest-0.0.61/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-07-13 10:13:09.000000 inhandtest-0.0.61/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1919 2023-07-13 10:13:09.000000 inhandtest-0.0.61/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 10:13:09.000000 inhandtest-0.0.61/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-07-13 10:13:09.000000 inhandtest-0.0.61/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-13 10:13:09.000000 inhandtest-0.0.61/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.61/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 10:13:10.000000 inhandtest-0.0.61/setup.cfg
--rw-rw-rw-   0        0        0     1615 2023-07-13 10:12:28.000000 inhandtest-0.0.61/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.62/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-07-27 06:49:58.000000 inhandtest-0.0.62/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.62/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.62/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.62/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    43260 2023-07-03 08:13:32.000000 inhandtest-0.0.62/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.62/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.62/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    66544 2023-07-26 06:03:35.000000 inhandtest-0.0.62/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    26127 2023-07-05 03:02:01.000000 inhandtest-0.0.62/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.62/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     5565 2023-07-27 05:23:00.000000 inhandtest-0.0.62/inhandtest/file.py
+-rw-rw-rw-   0        0        0    12257 2023-07-14 09:49:55.000000 inhandtest-0.0.62/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.62/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.62/inhandtest/inmqtt.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/inrequest/
+-rw-rw-rw-   0        0        0      573 2023-07-13 10:11:38.000000 inhandtest-0.0.62/inhandtest/inrequest/__init__.py
+-rw-rw-rw-   0        0        0    10424 2023-07-20 10:21:59.000000 inhandtest-0.0.62/inhandtest/inrequest/console.py
+-rw-rw-rw-   0        0        0    26186 2023-07-05 05:25:12.000000 inhandtest-0.0.62/inhandtest/inrequest/dm.py
+-rw-rw-rw-   0        0        0     4043 2023-07-05 05:22:24.000000 inhandtest-0.0.62/inhandtest/inrequest/dn.py
+-rw-rw-rw-   0        0        0    14989 2023-07-24 08:32:31.000000 inhandtest-0.0.62/inhandtest/inrequest/er_default_config.py
+-rw-rw-rw-   0        0        0    37418 2023-07-27 06:47:07.000000 inhandtest-0.0.62/inhandtest/inrequest/er_device.py
+-rw-rw-rw-   0        0        0     7352 2023-07-05 05:27:06.000000 inhandtest-0.0.62/inhandtest/inrequest/ics.py
+-rw-rw-rw-   0        0        0    11175 2023-07-24 02:46:52.000000 inhandtest-0.0.62/inhandtest/inrequest/inrequest.py
+-rw-rw-rw-   0        0        0    52445 2023-07-27 01:28:14.000000 inhandtest-0.0.62/inhandtest/inrequest/nezha.py
+-rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.62/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    16027 2023-07-06 07:21:54.000000 inhandtest-0.0.62/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.62/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.62/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     1390 2023-06-15 09:39:25.000000 inhandtest-0.0.62/inhandtest/log.py
+-rw-rw-rw-   0        0        0    15229 2023-07-18 03:57:23.000000 inhandtest-0.0.62/inhandtest/mail.py
+-rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.62/inhandtest/notice_email.html
+drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.62/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0    68559 2023-07-24 09:52:03.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0    76038 2023-07-21 09:18:02.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     3247 2023-07-05 03:12:45.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0    12188 2023-07-24 09:42:03.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    68039 2023-07-05 01:05:37.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    86226 2023-07-05 01:05:03.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0    28514 2023-06-26 05:24:31.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    30656 2023-06-26 05:24:31.000000 inhandtest-0.0.62/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.62/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    35543 2023-07-27 03:55:47.000000 inhandtest-0.0.62/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    30974 2023-07-27 05:13:54.000000 inhandtest-0.0.62/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1919 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 06:49:58.000000 inhandtest-0.0.62/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      155 2023-07-24 08:29:33.000000 inhandtest-0.0.62/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 06:49:58.000000 inhandtest-0.0.62/setup.cfg
+-rw-rw-rw-   0        0        0     1625 2023-07-27 06:46:21.000000 inhandtest-0.0.62/setup.py
```

### Comparing `inhandtest-0.0.61/PKG-INFO` & `inhandtest-0.0.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.61
+Version: 0.0.62
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.61/README.md` & `inhandtest-0.0.62/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.62/inhandtest/base_page/_ig_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.62/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.62/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/base_page/base_page.py` & `inhandtest-0.0.62/inhandtest/base_page/base_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 import os.path
 from os import path
 import playwright
 from inhandtest.base_page._ig_contents_locators import IGContentsLocators
 from typing import List
 from inhandtest.exception import ModelError
-from inhandtest.tools import loop_inspector, replace_str
+from inhandtest.tools import replace_str
 from playwright.sync_api import Page, Locator, expect, TimeoutError, sync_playwright
 from inhandtest.base_page._vg710_contents_locators import VGContentsLocators
 from inhandtest.base_page._ir3XX_contents_locators import Ir3XXContentsLocators
 from inhandtest.base_page.table_tr import Table, IgTable
 from collections import Counter
 import allure
 import re
@@ -677,64 +677,88 @@
             message = self.locale.get(message) if self.locale.get(message) else message
             with self.page.expect_event('dialog') as dialog_info:
                 f()
             assert message in dialog_info.value.message, f'{self.host} assert {message} dialog error'
             logging.info(f'Device {self.host} assert dialog {message} success')
 
     @allure.step("校验tip messages")
-    def tip_messages(self, messages: str or list = None, timeout=30) -> None:
+    def tip_messages(self, messages: str or re.Pattern or list = None, timeout=30) -> None:
         """ 某些提交操作会出现文本的提示，提示在过几秒钟后会消失，对于该类消息的验证使用该方法，
             使用时需要在base_locator tip_messages 且返回字典数据
 
-        :param messages: str or list 点击后等待该tip出现 再等待tip消失，如果有多个，使用列表传入
-                            tip_messages 是支持模糊匹配
+        :param messages: str or re.Pattern  点击后等待该tip出现 再等待tip消失，
+                            messages str 是支持模糊匹配 如果有多个，使用列表传入
+                            re.compile(message)  支持正则   如果有多个，使用列表传入
+                            re.compile(message, re.IGNORECASE) 支持正则忽略大小写  如果有多个，使用列表传入
                             该项校验 页面元素必须停留时间1秒及更多时间，否则不容易检测到导致报错
         :param timeout: 校验超时时间
         :return:
         """
         if messages:
-            tip_messages = [messages] if isinstance(messages, str) else messages
+            if isinstance(messages, str):
+                tip_messages = [self.locale.get(messages)] if self.locale.get(messages) else [messages]
+            elif isinstance(messages, re.Pattern):
+                tip_messages = [messages]  # 正则表达式 时需要自己做国际化转换
+            elif isinstance(messages, list):
+                tip_messages = [self.locale.get(message) if self.locale.get(message) else message for message in messages]
+            else:
+                raise Exception("messages type error")
             for message in tip_messages:
-                message = self.locale.get(message) if self.locale.get(message) else message  # 国际化转换
-                expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_visible(timeout=timeout * 1000)
-                expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_hidden(timeout=timeout * 1000)
+                expect(self.page.get_by_text(message)).to_be_visible(timeout=timeout * 1000)
+                expect(self.page.get_by_text(message)).to_be_hidden(timeout=timeout * 1000)
                 logging.info(f'{self.host} assert tip {message} visible success')
 
     @allure.step("校验text messages")
-    def text_messages(self, messages: str or list = None, timeout=10) -> None:
+    def text_messages(self, messages: str or re.Pattern or list = None, timeout=10) -> None:
         """ 对文本内容做验证，如在输入框输入错误内容时出现的文本，该类文本会一直存在
-        :param messages: str or list 文本内容，如果有多个，使用列表传入
+        :param messages: str or re.Pattern
+                            messages str 是支持模糊匹配 如果有多个，使用列表传入
+                            re.compile(message)  支持正则   如果有多个，使用列表传入
+                            re.compile(message, re.IGNORECASE) 支持正则忽略大小写  如果有多个，使用列表传入
         :param timeout: 校验超时时间
         :return:
         """
         if messages:
-            text_messages = [messages] if isinstance(messages, str) else messages
-            text_messages = Counter(text_messages)  # 处理多个相同的文本
+            if isinstance(messages, str):
+                messages = [self.locale.get(messages)] if self.locale.get(messages) else [messages]
+            elif isinstance(messages, re.Pattern):
+                messages = [messages]    # 正则表达式 时需要自己做国际化转换
+            elif isinstance(messages, list):
+                messages = [self.locale.get(message) if self.locale.get(message) else message for message in messages]
+            else:
+                raise Exception("messages type error")
+            text_messages = Counter(messages)  # 处理多个相同的文本
             for message, count in text_messages.items():
-                message = self.locale.get(message) if self.locale.get(message) else message  # 国际化转换
                 for i_ in range(0, count):
-                    expect(self.page.get_by_text(re.compile(message, re.IGNORECASE)).nth(i_)).to_be_visible(
-                        timeout=timeout * 1000)
+                    expect(self.page.get_by_text(message).nth(i_)).to_be_visible(timeout=timeout * 1000)
                     logging.info(f'{self.host} assert text the {i_}th {message}  visible success')
 
     @allure.step("校验元素Title")
-    def title_messages(self, messages: str or list = None, timeout=10) -> None:
+    def title_messages(self, messages: str or re.Pattern or list = None, timeout=10) -> None:
         """ 对元素的属性title做内容验证，
-        :param messages: str or list 文本内容，如果有多个，使用列表传入
+        :param messages: str or re.Pattern
+                            messages str 是支持模糊匹配 如果有多个，使用列表传入
+                            re.compile(message)  支持正则   如果有多个，使用列表传入
+                            re.compile(message, re.IGNORECASE) 支持正则忽略大小写  如果有多个，使用列表传入
         :param timeout: 校验超时时间
         :return:
         """
         if messages:
-            text_messages = [messages] if isinstance(messages, str) else messages
-            text_messages = Counter(text_messages)
+            if isinstance(messages, str):
+                messages = [self.locale.get(messages)] if self.locale.get(messages) else [messages]
+            elif isinstance(messages, re.Pattern):
+                messages = [messages]  # 正则表达式 时需要自己做国际化转换
+            elif isinstance(messages, list):
+                messages = [self.locale.get(message) if self.locale.get(message) else message for message in messages]
+            else:
+                raise Exception("messages type error")
+            text_messages = Counter(messages)
             for message, count in text_messages.items():
-                message = self.locale.get(message) if self.locale.get(message) else message  # 国际化转换
                 for i_ in range(0, count):
-                    expect(self.page.get_by_title(re.compile(message, re.IGNORECASE)).nth(i_)).to_be_visible(
-                        timeout=timeout * 1000)
+                    expect(self.page.get_by_title(message).nth(i_)).to_be_visible(timeout=timeout * 1000)
                     logging.info(f'{self.host} assert title the {i_}th {message} visible success')
 
     @allure.step('设置页面翻页')
     def page_refresh(self, refresh_time: str, select_locator: Locator) -> None:
         """
         :param refresh_time: str
                         '0'|'3'|'4'|'5'|'10'|'15'|'30'|'60'|'120'|'180'|'240'|'300'|'600'|'900'|'1200'|'1800'
@@ -857,36 +881,54 @@
         """
         self.click(locator, )
         self.page.keyboard.press('Control+A')
         self.page.keyboard.press('Delete')
         self.page.keyboard.type(value)
         logging.info(f'{log_desc} monaco-editor：{value}')
 
+    def value_mapping(self, locator, value: tuple or list):
+        """ 目前只有IG產品有
+
+        :param locator:
+        :param value:
+        :return:
+        """
+        for i in range(0, locator.get('table').locator('//tbody/tr').count()):
+            self.click(locator.get('table').locator('//tbody/tr').nth(0).locator('//td[3]/a'))
+            self.click(locator.get('ok'))
+            self.page.wait_for_timeout(1000)
+        for i in range(0, len(value)):
+            self.click(locator.get('add'))
+            self.fill(locator.get('table').locator('//tbody/tr').nth(i).locator('//td[1]').locator('//input'),
+                      value[i][0])
+            self.fill(locator.get('table').locator('//tbody/tr').nth(i).locator('//td[2]').locator('//input'),
+                      value[i][1])
+            self.page.wait_for_timeout(500)
+
     def agg_in(self, locators: list, action_dict: dict) -> None:
         """封装公共的整合输入操作
                 :param locators:  列表 嵌套 长度为2的元组，元组的第一项为操作项名称， 第二项为对应的一个字典
                     [($param1, {"locator": $locator1, "type": $type1, "relation": [($param2, $value2)], "param": {$key1: $value1}}),
                     ($param2, {"locator": $locator2, "type": $type2, "relation": [($param3, $value3),……], "param": {$key2: $value2}}),
                     ($param3, {"locator": $locator2, "type": 'table_tr', "relation": [($param3, $value3),……], "param": {$key2: $value2},
                                 "columns": list, 'unique_columns': list}),]
                     $param: 操作项的名称，如 'language'|'sim'|'status'
                     $locator: 操作项的元素定位， locator or [locator,locator,...]
                     $type: 操作项的类型 text|select|select_multi|select_more|button|check|upload_file|download_file|tip_messages|text_messages|title_messages|fill_date|
-                                     multi_select|multi_check|multi_fill|table_tr|switch_button|radio_select|expand|monaco
+                                     multi_select|multi_check|multi_fill|table_tr|switch_button|radio_select|expand|monaco|value_mapping
                             select value值可以是label|Value
                             multi_select指一个参数有多个select, 对应操作项的多个locator及value用[]传入
                     "relation":[($param, $value)]: 操作项的关联项，若有多个则首个为最先操作的关联项，其中$param为关联项的名称，$value为关联项的预期值
                     "param":{$key, $value}: 参数转换，如大小写转换{"ab":"AB"} {"wan":"Wan"}等.
                 :param action_dict: 要做操作的参数名称与对应的值{$param1: $value1, $param2: $value2}
                 :return:
                 """
         relations = []
 
         def operation(param, param_locator, value):
-
             if param_locator.get('type') == 'text':
                 self.fill(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'monaco':
                 self.monaco(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'select':
                 if param_locator.get('param'):
                     value = param_locator.get('param').get(value) if param_locator.get('param').get(value) else value
@@ -986,14 +1028,16 @@
                     messages, timeout = value, 10
                     if isinstance(value, dict):
                         timeout = value.get('timeout') if value.get('timeout') else 10
                         messages = value.get('messages')
                     self.title_messages(messages, timeout)
             elif param_locator.get('type') == 'fill_date':
                 self.fill_date(param_locator.get('locator'), value)
+            elif param_locator.get('type') == 'value_mapping':
+                self.value_mapping(param_locator.get('locator'), value)
             else:
                 logging.exception(f"not support this param type {param_locator.get('type')}")
                 raise Exception(f"not support this param type {param_locator.get('type')}")
             if param_locator.get('wait_for'):
                 wait_for = [param_locator.get('wait_for')] if isinstance(param_locator.get('wait_for'),
                                                                          dict) else param_locator.get('wait_for')
                 for wait_for_ in wait_for:
@@ -1072,15 +1116,17 @@
                             value = locator.first.inner_text() if locator.count() != 0 else 'None'
                         else:
                             value = str(locator)
                     try:
                         if '${value}' in expect_.get(key):
                             expression = expect_.get(key).replace('${value}', value).replace('\n', ' ')
                         else:
-                            expression = f'"{expect_.get(key)}" == "{value}"'  # 默认使用等于判断
+                            ex_ = expect_.get(key).replace("'", "\'")
+                            value = value.replace("'", "\'")
+                            expression = f'"""{ex_}""" == """{value}"""'  # 默认使用等于判断
                         if option[1].get('param'):
                             expression = replace_str(expression, option[1].get('param'))
                         if eval(expression):
                             logging.info(f'Check {option[0]} , {expression} is success')
                         else:
                             logging.info(f'Check {option[0]} , {expression} is failed')
                             return False
```

### Comparing `inhandtest-0.0.61/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.62/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/exception.py` & `inhandtest-0.0.62/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/file.py` & `inhandtest-0.0.62/inhandtest/file.py`

 * *Files 18% similar despite different names*

```diff
@@ -112,7 +112,56 @@
         raise Exception(f'Not support this hash_type {hash_type}')
     if os.path.isfile(file_path_or_msg):
         with open(file_path_or_msg, 'rb') as f:
             obj.update(f.read())
     else:
         obj.update(file_path_or_msg.encode('utf-8'))
     return obj.hexdigest().upper()
+
+
+def create_size_file(file_path, size='48KB'):
+    """创建一个指定大小的文件，文件内容是乱码
+
+    :param file_path:  文件路径包括文件名称
+    :param size:   KB  MB  GB  TB生成指定大小文件
+    :return:
+    """
+    size, unit = int(size[:-2]), size[-2:].lower()
+    sm = {'b': 1, 'kb': 1024, 'mb': 1024 * 1024, 'gb': 1024 * 1024 * 1024, 'tb': 1024 * 1024 * 1024 * 1024}
+    size = size * sm[unit]
+    with open(file_path, 'wb') as f:
+        f.write(os.urandom(size))
+    logging.info("file create done")
+
+
+def create_file(file_path, content: str, mode='w', encoding='utf-8'):
+    """创建一个文件，将内容写入文件
+
+    :param file_path:  文件路径包括文件名称
+    :param content: 文件内容
+    :param mode:  w | a  w:覆盖写入  a:追加写入
+    :param encoding:  文件编码
+    :return:
+    """
+    if not os.path.isfile(file_path):
+        with open(file_path, 'w'):
+            pass
+    with open(file_path, mode, encoding=encoding) as f:
+        f.write(content)
+        logging.info(f"{file_path} file create and write done")
+
+
+def file_to_csv(content: dict, file_path, header=False):
+    """ 将字典内容写入csv文件
+
+    :param content: {'id': ['i1', 'i2'], 'key': ['k1', 'k2']}
+    :param file_path: './test.csv'
+    :param header: 是否写入表头
+    :return:
+    """
+    import pandas
+    df = pandas.DataFrame(content)
+    df.to_csv(file_path, index=False, header=header)
+
+
+if __name__ == '__main__':
+    create_file('./test.txt', 'test\n1234123', mode='a')
```

### Comparing `inhandtest-0.0.61/inhandtest/inmodbus.py` & `inhandtest-0.0.62/inhandtest/inmodbus.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         :param stop_bits: 停止位
         """
         self.logging = utils.create_logger("console", level=logging.DEBUG)
         try:
             if protocol.upper() == 'TCP':
                 self.master = modbus_tcp.TcpMaster(host=host, port=port)
             else:
-                self.uart = serial.Serial(host, baudrate=baud_rate, bytesize=bytesize, parity=parity, stopbits=stop_bits)
+                self.uart = serial.Serial(host, baudrate=baud_rate, bytesize=bytesize, parity=parity,
+                                          stopbits=stop_bits)
                 self.master = modbus_rtu.RtuMaster(self.uart)
             self.master.set_timeout(5.0)
             self.master.set_verbose(True)
             self.logging.info("connected")
         except modbus_tk.modbus_rtu.ModbusInvalidResponseError as err:
             logging.exception("ModbusInvalidResponseError")
             raise err
@@ -69,26 +70,27 @@
             return self.master.execute(self.slave_id, function_code, int(addr[1:]) - 1, 1)[0]
         elif function_code in [3, 4] and type_ in \
                 ['INT', 'WORD', 'DINT', 'DWORD', 'LONG', 'ULONG', 'BCD16', 'BCD32', 'FLOAT', 'DOUBLE', 'STRING']:
             if type_ == 'INT':
                 data = self.read_holding_registers(addr, function_code, 1, symbol=True)[0]
             elif type_ == 'WORD':
                 data = self.read_holding_registers(addr, function_code, 1, symbol=False)[0]
-            elif type_  == 'BCD16':
+            elif type_ == 'BCD16':
                 data = int('{:x}'.format(self.read_holding_registers(addr, function_code, 1, symbol=False)[0]))
             elif type_ == 'FLOAT':
                 data = self.read_float_data(addr, function_code)
             elif type_ in ['DINT', 'DWORD', 'BCD32']:
                 data_tuple = self.read_holding_registers(addr, function_code, 2, symbol=False)
                 if type_ == 'DINT':
                     data = self.read_not_16int_data(data_tuple, datatype=type_)
                 elif type_ == 'DWORD':
                     data = ctypes.c_uint32(self.read_not_16int_data(data_tuple, datatype='DINT')).value
                 else:
-                    data = int('{:x}'.format(ctypes.c_uint32(self.read_not_16int_data(data_tuple, datatype='DINT')).value))
+                    data = int(
+                        '{:x}'.format(ctypes.c_uint32(self.read_not_16int_data(data_tuple, datatype='DINT')).value))
             elif type_ in ['LONG', 'ULONG', 'DOUBLE']:
                 data_tuple = self.read_holding_registers(addr, function_code, 4, symbol=False)
                 print(data_tuple)
                 if type_ == 'ULONG':
                     data = ctypes.c_uint64(self.read_not_16int_data(data_tuple, datatype='LONG')).value
                 else:
                     data = self.read_not_16int_data(data_tuple, datatype=type_)
@@ -128,27 +130,27 @@
             if type_ == 'FLOAT':
                 self.write_float_data(addr, write_value)
             elif type_ == 'INT':
                 self.master.execute(self.slave_id, cst.WRITE_MULTIPLE_REGISTERS, address, output_value=[write_value],
                                     data_format=">" + (1 * "h"))
             elif type_ in ['WORD', 'BCD16']:
                 if type_ == 'BCD16':
-                    write_value = int(write_value, 16)
+                    write_value = self.bcd_to_decimal(write_value)
                 self.master.execute(self.slave_id, cst.WRITE_MULTIPLE_REGISTERS, address, output_value=[write_value])
             elif type_ in ['DINT', 'LONG', 'DOUBLE', 'DWORD', 'ULONG', 'STRING', 'BCD32']:
                 if type_ in ['DWORD', 'BCD32']:
                     if type_ == 'BCD32':
-                        write_value = int(write_value, 16)
+                        write_value = self.bcd_to_decimal(write_value)
                     value = ctypes.c_int32(write_value).value
                     type_ = 'DINT'
                 elif type_ in ['ULONG']:
                     value = ctypes.c_int64(write_value).value
                     type_ = 'LONG'
                 elif type_ == 'STRING':
-                    value = write_value.ljust(math.ceil(len(write_value)/2) * 2)
+                    value = write_value.ljust(math.ceil(len(write_value) / 2) * 2)
                 else:
                     value = write_value
                 value_list = self.write_not_int16_data(value, type_)
                 self.master.execute(self.slave_id, cst.WRITE_MULTIPLE_REGISTERS, address, output_value=value_list)
         else:
             logging.exception('This address type does not support write operations.')
             raise Exception('This address type does not support write operations.')
@@ -259,7 +261,32 @@
         value_list = []
         for val in eval_val:
             val = int(val, 16)
             # print(val)
             value_list.append(val)
         return value_list
 
+    def bcd_to_decimal(self, bcd):
+        """
+        BCD码转换为十进制
+        :param bcd: BCD码
+        :return: 十进制
+        """
+        string = ''
+        if isinstance(bcd, int):
+            bcd = str(bcd)
+        for i in bcd:
+            string += '{0:b}'.format(int(i)).zfill(4)
+        decimal = int(string, 2)
+        return decimal
+
+    def decimal_to_bcd(self, decimal):
+        """
+        十进制转换为BCD码
+        :param decimal: 十进制
+        :return: BCD码
+        """
+        bcd = 0
+        for i in range(4):
+            bcd += (decimal // 10 ** i % 10) << (i * 4)
+        return bcd
+
```

### Comparing `inhandtest-0.0.61/inhandtest/inmongodb.py` & `inhandtest-0.0.62/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/inmqtt.py` & `inhandtest-0.0.62/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/inrequest/__init__.py` & `inhandtest-0.0.62/inhandtest/inrequest/__init__.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/inrequest/console.py` & `inhandtest-0.0.62/inhandtest/inrequest/console.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 # @Author  : Pane Li
 # @File    : console.py
 """
 console
 
 """
 import logging
-
+import allure
 from inhandtest.tools import dict_in
-
 from inhandtest.exception import ResourceNotFoundError
 from inhandtest.inrequest.inrequest import InRequest
 
 
 class Console:
     __doc__ = """nezha PaaS 后台 管理"""
 
@@ -56,14 +55,34 @@
             else:
                 logging.exception(f'the user {email} not exist')
                 raise ResourceNotFoundError(f'the user {email} not exist')
         else:
             logging.exception(f'the user {email} not exist')
             raise ResourceNotFoundError(f'the user {email} not exist')
 
+    def __get_product_info(self, product: str) -> dict:
+        """ 获取产品信息
+
+        :param product:
+        :return:
+        """
+        products = self.api.send_request('/api/v1/products', 'get',
+                                         param={'name': product, 'page': 0, 'limit': 100}).json().get('result')
+        if products:
+            for product_ in products:
+                if product_.get('name') == product:
+                    return product_
+            else:
+                logging.exception(f'the product {product} not exist')
+                raise ResourceNotFoundError(f'the product {product} not exist')
+        else:
+            logging.exception(f'the product {product} not exist')
+            raise ResourceNotFoundError(f'the product {product} not exist')
+
+    @allure.step('PaaS为机构创建license')
     def create_license_to_org(self, org_email: str, licenses: dict):
         """ 创建license
 
         :param org_email: 企业邮箱
         :param licenses: license {'slug': 'star_pro', 'period': 'year', 'periodCount':1, 'number': 1}
         """
         license_prices = self.api.send_request(f'/api/v1/billing/license-types/{licenses.get("slug")}/prices', 'get',
@@ -76,22 +95,25 @@
             self.api.send_request('/api/v1/billing/licenses', 'post',
                                   body={'type': licenses.get('slug'), 'active': True, 'count': licenses.get('number'),
                                         'oid': org_info.get('_id'), 'priceId': license_price['_id']}, code=200)
         except Exception:
             logging.exception(f'licenses create fail, please check the licenses info')
             raise
 
+    @allure.step('PaaS设备操作')
     def device(self, sn: str, action='delete', **kwargs):
         """
 
         :param sn: 设备序列号
-        :param action: delete|info
+        :param action: delete|info|add
         :param kwargs:
                 org_email: 当删除时， 如果填写了org_email, 则删除该机构下的设备，如果sn 为None, 则删除该机构下所有设备
                 state: {} 当获取到info 时 可以对 state 做判断
+                name: 设备名称  当添加设备时，需要填写
+                product: 设备产品  当添加设备时，需要填写
         :return:
         """
         if action == 'delete':
             oid = self.__get_org_info(kwargs.get('org_email')).get('_id') if kwargs.get('org_email') else None
             if sn:
                 param = {'oid': oid, 'serial_number': sn, 'limit': 100, 'page': 0}
                 _id = self.api.send_request(f'/api/v1/devices', 'get', param=param).json().get('result')[0].get('_id')
@@ -109,15 +131,19 @@
                                 self.api.send_request(f'api/v1/devices/{device.get("_id")}', 'delete')
                                 logging.debug(f'device {device.get("serialNumber")} delete success')
                     logging.info(f'admin delete {kwargs.get("org_email")} org all devices success')
         elif action == 'info':
             param = {'serial_number': sn, 'limit': 100, 'page': 0}
             result = self.api.send_request(f'/api/v1/devices', 'get', param=param).json().get('result')[0]
             dict_in(result, kwargs.get('state'))
+        elif action == 'add':
+            body = {"name": kwargs.get('name'), "serialNumber": sn, "product": kwargs.get('product')}
+            self.api.send_request('/api/v1/devices', 'post', body=body)
 
+    @allure.step('PaaS用户操作')
     def user(self, email: str, action='update_password', **kwargs):
         """
 
         :param email: 用户邮箱
         :param action: update_password|delete
                     update_password:
                         password
@@ -134,14 +160,15 @@
         elif action == 'delete':
             try:
                 self.api.send_request(f'api/v1/users/{user_id}', 'delete', param={'oid': oid})
                 logging.info(f'the {email} user delete success')
             except Exception:
                 logging.exception(f'the email be used by org, can not delete')
 
+    @allure.step('PaaS机构操作')
     def org(self, org_email: str, action='create', **kwargs):
         """
 
         :param org_email:
         :param action: create
         :param kwargs:
                 password:  create
@@ -159,17 +186,33 @@
                     self.api.send_request('api/v1/orgs', 'post', body=org_info)
                     logging.debug(f'admin create {org_info.get("email")} org success')
                 else:
                     self.user(org_email, action='update_password', password=kwargs.get('password'))
                     logging.debug(f'admin update {org_info.get("email")} org success')
             except ResourceNotFoundError:
                 try:
-                    self.user(org_email, 'delete')   # 删除该用户邮箱
+                    self.user(org_email, 'delete')  # 删除该用户邮箱
                 except ResourceNotFoundError:
                     pass
                 self.api.send_request('api/v1/orgs', 'post', body=org_info)
                 logging.debug(f'admin create {org_info.get("email")} org success')
         elif action == 'delete':
             org_id = self.__get_org_info(org_email).get('_id')
             self.device(sn='', action='delete', org_email=org_email)
             self.api.send_request(f'api/v1/orgs/{org_id}', 'delete')
             logging.info(f'admin delete {org_email} org success')
+
+    @allure.step('获取产品相关信息')
+    def get_product(self, product='ER805', type_='support_function') -> dict:
+        """
+
+        :param product:
+        :param type_: support_function
+                    :return {function_id: minVersion}
+        :return:
+        """
+        _id = self.__get_product_info(product).get('_id')
+        if type_ == 'support_function':
+            functions = self.api.send_request(f'/api/v1/products/{_id}/compatibilities', 'get',
+                                              {"limit": 100, "page": 0}).json().get('result')
+            return {function.get('compatibilityId'): function.get('minVersion') for function in functions if
+                    function.get('support')}
```

### Comparing `inhandtest-0.0.61/inhandtest/inrequest/dm.py` & `inhandtest-0.0.62/inhandtest/inrequest/dm.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/inrequest/dn.py` & `inhandtest-0.0.62/inhandtest/inrequest/dn.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/inrequest/er_default_config.py` & `inhandtest-0.0.62/inhandtest/inrequest/er_default_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,28 @@
             "password": "123456",  # 必填
             "ppp_auth": "auto",
             "tunnel_auth": {
                 "enabled": False,
                 "server": "",
                 "password": ""
             }
+        },
+        "clients": {
+            "alias": "test",
+            "enabled": True,
+            "nat": True,
+            "interface": "any",
+            "server_ip": "1.1.1.1",
+            "username": "adm",
+            "password": "123456",
+            "ppp_auth": "auto",
+            "tunnel_auth": {
+                "enabled": False
+            },
+            "name": "l2tp1"
         }
     },
     "ipsec": {  # 去除uuid
         "name": "test",  # 必填
         "ike_version": "ikev1",
         "key": "123456789",  # 必填
         "remote_key": "",
@@ -525,45 +539,16 @@
             "pvid": 1,
             "vid": [
                 "all"
             ]
         }
     },
     "static_route4": {
-        "default_wan1": {
-            "destination": "0.0.0.0/0",
-            "desc": "default1",
-            "next_hop": {
-                "type": "interface",
-                "interface": "wan1",
-                "distance": 1
-            }
-        },
-        "default_cell": {
-            "destination": "0.0.0.0/0",
-            "desc": "default2",
-            "next_hop": {
-                "type": "interface",
-                "interface": "cellular1",
-                "distance": 2
-            }
-        },
-        "default_sta": {
-            "destination": "0.0.0.0/0",
-            "desc": "",
-            "next_hop": {
-                "type": "interface",
-                "interface": "wlan-sta",
-                "distance": 3
-            }
-        },
-        "default_wan2": {
-            "destination": "0.0.0.0/0",
-            "desc": "",
-            "next_hop": {
-                "type": "interface",
-                "interface": "wan2",
-                "distance": 4
-            }
+        "destination": "0.0.0.0/0",
+        "desc": "default1",
+        "next_hop": {
+            "type": "interface",
+            "interface": "wan1",
+            "distance": 60
         }
     }
 }
```

### Comparing `inhandtest-0.0.61/inhandtest/inrequest/ics.py` & `inhandtest-0.0.62/inhandtest/inrequest/ics.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/inrequest/inrequest.py` & `inhandtest-0.0.62/inhandtest/inrequest/inrequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,23 +25,27 @@
         :param username:  用户名
         :param password: 密码
         :param type_: device|iot|ics|star|iscada|iwos|dn4  区分平台和设备
         :param protocol: 协议，当前只支持http https
         :param port: 端口
         :param kwargs: 'device_model'
                         device_model: 设备型号，用于区分设备类型
+                        param_remove_none_key: True|False  是否删除param 值为None 的key， 默认为False
+                        body_remove_none_key: True|False  是否删除body 值为None 的key， 默认为False
         """
         self.protocol = protocol
         self.host = host
         self.username = username
         self.password = password
         self.headers = {}
         self.type_ = type_
         self.port = port
         self.device_model = kwargs.get('device_model').upper() if kwargs and 'device_model' in kwargs.keys() else None
+        self.__param_remove_none_key = kwargs.get('param_remove_none_key', False)
+        self.__body_remove_none_key = kwargs.get('body_remove_none_key', False)
         self.__login()
 
     def __url_pre(self, path: str):
         """host+path
 
         :param path:  请求路径
         :return:
@@ -97,35 +101,47 @@
                                          body={'username': self.username, 'password': self.password}).json()
                 self.headers['Authorization'] = 'Bearer ' + resp.get('result').get('token')
             else:
                 resp = self.send_request('v1/user/login', 'post').json()
                 self.headers['Authorization'] = 'Bearer ' + resp['results']['web_session']
         logging.info(f'{self.username} login success')
 
+    @staticmethod
+    def remove_none_values(body: dict):
+        for k, v in dict(body).items():
+            if isinstance(v, dict):
+                InRequest.remove_none_values(v)
+            elif v is None:
+                del body[k]
+        return body
+
     def send_request(self, path, method, param=None, body=None, expect=None, file_path=None,
-                     params_type='json', header=None, code=200, auth=True):
+                     params_type='json', header=None, code=200, auth=True, url=None):
         """封装http请求，根据请求方式及参数类型自动判断使用哪些参数来发送请求
 
         :param path: 请求路径
         :param method: 请求方法
         :param param: 请求中的参数,
         :param body: post请求中的body，当消息体为json时使用
         :param expect: 期望包含的结果
         :param file_path: 文件路径，用于文件上传或者下载文件
         :param params_type: 参数类型，用于post请求，参数值：form|json
         :param header: 请求头 只支持字典
         :param code: 验证返回code
         :param auth: 是否认证， 默认需要的
+        :param url: 请求地址，如果不传就是默认组装，传了就是他
         :return:
         """
         header = dict_merge(self.headers, header) if auth else header
         urllib3.disable_warnings()  # 去除https warnings提示
         method = method.upper()
         params_type = params_type.upper()
-        url = self.__url_pre(path)
+        url = self.__url_pre(path) if not url else url
+        param = self.remove_none_values(param) if self.__param_remove_none_key and param else param
+        body = self.remove_none_values(body) if self.__body_remove_none_key and body else body
         if method == 'GET':
             res = requests.get(url=url, params=param, headers=header, verify=False)
             if file_path:
                 with open(file_path, 'w', encoding='UTF-8') as f:
                     f.write(res.text)
         elif method == 'POST':
             if params_type == 'FORM':
```

### Comparing `inhandtest-0.0.61/inhandtest/inrequest/nezha.py` & `inhandtest-0.0.62/inhandtest/inrequest/nezha.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 nezha
 
 """
 import logging
 import random
 import re
 import time
-from inhandtest.exception import TimeOutError, ResourceNotFoundError
-from inhandtest.tools import generate_string, get_time_stamp, dict_in
+import allure
+from inhandtest.exception import TimeOutError, ResourceNotFoundError, UpgradeFailedError
+from inhandtest.tools import generate_string, get_time_stamp, dict_in, loop_inspector, dict_merge, time_delta
 from inhandtest.inrequest.inrequest import InRequest
 
 
 class Base:
     def __init__(self, api: InRequest, email: str, host: str):
         self.api = api
         self.host = host
@@ -25,14 +26,15 @@
     def me(self) -> dict:
         """ 获取me的各种信息 包括oid
 
         :return:
         """
         return self.api.send_request('/api/v1/users/me', method='get', param={"expand": 'org'}).json().get('result')
 
+    @allure.step("位置查询")
     def location_suggestion(self, q: str, provider, expect=None):
         """位置查询
 
         :param q: 位置
         :param provider: 服务商 baidu|google
         :param expect: 每个返回的地址都包含的字段
         :return:
@@ -42,36 +44,70 @@
         if address:
             if expect:
                 for item in address:
                     assert expect in item.get('address')
         else:
             raise ResourceNotFoundError(f'the {q} address not found')
 
+    # 递归删除字典里面的None值
+
 
 class Overview(Base):
 
     def __init__(self, api, email, host):
         super().__init__(api, email, host)
         self.__device = Device(api, email, host)
 
+    @allure.step("概览地图位置验证")
     def map(self, sn: str, expect=None):
         """对概览的地图进行验证
 
         :param sn: 设备序列号
         :param expect: 期望值  字典 {'location': {'source': 'gps'}}
         :return:
         """
         if expect:
             name = self.__device.info(sn).get('name')
             devices = self.api.send_request('/api/v1/devices/locations', method='get').json().get('result')
             for device in devices:
                 if device.get('name') == name:
-                    assert dict_in(device, expect)
+                    dict_in(device, expect)
                     break
 
+    @allure.step("概览上行链路验证")
+    def uplink_status(self, expect: dict, param: dict = None):
+        """
+
+        :param expect:  {"result":{"connected":518,"disconnected":167,"disabled":154,"exception":54}}
+        :param param:  {"org": "5f0f1e9b9d6b4e0001a3e2b0"}
+        :return:
+        """
+        self.api.send_request('/api/v1/uplinks/status', method='get', expect=expect, param=param)
+
+    @allure.step("概览上行链路列表验证")
+    def assert_uplinks_list(self, sn: str, interfaces: list, param=None):
+        """
+
+        :param sn: 当sn为空时就对整体列表做验证
+        :param interfaces:
+        :param param: 查询参数
+        :return:
+        """
+        if interfaces and sn:
+            param = dict_merge({'limit': 100, 'page': 0}, param) if param else {'limit': 100, 'page': 0}
+            result = self.api.send_request('/api/v1/uplinks', 'get', param).json().get('result')
+            _id = self.__device.info(sn).get('_id')
+            for interface in interfaces:
+                for device in result:
+                    if device.get('deviceId') == _id and device.get('name') == interface.get('name'):
+                        dict_in(device, interface)
+                        break
+                else:
+                    raise ResourceNotFoundError(f'the {sn} not found in uplinks list')
+
 
 class Device(Base):
     def __init__(self, api, email, host):
         super().__init__(api, email, host)
         self.__firmware = Firmware(api, email, host)
 
     def info(self, sn: str, type_='list') -> dict:
@@ -86,44 +122,60 @@
                                        _id: 设备_id
                                        name: 设备名字
                                        org:  {'_id': oid, 'name': 'org_name', 'email': 'org_email'}
         :param sn: 设备序列号
         :param type_:  list|detail,  分别为设备列表或者设备详情返回该设备的信息
         :return: {'sn': $sn, 'online': 1, 'iccid': '', 'imei'}
         """
-
         try:
             response = self.api.send_request('/api/v1/devices', method='get', param={'serialNumber': sn}).json()
             info = response.get('result')[0]
         except Exception:
             raise ResourceNotFoundError(f'the device {sn} not exist')
         if type_ == 'list':
             return info
         else:
             return self.api.send_request(f'/api/v1/devices/{info["_id"]}', method='get').json().get('result')
 
-    def add(self, sn: str, mac_or_imei: str) -> None:
+    @allure.step("添加设备")
+    def add(self, sn: str, mac_or_imei: str, name=None) -> None:
         """添加设备，
 
         :param sn: 设备序列号
         :param mac_or_imei: 添加设备时需要依赖设备的mac地址或者IMEI号，去生产库查询该设备是否是映翰通设备
+        :param name: 设备名字
         :return:
         """
-        validated_field = self.api.send_request(f'api/v1/serialnumber/{sn}/validate', method='post').json().get(
-            'result').get('validatedField')
         try:
-            self.info(sn)
-        except ResourceNotFoundError:
-            self.api.send_request('api/v1/devices', 'post',
-                                  body={"name": sn + str(int(time.time())), "serialNumber": sn,
-                                        'oid': self.me.get('oid'),
-                                        validated_field: mac_or_imei})
+            validated_field = self.api.send_request(f'api/v1/serialnumber/{sn}/validate', method='post').json().get(
+                'result').get('validatedField')
+        except Exception:
+            raise Exception(f'the {sn} validate failed')
+        if name is None:
+            name = sn + str(int(time.time()))
+        self.api.send_request('api/v1/devices', 'post',
+                              body={"name": name, "serialNumber": sn, 'oid': self.me.get('oid'),
+                                    validated_field: mac_or_imei})
         logging.info(f"the {sn} device add success")
 
-    def assert_state(self, sn: str, state: dict, timeout=120, interval=5, type_='list') -> None:
+    @allure.step("编辑设备")
+    def update(self, sn: str, name: str = None, description: str = None) -> None:
+        """编辑设备
+
+        :param sn: 设备序列号
+        :param name: 设备名字
+        :param description: 设备描述
+        :return:
+        """
+        _id = self.info(sn).get('_id')
+        self.api.send_request(f'/api/v1/devices/{_id}', method='put',
+                              body={'name': name, 'description': description})
+
+    @allure.step("验证设备属性")
+    def assert_state(self, sn: str, state: dict, timeout=30, interval=5, type_='list') -> None:
         """校验设备基本状态
 
         :param sn: 序列号
         :param state:
                         online: 在线|离线   True|False
                         iccid:
                         imei:
@@ -135,24 +187,25 @@
         :param timeout: 校验信息，最大超时时间
         :param interval: 校验信息，校验间隔时间
         :param type_: list|detail, 分别是列表和详情返回的具体信息
         :return: True or False
         """
         if state:
             for i in range(0, timeout, interval):
-                result = self.info(sn, type_)
                 try:
+                    result = self.info(sn, type_)
                     dict_in(result, state)
                     break
-                except AssertionError:
+                except (ResourceNotFoundError, AssertionError):
                     time.sleep(interval)
             else:
                 logging.exception(f"the {sn} state {state} check failed")
                 raise TimeOutError(f"the {sn} state {state} check failed")
 
+    @allure.step("删除设备")
     def delete(self, sn: str or list) -> None:
         """
 
         :param sn: 设备序列号，一个或多个, sn='all' 时，删除所有设备
         :return:
         """
 
@@ -172,39 +225,56 @@
                     break
                 logging.info(f'{self.email} user delete all device success')
         else:
             sn = [sn] if isinstance(sn, str) else sn
             delete([self.info(sn_).get('_id') for sn_ in sn])
             logging.info(f'{self.email} user delete {sn} device success')
 
+    @allure.step("查询设备")
+    def find_device(self, expect, param: dict) -> list:
+        """
+
+        :param expect:
+        :param param:
+        :return:
+        """
+        return self.api.send_request('/api/v1/devices', method='get', param=param, expect=expect).json().get('result')
+
+    @allure.step("设备绑定license")
     def bind_license(self, sn: list, licenses: dict):
         """ 绑定license
 
         :param sn
         :param licenses: {'slug': 'star_pro'}
         """
         licenses_ = []
+        for sn_ in sn:
+            info = self.info(sn_)
+            if info.get('licenseStatus') == 'licensed':
+                sn.remove(sn_)
         org_license = self.api.send_request('/api/v1/billing/licenses', 'get',
                                             param={'expand': 'org,device,type', 'limit': 200, 'page': 0},
                                             code=200).json().get('result')
         if org_license:
             for org in org_license:
                 if org['status'] != 'expired' and org.get('device') is None and org['type']['slug'] == licenses.get(
                         'slug'):
                     licenses_.append(org['_id'])
-        if len(licenses_) < len(sn):
-            logging.error(f'licenses not enough, please check the licenses')
-        else:
-            device_ids = [self.info(sn_).get('_id') for sn_ in sn]
-            for license_, _id in zip(licenses_, device_ids):
-                self.api.send_request(f'/api/v1/billing/licenses/{license_}/device', 'put',
-                                      body={'deviceId': _id},
-                                      code=200)
-            logging.info(f'bind license success')
+        if sn:
+            if len(licenses_) < len(sn):
+                logging.error(f'licenses not enough, please check the licenses')
+            else:
+                device_ids = [self.info(sn_).get('_id') for sn_ in sn]
+                for license_, _id in zip(licenses_, device_ids):
+                    self.api.send_request(f'/api/v1/billing/licenses/{license_}/device', 'put',
+                                          body={'deviceId': _id},
+                                          code=200)
+                logging.info(f'bind license success')
 
+    @allure.step("设备位置")
     def location(self, sn: str, type_='sync', location=None, address=None) -> None:
         """对设备位置做操作
 
         :param sn:
         :param type_: sync|manually
         :param location:  {"latitude":30.588423465204404,"longitude":104.0541738405845}  仅手动方式有用
         :param address: "成都市-武侯区-府城大道西段399号"  仅手动方式有用
@@ -212,14 +282,15 @@
         """
         if type_ == 'sync':
             body = {'pinned': False}
         else:
             body = {"pinned": True, "location": location, "address": address}
         self.api.send_request(f'/api/v1/devices/{self.info(sn).get("_id")}/location', 'put', body=body)
 
+    @allure.step("设备升级")
     def upgrade_firmware(self, sn: str or list, version: str, schedule=None) -> str:
         """ 升级任务
 
         :param sn: 设备序列号 一个或多个，他们需要都是同一个产品型号
         :param version: 版本号
         :param schedule: 计划升级时间， int， 单位分钟
         :return str， job_id
@@ -230,52 +301,70 @@
         else:
             product = self.info(sn[0]).get('product')
             _id = [self.info(sn_).get('_id') for sn_ in sn]
         firmware_id = self.__firmware.info(product, version).get('_id')
         payload = {"jobs": [{"targets": _id, "firmware": firmware_id}], "targetType": "device"}
         if schedule:
             payload["scheduledAt"] = get_time_stamp(delta=schedule, delta_type='m')
-        return self.api.send_request('/api/v1/firmwares/batch/jobs', 'post', body=payload).json().get('result')[0][
-            '_id']
+        try:
+            return self.api.send_request('/api/v1/firmwares/batch/jobs', 'post', body=payload).json().get('result')[0][
+                '_id']
+        except IndexError:
+            logging.exception(f'firmware upgrade failed')
+            raise UpgradeFailedError(f'firmware upgrade failed')
 
+    @allure.step("设备取消最近固件升级任务")
     def cancel_latest_task(self, sn: str):
         detail = self.info(sn, 'detail')
         if detail.get('firmwareUpgradeStatus'):
             if detail.get('firmwareUpgradeStatus').get('status') == 'queued':
                 self.api.send_request(
                     f'/api/v1/job/executions/{detail.get("firmwareUpgradeStatus").get("jobExecutionId")}/cancel',
                     'put')
 
+    @allure.step("设备下发实时命令")
+    def commands_online(self, sn: str or list, method='nezha_reboot'):
+        """
+
+        :param sn:
+        :param method: nezha_reboot|nezha_restore_to_defaults
+        :return:
+        """
+        sn = [sn] if isinstance(sn, str) else sn
+        ids = [self.info(sn_).get('_id') for sn_ in sn]
+        body = {"deviceIds": ids, "method": method}
+        self.api.send_request('/api/v1/devices/bulk-invoke-methods', 'post', body=body, expect={'result': 'ok'})
+
+    @allure.step("在线下载日志")
+    def download_log_online(self, sn: str, type_='diagnostic'):
+        """
+
+        :param sn:
+        :param type_:diagnostic|syslog
+        :return:
+        """
+        _id = self.info(sn).get('_id')
+        if type_ == 'diagnostic':
+            host = 'https://nezha-demo-device-files.s3.cn-northwest-1.amazonaws.com.cn'
+        else:
+            host = 'https://nezha-demo-tmp-files.s3.cn-northwest-1.amazonaws.com.cn'
+        self.api.send_request(f'/api/v1/devices/{_id}/logs/download', 'get', {'type': type_},
+                              expect=f'"downloadUrl":"{host}/uploads/{_id}')
+
+    @allure.step("设备蜂窝历史数据")
     def assert_cellular_history(self, sn: str, state, delta_day=-1, data_interval=None):
         """
 
         :param sn:
         :param state:
         :param delta_day: 查询开始时间的起点， 默认晚一天时间
         :param data_interval: 当查询的时间越长时，返回的数据会少，防止页面在渲染时卡顿，所以返回的数据间隔增大，可以对间隔做判断， 单位秒
         :return:
         """
         time.sleep(2)
-
-        def time_reduction(time_list, delta):
-            """
-            校验数据点时间差
-            :param time_list: list of timestamp
-            :param delta: int
-            :return:
-            """
-            tmp = []
-            for each in time_list:
-                each = time.strptime(each, "%Y-%m-%dT%H:%M:%SZ")
-                tmp.append(int(time.mktime(each)))
-            t0 = tmp[0]
-            for i in tmp[1:]:
-                assert abs(t0 - i) == delta
-                t0 = i
-
         payload = {
             "after": get_time_stamp(delta=delta_day, delta_type='d', time_format='%Y-%m-%dT16:00:00.000Z'),
             "before": get_time_stamp(time_format='%Y-%m-%dT16:00:00.000Z')
         }
         resp = self.api.send_request(f'/api/v1/devices/{self.info(sn).get("_id")}/signal', 'get',
                                      param=payload, code=200).json().get('result').get('series')
         fields = resp[0]['fields']
@@ -299,17 +388,42 @@
                         assert temp in state, '查询结果不对'
             assert len(cellular_state) == len(state), '查询结果不对'
         if data_interval is not None:
             cellular_type = []
             for each_type in resp:
                 cellular_type.append(each_type['type'])
                 timestamp_ls = [i[0] for i in each_type['data']]
-                time_reduction(timestamp_ls, delta=data_interval)
+                time_delta(timestamp_ls, delta=data_interval)
             assert len(cellular_type) == len(set(cellular_type)), '蜂窝历史返回数据不对'
 
+    @allure.step("设备上线链路数据")
+    def assert_uplink_history(self, sn: str, name: str, param: dict = None, value: str or list = None,
+                              interval: int = None):
+        """
+
+        :param sn: 序列号
+        :param name: 上行链路接口名称 wan  cellular
+        :param param: {'name': 'cellular1', 'after': '2023-07-24T16:00:00.000Z'}
+        :param value: 期望返回的值，
+        :param interval: 期望返回的数据间隔， 单位秒
+        :return:
+        """
+        _id = self.info(sn).get('_id')
+        param = {'name': name} if param is None else dict_merge({'name': name}, param)
+        resp = self.api.send_request(f'/api/v1/devices/{_id}/uplinks/perf-trend', 'get', param=param)
+        if interval:
+            timestamp_ls = [i[0] for i in resp.json().get('result').get('series')[0].get('values')]
+            time_delta(timestamp_ls, delta=interval)
+        if isinstance(value, str):
+            assert value in resp.text, '查询结果不对'
+        elif isinstance(value, list):
+            for i in value:
+                assert i in resp.text, '查询结果不对'
+
+    @allure.step("设备流量数据")
     def assert_traffic(self, sn: str, date_='hourly', type_='overview', expect=None, **kwargs):
         """
 
         :param sn: 设备序列号
         :param date_: hourly|daily|monthly
         :param expect: 期望返回的内容
         :param type_: overview|detail
@@ -332,22 +446,215 @@
         if type_ == 'overview':
             self.api.send_request(f'/api/v1/devices/{self.info(sn).get("_id")}/datausage-{date_}/overview', 'get',
                                   param=param, expect=expect, )
         else:
             self.api.send_request(f'/api/v1/devices/{self.info(sn).get("_id")}/datausage-{date_}', 'get',
                                   param=param, expect=expect, )
 
+    @allure.step("设备在线事件")
+    @loop_inspector('device_online_event', timeout=20, interval=4)
+    def assert_online_event(self, sn: str, time_from=get_time_stamp('', -1, 'd', '%Y-%m-%dT16:00:00Z'),
+                            time_to=get_time_stamp('', 0, 'd', '%Y-%m-%dT16:00:00Z'), **kwargs):
+        """ 对在线图和在线统计表做验证
+
+        :param sn: 设备序列号
+        :param time_from: 查询开始时间
+        :param time_to: 查询结束时间
+        :param kwargs:
+            online: int 表示在线几次
+            offline: int 表示离线几次
+            event： list or dict {timestamp: "2023-06-14T16:00:00Z", online: false} 查询有该事件，多个使用列表传入
+        :return:
+        """
+        _id = self.info(sn).get('_id')
+        # 去除首尾两条记录，是时间戳划线时会自动补齐
+        online_statis = self.api.send_request(f'/api/v1/devices/{_id}/online-events-chart/statistics', 'get',
+                                              {'from': time_from, 'to': time_to}).json().get('result').get('list')[1:-1]
+        online_event = self.api.send_request(f'/api/v1/devices/{_id}/online-events-list', 'get',
+                                             {'from': time_from, 'to': time_to, 'limit': 100,
+                                              'page': 0}).json().get('result')
+        if kwargs.get('online'):
+            if not (len(list(filter(lambda x: x.get('online'), online_statis))) == len(
+                    list(filter(lambda x: x.get('eventType') == 'connected', online_event))) == kwargs.get('online')):
+                return False
+        if kwargs.get('offline'):
+            if not (len(list(filter(lambda x: not x.get('online'), online_statis))) == len(
+                    list(filter(lambda x: x.get('eventType') == 'disconnected', online_event))) == kwargs.get(
+                'offline')):
+                return False
+        if kwargs.get('event'):
+            events = [kwargs.get('event')] if isinstance(kwargs.get('event'), dict) else kwargs.get('event')
+            for event in events:
+                if event not in online_statis:
+                    return False
+                for _ in online_event:
+                    if event.get('timestamp') == _.get('timestamp'):
+                        if event.get('online') and _.get('eventType') == 'connected':
+                            break
+                        if (not event.get('online')) and _.get('eventType') == 'disconnected':
+                            break
+                else:
+                    return False
+
+    @allure.step("上行链路列表验证")
+    def assert_uplinks_list(self, sn: str, interfaces: list):
+        """
+
+        :param sn:
+        :param interfaces:
+        :return:
+        """
+        if interfaces:
+            _id = self.info(sn).get('_id')
+            result = self.api.send_request(f'/api/v1/devices/{_id}/uplinks', 'get', ).json().get('result')
+            for interface in interfaces:
+                for device in result:
+                    if device.get('name') == interface.get('name'):
+                        dict_in(device, interface)
+                        break
+                else:
+                    raise ResourceNotFoundError(f'the {sn} not found in uplinks list')
+
+    @allure.step("获取设备interface")
+    def get_interface(self, sn: str):
+        """
+
+        :param sn:
+        :return:
+        """
+        _id = self.info(sn).get('_id')
+        try:
+            self.api.send_request(f'/api/v1/devices/{_id}/interfaces/refresh', 'post')
+        except Exception as e:
+            logging.exception(e)
+            raise e
+
+    @allure.step("验证设备interface")
+    def assert_interface(self, sn: str, publish_info: dict):
+        """只验证设备interface 名称以及状态
+
+        :param sn:
+        :param publish_info:
+        :return:
+        """
+        _id = self.info(sn).get('_id')
+        interfaces = self.api.send_request(f'/api/v1/devices/{_id}/interfaces', 'get').json().get('result')
+
+        def switch_payload(payload: dict):
+            for key, value in payload.items():
+                if key == 'wifiSta':
+                    payload[key] = {'name': value.get('name'), 'state': value.get('status'),
+                                    'priority': value.get('priority')}
+                elif 'cellular' in key:
+                    new_v = [{'name': v_.get('name'), 'card': v_.get('card'), 'state': v_.get('status'),
+                              'priority': v_.get('priority')} for v_ in value]
+                    payload[key] = new_v
+                else:
+                    new_v = [{'name': v_.get('name'), 'state': v_.get('status'), 'priority': v_.get('priority')} for v_
+                             in value]
+                    payload[key] = new_v
+            return payload
+
+        if not publish_info:
+            assert not interfaces, "设备interface不为空"
+        else:
+            assert switch_payload(interfaces) == switch_payload(publish_info), '设备interface不一致'
+
+    @allure.step("下载批量导入模板")
+    def download_import_model(self, locale='en'):
+        """
+
+        :param locale: en or zh
+        :return:
+        """
+        param = {'local': 'us_EN'} if locale == 'en' else {'local': 'zh_CN'}
+        self.api.send_request('/api/v1/devices/template/download', 'get', param)
+
+    @allure.step("批量导入设备")
+    def import_devices(self, file_path) -> str:
+        """
+
+        :param file_path:
+        :return:
+        """
+        # 文件内容校验
+        try:
+            _id = self.api.send_request('api/v1/devices/imports', 'post', params_type='form',
+                                        file_path=file_path).json().get('result')
+            self.api.send_request(f'api/v1/devices/imports/{_id}', 'post', )
+            return _id
+        except Exception as e:
+            logging.exception(e)
+            raise e
+
+    @allure.step("导出设备")
+    def export_devices(self, param) -> str:
+        """
+
+        :param param:
+        :return:
+        """
+        return self.api.send_request('api/v1/devices/export', 'get', param).content.decode('UTF-8-sig')
+
+    @allure.step("批量导入设备任务状态查询")
+    @loop_inspector('import devices', timeout=10, interval=2)
+    def assert_import_devices_status(self, _id: str, expect: dict):
+        """
+
+        :param _id: 批量导入任务id
+        :param expect: 期望结果
+        :return: AssertionError
+        """
+        result = self.api.send_request('/api/v1/devices/imports?limit=100&page=0', 'get').json().get('result')
+        for i_ in result:
+            if i_.get('_id') == _id:
+                try:
+                    dict_in(i_, expect)
+                    return True
+                except AssertionError:
+                    return False
+
+    @allure.step("设备拥有功能校验")
+    def function_validate(self, sn: str, function: dict):
+        """
+
+        :param sn:
+        :param function: {'nezha_device_config': True, 'nezha_cellular_signal': False}
+        :return:
+        """
+        if function:
+            _id = self.info(sn).get('_id')
+            compatibilities = list(function.keys())
+            body = {"ids": [_id], "compatibilities": compatibilities, "type": "device"}
+            result = self.api.send_request(f'/api/v1/product-compatibilities/bulk-validate', 'post',
+                                           body=body).json().get('result')[0]
+            contain_ = {key: {"support": value} for key, value in function.items()}
+            dict_in(result, {"compatibilities": contain_})
+
+    @allure.step("设备上行链路历史校验")
+    def assert_uplink_history(self, sn: str, expect: dict, param=None):
+        """
+
+        :param sn:
+        :param expect: {'uplinkHistory': [{'timestamp': 1621574400000, 'uplink': 0.0}]}
+        :param param: {'from': 1621574400000, 'to': 1621574400000, 'interval': 86400000}
+        :return:
+        """
+        _id = self.info(sn).get('_id')
+        self.api.send_request(f'/api/v1/devices/{_id}/uplinks/perf-trend', 'get', param, expect=expect)
+
 
 class Config(Base):
 
     def __init__(self, api, email, host):
         super().__init__(api, email, host)
         self.__device = Device(api, email, host)
         self.__group = Group(api, email, host)
 
+    @allure.step("下发配置")
     def send(self, sn: str, payload: dict, commit=True) -> dict:
         """下发设备配置
 
         :param sn: 设备序列号
         :param commit: 是否提交, 在云端可以保存配置，默认是提交
         :param payload: 配置内容，当配置中的key是随机id时， 可使用$id，下发时会自动替换成随机id
         :return:
@@ -378,14 +685,15 @@
         assert resp == {'result': 'ok'}, 'save config failed'
         if commit:
             resp = self.api.send_request('/api/v1/config/commit', 'post', header=header).json()
             assert resp == {'result': 'ok'}, 'commit config failed'
             logging.info(f'the device {sn} config commit success')
         return payload
 
+    @allure.step("获取配置")
     def get(self, sn: str, expect: dict, type_='actual') -> dict or None:
         """获取校验备配置
 
         :param sn: 设备序列号
         :param expect: 配置内容，完整的配置路径，如{'lan': {'type': 'dhcp'}}
         :param type_: actual 实际设备上传的配置
                       group 设备所在组的配置
@@ -402,25 +710,27 @@
         if expect is not None:
             self.api.send_request(f'/api/v1/devices/{self.__device.info(sn).get("_id")}/config', 'get',
                                   expect=expect)
         else:
             return self.api.send_request(f'/api/v1/devices/{self.__device.info(sn).get("_id")}/config',
                                          'get').json().get('result').get(type_)
 
+    @allure.step("清除配置")
     def clear_config(self, sn: str):
         """清除设备配置
 
         :param sn:
         :return:
         """
         self.api.send_request(f'/api/v1/config/layer/device/{self.__device.info(sn).get("_id")}', 'delete',
                               expect={
                                   "result": 'ok'})
         self.get(sn, expect={}, type_='individual')
 
+    @allure.step("复制配置")
     def copy_config(self, source_sn: str, target_sns: list = None, target_group: list = None,
                     target_group_id: list = None):
         """清除设备配置
 
         :param source_sn: 源设备sn
         :param target_sns: 目标设备sn
         :param target_group: 目标分组名称
@@ -437,29 +747,71 @@
             body = {"sourceDeviceId": self.__device.info(source_sn).get("_id"),
                     "targetGroupIds": target_group_id}
             self.api.send_request(f'/api/v1/config/layer/bulk-copy', 'post', body=body, expect={"result": 'ok'})
 
 
 class Org(Base):
 
-    def org_info(self, name, _id=None, level=None) -> dict:
+    def org_info(self, name=None, **kwargs) -> dict:
+        """
+        获取组织信息
+        :param name: 根据组织名称返回信息
+        :param kwargs:
+               如果有_id: 就直接返回该组织的信息
+               如果有org_admin: 就返回该组织的管理员信息
+        :return:
+        """
+        _id = org_admin = None
+        if kwargs.get('_id'):
+            _id = kwargs.get('_id')
+        if kwargs.get('org_admin'):
+            org_admin = True
         for i in range(0, 20):  # 20次查询，如果组织数量超过100，就需要多次查询
             orgs = self.api.send_request('/api/v1/orgs', 'get', param={'depth': 5, 'limit': 100, 'page': i}).json()
             for org in orgs.get('result'):
-                if level == 1 and org.get('level') == 1:
-                    return org
-                elif level:
-                    if (org.get('name') == name or org.get('_id') == _id) and org.get('level') == level:
+                if _id:
+                    if org.get('_id') == _id:
+                        return org
+                elif org_admin:
+                    if org.get('level') == 1:
                         return org
                 else:
-                    if org.get('name') == name or org.get('_id') == _id:
+                    if org.get('name') == name:
                         return org
             if len(orgs.get('result')) <= 100:
                 raise ResourceNotFoundError(f'org not found')
 
+    def role_info(self, type_='admin') -> dict:
+        """
+        获取角色信息
+        :param type_: admin|orgAdmin|device_manager|readonly
+        :return:
+        """
+        roles = self.api.send_request('/api/v1/roles', 'get', param={'app': 'nezha', 'sort': 'index,desc'}).json()
+        for role in roles.get('result'):
+            if role.get('name') == type_:
+                return role
+        else:
+            raise ResourceNotFoundError(f'role not found')
+
+    def user_info(self, email: str) -> dict:
+        """
+        获取用户信息
+        :param email:
+        :return:
+        """
+        users = self.api.send_request('/api/v1/users', 'get',
+                                      param={'email': email, 'limit': 100, 'page': 0, 'expand': 'roles,mfa,org'}).json()
+        for user in users.get('result'):
+            if user.get('email') == email:
+                return user
+        else:
+            raise ResourceNotFoundError(f'user not found')
+
+    @allure.step("SaaS创建组织机构")
     def create(self, name: str, parent_name: str = None, level=2, email='', phone='', **kwargs) -> str:
         """创建组织, 创建2级组织时，parent_name和parent_id可以不传
 
         :param name: 组织名称 (在实现自动化时可让名称唯一，来实现创建组织的唯一性)
         :param parent_name: 父组织名称，如果组织名称唯一，可以传入，如果不唯一就拿第一个创建
         :param level: 组织层级，2 二级组织，3 三级组织 4 四级组织 5 五级组织
         :param email: 组织邮箱
@@ -467,59 +819,148 @@
         :param kwargs: 组织信息
                parent_id: 父组织id，唯一id，传入它时可以不用传入parent_name
                description: 组织描述
                force: 是否强制创建，如果组织已存在，是否强制创建
         :return: 组织id
         """
         if level in (2, 3, 4, 5):
-            parent_level = level - 1
-            parent_id = self.org_info(parent_name, kwargs.get('parent_id'), level=parent_level).get('_id')
+            org_admin = True if level - 1 == 1 else False
+            parent_id = self.org_info(name=parent_name, _id=kwargs.get('parent_id'), org_admin=org_admin).get('_id')
             body = {'name': name, 'parent': parent_id, 'phone': phone, 'email': email,
                     'description': kwargs.get('description')}
             logging.info(f'create org {name} success')
             return self.api.send_request('/api/v1/orgs', 'post', body=body).json().get('result').get('_id')
         else:
             raise ValueError('level must be in (2, 3, 4, 5)')
 
+    @allure.step("SaaS删除组织机构")
     def delete(self, name: str, _id=None, ):
         """删除组织, 不能删除一级组织
 
         :param name: 组织名称, _id 为None时，使用名称删除，搜索到名称一致的组织就全部删除
         :param _id: 组织id, 使用id删除，精确删除
         :return:
         """
-        id_ = self.org_info(name, _id).get('_id')
+        id_ = self.org_info(name=name, _id=_id).get('_id')
         self.api.send_request(f'/api/v1/orgs/{id_}', 'delete')
         logging.info(f'delete org success')
 
+    @allure.step("SaaS添加用户")
+    def add_user(self, email: str, org_name=None, role='admin', type_='internal', **kwargs):
+        """
+
+        :param email: 用户邮箱
+        :param org_name: 添加组织的名称
+        :param role: admin|orgAdmin|device_manager|readonly， 只有加入到一级组织时，才可以设置admin角色
+        :param type_: internal 内部用户，external 外部用户，invite 邀请用户, invite_link 获取邀请链接用户
+        :param kwargs:
+               name: 用户名称,  internal，invite 用户必填
+               password: 密码，internal，invite 用户必填
+               org_id: 组织机构id
+               org_admin: True 一级组织管理员，False 级组织管理员
+               reset_invite_link, 重置邀请链接 默认False
+        :return:
+        """
+        org_id = self.org_info(name=org_name, _id=kwargs.get('org_id'), org_admin=kwargs.get('org_admin', False)).get(
+            '_id')
+        role_id = self.role_info(role).get('_id')
+        if type_ == 'internal':
+            body = {'email': email, 'oid': org_id, 'roleId': role_id, 'type': type_, 'name': kwargs.get('name'),
+                    'password': kwargs.get('password')}
+            self.api.send_request('/api/v1/users', 'post', body=body)
+        elif type_ == 'external':
+            body = {'email': email, 'oid': org_id, 'roleId': role_id, 'type': type_, 'app': 'nezha'}
+            self.api.send_request('/api/v1/users/invite', 'post', body=body)  # 邀请外部用户， 只发出了邀请邮件
+        else:
+            body = {'oid': org_id, 'roleId': role_id}
+            url = self.api.send_request('/api/v1/users/invitations', 'post', body=body).json().get('result').get('url')
+            if kwargs.get('reset_invite_link'):
+                self.api.send_request(f'/api/v1/users/invitations/reset', 'put', body=body)
+            self.api.send_request(None, 'post',
+                                  body={'email': email, 'name': kwargs.get('name'), 'password': kwargs.get('password')},
+                                  auth=False, url=url + '/register')
+
+    @allure.step("SaaS外部用户重发邀请邮件")
+    def resend_external(self, email: str):
+        """
+
+        :param email:
+        :return:
+        """
+        _user_id = self.user_info(email).get('_id')
+        self.api.send_request(f'/api/v1/users/{_user_id}/resend-invite', 'get', param={'app': 'nezha'})
+
+    @allure.step("SaaS锁定用户")
+    def lock_user(self, email: str):
+        """
+
+        :param email:
+        :return:
+        """
+        _user_id = self.user_info(email).get('_id')
+        self.api.send_request(f'/api/v1/users/{_user_id}/lock', 'put')
+
+    @allure.step("SaaS解锁用户")
+    def unlock_user(self, email: str):
+        """
+
+        :param email:
+        :return:
+        """
+        _user_id = self.user_info(email).get('_id')
+        self.api.send_request(f'/api/v1/users/{_user_id}/unlock', 'put')
+
+    @allure.step("SaaS删除用户")
+    def delete_user(self, email: str or list):
+        """
+
+        :param email:
+        :return:
+        """
+        users = [self.user_info(email).get('_id')] if isinstance(email, str) else [self.user_info(e).get('_id') for e
+                                                                                   in email]
+
+        self.api.send_request(f'/api/v1/users/remove', 'post', body={"resourceIds": users})
+
+    @allure.step("SaaS更新用户属性")
     def update_user(self, email: str, **kwargs):
         """更新用户
 
         :param email: 用户邮箱
         :param kwargs:
                password: 密码
+               name: 用户名称
+               role: admin|orgAdmin|device_manager|readonly
+               org_name:
+               org_id:
+               org_admin:
         :return:
         """
-        users = self.api.send_request('api/v1/users', 'get',
-                                      param={'email': email, 'limit': 20, 'expand': 'roles,mfa,org'}).json().get(
-            'result')
-        if users:
-            if kwargs.get('password'):
-                for user in users:
-                    if email == user.get('email'):
-                        self.api.send_request(f'api/v1/users/{user.get("_id")}/password', 'put',
-                                              body={'password': kwargs.get('password')})
-                        logging.info(f'the {email} user update password success')
-                        if self.email == email:
-                            self.api = InRequest(self.host, email, kwargs.get('password'), 'star')  # 重新登录
-                        break
-                else:
-                    logging.warning(f'the {email} user not exist')
-        else:
-            logging.warning(f'the {email} user not exist')
+        _user = self.user_info(email)
+        if kwargs.get('password'):
+            self.api.send_request(f'api/v1/users/{_user.get("_id")}/password', 'put',
+                                  body={'password': kwargs.get('password')})
+        logging.info(f'the {email} user update password success')
+        if self.email == email:
+            self.api = InRequest(self.host, email, kwargs.get('password'), 'star')  # 重新登录
+        update_info = {}
+        if kwargs.get('name'):
+            if not _user.get('collaborator'):
+                update_info['name'] = kwargs.get('name')
+                update_info['type'] = 'internal'
+            else:
+                update_info['type'] = 'external'
+        if kwargs.get('role'):
+            update_info['roleId'] = self.role_info(kwargs.get('role')).get('_id')
+        if kwargs.get('org_name') or kwargs.get('org_id') or kwargs.get('org_level'):
+            org_id = self.org_info(name=kwargs.get('org_name'), _id=kwargs.get('org_id'),
+                                   org_admin=kwargs.get('org_admin', False)).get('_id')
+            update_info['oid'] = org_id
+        if update_info:
+            self.api.send_request(f'/api/v1/users/{_user.get("_id")}', 'put', body=update_info)
 
 
 class Group(Base):
     def __init__(self, api, email, host):
         super().__init__(api, email, host)
         self.__org = Org(api, email, host)
         self.__device = Device(api, email, host)
@@ -529,30 +970,33 @@
             groups = self.api.send_request('/api/v1/devicegroups', 'get', param={'page': i, 'limit': 100}).json()
             for group in groups.get('result'):
                 if group.get('name') == name or group.get('_id') == _id:
                     return group
             if len(groups.get('result')) <= 100:
                 raise ResourceNotFoundError(f'group not found')
 
-    def create(self, name: str, product: str, firmware: str, org_name: str, org_id=None) -> str:
+    @allure.step("SaaS创建分组")
+    def create(self, name: str, product: str, firmware: str, org_name: str, org_id=None, org_admin=False) -> str:
         """创建分组
 
         :param name: 分组名称(在实现自动化时可让名称唯一，来实现创建分组的唯一性)
         :param product: 产品名称
         :param firmware: 固件版本
         :param org_name: 所属组织名称
         :param org_id: 组织id，唯一id，传入它时可以不用传入org_name
+        :param org_admin: 是否为组织管理员
         :return: 组织id
         """
-        org_id = org_id if org_id else self.__org.org_info(org_name).get('_id')
+        org_id = org_id if org_id else self.__org.org_info(name=org_name, org_id=org_id, org_admin=org_admin).get('_id')
         body = {"name": name, "product": product, "firmware": firmware, "oid": org_id}
         result = self.api.send_request('/api/v1/devicegroups', 'post', body=body).json()
         logging.info(f'create group {name} success')
         return result.get('result').get('_id')
 
+    @allure.step("SaaS删除分组")
     def delete(self, name: str or list, _id: str or list = None, ):
         """删除分组
 
         :param name: 分组名称, _id 为None时，使用名称删除，搜索到名称一致的分组只删除第一个
         :param _id: 分组id, 使用id删除，精确删除
         :return:
         """
@@ -565,14 +1009,15 @@
                     _id = [self.info(name=name).get('_id')]
                 else:
                     _id = [self.info(group_name).get('_id') for group_name in name]
         if _id:
             self.api.send_request('/api/v1/devicegroups/remove', 'post', body={'ids': _id})
         logging.info(f'delete groups success')
 
+    @allure.step("SaaS分组移入或移出设备")
     def move(self, sn: list, group_name: str, group_id: str = None, type_='in'):
         """移动设备到分组
 
         :param sn: 设备sn列表
         :param group_name: 分组名称
         :param group_id: 分组id 二选一, 传入id时，不用传入group_name
         :param type_: 移动类型，in: 移入分组， out: 移出分组
@@ -584,14 +1029,15 @@
                      in [self.__device.info(sn_) for sn_ in sn]]
         else:
             items = [{"deviceId": info.get('_id'), 'oid': group.get('oid')} for info in
                      [self.__device.info(sn_) for sn_ in sn]]
         self.api.send_request('/api/v1/devices/move', 'put', body={'items': items})
         logging.info(f'move device {sn} {type_} group success')
 
+    @allure.step("SaaS分组获取配置")
     def get_config(self, group_name: str, expect: dict, type_='actual', group_id: str = None) -> dict or None:
         """分组获取配置校验
 
         :param group_name: 设备序列号
         :param expect: 配置内容，完整的配置路径，如{'lan': {'type': 'dhcp'}}
         :param type_: actual 实际设备上传的配置
                       group 设备所在组的配置
@@ -635,14 +1081,15 @@
 
 
 class Log(Base):
     def __init__(self, api, email, host):
         super().__init__(api, email, host)
         self.__device = Device(api, email, host)
 
+    @allure.step("SaaS验证job属性")
     def assert_job(self, job_id: str, **kwargs):
         """
         :param job_id: 任务id
         :param kwargs:
                status: canceled|
                type: firmware
                jobProcessDetails.total  总计下发的设备数
@@ -651,59 +1098,82 @@
         param = {'jobId': job_id, 'expand': 'jobProcessDetails', 'limit': 20, 'page': 0}
         try:
             result = self.api.send_request(f'api/v1/jobs', 'get', param=param).json().get('result')[0]
         except IndexError:
             raise ResourceNotFoundError(f'job {job_id} not found')
         dict_in(result, kwargs)
 
+    @allure.step("SaaS设备验证升级任务")
     def assert_device_task(self, sn: str, job_id: str, **kwargs):
         param = {'jobId': job_id, 'serialNumber': sn, 'limit': 20, 'page': 0}
         try:
             result = self.api.send_request('/api/v1/job/executions', 'get', param=param).json().get('result')[0]
         except IndexError:
             raise ResourceNotFoundError(f'job {job_id} not found')
         dict_in(result, kwargs)
 
+    @allure.step("SaaS取消设备最新任务")
     def cancel_device_latest_task(self, sn: str):
         param = {'serialNumber': sn, 'limit': 20, 'page': 0}
         try:
             result = self.api.send_request('/api/v1/job/executions', 'get', param=param).json().get('result')[0]
             if result.get('status') == 'queued':
                 self.api.send_request(f'/api/v1/job/executions/{result.get("_id")}/cancel', 'put')
             else:
                 logging.warning(f'the {sn} latest task status is {result.get("status")}, can not cancel')
         except IndexError:
             raise ResourceNotFoundError(f'the {sn} not has task')
 
+    @allure.step("SaaS取消任务")
     def cancel_job(self, job_id: str):
         """
 
         :param job_id: 任务id
         :return:
         """
         self.api.send_request(f'api/v1/jobs/{job_id}/cancel', 'put', expect={'result': 'ok'})
 
+    @allure.step("SaaS 设备取消等待任务")
+    def cancel_executions(self, job_id: str):
+        """
+
+        :param job_id: 任务id
+        :return:
+        """
+        for i_ in range(0, 10):
+            executions = self.api.send_request('api/v1/job/executions', 'get',
+                                               {'jobId': job_id, 'status': 'queued', 'limit': 100, 'page': 0}).json()
+            if executions.get('total') == 0:
+                break
+            else:
+                for execution in executions.get('result'):
+                    self.api.send_request(f'api/v1/job/executions/{execution.get("_id")}/cancel', 'put')
+
 
 class StarInterface:
 
     def __init__(self, email, password, host='star.inhandcloud.cn'):
         """ 须确保用户关闭了多因素认证
 
         :param email  平台用户名
         :param password  平台密码
         :param host: 'star.inhandcloud.cn'|'star.inhandcloud.cn'|'star.nezha.inhand.dev'|'star.nezha.inhand.design' 平台是哪个环境,
         """
-        self.api = InRequest(host, email, password, 'star')
+        self.api = InRequest(host, email, password, 'star', body_remove_none_key=True, param_remove_none_key=True)
         self.overview = Overview(self.api, email, host)
         self.device = Device(self.api, email, host)
+        self.firmware = Firmware(self.api, email, host)
         self.config = Config(self.api, email, host)
         self.org = Org(self.api, email, host)
         self.group = Group(self.api, email, host)
         self.log = Log(self.api, email, host)
 
 
 if __name__ == '__main__':
     from inhandtest.log import enable_log
 
     enable_log(console_level='debug')
-    star = StarInterface('liwei@inhand.com.cn', '123456', 'star.nezha.inhand.design')
-    print(star.device.assert_traffic('RT805LIWEI82113', after=-1, before=0))
+    # star = StarInterface('liwei@inhand.com.cn', '123456', 'star.nezha.inhand.design')
+    # for i in range(2001, 3000):
+    #     sn = f'EC94212345{str(i).rjust(5, "0")}'
+    #     star.device.add(sn=sn, mac_or_imei='00:18:05:00:00:00', name=sn)
+    #     star.group.move([sn], group_name='', group_id='64b8d9a90e1b8d1d245d79bf')
```

### Comparing `inhandtest-0.0.61/inhandtest/inserial.py` & `inhandtest-0.0.62/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/insocket.py` & `inhandtest-0.0.62/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/inssh.py` & `inhandtest-0.0.62/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/ip.py` & `inhandtest-0.0.62/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/log.py` & `inhandtest-0.0.62/inhandtest/log.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/mail.py` & `inhandtest-0.0.62/inhandtest/mail.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,14 +122,19 @@
     :param kwargs:
                   before_date: 匹配发送日期早于指定日期的邮件，格式：'2021-04-12 10:10:43'
                   after_date: 匹配发送日期晚于或等于指定日期的邮件，格式：'2021-04-12 10:10:43'
                   unseen: True| False 匹配未读邮件
                   seen_flag: True| False 对匹配到的所有邮件设置已读标记
                   body: str or list 对匹配到的邮件内容做校验，整个邮件的内容是text形式, 判断邮件内容是否包含body中的内容, 且html_body和body只能有一个
                   html_body: dict, {$xpath: $text()}对匹配到的邮件内容做校验，整个邮件的内容是html形式，example: {'//*[@id="mailContentContainer"]/div[1]': 'VG710自动化测试'}
+                  html_attribute: tuple or list, ($xpath, $attribute)对匹配到的邮件内容做校验，整个邮件的内容是html形式，example: ('//td[@align="center"]/a', 'href')
+                                   xpath: str,
+                                   attribute： str只能匹配一个属性
+                                   return str
+                  html_text: str,  $xpath,  return str
                   timeout: 超时时间，单位秒
                   interval: 每隔多久检查一次，单位秒
     :return:
     """
 
     def decode_str(s):
         """解码邮件标题"""
@@ -181,15 +186,15 @@
             subject_ = decode_str(email_message['Subject'])
             sender_from = decode_str(email_message['From'])
             if not ((subject in subject_) and (mail_from[0] in sender_from and mail_from[1] in sender_from)):
                 continue
             else:
                 logging.debug(f'get email success! subject: {subject_}, sender: {sender_from}')
             # 解析邮件正文
-            if not kwargs.get('body') and not kwargs.get('html_body'):
+            if not kwargs.get('body') and not kwargs.get('html_body') and not kwargs.get('html_attribute') and not kwargs.get('html_text'):
                 result = True
                 break
             else:
                 body = html_body = None
                 if email_message.is_multipart():
                     for part in email_message.walk():
                         content_type = part.get_content_type()
@@ -232,14 +237,26 @@
                             else:
                                 logging.warning(f'assert email html_body failed!')
                                 break
                         else:
                             result = True
                             logging.warning(f'assert email html_body success!')
                         break
+                if kwargs.get('html_attribute'):
+                    if not html_body:
+                        break
+                    else:
+                        html_body = etree.HTML(html_body)
+                        if isinstance(kwargs.get('html_attribute'), tuple):
+                            try:
+                                return html_body.xpath(kwargs.get('html_attribute')[0])[0].get(
+                                    kwargs.get('html_attribute')[1])
+                            except IndexError:
+                                logging.warning(f'not found html_attribute failed!')
+                                pass
         else:
             logging.debug(f'not found {subject} email')
     else:
         logging.error(f'get email failed: {status}')
     # 关闭 IMAP 连接
     imap_server.close()
     imap_server.logout()
@@ -272,8 +289,12 @@
     logging.info('delete all emails')
     imap_server.close()
     imap_server.logout()
 
 
 if __name__ == '__main__':
     # 设置日志
-    pass
+    delete_all_mail(('test@inhand.com.cn', 'ABc124'))
+    a = receive_last_mail(receiver=('test@inhand.com.cn', 'ABc124'),
+                          mail_from=('映翰通网络', 'iot_console@inhand.com.cn'), subject='邀请加入新组织',
+                          html_attribute=('//td[@align="center"]/a', 'href'))
+    print(a)
```

### Comparing `inhandtest-0.0.61/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py` & `inhandtest-0.0.62/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
                 # opc ua
                 ('servers_url', {'locator': self.pop_up.locator('#endpoint'), 'type': 'text'}),
 
                 # modbus tcp or rtu
                 ('ip_address', {'locator': self.page.locator('#point\.ip'), 'type': 'text'}),
                 ('port', {'locator': self.page.locator('#point\.port'), 'type': 'text'}),
                 # ISO-on-TCP
-                ('mode', {'locator': self.pop_up.locator('#args\.mode'), 'type': 'radio'}),
+                ('mode', {'locator': self.pop_up.locator('#args\.mode'), 'type': 'radio_select'}),
                 ('rack', {'locator': self.page.locator('#args\.rack'), 'type': 'text'}),
                 ('slot', {'locator': self.page.locator('#args\.slot'), 'type': 'text'}),
                 ('client_tsap', {'locator': self.page.locator('#args\.localTsap'), 'type': 'text'}),
                 ('server_tsap', {'locator': self.page.locator('#args\.remoteTsap'), 'type': 'text'}),
 
                 ('slave', {'locator': self.page.locator('#args\.slaveAddr'), 'type': 'text'}),
                 ('endpoint', {'locator': self.page.locator('#endpoint'), 'type': 'select'}),
@@ -292,29 +292,34 @@
     def controller_card(self, name) -> list:
         controller_name = f'//div[@class="ant-list-item"]//div[text()="{name}"]'
         controllers = [('select', {'locator': self.page.locator(controller_name), 'type': 'button'}),
                        ('check', {'locator': self.page.locator(f'{controller_name}/../../../../div[1]/label/span'),
                                   'type': 'check'}),
                        ('expand', {'locator': self.page.locator(f'{controller_name}/../../../../div[3]').locator(
                            '//i[@class="anticon anticon-ellipsis"]'), 'type': 'button'}),
-                       ('edit', {'locator': self.page.locator('.ant-dropdown-menu').locator('//li').nth(0),
+                       ('edit', {'locator': self.page.get_by_text(self.locale.edit, exact=True).locator("visible=true"),
                                  'type': 'button'}),
-                       ('set_as_template', {'locator': self.page.locator('.ant-dropdown-menu').locator('//li').nth(1),
-                                            'type': 'button'}),
-                       ('delete', {'locator': self.page.locator('.ant-dropdown-menu').locator('//li').nth(2),
-                                   'type': 'button'}),
+                       ('set_as_template', {
+                           'locator': self.page.get_by_text(self.locale.set_as_template, exact=True).locator(
+                               "visible=true"), 'type': 'button'}),
+                       ('delete',
+                        {'locator': self.page.get_by_text(self.locale.delete, exact=True).locator("visible=true"),
+                         'type': 'button'}),
                        ('delete_confirm',
                         {'locator': self.page.locator('.ant-modal-content').locator('.ant-btn.ant-btn-primary'),
                          'type': 'button', 'wait_for': {'type': 'timeout', 'timeout': 3 * 1000}}),
-                       ('disable', {'locator': self.page.locator('.ant-dropdown-menu').locator('//li').nth(3),
-                                    'type': 'button', 'wait_for': {'type': 'timeout', 'timeout': 3 * 1000}}),
-                       ('enable', {'locator': self.page.locator('.ant-dropdown-menu').locator('//li').nth(3),
-                                   'type': 'button', 'wait_for': {'type': 'timeout', 'timeout': 3 * 1000}}),
+                       ('disable',
+                        {'locator': self.page.get_by_text(self.locale.disable_2, exact=True).locator("visible=true"),
+                         'type': 'button', 'wait_for': {'type': 'timeout', 'timeout': 3 * 1000}}),
+                       ('enable',
+                        {'locator': self.page.get_by_text(self.locale.enable, exact=True).locator("visible=true"),
+                         'type': 'button', 'wait_for': {'type': 'timeout', 'timeout': 3 * 1000}}),
                        ('realtime_communication_message',
-                        {'locator': self.page.locator('.ant-dropdown-menu').locator('//li').nth(4),
+                        {'locator': self.page.get_by_text(self.locale.realtime_communication_message,
+                                                          exact=True).locator("visible=true"),
                          'type': 'button', }),
                        ]
         return controllers
 
     def controller_card_status(self, name) -> list:
         controller_name = f'//div[@class="ant-list-item"]//div[text()="{name}"]'
         controllers = [
@@ -404,19 +409,21 @@
         return [('name', {'locator': self.pop_up.locator('#name'), 'type': 'text'}),
                 # OPC-UA
                 ('namespace', {'locator': self.pop_up.locator('#index'), 'type': 'text'}),
                 ('address_type', {'locator': self.pop_up.locator('#idType'), 'type': 'select'}),
                 ('identifier', {'locator': self.pop_up.locator('#identifier'), 'type': 'text'}),
                 # ISO-on-TCP
                 ('register_type', {'locator': self.pop_up.locator('#regType'), 'type': 'select'}),
-                ('register_address', [{'locator': self.pop_up.locator(
+                ('dbnumber', {'locator': self.pop_up.locator('#dbnumber'), 'type': 'text'}),
+                ('modbus_register_address', [{'locator': self.pop_up.locator(
                     '.antd-pro-components-app-reg-addr-input-index-wrapper >> .ant-input-group-addon'),
                     'type': 'select'},
                     {'locator': self.pop_up.locator(
                         '.antd-pro-components-app-reg-addr-input-index-wrapper >> .ant-input'), 'type': 'text'}]),
+                ('register_address', {'locator': self.pop_up.locator('#regAddr'), 'type': 'text'}),
                 ('data_type', {'locator': self.pop_up.locator('#dataType'), 'type': 'select',
                                'param': {'bit': self.locale.get('bit'), 'word': self.locale.get('word'),
                                          'int': self.locale.get('int'), 'dword': self.locale.get('dword'),
                                          'dint': self.locale.get('dint'), 'bcd32': self.locale.get('bcd32'),
                                          'float': self.locale.get('float'), 'double': self.locale.get('double'),
                                          'string': self.locale.get('string'), 'bcd16': self.locale.get('bcd16'),
                                          'ulong': self.locale.get('ulong'), 'long': self.locale.get('long')}}),
@@ -430,14 +437,15 @@
                                      'param': {'ascii': 'ASCII', 'utf-8': 'UTF-8', 'utf-16': 'UTF-16',
                                                'utf-16-big': 'UTF-16-BIG', 'gb2312': 'GB2312'}}),
                 ('is_array', {'locator': self.pop_up.locator('#isArr'), 'type': 'switch_button'}),
                 ('read_write', {'locator': self.pop_up.locator('#readWrite'), 'type': 'select',
                                 'param': {'read': 'Read', 'read/write': 'Read/Write', 'write': 'Write'}}),
                 ('mode', {'locator': self.pop_up.locator('#uploadType'), 'type': 'select',
                           'param': {'periodic': 'Periodic', 'onchange': 'Onchange', 'never': 'Never'}}),
+                ('onchange_deadzone', {'locator': self.pop_up.locator('#deadZonePercent'), 'type': 'text'}),
                 ('unit', {'locator': self.pop_up.locator('#unit'), 'type': 'text'}),
                 ('description', {'locator': self.pop_up.locator('#desc'), 'type': 'text'}),
                 ('group', {'locator': self.pop_up.locator('#group'), 'type': 'select'}),
                 ('storage_lwtsdb', {'locator': self.pop_up.locator('#storageLwTSDB'), 'type': 'switch_button'}),
                 ('polling_interval', {'locator': self.pop_up.locator('#pollCycle'), 'type': 'select',
                                       'param': {'polling_interval': self.locale.polling_interval,
                                                 'polling_interval_2': self.locale.polling_interval_2}}),
@@ -457,14 +465,15 @@
                 ('magnification', {'locator': self.pop_up.locator('#gain'), 'type': 'text'}),
                 ('offset', {'locator': self.pop_up.locator('#offset'), 'type': 'text'}),
                 ('start_bit', {'locator': self.pop_up.locator('#startBit'), 'type': 'text'}),
                 ('end_bit', {'locator': self.pop_up.locator('#endBit'), 'type': 'text'}),
                 ('pt', {'locator': self.pop_up.locator('#pt'), 'type': 'text'}),
                 ('ct', {'locator': self.pop_up.locator('#ct'), 'type': 'text'}),
                 ('package_reporting', {'locator': self.pop_up.locator('#msecSample'), 'type': 'switch_button'}),
+                ('value_mapping', {'locator': self.value_mapping, 'type': 'value_mapping'}),
                 ('submit', {'locator': self.pop_up.locator('//button[@class="ant-btn ant-btn-primary"]'),
                             'type': 'button'}),
                 ('text_messages', {'type': 'text_messages'}),
                 ('tip_messages', {'type': 'tip_messages'}),
                 ('cancel', {'locator': self.pop_up.locator('//button[@class="ant-btn"]'),
                             'type': 'button'}),
                 ]
```

### Comparing `inhandtest-0.0.61/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.62/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 """
 python_edge_computing
 
 """
 import logging
 import random
 import allure
-import numpy as np
 from inhandtest.tools import loop_inspector
 from inhandtest.base_page.table_tr import IgTable
 from inhandtest.base_page.base_page import BasePage
 from inhandtest.pages.ingateway.locators import IgLocators
+from decimal import Decimal, ROUND_HALF_UP
 
 
 class PythonEdgeComputing(BasePage, IgLocators):
 
     def __init__(self, host: str, username: str, password: str, protocol='https',
                  port=443, model='IG902', language='en', page=None, locale: dict = None):
         super().__init__(host, username, password, protocol, port, model, language, page, locale=locale)
@@ -248,22 +248,18 @@
         :param action: [(action_type, value, ),]
         :return:
         """
         for ac in action:
             if ac[0] == 'add':
                 self.agg_in(self.edge_locators.measure_operation, {ac[0]: True})
                 self.agg_in(self.edge_locators.add_measure_all, ac[1])
-                if ac[1].get('value_mapping'):
-                    self.__value_mapping(self.edge_locators.value_mapping, ac[1].pop('value_mapping'))
             elif ac[0] == 'edit':
                 self.__turn_page(ac[1], 'measure')
                 self.agg_in(self.edge_locators.measure_table(ac[1]), {ac[0]: True})
                 self.agg_in(self.edge_locators.add_measure_all, ac[2])
-                if ac[2].get('value_mapping'):
-                    self.__value_mapping(self.edge_locators.value_mapping, ac[2].pop('value_mapping'))
             elif ac[0] == 'search':
                 self.agg_in(self.edge_locators.measure_operation, {"search_name": ac[1], 'search': True})
             elif ac[0] in ('import', 'export'):
                 self.agg_in(self.edge_locators.measure_operation, {ac[0]: ac[1]})
             elif ac[0] == 'check':
                 self.agg_in(self.edge_locators.measure_table(ac[1]), {'check': ac[2]})
             elif ac[0] == 'check_all':
@@ -276,15 +272,15 @@
             elif ac[0] == 'delete_all':
                 self.__measure([('check_all',)])
                 self.agg_in(self.edge_locators.measure_operation, {'delete_bulk': True, 'delete_bulk_confirm': True})
             elif ac[0] == 'delete':
                 self.agg_in(self.edge_locators.measure_table(ac[1]), {'delete': True, 'delete_confirm': True})
             elif ac[0] == 'value':
                 if list(filter(lambda x: x[0] == 'datatype', self.edge_locators.measure_card_status(ac[1])))[0][1].get(
-                        'locator').inner_text() == 'BIT':    # BIT 类型时是选择框
+                        'locator').inner_text() == 'BIT':  # BIT 类型时是选择框
                     if isinstance(ac[2], str):
                         value = {'value_edit': True, 'value_select': ac[2], 'submit': {"wait_for_time": 2 * 1000}}
                     else:
                         value = {'value_edit': True}
                         ac[2]['value_select'] = ac[2].pop('value')
                         value.update(ac[2])
                 else:
@@ -389,27 +385,30 @@
                         [('add', kwargs)]
                             kwargs:
                                 name: 名称
                                 namespace: 命名空间   OPC-UA
                                 address_type: String|Number   OPC-UA
                                 identifier: 标识符   OPC-UA
                                 register_type:   I|Q|M|DB    ISO-on-TCP
-                                register_address: 寄存器地址 list  ex: ['4X', '40001']
+                                dbnumber: 数据库号   ISO-on-TCP
+                                modbus_register_address: 寄存器地址 list  ex: ['4X', '40001']
+                                register_address: 寄存器地址 str ex: '1'
                                 data_type: 数据类型 bit,word,int,dword,dint,float,double,string,bcd16,ulong,long
                                 read_bit_data: enable | disable
                                 register_bit: 位寄存器
                                 data_register_bit: 数据寄存器
                                 negative_value: enable | disable
                                 storage_lwtsdb: enable | disable
                                 decimal_places: 小数位数
                                 size: 数据长度
                                 encoding_format: 编码格式 ascii, utf-8, utf-16, utf-16-big, gb2312
                                 is_array: enable | disable    OPC-UA
                                 read_write: 读写属性 read | write | read/write
                                 mode: periodic | onchange | never
+                                onchange_deadzone: onchange死区
                                 unit: 单位 str
                                 description: 描述
                                 group: 所属组
                                 polling_interval: polling_interval|polling_interval_2
                                 numerical_mapping: 数值映射 enable | disable
                                 data_calculation: 数据计算 no | ratio conversion | offset and zoom| bit truncation | pt/ct | value mapping
                                 trans_decimal: 数据运算小数位
@@ -1135,15 +1134,15 @@
         self.alarm = Alarm(host, username, password, protocol, port, model, language, page, locale)
         self.cloud = Cloud(host, username, password, protocol, port, model, language, page, locale)
         self.parameter = ParameterSettings(host, username, password, protocol, port, model, language, page, locale)
 
     @allure.step("数据运算计算")
     def data_calculation(self, transform_type, input_value, decimal=2, data_high_limit=0, data_lower_limit=0,
                          high_limit_of_proportion=0, lower_limit_of_proportion=0, magnification=0, offset=0, pt=0, ct=0,
-                         start_bit=0, end_bit=0, reverse=False) -> int or float:
+                         start_bit=0, end_bit=0, datatype='INT', reverse=False) -> int or float:
         """数据运算计算测点值
 
         :param transform_type: 1:比例换算 | 2:偏移及缩放 | 3:位截取 | 4:PT/CT
         :param input_value: 输入值
         :param decimal: 最后保留小数位
         :param data_high_limit: 数据上限
         :param data_lower_limit: 数据下限
@@ -1157,79 +1156,136 @@
         :param end_bit: 位截取截止位
         :param reverse: True | False
         :return:
         """
         operator_value = operation_value = 0.0
         if transform_type == 1:
             if reverse:
-                operation_value = (input_value - lower_limit_of_proportion) * (data_high_limit - data_lower_limit) / \
-                                  (high_limit_of_proportion - lower_limit_of_proportion) + data_lower_limit
+                operator_value = ((input_value - lower_limit_of_proportion) * (data_high_limit - data_lower_limit) / \
+                                  (high_limit_of_proportion - lower_limit_of_proportion)) + data_lower_limit
             else:
-                operation_value = (high_limit_of_proportion - lower_limit_of_proportion) / \
-                                  (data_high_limit - data_lower_limit) * (input_value - data_lower_limit) + \
-                                  lower_limit_of_proportion
+                operation_value = (Decimal(high_limit_of_proportion) - Decimal(lower_limit_of_proportion)) / \
+                                  (Decimal(data_high_limit) - Decimal(data_lower_limit)) * (
+                                              Decimal(input_value) - Decimal(data_lower_limit)) + \
+                                  Decimal(lower_limit_of_proportion)
         elif transform_type == 2:
             if reverse:
-                operation_value = (input_value - offset) / magnification
+                operator_value = (input_value - offset) / magnification
             else:
-                operation_value = input_value * magnification + offset
+                operation_value = Decimal(input_value) * Decimal(magnification) + Decimal(offset)
         elif transform_type == 3:
+            if 'BCD' in datatype.upper():
+                input_value = int(str(input_value), 16)
             if input_value >= 0:
                 bin_value = bin(input_value)
             else:
                 bin_value = bin((1 << 64) + input_value)
-            operation_value = int(bin_value[::-1][start_bit:end_bit][::-1], 2)
+            operation_value = int(bin_value[::-1][start_bit:end_bit + 1][::-1], 2)
         elif transform_type == 4:
             if reverse:
                 operator_value = (input_value / ct / pt - offset) / magnification
             else:
-                operation_value = (input_value * magnification + offset) * pt * ct
+                operation_value = (Decimal(input_value) * Decimal(magnification) + Decimal(offset)) * Decimal(
+                    pt) * Decimal(ct)
         else:
             raise Exception('NonsupportTransformType')
         if reverse:
-            return int(operator_value)
+            if isinstance(input_value, int):
+                return int(operator_value)
+            else:
+                return operator_value
         else:
-            return round(operation_value, decimal)
+            if transform_type != 3:
+                logging.info(type(operation_value))
+                decimal_value = Decimal(operation_value).quantize(Decimal('0.'.ljust(decimal + 2, '0')),
+                                                                  rounding=ROUND_HALF_UP)
+                logging.info('The number is {}, after operation is {}'.format(input_value, decimal_value))
+                # operation_value = round(operation_value, decimal)
+                if len(str(decimal_value).split('.')[0]) >= 22:
+                    logging.info('The number is {}, greater than 20 are represented by scientific notation!'.format(
+                        operation_value))
+                    return '{:.16e}'.format(operation_value)
+                else:
+                    return decimal_value
+            else:
+                return operation_value
 
     @allure.step("生成数据运算配置")
     def generate_config_parameter(self, transform_type: int, datatype: str):
         """
 
         :param transform_type: 1:比例换算 | 2:偏移及缩放 | 3:位截取 | 4:PT/CT
         :param datatype: 数据类型 BYTE| SINT| BCD| INT| WORD| DINT| DWORD| LONG| ULONG| FLOAT| DOUBLE
         :return:
         """
-        datatype_list = {'SINT': (-(2 ** 8 // 2), (2 ** 8 - 1) // 2), 'BYTE': (0, 2 ** 8 - 1), 'BCD': (0, 9999),
+        datatype_list = {'SINT': (-(2 ** 8 // 2), (2 ** 8 - 1) // 2), 'BYTE': (0, 2 ** 8 - 1), 'BCD16': (0, 9999),
                          'INT': (-(2 ** 16 // 2), (2 ** 16 - 1) // 2), 'WORD': (0, 2 ** 16 - 1),
-                         'DINT': (-(2 ** 32 // 2), (2 ** 32 - 1) // 2),
+                         'DINT': (-(2 ** 32 // 2), (2 ** 32 - 1) // 2), 'BCD32': (0, 99999999),
                          'DWORD': (0, 2 ** 32 - 1), 'LONG': (-(2 ** 64 // 2), (2 ** 64 - 1) // 2),
                          'ULONG': (0, 2 ** 64 - 1)}
-        digit_list = {'SINT': (0, 7), 'BYTE': (0, 7), 'BCD': (0, 15), 'INT': (0, 15), 'WORD': (0, 15), 'DINT': (0, 31),
-                      'DWORD': (0, 31), 'LONG': (0, 63), 'ULONG': (0, 63)}
+        digit_list = {'SINT': (0, 7), 'BYTE': (0, 7), 'BCD16': (0, 15), 'INT': (0, 15), 'WORD': (0, 15),
+                      'DINT': (0, 31),
+                      'DWORD': (0, 31), 'BCD32': (0, 31), 'LONG': (0, 63), 'ULONG': (0, 63)}
         type_ = datatype.upper()
         if transform_type == 1:
             if type_ in ['FLOAT', 'DOUBLE']:
-                value_range = sorted([random.uniform(-9999999999, 9999999999) for i in range(2)])
+                value_range = sorted([round(random.uniform(-9999999999, 9999999999), 6) for i in range(2)])
             else:
-                value_range = sorted(list(np.random.randint(datatype_list[type_][0], datatype_list[type_][1], 2)))
-            print(value_range)
-            scale_range = sorted([random.uniform(-9999999999, 9999999999) for i in range(2)])
-            print(scale_range)
+                value_range = sorted(
+                    [random.randint(datatype_list[type_][0], datatype_list[type_][1]) for i in range(2)])
+            scale_range = sorted([round(random.uniform(-9999999999, 9999999999), 6) for i in range(2)])
             gain_value = value_range + scale_range
+            logging.info('config parameter: {}'.format(gain_value))
             return gain_value
         elif transform_type == 2:
-            zoom_range = [random.uniform(-9999999999, 9999999999) for i in range(2)]
+            zoom_range = [round(random.uniform(-9999, 9999), 6) for i in range(2)]
             return zoom_range
         elif transform_type == 3:
             bit_range = sorted([random.randint(digit_list[type_][0], digit_list[type_][1]) for i in range(2)])
             return bit_range
         else:
-            pt_range = [random.uniform(-9999999999, 9999999999) for i in range(4)]
+            pt_range = [round(random.uniform(-999, 999), 6) for i in range(4)]
             return pt_range
 
+    @allure.step('根据数据类型生成随机值')
+    def generate_random_value(self, datatype, magnification=1, offset=0, pt=1, ct=1):
+        """
+        根据数据类型生成随机数
+        :param datatype:  数据类型 BYTE| SINT| BCD| INT| WORD| DINT| DWORD| LONG| ULONG| FLOAT| DOUBLE
+        :param magnification: 倍率
+        :param offset: 偏移量
+        :param pt:
+        :param ct:
+        :return:
+        """
+        type_ = datatype.upper()
+        datatype_list = {'SINT': (-(2 ** 8 // 2), (2 ** 8 - 1) // 2), 'BYTE': (0, 2 ** 8 - 1), 'BCD16': (0, 9999),
+                         'INT': (-(2 ** 16 // 2), (2 ** 16 - 1) // 2), 'WORD': (0, 2 ** 16 - 1),
+                         'DINT': (-(2 ** 32 // 2), (2 ** 32 - 1) // 2), 'BCD32': (0, 99999999),
+                         'DWORD': (0, 2 ** 32 - 1), 'LONG': (-(2 ** 64 // 2), (2 ** 64 - 1) // 2),
+                         'ULONG': (0, 2 ** 64 - 1)}
+        if type_ in ['FLOAT', 'DOUBLE']:
+            low, high = sorted(
+                [(-999999 * magnification + offset) * pt * ct, (999999 * magnification - offset) * pt * ct])
+            value = round(random.uniform(low, high), 2)
+        else:
+            if magnification == 1 and offset == 0 and pt == 1 and ct == 1:
+                if type_ in ['BYTE', 'SINT', 'BCD16', 'INT', 'WORD']:
+                    value = random.randint(datatype_list[type_][0], datatype_list[type_][1])
+                elif type_ in ['DINT', 'LONG', ]:
+                    value = random.randint(-32768, 32767)
+                elif type_ in ['DWORD', 'ULONG', 'BCD32']:
+                    value = random.randint(0, 65535)
+            else:
+                low, high = sorted([int((datatype_list[type_][0] * magnification + offset) * pt * ct),
+                                    int((datatype_list[type_][1] * magnification + offset) * pt * ct)])
+                value = random.randint(low, high)
+        logging.info(f'generate random value {value}')
+        return value
+
 
 class EdgeComputing:
 
     def __init__(self, host: str, username: str, password: str, protocol='https',
                  port=443, model='IG902', language='en', page=None, locale: dict = None):
         self.python_edge: PythonEdgeComputing = PythonEdgeComputing(host, username, password, protocol, port,
                                                                     model, language, page, locale)
```

### Comparing `inhandtest-0.0.61/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.62/inhandtest/pages/ingateway/ingateway.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.62/inhandtest/pages/ingateway/locale.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 en:
   client: Client
   server: Server
   ap: AP
+  edit: Edit
+  delete: Delete
+  set_as_template: Set as Template
+  realtime_communication_message: Realtime Communication Message
+  disable_2: Disable
   connect: Connected
   disconnect: Disconnected
   enable: Enable
   disable: Disable
   disable_: Disable
   not_enable: Not Enabled
   not_register: Not Register
@@ -198,14 +203,19 @@
   sign: Sign
   sign_encrypt: Sign & Encrypt
   siemens_plc: Siemens PLC
 cn:
   client: 客户端
   server: 服务器
   ap: 接入端
+  edit: 编辑
+  delete: 删除
+  set_as_template: 设为模板
+  realtime_communication_message: 实时通讯报文
+  disable_2: 禁用
   connect: 已连接
   disconnect: 未连接
   enable: 启用
   disable: 已关闭
   disable_: 关闭
   not_enable: 未启用
   not_register: 未注册
```

### Comparing `inhandtest-0.0.61/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.62/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.62/inhandtest/pages/ingateway/network/network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.62/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.62/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.62/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/pages/ingateway/system/system.py` & `inhandtest-0.0.62/inhandtest/pages/ingateway/system/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/pages/ingateway/system/system_locators.py` & `inhandtest-0.0.62/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/pytest_email.html` & `inhandtest-0.0.62/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/inhandtest/telnet.py` & `inhandtest-0.0.62/inhandtest/telnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,27 +360,28 @@
                 self.tn.write((com + "\n").encode("cp936"))
                 until_result = []
                 for i in range(0, timeout, 1):  # 30秒没有找到期望的就主动断开
                     time.sleep(1)
                     result = self.tn.read_very_eager().decode(read_content_decode, "ignore").strip().replace('\x08', '')
                     if result:
                         logging.debug(result)
-                        result = result.split(com + "\r\n")[-1]
                     if read_until_:
                         until_result.append(result)
+                        read_all_data = ''.join(until_result).split(com)[-1]  # 去除命令
                         if isinstance(read_until_, str):
-                            if read_until_ in ''.join(until_result):
-                                result = ''.join(until_result)
+                            if read_until_ in read_all_data:
+                                result = read_all_data
                                 break
                         elif isinstance(read_until_, list):
                             if not [read_until_one for read_until_one in read_until_ if
-                                    read_until_one not in ''.join(until_result)]:
-                                result = ''.join(until_result)
+                                    read_until_one not in read_all_data]:
+                                result = read_all_data
                                 break
                     else:
+                        result = result.split(com)[-1]
                         # 如果没有readuntil 直接返回
                         break
                 else:
                     self.tn.write(("\003" + "\r").encode("cp936"))
                     time.sleep(1)
                     if not kwargs.get('read_until_timeout_no_raise'):
                         logging.exception(f"Device {self.host} send cli {command} ReadUntilTimeOutError")
@@ -518,14 +519,15 @@
         :param expect: str or list or dict,
                        一条或多条希望校验的存在的结果，如需要判断不存在时，可以使用字典{$expect: False}
                        str或者list时都是判断存在
         :param kwargs: 命令参数, str, interface| param| cat_num
                         interface: 接口名称, wan| wifi_24g| wifi_5g| lan| cellular1
                         param: 抓包过滤关键字, None, 'icmp', 'http', 'port 21', 'host 1.1.1.1 and icmp'
                         catch_num: 抓包数量, int
+                        key_replace_type: 替换类型, str,  默认是cli
         :param key_replace: 字典类型， 传入的参数转换关系表{$old: $new}
         :param timeout: 校验超时时间, int
         :param interval: 5
         :return:
         """
         flag = {'interface': '-i', 'param': '', 'catch_num': '-c'}
         command = 'tcpdump'
@@ -546,27 +548,27 @@
                 expect_ = expect
             else:
                 logging.exception('parameter expect type error')
                 raise Exception('parameter expect type error')
             if expect_:
                 try:
                     _result = self.send_cli(command, [expect_], timeout=timeout, type_='super', key_replace=key_replace,
-                                            key_replace_type='cli')
+                                            key_replace_type=kwargs.get('key_replace_type', 'cli'),)
                     logging.debug('find the exception in tcpdump result.')
                     self.tn.write(("\003" + "\r").encode("cp936"))
                     if not_expect_:
                         if [not_expect for not_expect in not_expect_ if not_expect in _result]:
                             result = False
                 except:
                     result = False
             else:
                 if not_expect_:
                     _result = self.send_cli(command, '你还好', timeout=timeout, type_='super',
                                             key_replace=key_replace,
-                                            key_replace_type='cli',
+                                            key_replace_type=kwargs.get('key_replace_type', 'cli'),
                                             read_until_timeout_no_raise=True)
                     if [not_expect for not_expect in not_expect_ if not_expect in _result]:
                         result = False
             if result:
                 break
             else:
                 time.sleep(interval)
```

### Comparing `inhandtest-0.0.61/inhandtest/tools.py` & `inhandtest-0.0.62/inhandtest/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,21 +36,21 @@
         @wraps(func)
         def inspector(*args, **kwargs):
             nonlocal timeout, interval
             timeout = kwargs.get('timeout') if kwargs.get('timeout') else timeout
             interval = kwargs.get('interval') if kwargs.get('interval') else interval
             for i in range(0, timeout, interval):
                 result = func(*args, **kwargs)
-                if not result:
+                if result or result is None:
+                    logging.info(f'{flag} assert success')
+                    return result
+                else:
                     logging.info(f'{flag} assert failure, wait for {interval}s inspection')
                     time.sleep(interval)
                     continue
-                else:
-                    logging.info(f'{flag} assert success')
-                    return result
             else:
                 if assertion:
                     logging.exception(f'{flag} assert timeout failure')
                     raise AssertionError(f'{flag} assert timeout failure')
 
         return inspector
 
@@ -385,14 +385,37 @@
         time_stamp = datetime.datetime.utcnow() + delta_time
     else:
         time_stamp = datetime.datetime.strptime(time_, time_format) + delta_time
     res = time_stamp.strftime(time_format) if time_format else time_stamp.timestamp()
     return res
 
 
+def time_delta(time_list, delta, diff=0, time_format='%Y-%m-%dT%H:%M:%SZ', order_by=True):
+    """校验连续数据时间差
+
+    :param time_list: list of timestamp
+    :param delta: int 单位秒 两个数据点之间的时间差10s 正整数
+    :param diff: int 允许的误差 more为0  正整数
+    :param time_format: str 时间格式
+    :param order_by: bool True 传入的时间列表是按时间从小到大排列， False 传入的时间列表是按时间从大到小排列
+    :return:
+    """
+    tmp = []
+    for each in time_list:
+        each = time.strptime(each, time_format)
+        tmp.append(int(time.mktime(each)))
+    t0 = tmp[0]
+    for i_ in tmp[1:]:
+        if not order_by:
+            assert delta-diff <= t0 - i_ <= delta + diff, f'The time error between {t0} and {i_} is large'
+        else:
+            assert delta-diff <= i_ - t0 <= delta + diff, f'The time error between {t0} and {i_} is large'
+        t0 = i_
+
+
 def dict_in(expect_dict: dict, contain: dict) -> None:
     """验证字典包含关系
 
     :param expect_dict: dict {key: value}
     :param contain: dict,  支持${value} 表达式判断
     :return: AssertionError
     """
@@ -620,16 +643,15 @@
         except:
             pass
     else:
         logging.exception(f'all installed software is {all_installed}')
         raise ResourceNotFoundError(f'Not found the software {name}')
 
 
-
-@loop_inspector('PC Ping',)
+@loop_inspector('PC Ping', )
 def pc_ping(host_or_ip: str or list or tuple = 'www.baidu.com', number: int = 4, src=None,
             lost_packets=False, assert_result=True, timeout=120, interval=10) -> bool:
     """ 验证在PC机上ping某个地址是否丢包， 仅判断丢包
 
     :param lost_packets:
     :param src: 验证的源IP地址 '192.168.2.100'
     :param host_or_ip: 验证的目的IP地址, 可使用元组或列表接收多个地址
@@ -682,16 +704,10 @@
         except KeyError:
             logging.exception(f'Not found the key {key}')
             raise AttributeError(key)
 
     def __setattr__(self, key, value):
         self[key] = value
 
-if __name__ == '__main__':
-    # kill_windows_port('10.5.24.224', 1111)
 
-    for i in range(0,10):
-        print(generate_uuid())
-    # is_installed('Google Chrome123')
-    # print(windows_cmd('route delete 192.168.2.102 mask 255.255.255.255 192.168.4.2', '操作完成', {' ': '', '\n': ''}))
-    # print(generate_password(length=2, lowercase=True, uppercase=True, special_chars=True, chinese_chars=True))
-    # print(get_time_stamp('2022-02-18T13:39:32Z', -2))
+if __name__ == '__main__':
+    print(get_time_stamp('2022-02-18T13:39:32Z', -2))
```

### Comparing `inhandtest-0.0.61/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.62/inhandtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.61
+Version: 0.0.62
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.61/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.62/inhandtest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.61/setup.py` & `inhandtest-0.0.62/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.61',
+    version='0.0.62',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
@@ -25,11 +25,11 @@
     package_data={'inhandtest': ['*.html'], 'inhandtest.pages.ingateway': ['*.yml']},
     url='https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》',
     long_description='方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；\n映翰通出品，追尾必究！',
     classifiers=[
         "Programming Language :: Python :: 3.7",
     ],
     install_requires=['pytz', 'requests', 'playwright', 'pyserial', 'modbus-tk', 'paho-mqtt', 'urllib3', 'paramiko',
-                      'emails', 'Jinja2', 'pymongo', 'psutil', 'lxml', 'dynaconf', 'colorlog'
+                      'emails', 'Jinja2', 'pymongo', 'psutil', 'lxml', 'dynaconf', 'colorlog', 'pandas'
                       # 这里是依赖列表，表示运行这个包的运行某些功能还需要你安装其他的包
                       ],
 )
```

