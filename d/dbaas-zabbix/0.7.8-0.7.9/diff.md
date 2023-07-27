# Comparing `tmp/dbaas_zabbix-0.7.8.tar.gz` & `tmp/dbaas_zabbix-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbaas_zabbix-0.7.8.tar", last modified: Fri Apr  8 19:11:00 2022, max compression
+gzip compressed data, was "dbaas_zabbix-0.7.9.tar", max compression
```

## Comparing `dbaas_zabbix-0.7.8.tar` & `dbaas_zabbix-0.7.9.tar`

### file list

```diff
@@ -1,25 +1,10 @@
-drwxr-xr-x   0 ricardo.dias   (501) staff       (20)        0 2022-04-08 19:11:00.000000 dbaas_zabbix-0.7.8/
--rw-r--r--   0 ricardo.dias   (501) staff       (20)      715 2022-04-08 19:11:00.000000 dbaas_zabbix-0.7.8/PKG-INFO
-drwxr-xr-x   0 ricardo.dias   (501) staff       (20)        0 2022-04-08 19:11:00.000000 dbaas_zabbix-0.7.8/dbaas_zabbix.egg-info/
--rw-r--r--   0 ricardo.dias   (501) staff       (20)      715 2022-04-08 19:10:59.000000 dbaas_zabbix-0.7.8/dbaas_zabbix.egg-info/PKG-INFO
--rw-r--r--   0 ricardo.dias   (501) staff       (20)        1 2018-12-12 20:12:37.000000 dbaas_zabbix-0.7.8/dbaas_zabbix.egg-info/not-zip-safe
--rw-r--r--   0 ricardo.dias   (501) staff       (20)      495 2022-04-08 19:10:59.000000 dbaas_zabbix-0.7.8/dbaas_zabbix.egg-info/SOURCES.txt
--rw-r--r--   0 ricardo.dias   (501) staff       (20)        9 2022-04-08 19:10:59.000000 dbaas_zabbix-0.7.8/dbaas_zabbix.egg-info/requires.txt
--rw-r--r--   0 ricardo.dias   (501) staff       (20)       13 2022-04-08 19:10:59.000000 dbaas_zabbix-0.7.8/dbaas_zabbix.egg-info/top_level.txt
--rw-r--r--   0 ricardo.dias   (501) staff       (20)        1 2022-04-08 19:10:59.000000 dbaas_zabbix-0.7.8/dbaas_zabbix.egg-info/dependency_links.txt
--rw-r--r--   0 ricardo.dias   (501) staff       (20)     1473 2018-08-07 13:28:49.000000 dbaas_zabbix-0.7.8/LICENSE
--rw-r--r--   0 ricardo.dias   (501) staff       (20)     3217 2018-08-07 13:28:49.000000 dbaas_zabbix-0.7.8/CONTRIBUTING.rst
--rw-r--r--   0 ricardo.dias   (501) staff       (20)      137 2018-08-07 13:28:49.000000 dbaas_zabbix-0.7.8/MANIFEST.in
-drwxr-xr-x   0 ricardo.dias   (501) staff       (20)        0 2022-04-08 19:11:00.000000 dbaas_zabbix-0.7.8/dbaas_zabbix/
--rw-r--r--   0 ricardo.dias   (501) staff       (20)     2645 2022-04-08 15:52:37.000000 dbaas_zabbix-0.7.8/dbaas_zabbix/metrics.py
--rw-r--r--   0 ricardo.dias   (501) staff       (20)    10566 2020-02-17 19:10:06.000000 dbaas_zabbix-0.7.8/dbaas_zabbix/database_providers.py
--rwxr-xr-x   0 ricardo.dias   (501) staff       (20)     7238 2021-10-01 13:19:08.000000 dbaas_zabbix-0.7.8/dbaas_zabbix/provider.py
--rwxr-xr-x   0 ricardo.dias   (501) staff       (20)      654 2018-08-07 13:28:49.000000 dbaas_zabbix-0.7.8/dbaas_zabbix/__init__.py
--rw-r--r--   0 ricardo.dias   (501) staff       (20)     1197 2019-07-18 14:25:25.000000 dbaas_zabbix-0.7.8/dbaas_zabbix/provider_factory.py
--rw-r--r--   0 ricardo.dias   (501) staff       (20)      559 2018-08-07 13:28:49.000000 dbaas_zabbix-0.7.8/dbaas_zabbix/errors.py
--rw-r--r--   0 ricardo.dias   (501) staff       (20)     2687 2022-04-08 15:51:48.000000 dbaas_zabbix-0.7.8/dbaas_zabbix/dbaas_api.py
--rwxr-xr-x   0 ricardo.dias   (501) staff       (20)     1296 2022-04-08 18:44:58.000000 dbaas_zabbix-0.7.8/setup.py
--rw-r--r--   0 ricardo.dias   (501) staff       (20)      177 2018-08-07 13:28:49.000000 dbaas_zabbix-0.7.8/HISTORY.rst
--rw-r--r--   0 ricardo.dias   (501) staff       (20)      204 2018-08-07 13:28:49.000000 dbaas_zabbix-0.7.8/AUTHORS.rst
--rw-r--r--   0 ricardo.dias   (501) staff       (20)       61 2022-04-08 19:11:00.000000 dbaas_zabbix-0.7.8/setup.cfg
--rw-r--r--   0 ricardo.dias   (501) staff       (20)        0 2019-07-15 10:04:42.000000 dbaas_zabbix-0.7.8/README.rst
+-rwxr-xr-x   0        0        0     1184 2022-08-15 13:37:48.991298 dbaas_zabbix-0.7.9/dbaas_zabbix/__init__.py
+-rw-r--r--   0        0        0    10566 2022-08-04 18:15:43.049188 dbaas_zabbix-0.7.9/dbaas_zabbix/database_providers.py
+-rw-r--r--   0        0        0     2687 2022-08-04 18:15:43.049188 dbaas_zabbix-0.7.9/dbaas_zabbix/dbaas_api.py
+-rw-r--r--   0        0        0      559 2022-08-04 18:15:43.049188 dbaas_zabbix-0.7.9/dbaas_zabbix/errors.py
+-rw-r--r--   0        0        0     2645 2022-08-04 18:15:43.049188 dbaas_zabbix-0.7.9/dbaas_zabbix/metrics.py
+-rwxr-xr-x   0        0        0     7238 2022-08-05 12:55:46.810874 dbaas_zabbix-0.7.9/dbaas_zabbix/provider.py
+-rw-r--r--   0        0        0     1197 2022-08-04 18:15:43.049188 dbaas_zabbix-0.7.9/dbaas_zabbix/provider_factory.py
+-rw-r--r--   0        0        0      321 2022-08-15 19:50:32.241318 dbaas_zabbix-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0      521 2022-08-15 20:06:30.623972 dbaas_zabbix-0.7.9/setup.py
+-rw-r--r--   0        0        0      264 2022-08-15 20:06:30.624303 dbaas_zabbix-0.7.9/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dbaas_zabbix-0.7.8/dbaas_zabbix/metrics.py` & `dbaas_zabbix-0.7.9/dbaas_zabbix/metrics.py`

 * *Files identical despite different names*

### Comparing `dbaas_zabbix-0.7.8/dbaas_zabbix/database_providers.py` & `dbaas_zabbix-0.7.9/dbaas_zabbix/database_providers.py`

 * *Files identical despite different names*

### Comparing `dbaas_zabbix-0.7.8/dbaas_zabbix/provider.py` & `dbaas_zabbix-0.7.9/dbaas_zabbix/provider.py`

 * *Files identical despite different names*

### Comparing `dbaas_zabbix-0.7.8/dbaas_zabbix/provider_factory.py` & `dbaas_zabbix-0.7.9/dbaas_zabbix/provider_factory.py`

 * *Files identical despite different names*

### Comparing `dbaas_zabbix-0.7.8/dbaas_zabbix/errors.py` & `dbaas_zabbix-0.7.9/dbaas_zabbix/errors.py`

 * *Files identical despite different names*

### Comparing `dbaas_zabbix-0.7.8/dbaas_zabbix/dbaas_api.py` & `dbaas_zabbix-0.7.9/dbaas_zabbix/dbaas_api.py`

 * *Files identical despite different names*

