# Comparing `tmp/py-dactyl-2.0.2.tar.gz` & `tmp/py-dactyl-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-dactyl-2.0.2.tar", last modified: Tue May 23 02:36:19 2023, max compression
+gzip compressed data, was "py-dactyl-2.0.3.tar", last modified: Thu Jul 27 19:48:53 2023, max compression
```

## Comparing `py-dactyl-2.0.2.tar` & `py-dactyl-2.0.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.753814 py-dactyl-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-05-23 02:36:19.753814 py-dactyl-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.741814 py-dactyl-2.0.2/py_dactyl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-05-23 02:36:19.000000 py-dactyl-2.0.2/py_dactyl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-23 02:36:19.000000 py-dactyl-2.0.2/py_dactyl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 02:36:19.000000 py-dactyl-2.0.2/py_dactyl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 02:36:19.000000 py-dactyl-2.0.2/py_dactyl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 02:36:19.000000 py-dactyl-2.0.2/py_dactyl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.741814 py-dactyl-2.0.2/pydactyl/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/pydactyl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.745814 py-dactyl-2.0.2/pydactyl/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/pydactyl/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/pydactyl/api/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.745814 py-dactyl-2.0.2/pydactyl/api/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/pydactyl/api/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.745814 py-dactyl-2.0.2/pydactyl/api/client/account/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-23 02:36:06.000000 py-dactyl-2.0.2/pydactyl/api/client/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/account/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/client_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.745814 py-dactyl-2.0.2/pydactyl/api/client/servers/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/client/servers/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/nests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/servers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/pydactyl/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 02:36:19.753814 py-dactyl-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.745814 py-dactyl-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.745814 py-dactyl-2.0.2/tests/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/application/locations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/application/nests_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/application/nodes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/application/servers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/application/user_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.749814 py-dactyl-2.0.2/tests/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/base/api_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/base/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/base/responses_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:19.749814 py-dactyl-2.0.2/tests/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/account_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/backups_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/client_servers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/databases_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/files_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/schedules_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/settings_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/startup_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-23 02:36:07.000000 py-dactyl-2.0.2/tests/client/users_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:53.870573 py-dactyl-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-07-27 19:48:53.870573 py-dactyl-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:53.850571 py-dactyl-2.0.3/py_dactyl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-07-27 19:48:53.000000 py-dactyl-2.0.3/py_dactyl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-27 19:48:53.000000 py-dactyl-2.0.3/py_dactyl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:48:53.000000 py-dactyl-2.0.3/py_dactyl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 19:48:53.000000 py-dactyl-2.0.3/py_dactyl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 19:48:53.000000 py-dactyl-2.0.3/py_dactyl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:53.854572 py-dactyl-2.0.3/pydactyl/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:53.854572 py-dactyl-2.0.3/pydactyl/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:53.858572 py-dactyl-2.0.3/pydactyl/api/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:53.858572 py-dactyl-2.0.3/pydactyl/api/client/account/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/account/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/client_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:53.862572 py-dactyl-2.0.3/pydactyl/api/client/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/servers/backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/servers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/servers/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/servers/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/servers/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/servers/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/servers/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/servers/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/client/servers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/nests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/pydactyl/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:48:53.870573 py-dactyl-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:53.862572 py-dactyl-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:53.862572 py-dactyl-2.0.3/tests/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/application/locations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/application/nests_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/application/nodes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/application/servers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/application/user_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:53.866572 py-dactyl-2.0.3/tests/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/base/api_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/base/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/base/responses_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:53.870573 py-dactyl-2.0.3/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/client/account_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/client/backups_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/client/client_servers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/client/databases_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/client/files_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/client/network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/client/schedules_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/client/settings_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/client/startup_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-27 19:48:43.000000 py-dactyl-2.0.3/tests/client/users_test.py
```

### Comparing `py-dactyl-2.0.2/LICENSE` & `py-dactyl-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/PKG-INFO` & `py-dactyl-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-dactyl
-Version: 2.0.2
+Version: 2.0.3
 Summary: An easy to use Python wrapper for the Pterodactyl Panel API.
 Home-page: https://github.com/iamkubi/pydactyl
 Author: Ryan Kubiak
 Author-email: iamkubi@gmail.com
 Project-URL: Documentation, https://pydactyl.readthedocs.io/
 Project-URL: Source, https://github.com/iamkubi/pydactyl
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py-dactyl-2.0.2/README.md` & `py-dactyl-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/py_dactyl.egg-info/PKG-INFO` & `py-dactyl-2.0.3/py_dactyl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-dactyl
-Version: 2.0.2
+Version: 2.0.3
 Summary: An easy to use Python wrapper for the Pterodactyl Panel API.
 Home-page: https://github.com/iamkubi/pydactyl
 Author: Ryan Kubiak
 Author-email: iamkubi@gmail.com
 Project-URL: Documentation, https://pydactyl.readthedocs.io/
 Project-URL: Source, https://github.com/iamkubi/pydactyl
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py-dactyl-2.0.2/py_dactyl.egg-info/SOURCES.txt` & `py-dactyl-2.0.3/py_dactyl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/base.py` & `py-dactyl-2.0.3/pydactyl/api/base.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/client/account/base.py` & `py-dactyl-2.0.3/pydactyl/api/client/account/base.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/client/client_api.py` & `py-dactyl-2.0.3/pydactyl/api/client/client_api.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/client/servers/backups.py` & `py-dactyl-2.0.3/pydactyl/api/client/servers/backups.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/client/servers/base.py` & `py-dactyl-2.0.3/pydactyl/api/client/servers/base.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/client/servers/databases.py` & `py-dactyl-2.0.3/pydactyl/api/client/servers/databases.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/client/servers/files.py` & `py-dactyl-2.0.3/pydactyl/api/client/servers/files.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/client/servers/network.py` & `py-dactyl-2.0.3/pydactyl/api/client/servers/network.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/client/servers/schedules.py` & `py-dactyl-2.0.3/pydactyl/api/client/servers/schedules.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/client/servers/settings.py` & `py-dactyl-2.0.3/pydactyl/api/client/servers/settings.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/client/servers/startup.py` & `py-dactyl-2.0.3/pydactyl/api/client/servers/startup.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/client/servers/users.py` & `py-dactyl-2.0.3/pydactyl/api/client/servers/users.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/locations.py` & `py-dactyl-2.0.3/pydactyl/api/locations.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/nests.py` & `py-dactyl-2.0.3/pydactyl/api/nests.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/nodes.py` & `py-dactyl-2.0.3/pydactyl/api/nodes.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/servers.py` & `py-dactyl-2.0.3/pydactyl/api/servers.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api/user.py` & `py-dactyl-2.0.3/pydactyl/api/user.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/api_client.py` & `py-dactyl-2.0.3/pydactyl/api_client.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/pydactyl/responses.py` & `py-dactyl-2.0.3/pydactyl/responses.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,17 @@
             return self
         else:
             raise StopIteration
 
     def __str__(self):
         return '{}'.format(self.data)
 
+    def __len__(self):
+        return self.meta['pagination']['total']
+
     def get(self, key, default=None):
         """Retrieves a key from the paginated response.
 
         Returns:
             Value for the specified key
         """
         return getattr(self, key, default)
```

### Comparing `py-dactyl-2.0.2/setup.py` & `py-dactyl-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/application/locations_test.py` & `py-dactyl-2.0.3/tests/application/locations_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/application/nests_test.py` & `py-dactyl-2.0.3/tests/application/nests_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/application/nodes_test.py` & `py-dactyl-2.0.3/tests/application/nodes_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/application/servers_test.py` & `py-dactyl-2.0.3/tests/application/servers_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/application/user_test.py` & `py-dactyl-2.0.3/tests/application/user_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/base/api_client_test.py` & `py-dactyl-2.0.3/tests/base/api_client_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/base/base_test.py` & `py-dactyl-2.0.3/tests/base/base_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/base/responses_test.py` & `py-dactyl-2.0.3/tests/base/responses_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,7 +117,12 @@
         response = PaginatedResponse(self.client, 'asdf',
                                      MULTIPAGE_TEST_DATA[0])
         expected = [item for data in MULTIPAGE_TEST_DATA for item in
                     data['data']]
         expected_count = 16
         self.assertEqual(expected_count, len(expected))
         self.assertEqual(expected_count, len(response.collect()))
+
+    def test_paginated_response_len(self):
+        response = PaginatedResponse(self.client, 'anyendpoint', TEST_DATA)
+
+        self.assertEqual(106, len(response))
```

### Comparing `py-dactyl-2.0.2/tests/client/account_test.py` & `py-dactyl-2.0.3/tests/client/account_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/client/backups_test.py` & `py-dactyl-2.0.3/tests/client/backups_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/client/client_servers_test.py` & `py-dactyl-2.0.3/tests/client/client_servers_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/client/databases_test.py` & `py-dactyl-2.0.3/tests/client/databases_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/client/files_test.py` & `py-dactyl-2.0.3/tests/client/files_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/client/network_test.py` & `py-dactyl-2.0.3/tests/client/network_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/client/schedules_test.py` & `py-dactyl-2.0.3/tests/client/schedules_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/client/settings_test.py` & `py-dactyl-2.0.3/tests/client/settings_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/client/startup_test.py` & `py-dactyl-2.0.3/tests/client/startup_test.py`

 * *Files identical despite different names*

### Comparing `py-dactyl-2.0.2/tests/client/users_test.py` & `py-dactyl-2.0.3/tests/client/users_test.py`

 * *Files identical despite different names*

