# Comparing `tmp/remotemanager-0.9.5.tar.gz` & `tmp/remotemanager-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.9.5.tar", last modified: Wed Jul 26 10:32:40 2023, max compression
+gzip compressed data, was "remotemanager-0.9.6.tar", last modified: Thu Jul 27 15:22:59 2023, max compression
```

## Comparing `remotemanager-0.9.5.tar` & `remotemanager-0.9.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.943266 remotemanager-0.9.5/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-26 10:32:40.943266 remotemanager-0.9.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.9.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-25 14:08:53.000000 remotemanager-0.9.5/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.935266 remotemanager-0.9.5/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-25 14:08:53.000000 remotemanager-0.9.5/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.939266 remotemanager-0.9.5/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.9.5/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.939266 remotemanager-0.9.5/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.9.5/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.9.5/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.9.5/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.9.5/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.9.5/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:58.000000 remotemanager-0.9.5/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.939266 remotemanager-0.9.5/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    54656 2023-07-26 09:18:43.000000 remotemanager-0.9.5/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    10415 2023-07-26 09:18:43.000000 remotemanager-0.9.5/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-12 13:38:06.000000 remotemanager-0.9.5/remotemanager/dataset/lazy_append.py
--rw-rw-rw-   0 root         (0) root         (0)    23093 2023-07-26 09:18:43.000000 remotemanager-0.9.5/remotemanager/dataset/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-24 14:12:05.000000 remotemanager-0.9.5/remotemanager/dataset/runnerstates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.939266 remotemanager-0.9.5/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.5/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:28.000000 remotemanager-0.9.5/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.939266 remotemanager-0.9.5/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.9.5/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.9.5/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.5/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.5/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.943266 remotemanager-0.9.5/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.9.5/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.5/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.5/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.943266 remotemanager-0.9.5/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.5/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.9.5/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.5/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.943266 remotemanager-0.9.5/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.5/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.9.5/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:28.000000 remotemanager-0.9.5/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.943266 remotemanager-0.9.5/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.5/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.9.5/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:32:40.935266 remotemanager-0.9.5/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-26 10:32:40.000000 remotemanager-0.9.5/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-26 10:32:40.000000 remotemanager-0.9.5/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 10:32:40.000000 remotemanager-0.9.5/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-26 10:32:40.000000 remotemanager-0.9.5/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-26 10:32:40.000000 remotemanager-0.9.5/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 10:32:40.943266 remotemanager-0.9.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.005945 remotemanager-0.9.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-27 15:22:59.005945 remotemanager-0.9.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:43:02.000000 remotemanager-0.9.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-27 12:24:05.000000 remotemanager-0.9.6/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:58.997944 remotemanager-0.9.6/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-27 12:24:05.000000 remotemanager-0.9.6/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:58.997944 remotemanager-0.9.6/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:02.000000 remotemanager-0.9.6/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:58.997944 remotemanager-0.9.6/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:10.000000 remotemanager-0.9.6/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:40:04.000000 remotemanager-0.9.6/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:40:04.000000 remotemanager-0.9.6/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 07:32:25.000000 remotemanager-0.9.6/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:40:04.000000 remotemanager-0.9.6/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:57.000000 remotemanager-0.9.6/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.001945 remotemanager-0.9.6/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    55330 2023-07-27 14:22:14.000000 remotemanager-0.9.6/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    10415 2023-07-26 09:18:44.000000 remotemanager-0.9.6/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-13 05:21:38.000000 remotemanager-0.9.6/remotemanager/dataset/lazy_append.py
+-rw-rw-rw-   0 root         (0) root         (0)    23093 2023-07-26 09:18:44.000000 remotemanager-0.9.6/remotemanager/dataset/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-24 14:12:04.000000 remotemanager-0.9.6/remotemanager/dataset/runnerstates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.001945 remotemanager-0.9.6/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.6/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:27.000000 remotemanager-0.9.6/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.001945 remotemanager-0.9.6/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:02.000000 remotemanager-0.9.6/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:37.000000 remotemanager-0.9.6/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.6/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.6/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.001945 remotemanager-0.9.6/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:49.000000 remotemanager-0.9.6/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.6/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.6/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.001945 remotemanager-0.9.6/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.6/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:30.000000 remotemanager-0.9.6/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.6/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.005945 remotemanager-0.9.6/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.6/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:31.000000 remotemanager-0.9.6/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:27.000000 remotemanager-0.9.6/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:59.005945 remotemanager-0.9.6/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.6/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-21 10:04:17.000000 remotemanager-0.9.6/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 09:35:30.000000 remotemanager-0.9.6/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:22:58.997944 remotemanager-0.9.6/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-27 15:22:58.000000 remotemanager-0.9.6/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-07-27 15:22:58.000000 remotemanager-0.9.6/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 15:22:58.000000 remotemanager-0.9.6/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-27 15:22:58.000000 remotemanager-0.9.6/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-27 15:22:58.000000 remotemanager-0.9.6/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 15:22:59.005945 remotemanager-0.9.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.6/setup.py
```

### Comparing `remotemanager-0.9.5/LICENSE` & `remotemanager-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/PKG-INFO` & `remotemanager-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.5
+Version: 0.9.6
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.5/README.md` & `remotemanager-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/pyproject.toml` & `remotemanager-0.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.9.5"
+current_version = "0.9.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.9.5/remotemanager/connection/cmd.py` & `remotemanager-0.9.6/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/connection/computers/base.py` & `remotemanager-0.9.6/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/connection/computers/example.py` & `remotemanager-0.9.6/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/connection/computers/options.py` & `remotemanager-0.9.6/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/connection/computers/parsers.py` & `remotemanager-0.9.6/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/connection/testing_object.py` & `remotemanager-0.9.6/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/connection/url.py` & `remotemanager-0.9.6/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/dataset/dataset.py` & `remotemanager-0.9.6/remotemanager/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -742,17 +742,53 @@
         if not dependency_call and self.dependency is not None:
             return self.dependency.clear_results(wipe)
 
         self._logger.runtime("clearing results")
         for runner in self.runners:
             runner.clear_result(wipe)
 
+    def collect_files(self, remote_check: bool) -> list:
+        """
+        Collect created files
+
+        Args:
+            remote_check:
+                search for remote paths if True
+        Returns:
+            list of filepaths
+        """
+        target = "remote" if remote_check else "local"
+        fld = "remote_dir" if remote_check else "local_dir"
+
+        targets = [
+            self.master_script.__getattribute__(target),
+            self.repofile.__getattribute__(target),
+        ]
+        # grab all runner files
+        for runner in self.runners:
+            # start with constants
+            targets += [
+                runner.jobscript.__getattribute__(target),
+                runner.runfile.__getattribute__(target),
+                runner.resultfile.__getattribute__(target),
+                runner.errorfile.__getattribute__(target),
+            ]
+
+            # need extra files, within their remote/local dir
+            for file in runner.extra_files["send"] + runner.extra_files["recv"]:
+                targets.append(f"{runner.__getattribute__(fld)}/{file}")
+
+        # minimize length
+        targets = list(set(targets))
+
+        return targets
+
     def wipe_local(
         self,
-        files_only: bool = False,
+        files_only: bool = True,
         dry_run: bool = False,
         dependency_call: bool = False,
     ) -> None:
         """
         Clear out the local directory
 
         Args:
@@ -779,46 +815,51 @@
         if not check_dir_is_child(os.getcwd(), self.local_dir):
             raise RuntimeError(
                 f"local dir {self.local_dir} is not a child directory, "
                 f"deleting could have catastrophic effects"
             )
 
         self._logger.debug("wiping local")
-        locals = [self.local_dir]
-        for runner in self.runners:
-            if runner.local_dir not in locals:
-                locals.append(runner.local_dir)
 
-        self._logger.debug(f"locals: {format_iterable(locals)}")
-        if dry_run:
-            for local in locals:
-                print(f"targeting {local} for wipe")
+        if not files_only:
+            targets = [self.local_dir]
+            for runner in self.runners:
+                if runner.local_dir not in targets:
+                    targets.append(runner.local_dir)
 
-        elif not files_only:
-            for local in locals:
+            self._logger.debug(f"locals: {format_iterable(targets)}")
+            if dry_run:
+                for local in targets:
+                    print(f"targeting local {local} for wipe")
+
+            for local in targets:
                 try:
                     shutil.rmtree(local)
                     self._logger.debug(f"{local} removed")
                 except FileNotFoundError:
                     self._logger.debug(f"{local} not found")
 
         else:
             self._logger.debug("file only wipe")
-            for local in locals:
-                for file in os.listdir(local):
-                    path = f"{local}/{file}"
-                    try:
-                        os.remove(path)
-                        self._logger.debug(f"{path} removed")
-                    except FileNotFoundError:
-                        self._logger.debug(f"{path} not found")
+            targets = self.collect_files(remote_check=False)
+
+            if dry_run:
+                for local in targets:
+                    print(f"targeting local {local} for wipe")
+
+            for path in targets:
+                try:
+                    os.remove(path)
+                    self._logger.debug(f"{path} removed")
+                except FileNotFoundError:
+                    self._logger.debug(f"{path} not found")
 
     def wipe_remote(
         self,
-        files_only: bool = False,
+        files_only: bool = True,
         dry_run: bool = False,
         dependency_call: bool = False,
     ) -> None:
         """
         Clear out the remote directory (including run dir)
 
         Args:
@@ -845,52 +886,38 @@
                     remotes.append(runner.remote_dir)
                 if runner.run_path not in remotes:
                     remotes.append(runner.run_path)
 
             self._logger.debug(f"remotes: {format_iterable(remotes)}")
             if dry_run:
                 for remote in remotes:
-                    print(f"targeting {remote} for wipe")
+                    print(f"targeting remote {remote} for wipe")
 
             remotestr = ",".join(remotes)
             cmd = f"rm -rf {{{remotestr}}}"
 
             self.url.cmd(cmd)
 
         else:
             self._logger.debug("file only wipe")
-            # prime with dataset native files
-            targets = [self.master_script.remote, self.repofile.remote]
-            # grab all runner files
-            for runner in self.runners:
-                # start with constants
-                targets += [
-                    runner.jobscript.remote,
-                    runner.runfile.remote,
-                    runner.resultfile.remote,
-                    runner.errorfile.remote,
-                ]
-                # need extra files, within their remote dir
-                for file in runner.extra_files["send"] + runner.extra_files["recv"]:
-                    targets.append(f"{runner.remote_dir}/{file}")
-            # minimize command length
-            targets = list(set(targets))
+            targets = self.collect_files(remote_check=True)
 
             cmd = ",".join(targets)
             cmd = f"rm -f {{{cmd}}}"
 
             if dry_run:
-                print(f"removal command: {cmd}")
+                for remote in targets:
+                    print(f"targeting remote {remote} for wipe")
                 return
 
             self.url.cmd(cmd)
 
     def hard_reset(
         self,
-        files_only: bool = False,
+        files_only: bool = True,
         dry_run: bool = False,
         dependency_call: bool = False,
     ) -> None:
         """
         Hard reset the dataset, including wiping local and remote folders
 
         Args:
```

### Comparing `remotemanager-0.9.5/remotemanager/dataset/dependency.py` & `remotemanager-0.9.6/remotemanager/dataset/dependency.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/dataset/lazy_append.py` & `remotemanager-0.9.6/remotemanager/dataset/lazy_append.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/dataset/runner.py` & `remotemanager-0.9.6/remotemanager/dataset/runner.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/dataset/runnerstates.py` & `remotemanager-0.9.6/remotemanager/dataset/runnerstates.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/jupyter/magic.py` & `remotemanager-0.9.6/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/logging/__init__.py` & `remotemanager-0.9.6/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/logging/log.py` & `remotemanager-0.9.6/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/logging/utils.py` & `remotemanager-0.9.6/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/logging/verbosity.py` & `remotemanager-0.9.6/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/serialisation/__init__.py` & `remotemanager-0.9.6/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/serialisation/serial.py` & `remotemanager-0.9.6/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.9.6/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.9.6/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/storage/database.py` & `remotemanager-0.9.6/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/storage/function.py` & `remotemanager-0.9.6/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/storage/remotefunction.py` & `remotemanager-0.9.6/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/storage/sendablemixin.py` & `remotemanager-0.9.6/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/storage/trackedfile.py` & `remotemanager-0.9.6/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/transport/cp.py` & `remotemanager-0.9.6/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/transport/rsync.py` & `remotemanager-0.9.6/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/transport/scp.py` & `remotemanager-0.9.6/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/transport/transport.py` & `remotemanager-0.9.6/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/utils/__init__.py` & `remotemanager-0.9.6/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/utils/flags.py` & `remotemanager-0.9.6/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager/utils/version.py` & `remotemanager-0.9.6/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.5/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.9.6/remotemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.5
+Version: 0.9.6
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.5/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.9.6/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

