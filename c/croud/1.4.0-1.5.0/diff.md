# Comparing `tmp/croud-1.4.0.tar.gz` & `tmp/croud-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croud-1.4.0.tar", last modified: Thu Jun 22 13:31:19 2023, max compression
+gzip compressed data, was "croud-1.5.0.tar", last modified: Thu Jul 27 14:49:25 2023, max compression
```

## Comparing `croud-1.4.0.tar` & `croud-1.5.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.125494 croud-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-06-22 13:31:14.000000 croud-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-22 13:31:19.125494 croud-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-22 13:31:14.000000 croud-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.117494 croud-1.4.0/croud/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 13:31:14.000000 croud-1.4.0/croud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48294 2023-06-22 13:31:14.000000 croud-1.4.0/croud/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-22 13:31:14.000000 croud-1.4.0/croud/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.117494 croud-1.4.0/croud/apikeys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/apikeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-22 13:31:14.000000 croud-1.4.0/croud/apikeys/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.117494 croud-1.4.0/croud/clusters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-06-22 13:31:14.000000 croud-1.4.0/croud/clusters/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-22 13:31:14.000000 croud-1.4.0/croud/clusters/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-22 13:31:14.000000 croud-1.4.0/croud/config/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-22 13:31:14.000000 croud-1.4.0/croud/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-22 13:31:14.000000 croud-1.4.0/croud/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-22 13:31:14.000000 croud-1.4.0/croud/me.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/organizations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/organizations/auditlogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/organizations/auditlogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-22 13:31:14.000000 croud-1.4.0/croud/organizations/auditlogs/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-06-22 13:31:14.000000 croud-1.4.0/croud/organizations/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/organizations/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/organizations/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-22 13:31:14.000000 croud-1.4.0/croud/organizations/users/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-06-22 13:31:14.000000 croud-1.4.0/croud/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-22 13:31:14.000000 croud-1.4.0/croud/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/products/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-22 13:31:14.000000 croud-1.4.0/croud/products/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-06-22 13:31:14.000000 croud-1.4.0/croud/projects/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/projects/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/projects/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-22 13:31:14.000000 croud-1.4.0/croud/projects/users/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/regions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/regions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-22 13:31:14.000000 croud-1.4.0/croud/regions/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-06-22 13:31:14.000000 croud-1.4.0/croud/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-22 13:31:14.000000 croud-1.4.0/croud/subscriptions/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-22 13:31:14.000000 croud-1.4.0/croud/tools/spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-22 13:31:14.000000 croud-1.4.0/croud/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-22 13:31:14.000000 croud-1.4.0/croud/users/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.121494 croud-1.4.0/croud/users/roles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/croud/users/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-22 13:31:14.000000 croud-1.4.0/croud/users/roles/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-22 13:31:14.000000 croud-1.4.0/croud/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.117494 croud-1.4.0/croud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-22 13:31:19.000000 croud-1.4.0/croud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-22 13:31:19.000000 croud-1.4.0/croud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:31:19.000000 croud-1.4.0/croud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 13:31:19.000000 croud-1.4.0/croud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-22 13:31:19.000000 croud-1.4.0/croud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 13:31:19.000000 croud-1.4.0/croud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-22 13:31:19.125494 croud-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-22 13:31:14.000000 croud-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.125494 croud-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.125494 croud-1.4.0/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    43174 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_me.py
--rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-22 13:31:14.000000 croud-1.4.0/tests/commands/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-22 13:31:14.000000 croud-1.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_config_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-22 13:31:14.000000 croud-1.4.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:31:19.125494 croud-1.4.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-22 13:31:14.000000 croud-1.4.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-22 13:31:14.000000 croud-1.4.0/tests/util/fake_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.200730 croud-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-07-27 14:49:20.000000 croud-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-27 14:49:25.200730 croud-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-27 14:49:20.000000 croud-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.188730 croud-1.5.0/croud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-27 14:49:20.000000 croud-1.5.0/croud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52793 2023-07-27 14:49:20.000000 croud-1.5.0/croud/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-27 14:49:20.000000 croud-1.5.0/croud/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.192730 croud-1.5.0/croud/apikeys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/apikeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-27 14:49:20.000000 croud-1.5.0/croud/apikeys/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.192730 croud-1.5.0/croud/clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28469 2023-07-27 14:49:20.000000 croud-1.5.0/croud/clusters/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-27 14:49:20.000000 croud-1.5.0/croud/clusters/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.192730 croud-1.5.0/croud/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-27 14:49:20.000000 croud-1.5.0/croud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-27 14:49:20.000000 croud-1.5.0/croud/config/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-27 14:49:20.000000 croud-1.5.0/croud/config/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-27 14:49:20.000000 croud-1.5.0/croud/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-27 14:49:20.000000 croud-1.5.0/croud/config/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-27 14:49:20.000000 croud-1.5.0/croud/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-27 14:49:20.000000 croud-1.5.0/croud/config/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.192730 croud-1.5.0/croud/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-27 14:49:20.000000 croud-1.5.0/croud/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-27 14:49:20.000000 croud-1.5.0/croud/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-27 14:49:20.000000 croud-1.5.0/croud/me.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.192730 croud-1.5.0/croud/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/organizations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.192730 croud-1.5.0/croud/organizations/auditlogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/organizations/auditlogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-27 14:49:20.000000 croud-1.5.0/croud/organizations/auditlogs/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-07-27 14:49:20.000000 croud-1.5.0/croud/organizations/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.192730 croud-1.5.0/croud/organizations/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/organizations/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-27 14:49:20.000000 croud-1.5.0/croud/organizations/users/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-07-27 14:49:20.000000 croud-1.5.0/croud/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-27 14:49:20.000000 croud-1.5.0/croud/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.192730 croud-1.5.0/croud/products/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-27 14:49:20.000000 croud-1.5.0/croud/products/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.192730 croud-1.5.0/croud/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-27 14:49:20.000000 croud-1.5.0/croud/projects/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.196730 croud-1.5.0/croud/projects/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/projects/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-27 14:49:20.000000 croud-1.5.0/croud/projects/users/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.196730 croud-1.5.0/croud/regions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/regions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-27 14:49:20.000000 croud-1.5.0/croud/regions/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-27 14:49:20.000000 croud-1.5.0/croud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.196730 croud-1.5.0/croud/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-27 14:49:20.000000 croud-1.5.0/croud/subscriptions/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.196730 croud-1.5.0/croud/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-27 14:49:20.000000 croud-1.5.0/croud/tools/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-27 14:49:20.000000 croud-1.5.0/croud/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.196730 croud-1.5.0/croud/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-27 14:49:20.000000 croud-1.5.0/croud/users/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.196730 croud-1.5.0/croud/users/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/croud/users/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-27 14:49:20.000000 croud-1.5.0/croud/users/roles/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-27 14:49:20.000000 croud-1.5.0/croud/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.192730 croud-1.5.0/croud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-27 14:49:25.000000 croud-1.5.0/croud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-27 14:49:25.000000 croud-1.5.0/croud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:49:25.000000 croud-1.5.0/croud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 14:49:25.000000 croud-1.5.0/croud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-27 14:49:25.000000 croud-1.5.0/croud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 14:49:25.000000 croud-1.5.0/croud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-27 14:49:25.200730 croud-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-27 14:49:20.000000 croud-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.196730 croud-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.200730 croud-1.5.0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/test_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51277 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/test_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/test_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/test_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13638 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/test_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/test_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/test_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-27 14:49:20.000000 croud-1.5.0/tests/commands/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-27 14:49:20.000000 croud-1.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-07-27 14:49:20.000000 croud-1.5.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-27 14:49:20.000000 croud-1.5.0/tests/test_config_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-27 14:49:20.000000 croud-1.5.0/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-27 14:49:20.000000 croud-1.5.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-07-27 14:49:20.000000 croud-1.5.0/tests/test_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 14:49:20.000000 croud-1.5.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-07-27 14:49:20.000000 croud-1.5.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:25.200730 croud-1.5.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-27 14:49:20.000000 croud-1.5.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-27 14:49:20.000000 croud-1.5.0/tests/util/fake_cloud.py
```

### Comparing `croud-1.4.0/LICENSE` & `croud-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/PKG-INFO` & `croud-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croud
-Version: 1.4.0
+Version: 1.5.0
 Summary: A command line interface for CrateDB Cloud
 Home-page: https://github.com/crate/croud
 Author: Crate.io
 Author-email: office@crate.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `croud-1.4.0/README.rst` & `croud-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/__init__.py` & `croud-1.5.0/croud/__init__.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/__main__.py` & `croud-1.5.0/croud/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,17 @@
     clusters_set_deletion_protection,
     clusters_set_ip_whitelist,
     clusters_set_product,
     clusters_set_suspended,
     clusters_snapshots_list,
     clusters_snapshots_restore,
     clusters_upgrade,
+    export_jobs_create,
+    export_jobs_delete,
+    export_jobs_list,
     import_jobs_create_from_file,
     import_jobs_create_from_url,
     import_jobs_delete,
     import_jobs_list,
 )
 from croud.config import CONFIG
 from croud.config.commands import (
@@ -63,14 +66,15 @@
 from croud.login import login
 from croud.logout import logout
 from croud.me import me, me_edit
 from croud.organizations.auditlogs.commands import auditlogs_list
 from croud.organizations.commands import (
     org_files_create,
     org_files_delete,
+    org_files_get,
     org_files_list,
     organizations_create,
     organizations_delete,
     organizations_edit,
     organizations_get,
     organizations_list,
 )
@@ -427,18 +431,24 @@
                         help="The product tier to use.",
                     ),
                     Argument(
                         "--unit", type=int, required=False,
                         help="The product scale unit to use.",
                     ),
                     Argument(
-                        "-p", "--project-id", type=str, required=True,
+                        "-p", "--project-id", type=str,
+                        required=False,
                         help="The project ID to use.",
                     ),
                     Argument(
+                        "--org-id", type=str,
+                        required=False,
+                        help="The organization ID to use.",
+                    ),
+                    Argument(
                         "--cluster-name", type=str, required=True,
                         help="The CrateDB cluster name to use.",
                     ),
                     Argument(
                         "--version", type=str, required=True,
                         help="The CrateDB version to use.",
                     ),
@@ -752,14 +762,86 @@
                                 ] + import_job_create_common_args,
                                 "resolver": import_jobs_create_from_file,
                             },
                         },
                     },
                 },
             },
+            "export-jobs": {
+                "help": "Manage data export jobs.",
+                "commands": {
+                    "delete": {
+                        "help": "Cancels an already running data export job that has "
+                                "not finished yet. "
+                                "If the job has already finished it deletes it from "
+                                "the job history.",
+                        "extra_args": [
+                            Argument(
+                                "--cluster-id", type=str, required=True,
+                                help="The cluster the job belongs to."
+                            ),
+                            Argument(
+                                "--export-job-id", type=str,
+                                required=True,
+                                help="The ID of the export job."
+                            ),
+                        ],
+                        "resolver": export_jobs_delete,
+                    },
+                    "list": {
+                        "help": "Lists data export jobs that belong to a specific "
+                                "cluster.",
+                        "extra_args": [
+                            Argument(
+                                "--cluster-id", type=str, required=True,
+                                help="The cluster the export jobs belong to."
+                            ),
+                        ],
+                        "resolver": export_jobs_list,
+                    },
+                    "create": {
+                        "help": "Create a data export job for the specified cluster.",
+                        "extra_args": [
+                            Argument(
+                                "--cluster-id", type=str, required=True,
+                                help="The cluster the data will be exported from."
+                            ),
+                            Argument(
+                                "--table",
+                                type=str,
+                                required=True,
+                                help="The table the data will be exported from.",
+                            ),
+                            Argument(
+                                "--file-format",
+                                type=str,
+                                required=True,
+                                choices=["csv", "json", "parquet"],
+                                help="The format of the data in the file.",
+                            ),
+                            Argument(
+                                "--compression",
+                                type=str,
+                                required=False,
+                                choices=["gzip"],
+                                help="The compression method of the exported file.",
+                            ),
+                            Argument(
+                                "--save-as",
+                                type=str,
+                                required=False,
+                                help="The file on your local filesystem the data will "
+                                     "be exported to. If not specified, you will "
+                                     "receive the URL to download the file.",
+                            ),
+                        ],
+                        "resolver": export_jobs_create,
+                    },
+                },
+            },
         },
     },
     "products": {
         "help": "Manage Products.",
         "commands": {
             "list": {
                 "help": "List all available products in the current region.",
@@ -914,14 +996,30 @@
                         "resolver": org_users_remove,
                     },
                 },
             },
             "files": {
                 "help": "Manage organization's files.",
                 "commands": {
+                    "get": {
+                        "help": (
+                            "Get a file by its ID."
+                        ),
+                        "extra_args": [
+                            Argument(
+                                "--org-id", type=str, required=True,
+                                help="The organization ID to use.",
+                            ),
+                            Argument(
+                                "--file-id", type=str, required=True,
+                                help="The ID of the file.",
+                            ),
+                        ],
+                        "resolver": org_files_get,
+                    },
                     "list": {
                         "help": "List all files uploaded to this organization.",
                         "extra_args": [
                             Argument(
                                 "--org-id", type=str, required=True,
                                 help="The organization ID to use.",
                             ),
```

### Comparing `croud-1.4.0/croud/api.py` & `croud-1.5.0/croud/api.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/apikeys/commands.py` & `croud-1.5.0/croud/apikeys/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/clusters/commands.py` & `croud-1.5.0/croud/clusters/commands.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,20 +12,25 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
 # License for the specific language governing permissions and limitations
 # under the License.
 #
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
+import functools
+import pathlib
 import time
 from argparse import Namespace
 from datetime import datetime, timedelta, timezone
-from typing import Any, Dict, Optional
+from shutil import copyfileobj
+from typing import Any, Dict, Optional, cast
 
 import bitmath
+import requests
+from tqdm.auto import tqdm
 
 from croud.api import Client
 from croud.clusters.exceptions import AsyncOperationNotFound
 from croud.config import get_output_format
 from croud.organizations.commands import op_upload_file_to_org
 from croud.printer import print_error, print_info, print_response, print_success
 from croud.tools.spinner import HALO
@@ -69,34 +74,45 @@
             "channel",
         ],
         output_fmt=get_output_format(args),
     )
 
 
 def clusters_deploy(args: Namespace) -> None:
+    if not args.project_id and not (args.org_id and args.region):
+        # We cannot have dynamically required params in croud, so have to verify here.
+        print_error("Either a project id or organization id and region are required.")
+        return
+
     body = {
         "cluster": {
             "crate_version": args.version,
             "name": args.cluster_name,
             "password": args.password,
             "product_name": args.product_name,
             "product_tier": args.tier,
             "username": args.username,
             "channel": args.channel,
         },
-        "project_id": args.project_id,
         "subscription_id": args.subscription_id,
     }
+    if args.project_id:
+        body["project_id"] = args.project_id
+    else:
+        body["project"] = {"name": args.cluster_name, "region": args.region}
+
     if args.unit:
         body["cluster"]["product_unit"] = args.unit
     _handle_edge_params(body["cluster"], args)
 
     client = Client.from_args(args)
 
-    org_id = _lookup_organization_id_for_project(client, args, args.project_id)
+    org_id = args.org_id or _lookup_organization_id_for_project(
+        client, args, args.project_id
+    )
     if not org_id:
         return
 
     data, errors = client.post(f"/api/v2/organizations/{org_id}/clusters/", body=body)
     print_response(
         data=data,
         errors=errors,
@@ -238,42 +254,26 @@
     print_response(
         data=data,
         errors=errors,
         keys=["id", "cluster_id", "status"],
         output_fmt=get_output_format(args),
     )
 
-    def import_job_feedback_func(status: str, feedback: dict):
-        num_records = feedback.get("progress", {}).get("records")
-        num_bytes = feedback.get("progress", {}).get("bytes")
-
-        records_normalized = num_records
-
-        if num_records > 1_000_000:
-            records_normalized = f"{records_normalized / 1_000_000:.2f} M"
-        elif num_records > 1_000:
-            records_normalized = f"{records_normalized / 1_000:.2f} K"
-
-        size = bitmath.Byte(num_bytes).best_prefix().format("{value:.2f} {unit}")
-        if status == "SUCCEEDED":
-            print_info(f"Done importing {records_normalized} records and {size}.")
-        else:
-            print_info(
-                f"Importing... {records_normalized} records and {size} imported so far."
-            )
-
     if data:
         import_job_id = data["id"]
 
         _wait_for_completed_operation(
             client=client,
             cluster_id=args.cluster_id,
             request_params={"import_job_id": import_job_id},
             operation_status_func=_get_import_job_operation_status,
-            feedback_func=import_job_feedback_func,
+            feedback_func=(
+                _data_job_feedback_func,
+                ("import",),
+            ),
         )
 
 
 def import_jobs_delete(args: Namespace) -> None:
     client = Client.from_args(args)
     data, errors = client.delete(
         f"/api/v2/clusters/{args.cluster_id}/import-jobs/{args.import_job_id}/"
@@ -648,14 +648,91 @@
             "repository",
             "snapshot",
         ],
         output_fmt=get_output_format(args),
     )
 
 
+def export_jobs_create(args: Namespace) -> None:
+    body = {
+        "source": {
+            "table": args.table,
+        },
+        "destination": {"format": args.file_format},
+    }
+
+    if args.compression:
+        body["compression"] = args.compression
+
+    client = Client.from_args(args)
+    data, errors = client.post(
+        f"/api/v2/clusters/{args.cluster_id}/export-jobs/", body=body
+    )
+    print_response(
+        data=data,
+        errors=errors,
+        keys=["id", "cluster_id", "status"],
+        output_fmt=get_output_format(args),
+    )
+
+    if data:
+        export_job_id = data["id"]
+
+        _wait_for_completed_operation(
+            client=client,
+            cluster_id=args.cluster_id,
+            request_params={"export_job_id": export_job_id},
+            operation_status_func=_get_export_job_operation_status,
+            feedback_func=(
+                _data_job_feedback_func,
+                ("export",),
+            ),
+            post_success_func=(
+                _download_exported_file,
+                (client, args.cluster_id, args.save_as, export_job_id),
+            ),
+        )
+
+
+def export_jobs_delete(args: Namespace) -> None:
+    client = Client.from_args(args)
+    data, errors = client.delete(
+        f"/api/v2/clusters/{args.cluster_id}/export-jobs/{args.export_job_id}/"
+    )
+    print_response(
+        data=data,
+        errors=errors,
+        keys=["id", "cluster_id", "status"],
+        output_fmt=get_output_format(args),
+    )
+
+
+def export_jobs_list(args: Namespace) -> None:
+    client = Client.from_args(args)
+    data, errors = client.get(f"/api/v2/clusters/{args.cluster_id}/export-jobs/")
+    print_response(
+        data=data,
+        errors=errors,
+        keys=["id", "cluster_id", "status", "source", "destination"],
+        output_fmt=get_output_format(args),
+        transforms={
+            "source": _transform_export_job_source,
+            "destination": _transform_export_job_destination,
+        },
+    )
+
+
+def _transform_export_job_source(field):
+    return field["table"]
+
+
+def _transform_export_job_destination(field):
+    return f"Format: {field['format']}\nFile ID: {field.get('file', {}).get('id')}"
+
+
 # We want to map the custom hardware specs to slightly nicer params in croud,
 # hence this mapping here
 def _handle_edge_params(body, args):
     if args.cpus:
         body.setdefault("hardware_specs", {})["cpus_per_node"] = args.cpus
     if args.disks:
         body.setdefault("hardware_specs", {})["disks_per_node"] = args.disks
@@ -702,21 +779,121 @@
     status = data["status"]
     feedback_data = {"progress": data["progress"]}
     msg = data["progress"]["message"]
 
     return status, msg, feedback_data
 
 
+def _get_formatted_size(feedback: dict) -> str:
+    num_bytes = feedback.get("progress", {}).get("bytes")
+    return bitmath.Byte(num_bytes).best_prefix().format("{value:.2f} {unit}")
+
+
+def _get_formatted_records_normalized(feedback: dict) -> str:
+    num_records = feedback.get("progress", {}).get("records")
+
+    records_normalized = num_records
+
+    if num_records > 1_000_000:
+        records_normalized = f"{records_normalized / 1_000_000:.2f} M"
+    elif num_records > 1_000:
+        records_normalized = f"{records_normalized / 1_000:.2f} K"
+
+    return records_normalized
+
+
+def _data_job_feedback_func(status: str, feedback: dict, job_type: str):
+    records_normalized = _get_formatted_records_normalized(feedback)
+    size = _get_formatted_size(feedback)
+
+    if status == "SUCCEEDED":
+        print_info(f"Done {job_type}ing {records_normalized} records and {size}.")
+    else:
+        print_info(
+            f"{job_type}ing... {records_normalized} records and {size} {job_type}ed "
+            "so far."
+        )
+
+
+def _download_exported_file(
+    client: Client, cluster_id: str, save_as: str, export_job_id: str
+):
+    data, errors = client.get(
+        f"/api/v2/clusters/{cluster_id}/export-jobs/{export_job_id}/"
+    )
+
+    if not data or not data.get("progress"):
+        raise AsyncOperationNotFound("Failed retrieving operation status.")
+
+    status = data["status"]
+    if status == "SUCCEEDED":
+        file_id = data.get("destination", {}).get("file", {}).get("id")
+        if file_id:
+            org_id = _get_org_id_from_cluster_id(client, cluster_id)
+            data, errors = client.get(
+                f"/api/v2/organizations/{org_id}/files/{file_id}/"
+            )
+            file_data: dict = cast(dict, data)
+            if not (file_data and file_data.get("download_url")):
+                print_error("File could not be fetched.")
+            if not save_as:
+                print_success(f"Download URL: {file_data['download_url']}")
+                return
+            HALO.stop()
+            print_info("Downloading file...")
+
+            r = requests.get(
+                file_data["download_url"], stream=True, allow_redirects=True
+            )
+            if r.status_code != 200:
+                r.raise_for_status()
+                print_error(
+                    f"Request to {file_data['download_url']} returned status code "
+                    f"{r.status_code}"
+                )
+            file_size = int(r.headers.get("Content-Length", 0))
+
+            path = pathlib.Path(save_as).expanduser().resolve()
+            path.parent.mkdir(parents=True, exist_ok=True)
+
+            desc = "(Unknown total file size)" if file_size == 0 else ""
+            r.raw.read = functools.partial(r.raw.read, decode_content=True)
+            with tqdm.wrapattr(r.raw, "read", total=file_size, desc=desc) as r_raw:
+                with path.open("wb") as f:
+                    copyfileobj(r_raw, f)
+
+            print_success(f"Successfully downloaded file to {path}")
+
+
+def _get_export_job_operation_status(
+    client: Client, cluster_id: str, request_params: Dict
+):
+    export_job_id = request_params["export_job_id"]
+    data, errors = client.get(
+        f"/api/v2/clusters/{cluster_id}/export-jobs/{export_job_id}/"
+    )
+
+    if not data or not data.get("progress"):
+        raise AsyncOperationNotFound("Failed retrieving export operation status.")
+
+    status = data["status"]
+    feedback_data = {"progress": data["progress"]}
+    msg = data["progress"]["message"]
+
+    return status, msg, feedback_data
+
+
 def _wait_for_completed_operation(
     *,
     client: Client,
     cluster_id: str,
     request_params: Dict,
     operation_status_func=_get_operation_status,
     feedback_func=None,
+    post_success_func=None,
 ):
     last_status = None
     last_msg = None
     while True:
         try:
             status, msg, feedback = operation_status_func(
                 client=client, cluster_id=cluster_id, request_params=request_params
@@ -732,18 +909,22 @@
             to_print = f"Status: {status} ({msg})" if msg else f"Status: {status}"
             print_info(to_print)
             last_status = status
             last_msg = msg
 
         # Call for custom feedback if function available and there is status to report.
         if status in ["IN_PROGRESS", "SUCCEEDED"] and feedback_func:
-            feedback_func(status, feedback)
+            (feedback_func, feedback_args) = feedback_func
+            feedback_func(status, feedback, *feedback_args)
 
         # Final statuses
         if status == "SUCCEEDED":
+            if post_success_func:
+                (func, call_args) = post_success_func
+                func(*call_args)
             print_success("Operation completed.")
             break
         if status == "FAILED":
             if msg:
                 print_error(msg)
             else:
                 print_error(
```

### Comparing `croud-1.4.0/croud/clusters/exceptions.py` & `croud-1.5.0/croud/clusters/exceptions.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/config/__init__.py` & `croud-1.5.0/croud/config/__init__.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/config/commands.py` & `croud-1.5.0/croud/config/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/config/configuration.py` & `croud-1.5.0/croud/config/configuration.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/config/exceptions.py` & `croud-1.5.0/croud/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/config/schemas.py` & `croud-1.5.0/croud/config/schemas.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/config/types.py` & `croud-1.5.0/croud/config/types.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/config/util.py` & `croud-1.5.0/croud/config/util.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/login.py` & `croud-1.5.0/croud/login.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/logout.py` & `croud-1.5.0/croud/logout.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/me.py` & `croud-1.5.0/croud/me.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/organizations/auditlogs/commands.py` & `croud-1.5.0/croud/organizations/auditlogs/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/organizations/commands.py` & `croud-1.5.0/croud/organizations/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
 import os
 from argparse import Namespace
 from typing import Any, Tuple
 
+import bitmath
 import requests
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 
 from croud.api import Client
 from croud.config import CONFIG, get_output_format
 from croud.printer import print_error, print_info, print_response
@@ -189,7 +190,29 @@
     )
     print_response(
         data=data,
         errors=errors,
         success_message="File upload deleted.",
         output_fmt=get_output_format(args),
     )
+
+
+def org_files_get(args: Namespace) -> None:
+    client = Client.from_args(args)
+    data, errors = client.get(
+        f"/api/v2/organizations/{args.org_id}/files/{args.file_id}/"
+    )
+    print_response(
+        data=data,
+        errors=errors,
+        keys=["id", "name", "status", "file_size", "download_url"],
+        output_fmt=get_output_format(args),
+        transforms={
+            "file_size": _transform_file_size,
+        },
+    )
+
+
+def _transform_file_size(size_bytes):
+    if not size_bytes:
+        return None
+    return bitmath.Byte(size_bytes).best_prefix().format("{value:.2f} {unit}")
```

### Comparing `croud-1.4.0/croud/organizations/users/commands.py` & `croud-1.5.0/croud/organizations/users/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/parser.py` & `croud-1.5.0/croud/parser.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/printer.py` & `croud-1.5.0/croud/printer.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/products/commands.py` & `croud-1.5.0/croud/products/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/projects/commands.py` & `croud-1.5.0/croud/projects/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/projects/users/commands.py` & `croud-1.5.0/croud/projects/users/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/regions/commands.py` & `croud-1.5.0/croud/regions/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/server.py` & `croud-1.5.0/croud/server.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/subscriptions/commands.py` & `croud-1.5.0/croud/subscriptions/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/typing.py` & `croud-1.5.0/croud/typing.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/users/commands.py` & `croud-1.5.0/croud/users/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/users/roles/commands.py` & `croud-1.5.0/croud/users/roles/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud/util.py` & `croud-1.5.0/croud/util.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/croud.egg-info/PKG-INFO` & `croud-1.5.0/croud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croud
-Version: 1.4.0
+Version: 1.5.0
 Summary: A command line interface for CrateDB Cloud
 Home-page: https://github.com/crate/croud
 Author: Crate.io
 Author-email: office@crate.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `croud-1.4.0/croud.egg-info/SOURCES.txt` & `croud-1.5.0/croud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/setup.py` & `croud-1.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
 
 from pkg_resources.extern.packaging.version import Version
 from setuptools import find_packages, setup
 
-__version__ = Version("1.4.0")
+__version__ = Version("1.5.0")
 
 try:
     with open("README.rst", "r", encoding="utf-8") as f:
         readme = f.read()
 except IOError:
     readme = ""
 
@@ -44,19 +44,19 @@
     install_requires=[
         "appdirs==1.4.4",
         "bitmath==1.3.3.1",
         "certifi",
         "colorama==0.4.6",
         "marshmallow==3.19.0",
         "pyyaml==6.0",
-        "requests==2.28.2",
+        "requests==2.31.0",
         "tabulate>=0.8,<1.0",
         "yarl==1.9.2",
         "halo==0.0.31",
-        "shtab==1.6.1",
+        "shtab==1.6.2",
         "tqdm==4.65.0",
     ],
     extras_require={
         "testing": [
             "tox==3.14.2",
             "pytest-freezegun==0.4.2",
         ],
```

### Comparing `croud-1.4.0/tests/commands/test_api_keys.py` & `croud-1.5.0/tests/commands/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/commands/test_clusters.py` & `croud-1.5.0/tests/commands/test_clusters.py`

 * *Files 15% similar despite different names*

```diff
@@ -147,14 +147,92 @@
         mock_request,
         RequestMethod.GET,
         f"/api/v2/clusters/{cluster_id}/",
         any_times=True,
     )
 
 
+@mock.patch.object(Client, "request", return_value=({}, None))
+@mock.patch("time.sleep")
+def test_clusters_deploy_no_project(_mock_sleep, mock_request):
+    cluster_id = gen_uuid()
+    subscription_id = gen_uuid()
+
+    def mock_call(*args, **kwargs):
+        if args[0] == RequestMethod.POST:
+            return {"id": cluster_id}, None
+        if args[0] == RequestMethod.GET and "/operations/" in args[1]:
+            global times_create_operations_called
+            if times_create_operations_called == 0:
+                times_create_operations_called += 1
+                return {"operations": [{"status": "SENT"}]}, None
+            return {"operations": [{"status": "SUCCEEDED"}]}, None
+        return None, None
+
+    mock_request.side_effect = mock_call
+    call_command(
+        "croud",
+        "clusters",
+        "deploy",
+        "--product-name",
+        "cratedb.az1",
+        "--tier",
+        "xs",
+        "--unit",
+        "1",
+        "--cluster-name",
+        "crate_cluster",
+        "--version",
+        "3.2.5",
+        "--username",
+        "foobar",
+        "--password",
+        "s3cr3t!",
+        "--subscription-id",
+        subscription_id,
+        "--org-id",
+        "123",
+        "--region",
+        "some.region",
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.POST,
+        "/api/v2/organizations/123/clusters/",
+        body={
+            "cluster": {
+                "crate_version": "3.2.5",
+                "name": "crate_cluster",
+                "password": "s3cr3t!",
+                "product_name": "cratedb.az1",
+                "product_tier": "xs",
+                "product_unit": 1,
+                "username": "foobar",
+                "channel": "stable",
+            },
+            "project": {"name": "crate_cluster", "region": "some.region"},
+            "subscription_id": subscription_id,
+        },
+        any_times=True,
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.GET,
+        f"/api/v2/clusters/{cluster_id}/operations/",
+        params={"type": "CREATE", "limit": 1},
+        any_times=True,
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.GET,
+        f"/api/v2/clusters/{cluster_id}/",
+        any_times=True,
+    )
+
+
 @mock.patch.object(Client, "request", return_value=(None, {}))
 def test_clusters_deploy_fails(mock_request, capsys):
     project_id = gen_uuid()
     subscription_id = gen_uuid()
 
     def mock_call(*args, **kwargs):
         if args[0] == RequestMethod.GET and "/projects/" in args[1]:
@@ -205,14 +283,46 @@
         },
         any_times=True,
     )
     _, err_output = capsys.readouterr()
     assert "Some Error" in err_output
 
 
+@pytest.mark.parametrize(
+    "additional_args", [[], ["--org-id", "123"], ["--region", "region"]]
+)
+def test_clusters_deploy_missing_args(additional_args, capsys):
+    args = [
+        "croud",
+        "clusters",
+        "deploy",
+        "--product-name",
+        "cratedb.az1",
+        "--tier",
+        "xs",
+        "--unit",
+        "1",
+        "--cluster-name",
+        "crate_cluster",
+        "--version",
+        "3.2.5",
+        "--username",
+        "foobar",
+        "--password",
+        "s3cr3t!",
+        "--subscription-id",
+        "123",
+    ]
+    call_command(*(args + additional_args))
+    _, err_output = capsys.readouterr()
+    assert (
+        "Either a project id or organization id and region are required." in err_output
+    )
+
+
 @mock.patch.object(Client, "request", return_value=({}, None))
 @mock.patch("time.sleep")
 def test_clusters_edge(_mock_sleep, mock_request):
     project_id = gen_uuid()
     cluster_id = gen_uuid()
 
     def mock_call(*args, **kwargs):
@@ -1250,15 +1360,16 @@
         assert e_info.value.code == 1
 
 
 times_restore_operations_called = 0
 
 
 @mock.patch.object(Client, "request")
-def test_cluster_snapshots_restore(mock_request):
+@mock.patch("time.sleep")
+def test_cluster_snapshots_restore(_mock_sleep, mock_request):
     cluster_id = gen_uuid()
 
     def mock_call(*args, **kwargs):
         if args[0] == RequestMethod.GET and "/operations/" in args[1]:
             global times_restore_operations_called
 
             if times_restore_operations_called == 0:
@@ -1304,15 +1415,16 @@
     assert mock_request.call_count == 3
 
 
 times_opt_restore_operations_called = 0
 
 
 @mock.patch.object(Client, "request")
-def test_cluster_snapshots_restore_with_optional_params(mock_request):
+@mock.patch("time.sleep")
+def test_cluster_snapshots_restore_with_optional_params(_mock_sleep, mock_request):
     cluster_id = gen_uuid()
 
     def mock_call(*args, **kwargs):
         if args[0] == RequestMethod.GET and "/operations/" in args[1]:
             global times_opt_restore_operations_called
 
             if times_opt_restore_operations_called == 0:
@@ -1503,7 +1615,189 @@
     call_command("croud", "clusters", "import-jobs", "list", "--cluster-id", "123")
     assert_rest(
         mock_request,
         RequestMethod.GET,
         "/api/v2/clusters/123/import-jobs/",
         params=None,
     )
+
+
+@mock.patch.object(
+    Client,
+    "request",
+    return_value=(
+        [
+            {
+                "cluster_id": "12345",
+                "dc": {
+                    "created": "2023-07-04T10:12:29.763000+00:00",
+                    "modified": "2023-07-04T10:12:29.763000+00:00",
+                },
+                "source": {"table": "my_table"},
+                "destination": {"format": "csv", "file": {"id": ""}},
+                "id": "45678",
+                "progress": {
+                    "bytes": 0,
+                    "message": "Failed",
+                    "records": 0,
+                },
+                "status": "FAILED",
+            }
+        ],
+        None,
+    ),
+)
+def test_export_job_list(mock_request):
+    cluster_id = gen_uuid()
+    call_command("croud", "clusters", "export-jobs", "list", "--cluster-id", cluster_id)
+    assert_rest(
+        mock_request,
+        RequestMethod.GET,
+        f"/api/v2/clusters/{cluster_id}/export-jobs/",
+        params=None,
+    )
+
+
+@mock.patch.object(Client, "request", return_value=({}, None))
+def test_export_job_delete(mock_request):
+    cluster_id = gen_uuid()
+    export_job_id = gen_uuid()
+    call_command(
+        "croud",
+        "clusters",
+        "export-jobs",
+        "delete",
+        "--export-job-id",
+        export_job_id,
+        "--cluster-id",
+        cluster_id,
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.DELETE,
+        f"/api/v2/clusters/{cluster_id}/export-jobs/{export_job_id}/",
+    )
+
+
+@pytest.mark.parametrize("save_file", [True, False])
+@mock.patch("croud.clusters.commands.copyfileobj")
+@mock.patch.object(Client, "request")
+def test_export_job_create(mock_client_request, mock_copy, save_file):
+    cluster_id = gen_uuid()
+    project_id = gen_uuid()
+    org_id = gen_uuid()
+    file_id = gen_uuid()
+    export_job_id = gen_uuid()
+    mock_client_request.side_effect = [
+        (
+            {
+                "id": export_job_id,
+                "status": "IN_PROGRESS",
+                "progress": {"message": "Export in progress."},
+            },
+            None,
+        ),
+        (
+            {
+                "id": export_job_id,
+                "status": "SUCCEEDED",
+                "destination": {"file": {"id": file_id}},
+                "progress": {
+                    "message": "Export finished successfully.",
+                    "records": 123,
+                    "bytes": 456,
+                },
+            },
+            None,
+        ),
+        (
+            {
+                "id": export_job_id,
+                "status": "SUCCEEDED",
+                "destination": {"file": {"id": file_id}},
+                "progress": {
+                    "message": "Export finished successfully.",
+                    "records": 123,
+                    "bytes": 456,
+                },
+            },
+            None,
+        ),
+        ({"project_id": project_id}, None),
+        ({"organization_id": org_id}, None),
+        (
+            {"download_url": "https://s3-presigned-url.s3.amazonaws.com/some/bla"},
+            None,
+        ),
+    ]
+
+    cluster_id = gen_uuid()
+
+    mock_response = mock.MagicMock()
+    mock_response.headers = {"Content-Length": 123}
+    mock_response.status_code = 200
+
+    with mock.patch("requests.get", return_value=mock_response):
+        with mock.patch("builtins.open", mock.mock_open(read_data="id,name,path")):
+            cmd = (
+                "croud",
+                "clusters",
+                "export-jobs",
+                "create",
+                "--cluster-id",
+                cluster_id,
+                "--file-format",
+                "csv",
+                "--table",
+                "my-table",
+                "--compression",
+                "gzip",
+            )
+            if save_file:
+                cmd = cmd + (
+                    "--save-as",
+                    "./my_table.csv",
+                )
+            call_command(*cmd)
+
+    body = {
+        "source": {
+            "table": "my-table",
+        },
+        "destination": {"format": "csv"},
+        "compression": "gzip",
+    }
+    assert_rest(
+        mock_client_request,
+        RequestMethod.POST,
+        f"/api/v2/clusters/{cluster_id}/export-jobs/",
+        body=body,
+        any_times=True,
+    )
+    assert_rest(
+        mock_client_request,
+        RequestMethod.GET,
+        f"/api/v2/clusters/{cluster_id}/export-jobs/{export_job_id}/",
+        any_times=True,
+    )
+    assert_rest(
+        mock_client_request,
+        RequestMethod.GET,
+        f"/api/v2/clusters/{cluster_id}/",
+        any_times=True,
+    )
+    assert_rest(
+        mock_client_request,
+        RequestMethod.GET,
+        f"/api/v2/projects/{project_id}/",
+        any_times=True,
+    )
+    assert_rest(
+        mock_client_request,
+        RequestMethod.GET,
+        f"/api/v2/organizations/{org_id}/files/{file_id}/",
+        any_times=True,
+    )
+    if save_file:
+        mock_copy.assert_called_once()
+    else:
+        mock_copy.assert_not_called()
```

### Comparing `croud-1.4.0/tests/commands/test_config.py` & `croud-1.5.0/tests/commands/test_config.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/commands/test_login.py` & `croud-1.5.0/tests/commands/test_login.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/commands/test_logout.py` & `croud-1.5.0/tests/commands/test_logout.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/commands/test_me.py` & `croud-1.5.0/tests/commands/test_me.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/commands/test_organizations.py` & `croud-1.5.0/tests/commands/test_organizations.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,14 +370,35 @@
         ]
     }
     response = organization_role_fqn_transform(user["organization_roles"])
     assert response == "organization_admin"
 
 
 @mock.patch.object(Client, "request", return_value=({}, None))
+def test_organizations_files_get(mock_request):
+    org_id = gen_uuid()
+    file_id = gen_uuid()
+    call_command(
+        "croud",
+        "organizations",
+        "files",
+        "get",
+        "--org-id",
+        org_id,
+        "--file-id",
+        file_id,
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.GET,
+        f"/api/v2/organizations/{org_id}/files/{file_id}/",
+    )
+
+
+@mock.patch.object(Client, "request", return_value=({}, None))
 def test_organizations_files_list(mock_request):
     org_id = gen_uuid()
 
     call_command("croud", "organizations", "files", "list", "--org-id", org_id)
     assert_rest(
         mock_request, RequestMethod.GET, f"/api/v2/organizations/{org_id}/files/"
     )
```

### Comparing `croud-1.4.0/tests/commands/test_products.py` & `croud-1.5.0/tests/commands/test_products.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/commands/test_projects.py` & `croud-1.5.0/tests/commands/test_projects.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/commands/test_regions.py` & `croud-1.5.0/tests/commands/test_regions.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/commands/test_subscriptions.py` & `croud-1.5.0/tests/commands/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/commands/test_users.py` & `croud-1.5.0/tests/commands/test_users.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/conftest.py` & `croud-1.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/test_api.py` & `croud-1.5.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/test_config_schemas.py` & `croud-1.5.0/tests/test_config_schemas.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/test_configuration.py` & `croud-1.5.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/test_parser.py` & `croud-1.5.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/test_printer.py` & `croud-1.5.0/tests/test_printer.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/test_server.py` & `croud-1.5.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/test_util.py` & `croud-1.5.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/util/__init__.py` & `croud-1.5.0/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `croud-1.4.0/tests/util/fake_cloud.py` & `croud-1.5.0/tests/util/fake_cloud.py`

 * *Files identical despite different names*

