# Comparing `tmp/devcycle-python-server-sdk-3.3.3.tar.gz` & `tmp/devcycle-python-server-sdk-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/devcycle-python-server-sdk-3.3.3.tar", last modified: Fri Jul 21 20:44:11 2023, max compression
+gzip compressed data, was "dist/devcycle-python-server-sdk-3.3.4.tar", last modified: Thu Jul 27 14:39:11 2023, max compression
```

## Comparing `devcycle-python-server-sdk-3.3.3.tar` & `devcycle-python-server-sdk-3.3.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/bucketing_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/config_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/event_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/local_bucketing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/managers/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/managers/event_queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/bucketed_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/platform_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/protobuf/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/util/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/example/cloud_client_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/example/local_bucketing_client_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/test/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/api/test_bucketing_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/api/test_config_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/api/test_event_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/api/test_local_bucketing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/test/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/fixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/fixture/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/test/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/managers/test_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/managers/test_event_queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/test/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/models/test_bucketed_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/test_cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/test_local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:44:11.000000 devcycle-python-server-sdk-3.3.3/test/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/util/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-21 20:43:57.000000 devcycle-python-server-sdk-3.3.3/test/util/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/bucketing_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/config_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/event_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16332 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/local_bucketing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/managers/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/managers/event_queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/bucketed_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/platform_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/protobuf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/example/cloud_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/example/local_bucketing_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/test/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/api/test_bucketing_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/api/test_config_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/api/test_event_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/api/test_local_bucketing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/test/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/fixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/fixture/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/test/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/managers/test_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/managers/test_event_queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/test/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/models/test_bucketed_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/test_cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/test_local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/test/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/util/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/util/test_version.py
```

### Comparing `devcycle-python-server-sdk-3.3.3/README.md` & `devcycle-python-server-sdk-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/bucketing_client.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/config_client.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/config_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/event_client.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/event_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/api/local_bucketing.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/local_bucketing.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
         wasm_linker.define_func(
             "env", "seed", FuncType([], [ValType.f64()]), __seed_func
         )
 
         def __console_log_func(message_ptr) -> None:
             message: str = self._read_assembly_script_string(message_ptr)
-            logger.warning(f"WASM console: {message!r}")
+            logger.warning(f"DevCycle: WASM console: {message!r}")
 
         wasm_linker.define_func(
             "env", "console.log", FuncType([ValType.i32()], []), __console_log_func
         )
 
         wasm_instance = wasm_linker.instantiate(wasm_store, wasm_module)
         self.wasm_instance = wasm_instance
```

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/cloud_client.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/cloud_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,33 +69,33 @@
 
         if default_value is None:
             raise ValueError("Missing parameter: defaultValue")
 
         try:
             variable = self.bucketing_api.variable(key, user)
         except CloudClientUnauthorizedError as e:
-            logger.warning("DevCycle SDK key is invalid, unable to make cloud request")
+            logger.warning("DevCycle: SDK key is invalid, unable to make cloud request")
             raise e
         except NotFoundError:
-            logger.warning(f"Variable not found: {key}")
+            logger.warning(f"DevCycle: Variable not found: {key}")
             return Variable.create_default_variable(
                 key=key, default_value=default_value
             )
         except Exception as e:
-            logger.error(f"Error evaluating variable: {e}")
+            logger.error(f"DevCycle: Error evaluating variable: {e}")
             return Variable.create_default_variable(
                 key=key, default_value=default_value
             )
 
         variable.defaultValue = default_value
 
         # Allow default value to be a subclass of the same type as the variable
         if not isinstance(default_value, type(variable.value)):
             logger.warning(
-                f"Variable {key} is type {type(variable.value)}, but default value is type {type(default_value)}",
+                f"DevCycle: Variable {key} is type {type(variable.value)}, but default value is type {type(default_value)}",
             )
             return Variable.create_default_variable(
                 key=key, default_value=default_value
             )
 
         return variable
 
@@ -108,18 +108,18 @@
         _validate_user(user)
         user = self._add_platform_data_to_user(user)
 
         variable_map: Dict[str, Variable] = {}
         try:
             variable_map = self.bucketing_api.variables(user)
         except CloudClientUnauthorizedError as e:
-            logger.warning("SDK key is invalid, unable to make cloud request")
+            logger.warning("DevCycle: SDK key is invalid, unable to make cloud request")
             raise e
         except Exception as e:
-            logger.error(f"Error retrieving all features for a user: {e}")
+            logger.error(f"DevCycle: Error retrieving all features for a user: {e}")
 
         return variable_map
 
     def all_features(self, user: DevCycleUser) -> Dict[str, Feature]:
         """
         Returns all segmented and bucketed features for a user.  This method will return an empty map if the user is not bucketed into any features
 
@@ -128,18 +128,18 @@
         _validate_user(user)
         user = self._add_platform_data_to_user(user)
 
         feature_map: Dict[str, Feature] = {}
         try:
             feature_map = self.bucketing_api.features(user)
         except CloudClientUnauthorizedError as e:
-            logger.warning("SDK key is invalid, unable to make cloud request")
+            logger.warning("DevCycle: SDK key is invalid, unable to make cloud request")
             raise e
         except Exception as e:
-            logger.error(f"Error retrieving all features for a user: {e}")
+            logger.error(f"DevCycle: Error retrieving all features for a user: {e}")
 
         return feature_map
 
     def track(self, user: DevCycleUser, user_event: DevCycleEvent) -> None:
         """
         Tracks a custom event for a user.
 
@@ -156,18 +156,18 @@
         if user_event is None or not user_event.type:
             raise ValueError("Invalid Event")
 
         events = [user_event]
         try:
             self.bucketing_api.track(user, events)
         except CloudClientUnauthorizedError as e:
-            logger.warning("SDK key is invalid, unable to make cloud request")
+            logger.warning("DevCycle: SDK key is invalid, unable to make cloud request")
             raise e
         except Exception as e:
-            logger.error(f"Error tracking event: {e}")
+            logger.error(f"DevCycle: Error tracking event: {e}")
 
 
 def _validate_sdk_key(sdk_key: str) -> None:
     if sdk_key is None or len(sdk_key) == 0:
         raise ValueError("Missing SDK key! Call initialize with a valid SDK key")
 
     if not sdk_key.startswith("server") and not sdk_key.startswith("dvc_server"):
```

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/exceptions.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/local_client.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/local_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,23 +53,25 @@
         decisions. This data will be merged with any custom data set on the user object, with user data
         taking priority
 
         :param custom_data: Global data to set.  Supported values are strings, numbers, booleans. Nested dictionaries
         are not permitted
         """
         if not self.is_initialized():
-            logger.debug("set_client_custom_data called before client has initialized")
+            logger.debug(
+                "DevCycle: set_client_custom_data called before client has initialized"
+            )
             return
 
         if custom_data:
             try:
                 custom_data_json = json.dumps(custom_data)
                 self.local_bucketing.set_client_custom_data(custom_data_json)
             except Exception as e:
-                logger.error("Error setting custom data: " + str(e))
+                logger.error("DevCycle: Error setting custom data: " + str(e))
 
     def variable_value(self, user: DevCycleUser, key: str, default_value: Any) -> Any:
         """
         Evaluates a variable for a user and returns the value.  If the user is not bucketed into the variable, the default value will be returned
 
         :param user: The user to evaluate the variable for
         """
@@ -88,38 +90,38 @@
         if not key:
             raise ValueError("Missing parameter: key")
 
         if default_value is None:
             raise ValueError("Missing parameter: defaultValue")
 
         if not self.is_initialized():
-            logger.debug("variable called before client has initialized")
+            logger.debug("DevCycle: variable called before client has initialized")
             try:
                 self.event_queue_manager.queue_aggregate_event(
                     event=DevCycleEvent(
                         type=EventType.AggVariableDefaulted, target=key, value=1
                     ),
                     bucketed_config=None,
                 )
             except Exception as e:
                 logger.warning(
-                    f"Unable to track AggVariableDefaulted event for Variable {key}: {e}"
+                    f"DevCycle: Unable to track AggVariableDefaulted event for Variable {key}: {e}"
                 )
             return Variable.create_default_variable(key, default_value)
 
         try:
             variable = self.local_bucketing.get_variable_for_user_protobuf(
                 user, key, default_value
             )
             if variable:
                 return variable
         except VariableTypeMismatchError:
-            logger.debug("Variable type mismatch, returning default value")
+            logger.debug("DevCycle: Variable type mismatch, returning default value")
         except Exception as e:
-            logger.warning(f"Error retrieving variable for user: {e}")
+            logger.warning(f"DevCycle: Error retrieving variable for user: {e}")
 
         return Variable.create_default_variable(key, default_value)
 
     def _generate_bucketed_config(self, user: DevCycleUser) -> BucketedConfig:
         """
         Generates a bucketed config for a user.  This method will return an empty config if the client has not been initialized or if the user is not bucketed into any features or variables
         """
@@ -133,44 +135,50 @@
         Returns all segmented and bucketed variables for a user.  This method will return an empty map if the client has not been initialized or if the user is not bucketed into any variables
 
         :param user: The user to retrieve variables for
         """
         _validate_user(user)
 
         if not self.is_initialized():
-            logger.warning("all_variables called before client has initialized")
+            logger.warning(
+                "DevCycle: all_variables called before client has initialized"
+            )
             return {}
 
         variable_map: Dict[str, Variable] = {}
 
         try:
             return self.local_bucketing.generate_bucketed_config(user).variables
         except Exception as e:
-            logger.exception(f"Error retrieving all variables for a user: {e}")
+            logger.exception(
+                f"DevCycle: Error retrieving all variables for a user: {e}"
+            )
             return {}
 
         return variable_map
 
     def all_features(self, user: DevCycleUser) -> Dict[str, Feature]:
         """
         Returns all segmented and bucketed features for a user.  This method will return an empty map if the client has not been initialized or if the user is not bucketed into any features
 
         :param user: The user to retrieve features for
         """
         _validate_user(user)
 
         if not self.is_initialized():
-            logger.warning("all_features called before client has initialized")
+            logger.warning(
+                "DevCycle: all_features called before client has initialized"
+            )
             return {}
 
         feature_map: Dict[str, Feature] = {}
         try:
             return self.local_bucketing.generate_bucketed_config(user).features
         except Exception as e:
-            logger.exception(f"Error retrieving all features for a user: {e}")
+            logger.exception(f"DevCycle: Error retrieving all features for a user: {e}")
 
         return feature_map
 
     def track(self, user: DevCycleUser, user_event: DevCycleEvent) -> None:
         """
         Tracks a custom event for a user.  This method will return immediately and the event will be queued for processing in the background.  If the client has not been initialized, this method will return immediately and the event will be discarded.
 
@@ -182,21 +190,21 @@
         if user_event is None:
             raise ValueError("Invalid Event")
 
         if user_event.type is None or len(user_event.type) == 0:
             raise ValueError("Missing parameter: type")
 
         if not self.is_initialized():
-            logger.debug("track called before client has initialized")
+            logger.debug("DevCycle: track called before client has initialized")
             return
 
         try:
             self.event_queue_manager.queue_event(user, user_event)
         except Exception as e:
-            logger.error(f"Error tracking event: {e}")
+            logger.error(f"DevCycle: Error tracking event: {e}")
 
     def close(self) -> None:
         """
         Closes the client and releases any resources held by it.
         """
         self.config_manager.close()
         self.event_queue_manager.close()
```

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/managers/config_manager.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/managers/config_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
             if new_config is None and new_etag == self._config_etag:
                 # api not returning data and the etag is the same
                 # no change to the config since last request
                 return
             elif new_config is None:
                 logger.warning(
-                    "Config CDN fetch returned no data with a different etag"
+                    "DevCycle: Config CDN fetch returned no data with a different etag"
                 )
                 return
 
             trigger_on_client_initialized = self._config is None
 
             self._config = new_config
             self._config_etag = new_etag
@@ -69,27 +69,31 @@
                 and self._options.on_client_initialized is not None
             ):
                 try:
                     self._options.on_client_initialized()
                 except Exception as e:
                     # consume any error
                     logger.warning(
-                        f"Error received from on_client_initialized callback: {str(e)}"
+                        f"DevCycle: Error received from on_client_initialized callback: {str(e)}"
                     )
         except CloudClientError as e:
-            logger.warning(f"Config fetch failed. Status: {str(e)}")
+            logger.warning(f"DevCycle: Config fetch failed. Status: {str(e)}")
         except CloudClientUnauthorizedError:
-            logger.error("Unauthorized to get config. Aborting config polling.")
+            logger.error(
+                "DevCycle: Unauthorized to get config. Aborting config polling."
+            )
             self._polling_enabled = False
 
     def run(self):
         while self._polling_enabled:
             try:
                 self._get_config()
             except Exception as e:
                 if self._polling_enabled:
                     # Only log a warning if we're still polling
-                    logger.warning(f"Error polling for config changes: {str(e)}")
+                    logger.warning(
+                        f"DevCycle: Error polling for config changes: {str(e)}"
+                    )
             time.sleep(self._options.config_polling_interval_ms / 1000.0)
 
     def close(self):
         self._polling_enabled = False
```

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/managers/event_queue_manager.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/managers/event_queue_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,46 +87,48 @@
         if self._flush_lock.locked():
             return 0
 
         with self._flush_lock:
             try:
                 payloads = self._local_bucketing.flush_event_queue()
             except Exception as e:
-                logger.error(f"Error flushing event payloads: {str(e)}")
+                logger.error(f"DevCycle: Error flushing event payloads: {str(e)}")
 
             event_count = 0
             if payloads:
-                logger.debug(f"Flush {len(payloads)} event payloads")
+                logger.debug(f"DevCycle: Flush {len(payloads)} event payloads")
                 for payload in payloads:
                     event_count += payload.eventCount
                     self._publish_event_payload(payload)
-                logger.debug(f"Flush {event_count} events, for {len(payloads)} users")
+                logger.debug(
+                    f"DevCycle: Flush {event_count} events, for {len(payloads)} users"
+                )
             return event_count
 
     def _publish_event_payload(self, payload: FlushPayload) -> None:
         if payload and payload.records:
             try:
                 self._event_api_client.publish_events(payload.records)
                 self._local_bucketing.on_event_payload_success(payload.payloadId)
             except APIClientUnauthorizedError:
                 logger.error(
-                    "Unauthorized to publish events, please check your SDK key"
+                    "DevCycle: Unauthorized to publish events, please check your SDK key"
                 )
                 # stop the thread
                 self._stop_running()
                 self._local_bucketing.on_event_payload_failure(payload.payloadId, False)
             except NotFoundError as e:
                 logger.error(
-                    f"Unable to reach the DevCycle Events API service: {str(e)}"
+                    f"DevCycle: Unable to reach the DevCycle Events API service: {str(e)}"
                 )
                 self._stop_running()
                 self._local_bucketing.on_event_payload_failure(payload.payloadId, False)
             except APIClientError as e:
                 logger.warning(
-                    f"Error publishing events to DevCycle Events API service: {str(e)}"
+                    f"DevCycle: Error publishing events to DevCycle Events API service: {str(e)}"
                 )
                 self._local_bucketing.on_event_payload_failure(payload.payloadId, True)
 
     def is_event_logging_disabled(self, event_type: str) -> bool:
         if event_type in [
             EventType.VariableDefaulted,
             EventType.VariableEvaluated,
@@ -138,48 +140,50 @@
             return self._options.disable_custom_event_logging
 
     def run(self):
         while self._should_run():
             try:
                 self._flush_events()
             except Exception as e:
-                logger.warning(f"Error flushing events: {str(e)}")
+                logger.warning(f"DevCycle: flushing events: {str(e)}")
 
             self._sleep()
 
         self._mark_exited()
 
     def close(self):
         self._stop_running()
 
         # Wait up to 1s for the thread to exit.
         # Because the sleeping between batches is interruptible, this is only
         # providing time for an in-flight batch to finish.
         if not self._wait_for_exit(1.0):
-            logger.error("Timed out waiting for event flushing thread to stop")
+            logger.error(
+                "DevCycle: Timed out waiting for event flushing thread to stop"
+            )
 
         try:
             self._flush_events()
         except Exception as e:
-            logger.warning(f"DVC Error flushing events when closing client: {str(e)}")
+            logger.warning(f"DevCycle: flushing events when closing client: {str(e)}")
 
     def queue_event(self, user: DevCycleUser, event: DevCycleEvent) -> None:
         if user is None:
             raise ValueError("user cannot be None")
 
         if event is None:
             raise ValueError("event cannot be None")
 
         if not event.type:
             raise ValueError("event type not set")
 
         try:
             self._check_queue_status()
         except QueueFullError:
-            logger.warning("Event queue is full, dropping user event")
+            logger.warning("DevCycle: Event queue is full, dropping user event")
             return
 
         user_json = json.dumps(user.to_json())
         event_json = json.dumps(event.to_json())
         self._local_bucketing.queue_event(user_json, event_json)
 
     def queue_aggregate_event(
@@ -193,15 +197,15 @@
 
         if not event.target:
             raise ValueError("event target not set")
 
         try:
             self._check_queue_status()
         except QueueFullError:
-            logger.warning("Event queue is full, dropping aggregate event")
+            logger.warning("DevCycle: Event queue is full, dropping aggregate event")
             return
 
         event_json = json.dumps(event.to_json())
         if bucketed_config and bucketed_config.variable_variation_map:
             variation_map_json = json.dumps(bucketed_config.variable_variation_map)
         else:
             variation_map_json = "{}"
```

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/bucketed_config.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/bucketed_config.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/event.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/event.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/feature.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/feature.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/platform_data.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/platform_data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/user.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/models/variable.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/variable.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/options.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,39 +59,39 @@
         self.config_retry_delay_ms = config_retry_delay_ms
         self.on_client_initialized = on_client_initialized
         self.event_request_timeout_ms = event_request_timeout_ms
         self.event_retry_delay_ms = event_retry_delay_ms
 
         if self.flush_event_queue_size >= self.max_event_queue_size:
             logger.warning(
-                f"flush_event_queue_size: {self.flush_event_queue_size} must be smaller than max_event_queue_size: {self.max_event_queue_size}"
+                f"DevCycle: flush_event_queue_size: {self.flush_event_queue_size} must be smaller than max_event_queue_size: {self.max_event_queue_size}"
             )
             self.flush_event_queue_size = self.max_event_queue_size - 1
 
         if self.event_request_chunk_size > self.flush_event_queue_size:
             logger.warning(
-                f"event_request_chunk_size: {self.event_request_chunk_size} must be smaller than flush_event_queue_size: {self.flush_event_queue_size}"
+                f"DevCycle: event_request_chunk_size: {self.event_request_chunk_size} must be smaller than flush_event_queue_size: {self.flush_event_queue_size}"
             )
             self.event_request_chunk_size = 100
 
         if self.event_request_chunk_size > self.max_event_queue_size:
             logger.warning(
-                f"event_request_chunk_size: {self.event_request_chunk_size} must be smaller than max_event_queue_size: { self.max_event_queue_size}"
+                f"DevCycle: event_request_chunk_size: {self.event_request_chunk_size} must be smaller than max_event_queue_size: { self.max_event_queue_size}"
             )
             self.event_request_chunk_size = 100
 
         if self.flush_event_queue_size > 20000:
             logger.warning(
-                f"flush_event_queue_size: {self.flush_event_queue_size} must be smaller than 20,000"
+                f"DevCycle: flush_event_queue_size: {self.flush_event_queue_size} must be smaller than 20,000"
             )
             self.flush_event_queue_size = 20000
 
         if self.max_event_queue_size > 20000:
             logger.warning(
-                f"max_event_queue_size: {self.max_event_queue_size} must be smaller than 20,000"
+                f"DevCycle: max_event_queue_size: {self.max_event_queue_size} must be smaller than 20,000"
             )
             self.max_event_queue_size = 20000
 
     def event_queue_options(self) -> Dict[str, Any]:
         """
         Returns a read-only view of the options that are relevant to the event subsystem
         """
```

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/protobuf/utils.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/protobuf/utils.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py` & `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/devcycle_python_server_sdk.egg-info/SOURCES.txt` & `devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/example/cloud_client_example.py` & `devcycle-python-server-sdk-3.3.4/example/cloud_client_example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/example/local_bucketing_client_example.py` & `devcycle-python-server-sdk-3.3.4/example/local_bucketing_client_example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/pyproject.toml` & `devcycle-python-server-sdk-3.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/setup.py` & `devcycle-python-server-sdk-3.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/test/api/test_bucketing_client.py` & `devcycle-python-server-sdk-3.3.4/test/api/test_bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/test/api/test_config_client.py` & `devcycle-python-server-sdk-3.3.4/test/api/test_config_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/test/api/test_event_client.py` & `devcycle-python-server-sdk-3.3.4/test/api/test_event_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/test/api/test_local_bucketing.py` & `devcycle-python-server-sdk-3.3.4/test/api/test_local_bucketing.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/test/fixture/data.py` & `devcycle-python-server-sdk-3.3.4/test/fixture/data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/test/managers/test_config_manager.py` & `devcycle-python-server-sdk-3.3.4/test/managers/test_config_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/test/managers/test_event_queue_manager.py` & `devcycle-python-server-sdk-3.3.4/test/managers/test_event_queue_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/test/models/test_bucketed_config.py` & `devcycle-python-server-sdk-3.3.4/test/models/test_bucketed_config.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/test/test_cloud_client.py` & `devcycle-python-server-sdk-3.3.4/test/test_cloud_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/test/test_local_client.py` & `devcycle-python-server-sdk-3.3.4/test/test_local_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.3/test/util/test_utils.py` & `devcycle-python-server-sdk-3.3.4/test/util/test_utils.py`

 * *Files identical despite different names*

