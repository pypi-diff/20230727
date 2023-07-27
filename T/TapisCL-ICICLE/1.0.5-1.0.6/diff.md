# Comparing `tmp/TapisCL-ICICLE-1.0.5.tar.gz` & `tmp/TapisCL-ICICLE-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-1.0.5.tar", last modified: Fri Jul 21 20:19:37 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-1.0.6.tar", last modified: Thu Jul 27 21:27:02 2023, max compression
```

## Comparing `TapisCL-ICICLE-1.0.5.tar` & `TapisCL-ICICLE-1.0.6.tar`

### file list

```diff
@@ -1,67 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.214107 TapisCL-ICICLE-1.0.5/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-1.0.5/LICENSE
--rw-rw-rw-   0        0        0    58862 2023-07-21 20:19:37.213106 TapisCL-ICICLE-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    16957 2023-07-21 17:35:54.000000 TapisCL-ICICLE-1.0.5/README.md
--rw-rw-rw-   0        0        0     1249 2023-07-21 20:15:37.000000 TapisCL-ICICLE-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 20:19:37.214107 TapisCL-ICICLE-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.172550 TapisCL-ICICLE-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.176057 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      321 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.179057 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0       84 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0    10916 2023-07-18 21:38:48.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0    16126 2023-07-21 19:28:18.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/client/handlers.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.187565 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.190564 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/
--rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/__init__.py
--rw-rw-rw-   0        0        0    11086 2023-07-21 19:35:57.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/appCommands.py
--rw-rw-rw-   0        0        0      259 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/appConfigGenerator.py
--rw-rw-rw-   0        0        0     4859 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/appForms.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.192567 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Systems/
--rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Systems/__init__.py
--rw-rw-rw-   0        0        0    23546 2023-07-17 15:51:32.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Systems/systemCommands.py
--rw-rw-rw-   0        0        0     3938 2023-07-21 19:22:41.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Systems/systemForms.py
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.195072 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/arguments/
--rw-rw-rw-   0        0        0        0 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/arguments/__init__.py
--rw-rw-rw-   0        0        0     9613 2023-07-21 19:10:55.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/arguments/argument.py
--rw-rw-rw-   0        0        0     4814 2023-07-21 18:30:09.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/arguments/argumentValidators.py
--rw-rw-rw-   0        0        0    21343 2023-07-21 19:33:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0    10976 2023-07-18 20:01:13.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2221 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/commandOpts.py
--rw-rw-rw-   0        0        0     1828 2023-07-18 22:42:23.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     4947 2023-07-10 21:26:23.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/decorators.py
--rw-rw-rw-   0        0        0    12824 2023-07-18 20:04:51.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     7522 2023-07-18 20:00:48.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/jobCommands.py
--rw-rw-rw-   0        0        0    13236 2023-07-18 18:01:26.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.197079 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1727 2023-07-21 20:08:39.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      941 2023-07-21 20:10:12.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     4412 2023-07-17 15:54:36.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0     7990 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/volumeCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.199085 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0    10928 2023-07-06 00:52:04.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/server/auth.py
--rw-rw-rw-   0        0        0    10402 2023-07-17 16:55:28.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      290 2023-07-05 15:04:52.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.201085 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/socketopts/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/socketopts/__init__.py
--rw-rw-rw-   0        0        0     2233 2023-07-10 21:26:16.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/socketopts/schemas.py
--rw-rw-rw-   0        0        0     4810 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/socketopts/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.203593 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-06-16 02:31:56.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1044 2023-06-29 21:33:53.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0     2328 2023-07-08 04:38:18.000000 TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.210108 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    58862 2023-07-21 20:19:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2003 2023-07-21 20:19:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 20:19:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-21 20:19:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      164 2023-07-21 20:19:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-21 20:19:37.000000 TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 20:19:37.211107 TapisCL-ICICLE-1.0.5/tests/
--rw-rw-rw-   0        0        0       48 2023-07-18 20:13:22.000000 TapisCL-ICICLE-1.0.5/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:02.313906 TapisCL-ICICLE-1.0.6/
+-rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0    58862 2023-07-27 21:27:02.313906 TapisCL-ICICLE-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    16957 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/README.md
+-rw-rw-rw-   0        0        0     1249 2023-07-27 21:25:49.000000 TapisCL-ICICLE-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 21:27:02.313906 TapisCL-ICICLE-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:01.880410 TapisCL-ICICLE-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:01.900946 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      321 2023-06-28 16:15:55.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:01.920943 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0    10916 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0    16126 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:02.041296 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:02.073506 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Apps/
+-rw-rw-rw-   0        0        0        0 2023-07-13 16:11:38.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Apps/__init__.py
+-rw-rw-rw-   0        0        0    11086 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Apps/appCommands.py
+-rw-rw-rw-   0        0        0      259 2023-07-14 22:54:08.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Apps/appConfigGenerator.py
+-rw-rw-rw-   0        0        0     4859 2023-07-14 19:32:43.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Apps/appForms.py
+-rw-rw-rw-   0        0        0      216 2023-07-27 21:13:28.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/GlobusProxy.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:02.089503 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Systems/
+-rw-rw-rw-   0        0        0        0 2023-07-13 16:11:31.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Systems/__init__.py
+-rw-rw-rw-   0        0        0    23546 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Systems/systemCommands.py
+-rw-rw-rw-   0        0        0     3938 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Systems/systemForms.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:02.106111 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     9613 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0     4814 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/arguments/argumentValidators.py
+-rw-rw-rw-   0        0        0     2026 2023-07-27 20:53:45.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/authenticatorClients.py
+-rw-rw-rw-   0        0        0    21343 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0    11771 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2221 2023-07-13 18:04:31.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/commandOpts.py
+-rw-rw-rw-   0        0        0     1828 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4947 2023-07-13 23:03:51.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    12824 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     7522 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/jobCommands.py
+-rw-rw-rw-   0        0        0    13866 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:02.130141 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1727 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0     1003 2023-07-27 21:23:21.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     4412 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0     2903 2023-07-27 20:34:13.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/snapshotCommands.py
+-rw-rw-rw-   0        0        0     7990 2023-07-15 00:10:59.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/volumeCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:02.146132 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0    10928 2023-07-07 19:54:35.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0    10402 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      290 2023-07-03 18:17:51.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:02.170131 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2233 2023-07-13 15:48:03.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4810 2023-07-14 16:54:08.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:02.194191 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     2328 2023-07-07 19:32:32.000000 TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:02.297820 TapisCL-ICICLE-1.0.6/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    58862 2023-07-27 21:27:01.000000 TapisCL-ICICLE-1.0.6/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2143 2023-07-27 21:27:01.000000 TapisCL-ICICLE-1.0.6/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 21:27:01.000000 TapisCL-ICICLE-1.0.6/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-27 21:27:01.000000 TapisCL-ICICLE-1.0.6/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      164 2023-07-27 21:27:01.000000 TapisCL-ICICLE-1.0.6/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-27 21:27:01.000000 TapisCL-ICICLE-1.0.6/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-27 23:09:19.000000 TapisCL-ICICLE-1.0.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:27:02.305874 TapisCL-ICICLE-1.0.6/tests/
+-rw-rw-rw-   0        0        0       48 2023-07-27 21:23:03.000000 TapisCL-ICICLE-1.0.6/tests/test.py
```

### Comparing `TapisCL-ICICLE-1.0.5/LICENSE` & `TapisCL-ICICLE-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/PKG-INFO` & `TapisCL-ICICLE-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 1.0.5
+Version: 1.0.6
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-1.0.5/README.md` & `TapisCL-ICICLE-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/pyproject.toml` & `TapisCL-ICICLE-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "poetry-core>=1.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "1.0.5"
+version = "1.0.6"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.6"
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
```

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/client/cli.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/client/handlers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/appCommands.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Apps/appCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Apps/appForms.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Apps/appForms.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Systems/systemCommands.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Systems/systemCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/Systems/systemForms.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/Systems/systemForms.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/arguments/argument.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/arguments/argument.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/arguments/argumentValidators.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/arguments/argumentValidators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/baseCommand.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/commandMap.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .Apps import appCommands
 from .Systems import systemCommands
 import pprint
 
 
 if __name__ != "__main__":
-    from . import volumeCommands, serverCommands, podCommands, fileCommands, dataFormatters, baseCommand, jobCommands
+    from . import authenticatorClients, snapshotCommands, volumeCommands, serverCommands, podCommands, fileCommands, dataFormatters, baseCommand, jobCommands
     from .query import postgres, neo4j
     from utilities import exceptions
     from commands.arguments.argument import Argument
     from commands.commandOpts import CHECK_EXPLICIT_ID
 
 
 class Systems(baseCommand.BaseCommandMap):
@@ -72,15 +72,16 @@
         'start_pod':podCommands.start_pod(),
         'restart_pod':podCommands.restart_pod(),
         'delete_pod':podCommands.delete_pod(),
         'set_pod_perms':podCommands.set_pod_perms(),
         'stop_pod':podCommands.stop_pod(),
         'delete_pod_perms':podCommands.delete_pod_perms(),
         'get_pod_perms':podCommands.get_pod_perms(),
-        'copy_pod_password':podCommands.copy_pod_password(),
+        'get_pod_credentials':podCommands.get_pod_credentials(),
+        'get_pod_uri':podCommands.get_pod_uri(),
         'get_pod_logs':podCommands.get_pod_logs(),
     }
 
 
 class Volumes(baseCommand.BaseCommandMap):
     """
     @help: run operations on tapis volumes and snapshots
@@ -94,23 +95,43 @@
         'update_volume':volumeCommands.update_volume(),
         'delete_volume':volumeCommands.delete_volume(),
         'dir':volumeCommands.dir(),
         'upload_volume':volumeCommands.upload_volume(),
         'set_volume_permission':volumeCommands.set_volume_permission(),
         'get_volume_permissions':volumeCommands.get_volume_permissions(),
         'delete_volume_permission':volumeCommands.delete_volume_permission(),
-        'get_snapshots':volumeCommands.get_snapshots(),
-        'create_snapshot':volumeCommands.create_snapshot(),
-        'get_snapshot':volumeCommands.get_snapshot(),
-        'update_snapshot':volumeCommands.update_snapshot(),
-        'delete_snapshot':volumeCommands.delete_snapshot(),
-        'list_snapshot_files':volumeCommands.list_snapshot_files()
     }
 
 
+class Snapshots(baseCommand.BaseCommandMap):
+    """
+    @help: commands to deal with snapshots
+    """
+    command_map = {
+        'get_snapshots':snapshotCommands.get_snapshots(),
+        'create_snapshot':snapshotCommands.create_snapshot(),
+        'get_snapshot':snapshotCommands.get_snapshot(),
+        'update_snapshot':snapshotCommands.update_snapshot(),
+        'delete_snapshot':snapshotCommands.delete_snapshot(),
+        'list_snapshot_files':snapshotCommands.list_snapshot_files()
+    }
+
+
+class AuthClients(baseCommand.BaseCommandMap):
+    """
+    @help: manage auth clients to be used on your own applications
+    """
+    command_map = {
+        'list_clients': authenticatorClients.list_clients(),
+        'create_client': authenticatorClients.create_client(),
+        'get_client': authenticatorClients.get_client(),
+        'update_client': authenticatorClients.update_client(),
+        'delete_client': authenticatorClients.delete_client()
+    }
+
 class Files(baseCommand.BaseCommandMap):
     """
     @help: run operations on tapis files
     """
     command_map = {
         'ls':fileCommands.ls(),
         'cd':fileCommands.cd(),
@@ -218,15 +239,17 @@
         'Systems': Systems(),
         'General': General(),
         'Pods': Pods(),
         'Files': Files(),
         'Apps': Apps(),
         'Query': Query(),
         'Volumes':Volumes(),
-        'Jobs': Jobs()
+        'Jobs': Jobs(),
+        'Snapshots': Snapshots(),
+        'AuthClients': AuthClients()
     }
     def __init__(self):
         truncated_arguments = self.generate_truncated_arguments(self.arguments)
         for command in self.aggregate_command_map.values():
             command.update_args_with_truncated(truncated_arguments)
         for name, argument in self.arguments.items():
             argument.truncated_arg = truncated_arguments[name]
```

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/commandOpts.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/commandOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/dataFormatters.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/decorators.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/fileCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/jobCommands.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/jobCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/podCommands.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/podCommands.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,26 +246,43 @@
         Argument('pod_id', positional=True),
     ]
     async def run(self, *args, **kwargs) -> str: # return a list of permissions on a given pod
         return_information = self.t.pods.get_pod_permissions(pod_id=kwargs['pod_id'])
         return return_information
 
 
-class copy_pod_password(baseCommand.BaseCommand):
+class get_pod_credentials(baseCommand.BaseCommand):
     """
     @help: copy the pod password to the clipboard
     """
     required_arguments=[
         Argument('pod_id', positional=True),
     ]
     async def run(self, *args, **kwargs) -> str: # copies the pod password to clipboard so that the user can access the pod via the neo4j desktop app. Maybe a security risk? not as bad as printing passwords out!
-        password = self.t.pods.get_pod_credentials(pod_id=kwargs['pod_id']).user_password
+        creds = self.t.pods.get_pod_credentials(pod_id=kwargs['pod_id'])
+        username = creds.user_username
+        password = creds.user_password
         pyperclip.copy(password)
         password = None
-        return 'copied to clipboard'
+        return f'Username: {username}\nCopied password to clipboard'
+    
+
+class get_pod_uri(baseCommand.BaseCommand):
+    """
+    @help: get the URI for a pod
+    """
+    required_arguments = [
+        Argument('pod_id')
+    ]
+    async def run(self, *args, **kwargs):
+        pod_template = self.t.pods.get_pod(pod_id=kwargs["pod_id"]).pod_template
+        if pod_template == 'template/neo4j':
+            return f"bolt+ssc://{kwargs['id']}.pods.{self.t.base_url.split('https://')[1]}:443"
+        else:
+            return f"{kwargs['id']}.pods.{self.t.base_url.split('https://')[1]}"
 
 
 class get_pod_logs(baseCommand.BaseCommand):
     """
     @help: retrieve the logs of an active pod and either print them to the console, or write them to the specified file
     """
     return_fields = ['logs']
```

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/commands/volumeCommands.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/commands/volumeCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/server/auth.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/server/auth.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/server/server.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/socketopts/schemas.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/socketopts/socketOpts.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/socketopts/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-1.0.6/src/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-1.0.6/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 1.0.5
+Version: 1.0.6
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-1.0.5/src/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-1.0.6/src/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 src/__init__.py
 src/TapisCLICICLE/__init__.py
 src/TapisCLICICLE/__main__.py
 src/TapisCLICICLE/serverRun.py
 src/TapisCLICICLE/client/__init__.py
 src/TapisCLICICLE/client/cli.py
 src/TapisCLICICLE/client/handlers.py
+src/TapisCLICICLE/commands/GlobusProxy.py
 src/TapisCLICICLE/commands/__init__.py
+src/TapisCLICICLE/commands/authenticatorClients.py
 src/TapisCLICICLE/commands/baseCommand.py
 src/TapisCLICICLE/commands/commandMap.py
 src/TapisCLICICLE/commands/commandOpts.py
 src/TapisCLICICLE/commands/dataFormatters.py
 src/TapisCLICICLE/commands/decorators.py
 src/TapisCLICICLE/commands/fileCommands.py
 src/TapisCLICICLE/commands/jobCommands.py
 src/TapisCLICICLE/commands/podCommands.py
 src/TapisCLICICLE/commands/serverCommands.py
+src/TapisCLICICLE/commands/snapshotCommands.py
 src/TapisCLICICLE/commands/volumeCommands.py
 src/TapisCLICICLE/commands/Apps/__init__.py
 src/TapisCLICICLE/commands/Apps/appCommands.py
 src/TapisCLICICLE/commands/Apps/appConfigGenerator.py
 src/TapisCLICICLE/commands/Apps/appForms.py
 src/TapisCLICICLE/commands/Systems/__init__.py
 src/TapisCLICICLE/commands/Systems/systemCommands.py
```

